# Comparing `tmp/Rbeast-0.1.13.tar.gz` & `tmp/Rbeast-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Rbeast-0.1.13.tar", last modified: Wed Oct  5 03:10:32 2022, max compression
+gzip compressed data, was "Rbeast-0.1.14.tar", last modified: Tue Jul 18 19:26:55 2023, max compression
```

## Comparing `Rbeast-0.1.13.tar` & `Rbeast-0.1.14.tar`

### file list

```diff
@@ -1,133 +1,138 @@
-drwxrwxrwx   0        0        0        0 2022-10-05 03:10:32.070844 Rbeast-0.1.13/
--rw-rw-rw-   0        0        0     1083 2018-08-16 08:10:57.000000 Rbeast-0.1.13/LICENSE
--rw-rw-rw-   0        0        0       62 2022-09-28 19:12:21.000000 Rbeast-0.1.13/MANIFEST.in
--rw-rw-rw-   0        0        0    20436 2022-10-05 03:10:32.069844 Rbeast-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0    19163 2022-10-05 03:03:38.000000 Rbeast-0.1.13/README.md
-drwxrwxrwx   0        0        0        0 2022-10-05 03:10:31.661559 Rbeast-0.1.13/Rbeast.egg-info/
--rw-rw-rw-   0        0        0    20436 2022-10-05 03:10:31.000000 Rbeast-0.1.13/Rbeast.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2022-10-05 03:10:31.000000 Rbeast-0.1.13/Rbeast.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-05 03:10:31.000000 Rbeast-0.1.13/Rbeast.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-10-05 03:10:31.000000 Rbeast-0.1.13/Rbeast.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-10-05 03:10:31.000000 Rbeast-0.1.13/Rbeast.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-05 03:10:32.015875 Rbeast-0.1.13/ext_src/
--rw-rw-rw-   0        0        0    12040 2022-10-01 17:23:15.000000 Rbeast-0.1.13/ext_src/_beastv2_gui_plot.c
--rw-rw-rw-   0        0        0    35439 2021-11-15 17:35:02.000000 Rbeast-0.1.13/ext_src/_beastv2_gui_winmain.c
--rw-rw-rw-   0        0        0    19211 2022-09-19 02:31:42.000000 Rbeast-0.1.13/ext_src/abc_000_macro.h
--rw-rw-rw-   0        0        0      457 2021-11-13 15:48:56.000000 Rbeast-0.1.13/ext_src/abc_000_warning.h
--rw-rw-rw-   0        0        0     8830 2022-09-19 04:15:29.000000 Rbeast-0.1.13/ext_src/abc_001_config.h
--rw-rw-rw-   0        0        0      398 2021-08-31 19:23:27.000000 Rbeast-0.1.13/ext_src/abc_blas_lapack_lib.h
--rw-rw-rw-   0        0        0     2014 2021-08-10 05:30:13.000000 Rbeast-0.1.13/ext_src/abc_blas_lapack_mkl.h
--rw-rw-rw-   0        0        0    14539 2021-11-12 02:43:31.000000 Rbeast-0.1.13/ext_src/abc_blas_lapack_myl.h
--rw-rw-rw-   0        0        0    28626 2022-09-25 05:45:30.000000 Rbeast-0.1.13/ext_src/abc_common.c
--rw-rw-rw-   0        0        0     3404 2022-04-30 18:53:33.000000 Rbeast-0.1.13/ext_src/abc_common.h
--rw-rw-rw-   0        0        0    18962 2021-11-23 05:20:29.000000 Rbeast-0.1.13/ext_src/abc_cpu.c
--rw-rw-rw-   0        0        0     1569 2021-08-11 21:00:21.000000 Rbeast-0.1.13/ext_src/abc_cpu.h
--rw-rw-rw-   0        0        0     3467 2022-09-18 18:45:48.000000 Rbeast-0.1.13/ext_src/abc_datatype.h
--rw-rw-rw-   0        0        0    10384 2021-11-13 15:50:48.000000 Rbeast-0.1.13/ext_src/abc_date.c
--rw-rw-rw-   0        0        0     1072 2021-10-02 06:07:54.000000 Rbeast-0.1.13/ext_src/abc_date.h
--rw-rw-rw-   0        0        0     3825 2021-11-13 15:57:28.000000 Rbeast-0.1.13/ext_src/abc_dir.c
--rw-rw-rw-   0        0        0      315 2020-01-28 18:27:35.000000 Rbeast-0.1.13/ext_src/abc_dir.h
--rw-rw-rw-   0        0        0    27928 2021-11-12 15:27:05.000000 Rbeast-0.1.13/ext_src/abc_dirent.h
--rw-rw-rw-   0        0        0     8381 2022-09-23 03:59:45.000000 Rbeast-0.1.13/ext_src/abc_ide_util.h
--rw-rw-rw-   0        0        0    13100 2022-09-17 01:32:01.000000 Rbeast-0.1.13/ext_src/abc_ide_util_R.c
--rw-rw-rw-   0        0        0     7726 2022-09-25 05:39:16.000000 Rbeast-0.1.13/ext_src/abc_ide_util_common.c
--rw-rw-rw-   0        0        0    10694 2022-09-17 01:49:44.000000 Rbeast-0.1.13/ext_src/abc_ide_util_matlab.c
--rw-rw-rw-   0        0        0    23877 2022-10-01 22:40:26.000000 Rbeast-0.1.13/ext_src/abc_ide_util_python.c
--rw-rw-rw-   0        0        0     1182 2022-04-01 19:45:52.000000 Rbeast-0.1.13/ext_src/abc_ioFlush.c
--rw-rw-rw-   0        0        0      711 2022-03-31 19:17:27.000000 Rbeast-0.1.13/ext_src/abc_ioFlushcpp.cpp
--rw-rw-rw-   0        0        0    12127 2021-11-13 15:52:14.000000 Rbeast-0.1.13/ext_src/abc_lzw.c
--rw-rw-rw-   0        0        0    34845 2022-07-06 02:09:47.000000 Rbeast-0.1.13/ext_src/abc_mat.c
--rw-rw-rw-   0        0        0     3168 2022-06-04 03:02:31.000000 Rbeast-0.1.13/ext_src/abc_mat.h
--rw-rw-rw-   0        0        0     4448 2021-11-13 15:52:53.000000 Rbeast-0.1.13/ext_src/abc_math.c
--rw-rw-rw-   0        0        0      256 2021-04-29 04:37:33.000000 Rbeast-0.1.13/ext_src/abc_math.h
--rw-rw-rw-   0        0        0    39930 2022-08-09 18:42:38.000000 Rbeast-0.1.13/ext_src/abc_math_avx.c
--rw-rw-rw-   0        0        0     1517 2021-10-15 03:47:41.000000 Rbeast-0.1.13/ext_src/abc_math_avx.h
--rw-rw-rw-   0        0        0    22808 2022-01-18 20:36:00.000000 Rbeast-0.1.13/ext_src/abc_math_avx512.c
--rw-rw-rw-   0        0        0      531 2021-08-13 04:32:54.000000 Rbeast-0.1.13/ext_src/abc_math_avx512.h
--rw-rw-rw-   0        0        0     7526 2022-08-09 18:45:39.000000 Rbeast-0.1.13/ext_src/abc_mcmc.c
--rw-rw-rw-   0        0        0     2022 2022-08-09 18:46:23.000000 Rbeast-0.1.13/ext_src/abc_mcmc.h
--rw-rw-rw-   0        0        0     7677 2022-08-09 15:10:51.000000 Rbeast-0.1.13/ext_src/abc_mem.c
--rw-rw-rw-   0        0        0     1307 2022-06-06 04:59:42.000000 Rbeast-0.1.13/ext_src/abc_mem.h
--rw-rw-rw-   0        0        0     2603 2021-11-13 15:54:47.000000 Rbeast-0.1.13/ext_src/abc_mem_ext.c
--rw-rw-rw-   0        0        0     1239 2021-08-10 03:52:54.000000 Rbeast-0.1.13/ext_src/abc_mem_ext.h
--rw-rw-rw-   0        0        0    21857 2021-12-20 01:00:10.000000 Rbeast-0.1.13/ext_src/abc_pthread.c
--rw-rw-rw-   0        0        0    12541 2022-03-31 20:57:57.000000 Rbeast-0.1.13/ext_src/abc_pthread.h
--rw-rw-rw-   0        0        0      198 2021-05-04 01:40:11.000000 Rbeast-0.1.13/ext_src/abc_rand.h
--rw-rw-rw-   0        0        0      575 2018-08-12 02:27:12.000000 Rbeast-0.1.13/ext_src/abc_rand_mkl.h
--rw-rw-rw-   0        0        0    16303 2021-11-13 16:09:26.000000 Rbeast-0.1.13/ext_src/abc_rand_pcg_global.c
--rw-rw-rw-   0        0        0     1245 2021-09-06 15:11:50.000000 Rbeast-0.1.13/ext_src/abc_rand_pcg_global.h
--rw-rw-rw-   0        0        0     9901 2021-11-13 16:09:38.000000 Rbeast-0.1.13/ext_src/abc_rand_pcg_local.c
--rw-rw-rw-   0        0        0     3066 2021-09-06 15:12:41.000000 Rbeast-0.1.13/ext_src/abc_rand_pcg_local.h
--rw-rw-rw-   0        0        0    13456 2021-11-16 01:38:06.000000 Rbeast-0.1.13/ext_src/abc_rand_pcg_local_avx2.c
--rw-rw-rw-   0        0        0     8211 2021-11-16 03:03:37.000000 Rbeast-0.1.13/ext_src/abc_rand_pcg_local_avx512.c
--rw-rw-rw-   0        0        0     3210 2021-11-14 03:59:07.000000 Rbeast-0.1.13/ext_src/abc_rand_pcg_local_generic.c
--rw-rw-rw-   0        0        0     2662 2021-11-14 04:00:06.000000 Rbeast-0.1.13/ext_src/abc_sort.c
--rw-rw-rw-   0        0        0      168 2019-11-27 04:35:13.000000 Rbeast-0.1.13/ext_src/abc_sort.h
--rw-rw-rw-   0        0        0    10477 2021-11-14 03:07:44.000000 Rbeast-0.1.13/ext_src/abc_svd.c
--rw-rw-rw-   0        0        0     1366 2021-11-13 15:59:09.000000 Rbeast-0.1.13/ext_src/abc_system.c
--rw-rw-rw-   0        0        0       88 2021-04-11 04:26:17.000000 Rbeast-0.1.13/ext_src/abc_system.h
--rw-rw-rw-   0        0        0     3385 2021-11-16 02:56:49.000000 Rbeast-0.1.13/ext_src/abc_timer.c
--rw-rw-rw-   0        0        0     4201 2021-11-16 03:14:23.000000 Rbeast-0.1.13/ext_src/abc_timer.h
--rw-rw-rw-   0        0        0     8665 2022-04-20 05:10:10.000000 Rbeast-0.1.13/ext_src/abc_ts_func.c
--rw-rw-rw-   0        0        0      986 2022-04-20 05:10:10.000000 Rbeast-0.1.13/ext_src/abc_ts_func.h
--rw-rw-rw-   0        0        0    29879 2022-09-25 05:44:22.000000 Rbeast-0.1.13/ext_src/abc_vec.c
--rw-rw-rw-   0        0        0    13645 2022-09-25 05:44:49.000000 Rbeast-0.1.13/ext_src/abc_vec.h
--rw-rw-rw-   0        0        0   103711 2022-07-17 13:47:03.000000 Rbeast-0.1.13/ext_src/abc_vec_avx2.c
--rw-rw-rw-   0        0        0   107664 2022-07-12 19:45:30.000000 Rbeast-0.1.13/ext_src/abc_vec_avx512.c
--rw-rw-rw-   0        0        0    46997 2022-07-28 00:37:00.000000 Rbeast-0.1.13/ext_src/abc_vec_generic.c
--rw-rw-rw-   0        0        0    12347 2022-05-26 22:11:53.000000 Rbeast-0.1.13/ext_src/abc_win32_demo.c
--rw-rw-rw-   0        0        0     3464 2022-09-19 03:21:18.000000 Rbeast-0.1.13/ext_src/abc_win32_demo.h
--rw-rw-rw-   0        0        0    84250 2022-08-09 02:13:30.000000 Rbeast-0.1.13/ext_src/beastv2_COREV4.c
--rw-rw-rw-   0        0        0    90406 2022-08-09 04:17:33.000000 Rbeast-0.1.13/ext_src/beastv2_COREV4_gui.c
--rw-rw-rw-   0        0        0    86780 2022-08-09 02:36:21.000000 Rbeast-0.1.13/ext_src/beastv2_COREV4_mthrd.c
--rw-rw-rw-   0        0        0     5166 2022-08-09 01:45:39.000000 Rbeast-0.1.13/ext_src/beastv2_basis_allocinitmem.c
--rw-rw-rw-   0        0        0     3544 2022-04-23 04:38:27.000000 Rbeast-0.1.13/ext_src/beastv2_basis_computexy_q.c
--rw-rw-rw-   0        0        0     1936 2022-04-15 02:17:45.000000 Rbeast-0.1.13/ext_src/beastv2_basis_cvtKnotsToBinVec.c
--rw-rw-rw-   0        0        0     3075 2022-01-16 21:11:00.000000 Rbeast-0.1.13/ext_src/beastv2_basis_genrandbasis.c
--rw-rw-rw-   0        0        0    13803 2022-07-01 03:31:03.000000 Rbeast-0.1.13/ext_src/beastv2_basis_gensegment.c
--rw-rw-rw-   0        0        0     5230 2022-01-21 01:32:30.000000 Rbeast-0.1.13/ext_src/beastv2_basis_pickcmptId.c
--rw-rw-rw-   0        0        0    44558 2022-04-29 05:10:14.000000 Rbeast-0.1.13/ext_src/beastv2_basis_proposeNew_q.c
--rw-rw-rw-   0        0        0    10749 2022-07-01 04:55:26.000000 Rbeast-0.1.13/ext_src/beastv2_basis_updateKsKe_prec0123.c
--rw-rw-rw-   0        0        0     6651 2022-04-29 13:41:37.000000 Rbeast-0.1.13/ext_src/beastv2_basis_updategoodvec.c
--rw-rw-rw-   0        0        0     4852 2022-07-02 16:47:32.000000 Rbeast-0.1.13/ext_src/beastv2_func.h
--rw-rw-rw-   0        0        0    24692 2022-07-02 15:15:46.000000 Rbeast-0.1.13/ext_src/beastv2_func_q.c
--rw-rw-rw-   0        0        0    12660 2022-08-09 01:02:15.000000 Rbeast-0.1.13/ext_src/beastv2_header.h
--rw-rw-rw-   0        0        0    12434 2022-08-09 02:01:47.000000 Rbeast-0.1.13/ext_src/beastv2_header_solaris.h
--rw-rw-rw-   0        0        0     1423 2022-04-04 21:32:33.000000 Rbeast-0.1.13/ext_src/beastv2_io.h
--rw-rw-rw-   0        0        0    55962 2022-09-25 05:36:41.000000 Rbeast-0.1.13/ext_src/beastv2_io_in_args.c
--rw-rw-rw-   0        0        0     9313 2022-01-21 05:20:42.000000 Rbeast-0.1.13/ext_src/beastv2_io_in_readts.c
--rw-rw-rw-   0        0        0    48052 2022-08-09 05:07:34.000000 Rbeast-0.1.13/ext_src/beastv2_io_out_allocmem_q.c
--rw-rw-rw-   0        0        0    10311 2022-09-29 19:28:45.000000 Rbeast-0.1.13/ext_src/beastv2_io_out_printargs.c
--rw-rw-rw-   0        0        0    30793 2022-09-20 00:08:04.000000 Rbeast-0.1.13/ext_src/beastv2_io_out_tsextractprint.c
--rw-rw-rw-   0        0        0    12055 2022-08-09 05:25:32.000000 Rbeast-0.1.13/ext_src/beastv2_io_out_write_q.c
--rw-rw-rw-   0        0        0      226 2022-07-01 04:48:17.000000 Rbeast-0.1.13/ext_src/beastv2_model_allocinit.h
--rw-rw-rw-   0        0        0    28544 2022-08-09 20:41:43.000000 Rbeast-0.1.13/ext_src/beastv2_model_allocinit_q.c
--rw-rw-rw-   0        0        0     7371 2022-04-30 03:55:23.000000 Rbeast-0.1.13/ext_src/beastv2_prior_model.c
--rw-rw-rw-   0        0        0    21185 2022-07-02 17:18:16.000000 Rbeast-0.1.13/ext_src/beastv2_prior_precfunc.c
--rw-rw-rw-   0        0        0     1084 2022-07-01 03:52:41.000000 Rbeast-0.1.13/ext_src/beastv2_prior_precfunc.h
--rw-rw-rw-   0        0        0      439 2021-09-04 20:00:08.000000 Rbeast-0.1.13/ext_src/beastv2_xxyy_allocmem.h
--rw-rw-rw-   0        0        0     6228 2022-08-09 02:20:13.000000 Rbeast-0.1.13/ext_src/beastv2_xxyy_allocmem_q.c
--rw-rw-rw-   0        0        0      639 2022-04-14 23:32:18.000000 Rbeast-0.1.13/ext_src/globalvars.c
--rw-rw-rw-   0        0        0      510 2021-11-13 02:12:34.000000 Rbeast-0.1.13/ext_src/globalvars.h
--rw-rw-rw-   0        0        0    64078 2022-10-01 21:27:09.000000 Rbeast-0.1.13/ext_src/glue_code.c
-drwxrwxrwx   0        0        0        0 2022-10-05 03:10:31.622573 Rbeast-0.1.13/py_src/
-drwxrwxrwx   0        0        0        0 2022-10-05 03:10:32.046858 Rbeast-0.1.13/py_src/Rbeast/
--rw-rw-rw-   0        0        0     4797 2022-10-04 04:12:52.000000 Rbeast-0.1.13/py_src/Rbeast/__init__.py
--rw-rw-rw-   0        0        0     4344 2022-10-04 02:45:11.000000 Rbeast-0.1.13/py_src/Rbeast/beast.py
--rw-rw-rw-   0        0        0     1120 2022-10-04 18:17:05.000000 Rbeast-0.1.13/py_src/Rbeast/beast123.py
--rw-rw-rw-   0        0        0     4824 2022-10-04 15:11:17.000000 Rbeast-0.1.13/py_src/Rbeast/beast_irreg.py
--rw-rw-rw-   0        0        0     1053 2022-10-04 04:31:57.000000 Rbeast-0.1.13/py_src/Rbeast/cvt_to_numpy.py
-drwxrwxrwx   0        0        0        0 2022-10-05 03:10:32.065846 Rbeast-0.1.13/py_src/Rbeast/data/
--rw-rw-rw-   0        0        0     3175 2022-09-27 03:42:51.000000 Rbeast-0.1.13/py_src/Rbeast/data/beach.csv
--rw-rw-rw-   0        0        0   387328 2022-09-29 04:45:05.000000 Rbeast-0.1.13/py_src/Rbeast/data/ndvi.npy
--rw-rw-rw-   0        0        0    11616 2022-09-29 04:47:19.000000 Rbeast-0.1.13/py_src/Rbeast/data/ndvi_filename.txt
--rw-rw-rw-   0        0        0     4000 2022-09-29 04:45:25.000000 Rbeast-0.1.13/py_src/Rbeast/data/ndvi_fyear.npy
--rw-rw-rw-   0        0        0     1041 2022-09-25 04:06:00.000000 Rbeast-0.1.13/py_src/Rbeast/data/nile.csv
--rw-rw-rw-   0        0        0      904 2022-09-28 04:29:35.000000 Rbeast-0.1.13/py_src/Rbeast/extractbeast.py
--rw-rw-rw-   0        0        0     1605 2022-10-04 03:20:54.000000 Rbeast-0.1.13/py_src/Rbeast/load_example.py
--rw-rw-rw-   0        0        0    21879 2022-10-04 05:55:13.000000 Rbeast-0.1.13/py_src/Rbeast/plotbeast.py
--rw-rw-rw-   0        0        0     2689 2022-09-28 04:29:35.000000 Rbeast-0.1.13/py_src/Rbeast/printbeast.py
--rw-rw-rw-   0        0        0      203 2022-10-01 03:59:34.000000 Rbeast-0.1.13/pyproject.toml
--rw-rw-rw-   0        0        0       27 2022-09-28 04:33:14.000000 Rbeast-0.1.13/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-10-05 03:10:32.071843 Rbeast-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0     4835 2022-10-05 03:09:47.000000 Rbeast-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 19:26:53.600000 Rbeast-0.1.14/
+-rw-rw-rw-   0        0        0     1083 2018-08-16 08:10:58.000000 Rbeast-0.1.14/LICENSE
+-rw-rw-rw-   0        0        0       62 2022-09-28 19:12:22.000000 Rbeast-0.1.14/MANIFEST.in
+-rw-rw-rw-   0        0        0    20488 2023-07-18 19:26:56.000000 Rbeast-0.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0    19163 2022-10-05 03:03:40.000000 Rbeast-0.1.14/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 19:26:53.720000 Rbeast-0.1.14/Rbeast.egg-info/
+-rw-rw-rw-   0        0        0    20488 2023-07-18 19:26:54.000000 Rbeast-0.1.14/Rbeast.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3366 2023-07-18 19:26:54.000000 Rbeast-0.1.14/Rbeast.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 19:26:54.000000 Rbeast-0.1.14/Rbeast.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-18 19:26:54.000000 Rbeast-0.1.14/Rbeast.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 19:26:54.000000 Rbeast-0.1.14/Rbeast.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 19:26:53.850000 Rbeast-0.1.14/ext_src/
+-rw-rw-rw-   0        0        0    12052 2023-01-14 01:15:26.000000 Rbeast-0.1.14/ext_src/_beastv2_gui_plot.c
+-rw-rw-rw-   0        0        0    35463 2023-01-14 17:38:10.000000 Rbeast-0.1.14/ext_src/_beastv2_gui_winmain.c
+-rw-rw-rw-   0        0        0    19658 2023-07-18 19:24:42.000000 Rbeast-0.1.14/ext_src/abc_000_macro.h
+-rw-rw-rw-   0        0        0      458 2023-04-22 19:45:00.000000 Rbeast-0.1.14/ext_src/abc_000_warning.h
+-rw-rw-rw-   0        0        0     9433 2023-05-02 04:19:22.000000 Rbeast-0.1.14/ext_src/abc_001_config.h
+-rw-rw-rw-   0        0        0      474 2023-04-22 19:18:30.000000 Rbeast-0.1.14/ext_src/abc_blas_lapack_lib.h
+-rw-rw-rw-   0        0        0     2014 2021-08-10 05:30:14.000000 Rbeast-0.1.14/ext_src/abc_blas_lapack_mkl.h
+-rw-rw-rw-   0        0        0    14539 2021-11-12 02:43:32.000000 Rbeast-0.1.14/ext_src/abc_blas_lapack_myl.h
+-rw-rw-rw-   0        0        0    21190 2023-03-18 18:20:32.000000 Rbeast-0.1.14/ext_src/abc_blas_lapack_myl_old.h
+-rw-rw-rw-   0        0        0    40971 2023-06-16 00:30:02.000000 Rbeast-0.1.14/ext_src/abc_common.c
+-rw-rw-rw-   0        0        0     3283 2023-05-19 18:56:48.000000 Rbeast-0.1.14/ext_src/abc_common.h
+-rw-rw-rw-   0        0        0    19131 2023-05-18 04:56:14.000000 Rbeast-0.1.14/ext_src/abc_cpu.c
+-rw-rw-rw-   0        0        0     1630 2023-05-10 05:24:42.000000 Rbeast-0.1.14/ext_src/abc_cpu.h
+-rw-rw-rw-   0        0        0     4236 2023-06-15 23:30:08.000000 Rbeast-0.1.14/ext_src/abc_datatype.h
+-rw-rw-rw-   0        0        0    41279 2023-07-05 06:15:56.000000 Rbeast-0.1.14/ext_src/abc_date.c
+-rw-rw-rw-   0        0        0     1988 2023-06-20 16:14:02.000000 Rbeast-0.1.14/ext_src/abc_date.h
+-rw-rw-rw-   0        0        0     3836 2023-06-16 00:30:00.000000 Rbeast-0.1.14/ext_src/abc_dir.c
+-rw-rw-rw-   0        0        0      331 2022-11-07 18:40:20.000000 Rbeast-0.1.14/ext_src/abc_dir.h
+-rw-rw-rw-   0        0        0    28047 2023-05-10 07:50:52.000000 Rbeast-0.1.14/ext_src/abc_dirent.h
+-rw-rw-rw-   0        0        0    10989 2023-06-15 18:31:24.000000 Rbeast-0.1.14/ext_src/abc_ide_util.h
+-rw-rw-rw-   0        0        0    13896 2023-07-08 17:25:46.000000 Rbeast-0.1.14/ext_src/abc_ide_util_R.c
+-rw-rw-rw-   0        0        0    46156 2023-07-08 17:28:46.000000 Rbeast-0.1.14/ext_src/abc_ide_util_common.c
+-rw-rw-rw-   0        0        0    12949 2023-07-08 05:09:08.000000 Rbeast-0.1.14/ext_src/abc_ide_util_matlab.c
+-rw-rw-rw-   0        0        0    25318 2023-06-14 22:49:24.000000 Rbeast-0.1.14/ext_src/abc_ide_util_python.c
+-rw-rw-rw-   0        0        0     1278 2023-07-17 03:03:28.000000 Rbeast-0.1.14/ext_src/abc_ioFlush.c
+-rw-rw-rw-   0        0        0      767 2023-05-07 06:48:34.000000 Rbeast-0.1.14/ext_src/abc_ioFlushcpp.cpp
+-rw-rw-rw-   0        0        0    12130 2023-01-14 01:18:08.000000 Rbeast-0.1.14/ext_src/abc_lzw.c
+-rw-rw-rw-   0        0        0    46174 2023-06-17 18:30:52.000000 Rbeast-0.1.14/ext_src/abc_mat.c
+-rw-rw-rw-   0        0        0     4454 2023-06-16 05:40:08.000000 Rbeast-0.1.14/ext_src/abc_mat.h
+-rw-rw-rw-   0        0        0     8613 2023-02-27 15:14:48.000000 Rbeast-0.1.14/ext_src/abc_math.c
+-rw-rw-rw-   0        0        0      256 2021-04-29 04:37:34.000000 Rbeast-0.1.14/ext_src/abc_math.h
+-rw-rw-rw-   0        0        0    39930 2022-08-09 18:42:40.000000 Rbeast-0.1.14/ext_src/abc_math_avx.c
+-rw-rw-rw-   0        0        0     1544 2022-11-07 18:48:20.000000 Rbeast-0.1.14/ext_src/abc_math_avx.h
+-rw-rw-rw-   0        0        0    22808 2022-01-18 20:36:02.000000 Rbeast-0.1.14/ext_src/abc_math_avx512.c
+-rw-rw-rw-   0        0        0      531 2021-08-13 04:32:56.000000 Rbeast-0.1.14/ext_src/abc_math_avx512.h
+-rw-rw-rw-   0        0        0     7526 2022-08-09 18:45:40.000000 Rbeast-0.1.14/ext_src/abc_mcmc.c
+-rw-rw-rw-   0        0        0     2022 2022-08-09 18:46:24.000000 Rbeast-0.1.14/ext_src/abc_mcmc.h
+-rw-rw-rw-   0        0        0    17482 2023-07-08 17:04:50.000000 Rbeast-0.1.14/ext_src/abc_mem.c
+-rw-rw-rw-   0        0        0     3379 2023-07-08 16:24:02.000000 Rbeast-0.1.14/ext_src/abc_mem.h
+-rw-rw-rw-   0        0        0     2603 2021-11-13 15:54:48.000000 Rbeast-0.1.14/ext_src/abc_mem_ext.c
+-rw-rw-rw-   0        0        0     1239 2021-08-10 03:52:56.000000 Rbeast-0.1.14/ext_src/abc_mem_ext.h
+-rw-rw-rw-   0        0        0    30723 2023-07-17 16:34:48.000000 Rbeast-0.1.14/ext_src/abc_pthread.c
+-rw-rw-rw-   0        0        0    14210 2023-07-17 16:27:40.000000 Rbeast-0.1.14/ext_src/abc_pthread.h
+-rw-rw-rw-   0        0        0      198 2021-05-04 01:40:12.000000 Rbeast-0.1.14/ext_src/abc_rand.h
+-rw-rw-rw-   0        0        0      575 2018-08-12 02:27:14.000000 Rbeast-0.1.14/ext_src/abc_rand_mkl.h
+-rw-rw-rw-   0        0        0    18337 2023-05-12 23:19:16.000000 Rbeast-0.1.14/ext_src/abc_rand_pcg_global.c
+-rw-rw-rw-   0        0        0     1273 2023-03-03 22:34:46.000000 Rbeast-0.1.14/ext_src/abc_rand_pcg_global.h
+-rw-rw-rw-   0        0        0    16900 2023-06-06 17:40:04.000000 Rbeast-0.1.14/ext_src/abc_rand_pcg_local.c
+-rw-rw-rw-   0        0        0     3489 2023-06-06 19:20:50.000000 Rbeast-0.1.14/ext_src/abc_rand_pcg_local.h
+-rw-rw-rw-   0        0        0    16852 2023-07-05 05:20:48.000000 Rbeast-0.1.14/ext_src/abc_rand_pcg_local_avx2.c
+-rw-rw-rw-   0        0        0     8968 2023-06-06 18:11:08.000000 Rbeast-0.1.14/ext_src/abc_rand_pcg_local_avx512.c
+-rw-rw-rw-   0        0        0     3583 2023-06-06 18:12:10.000000 Rbeast-0.1.14/ext_src/abc_rand_pcg_local_generic.c
+-rw-rw-rw-   0        0        0     5582 2023-06-15 05:18:24.000000 Rbeast-0.1.14/ext_src/abc_sort.c
+-rw-rw-rw-   0        0        0      534 2023-06-15 04:02:22.000000 Rbeast-0.1.14/ext_src/abc_sort.h
+-rw-rw-rw-   0        0        0    10477 2021-11-14 03:07:46.000000 Rbeast-0.1.14/ext_src/abc_svd.c
+-rw-rw-rw-   0        0        0     1366 2021-11-13 15:59:10.000000 Rbeast-0.1.14/ext_src/abc_system.c
+-rw-rw-rw-   0        0        0       92 2022-11-24 03:48:18.000000 Rbeast-0.1.14/ext_src/abc_system.h
+-rw-rw-rw-   0        0        0     3405 2022-11-24 03:48:18.000000 Rbeast-0.1.14/ext_src/abc_timer.c
+-rw-rw-rw-   0        0        0     4494 2023-04-22 20:25:02.000000 Rbeast-0.1.14/ext_src/abc_timer.h
+-rw-rw-rw-   0        0        0    21155 2023-05-10 07:17:54.000000 Rbeast-0.1.14/ext_src/abc_tranpose.c
+-rw-rw-rw-   0        0        0      567 2023-04-22 20:27:02.000000 Rbeast-0.1.14/ext_src/abc_tranpose.h
+-rw-rw-rw-   0        0        0    11435 2023-06-16 00:16:08.000000 Rbeast-0.1.14/ext_src/abc_ts_func.c
+-rw-rw-rw-   0        0        0     1833 2023-06-15 04:41:16.000000 Rbeast-0.1.14/ext_src/abc_ts_func.h
+-rw-rw-rw-   0        0        0    46128 2023-06-16 00:30:02.000000 Rbeast-0.1.14/ext_src/abc_vec.c
+-rw-rw-rw-   0        0        0    16167 2023-06-08 05:56:44.000000 Rbeast-0.1.14/ext_src/abc_vec.h
+-rw-rw-rw-   0        0        0   104258 2023-06-08 05:41:46.000000 Rbeast-0.1.14/ext_src/abc_vec_avx2.c
+-rw-rw-rw-   0        0        0   108119 2023-06-08 00:55:58.000000 Rbeast-0.1.14/ext_src/abc_vec_avx512.c
+-rw-rw-rw-   0        0        0    47454 2023-06-15 23:52:04.000000 Rbeast-0.1.14/ext_src/abc_vec_generic.c
+-rw-rw-rw-   0        0        0    12347 2022-05-26 22:11:54.000000 Rbeast-0.1.14/ext_src/abc_win32_demo.c
+-rw-rw-rw-   0        0        0     3464 2022-09-19 03:21:20.000000 Rbeast-0.1.14/ext_src/abc_win32_demo.h
+-rw-rw-rw-   0        0        0    84559 2023-07-11 00:33:28.000000 Rbeast-0.1.14/ext_src/beastv2_COREV4.c
+-rw-rw-rw-   0        0        0    90151 2023-06-15 22:32:20.000000 Rbeast-0.1.14/ext_src/beastv2_COREV4_gui.c
+-rw-rw-rw-   0        0        0    87088 2023-06-15 22:20:00.000000 Rbeast-0.1.14/ext_src/beastv2_COREV4_mthrd.c
+-rw-rw-rw-   0        0        0     5166 2022-08-09 01:45:40.000000 Rbeast-0.1.14/ext_src/beastv2_basis_allocinitmem.c
+-rw-rw-rw-   0        0        0     3544 2022-04-23 04:38:28.000000 Rbeast-0.1.14/ext_src/beastv2_basis_computexy_q.c
+-rw-rw-rw-   0        0        0     1936 2022-04-15 02:17:46.000000 Rbeast-0.1.14/ext_src/beastv2_basis_cvtKnotsToBinVec.c
+-rw-rw-rw-   0        0        0     3075 2022-01-16 21:11:02.000000 Rbeast-0.1.14/ext_src/beastv2_basis_genrandbasis.c
+-rw-rw-rw-   0        0        0    13876 2023-06-09 04:54:12.000000 Rbeast-0.1.14/ext_src/beastv2_basis_gensegment.c
+-rw-rw-rw-   0        0        0     5230 2022-01-21 01:32:32.000000 Rbeast-0.1.14/ext_src/beastv2_basis_pickcmptId.c
+-rw-rw-rw-   0        0        0    44558 2022-04-29 05:10:16.000000 Rbeast-0.1.14/ext_src/beastv2_basis_proposeNew_q.c
+-rw-rw-rw-   0        0        0    10749 2022-07-01 04:55:28.000000 Rbeast-0.1.14/ext_src/beastv2_basis_updateKsKe_prec0123.c
+-rw-rw-rw-   0        0        0     6651 2023-05-09 16:18:04.000000 Rbeast-0.1.14/ext_src/beastv2_basis_updategoodvec.c
+-rw-rw-rw-   0        0        0     4769 2023-02-11 05:12:12.000000 Rbeast-0.1.14/ext_src/beastv2_func.h
+-rw-rw-rw-   0        0        0    23709 2023-02-11 05:01:12.000000 Rbeast-0.1.14/ext_src/beastv2_func_q.c
+-rw-rw-rw-   0        0        0    12587 2023-07-10 18:00:34.000000 Rbeast-0.1.14/ext_src/beastv2_header.h
+-rw-rw-rw-   0        0        0    12216 2023-06-14 17:13:14.000000 Rbeast-0.1.14/ext_src/beastv2_header_solaris.h
+-rw-rw-rw-   0        0        0     1418 2022-11-01 01:40:36.000000 Rbeast-0.1.14/ext_src/beastv2_io.h
+-rw-rw-rw-   0        0        0    57853 2023-07-10 17:21:00.000000 Rbeast-0.1.14/ext_src/beastv2_io_in_args.c
+-rw-rw-rw-   0        0        0     7866 2023-07-04 05:25:48.000000 Rbeast-0.1.14/ext_src/beastv2_io_in_readts.c
+-rw-rw-rw-   0        0        0    46576 2023-06-20 16:16:00.000000 Rbeast-0.1.14/ext_src/beastv2_io_out_allocmem_q.c
+-rw-rw-rw-   0        0        0    20131 2023-07-10 17:25:58.000000 Rbeast-0.1.14/ext_src/beastv2_io_out_printargs.c
+-rw-rw-rw-   0        0        0    30798 2023-06-16 00:11:42.000000 Rbeast-0.1.14/ext_src/beastv2_io_out_tsextractprint.c
+-rw-rw-rw-   0        0        0    10048 2022-11-05 02:15:42.000000 Rbeast-0.1.14/ext_src/beastv2_io_out_write_q.c
+-rw-rw-rw-   0        0        0      226 2022-07-01 04:48:18.000000 Rbeast-0.1.14/ext_src/beastv2_model_allocinit.h
+-rw-rw-rw-   0        0        0    28599 2023-06-15 21:55:14.000000 Rbeast-0.1.14/ext_src/beastv2_model_allocinit_q.c
+-rw-rw-rw-   0        0        0     7371 2022-04-30 03:55:24.000000 Rbeast-0.1.14/ext_src/beastv2_prior_model.c
+-rw-rw-rw-   0        0        0    21185 2022-07-02 17:18:18.000000 Rbeast-0.1.14/ext_src/beastv2_prior_precfunc.c
+-rw-rw-rw-   0        0        0     1084 2022-07-01 03:52:42.000000 Rbeast-0.1.14/ext_src/beastv2_prior_precfunc.h
+-rw-rw-rw-   0        0        0     9155 2023-07-08 16:54:10.000000 Rbeast-0.1.14/ext_src/beastv2_svdbasis.c
+-rw-rw-rw-   0        0        0      439 2021-09-04 20:00:10.000000 Rbeast-0.1.14/ext_src/beastv2_xxyy_allocmem.h
+-rw-rw-rw-   0        0        0     7155 2023-06-11 18:15:10.000000 Rbeast-0.1.14/ext_src/beastv2_xxyy_allocmem_q.c
+-rw-rw-rw-   0        0        0      660 2023-01-10 03:57:42.000000 Rbeast-0.1.14/ext_src/globalvars.c
+-rw-rw-rw-   0        0        0      672 2023-01-14 17:52:56.000000 Rbeast-0.1.14/ext_src/globalvars.h
+-rw-rw-rw-   0        0        0    29909 2023-07-17 16:52:20.000000 Rbeast-0.1.14/ext_src/glue_code.c
+-rw-rw-rw-   0        0        0     6058 2021-11-23 23:14:48.000000 Rbeast-0.1.14/ext_src/tetris.c
+drwxrwxrwx   0        0        0        0 2023-07-18 19:26:53.970000 Rbeast-0.1.14/py_src/
+drwxrwxrwx   0        0        0        0 2023-07-18 19:26:54.100000 Rbeast-0.1.14/py_src/Rbeast/
+-rw-rw-rw-   0        0        0     4797 2022-10-04 04:12:54.000000 Rbeast-0.1.14/py_src/Rbeast/__init__.py
+-rw-rw-rw-   0        0        0     4344 2022-10-04 02:45:12.000000 Rbeast-0.1.14/py_src/Rbeast/beast.py
+-rw-rw-rw-   0        0        0     1120 2022-10-04 18:17:06.000000 Rbeast-0.1.14/py_src/Rbeast/beast123.py
+-rw-rw-rw-   0        0        0     4824 2022-10-04 15:11:18.000000 Rbeast-0.1.14/py_src/Rbeast/beast_irreg.py
+-rw-rw-rw-   0        0        0     1053 2022-10-04 04:31:58.000000 Rbeast-0.1.14/py_src/Rbeast/cvt_to_numpy.py
+drwxrwxrwx   0        0        0        0 2023-07-18 19:26:54.220000 Rbeast-0.1.14/py_src/Rbeast/data/
+-rw-rw-rw-   0        0        0     3175 2022-09-27 03:42:52.000000 Rbeast-0.1.14/py_src/Rbeast/data/beach.csv
+-rw-rw-rw-   0        0        0   387328 2022-09-29 04:45:06.000000 Rbeast-0.1.14/py_src/Rbeast/data/ndvi.npy
+-rw-rw-rw-   0        0        0    11616 2022-09-29 04:47:20.000000 Rbeast-0.1.14/py_src/Rbeast/data/ndvi_filename.txt
+-rw-rw-rw-   0        0        0     4000 2022-09-29 04:45:26.000000 Rbeast-0.1.14/py_src/Rbeast/data/ndvi_fyear.npy
+-rw-rw-rw-   0        0        0     1041 2022-09-25 04:06:02.000000 Rbeast-0.1.14/py_src/Rbeast/data/nile.csv
+-rw-rw-rw-   0        0        0      904 2022-09-28 04:29:36.000000 Rbeast-0.1.14/py_src/Rbeast/extractbeast.py
+-rw-rw-rw-   0        0        0     1605 2022-10-04 03:20:56.000000 Rbeast-0.1.14/py_src/Rbeast/load_example.py
+-rw-rw-rw-   0        0        0    21879 2022-10-04 05:55:14.000000 Rbeast-0.1.14/py_src/Rbeast/plotbeast.py
+-rw-rw-rw-   0        0        0     2689 2022-09-28 04:29:36.000000 Rbeast-0.1.14/py_src/Rbeast/printbeast.py
+-rw-rw-rw-   0        0        0      731 2023-07-17 19:23:34.000000 Rbeast-0.1.14/pyproject.toml
+-rw-rw-rw-   0        0        0       27 2022-09-28 04:33:16.000000 Rbeast-0.1.14/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 19:26:56.000000 Rbeast-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0     4962 2023-07-18 19:25:08.000000 Rbeast-0.1.14/setup.py
```

### Comparing `Rbeast-0.1.13/LICENSE` & `Rbeast-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/PKG-INFO` & `Rbeast-0.1.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Rbeast
-Version: 0.1.13
+Version: 0.1.14
 Summary: Bayesian changepoint detection and time series decomposition
 Home-page: https://github.com/zhaokg/Rbeast
 Author: Kaiguang Zhao
 Author-email: zhao.1423@osu.edu
 Keywords: changepoint,structural breaks,time series decompositiontime series analysis,trend analysis
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: Rbeast Version: 0.1.13 Summary: Bayesian
+Metadata-Version: 2.1 Name: Rbeast Version: 0.1.14 Summary: Bayesian
 changepoint detection and time series decomposition Home-page: https://
 github.com/zhaokg/Rbeast Author: Kaiguang Zhao Author-email: zhao.1423@osu.edu
 Keywords: changepoint,structural breaks,time series decompositiontime series
 analysis,trend analysis Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering :: Hydrology Classifier: Topic :: Scientific/
-Engineering :: Atmospheric Science Classifier: Topic :: Scientific/Engineering
-:: Artificial Intelligence Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License Requires-Python: >=3.5
-Description-Content-Type: text/markdown License-File: LICENSE # Rbeast: A
-Python package for Bayesian changepoint detection and time series decomposition
-#### BEAST (Bayesian Estimator of Abrupt change, Seasonality, and Trend) is a
-fast, generic Bayesian model averaging algorithm to decompose time series or 1D
-sequential data into individual components, such as abrupt changes, trends, and
-periodic/seasonal variations, as described in [Zhao et al. (2019)](https://
-go.osu.edu/beast2019). BEAST is useful for *changepoint detection (e.g.,
-breakpoints, structural breaks, regime shifts, or anomalies), trend analysis,
-time series decomposition (e.g., trend vs seasonality), time series
-segmentation, and interrupted time series analysis*. See a list of selected
-studies_using_BEAST. **Quick Installation** > BEAST was impemented in C/C++ but
-accessible from R, Python, and Matlab. Run the following to install: * Python:
-**`pip install Rbeast`** * Matlab: **`eval(webread('http://b.link/
-rbeast',weboptions('cert','')))`** * R lang: **`install.packages("Rbeast")`**
-**Quick Usage** > One-liner code for Python, Matlab and R. Check below or
-[github.com/zhaokg/Rbeast](https://github.com/zhaokg/Rbeast) for more details.
-``` # Python example import Rbeast as rb; (Nile, Year)=rb.load_example('nile');
-o=rb.beast(Nile,season='none'); rb.plot(o) # Matlab example load('Nile'); o =
-beast(Nile, 'season','none'); plotbeast(o) # R example library(Rbeast); data
-(Nile); o = beast(Nile); plot(o) ``` ## Installation for Python
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Hydrology Classifier: Topic :: Scientific/Engineering ::
+Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Scientific/Engineering Classifier: License ::
+OSI Approved :: MIT License Requires-Python: >=3.5 Description-Content-Type:
+text/markdown License-File: LICENSE # Rbeast: A Python package for Bayesian
+changepoint detection and time series decomposition #### BEAST (Bayesian
+Estimator of Abrupt change, Seasonality, and Trend) is a fast, generic Bayesian
+model averaging algorithm to decompose time series or 1D sequential data into
+individual components, such as abrupt changes, trends, and periodic/seasonal
+variations, as described in [Zhao et al. (2019)](https://go.osu.edu/beast2019).
+BEAST is useful for *changepoint detection (e.g., breakpoints, structural
+breaks, regime shifts, or anomalies), trend analysis, time series decomposition
+(e.g., trend vs seasonality), time series segmentation, and interrupted time
+series analysis*. See a list of selected_studies_using_BEAST. **Quick
+Installation** > BEAST was impemented in C/C++ but accessible from R, Python,
+and Matlab. Run the following to install: * Python: **`pip install Rbeast`** *
+Matlab: **`eval(webread('http://b.link/rbeast',weboptions('cert','')))`** * R
+lang: **`install.packages("Rbeast")`** **Quick Usage** > One-liner code for
+Python, Matlab and R. Check below or [github.com/zhaokg/Rbeast](https://
+github.com/zhaokg/Rbeast) for more details. ``` # Python example import Rbeast
+as rb; (Nile, Year)=rb.load_example('nile'); o=rb.beast(Nile,season='none');
+rb.plot(o) # Matlab example load('Nile'); o = beast(Nile, 'season','none');
+plotbeast(o) # R example library(Rbeast); data(Nile); o = beast(Nile); plot(o)
+``` ## Installation for Python
 [https://img.shields.io/static/v1?style=plastic&logo=github&label=see
 also&message=github.com/zhaokg/Rbeast&color=brightgreen]
 A package **`Rbeast`** has been deposited here at PyPI: https://pypi.org/
 project/Rbeast/. Run the command below in a console to install: ```python pip
 install Rbeast ``` Currently, a binary wheel file was built only for Windows
 and Python 3.8. For other OS platforms or Python versions, the installation
 requires a compiler to build the package from the C/C++ code, which is a
```

### Comparing `Rbeast-0.1.13/README.md` & `Rbeast-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/Rbeast.egg-info/PKG-INFO` & `Rbeast-0.1.14/Rbeast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: Rbeast
-Version: 0.1.13
+Version: 0.1.14
 Summary: Bayesian changepoint detection and time series decomposition
 Home-page: https://github.com/zhaokg/Rbeast
 Author: Kaiguang Zhao
 Author-email: zhao.1423@osu.edu
 Keywords: changepoint,structural breaks,time series decompositiontime series analysis,trend analysis
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: Rbeast Version: 0.1.13 Summary: Bayesian
+Metadata-Version: 2.1 Name: Rbeast Version: 0.1.14 Summary: Bayesian
 changepoint detection and time series decomposition Home-page: https://
 github.com/zhaokg/Rbeast Author: Kaiguang Zhao Author-email: zhao.1423@osu.edu
 Keywords: changepoint,structural breaks,time series decompositiontime series
 analysis,trend analysis Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering :: Hydrology Classifier: Topic :: Scientific/
-Engineering :: Atmospheric Science Classifier: Topic :: Scientific/Engineering
-:: Artificial Intelligence Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License Requires-Python: >=3.5
-Description-Content-Type: text/markdown License-File: LICENSE # Rbeast: A
-Python package for Bayesian changepoint detection and time series decomposition
-#### BEAST (Bayesian Estimator of Abrupt change, Seasonality, and Trend) is a
-fast, generic Bayesian model averaging algorithm to decompose time series or 1D
-sequential data into individual components, such as abrupt changes, trends, and
-periodic/seasonal variations, as described in [Zhao et al. (2019)](https://
-go.osu.edu/beast2019). BEAST is useful for *changepoint detection (e.g.,
-breakpoints, structural breaks, regime shifts, or anomalies), trend analysis,
-time series decomposition (e.g., trend vs seasonality), time series
-segmentation, and interrupted time series analysis*. See a list of selected
-studies_using_BEAST. **Quick Installation** > BEAST was impemented in C/C++ but
-accessible from R, Python, and Matlab. Run the following to install: * Python:
-**`pip install Rbeast`** * Matlab: **`eval(webread('http://b.link/
-rbeast',weboptions('cert','')))`** * R lang: **`install.packages("Rbeast")`**
-**Quick Usage** > One-liner code for Python, Matlab and R. Check below or
-[github.com/zhaokg/Rbeast](https://github.com/zhaokg/Rbeast) for more details.
-``` # Python example import Rbeast as rb; (Nile, Year)=rb.load_example('nile');
-o=rb.beast(Nile,season='none'); rb.plot(o) # Matlab example load('Nile'); o =
-beast(Nile, 'season','none'); plotbeast(o) # R example library(Rbeast); data
-(Nile); o = beast(Nile); plot(o) ``` ## Installation for Python
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Hydrology Classifier: Topic :: Scientific/Engineering ::
+Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Scientific/Engineering Classifier: License ::
+OSI Approved :: MIT License Requires-Python: >=3.5 Description-Content-Type:
+text/markdown License-File: LICENSE # Rbeast: A Python package for Bayesian
+changepoint detection and time series decomposition #### BEAST (Bayesian
+Estimator of Abrupt change, Seasonality, and Trend) is a fast, generic Bayesian
+model averaging algorithm to decompose time series or 1D sequential data into
+individual components, such as abrupt changes, trends, and periodic/seasonal
+variations, as described in [Zhao et al. (2019)](https://go.osu.edu/beast2019).
+BEAST is useful for *changepoint detection (e.g., breakpoints, structural
+breaks, regime shifts, or anomalies), trend analysis, time series decomposition
+(e.g., trend vs seasonality), time series segmentation, and interrupted time
+series analysis*. See a list of selected_studies_using_BEAST. **Quick
+Installation** > BEAST was impemented in C/C++ but accessible from R, Python,
+and Matlab. Run the following to install: * Python: **`pip install Rbeast`** *
+Matlab: **`eval(webread('http://b.link/rbeast',weboptions('cert','')))`** * R
+lang: **`install.packages("Rbeast")`** **Quick Usage** > One-liner code for
+Python, Matlab and R. Check below or [github.com/zhaokg/Rbeast](https://
+github.com/zhaokg/Rbeast) for more details. ``` # Python example import Rbeast
+as rb; (Nile, Year)=rb.load_example('nile'); o=rb.beast(Nile,season='none');
+rb.plot(o) # Matlab example load('Nile'); o = beast(Nile, 'season','none');
+plotbeast(o) # R example library(Rbeast); data(Nile); o = beast(Nile); plot(o)
+``` ## Installation for Python
 [https://img.shields.io/static/v1?style=plastic&logo=github&label=see
 also&message=github.com/zhaokg/Rbeast&color=brightgreen]
 A package **`Rbeast`** has been deposited here at PyPI: https://pypi.org/
 project/Rbeast/. Run the command below in a console to install: ```python pip
 install Rbeast ``` Currently, a binary wheel file was built only for Windows
 and Python 3.8. For other OS platforms or Python versions, the installation
 requires a compiler to build the package from the C/C++ code, which is a
```

### Comparing `Rbeast-0.1.13/Rbeast.egg-info/SOURCES.txt` & `Rbeast-0.1.14/Rbeast.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ext_src/_beastv2_gui_winmain.c
 ext_src/abc_000_macro.h
 ext_src/abc_000_warning.h
 ext_src/abc_001_config.h
 ext_src/abc_blas_lapack_lib.h
 ext_src/abc_blas_lapack_mkl.h
 ext_src/abc_blas_lapack_myl.h
+ext_src/abc_blas_lapack_myl_old.h
 ext_src/abc_common.c
 ext_src/abc_common.h
 ext_src/abc_cpu.c
 ext_src/abc_cpu.h
 ext_src/abc_datatype.h
 ext_src/abc_date.c
 ext_src/abc_date.h
@@ -63,14 +64,16 @@
 ext_src/abc_sort.c
 ext_src/abc_sort.h
 ext_src/abc_svd.c
 ext_src/abc_system.c
 ext_src/abc_system.h
 ext_src/abc_timer.c
 ext_src/abc_timer.h
+ext_src/abc_tranpose.c
+ext_src/abc_tranpose.h
 ext_src/abc_ts_func.c
 ext_src/abc_ts_func.h
 ext_src/abc_vec.c
 ext_src/abc_vec.h
 ext_src/abc_vec_avx2.c
 ext_src/abc_vec_avx512.c
 ext_src/abc_vec_generic.c
@@ -100,19 +103,21 @@
 ext_src/beastv2_io_out_tsextractprint.c
 ext_src/beastv2_io_out_write_q.c
 ext_src/beastv2_model_allocinit.h
 ext_src/beastv2_model_allocinit_q.c
 ext_src/beastv2_prior_model.c
 ext_src/beastv2_prior_precfunc.c
 ext_src/beastv2_prior_precfunc.h
+ext_src/beastv2_svdbasis.c
 ext_src/beastv2_xxyy_allocmem.h
 ext_src/beastv2_xxyy_allocmem_q.c
 ext_src/globalvars.c
 ext_src/globalvars.h
 ext_src/glue_code.c
+ext_src/tetris.c
 py_src/Rbeast/__init__.py
 py_src/Rbeast/beast.py
 py_src/Rbeast/beast123.py
 py_src/Rbeast/beast_irreg.py
 py_src/Rbeast/cvt_to_numpy.py
 py_src/Rbeast/extractbeast.py
 py_src/Rbeast/load_example.py
```

### Comparing `Rbeast-0.1.13/ext_src/_beastv2_gui_plot.c` & `Rbeast-0.1.14/ext_src/_beastv2_gui_plot.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #include "abc_000_macro.h"
 #include "abc_000_warning.h"
 
 #if defined(WIN64_OS) 
 
 #include "abc_win32_demo.h"
-void BEAST2_InitGlobalData() {
+void BEAST2_InitGlobalData(void) {
 	style = (Style) {
 			.hMargin		= 3.f,
 			.rEdit			= 0.1f,
 			.hgtButtonBar	= 30.f,
 			.wButton        = 72.f,
 			.sep            = 10.f,
 			.vButtonRatio   = 0.7f,
@@ -34,15 +34,15 @@
 	InitializeConditionVariable(&gData.cv);
 
 	gData.timerInterval = 25;
 	gData.sleepInterval = 50;
 	gData.status	= RUN;
 	gData.optStatus = NotAssigned;
 }
-void BEAST2_AllocatePlotData()
+void BEAST2_AllocatePlotData(void)
 {
 	gData.plotData[0][0] = malloc(sizeof(int)*gData.N * 2); //Yfit_mean
 	gData.plotData[0][1] = malloc(sizeof(int)*gData.N * 2); //Yfit_cur
 	
 
 	gData.plotData[1][0] = malloc(sizeof(int)*gData.N * 2); //S_mean
 	gData.plotData[1][1] = malloc(sizeof(int)*gData.N * 2); //S_cur
@@ -58,15 +58,15 @@
 	gData.plotData[3][2] = malloc(sizeof(int)*gData.N);     //T_bp
 	gData.plotData[3][3] = malloc(sizeof(int)*gData.N);     //T_bp
 	gData.plotData[3][4] = malloc(sizeof(int)*gData.N * 4); //T_CI
 
 	gData.plotData[4][0] = malloc(sizeof(int)*gData.N * 2); //T_Pprob
  
 }
-void BEAST2_GeneratePlotData()
+void BEAST2_GeneratePlotData(void)
 {
 	int N      = gData.N;
 	int sample = gData.sample;
 
 
 	F32 W, H, Ymax, Ymin, dX;
 	F32 x;
```

### Comparing `Rbeast-0.1.13/ext_src/_beastv2_gui_winmain.c` & `Rbeast-0.1.14/ext_src/_beastv2_gui_winmain.c`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 }
 PostMessage(gData.hwnd, WM_USER + 1, 0, 0);
 return 0;
 }
 */
 static LRESULT CALLBACK DialogProc(HWND hwnd, UINT msg, WPARAM wParam, LPARAM lParam);
 static LRESULT CALLBACK WndProc(HWND hwnd, UINT msg, WPARAM wParam, LPARAM lParam);
-static HICON CreateMyIcon( ) {
+static HICON CreateMyIcon(void) {
 	// Yang icon AND bitmask 
 	static BYTE ANDmaskIcon[] = { 0xFF, 0xFF, 0xFF, 0xFF,   // line 1 
 			0xFF, 0xFF, 0xC3, 0xFF,   // line 2 
 			0xFF, 0xFF, 0x00, 0xFF,   // line 3 
 			0xFF, 0xFE, 0x00, 0x7F,   // line 4 
 
 			0xFF, 0xFC, 0x00, 0x1F,   // line 5 
@@ -188,17 +188,17 @@
 	}
 }
 
  
 /***********************************/ 
 // Defined in beastv2_gui_plot.c
 /***********************************/
-extern void BEAST2_InitGlobalData();
-extern void BEAST2_AllocatePlotData();
-extern void BEAST2_GeneratePlotData();
+extern void BEAST2_InitGlobalData(void);
+extern void BEAST2_AllocatePlotData(void);
+extern void BEAST2_GeneratePlotData(void);
 extern void BEAST2_DrawPlots(HDC hdc);
 
 
 DWORD WINAPI beast_thread(__in LPVOID dummy_GLOBAL_OPTIONS) {
 	#if R_INTERFACE==1
 	//mexPrintf is not thread-safe.
 	BEAST2_print_options(GLOBAL_OPTIONS);
@@ -639,17 +639,17 @@
 	case WM_USER + 2:
 
 		EnterCriticalSection(&gData.cs);
 		{
 			char str[100];
 			wsprintf(str, "Chain #%d is finished\r\n", gData.curChainNumber);
 			LoggerInsert(str);
-			sprintf(str, "Mean number of scp is %8.2f\r\n", gData.sN);
+			snprintf(str, 99, "Mean number of scp is %8.2f\r\n", gData.sN);
 			LoggerInsert(str);
-			sprintf(str, "Mean number of tcp is %8.2f\r\n", gData.tN);
+			snprintf(str,99, "Mean number of tcp is %8.2f\r\n", gData.tN);
 			LoggerInsert(str);
 		}
 		LeaveCriticalSection(&gData.cs);
 
 		break;
 	case WM_SIZE:
 	{
```

### Comparing `Rbeast-0.1.13/ext_src/abc_000_macro.h` & `Rbeast-0.1.14/ext_src/abc_000_macro.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 #pragma once
 
+//#define  PLAY_MODE
+//#define  M_RELEASE
+//#define  P_RELEASE
+//#define  R_RELEASE
+
 // https://social.msdn.microsoft.com/Forums/vstudio/en-US/355ed7af-4037-4587-8614-34d51d865f03/missing-prototype-warning?forum=vclanguage
 // In MSVC, set the warning level to Level 3 to get warnings of unfctions without prototypes
 //ERROR: function returning a value
 //ERROR: undefined; assuming extern returning int
 
 //gcc.gnu.org/onlinedocs/cpp/Variadic-Macros.html
  
-#define R_INTERFACE    0
-#define M_INTERFACE    0
-#define P_INTERFACE    1
+// file externsion: .mexw64 for Matlab, .pyd for Pyhton
+
+#define R_INTERFACE   1
+#define M_INTERFACE   0
+#define P_INTERFACE   0
 /*------------------------------------------------------------*/
 #define MYMAT_LIBRARY   1
 #define MKL_LIBRARY     0
 #define MATLAB_LIBRARY  0 // For some uknown reason, the Matlab version of Blas and Lapack function doesn't work.
 
 /*------------------------------------------------------------*/
 #define PCGRAND_LIBRARY 1
 #define MKLRAND_LIBRARY 0
-
-
-//#define M_RELEASE
+ 
+ 
+ //#define  M_RELEASE
 
 #ifdef R_RELEASE
         // For R interface
 		#undef   R_INTERFACE
 		#undef   M_INTERFACE
 		#undef   P_INTERFACE
 		#define  R_INTERFACE 1
@@ -164,34 +171,42 @@
 		#define TARGET_64
 	#else
 		#define TARGET_32
 	#endif
 #endif
 
 #if defined(__aarch64__)
-	 //https://stackoverflow.com/questions/60588765/how-to-get-cpu-brand-information-in-arm64
+	//https://stackoverflow.com/questions/60588765/how-to-get-cpu-brand-information-in-arm64
     //https://stackoverflow.com/questions/23934862/what-predefined-macro-can-i-use-to-detect-the-target-architecture-in-clang
 
     #define  ARM64_OS
 #endif
 
 
+//https://stackoverflow.com/questions/152016/detecting-cpu-architecture-compile-time
+#if defined(__powerpc) || defined(__powerpc__) || defined(__powerpc64__)  || defined(__POWERPC__) || defined(__ppc__) || defined(__PPC__) || defined(_ARCH_PPC) \
+     || defined(__PPC64__) || defined(__ppc64__) || defined(_ARCH_PPC64)
+	#define POWERPC_OS
+#endif
+
 #if defined(TARGET_32) && defined (MSVC_COMPILER)
     //'strcpy': This function or variable may be unsafe. Consider using strcpy_s instead. To disable deprecation, use _CRT_SECURE_NO_WARNING
 	#define _CRT_SECURE_NO_WARNINGS
 	#pragma warning (disable: 4703) //potentially uninitialized local pointer variable
 
 #endif
 
 
 /*------------------------------------------------------------*/
 #if MYMAT_LIBRARY==1
 		#define PCGRAND_LIBRARY 1
 		#define MKLRAND_LIBRARY 0
 #endif
+
+
 /*------------------------------------------------------------*/
 #if defined(MSVC_COMPILER)
 		#define INLINE    __inline
 		#define _restrict __restrict
         #define UNUSED_DECORATOR 
 #elif defined(SOLARIS_COMPILER) 
 	//#if defined(__SUNPRO_C)||defined(__SUNPRO_CC)
@@ -214,30 +229,14 @@
 	//https://stackoverflow.com/questions/4750880/can-i-treat-a-specific-warning-as-an-error
 	// #pragma warning (error: 4013)
 #else
     # define ALIGN32_BEG
     # define ALIGN32_END __attribute__((aligned(32)))
 #endif
 
-#define _in_
-#define _inout_
-#define _out_
-
-
-#define max(a,b)			(((a) > (b)) ? (a) : (b))
-#define min(a,b)			(((a) < (b)) ? (a) : (b))
-// The outermost parentheses are DEFINITELY needed. If not, subtile errors
-// can creep. Here is a failing example from beastv2_func.c
-// min(Kbase + b->ke[j], Klastcol) - (Kbase + b->ks[j]) + 1
-
-#define mv(n, src, dest)	r_cblas_scopy( n,src, 1L, dest, 1L) 
-#define cp(n, src, dest)    memcpy(dest, src, sizeof(F32)*(size_t)(n))
-#define SCPY(n, src, dest)  memcpy(dest, src, sizeof(F32)*(size_t)(n))
-#define FILL0(dest,n)       memset(dest, 0L,  sizeof(F32)*(size_t)(n))
-
 
 /*------------------------------------------------------------*/
 	#define DIAG_STR(s) #s
 	#define DIAG_JOINSTR(x,y) DIAG_STR(x ## y)
 	#ifdef MSVC_COMPILER
 		#define DIAG_DO_PRAGMA(x) __pragma (#x)
 		#define DIAG_PRAGMA(compiler,x) DIAG_DO_PRAGMA(warning(x))
@@ -289,17 +288,19 @@
 	DISABLE_WARNING(incompatible-pointer-types,incompatible-pointer-types, NOT_USED)\
 	DISABLE_WARNING(self-assign,self-assign, NOT_USED) \
     DISABLE_WARNING(unused-value,unused-value, NOT_USED) \
     DISABLE_WARNING(int-conversion,int-conversion, NOT_USED) \
     DISABLE_WARNING(restrict,restrict, NOT_USED)\
     DISABLE_WARNING(switch, switch, NOT_USED) \
     DISABLE_WARNING(uninitialized, uninitialized, NOT_USED)\
-    DISABLE_WARNING(pedantic, pedantic, NOT_USED)
+    DISABLE_WARNING(pedantic, pedantic, NOT_USED) \
+    DISABLE_WARNING(div-by-zero,div-by-zero, NOT_USED)
 
 	#define  ENABLE_MANY_WARNINGS   \
+    ENABLE_WARNING(div-by-zero,div-by-zero, NOT_USED) \
     ENABLE_WARNING(pedantic, pedantic, NOT_USED)\
     ENABLE_WARNING(uninitialized, uninitialized, NOT_USED)\
     ENABLE_WARNING(switch, switch, NOT_USED)\
     ENABLE_WARNING(restrict, restrict, NOT_USED)\
     ENABLE_WARNING(int-conversion,int-conversion, NOT_USED) \
     ENABLE_WARNING(unused-value,unused-value, NOT_USED) \
 	ENABLE_WARNING(self-assign,self-assign, NOT_USED) \
@@ -343,16 +344,16 @@
 	DISABLE_WARNING(incompatible-pointer-types,incompatible-pointer-types, NOT_USED)\
 	DISABLE_WARNING(self-assign,self-assign, NOT_USED)  \
     DISABLE_WARNING(unused-value,unused-value, NOT_USED) \
     DISABLE_WARNING(int-conversion,int-conversion, NOT_USED) \
     DISABLE_WARNING(switch, switch, NOT_USED) \
     DISABLE_WARNING(uninitialized, uninitialized, NOT_USED)\
     DISABLE_WARNING(pedantic, pedantic, NOT_USED) \
-    DISABLE_WARNING(typedef-redefinition, typedef-redefinition, NOT_USED) 
-
+    DISABLE_WARNING(typedef-redefinition, typedef-redefinition, NOT_USED) \
+    DISABLE_WARNING(div-by-zero,div-by-zero, NOT_USED)
 
 	/*DISABLE_WARNING(restrict, restrict, NOT_USED)\*/
 	/*ENABLE_WARNING(restrict, restrict, NOT_USED)\*/
 
 	//https: //github.com/nasa/trick/issues/600
 	//Clang no longer supports -Wno-unused-but-set-variable
 
@@ -362,14 +363,15 @@
 
 	//DISABLE_WARNING(unused-but-set-variable, unused-but-set-variable, NOT_USED) 
 	//DISABLE_WARNING(maybe-uninitialized, maybe-uninitialized, NOT_USED)
 
 	//https://clang.llvm.org/docs/DiagnosticsReference.html#wpragmas
 	//https://clang.llvm.org/docs/DiagnosticsReference.html#wrestrict-expansion
 	#define  ENABLE_MANY_WARNINGS  \
+    ENABLE_WARNING(div-by-zero,div-by-zero, NOT_USED) \
     ENABLE_WARNING(typedef-redefinition, typedef-redefinition, NOT_USED)\
     ENABLE_WARNING(pedantic, pedantic, NOT_USED)\
     ENABLE_WARNING(uninitialized, uninitialized, NOT_USED)\
     ENABLE_WARNING(switch, switch, NOT_USED)\
     ENABLE_WARNING(int-conversion,int-conversion, NOT_USED) \
     ENABLE_WARNING(unused-value,unused-value, NOT_USED) \
 	ENABLE_WARNING(self-assign,self-assign, NOT_USED) \
@@ -430,8 +432,21 @@
 //https://stackoverflow.com/questions/45477355/difference-between-pragma-and-pragma-in-c
 //_Pragma ("GCC dependency \"parse.y\"")
 
 #define  CHANGE_TO_AVX_GCC  \
           DIAG_DO_PRAGMA(GCC optimization_level 3) \
           DIAG_DO_PRAGMA(GCC optimize("O3,Ofast,inline,omit-frame-pointer,no-asynchronous-unwind-tables")) \
           DIAG_DO_PRAGMA(GCC target("sse,sse2,sse3,ssse3,sse4,popcnt,avx,avx2,fma,tune=haswell"))  
- 
+
+
+
+#define _in_
+#define _inout_
+#define _out_
+
+
+
+
+#define mv(n, src, dest)	r_cblas_scopy( n,src, 1L, dest, 1L) 
+#define cp(n, src, dest)    memcpy(dest, src, sizeof(F32)*(size_t)(n))
+#define SCPY(n, src, dest)  memcpy(dest, src, sizeof(F32)*(size_t)(n))
+#define FILL0(dest,n)       memset(dest, 0L,  sizeof(F32)*(size_t)(n))
```

### Comparing `Rbeast-0.1.13/ext_src/abc_001_config.h` & `Rbeast-0.1.14/ext_src/abc_001_config.h`

 * *Files 4% similar despite different names*

```diff
@@ -17,36 +17,38 @@
 	#elif P_INTERFACE==1
 		#define DllExport   __declspec( dllexport ) 
 	#elif M_INTERFACE==1
 		#define DllExport 
 		#pragma comment(linker, "/export:mexFunction")  //(Linker option) export:mexFunction   
     #endif
 
-	#define INCLUDE_PTHREAD(_X_) QUOTE_IT(C:/USERS/zehaokg/Documents/Visual Studio 2013/Projects/Matlab_Mex_Test/Pthread_IncludeLib/_X_ )
+	#define INCLUDE_PTHREAD(_X_) QUOTE_IT(C:/USERS/zhaokg/Documents/Visual Studio 2013/Projects/Matlab_Mex_Test/Pthread_IncludeLib/_X_ )
 	#define INCLUDE_MATLAB(_X_)  QUOTE_IT(C:/Program Files/MATLAB/R2019a/extern/include/_X_ )
 	#define INCLUDE_MKL(_X_)     QUOTE_IT(C:/Program Files (x86)/Intel/oneAPI/mkl/latest/include/_X_ )
 	#define INCLUDE_IPP(_X_)     QUOTE_IT(C:/Program Files (x86)/Intel/oneAPI/ipp/latest/include/_X_ )
 	#define INCLUDE_R(_X_)       QUOTE_IT(C:/Program Files/R/R-3.6.2/include/_X_ )
 
+    #define LIB_FORTRAN(_X_) QUOTE_IT(C:/Program Files (x86)/Intel/oneAPI/compiler/latest/windows/compiler/lib/intel64_win/_X_ )
 	#define LIB_PTHREAD(_X_) QUOTE_IT(C:/USERS/zhaokg/Documents/Visual Studio 2013/Projects/Matlab_Mex_Test/Pthread_IncludeLib/_X_ )
 	#define LIB_MATLAB(_X_)  QUOTE_IT(C:/Program Files/MATLAB/R2019a/extern/lib/win64/microsoft/_X_ )
 	#define LIB_TBB(_X_)     QUOTE_IT(C:/Program Files (x86)/IntelSWTools/compilers_and_libraries/windows/tbb/lib/intel64_win/vc_mt/_X_ )
 	//#define LIB_TBBstatic(_X_) QUOTE_IT(G:/Intel_Library/tbb-2019_U3/build/vs2013/x64/Release-MT/_X_ )
 	#define LIB_MKL(_X_)     QUOTE_IT(C:/Program Files (x86)/Intel/oneAPI/mkl/latest/lib/intel64/_X_ )
 	#define LIB_IPP(_X_)     QUOTE_IT(C:/Program Files (x86)/Intel/oneAPI/ipp/latest/lib/intel64/_X_ )
     #define LIB_OpenMP(_X_)  QUOTE_IT(C:/Program Files (x86)/IntelSWTools/compilers_and_libraries/windows/compiler/lib/intel64_win/_X_ )
-	#define LIB_MyLIB(_X_)   QUOTE_IT(C:/Share/Fortran_blas_lib/_X_ )
-    #define LIB_Python(_X_)   QUOTE_IT(C:/Anaconda3/libs/_X_ )
+	#define LIB_MyLIB(_X_)   QUOTE_IT(D:/Share/Fortran_blas_lib/_X_ )
+    #define LIB_Python(_X_)  QUOTE_IT(C:/Anaconda3/libs/_X_ )
+    #define LIB_R(_X_)       QUOTE_IT(C:/Program Files/R/R-4.2.2/implib/_X_ )
+
+	#ifdef TARGET_32
+        #undef  LIB_R
+		#define LIB_R(_X_)       QUOTE_IT(C:/Program Files/R/R-4.2.2/implib/i386/_X_ )			
+	#endif
 
-#ifdef TARGET_32
-	#define LIB_R(_X_)       QUOTE_IT(C:/Program Files/R/R-4.1.0/implib/i386/_X_ )
-#else
-	#define LIB_R(_X_)       QUOTE_IT(C:/Program Files/R/R-4.1.0/implib/_X_ )
-#endif
-	#define LIB_FORTRAN(_X_) QUOTE_IT(C:/Program Files (x86)/Intel/oneAPI/compiler/latest/windows/compiler/lib/intel64_win/_X_ )
+	
 
 	#if R_INTERFACE==1
         // The R import libs are generated by:
          // gendef  Rlapack.dll
          // lib /def:Rlapack.def /machine:x64 /out:Rlapack.lib
 		#pragma comment( lib , LIB_R(R.lib)       )
 		#pragma comment( lib , LIB_R(Rblas.lib)   )
@@ -141,29 +143,29 @@
 	#pragma comment(lib , LIB_MATLAB(libmex.lib) )
 	#pragma comment(lib , LIB_MATLAB(libmat.lib) )
     #pragma comment(lib,  LIB_MATLAB(libmwservices.lib) )	 
     #pragma comment(lib , LIB_MATLAB(libut.lib) ) 
     // https://stackoverflow.com/questions/26271154/how-can-i-make-a-mex-function-printf-while-its-running/26271557
     //    libmwservices: for ioFlush (this is a C++ function with naming managling)
 	// https://www.advanpix.com/2016/07/02/devnotes-3-proper-handling-of-ctrl-c-in-mex-module/
-    //    libut.lib :    for utIsInterruptPending and utSetInterruptPending(bool); 
+    //    libut.lib :    for utIsInterruptPending and utSetInterruptPending(Bool); 
 #endif
 
 #if R_INTERFACE == 1
     
    #ifdef ERROR 
        #undef ERROR  //ERROR is defined in both windwos.h/wingdi.h and R.h
    #endif
 
 	#include <R.h>
 	#include <Rinternals.h>
 	#include <Rdefines.h>
-	#include "Rmath.h"
-	#include "R_ext/GraphicsEngine.h"
-	#include "R_ext/GraphicsDevice.h"	
+	#include <Rmath.h>
+	#include <R_ext/GraphicsEngine.h>
+	#include <R_ext/GraphicsDevice.h>	
 	#if MYMAT_LIBRARY ==1
 		//#include "R_ext\Lapack.h"
 		//#include "R_ext\BLAS.h"
 	#endif
 
 	//#include <R_ext\Rdynload.h>
 
@@ -210,8 +212,35 @@
   /*********************/
   // No need to set up the lib explicitly 
   // (1) pynconfig.h has a pragma line to add python.lib
   //  pragma comment(lib,"python37.lib")  //: #pragma comment(lib , LIB_MATLAB(libmx.lib) )
   // (2) Numpy usss the import_array to load the (np.core._multiarray_umath._ARRAY_API) variable
   //    to fill the api arrays
 
-#endif
+#endif
+
+
+
+
+// bool is defined in matlab's tmwtypes.h
+// bool is a keyword in C24
+#if R_INTERFACE==1 || P_INTERFACE==1
+	#ifndef Bool
+		//typedef uint8_t Bool;
+		#define  Bool  unsigned char
+	#endif
+#elif M_INTERFACE == 1
+	#ifndef Bool
+		//typedef uint8_t Bool;
+		 #include "mex.h"
+		 #define  Bool  bool     
+    #endif
+#endif
+
+
+// This must appear after the inclusion of R.h
+#ifdef CLANG_COMPILER
+	#undef sign    // In R, 'sign' is  defined as Rf_sign
+	#undef warning // In R 'warning' is defined as Rf_warning; warnng is also a C++ keyword
+#endif
+
+
```

### Comparing `Rbeast-0.1.13/ext_src/abc_blas_lapack_mkl.h` & `Rbeast-0.1.14/ext_src/abc_blas_lapack_mkl.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_blas_lapack_myl.h` & `Rbeast-0.1.14/ext_src/abc_blas_lapack_myl.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_common.c` & `Rbeast-0.1.14/ext_src/abc_common.c`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #include "abc_000_warning.h"
 
 #include "abc_common.h"
 #include "abc_001_config.h"
 #include "abc_sort.h"
 #include "abc_vec.h" //f32_sumfilter
 #include "abc_blas_lapack_lib.h"
+#include "abc_rand_pcg_local.h"
 
 
 /*Discarded code*/
 //clock_t tic, toc; tic = clock(); toc = clock();   
 /**********************************************/
 static INLINE int isSpace(char c) {return (c == ' ' || c == '\t' || c == '\n');}
 
@@ -31,38 +32,95 @@
 	int wordLen;                     /* length of current word */
 	int current_lineLen = 0;             /* current length of line */
 	int start_curLen = 0;              /* index of beginning if line */
 
 	while ((wordLen = get_word(str + start_curLen+ current_lineLen)) > 0) {
 		if (current_lineLen + wordLen < LINE_LENGTH) {
 			current_lineLen += wordLen;
-		}else {
+		} else {
 			str[start_curLen + current_lineLen] = '\n';
 			start_curLen += current_lineLen + 1L;
 			current_lineLen = 0L;
 		}
 
 	}
 	return str;
 }
 
+char* word_wrap_indented(char* str, int LINE_LENGTH, int nspace) {
+	char* space = "                      ";
+	char newstr[2000];
+	int  newlen = 0;
+	int  isfirstline = 1;
+
+	int wordLen;                     /* length of current word */
+	int current_lineLen = 0;             /* current length of line */
+	int start_curLen = 0;              /* index of beginning if line */
+
+	while ((wordLen = get_word(str + start_curLen + current_lineLen)) > 0) {
+
+		if (current_lineLen + wordLen < LINE_LENGTH) {
+			current_lineLen += wordLen;
+		}
+		else {
+
+			str[start_curLen + current_lineLen] = '\n';
+
+			if (isfirstline) {
+				isfirstline = 0;
+				memcpy(newstr + newlen, str + start_curLen, current_lineLen);
+				newlen += current_lineLen;
+				newstr[newlen++] = '\n';
+				LINE_LENGTH -= nspace;
+			}
+			else {
+				memcpy(newstr + newlen, space, nspace);
+				newlen += nspace;
+				memcpy(newstr + newlen, str + start_curLen, current_lineLen);
+				newlen += current_lineLen;
+				newstr[newlen++] = '\n';
+			}
+
+			start_curLen += current_lineLen + 1L;
+			current_lineLen = 0;
+
+		}
+	}
+	
+	if (isfirstline) {
+		memcpy(newstr + newlen, str + start_curLen, current_lineLen);
+	} else {
+		memcpy(newstr + newlen, space, nspace);
+		newlen += nspace;
+		memcpy(newstr + newlen, str + start_curLen, current_lineLen);
+	}
+	newlen += current_lineLen;
+	if (newstr[newlen] != '\n') {
+		newstr[newlen++] = '\n';
+	}
+	newstr[newlen++] = 0;
+	strcpy(str, newstr);
+	return str;
+}
+
+
 void ToUpper(char* s) { for (int i = 0; s[i] != '\0'; i++) 	s[i] = s[i] >= 'a' && s[i] <= 'z' ? s[i] - 32 : s[i]; }
 
 I32 strcicmp(char const * _restrict a, char const * _restrict b) {
 	for (;; a++, b++) {
 		I32 d = ((*a) | (U08)32) - ((*b) | (U08)32);
 		if (d != 0 || !*a)	
 			return d;
 	}
 }
 
 I32 strcicmp_nfirst(char const* _restrict a, char const* _restrict b, int nfirst) {
 	// only compare the strings up to the first 'nfirst' bytes
 	if (nfirst == 0) {
-		nfirst = strlen(a) + 1;
+		nfirst = (int) strlen(a) + 1;
 	}
 
 	int i = 0;
 	for (;; a++, b++) {
 		I32 d = ((*a) | (U08)32) - ((*b) | (U08)32);
 		i++;
 		if (d != 0 || !*a || i >= nfirst) {
@@ -149,15 +207,15 @@
 	}
 
 
 	//isNA is reused as a tmp buff
 	U08PTR isPeak = isNA;
 	I32PTR INDEX  = (I32PTR)(TMP + M); // INDEX is an array of lenght M
 
-	memset(isNA, 0, M);
+	memset(isNA, 0, (size_t) M);
 	I32  numPeaks = 0;
 	for ( I32 i = 2; i <= (M - 1); i++)	{
 		if (ans[(i)-1] > ans[(i - 1) - 1] && ans[(i)-1] > ans[(i + 1) - 1]) {
 			isPeak[i - 1] = 1;
 			INDEX[numPeaks++] = i;
 		}
 	}
@@ -254,16 +312,16 @@
 
 	I32  UPPERIDX  = N - w;
 	I32  numCpt = 0;
 	for (I32 i = w; i < UPPERIDX; i++)
 	{
 		if (mem[i] < threshold) continue;
 		
-		bool isLargeThanNearestNeighor		= (mem[i] >= mem[i - 1]) && (mem[i] >= mem[i + 1]);
-		bool isLargeThanNearestTwoNeighors	= (mem[i] * 4.0) > (mem[i + 1] + mem[i + 2] + mem[i - 1] + mem[i - 2]);
+		Bool isLargeThanNearestNeighor		= (mem[i] >= mem[i - 1]) && (mem[i] >= mem[i + 1]);
+		Bool isLargeThanNearestTwoNeighors	= (mem[i] * 4.0) > (mem[i + 1] + mem[i + 2] + mem[i - 1] + mem[i - 2]);
 		if (!(isLargeThanNearestNeighor && isLargeThanNearestTwoNeighors)) continue;
 
 		// If the current point is a local maximum in the filtered prob curve
 		// , then find the maximum in the prob curve within a (w2+1) window at the current point
 		I32		upperIdx_1	= i + w;
 		I32		maxIdx		= -999;
 		F32		maxVal		= -999;
@@ -429,16 +487,16 @@
 	I32  LOWERIDX  = (minSepDist + 1);
 	I32  UPPERIDX  = N - (minSepDist + 1);
 	I32  numCpt    = 0;
 	for (I32 i = LOWERIDX; i < UPPERIDX; i++)
 	{
 		if (mem[i] < threshold) continue;
 
-		bool isLargeThanNearestNeighor     = (mem[i] >= mem[i - 1]) && (mem[i] >= mem[i + 1]);
-		bool isLargeThanNearestTwoNeighors = (mem[i] * 4.0) > (mem[i + 1] + mem[i + 2] + mem[i - 1] + mem[i - 2]);
+		Bool isLargeThanNearestNeighor     = (mem[i] >= mem[i - 1]) && (mem[i] >= mem[i + 1]);
+		Bool isLargeThanNearestTwoNeighors = (mem[i] * 4.0) > (mem[i + 1] + mem[i + 2] + mem[i - 1] + mem[i - 2]);
 		if ( isLargeThanNearestNeighor==0 || isLargeThanNearestTwoNeighors==0 ) continue;
 
 		// If the current point is a local maximum in the filtered prob curve
 		// , then find the maximum in the PROB curve within a (w2+1) window at the current point
 		I32		UPPERIDX_1 = i + w1;
 		I32		maxIdx = -9999;
 		F32		maxVal = -9999.f;
@@ -560,162 +618,343 @@
 
 		cpt_summedProb[i] = cpfromSumP_Val[i]>1 ? 1.f : cpfromSumP_Val[i];
 	}
 
 	return numCpt;
 }
 
+static I32 FindChangepoint_minseg_is_1(F32PTR prob, F32PTR mem, F32 threshold, I32PTR cpt, F32PTR cptCI, I32 N, I32 minSepDist, I32 maxCptNumber) {
+
+	// minSepDist may be zero.
+	
+	F32PTR sump           = mem;
+	I32PTR cpfromSumP_Pos = (I32PTR)mem + N;
+	F32PTR cpfromSumP_Val = (F32PTR)mem + N * 2;
+	I32PTR cpfromProb_Pos = (I32PTR)mem + N * 3;
+	F32PTR cpfromProb_Val = (F32PTR)mem + N * 4;
+
+	// Set zeros to the mem array--used to hold the sum-filtered prob
+	r_ippsSet_32f(0, sump, N);        
+
+    // Now mem holds the sum-filterd probability profile: the value at a point  is the sume 
+	// of the prob values within a window [i-w0,i+w1].In this funciton, the two parts of 
+	// the window are computed differently from the above commented routine [i-w0, i+w1]
+	I32 minSegLen = minSepDist + 1;
+	I32 w0 = minSegLen / 2;       // leftside half
+	I32 w1 = (minSegLen - w0)-1;  // rightside half	  and we have  w0 >= w1		
+	f32_sumfilter(prob, sump, N, minSegLen);
+
+	//Special treatment when minSepDist=0; this is for the outlier component only
+	I32  LOWERIDX = 0;       // LOWERIDX=(minSepDist + 1);  
+	I32  UPPERIDX = N - 1;   /// N - (minSepDist + 1);
+	I32  numCpt = 0;
+
+	for (I32 i = LOWERIDX; i < UPPERIDX; i++) 	{
+		if (sump[i] < threshold) continue;
+		cpfromSumP_Pos[numCpt] = i;
+		cpfromSumP_Val[numCpt] = sump[i];
+		numCpt++;	 
+	}
+
+	// The cpts identified above are based on peak in the summed probability, and now for each of them
+	// find the best peak in the original prob.
+	for (I32 i = 0; i < numCpt; i++) {
+		I32     cpt         = cpfromSumP_Pos[i];		
+		I32     LOWERIDX    = cpt-w0;
+		I32		UPPERIDX    = cpt+w1;
+
+		cpfromProb_Pos[i] = cpt;
+		cpfromProb_Val[i] = prob[cpt];
+
+	}
+	//cpfromProb_Pos may contian changepoinss that are within a distance of minSepDist from each other
+ 
+	if (numCpt == 0) { return numCpt; }
+
+	QuickSortD(cpfromSumP_Val, cpfromProb_Pos, 0, numCpt - 1);
+	numCpt = min(numCpt, maxCptNumber);
+
+	f32_copy((F32PTR)cpfromProb_Pos, (F32PTR)cpt, numCpt);
+	// At this point, cpfromSumP_val has the prob values sorted from largest to least
+	// cpfromProb_Pos and cpt (integers) are the same, containing the cpt locations
+
+	// Now cpfromSumP_Val(mem+2*N) should not be touched and will be used later
+	I32PTR INDEX_timeToProbAmp = (I32*)mem;
+	F32PTR cpt_f32              = (F32*)mem + N;
+	for (I32 i = 0; i < numCpt; i++) {
+		cpt_f32[i]             = (F32)cpt[i];
+		INDEX_timeToProbAmp[i] = i;
+	}
+	QuickSortA(cpt_f32, INDEX_timeToProbAmp, 0, numCpt - 1);
+	// Now, cpt_f32 contains the cpts ranked in the order of time
+	// INDEX saves the indices mapping to the list ranked in magnitdue
+
+	//Compute confidence intervals for indentified changepoints
+	// Fill the ctpCI with negative values
+	
+
+	//Now, cpt contains knots sorted in magnitude
+	// cptCI contains CI for knots sorted in time
+
+	F32PTR cpt_summedProb = mem;
+	/*
+	mem   : Index/cpt_summedProb
+	mem+N : CPT_float
+	mem+2*N:cpfromSum_Val
+	mem+3*N:cpt_CI_backup
+	*/
+	for (I32 i = 0; i < numCpt; i++) {
+		//Duel use of mem: one for INDEX and another for cpt_summrProb
+		//The index is feteched first and the same elment is overwritten with the summProb
+		I32 idx = INDEX_timeToProbAmp[i];
+		cptCI[idx]          = cpt_f32[i] - 0;
+		cptCI[numCpt + idx] = cpt_f32[i] + 0;
+
+		cpt_summedProb[i] = cpfromSumP_Val[i] > 1 ? 1.f : cpfromSumP_Val[i];
+	}
+
+	return numCpt;
+}
+
+ 
 I32 FindChangepoint(F32PTR prob, F32PTR mem, F32 threshold, I32PTR cpt, F32PTR cptCI, I32 N, I32 minSepDist, I32 maxCptNumber)
 {
+	// minSepDist may be zero.
+	// The seg pattern is  "c"     when minseg=1
+	// The seg pattern is  "xc"    when minseg=2
+	// The seg pattern is  "xcx"   when minseg=3
+	// The seg pattern is  "xxcx"   when minseg=4
+	// The seg pattern is  "xxcxx"  when minseg=5
+
 	if (maxCptNumber == 0) { return maxCptNumber; }
 
+	if (minSepDist == 0) {
+	// this is only for the outlier component
+		return FindChangepoint_minseg_is_1(prob, mem, threshold, cpt, cptCI, N, minSepDist, maxCptNumber);
+	}
+
 	F32PTR sump           = mem;
 	I32PTR cpfromSumP_Pos = (I32PTR)mem + N;
 	F32PTR cpfromSumP_Val = (F32PTR)mem + N * 2;
 	I32PTR cpfromProb_Pos = (I32PTR)mem + N * 3;
 	F32PTR cpfromProb_Val = (F32PTR)mem + N * 4;
 
-	// Half the inter-changepoint distacne
-	I32 w0 = minSepDist / 2;   // leftside half
-	I32 w1 = minSepDist - w0;  // rightside half
-	/*
-	// A fast way to apply a w-sum filter to the prob arrary
-	for (I32 i = -w1; i <= w0; i++)
-	{
-		I32 len = i > 0 ? i : -i;
+	/* // A fast way to apply a w-sum filter to the prob arrary
+	for (I32 i = -w1; i <= w0; i++)	{
+		I32 len          = i > 0 ? i : -i;
 		I32 startIdx_mem = i <= 0 ? 0 : i;
 		I32 startIdx_prob = i <= 0 ? -i : 0;
 		r_ippsAdd_32f_I(prob + startIdx_prob, mem + startIdx_mem, N - len);
-	}
-	// Now mem holds the sum-filterd probability profile: the value at a point
-	// is the sume of the prob values within a window [i-w0, i+w1]
+	} // Now mem holds the sum-filterd probability profile: the value at a point is the sume of the prob values within a window [i-w0, i+w1]
 	*/
 
-	// Now mem holds the sum-filterd probability profile: the value at a point  is the sume 
+	// Set zeros to the mem array--used to hold the sum-filtered prob
+	r_ippsSet_32f(0, sump, N);        
+
+    // Now mem holds the sum-filterd probability profile: the value at a point  is the sume 
 	// of the prob values within a window [i-w0,i+w1].In this funciton, the two parts of 
-	// the window are computed differently from the above commented routine
-	//	I32 w0 = minSepDist / 2;       // leftside half
-	//  I32 w1 = (minSepDist - w0)-1;  // rightside half
-	
-	r_ippsSet_32f(0, sump, N);                                     // Set zeros to the mem array--used to hold the sum-filtered prob
-	f32_sumfilter(prob, sump, N, minSepDist);
+	// the window are computed differently from the above commented routine [i-w0, i+w1]
+	I32 minSegLen = minSepDist + 1;
+	I32 w0        = minSegLen / 2;       // leftside half
+	I32 w1        = (minSegLen - w0)-1;  // rightside half	  and we have  w0 >= w1		
+	f32_sumfilter(prob, sump, N, minSegLen);
 
 	I32  LOWERIDX = (minSepDist + 1);
 	I32  UPPERIDX = N - (minSepDist + 1);
 	I32  numCpt = 0;
-	for (I32 i = LOWERIDX; i < UPPERIDX; i++)
-	{
-		if (sump[i] < threshold) continue;
+	for (I32 i = LOWERIDX; i < UPPERIDX; i++) 	{
 
-		bool isLargeThanNearestNeighor     = (sump[i] >= sump[i - 1]) && (sump[i] >= sump[i + 1]);
-		bool isLargeThanNearestTwoNeighors = (sump[i] * 4.0) > (sump[i + 1] + sump[i + 2] + sump[i - 1] + sump[i - 2]);
-		if (isLargeThanNearestNeighor == 0 || isLargeThanNearestTwoNeighors == 0) continue;
+		if (sump[i] < threshold) continue;
 
+		// Imporant: stricltly larger than the keft, larger or equal to the right: oick up the rising side of the plateau peak
+		Bool isLargeThanNearestNeighor     = (sump[i] > sump[i - 1] && sump[i] >= sump[i + 1]) || (sump[i] >= sump[i - 1] && sump[i] >  sump[i + 1]);
+		Bool isLargeThanNearestTwoNeighors = (sump[i] * 4.0) >= (sump[i + 1] + sump[i + 2] + sump[i - 1] + sump[i - 2]);
+		// if minSegLen = 1,2, 3, or 4, we only check the two neihgoring points, not the four neighors
+		if (isLargeThanNearestNeighor == 0 || (minSegLen>4 && isLargeThanNearestTwoNeighors == 0)  ) continue;
 
 		/*********************************************************************/
 		// If the current point is a local maximum in the filtered prob curve
 		/*********************************************************************/
-		I32 dist_to_prevCpt = i - cpfromSumP_Pos[numCpt - 1];
+		I32 dist_to_prevCpt = i - cpfromSumP_Pos[numCpt - 1]; //invalid if numCpt==0
 		if ((numCpt == 0) || dist_to_prevCpt > minSepDist || dist_to_prevCpt < -minSepDist) {
 			//If the current identified peak is NOT within a distance less (2*w+1)
 			cpfromSumP_Pos[numCpt] = i;
 			cpfromSumP_Val[numCpt] = sump[i];
 			numCpt++;
 			continue;
-		}
-		else {
+		} else {
 			//if it is within a distance less than minSepDist PLUS the current peak has 
 			// a larer magnitude than the previously identified cp then replace the old changepoint
 			// with the new peak.			
-			if (sump[i] >= cpfromSumP_Val[numCpt - 1]) {
+			if (sump[i] > cpfromSumP_Val[numCpt - 1]) { // Possible buggy if using sump[i] ">=" cpfromSumP_Val[numCpt - 1]
 				cpfromSumP_Pos[numCpt - 1] = i;
 				cpfromSumP_Val[numCpt - 1] = sump[i];
 				continue;
 			}
 		}
 
 	}
 
-	// The cpts identified above are based peak summed probability, and now for each of them
-	// find the best peak in prob.
-	for (I32 i = 0; i < numCpt; i++) {
-
-		I32     cpt         = cpfromSumP_Pos[i];
-		
-		I32     LOWERIDX    = cpt-w0;
-		I32		UPPERIDX    = cpt+w1;
-
-		// Pre-assign the best cpt to the sumP-based cpt: this is needed when minSepdist=0 (i.e., outlier componet)
-		// such that the following loop only runs once and no local min is found to update maxIdx and maxVAl
-		I32		maxIdx      = cpt;              
-		F32		maxVal      = prob[cpt];
-		for (I32 j = LOWERIDX;  j <= UPPERIDX; j++) {
-			if ((prob[j] > prob[j - 1] && prob[j] >= prob[j + 1]) || (prob[j] >= prob[j - 1] && prob[j] > prob[j + 1])) {
-				if (prob[j] > maxVal) {
-					maxIdx = j;
-					maxVal = prob[j];
+	/************************************************************************************************/
+	// The cpts identified above are based on peak in the summed probability, and now for each of them
+	// find the best peak in the original prob.
+	/************************************************************************************************/
+	if (minSepDist <= 4) {
+		for (I32 i = 0; i < numCpt; i++) {
+			I32     cpt = cpfromSumP_Pos[i];
+			I32     LOWERIDX = cpt - w0;
+			I32		UPPERIDX = cpt + w1;
+
+			// Pre-assign the best cpt to the sumP-based cpt: this is needed when minSepdist=0 (i.e., outlier componet)
+			// such that the following loop only runs once and no local min is found to update maxIdx and maxVAl
+			I32		maxIdx = cpt;
+			F32		maxVal = prob[cpt];
+			for (I32 j = LOWERIDX; j <= UPPERIDX; j++) {
+				F32 curProb = prob[j];
+				if ((curProb > prob[j - 1] && curProb >= prob[j + 1]) || (curProb >= prob[j - 1] && curProb > prob[j + 1])) {
+					if (curProb > maxVal) {
+						maxIdx = j;
+						maxVal = curProb;
+					}
 				}
 			}
+			cpfromProb_Pos[i] = maxIdx;
+			cpfromProb_Val[i] = maxVal;
+
 		}
-		cpfromProb_Pos[i] = maxIdx;
-		cpfromProb_Val[i] = maxVal;
+	} else {
+		// if minSeptDist >4, we will use a more complex rule to pinpoint the best peak bcz  the simple alg for the minsepdist,4 case
+		// may not find the location with the highest amassed probability
+		for (I32 i = 0; i < numCpt; i++) {
+			I32     cpt = cpfromSumP_Pos[i];
+			I32     LOWERIDX = cpt - w0;
+			I32		UPPERIDX = cpt + w1;
+
+			//First, find all the local peaks up to a number of 10
+			I32 topTenPeaksLoc[10];
+			F32 topTenPeaksPrb[10];
+			I32 numTopTenCpt = 0;
+
+			for (I32 j = LOWERIDX; j <= UPPERIDX; j++) {
+				F32 curProb = prob[j];
+				if ((curProb > prob[j - 1] && curProb >= prob[j + 1]) || (curProb >= prob[j - 1] && curProb > prob[j + 1])) {
+					if (numTopTenCpt < 10) {
+						topTenPeaksLoc[numTopTenCpt] = j;
+						topTenPeaksPrb[numTopTenCpt] = curProb;
+						numTopTenCpt++;
+					}	else {
+						// If the buf is full, find the worst peak and replace if the curprob is higher.
+						F32 minProbInList    = 100.f;
+						int minProbListIndex = 0;
+						for (int k = 0; k < 10; k++) {
+							if (minProbInList > topTenPeaksPrb[k]) {
+								minProbListIndex = k;
+								minProbInList    = topTenPeaksPrb[k];
+							}
+						}
+
+						if (curProb > minProbInList) {
+							topTenPeaksLoc[minProbListIndex] = j;
+							topTenPeaksPrb[minProbListIndex] = curProb;
+						}
+					}					
+				} //(curProb > prob[j - 1] && curProb >= prob[j + 1]) || (curProb >= prob[j - 1] && curProb > prob[j + 1]))
+			} //for (I32 j = LOWERIDX; j <= UPPERIDX; j++) 
+
+			if (numTopTenCpt == 0) {
+				// If no local peask were found (this is unlikely the case),just use the best cpt to the sumP-based cpt: 
+				cpfromProb_Pos[i] = cpt;
+				cpfromProb_Val[i] = prob[cpt];
+			}
+			else if (numTopTenCpt == 1) {
+				cpfromProb_Pos[i] = topTenPeaksLoc[0];
+				cpfromProb_Val[i] = topTenPeaksPrb[0];
+			}
+			else {
+				// there are at least 2 cpts in the top list
+				QuickSortD(topTenPeaksPrb, topTenPeaksLoc, 0, numTopTenCpt - 1);
+				if (topTenPeaksPrb[0] > 1.5 * topTenPeaksPrb[1]) {
+					// if the best peak is far beter than the the seond best peak
+					cpfromProb_Pos[i] = topTenPeaksLoc[0];
+					cpfromProb_Val[i] = topTenPeaksPrb[0];
+				}
+				else {
+					int bestK = 0;
+					F32 bestProb_3Neighors = -9999;
+					for (int k = 0; k < numTopTenCpt; k++) {
+						int cpLoc = topTenPeaksLoc[k];
+						F32 cpProb_3Neighors = prob[cpLoc] + prob[cpLoc + 1] + prob[cpLoc - 1];
+						if (cpProb_3Neighors > bestProb_3Neighors) {
+							bestProb_3Neighors = cpProb_3Neighors;
+							bestK              = k;
+						}
+					}
+					cpfromProb_Pos[i] = topTenPeaksLoc[bestK];
+					cpfromProb_Val[i] = topTenPeaksPrb[bestK];
+				}
+			} //if (numTopTenCpt == 0) 
 
+		}//for (I32 i = 0; i < numCpt; i++)
 	}
+
 	//cpfromProb_Pos may contian changepoinss that are within a distance of minSepDist from each other
  
+
+
 	if (numCpt == 0) { return numCpt; }
 
 	QuickSortD(cpfromSumP_Val, cpfromProb_Pos, 0, numCpt - 1);
 	numCpt = min(numCpt, maxCptNumber);
 
 	f32_copy((F32PTR)cpfromProb_Pos, (F32PTR)cpt, numCpt);
 	// At this point, cpfromSumP_val has the prob values sorted from largest to least
 	// cpfromProb_Pos and cpt (integers) are the same, containing the cpt locations
 
-	// Now cpfromSum_Val(mem+2*N) should not be touched and will be used later
+	// Now cpfromSumP_Val(mem+2*N) should not be touched and will be used later
 	I32PTR INDEX_timeToProbAmp = (I32*)mem;
-	F32PTR cpt_f32 = (F32*)mem + N;
+	F32PTR cpt_f32              = (F32*)mem + N;
 	for (I32 i = 0; i < numCpt; i++) {
 		cpt_f32[i]             = (F32)cpt[i];
 		INDEX_timeToProbAmp[i] = i;
 	}
 	QuickSortA(cpt_f32, INDEX_timeToProbAmp, 0, numCpt - 1);
 	// Now, cpt_f32 contains the cpts ranked in the order of time
 	// INDEX saves the indices mapping to the list ranked in magnitdue
 
 	//Compute confidence intervals for indentified changepoints
 	// Fill the ctpCI with negative values
 	f32_fill_val(-9999.f, cptCI, 2 * numCpt);
 
 	F32PTR tmpSeg = (F32*)mem + 3 * N;
 	I32PTR nullSeg = (I32*)mem + 4 * N;
-	for (I32 i = 0; i < numCpt; i++)
-	{
+	for (I32 i = 0; i < numCpt; i++) 	{
+
 		I32 startIdx, endIdx, len;
 
+		//-------------------------------------------------------------------
 		endIdx = (I32)cpt_f32[i];
 		startIdx = i == 0 ? 0 : (I32)cpt_f32[i - 1];
 		startIdx = (startIdx + endIdx) / 2;
 		len = endIdx - startIdx + 1;
 
 		f32_copy(prob + startIdx, tmpSeg, len);
 		QuickSortA(tmpSeg, nullSeg, 0, len - 1); // nullSeg is just provided as an input but the result is not used
-		cptCI[i] = confidenceInterval(tmpSeg, len, 'L');
-
-		//-------------------------------------------------------------------
+		cptCI[i] = confidenceInterval(tmpSeg, len, 'L');		
 		//-------------------------------------------------------------------
 
+		//-------------------------------------------------------------------
 		startIdx = (I32)cpt_f32[i];
 		endIdx = i == (numCpt - 1) ? (N - 1) : (I32)cpt_f32[i + 1];
 		endIdx = (startIdx + endIdx) / 2;
 		len = endIdx - startIdx + 1;
 
 		f32_copy(prob + startIdx, tmpSeg, len);
 		QuickSortD(tmpSeg, nullSeg, 0, len - 1); // nullSeg is just provided as an input but the result is not used
 		cptCI[numCpt + i] = confidenceInterval(tmpSeg, len, 'R');
+		//-------------------------------------------------------------------
 	}
 
 	//Now, cpt contains knots sorted in magnitude
 	// cptCI contains CI for knots sorted in time
 
 	F32PTR cptCI_backup = mem + 3 * N;
 	f32_copy(cptCI, cptCI_backup, 2 * numCpt);
@@ -727,65 +966,24 @@
 	mem+2*N:cpfromSum_Val
 	mem+3*N:cpt_CI_backup
 	*/
 	for (I32 i = 0; i < numCpt; i++) {
 		//Duel use of mem: one for INDEX and another for cpt_summrProb
 		//The index is feteched first and the same elment is overwritten with the summProb
 		I32 idx = INDEX_timeToProbAmp[i];
-		cptCI[idx] = cpt_f32[i] - cptCI_backup[i];
+		cptCI[idx]          = cpt_f32[i] - cptCI_backup[i];
 		cptCI[numCpt + idx] = cpt_f32[i] + cptCI_backup[numCpt + i];
 
 		cpt_summedProb[i] = cpfromSumP_Val[i] > 1 ? 1.f : cpfromSumP_Val[i];
 	}
 
 	return numCpt;
 }
 
-void WriteF32ArraryToStrideMEM(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 dstOffset, DATA_TYPE dtype) 
-{
-	if ( dtype == DATA_FLOAT  )	{	  
-		f32_to_strided_f32(src, dst, N, stride, dstOffset);
-	}
-	else if (dtype == DATA_DOUBLE) {
-		f32_to_strided_f64(src, dst, N, stride, dstOffset);
-	}
-}
-
-
-void CopyStrideMEMToF32Arr(F32PTR dst,  VOID_PTR src, int N, int srcStride, int srcOffset, DATA_TYPE srcDataType)
-{
-	if      (srcDataType== DATA_FLOAT) 	{
-		f32_from_strided_f32(dst, src, N, srcStride, srcOffset);
-	}  
-	else if (srcDataType == DATA_DOUBLE){
-		f32_from_strided_f64(dst, src, N, srcStride, srcOffset);
-	}  
-	else if (srcDataType == DATA_INT64) {
-		f32_from_strided_i64(dst, src, N, srcStride, srcOffset);
-	}
-	else if (srcDataType == DATA_INT32)	{
-		f32_from_strided_i32(dst, src, N, srcStride, srcOffset);
-	}  
-	else if (srcDataType == DATA_INT16)	{
-		f32_from_strided_i16(dst, src, N, srcStride, srcOffset);
-	}  
- 
-}
 
-void WriteStrideMEMToArrMEM(VOID_PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset, DATA_TYPE srcDstDataType)
-{
-	if (srcDstDataType == DATA_FLOAT) {
-		f32_from_strided_f32(dst, src, N, srcStride, srcOffset);
-	} else if (srcDstDataType == DATA_DOUBLE) {
-		f32_from_strided_f64(dst, src, N, srcStride, srcOffset);
-		f32_to_f64_inplace(dst, N);
-	}
-	 
- 
-}
 /*
 int NormalizeF32ArrayWithNaNOmitted(F32PTR Y, U32PTR rowsMissing, I32 N,F32PTR mean, F32PTR sd, F32PTR yty) {
 
 	I32     nMissing = 0;	
 	F64     sum      = 0;
 	F64     sqsum    = 0;
 	for (rI32 i = 0; i < N; i++) { 
@@ -826,44 +1024,52 @@
 		yty[0]  = YtY;
 
 	}
 
 	return nMissing;
 }
 */
+
 #if defined(WIN64_OS) || defined(WIN32_OS) 
 	#include "float.h"
 	#if defined(MSVC_COMPILER)
-	void EnableFloatExcetion() {
+	void EnableFloatExcetion(void) {
 		unsigned int _oldState;
 		errno_t err = _controlfp_s(&_oldState, EM_OVERFLOW | EM_UNDERFLOW | EM_ZERODIVIDE | EM_DENORMAL | EM_INVALID, MCW_EM);
 		//errno_t err = _controlfp_s(&_oldState, EM_OVERFLOW | EM_ZERODIVIDE | EM_DENORMAL | EM_INVALID, MCW_EM);
 		//errno_t err = _controlfp_s(&_oldState, EM_OVERFLOW | EM_ZERODIVIDE | EM_INVALID, MCW_EM); 
 	}
 	#elif defined(GCC_COMPILER)
-void EnableFloatExcetion() {
+void EnableFloatExcetion(void) {
 		unsigned int _oldState;
 		errno_t err = _controlfp_s(&_oldState, _EM_OVERFLOW | _EM_UNDERFLOW | _EM_ZERODIVIDE | _EM_DENORMAL | _EM_INVALID, _MCW_EM);
 		//errno_t err = _controlfp_s(&_oldState, EM_OVERFLOW | EM_ZERODIVIDE | EM_DENORMAL | EM_INVALID, MCW_EM);
 		//errno_t err = _controlfp_s(&_oldState, EM_OVERFLOW | EM_ZERODIVIDE | EM_INVALID, MCW_EM); 
 	}
 	#endif
 #else
 	#include "fenv.h" 
-void EnableFloatExcetion() {
-	 // https://lists.gnu.org/archive/html/bug-gsl/2009-01/msg00001.html 
+void EnableFloatExcetion(void) {
+     // https://lists.gnu.org/archive/html/bug-gsl/2009-01/msg00001.html 
      // for unknow reasons, feenableexcept is not in fenv.h for Rtools.
-	//https://stackoverflow.com/questions/33191530/how-to-solve-undefined-reference-to-functions-in-fenv-h-when-using-uclibc
-	//lm is need for the linker 
+	 //https://stackoverflow.com/questions/33191530/how-to-solve-undefined-reference-to-functions-in-fenv-h-when-using-uclibc
+	 //lm is need for the linker 
 
 	//stackoverflow.com/questions/37819235/how-do-you-enable-floating-point-exceptions-for-clang-in-os-x
 	//https://gitlab.ikp.kit.edu/AirShowerPhysics/corsika/-/issues/415
 	#if defined(LINUX_OS) 
-	feenableexcept(FE_DIVBYZERO | FE_INVALID | FE_OVERFLOW); 
+	   // Not availalbe in C23 for clang16
+	   //feenableexcept(FE_DIVBYZERO | FE_INVALID | FE_OVERFLOW); 
 	#endif
+
+	
+    // MacOS: feenableexcept not defined on MacOS  //https://philbull.wordpress.com/2012/07/27/portability-issues-with-floating-point-exception-handling/
+	// Rtools: feenableexcept not defined for Rtools
+	// Linux:  seems to be only defined for C99    https://linux.die.net/man/3/feenableexcept
+	// Check C99: https://stackoverflow.com/questions/19674401/is-there-a-preprocessor-macro-to-detect-c99-across-platforms
 }
 #endif
 
 
 /*
 static INLINE void zeroOut_Xmars_zero(F32PTR Xt_mars, F32PTR Xt_zeroBackup, U32PTR rowsMissing,
 	U32 nMissing, I32 N, I32 Npad, int k)
@@ -893,8 +1099,130 @@
 		Xt_mars += Npad;
 	}
 
 }
 */
  
  
+
+#include "abc_cpu.h"
+#include "abc_ide_util.h"
+void SetupRoutines_AutoByCPU(Bool quite) {
+
+	static int IS_CPU_INSTRUCTON_CHECKED = 0;
+	if (IS_CPU_INSTRUCTON_CHECKED) {
+		return;
+	}
+	if (!quite)	r_printf("\nOn the first run, check the CPU instruction set ... \n");
+	 
+	 struct cpu_x86 cpuinfo;
+	 detect_host(&cpuinfo);
+	 if (!quite) print_cpuinfo(&cpuinfo);
+	 i386_cpuid_caches(quite);
+
+#if !defined(SOLARIS_COMPILER) && defined(TARGET_64) && !defined(ARM64_OS)
+	if (cpuinfo.HW_AVX512_F /*Foundation*/ && cpuinfo.HW_AVX512_BW && cpuinfo.HW_AVX512_DQ && cpuinfo.HW_AVX512_VL) {
+		 SetupVectorFunction_AVX512();
+		 SetupPCG_AVX512();
+		 if (!quite)	  r_printf("CPU checking result: The AVX512-enabled library is used ... \n\n");
+	}
+	else if (cpuinfo.HW_AVX &&cpuinfo.HW_AVX2 && cpuinfo.HW_FMA3) {
+		 SetupVectorFunction_AVX2();
+		 SetupPCG_AVX2();
+		 if (!quite)	 r_printf("CPU checking result: The AVX2-enabled library is used ...\n\n");
+	}
+	else {
+		 SetupVectorFunction_Generic();
+		 SetupPCG_GENERIC();
+		 if (!quite)	 r_printf("CPU checking result: No AVX2/AVX512 is supported and the default library is used ...\n\n");
+	}
+#else
+	 SetupVectorFunction_Generic();
+	 SetupPCG_GENERIC();
+	 if (!quite) r_printf("CPU checking result: No AVX2 is supported and the default library is used ...");
+#endif
+
+	 IS_CPU_INSTRUCTON_CHECKED = 1;
+
+}
+
+void SetupRoutines_UserChoice(int avxOption) {
+
+#if !defined(SOLARIS_COMPILER) && defined(TARGET_64) && !defined(ARM64_OS)
+
+	if (avxOption == 0) {
+		SetupVectorFunction_Generic();
+		SetupPCG_GENERIC();
+	}
+	else if (avxOption == 2) {
+		SetupVectorFunction_AVX2();
+		SetupPCG_AVX2();
+	}
+	else if (avxOption == 512) {
+		SetupVectorFunction_AVX512();
+		SetupPCG_AVX512();
+	}
+	else {
+		SetupRoutines_AutoByCPU(1L); // Do not print out
+	} 
+#else
+	//for SOaris system or Win32
+	SetupVectorFunction_Generic();
+	SetupPCG_GENERIC();
+#endif
+
+}
+
+
+//https:// stackoverflow.com/questions/152016/detecting-cpu-architecture-compile-time
+ 
+  const char *getBuild( void ) {
+	  //Get current architecture, detectx nearly every architecture. Coded by Freak
+        #if defined(__x86_64__) || defined(_M_X64)
+        return "x86_64";
+        #elif defined(i386) || defined(__i386__) || defined(__i386) || defined(_M_IX86)
+        return "x86_32";
+        #elif defined(__ARM_ARCH_2__)
+        return "ARM2";
+        #elif defined(__ARM_ARCH_3__) || defined(__ARM_ARCH_3M__)
+        return "ARM3";
+        #elif defined(__ARM_ARCH_4T__) || defined(__TARGET_ARM_4T)
+        return "ARM4T";
+        #elif defined(__ARM_ARCH_5_) || defined(__ARM_ARCH_5E_)
+        return "ARM5"
+        #elif defined(__ARM_ARCH_6T2_) || defined(__ARM_ARCH_6T2_)
+        return "ARM6T2";
+        #elif defined(__ARM_ARCH_6__) || defined(__ARM_ARCH_6J__) || defined(__ARM_ARCH_6K__) || defined(__ARM_ARCH_6Z__) || defined(__ARM_ARCH_6ZK__)
+        return "ARM6";
+        #elif defined(__ARM_ARCH_7__) || defined(__ARM_ARCH_7A__) || defined(__ARM_ARCH_7R__) || defined(__ARM_ARCH_7M__) || defined(__ARM_ARCH_7S__)
+        return "ARM7";
+        #elif defined(__ARM_ARCH_7A__) || defined(__ARM_ARCH_7R__) || defined(__ARM_ARCH_7M__) || defined(__ARM_ARCH_7S__)
+        return "ARM7A";
+        #elif defined(__ARM_ARCH_7R__) || defined(__ARM_ARCH_7M__) || defined(__ARM_ARCH_7S__)
+        return "ARM7R";
+        #elif defined(__ARM_ARCH_7M__)
+        return "ARM7M";
+        #elif defined(__ARM_ARCH_7S__)
+        return "ARM7S";
+        #elif defined(__aarch64__) || defined(_M_ARM64)
+        return "ARM64";
+        #elif defined(mips) || defined(__mips__) || defined(__mips)
+        return "MIPS";
+        #elif defined(__sh__)
+        return "SUPERH";
+        #elif defined(__powerpc) || defined(__powerpc__) || defined(__powerpc64__) || defined(__POWERPC__) || defined(__ppc__) || defined(__PPC__) || defined(_ARCH_PPC)
+        return "POWERPC";
+        #elif defined(__PPC64__) || defined(__ppc64__) || defined(_ARCH_PPC64)
+        return "POWERPC64";
+        #elif defined(__sparc__) || defined(__sparc)
+        return "SPARC";
+        #elif defined(__m68k__)
+        return "M68K";
+        #else
+        return "UNKNOWN";
+        #endif
+ }
+ 
+
+
+
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/abc_common.h` & `Rbeast-0.1.14/ext_src/abc_common.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #pragma once
 
 #include <stdio.h>
 #include "abc_000_macro.h"
+#include "abc_001_config.h"
 #include "abc_mem.h"
 #include "abc_datatype.h"       //#include <inttypes.h>//#include <stdint.h>
 
+char* word_wrap(char* str, int LINE_LENGTH);
+char* word_wrap_indented(char* str, int LINE_LENGTH, int nspace);
 
 extern void    ToUpper(char* s);
 extern void    QuickSortD(F32PTR arr, I32PTR  index, I32 low, I32 high);
 extern void    QuickSortA(F32PTR arr, I32PTR  index, I32 low, I32 high);
 extern I32	   strcicmp(char const * _restrict a, char const * _restrict b);
 extern I32     strcicmp_nfirst(char const* _restrict a, char const* _restrict b, int nfirst);
 extern I32     strmatch(char const* _restrict full, char const* _restrict part);
 extern F32     DeterminePeriod(F32PTR Y, I32 N);
 extern I32     FindChangepoint(F32PTR prob, F32PTR mem, F32 threshold, I32PTR cpt, F32PTR cptCI, I32 N, I32 minSepDist, I32 maxCptNumber);
 
 
-extern void WriteF32ArraryToStrideMEM(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 offset, DATA_TYPE dtype);
-extern void CopyStrideMEMToF32Arr(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset, DATA_TYPE srcDataType);
-extern void WriteStrideMEMToArrMEM(VOID_PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset, DATA_TYPE srcDstDataType);
- 
+extern void SetupRoutines_AutoByCPU(Bool quiet);
+extern void SetupRoutines_UserChoice(int avxOption);
 
 //SUM: IppStatus ippsSum_32f(const Ipp64f* pSrc, int len, Ipp64f* pSum); 
 //r_ippsSum_32f(ptr, N, &mValue, ippAlgHintAccurate);
 //r_ippsMeanStdDev_32f(ptr, N, &mean, &std, ippAlgHintAccurate);
 //ippsSubC_32f_I(Ipp64f val, Ipp64f* pSrcDst, int len);
 //r_ippsSubC_32f_I(mean, ptr, N);
 //IppStatus ippsStdDev_32f(const Ipp64f* pSrc, int len, Ipp64f* pStdDev);
```

### Comparing `Rbeast-0.1.13/ext_src/abc_cpu.c` & `Rbeast-0.1.14/ext_src/abc_cpu.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,112 +1,109 @@
 #include <stdio.h>
 #include <string.h>
-#include "abc_000_warning.h"
 
+#include "abc_000_warning.h"
 
 #include "abc_common.h"
 #include "abc_ide_util.h" // r_printf
 #include "abc_cpu.h"
 
 
-//https://github.com/Mysticial/FeatureDetector
-//https://stackoverflow.com/questions/6121792/how-to-check-if-a-cpu-supports-the-sse3-instruction-set/22521619#22521619
+//https:// github.com/Mysticial/FeatureDetector
+//https:// stackoverflow.com/questions/6121792/how-to-check-if-a-cpu-supports-the-sse3-instruction-set/22521619#22521619
 /*
 Mysticial's answer is a bit dangerous -- it explains how to detect CPU support but not OS support. You need to use _xgetbv to check
 whether the OS has enabled the required CPU extended state. See here for another source. Even gcc
 has made the same mistake. The meat of the code is:
 */
-//https://insufficientlycomplicated.wordpress.com/2011/11/07/detecting-intel-advanced-vector-extensions-avx-in-visual-studio/
+
+//https:// insufficientlycomplicated.wordpress.com/2011/11/07/detecting-intel-advanced-vector-extensions-avx-in-visual-studio/
 /*
     // Checking for AVX requires 3 things:
     // 1) CPUID indicates that the OS uses XSAVE and XRSTORE
     //     instructions (allowing saving YMM registers on context
     //     switch)
     // 2) CPUID indicates support for AVX
     // 3) XGETBV indicates the AVX registers will be saved and
     //     restored on context switch
     //
     // Note that XGETBV is only available on 686 or later CPUs, so
     // the instruction needs to be conditionally run.
 */
+
 #if defined(__x86_64__) || defined(_M_X64) || defined(__i386) || defined(_M_IX86)
     //#if _WIN32 
+
+    /*********************************************/
+    //        WINDOWS
+     /*********************************************/
     #if defined(MSVC_COMPILER) 
 
-        /*********************************************/
-        //        WINDOWS
-        /*********************************************/
+
         #define WIN32_LEAN_AND_MEAN
         #include <Windows.h>
         #include <intrin.h>
 
         #define _XCR_XFEATURE_ENABLED_MASK  0 //t should be already defined in intrinh, but Rtootls stsill compains
 
-        void    cpuid(int32_t out[4], int32_t eax, int32_t ecx) {
-            __cpuidex(out, eax, ecx); 
-        }
-        __int64 xgetbv(unsigned int x)     {
-            return _xgetbv(x);  
-        }
+        void     cpuid(int32_t out[4], int32_t eax, int32_t ecx) {   __cpuidex(out, eax, ecx);      }
+        uint64_t xgetbv(unsigned int x)                          {   return _xgetbv(x);             }
  
         //  Detect 64-bit - Note that this snippet of code for detecting 64-bit has been copied from MSDN.
         typedef BOOL(WINAPI* LPFN_ISWOW64PROCESS) (HANDLE, PBOOL);
-        BOOL IsWow64()  
-        {
-            BOOL bIsWow64 = FALSE;
+        BOOL IsWow64(void)           {
 
+            BOOL                bIsWow64         = FALSE;
             LPFN_ISWOW64PROCESS fnIsWow64Process = (LPFN_ISWOW64PROCESS)GetProcAddress(
                 GetModuleHandle(TEXT("kernel32")), "IsWow64Process");
 
-            if (NULL != fnIsWow64Process)
-            {
-                if (!fnIsWow64Process(GetCurrentProcess(), &bIsWow64))
-                {
+            if (NULL != fnIsWow64Process)       {
+                if (!fnIsWow64Process(GetCurrentProcess(), &bIsWow64))     {
                     r_printf("Error Detecting Operating System.\n");
                     r_printf("Defaulting to 32-bit OS.\n\n");
                     bIsWow64 = FALSE;
                 }
             }
             return bIsWow64;
         }
 
-        int detect_OS_x64() {
+        int detect_OS_x64(void) {
             #ifdef _M_X64
                     return 1;
             #else
                     return IsWow64() != 0;
             #endif
         }
  
+    /*********************************************/
+    //        LINUX
+    /*********************************************/
     #elif defined(__GNUC__) || defined(__clang__)
-    
-        /*********************************************/
-        //        LINUX
-        /*********************************************/
+
         #include <cpuid.h>
         void cpuid(int32_t out[4], int32_t eax, int32_t ecx) {
             __cpuid_count(eax, ecx, out[0], out[1], out[2], out[3]);
         }
         uint64_t xgetbv(unsigned int index) {
             uint32_t eax, edx;
             __asm__ __volatile__("xgetbv" : "=a"(eax), "=d"(edx) : "c"(index));
             return ((uint64_t)edx << 32) | eax;
         }
         #define _XCR_XFEATURE_ENABLED_MASK  0
-        int detect_OS_x64() {
+        int detect_OS_x64(void) {
             //  We only support x64 on Linux.
             return 1;
         }
 
     #elif defined (SOLARIS_OS)
     
-    // cpuid:  https://docs.oracle.com/cd/E23824_01/html/821-1475/cpuid-7d.html
+    // cpuid:  https:// docs.oracle.com/cd/E23824_01/html/821-1475/cpuid-7d.html
 
     // __asm and __asm__ are synonoous for Solaris CC
-    // https://docs.oracle.com/cd/E26502_01/html/E28387/gmacx.html#scrolltoc
+    // https:// docs.oracle.com/cd/E26502_01/html/E28387/gmacx.html#scrolltoc
     // Oracle® Solaris Studio 12.4: C User'sGuide
 
    //
         #define __cpuid(level, a, b, c, d)                                             \
           __asm__("cpuid\n\t" : "=a"(a), "=b"(b), "=c"(c), "=d"(d) : "0"(level))
 
         #define __cpuid_count(level, count, a, b, c, d)                                \
@@ -120,100 +117,102 @@
         #define _XCR_XFEATURE_ENABLED_MASK  0
         uint64_t xgetbv(unsigned int index) {
             uint32_t eax, edx;
             __asm__ ("xgetbv" : "=a"(eax), "=d"(edx) : "c"(index));
             return ((uint64_t)edx << 32) | eax;
         }
 
-        int detect_OS_x64() {
+        int detect_OS_x64(void) {
             //  We only support x64 on Linux.
             return 1;
         }
         #warning "Warning:No cpuid intrinsic defined for compiler."
     #else
         #define _XCR_XFEATURE_ENABLED_MASK  0
         void cpuid(int32_t out[4], int32_t eax, int32_t ecx) {
             out[0]=out[1]=out[2]= out[3]=0;
         }
  
         uint64_t xgetbv(unsigned int index) {            
             return 0;
         }
-        int detect_OS_x64() {
+        int detect_OS_x64(void) {
             //  We only support x64 on Linux.
             return 1;
         }
         //#error  "No cpuid intrinsic defined for compiler."
         #warning "No cpuid intrinsic defined for compiler: a placeholder created!"
     #endif
-#elif defined(ARM64_OS)
+#elif defined(ARM64_OS) || defined (POWERPC_OS)
         //https://stackoverflow.com/questions/60588765/how-to-get-cpu-brand-information-in-arm64
         //https://stackoverflow.com/questions/23934862/what-predefined-macro-can-i-use-to-detect-the-target-architecture-in-clang
         #define _XCR_XFEATURE_ENABLED_MASK  0
         void cpuid(int32_t out[4], int32_t eax, int32_t ecx) {
             out[0] = out[1] = out[2] = out[3] = 0;
         }
 
         uint64_t xgetbv(unsigned int index) {
             return 0;
         }
-        int detect_OS_x64() {
+        int detect_OS_x64(void) {
             //  We only support x64 on Linux.
             return 1;
         }
        // #warning "No cpuid intrinsic defined for ARM64: a placeholder created!"
+
+// https://stackoverflow.com/questions/34488604/equivalent-for-sse-in-power-pc
+// There is no SSE/AVX for POWEPC,Altivec is the POWERPC alternatives
 #else
 #   error "No cpuid intrinsic defined for processor architecture."
 #endif
 
  
  
 static void cpu_print(const char* label, uint8_t yes) {
     r_printf("%s%s\n", label, (yes ? "Yes" : "No"));
 }
  
  
-uint8_t detect_OS_AVX(){
+uint8_t detect_OS_AVX(void){
     //  Copied from: http://stackoverflow.com/a/22521619/922184
 
-    bool avxSupported = false;
+    Bool avxSupported = _False_;
 
     int  cpuInfo[4];
     cpuid(cpuInfo, 1, 0);
 
-    bool osUsesXSAVE_XRSTORE = (cpuInfo[2] & (1 << 27)) != 0;
-    bool cpuAVXSuport        = (cpuInfo[2] & (1 << 28)) != 0;
+    Bool osUsesXSAVE_XRSTORE = (cpuInfo[2] & (1 << 27)) != 0;
+    Bool cpuAVXSuport        = (cpuInfo[2] & (1 << 28)) != 0;
 
-    if (osUsesXSAVE_XRSTORE && cpuAVXSuport)
-    {
+    if (osUsesXSAVE_XRSTORE && cpuAVXSuport)   {
         uint64_t xcrFeatureMask = xgetbv(_XCR_XFEATURE_ENABLED_MASK);
         avxSupported = (xcrFeatureMask & 0x6) == 0x6;
     }
 
     return avxSupported;
 }
-bool detect_OS_AVX512(){
+Bool detect_OS_AVX512(void){
     if (!detect_OS_AVX())
-        return false;
+        return _False_;
 
     uint64_t xcrFeatureMask = xgetbv(_XCR_XFEATURE_ENABLED_MASK);
     return (xcrFeatureMask & 0xe6) == 0xe6;
 }
 void get_vendor_string(char * name){
     int32_t CPUInfo[4];
     //char name[13];
 
     cpuid(CPUInfo, 0, 0);
     memcpy(name + 0, &CPUInfo[1], 4);
     memcpy(name + 4, &CPUInfo[3], 4);
     memcpy(name + 8, &CPUInfo[2], 4);
     name[12] = '\0';
 }
-////////////////////////////////////////////////////////////////////////////////
-////////////////////////////////////////////////////////////////////////////////
+
+
 ////////////////////////////////////////////////////////////////////////////////
 ////////////////////////////////////////////////////////////////////////////////
 void detect_host(struct cpu_x86 *cpu){
 
     memset(cpu, 0, sizeof(struct cpu_x86));
 
     //  OS Features
@@ -221,27 +220,28 @@
     cpu->OS_AVX    = detect_OS_AVX();
     cpu->OS_AVX512 = detect_OS_AVX512();
 
     //  Vendor
     char vendor[13];
     get_vendor_string(vendor);
     if (strcmp(vendor,"GenuineIntel") ==0){
-        cpu->Vendor_Intel = true;
+        cpu->Vendor_Intel = _True_;
     }else if (strcmp(vendor, "AuthenticAMD") ==0){
-        cpu->Vendor_AMD = true;
+        cpu->Vendor_AMD = _True_;
     }
 
     int info[4];
     cpuid(info, 0, 0);
     int nIds = info[0];
 
     cpuid(info, 0x80000000, 0);
     uint32_t nExIds = info[0];
 
-    r_printf("%d\n",nIds);
+    // r_printf("%d\n",nIds);
+
     //  Detect Features
     if (nIds >= 0x00000001){
         cpuid(info, 0x00000001, 0);
         cpu->HW_MMX    = (info[3] & ((uint32_t)1 << 23)) != 0;
         cpu->HW_SSE    = (info[3] & ((uint32_t)1 << 25)) != 0;
         cpu->HW_SSE2   = (info[3] & ((uint32_t)1 << 26)) != 0;
         cpu->HW_SSE3   = (info[2] & ((uint32_t)1 <<  0)) != 0;
@@ -303,15 +303,16 @@
         cpu->HW_x64   = (info[3] & ((int)1 << 29)) != 0;
         cpu->HW_ABM   = (info[2] & ((int)1 <<  5)) != 0;
         cpu->HW_SSE4a = (info[2] & ((int)1 <<  6)) != 0;
         cpu->HW_FMA4  = (info[2] & ((int)1 << 16)) != 0;
         cpu->HW_XOP   = (info[2] & ((int)1 << 11)) != 0;
     }
 }
-void printinfo(struct cpu_x86 *cpu) {
+
+void print_cpuinfo(struct cpu_x86 *cpu) {
     r_printf("CPU Vendor:\n");
     cpu_print("    AMD         = ", cpu->Vendor_AMD);
     cpu_print("    Intel       = ", cpu->Vendor_Intel);
     r_printf(" \n");
  
     r_printf("OS Features:\n");
 #ifdef _WIN32
@@ -378,24 +379,22 @@
  
 
     r_printf("\nSummary\n");
     cpu_print("    Safe to use AVX:     ", cpu->HW_AVX && cpu->OS_AVX);
     cpu_print("    Safe to use AVX512:  ", cpu->HW_AVX512_F && cpu->OS_AVX512);
     r_printf("\n");
 }
-void cpu_print_info(){
+
+void detect_print_cpu(void) {
     struct cpu_x86 cpuinfo;
      detect_host(&cpuinfo);
-     printinfo(&cpuinfo);
+     print_cpuinfo(&cpuinfo);
 }
 
-#undef bool
  
-
-
 //https://stackoverflow.com/questions/12594208/c-program-to-determine-levels-size-of-cache
 /*
 To get L2 and L3 cache sizes, you need to use CPUID with EAX=4, and set ECX to 0, 1, 2, ... for
 each caching level. The linked code shows this, and Intel's docs have details on which bits mean 
 what.
 */
 
@@ -403,17 +402,17 @@
 When eax = 4 and ecx is the cache level,
 Ways = EBX[31:22]
 Partitions = EBX[21:12]
 LineSize = EBX[11:0]
 Sets = ECX
 Total Size = (Ways + 1) * (Partitions + 1) * (Line_Size + 1) * (Sets + 1)
 */
-void i386_cpuid_caches () {
-    int i;
-    for (i = 0; i < 32; i++) {
+void i386_cpuid_caches (Bool quiet) {
+ 
+    for (int i = 0; i < 32; i++) {
 
         // Variables to hold the contents of the 4 i386 legacy registers
         uint32_t eax, ebx, ecx, edx; 
 
         eax = 4; // get cache info
         ecx = i; // cache id
 
@@ -436,15 +435,15 @@
             edx = out[3];
 
         #endif
 
         // See the page 3-191 of the manual.
         int cache_type = eax & 0x1F; 
 
-        if (cache_type == 0) // end of valid cache identifiers
+        if (cache_type == 0) // CODE_EOF of valid cache identifiers
             break;
 
         char * cache_type_string;
         switch (cache_type) {
             case 1: cache_type_string = "Data Cache"; break;
             case 2: cache_type_string = "Instruction Cache"; break;
             case 3: cache_type_string = "Unified Cache"; break;
@@ -462,34 +461,35 @@
         unsigned int cache_coherency_line_size = (ebx & 0xFFF) + 1;
         unsigned int cache_physical_line_partitions = ((ebx >>= 12) & 0x3FF) + 1;
         unsigned int cache_ways_of_associativity = ((ebx >>= 10) & 0x3FF) + 1;
 
         // Total cache size is the product
         size_t cache_total_size = cache_ways_of_associativity * cache_physical_line_partitions * cache_coherency_line_size * cache_sets;
 
-        r_printf(
-            "Cache ID %d:\n"
-            "- Level: %d\n"
-            "- Type: %s\n"
-            "- Sets: %d\n"
-            "- System Coherency Line Size: %d bytes\n"
-            "- Physical Line partitions: %d\n"
-            "- Ways of associativity: %d\n"
-            "- Total Size: %zu bytes (%zu kb)\n"
-            "- Is fully associative: %s\n"
-            "- Is Self Initializing: %s\n"
-            "\n"
-            , i
-            , cache_level
-            , cache_type_string
-            , cache_sets
-            , cache_coherency_line_size
-            , cache_physical_line_partitions
-            , cache_ways_of_associativity
-            , cache_total_size, cache_total_size >> 10
-            , cache_is_fully_associative ? "true" : "false"
-            , cache_is_self_initializing ? "true" : "false"
-        );
+        if (!quiet)
+            r_printf(
+                "Cache ID %d:\n"
+                "- Level: %d\n"
+                "- Type: %s\n"
+                "- Sets: %d\n"
+                "- System Coherency Line Size: %d bytes\n"
+                "- Physical Line partitions: %d\n"
+                "- Ways of associativity: %d\n"
+                "- Total Size: %zu bytes (%zu kb)\n"
+                "- Is fully associative: %s\n"
+                "- Is Self Initializing: %s\n"
+                "\n"
+                , i
+                , cache_level
+                , cache_type_string
+                , cache_sets
+                , cache_coherency_line_size
+                , cache_physical_line_partitions
+                , cache_ways_of_associativity
+                , cache_total_size, cache_total_size >> 10
+                , cache_is_fully_associative ? "true" : "false"
+                , cache_is_self_initializing ? "true" : "false"
+            );
     }
 }
 
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/abc_dir.c` & `Rbeast-0.1.14/ext_src/abc_dir.c`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,17 @@
 		char  fullpath[1000];
 		strcpy(fullpath, path);
 		strcat(fullpath, "/");
 		strcat(fullpath, dp->d_name);
 
 		// stackoverflow.com/questions/22886290/c-get-all-files-with-certain-extension
 		if (dp->d_type == DT_REG /*DT_DIR*/) {
-			char * const ext = strrchr(dp->d_name, '.');
-			if (ext != NULL && ext != dp->d_name)
-			{
-				if (strcmp(ext, ".tif") == 0){
+			char * const pext = strrchr(dp->d_name, '.');
+			if (pext != NULL && pext != dp->d_name)		{
+				if (strcmp(pext, ".tif") == 0){
 					r_printf("%s\n", dp->d_name);
 				}				
 			}
 		}
 
 		/*
 		struct stat s;
@@ -69,15 +68,15 @@
 	  // stackoverflow.com/questions/22886290/c-get-all-files-with-certain-extension
 		if (dp->d_type == DT_REG /*DT_DIR*/) {
 			char * const pEXT = strrchr(dp->d_name, '.');
 			if (pEXT != NULL && pEXT != dp->d_name)
 			{
 				if (stricmp(pEXT+1, ext) == 0){
 					fNum++;
-					memSize += strlen(dp->d_name)+ 1L;
+					memSize += (int)strlen(dp->d_name)+ 1L;
 				}
 			}
 		}
 
 		/*
 		struct stat s;
 		if (stat(fullpath, &s) == 0)
@@ -106,15 +105,15 @@
 	while ((dp = readdir(dir)) != NULL) {
 		// stackoverflow.com/questions/22886290/c-get-all-files-with-certain-extension
 		if (dp->d_type == DT_REG /*DT_DIR*/) {
 			char * const pEXT = strrchr(dp->d_name, '.');
 			if (pEXT != NULL && pEXT != dp->d_name)
 			{
 				if (stricmp(pEXT+1, ext) == 0){
-					int size = strlen(dp->d_name);
+					int size = (int)strlen(dp->d_name);
 					flist->offset[fNum] =  ptr; //-Wint-conversion
 					memcpy(ptr, dp->d_name, size);
 					ptr[size] = 0;
 
 					fNum++;
 					ptr += (size + 1);
 				}
```

### Comparing `Rbeast-0.1.13/ext_src/abc_dirent.h` & `Rbeast-0.1.14/ext_src/abc_dirent.h`

 * *Files 1% similar despite different names*

```diff
@@ -292,18 +292,16 @@
 /* Dirent functions */
 static DIR *opendir (const char *dirname);
 static _WDIR *_wopendir (const wchar_t *dirname);
 
 static struct dirent *readdir (DIR *dirp);
 static struct _wdirent *_wreaddir (_WDIR *dirp);
 
-static int readdir_r(
-    DIR *dirp, struct dirent *entry, struct dirent **result);
-static int _wreaddir_r(
-    _WDIR *dirp, struct _wdirent *entry, struct _wdirent **result);
+static struct dirent*  readdir_r(    DIR *dirp, struct dirent *entry, int *result);
+static int _wreaddir_r(   _WDIR *dirp, struct _wdirent *entry, struct _wdirent **result);
 
 static int closedir (DIR *dirp);
 static int _wclosedir (_WDIR *dirp);
 
 static void rewinddir (DIR* dirp);
 static void _wrewinddir (_WDIR* dirp);
 
@@ -671,17 +669,15 @@
 
     return p;
 }
 
 /*
  * Open directory stream using plain old C-string.
  */
-static DIR*
-opendir(
-    const char *dirname)
+static DIR* opendir( const char *dirname)
 {
     struct DIR *dirp;
 
     /* Must have directory name */
     if (dirname == NULL  ||  dirname[0] == '\0') {
         dirent_set_errno (ENOENT);
         return NULL;
@@ -727,42 +723,43 @@
     free (dirp);
     return NULL;
 }
 
 /*
  * Read next directory entry.
  */
-static struct dirent*
-readdir(
-    DIR *dirp)
+static struct dirent* readdir(   DIR *dirp)
 {
-    struct dirent *entry;
+ 
 
     /*
      * Read directory entry to buffer.  We can safely ignore the return value
      * as entry will be set to NULL in case of error.
      */
-    (void) readdir_r (dirp, &dirp->ent, &entry);
+    int result;
+    struct dirent* entry = readdir_r (dirp, &dirp->ent, &result);
 
     /* Return pointer to statically allocated directory entry */
     return entry;
 }
 
 /*
  * Read next directory entry into called-allocated buffer.
  *
  * Returns zero on success.  If the end of directory stream is reached, then
  * sets result to NULL and returns zero.
  */
-static int
+static   struct dirent*
 readdir_r(
     DIR *dirp,
     struct dirent *entry,
-    struct dirent **result)
+    int *status)
 {
+    struct dirent* result;
+
     WIN32_FIND_DATAW *datap;
 
     /* Read next directory entry */
     datap = dirent_next (dirp->wdirp);
     if (datap) {
         size_t n;
         int error;
@@ -823,32 +820,33 @@
             entry->d_ino = 0;
             entry->d_off = -1;
             entry->d_reclen = 0;
 
         }
 
         /* Return pointer to directory entry */
-        *result = entry;
+        result = entry;
 
     } else {
 
         /* No more directory entries */
-        *result = NULL;
+        result = NULL;
 
     }
 
+    status[0] = 0; /*OK*/
+    return result;
+
     return /*OK*/0;
 }
 
 /*
  * Close directory stream.
  */
-static int
-closedir(
-    DIR *dirp)
+static int closedir(    DIR *dirp)
 {
     int ok;
     if (dirp) {
 
         /* Close wide-character directory stream */
         ok = _wclosedir (dirp->wdirp);
         dirp->wdirp = NULL;
@@ -865,27 +863,24 @@
     }
     return ok;
 }
 
 /*
  * Rewind directory stream to beginning.
  */
-static void
-rewinddir(
-    DIR* dirp)
+static void rewinddir( DIR* dirp)
 {
     /* Rewind wide-character string directory stream */
     _wrewinddir (dirp->wdirp);
 }
 
 /*
  * Scan directory for entries.
  */
-static int
-scandir(
+static int scandir(
     const char *dirname,
     struct dirent ***namelist,
     int (*filter)(const struct dirent*),
     int (*compare)(const struct dirent**, const struct dirent**))
 {
     struct dirent **files = NULL;
     size_t size = 0;
@@ -939,15 +934,17 @@
                     /* Cannot allocate temporary directory entry */
                     result = -1;
                     break;
                 }
             }
 
             /* Read directory entry to temporary area */
-            if (readdir_r (dir, tmp, &entry) == /*OK*/0) {
+            int status;
+            entry = readdir_r(dir, tmp, &status);
+            if (status == /*OK*/0) {
 
                 /* Did we get an entry? */
                 if (entry != NULL) {
                     int pass;
 
                     /* Determine whether to include the entry in result */
                     if (filter) {
```

### Comparing `Rbeast-0.1.13/ext_src/abc_ide_util_R.c` & `Rbeast-0.1.14/ext_src/abc_ide_util_R.c`

 * *Files 7% similar despite different names*

```diff
@@ -11,32 +11,38 @@
 // fflush(stdout);   //: c function: fflush(stdout)--flush the line buffer to see immediate outputs
 // R_FlushConsole(); 
 // Rf_GetOption
 
 
 #if R_INTERFACE == 1
 
+
+int  JDN_to_DateNum(int jdn) {
+	return jdn - 2440588;
+}
+
+
 SEXP getListElement(SEXP list, const char* str) {
 
 	SEXP elmt = NULL; // R_NilValue;
 	SEXP names = getAttrib(list, R_NamesSymbol);
-	for (int i = 0; i < length(list); i++)
+	for (int i = 0; i < length(names); i++)
 		if (strcmp(CHAR(STRING_ELT(names, i)), str) == 0) {
 			elmt = VECTOR_ELT(list, i);
 			break;
 		}
 	return elmt;
 }
 
 
 SEXP getListElement_CaseIn(SEXP list, const char* str)
 {
 	SEXP elmt = NULL; // R_NilValue;
-	SEXP names = getAttrib(list, R_NamesSymbol);
-	for (int i = 0; i < length(list); i++)
+	SEXP names = getAttrib(list, R_NamesSymbol); 
+	for (int i = 0; i < length(names); i++)
 		if (strcicmp(CHAR(STRING_ELT(names, i)), str) == 0) {
 			elmt = VECTOR_ELT(list, i);
 			break;
 		}
 	return elmt;
 }
 
@@ -71,43 +77,54 @@
 int IsNumeric(void* ptr) { return isNumeric((SEXP)ptr); }
 int IsDouble(void* ptr)  { return TYPEOF((SEXP)ptr) == REALSXP; }
 int IsSingle(void* ptr)  { return 0; }
 int IsInt32(void* ptr)   { return TYPEOF((SEXP)ptr) == INTSXP;  }
 int IsInt16(void* ptr)   { return 0; }
 int IsInt64(void* ptr)   { return 0; }
 //http://adv-r.had.co.nz/C-interface.html
-int IsLogical(void* ptr) { return TYPEOF((SEXP)ptr) == LGLSXP; };
+int IsLogical(void* ptr) { return TYPEOF((SEXP)ptr) == LGLSXP; }
 
-VOID_PTR GetFieldByIdx(VOID_PTR strucVar, I32 ind) { 
-	return VECTOR_ELT(strucVar, ind); 
+VOID_PTR GetFieldByIdx(VOID_PTR strucVar, I32 ind0) { 
+	return VECTOR_ELT(strucVar, ind0); 
 }
 
+void GetFieldNameByIdx(VOID_PTR strucVar, I32 ind0, char* str, int buflen) {
+ 
+	SEXP names = getAttrib(strucVar, R_NamesSymbol);
+	int  n     = length(names);
+	if (ind0 < n) {
+		const char* name = CHAR(STRING_ELT(names, ind0));
+		strncpy(str, name, buflen);
+		str[buflen - 1] = 0;
+	}	else {
+		str[0] = 0;
+	}
+ 	
+}
 
 I32 GetCharArray(void *ptr, char * dst, int n) {
-
-	if (TYPEOF((SEXP)ptr) != STRSXP) {
+	dst[0] = 0;
+	if (ptr==NULL || TYPEOF((SEXP)ptr) != STRSXP) {
 		return 0;
 	}
 
-	char* tmpstr;
-	tmpstr = CHAR(STRING_ELT(ptr, 0));
+	const char* tmpstr= CHAR(STRING_ELT(ptr, 0));
 	strncpy(dst, tmpstr, n);
 	dst[n] = 0;
 	return (I32) strlen(dst);
 	
 }
 
 I32 GetCharVecElem(void* ptr, int idx, char* dst, int n) {
 
 	if (TYPEOF((SEXP)ptr) != STRSXP) {
 		return 0;
 	}
 
-	char* tmpstr;
-	tmpstr = CHAR(STRING_ELT((SEXP)ptr, idx));
+	const char* tmpstr = CHAR(STRING_ELT((SEXP)ptr, idx));
 	strncpy(dst, tmpstr, n);
 	dst[n] = 0;
 	return (I32)strlen(dst);
 }
 
 I32  GetNumberOfFields(const void* structVar) { 
 	return Rf_length (structVar); 
@@ -128,16 +145,16 @@
 
 void* GetField123(const void* structVar, char* fname, int nPartial) {
 
 	if (!structVar) return NULL;
 
 	void* elem = (void*)getListElement_CaseIn(structVar, fname);
 	if (elem == NULL) {	 
-		SEXP names = getAttrib(structVar, R_NamesSymbol);
-		for (int i = 0; i < length(structVar); i++)
+		SEXP names = getAttrib(structVar, R_NamesSymbol); // names may be NULL
+		for (int i = 0; i < length(names); i++)
 			if (strcicmp_nfirst(CHAR(STRING_ELT(names, i)), fname,nPartial) == 0) {
 				elem = VECTOR_ELT(structVar, i);
 				break;
 			} 
 	}
 	return elem;
 }
@@ -193,14 +210,28 @@
 	SEXP DIMS = PROTECT(getAttrib((SEXP)ptr, R_DimSymbol));
 	for (int i = 0; i < N; i++)
 	{
 		dims[i] = INTEGER(DIMS)[i];
 	}
 	UNPROTECT(1);
 }
+void * SetDimensions(const void* ptr, int dims[], int ndims) {
+	
+	if (!ptr) return NULL;
+
+	SEXP  tmp = PROTECT(allocVector(INTSXP, ndims));	
+	for (int i = 0; i < ndims; i++) 	{
+		INTEGER(tmp)[i] = dims[i];
+	}
+	setAttrib(ptr, R_DimSymbol, tmp);
+	UNPROTECT(1);
+
+	return ptr;
+}
+
 
 int GetNumberOfElements(const void * ptr) {	
 	return Rf_length((SEXP)ptr);
 }
 
 
 void *CreateNumVar(DATA_TYPE dtype, int *dims, int ndims, VOIDPTR * data_ptr) {
@@ -353,14 +384,17 @@
 
 void ReplaceStructField(VOIDPTR s, char* fname, VOIDPTR newvalue){
 
 	int index= __GetFieldIndex(s,fname);
 	if (index <0) {
 		return;
 	}
+
+	
+	// no need to porect old value; we want to let it get destoried
 	SEXP oldvalue = VECTOR_ELT(s, index);
 
 	SET_VECTOR_ELT(s, index, newvalue);
 }
 
 void  DestoryStructVar(VOID_PTR strutVar) {
 
@@ -428,15 +462,15 @@
 			R_ReadConsole = GetProcAddress(hinstLib, "R_ReadConsole");
 			FreeLibrary(hinstLib);
 			//r_printf("%#010x\n", R_ReadConsole);
 		}
 
 		/*		
 		char s[10];
-		while (stricmp(s, "exit")!=0) {	R_ReadConsole("", s, 1, 0);	s[4] = 0;	}		
+		while (strcicmp(s, "exit")!=0) {	R_ReadConsole("", s, 1, 0);	s[4] = 0;	}		
 		*/
 		return R_ReadConsole;
 	}
 
 
 	 void* GetR_interrupts_pending(void) {
 		char* RHOME = get_R_HOME();
@@ -450,29 +484,29 @@
 		void * R_interrupts_pending = GetProcAddress(hinstLib, "R_interrupts_pending");
 		FreeLibrary(hinstLib);
 
 		return R_interrupts_pending;
 	}
 
 
-	bool GetUserInput(void * nullPtr)
+	 Bool GetUserInput(void * nullPtr)
 	{
 		int (*R_ReadConsole)(const char *prompt, unsigned char *buf, int len, int addtohistory);
 		R_ReadConsole = GetReadConsole();
 		char str[100];
 		str[0]=0;
 
-		while (stricmp(str, "exit") != 0) {
+		while (strcicmp(str, "exit") != 0) {
 			R_ReadConsole("", str, 10, 0);
 			str[4] = 0;
 		}
 		r_printf("Program is forcely terminated ...");
 		IDE_USER_INTERRUPT = 1L;
 	}
 #endif
 
 #else
 
-const static achar = 'a';
+const static char achar = 'a';
 #endif
 
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/abc_ide_util_matlab.c` & `Rbeast-0.1.14/ext_src/abc_ide_util_matlab.c`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 #include "assert.h"
 #include "abc_000_warning.h"
 
 #include "abc_ide_util.h"
 #include "abc_common.h"
 #include "abc_date.h"
 
-#if M_INTERFACE==1
+#if M_INTERFACE==1  
+
+
+int  JDN_to_DateNum(int jdn) {
+	return jdn - 1721059;
+}
 
 I32 GetConsoleWidth() {
 	mxArray *pOut[1], *pIn[2];
 	pIn[0] = mxCreateDoubleScalar(0);
 	pIn[1] = mxCreateString("CommandWindowSize");
 	mexCallMATLAB(1, pOut, 2, pIn, "get");
 	F64 *ptr = mxGetData(pOut[0]);
@@ -22,14 +27,17 @@
 	return screenWidth;
 }
 
 int IsClass(void* ptr, char* class) { return 0; }
 
 int IsCell(void* ptr) { return mxIsCell(ptr); }
 int IsChar(void* ptr)    { 
+
+	if (ptr == NULL) return 0;
+
 	if (IsCell(ptr)) {
 		// if ptr is a cell, iterate through all elements and return 1L if all the elems are char.
 		int n = GetNumberOfElements(ptr);
 		for (int i = 0; i < n; ++i) {
 			void *tmp = mxGetCell(ptr, i);
 			if ( !mxIsChar(tmp) && !mxIsClass(tmp, "string")) return 0; 
 		}
@@ -44,31 +52,47 @@
 int IsStruct(void* ptr)  { return mxIsStruct(ptr) ||  mxIsEmpty(ptr); } // We simply treat an empty mxArray as a struct, though matlab treats it as numeric
 int IsNumeric(void* ptr) { return mxIsNumeric(ptr) && !mxIsEmpty(ptr); } // Matlab treates an empty as Numeric
 int IsDouble(void* ptr)  { return mxIsDouble(ptr); }
 int IsSingle(void* ptr)  { return mxIsSingle(ptr); }
 int IsInt32(void* ptr)   { return mxIsInt32(ptr); }
 int IsInt16(void* ptr) { return mxIsInt16(ptr); }
 int IsInt64(void* ptr) { return mxIsInt64(ptr); }
+//int IsInt08(void* ptr) { return mxIsInt8(ptr); }
 int IsLogical(void* ptr) { return mxIsLogical(ptr); }
 
 VOID_PTR GetFieldByIdx(VOID_PTR ptr, I32 ind) {
 
 	//https://www.mathworks.com/help/matlab/apiref/mxgetfieldbynumber.html
 	if (IsCell(ptr)) {
 		return  mxGetCell(ptr, ind);
 	}
 	if (IsStruct(ptr)) {
-		mxGetFieldByNumber(ptr, 0, ind);
+		return mxGetFieldByNumber(ptr, 0, ind);
 	}
 	return NULL;
 }
- 
+
+void GetFieldNameByIdx(VOID_PTR strucVar, I32 ind0, char *str, int buflen) {
+	I32 numFlds   = mxGetNumberOfFields(strucVar); 
+	if (ind0 < numFlds) {
+		char* name = mxGetFieldNameByNumber(strucVar, ind0);
+		strncpy(str, name, buflen);
+		str[buflen - 1] = 0;
+	}	else {
+		str[0] = 0;
+	}
+	
+}
+
 I32 GetCharArray(void* ptr, char* dst,   int n) {
+	dst[0] = 0;
 	//Dsr needs to be at least of length (n+1);
-
+	if (ptr == NULL) {
+		return 0;
+	}
 	int len = 0;
 	if (mxIsChar(ptr)){		
 		// This func allocates new mem for tmp, which needs to be explicitlly dellocated later
 		//http://www.ece.northwestern.edu/local-apps/matlabhelp/techdoc/apiref/mxarraytostring.html#976726
 		char* tmp = mxArrayToString(ptr);
 		strncpy(dst, tmp, n); dst[n] = 0;	len  = strlen(dst);
 		r_free(tmp);
@@ -93,26 +117,32 @@
 
 			strncpy(dst, tmp, n); dst[n] = 0;	len = strlen(dst);
 			r_free(tmp);
 			return len;			
 		}
 	}
 	else {
+		dst[0] = 0;
 		return 0L;
 	}
 	
 }
 
 I32 GetCharVecElem(void* ptr, int idx, char* dst, int n) {
 	//Dsr needs to be at least of length (n+1);
 
 	int len = 0;
 
 	if (IsCell(ptr) ) {
-		
+		int  nelem = mxGetNumberOfElements(ptr);
+		if (idx >= nelem) {
+			dst[0] = 0;
+			return 0;
+		}
+
 		void* elem = mxGetCell(ptr, idx);
 
 		if (mxIsChar(elem)) {
 
 			// This func allocates new mem for tmp, which needs to be explicitlly dellocated later
 			// www.ece.northwestern.edu/local-apps/matlabhelp/techdoc/apiref/mxarraytostring.html#976726
 			char* tmp = mxArrayToString(elem);
@@ -140,18 +170,51 @@
 
 				strncpy(dst, tmp, n); dst[n] = 0;	len = strlen(dst);
 				r_free(tmp);
 				return len;
 			}
 		}
 		else {
+			dst[0] = 0;
 			return 0L;
 		}
 
 	}
+	else if (mxIsChar(ptr)) {
+		int            ndims = mxGetNumberOfDimensions(ptr);
+		const mwSize*  dims  = mxGetDimensions(ptr);
+		if (idx >= dims[0] || ndims > 2) {
+			dst[0] = 0;
+			return 0;
+		}
+		else {
+			int    cols = dims[1];
+			int    rows = dims[0];
+			//MATLAB uses 16-bit unsigned integer character encoding for Unicode® characters.
+			mwSize   newdims[2] = {1,cols };
+			mxArray* newrow     = mxCreateCharArray(2, newdims);
+			
+			mxChar* newpos = mxGetChars(newrow);
+			mxChar* oldpos = mxGetChars(ptr) + idx;
+			for (int i = 0; i < cols; i++) {
+				newpos[i] = *oldpos;
+				oldpos   += rows;
+			}			
+
+			char* tmp = mxArrayToString(newrow);
+			strncpy(dst, tmp, n); dst[n] = 0;
+			len = strlen(dst);
+			r_free(tmp);
+
+			mxDestroyArray(newrow);
+
+			return len;
+		}
+
+	}
 	else if (mxIsClass(ptr, "string") && !IsCell(ptr)) {
 
 		//["a","b","c"...]
 
 		void* elem = (void**)mxGetData(ptr) + idx;
 
 		//www.mathworks.com/matlabcentral/answers/330929-how-to-access-matlab-string-data-in-mex-c
@@ -171,15 +234,17 @@
 			mxDestroyArray(char_array[0]);
 
 			strncpy(dst, tmp, n); dst[n] = 0;	len = strlen(dst);
 			r_free(tmp);
 			return len;
 		}
 	}
+
 	else {
+		dst[0] = 0;
 		return 0L;
 	}
 
 }
 
 I32  GetNumberOfFields(const void* structVar) {
 	return mxGetNumberOfFields(structVar); 
@@ -231,25 +296,40 @@
 
 F64    GetScalar(const void * ptr) { return mxGetScalar((mxArray *)ptr); }
 void * GetData(const void * ptr) {   return mxGetData((mxArray *)ptr); }
 int    GetDim1(const void * ptr) {   return mxGetM((mxArray *)ptr); }
 int    GetDim2(const void * ptr) {   return mxGetN((mxArray *)ptr); }
 int    GetNumOfDim(const void * ptr) { return mxGetNumberOfDimensions((mxArray *)ptr); }
 void   GetDimensions(const void * ptr, int dims[], int ndims) {
-	int N = min(ndims, GetNumOfDim(ptr) );
-	const mwSize *dimArr = mxGetDimensions((mxArray *)ptr);
-	for (int i = 0; i < N; i++)
-	{
-		dims[i] = dimArr[i];
+	int   N            = min(ndims, GetNumOfDim(ptr) );
+	const mwSize *mxdims = mxGetDimensions((mxArray *)ptr);
+	for (int i = 0; i < N; i++) 	{
+		dims[i] = mxdims[i];
 	}	
 }
 
+void  * SetDimensions(const void* ptr, int dims[], int ndims) {
+	if (!ptr) return NULL;
+	mwSize mwdims[20];
+	for (int i = 0; i < ndims; i++) mwdims[i] = dims[i];
+	mwSize ndimension = ndims;
+	int res=mxSetDimensions(ptr, mwdims, ndimension);
+	mwSize* p = mxGetDimensions(ptr);
+	return ptr;
+}
+
 int    GetNumberOfElements(const void * ptr)
 { // Do not work for a vector of opaque objects for some reason 
-	return mxGetNumberOfElements(ptr);
+	if (mxIsChar(ptr)) {
+		// Suppose it is a 2d mxCharArray
+		const mwSize* dims = mxGetDimensions((mxArray*)ptr);
+		return dims[0]; 		
+	} else {
+		return mxGetNumberOfElements(ptr);
+	}	
 }
 
 void* CreateNumVar(DATA_TYPE dtype, int* dims, int ndims, VOIDPTR* data_ptr) {
 
 		// Not a struct variable to be created
 		mxClassID fieldDataType;
 		switch (dtype)	{
@@ -319,14 +399,22 @@
 
 		mxSetField(out, 0L, fieldList[i].name, newFldPtr);		
 	}
 
 	return (void*)out;
 }
 
+void ReplaceStructField(VOIDPTR s, char* fname, VOIDPTR newvalue){
+
+	mxArray *fld= mxGetField(s, 0, fname);
+	if (fld != NULL) {
+		mxDestroyArray(fld);
+	}
+	mxSetField(s, 0, fname, newvalue);
+}
 //https://www.mathworks.com/help/matlab/apiref/mxdestroyarray.html
 void  DestoryStructVar(VOID_PTR strutVar) {
 		mxDestroyArray(strutVar);
 }
 
 void AddStringAttribute(VOID_PTR listVar, const char* field, const char* value) {
 
@@ -349,20 +437,25 @@
 	 
 }
 
 
 //https://stackoverflow.com/questions/25998442/mex-options-when-compiling-with-visual-studio
 //https://undocumentedmatlab.com/articles/mex-ctrl-c-interrupt
 // The following 2 function are exported from libut.lib
-bool utIsInterruptPending();
-void utSetInterruptPending(bool);
+Bool utIsInterruptPending();
+void utSetInterruptPending(Bool);
 
+#ifndef O_INTERFACE
 I32  CheckInterrupt()         { return utIsInterruptPending(); }
-void ConsumeInterruptSignal() { utSetInterruptPending(false); }
+void ConsumeInterruptSignal() { utSetInterruptPending(_False_); }
+#else
+I32  CheckInterrupt() { return 0; }
+void ConsumeInterruptSignal() { ; }
+#endif
 
 #else
-const static achar = 'a';
+const static char achar = 'a';
 #endif
 
 
 
 #include "abc_000_warning.h"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+iso-8859-1
```

### Comparing `Rbeast-0.1.13/ext_src/abc_ide_util_python.c` & `Rbeast-0.1.14/ext_src/abc_ide_util_python.c`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 #include "assert.h"
 #include "abc_000_warning.h"
 
 #include "abc_ide_util.h"
 #include "abc_common.h"
 #include "abc_date.h"
 
-#if P_INTERFACE==1
+#if P_INTERFACE==1  
+
+int  JDN_to_DateNum(int jdn) {
+    return jdn - JulianDayNum_from_civil_ag1(1, 1, 1);
+}
 
 PyObject* currentModule;
 PyObject* classOutput=NULL;
 
 PyObject* setClassObjects(PyObject* self, PyObject* args){
 
     if (PyTuple_Size(args) == 1) {
@@ -25,15 +29,15 @@
 
 void* CvtToPyArray_NewRef(VOIDPTR Y) {
 
     if (PyArray_Check(Y)) {
     // Accessing view of a NumPy array using the C API
     // https://stackoverflow.com/questions/35000565/accessing-view-of-a-numpy-array-using-the-c-api
         PyArray_Descr* reqDescr = PyArray_DescrFromType(PyArray_TYPE(Y));
-        Pob            out    = PyArray_FromArray(Y, reqDescr, NPY_ARRAY_FARRAY);
+        Pob            out      = PyArray_FromArray(Y, reqDescr, NPY_ARRAY_FARRAY);
         return out;
     }   else {
         Pob            out = PyArray_FROM_OF(Y, NPY_ARRAY_FARRAY);
         return out;
     }
 
     return NULL;
@@ -132,14 +136,15 @@
 
 }
 
 
 int IsClass(void* ptr, char* class) { return 0; }
 int IsCell(void* ptr) { return 0; }
 int IsChar(void* ptr) {   
+    if (ptr == NULL) return 0;
 
     if (PyUnicode_Check(ptr)) {
         return 1;
     } 
     if (PyArray_Check(ptr) && PyArray_TYPE(ptr) == NPY_STRING) {
         return 1;
     }
@@ -316,14 +321,38 @@
             Py_DECREF(list);
             return item;   
     }
 
     return NULL;
 }
 
+
+void  GetFieldNameByIdx(VOID_PTR strucVar, I32 ind0, char *str, int buflen) {
+
+    Pob dict   = PyGetDict(strucVar);
+    
+    if (dict) {
+        PyObject* keys = PyDict_Keys(dict);              // new ref
+        int       n    = PyList_Size(keys);
+
+        PyObject* tmpkey = PyList_GetItem(keys, ind0);  // borrowed ref
+        if (IsChar(tmpkey)) {
+            int       len = GetCharArray(tmpkey, str, buflen);
+        }   else {
+            str[0] = 0;
+        }        
+
+        Py_DECREF(keys);
+    }    else {
+        str[0] = 0;
+    }
+    
+    
+}
+
 void* CreateStructVar(FIELD_ITEM* fieldList, int nfields); //Done
 
 void  DestoryStructVar(VOID_PTR strutVar) {  Py_XDECREF(strutVar);}
 
 void  RemoveField(FIELD_ITEM* fieldList, int nfields, char* fieldName); // Done. IDE-independent
 
 void AddStringAttribute(VOID_PTR listVar, const char* field, const char* value) {
@@ -378,15 +407,15 @@
     Py_XDECREF(col);
     return width;
 }
 
 
 I32 GetCharArray(void* ptr, char* dst, int n) {
     dst[0] = 0;
-    if (!IsChar(ptr)) return 0;
+    if (ptr ==NULL || !IsChar(ptr)) return 0;
 
     if (PyUnicode_Check(ptr)) {
         //int len;
         /* STUPID ME. it took me one day to figure out this bug:
         * if using int, the upper exta 32-bits will be reset to zero,
         * this will corrupt the pushed 'si' regiser, the si regiseter
         * seems to hold the prhs passed in the mainFunction
@@ -615,14 +644,39 @@
         }
     }
 
     if (PyList_Check(ptr) || PyTuple_Check(ptr) ) {
         dims[0] = PyObject_Size(ptr);
     }   
 }
+ 
+
+void * SetDimensions(const void* ptr, int dims[], int ndims) {
+    if (PyArray_Check(ptr)) {
+        //PyObject* PyArray_Newshape(PyArrayObject * self, PyArray_Dims * newshape, NPY_ORDER order);
+        //NPY_ANYORDER: keep the orignal order
+        
+        PyArray_Dims newshape;
+        npy_intp  newdims[100];
+        newshape.len = ndims;
+        newshape.ptr = newdims;
+         for (int i = 0; i < ndims; i++) {
+             newdims[i] = dims[i];
+        }
+
+         PyObject *newptr=PyArray_Newshape(ptr, &newshape, NPY_ANYORDER);
+
+         return newptr;
+
+    }
+    return NULL;
+    if (PyList_Check(ptr) || PyTuple_Check(ptr)) {
+      //  dims[0] = PyObject_Size(ptr);
+    }
+}
 
 int  GetNumberOfElements(const void* ptr) {
     
     if (PyArray_Check(ptr)) {
         return PyArray_SIZE(ptr);
     }
 
@@ -650,15 +704,15 @@
         return PyDict_Size(dict);
     }
     return -999;
 }
 
 
 int HaveEqualDimesions(const void* p1, const void* p2);
-int CopyNumericArrToF32Arr(F32PTR outmem, VOID_PTR infield, int N);
+int CopyNumericObjToF32Arr(F32PTR outmem, VOID_PTR infield, int N);
  
 void* CreateNumVar(DATA_TYPE dtype, int* dims, int ndims, VOIDPTR* data_ptr) {
 
     npy_intp dimsnp[10];
     for (int i = 0; i < ndims; i++) {
         dimsnp[i] = dims[i];
     }
```

### Comparing `Rbeast-0.1.13/ext_src/abc_ioFlush.c` & `Rbeast-0.1.14/ext_src/abc_ioFlush.c`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 #include "abc_000_macro.h"
 #include "abc_000_warning.h"
 
-#if M_INTERFACE ==1 && !defined(MSVC_COMPILER)
+#include "abc_001_config.h"
+#include "abc_datatype.h"
+
+ #if M_INTERFACE ==1 &&  !defined(MSVC_COMPILER)
+
 	#include "inttypes.h"
 	#include "mex.h"
     //https://stackoverflow.com/questions/26271154/how-can-i-make-a-mex-function-printf-while-its-running/26271557
     //isoFlush is  an undocumented C++ function that resides in libmwservices.dll
 	#if defined(WIN_OS)
-		extern bool ioFlush(void)  asm("?ioFlush@@YA_NXZ");
+		extern Bool ioFlush(void)  asm("?ioFlush@@YA_NXZ");
 	#elif defined(MAC_OS)
       // Linux		
-		extern bool ioFlush(void)  asm("__Z7ioFlushv");
+		extern Bool ioFlush(void)  asm("__Z7ioFlushv");
 	#else 
-		extern bool ioFlush(void)  asm("_Z7ioFlushv");
+		extern Bool ioFlush(void)  asm("_Z7ioFlushv");
 	#endif
 
 //https://stackoverflow.com/questions/35837694/how-to-manually-mangle-names-in-visual-c
 		//https://gcc.gnu.org/onlinedocs/gcc/Asm-Labels.html
 		// ON Windows, for MSVC C++ only, use the __identififer macro to give an alias
 		// Using gcc, use  int a asm("xxx")
 
     void matlab_IOflush(void)	{
-		ioFlush();
+		#ifndef O_INTERFACE
+			ioFlush();
+		#endif
 	}
 
 	////https://stackoverflow.com/questions/10529500/what-does-this-mean-int-a
 	/*
 		in C++, (int &) is a type punning that can force converstion of a variable to int
 	*/
```

### Comparing `Rbeast-0.1.13/ext_src/abc_ioFlushcpp.cpp` & `Rbeast-0.1.14/ext_src/abc_ioFlushcpp.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #include "abc_000_macro.h"
 #include "abc_000_warning.h"
+#include "abc_datatype.h"
+#include "abc_001_config.h"
 
 #if M_INTERFACE ==1 && defined(MSVC_COMPILER)
 	#include "inttypes.h"
 	#include "mex.h"
     //https://stackoverflow.com/questions/26271154/how-can-i-make-a-mex-function-printf-while-its-running/26271557
     //isoFlush is  an undocumented C++ function that resides in libmwservices.dll
-	extern bool ioFlush(void);
+	extern Bool ioFlush(void);
 	extern "C"  void matlab_IOflush(void)	{
 		ioFlush();
 	}
 
 	////https://stackoverflow.com/questions/10529500/what-does-this-mean-int-a
 	/*
 		in C++, (int &) is a type punning that can force converstion of a variable to int
```

### Comparing `Rbeast-0.1.13/ext_src/abc_lzw.c` & `Rbeast-0.1.14/ext_src/abc_lzw.c`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 		nextbits += 8;					\
 	}							\
 	code = (hcode_t)((nextdata >> (nextbits-nbits)) & nbitsmask);	\
 	nextbits -= nbits;					\
 }
 
 
-static LZWCodecState* LZWSetupDecode( )
+static LZWCodecState* LZWSetupDecode(void)
 {
 	LZWCodecState* sp = NULL;
 	int code;
 
 
 		/*
 		* Allocate state block so tag methods have storage to record
```

### Comparing `Rbeast-0.1.13/ext_src/abc_mat.c` & `Rbeast-0.1.14/ext_src/abc_mat.c`

 * *Files 21% similar despite different names*

```diff
@@ -726,19 +726,19 @@
 			F32  Ukk_invert = U[col - 1];
 			F64  Ucol_curElem = (Au[col - 1] - sum) * Ukk_invert; //invert diagoal element
 			Ucol[col - 1] = Ucol_curElem;
 			SUM += Ucol_curElem * Ucol_curElem;
 			U += N;
 		}
 
-		F32 prec = (COL == 1) ? 0. : *precPrior;
-		Ucol[COL - 1] = 1.f / sqrt((Au[COL - 1] + prec) - SUM); //invert diagoal element
+		F32 prec       = (COL == 1) ? 0.f : *precPrior;
+		Ucol[COL - 1]  = 1.f / sqrt((Au[COL - 1] + prec) - SUM); //invert diagoal element
 
 		Ucol += N;
-		Au += N;
+		Au   += N;
 	}
 
 }
 
 void chol_addCol_skipleadingzeros_prec_invdiag(F32PTR Au, F32PTR U, F32PTR precPrior, I64 N, I64 K0, I64 K1)
 {
 	// A =U'*U:  A of size NxN
@@ -1017,14 +1017,79 @@
 
 	r_cblas_sgemv(CblasColMajor, CblasNoTrans, N, K, 1.f, X, ldx, B, 1L, 0.f, Yfit, 1L);
 
 	if (Yerror)
 		r_ippsSub_32f(Yfit, Y, Yerror,N); //Yerror=Y-Yfit 
 
 }
+
+void simple_linear_regression_nan(F32PTR Y, F32PTR X, int N, F32PTR Yfit, F32PTR Yerror) {
+	F64 Xsum, Ysum, XY, XX;
+	F64 b0, b1;
+	int Ngood;
+
+	Xsum = Ysum = XX = XY = Ngood = 0;
+	
+	if (X) {
+		for (int i = 0; i < N; i++) {
+			int isGoodPt = (X[i] == X[i]) && (Y[i] == Y[i]);
+			Xsum += isGoodPt ? X[i] : 0;
+			Ysum += isGoodPt ? Y[i] : 0;
+			XY += isGoodPt ? X[i] * Y[i] : 0;
+			XX += isGoodPt ? X[i] * X[i] : 0;
+			Ngood += isGoodPt;
+		}
+
+	}
+	else {
+		//Assume X is 0, 1/N, 2/N, (N-1)/N
+		for (int i = 0; i < N; i++) {
+			int isGoodPt =  (Y[i] == Y[i]);
+			F64 x = (double) i / (double)N;
+			Xsum += isGoodPt ? x : 0;
+			Ysum += isGoodPt ? Y[i] : 0;
+			XY += isGoodPt ? x * Y[i] : 0;
+			XX += isGoodPt ? x *x : 0;
+			Ngood += isGoodPt;
+		}
+	}
+	F64 SXY = XY - Xsum * Ysum / Ngood;
+	F64 SXx = XX - Xsum * Xsum / Ngood;
+
+	b1 = SXY / SXx;
+	b0 = Ysum / Ngood - b1 * Xsum / Ngood;
+
+	if (Yfit) {
+		if (X) {
+			for (int i = 0; i < N; i++) {	 
+				Yfit[i] = X[i] * b1 + b0;
+			}
+		}else {
+			for (int i = 0; i < N; i++) {
+				Yfit[i] =  b1*i/N + b0;
+			}
+		}
+	}
+
+	if (Yerror) {
+		if (X) {
+			for (int i = 0; i < N; i++) {
+				Yerror[i] = Y[i]-(X[i] * b1 + b0);
+			}
+		}
+		else {
+			for (int i = 0; i < N; i++) {
+				Yerror[i] = Y[i] - (b1 * i / N + b0);
+			}
+		}
+	}
+}
+
+
+
 /*
 void f32_gemm_XtY1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc) 
 {
  	for (int col = 0; col < N; ++col) {
 		int dir = 1;
 		int row = 0;		
 		for (; row < M-(2-1); row +=2) {
@@ -1194,10 +1259,362 @@
 				SCPY(KNEW - k2_new, XtY + (k2_old + 1L) - 1L + KOLD * c, XtYnew + (k2_new + 1) - 1 + KNEW * c);
 			}
 		}
 
 
 	}
 }
+
+
+
+void get_parts_for_newinfo(NEWCOLINFOv2* new) {
+	// x1, xnew1, x2, xnew2, x3, xnew3, x4
+
+	int Knewterm    = 0;
+	int Kbase_dst   = 1;
+
+	int jParts      = 0;
+	for (int i = 0; i <  new->nbands; ++i) {
+
+		new->parts[jParts].X      = new->X;
+		new->parts[jParts].ks_dst = Kbase_dst;
+		
+		if (i == 0) {
+			new->parts[jParts].ks_src = 1;
+		} else {
+			new->parts[jParts].ks_src = new->ks_x[i-1] + new->kterms_x[i-1];
+		}
+		new->parts[jParts].kterms = new->ks_x[i]- new->parts[jParts].ks_src;
+
+		Kbase_dst += new->parts[jParts].kterms;
+		jParts++;
+		///////////////////////////////////////////////////////	
+
+
+		//////////////////////////////////////////////////////
+		new->parts[jParts].X      = new->Xnewterm;
+		new->parts[jParts].ks_dst = Kbase_dst;
+		
+		new->parts[jParts].ks_src = new->ks_xnewterm[i];
+		new->parts[jParts].kterms = new->kterms_xnewterm[i];
+		Kbase_dst    += new->parts[jParts].kterms;
+		Knewterm     += new->kterms_xnewterm[i];
+
+		jParts++;
+		
+	}
+	// The last part is the X's remaining part
+	new->parts[jParts].X       = new->X;
+	new->parts[jParts].ks_dst = Kbase_dst;	
+	new->parts[jParts].ks_src = new->ks_x[new->nbands - 1] + new->kterms_x[new->nbands - 1];
+	new->parts[jParts].kterms = (new->K - new->parts[jParts].ks_src)+1L;
+    
+	new->Knew     = Kbase_dst + (new->parts[jParts].kterms - 1L);
+	new->Knewterm = Knewterm;
+	new->Kchol    = new->ks_x[0];
+
+	new->isEqualSwap = 0;
+	if (new->K == new->Knew) {
+		new->isEqualSwap = 1;
+		for (int i = 0; i < new->nbands; i++) {
+			if (new->kterms_x[i] != new->kterms_xnewterm[i]) {
+				new->isEqualSwap = 0;
+				break;
+			}
+		}
+	}	
+}
+
+
+void update_XtX_from_Xnewterm_v2(F32PTR XtX, F32PTR XtXnew, NEWCOLINFOv2* new ) {
+
+ 
+	I32 N    = new->N;
+	I32 Nlda = new->Nlda;
+
+	I32 KOLD = new->K;
+	I32 KNEW = new->Knew;
+
+	if (new->isEqualSwap) {
+		SCPY(KOLD * KOLD, XtX, XtXnew);
+	}
+
+	I32 colbase = 1;	
+	for (int i = 0; i < (new->nbands * 2 + 1); i++) {		
+		I32 Kcol = new->parts[i].kterms;
+		if (Kcol == 0) {
+			continue;
+		}
+
+		I32     rowbase = 1;
+		F32PTR  Xcol0 = new->parts[i].X;
+		F32PTR  Xcol  = Xcol0 + (new->parts[i].ks_src - 1) * Nlda;		
+		for (int j = 0; j <= i; j++) {
+			I32  Krow = new->parts[j].kterms;
+			if (Krow == 0) {
+				continue;
+			}
+
+			F32PTR  Xrow0  = new->parts[j].X;
+			F32PTR  Xrow   = Xrow0 + (new->parts[j].ks_src - 1) * Nlda;
+			if (Xcol0 != new->X || Xrow0 != new->X) {
+			 // New XtX values needed to be computed
+				r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, 
+					Krow, Kcol, N, 1.0f,
+					Xrow, Nlda,	Xcol, Nlda, 0.f,
+					XtXnew + (colbase - 1L) * KNEW + rowbase - 1, KNEW);
+			}
+			else if (new->isEqualSwap==0) {
+			// Need to copy old values from XtX to XtXnew
+			
+				I32 row_old = new->parts[j].ks_src;
+				I32 col_old = new->parts[i].ks_src;
+
+				F32PTR ColStart_old = XtX    + (col_old - 1) * KOLD + row_old -1L;
+				F32PTR ColStart_new = XtXnew + (colbase - 1) * KNEW + rowbase- 1L;
+				if (i == j) {
+					// Copy the existing values of the upper triangle from XtX to XtXnew
+					for (int k = 1; k <= Kcol; ++k) {
+						SCPY(k, ColStart_old + (k - 1) * KOLD, ColStart_new + (k - 1) * KNEW);
+					}
+				} else {
+					// Copy the existing values of the full rectangle from XtX to XtXnew
+					for (int k = 1; k <= Kcol; ++k) {						
+						SCPY(Krow, ColStart_old + (k - 1) * KOLD, ColStart_new + (k - 1) * KNEW);
+					}
+				}
+				
+
+	 	   } // if (Xcol0 != new->X || Xrow0 != new->X) 	
+
+		   rowbase += Krow;
+
+		} //for (int j = 0; j <= i; j++)
+
+		colbase += Kcol;
+	}
+	
+
+			 
+}
+
+void update_XtY_from_Xnewterm_v2(F32PTR XtY, F32PTR XtYnew, F32PTR Y, NEWCOLINFOv2* new, I32 q) {
+
+	// X and Xnewterm has a leading dimesnion of new.Nlada
+	// Y has a leading dimension of new.N
+
+	I32 N    = new->N;
+	I32 Nlda = new->Nlda;
+
+	I32 KOLD = new->K;
+	I32 KNEW = new->Knew;
+
+	if (new->isEqualSwap) {
+		SCPY(KOLD*q, XtY, XtYnew);
+	}
+
+	if (q == 1) {
+		I32     rowbase = 1;
+		for (int i = 0; i < (new->nbands * 2 + 1); i++) {
+			I32 Krow = new->parts[i].kterms;
+			I32 row_old = new->parts[i].ks_src;
+			if (Krow == 0) {
+				continue;
+			}
+
+			F32PTR  Xrow0 = new->parts[i].X;
+			F32PTR  Xrow = Xrow0 + (row_old - 1) * Nlda;
+			if (Xrow0 != new->X) {
+				// New XtX values needed to be computed
+				r_cblas_sgemv(CblasColMajor, CblasTrans,
+					N, Krow, 1.f,
+					Xrow, Nlda,
+					Y, 1L, 0.f,
+					XtYnew + rowbase - 1, 1L);
+			}
+			else if (new->isEqualSwap == 0) {
+				// Need to copy old values from XtX to XtXnew			
+				SCPY(Krow, XtY + row_old - 1L, XtYnew + rowbase - 1);
+
+			} // if (Xcol0 != new->X || Xrow0 != new->X) 	
+
+			rowbase += Krow;
+		}
+	}
+	else {	// q > 1
+
+		I32     rowbase = 1;
+		for (int i = 0; i < (new->nbands * 2 + 1); i++) {
+			I32 Krow = new->parts[i].kterms;
+			I32 row_old = new->parts[i].ks_src;
+			if (Krow == 0) {
+				continue;
+			}
+
+			F32PTR  Xrow0 = new->parts[i].X;
+			F32PTR  Xrow = Xrow0 + (row_old - 1) * Nlda;
+			if (Xrow0 != new->X) {
+				// New XtX values needed to be computed
+				r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans,
+					Krow, q, N, 1.f,
+					Xrow, Nlda,
+					Y, N, 0.f,
+					XtYnew + rowbase - 1, KNEW);
+			}
+			else if (new->isEqualSwap == 0) {
+				// Need to copy old values from XtX to XtXnew							
+				for (I32 c = 0; c < q; ++c) {
+					SCPY(Krow, XtY +c*KOLD+ row_old - 1L, XtYnew + c * KNEW + rowbase - 1);
+				}
+			} // if (Xcol0 != new->X || Xrow0 != new->X) 	
+
+			rowbase += Krow;
+		}
+	
+	} //else {	// q > 1
+
+ 
+}
+
+void shift_last_elems(void * X, I32 Kstart, I32 Kend, I32 Knewstart, I32 elemSize) {
+	// K are all one-based indices
+	
+	I08PTR x = X;
+	if (Knewstart == Kstart) { 	// a. No need to move at all
+		return;
+	}	else if (Knewstart < Kstart || Knewstart > Kend) {	// b.Move forwward or no overlapping
+		// dst(k2_new):-----123455----
+		// src(k2_old):----------123455----
+
+		// dst(k2_new):----------------123455----
+		// src(k2_old):-----123455----		
+		memcpy(x + (Knewstart - 1) * elemSize, x+(Kstart - 1) *elemSize,  (Kend - Kstart + 1) * elemSize);
+		//memcpy(dst, src, size)
+	}	else {	// c. Movee backward with some overlapping
+		// dst(k2_new):-------------123456----
+		// src(k2_old):---------123456----
+		I32 segStartIdx = Kend + 1;	
+		int nElemsCopy  = Knewstart-Kstart;  //j>0
+		while (_True_) {
+			segStartIdx = segStartIdx - nElemsCopy;
+			if (segStartIdx > Kstart) {
+				//memcpy(dst, src, size)
+				memcpy(x + ((segStartIdx + nElemsCopy) - 1) * elemSize, x + (segStartIdx - 1) * elemSize, nElemsCopy * elemSize) ;
+			} else {
+				nElemsCopy = (segStartIdx + nElemsCopy) - Kstart;
+				memcpy(x + (Knewstart - 1) * elemSize,  x+ (Kstart - 1) * elemSize, nElemsCopy * elemSize);
+				break;
+			}
+		}//while (_True_)
+	} //if (j < 0 || k2_new + 1 > Kold)
+
+}
+
+void swap_elem_bands(NEWCOLINFOv2* new, void *x, void *xnew, I32 elemSize) {
+
+	U08PTR X    = x;
+	U08PTR Xnew = xnew;
+
+	if (new->isEqualSwap == 0) {
+		// First, shift X's col bands
+		// X1, Xnewterm1, X2, Xnewterm2, X3, Xnewtem4, Xn4
+		// Need to shift X2, X3, and X4
+		int    Kend    = new->K;
+		int    Kadjust = 0;
+		for (int i = 3; i <= (new->nbands * 2 + 1); i += 2) {
+			if (new->parts[i - 1].kterms == 0) {
+				continue;
+			}
+			int Kstart    = new->parts[i - 1].ks_src + Kadjust;
+			int Knewstart = new->parts[i - 1].ks_dst;
+			shift_last_elems(X,Kstart, Kend, Knewstart, elemSize);
+
+			// then the original cols have been shifted
+			Kadjust += (Knewstart - Kstart);
+			Kend    += Kadjust;
+		}
+
+	}
+
+	// Insert the Xnewterm nto the shiftted X 
+	for (int i = 2; i <= (new->nbands * 2 + 1); i += 2) {
+		if (new->parts[i - 1].kterms == 0) {
+			continue;
+		}
+		int Knewterm = new->parts[i - 1].kterms;
+		// memcpy(dst, src, size)
+		memcpy(X + (new->parts[i - 1].ks_dst - 1) * elemSize, Xnew + (new->parts[i - 1].ks_src - 1) * elemSize, Knewterm * elemSize);		
+	}
+
+}
+
+void shift_lastcols_within_matrix(F32PTR X, I32 N, I32 Kstart, I32 Kend, I32 Knewstart) {
+
+	if (Knewstart == Kstart) {
+		return;
+	}
+
+	int j = Knewstart - Kstart;
+	if (j < 0 || Knewstart > Kend) {
+		// dst(k2_new):-----123455----
+		// src(k2_old):----------123455----
+
+		// dst(k2_new):----------------123455----
+		// src(k2_old):-----123455----
+		r_cblas_scopy((Kend - Kstart + 1) * N, X + (Kstart - 1) * N, 1, X + (Knewstart - 1) * N, 1);
+	} else {
+		// dst(k2_new):-------------123456----
+		// src(k2_old):---------123456----
+		I32 segStartIdx = Kend + 1;
+		while (_True_) {
+			segStartIdx = segStartIdx - j;
+			if (segStartIdx > Kstart) {
+				SCPY(j * N, X + (segStartIdx - 1) * N, X + ((segStartIdx + j) - 1) * N);				
+			} else {
+				j = (segStartIdx + j) - Kstart;
+				SCPY(j * N, X + (Kstart - 1) * N, X + (Knewstart - 1) * N);
+				break;
+			}
+		}//while (_True_)
+	}//if (j < 0 || k2_new + 1 > Kold)
+
+}
+
+void swap_cols_bands_within_matrx(NEWCOLINFOv2* new) {
+	
+	F32PTR X = new->X;
+
+	if (new->isEqualSwap == 0) {
+		// First, shift X's col bands
+		// X1, Xnewterm1, X2, Xnewterm2, X3, Xnewtem4, Xn4
+		// Need to shift X2, X3, and X4
+		int    Kend    = new->K;
+		int    Kadjust = 0;		
+		for (int i = 3; i <= (new->nbands * 2 + 1); i += 2) {
+			if (new->parts[i - 1].kterms == 0) {
+				continue;
+			}
+			int Kstart     = new->parts[i - 1].ks_src + Kadjust;
+			int Knewstart  = new->parts[i - 1].ks_dst;
+			shift_lastcols_within_matrix(X, new->Nlda, Kstart, Kend, Knewstart);
+						
+			// then the original cols have been shifted
+			Kadjust += (Knewstart - Kstart);
+			Kend    += Kadjust;		
+		}
+
+	}
+
+	// Insert the Xnewterm nto the shiftted X
+	int N = new->Nlda;
+	for (int i = 2; i <= (new->nbands * 2 + 1); i += 2) {
+		if (new->parts[i - 1].kterms == 0) {
+			continue;
+		}
+		int Knewterm = new->parts[i - 1].kterms;
+		SCPY(Knewterm*N, new->Xnewterm + (new->parts[i-1].ks_src- 1) * N, X + (new->parts[i - 1].ks_dst - 1) * N);
+	}
+		
+}
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/abc_math_avx.c` & `Rbeast-0.1.14/ext_src/abc_math_avx.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_math_avx.h` & `Rbeast-0.1.14/ext_src/abc_math_avx.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #pragma once
 #include <immintrin.h>
 #include "abc_000_macro.h"
+#include "abc_datatype.h"
 
 typedef __m256  v8sf; // vector of 8 float (avx)
 typedef __m256i v8si; // vector of 8 int   (avx)
 typedef __m128i v4si; // vector of 8 int   (avx) 
 typedef __m128  v4sf; // vector of 8 int   (avx) 
 
 #if defined(MSVC_COMPILER)
```

### Comparing `Rbeast-0.1.13/ext_src/abc_math_avx512.c` & `Rbeast-0.1.14/ext_src/abc_math_avx512.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_math_avx512.h` & `Rbeast-0.1.14/ext_src/abc_math_avx512.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_mcmc.c` & `Rbeast-0.1.14/ext_src/abc_mcmc.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_mcmc.h` & `Rbeast-0.1.14/ext_src/abc_mcmc.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_mem_ext.c` & `Rbeast-0.1.14/ext_src/abc_mem_ext.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_mem_ext.h` & `Rbeast-0.1.14/ext_src/abc_mem_ext.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_pthread.c` & `Rbeast-0.1.14/ext_src/abc_pthread.c`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,74 @@
 #include "abc_000_warning.h"
 #include "abc_000_macro.h"
+#include "abc_ide_util.h"  // for printf only
 
 //https://stackoverflow.com/questions/150355/programmatically-find-the-number-of-cores-on-a-machine
 #if defined(_WIN32) || defined(WIN64_OS)
     //#define WIN32_LEAN_AND_MEAN
 	//#include <windows.h>
     #include "abc_pthread.h"
 #elif defined(MAC_OS)
 	#include <sys/param.h>
 	#include <sys/sysctl.h>
 #elif defined(LINUX_OS) || defined(SOLARIS_OS)
-//https://docs.oracle.com/cd/E36784_01/html/E36874/sysconf-3c.html
-	#include <unistd.h>
+   //https://docs.oracle.com/cd/E36784_01/html/E36874/sysconf-3c.html
+	#include <unistd.h> // needed for sysconf
 #endif
 
-#include <inttypes.h>
-#include "abc_ide_util.h" // for printf only
+#if  defined(LINUX_OS) 
+    //you have to define_GNU_SOURCE before anything else
+    //https://stackoverflow.com/questions/1407786/how-to-set-cpu-affinity-of-a-particular-pthread
+    //https://stackoverflow.com/questions/7296963/gnu-source-and-use-gnu/7297011#7297011
+    //https://stackoverflow.com/questions/24034631/error-message-undefined-reference-for-cpu-zero/24034698
+    #ifndef _GNU_SOURCE
+        #define _GNU_SOURCE
+    #endif
+    #include <sched.h>  ////cpu_set_t , CPU_SET
+    #include <pthread.h>
+#elif defined(SOLARIS_OS)
+    #include <sched.h>  ////cpu_set_t , CPU_SET
+    #include <pthread.h>
+#endif
+
+/*
+https://stackoverflow.com/questions/2127797/significance-of-pthread-flag-when-compiling
+
+-pthread Adds support for multithreading with the pthreads library.
+This option sets flags for both the preprocessorand linker.
+
+for clang,
+https://github.com/mesonbuild/meson/issues/2628
+
+Strange. Now that you mentioned it I tried two compilers, the native clang that's shipped by the system, and version 5.0 as compiled by MacPorts. Only the one which comes with the system complains, the other one does not.
+
+But just to confirm once again:
+clang[++] -pthread hello.c[pp] -o hello OK
+clang[++] -pthread hello.o -o hello complains because this only calls linker
+clang[++]-mp-5.0 -pthread hello.c[pp] -o hello OK
+clang[++]-mp-5.0 -pthread hello.o -o hello OK
+
+https://stackoverflow.com/questions/17841140/os-x-clang-pthread
+clang requires -pthread when compiling but not when linking. This is annoying, but it is observed behavior:
+
+*/
+
+void PrintBits(size_t const size, void const* const ptr)
+{
+    unsigned char* b = (unsigned char*)ptr;
+    unsigned char byte;
+    int i, j;
+
+    for (i = size - 1; i >= 0; i--) {
+        for (j = 7; j >= 0; j--) {
+            byte = (b[i] >> j) & 1;
+            r_printf("%u", byte);
+        }
+    }
+}
 
 int CountSetBits32(uint32_t x)  {
     //https://en.wikipedia.org/wiki/Hamming_weight
     //https://stackoverflow.com/questions/109023/how-to-count-the-number-of-set-bits-in-a-32-bit-integer
     x = x - ((x >> 1) & 0x55555555);
     x = (x & 0x33333333) + ((x >> 2) & 0x33333333);
     x = (x + (x >> 4)) & 0x0F0F0F0F;
@@ -43,15 +92,15 @@
     x = (x + (x >> 4)) & m4;        //put count of each 8 bits into those 8 bits 
     x += x >> 8;  //put count of each 16 bits into their lowest 8 bits
     x += x >> 16;  //put count of each 32 bits into their lowest 8 bits
     x += x >> 32;  //put count of each 64 bits into their lowest 8 bits
     return x & 0x7f;
 }
 
-int GetNumCores()  {
+int GetNumCores(void)  {
     //https://stackoverflow.com/questions/150355/programmatically-find-the-number-of-cores-on-a-machine
 #if defined(_WIN32) || defined(WIN64_OS)    
     uint32_t count;
 	count = GetCPUInfo(); 
 #elif defined(__MACH__)
     int nm[2];
     size_t   len = 4;
@@ -74,15 +123,15 @@
 }
 
 
 #if defined(_WIN32) || defined(WIN64_OS)
 
 typedef struct __CPUINFO {
     //docs.microsoft.com/en-us/windows/win32/procthread/what-s-new-in-processes-and-threads
-    DWORD (WINAPI* GetActiveProcessorGroupCount)     ();
+    DWORD (WINAPI* GetActiveProcessorGroupCount)     (void);
     DWORD (WINAPI* GetActiveProcessorCount)          (WORD GroupNumber);
     BOOL  (WINAPI* GetLogicalProcessorInformationEx) (
             LOGICAL_PROCESSOR_RELATIONSHIP           RelationshipType,        
             PSYSTEM_LOGICAL_PROCESSOR_INFORMATION_EX Buffer,
             PDWORD                                   ReturnedLength );
     HANDLE (WINAPI*  CreateRemoteThreadEx) (
             HANDLE                       hProcess,
@@ -107,36 +156,38 @@
                 UCHAR      Node,
                 PULONGLONG AvailableBytes   ); //available since Win XP
 
     char isInitilized;
 } CPUFUCINFO;
 
 typedef struct __CPUINFO1 {
-    DWORD logicalProcessorCount;
-    DWORD numaNodeCount;    
+    DWORD numaNodeCount;
+    DWORD processorPackageCount;
     DWORD processorCoreCount;
+    DWORD logicalProcessorCount;        
+
     DWORD processorL1CacheCount;
     DWORD processorL2CacheCount;
     DWORD processorL3CacheCount ;
-    DWORD processorPackageCount;
-    DWORD processorGroupCount;
-    DWORD coreCountPerGrp[10];
-    DWORD currentGroup;
-    DWORD currentCoreNumber;
-    uint64_t currentThreadAffinity;
-    char cpuGroup[256];
-    char numCPUCoresToUseber[256];
+    
+    
+    DWORD    processorGroupCount;
+    DWORD    coreCountPerGrp[10];
+    uint64_t affinityPerGrp[10];
+
+    char    cpuGroup[256];
+    char    coreIDinGroup[256];
     //uint64_t currentGroupAffinity;
 
 } CPUINFO;
 
 static CPUFUCINFO cpuFunc = {0,};
 static CPUINFO    cpuInfo = {0,};
 
-static void InitCPUFuncs( ) {
+static void InitCPUFuncs(void) {
     if (cpuFunc.isInitilized)  {
         return;
     }
     HMODULE kerHandle  = GetModuleHandle(TEXT("kernel32"));
     cpuFunc.GetActiveProcessorGroupCount     =  GetProcAddress(kerHandle, "GetActiveProcessorGroupCount");
     cpuFunc.GetActiveProcessorCount          =  GetProcAddress(kerHandle, "GetActiveProcessorCount");
     cpuFunc.GetLogicalProcessorInformationEx = GetProcAddress(kerHandle, "GetLogicalProcessorInformationEx");
@@ -146,28 +197,28 @@
     cpuFunc.GetCurrentProcessorNumber        = GetProcAddress(kerHandle, "GetCurrentProcessorNumber");
     cpuFunc.GetNumaHighestNodeNumber         = GetProcAddress(kerHandle, "GetNumaHighestNodeNumber");
     cpuFunc.GetNumaProcessorNodeEx           = GetProcAddress(kerHandle, "GetNumaProcessorNodeEx");
     cpuFunc.GetNumaAvailableMemoryNode       = GetProcAddress(kerHandle, "GetNumaAvailableMemoryNode");
     cpuFunc.isInitilized = 1;
 }
 
-static int  GetCoreNumbers_WIN32() {
+static int  GetCoreNumbers_WIN32(void) {
 
     cpuInfo = (CPUINFO){ 0, };
 
     SYSTEM_INFO   sysinfo;
     GetSystemInfo(&sysinfo);   
     cpuInfo.logicalProcessorCount = sysinfo.dwNumberOfProcessors;
     
     cpuInfo.processorGroupCount = 1;
     uint64_t currentGroupAffinity;
     return cpuInfo.logicalProcessorCount;
 }
 
-static int GetCoreNumbers_WIN7V1() {
+static int  GetCoreNumbers_WIN7V1(void) {
     cpuInfo = (CPUINFO){ 0, };
 
     InitCPUFuncs();
     if (NULL == cpuFunc.GetActiveProcessorGroupCount)   {
         return -1;
     }
 
@@ -187,15 +238,15 @@
     ULONG numaCount;
     cpuFunc.GetNumaHighestNodeNumber(&numaCount);
     cpuInfo.numaNodeCount = numaCount+1L;
     return cpuInfo.logicalProcessorCount; 
 }
 
 //https://docs.microsoft.com/en-us/windows/win32/api/sysinfoapi/nf-sysinfoapi-getlogicalprocessorinformation
-static int GetCoreNumbers_WINXP()
+static int GetCoreNumbers_WINXP(void)
 {         
     cpuInfo = (CPUINFO){ 0, };
 
     PSYSTEM_LOGICAL_PROCESSOR_INFORMATION buffer = NULL;
    
 
   
@@ -277,15 +328,15 @@
     */
 
     free(buffer);
 
     return cpuInfo.logicalProcessorCount;
 }
 
-static int GetCoreNumbers_WIN7V2() {
+static int GetCoreNumbers_WIN7V2(void) {
 
     #ifdef WIN64_OS
 
     cpuInfo = (CPUINFO){0, };
     
 
     InitCPUFuncs();
@@ -294,275 +345,430 @@
     DWORD returnLength = 0;
     BOOL  done         = FALSE;
     while (!done) {
          DWORD fOK = cpuFunc.GetLogicalProcessorInformationEx(
                              RelationAll, (PSYSTEM_LOGICAL_PROCESSOR_INFORMATION_EX) buffer, &returnLength);         
          if (FALSE == fOK) {
             if (GetLastError() == ERROR_INSUFFICIENT_BUFFER)  {
-               if (buffer) 
-                   free(buffer);
+               if (buffer)     free(buffer);
                buffer = (PSYSTEM_LOGICAL_PROCESSOR_INFORMATION_EX)malloc(returnLength);
 
                if (NULL == buffer) {  // _tprintf(TEXT("\nError: Allocation failure\n"));
                     return (-1);
                }
             } else {       //_tprintf(TEXT("\nError %d\n"), GetLastError());
                 return (-1);
             }
          }  else {
                 done = TRUE;
          }
 
     }
 
+    int num_RelationProcessorCore=0;
+    int num_RelationGroup       = 0;
      PSYSTEM_LOGICAL_PROCESSOR_INFORMATION_EX  ptr = buffer;
  
      DWORD byteOffset = 0;
      while (byteOffset < returnLength) {
 
             switch (ptr->Relationship)
             {
             case RelationNumaNode:
                 // Non-NUMA systems report a single record of this type.
                 cpuInfo.numaNodeCount++;
                 break;
                 
             case RelationProcessorCore:
                 cpuInfo.processorCoreCount++;
-                /*
-                printf("************\n");
-                printf("%u\n",  ptr->Processor.Flags);
+                //A hyperthreaded core supplies more than one logical processor.
+                cpuInfo.logicalProcessorCount += ptr->Processor.Flags + 1L;                 
+              /*
+                r_printf("************************************\n");
+                r_printf("Entry ID        : %u\n", num_RelationProcessorCore++);
+                r_printf("Has Logical Core: %u\n",  ptr->Processor.Flags);
                 for (int i = 0; i < ptr->Processor.GroupCount; i++)  {
-
-                    printf("%u\n",   ptr->Processor.GroupMask[i].Group);
-                    printf("%08x\n", ptr->Processor.GroupMask[i].Mask);
+                    r_printf("Group ID        : %u\n",   ptr->Processor.GroupMask[i].Group);
+                    //r_printf("Group Mask      : %08x\n", ptr->Processor.GroupMask[i].Mask);
+                    r_printf("Group Mask      : ");
+                    PrintBits(sizeof(ptr->Processor.GroupMask[i].Mask), &ptr->Processor.GroupMask[i].Mask);
+                    r_printf("\n");
                 }
-
-                printf("------\n");
                 */
-                //A hyperthreaded core supplies more than one logical processor.
-                cpuInfo.logicalProcessorCount += ptr->Processor.Flags + 1L;
                 break;
-
+ 
             case RelationCache:
-                // Cache data is in ptr->Cache, one CACHE_DESCRIPTOR structure for each cache. 
-
+                // Cache data is in ptr->Cache, one CACHE_DESCRIPTOR structure for each cache.    
+                if (ptr->Cache.Level == 1)                {
+                    cpuInfo.processorL1CacheCount++;
+                }  else if (ptr->Cache.Level == 2)            {
+                    cpuInfo.processorL2CacheCount++;
+                } else if (ptr->Cache.Level == 3)   {
+                    cpuInfo.processorL3CacheCount++;
+                }
                 break;
-
             case RelationProcessorPackage:
                 // Logical processors share a physical package.
                 cpuInfo.processorPackageCount++;
+            
                 /*
-                printf("************\n");
-                printf("%u\n", ptr->Processor.Flags);
+                r_printf("************************************\n");
+                r_printf("%u\n", ptr->Processor.Flags);
                 for (int i = 0; i < ptr->Processor.GroupCount; i++) {
-                    printf("%u\n", ptr->Processor.GroupMask[i].Group);
-                    printf("%08x\n", ptr->Processor.GroupMask[i].Mask);
+                    r_printf("%u\n", ptr->Processor.GroupMask[i].Group);
+                    r_printf("%08x\n", ptr->Processor.GroupMask[i].Mask);
                 }
-                printf("------\n");
                 */
+              
                 break;
             case RelationGroup:
                 /*
-                printf("************\n");
-                printf("%u\n", ptr->Group.ActiveGroupCount);
+                r_printf("************************************\n");
+                r_printf("Entry ID        : %u\n", num_RelationGroup++);        
+                r_printf("Num of Groups   : %u\n", ptr->Group.ActiveGroupCount);
                 for (int i = 0; i < ptr->Group.ActiveGroupCount; i++) {
-                    printf("%u\n", ptr->Group.GroupInfo[i].ActiveProcessorCount);
-                    printf("%08x\n", ptr->Group.GroupInfo[i].ActiveProcessorMask);
+                    r_printf("                | count %u : mask, ",   ptr->Group.GroupInfo[i].ActiveProcessorCount);
+                    //r_printf("                | %08x\n", ptr->Group.GroupInfo[i].ActiveProcessorMask);
+                    PrintBits(sizeof(ptr->Group.GroupInfo[i].ActiveProcessorMask), &ptr->Group.GroupInfo[i].ActiveProcessorMask);
+                    r_printf("\n");
                 }
-                printf("------\n");
                 */
                 {
-                    int activeCount = ptr->Group.ActiveGroupCount;
+                    int numGrp_sofar = cpuInfo.processorGroupCount;
+                    int activeCount  = ptr->Group.ActiveGroupCount;
                     for (int i = 0; i < activeCount; i++) {
-                          cpuInfo.coreCountPerGrp[cpuInfo.processorGroupCount + i] = ptr->Group.GroupInfo[i].ActiveProcessorCount;
+                          cpuInfo.coreCountPerGrp[numGrp_sofar + i] = ptr->Group.GroupInfo[i].ActiveProcessorCount;
+                          cpuInfo.affinityPerGrp [numGrp_sofar + i] = ptr->Group.GroupInfo[i].ActiveProcessorMask;
                      }
-                    cpuInfo.processorGroupCount += activeCount;
+                    numGrp_sofar                += activeCount;
+                    cpuInfo.processorGroupCount += numGrp_sofar;
                 }
                 break;
             default:
                 //_tprintf(TEXT("\nError: Unsupported LOGICAL_PROCESSOR_RELATIONSHIP value.\n"));
                 break;
             }
 
             byteOffset += ptr->Size;
             ptr         = (char*)ptr + ptr->Size;
         }
 
-     
-     PROCESSOR_NUMBER procNum;
-     cpuFunc.GetCurrentProcessorNumberEx(&procNum);
-     cpuInfo.currentGroup = procNum.Group;
-     cpuInfo.currentCoreNumber = procNum.Number;
-
-     GROUP_AFFINITY grpAffinity;
-     cpuFunc.GetThreadGroupAffinity( GetCurrentThread(), &grpAffinity);
-     cpuInfo.currentThreadAffinity = grpAffinity.Mask;
+
+   
+     int idx = 0;
+     for (int grp = 0; grp < cpuInfo.processorGroupCount; grp++) {
+         int coreCountsPerGrp = cpuInfo.coreCountPerGrp[grp];
+         for (int i = 0; i < coreCountsPerGrp; i++) {
+             cpuInfo.cpuGroup[idx % 256]      = grp;
+             cpuInfo.coreIDinGroup[idx % 256] = i;
+             idx++;
+         }
+     }
+   
      
      return cpuInfo.logicalProcessorCount;
-
-  
+ 
     #endif
 
      return 0;
 }
 
-static void RankCPU() {
+static void RankCPU(void) {
 
 #ifdef WIN64_OS
 
+    PROCESSOR_NUMBER procNum;
+    cpuFunc.GetCurrentProcessorNumberEx(&procNum);
+    int curGrp = procNum.Group;
+    int curNo  = procNum.Number;
 
-    int nGrp   = cpuInfo.processorGroupCount;
-    int curGrp = cpuInfo.currentGroup;
-    int curNo  = cpuInfo.currentCoreNumber;
 
-    int coreCounts = cpuInfo.coreCountPerGrp[curGrp];
+    int nGrp             = cpuInfo.processorGroupCount;
+    int coreCountsPerGrp = cpuInfo.coreCountPerGrp[curGrp];
 
     int idx = 0;
-    for (int i = 0; i < coreCounts; i++) {
+    for (int i = 0; i < coreCountsPerGrp; i++) {
         if (i != curNo) {
-            cpuInfo.cpuGroup[idx]      = curGrp;
-            cpuInfo.numCPUCoresToUseber[idx] = i;
+            cpuInfo.cpuGroup[idx]           = curGrp;
+            cpuInfo.coreIDinGroup[idx] = i;
             idx++;
         }
     }
-    idx = coreCounts - 1;
+    idx = coreCountsPerGrp - 1;
     cpuInfo.cpuGroup[idx]      = curGrp;
-    cpuInfo.numCPUCoresToUseber[idx] = curNo;
+    cpuInfo.coreIDinGroup[idx] = curNo;
 
 
     // Sort through the other processor groups
-    idx = coreCounts;
+    idx = coreCountsPerGrp;
     for (int grp = 0; grp < nGrp; grp++) {
         if (grp == curGrp)
             continue;        
 
-        coreCounts = cpuInfo.coreCountPerGrp[grp];
-        for (int i = 0; i < coreCounts; i++) {
+        coreCountsPerGrp = cpuInfo.coreCountPerGrp[grp];
+        for (int i = 0; i < coreCountsPerGrp; i++) {
             cpuInfo.cpuGroup[idx %256]      = grp;
-            cpuInfo.numCPUCoresToUseber[idx %256] = i;
+            cpuInfo.coreIDinGroup[idx %256] = i;
             idx++;
         }
 
     }
 #endif
 }
 
+int sched_getcpu(void) {
+
+    if (cpuFunc.GetCurrentProcessorNumberEx != NULL) {
+        // Get the core id of the current thread
+        PROCESSOR_NUMBER procNum;
+        cpuFunc.GetCurrentProcessorNumberEx(&procNum);
+        int currentGroup      = procNum.Group;
+        int currentCoreNumber = procNum.Number;
+
+        int coreNum = 0;
+        for (int nGrp = 0; nGrp < (currentGroup - 1); nGrp++) {
+            coreNum += cpuInfo.coreCountPerGrp[nGrp];
+        }
+        coreNum += currentCoreNumber;
+        return coreNum;
+
+    }    else {
+        // the result is the core number within the current group.
+        return GetCurrentProcessorNumber();
+    }
+
+
+    GROUP_AFFINITY grpAffinity;
+    GetThreadGroupAffinity(GetCurrentThread(), &grpAffinity);
+    uint64_t  currentThreadAffinity = grpAffinity.Mask;
+}
+
 int GetCPUInfo() {
 
+    if (cpuInfo.logicalProcessorCount > 0) {
+        // Have alrady been obtained previously
+        return cpuInfo.logicalProcessorCount;
+    }
+ 
     InitCPUFuncs();
-
+ 
     int nCores;
     if (cpuFunc.GetLogicalProcessorInformationEx != NULL) {    
         nCores=GetCoreNumbers_WIN7V2();
-        RankCPU();
+      //  RankCPU();
     }  else  {
         nCores = GetCoreNumbers_WIN32();
     }
     PrintCPUInfo();
     return nCores;
 }
 
-
 void PrintCPUInfo() {
 
     r_printf("\nCPU Information:\n");
     r_printf(" - Number of NUMA nodes: %d\n", cpuInfo.numaNodeCount);
     r_printf((" - Number of physical processors (sockets): %d\n"), cpuInfo.processorPackageCount);
     r_printf((" - Number of processor cores: %d\n"), cpuInfo.processorCoreCount);
     r_printf((" - Number of logical processors: %d\n"), cpuInfo.logicalProcessorCount);
     r_printf(" - Number of processor groups: %d\n", cpuInfo.processorGroupCount);
     for (int i = 0; i < cpuInfo.processorGroupCount; i++) {
         r_printf(" -- Processor group #%d: %d cores\n", i, cpuInfo.coreCountPerGrp[i]);
     }
-    r_printf((" - Number of processor L1/L2/L3 caches: %d/%d/%d\n"), cpuInfo.processorL1CacheCount,
-        cpuInfo.processorL2CacheCount, cpuInfo.processorL3CacheCount);
-    r_printf(" - Group ID of current thread: %d\n", cpuInfo.currentGroup);
-    r_printf(" - Core ID of current thread: %d\n", cpuInfo.currentCoreNumber);
-    r_printf(" - CPU affinity mask of current thread: %#x\n", cpuInfo.currentThreadAffinity);
+    r_printf((" - Number of processor L1/L2/L3 caches: %d/%d/%d\n"), cpuInfo.processorL1CacheCount, cpuInfo.processorL2CacheCount, cpuInfo.processorL3CacheCount);
+
+    //r_printf(" - Group ID of current thread: %d\n", cpuInfo.currentGroup);
+    //r_printf(" - Core ID of current thread: %d\n", cpuInfo.currentCoreNumber);
+    //r_printf(" - CPU affinity mask of current thread: %#x\n", cpuInfo.currentThreadAffinity);
 
 }
 
- void CPU_ZERO(cpu_set_t* cpus) {
-    //cpus->cpu is a PROCESSRO_NUMBER; the reserved field must be sset to 0s; otherwise
-    //CreateRemoteTHreadEX fails.
-    //PROCESSOR_NUMBER procNum = {0,};
-    memset(cpus, 0, sizeof(cpu_set_t));
+ void   CPU_ZERO(cpu_set_t* cs) {
+    cs->core_count    = GetNumCores();
+    if (cs->core_count > 256) cs->core_count = 256; // bcz we use a int64 as the mask, so up to 64 cores are suppored
+    cs->core_mask[0] = cs->core_mask[1] = cs->core_mask[2] = cs->core_mask[3] = 0;
 }
- void CPU_SET(int i, cpu_set_t* cpus) {     
-    #ifdef WIN64_OS
-    cpus->ProcNumber.Group  = cpuInfo.cpuGroup[i];
-    cpus->ProcNumber.Number = cpuInfo.numCPUCoresToUseber[i];
-    #endif
+
+void    CPU_SET(int num, cpu_set_t* cs) {
+    num = num % cs->core_count;;
+    int grpId = num / 64;
+    int bitId = num - grpId * 64;
+    cs->core_mask[grpId] |= (1 << bitId);
 }
 
+ int   CPU_ISSET(int num, cpu_set_t* cs) {
+    num = num % cs->core_count;;
+    int grpId = num / 64;
+    int bitId = num - grpId * 64;
+    return (cs->core_mask[grpId] & (1 << bitId));
+}
+
+  int   CPU_get_first_bit_id(cpu_set_t* cs) {
+    int grpId = 0;
+    for (grpId = 0; grpId < 4; grpId++) {
+        if (cs->core_mask[grpId] != 0)   break;
+    }
+
+    if (grpId < 4) {
+        int      num = 0;
+        uint64_t mask = cs->core_mask[grpId];
+        for (num = 0; num < 64; num++) {
+            if (mask & (1 << num)) {
+                break;
+            }
+        }
+        return grpId * 64 + num;
+    }
+    else {
+        return 0;
+    }
+
+}
+ 
+
+ int pthread_attr_setaffinity_np(pthread_attr_t* attr, size_t cpusetsize, const cpu_set_t* cpuset) {
+     
+     if (cpuset == NULL)   return 0; 
+
+    //https://stackoverflow.com/questions/25472441/pthread-affinity-before-create-threads
+#ifdef WIN64_OS
+
+     if (attr->lpAttributeList != NULL) {
+         DeleteProcThreadAttributeList(attr->lpAttributeList);
+         free(attr->lpAttributeList);
+         attr->lpAttributeList = NULL;
+     }
+
+     DWORD  attributeCounts = 1L;
+     attr->lpAttributeList  = malloc(attr->sizeAttributeList);
+     InitializeProcThreadAttributeList(attr->lpAttributeList, attributeCounts, 0, &attr->sizeAttributeList);
+
+    int coreId                = CPU_get_first_bit_id(cpuset);    
+    attr->ProcNumber.Group    =   cpuInfo.cpuGroup[coreId];
+    attr->ProcNumber.Number   =   cpuInfo.coreIDinGroup[coreId];
+    attr->ProcNumber.Reserved =   0;    // PROCESSRO_NUMBER; the reserved field must be sset to 0s; otherwise CreateRemoteTHreadEX fails.
+    // https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/nf-processthreadsapi-updateprocthreadattribute
+    // ProcNumber must persit  until the attribute list is destroyed using the DeleteProcThreadAttributeList function.
+    // That is, when calling CreateRemoteThreadEx, ProcNumber must be sitll in the memoery, so we move it as fields of attr
+    BOOL fok = UpdateProcThreadAttribute( attr->lpAttributeList, 0L, PROC_THREAD_ATTRIBUTE_IDEAL_PROCESSOR,
+                                         &attr->ProcNumber, sizeof(PROCESSOR_NUMBER), NULL, NULL);
+    return fok;
+#else
+    //Do nothing
+    return 0;
+#endif
+}
 
  // pthread_create has a conflict with the pthread lib if provided/
  // instead of exploring options with weak symbol, I make it static here
-int  pthread_create0(pthread_t* tid,  const pthread_attr_t* attr, void* (*start) (void*), void* arg)
-{
+int  pthread_create(pthread_t* tid,  const pthread_attr_t* attr, void* (*start) (void*), void* arg) {
 
 #ifdef WIN64_OS
-    if (cpuFunc.CreateRemoteThreadEx == NULL) {
-        r_printf("the CreateRemoteThreadEx funnction is not detected!\n");
+    if (cpuFunc.CreateRemoteThreadEx == NULL || attr==NULL || attr->lpAttributeList==NULL ) {
+        // r_printf("the CreateRemoteThreadEx funnction is not detected!\n");
         *tid = CreateThread(NULL, NULL, (LPTHREAD_START_ROUTINE) start, arg, 0, 0);
     }  else {
         //https://docs.microsoft.com/en-us/windows/win32/procthread/thread-stack-size
         *tid = cpuFunc.CreateRemoteThreadEx(
             GetCurrentProcess(),
             (LPSECURITY_ATTRIBUTES)NULL,
-            (SIZE_T)attr->dwStackSize, // if 0, use the default stack size
-            (LPTHREAD_START_ROUTINE)start,
-            (LPVOID)arg,
-            (DWORD)0,
-            (LPPROC_THREAD_ATTRIBUTE_LIST)attr->lpAttributeList,
+            (SIZE_T) attr->dwStackSize, // if 0, use the default stack size
+            (LPTHREAD_START_ROUTINE) start,
+            (LPVOID) arg,
+            (DWORD) 0,
+            (LPPROC_THREAD_ATTRIBUTE_LIST) attr->lpAttributeList,
             (LPDWORD)NULL
         );
 
         //https://microsoft.public.win32.programmer.kernel.narkive.com/7QcTnq9M/createthread-fails-with-error-not-enough-memory
     }
 #else
-    * tid = CreateThread(NULL, attr->dwStackSize, (LPTHREAD_START_ROUTINE)start, arg, 0, 0);
+    if (attr!=NULL)
+        *tid = CreateThread(NULL, attr->dwStackSize, (LPTHREAD_START_ROUTINE)start, arg, 0, 0);
+    else
+        *tid = CreateThread(NULL, NULL,              (LPTHREAD_START_ROUTINE)start, arg, 0, 0);
 #endif
 
-    return 0;
+    // If failing, tid is NULL;  if susccess, return 0
+    return  (tid == NULL);               
 }
 
 
- 
-
 #endif
 
 
+
 #if defined(_WIN32) || defined(WIN64_OS)
 
     #if _WIN32_WINNT >= 0x0602
        //The function below is to get hte stackszie of the current thread.  
-        int get_thread_stacksize() {
+        int get_thread_stacksize(void) {
             ULONG_PTR lowLimit;
             ULONG_PTR highLimit; 
             GetCurrentThreadStackLimits(&lowLimit, &highLimit);
             return (highLimit - lowLimit);
         }
     #else
-       // https://www.xsprogram.com/content/can-i-get-the-limits-of-the-stack-in-c-c.html
-        int get_thread_stacksize() {
-             NT_TIB* tib = (NT_TIB*)NtCurrentTeb();
+       // https://stackoverflow.com/questions/28708213/can-i-get-the-limits-of-the-stack-in-c-c
+        #if defined(MSVC_COMPILER)
+        int get_thread_stacksize(void) {
+             NT_TIB* tib         = (NT_TIB*)NtCurrentTeb();
              LPVOID   StackLimit = tib->StackLimit;
              LPVOID   StackBase  = tib->StackBase;
              return  StackLimit;
         }
+        #elif  defined(GCC_COMPILER)
+
+            static INLINE unsigned __int64 readgsqword_bad(unsigned __int64 Offset) {
+                // this verseion will give a warning of  array subscript 0 is outside array bounds of 'long long unsigned int[0]' [-Warray-bounds]
+                // the bug has been reported at https://gcc.gnu.org/bugzilla/show_bug.cgi?id=105523
+                unsigned char ret;
+                __asm__( "mov{" "q" " %%" "gs" ":%[offset], %[ret] | %[ret], %%" "gs" ":%[offset]}" 
+                         : [ret] "=r" (ret) 
+                        : [offset] "m" ((*(unsigned __int64*)(size_t)Offset)));
+                return ret; 
+            }
+
+            static INLINE unsigned __int64  readgsqword_good(unsigned __int64 Offset) {
+                // this is a solution proposed here https://gcc.gnu.org/bugzilla/show_bug.cgi?id=104657
+                unsigned __int64 ret;
+                unsigned __int64 volatile Offset1 = Offset;
+                __asm__("mov{" "q" " %%" "gs" ":%[offset], %[ret] | %[ret], %%" "gs" ":%[offset]}"
+                    : [ret] "=r" (ret)
+                    : [offset] "m" ((*(unsigned __int64*)(size_t)Offset1)));
+                return ret;
+            }
+
+            int get_thread_stacksize(void) {
+                ///(struct _TEB *)__readgsqword(FIELD_OFFSET(NT_TIB, Self));
+                //NT_TIB* tib = (NT_TIB*)NtCurrentTeb();
+                NT_TIB* tib = (NT_TIB*)readgsqword_good(FIELD_OFFSET(NT_TIB, Self));
+                LPVOID   StackLimit = tib->StackLimit;
+                LPVOID   StackBase = tib->StackBase;
+                return  StackLimit;
+            }  
+       
+        
+       #else
+        int get_thread_stacksize(void) { 
+             return  0;
+        }
+       #endif
     #endif
 
+
+
     // On Windows, Seems like that there is no functions to get the default stack size;
      //, except parseing the PE's header: https://stackoverflow.com/questions/42420727/default-stack-size
     // A sloppy way to get the default stack size: create a thread and run GetCurrentTrheadLimits
-    static void * __getstacksize(void * arg) {  *((size_t*) arg)=get_thread_stacksize();  return 0; }
+    static void * __getstacksize(void * arg) {  
+        *((size_t*) arg)=get_thread_stacksize();  return 0; 
+    }
+
     int pthread_attr_getstacksize_win32(pthread_attr_t* attr, size_t* stacksize) {
-        static int default_stacksize=0;
+        static size_t default_stacksize=0;
         if (attr->dwStackSize > 0) {
             *stacksize = attr->dwStackSize;            
         } else{
             if (default_stacksize == 0) {
                 pthread_t tid =  CreateThread(NULL, 0, (LPTHREAD_START_ROUTINE)__getstacksize, stacksize, 0, 0);
                 pthread_join(tid, NULL);
                 default_stacksize = *stacksize;
@@ -573,28 +779,28 @@
 
         return 0;        
     }
     
 #elif defined(LINUX_OS) 
 
 //https://docs.oracle.com/cd/E88353_01/html/E37843/pthread-getattr-np-3c.html
-int get_thread_stacksize() {
+int get_thread_stacksize(void) {
 
     pthread_attr_t attr;
     size_t   stksize;
     void*    stkaddr;
     //pthread_getattr_np not available in Solaris as reported by R-hub
     (void)pthread_getattr_np(pthread_self(), &attr);
     (void)pthread_attr_getstack(&attr, &stkaddr, &stksize);
     (void)pthread_attr_destroy(&attr);
     return stksize;
 }
 
 #else // For non-windows systems, define a dummy function
 //pthread_getattr_np ; But not portable to Mac OS
 //pthread_self() 
-int get_thread_stacksize() {
+int get_thread_stacksize(void) {
 
     return  0;
     }
 #endif
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/abc_pthread.h` & `Rbeast-0.1.14/ext_src/abc_pthread.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #pragma once
 #include "abc_000_macro.h"
+#include <inttypes.h>
+
+extern int get_thread_stacksize(void);
+extern int GetNumCores(void);
 
-extern int get_thread_stacksize();
-extern int GetNumCores();
- 
  
 #if defined(WIN64_OS) || defined(WIN32_OS)
 
 //https://stackoverflow.com/questions/13828913/mingw-gcc-not-recognizing-memstatusex
 //https://docs.microsoft.com/en-us/windows/win32/winprog/using-the-windows-headers?redirectedfrom=MSDN
 
 //#undef   _WIN32_WINNT
@@ -70,230 +71,233 @@
 
 #endif
 
 #ifdef WIN64_OS
     #include "Processthreadsapi.h" //InitializeProcThreadAttributeList DeleteProcThreadAttributeList
 #endif
 
-typedef HANDLE        pthread_t;
+typedef HANDLE    pthread_t;
 typedef struct {
-                  LPPROC_THREAD_ATTRIBUTE_LIST lpAttributeList;
-	              SIZE_T                       dwStackSize;    
+         SIZE_T                       sizeAttributeList;
+         PPROC_THREAD_ATTRIBUTE_LIST  lpAttributeList;
+	     SIZE_T                       dwStackSize;    
+    #ifdef WIN64_OS
+	    PROCESSOR_NUMBER ProcNumber;
+    #else
+         void * ProcNumber;
+    #endif
 }   pthread_attr_t;
 
 typedef CRITICAL_SECTION   pthread_mutex_t;
 typedef int                pthread_mutexattr_t;
 typedef CONDITION_VARIABLE pthread_cond_t;
 typedef int                pthread_condattr_t;
 
-typedef struct {
-    #ifdef WIN64_OS
-	PROCESSOR_NUMBER ProcNumber;
-    #else
-    void * ProcNumber;
-    #endif
+
+ 
+
+typedef struct cpu_set {
+    int        core_count;
+    uint64_t   core_mask[4];
 } cpu_set_t;
 
+ 
+static INLINE int pthread_attr_init(pthread_attr_t * attr) {
 
-static INLINE int pthread_attr_init(pthread_attr_t * attr)
-{
-#ifdef WIN64_OS
-    attr->dwStackSize     = 0;
-    attr->lpAttributeList = NULL;
+    if (attr == NULL) return 0;
 
+    attr->dwStackSize      = 0;
+    attr->lpAttributeList  = NULL;
+    attr->sizeAttributeList = 0;
+
+#ifdef WIN64_OS    
     // stackoverflow.com/questions/25472441/pthread-affinity-before-create-threads
     DWORD  attributeCounts = 1L;
     SIZE_T size;
-    if (InitializeProcThreadAttributeList(NULL, attributeCounts, 0, &size)
-        || GetLastError() == ERROR_INSUFFICIENT_BUFFER)  {
-        attr->lpAttributeList =  malloc(size);
-        InitializeProcThreadAttributeList(attr->lpAttributeList, attributeCounts, 0, &size);
+    if ( InitializeProcThreadAttributeList(NULL, attributeCounts, 0, &size) || GetLastError() == ERROR_INSUFFICIENT_BUFFER)  {      
+        attr->sizeAttributeList        = size;
+       // Pm;u get the size of the mem needed for attributeLists
+       // The actual allocation will be done in pthread_setaffinity_np
     }
 #endif
     return 0;
 }
 
-static INLINE int	pthread_attr_setstacksize(pthread_attr_t* tattr, size_t  size) {
-       tattr->dwStackSize = size;
-       return 0;
-}
+static INLINE int	pthread_attr_setstacksize(pthread_attr_t* tattr, size_t  size) {  tattr->dwStackSize = size;    return 0;}
 
 // On windows,A sloppy way to get the default stack size: create a thread and run GetCurrentTrheadLimits
-static int pthread_attr_getstacksize(pthread_attr_t* attr, size_t* stacksize) {
-    return pthread_attr_getstacksize_win32(attr, stacksize);
-}
-
-static INLINE  int pthread_attr_destroy(pthread_attr_t* attr)
-{
-#ifdef WIN64_OS
+extern int pthread_attr_getstacksize_win32(pthread_attr_t* attr, size_t* stacksize);
+static INLINE int pthread_attr_getstacksize(pthread_attr_t* attr, size_t* stacksize) {    return pthread_attr_getstacksize_win32(attr, stacksize); }
+static INLINE int pthread_attr_destroy(pthread_attr_t* attr) {
+    #ifdef WIN64_OS
     if (attr->lpAttributeList != NULL) {
         DeleteProcThreadAttributeList(attr->lpAttributeList);
         free(attr->lpAttributeList);
     }    
-#endif
-    return 0;
-}
-
-//https://stackoverflow.com/questions/25472441/pthread-affinity-before-create-threads
-static INLINE  int pthread_attr_setaffinity_np ( pthread_attr_t* attr, size_t cpusetsize, const cpu_set_t* cpuset)
-{
-    #ifdef WIN64_OS
-    BOOL fok = UpdateProcThreadAttribute(
-                    attr->lpAttributeList,
-                    0L,
-                    PROC_THREAD_ATTRIBUTE_IDEAL_PROCESSOR,
-                    &( ((cpu_set_t *)cpuset)->ProcNumber),
-                    sizeof(PROCESSOR_NUMBER), NULL, NULL);
-    return fok;
-    #else
-    //Do notting
-    return 0;
     #endif
-}
-static int pthread_mutex_init(pthread_mutex_t* mutex, const pthread_mutexattr_t* attr) {
-	InitializeCriticalSection(mutex); 
     return 0;
 }
 
-static INLINE int pthread_mutex_destroy(pthread_mutex_t* mutex) {
-	DeleteCriticalSection(mutex);
-    return 0;
-}
-static INLINE int pthread_mutex_lock(pthread_mutex_t* mutex) {
-	EnterCriticalSection(mutex);
-    return 0;
-}
-static INLINE int pthread_mutex_unlock(pthread_mutex_t* mutex){
-	LeaveCriticalSection(mutex);
-    return 0;
-}
-static INLINE int pthread_cond_init(pthread_cond_t * cond, const pthread_condattr_t * attr) {
-	InitializeConditionVariable(cond);
-    return 0;
-}
+extern int pthread_attr_setaffinity_np(pthread_attr_t* attr, size_t cpusetsize, const cpu_set_t* cpuset);
 
-static INLINE int pthread_cond_wait(pthread_cond_t * cond, pthread_mutex_t * mutex) {
-	SleepConditionVariableCS(cond, mutex, INFINITE);
-    return 0;
-}
-static INLINE int pthread_cond_signal(pthread_cond_t * cond) {
-	WakeConditionVariable(cond);
-    return 0;
-}
+static INLINE int pthread_mutex_init(pthread_mutex_t* mutex, const pthread_mutexattr_t* attr) {    InitializeCriticalSection(mutex);    return 0;}
+static INLINE int pthread_mutex_destroy(pthread_mutex_t* mutex) {     DeleteCriticalSection(mutex);   return 0;}
+static INLINE int pthread_mutex_lock(pthread_mutex_t* mutex)    {     EnterCriticalSection(mutex);    return 0; }
+static INLINE int pthread_mutex_unlock(pthread_mutex_t* mutex)  {     LeaveCriticalSection(mutex);   return 0; }
+static INLINE int pthread_cond_init(pthread_cond_t * cond, const pthread_condattr_t * attr) {     InitializeConditionVariable(cond);  return 0;}
+static INLINE int pthread_cond_wait(pthread_cond_t * cond, pthread_mutex_t * mutex) {   SleepConditionVariableCS(cond, mutex, INFINITE);  return 0;}
+static INLINE int pthread_cond_signal(pthread_cond_t * cond) {   	WakeConditionVariable(cond);    return 0;}
 static INLINE int pthread_cond_destroy(pthread_cond_t * cond) {
 	//https:// stackoverflow.com/questions/28975958/why-does-windows-have-no-deleteconditionvariable-function-to-go-together-with
     return 0;
 }
-static INLINE void pthread_exit(void *value_ptr)
-{
+static INLINE void pthread_exit(void *value_ptr) {
 	//https:// stackoverflow.com/questions/11226072/windows-c-closing-thread-with-closehandle
 	//Closehandle doesn't destory the thread; it only destory the handle itself and the thread may still run and 
 	// we lose the handle to kil or wait on it
     //https:// stackoverflow.com/questions/3959473/must-i-closehandle-on-a-thread-handle
 }
 
 #define PTHREAD_CREATE_JOINABLE  1
-static INLINE int  pthread_attr_setdetachstate(pthread_attr_t * attr, int detachstate)
-{
-    return 0;
-}
-static INLINE int pthread_join(pthread_t thread, void **retvalue_ptr)
-{  //Even after the thread exited - its handle is valid. You can for instance query its return value
+static INLINE int         pthread_attr_setdetachstate(pthread_attr_t * attr, int detachstate) {   return 0;}
+static INLINE  pthread_t  pthread_self(void) { return (pthread_t)GetCurrentThreadId(); }
+static INLINE int pthread_join(pthread_t thread, void **retvalue_ptr) {
+  //Even after the thread exited - its handle is valid. You can for instance query its return value
 	WaitForSingleObject(thread, INFINITE);
     if (retvalue_ptr) {
         //https://stackoverflow.com/questions/7100441/how-can-you-get-the-return-value-of-a-windows-thread
         GetExitCodeThread(thread, retvalue_ptr);
     }
 	CloseHandle(thread);
     return 0;
 }
-static INLINE  pthread_t  pthread_self(void) {
-    return (pthread_t) GetCurrentThreadId();
-}
 
-extern int  GetCPUInfo();
-extern void PrintCPUInfo();
+extern int  GetCPUInfo(void);
+extern void PrintCPUInfo(void);
 
 extern void CPU_ZERO(cpu_set_t* cpus);
 extern void CPU_SET(int i, cpu_set_t* cpus);
+extern int  CPU_ISSET(int i, cpu_set_t* cpus);
 
-extern int  pthread_create0(pthread_t* tid, const pthread_attr_t* attr, void* (*start) (void*), void* arg);
-
-static int  pthread_create(pthread_t* tid, const pthread_attr_t* attr, void* (*start) (void*), void* arg)
-{
-    pthread_create0(tid, attr, start, arg);
-    return 0;
-}
+extern int  pthread_create(pthread_t* tid, const pthread_attr_t* attr, void* (*start) (void*), void* arg);
+extern int  sched_getcpu(void);
 
 #elif   defined(LINUX_OS)
     
         //you have to define_GNU_SOURCE before anything else
         //https://stackoverflow.com/questions/1407786/how-to-set-cpu-affinity-of-a-particular-pthread
         //https://stackoverflow.com/questions/7296963/gnu-source-and-use-gnu/7297011#7297011
         //https://stackoverflow.com/questions/24034631/error-message-undefined-reference-for-cpu-zero/24034698
 	    #ifndef _GNU_SOURCE
 		    #define _GNU_SOURCE
 	    #endif
         #include <sched.h>  ////cpu_set_t , CPU_SET
 	    #include <pthread.h>
 
-
-#elif   defined(MAC_OS) 
-
+#elif    defined(MAC_OS) 
+ 
     #include <mach/thread_policy.h> // for thread_port_t etc. //https://github.com/xoreaxeaxeax/sandsifter/issues/3
+
+   //https://lists.apple.com/archives/darwin-kernel/2014/Nov/msg00003.html
+   //protoptye for thread_policy_st moved here
+    #include <mach/thread_act.h> 
+    #include <sys/sysctl.h> // header for systclbyname()
     #include <pthread.h>
    //https://stackoverflow.com/questions/32282270/c99-error-unknown-type-name-pid-t
     #include <sys/types.h> // pid_t
     #include <unistd.h>   // pid_t
-    #include <inttypes.h>
     #define SYSCTL_CORE_COUNT   "machdep.cpu.core_count"
 
-    typedef struct cpu_set {    uint32_t    count; } cpu_set_t;
+   // Borrowed from http://www.hybridkernel.com/2015/01/18/binding_threads_to_cores_osx.html
+   // https://developer.apple.com/library/archive/releasenotes/Performance/RN-AffinityAPI/
+typedef struct cpu_set { 
+        int        core_count; 
+        uint64_t   core_mask[4]; } cpu_set_t;
 
     static inline void   CPU_ZERO(cpu_set_t* cs) {
-        cs->count = 0; 
+        cs->core_count   = GetNumCores();
+        if (cs->core_count > 256) cs->core_count = 256; // bcz we use a int64 as the mask, so up to 64 cores are suppored
+        cs->core_mask[0] = cs->core_mask[1]= cs->core_mask[2]= cs->core_mask[3]= 0;
     }
 
-    static inline void    CPU_SET(int num, cpu_set_t* cs) { 
-        num = num % GetNumCores(); cs->count |= (1 << num); 
+    static inline void    CPU_SET(int num, cpu_set_t* cs) {           
+        num = num % cs->core_count;;
+        int grpId = num / 64;
+        int bitId = num - grpId * 64;
+        cs->core_mask[grpId] |= (1 << bitId);
     }
 
     static inline int     CPU_ISSET(int num, cpu_set_t* cs) {
-        num = num % GetNumCores(); return (cs->count & (1 << num)); 
+        num       = num % cs->core_count;;
+        int grpId = num / 64;
+        int bitId = num - grpId * 64;
+        return (cs->core_mask[grpId] & (1 << bitId));
     }
 
-    static int sched_getaffinity(pid_t pid, size_t cpu_size, cpu_set_t* cpu_set)    {
+    static inline int     CPU_get_first_bit_id(cpu_set_t* cs) {
+        int grpId = 0;
+        for (grpId = 0; grpId < 4; grpId++) {
+            if (cs->core_mask[grpId] != 0)   break;
+        }
+
+        if (grpId < 4) {
+            int      num  = 0;
+            uint64_t mask = cs->core_mask[grpId];
+            for (num = 0; num < 64  ; num++) {
+                if (mask & (1 << num)) {
+                    break;
+                }
+            }
+            return grpId * 64 + num;
+        }
+        else {
+            return 0;
+        }
+
+    }
+    static inline int sched_getaffinity(pid_t pid, size_t cpu_size, cpu_set_t* cpu_set)    {
         int32_t core_count = 0;
-        size_t  len = sizeof(core_count);
+        size_t  len        = sizeof(core_count);
         int ret = sysctlbyname(SYSCTL_CORE_COUNT, &core_count, &len, 0, 0);
         if (ret) {
-            //printf("error while get core count %d\n", ret);
-            return -1;
+            return -1;             //printf("error while get core count %d\n", ret);
         }
-        cpu_set->count = 0;
+        CPU_ZERO(cpu_set);
         for (int i = 0; i < core_count; i++) {
-            cpu_set->count |= (1 << i);
+            CPU_SET(i, cpu_set);
         }
 
         return 0;
     }
 
-    static int pthread_setaffinity_np(pthread_t thread, size_t cpu_size,   cpu_set_t *cpu_set) {
-
-            thread_port_t mach_thread;
-            int core = 0;
+    // /stackoverflow.com/questions/33745364/sched-getcpu-equivalent-for-os-x
+    #include <cpuid.h>
+    #define CPUID(INFO, LEAF, SUBLEAF) __cpuid_count(LEAF, SUBLEAF, INFO[0], INFO[1], INFO[2], INFO[3])
+
+    static int sched_getcpu() {
+        uint32_t CPUInfo[4];
+        CPUID(CPUInfo, 1, 0);
+        /* CPUInfo[1] is EBX, bits 24-31 are APIC ID */
+        int CPU;
+        if ((CPUInfo[3] & (1 << 9)) == 0) {
+            CPU = -1;  /* no APIC on chip */
+        }
+        else {
+            CPU = (unsigned)CPUInfo[1] >> 24;
+        }
+        return CPU;
+    }
 
-            for (core = 0; core < 8 * cpu_size; core++) {
-                  if (CPU_ISSET(core, cpu_set)) break;
-            }
-            //printf("binding to core %d\n", core);
-            thread_affinity_policy_data_t policy = { core };
-            mach_thread = pthread_mach_thread_np(thread);
-            thread_policy_set(mach_thread, THREAD_AFFINITY_POLICY,
-                            (thread_policy_t)&policy, 1);
+    static int pthread_setaffinity_np(pthread_t thread, size_t cpu_size,   cpu_set_t *cpu_set) {            
+            thread_port_t mach_thread = pthread_mach_thread_np(thread);             
+            int core = CPU_get_first_bit_id(cpu_set);
+            // binding to core %d\n"
+            thread_affinity_policy_data_t policy;
+            policy.affinity_tag                 = core;            
+            thread_policy_set(mach_thread, THREAD_AFFINITY_POLICY, (thread_policy_t)&policy, 1);
             return 0;
         }
 
 #elif  defined(SOLARIS_OS)
     //you have to define_GNU_SOURCE before anything else
     //https://stackoverflow.com/questions/1407786/how-to-set-cpu-affinity-of-a-particular-pthread
     //https://stackoverflow.com/questions/7296963/gnu-source-and-use-gnu/7297011#7297011
```

### Comparing `Rbeast-0.1.13/ext_src/abc_rand_mkl.h` & `Rbeast-0.1.14/ext_src/abc_rand_mkl.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_rand_pcg_global.c` & `Rbeast-0.1.14/ext_src/abc_rand_pcg_global.c`

 * *Files 11% similar despite different names*

```diff
@@ -7,1013 +7,1141 @@
 00000060: 2261 6263 5f64 6174 6174 7970 652e 6822  "abc_datatype.h"
 00000070: 200d 0a23 696e 636c 7564 6520 2261 6263   ..#include "abc
 00000080: 5f72 616e 645f 7063 675f 676c 6f62 616c  _rand_pcg_global
 00000090: 2e68 2220 0d0a 2369 6e63 6c75 6465 2022  .h" ..#include "
 000000a0: 6162 635f 6964 655f 7574 696c 2e68 2220  abc_ide_util.h" 
 000000b0: 2020 202f 2f72 5f70 7269 6e74 660d 0a23     //r_printf..#
 000000c0: 696e 636c 7564 6520 2261 6263 5f76 6563  include "abc_vec
-000000d0: 2e68 2220 200d 0a0d 0a0d 0a20 0d0a 0d0a  .h"  ...... ....
-000000e0: 2f2f 6874 7470 733a 2f2f 6861 6c2e 6172  //https://hal.ar
-000000f0: 6368 6976 6573 2d6f 7576 6572 7465 732e  chives-ouvertes.
-00000100: 6672 2f68 616c 2d30 3237 3030 3739 312f  fr/hal-02700791/
-00000110: 646f 6375 6d65 6e74 3a20 6120 6e69 6365  document: a nice
-00000120: 2069 6e74 726f 2074 6f20 7468 6520 7063   intro to the pc
-00000130: 6720 616c 670d 0a2f 2a50 7261 6374 6963  g alg../*Practic
-00000140: 616c 2073 6565 642d 7265 636f 7665 7279  al seed-recovery
-00000150: 2066 6f72 2074 6865 2050 4347 2050 7365   for the PCG Pse
-00000160: 7564 6f2d 5261 6e64 6f6d 204e 756d 6272  udo-Random Numbr
-00000170: 2047 656e 6572 6174 6f72 2a2f 0d0a 0d0a   Generator*/....
-00000180: 2f2a 0d0a 496e 7465 726e 616c 6c79 2c20  /*..Internally, 
-00000190: 7468 6973 2052 4e47 2075 7365 7320 7477  this RNG uses tw
-000001a0: 6f20 3634 2d62 6974 2069 6e74 6567 6572  o 64-bit integer
-000001b0: 7320 666f 7220 6974 7320 696e 7465 726e  s for its intern
-000001c0: 616c 2073 7461 7465 2c20 636f 6e73 6973  al state, consis
-000001d0: 7469 6e67 206f 663a 0d0a 7468 6520 6375  ting of:..the cu
-000001e0: 7272 656e 7420 7374 6174 6520 9720 7468  rrent state . th
-000001f0: 6520 524e 4720 6974 6572 6174 6573 2074  e RNG iterates t
-00000200: 6872 6f75 6768 2061 6c6c 2032 3634 2070  hrough all 264 p
-00000210: 6f73 7369 626c 6520 696e 7465 726e 616c  ossible internal
-00000220: 2073 7461 7465 732e 0d0a 7468 6520 524e   states...the RN
-00000230: 472d 7365 7175 656e 6365 2063 6f6e 7374  G-sequence const
-00000240: 616e 7420 9720 6120 7661 6c75 6520 7468  ant . a value th
-00000250: 6174 2064 6566 696e 6573 2077 6869 6368  at defines which
-00000260: 206f 6620 3236 3320 706f 7373 6962 6c65   of 263 possible
-00000270: 2072 616e 646f 6d20 7365 7175 656e 6365   random sequence
-00000280: 730d 0a74 6865 2063 7572 7265 6e74 2073  s..the current s
-00000290: 7461 7465 2069 7320 6974 6572 6174 696e  tate is iteratin
-000002a0: 6720 7468 726f 7567 683b 2069 7420 686f  g through; it ho
-000002b0: 6c64 7320 7468 6520 7361 6d65 2076 616c  lds the same val
-000002c0: 7565 206f 7665 7220 7468 6520 6c69 6665  ue over the life
-000002d0: 7469 6d65 206f 6620 7468 6520 524e 472e  time of the RNG.
-000002e0: 0d0a 2a2f 0d0a 0d0a 2f2a 0d0a 466f 7220  ..*/..../*..For 
-000002f0: 7468 6973 2067 656e 6572 6174 6f72 2c20  this generator, 
-00000300: 7468 6572 6520 6172 6520 325e 3633 2070  there are 2^63 p
-00000310: 6f73 7369 626c 6520 7365 7175 656e 6365  ossible sequence
-00000320: 7320 6f66 2070 7365 7564 6f72 616e 646f  s of pseudorando
-00000330: 6d20 6e75 6d62 6572 732e 2045 6163 6820  m numbers. Each 
-00000340: 7365 7175 656e 6365 2069 730d 0a65 6e74  sequence is..ent
-00000350: 6972 656c 7920 6469 7374 696e 6374 2061  irely distinct a
-00000360: 6e64 2068 6173 2061 2070 6572 696f 6420  nd has a period 
-00000370: 6f66 2032 5e36 342e 2054 6865 2069 6e69  of 2^64. The ini
-00000380: 7473 6571 2061 7267 756d 656e 7420 7365  tseq argument se
-00000390: 6c65 6374 7320 7768 6963 6820 7374 7265  lects which stre
-000003a0: 616d 2079 6f75 2077 696c 6c20 7573 652e  am you will use.
-000003b0: 200d 0a54 6865 2069 6e69 7473 7461 7465   ..The initstate
-000003c0: 2061 7267 756d 656e 7420 7370 6563 6966   argument specif
-000003d0: 6965 7320 7768 6572 6520 796f 7520 6172  ies where you ar
-000003e0: 6520 696e 2074 6861 7420 3236 3420 7065  e in that 264 pe
-000003f0: 7269 6f64 2e0d 0a2a 2f0d 0a0d 0a23 6465  riod...*/....#de
-00000400: 6669 6e65 2050 4347 5f44 4546 4155 4c54  fine PCG_DEFAULT
-00000410: 5f4d 554c 5449 504c 4945 525f 3634 2020  _MULTIPLIER_64  
-00000420: 3633 3634 3133 3632 3233 3834 3637 3933  6364136223846793
-00000430: 3030 3555 4c4c 202f 2f68 7474 7073 3a2f  005ULL //https:/
-00000440: 2f67 6974 6875 622e 636f 6d2f 696d 6e65  /github.com/imne
-00000450: 6d65 2f70 6367 2d63 2d62 6173 6963 2f62  me/pcg-c-basic/b
-00000460: 6c6f 622f 6d61 7374 6572 2f70 6367 5f62  lob/master/pcg_b
-00000470: 6173 6963 2e63 0d0a 2364 6566 696e 6520  asic.c..#define 
-00000480: 5043 475f 4445 4641 554c 545f 494e 4352  PCG_DEFAULT_INCR
-00000490: 454d 454e 545f 3634 2020 2031 3434 3236  EMENT_64   14426
-000004a0: 3935 3034 3038 3838 3936 3334 3037 554c  95040888963407UL
-000004b0: 4c20 2f2f 2f2f 6874 7470 733a 2f2f 6769  L ////https://gi
-000004c0: 7468 7562 2e63 6f6d 2f69 6d6e 656d 652f  thub.com/imneme/
-000004d0: 7063 672d 632f 626c 6f62 2f6d 6173 7465  pcg-c/blob/maste
-000004e0: 722f 696e 636c 7564 652f 7063 675f 7661  r/include/pcg_va
-000004f0: 7269 616e 7473 2e68 0d0a 0d0a 0d0a 2f2f  riants.h......//
-00000500: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000510: 6f6d 2f69 6d6e 656d 652f 7063 672d 632d  om/imneme/pcg-c-
-00000520: 6261 7369 632f 626c 6f62 2f6d 6173 7465  basic/blob/maste
-00000530: 722f 7063 675f 6261 7369 632e 680d 0a23  r/pcg_basic.h..#
-00000540: 6465 6669 6e65 2050 4347 5f44 4546 4155  define PCG_DEFAU
-00000550: 4c54 5f47 4c4f 4241 4c5f 5354 4154 455f  LT_GLOBAL_STATE_
-00000560: 3634 2020 2020 2030 7838 3533 6334 3965  64     0x853c49e
-00000570: 3637 3438 6665 6139 6255 4c4c 0d0a 2364  6748fea9bULL..#d
-00000580: 6566 696e 6520 5043 475f 4445 4641 554c  efine PCG_DEFAUL
-00000590: 545f 474c 4f42 414c 5f49 4e43 5245 4d45  T_GLOBAL_INCREME
-000005a0: 4e54 5f36 3420 3078 6461 3365 3339 6362  NT_64 0xda3e39cb
-000005b0: 3934 6239 3562 6462 554c 4c0d 0a0d 0a2f  94b95bdbULL..../
-000005c0: 2f20 4c69 6e65 6172 2043 6f6e 6772 7565  / Linear Congrue
-000005d0: 6e74 6961 6c20 4765 6e65 7261 746f 7220  ntial Generator 
-000005e0: 284c 4347 293a 0d0a 2f2f 2058 2020 2020  (LCG):..// X    
-000005f0: 203d 2020 5820 2020 202a 204d 554c 5449   =  X    * MULTI
-00000600: 504c 4945 5220 2b20 494e 4352 454d 454e  PLIER + INCREMEN
-00000610: 5428 7368 6966 742f 706c 7573 2f73 7461  T(shift/plus/sta
-00000620: 7465 2e69 6e63 2920 6d6f 6420 325e 3634  te.inc) mod 2^64
-00000630: 0d0a 2f2f 2053 7461 7465 203d 2020 5374  ..// State =  St
-00000640: 6174 652a 204d 554c 5449 504c 4945 5220  ate* MULTIPLIER 
-00000650: 2b20 494e 4352 454d 454e 5428 7368 6966  + INCREMENT(shif
-00000660: 742f 706c 7573 2f49 4e43 2920 2020 2020  t/plus/INC)     
-00000670: 2020 6d6f 6420 325e 3634 0d0a 0d0a 0d0a    mod 2^64......
-00000680: 7479 7065 6465 6620 7374 7275 6374 2070  typedef struct p
-00000690: 6367 3332 5f72 616e 646f 6d5f 7374 7275  cg32_random_stru
-000006a0: 6374 207b 2009 2f2f 6874 7470 733a 2f2f  ct { .//https://
-000006b0: 6769 7468 7562 2e63 6f6d 2f69 6d6e 656d  github.com/imnem
-000006c0: 652f 7063 672d 632d 6261 7369 632f 626c  e/pcg-c-basic/bl
-000006d0: 6f62 2f6d 6173 7465 722f 7063 675f 6261  ob/master/pcg_ba
-000006e0: 7369 632e 680d 0a09 5536 3420 7374 6174  sic.h...U64 stat
-000006f0: 653b 202f 2f2f 2052 4e47 2073 7461 7465  e; /// RNG state
-00000700: 2e41 6c6c 2076 616c 7565 7320 6172 6520  .All values are 
-00000710: 706f 7373 6962 6c65 2e0d 0a09 5536 3420  possible....U64 
-00000720: 696e 633b 2020 202f 2f20 436f 6e74 726f  inc;   // Contro
-00000730: 6c73 2077 6869 6368 2052 4e47 2073 6571  ls which RNG seq
-00000740: 7565 6e63 6520 2873 7472 6561 6d29 2069  uence (stream) i
-00000750: 730d 0a09 0909 2020 202f 2f20 7365 6c65  s.....   // sele
-00000760: 6374 6564 2e20 4d75 7374 202a 616c 7761  cted. Must *alwa
-00000770: 7973 2a20 6265 206f 6464 2e0d 0a7d 2070  ys* be odd...} p
-00000780: 6367 3332 5f72 616e 646f 6d5f 743b 0d0a  cg32_random_t;..
-00000790: 0d0a 7374 6174 6963 2070 6367 3332 5f72  ..static pcg32_r
-000007a0: 616e 646f 6d5f 7420 676c 6f62 616c 5f73  andom_t global_s
-000007b0: 7461 7465 203d 207b 0d0a 092e 7374 6174  tate = {....stat
-000007c0: 653d 2050 4347 5f44 4546 4155 4c54 5f47  e= PCG_DEFAULT_G
-000007d0: 4c4f 4241 4c5f 5354 4154 455f 3634 2c0d  LOBAL_STATE_64,.
-000007e0: 0a09 2e69 6e63 2020 3d20 5043 475f 4445  ...inc  = PCG_DE
-000007f0: 4641 554c 545f 474c 4f42 414c 5f49 4e43  FAULT_GLOBAL_INC
-00000800: 5245 4d45 4e54 5f36 3420 7d3b 0d0a 0d0a  REMENT_64 };....
-00000810: 766f 6964 2070 6367 5f73 6574 5f73 6565  void pcg_set_see
-00000820: 6428 5536 3420 696e 6974 7374 6174 652c  d(U64 initstate,
-00000830: 2055 3634 2069 6e69 7473 6571 290d 0a7b   U64 initseq)..{
-00000840: 090d 0a09 696e 6974 7374 6174 6520 3d20  ....initstate = 
-00000850: 696e 6974 7374 6174 6520 2620 696e 6974  initstate & init
-00000860: 7365 713b 202f 2f41 6464 6564 2062 637a  seq; //Added bcz
-00000870: 206f 6e6c 7920 696e 6974 7365 7120 6973   only initseq is
-00000880: 2073 7570 706c 6965 6420 6173 2061 2073   supplied as a s
-00000890: 6565 642e 2057 6520 7275 6e20 696e 6974  eed. We run init
-000008a0: 7365 7120 746f 2072 616e 646f 6d69 7a65  seq to randomize
-000008b0: 2069 6e69 7473 7461 7465 2061 206c 6974   initstate a lit
-000008c0: 746c 6520 6269 740d 0a0d 0a09 696e 6974  tle bit.....init
-000008d0: 7374 6174 6520 3d20 696e 6974 7374 6174  state = initstat
-000008e0: 6520 3d3d 2030 203f 2050 4347 5f44 4546  e == 0 ? PCG_DEF
-000008f0: 4155 4c54 5f47 4c4f 4241 4c5f 5354 4154  AULT_GLOBAL_STAT
-00000900: 455f 3634 2020 2020 3a20 696e 6974 7374  E_64    : initst
-00000910: 6174 653b 0d0a 0969 6e69 7473 6571 2020  ate;...initseq  
-00000920: 203d 2069 6e69 7473 6571 203d 3d20 3020   = initseq == 0 
-00000930: 2020 3f20 5043 475f 4445 4641 554c 545f    ? PCG_DEFAULT_
-00000940: 474c 4f42 414c 5f49 4e43 5245 4d45 4e54  GLOBAL_INCREMENT
-00000950: 5f36 3420 3a20 696e 6974 7365 713b 0d0a  _64 : initseq;..
-00000960: 0d0a 0967 6c6f 6261 6c5f 7374 6174 652e  ...global_state.
-00000970: 7374 6174 6520 3d20 3055 3b0d 0a09 676c  state = 0U;...gl
-00000980: 6f62 616c 5f73 7461 7465 2e69 6e63 2020  obal_state.inc  
-00000990: 203d 2028 696e 6974 7365 7120 3c3c 2031   = (initseq << 1
-000009a0: 7529 207c 2031 753b 2020 092f 2f69 6e63  u) | 1u;  .//inc
-000009b0: 206d 7573 7420 6265 2061 6e20 6f64 6420   must be an odd 
-000009c0: 6e75 6d62 6572 0d0a 0d0a 0955 3332 2072  number.....U32 r
-000009d0: 6e64 3b0d 0a09 7063 675f 7261 6e64 6f6d  nd;...pcg_random
-000009e0: 2826 726e 642c 2031 293b 0d0a 0967 6c6f  (&rnd, 1);...glo
-000009f0: 6261 6c5f 7374 6174 652e 7374 6174 6520  bal_state.state 
-00000a00: 2b3d 2069 6e69 7473 7461 7465 3b0d 0a09  += initstate;...
-00000a10: 7063 675f 7261 6e64 6f6d 2826 726e 642c  pcg_random(&rnd,
-00000a20: 2031 293b 0d0a 7d0d 0a76 6f69 6420 7063   1);..}..void pc
-00000a30: 675f 7072 696e 745f 7374 6174 6528 2920  g_print_state() 
-00000a40: 7b72 5f70 7269 6e74 6628 2273 7461 7465  {r_printf("state
-00000a50: 3a20 2533 3022 2050 5249 7536 3420 2220  : %30" PRIu64 " 
-00000a60: 696e 633a 2025 3330 2220 2050 5249 7536  inc: %30"  PRIu6
-00000a70: 3420 225c 6e22 2c20 676c 6f62 616c 5f73  4 "\n", global_s
-00000a80: 7461 7465 2e73 7461 7465 2c20 676c 6f62  tate.state, glob
-00000a90: 616c 5f73 7461 7465 2e69 6e63 293b 7d0d  al_state.inc);}.
-00000aa0: 0a0d 0a2f 2f20 7063 6733 325f 7261 6e64  ...// pcg32_rand
-00000ab0: 6f6d 5f72 2872 6e67 290d 0a2f 2f20 2020  om_r(rng)..//   
-00000ac0: 4765 6e65 7261 7465 2061 2075 6e69 666f  Generate a unifo
-00000ad0: 726d 6c79 2064 6973 7472 6962 7574 6564  rmly distributed
-00000ae0: 2033 322d 6269 7420 7261 6e64 6f6d 206e   32-bit random n
-00000af0: 756d 6265 720d 0a76 6f69 6420 7063 675f  umber..void pcg_
-00000b00: 7261 6e64 6f6d 2855 3332 5054 5220 726e  random(U32PTR rn
-00000b10: 642c 2049 3332 204e 290d 0a7b 0d0a 0955  d, I32 N)..{...U
-00000b20: 3634 206f 6c64 7374 6174 6520 3d20 676c  64 oldstate = gl
-00000b30: 6f62 616c 5f73 7461 7465 2e73 7461 7465  obal_state.state
-00000b40: 3b0d 0a09 5536 3420 7368 6966 7420 2020  ;...U64 shift   
-00000b50: 203d 2067 6c6f 6261 6c5f 7374 6174 652e   = global_state.
-00000b60: 696e 633b 0d0a 0d0a 0966 6f72 2028 696e  inc;.....for (in
-00000b70: 7420 6920 3d20 303b 2069 203c 204e 3b20  t i = 0; i < N; 
-00000b80: 692b 2b29 207b 0d0a 0909 5533 3220 786f  i++) {....U32 xo
-00000b90: 7273 6869 6674 6564 203d 2020 2020 2028  rshifted =     (
-00000ba0: 286f 6c64 7374 6174 6520 3e3e 2031 3875  (oldstate >> 18u
-00000bb0: 2920 5e20 6f6c 6473 7461 7465 2920 3e3e  ) ^ oldstate) >>
-00000bc0: 2032 3775 2020 203b 0d0a 0909 5533 3220   27u   ;....U32 
-00000bd0: 726f 7420 3d20 6f6c 6473 7461 7465 203e  rot = oldstate >
-00000be0: 3e20 3539 753b 0d0a 0909 2f2f 2a72 6e64  > 59u;....//*rnd
-00000bf0: 2b2b 203d 2028 786f 7273 6869 6674 6564  ++ = (xorshifted
-00000c00: 203e 3e20 726f 7429 207c 2028 786f 7273   >> rot) | (xors
-00000c10: 6869 6674 6564 203c 3c20 2828 2d72 6f74  hifted << ((-rot
-00000c20: 2920 2620 3331 2929 3b0d 0a09 092a 726e  ) & 31));....*rn
-00000c30: 642b 2b20 3d20 2878 6f72 7368 6966 7465  d++ = (xorshifte
-00000c40: 6420 3e3e 2072 6f74 2920 7c20 2878 6f72  d >> rot) | (xor
-00000c50: 7368 6966 7465 6420 3c3c 2028 282d 202a  shifted << ((- *
-00000c60: 2828 4933 322a 2928 2672 6f74 2929 2020  ((I32*)(&rot))  
-00000c70: 2920 2620 3331 2929 3b0d 0a09 096f 6c64  ) & 31));....old
-00000c80: 7374 6174 6520 3d20 6f6c 6473 7461 7465  state = oldstate
-00000c90: 202a 2050 4347 5f44 4546 4155 4c54 5f4d   * PCG_DEFAULT_M
-00000ca0: 554c 5449 504c 4945 525f 3634 202b 2073  ULTIPLIER_64 + s
-00000cb0: 6869 6674 3b0d 0a09 7d0d 0a09 676c 6f62  hift;...}...glob
-00000cc0: 616c 5f73 7461 7465 2e73 7461 7465 203d  al_state.state =
-00000cd0: 206f 6c64 7374 6174 653b 0d0a 7d0d 0a0d   oldstate;..}...
-00000ce0: 0a2f 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ./**************
-00000cf0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000d00: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000d10: 2f0d 0a2f 2f20 4e6f 206e 6565 6420 746f  /..// No need to
-00000d20: 2065 7870 6f72 7420 7468 6973 2066 756e   export this fun
-00000d30: 630d 0a55 3634 2070 6367 5f61 6476 616e  c..U64 pcg_advan
-00000d40: 6365 5f6c 6367 5f36 3428 5536 3420 7374  ce_lcg_64(U64 st
-00000d50: 6174 652c 2055 3634 2064 656c 7461 2c20  ate, U64 delta, 
-00000d60: 5536 3420 6375 725f 6d75 6c74 2c20 5536  U64 cur_mult, U6
-00000d70: 3420 6375 725f 706c 7573 290d 0a7b 2020  4 cur_plus)..{  
-00000d80: 200d 0a09 2f2f 4164 7661 6e63 6520 7468   ...//Advance th
-00000d90: 6520 7374 6174 6520 6279 2061 2074 6f74  e state by a tot
-00000da0: 616c 206f 6620 6465 6c74 6120 7374 6570  al of delta step
-00000db0: 730d 0a09 2f2f 6874 7470 733a 2f2f 6769  s...//https://gi
-00000dc0: 7468 7562 2e63 6f6d 2f69 6d6e 656d 652f  thub.com/imneme/
-00000dd0: 7063 672d 632f 626c 6f62 2f6d 6173 7465  pcg-c/blob/maste
-00000de0: 722f 7372 632f 7063 672d 6164 7661 6e63  r/src/pcg-advanc
-00000df0: 652d 3634 2e63 0d0a 0955 3634 2061 6363  e-64.c...U64 acc
-00000e00: 5f6d 756c 7420 3d20 3175 3b0d 0a09 5536  _mult = 1u;...U6
-00000e10: 3420 6163 635f 706c 7573 203d 2030 753b  4 acc_plus = 0u;
-00000e20: 0d0a 0977 6869 6c65 2028 6465 6c74 6120  ...while (delta 
-00000e30: 3e20 3029 207b 0d0a 0909 6966 2028 6465  > 0) {....if (de
-00000e40: 6c74 6120 2620 3129 207b 0d0a 0909 0961  lta & 1) {.....a
-00000e50: 6363 5f6d 756c 7420 2a3d 2063 7572 5f6d  cc_mult *= cur_m
-00000e60: 756c 743b 0d0a 0909 0961 6363 5f70 6c75  ult;.....acc_plu
-00000e70: 7320 3d20 6163 635f 706c 7573 202a 2063  s = acc_plus * c
-00000e80: 7572 5f6d 756c 7420 2b20 6375 725f 706c  ur_mult + cur_pl
-00000e90: 7573 3b0d 0a09 097d 0d0a 0909 6375 725f  us;....}....cur_
-00000ea0: 706c 7573 203d 2028 6375 725f 6d75 6c74  plus = (cur_mult
-00000eb0: 202b 2031 2920 2a20 6375 725f 706c 7573   + 1) * cur_plus
-00000ec0: 3b0d 0a09 0963 7572 5f6d 756c 7420 2a3d  ;....cur_mult *=
-00000ed0: 2063 7572 5f6d 756c 743b 0d0a 0909 6465   cur_mult;....de
-00000ee0: 6c74 6120 2f3d 2032 3b0d 0a09 7d0d 0a09  lta /= 2;...}...
-00000ef0: 7265 7475 726e 2061 6363 5f6d 756c 7420  return acc_mult 
-00000f00: 2a20 7374 6174 6520 2b20 6163 635f 706c  * state + acc_pl
-00000f10: 7573 3b0d 0a7d 0d0a 766f 6964 2070 6367  us;..}..void pcg
-00000f20: 5f67 6574 5f6c 6367 5f6d 756c 7469 706c  _get_lcg_multipl
-00000f30: 6965 725f 7368 6966 745f 6d75 6c74 6973  ier_shift_multis
-00000f40: 7465 7028 2049 3332 2064 656c 7461 2c20  tep( I32 delta, 
-00000f50: 5536 3420 6375 725f 6d75 6c74 2c20 5536  U64 cur_mult, U6
-00000f60: 3420 6375 725f 706c 7573 2c20 5536 3420  4 cur_plus, U64 
-00000f70: 2a20 6d75 6c74 2c20 5536 3420 2a73 6869  * mult, U64 *shi
-00000f80: 6674 2920 0d0a 7b0d 0a09 2f2f 2046 696e  ft) ..{...// Fin
-00000f90: 6420 7468 6520 6d75 6c74 6c69 706c 6965  d the multliplie
-00000fa0: 7220 616e 6420 7368 6966 7420 2870 6c75  r and shift (plu
-00000fb0: 7329 2066 6f72 2061 206d 756c 7469 2d73  s) for a multi-s
-00000fc0: 7465 7020 6164 7661 6e63 650d 0a0d 0a09  tep advance.....
-00000fd0: 2f2f 4933 3220 6465 6c74 6120 3d20 343b  //I32 delta = 4;
-00000fe0: 202f 2f4d 6f76 6520 666f 7277 6172 6420   //Move forward 
-00000ff0: 6279 2034 2073 7465 7073 0d0a 092f 2f55  by 4 steps...//U
-00001000: 3634 2063 7572 5f6d 756c 7420 3d20 5043  64 cur_mult = PC
-00001010: 475f 4445 4641 554c 545f 4d55 4c54 4950  G_DEFAULT_MULTIP
-00001020: 4c49 4552 5f36 343b 2020 202f 2f46 6965  LIER_64;   //Fie
-00001030: 7865 6420 746f 2061 2063 6f6e 7374 0d0a  xed to a const..
-00001040: 092f 2f55 3634 2063 7572 5f70 6c75 7320  .//U64 cur_plus 
-00001050: 3d20 676c 6f62 616c 5f73 7461 7465 2e49  = global_state.I
-00001060: 4e43 3b20 2020 2020 2020 2020 2020 202f  NC;            /
-00001070: 2f53 7570 706c 6965 6420 6279 2074 6865  /Supplied by the
-00001080: 2075 7365 720d 0a09 0d0a 0955 3634 2061   user......U64 a
-00001090: 6363 5f6d 756c 7420 3d20 3175 3b0d 0a09  cc_mult = 1u;...
-000010a0: 5536 3420 6163 635f 706c 7573 203d 2030  U64 acc_plus = 0
-000010b0: 753b 0d0a 0977 6869 6c65 2028 6465 6c74  u;...while (delt
-000010c0: 6120 3e20 3029 207b 0d0a 0909 6966 2028  a > 0) {....if (
-000010d0: 6465 6c74 6120 2620 3129 207b 0d0a 0909  delta & 1) {....
-000010e0: 0961 6363 5f6d 756c 7420 2a3d 2063 7572  .acc_mult *= cur
-000010f0: 5f6d 756c 743b 0d0a 0909 0961 6363 5f70  _mult;.....acc_p
-00001100: 6c75 7320 3d20 6163 635f 706c 7573 202a  lus = acc_plus *
-00001110: 2063 7572 5f6d 756c 7420 2b20 6375 725f   cur_mult + cur_
-00001120: 706c 7573 3b0d 0a09 097d 0d0a 0909 6375  plus;....}....cu
-00001130: 725f 706c 7573 203d 2028 6375 725f 6d75  r_plus = (cur_mu
-00001140: 6c74 202b 2031 2920 2a20 6375 725f 706c  lt + 1) * cur_pl
-00001150: 7573 3b0d 0a09 0963 7572 5f6d 756c 7420  us;....cur_mult 
-00001160: 2a3d 2063 7572 5f6d 756c 743b 0d0a 0909  *= cur_mult;....
-00001170: 6465 6c74 6120 2f3d 2032 3b0d 0a09 7d09  delta /= 2;...}.
-00001180: 0d0a 092f 2f72 5f70 7269 6e74 6628 2225  ...//r_printf("%
-00001190: 2220 5052 4975 3634 2022 2025 2220 2050  " PRIu64 " %"  P
-000011a0: 5249 7536 3420 225c 6e22 2c20 2061 6363  RIu64 "\n",  acc
-000011b0: 5f6d 756c 742c 2061 6363 5f70 6c75 7329  _mult, acc_plus)
-000011c0: 3b0d 0a09 6d75 6c74 5b30 5d20 203d 2061  ;...mult[0]  = a
-000011d0: 6363 5f6d 756c 743b 0d0a 0973 6869 6674  cc_mult;...shift
-000011e0: 5b30 5d20 3d20 6163 635f 706c 7573 3b0d  [0] = acc_plus;.
-000011f0: 0a09 2f2f 7265 7475 726e 2061 6363 5f6d  ..//return acc_m
-00001200: 756c 7420 2a20 7374 6174 6520 2b20 6163  ult * state + ac
-00001210: 635f 706c 7573 3b0d 0a7d 0d0a 0d0a 200d  c_plus;..}.... .
-00001220: 0a0d 0a2f 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  .../************
-00001230: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00001240: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00001250: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00001260: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2f0d  **************/.
-00001270: 0a2f 2f20 2050 7265 2d63 6163 6c63 7561  .//  Pre-caclcua
-00001280: 7465 6420 636f 6e73 7461 6e74 7320 666f  ted constants fo
-00001290: 7220 7468 6520 4761 7573 7361 696e 2072  r the Gaussain r
-000012a0: 6164 6f6d 2067 656e 6572 6174 6f72 2062  adom generator b
-000012b0: 6173 6564 206f 6e20 0d0a 2f2f 2020 6120  ased on ..//  a 
-000012c0: 6879 6272 6964 2072 656a 6563 7469 6f6e  hybrid rejection
-000012d0: 2073 616d 706c 696e 6720 6d65 7468 6f64   sampling method
-000012e0: 0d0a 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ../*************
+000000d0: 2e68 2220 200d 0a0d 0a23 696e 636c 7564  .h"  ....#includ
+000000e0: 6520 2261 7373 6572 742e 6822 2020 0d0a  e "assert.h"  ..
+000000f0: 200d 0a0d 0a2f 2f68 7474 7073 3a2f 2f68   ....//https://h
+00000100: 616c 2e61 7263 6869 7665 732d 6f75 7665  al.archives-ouve
+00000110: 7274 6573 2e66 722f 6861 6c2d 3032 3730  rtes.fr/hal-0270
+00000120: 3037 3931 2f64 6f63 756d 656e 743a 2061  0791/document: a
+00000130: 206e 6963 6520 696e 7472 6f20 746f 2074   nice intro to t
+00000140: 6865 2070 6367 2061 6c67 0d0a 2f2a 5072  he pcg alg../*Pr
+00000150: 6163 7469 6361 6c20 7365 6564 2d72 6563  actical seed-rec
+00000160: 6f76 6572 7920 666f 7220 7468 6520 5043  overy for the PC
+00000170: 4720 5073 6575 646f 2d52 616e 646f 6d20  G Pseudo-Random 
+00000180: 4e75 6d62 7220 4765 6e65 7261 746f 722a  Numbr Generator*
+00000190: 2f0d 0a0d 0a2f 2a0d 0a49 6e74 6572 6e61  /..../*..Interna
+000001a0: 6c6c 792c 2074 6869 7320 524e 4720 7573  lly, this RNG us
+000001b0: 6573 2074 776f 2036 342d 6269 7420 696e  es two 64-bit in
+000001c0: 7465 6765 7273 2066 6f72 2069 7473 2069  tegers for its i
+000001d0: 6e74 6572 6e61 6c20 7374 6174 652c 2063  nternal state, c
+000001e0: 6f6e 7369 7374 696e 6720 6f66 3a0d 0a74  onsisting of:..t
+000001f0: 6865 2063 7572 7265 6e74 2073 7461 7465  he current state
+00000200: 2097 2074 6865 2052 4e47 2069 7465 7261   . the RNG itera
+00000210: 7465 7320 7468 726f 7567 6820 616c 6c20  tes through all 
+00000220: 3236 3420 706f 7373 6962 6c65 2069 6e74  264 possible int
+00000230: 6572 6e61 6c20 7374 6174 6573 2e0d 0a74  ernal states...t
+00000240: 6865 2052 4e47 2d73 6571 7565 6e63 6520  he RNG-sequence 
+00000250: 636f 6e73 7461 6e74 2097 2061 2076 616c  constant . a val
+00000260: 7565 2074 6861 7420 6465 6669 6e65 7320  ue that defines 
+00000270: 7768 6963 6820 6f66 2032 3633 2070 6f73  which of 263 pos
+00000280: 7369 626c 6520 7261 6e64 6f6d 2073 6571  sible random seq
+00000290: 7565 6e63 6573 0d0a 7468 6520 6375 7272  uences..the curr
+000002a0: 656e 7420 7374 6174 6520 6973 2069 7465  ent state is ite
+000002b0: 7261 7469 6e67 2074 6872 6f75 6768 3b20  rating through; 
+000002c0: 6974 2068 6f6c 6473 2074 6865 2073 616d  it holds the sam
+000002d0: 6520 7661 6c75 6520 6f76 6572 2074 6865  e value over the
+000002e0: 206c 6966 6574 696d 6520 6f66 2074 6865   lifetime of the
+000002f0: 2052 4e47 2e0d 0a2a 2f0d 0a0d 0a2f 2a0d   RNG...*/..../*.
+00000300: 0a46 6f72 2074 6869 7320 6765 6e65 7261  .For this genera
+00000310: 746f 722c 2074 6865 7265 2061 7265 2032  tor, there are 2
+00000320: 5e36 3320 706f 7373 6962 6c65 2073 6571  ^63 possible seq
+00000330: 7565 6e63 6573 206f 6620 7073 6575 646f  uences of pseudo
+00000340: 7261 6e64 6f6d 206e 756d 6265 7273 2e20  random numbers. 
+00000350: 4561 6368 2073 6571 7565 6e63 6520 6973  Each sequence is
+00000360: 0d0a 656e 7469 7265 6c79 2064 6973 7469  ..entirely disti
+00000370: 6e63 7420 616e 6420 6861 7320 6120 7065  nct and has a pe
+00000380: 7269 6f64 206f 6620 325e 3634 2e20 5468  riod of 2^64. Th
+00000390: 6520 696e 6974 7365 7120 6172 6775 6d65  e initseq argume
+000003a0: 6e74 2073 656c 6563 7473 2077 6869 6368  nt selects which
+000003b0: 2073 7472 6561 6d20 796f 7520 7769 6c6c   stream you will
+000003c0: 2075 7365 2e20 0d0a 5468 6520 696e 6974   use. ..The init
+000003d0: 7374 6174 6520 6172 6775 6d65 6e74 2073  state argument s
+000003e0: 7065 6369 6669 6573 2077 6865 7265 2079  pecifies where y
+000003f0: 6f75 2061 7265 2069 6e20 7468 6174 2032  ou are in that 2
+00000400: 3634 2070 6572 696f 642e 0d0a 2a2f 0d0a  64 period...*/..
+00000410: 0d0a 2364 6566 696e 6520 5043 475f 4445  ..#define PCG_DE
+00000420: 4641 554c 545f 4d55 4c54 4950 4c49 4552  FAULT_MULTIPLIER
+00000430: 5f36 3420 2036 3336 3431 3336 3232 3338  _64  63641362238
+00000440: 3436 3739 3330 3035 554c 4c20 2f2f 6874  46793005ULL //ht
+00000450: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000460: 2f69 6d6e 656d 652f 7063 672d 632d 6261  /imneme/pcg-c-ba
+00000470: 7369 632f 626c 6f62 2f6d 6173 7465 722f  sic/blob/master/
+00000480: 7063 675f 6261 7369 632e 630d 0a23 6465  pcg_basic.c..#de
+00000490: 6669 6e65 2050 4347 5f44 4546 4155 4c54  fine PCG_DEFAULT
+000004a0: 5f49 4e43 5245 4d45 4e54 5f36 3420 2020  _INCREMENT_64   
+000004b0: 3134 3432 3639 3530 3430 3838 3839 3633  1442695040888963
+000004c0: 3430 3755 4c4c 202f 2f2f 2f68 7474 7073  407ULL ////https
+000004d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 696d  ://github.com/im
+000004e0: 6e65 6d65 2f70 6367 2d63 2f62 6c6f 622f  neme/pcg-c/blob/
+000004f0: 6d61 7374 6572 2f69 6e63 6c75 6465 2f70  master/include/p
+00000500: 6367 5f76 6172 6961 6e74 732e 680d 0a0d  cg_variants.h...
+00000510: 0a0d 0a2f 2f68 7474 7073 3a2f 2f67 6974  ...//https://git
+00000520: 6875 622e 636f 6d2f 696d 6e65 6d65 2f70  hub.com/imneme/p
+00000530: 6367 2d63 2d62 6173 6963 2f62 6c6f 622f  cg-c-basic/blob/
+00000540: 6d61 7374 6572 2f70 6367 5f62 6173 6963  master/pcg_basic
+00000550: 2e68 0d0a 2364 6566 696e 6520 5043 475f  .h..#define PCG_
+00000560: 4445 4641 554c 545f 474c 4f42 414c 5f53  DEFAULT_GLOBAL_S
+00000570: 5441 5445 5f36 3420 2020 2020 3078 3835  TATE_64     0x85
+00000580: 3363 3439 6536 3734 3866 6561 3962 554c  3c49e6748fea9bUL
+00000590: 4c0d 0a23 6465 6669 6e65 2050 4347 5f44  L..#define PCG_D
+000005a0: 4546 4155 4c54 5f47 4c4f 4241 4c5f 494e  EFAULT_GLOBAL_IN
+000005b0: 4352 454d 454e 545f 3634 2030 7864 6133  CREMENT_64 0xda3
+000005c0: 6533 3963 6239 3462 3935 6264 6255 4c4c  e39cb94b95bdbULL
+000005d0: 0d0a 0d0a 2f2f 204c 696e 6561 7220 436f  ....// Linear Co
+000005e0: 6e67 7275 656e 7469 616c 2047 656e 6572  ngruential Gener
+000005f0: 6174 6f72 2028 4c43 4729 3a0d 0a2f 2f20  ator (LCG):..// 
+00000600: 5820 2020 2020 3d20 2058 2020 2020 2a20  X     =  X    * 
+00000610: 4d55 4c54 4950 4c49 4552 202b 2049 4e43  MULTIPLIER + INC
+00000620: 5245 4d45 4e54 2873 6869 6674 2f70 6c75  REMENT(shift/plu
+00000630: 732f 7374 6174 652e 696e 6329 206d 6f64  s/state.inc) mod
+00000640: 2032 5e36 340d 0a2f 2f20 5374 6174 6520   2^64..// State 
+00000650: 3d20 2053 7461 7465 2a20 4d55 4c54 4950  =  State* MULTIP
+00000660: 4c49 4552 202b 2049 4e43 5245 4d45 4e54  LIER + INCREMENT
+00000670: 2873 6869 6674 2f70 6c75 732f 494e 4329  (shift/plus/INC)
+00000680: 2020 2020 2020 206d 6f64 2032 5e36 340d         mod 2^64.
+00000690: 0a0d 0a0d 0a74 7970 6564 6566 2073 7472  .....typedef str
+000006a0: 7563 7420 7063 6733 325f 7261 6e64 6f6d  uct pcg32_random
+000006b0: 5f73 7472 7563 7420 7b20 092f 2f68 7474  _struct { .//htt
+000006c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000006d0: 696d 6e65 6d65 2f70 6367 2d63 2d62 6173  imneme/pcg-c-bas
+000006e0: 6963 2f62 6c6f 622f 6d61 7374 6572 2f70  ic/blob/master/p
+000006f0: 6367 5f62 6173 6963 2e68 0d0a 0955 3634  cg_basic.h...U64
+00000700: 2073 7461 7465 3b20 2f2f 2f20 524e 4720   state; /// RNG 
+00000710: 7374 6174 652e 416c 6c20 7661 6c75 6573  state.All values
+00000720: 2061 7265 2070 6f73 7369 626c 652e 0d0a   are possible...
+00000730: 0955 3634 2069 6e63 3b20 2020 2f2f 2043  .U64 inc;   // C
+00000740: 6f6e 7472 6f6c 7320 7768 6963 6820 524e  ontrols which RN
+00000750: 4720 7365 7175 656e 6365 2028 7374 7265  G sequence (stre
+00000760: 616d 2920 6973 0d0a 0909 0920 2020 2f2f  am) is.....   //
+00000770: 2073 656c 6563 7465 642e 204d 7573 7420   selected. Must 
+00000780: 2a61 6c77 6179 732a 2062 6520 6f64 642e  *always* be odd.
+00000790: 0d0a 7d20 7063 6733 325f 7261 6e64 6f6d  ..} pcg32_random
+000007a0: 5f74 3b0d 0a0d 0a73 7461 7469 6320 7063  _t;....static pc
+000007b0: 6733 325f 7261 6e64 6f6d 5f74 2067 6c6f  g32_random_t glo
+000007c0: 6261 6c5f 7374 6174 6520 3d20 7b0d 0a09  bal_state = {...
+000007d0: 2e73 7461 7465 3d20 5043 475f 4445 4641  .state= PCG_DEFA
+000007e0: 554c 545f 474c 4f42 414c 5f53 5441 5445  ULT_GLOBAL_STATE
+000007f0: 5f36 342c 0d0a 092e 696e 6320 203d 2050  _64,....inc  = P
+00000800: 4347 5f44 4546 4155 4c54 5f47 4c4f 4241  CG_DEFAULT_GLOBA
+00000810: 4c5f 494e 4352 454d 454e 545f 3634 207d  L_INCREMENT_64 }
+00000820: 3b0d 0a0d 0a76 6f69 6420 7063 675f 7365  ;....void pcg_se
+00000830: 745f 7365 6564 2855 3634 2069 6e69 7473  t_seed(U64 inits
+00000840: 7461 7465 2c20 5536 3420 696e 6974 7365  tate, U64 initse
+00000850: 7129 0d0a 7b09 0d0a 0965 7874 6572 6e20  q)..{....extern 
+00000860: 766f 6964 2069 6e69 745f 6761 7573 735f  void init_gauss_
+00000870: 726e 6428 766f 6964 293b 0d0a 0969 6e69  rnd(void);...ini
+00000880: 745f 6761 7573 735f 726e 6428 293b 0d0a  t_gauss_rnd();..
+00000890: 0d0a 0969 6620 2869 6e69 7473 7461 7465  ...if (initstate
+000008a0: 203d 3d20 3020 2920 7b0d 0a09 2f2f 2055   == 0 ) {...// U
+000008b0: 7365 6420 746f 206a 7573 7420 696e 6974  sed to just init
+000008c0: 6961 6c7a 6965 2074 6865 2047 7561 7373  ialzie the Guass
+000008d0: 2073 7472 7563 7475 7265 2e0d 0a09 0972   structure.....r
+000008e0: 6574 7572 6e3b 0d0a 097d 0d0a 0d0a 0969  eturn;...}.....i
+000008f0: 6e69 7473 7461 7465 203d 2069 6e69 7473  nitstate = inits
+00000900: 7461 7465 2026 2069 6e69 7473 6571 3b20  tate & initseq; 
+00000910: 2f2f 4164 6465 6420 6263 7a20 6f6e 6c79  //Added bcz only
+00000920: 2069 6e69 7473 6571 2069 7320 7375 7070   initseq is supp
+00000930: 6c69 6564 2061 7320 6120 7365 6564 2e20  lied as a seed. 
+00000940: 5765 2072 756e 2069 6e69 7473 6571 2074  We run initseq t
+00000950: 6f20 7261 6e64 6f6d 697a 6520 696e 6974  o randomize init
+00000960: 7374 6174 6520 6120 6c69 7474 6c65 2062  state a little b
+00000970: 6974 0d0a 0d0a 0969 6e69 7473 7461 7465  it.....initstate
+00000980: 203d 2069 6e69 7473 7461 7465 203d 3d20   = initstate == 
+00000990: 3020 3f20 5043 475f 4445 4641 554c 545f  0 ? PCG_DEFAULT_
+000009a0: 474c 4f42 414c 5f53 5441 5445 5f36 3420  GLOBAL_STATE_64 
+000009b0: 2020 203a 2069 6e69 7473 7461 7465 3b0d     : initstate;.
+000009c0: 0a09 696e 6974 7365 7120 2020 3d20 696e  ..initseq   = in
+000009d0: 6974 7365 7120 3d3d 2030 2020 203f 2050  itseq == 0   ? P
+000009e0: 4347 5f44 4546 4155 4c54 5f47 4c4f 4241  CG_DEFAULT_GLOBA
+000009f0: 4c5f 494e 4352 454d 454e 545f 3634 203a  L_INCREMENT_64 :
+00000a00: 2069 6e69 7473 6571 3b0d 0a0d 0a09 676c   initseq;.....gl
+00000a10: 6f62 616c 5f73 7461 7465 2e73 7461 7465  obal_state.state
+00000a20: 203d 2030 553b 0d0a 0967 6c6f 6261 6c5f   = 0U;...global_
+00000a30: 7374 6174 652e 696e 6320 2020 3d20 2869  state.inc   = (i
+00000a40: 6e69 7473 6571 203c 3c20 3175 2920 7c20  nitseq << 1u) | 
+00000a50: 3175 3b20 2009 2f2f 696e 6320 6d75 7374  1u;  .//inc must
+00000a60: 2062 6520 616e 206f 6464 206e 756d 6265   be an odd numbe
+00000a70: 720d 0a0d 0a09 5533 3220 726e 643b 0d0a  r.....U32 rnd;..
+00000a80: 0970 6367 5f72 616e 646f 6d28 2672 6e64  .pcg_random(&rnd
+00000a90: 2c20 3129 3b0d 0a09 676c 6f62 616c 5f73  , 1);...global_s
+00000aa0: 7461 7465 2e73 7461 7465 202b 3d20 696e  tate.state += in
+00000ab0: 6974 7374 6174 653b 0d0a 0970 6367 5f72  itstate;...pcg_r
+00000ac0: 616e 646f 6d28 2672 6e64 2c20 3129 3b0d  andom(&rnd, 1);.
+00000ad0: 0a7d 0d0a 766f 6964 2070 6367 5f70 7269  .}..void pcg_pri
+00000ae0: 6e74 5f73 7461 7465 2876 6f69 6429 207b  nt_state(void) {
+00000af0: 725f 7072 696e 7466 2822 7374 6174 653a  r_printf("state:
+00000b00: 2025 3330 2220 5052 4975 3634 2022 2069   %30" PRIu64 " i
+00000b10: 6e63 3a20 2533 3022 2020 5052 4975 3634  nc: %30"  PRIu64
+00000b20: 2022 5c6e 222c 2067 6c6f 6261 6c5f 7374   "\n", global_st
+00000b30: 6174 652e 7374 6174 652c 2067 6c6f 6261  ate.state, globa
+00000b40: 6c5f 7374 6174 652e 696e 6329 3b7d 0d0a  l_state.inc);}..
+00000b50: 0d0a 2f2f 2070 6367 3332 5f72 616e 646f  ..// pcg32_rando
+00000b60: 6d5f 7228 726e 6729 0d0a 2f2f 2020 2047  m_r(rng)..//   G
+00000b70: 656e 6572 6174 6520 6120 756e 6966 6f72  enerate a unifor
+00000b80: 6d6c 7920 6469 7374 7269 6275 7465 6420  mly distributed 
+00000b90: 3332 2d62 6974 2072 616e 646f 6d20 6e75  32-bit random nu
+00000ba0: 6d62 6572 0d0a 766f 6964 2070 6367 5f72  mber..void pcg_r
+00000bb0: 616e 646f 6d28 5533 3250 5452 2072 6e64  andom(U32PTR rnd
+00000bc0: 2c20 4933 3220 4e29 0d0a 7b0d 0a09 5536  , I32 N)..{...U6
+00000bd0: 3420 6f6c 6473 7461 7465 203d 2067 6c6f  4 oldstate = glo
+00000be0: 6261 6c5f 7374 6174 652e 7374 6174 653b  bal_state.state;
+00000bf0: 0d0a 0955 3634 2073 6869 6674 2020 2020  ...U64 shift    
+00000c00: 3d20 676c 6f62 616c 5f73 7461 7465 2e69  = global_state.i
+00000c10: 6e63 3b0d 0a0d 0a09 666f 7220 2869 6e74  nc;.....for (int
+00000c20: 2069 203d 2030 3b20 6920 3c20 4e3b 2069   i = 0; i < N; i
+00000c30: 2b2b 2920 7b0d 0a09 0955 3332 2078 6f72  ++) {....U32 xor
+00000c40: 7368 6966 7465 6420 3d20 2020 2020 2828  shifted =     ((
+00000c50: 6f6c 6473 7461 7465 203e 3e20 3138 7529  oldstate >> 18u)
+00000c60: 205e 206f 6c64 7374 6174 6529 203e 3e20   ^ oldstate) >> 
+00000c70: 3237 7520 2020 3b0d 0a09 0955 3332 2072  27u   ;....U32 r
+00000c80: 6f74 203d 206f 6c64 7374 6174 6520 3e3e  ot = oldstate >>
+00000c90: 2035 3975 3b0d 0a09 092f 2f2a 726e 642b   59u;....//*rnd+
+00000ca0: 2b20 3d20 2878 6f72 7368 6966 7465 6420  + = (xorshifted 
+00000cb0: 3e3e 2072 6f74 2920 7c20 2878 6f72 7368  >> rot) | (xorsh
+00000cc0: 6966 7465 6420 3c3c 2028 282d 726f 7429  ifted << ((-rot)
+00000cd0: 2026 2033 3129 293b 0d0a 0909 2a72 6e64   & 31));....*rnd
+00000ce0: 2b2b 203d 2028 786f 7273 6869 6674 6564  ++ = (xorshifted
+00000cf0: 203e 3e20 726f 7429 207c 2028 786f 7273   >> rot) | (xors
+00000d00: 6869 6674 6564 203c 3c20 2828 2d20 2a28  hifted << ((- *(
+00000d10: 2849 3332 2a29 2826 726f 7429 2920 2029  (I32*)(&rot))  )
+00000d20: 2026 2033 3129 293b 0d0a 0909 6f6c 6473   & 31));....olds
+00000d30: 7461 7465 203d 206f 6c64 7374 6174 6520  tate = oldstate 
+00000d40: 2a20 5043 475f 4445 4641 554c 545f 4d55  * PCG_DEFAULT_MU
+00000d50: 4c54 4950 4c49 4552 5f36 3420 2b20 7368  LTIPLIER_64 + sh
+00000d60: 6966 743b 0d0a 097d 0d0a 0967 6c6f 6261  ift;...}...globa
+00000d70: 6c5f 7374 6174 652e 7374 6174 6520 3d20  l_state.state = 
+00000d80: 6f6c 6473 7461 7465 3b0d 0a7d 0d0a 0d0a  oldstate;..}....
+00000d90: 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  /***************
+00000da0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000db0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2f  ***************/
+00000dc0: 0d0a 2f2f 204e 6f20 6e65 6564 2074 6f20  ..// No need to 
+00000dd0: 6578 706f 7274 2074 6869 7320 6675 6e63  export this func
+00000de0: 0d0a 5536 3420 7063 675f 6164 7661 6e63  ..U64 pcg_advanc
+00000df0: 655f 6c63 675f 3634 2855 3634 2073 7461  e_lcg_64(U64 sta
+00000e00: 7465 2c20 5536 3420 6465 6c74 612c 2055  te, U64 delta, U
+00000e10: 3634 2063 7572 5f6d 756c 742c 2055 3634  64 cur_mult, U64
+00000e20: 2063 7572 5f70 6c75 7329 0d0a 7b20 2020   cur_plus)..{   
+00000e30: 0d0a 092f 2f41 6476 616e 6365 2074 6865  ...//Advance the
+00000e40: 2073 7461 7465 2062 7920 6120 746f 7461   state by a tota
+00000e50: 6c20 6f66 2064 656c 7461 2073 7465 7073  l of delta steps
+00000e60: 0d0a 092f 2f68 7474 7073 3a2f 2f67 6974  ...//https://git
+00000e70: 6875 622e 636f 6d2f 696d 6e65 6d65 2f70  hub.com/imneme/p
+00000e80: 6367 2d63 2f62 6c6f 622f 6d61 7374 6572  cg-c/blob/master
+00000e90: 2f73 7263 2f70 6367 2d61 6476 616e 6365  /src/pcg-advance
+00000ea0: 2d36 342e 630d 0a09 5536 3420 6163 635f  -64.c...U64 acc_
+00000eb0: 6d75 6c74 203d 2031 753b 0d0a 0955 3634  mult = 1u;...U64
+00000ec0: 2061 6363 5f70 6c75 7320 3d20 3075 3b0d   acc_plus = 0u;.
+00000ed0: 0a09 7768 696c 6520 2864 656c 7461 203e  ..while (delta >
+00000ee0: 2030 2920 7b0d 0a09 0969 6620 2864 656c   0) {....if (del
+00000ef0: 7461 2026 2031 2920 7b0d 0a09 0909 6163  ta & 1) {.....ac
+00000f00: 635f 6d75 6c74 202a 3d20 6375 725f 6d75  c_mult *= cur_mu
+00000f10: 6c74 3b0d 0a09 0909 6163 635f 706c 7573  lt;.....acc_plus
+00000f20: 203d 2061 6363 5f70 6c75 7320 2a20 6375   = acc_plus * cu
+00000f30: 725f 6d75 6c74 202b 2063 7572 5f70 6c75  r_mult + cur_plu
+00000f40: 733b 0d0a 0909 7d0d 0a09 0963 7572 5f70  s;....}....cur_p
+00000f50: 6c75 7320 3d20 2863 7572 5f6d 756c 7420  lus = (cur_mult 
+00000f60: 2b20 3129 202a 2063 7572 5f70 6c75 733b  + 1) * cur_plus;
+00000f70: 0d0a 0909 6375 725f 6d75 6c74 202a 3d20  ....cur_mult *= 
+00000f80: 6375 725f 6d75 6c74 3b0d 0a09 0964 656c  cur_mult;....del
+00000f90: 7461 202f 3d20 323b 0d0a 097d 0d0a 0972  ta /= 2;...}...r
+00000fa0: 6574 7572 6e20 6163 635f 6d75 6c74 202a  eturn acc_mult *
+00000fb0: 2073 7461 7465 202b 2061 6363 5f70 6c75   state + acc_plu
+00000fc0: 733b 0d0a 7d0d 0a76 6f69 6420 7063 675f  s;..}..void pcg_
+00000fd0: 6765 745f 6c63 675f 6d75 6c74 6970 6c69  get_lcg_multipli
+00000fe0: 6572 5f73 6869 6674 5f6d 756c 7469 7374  er_shift_multist
+00000ff0: 6570 2820 4933 3220 6465 6c74 612c 2055  ep( I32 delta, U
+00001000: 3634 2063 7572 5f6d 756c 742c 2055 3634  64 cur_mult, U64
+00001010: 2063 7572 5f70 6c75 732c 2055 3634 202a   cur_plus, U64 *
+00001020: 206d 756c 742c 2055 3634 202a 7368 6966   mult, U64 *shif
+00001030: 7429 200d 0a7b 0d0a 092f 2f20 4669 6e64  t) ..{...// Find
+00001040: 2074 6865 206d 756c 746c 6970 6c69 6572   the multliplier
+00001050: 2061 6e64 2073 6869 6674 2028 706c 7573   and shift (plus
+00001060: 2920 666f 7220 6120 6d75 6c74 692d 7374  ) for a multi-st
+00001070: 6570 2061 6476 616e 6365 0d0a 0d0a 092f  ep advance...../
+00001080: 2f49 3332 2064 656c 7461 203d 2034 3b20  /I32 delta = 4; 
+00001090: 2f2f 4d6f 7665 2066 6f72 7761 7264 2062  //Move forward b
+000010a0: 7920 3420 7374 6570 730d 0a09 2f2f 5536  y 4 steps...//U6
+000010b0: 3420 6375 725f 6d75 6c74 203d 2050 4347  4 cur_mult = PCG
+000010c0: 5f44 4546 4155 4c54 5f4d 554c 5449 504c  _DEFAULT_MULTIPL
+000010d0: 4945 525f 3634 3b20 2020 2f2f 4669 6578  IER_64;   //Fiex
+000010e0: 6564 2074 6f20 6120 636f 6e73 740d 0a09  ed to a const...
+000010f0: 2f2f 5536 3420 6375 725f 706c 7573 203d  //U64 cur_plus =
+00001100: 2067 6c6f 6261 6c5f 7374 6174 652e 494e   global_state.IN
+00001110: 433b 2020 2020 2020 2020 2020 2020 2f2f  C;            //
+00001120: 5375 7070 6c69 6564 2062 7920 7468 6520  Supplied by the 
+00001130: 7573 6572 0d0a 090d 0a09 5536 3420 6163  user......U64 ac
+00001140: 635f 6d75 6c74 203d 2031 753b 0d0a 0955  c_mult = 1u;...U
+00001150: 3634 2061 6363 5f70 6c75 7320 3d20 3075  64 acc_plus = 0u
+00001160: 3b0d 0a09 7768 696c 6520 2864 656c 7461  ;...while (delta
+00001170: 203e 2030 2920 7b0d 0a09 0969 6620 2864   > 0) {....if (d
+00001180: 656c 7461 2026 2031 2920 7b0d 0a09 0909  elta & 1) {.....
+00001190: 6163 635f 6d75 6c74 202a 3d20 6375 725f  acc_mult *= cur_
+000011a0: 6d75 6c74 3b0d 0a09 0909 6163 635f 706c  mult;.....acc_pl
+000011b0: 7573 203d 2061 6363 5f70 6c75 7320 2a20  us = acc_plus * 
+000011c0: 6375 725f 6d75 6c74 202b 2063 7572 5f70  cur_mult + cur_p
+000011d0: 6c75 733b 0d0a 0909 7d0d 0a09 0963 7572  lus;....}....cur
+000011e0: 5f70 6c75 7320 3d20 2863 7572 5f6d 756c  _plus = (cur_mul
+000011f0: 7420 2b20 3129 202a 2063 7572 5f70 6c75  t + 1) * cur_plu
+00001200: 733b 0d0a 0909 6375 725f 6d75 6c74 202a  s;....cur_mult *
+00001210: 3d20 6375 725f 6d75 6c74 3b0d 0a09 0964  = cur_mult;....d
+00001220: 656c 7461 202f 3d20 323b 0d0a 097d 090d  elta /= 2;...}..
+00001230: 0a09 2f2f 725f 7072 696e 7466 2822 2522  ..//r_printf("%"
+00001240: 2050 5249 7536 3420 2220 2522 2020 5052   PRIu64 " %"  PR
+00001250: 4975 3634 2022 5c6e 222c 2020 6163 635f  Iu64 "\n",  acc_
+00001260: 6d75 6c74 2c20 6163 635f 706c 7573 293b  mult, acc_plus);
+00001270: 0d0a 096d 756c 745b 305d 2020 3d20 6163  ...mult[0]  = ac
+00001280: 635f 6d75 6c74 3b0d 0a09 7368 6966 745b  c_mult;...shift[
+00001290: 305d 203d 2061 6363 5f70 6c75 733b 0d0a  0] = acc_plus;..
+000012a0: 092f 2f72 6574 7572 6e20 6163 635f 6d75  .//return acc_mu
+000012b0: 6c74 202a 2073 7461 7465 202b 2061 6363  lt * state + acc
+000012c0: 5f70 6c75 733b 0d0a 7d0d 0a0d 0a20 0d0a  _plus;..}.... ..
+000012d0: 0d0a 2f2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ../*************
+000012e0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 000012f0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00001300: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00001310: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00001320: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2f 0d0a  *************/..
-00001330: 4741 5553 535f 434f 4e53 5441 4e54 2047  GAUSS_CONSTANT G
-00001340: 4155 5353 0d0a 3d20 7b20 2e78 203d 207b  AUSS..= { .x = {
-00001350: 2030 2c20 302e 3031 3935 3834 3238 3532   0, 0.0195842852
-00001360: 3330 3132 372c 2030 2e30 3339 3137 3630  30127, 0.0391760
-00001370: 3835 3530 3330 3938 2c20 302e 3035 3837  85503098, 0.0587
-00001380: 3832 3933 3630 3638 3934 332c 2030 2e30  82936068943, 0.0
-00001390: 3738 3431 3234 3132 3733 3331 3132 2c0d  78412412733112,.
-000013a0: 0a30 2e30 3938 3037 3231 3532 3438 3836  .0.0980721524886
-000013b0: 3631 2c20 302e 3131 3737 3639 3837 3435  61, 0.1177698745
-000013c0: 3739 3039 352c 2030 2e31 3337 3531 3334  79095, 0.1375134
-000013d0: 3032 3134 3433 3336 2c20 302e 3135 3733  02144336, 0.1573
-000013e0: 3130 3638 3436 3130 3137 312c 2030 2e31  10684610171, 0.1
-000013f0: 3737 3136 3938 3230 3939 3137 3430 2c20  77169820991740, 
-00001400: 302e 3139 3730 3939 3038 3432 3934 3331  0.19709908429431
-00001410: 322c 0d0a 302e 3231 3731 3036 3934 3732  2,..0.2171069472
-00001420: 3130 3133 302c 2030 2e32 3337 3230 3231  10130, 0.2372021
-00001430: 3039 3332 3837 3838 2c20 302e 3235 3733  09328788, 0.2573
-00001440: 3933 3532 3631 3030 3933 382c 2030 2e32  93526100938, 0.2
-00001450: 3737 3639 3034 3339 3832 3135 3737 2c20  77690439821577, 
-00001460: 302e 3239 3831 3032 3431 3239 3330 3438  0.29810241293048
-00001470: 372c 2030 2e33 3138 3633 3933 3633 3936  7, 0.31863936396
-00001480: 3433 3735 2c0d 0a30 2e33 3339 3331 3136  4375,..0.3393116
-00001490: 3036 3533 3838 3137 2c20 302e 3336 3031  06538817, 0.3601
-000014a0: 3239 3839 3137 3839 3536 392c 2030 2e33  29891789569, 0.3
-000014b0: 3831 3130 3534 3534 3736 3335 3537 2c20  81105454763557, 
-000014c0: 302e 3430 3232 3530 3036 3533 3231 3732  0.40225006532172
-000014d0: 352c 2030 2e34 3233 3537 3630 3834 3230  5, 0.42357608420
-000014e0: 3132 3030 2c20 302e 3434 3530 3936 3532  1200, 0.44509652
-000014f0: 3439 3835 3531 362c 0d0a 302e 3436 3638  4985516,..0.4668
-00001500: 3235 3132 3238 3532 3539 302c 2030 2e34  25122852590, 0.4
-00001510: 3838 3737 3634 3131 3131 3436 3730 2c20  88776411114670, 
-00001520: 302e 3531 3039 3635 3830 3637 3338 3234  0.51096580673824
-00001530: 372c 2030 2e35 3333 3430 3937 3036 3234  7, 0.53340970624
-00001540: 3132 3831 2c20 302e 3535 3631 3235 3539  1281, 0.55612559
-00001550: 3336 3138 3639 312c 2030 2e35 3739 3133  3618691, 0.57913
-00001560: 3231 3632 3235 3535 3536 2c0d 0a30 2e36  2162255556,..0.6
-00001570: 3032 3434 3934 3533 3136 3434 3234 2c20  02449453164424, 
-00001580: 302e 3632 3630 3939 3031 3233 3436 3432  0.62609901234642
-00001590: 312c 2030 2e36 3530 3130 3430 3730 3634  1, 0.65010407064
-000015a0: 3739 3935 2c20 302e 3637 3434 3839 3735  7995, 0.67448975
-000015b0: 3031 3936 3038 322c 2030 2e36 3939 3238  0196082, 0.69928
-000015c0: 3333 3032 3338 3332 3230 2c20 302e 3732  3302383220, 0.72
-000015d0: 3435 3134 3338 3334 3932 3336 362c 0d0a  4514383492366,..
-000015e0: 302e 3735 3032 3135 3337 3534 3637 3934  0.75021537546794
-000015f0: 312c 2030 2e37 3736 3432 3137 3631 3134  1, 0.77642176114
-00001600: 3739 3238 2c20 302e 3830 3331 3732 3536  7928, 0.80317256
-00001610: 3535 3937 3931 382c 2030 2e38 3330 3531  5597918, 0.83051
-00001620: 3038 3738 3230 3533 3939 2c20 302e 3835  0878205399, 0.85
-00001630: 3834 3834 3437 3431 3431 3833 322c 2030  8484474141832, 0
-00001640: 2e38 3837 3134 3635 3539 3031 3838 3736  .887146559018876
-00001650: 2c0d 0a30 2e39 3136 3535 3636 3637 3533  ,..0.91655666753
-00001660: 3331 3133 2c20 302e 3934 3637 3831 3735  3113, 0.94678175
-00001670: 3633 3031 3034 362c 2030 2e39 3737 3839  6301046, 0.97789
-00001680: 3735 3433 3934 3035 3432 2c20 312e 3030  7543940542, 1.00
-00001690: 3939 3930 3136 3932 3439 3538 322c 2031  9990169249582, 1
-000016a0: 2e30 3433 3135 3832 3633 3331 3834 3534  .043158263318454
-000016b0: 2c20 312e 3037 3735 3135 3536 3730 3430  , 1.077515567040
-000016c0: 3238 302c 0d0a 312e 3131 3331 3934 3237  280,..1.11319427
-000016d0: 3731 3630 3932 392c 2031 2e31 3530 3334  7160929, 1.15034
-000016e0: 3933 3830 3337 3630 3038 2c20 312e 3138  9380376008, 1.18
-000016f0: 3931 3634 3335 3031 3939 3333 372c 2031  9164350199337, 1
-00001700: 2e32 3239 3835 3837 3539 3231 3635 3839  .229858759216589
-00001710: 2c20 312e 3237 3236 3938 3634 3131 3930  , 1.272698641190
-00001720: 3533 362c 2031 2e33 3138 3031 3038 3937  536, 1.318010897
-00001730: 3330 3335 3337 2c0d 0a31 2e33 3636 3230  303537,..1.36620
-00001740: 3338 3136 3337 3230 3938 2c20 312e 3431  3816372098, 1.41
-00001750: 3737 3937 3133 3739 3936 3236 382c 2031  7797137996268, 1
-00001760: 2e34 3733 3436 3735 3737 3934 3731 3031  .473467577947101
-00001770: 2c20 312e 3533 3431 3230 3534 3433 3532  , 1.534120544352
-00001780: 3534 372c 2031 2e36 3031 3030 3836 3634  547, 1.601008664
-00001790: 3838 3630 3736 2c20 312e 3637 3539 3339  886076, 1.675939
-000017a0: 3732 3237 3733 3434 342c 0d0a 312e 3736  722773444,..1.76
-000017b0: 3136 3730 3431 3033 3633 3036 372c 2031  1670410363067, 1
-000017c0: 2e38 3632 3733 3138 3637 3432 3136 3532  .862731867421652
-000017d0: 2c20 312e 3938 3734 3237 3838 3539 3239  , 1.987427885929
-000017e0: 3839 362c 2032 2e31 3533 3837 3436 3934  896, 2.153874694
-000017f0: 3036 3134 3536 2c20 322e 3431 3735 3539  061456, 2.417559
-00001800: 3031 3632 3336 3530 207d 2c0d 0a2f 2f79  01623650 },..//y
-00001810: 5b69 2b31 5d2f 795b 695d 2a32 5e32 340d  [i+1]/y[i]*2^24.
-00001820: 0a2e 7952 6174 696f 203d 207b 2031 3637  ..yRatio = { 167
-00001830: 3733 3939 392c 2031 3637 3637 3536 322c  73999, 16767562,
-00001840: 2031 3637 3631 3131 322c 2031 3637 3534   16761112, 16754
-00001850: 3634 302c 2031 3637 3438 3133 362c 2031  640, 16748136, 1
-00001860: 3637 3431 3538 392c 2031 3637 3334 3938  6741589, 1673498
-00001870: 392c 2031 3637 3238 3332 352c 2031 3637  9, 16728325, 167
-00001880: 3231 3538 372c 2031 3637 3134 3736 332c  21587, 16714763,
-00001890: 0d0a 3136 3730 3738 3430 2c20 3136 3730  ..16707840, 1670
-000018a0: 3038 3037 2c20 3136 3639 3336 3531 2c20  0807, 16693651, 
-000018b0: 3136 3638 3633 3538 2c20 3136 3637 3839  16686358, 166789
-000018c0: 3133 2c20 3136 3637 3133 3032 2c20 3136  13, 16671302, 16
-000018d0: 3636 3335 3037 2c20 3136 3635 3535 3132  663507, 16655512
-000018e0: 2c20 3136 3634 3732 3937 2c20 3136 3633  , 16647297, 1663
-000018f0: 3838 3433 2c20 3136 3633 3031 3238 2c20  8843, 16630128, 
-00001900: 3136 3632 3131 3238 2c0d 0a31 3636 3131  16621128,..16611
-00001910: 3831 382c 2031 3636 3032 3137 302c 2031  818, 16602170, 1
-00001920: 3635 3932 3135 342c 2031 3635 3831 3733  6592154, 1658173
-00001930: 362c 2031 3635 3730 3837 392c 3136 3535  6, 16570879,1655
-00001940: 3935 3434 2c20 3136 3534 3736 3834 2c20  9544, 16547684, 
-00001950: 3136 3533 3532 3530 2c20 3136 3532 3231  16535250, 165221
-00001960: 3836 2c20 3136 3530 3834 3331 2c20 3136  86, 16508431, 16
-00001970: 3439 3339 3133 2c20 3136 3437 3835 3534  493913, 16478554
-00001980: 2c0d 0a31 3634 3632 3236 352c 2031 3634  ,..16462265, 164
-00001990: 3434 3934 322c 2031 3634 3236 3437 302c  44942, 16426470,
-000019a0: 2031 3634 3036 3731 352c 2031 3633 3835   16406715, 16385
-000019b0: 3532 322c 2031 3633 3632 3731 322c 2031  522, 16362712, 1
-000019c0: 3633 3338 3037 342c 3136 3331 3133 3633  6338074,16311363
-000019d0: 2c20 3136 3238 3232 3837 2c20 3136 3235  , 16282287, 1625
-000019e0: 3034 3937 2c20 3136 3231 3535 3736 2c20  0497, 16215576, 
-000019f0: 3136 3137 3730 3136 2c0d 0a31 3631 3334  16177016,..16134
-00001a00: 3139 352c 2031 3630 3836 3334 332c 2031  195, 16086343, 1
-00001a10: 3630 3332 3439 372c 2031 3539 3731 3432  6032497, 1597142
-00001a20: 392c 2031 3539 3031 3535 392c 2031 3538  9, 15901559, 158
-00001a30: 3230 3831 332c 2031 3537 3236 3431 342c  20813, 15726414,
-00001a40: 2031 3536 3134 3536 312c 2031 3534 3739   15614561, 15479
-00001a50: 3930 362c 3135 3331 3436 3836 2c20 3135  906,15314686, 15
-00001a60: 3130 3731 3833 2c20 3134 3833 3838 3536  107183, 14838856
-00001a70: 2c0d 0a31 3434 3738 3533 382c 2031 3339  ,..14478538, 139
-00001a80: 3639 3532 342c 2031 3331 3936 3736 382c  69524, 13196768,
-00001a90: 2031 3138 3836 3038 362c 2039 3138 3236   11886086, 91826
-00001aa0: 3334 207d 2c0d 0a2f 2f31 2f79 5b69 5d2a  34 },..//1/y[i]*
-00001ab0: 325e 3234 0d0a 2e79 496e 7665 7273 6520  2^24...yInverse 
-00001ac0: 3d20 7b20 302e 3136 3737 3732 3136 3030  = { 0.1677721600
-00001ad0: 3030 3030 3065 382c 2030 2e31 3637 3830  00000e8, 0.16780
-00001ae0: 3433 3337 3130 3730 3239 6538 2c20 302e  4337107029e8, 0.
-00001af0: 3136 3739 3030 3935 3438 3837 3339 3665  167900954887396e
-00001b00: 382c 2030 2e31 3638 3036 3232 3733 3332  8, 0.16806227332
-00001b10: 3137 3932 6538 2c20 302e 3136 3832 3838  1792e8, 0.168288
-00001b20: 3732 3737 3238 3834 3065 382c 0d0a 302e  727728840e8,..0.
-00001b30: 3136 3835 3830 3933 3138 3139 3432 3265  168580931819422e
-00001b40: 382c 2030 2e31 3638 3933 3936 3832 3032  8, 0.16893968202
-00001b50: 3935 3930 6538 2c20 302e 3136 3933 3635  9590e8, 0.169365
-00001b60: 3936 3331 3930 3338 3965 382c 2030 2e31  963190389e8, 0.1
-00001b70: 3639 3836 3039 3535 3631 3137 3533 6538  69860955611753e8
-00001b80: 2c30 2e31 3730 3432 3630 3433 3637 3831  ,0.1704260436781
-00001b90: 3831 6538 2c20 302e 3137 3130 3632 3832  81e8, 0.17106282
-00001ba0: 3630 3736 3633 3665 382c 0d0a 302e 3137  6076636e8,..0.17
-00001bb0: 3137 3733 3132 3738 3032 3636 3065 382c  1773127802660e8,
-00001bc0: 2030 2e31 3732 3535 3930 3134 3131 3936   0.1725590141196
-00001bd0: 3633 6538 2c20 302e 3137 3334 3232 3830  63e8, 0.17342280
-00001be0: 3636 3739 3532 3865 382c 2030 2e31 3734  6679528e8, 0.174
-00001bf0: 3336 3731 3032 3035 3130 3339 6538 2c20  367102051039e8, 
-00001c00: 302e 3137 3533 3934 3739 3239 3437 3239  0.17539479294729
-00001c10: 3965 382c 2030 2e31 3736 3530 3930 3932  9e8, 0.176509092
-00001c20: 3439 3535 3939 6538 2c0d 0a30 2e31 3737  495599e8,..0.177
-00001c30: 3731 3335 3631 3935 3438 3933 6538 2c20  713561954893e8, 
-00001c40: 302e 3137 3930 3132 3134 3233 3539 3132  0.17901214235912
-00001c50: 3865 382c 302e 3138 3034 3039 3139 3036  8e8,0.1804091906
-00001c60: 3531 3730 3865 382c 2030 2e31 3831 3930  51708e8, 0.18190
-00001c70: 3935 3230 3938 3036 3636 6538 2c20 302e  9520980666e8, 0.
-00001c80: 3138 3335 3138 3435 3139 3439 3434 3765  183518451949447e
-00001c90: 382c 2030 2e31 3835 3234 3138 3630 3736  8, 0.18524186076
-00001ca0: 3937 3833 6538 2c0d 0a30 2e31 3837 3038  9783e8,..0.18708
-00001cb0: 3632 3435 3434 3731 3335 6538 2c20 302e  6245447135e8, 0.
-00001cc0: 3138 3930 3538 3739 3633 3533 3737 3465  189058796353774e
-00001cd0: 382c 2030 2e31 3931 3136 3734 3738 3831  8, 0.19116747881
-00001ce0: 3938 3938 6538 2c20 302e 3139 3334 3231  9898e8, 0.193421
-00001cf0: 3132 3837 3132 3633 3765 382c 2030 2e31  128712637e8, 0.1
-00001d00: 3935 3832 3935 3633 3339 3333 3038 6538  95829563393308e8
-00001d10: 2c20 302e 3139 3834 3033 3731 3039 3637  , 0.198403710967
-00001d20: 3234 3765 382c 0d0a 302e 3230 3131 3535  247e8,..0.201155
-00001d30: 3736 3133 3937 3031 3665 382c 2030 2e32  761397016e8, 0.2
-00001d40: 3034 3039 3933 3433 3837 3733 3634 6538  04099343877364e8
-00001d50: 2c20 302e 3230 3732 3439 3733 3539 3230  , 0.207249735920
-00001d60: 3036 3365 382c 2030 2e32 3130 3632 3431  063e8, 0.2106241
-00001d70: 3130 3933 3732 3432 6538 2c20 302e 3231  10937242e8, 0.21
-00001d80: 3432 3431 3833 3238 3335 3636 3565 382c  4241832835665e8,
-00001d90: 2030 2e32 3138 3132 3438 3038 3336 3735   0.2181248083675
-00001da0: 3530 6538 2c0d 0a30 2e32 3232 3239 3739  50e8,..0.2222979
-00001db0: 3130 3839 3934 3532 6538 2c20 302e 3232  10899452e8, 0.22
-00001dc0: 3637 3839 3439 3330 3939 3930 3565 382c  6789493099905e8,
-00001dd0: 2030 2e32 3331 3633 3230 3131 3134 3634   0.2316320111464
-00001de0: 3433 6538 2c20 302e 3233 3638 3632 3738  43e8, 0.23686278
-00001df0: 3938 3931 3830 3465 382c 302e 3234 3235  9891804e8,0.2425
-00001e00: 3234 3936 3736 3933 3832 3965 382c 2030  24967693829e8, 0
-00001e10: 2e32 3438 3636 3836 3732 3330 3133 3036  .248668672301306
-00001e20: 6538 2c0d 0a30 2e32 3535 3335 3234 3936  e8,..0.255352496
-00001e30: 3736 3639 3237 6538 2c20 302e 3236 3236  766927e8, 0.2626
-00001e40: 3435 3336 3930 3232 3438 3565 382c 2030  45369022485e8, 0
-00001e50: 2e32 3730 3632 3839 3433 3832 3930 3438  .270628943829048
-00001e60: 6538 2c20 302e 3237 3934 3030 3639 3634  e8, 0.2794006964
-00001e70: 3433 3336 3665 382c 2030 2e32 3839 3037  43366e8, 0.28907
-00001e80: 3739 3731 3539 3539 3130 6538 2c20 302e  7971595910e8, 0.
-00001e90: 3239 3938 3033 3335 3232 3034 3536 3965  299803352204569e
-00001ea0: 382c 0d0a 302e 3331 3137 3531 3838 3038  8,..0.3117518808
-00001eb0: 3734 3535 3265 382c 2030 2e33 3235 3134  74552e8, 0.32514
-00001ec0: 3039 3239 3239 3331 3033 6538 2c30 2e33  0929293103e8,0.3
-00001ed0: 3430 3234 3339 3237 3535 3433 3838 6538  40243927554388e8
-00001ee0: 2c20 302e 3335 3734 3039 3834 3633 3436  , 0.357409846346
-00001ef0: 3233 3665 382c 2030 2e33 3737 3039 3134  236e8, 0.3770914
-00001f00: 3730 3033 3732 3536 6538 2c20 302e 3339  70037256e8, 0.39
-00001f10: 3938 3837 3438 3934 3532 3631 3265 382c  9887489452612e8,
-00001f20: 0d0a 302e 3432 3636 3037 3033 3734 3037  ..0.426607037407
-00001f30: 3830 3365 382c 2030 2e34 3538 3337 3230  803e8, 0.4583720
-00001f40: 3638 3339 3531 3334 6538 2c20 302e 3439  68395134e8, 0.49
-00001f50: 3637 3836 3433 3233 3138 3835 3565 382c  6786432318855e8,
-00001f60: 2030 2e35 3434 3232 3838 3234 3030 3135   0.5442288240015
-00001f70: 3436 6538 2c20 302e 3630 3433 3930 3934  46e8, 0.60439094
-00001f80: 3034 3638 3530 3865 382c 2030 2e36 3833  0468508e8, 0.683
-00001f90: 3334 3038 3932 3533 3736 3831 6538 2c0d  340892537681e8,.
-00001fa0: 0a30 2e37 3931 3833 3131 3538 3837 3031  .0.7918311588701
-00001fb0: 3138 6538 2c20 302e 3935 3039 3738 3839  18e8, 0.95097889
-00001fc0: 3833 3738 3238 3065 382c 2031 2e32 3038  8378280e8, 1.208
-00001fd0: 3939 3133 3137 3838 3732 3936 6538 2c20  991317887296e8, 
-00001fe0: 312e 3730 3634 3931 3830 3730 3830 3531  1.70649180708051
-00001ff0: 3120 7d2c 0d0a 0d0a 2e50 4152 414d 5f52  1 },.....PARAM_R
-00002000: 203d 2032 2e34 3137 3535 3930 3136 3233   = 2.41755901623
-00002010: 3635 302c 0d0a 2e49 4e56 5f50 4152 414d  650,...INV_PARAM
-00002020: 5f52 203d 2030 2e34 3133 3634 3033 3637  _R = 0.413640367
-00002030: 3532 3933 3637 0d0a 7d3b 0d0a 0d0a 0d0a  529367..};......
-00002040: 766f 6964 2070 6367 5f67 6175 7373 2846  void pcg_gauss(F
-00002050: 3332 5054 5220 524e 442c 2069 6e74 204e  32PTR RND, int N
-00002060: 290d 0a7b 0d0a 0966 6f72 2028 696e 7420  )..{...for (int 
-00002070: 6920 3d20 313b 2069 203c 3d20 4e3b 2069  i = 1; i <= N; i
-00002080: 2b2b 290d 0a09 7b0d 0a09 0955 3332 2072  ++)...{....U32 r
-00002090: 6e64 5b32 5d3b 0d0a 0909 7063 675f 7261  nd[2];....pcg_ra
-000020a0: 6e64 6f6d 2872 6e64 2c20 3229 3b0d 0a0d  ndom(rnd, 2);...
-000020b0: 0a09 0955 3332 2055 3234 203d 2072 6e64  ...U32 U24 = rnd
-000020c0: 5b30 5d3b 0d0a 0909 5530 3820 2075 3820  [0];....U08  u8 
-000020d0: 3d20 5532 3420 2620 3078 6666 3b0d 0a09  = U24 & 0xff;...
-000020e0: 0955 3234 203d 2055 3234 203e 3e20 383b  .U24 = U24 >> 8;
-000020f0: 0d0a 0909 696e 7420 7369 676e 203d 2028  ....int sign = (
-00002100: 7538 2026 2030 7838 3029 203f 202b 3120  u8 & 0x80) ? +1 
-00002110: 3a20 2d31 3b0d 0a09 0975 3820 3d20 7538  : -1;....u8 = u8
-00002120: 2026 2030 7833 663b 0d0a 0d0a 0909 4633   & 0x3f;......F3
-00002130: 3220 783b 0d0a 0909 4936 3420 4944 5820  2 x;....I64 IDX 
-00002140: 3d20 7538 3b0d 0a09 0969 6620 2875 3820  = u8;....if (u8 
-00002150: 3c20 3633 290d 0a09 097b 0d0a 0909 0946  < 63)....{.....F
-00002160: 3332 2064 656c 7461 3b0d 0a09 0909 6465  32 delta;.....de
-00002170: 6c74 6120 3d20 2847 4155 5353 2e78 5b49  lta = (GAUSS.x[I
-00002180: 4458 202b 2031 5d20 2d20 4741 5553 532e  DX + 1] - GAUSS.
-00002190: 785b 4944 585d 2920 2a20 322e 3332 3833  x[IDX]) * 2.3283
-000021a0: 3036 3433 3635 3338 3639 3665 2d31 3066  06436538696e-10f
-000021b0: 3b2f 2f64 6976 6964 6564 2062 7920 325e  ;//divided by 2^
-000021c0: 3332 3b0d 0a09 0909 7768 696c 6520 2831  32;.....while (1
-000021d0: 2920 7b0d 0a09 0909 0978 203d 2047 4155  ) {......x = GAU
-000021e0: 5353 2e78 5b49 4458 5d20 2b20 6465 6c74  SS.x[IDX] + delt
-000021f0: 612a 2846 3332 2972 6e64 5b31 5d3b 0d0a  a*(F32)rnd[1];..
-00002200: 0909 0909 6966 2028 5532 3420 3c3d 2047  ....if (U24 <= G
-00002210: 4155 5353 2e79 5261 7469 6f5b 4944 585d  AUSS.yRatio[IDX]
-00002220: 2920 0d0a 0909 0909 0962 7265 616b 3b0d  ) .......break;.
-00002230: 0a09 0909 0969 6620 2855 3234 203c 3d20  .....if (U24 <= 
-00002240: 6578 7066 282d 302e 3566 2a78 2a78 292a  expf(-0.5f*x*x)*
-00002250: 2047 4155 5353 2e79 496e 7665 7273 655b   GAUSS.yInverse[
-00002260: 4944 585d 290d 0a09 0909 0909 6272 6561  IDX]).......brea
-00002270: 6b3b 0d0a 0909 0909 7063 675f 7261 6e64  k;......pcg_rand
-00002280: 6f6d 2872 6e64 2c20 3229 3b0d 0a09 0909  om(rnd, 2);.....
-00002290: 0955 3234 203d 2072 6e64 5b30 5d20 3e3e  .U24 = rnd[0] >>
-000022a0: 2038 3b0d 0a09 0909 7d0d 0a09 097d 0d0a   8;.....}....}..
-000022b0: 0909 656c 7365 0d0a 0909 7b0d 0a09 0909  ..else....{.....
-000022c0: 4633 3220 5531 2c20 5532 3b0d 0a0d 0a09  F32 U1, U2;.....
-000022d0: 0909 5532 203d 2028 4633 3229 5532 342a  ..U2 = (F32)U24*
-000022e0: 2035 2e39 3630 3436 3434 3737 3533 3930   5.9604644775390
-000022f0: 3633 652d 3038 663b 202f 2f20 6469 7675  63e-08f; // divu
-00002300: 6465 6420 6279 2032 5e32 340d 0a09 0909  ded by 2^24.....
-00002310: 7768 696c 6520 2831 290d 0a09 0909 7b0d  while (1).....{.
-00002320: 0a09 0909 0955 3120 3d20 726e 645b 315d  .....U1 = rnd[1]
-00002330: 202a 2032 2e33 3238 3330 3634 3336 3533   * 2.32830643653
-00002340: 3836 3936 652d 3130 663b 202f 2f64 6976  8696e-10f; //div
-00002350: 6964 6565 6420 6279 2032 5e33 320d 0a09  ideed by 2^32...
-00002360: 0909 0955 3120 3d20 3120 2d20 5531 3b0d  ...U1 = 1 - U1;.
-00002370: 0a0d 0a09 0909 0978 203d 2047 4155 5353  .......x = GAUSS
-00002380: 2e50 4152 414d 5f52 202d 206c 6f67 6628  .PARAM_R - logf(
-00002390: 5531 2920 2a47 4155 5353 2e49 4e56 5f50  U1) *GAUSS.INV_P
-000023a0: 4152 414d 5f52 3b0d 0a09 0909 0969 6620  ARAM_R;......if 
-000023b0: 2865 7870 282d 4741 5553 532e 5041 5241  (exp(-GAUSS.PARA
-000023c0: 4d5f 5220 2a20 2878 202d 2030 2e35 6620  M_R * (x - 0.5f 
-000023d0: 2a20 4741 5553 532e 5041 5241 4d5f 5229  * GAUSS.PARAM_R)
-000023e0: 2920 2a20 5532 2020 3c20 6578 7066 282d  ) * U2  < expf(-
-000023f0: 302e 3566 202a 2078 202a 2078 2929 0d0a  0.5f * x * x))..
-00002400: 0909 0909 0962 7265 616b 3b0d 0a0d 0a09  .....break;.....
-00002410: 0909 0970 6367 5f72 616e 646f 6d28 726e  ...pcg_random(rn
-00002420: 642c 2032 293b 0d0a 0909 0909 5532 203d  d, 2);......U2 =
-00002430: 2072 6e64 5b30 5d20 2a20 322e 3332 3833   rnd[0] * 2.3283
-00002440: 3036 3433 3635 3338 3639 3665 2d31 3066  06436538696e-10f
-00002450: 3b0d 0a0d 0a09 0909 7d0d 0a09 097d 0d0a  ;.......}....}..
-00002460: 0d0a 0909 2a52 4e44 2b2b 203d 2078 2a73  ....*RND++ = x*s
-00002470: 6967 6e3b 0d0a 097d 2f2f 436f 6d70 6c65  ign;...}//Comple
-00002480: 7469 6f6e 206f 6620 7468 6520 466f 7220  tion of the For 
-00002490: 6c6f 6f70 0d0a 7d0d 0a20 0d0a 766f 6964  loop..}.. ..void
-000024a0: 2070 6367 5f67 616d 6d61 2846 3332 5054   pcg_gamma(F32PT
-000024b0: 5220 726e 642c 2046 3332 2061 2c20 696e  R rnd, F32 a, in
-000024c0: 7420 4e29 0d0a 7b0d 0a09 2f2a 0d0a 0925  t N)..{.../*...%
-000024d0: 2054 6869 7320 6675 6e63 7469 6f6e 2069   This function i
-000024e0: 7320 7573 6564 2074 6f20 6472 6177 2067  s used to draw g
-000024f0: 616d 6d61 2072 616e 646f 6d20 7661 7269  amma random vari
-00002500: 6162 6c65 732e 0d0a 0925 2049 2063 616e  ables....% I can
-00002510: 2774 2072 656d 656d 6265 7220 7768 6f20  't remember who 
-00002520: 4920 6e69 636b 6564 2074 6869 7320 6f66  I nicked this of
-00002530: 663f 3f3f 3f0d 0a09 2520 6966 2079 6f75  f????...% if you
-00002540: 206c 6574 206d 6520 6b6e 6f77 2074 6865   let me know the
-00002550: 6e20 4927 6c6c 2063 7265 6469 7420 7468  n I'll credit th
-00002560: 656d 2c20 706c 6561 7365 2065 6d61 696c  em, please email
-00002570: 206d 652e 0d0a 0925 0d0a 0925 2049 7420   me....%...% It 
-00002580: 7761 7320 6164 6461 7074 6564 2066 726f  was addapted fro
-00002590: 6d2e 2e2e 2e2e 2e2e 2e0d 0a09 250d 0a09  m...........%...
-000025a0: 2520 5241 4e44 4741 4d4d 2047 656e 6572  % RANDGAMM Gener
-000025b0: 6174 6573 204e 2067 616d 6d61 2072 616e  ates N gamma ran
-000025c0: 646f 6d20 6465 7669 6174 6573 2e0d 0a09  dom deviates....
-000025d0: 2520 2020 2020 5241 4e44 4741 4d4d 2841  %     RANDGAMM(A
-000025e0: 2c20 4e29 2069 7320 6120 7261 6e64 6f6d  , N) is a random
-000025f0: 2064 6576 6961 7465 2066 726f 6d20 7468   deviate from th
-00002600: 6520 7374 616e 6461 7264 2067 616d 6d61  e standard gamma
-00002610: 0d0a 0925 2020 2020 2064 6973 7472 6962  ...%     distrib
-00002620: 7574 696f 6e20 7769 7468 2073 6861 7065  ution with shape
-00002630: 2070 6172 616d 6574 6572 2041 2e0d 0a09   parameter A....
-00002640: 250d 0a09 2520 2020 2020 422a 5241 4e44  %...%     B*RAND
-00002650: 4741 4d4d 2841 2c20 4e29 2069 7320 6120  GAMM(A, N) is a 
-00002660: 7261 6e64 6f6d 2064 6576 6961 7465 2066  random deviate f
-00002670: 726f 6d20 7468 6520 6761 6d6d 6120 6469  rom the gamma di
-00002680: 7374 7269 6275 7469 6f6e 0d0a 0925 2020  stribution...%  
-00002690: 2020 2077 6974 6820 7368 6170 6520 7061     with shape pa
-000026a0: 7261 6d65 7465 7220 4120 616e 6420 7363  rameter A and sc
-000026b0: 616c 6520 7061 7261 6d65 7465 7220 422e  ale parameter B.
-000026c0: 5468 6520 6469 7374 7269 6275 7469 6f6e  The distribution
-000026d0: 0d0a 0925 2020 2020 2074 6865 6e20 6861  ...%     then ha
-000026e0: 7320 6d65 616e 2041 2a42 2061 6e64 2076  s mean A*B and v
-000026f0: 6172 6961 6e63 6520 412a 425e 322e 0d0a  ariance A*B^2...
-00002700: 0925 0d0a 0925 2020 2020 2053 6565 2052  .%...%     See R
-00002710: 414e 442e 0d0a 0925 2047 4b53 2033 3120  AND....% GKS 31 
-00002720: 4a75 6c79 2039 330d 0a09 2520 416c 676f  July 93...% Algo
-00002730: 7269 7468 6d20 666f 7220 4120 3e3d 2031  rithm for A >= 1
-00002740: 2069 7320 4265 7374 2773 2072 656a 6563   is Best's rejec
-00002750: 7469 6f6e 2061 6c67 6f72 6974 686d 2058  tion algorithm X
-00002760: 470d 0a09 2520 4164 6170 7465 6420 6672  G...% Adapted fr
-00002770: 6f6d 204c 2e44 6576 726f 7965 2c20 224e  om L.Devroye, "N
-00002780: 6f6e 2d75 6e69 666f 726d 2072 616e 646f  on-uniform rando
-00002790: 6d20 7661 7269 6174 650d 0a09 2520 6765  m variate...% ge
-000027a0: 6e65 7261 7469 6f6e 222c 2053 7072 696e  neration", Sprin
-000027b0: 6765 722d 5665 726c 6167 2c20 4e65 7720  ger-Verlag, New 
-000027c0: 596f 726b 2c20 3139 3836 2c20 702e 2034  York, 1986, p. 4
-000027d0: 3130 2e0d 0a09 2520 416c 676f 7269 7468  10....% Algorith
-000027e0: 6d20 666f 7220 4120 3c20 3120 6973 2072  m for A < 1 is r
-000027f0: 656a 6563 7469 6f6e 2061 6c67 6f72 6974  ejection algorit
-00002800: 686d 2047 5320 6672 6f6d 0d0a 0925 2041  hm GS from...% A
-00002810: 6872 656e 732c 204a 2e48 2e61 6e64 2044  hrens, J.H.and D
-00002820: 6965 7465 722c 2055 2e43 6f6d 7075 7465  ieter, U.Compute
-00002830: 7220 6d65 7468 6f64 7320 666f 7220 7361  r methods for sa
-00002840: 6d70 6c69 6e67 0d0a 0925 2066 726f 6d20  mpling...% from 
-00002850: 6761 6d6d 612c 2062 6574 612c 2050 6f69  gamma, beta, Poi
-00002860: 7373 6f6e 2061 6e64 2062 696e 6f6d 6961  sson and binomia
-00002870: 6c20 6469 7374 7269 6275 7469 6f6e 732e  l distributions.
-00002880: 0d0a 0925 2043 6f6d 7075 7469 6e67 2c20  ...% Computing, 
-00002890: 3132 2028 3139 3734 292c 2032 3233 202d  12 (1974), 223 -
-000028a0: 2032 3436 2e20 2041 6461 7074 6564 2066   246.  Adapted f
-000028b0: 726f 6d20 4e65 746c 6962 0d0a 0925 2046  rom Netlib...% F
-000028c0: 6f72 7472 616e 2072 6f75 7469 6e65 2e0d  ortran routine..
-000028d0: 0a0d 0a09 6761 6d6d 615f 7374 6f72 6520  ....gamma_store 
-000028e0: 3d20 7a65 726f 7328 4e2c 204d 293b 0d0a  = zeros(N, M);..
-000028f0: 092a 2f0d 0a09 4633 3220 494e 565f 4d41  .*/...F32 INV_MA
-00002900: 5820 3d20 322e 3332 3833 3036 3433 3635  X = 2.3283064365
-00002910: 3338 3639 3665 2d31 3066 3b0d 0a09 6966  38696e-10f;...if
-00002920: 2028 6120 3e3d 2031 290d 0a09 7b0d 0a09   (a >= 1)...{...
-00002930: 0946 3332 2062 203d 2061 202d 2031 2e30  .F32 b = a - 1.0
-00002940: 663b 0d0a 0909 4633 3220 6320 3d20 6120  f;....F32 c = a 
-00002950: 2b20 6120 2b20 6120 2d20 302e 3735 663b  + a + a - 0.75f;
-00002960: 0d0a 0d0a 0909 666f 7220 2869 6e74 2069  ......for (int i
-00002970: 203d 2030 3b20 6920 3c20 4e3b 2069 2b2b   = 0; i < N; i++
-00002980: 290d 0a09 097b 0d0a 0909 0946 3332 2067  )....{.....F32 g
-00002990: 616d 3b0d 0a09 0909 7768 696c 6520 2831  am;.....while (1
-000029a0: 290d 0a09 0909 7b0d 0a0d 0a09 0909 090d  ).....{.........
-000029b0: 0a2f 2f23 6966 2064 6566 696e 6564 285f  .//#if defined(_
-000029c0: 5f47 4e55 435f 5f29 207c 7c20 6465 6669  _GNUC__) || defi
-000029d0: 6e65 6428 5f5f 434c 414e 475f 5f29 200d  ned(__CLANG__) .
-000029e0: 0a2f 2f09 4449 5341 424c 455f 5741 524e  .//.DISABLE_WARN
-000029f0: 494e 4728 7374 7269 6374 2d61 6c69 6173  ING(strict-alias
-00002a00: 696e 672c 2073 7472 6963 742d 616c 6961  ing, strict-alia
-00002a10: 7369 6e67 2c20 4e4f 545f 5553 4544 290d  sing, NOT_USED).
-00002a20: 0a2f 2f23 656e 6469 660d 0a09 0909 0946  .//#endif......F
-00002a30: 3332 2075 5b32 5d3b 0d0a 0909 0909 7063  32 u[2];......pc
-00002a40: 675f 7261 6e64 6f6d 2828 5533 3250 5452  g_random((U32PTR
-00002a50: 2975 2c20 3229 3b0d 0a09 0909 0975 5b30  )u, 2);......u[0
-00002a60: 5d20 3d20 2846 3332 2928 2a28 5533 3250  ] = (F32)(*(U32P
-00002a70: 5452 2926 755b 305d 2920 2a20 494e 565f  TR)&u[0]) * INV_
-00002a80: 4d41 583b 0d0a 0909 0909 755b 315d 203d  MAX;......u[1] =
-00002a90: 2028 4633 3229 282a 2855 3332 5054 5229   (F32)(*(U32PTR)
-00002aa0: 2675 5b31 5d29 202a 2049 4e56 5f4d 4158  &u[1]) * INV_MAX
-00002ab0: 3b0d 0a0d 0a09 0909 0946 3332 2077 203d  ;........F32 w =
-00002ac0: 2075 5b30 5d20 2a20 2831 202d 2075 5b30   u[0] * (1 - u[0
-00002ad0: 5d29 3b0d 0a09 0909 0946 3332 2079 203d  ]);......F32 y =
-00002ae0: 2073 7172 7466 2863 202f 2077 2920 2a20   sqrtf(c / w) * 
-00002af0: 2875 5b30 5d20 2d20 302e 3566 293b 0d0a  (u[0] - 0.5f);..
-00002b00: 0909 0909 6761 6d20 3d20 6220 2b20 793b  ....gam = b + y;
-00002b10: 0d0a 0909 0909 6966 2028 6761 6d20 3e3d  ......if (gam >=
-00002b20: 2030 290d 0a09 0909 097b 0d0a 0909 0909   0)......{......
-00002b30: 0946 3332 207a 203d 2036 342e 3066 202a  .F32 z = 64.0f *
-00002b40: 2028 772a 772a 7729 202a 2028 755b 315d   (w*w*w) * (u[1]
-00002b50: 202a 2075 5b31 5d29 3b0d 0a09 0909 0909   * u[1]);.......
-00002b60: 6966 2028 7a20 3c3d 2028 3120 2d20 3220  if (z <= (1 - 2 
-00002b70: 2a20 2879 2a79 2920 2f20 6761 6d29 290d  * (y*y) / gam)).
-00002b80: 0a09 0909 0909 0962 7265 616b 3b0d 0a0d  .......break;...
-00002b90: 0a09 0909 0909 4633 3220 6c6f 675a 203d  ......F32 logZ =
-00002ba0: 206c 6f67 6628 7a29 3b0d 0a09 0909 0909   logf(z);.......
-00002bb0: 6966 2028 6220 3d3d 2030 2909 0909 0909  if (b == 0).....
-00002bc0: 7b0d 0a09 0909 0909 0969 6620 286c 6f67  {........if (log
-00002bd0: 5a20 3c3d 202d 3220 2a20 7929 2062 7265  Z <= -2 * y) bre
-00002be0: 616b 3b0d 0a09 0909 0909 7d09 0965 6c73  ak;.......}..els
-00002bf0: 6509 0909 0909 7b0d 0a09 0909 0909 0969  e.....{........i
-00002c00: 6620 286c 6f67 5a20 3c3d 2032 202a 2028  f (logZ <= 2 * (
-00002c10: 6220 2a20 6c6f 6766 2867 616d 202f 2062  b * logf(gam / b
-00002c20: 2920 2d20 7929 2920 6272 6561 6b3b 0d0a  ) - y)) break;..
-00002c30: 0909 0909 097d 0d0a 0909 0909 7d20 2f2f  .....}......} //
-00002c40: 454e 4420 6f66 2020 2867 616d 203e 3d20  END of  (gam >= 
-00002c50: 3029 0d0a 0d0a 0909 097d 2f2f 454e 4420  0).......}//END 
-00002c60: 5748 494c 450d 0a09 0909 2a72 6e64 2b2b  WHILE.....*rnd++
-00002c70: 203d 2067 616d 3b0d 0a0d 0a09 097d 2f2f   = gam;......}//
-00002c80: 454e 4420 464f 520d 0a09 0972 6574 7572  END FOR....retur
-00002c90: 6e3b 0d0a 097d 0d0a 0d0a 0969 6620 2861  n;...}.....if (a
-00002ca0: 203e 2030 2920 2f2f 2030 3c61 3c31 0d0a   > 0) // 0<a<1..
-00002cb0: 097b 0d0a 0909 4633 3220 6220 3d20 3120  .{....F32 b = 1 
-00002cc0: 2b20 2e33 3637 3837 3934 6620 2a20 613b  + .3678794f * a;
-00002cd0: 0d0a 0909 666f 7220 2869 6e74 2069 203d  ....for (int i =
-00002ce0: 2030 3b20 6920 3c20 4e3b 2069 2b2b 290d   0; i < N; i++).
-00002cf0: 0a09 097b 0d0a 0909 0946 3332 2067 616d  ...{.....F32 gam
-00002d00: 3b0d 0a09 0909 7768 696c 6520 2831 290d  ;.....while (1).
-00002d10: 0a09 0909 7b0d 0a2f 2f23 6966 2064 6566  ....{..//#if def
-00002d20: 696e 6564 285f 5f47 4e55 435f 5f29 207c  ined(__GNUC__) |
-00002d30: 7c20 6465 6669 6e65 6428 5f5f 434c 414e  | defined(__CLAN
-00002d40: 475f 5f29 200d 0a2f 2f09 4449 5341 424c  G__) ..//.DISABL
-00002d50: 455f 5741 524e 494e 4728 7374 7269 6374  E_WARNING(strict
-00002d60: 2d61 6c69 6173 696e 672c 2073 7472 6963  -aliasing, stric
-00002d70: 742d 616c 6961 7369 6e67 2c20 4e4f 545f  t-aliasing, NOT_
-00002d80: 5553 4544 290d 0a2f 2f23 656e 6469 660d  USED)..//#endif.
-00002d90: 0a09 0909 0946 3332 2075 5b32 5d3b 0d0a  .....F32 u[2];..
-00002da0: 0909 0909 7063 675f 7261 6e64 6f6d 2828  ....pcg_random((
-00002db0: 5533 3250 5452 2975 2c20 3229 3b0d 0a09  U32PTR)u, 2);...
-00002dc0: 0909 0975 5b30 5d20 3d20 2846 3332 2928  ...u[0] = (F32)(
-00002dd0: 2a28 5533 3250 5452 2926 755b 305d 2920  *(U32PTR)&u[0]) 
-00002de0: 2a20 494e 565f 4d41 583b 0d0a 0909 0909  * INV_MAX;......
-00002df0: 755b 315d 203d 2028 4633 3229 282a 2855  u[1] = (F32)(*(U
-00002e00: 3332 5054 5229 2675 5b31 5d29 202a 2049  32PTR)&u[1]) * I
-00002e10: 4e56 5f4d 4158 3b0d 0a2f 2f23 6966 2064  NV_MAX;..//#if d
-00002e20: 6566 696e 6564 285f 5f47 4e55 435f 5f29  efined(__GNUC__)
-00002e30: 207c 7c20 6465 6669 6e65 6428 5f5f 434c   || defined(__CL
-00002e40: 414e 475f 5f29 200d 0a2f 2f09 454e 4142  ANG__) ..//.ENAB
-00002e50: 4c45 5f57 4152 4e49 4e47 2873 7472 6963  LE_WARNING(stric
-00002e60: 742d 616c 6961 7369 6e67 2c20 7374 7269  t-aliasing, stri
-00002e70: 6374 2d61 6c69 6173 696e 672c 204e 4f54  ct-aliasing, NOT
-00002e80: 5f55 5345 4429 0d0a 2f2f 2365 6e64 6966  _USED)..//#endif
-00002e90: 0d0a 0909 0909 4633 3220 6320 3d20 6220  ......F32 c = b 
-00002ea0: 2a20 755b 305d 3b0d 0a09 0909 0969 6620  * u[0];......if 
-00002eb0: 2863 203c 2031 290d 0a09 0909 097b 0d0a  (c < 1)......{..
-00002ec0: 0909 0909 0967 616d 203d 2065 7870 6628  .....gam = expf(
-00002ed0: 6c6f 6766 2863 2920 2f20 6129 3b0d 0a09  logf(c) / a);...
-00002ee0: 0909 0909 6966 2028 2d6c 6f67 6628 3120  ....if (-logf(1 
-00002ef0: 2d20 755b 315d 2920 3e3d 2067 616d 2920  - u[1]) >= gam) 
-00002f00: 6272 6561 6b3b 0d0a 0909 0909 7d0d 0a09  break;......}...
-00002f10: 0909 0965 6c73 650d 0a09 0909 097b 0d0a  ...else......{..
-00002f20: 0909 0909 0967 616d 203d 202d 6c6f 6766  .....gam = -logf
-00002f30: 2828 6220 2d20 6329 202f 2061 293b 0d0a  ((b - c) / a);..
-00002f40: 0909 0909 0969 6620 282d 6c6f 6766 2831  .....if (-logf(1
-00002f50: 202d 2075 5b31 5d29 203e 3d20 2831 202d   - u[1]) >= (1 -
-00002f60: 2061 2920 2a20 6c6f 6766 2867 616d 2929   a) * logf(gam))
-00002f70: 0d0a 0909 0909 0909 6272 6561 6b3b 0d0a  ........break;..
-00002f80: 0909 0909 7d0d 0a09 0909 7d2f 2f45 4e44  ....}.....}//END
-00002f90: 2057 4849 4c45 0d0a 0909 092a 726e 642b   WHILE.....*rnd+
-00002fa0: 2b20 3d20 6761 6d3b 0d0a 0909 7d2f 2f45  + = gam;....}//E
-00002fb0: 4e44 2046 4f52 0d0a 0909 7265 7475 726e  ND FOR....return
-00002fc0: 3b0d 0a09 7d0d 0a0d 0a0d 0a09 6966 2028  ;...}.......if (
-00002fd0: 6120 3c20 302e 6629 2009 7b0d 0a09 0946  a < 0.f) .{....F
-00002fe0: 3332 206e 616e 203d 2067 6574 4e61 4e28  32 nan = getNaN(
-00002ff0: 293b 0d0a 0909 666f 7220 2869 6e74 2069  );....for (int i
-00003000: 203d 2030 3b20 6920 3c20 4e3b 2069 2b2b   = 0; i < N; i++
-00003010: 2909 092a 726e 642b 2b20 3d20 6e61 6e3b  )..*rnd++ = nan;
-00003020: 0d0a 0909 7265 7475 726e 3b0d 0a09 7d0d  ....return;...}.
-00003030: 0a0d 0a0d 0a09 6966 2028 6120 3d3d 2030  ......if (a == 0
-00003040: 2e66 2909 7b0d 0a09 0966 6f72 2028 696e  .f).{....for (in
-00003050: 7420 6920 3d20 303b 2069 203c 204e 3b20  t i = 0; i < N; 
-00003060: 692b 2b29 092a 726e 642b 2b20 3d20 302e  i++).*rnd++ = 0.
-00003070: 663b 0d0a 0909 7265 7475 726e 3b0d 0a09  f;....return;...
-00003080: 7d0d 0a0d 0a0d 0a7d 0d0a 0d0a 0d0a 766f  }......}......vo
-00003090: 6964 2020 7063 675f 7769 7368 6172 745f  id  pcg_wishart_
-000030a0: 756e 6974 5f6c 6f77 7472 6961 6e67 6c65  unit_lowtriangle
-000030b0: 5f6e 6f7a 6572 6f6f 7574 2846 3332 5054  _nozeroout(F32PT
-000030c0: 5220 726e 642c 2046 3332 5054 5220 746d  R rnd, F32PTR tm
-000030d0: 702c 2049 3332 206d 2c20 4633 3220 6466  p, I32 m, F32 df
-000030e0: 2029 0d0a 7b0d 0a09 4933 3220 4e20 3d20   )..{...I32 N = 
-000030f0: 286d 202d 2031 292a 6d20 2f20 323b 0d0a  (m - 1)*m / 2;..
-00003100: 2020 2020 2070 6367 5f67 6175 7373 2874       pcg_gauss(t
-00003110: 6d70 2c20 4e29 3b0d 0a0d 0a09 4633 3250  mp, N);.....F32P
-00003120: 5452 2074 7074 3b0d 0a09 7470 7420 3d20  TR tpt;...tpt = 
-00003130: 726e 6420 2b20 313b 0d0a 0d0a 0966 6f72  rnd + 1;.....for
-00003140: 2028 696e 7420 6920 3d20 313b 2069 3c6d   (int i = 1; i<m
-00003150: 2020 3b20 692b 2b29 0d0a 097b 0909 090d    ; i++)...{....
-00003160: 0a09 0949 3332 2020 6d6f 7645 6c65 6d20  ...I32  movElem 
-00003170: 3d20 6d20 2d20 693b 0d0a 0909 666f 7220  = m - i;....for 
-00003180: 2869 6e74 206a 203d 2030 3b20 6a20 3c20  (int j = 0; j < 
-00003190: 6d6f 7645 6c65 6d3b 206a 2b2b 290d 0a09  movElem; j++)...
-000031a0: 097b 0d0a 0909 092a 7470 742b 2b20 3d20  .{.....*tpt++ = 
-000031b0: 2a74 6d70 2b2b 3b0d 0a09 097d 0d0a 0909  *tmp++;....}....
-000031c0: 7470 7420 3d20 7470 7420 2b20 692b 313b  tpt = tpt + i+1;
-000031d0: 0d0a 097d 0d0a 090d 0a09 746d 7020 3d20  ...}......tmp = 
-000031e0: 726e 643b 0d0a 0966 6f72 2028 696e 7420  rnd;...for (int 
-000031f0: 6920 3d20 313b 2069 203c 3d6d 3b20 692b  i = 1; i <=m; i+
-00003200: 2b29 0d0a 097b 0d0a 0909 7063 675f 6761  +)...{....pcg_ga
-00003210: 6d6d 6128 746d 702c 2028 4633 3229 2864  mma(tmp, (F32)(d
-00003220: 662d 692b 312e 292f 2032 2e66 2c20 3129  f-i+1.)/ 2.f, 1)
-00003230: 3b0d 0a09 092a 746d 7020 3d20 7371 7274  ;....*tmp = sqrt
-00003240: 6628 282a 746d 7029 202a 2032 2e66 293b  f((*tmp) * 2.f);
-00003250: 0d0a 0909 746d 7020 3d20 746d 7020 2b20  ....tmp = tmp + 
-00003260: 286d 202b 2031 293b 0d0a 097d 0d0a 0d0a  (m + 1);...}....
-00003270: 7d0d 0a0d 0a76 6f69 6420 7063 675f 7769  }....void pcg_wi
-00003280: 7368 6172 745f 756e 6974 5f6c 6f77 7472  shart_unit_lowtr
-00003290: 6961 6e67 6c65 5f6e 6f7a 6572 6f6f 7574  iangle_nozeroout
-000032a0: 5f6e 6f74 6d70 2846 3332 5054 5220 7769  _notmp(F32PTR wi
-000032b0: 7368 726e 642c 2049 3332 206d 2c20 4633  shrnd, I32 m, F3
-000032c0: 3220 6466 290d 0a7b 0d0a 092f 2f20 5468  2 df)..{...// Th
-000032d0: 6973 2069 7320 616e 2069 6d70 6c6d 656e  is is an implmen
-000032e0: 7461 7469 6f6e 206f 6620 7468 6520 4261  tation of the Ba
-000032f0: 726c 6c65 7420 616c 676f 7274 6968 6d0d  rllet algortihm.
-00003300: 0a09 6d65 6d73 6574 2877 6973 6872 6e64  ..memset(wishrnd
-00003310: 2c20 302c 2073 697a 656f 6628 4633 3229  , 0, sizeof(F32)
-00003320: 202a 206d 202a 206d 293b 0d0a 0d0a 092f   * m * m);...../
-00003330: 2f20 7468 6520 6e75 6d62 6572 206f 6620  / the number of 
-00003340: 656c 656d 6e74 7320 6265 6c6f 7720 7468  elemnts below th
-00003350: 6520 6469 6167 6f6e 616c 3a20 2830 2b20  e diagonal: (0+ 
-00003360: 286d 3d31 2929 2a6d 2f32 0d0a 0949 3332  (m=1))*m/2...I32
-00003370: 2020 2020 206e 756d 4761 7573 7352 6e64       numGaussRnd
-00003380: 203d 2028 6d20 2d20 3129 202a 206d 202f   = (m - 1) * m /
-00003390: 2032 3b0d 0a09 4633 3250 5452 2020 6761   2;...F32PTR  ga
-000033a0: 7573 7320 2020 2020 2020 3d20 7769 7368  uss       = wish
-000033b0: 726e 6420 2b20 6d20 2a20 6d20 202d 206e  rnd + m * m  - n
-000033c0: 756d 4761 7573 7352 6e64 3b0d 0a09 7063  umGaussRnd;...pc
-000033d0: 675f 6761 7573 7328 6761 7573 732c 206e  g_gauss(gauss, n
-000033e0: 756d 4761 7573 7352 6e64 293b 0d0a 0d0a  umGaussRnd);....
-000033f0: 0966 6f72 2028 696e 7420 636f 6c20 3d20  .for (int col = 
-00003400: 313b 2063 6f6c 203c 206d 3b20 2b2b 636f  1; col < m; ++co
-00003410: 6c29 207b 0d0a 0909 666f 7220 2869 6e74  l) {....for (int
-00003420: 2072 6f77 203d 2063 6f6c 202b 2031 3b20   row = col + 1; 
-00003430: 726f 7720 3c3d 206d 3b20 726f 772b 2b29  row <= m; row++)
-00003440: 207b 0d0a 0909 0977 6973 6872 6e64 5b72   {.....wishrnd[r
-00003450: 6f77 202d 2031 5d20 3d20 2a67 6175 7373  ow - 1] = *gauss
-00003460: 2b2b 3b0d 0a09 097d 0d0a 0909 7769 7368  ++;....}....wish
-00003470: 726e 6420 2b3d 206d 3b0d 0a09 7d0d 0a09  rnd += m;...}...
-00003480: 7769 7368 726e 6420 2d3d 2028 6d20 2d20  wishrnd -= (m - 
-00003490: 3129 202a 206d 3b20 202f 2f67 6f20 6261  1) * m;  //go ba
-000034a0: 636b 2074 6f20 7468 6520 7374 6172 7420  ck to the start 
-000034b0: 6f66 2072 6e64 0d0a 0d0a 2020 202f 2f20  of rnd....   // 
-000034c0: 2046 696c 6c20 7468 6520 6469 6167 6f6e   Fill the diagon
-000034d0: 6c20 7769 7468 2067 616d 6d61 2072 616e  l with gamma ran
-000034e0: 646f 6d20 7661 7269 6162 6c65 730d 0a09  dom variables...
-000034f0: 666f 7220 2869 6e74 2069 203d 2031 3b20  for (int i = 1; 
-00003500: 6920 3c3d 206d 3b20 692b 2b29 207b 0d0a  i <= m; i++) {..
-00003510: 0909 4633 3220 6368 6973 7161 7572 653b  ..F32 chisqaure;
-00003520: 0d0a 0909 7063 675f 6761 6d6d 6128 2663  ....pcg_gamma(&c
-00003530: 6869 7371 6175 7265 2c20 2846 3332 2928  hisqaure, (F32)(
-00003540: 6466 202d 2069 202b 2031 2920 2f20 322e  df - i + 1) / 2.
-00003550: 662c 2031 293b 0d0a 0909 2a77 6973 6872  f, 1);....*wishr
-00003560: 6e64 203d 2063 6869 7371 6175 7265 203d  nd = chisqaure =
-00003570: 2073 7172 7466 2863 6869 7371 6175 7265   sqrtf(chisqaure
-00003580: 202a 2032 2e66 293b 0d0a 0909 7769 7368   * 2.f);....wish
-00003590: 726e 6420 2b3d 2028 6d20 2b20 3129 3b0d  rnd += (m + 1);.
-000035a0: 0a09 7d0d 0a0d 0a7d 0d0a 0d0a 200d 0a0d  ..}....}.... ...
-000035b0: 0a20 0d0a 0d0a 766f 6964 2020 7063 675f  . ....void  pcg_
-000035c0: 7769 7368 6172 745f 756e 6974 5f6c 6f77  wishart_unit_low
-000035d0: 7472 6961 6e67 6c65 5f7a 6572 6f6f 7574  triangle_zeroout
-000035e0: 5f6e 6f74 6d70 2846 3332 5054 5220 7769  _notmp(F32PTR wi
-000035f0: 7368 726e 642c 2049 3332 206d 2c20 4633  shrnd, I32 m, F3
-00003600: 3220 6466 290d 0a7b 0d0a 092f 2f20 5468  2 df)..{...// Th
-00003610: 6973 2069 7320 616e 2069 6d70 6c6d 656e  is is an implmen
-00003620: 7461 7469 6f6e 206f 6620 7468 6520 4261  tation of the Ba
-00003630: 726c 6c65 7420 616c 676f 7274 6968 6d0d  rllet algortihm.
-00003640: 0a20 0d0a 092f 2a0d 0a09 2f2f 2074 6865  . .../*...// the
-00003650: 206e 756d 6265 7220 6f66 2065 6c65 6d6e   number of elemn
-00003660: 7473 2062 656c 6f77 2074 6865 2064 6961  ts below the dia
-00003670: 676f 6e61 6c3a 2028 302b 2028 6d3d 3129  gonal: (0+ (m=1)
-00003680: 292a 6d2f 3209 200d 0a09 4933 3220 2020  )*m/2. ...I32   
-00003690: 2020 6e75 6d47 6175 7373 526e 6420 3d20    numGaussRnd = 
-000036a0: 286d 202d 2031 2920 2a20 6d20 2f20 323b  (m - 1) * m / 2;
-000036b0: 0d0a 0946 3332 5054 5220 2067 6175 7373  ...F32PTR  gauss
-000036c0: 203d 2020 7769 7368 726e 6420 2b20 6d20   =  wishrnd + m 
-000036d0: 2a20 6d20 2d20 6e75 6d47 6175 7373 526e  * m - numGaussRn
-000036e0: 643b 0d0a 096c 6f63 616c 5f70 6367 5f67  d;...local_pcg_g
-000036f0: 6175 7373 2872 6e67 2c20 6761 7573 7320  auss(rng, gauss 
-00003700: 2c20 6e75 6d47 6175 7373 526e 6429 3b0d  , numGaussRnd);.
-00003710: 0a09 0d0a 0966 6f72 2028 696e 7420 636f  .....for (int co
-00003720: 6c20 3d20 313b 2063 6f6c 203c 206d 3b20  l = 1; col < m; 
-00003730: 2b2b 636f 6c29 207b 0d0a 0909 666f 7220  ++col) {....for 
-00003740: 2869 6e74 2072 6f77 203d 2063 6f6c 202b  (int row = col +
-00003750: 2031 3b20 726f 7720 3c3d 206d 3b20 726f   1; row <= m; ro
-00003760: 772b 2b29 207b 0d0a 0909 0977 6973 6872  w++) {.....wishr
-00003770: 6e64 5b72 6f77 202d 2031 5d20 3d20 2a67  nd[row - 1] = *g
-00003780: 6175 7373 2b2b 3b0d 0a09 097d 0d0a 0909  auss++;....}....
-00003790: 7769 7368 726e 6420 2b3d 206d 3b0d 0a09  wishrnd += m;...
-000037a0: 7d0d 0a09 7769 7368 726e 6420 2d3d 2028  }...wishrnd -= (
-000037b0: 6d20 2d20 3129 202a 206d 3b20 202f 2f67  m - 1) * m;  //g
-000037c0: 6f20 6261 636b 2074 6f20 7468 6520 7374  o back to the st
-000037d0: 6172 7420 6f66 2072 6e64 0d0a 0920 2a2f  art of rnd... */
-000037e0: 0d0a 0d0a 200d 0a09 2f2f 2074 6865 206e  .... ...// the n
-000037f0: 756d 6265 7220 6f66 2065 6c65 6d6e 7473  umber of elemnts
-00003800: 2062 656c 6f77 2074 6865 2064 6961 676f   below the diago
-00003810: 6e61 6c3a 2028 302b 2028 6d3d 3129 292a  nal: (0+ (m=1))*
-00003820: 6d2f 3209 0d0a 0949 3332 2020 2020 206e  m/2....I32     n
-00003830: 756d 4761 7573 7352 6e64 203d 2028 6d20  umGaussRnd = (m 
-00003840: 2d20 3129 202a 206d 202f 2032 3b0d 0a09  - 1) * m / 2;...
-00003850: 4633 3250 5452 2020 6761 7573 7320 2020  F32PTR  gauss   
-00003860: 2020 2020 3d20 2077 6973 6872 6e64 202b      =  wishrnd +
-00003870: 2031 3b0d 0a09 7063 675f 6761 7573 7328   1;...pcg_gauss(
-00003880: 6761 7573 732c 206e 756d 4761 7573 7352  gauss, numGaussR
-00003890: 6e64 293b 0d0a 0967 6175 7373 203d 2067  nd);...gauss = g
-000038a0: 6175 7373 202b 206e 756d 4761 7573 7352  auss + numGaussR
-000038b0: 6e64 2d31 3b20 2f2f 676f 2074 6f20 7468  nd-1; //go to th
-000038c0: 6520 656e 6420 6f66 2074 6865 2067 7561  e end of the gua
-000038d0: 7373 0d0a 0d0a 0977 6973 6872 6e64 202b  ss.....wishrnd +
-000038e0: 3d20 286d 2d32 2920 2a20 6d3b 202f 2f20  = (m-2) * m; // 
-000038f0: 676f 2074 6f20 7468 6520 7374 6172 7420  go to the start 
-00003900: 6f66 2074 6865 2073 6563 6f6e 6420 726f  of the second ro
-00003910: 7720 6672 6f6d 2074 6865 206c 6173 740d  w from the last.
-00003920: 0a09 666f 7220 2869 6e74 2063 6f6c 203d  ..for (int col =
-00003930: 6d2d 313b 2063 6f6c 203e 3d32 3b20 636f  m-1; col >=2; co
-00003940: 6c2d 2d29 207b 0d0a 0909 666f 7220 2869  l--) {....for (i
-00003950: 6e74 2072 6f77 203d 206d 3b20 726f 7720  nt row = m; row 
-00003960: 3e3d 2063 6f6c 2b31 3b20 726f 772d 2d29  >= col+1; row--)
-00003970: 207b 0d0a 0909 0977 6973 6872 6e64 5b72   {.....wishrnd[r
-00003980: 6f77 202d 2031 5d20 3d20 2a67 6175 7373  ow - 1] = *gauss
-00003990: 2d2d 3b0d 0a09 097d 0d0a 0909 7769 7368  --;....}....wish
-000039a0: 726e 6420 2d3d 206d 3b0d 0a09 7d0d 0a09  rnd -= m;...}...
-000039b0: 2077 6973 6872 6e64 203d 2077 6973 6872   wishrnd = wishr
-000039c0: 6e64 3b20 202f 2f67 6f20 6261 636b 2074  nd;  //go back t
-000039d0: 6f20 7468 6520 7374 6172 7420 6f66 2072  o the start of r
-000039e0: 6e64 0d0a 0920 0d0a 0d0a 0d0a 0920 2f2f  nd... ....... //
-000039f0: 205a 6572 6f6f 7574 2074 6865 2075 7070   Zeroout the upp
-00003a00: 6572 2074 7269 616e 676c 650d 0a09 2066  er triangle... f
-00003a10: 6f72 2028 696e 7420 636f 6c20 3d20 303b  or (int col = 0;
-00003a20: 2063 6f6c 203c 6d3b 2063 6f6c 2b2b 2920   col <m; col++) 
-00003a30: 7b0d 0a09 0920 666f 7220 2869 6e74 2072  {.... for (int r
-00003a40: 6f77 203d 2030 3b20 726f 773c 636f 6c3b  ow = 0; row<col;
-00003a50: 2072 6f77 2b2b 2920 7b0d 0a09 0909 2077   row++) {..... w
-00003a60: 6973 6872 6e64 5b72 6f77 5d20 3d20 303b  ishrnd[row] = 0;
-00003a70: 0d0a 0909 207d 0d0a 0909 2077 6973 6872  .... }.... wishr
-00003a80: 6e64 202b 3d20 6d3b 0d0a 0920 7d0d 0a09  nd += m;... }...
-00003a90: 2077 6973 6872 6e64 203d 2077 6973 6872   wishrnd = wishr
-00003aa0: 6e64 202d 6d2a 6d3b 2020 2f2f 676f 2062  nd -m*m;  //go b
-00003ab0: 6163 6b20 746f 2074 6865 2073 7461 7274  ack to the start
-00003ac0: 206f 6620 726e 6409 0d0a 0d0a 2020 202f   of rnd.....   /
-00003ad0: 2f20 2046 696c 6c20 7468 6520 6469 6167  /  Fill the diag
-00003ae0: 6f6e 6c20 7769 7468 2067 616d 6d61 2072  onl with gamma r
-00003af0: 616e 646f 6d20 7661 7269 6162 6c65 730d  andom variables.
-00003b00: 0a09 666f 7220 2869 6e74 2069 203d 2031  ..for (int i = 1
-00003b10: 3b20 6920 3c3d 206d 3b20 692b 2b29 207b  ; i <= m; i++) {
-00003b20: 0d0a 0909 4633 3220 6368 6973 7161 7572  ....F32 chisqaur
-00003b30: 653b 0d0a 0909 7063 675f 6761 6d6d 6128  e;....pcg_gamma(
-00003b40: 2663 6869 7371 6175 7265 2c20 2846 3332  &chisqaure, (F32
-00003b50: 2928 6466 202d 2069 202b 2031 2920 2f20  )(df - i + 1) / 
-00003b60: 322e 662c 2031 293b 0d0a 0909 2a77 6973  2.f, 1);....*wis
-00003b70: 6872 6e64 203d 2063 6869 7371 6175 7265  hrnd = chisqaure
-00003b80: 203d 2073 7172 7466 2863 6869 7371 6175   = sqrtf(chisqau
-00003b90: 7265 202a 2032 2e66 293b 0d0a 0909 7769  re * 2.f);....wi
-00003ba0: 7368 726e 6420 2b3d 2028 6d20 2b20 3129  shrnd += (m + 1)
-00003bb0: 3b0d 0a09 7d0d 0a0d 0a7d 0d0a 0d0a 2369  ;...}....}....#i
-00003bc0: 6e63 6c75 6465 2022 6162 635f 6d61 742e  nclude "abc_mat.
-00003bd0: 6822 0d0a 766f 6964 2020 7063 675f 696e  h"..void  pcg_in
-00003be0: 7677 6973 6861 7274 5f75 7070 6572 2846  vwishart_upper(F
-00003bf0: 3332 5054 5220 6977 726e 645f 7570 7065  32PTR iwrnd_uppe
-00003c00: 722c 2046 3332 5054 5220 6977 726e 645f  r, F32PTR iwrnd_
-00003c10: 7570 7065 725f 696e 762c 2046 3332 5054  upper_inv, F32PT
-00003c20: 5220 746d 702c 2049 3332 206d 2c20 4633  R tmp, I32 m, F3
-00003c30: 3250 5452 2051 7570 2c20 4633 3220 6466  2PTR Qup, F32 df
-00003c40: 290d 0a7b 2020 200d 0a09 2f2f 4957 2851  )..{   ...//IW(Q
-00003c50: 2c76 293a 2051 3d51 7527 2a51 7570 0d0a  ,v): Q=Qu'*Qup..
-00003c60: 092f 2f54 6865 2049 5720 6d61 7472 6978  .//The IW matrix
-00003c70: 2073 686f 756c 6420 6265 2052 272a 5220   should be R'*R 
-00003c80: 7768 6572 6520 523d 6977 726e 645f 7570  where R=iwrnd_up
-00003c90: 7065 723d 2069 6e76 2857 292a 5175 700d  per= inv(W)*Qup.
-00003ca0: 0a09 2f2f 200d 0a09 2f2f 2069 7277 6e64  ..// ...// irwnd
-00003cb0: 5f75 7070 6572 5f69 6e76 2d20 696e 7628  _upper_inv- inv(
-00003cc0: 5229 3d69 6e76 2851 7570 292a 572e 0d0a  R)=inv(Qup)*W...
-00003cd0: 0920 0d0a 0946 3332 5054 5220 576c 6f77  . ...F32PTR Wlow
-00003ce0: 6572 203d 2074 6d70 3b0d 0a0d 0a09 2f2f  er = tmp;.....//
-00003cf0: 2054 6869 7320 6973 2061 6e20 696d 706c   This is an impl
-00003d00: 6d65 6e74 6174 696f 6e20 6f66 2074 6865  mentation of the
-00003d10: 2042 6172 6c6c 6574 2061 6c67 6f72 7469   Barllet algorti
-00003d20: 686d 0d0a 092f 2f6c 6f63 616c 5f70 6367  hm...//local_pcg
-00003d30: 5f77 6973 6861 7274 5f75 6e69 745f 6c6f  _wishart_unit_lo
-00003d40: 7774 7269 616e 676c 655f 6e6f 7a65 726f  wtriangle_nozero
-00003d50: 6f75 7428 726e 672c 2057 6c6f 7765 722c  out(rng, Wlower,
-00003d60: 2057 6c6f 7765 7220 2b6d 2a6d 2c20 6d2c   Wlower +m*m, m,
-00003d70: 2064 6629 3b0d 0a09 7063 675f 7769 7368   df);...pcg_wish
-00003d80: 6172 745f 756e 6974 5f6c 6f77 7472 6961  art_unit_lowtria
-00003d90: 6e67 6c65 5f7a 6572 6f6f 7574 5f6e 6f74  ngle_zeroout_not
-00003da0: 6d70 2857 6c6f 7765 722c 206d 2c20 6466  mp(Wlower, m, df
-00003db0: 293b 0d0a 090d 0a0d 0a09 2f2f 2053 6f6c  );........// Sol
-00003dc0: 7665 2057 6c2a 6977 726e 645f 7570 7065  ve Wl*iwrnd_uppe
-00003dd0: 723d 5175 700d 0a09 6633 325f 636f 7079  r=Qup...f32_copy
-00003de0: 2851 7570 2c20 6977 726e 645f 7570 7065  (Qup, iwrnd_uppe
-00003df0: 722c 206d 202a 206d 293b 0d0a 0966 6f72  r, m * m);...for
-00003e00: 2028 696e 7420 6920 3d20 303b 2069 203c   (int i = 0; i <
-00003e10: 206d 3b20 2b2b 6929 207b 0d0a 0909 736f   m; ++i) {....so
-00003e20: 6c76 655f 4c5f 6173 5f4c 2857 6c6f 7765  lve_L_as_L(Wlowe
-00003e30: 722c 2069 7772 6e64 5f75 7070 6572 2c20  r, iwrnd_upper, 
-00003e40: 6d2c 206d 293b 0d0a 0909 6977 726e 645f  m, m);....iwrnd_
-00003e50: 7570 7065 7220 3d20 6977 726e 645f 7570  upper = iwrnd_up
-00003e60: 7065 7220 2b20 6d3b 0d0a 097d 0d0a 0d0a  per + m;...}....
-00003e70: 090d 0a09 2f2f 536f 6c76 6520 5175 702a  ....//Solve Qup*
-00003e80: 6972 776e 645f 7570 7065 725f 696e 763d  irwnd_upper_inv=
-00003e90: 570d 0a09 6966 2028 6977 726e 645f 7570  W...if (iwrnd_up
-00003ea0: 7065 725f 696e 7629 207b 0d0a 0909 2f2f  per_inv) {....//
-00003eb0: 2069 7277 6e64 5f75 7070 6572 5f69 6e76   irwnd_upper_inv
-00003ec0: 2d69 6e76 2852 293d 696e 7628 5175 7029  -inv(R)=inv(Qup)
-00003ed0: 2a57 2e09 090d 0a09 0966 3332 5f63 6f70  *W.......f32_cop
-00003ee0: 7928 576c 6f77 6572 2c20 6977 726e 645f  y(Wlower, iwrnd_
-00003ef0: 7570 7065 725f 696e 762c 206d 202a 206d  upper_inv, m * m
-00003f00: 293b 0d0a 0909 666f 7220 2869 6e74 2069  );....for (int i
-00003f10: 203d 2030 3b20 6920 3c20 6d3b 202b 2b69   = 0; i < m; ++i
-00003f20: 2920 7b0d 0a09 0909 736f 6c76 655f 555f  ) {.....solve_U_
-00003f30: 6173 5f55 2851 7570 2c20 6977 726e 645f  as_U(Qup, iwrnd_
-00003f40: 7570 7065 725f 696e 762c 206d 2c20 6d29  upper_inv, m, m)
-00003f50: 3b0d 0a09 0909 6977 726e 645f 7570 7065  ;.....iwrnd_uppe
-00003f60: 725f 696e 7620 3d20 6977 726e 645f 7570  r_inv = iwrnd_up
-00003f70: 7065 725f 696e 7620 2b20 6d3b 0d0a 0909  per_inv + m;....
-00003f80: 7d0d 0a09 7d0d 0a09 0d0a 7d0d 0a0d 0a0d  }...}.....}.....
-00003f90: 0a23 696e 636c 7564 6520 2261 6263 5f30  .#include "abc_0
-00003fa0: 3030 5f77 6172 6e69 6e67 2e68 220d 0a    00_warning.h"..
+00001310: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2f 0d0a  *************/..
+00001320: 2f2f 2020 5072 652d 6361 636c 6375 6174  //  Pre-caclcuat
+00001330: 6564 2063 6f6e 7374 616e 7473 2066 6f72  ed constants for
+00001340: 2074 6865 2047 6175 7373 6169 6e20 7261   the Gaussain ra
+00001350: 646f 6d20 6765 6e65 7261 746f 7220 6261  dom generator ba
+00001360: 7365 6420 6f6e 200d 0a2f 2f20 2061 2068  sed on ..//  a h
+00001370: 7962 7269 6420 7265 6a65 6374 696f 6e20  ybrid rejection 
+00001380: 7361 6d70 6c69 6e67 206d 6574 686f 640d  sampling method.
+00001390: 0a2f 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ./**************
+000013a0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000013b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000013c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000013d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2f0d 0a47  ************/..G
+000013e0: 4155 5353 5f43 4f4e 5354 414e 5420 4741  AUSS_CONSTANT GA
+000013f0: 5553 530d 0a3d 207b 200d 0a09 0d0a 2e78  USS..= { ......x
+00001400: 203d 207b 2030 2c20 302e 3031 3935 3834   = { 0, 0.019584
+00001410: 3238 3532 3330 3132 372c 2030 2e30 3339  285230127, 0.039
+00001420: 3137 3630 3835 3530 3330 3938 2c20 302e  176085503098, 0.
+00001430: 3035 3837 3832 3933 3630 3638 3934 332c  058782936068943,
+00001440: 2030 2e30 3738 3431 3234 3132 3733 3331   0.0784124127331
+00001450: 3132 2c0d 0a30 2e30 3938 3037 3231 3532  12,..0.098072152
+00001460: 3438 3836 3631 2c20 302e 3131 3737 3639  488661, 0.117769
+00001470: 3837 3435 3739 3039 352c 2030 2e31 3337  874579095, 0.137
+00001480: 3531 3334 3032 3134 3433 3336 2c20 302e  513402144336, 0.
+00001490: 3135 3733 3130 3638 3436 3130 3137 312c  157310684610171,
+000014a0: 2030 2e31 3737 3136 3938 3230 3939 3137   0.1771698209917
+000014b0: 3430 2c20 302e 3139 3730 3939 3038 3432  40, 0.1970990842
+000014c0: 3934 3331 322c 0d0a 302e 3231 3731 3036  94312,..0.217106
+000014d0: 3934 3732 3130 3133 302c 2030 2e32 3337  947210130, 0.237
+000014e0: 3230 3231 3039 3332 3837 3838 2c20 302e  202109328788, 0.
+000014f0: 3235 3733 3933 3532 3631 3030 3933 382c  257393526100938,
+00001500: 2030 2e32 3737 3639 3034 3339 3832 3135   0.2776904398215
+00001510: 3737 2c20 302e 3239 3831 3032 3431 3239  77, 0.2981024129
+00001520: 3330 3438 372c 2030 2e33 3138 3633 3933  30487, 0.3186393
+00001530: 3633 3936 3433 3735 2c0d 0a30 2e33 3339  63964375,..0.339
+00001540: 3331 3136 3036 3533 3838 3137 2c20 302e  311606538817, 0.
+00001550: 3336 3031 3239 3839 3137 3839 3536 392c  360129891789569,
+00001560: 2030 2e33 3831 3130 3534 3534 3736 3335   0.3811054547635
+00001570: 3537 2c20 302e 3430 3232 3530 3036 3533  57, 0.4022500653
+00001580: 3231 3732 352c 2030 2e34 3233 3537 3630  21725, 0.4235760
+00001590: 3834 3230 3132 3030 2c20 302e 3434 3530  84201200, 0.4450
+000015a0: 3936 3532 3439 3835 3531 362c 0d0a 302e  96524985516,..0.
+000015b0: 3436 3638 3235 3132 3238 3532 3539 302c  466825122852590,
+000015c0: 2030 2e34 3838 3737 3634 3131 3131 3436   0.4887764111146
+000015d0: 3730 2c20 302e 3531 3039 3635 3830 3637  70, 0.5109658067
+000015e0: 3338 3234 372c 2030 2e35 3333 3430 3937  38247, 0.5334097
+000015f0: 3036 3234 3132 3831 2c20 302e 3535 3631  06241281, 0.5561
+00001600: 3235 3539 3336 3138 3639 312c 2030 2e35  25593618691, 0.5
+00001610: 3739 3133 3231 3632 3235 3535 3536 2c0d  79132162255556,.
+00001620: 0a30 2e36 3032 3434 3934 3533 3136 3434  .0.6024494531644
+00001630: 3234 2c20 302e 3632 3630 3939 3031 3233  24, 0.6260990123
+00001640: 3436 3432 312c 2030 2e36 3530 3130 3430  46421, 0.6501040
+00001650: 3730 3634 3739 3935 2c20 302e 3637 3434  70647995, 0.6744
+00001660: 3839 3735 3031 3936 3038 322c 2030 2e36  89750196082, 0.6
+00001670: 3939 3238 3333 3032 3338 3332 3230 2c20  99283302383220, 
+00001680: 302e 3732 3435 3134 3338 3334 3932 3336  0.72451438349236
+00001690: 362c 0d0a 302e 3735 3032 3135 3337 3534  6,..0.7502153754
+000016a0: 3637 3934 312c 2030 2e37 3736 3432 3137  67941, 0.7764217
+000016b0: 3631 3134 3739 3238 2c20 302e 3830 3331  61147928, 0.8031
+000016c0: 3732 3536 3535 3937 3931 382c 2030 2e38  72565597918, 0.8
+000016d0: 3330 3531 3038 3738 3230 3533 3939 2c20  30510878205399, 
+000016e0: 302e 3835 3834 3834 3437 3431 3431 3833  0.85848447414183
+000016f0: 322c 2030 2e38 3837 3134 3635 3539 3031  2, 0.88714655901
+00001700: 3838 3736 2c0d 0a30 2e39 3136 3535 3636  8876,..0.9165566
+00001710: 3637 3533 3331 3133 2c20 302e 3934 3637  67533113, 0.9467
+00001720: 3831 3735 3633 3031 3034 362c 2030 2e39  81756301046, 0.9
+00001730: 3737 3839 3735 3433 3934 3035 3432 2c20  77897543940542, 
+00001740: 312e 3030 3939 3930 3136 3932 3439 3538  1.00999016924958
+00001750: 322c 2031 2e30 3433 3135 3832 3633 3331  2, 1.04315826331
+00001760: 3834 3534 2c20 312e 3037 3735 3135 3536  8454, 1.07751556
+00001770: 3730 3430 3238 302c 0d0a 312e 3131 3331  7040280,..1.1131
+00001780: 3934 3237 3731 3630 3932 392c 2031 2e31  94277160929, 1.1
+00001790: 3530 3334 3933 3830 3337 3630 3038 2c20  50349380376008, 
+000017a0: 312e 3138 3931 3634 3335 3031 3939 3333  1.18916435019933
+000017b0: 372c 2031 2e32 3239 3835 3837 3539 3231  7, 1.22985875921
+000017c0: 3635 3839 2c20 312e 3237 3236 3938 3634  6589, 1.27269864
+000017d0: 3131 3930 3533 362c 2031 2e33 3138 3031  1190536, 1.31801
+000017e0: 3038 3937 3330 3335 3337 2c0d 0a31 2e33  0897303537,..1.3
+000017f0: 3636 3230 3338 3136 3337 3230 3938 2c20  66203816372098, 
+00001800: 312e 3431 3737 3937 3133 3739 3936 3236  1.41779713799626
+00001810: 382c 2031 2e34 3733 3436 3735 3737 3934  8, 1.47346757794
+00001820: 3731 3031 2c20 312e 3533 3431 3230 3534  7101, 1.53412054
+00001830: 3433 3532 3534 372c 2031 2e36 3031 3030  4352547, 1.60100
+00001840: 3836 3634 3838 3630 3736 2c20 312e 3637  8664886076, 1.67
+00001850: 3539 3339 3732 3237 3733 3434 342c 0d0a  5939722773444,..
+00001860: 312e 3736 3136 3730 3431 3033 3633 3036  1.76167041036306
+00001870: 372c 2031 2e38 3632 3733 3138 3637 3432  7, 1.86273186742
+00001880: 3136 3532 2c20 312e 3938 3734 3237 3838  1652, 1.98742788
+00001890: 3539 3239 3839 362c 2032 2e31 3533 3837  5929896, 2.15387
+000018a0: 3436 3934 3036 3134 3536 2c20 322e 3431  4694061456, 2.41
+000018b0: 3735 3539 3031 3632 3336 3530 207d 2c0d  755901623650 },.
+000018c0: 0a0d 0a2f 2f79 5b69 2b31 5d2f 795b 695d  ...//y[i+1]/y[i]
+000018d0: 2a32 5e32 340d 0a2e 7952 6174 696f 203d  *2^24...yRatio =
+000018e0: 207b 2031 3637 3733 3939 392c 2031 3637   { 16773999, 167
+000018f0: 3637 3536 322c 2031 3637 3631 3131 322c  67562, 16761112,
+00001900: 2031 3637 3534 3634 302c 2031 3637 3438   16754640, 16748
+00001910: 3133 362c 2031 3637 3431 3538 392c 2031  136, 16741589, 1
+00001920: 3637 3334 3938 392c 2031 3637 3238 3332  6734989, 1672832
+00001930: 352c 2031 3637 3231 3538 372c 2031 3637  5, 16721587, 167
+00001940: 3134 3736 332c 0d0a 3136 3730 3738 3430  14763,..16707840
+00001950: 2c20 3136 3730 3038 3037 2c20 3136 3639  , 16700807, 1669
+00001960: 3336 3531 2c20 3136 3638 3633 3538 2c20  3651, 16686358, 
+00001970: 3136 3637 3839 3133 2c20 3136 3637 3133  16678913, 166713
+00001980: 3032 2c20 3136 3636 3335 3037 2c20 3136  02, 16663507, 16
+00001990: 3635 3535 3132 2c20 3136 3634 3732 3937  655512, 16647297
+000019a0: 2c20 3136 3633 3838 3433 2c20 3136 3633  , 16638843, 1663
+000019b0: 3031 3238 2c20 3136 3632 3131 3238 2c0d  0128, 16621128,.
+000019c0: 0a31 3636 3131 3831 382c 2031 3636 3032  .16611818, 16602
+000019d0: 3137 302c 2031 3635 3932 3135 342c 2031  170, 16592154, 1
+000019e0: 3635 3831 3733 362c 2031 3635 3730 3837  6581736, 1657087
+000019f0: 392c 3136 3535 3935 3434 2c20 3136 3534  9,16559544, 1654
+00001a00: 3736 3834 2c20 3136 3533 3532 3530 2c20  7684, 16535250, 
+00001a10: 3136 3532 3231 3836 2c20 3136 3530 3834  16522186, 165084
+00001a20: 3331 2c20 3136 3439 3339 3133 2c20 3136  31, 16493913, 16
+00001a30: 3437 3835 3534 2c0d 0a31 3634 3632 3236  478554,..1646226
+00001a40: 352c 2031 3634 3434 3934 322c 2031 3634  5, 16444942, 164
+00001a50: 3236 3437 302c 2031 3634 3036 3731 352c  26470, 16406715,
+00001a60: 2031 3633 3835 3532 322c 2031 3633 3632   16385522, 16362
+00001a70: 3731 322c 2031 3633 3338 3037 342c 3136  712, 16338074,16
+00001a80: 3331 3133 3633 2c20 3136 3238 3232 3837  311363, 16282287
+00001a90: 2c20 3136 3235 3034 3937 2c20 3136 3231  , 16250497, 1621
+00001aa0: 3535 3736 2c20 3136 3137 3730 3136 2c0d  5576, 16177016,.
+00001ab0: 0a31 3631 3334 3139 352c 2031 3630 3836  .16134195, 16086
+00001ac0: 3334 332c 2031 3630 3332 3439 372c 2031  343, 16032497, 1
+00001ad0: 3539 3731 3432 392c 2031 3539 3031 3535  5971429, 1590155
+00001ae0: 392c 2031 3538 3230 3831 332c 2031 3537  9, 15820813, 157
+00001af0: 3236 3431 342c 2031 3536 3134 3536 312c  26414, 15614561,
+00001b00: 2031 3534 3739 3930 362c 3135 3331 3436   15479906,153146
+00001b10: 3836 2c20 3135 3130 3731 3833 2c20 3134  86, 15107183, 14
+00001b20: 3833 3838 3536 2c0d 0a31 3434 3738 3533  838856,..1447853
+00001b30: 382c 2031 3339 3639 3532 342c 2031 3331  8, 13969524, 131
+00001b40: 3936 3736 382c 2031 3138 3836 3038 362c  96768, 11886086,
+00001b50: 2039 3138 3236 3334 207d 2c0d 0a0d 0a2f   9182634 },..../
+00001b60: 2f31 2f79 5b69 5d2a 325e 3234 0d0a 2f2a  /1/y[i]*2^24../*
+00001b70: 0d0a 2e79 496e 7665 7273 6520 3d20 7b20  ...yInverse = { 
+00001b80: 302e 3136 3737 3732 3136 3030 3030 3030  0.16777216000000
+00001b90: 3065 382c 2030 2e31 3637 3830 3433 3337  0e8, 0.167804337
+00001ba0: 3130 3730 3239 6538 2c20 302e 3136 3739  107029e8, 0.1679
+00001bb0: 3030 3935 3438 3837 3339 3665 382c 2030  00954887396e8, 0
+00001bc0: 2e31 3638 3036 3232 3733 3332 3137 3932  .168062273321792
+00001bd0: 6538 2c20 302e 3136 3832 3838 3732 3737  e8, 0.1682887277
+00001be0: 3238 3834 3065 382c 0d0a 302e 3136 3835  28840e8,..0.1685
+00001bf0: 3830 3933 3138 3139 3432 3265 382c 2030  80931819422e8, 0
+00001c00: 2e31 3638 3933 3936 3832 3032 3935 3930  .168939682029590
+00001c10: 6538 2c20 302e 3136 3933 3635 3936 3331  e8, 0.1693659631
+00001c20: 3930 3338 3965 382c 2030 2e31 3639 3836  90389e8, 0.16986
+00001c30: 3039 3535 3631 3137 3533 6538 2c30 2e31  0955611753e8,0.1
+00001c40: 3730 3432 3630 3433 3637 3831 3831 6538  70426043678181e8
+00001c50: 2c20 302e 3137 3130 3632 3832 3630 3736  , 0.171062826076
+00001c60: 3633 3665 382c 0d0a 302e 3137 3137 3733  636e8,..0.171773
+00001c70: 3132 3738 3032 3636 3065 382c 2030 2e31  127802660e8, 0.1
+00001c80: 3732 3535 3930 3134 3131 3936 3633 6538  72559014119663e8
+00001c90: 2c20 302e 3137 3334 3232 3830 3636 3739  , 0.173422806679
+00001ca0: 3532 3865 382c 2030 2e31 3734 3336 3731  528e8, 0.1743671
+00001cb0: 3032 3035 3130 3339 6538 2c20 302e 3137  02051039e8, 0.17
+00001cc0: 3533 3934 3739 3239 3437 3239 3965 382c  5394792947299e8,
+00001cd0: 2030 2e31 3736 3530 3930 3932 3439 3535   0.1765090924955
+00001ce0: 3939 6538 2c0d 0a30 2e31 3737 3731 3335  99e8,..0.1777135
+00001cf0: 3631 3935 3438 3933 6538 2c20 302e 3137  61954893e8, 0.17
+00001d00: 3930 3132 3134 3233 3539 3132 3865 382c  9012142359128e8,
+00001d10: 302e 3138 3034 3039 3139 3036 3531 3730  0.18040919065170
+00001d20: 3865 382c 2030 2e31 3831 3930 3935 3230  8e8, 0.181909520
+00001d30: 3938 3036 3636 6538 2c20 302e 3138 3335  980666e8, 0.1835
+00001d40: 3138 3435 3139 3439 3434 3765 382c 2030  18451949447e8, 0
+00001d50: 2e31 3835 3234 3138 3630 3736 3937 3833  .185241860769783
+00001d60: 6538 2c0d 0a30 2e31 3837 3038 3632 3435  e8,..0.187086245
+00001d70: 3434 3731 3335 6538 2c20 302e 3138 3930  447135e8, 0.1890
+00001d80: 3538 3739 3633 3533 3737 3465 382c 2030  58796353774e8, 0
+00001d90: 2e31 3931 3136 3734 3738 3831 3938 3938  .191167478819898
+00001da0: 6538 2c20 302e 3139 3334 3231 3132 3837  e8, 0.1934211287
+00001db0: 3132 3633 3765 382c 2030 2e31 3935 3832  12637e8, 0.19582
+00001dc0: 3935 3633 3339 3333 3038 6538 2c20 302e  9563393308e8, 0.
+00001dd0: 3139 3834 3033 3731 3039 3637 3234 3765  198403710967247e
+00001de0: 382c 0d0a 302e 3230 3131 3535 3736 3133  8,..0.2011557613
+00001df0: 3937 3031 3665 382c 2030 2e32 3034 3039  97016e8, 0.20409
+00001e00: 3933 3433 3837 3733 3634 6538 2c20 302e  9343877364e8, 0.
+00001e10: 3230 3732 3439 3733 3539 3230 3036 3365  207249735920063e
+00001e20: 382c 2030 2e32 3130 3632 3431 3130 3933  8, 0.21062411093
+00001e30: 3732 3432 6538 2c20 302e 3231 3432 3431  7242e8, 0.214241
+00001e40: 3833 3238 3335 3636 3565 382c 2030 2e32  832835665e8, 0.2
+00001e50: 3138 3132 3438 3038 3336 3735 3530 6538  18124808367550e8
+00001e60: 2c0d 0a30 2e32 3232 3239 3739 3130 3839  ,..0.22229791089
+00001e70: 3934 3532 6538 2c20 302e 3232 3637 3839  9452e8, 0.226789
+00001e80: 3439 3330 3939 3930 3565 382c 2030 2e32  493099905e8, 0.2
+00001e90: 3331 3633 3230 3131 3134 3634 3433 6538  31632011146443e8
+00001ea0: 2c20 302e 3233 3638 3632 3738 3938 3931  , 0.236862789891
+00001eb0: 3830 3465 382c 302e 3234 3235 3234 3936  804e8,0.24252496
+00001ec0: 3736 3933 3832 3965 382c 2030 2e32 3438  7693829e8, 0.248
+00001ed0: 3636 3836 3732 3330 3133 3036 6538 2c0d  668672301306e8,.
+00001ee0: 0a30 2e32 3535 3335 3234 3936 3736 3639  .0.2553524967669
+00001ef0: 3237 6538 2c20 302e 3236 3236 3435 3336  27e8, 0.26264536
+00001f00: 3930 3232 3438 3565 382c 2030 2e32 3730  9022485e8, 0.270
+00001f10: 3632 3839 3433 3832 3930 3438 6538 2c20  628943829048e8, 
+00001f20: 302e 3237 3934 3030 3639 3634 3433 3336  0.27940069644336
+00001f30: 3665 382c 2030 2e32 3839 3037 3739 3731  6e8, 0.289077971
+00001f40: 3539 3539 3130 6538 2c20 302e 3239 3938  595910e8, 0.2998
+00001f50: 3033 3335 3232 3034 3536 3965 382c 0d0a  03352204569e8,..
+00001f60: 302e 3331 3137 3531 3838 3038 3734 3535  0.31175188087455
+00001f70: 3265 382c 2030 2e33 3235 3134 3039 3239  2e8, 0.325140929
+00001f80: 3239 3331 3033 6538 2c30 2e33 3430 3234  293103e8,0.34024
+00001f90: 3339 3237 3535 3433 3838 6538 2c20 302e  3927554388e8, 0.
+00001fa0: 3335 3734 3039 3834 3633 3436 3233 3665  357409846346236e
+00001fb0: 382c 2030 2e33 3737 3039 3134 3730 3033  8, 0.37709147003
+00001fc0: 3732 3536 6538 2c20 302e 3339 3938 3837  7256e8, 0.399887
+00001fd0: 3438 3934 3532 3631 3265 382c 0d0a 302e  489452612e8,..0.
+00001fe0: 3432 3636 3037 3033 3734 3037 3830 3365  426607037407803e
+00001ff0: 382c 2030 2e34 3538 3337 3230 3638 3339  8, 0.45837206839
+00002000: 3531 3334 6538 2c20 302e 3439 3637 3836  5134e8, 0.496786
+00002010: 3433 3233 3138 3835 3565 382c 2030 2e35  432318855e8, 0.5
+00002020: 3434 3232 3838 3234 3030 3135 3436 6538  44228824001546e8
+00002030: 2c20 302e 3630 3433 3930 3934 3034 3638  , 0.604390940468
+00002040: 3530 3865 382c 2030 2e36 3833 3334 3038  508e8, 0.6833408
+00002050: 3932 3533 3736 3831 6538 2c0d 0a30 2e37  92537681e8,..0.7
+00002060: 3931 3833 3131 3538 3837 3031 3138 6538  91831158870118e8
+00002070: 2c20 302e 3935 3039 3738 3839 3833 3738  , 0.950978898378
+00002080: 3238 3065 382c 2031 2e32 3038 3939 3133  280e8, 1.2089913
+00002090: 3137 3838 3732 3936 6538 2c20 312e 3730  17887296e8, 1.70
+000020a0: 3634 3931 3830 3730 3830 3531 3120 7d2c  6491807080511 },
+000020b0: 0d0a 0d0a 202e 5041 5241 4d5f 5220 2020  .... .PARAM_R   
+000020c0: 2020 3d20 322e 3431 3735 3539 3031 3632    = 2.4175590162
+000020d0: 3336 3530 2c0d 0a20 2e49 4e56 5f50 4152  3650,.. .INV_PAR
+000020e0: 414d 5f52 203d 2030 2e34 3133 3634 3033  AM_R = 0.4136403
+000020f0: 3637 3532 3933 3637 0d0a 202a 2f0d 0a7d  67529367.. */..}
+00002100: 3b0d 0a0d 0a23 6465 6669 6e65 2049 4e56  ;....#define INV
+00002110: 5f32 7032 3420 2028 2846 3634 2931 2e2f  _2p24  ((F64)1./
+00002120: 2831 4c4c 3c3c 3234 2929 0d0a 2364 6566  (1LL<<24))..#def
+00002130: 696e 6520 494e 565f 3270 3235 2020 2828  ine INV_2p25  ((
+00002140: 4636 3429 312e 2f28 314c 4c3c 3c32 3529  F64)1./(1LL<<25)
+00002150: 290d 0a23 6465 6669 6e65 2049 4e56 5f32  )..#define INV_2
+00002160: 7033 3220 2028 2846 3634 2931 2e2f 2831  p32  ((F64)1./(1
+00002170: 4c4c 3c3c 3332 2929 0d0a 0d0a 0d0a 6578  LL<<32))......ex
+00002180: 7465 726e 2076 6f69 6420 696e 6974 5f67  tern void init_g
+00002190: 6175 7373 5f72 6e64 2876 6f69 6429 3b0d  auss_rnd(void);.
+000021a0: 0a76 6f69 6420 696e 6974 5f67 6175 7373  .void init_gauss
+000021b0: 5f72 6e64 2876 6f69 6429 207b 0d0a 0d0a  _rnd(void) {....
+000021c0: 0973 7461 7469 6320 4930 3820 6973 496e  .static I08 isIn
+000021d0: 6974 6961 6c69 7a65 6420 3d20 303b 0d0a  itialized = 0;..
+000021e0: 0969 6620 2869 7349 6e69 7469 616c 697a  .if (isInitializ
+000021f0: 6564 2920 7b0d 0a09 0972 6574 7572 6e3b  ed) {....return;
+00002200: 0d0a 097d 0d0a 0d0a 0966 6f72 2028 696e  ...}.....for (in
+00002210: 7420 6920 3d20 303b 2069 203c 2036 333b  t i = 0; i < 63;
+00002220: 2069 2b2b 2920 7b0d 0a09 0947 4155 5353   i++) {....GAUSS
+00002230: 2e79 5261 7469 6f5b 695d 203d 2065 7870  .yRatio[i] = exp
+00002240: 282d 302e 3520 2a20 2847 4155 5353 2e78  (-0.5 * (GAUSS.x
+00002250: 5b69 202b 2031 5d20 2a20 4741 5553 532e  [i + 1] * GAUSS.
+00002260: 785b 6920 2b20 315d 202d 2047 4155 5353  x[i + 1] - GAUSS
+00002270: 2e78 5b69 5d20 2a20 4741 5553 532e 785b  .x[i] * GAUSS.x[
+00002280: 695d 2929 3b0d 0a09 7d0d 0a0d 0a09 666f  i]));...}.....fo
+00002290: 7220 2869 6e74 2069 203d 2030 3b20 6920  r (int i = 0; i 
+000022a0: 3c20 3633 3b20 692b 2b29 207b 0d0a 0909  < 63; i++) {....
+000022b0: 6966 2028 4741 5553 532e 785b 6920 2b20  if (GAUSS.x[i + 
+000022c0: 315d 203e 3d20 312e 3029 207b 0d0a 0909  1] >= 1.0) {....
+000022d0: 0947 4155 5353 2e69 6e66 6c65 6374 696f  .GAUSS.inflectio
+000022e0: 6e49 6420 3d20 693b 0d0a 0909 0962 7265  nId = i;.....bre
+000022f0: 616b 3b0d 0a09 097d 0d0a 097d 0d0a 090d  ak;....}...}....
+00002300: 0a09 2f2f 2074 6869 7320 6973 2074 6865  ..// this is the
+00002310: 206f 7074 696d 616c 206c 616d 6461 206d   optimal lamda m
+00002320: 6178 696d 697a 696e 6720 7468 6520 6163  aximizing the ac
+00002330: 6365 7074 616e 6365 2072 6174 696f 2e0d  ceptance ratio..
+00002340: 0a09 4633 3220 6120 3d20 4741 5553 532e  ..F32 a = GAUSS.
+00002350: 785b 3633 5d3b 0d0a 0947 4155 5353 2e65  x[63];...GAUSS.e
+00002360: 7870 5f6c 616d 6461 203d 2028 6120 2b20  xp_lamda = (a + 
+00002370: 7371 7274 2861 202a 2061 202b 2034 2929  sqrt(a * a + 4))
+00002380: 202f 2032 3b0d 0a0d 0a09 4633 3250 5452   / 2;.....F32PTR
+00002390: 2078 2020 2020 3d20 4741 5553 532e 783b   x    = GAUSS.x;
+000023a0: 0d0a 0946 3332 2020 2020 6465 6c20 203d  ...F32    del  =
+000023b0: 2047 4155 5353 2e78 5b31 5d3b 0d0a 0949   GAUSS.x[1];...I
+000023c0: 3332 2020 2020 496d 6178 203d 2063 6569  32    Imax = cei
+000023d0: 6c28 4741 5553 532e 785b 3633 5d20 2f20  l(GAUSS.x[63] / 
+000023e0: 6465 6c29 3b20 0d0a 0d0a 092f 2f20 4755  del); .....// GU
+000023f0: 4153 532e 696e 6469 6365 7320 7361 7665  ASS.indices save
+00002400: 7320 7468 6520 6c65 6674 2d73 6964 6520  s the left-side 
+00002410: 6269 6e20 696e 6465 780d 0a09 666f 7220  bin index...for 
+00002420: 2869 6e74 2069 203d 2030 3b20 6920 3c20  (int i = 0; i < 
+00002430: 496d 6178 3b20 692b 2b29 207b 0d0a 0909  Imax; i++) {....
+00002440: 4633 3220 6c6f 7720 3d20 6920 2a20 6465  F32 low = i * de
+00002450: 6c3b 0d0a 0909 4633 3220 7570 2020 3d20  l;....F32 up  = 
+00002460: 2869 202b 2031 2920 2a20 6465 6c3b 0d0a  (i + 1) * del;..
+00002470: 0909 0d0a 0909 4741 5553 532e 696e 6469  ......GAUSS.indi
+00002480: 6365 735b 695d 203d 202d 3939 3939 3b0d  ces[i] = -9999;.
+00002490: 0a0d 0a09 0969 6e74 2062 696e 676f 203d  .....int bingo =
+000024a0: 2030 3b0d 0a09 0966 6f72 2028 696e 7420   0;....for (int 
+000024b0: 6b20 3d20 303b 206b 203c 2036 343b 206b  k = 0; k < 64; k
+000024c0: 2b2b 2920 7b0d 0a0d 0a09 0909 6966 2028  ++) {.......if (
+000024d0: 785b 6b5d 203e 3d20 6c6f 7720 2626 2078  x[k] >= low && x
+000024e0: 5b6b 5d20 3c3d 2075 7029 207b 0d0a 0909  [k] <= up) {....
+000024f0: 0909 6966 2028 785b 6b5d 203d 3d20 6c6f  ..if (x[k] == lo
+00002500: 7729 207b 0d0a 0909 0909 0947 4155 5353  w) {.......GAUSS
+00002510: 2e69 6e64 6963 6573 5b69 5d20 3d20 6b3b  .indices[i] = k;
+00002520: 0909 0909 090d 0a09 0909 097d 0965 6c73  ...........}.els
+00002530: 6520 7b0d 0a09 0909 0909 4741 5553 532e  e {.......GAUSS.
+00002540: 696e 6469 6365 735b 695d 203d 206b 202d  indices[i] = k -
+00002550: 2031 3b0d 0a09 0909 097d 090d 0a0d 0a09   1;......}......
+00002560: 0909 0962 696e 676f 203d 2031 3b0d 0a09  ...bingo = 1;...
+00002570: 0909 0962 7265 616b 3b09 090d 0a09 0909  ...break;.......
+00002580: 7d0d 0a0d 0a0d 0a09 0909 6966 2028 785b  }.........if (x[
+00002590: 6b5d 203c 3d20 6c6f 7720 2626 2075 7020  k] <= low && up 
+000025a0: 3c3d 2078 5b6b 202b 2031 5d29 207b 0d0a  <= x[k + 1]) {..
+000025b0: 0909 0909 4741 5553 532e 696e 6469 6365  ....GAUSS.indice
+000025c0: 735b 695d 203d 206b 3b0d 0a09 0909 0962  s[i] = k;......b
+000025d0: 696e 676f 203d 2031 3b0d 0a09 0909 0962  ingo = 1;......b
+000025e0: 7265 616b 3b0d 0a09 0909 7d0d 0a0d 0a09  reak;.....}.....
+000025f0: 097d 0d0a 090d 0a09 0961 7373 6572 7428  .}.......assert(
+00002600: 6269 6e67 6f29 3b0d 0a09 7d0d 0a0d 0a0d  bingo);...}.....
+00002610: 0a09 6973 496e 6974 6961 6c69 7a65 6420  ..isInitialized 
+00002620: 3d20 313b 0d0a 7d0d 0a0d 0a76 6f69 6420  = 1;..}....void 
+00002630: 7063 675f 6761 7573 7328 4633 3250 5452  pcg_gauss(F32PTR
+00002640: 2052 4e44 2c20 696e 7420 4e29 0d0a 7b0d   RND, int N)..{.
+00002650: 0a09 666f 7220 2869 6e74 2069 203d 2031  ..for (int i = 1
+00002660: 3b20 6920 3c3d 204e 3b20 692b 2b29 207b  ; i <= N; i++) {
+00002670: 0d0a 0d0a 0909 5533 3220 726e 645b 325d  ......U32 rnd[2]
+00002680: 3b0d 0a09 0970 6367 5f72 616e 646f 6d28  ;....pcg_random(
+00002690: 726e 642c 2032 293b 0d0a 0d0a 0909 5533  rnd, 2);......U3
+000026a0: 3220 2055 3234 5f33 3220 3d20 2872 6e64  2  U24_32 = (rnd
+000026b0: 5b30 5d20 3e3e 2037 2920 2a20 494e 565f  [0] >> 7) * INV_
+000026c0: 3270 3235 3b0d 0a09 0955 3332 2020 4269  2p25;....U32  Bi
+000026d0: 6e49 6478 2020 3d20 726e 645b 305d 2026  nIdx  = rnd[0] &
+000026e0: 2030 7833 663b 0d0a 0909 4933 3220 2073   0x3f;....I32  s
+000026f0: 6967 6e20 2020 203d 2072 6e64 5b30 5d20  ign    = rnd[0] 
+00002700: 2620 3078 3430 3b20 202f 2f55 3234 2026  & 0x40;  //U24 &
+00002710: 2030 7838 3009 090d 0a0d 0a09 0946 3332   0x80........F32
+00002720: 2078 3b20 0d0a 0909 6966 2028 4269 6e49   x; ....if (BinI
+00002730: 6478 203c 2036 3329 2009 7b0d 0a09 0909  dx < 63) .{.....
+00002740: 4633 3220 6465 6c74 6120 2020 3d20 4741  F32 delta   = GA
+00002750: 5553 532e 785b 4269 6e49 6478 202b 2031  USS.x[BinIdx + 1
+00002760: 5d20 2d20 4741 5553 532e 785b 4269 6e49  ] - GAUSS.x[BinI
+00002770: 6478 5d3b 0d0a 0909 0946 3332 2079 5261  dx];.....F32 yRa
+00002780: 7469 6f20 203d 2047 4155 5353 2e79 5261  tio  = GAUSS.yRa
+00002790: 7469 6f5b 4269 6e49 6478 5d20 3b0d 0a09  tio[BinIdx] ;...
+000027a0: 0909 7768 696c 6520 2831 2920 7b0d 0a20  ..while (1) {.. 
+000027b0: 0d0a 0909 0909 6966 2028 5532 345f 3332  ......if (U24_32
+000027c0: 203c 3d20 7952 6174 696f 2920 7b0d 0a09   <= yRatio) {...
+000027d0: 0909 0909 7820 3d20 4741 5553 532e 785b  ....x = GAUSS.x[
+000027e0: 4269 6e49 6478 5d20 2b20 6465 6c74 6120  BinIdx] + delta 
+000027f0: 2a20 5532 345f 3332 202f 2079 5261 7469  * U24_32 / yRati
+00002800: 6f3b 0d0a 0909 0909 0962 7265 616b 3b0d  o;.......break;.
+00002810: 0a09 0909 097d 0d0a 0d0a 0909 0909 4636  .....}........F6
+00002820: 3420 5531 2020 2020 3d20 726e 645b 315d  4 U1    = rnd[1]
+00002830: 202a 2049 4e56 5f32 7033 323b 0d0a 0909   * INV_2p32;....
+00002840: 0909 696e 7420 6368 6563 6b20 3d20 5532  ..int check = U2
+00002850: 345f 3332 203c 3d20 7952 6174 696f 202b  4_32 <= yRatio +
+00002860: 2028 312e 6620 2d20 7952 6174 696f 2920   (1.f - yRatio) 
+00002870: 2a20 5531 3b09 0d0a 0909 0909 7820 2020  * U1;.......x   
+00002880: 2020 2020 2020 3d20 4741 5553 532e 785b        = GAUSS.x[
+00002890: 4269 6e49 6478 2b31 5d20 2d20 2064 656c  BinIdx+1] -  del
+000028a0: 7461 202a 2055 313b 0d0a 0909 0920 0d0a  ta * U1;..... ..
+000028b0: 0909 0909 6966 2028 4269 6e49 6478 203c  ....if (BinIdx <
+000028c0: 2047 4155 5353 2e69 6e66 6c65 6374 696f   GAUSS.inflectio
+000028d0: 6e49 6420 2626 2063 6865 636b 2920 2020  nId && check)   
+000028e0: 2020 207b 2062 7265 616b 3b20 7d0d 0a09     { break; }...
+000028f0: 0909 0969 6620 2842 696e 4964 7820 3e20  ...if (BinIdx > 
+00002900: 4741 5553 532e 696e 666c 6563 7469 6f6e  GAUSS.inflection
+00002910: 4964 2026 2620 6368 6563 6b20 3d3d 2030  Id && check == 0
+00002920: 2920 7b20 676f 746f 2055 7064 6174 6553  ) { goto UpdateS
+00002930: 616d 706c 6572 4c61 6265 6c3b 207d 0d0a  amplerLabel; }..
+00002940: 0909 0909 6966 2028 206c 6f67 2855 3234  ....if ( log(U24
+00002950: 5f33 3229 203c 3d20 2d30 2e35 662a 2028  _32) <= -0.5f* (
+00002960: 7820 2a20 782d 2047 4155 5353 2e78 5b42  x * x- GAUSS.x[B
+00002970: 696e 4964 785d 2a20 4741 5553 532e 785b  inIdx]* GAUSS.x[
+00002980: 4269 6e49 6478 5d29 2020 2920 7b0d 0a09  BinIdx])  ) {...
+00002990: 0909 0909 6272 6561 6b3b 0d0a 0909 0909  ....break;......
+000029a0: 7d09 0909 090d 0a0d 0a09 0909 092f 2f20  }............// 
+000029b0: 4e65 6564 2061 7420 6c65 6173 7420 7477  Need at least tw
+000029c0: 6f20 7261 6e64 206e 756d 6265 7273 0d0a  o rand numbers..
+000029d0: 0909 0909 5570 6461 7465 5361 6d70 6c65  ....UpdateSample
+000029e0: 724c 6162 656c 3a0d 0a09 0909 0970 6367  rLabel:......pcg
+000029f0: 5f72 616e 646f 6d28 726e 642c 2032 293b  _random(rnd, 2);
+00002a00: 0d0a 0909 0909 5532 345f 3332 203d 2028  ......U24_32 = (
+00002a10: 4636 3429 726e 645b 305d 202a 2049 4e56  F64)rnd[0] * INV
+00002a20: 5f32 7033 323b 202f 2f33 322d 6269 7420  _2p32; //32-bit 
+00002a30: 7261 6e64 6f6d 206e 756d 6265 720d 0a09  random number...
+00002a40: 0909 7d0d 0a09 097d 2065 6c73 6509 7b0d  ..}....} else.{.
+00002a50: 0a09 0977 6869 6c65 2028 3129 207b 0d0a  ...while (1) {..
+00002a60: 0909 0909 4636 3420 5531 203d 2072 6e64  ....F64 U1 = rnd
+00002a70: 5b31 5d20 2a20 494e 565f 3270 3332 3b20  [1] * INV_2p32; 
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 2020 2f2f 2064 6976 6964 6565 6420 6279    // divideed by
+00002aa0: 2032 5e33 3209 0909 0d0a 0909 0909 7820   2^32.........x 
+00002ab0: 3d20 4741 5553 532e 785b 3633 5d20 2d20  = GAUSS.x[63] - 
+00002ac0: 6c6f 6728 5531 2920 2f20 4741 5553 532e  log(U1) / GAUSS.
+00002ad0: 6578 705f 6c61 6d64 613b 2020 2020 2020  exp_lamda;      
+00002ae0: 2020 2f2f 2078 2069 7320 696e 6620 6966    // x is inf if
+00002af0: 2055 313d 3d30 0d0a 0909 0909 2f2f 6966   U1==0......//if
+00002b00: 2028 6578 7066 282d 4741 5553 532e 5041   (expf(-GAUSS.PA
+00002b10: 5241 4d5f 5220 2a20 2878 202d 2030 2e35  RAM_R * (x - 0.5
+00002b20: 6620 2a20 4741 5553 532e 5041 5241 4d5f  f * GAUSS.PARAM_
+00002b30: 5229 2920 2a20 5532 2020 3c20 6578 7066  R)) * U2  < expf
+00002b40: 282d 302e 3566 202a 2078 202a 2078 2929  (-0.5f * x * x))
+00002b50: 0d0a 0909 0909 6966 2028 6c6f 6728 5532  ......if (log(U2
+00002b60: 345f 3332 2920 3c20 2d30 2e35 6620 2a20  4_32) < -0.5f * 
+00002b70: 2828 7820 2d20 4741 5553 532e 6578 705f  ((x - GAUSS.exp_
+00002b80: 6c61 6d64 6129 202a 2028 7820 2d20 4741  lamda) * (x - GA
+00002b90: 5553 532e 6578 705f 6c61 6d64 6129 2929  USS.exp_lamda)))
+00002ba0: 0d0a 0909 0909 0962 7265 616b 3b0d 0a0d  .......break;...
+00002bb0: 0a09 0909 092f 2f20 4e65 6564 2061 7420  .....// Need at 
+00002bc0: 6c65 6173 7420 7477 6f20 7261 6e64 206e  least two rand n
+00002bd0: 756d 6265 7273 0d0a 0909 0909 7063 675f  umbers......pcg_
+00002be0: 7261 6e64 6f6d 2872 6e64 2c20 3229 3b0d  random(rnd, 2);.
+00002bf0: 0a09 0909 0955 3234 5f33 3220 3d20 726e  .....U24_32 = rn
+00002c00: 645b 305d 202a 2049 4e56 5f32 7033 323b  d[0] * INV_2p32;
+00002c10: 202f 2f64 6976 6964 6565 6420 6279 2032   //divideed by 2
+00002c20: 5e33 320d 0a09 0909 7d0d 0a09 097d 0d0a  ^32.....}....}..
+00002c30: 0d0a 0909 2a52 4e44 2b2b 203d 2073 6967  ....*RND++ = sig
+00002c40: 6e3f 2078 3a2d 783b 0d0a 097d 2f2f 436f  n? x:-x;...}//Co
+00002c50: 6d70 6c65 7469 6f6e 206f 6620 7468 6520  mpletion of the 
+00002c60: 466f 7220 6c6f 6f70 0d0a 7d0d 0a20 0d0a  For loop..}.. ..
+00002c70: 766f 6964 2070 6367 5f67 616d 6d61 2846  void pcg_gamma(F
+00002c80: 3332 5054 5220 726e 642c 2046 3332 2061  32PTR rnd, F32 a
+00002c90: 2c20 696e 7420 4e29 0d0a 7b0d 0a09 2f2a  , int N)..{.../*
+00002ca0: 0d0a 0925 2054 6869 7320 6675 6e63 7469  ...% This functi
+00002cb0: 6f6e 2069 7320 7573 6564 2074 6f20 6472  on is used to dr
+00002cc0: 6177 2067 616d 6d61 2072 616e 646f 6d20  aw gamma random 
+00002cd0: 7661 7269 6162 6c65 732e 0d0a 0925 2049  variables....% I
+00002ce0: 2063 616e 2774 2072 656d 656d 6265 7220   can't remember 
+00002cf0: 7768 6f20 4920 6e69 636b 6564 2074 6869  who I nicked thi
+00002d00: 7320 6f66 663f 3f3f 3f0d 0a09 2520 6966  s off????...% if
+00002d10: 2079 6f75 206c 6574 206d 6520 6b6e 6f77   you let me know
+00002d20: 2074 6865 6e20 4927 6c6c 2063 7265 6469   then I'll credi
+00002d30: 7420 7468 656d 2c20 706c 6561 7365 2065  t them, please e
+00002d40: 6d61 696c 206d 652e 0d0a 0925 0d0a 0925  mail me....%...%
+00002d50: 2049 7420 7761 7320 6164 6461 7074 6564   It was addapted
+00002d60: 2066 726f 6d2e 2e2e 2e2e 2e2e 2e0d 0a09   from...........
+00002d70: 250d 0a09 2520 5241 4e44 4741 4d4d 2047  %...% RANDGAMM G
+00002d80: 656e 6572 6174 6573 204e 2067 616d 6d61  enerates N gamma
+00002d90: 2072 616e 646f 6d20 6465 7669 6174 6573   random deviates
+00002da0: 2e0d 0a09 2520 2020 2020 5241 4e44 4741  ....%     RANDGA
+00002db0: 4d4d 2841 2c20 4e29 2069 7320 6120 7261  MM(A, N) is a ra
+00002dc0: 6e64 6f6d 2064 6576 6961 7465 2066 726f  ndom deviate fro
+00002dd0: 6d20 7468 6520 7374 616e 6461 7264 2067  m the standard g
+00002de0: 616d 6d61 0d0a 0925 2020 2020 2064 6973  amma...%     dis
+00002df0: 7472 6962 7574 696f 6e20 7769 7468 2073  tribution with s
+00002e00: 6861 7065 2070 6172 616d 6574 6572 2041  hape parameter A
+00002e10: 2e0d 0a09 250d 0a09 2520 2020 2020 422a  ....%...%     B*
+00002e20: 5241 4e44 4741 4d4d 2841 2c20 4e29 2069  RANDGAMM(A, N) i
+00002e30: 7320 6120 7261 6e64 6f6d 2064 6576 6961  s a random devia
+00002e40: 7465 2066 726f 6d20 7468 6520 6761 6d6d  te from the gamm
+00002e50: 6120 6469 7374 7269 6275 7469 6f6e 0d0a  a distribution..
+00002e60: 0925 2020 2020 2077 6974 6820 7368 6170  .%     with shap
+00002e70: 6520 7061 7261 6d65 7465 7220 4120 616e  e parameter A an
+00002e80: 6420 7363 616c 6520 7061 7261 6d65 7465  d scale paramete
+00002e90: 7220 422e 5468 6520 6469 7374 7269 6275  r B.The distribu
+00002ea0: 7469 6f6e 0d0a 0925 2020 2020 2074 6865  tion...%     the
+00002eb0: 6e20 6861 7320 6d65 616e 2041 2a42 2061  n has mean A*B a
+00002ec0: 6e64 2076 6172 6961 6e63 6520 412a 425e  nd variance A*B^
+00002ed0: 322e 0d0a 0925 0d0a 0925 2020 2020 2053  2....%...%     S
+00002ee0: 6565 2052 414e 442e 0d0a 0925 2047 4b53  ee RAND....% GKS
+00002ef0: 2033 3120 4a75 6c79 2039 330d 0a09 2520   31 July 93...% 
+00002f00: 416c 676f 7269 7468 6d20 666f 7220 4120  Algorithm for A 
+00002f10: 3e3d 2031 2069 7320 4265 7374 2773 2072  >= 1 is Best's r
+00002f20: 656a 6563 7469 6f6e 2061 6c67 6f72 6974  ejection algorit
+00002f30: 686d 2058 470d 0a09 2520 4164 6170 7465  hm XG...% Adapte
+00002f40: 6420 6672 6f6d 204c 2e44 6576 726f 7965  d from L.Devroye
+00002f50: 2c20 224e 6f6e 2d75 6e69 666f 726d 2072  , "Non-uniform r
+00002f60: 616e 646f 6d20 7661 7269 6174 650d 0a09  andom variate...
+00002f70: 2520 6765 6e65 7261 7469 6f6e 222c 2053  % generation", S
+00002f80: 7072 696e 6765 722d 5665 726c 6167 2c20  pringer-Verlag, 
+00002f90: 4e65 7720 596f 726b 2c20 3139 3836 2c20  New York, 1986, 
+00002fa0: 702e 2034 3130 2e0d 0a09 2520 416c 676f  p. 410....% Algo
+00002fb0: 7269 7468 6d20 666f 7220 4120 3c20 3120  rithm for A < 1 
+00002fc0: 6973 2072 656a 6563 7469 6f6e 2061 6c67  is rejection alg
+00002fd0: 6f72 6974 686d 2047 5320 6672 6f6d 0d0a  orithm GS from..
+00002fe0: 0925 2041 6872 656e 732c 204a 2e48 2e61  .% Ahrens, J.H.a
+00002ff0: 6e64 2044 6965 7465 722c 2055 2e43 6f6d  nd Dieter, U.Com
+00003000: 7075 7465 7220 6d65 7468 6f64 7320 666f  puter methods fo
+00003010: 7220 7361 6d70 6c69 6e67 0d0a 0925 2066  r sampling...% f
+00003020: 726f 6d20 6761 6d6d 612c 2062 6574 612c  rom gamma, beta,
+00003030: 2050 6f69 7373 6f6e 2061 6e64 2062 696e   Poisson and bin
+00003040: 6f6d 6961 6c20 6469 7374 7269 6275 7469  omial distributi
+00003050: 6f6e 732e 0d0a 0925 2043 6f6d 7075 7469  ons....% Computi
+00003060: 6e67 2c20 3132 2028 3139 3734 292c 2032  ng, 12 (1974), 2
+00003070: 3233 202d 2032 3436 2e20 2041 6461 7074  23 - 246.  Adapt
+00003080: 6564 2066 726f 6d20 4e65 746c 6962 0d0a  ed from Netlib..
+00003090: 0925 2046 6f72 7472 616e 2072 6f75 7469  .% Fortran routi
+000030a0: 6e65 2e0d 0a0d 0a09 6761 6d6d 615f 7374  ne......gamma_st
+000030b0: 6f72 6520 3d20 7a65 726f 7328 4e2c 204d  ore = zeros(N, M
+000030c0: 293b 0d0a 092a 2f0d 0a09 4633 3220 494e  );...*/...F32 IN
+000030d0: 565f 4d41 5820 3d20 322e 3332 3833 3036  V_MAX = 2.328306
+000030e0: 3433 3635 3338 3639 3665 2d31 3066 3b0d  436538696e-10f;.
+000030f0: 0a09 6966 2028 6120 3e3d 2031 290d 0a09  ..if (a >= 1)...
+00003100: 7b0d 0a09 0946 3332 2062 203d 2061 202d  {....F32 b = a -
+00003110: 2031 2e30 663b 0d0a 0909 4633 3220 6320   1.0f;....F32 c 
+00003120: 3d20 6120 2b20 6120 2b20 6120 2d20 302e  = a + a + a - 0.
+00003130: 3735 663b 0d0a 0d0a 0909 666f 7220 2869  75f;......for (i
+00003140: 6e74 2069 203d 2030 3b20 6920 3c20 4e3b  nt i = 0; i < N;
+00003150: 2069 2b2b 290d 0a09 097b 0d0a 0909 0946   i++)....{.....F
+00003160: 3332 2067 616d 3b0d 0a09 0909 7768 696c  32 gam;.....whil
+00003170: 6520 2831 290d 0a09 0909 7b0d 0a0d 0a09  e (1).....{.....
+00003180: 0909 090d 0a2f 2f23 6966 2064 6566 696e  .....//#if defin
+00003190: 6564 285f 5f47 4e55 435f 5f29 207c 7c20  ed(__GNUC__) || 
+000031a0: 6465 6669 6e65 6428 5f5f 434c 414e 475f  defined(__CLANG_
+000031b0: 5f29 200d 0a2f 2f09 4449 5341 424c 455f  _) ..//.DISABLE_
+000031c0: 5741 524e 494e 4728 7374 7269 6374 2d61  WARNING(strict-a
+000031d0: 6c69 6173 696e 672c 2073 7472 6963 742d  liasing, strict-
+000031e0: 616c 6961 7369 6e67 2c20 4e4f 545f 5553  aliasing, NOT_US
+000031f0: 4544 290d 0a2f 2f23 656e 6469 660d 0a09  ED)..//#endif...
+00003200: 0909 0946 3332 2075 5b32 5d3b 0d0a 0909  ...F32 u[2];....
+00003210: 0909 7063 675f 7261 6e64 6f6d 2828 5533  ..pcg_random((U3
+00003220: 3250 5452 2975 2c20 3229 3b0d 0a09 0909  2PTR)u, 2);.....
+00003230: 0975 5b30 5d20 3d20 2846 3332 2928 2a28  .u[0] = (F32)(*(
+00003240: 5533 3250 5452 2926 755b 305d 2920 2a20  U32PTR)&u[0]) * 
+00003250: 494e 565f 4d41 583b 0d0a 0909 0909 755b  INV_MAX;......u[
+00003260: 315d 203d 2028 4633 3229 282a 2855 3332  1] = (F32)(*(U32
+00003270: 5054 5229 2675 5b31 5d29 202a 2049 4e56  PTR)&u[1]) * INV
+00003280: 5f4d 4158 3b0d 0a0d 0a09 0909 0946 3332  _MAX;........F32
+00003290: 2077 203d 2075 5b30 5d20 2a20 2831 202d   w = u[0] * (1 -
+000032a0: 2075 5b30 5d29 3b0d 0a09 0909 0946 3332   u[0]);......F32
+000032b0: 2079 203d 2073 7172 7466 2863 202f 2077   y = sqrtf(c / w
+000032c0: 2920 2a20 2875 5b30 5d20 2d20 302e 3566  ) * (u[0] - 0.5f
+000032d0: 293b 0d0a 0909 0909 6761 6d20 3d20 6220  );......gam = b 
+000032e0: 2b20 793b 0d0a 0909 0909 6966 2028 6761  + y;......if (ga
+000032f0: 6d20 3e3d 2030 290d 0a09 0909 097b 0d0a  m >= 0)......{..
+00003300: 0909 0909 0946 3332 207a 203d 2036 342e  .....F32 z = 64.
+00003310: 3066 202a 2028 772a 772a 7729 202a 2028  0f * (w*w*w) * (
+00003320: 755b 315d 202a 2075 5b31 5d29 3b0d 0a09  u[1] * u[1]);...
+00003330: 0909 0909 6966 2028 7a20 3c3d 2028 3120  ....if (z <= (1 
+00003340: 2d20 3220 2a20 2879 2a79 2920 2f20 6761  - 2 * (y*y) / ga
+00003350: 6d29 290d 0a09 0909 0909 0962 7265 616b  m))........break
+00003360: 3b0d 0a0d 0a09 0909 0909 4633 3220 6c6f  ;.........F32 lo
+00003370: 675a 203d 206c 6f67 6628 7a29 3b0d 0a09  gZ = logf(z);...
+00003380: 0909 0909 6966 2028 6220 3d3d 2030 2909  ....if (b == 0).
+00003390: 0909 0909 7b0d 0a09 0909 0909 0969 6620  ....{........if 
+000033a0: 286c 6f67 5a20 3c3d 202d 3220 2a20 7929  (logZ <= -2 * y)
+000033b0: 2062 7265 616b 3b0d 0a09 0909 0909 7d09   break;.......}.
+000033c0: 0965 6c73 6509 0909 0909 7b0d 0a09 0909  .else.....{.....
+000033d0: 0909 0969 6620 286c 6f67 5a20 3c3d 2032  ...if (logZ <= 2
+000033e0: 202a 2028 6220 2a20 6c6f 6766 2867 616d   * (b * logf(gam
+000033f0: 202f 2062 2920 2d20 7929 2920 6272 6561   / b) - y)) brea
+00003400: 6b3b 0d0a 0909 0909 097d 0d0a 0909 0909  k;.......}......
+00003410: 7d20 2f2f 434f 4445 5f45 4f46 206f 6620  } //CODE_EOF of 
+00003420: 2028 6761 6d20 3e3d 2030 290d 0a0d 0a09   (gam >= 0).....
+00003430: 0909 7d2f 2f43 4f44 455f 454f 4620 5748  ..}//CODE_EOF WH
+00003440: 494c 450d 0a09 0909 2a72 6e64 2b2b 203d  ILE.....*rnd++ =
+00003450: 2067 616d 3b0d 0a0d 0a09 097d 2f2f 434f   gam;......}//CO
+00003460: 4445 5f45 4f46 2046 4f52 0d0a 0909 7265  DE_EOF FOR....re
+00003470: 7475 726e 3b0d 0a09 7d0d 0a0d 0a09 6966  turn;...}.....if
+00003480: 2028 6120 3e20 3029 202f 2f20 303c 613c   (a > 0) // 0<a<
+00003490: 310d 0a09 7b0d 0a09 0946 3332 2062 203d  1...{....F32 b =
+000034a0: 2031 202b 202e 3336 3738 3739 3466 202a   1 + .3678794f *
+000034b0: 2061 3b0d 0a09 0966 6f72 2028 696e 7420   a;....for (int 
+000034c0: 6920 3d20 303b 2069 203c 204e 3b20 692b  i = 0; i < N; i+
+000034d0: 2b29 0d0a 0909 7b0d 0a09 0909 4633 3220  +)....{.....F32 
+000034e0: 6761 6d3b 0d0a 0909 0977 6869 6c65 2028  gam;.....while (
+000034f0: 3129 0d0a 0909 097b 0d0a 2f2f 2369 6620  1).....{..//#if 
+00003500: 6465 6669 6e65 6428 5f5f 474e 5543 5f5f  defined(__GNUC__
+00003510: 2920 7c7c 2064 6566 696e 6564 285f 5f43  ) || defined(__C
+00003520: 4c41 4e47 5f5f 2920 0d0a 2f2f 0944 4953  LANG__) ..//.DIS
+00003530: 4142 4c45 5f57 4152 4e49 4e47 2873 7472  ABLE_WARNING(str
+00003540: 6963 742d 616c 6961 7369 6e67 2c20 7374  ict-aliasing, st
+00003550: 7269 6374 2d61 6c69 6173 696e 672c 204e  rict-aliasing, N
+00003560: 4f54 5f55 5345 4429 0d0a 2f2f 2365 6e64  OT_USED)..//#end
+00003570: 6966 0d0a 0909 0909 4633 3220 755b 325d  if......F32 u[2]
+00003580: 3b0d 0a09 0909 0970 6367 5f72 616e 646f  ;......pcg_rando
+00003590: 6d28 2855 3332 5054 5229 752c 2032 293b  m((U32PTR)u, 2);
+000035a0: 0d0a 0909 0909 755b 305d 203d 2028 4633  ......u[0] = (F3
+000035b0: 3229 282a 2855 3332 5054 5229 2675 5b30  2)(*(U32PTR)&u[0
+000035c0: 5d29 202a 2049 4e56 5f4d 4158 3b0d 0a09  ]) * INV_MAX;...
+000035d0: 0909 0975 5b31 5d20 3d20 2846 3332 2928  ...u[1] = (F32)(
+000035e0: 2a28 5533 3250 5452 2926 755b 315d 2920  *(U32PTR)&u[1]) 
+000035f0: 2a20 494e 565f 4d41 583b 0d0a 2f2f 2369  * INV_MAX;..//#i
+00003600: 6620 6465 6669 6e65 6428 5f5f 474e 5543  f defined(__GNUC
+00003610: 5f5f 2920 7c7c 2064 6566 696e 6564 285f  __) || defined(_
+00003620: 5f43 4c41 4e47 5f5f 2920 0d0a 2f2f 0945  _CLANG__) ..//.E
+00003630: 4e41 424c 455f 5741 524e 494e 4728 7374  NABLE_WARNING(st
+00003640: 7269 6374 2d61 6c69 6173 696e 672c 2073  rict-aliasing, s
+00003650: 7472 6963 742d 616c 6961 7369 6e67 2c20  trict-aliasing, 
+00003660: 4e4f 545f 5553 4544 290d 0a2f 2f23 656e  NOT_USED)..//#en
+00003670: 6469 660d 0a09 0909 0946 3332 2063 203d  dif......F32 c =
+00003680: 2062 202a 2075 5b30 5d3b 0d0a 0909 0909   b * u[0];......
+00003690: 6966 2028 6320 3c20 3129 0d0a 0909 0909  if (c < 1)......
+000036a0: 7b0d 0a09 0909 0909 6761 6d20 3d20 6578  {.......gam = ex
+000036b0: 7066 286c 6f67 6628 6329 202f 2061 293b  pf(logf(c) / a);
+000036c0: 0d0a 0909 0909 0969 6620 282d 6c6f 6766  .......if (-logf
+000036d0: 2831 202d 2075 5b31 5d29 203e 3d20 6761  (1 - u[1]) >= ga
+000036e0: 6d29 2062 7265 616b 3b0d 0a09 0909 097d  m) break;......}
+000036f0: 0d0a 0909 0909 656c 7365 0d0a 0909 0909  ......else......
+00003700: 7b0d 0a09 0909 0909 6761 6d20 3d20 2d6c  {.......gam = -l
+00003710: 6f67 6628 2862 202d 2063 2920 2f20 6129  ogf((b - c) / a)
+00003720: 3b0d 0a09 0909 0909 6966 2028 2d6c 6f67  ;.......if (-log
+00003730: 6628 3120 2d20 755b 315d 2920 3e3d 2028  f(1 - u[1]) >= (
+00003740: 3120 2d20 6129 202a 206c 6f67 6628 6761  1 - a) * logf(ga
+00003750: 6d29 290d 0a09 0909 0909 0962 7265 616b  m))........break
+00003760: 3b0d 0a09 0909 097d 0d0a 0909 097d 2f2f  ;......}.....}//
+00003770: 434f 4445 5f45 4f46 2057 4849 4c45 0d0a  CODE_EOF WHILE..
+00003780: 0909 092a 726e 642b 2b20 3d20 6761 6d3b  ...*rnd++ = gam;
+00003790: 0d0a 0909 7d2f 2f43 4f44 455f 454f 4620  ....}//CODE_EOF 
+000037a0: 464f 520d 0a09 0972 6574 7572 6e3b 0d0a  FOR....return;..
+000037b0: 097d 0d0a 0d0a 0d0a 0969 6620 2861 203c  .}.......if (a <
+000037c0: 2030 2e66 2920 097b 0d0a 0909 4633 3220   0.f) .{....F32 
+000037d0: 6e61 6e20 3d20 6765 744e 614e 2829 3b0d  nan = getNaN();.
+000037e0: 0a09 0966 6f72 2028 696e 7420 6920 3d20  ...for (int i = 
+000037f0: 303b 2069 203c 204e 3b20 692b 2b29 0909  0; i < N; i++)..
+00003800: 2a72 6e64 2b2b 203d 206e 616e 3b0d 0a09  *rnd++ = nan;...
+00003810: 0972 6574 7572 6e3b 0d0a 097d 0d0a 0d0a  .return;...}....
+00003820: 0d0a 0969 6620 2861 203d 3d20 302e 6629  ...if (a == 0.f)
+00003830: 097b 0d0a 0909 666f 7220 2869 6e74 2069  .{....for (int i
+00003840: 203d 2030 3b20 6920 3c20 4e3b 2069 2b2b   = 0; i < N; i++
+00003850: 2909 2a72 6e64 2b2b 203d 2030 2e66 3b0d  ).*rnd++ = 0.f;.
+00003860: 0a09 0972 6574 7572 6e3b 0d0a 097d 0d0a  ...return;...}..
+00003870: 0d0a 0d0a 7d0d 0a0d 0a0d 0a76 6f69 6420  ....}......void 
+00003880: 2070 6367 5f77 6973 6861 7274 5f75 6e69   pcg_wishart_uni
+00003890: 745f 6c6f 7774 7269 616e 676c 655f 6e6f  t_lowtriangle_no
+000038a0: 7a65 726f 6f75 7428 4633 3250 5452 2072  zeroout(F32PTR r
+000038b0: 6e64 2c20 4633 3250 5452 2074 6d70 2c20  nd, F32PTR tmp, 
+000038c0: 4933 3220 6d2c 2046 3332 2064 6620 290d  I32 m, F32 df ).
+000038d0: 0a7b 0d0a 0949 3332 204e 203d 2028 6d20  .{...I32 N = (m 
+000038e0: 2d20 3129 2a6d 202f 2032 3b0d 0a20 2020  - 1)*m / 2;..   
+000038f0: 2020 7063 675f 6761 7573 7328 746d 702c    pcg_gauss(tmp,
+00003900: 204e 293b 0d0a 0d0a 0946 3332 5054 5220   N);.....F32PTR 
+00003910: 7470 743b 0d0a 0974 7074 203d 2072 6e64  tpt;...tpt = rnd
+00003920: 202b 2031 3b0d 0a0d 0a09 666f 7220 2869   + 1;.....for (i
+00003930: 6e74 2069 203d 2031 3b20 693c 6d20 203b  nt i = 1; i<m  ;
+00003940: 2069 2b2b 290d 0a09 7b09 0909 0d0a 0909   i++)...{.......
+00003950: 4933 3220 206d 6f76 456c 656d 203d 206d  I32  movElem = m
+00003960: 202d 2069 3b0d 0a09 0966 6f72 2028 696e   - i;....for (in
+00003970: 7420 6a20 3d20 303b 206a 203c 206d 6f76  t j = 0; j < mov
+00003980: 456c 656d 3b20 6a2b 2b29 0d0a 0909 7b0d  Elem; j++)....{.
+00003990: 0a09 0909 2a74 7074 2b2b 203d 202a 746d  ....*tpt++ = *tm
+000039a0: 702b 2b3b 0d0a 0909 7d0d 0a09 0974 7074  p++;....}....tpt
+000039b0: 203d 2074 7074 202b 2069 2b31 3b0d 0a09   = tpt + i+1;...
+000039c0: 7d0d 0a09 0d0a 0974 6d70 203d 2072 6e64  }......tmp = rnd
+000039d0: 3b0d 0a09 666f 7220 2869 6e74 2069 203d  ;...for (int i =
+000039e0: 2031 3b20 6920 3c3d 6d3b 2069 2b2b 290d   1; i <=m; i++).
+000039f0: 0a09 7b0d 0a09 0970 6367 5f67 616d 6d61  ..{....pcg_gamma
+00003a00: 2874 6d70 2c20 2846 3332 2928 6466 2d69  (tmp, (F32)(df-i
+00003a10: 2b31 2e29 2f20 322e 662c 2031 293b 0d0a  +1.)/ 2.f, 1);..
+00003a20: 0909 2a74 6d70 203d 2073 7172 7466 2828  ..*tmp = sqrtf((
+00003a30: 2a74 6d70 2920 2a20 322e 6629 3b0d 0a09  *tmp) * 2.f);...
+00003a40: 0974 6d70 203d 2074 6d70 202b 2028 6d20  .tmp = tmp + (m 
+00003a50: 2b20 3129 3b0d 0a09 7d0d 0a0d 0a7d 0d0a  + 1);...}....}..
+00003a60: 0d0a 766f 6964 2070 6367 5f77 6973 6861  ..void pcg_wisha
+00003a70: 7274 5f75 6e69 745f 6c6f 7774 7269 616e  rt_unit_lowtrian
+00003a80: 676c 655f 6e6f 7a65 726f 6f75 745f 6e6f  gle_nozeroout_no
+00003a90: 746d 7028 4633 3250 5452 2077 6973 6872  tmp(F32PTR wishr
+00003aa0: 6e64 2c20 4933 3220 6d2c 2046 3332 2064  nd, I32 m, F32 d
+00003ab0: 6629 0d0a 7b0d 0a09 2f2f 2054 6869 7320  f)..{...// This 
+00003ac0: 6973 2061 6e20 696d 706c 6d65 6e74 6174  is an implmentat
+00003ad0: 696f 6e20 6f66 2074 6865 2042 6172 6c6c  ion of the Barll
+00003ae0: 6574 2061 6c67 6f72 7469 686d 0d0a 096d  et algortihm...m
+00003af0: 656d 7365 7428 7769 7368 726e 642c 2030  emset(wishrnd, 0
+00003b00: 2c20 7369 7a65 6f66 2846 3332 2920 2a20  , sizeof(F32) * 
+00003b10: 6d20 2a20 6d29 3b0d 0a0d 0a09 2f2f 2074  m * m);.....// t
+00003b20: 6865 206e 756d 6265 7220 6f66 2065 6c65  he number of ele
+00003b30: 6d6e 7473 2062 656c 6f77 2074 6865 2064  mnts below the d
+00003b40: 6961 676f 6e61 6c3a 2028 302b 2028 6d3d  iagonal: (0+ (m=
+00003b50: 3129 292a 6d2f 320d 0a09 4933 3220 2020  1))*m/2...I32   
+00003b60: 2020 6e75 6d47 6175 7373 526e 6420 3d20    numGaussRnd = 
+00003b70: 286d 202d 2031 2920 2a20 6d20 2f20 323b  (m - 1) * m / 2;
+00003b80: 0d0a 0946 3332 5054 5220 2067 6175 7373  ...F32PTR  gauss
+00003b90: 2020 2020 2020 203d 2077 6973 6872 6e64         = wishrnd
+00003ba0: 202b 206d 202a 206d 2020 2d20 6e75 6d47   + m * m  - numG
+00003bb0: 6175 7373 526e 643b 0d0a 0970 6367 5f67  aussRnd;...pcg_g
+00003bc0: 6175 7373 2867 6175 7373 2c20 6e75 6d47  auss(gauss, numG
+00003bd0: 6175 7373 526e 6429 3b0d 0a0d 0a09 666f  aussRnd);.....fo
+00003be0: 7220 2869 6e74 2063 6f6c 203d 2031 3b20  r (int col = 1; 
+00003bf0: 636f 6c20 3c20 6d3b 202b 2b63 6f6c 2920  col < m; ++col) 
+00003c00: 7b0d 0a09 0966 6f72 2028 696e 7420 726f  {....for (int ro
+00003c10: 7720 3d20 636f 6c20 2b20 313b 2072 6f77  w = col + 1; row
+00003c20: 203c 3d20 6d3b 2072 6f77 2b2b 2920 7b0d   <= m; row++) {.
+00003c30: 0a09 0909 7769 7368 726e 645b 726f 7720  ....wishrnd[row 
+00003c40: 2d20 315d 203d 202a 6761 7573 732b 2b3b  - 1] = *gauss++;
+00003c50: 0d0a 0909 7d0d 0a09 0977 6973 6872 6e64  ....}....wishrnd
+00003c60: 202b 3d20 6d3b 0d0a 097d 0d0a 0977 6973   += m;...}...wis
+00003c70: 6872 6e64 202d 3d20 286d 202d 2031 2920  hrnd -= (m - 1) 
+00003c80: 2a20 6d3b 2020 2f2f 676f 2062 6163 6b20  * m;  //go back 
+00003c90: 746f 2074 6865 2073 7461 7274 206f 6620  to the start of 
+00003ca0: 726e 640d 0a0d 0a20 2020 2f2f 2020 4669  rnd....   //  Fi
+00003cb0: 6c6c 2074 6865 2064 6961 676f 6e6c 2077  ll the diagonl w
+00003cc0: 6974 6820 6761 6d6d 6120 7261 6e64 6f6d  ith gamma random
+00003cd0: 2076 6172 6961 626c 6573 0d0a 0966 6f72   variables...for
+00003ce0: 2028 696e 7420 6920 3d20 313b 2069 203c   (int i = 1; i <
+00003cf0: 3d20 6d3b 2069 2b2b 2920 7b0d 0a09 0946  = m; i++) {....F
+00003d00: 3332 2063 6869 7371 6175 7265 3b0d 0a09  32 chisqaure;...
+00003d10: 0970 6367 5f67 616d 6d61 2826 6368 6973  .pcg_gamma(&chis
+00003d20: 7161 7572 652c 2028 4633 3229 2864 6620  qaure, (F32)(df 
+00003d30: 2d20 6920 2b20 3129 202f 2032 2e66 2c20  - i + 1) / 2.f, 
+00003d40: 3129 3b0d 0a09 092a 7769 7368 726e 6420  1);....*wishrnd 
+00003d50: 3d20 6368 6973 7161 7572 6520 3d20 7371  = chisqaure = sq
+00003d60: 7274 6628 6368 6973 7161 7572 6520 2a20  rtf(chisqaure * 
+00003d70: 322e 6629 3b0d 0a09 0977 6973 6872 6e64  2.f);....wishrnd
+00003d80: 202b 3d20 286d 202b 2031 293b 0d0a 097d   += (m + 1);...}
+00003d90: 0d0a 0d0a 7d0d 0a0d 0a20 0d0a 0d0a 200d  ....}.... .... .
+00003da0: 0a0d 0a76 6f69 6420 2070 6367 5f77 6973  ...void  pcg_wis
+00003db0: 6861 7274 5f75 6e69 745f 6c6f 7774 7269  hart_unit_lowtri
+00003dc0: 616e 676c 655f 7a65 726f 6f75 745f 6e6f  angle_zeroout_no
+00003dd0: 746d 7028 4633 3250 5452 2077 6973 6872  tmp(F32PTR wishr
+00003de0: 6e64 2c20 4933 3220 6d2c 2046 3332 2064  nd, I32 m, F32 d
+00003df0: 6629 0d0a 7b0d 0a09 2f2f 2054 6869 7320  f)..{...// This 
+00003e00: 6973 2061 6e20 696d 706c 6d65 6e74 6174  is an implmentat
+00003e10: 696f 6e20 6f66 2074 6865 2042 6172 6c6c  ion of the Barll
+00003e20: 6574 2061 6c67 6f72 7469 686d 0d0a 200d  et algortihm.. .
+00003e30: 0a09 2f2a 0d0a 092f 2f20 7468 6520 6e75  ../*...// the nu
+00003e40: 6d62 6572 206f 6620 656c 656d 6e74 7320  mber of elemnts 
+00003e50: 6265 6c6f 7720 7468 6520 6469 6167 6f6e  below the diagon
+00003e60: 616c 3a20 2830 2b20 286d 3d31 2929 2a6d  al: (0+ (m=1))*m
+00003e70: 2f32 0920 0d0a 0949 3332 2020 2020 206e  /2. ...I32     n
+00003e80: 756d 4761 7573 7352 6e64 203d 2028 6d20  umGaussRnd = (m 
+00003e90: 2d20 3129 202a 206d 202f 2032 3b0d 0a09  - 1) * m / 2;...
+00003ea0: 4633 3250 5452 2020 6761 7573 7320 3d20  F32PTR  gauss = 
+00003eb0: 2077 6973 6872 6e64 202b 206d 202a 206d   wishrnd + m * m
+00003ec0: 202d 206e 756d 4761 7573 7352 6e64 3b0d   - numGaussRnd;.
+00003ed0: 0a09 6c6f 6361 6c5f 7063 675f 6761 7573  ..local_pcg_gaus
+00003ee0: 7328 726e 672c 2067 6175 7373 202c 206e  s(rng, gauss , n
+00003ef0: 756d 4761 7573 7352 6e64 293b 0d0a 090d  umGaussRnd);....
+00003f00: 0a09 666f 7220 2869 6e74 2063 6f6c 203d  ..for (int col =
+00003f10: 2031 3b20 636f 6c20 3c20 6d3b 202b 2b63   1; col < m; ++c
+00003f20: 6f6c 2920 7b0d 0a09 0966 6f72 2028 696e  ol) {....for (in
+00003f30: 7420 726f 7720 3d20 636f 6c20 2b20 313b  t row = col + 1;
+00003f40: 2072 6f77 203c 3d20 6d3b 2072 6f77 2b2b   row <= m; row++
+00003f50: 2920 7b0d 0a09 0909 7769 7368 726e 645b  ) {.....wishrnd[
+00003f60: 726f 7720 2d20 315d 203d 202a 6761 7573  row - 1] = *gaus
+00003f70: 732b 2b3b 0d0a 0909 7d0d 0a09 0977 6973  s++;....}....wis
+00003f80: 6872 6e64 202b 3d20 6d3b 0d0a 097d 0d0a  hrnd += m;...}..
+00003f90: 0977 6973 6872 6e64 202d 3d20 286d 202d  .wishrnd -= (m -
+00003fa0: 2031 2920 2a20 6d3b 2020 2f2f 676f 2062   1) * m;  //go b
+00003fb0: 6163 6b20 746f 2074 6865 2073 7461 7274  ack to the start
+00003fc0: 206f 6620 726e 640d 0a09 202a 2f0d 0a0d   of rnd... */...
+00003fd0: 0a20 0d0a 092f 2f20 7468 6520 6e75 6d62  . ...// the numb
+00003fe0: 6572 206f 6620 656c 656d 6e74 7320 6265  er of elemnts be
+00003ff0: 6c6f 7720 7468 6520 6469 6167 6f6e 616c  low the diagonal
+00004000: 3a20 2830 2b20 286d 3d31 2929 2a6d 2f32  : (0+ (m=1))*m/2
+00004010: 090d 0a09 4933 3220 2020 2020 6e75 6d47  ....I32     numG
+00004020: 6175 7373 526e 6420 3d20 286d 202d 2031  aussRnd = (m - 1
+00004030: 2920 2a20 6d20 2f20 323b 0d0a 0946 3332  ) * m / 2;...F32
+00004040: 5054 5220 2067 6175 7373 2020 2020 2020  PTR  gauss      
+00004050: 203d 2020 7769 7368 726e 6420 2b20 313b   =  wishrnd + 1;
+00004060: 0d0a 0970 6367 5f67 6175 7373 2867 6175  ...pcg_gauss(gau
+00004070: 7373 2c20 6e75 6d47 6175 7373 526e 6429  ss, numGaussRnd)
+00004080: 3b0d 0a09 6761 7573 7320 3d20 6761 7573  ;...gauss = gaus
+00004090: 7320 2b20 6e75 6d47 6175 7373 526e 642d  s + numGaussRnd-
+000040a0: 313b 202f 2f67 6f20 746f 2074 6865 2043  1; //go to the C
+000040b0: 4f44 455f 454f 4620 6f66 2074 6865 2067  ODE_EOF of the g
+000040c0: 7561 7373 0d0a 0d0a 0977 6973 6872 6e64  uass.....wishrnd
+000040d0: 202b 3d20 286d 2d32 2920 2a20 6d3b 202f   += (m-2) * m; /
+000040e0: 2f20 676f 2074 6f20 7468 6520 7374 6172  / go to the star
+000040f0: 7420 6f66 2074 6865 2073 6563 6f6e 6420  t of the second 
+00004100: 726f 7720 6672 6f6d 2074 6865 206c 6173  row from the las
+00004110: 740d 0a09 666f 7220 2869 6e74 2063 6f6c  t...for (int col
+00004120: 203d 6d2d 313b 2063 6f6c 203e 3d32 3b20   =m-1; col >=2; 
+00004130: 636f 6c2d 2d29 207b 0d0a 0909 666f 7220  col--) {....for 
+00004140: 2869 6e74 2072 6f77 203d 206d 3b20 726f  (int row = m; ro
+00004150: 7720 3e3d 2063 6f6c 2b31 3b20 726f 772d  w >= col+1; row-
+00004160: 2d29 207b 0d0a 0909 0977 6973 6872 6e64  -) {.....wishrnd
+00004170: 5b72 6f77 202d 2031 5d20 3d20 2a67 6175  [row - 1] = *gau
+00004180: 7373 2d2d 3b0d 0a09 097d 0d0a 0909 7769  ss--;....}....wi
+00004190: 7368 726e 6420 2d3d 206d 3b0d 0a09 7d0d  shrnd -= m;...}.
+000041a0: 0a09 2077 6973 6872 6e64 203d 2077 6973  .. wishrnd = wis
+000041b0: 6872 6e64 3b20 202f 2f67 6f20 6261 636b  hrnd;  //go back
+000041c0: 2074 6f20 7468 6520 7374 6172 7420 6f66   to the start of
+000041d0: 2072 6e64 0d0a 0920 0d0a 0d0a 0d0a 0920   rnd... ....... 
+000041e0: 2f2f 205a 6572 6f6f 7574 2074 6865 2075  // Zeroout the u
+000041f0: 7070 6572 2074 7269 616e 676c 650d 0a09  pper triangle...
+00004200: 2066 6f72 2028 696e 7420 636f 6c20 3d20   for (int col = 
+00004210: 303b 2063 6f6c 203c 6d3b 2063 6f6c 2b2b  0; col <m; col++
+00004220: 2920 7b0d 0a09 0920 666f 7220 2869 6e74  ) {.... for (int
+00004230: 2072 6f77 203d 2030 3b20 726f 773c 636f   row = 0; row<co
+00004240: 6c3b 2072 6f77 2b2b 2920 7b0d 0a09 0909  l; row++) {.....
+00004250: 2077 6973 6872 6e64 5b72 6f77 5d20 3d20   wishrnd[row] = 
+00004260: 303b 0d0a 0909 207d 0d0a 0909 2077 6973  0;.... }.... wis
+00004270: 6872 6e64 202b 3d20 6d3b 0d0a 0920 7d0d  hrnd += m;... }.
+00004280: 0a09 2077 6973 6872 6e64 203d 2077 6973  .. wishrnd = wis
+00004290: 6872 6e64 202d 6d2a 6d3b 2020 2f2f 676f  hrnd -m*m;  //go
+000042a0: 2062 6163 6b20 746f 2074 6865 2073 7461   back to the sta
+000042b0: 7274 206f 6620 726e 6409 0d0a 0d0a 2020  rt of rnd.....  
+000042c0: 202f 2f20 2046 696c 6c20 7468 6520 6469   //  Fill the di
+000042d0: 6167 6f6e 6c20 7769 7468 2067 616d 6d61  agonl with gamma
+000042e0: 2072 616e 646f 6d20 7661 7269 6162 6c65   random variable
+000042f0: 730d 0a09 666f 7220 2869 6e74 2069 203d  s...for (int i =
+00004300: 2031 3b20 6920 3c3d 206d 3b20 692b 2b29   1; i <= m; i++)
+00004310: 207b 0d0a 0909 4633 3220 6368 6973 7161   {....F32 chisqa
+00004320: 7572 653b 0d0a 0909 7063 675f 6761 6d6d  ure;....pcg_gamm
+00004330: 6128 2663 6869 7371 6175 7265 2c20 2846  a(&chisqaure, (F
+00004340: 3332 2928 6466 202d 2069 202b 2031 2920  32)(df - i + 1) 
+00004350: 2f20 322e 662c 2031 293b 0d0a 0909 2a77  / 2.f, 1);....*w
+00004360: 6973 6872 6e64 203d 2063 6869 7371 6175  ishrnd = chisqau
+00004370: 7265 203d 2073 7172 7466 2863 6869 7371  re = sqrtf(chisq
+00004380: 6175 7265 202a 2032 2e66 293b 0d0a 0909  aure * 2.f);....
+00004390: 7769 7368 726e 6420 2b3d 2028 6d20 2b20  wishrnd += (m + 
+000043a0: 3129 3b0d 0a09 7d0d 0a0d 0a7d 0d0a 0d0a  1);...}....}....
+000043b0: 2369 6e63 6c75 6465 2022 6162 635f 6d61  #include "abc_ma
+000043c0: 742e 6822 0d0a 766f 6964 2020 7063 675f  t.h"..void  pcg_
+000043d0: 696e 7677 6973 6861 7274 5f75 7070 6572  invwishart_upper
+000043e0: 2846 3332 5054 5220 6977 726e 645f 7570  (F32PTR iwrnd_up
+000043f0: 7065 722c 2046 3332 5054 5220 6977 726e  per, F32PTR iwrn
+00004400: 645f 7570 7065 725f 696e 762c 2046 3332  d_upper_inv, F32
+00004410: 5054 5220 746d 702c 2049 3332 206d 2c20  PTR tmp, I32 m, 
+00004420: 4633 3250 5452 2051 7570 2c20 4633 3220  F32PTR Qup, F32 
+00004430: 6466 290d 0a7b 2020 200d 0a09 2f2f 4957  df)..{   ...//IW
+00004440: 2851 2c76 293a 2051 3d51 7527 2a51 7570  (Q,v): Q=Qu'*Qup
+00004450: 0d0a 092f 2f54 6865 2049 5720 6d61 7472  ...//The IW matr
+00004460: 6978 2073 686f 756c 6420 6265 2052 272a  ix should be R'*
+00004470: 5220 7768 6572 6520 523d 6977 726e 645f  R where R=iwrnd_
+00004480: 7570 7065 723d 2069 6e76 2857 292a 5175  upper= inv(W)*Qu
+00004490: 700d 0a09 2f2f 200d 0a09 2f2f 2069 7277  p...// ...// irw
+000044a0: 6e64 5f75 7070 6572 5f69 6e76 2d20 696e  nd_upper_inv- in
+000044b0: 7628 5229 3d69 6e76 2851 7570 292a 572e  v(R)=inv(Qup)*W.
+000044c0: 0d0a 0920 0d0a 0946 3332 5054 5220 576c  ... ...F32PTR Wl
+000044d0: 6f77 6572 203d 2074 6d70 3b0d 0a0d 0a09  ower = tmp;.....
+000044e0: 2f2f 2054 6869 7320 6973 2061 6e20 696d  // This is an im
+000044f0: 706c 6d65 6e74 6174 696f 6e20 6f66 2074  plmentation of t
+00004500: 6865 2042 6172 6c6c 6574 2061 6c67 6f72  he Barllet algor
+00004510: 7469 686d 0d0a 092f 2f6c 6f63 616c 5f70  tihm...//local_p
+00004520: 6367 5f77 6973 6861 7274 5f75 6e69 745f  cg_wishart_unit_
+00004530: 6c6f 7774 7269 616e 676c 655f 6e6f 7a65  lowtriangle_noze
+00004540: 726f 6f75 7428 726e 672c 2057 6c6f 7765  roout(rng, Wlowe
+00004550: 722c 2057 6c6f 7765 7220 2b6d 2a6d 2c20  r, Wlower +m*m, 
+00004560: 6d2c 2064 6629 3b0d 0a09 7063 675f 7769  m, df);...pcg_wi
+00004570: 7368 6172 745f 756e 6974 5f6c 6f77 7472  shart_unit_lowtr
+00004580: 6961 6e67 6c65 5f7a 6572 6f6f 7574 5f6e  iangle_zeroout_n
+00004590: 6f74 6d70 2857 6c6f 7765 722c 206d 2c20  otmp(Wlower, m, 
+000045a0: 6466 293b 0d0a 090d 0a0d 0a09 2f2f 2053  df);........// S
+000045b0: 6f6c 7665 2057 6c2a 6977 726e 645f 7570  olve Wl*iwrnd_up
+000045c0: 7065 723d 5175 700d 0a09 6633 325f 636f  per=Qup...f32_co
+000045d0: 7079 2851 7570 2c20 6977 726e 645f 7570  py(Qup, iwrnd_up
+000045e0: 7065 722c 206d 202a 206d 293b 0d0a 0966  per, m * m);...f
+000045f0: 6f72 2028 696e 7420 6920 3d20 303b 2069  or (int i = 0; i
+00004600: 203c 206d 3b20 2b2b 6929 207b 0d0a 0909   < m; ++i) {....
+00004610: 736f 6c76 655f 4c5f 6173 5f4c 2857 6c6f  solve_L_as_L(Wlo
+00004620: 7765 722c 2069 7772 6e64 5f75 7070 6572  wer, iwrnd_upper
+00004630: 2c20 6d2c 206d 293b 0d0a 0909 6977 726e  , m, m);....iwrn
+00004640: 645f 7570 7065 7220 3d20 6977 726e 645f  d_upper = iwrnd_
+00004650: 7570 7065 7220 2b20 6d3b 0d0a 097d 0d0a  upper + m;...}..
+00004660: 0d0a 090d 0a09 2f2f 536f 6c76 6520 5175  ......//Solve Qu
+00004670: 702a 6972 776e 645f 7570 7065 725f 696e  p*irwnd_upper_in
+00004680: 763d 570d 0a09 6966 2028 6977 726e 645f  v=W...if (iwrnd_
+00004690: 7570 7065 725f 696e 7629 207b 0d0a 0909  upper_inv) {....
+000046a0: 2f2f 2069 7277 6e64 5f75 7070 6572 5f69  // irwnd_upper_i
+000046b0: 6e76 2d69 6e76 2852 293d 696e 7628 5175  nv-inv(R)=inv(Qu
+000046c0: 7029 2a57 2e09 090d 0a09 0966 3332 5f63  p)*W.......f32_c
+000046d0: 6f70 7928 576c 6f77 6572 2c20 6977 726e  opy(Wlower, iwrn
+000046e0: 645f 7570 7065 725f 696e 762c 206d 202a  d_upper_inv, m *
+000046f0: 206d 293b 0d0a 0909 666f 7220 2869 6e74   m);....for (int
+00004700: 2069 203d 2030 3b20 6920 3c20 6d3b 202b   i = 0; i < m; +
+00004710: 2b69 2920 7b0d 0a09 0909 736f 6c76 655f  +i) {.....solve_
+00004720: 555f 6173 5f55 2851 7570 2c20 6977 726e  U_as_U(Qup, iwrn
+00004730: 645f 7570 7065 725f 696e 762c 206d 2c20  d_upper_inv, m, 
+00004740: 6d29 3b0d 0a09 0909 6977 726e 645f 7570  m);.....iwrnd_up
+00004750: 7065 725f 696e 7620 3d20 6977 726e 645f  per_inv = iwrnd_
+00004760: 7570 7065 725f 696e 7620 2b20 6d3b 0d0a  upper_inv + m;..
+00004770: 0909 7d0d 0a09 7d0d 0a09 0d0a 7d0d 0a0d  ..}...}.....}...
+00004780: 0a0d 0a23 696e 636c 7564 6520 2261 6263  ...#include "abc
+00004790: 5f30 3030 5f77 6172 6e69 6e67 2e68 220d  _000_warning.h".
+000047a0: 0a                                       .
```

### Comparing `Rbeast-0.1.13/ext_src/abc_rand_pcg_global.h` & `Rbeast-0.1.14/ext_src/abc_rand_pcg_global.h`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,14 @@
 
 
 /*****************************************************************************************/
 /*                                                                                        */
 /*****************************************************************************************/
 typedef struct GAUSS_CONSTANT {
 	F32    x[64];
-	U32    yRatio[63];
-	F32    yInverse[63];
-	F32    PARAM_R, INV_PARAM_R;
+	F32    yRatio[63];	
+	I16    indices[125];
+	F32    amax;
+	F32    exp_lamda;
+	I32    inflectionId;
 } GAUSS_CONSTANT;
 extern GAUSS_CONSTANT GAUSS;
```

### Comparing `Rbeast-0.1.13/ext_src/abc_rand_pcg_local.h` & `Rbeast-0.1.14/ext_src/abc_rand_pcg_local.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 #pragma once
 #include "abc_datatype.h"
+
  
-//LCG:
+// LCG:
 // X     =  X    * multiplier + shift(plus/state.inc) mod 2^64
 // State =  State* multiplier + shift(plus/INC)       mod 2^64
+
 typedef union local_pcg32_random_struct {
 	//https://github.com/imneme/pcg-c-basic/blob/master/pcg_basic.h
 	/**************/
 	//for pcg_avx
 	/**************/
 	struct {
 	U64 ALIGN32_BEG
 		state[4]
 		ALIGN32_END;  // RNG state. All values are possible.
-	U64	increment;	// Controls which RNG sequence (stream) is
-					// selected. Must *always* be odd.
+	U64	increment;	  // Controls which RNG sequence (stream) is
+					  // selected. Must *always* be odd.
 	U64 MULTIPLIER_4steps;
 	U64 INCREMENT_4steps;
+	
+	U32 INTERNAL_RNDBUF[4];  // Used in pcg_random_with_internalbuf to save unused random numbers
+	int BUF_PTR;
 	};
 
 	/**************/
-	//for pcg_avx
+	//for pcg_avx512
 	/**************/
 	struct {
 		U64 ALIGN32_BEG
 			state512[8]
-			ALIGN32_END;  // RNG state. All values are possible.
+			ALIGN32_END;    // RNG state. All values are possible.
 		U64	increment512;	// Controls which RNG sequence (stream) is
-						// selected. Must *always* be odd.
+						    // selected. Must *always* be odd.
 		U64 MULTIPLIER_8steps;
 		U64 INCREMENT_8steps;
 	};
 
-	// forl pcg_local
+	// forl pcg_local_generic
 	struct {
 		U64 STATE;
 		U64	INCREMENT;	// Controls which RNG sequence (stream) is
 	};
 } local_pcg32_random_t;
 
 extern void (*local_pcg_set_seed)(local_pcg32_random_t* rng, U64 initstate, U64 initseq);
 extern void (*local_pcg_random)(local_pcg32_random_t* rng, U32PTR rnd, I32 N);
+extern void (*local_pcg_print_state)(local_pcg32_random_t* rng);
 
+extern F32  local_pcg_trgauss_oneside_scalar(local_pcg32_random_t* rng, F32 a, int whichside);
+extern  void local_pcg_randint(local_pcg32_random_t* rng, int bnd, I32PTR RND, int N);
 extern void local_pcg_gauss(local_pcg32_random_t* rng, F32PTR RND, int N);
 extern void local_pcg_gamma(local_pcg32_random_t* rng, F32PTR rnd, F32 a, int N);
 extern void local_pcg_wishart_unit_lowtriangle_zeroout(local_pcg32_random_t* rng, F32PTR rnd, F32PTR tmp, I32 m, F32 df);
 extern void local_pcg_wishart_unit_lowtriangle_zeroout_notmp(local_pcg32_random_t* rng, F32PTR wishrnd, I32 m, F32 df);
 extern void local_pcg_invwishart_upper(local_pcg32_random_t* rng, F32PTR iwrnd_upper, F32PTR iwrnd_upper_inv, F32PTR tmp, I32 m, F32PTR Qup, F32 df);
-void SetupPCG_GENERIC();
-void SetupPCG_AVX2();
-void SetupPCG_AVX512();
+extern void SetupPCG_GENERIC(void);
+extern void SetupPCG_AVX2(void);
+extern void SetupPCG_AVX512(void);
 
 
 // r_vsRngGaussian(VSL_RNG_METHOD_GAUSSIAN_ICDF, stream, k, beta, 0, 1);
 #define VSLStreamStatePtr													  local_pcg32_random_t														 
 #define r_vslNewStream(stream, METHOD_dummy, seed)							  local_pcg_set_seed(stream, 0x853c49e6748fea9bULL, seed)  //	pcg_set_seed(seed, (size_t) &globalStream)
 #define r_viRngUniformBits32(  METHOD_dummy, stream, N, rnd)				  local_pcg_random(&stream,rnd, N)
 #define r_vsRngGamma(		   METHOD_dummy, stream, N, rnd, a, b, beta_dummy) local_pcg_gamma(&stream, rnd, a,N)
```

### Comparing `Rbeast-0.1.13/ext_src/abc_rand_pcg_local_avx2.c` & `Rbeast-0.1.14/ext_src/abc_rand_pcg_local_avx2.c`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #include "abc_ide_util.h"
 
 #include "abc_vec.h"
 
 #include "abc_rand_pcg_global.h"
 #include "abc_rand_pcg_local.h"
  
-
+#include "assert.h"
 
 #ifdef MSVC_COMPILER
 #define __attribute__(x)
 //https://stackoverflow.com/questions/21116270/gcc-attributes-with-c-methods
 // In a function definition, the attribute field should go before the function name
 //, but it can be put after the function decleration in the decleration
 #endif
@@ -83,14 +83,23 @@
 #define PCG_DEFAULT_INCREMENT_64   1442695040888963407ULL ////https://github.com/imneme/pcg-c/blob/master/include/pcg_variants.h
 
 
 //https://github.com/imneme/pcg-c-basic/blob/master/pcg_basic.h
 #define PCG_DEFAULT_GLOBAL_STATE_64     0x853c49e6748fea9bULL
 #define PCG_DEFAULT_GLOBAL_INCREMENT_64 0xda3e39cb94b95bdbULL
 
+ 
+void avx_pcg_print_state(local_pcg32_random_t* rng) {
+
+	r_printf("PCG State: \n");
+	r_printf("State: %"  PRIx64 " %" PRIx64 " %" PRIx64 " %" PRIx64 "\n", rng->state[0], rng->state[1], rng->state[2], rng->state[3] );
+	r_printf("Increment: %"  PRIx64  "\n", rng->increment);
+	r_printf("Mutiplier4: %"  PRIx64  "\n", rng->MULTIPLIER_4steps);
+	r_printf("INcrementr4: %"  PRIx64  "\n\n", rng->INCREMENT_4steps);
+}
 
  void avx_pcg_set_seed(local_pcg32_random_t *rng, U64 initstate, U64 initseq)
 {
 	
 	 initstate = PCG_DEFAULT_GLOBAL_STATE_64 ^ initseq; //Added bcz only initseq is supplied as a seed. We run initseq to randomize initstate a little bit
 
 	initstate = initstate == 0 ? PCG_DEFAULT_GLOBAL_STATE_64 : initstate;
@@ -106,14 +115,19 @@
 	rng->state[3] = state = state * PCG_DEFAULT_MULTIPLIER_64 + rng->increment;// pcg_random(&rnd, 1);
 	__m256i state256 = _mm256_set_epi64x(rng->state[3], rng->state[2], rng->state[1], rng->state[0]);;
 
 	//r_printf("state: %30" PRIu64 " inc: %30"  PRIu64 "\n", rng->state[0], rng->increment);
 
 	// Compute the multiper and shift constants for a four-step advance
 	pcg_get_lcg_multiplier_shift_multistep(4L, PCG_DEFAULT_MULTIPLIER_64, rng->increment, &rng->MULTIPLIER_4steps, &rng->INCREMENT_4steps);
+
+	rng->BUF_PTR = 4;// used in the pcg_random_internalbuf (4 meaans the buf is empty: 0,1,2,3: there are still data)
+
+	extern void init_gauss_rnd(void);
+	init_gauss_rnd(); //Indepedent of PCG, used to initialize the GAUSS structure
 }
 
  static INLINE  __m256i  __attribute__((always_inline)) GetMoveMask(int n)    {
     __m128i maskIdx = _mm_cvtsi64_si128(0x0706050403020100);
     __m256i maskNum = _mm256_cvtepu8_epi32(maskIdx);
     __m256i nvec    = _mm256_set1_epi32(n);
     //__m256i maskmov = _mm256_sub_epi32(maskNum, nvec);
@@ -226,14 +240,91 @@
 
 	}
 	_mm256_storeu_si256(rng->state, oldstate);
 
 	_mm256_zeroupper();
 }
  
+void avx_pcg_random_with_internalbuf(local_pcg32_random_t* rng, U32PTR rnd, I32 N) {
+
+// Move these two local variable  to the rng structure so they can be initizeled during pcg_set_seed
+//	static  __m128 INTERNAL_RNDBUF;
+//	static  I32    BUF_PTR = 4;   // 4 means theare are no data: (0,1,2,3: there are data left)
+
+	__m256i oldstate = _mm256_loadu_si256(rng->state);
+
+	// N is changing, indicating the remaining number
+	while (N > 0) {
+		
+		if (rng->BUF_PTR < 4) {
+        // there is still data in the buffer; first consume the buffer
+			U32PTR rndbuf = (U32PTR) rng->INTERNAL_RNDBUF + rng->BUF_PTR;
+			if (N == 1L || rng->BUF_PTR ==3) {
+				rnd[0] = rndbuf[0];
+				++rng->BUF_PTR;
+				++rnd;
+				--N;				
+			}
+			else if (rng->BUF_PTR == 0 && N >= 4) {
+				_mm_storeu_ps(rnd, _mm_loadu_ps(rng->INTERNAL_RNDBUF));
+				rng->BUF_PTR = 4L;
+				rnd     += 4;
+				N       -= 4;
+				// THen run to the bottom part to replish the buffer
+			} else {
+			// nCopy must be one of 2 and 3.
+				int nAvailable = (4 - rng->BUF_PTR);
+				int nCopy      = min(nAvailable, N);
+				rnd[0] = rndbuf[0];
+				rnd[1] = rndbuf[1];
+                if (nCopy == 3) {
+					rnd[2] = rndbuf[2];
+				}
+				rng->BUF_PTR += nCopy;
+				rnd          += nCopy;
+				N            -= nCopy;
+			}
+		}
+	
+		if (rng->BUF_PTR != 4) {
+			//assert(N == 0);
+			continue;
+		}
+ 
+		// Jump here to sample if BUF_PTR == 4
+
+		const __m256i	INCREMENT_SHIFT = _mm256_set1_epi64x(rng->INCREMENT_4steps);
+		const __m256i	MULITPLIER     = _mm256_set1_epi64x(rng->MULTIPLIER_4steps);
+
+		#define srl	_mm256_srli_epi64
+		#define xor _mm256_xor_si256
+
+		__m256i xorshifted = srl(xor (srl(oldstate, 18u), oldstate), 27u);
+		__m256i rot = srl(oldstate, 59u);
+		oldstate = _mm256_add_epi64(__mul64_haswell(oldstate, MULITPLIER), INCREMENT_SHIFT); //oldstate = oldstate * PCG_DEFAULT_MULTIPLIER_64 + shift;
+
+		__m256i result = _mm256_or_si256(
+			_mm256_srlv_epi32(xorshifted, rot),
+			_mm256_sllv_epi32(xorshifted, _mm256_sub_epi32(_mm256_set1_epi32(32), rot)) //	//https://en.wikipedia.org/wiki/Circular_shift
+		);	//*rnd++ = (xorshifted >> rot) | (xorshifted << ((- *((I32*)(&rot))  ) & 31)); //*rnd++ = (xorshifted >> rot) | (xorshifted << ((-rot) & 31));
+
+		__m128i r1 = _mm256_castsi256_si128(result);
+		__m128i r2 = _mm256_extracti128_si256(result, 1);
+		__m128  r = _mm_shuffle_ps(_mm_castsi128_ps(r1), _mm_castsi128_ps(r2), _MM_SHUFFLE(2, 0, 2, 0));
+
+		_mm_storeu_ps(rng->INTERNAL_RNDBUF, r);
+
+		rng->BUF_PTR = 0;
+	 
+
+	}
+	_mm256_storeu_si256(rng->state, oldstate);
+	_mm256_zeroupper();
+}
+
 void avx_pcg_random_vec8_slow(local_pcg32_random_t* rng,U32PTR rnd, I32 N) {
 
 	__m256i			oldstate	= _mm256_loadu_si256(rng->state );
 	const __m256i	SHIFT		= _mm256_set1_epi64x(rng->INCREMENT_4steps);
 	const __m256i	MULITPLIER	= _mm256_set1_epi64x(rng->MULTIPLIER_4steps);
  
 	#define srl	_mm256_srli_epi64
@@ -273,17 +364,19 @@
 
 	}
 	_mm256_storeu_si256(rng->state, oldstate);	
 }
 
 
 
-void SetupPCG_AVX2(){
+void SetupPCG_AVX2(void){
 	 local_pcg_set_seed = avx_pcg_set_seed;
-	 local_pcg_random   = avx_pcg_random;
+	 //local_pcg_random = avx_pcg_random;
+	 local_pcg_random=avx_pcg_random_with_internalbuf;
+	 local_pcg_print_state = avx_pcg_print_state;
  
 }
 #endif
 
 
 ///////////////////////////////////////////////////////////////////////////
 #ifdef CLANG_COMPILER
```

### Comparing `Rbeast-0.1.13/ext_src/abc_rand_pcg_local_avx512.c` & `Rbeast-0.1.14/ext_src/abc_rand_pcg_local_avx512.c`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,25 @@
 
 
 //https://github.com/imneme/pcg-c-basic/blob/master/pcg_basic.h
 #define PCG_DEFAULT_GLOBAL_STATE_64     0x853c49e6748fea9bULL
 #define PCG_DEFAULT_GLOBAL_INCREMENT_64 0xda3e39cb94b95bdbULL
 
 
+void avx512_pcg_print_state(local_pcg32_random_t* rng) {
+
+	r_printf("PCG State: \n");
+	r_printf("State: %"  PRIx64 " %" PRIx64 " %" PRIx64 " %" PRIx64 "\n", rng->state512[0], rng->state512[1], rng->state512[2], rng->state512[3]);
+	r_printf("State: %"  PRIx64 " %" PRIx64 " %" PRIx64 " %" PRIx64 "\n", rng->state512[4], rng->state512[5], rng->state512[6], rng->state512[7]);
+	r_printf("Increment: %"  PRIx64  "\n", rng->increment512);
+	r_printf("Mutiplier8: %"  PRIx64  "\n", rng->MULTIPLIER_8steps);
+	r_printf("INcrementr8: %"  PRIx64  "\n\n", rng->INCREMENT_8steps);
+}
+
+
 void avx512_pcg_set_seed(local_pcg32_random_t* rng, U64 initstate, U64 initseq)
 {
 	initstate = PCG_DEFAULT_GLOBAL_STATE_64 ^ initseq; //Added bcz only initseq is supplied as a seed. We run initseq to randomize initstate a little bit
 
 	initstate = initstate == 0 ? PCG_DEFAULT_GLOBAL_STATE_64 : initstate;
 	initseq   = initseq == 0 ? PCG_DEFAULT_GLOBAL_INCREMENT_64 : initseq;
 
@@ -108,18 +119,21 @@
 	__m512i state512 = _mm512_set_epi64(rng->state512[7], rng->state512[6], rng->state512[5], rng->state512[4],
 									   rng->state512[3], rng->state512[2], rng->state512[1], rng->state512[0]);
 
 	//r_printf("state: %30" PRIu64 " inc: %30"  PRIu64 "\n", rng->state[0], rng->increment);
 
 	// Compute the multiper and shift constants for a four-step advance
 	pcg_get_lcg_multiplier_shift_multistep(8L, PCG_DEFAULT_MULTIPLIER_64, rng->increment512, &rng->MULTIPLIER_8steps, &rng->INCREMENT_8steps);
+
+	extern void init_gauss_rnd(void);
+	init_gauss_rnd(); //Indepedent of PCG, used to initialize the GAUSS structure
 }
 
 static __mmask16        masktemplate[16];
-static INLINE void      FillMaskTemplate() { for (I32 i = 0; i < 16; i++)    masktemplate[i] = (1UL << i) - 1UL; }
+static INLINE void      FillMaskTemplate(void) { for (I32 i = 0; i < 16; i++)    masktemplate[i] = (1UL << i) - 1UL; }
 static INLINE __mmask16 GetMoveMask(int n) { return masktemplate[n]; }
 
 
 
 void avx512_pcg_random(local_pcg32_random_t* rng, U32PTR rnd, I32 N) {
 
 	const __m512i	INCREMENT_SHIFT = _mm512_set1_epi64(rng->INCREMENT_8steps);
@@ -158,19 +172,19 @@
 
 	}
 	_mm512_storeu_si512(rng->state512, oldstate);
 
 	_mm256_zeroupper();
 }
 
-void SetupPCG_AVX512() {
+void SetupPCG_AVX512(void) {
 	FillMaskTemplate();
 	local_pcg_set_seed = avx512_pcg_set_seed;
 	local_pcg_random   = avx512_pcg_random;
-
+	local_pcg_print_state = avx512_pcg_print_state;
 }
 #endif
 
 
 ///////////////////////////////////////////////////////////////////////////
 #ifdef CLANG_COMPILER
 	//pragma clang attribute push (__attribute__((target("avx,avx2"))), apply_to=function)
```

### Comparing `Rbeast-0.1.13/ext_src/abc_rand_pcg_local_generic.c` & `Rbeast-0.1.14/ext_src/abc_rand_pcg_local_generic.c`

 * *Files 6% similar despite different names*

```diff
@@ -107,95 +107,118 @@
 000006a0: 494e 4352 454d 454e 543b 092f 2f20 436f  INCREMENT;.// Co
 000006b0: 6e74 726f 6c73 2077 6869 6368 2052 4e47  ntrols which RNG
 000006c0: 2073 6571 7565 6e63 6520 2873 7472 6561   sequence (strea
 000006d0: 6d29 2069 7320 0d0a 0909 0909 092f 2f20  m) is .......// 
 000006e0: 7365 6c65 6374 6564 2e20 4d75 7374 202a  selected. Must *
 000006f0: 616c 7761 7973 2a20 6265 206f 6464 2e0d  always* be odd..
 00000700: 0a7d 3b0d 0a20 2a2f 0d0a 0d0a 766f 6964  .};.. */....void
-00000710: 2067 656e 5f70 6367 5f72 616e 646f 6d28   gen_pcg_random(
-00000720: 6c6f 6361 6c5f 7063 6733 325f 7261 6e64  local_pcg32_rand
-00000730: 6f6d 5f74 2a20 726e 672c 2055 3332 5054  om_t* rng, U32PT
-00000740: 5220 726e 642c 2049 3332 204e 293b 0d0a  R rnd, I32 N);..
-00000750: 766f 6964 2067 656e 5f70 6367 5f73 6574  void gen_pcg_set
-00000760: 5f73 6565 6428 6c6f 6361 6c5f 7063 6733  _seed(local_pcg3
-00000770: 325f 7261 6e64 6f6d 5f74 2a20 726e 672c  2_random_t* rng,
-00000780: 2055 3634 2069 6e69 7473 7461 7465 2c20   U64 initstate, 
-00000790: 5536 3420 696e 6974 7365 7129 0d0a 7b0d  U64 initseq)..{.
-000007a0: 0a0d 0a09 696e 6974 7374 6174 6520 3d20  ....initstate = 
-000007b0: 5043 475f 4445 4641 554c 545f 474c 4f42  PCG_DEFAULT_GLOB
-000007c0: 414c 5f53 5441 5445 5f36 3420 5e20 696e  AL_STATE_64 ^ in
-000007d0: 6974 7365 713b 202f 2f41 6464 6564 2062  itseq; //Added b
-000007e0: 637a 206f 6e6c 7920 696e 6974 7365 7120  cz only initseq 
-000007f0: 6973 2073 7570 706c 6965 6420 6173 2061  is supplied as a
-00000800: 2073 6565 642e 2057 6520 7275 6e20 696e   seed. We run in
-00000810: 6974 7365 7120 746f 2072 616e 646f 6d69  itseq to randomi
-00000820: 7a65 2069 6e69 7473 7461 7465 2061 206c  ze initstate a l
-00000830: 6974 746c 6520 6269 740d 0a0d 0a09 696e  ittle bit.....in
-00000840: 6974 7374 6174 6520 3d20 696e 6974 7374  itstate = initst
-00000850: 6174 6520 3d3d 2030 203f 2050 4347 5f44  ate == 0 ? PCG_D
-00000860: 4546 4155 4c54 5f47 4c4f 4241 4c5f 5354  EFAULT_GLOBAL_ST
-00000870: 4154 455f 3634 203a 2069 6e69 7473 7461  ATE_64 : initsta
-00000880: 7465 3b0d 0a09 696e 6974 7365 7120 2020  te;...initseq   
-00000890: 3d20 696e 6974 7365 7120 3d3d 2030 203f  = initseq == 0 ?
-000008a0: 2020 2050 4347 5f44 4546 4155 4c54 5f47     PCG_DEFAULT_G
-000008b0: 4c4f 4241 4c5f 494e 4352 454d 454e 545f  LOBAL_INCREMENT_
-000008c0: 3634 203a 2069 6e69 7473 6571 3b0d 0a0d  64 : initseq;...
-000008d0: 0a0d 0a09 726e 672d 3e53 5441 5445 0909  ....rng->STATE..
-000008e0: 203d 2030 553b 0d0a 0972 6e67 2d3e 494e   = 0U;...rng->IN
-000008f0: 4352 454d 454e 5420 2020 3d20 2869 6e69  CREMENT   = (ini
-00000900: 7473 6571 203c 3c20 3175 2920 7c20 3175  tseq << 1u) | 1u
-00000910: 3b20 2009 2f2f 696e 6320 6d75 7374 2062  ;  .//inc must b
-00000920: 6520 616e 206f 6464 206e 756d 6265 720d  e an odd number.
-00000930: 0a0d 0a09 5533 3220 726e 643b 0d0a 0967  ....U32 rnd;...g
-00000940: 656e 5f70 6367 5f72 616e 646f 6d28 726e  en_pcg_random(rn
-00000950: 672c 2026 726e 642c 2031 293b 0d0a 0972  g, &rnd, 1);...r
-00000960: 6e67 2d3e 5354 4154 4520 2b3d 2069 6e69  ng->STATE += ini
-00000970: 7473 7461 7465 3b0d 0a09 6765 6e5f 7063  tstate;...gen_pc
-00000980: 675f 7261 6e64 6f6d 2872 6e67 2c20 2672  g_random(rng, &r
-00000990: 6e64 2c20 3129 3b0d 0a7d 0d0a 200d 0a76  nd, 1);..}.. ..v
-000009a0: 6f69 6420 6765 6e5f 7063 675f 7261 6e64  oid gen_pcg_rand
-000009b0: 6f6d 286c 6f63 616c 5f70 6367 3332 5f72  om(local_pcg32_r
-000009c0: 616e 646f 6d5f 742a 2072 6e67 2c20 5533  andom_t* rng, U3
-000009d0: 3250 5452 2072 6e64 2c20 4933 3220 4e29  2PTR rnd, I32 N)
-000009e0: 200d 0a7b 0d0a 0955 3634 206f 6c64 7374   ..{...U64 oldst
-000009f0: 6174 6520 3d20 726e 672d 3e53 5441 5445  ate = rng->STATE
-00000a00: 3b0d 0a09 5536 3420 7368 6966 7420 2020  ;...U64 shift   
-00000a10: 203d 2072 6e67 2d3e 494e 4352 454d 454e   = rng->INCREMEN
-00000a20: 543b 0d0a 0d0a 0966 6f72 2028 696e 7420  T;.....for (int 
-00000a30: 6920 3d20 303b 2069 203c 204e 3b20 692b  i = 0; i < N; i+
-00000a40: 2b29 0d0a 097b 0d0a 0909 5533 3220 786f  +)...{....U32 xo
-00000a50: 7273 6869 6674 6564 203d 2020 2020 2028  rshifted =     (
-00000a60: 286f 6c64 7374 6174 6520 3e3e 2031 3875  (oldstate >> 18u
-00000a70: 2920 5e20 6f6c 6473 7461 7465 2920 3e3e  ) ^ oldstate) >>
-00000a80: 2032 3775 2020 203b 0d0a 0909 5533 3220   27u   ;....U32 
-00000a90: 726f 7420 3d20 6f6c 6473 7461 7465 203e  rot = oldstate >
-00000aa0: 3e20 3539 753b 0d0a 0909 2f2f 2a72 6e64  > 59u;....//*rnd
-00000ab0: 2b2b 203d 2028 786f 7273 6869 6674 6564  ++ = (xorshifted
-00000ac0: 203e 3e20 726f 7429 207c 2028 786f 7273   >> rot) | (xors
-00000ad0: 6869 6674 6564 203c 3c20 2828 2d72 6f74  hifted << ((-rot
-00000ae0: 2920 2620 3331 2929 3b0d 0a09 092f 2f68  ) & 31));....//h
-00000af0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00000b00: 6469 612e 6f72 672f 7769 6b69 2f43 6972  dia.org/wiki/Cir
-00000b10: 6375 6c61 725f 7368 6966 740d 0a09 092a  cular_shift....*
-00000b20: 726e 642b 2b20 3d20 2878 6f72 7368 6966  rnd++ = (xorshif
-00000b30: 7465 6420 3e3e 2072 6f74 2920 7c20 2878  ted >> rot) | (x
-00000b40: 6f72 7368 6966 7465 6420 3c3c 2028 282d  orshifted << ((-
-00000b50: 202a 2828 4933 322a 2928 2672 6f74 2929   *((I32*)(&rot))
-00000b60: 2020 2920 2620 3331 2929 3b20 0d0a 0909    ) & 31)); ....
-00000b70: 6f6c 6473 7461 7465 203d 206f 6c64 7374  oldstate = oldst
-00000b80: 6174 6520 2a20 5043 475f 4445 4641 554c  ate * PCG_DEFAUL
-00000b90: 545f 4d55 4c54 4950 4c49 4552 5f36 3420  T_MULTIPLIER_64 
-00000ba0: 2b20 7368 6966 743b 0d0a 097d 0d0a 0972  + shift;...}...r
-00000bb0: 6e67 2d3e 5354 4154 4520 3d20 6f6c 6473  ng->STATE = olds
-00000bc0: 7461 7465 3b0d 0a7d 0d0a 0d0a 766f 6964  tate;..}....void
-00000bd0: 2053 6574 7570 5043 475f 4745 4e45 5249   SetupPCG_GENERI
-00000be0: 4328 2920 7b0d 0a0d 0a09 6c6f 6361 6c5f  C() {.....local_
-00000bf0: 7063 675f 7365 745f 7365 6564 203d 2067  pcg_set_seed = g
-00000c00: 656e 5f70 6367 5f73 6574 5f73 6565 643b  en_pcg_set_seed;
-00000c10: 0d0a 096c 6f63 616c 5f70 6367 5f72 616e  ...local_pcg_ran
-00000c20: 646f 6d20 3d20 6765 6e5f 7063 675f 7261  dom = gen_pcg_ra
-00000c30: 6e64 6f6d 3b0d 0a7d 0d0a 2f2a 2a2a 2a2a  ndom;..}../*****
-00000c40: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000c50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000c60: 2a2a 2a2a 2a2a 2a2a 2a2f 0d0a 2369 6e63  *********/..#inc
-00000c70: 6c75 6465 2022 6162 635f 3030 305f 7761  lude "abc_000_wa
-00000c80: 726e 696e 672e 6822 0d0a                 rning.h"..
+00000710: 2067 656e 5f70 6367 5f70 7269 6e74 5f73   gen_pcg_print_s
+00000720: 7461 7465 286c 6f63 616c 5f70 6367 3332  tate(local_pcg32
+00000730: 5f72 616e 646f 6d5f 742a 2072 6e67 2920  _random_t* rng) 
+00000740: 7b0d 0a0d 0a09 725f 7072 696e 7466 2822  {.....r_printf("
+00000750: 5043 4720 5374 6174 653a 205c 6e22 293b  PCG State: \n");
+00000760: 0d0a 0972 5f70 7269 6e74 6628 2253 7461  ...r_printf("Sta
+00000770: 7465 3a20 2522 2020 5052 4978 3634 2022  te: %"  PRIx64 "
+00000780: 5c6e 222c 2072 6e67 2d3e 5354 4154 4529  \n", rng->STATE)
+00000790: 3b09 0d0a 0972 5f70 7269 6e74 6628 2249  ;....r_printf("I
+000007a0: 6e63 7265 6d65 6e74 3a20 2522 2020 5052  ncrement: %"  PR
+000007b0: 4978 3634 2020 225c 6e22 2c20 726e 672d  Ix64  "\n", rng-
+000007c0: 3e49 4e43 5245 4d45 4e54 293b 0d0a 200d  >INCREMENT);.. .
+000007d0: 0a7d 0d0a 0d0a 0d0a 766f 6964 2067 656e  .}......void gen
+000007e0: 5f70 6367 5f72 616e 646f 6d28 6c6f 6361  _pcg_random(loca
+000007f0: 6c5f 7063 6733 325f 7261 6e64 6f6d 5f74  l_pcg32_random_t
+00000800: 2a20 726e 672c 2055 3332 5054 5220 726e  * rng, U32PTR rn
+00000810: 642c 2049 3332 204e 293b 0d0a 766f 6964  d, I32 N);..void
+00000820: 2067 656e 5f70 6367 5f73 6574 5f73 6565   gen_pcg_set_see
+00000830: 6428 6c6f 6361 6c5f 7063 6733 325f 7261  d(local_pcg32_ra
+00000840: 6e64 6f6d 5f74 2a20 726e 672c 2055 3634  ndom_t* rng, U64
+00000850: 2069 6e69 7473 7461 7465 2c20 5536 3420   initstate, U64 
+00000860: 696e 6974 7365 7129 0d0a 7b0d 0a0d 0a09  initseq)..{.....
+00000870: 696e 6974 7374 6174 6520 3d20 5043 475f  initstate = PCG_
+00000880: 4445 4641 554c 545f 474c 4f42 414c 5f53  DEFAULT_GLOBAL_S
+00000890: 5441 5445 5f36 3420 5e20 696e 6974 7365  TATE_64 ^ initse
+000008a0: 713b 202f 2f41 6464 6564 2062 637a 206f  q; //Added bcz o
+000008b0: 6e6c 7920 696e 6974 7365 7120 6973 2073  nly initseq is s
+000008c0: 7570 706c 6965 6420 6173 2061 2073 6565  upplied as a see
+000008d0: 642e 2057 6520 7275 6e20 696e 6974 7365  d. We run initse
+000008e0: 7120 746f 2072 616e 646f 6d69 7a65 2069  q to randomize i
+000008f0: 6e69 7473 7461 7465 2061 206c 6974 746c  nitstate a littl
+00000900: 6520 6269 740d 0a0d 0a09 696e 6974 7374  e bit.....initst
+00000910: 6174 6520 3d20 696e 6974 7374 6174 6520  ate = initstate 
+00000920: 3d3d 2030 203f 2050 4347 5f44 4546 4155  == 0 ? PCG_DEFAU
+00000930: 4c54 5f47 4c4f 4241 4c5f 5354 4154 455f  LT_GLOBAL_STATE_
+00000940: 3634 2020 2020 203a 2069 6e69 7473 7461  64     : initsta
+00000950: 7465 3b0d 0a09 696e 6974 7365 7120 2020  te;...initseq   
+00000960: 3d20 696e 6974 7365 7120 3d3d 2030 2020  = initseq == 0  
+00000970: 203f 2050 4347 5f44 4546 4155 4c54 5f47   ? PCG_DEFAULT_G
+00000980: 4c4f 4241 4c5f 494e 4352 454d 454e 545f  LOBAL_INCREMENT_
+00000990: 3634 203a 2069 6e69 7473 6571 3b0d 0a0d  64 : initseq;...
+000009a0: 0a09 726e 672d 3e53 5441 5445 0909 203d  ..rng->STATE.. =
+000009b0: 2030 553b 0d0a 0972 6e67 2d3e 494e 4352   0U;...rng->INCR
+000009c0: 454d 454e 5420 2020 3d20 2869 6e69 7473  EMENT   = (inits
+000009d0: 6571 203c 3c20 3175 2920 7c20 3175 3b20  eq << 1u) | 1u; 
+000009e0: 2009 2f2f 696e 6320 6d75 7374 2062 6520   .//inc must be 
+000009f0: 616e 206f 6464 206e 756d 6265 720d 0a0d  an odd number...
+00000a00: 0a09 5533 3220 726e 643b 0d0a 0967 656e  ..U32 rnd;...gen
+00000a10: 5f70 6367 5f72 616e 646f 6d28 726e 672c  _pcg_random(rng,
+00000a20: 2026 726e 642c 2031 293b 0d0a 0972 6e67   &rnd, 1);...rng
+00000a30: 2d3e 5354 4154 4520 2b3d 2069 6e69 7473  ->STATE += inits
+00000a40: 7461 7465 3b0d 0a09 6765 6e5f 7063 675f  tate;...gen_pcg_
+00000a50: 7261 6e64 6f6d 2872 6e67 2c20 2672 6e64  random(rng, &rnd
+00000a60: 2c20 3129 3b0d 0a0d 0a09 6578 7465 726e  , 1);.....extern
+00000a70: 2076 6f69 6420 696e 6974 5f67 6175 7373   void init_gauss
+00000a80: 5f72 6e64 2876 6f69 6429 3b0d 0a09 696e  _rnd(void);...in
+00000a90: 6974 5f67 6175 7373 5f72 6e64 2829 3b20  it_gauss_rnd(); 
+00000aa0: 2f2f 496e 6465 7065 6465 6e74 206f 6620  //Indepedent of 
+00000ab0: 5043 472c 2075 7365 6420 746f 2069 6e69  PCG, used to ini
+00000ac0: 7469 616c 697a 6520 7468 6520 4741 5553  tialize the GAUS
+00000ad0: 5320 7374 7275 6374 7572 650d 0a7d 0d0a  S structure..}..
+00000ae0: 200d 0a76 6f69 6420 6765 6e5f 7063 675f   ..void gen_pcg_
+00000af0: 7261 6e64 6f6d 286c 6f63 616c 5f70 6367  random(local_pcg
+00000b00: 3332 5f72 616e 646f 6d5f 742a 2072 6e67  32_random_t* rng
+00000b10: 2c20 5533 3250 5452 2072 6e64 2c20 4933  , U32PTR rnd, I3
+00000b20: 3220 4e29 200d 0a7b 0d0a 0955 3634 206f  2 N) ..{...U64 o
+00000b30: 6c64 7374 6174 6520 3d20 726e 672d 3e53  ldstate = rng->S
+00000b40: 5441 5445 3b0d 0a09 5536 3420 7368 6966  TATE;...U64 shif
+00000b50: 7420 2020 203d 2072 6e67 2d3e 494e 4352  t    = rng->INCR
+00000b60: 454d 454e 543b 0d0a 0d0a 0966 6f72 2028  EMENT;.....for (
+00000b70: 696e 7420 6920 3d20 303b 2069 203c 204e  int i = 0; i < N
+00000b80: 3b20 692b 2b29 0d0a 097b 0d0a 0909 5533  ; i++)...{....U3
+00000b90: 3220 786f 7273 6869 6674 6564 203d 2020  2 xorshifted =  
+00000ba0: 2020 2028 286f 6c64 7374 6174 6520 3e3e     ((oldstate >>
+00000bb0: 2031 3875 2920 5e20 6f6c 6473 7461 7465   18u) ^ oldstate
+00000bc0: 2920 3e3e 2032 3775 2020 203b 0d0a 0909  ) >> 27u   ;....
+00000bd0: 5533 3220 726f 7420 3d20 6f6c 6473 7461  U32 rot = oldsta
+00000be0: 7465 203e 3e20 3539 753b 0d0a 0909 2f2f  te >> 59u;....//
+00000bf0: 2a72 6e64 2b2b 203d 2028 786f 7273 6869  *rnd++ = (xorshi
+00000c00: 6674 6564 203e 3e20 726f 7429 207c 2028  fted >> rot) | (
+00000c10: 786f 7273 6869 6674 6564 203c 3c20 2828  xorshifted << ((
+00000c20: 2d72 6f74 2920 2620 3331 2929 3b0d 0a09  -rot) & 31));...
+00000c30: 092f 2f68 7474 7073 3a2f 2f65 6e2e 7769  .//https://en.wi
+00000c40: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00000c50: 2f43 6972 6375 6c61 725f 7368 6966 740d  /Circular_shift.
+00000c60: 0a09 092a 726e 642b 2b20 3d20 2878 6f72  ...*rnd++ = (xor
+00000c70: 7368 6966 7465 6420 3e3e 2072 6f74 2920  shifted >> rot) 
+00000c80: 7c20 2878 6f72 7368 6966 7465 6420 3c3c  | (xorshifted <<
+00000c90: 2028 282d 202a 2828 4933 322a 2928 2672   ((- *((I32*)(&r
+00000ca0: 6f74 2929 2020 2920 2620 3331 2929 3b20  ot))  ) & 31)); 
+00000cb0: 0d0a 0909 6f6c 6473 7461 7465 203d 206f  ....oldstate = o
+00000cc0: 6c64 7374 6174 6520 2a20 5043 475f 4445  ldstate * PCG_DE
+00000cd0: 4641 554c 545f 4d55 4c54 4950 4c49 4552  FAULT_MULTIPLIER
+00000ce0: 5f36 3420 2b20 7368 6966 743b 0d0a 097d  _64 + shift;...}
+00000cf0: 0d0a 0972 6e67 2d3e 5354 4154 4520 3d20  ...rng->STATE = 
+00000d00: 6f6c 6473 7461 7465 3b0d 0a7d 0d0a 0d0a  oldstate;..}....
+00000d10: 766f 6964 2053 6574 7570 5043 475f 4745  void SetupPCG_GE
+00000d20: 4e45 5249 4328 2920 7b0d 0a0d 0a09 6c6f  NERIC() {.....lo
+00000d30: 6361 6c5f 7063 675f 7365 745f 7365 6564  cal_pcg_set_seed
+00000d40: 203d 2067 656e 5f70 6367 5f73 6574 5f73   = gen_pcg_set_s
+00000d50: 6565 643b 0d0a 096c 6f63 616c 5f70 6367  eed;...local_pcg
+00000d60: 5f72 616e 646f 6d20 2020 3d20 6765 6e5f  _random   = gen_
+00000d70: 7063 675f 7261 6e64 6f6d 3b0d 0a09 6c6f  pcg_random;...lo
+00000d80: 6361 6c5f 7063 675f 7072 696e 745f 7374  cal_pcg_print_st
+00000d90: 6174 6520 3d20 6765 6e5f 7063 675f 7072  ate = gen_pcg_pr
+00000da0: 696e 745f 7374 6174 653b 0d0a 7d0d 0a2f  int_state;..}../
+00000db0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000dc0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000dd0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2f0d  **************/.
+00000de0: 0a23 696e 636c 7564 6520 2261 6263 5f30  .#include "abc_0
+00000df0: 3030 5f77 6172 6e69 6e67 2e68 220d 0a    00_warning.h"..
```

### Comparing `Rbeast-0.1.13/ext_src/abc_svd.c` & `Rbeast-0.1.14/ext_src/abc_svd.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_system.c` & `Rbeast-0.1.14/ext_src/abc_system.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_timer.c` & `Rbeast-0.1.14/ext_src/abc_timer.c`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,14 @@
 #elif defined(__MACH__) //https: //stackoverflow.com/questions/5167269/clock-gettime-alternative-in-mac-os-x
 	tick= mach_absolute_time();
 #endif
 	return tick;
 }
 
 
-static unsigned long long ReadTSC_InternalTime;
-void				tic() { ReadTSC_InternalTime = readTSC();}
-unsigned long long  toc() {	return readTSC()- ReadTSC_InternalTime;}
+static unsigned long long ReadTSC_InternalTime_TIC;
+void				tic(void) { ReadTSC_InternalTime_TIC = readTSC();}
+unsigned long long  toc(void) {	return readTSC()- ReadTSC_InternalTime_TIC;}
 
 
 
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/abc_timer.h` & `Rbeast-0.1.14/ext_src/abc_timer.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 #pragma once
 
 #include "abc_000_macro.h"
 #include "abc_datatype.h"
 
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+
+
 #ifdef MSVC_COMPILER
     #define WIN32_LEAN_AND_MEAN
     #include <windows.h>          //QueryPerformanceFrequency QueryPerformanceCounter
 #elif defined( __MACH__)
     #include <mach/mach_time.h>
 #endif
 
@@ -37,33 +43,34 @@
         struct timeval tv; 
         tv.tv_sec  = milliseconds / 1000;
         tv.tv_usec = milliseconds % 1000 * 1000; 
         select(0, NULL, NULL, NULL, &tv);
     #endif
 }
 
-
-extern void InitTimerFunc();
-extern void StartTimer();
-extern F64  GetElapsedSecondsSinceStart();
-extern void SetBreakPointForStartedTimer();
-extern F64  GetElaspedTimeFromBreakPoint();
-extern U64  TimerGetTickCount();
+//warning: function declaration isn't a prototype [-Wstrict-prototypes]
+//https://stackoverflow.com/questions/42125/warning-error-function-declaration-isnt-a-prototype
+extern void InitTimerFunc(void);
+extern void StartTimer(void);
+extern F64  GetElapsedSecondsSinceStart(void);
+extern void SetBreakPointForStartedTimer(void);
+extern F64  GetElaspedTimeFromBreakPoint(void);
+extern U64  TimerGetTickCount(void);
 
 
 // stackoverflow.com/questions/9887839/how-to-count-clock-cycles-with-rdtsc-in-gcc-x86
 #ifdef MSVC_COMPILER
     #include <intrin.h>    // __rdtsc
 #elif defined(SOLARIS_COMPILER)
     //https://docs.oracle.com/cd/E24457_01/html/E21991/gliwk.html
     //#include <mmintrin.h> // __rdtsc for some reason, mmintrinc.h deson't contain rdtsc
     
    //https://github.com/BackupTheBerlios/iometer-svn/blob/cd9ca025b44a0e80015a040b838d6dc7d486642a/tags/initial/iometer/src/rdtsc.c
    #include <sys/time.h>
-    static INLINE   unsigned long long __rdtsc() {
+    static INLINE   unsigned long long __rdtsc(void) {
         //https://community.oracle.com/tech/developers/discussion/2490026/about-gethrtime-function
         return  gethrtime();
     }
 
  
     /*
     //https://github.com/michealbrownm/phantom/blob/670d80162ac2e05ebcaffa7a61365068d84a3672/3rd/ed25519-donna/test-ticks.h
@@ -103,15 +110,21 @@
         return val;
     }
 
 #else
     #include <x86intrin.h> // __rdtsc
 #endif
 
-static INLINE unsigned long long readTSC() {
+static INLINE unsigned long long readTSC(void) {
     // _mm_lfence();  // optionally wait for earlier insns to retire before reading the clock
     return __rdtsc();
     // _mm_lfence();  // optionally block later instructions until rdtsc retires
 }
 
-extern void               tic();
-extern unsigned long long toc();
+extern void               tic(void);
+extern unsigned long long toc(void);
+
+
+
+#ifdef __cplusplus
+}
+#endif
```

### Comparing `Rbeast-0.1.13/ext_src/abc_vec.h` & `Rbeast-0.1.14/ext_src/abc_vec.h`

 * *Files 11% similar despite different names*

```diff
@@ -56,30 +56,69 @@
 
 	extern void f32_cumsum_inplace(const F32PTR X, int N);
 	extern void f32_cumsumsqr_inplace(const F32PTR X, int N);
 	extern F32 f32_sumlog_slow(const F32PTR  X, const int N);
 	extern F32 f32_sumlog(const F32PTR  X, const int N);
 	extern I32 i08_find_nth_onebyte_binvec(U08PTR binvec, I32 N, I32 nth);
 	extern I32 i08_find_nth_onebyte_binvec_v2(U08PTR binvec, I32 N, I32 numOneBytes, U32 rnd);
+	extern I64 i08_sum(I08PTR x, int N);
+
+
+	extern int i32_insert_noduplicate(I32PTR x, I32 N, I32PTR Xnew, I32 Nnew);
+	extern int i32_unique_inplace(I32PTR x, int N);
+	extern int i32_exclude_inplace(I32PTR x, int N, I32PTR excludeList, I32 Nexclude);
 	extern void f32_sumfilter(const F32PTR X, F32PTR Y, int N, int winSize);
 	extern F32  f32_corr_rmse_nan(const F32PTR X, const F32PTR Y, int N, F32PTR rmse);
 	extern void  f32_truncate_inplace(const F32PTR X, F32 value, int N);
 
 
+	I32 i32_maxidx(const I32PTR  X, const  int N, I32PTR val);
+	I32 i32_minidx(const I32PTR  X, const  int N, I32PTR val);
+
 	void f32_to_strided_f64(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 dstOffset);
+	void f32_to_strided_i64(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 dstOffset);
 	void f32_to_strided_f32(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 dstOffset);
+	void f32_to_strided_i32(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 dstOffset);
+	void f32_to_strided_i16(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 dstOffset);
 
-	void f32_from_strided_f32(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset);
 	void f32_from_strided_f64(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset);
 	void f32_from_strided_i64(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset);
+	void f32_from_strided_f32(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset);
 	void f32_from_strided_i32(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset);
 	void f32_from_strided_i16(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset);
-	void f32_set_nan_by_value(F32PTR a, I32 N, F32 missingValue);
+
+	void f32_to_strided_mem(F32PTR src, VOID_PTR dst, I64 N, I64 stride, I64 dstOffset, DATA_TYPE dtype);
+	void f32_from_strided_mem(F32PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset, DATA_TYPE srcDataType);
+	void arr_from_strided_mem(VOID_PTR dst, VOID_PTR src, int N, int srcStride, int srcOffset, DATA_TYPE srcDstDataType);
+
+	void f32_interp1dvec_cycled_inplace(F32PTR Y, int P, I32PTR goodIndices, int Pgood);
+	void f32_rep_vec1d_upto_inplace(F32PTR Y, int P, int N);
+	void f32_compute_seasonal_avg(F32PTR y, int N, int P, F32PTR mean, I32PTR NumGoodPtsPerTime);
+	void f32_deseasonalize_inplace(F32PTR y, int N, int P,  F32PTR mean_tmp, I32PTR NumGoodPtsPerTime_tmp);
+
+	F32 f32_nansum(F32PTR x, int N) ;
+	F32 f32_nanmean(F32PTR x, int N, int* Ngood);
+	F32 f32_absmax(F32PTR x, int N);
+
+	I64  sub2ind(int* dims, int ndim, int* subs);
+	void ind2sub(int* dims, int ndim, I64 ind, int* subs);
+	int  ndarray_get1d_stride_offset(int* dims, int ndim, int* subs, int whichdim, I64* stride, I64* offset);
+	void f32_get1d_from_ndarray(F32PTR dst, VOID_PTR src, int* dims, int ndim, int* subs, int whichdim, DATA_TYPE srcDtype);
+	void f32_set1d_to_ndarray(F32PTR src, VOID_PTR dst, int* dims, int ndim, int* subs, int whichdim, DATA_TYPE dstDtype);
+	void f32_get2d_from_ndarray(F32PTR dst, VOID_PTR src, int* dims, int ndim, int* subs, int d1, int d2, DATA_TYPE srcDtype);
+	void f32_set2d_from_ndarray(F32PTR src, VOID_PTR dst, int* dims, int ndim, int* subs, int d1, int d2, DATA_TYPE dstDtype);
+
+
+
+	void f32_set_value_to_nan(F32PTR a, I32 N, F32 missingValue);
 	int f32_normalize_multicols_zeroout_nans(F32PTR Y, I32PTR BadRowIndices, I32 ldy, I32 N, I32 q, F32PTR mean, F32PTR sd);
 	extern void f32_transpose_inplace(F32PTR Mat, I32 ROW, I32 COL);
+	extern void i32_transpose_inplace(I32PTR Mat, I32 NROW, I32 NCOL);
+	void i32_transpose_inplace_prev(I32PTR Mat, I32 NROW, I32 NCOL);
+	void i32_transpose_inplace_prev_two_ends(I32PTR Mat, I32 NROW, I32 NCOL);
 	extern void f32_fill_val_matrixdiag(F32PTR mat, const F32 value, I32 N);
 	extern void f32_add_val_matrixdiag(F32PTR mat, const F32 value, I32 N);
 	extern F32 f32_sum_matrixdiag(F32PTR mat, I32 N);
 	extern F32 f32_abs_sum(F32PTR X, I32 N);
 
 	extern void f32_mat_multirows_extract_set_by_scalar(F32PTR X, I32 ROW, I32 COL, F32PTR Xcopy, I32PTR RowIndices, I32 nRows, F32 newValue);
 	extern void f32_mat_multirows_set_by_submat(F32PTR X, I32 ROW, I32 COL, F32PTR Xcopy, I32PTR RowIndices, I32 nRows);
@@ -89,25 +128,18 @@
 	extern I32  f32_find_nans(const F32PTR X, int N, I32PTR index);
 
 	extern void  (*f32_hinge_neg)(const F32PTR X, const F32PTR Y, const F32 knot, const int N);
 	extern void  (*f32_hinge_pos)(const F32PTR X, const F32PTR Y, const F32 knot, const int N);
 	extern void  (*f32_step_neg)(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N);
 	extern void  (*f32_step_pos)(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N);
 	extern void  (*f32_axpy_inplace)(const F32 a, const F32PTR x, F32PTR y, const int N);
-#define f32_copy(src, dst,N)  memcpy(dst,src, sizeof(F32)*N)
-
-
-
-
-
-
-
-
 
 
+   //https://stackoverflow.com/questions/47450718/gcc7-2-argument-range-exceeds-maximum-object-size-9-7-werror-alloc-size-larg
+   #define f32_copy(src, dst,N)  memcpy(dst,src, (U32)sizeof(F32)*(U32)(N))
 
 
 	extern void (*f32_gemm_XtY2x1)(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc);
 	extern void (*f32_gemm_XtY2x2)(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc);
 
 	extern void (*f32_gemm_XY1x2)(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc);
 	extern void (*f32_gemm_XY2x2)(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc);
@@ -117,19 +149,19 @@
 	extern void(*f32_gemv_Xb)(int N, int K, F32PTR X, int lda, F32PTR b, F32PTR C);
 
 	extern I32(*f32_findindex)(F32PTR  x, I32PTR indices, F32 value, int N, CmpFlag flag);
 	extern void  (*f32_scatter_vec_byindex)(F32PTR  x, I32PTR indices, F32PTR values, int N);
 	extern void (*f32_gatherVec_scatterVal_byindex)(F32PTR  x, I32PTR indices, F32PTR values, F32 newValue, int N);
 	extern void (*f32_gather2Vec_scatterVal_byindex)(F32PTR  x, F32PTR  y, I32PTR indices, F32PTR values, F32 newValue, int N);
 	extern void (*f32_scale_inplace)(const F32 gain, const F32 offset, const F32PTR x, const int N);
-	extern void SetupVectorFunction_AVX2();
-	extern void SetupVectorFunction_AVX512();
-	extern void SetupVectorFunction_Generic();
+	extern void SetupVectorFunction_AVX2(void);
+	extern void SetupVectorFunction_AVX512(void);
+	extern void SetupVectorFunction_Generic(void);
 
-	void print_funcs();
+	void print_funcs(void);
 
 	/////////////////////////////////////////
 	// THis is the older header of abc_generic.h, kept here to 
 	// give a quick referene to the conversions between the C and fortran function interfaces
 	////////////////////////////////////////////////
 
 	/*
```

### Comparing `Rbeast-0.1.13/ext_src/abc_vec_avx2.c` & `Rbeast-0.1.14/ext_src/abc_vec_avx2.c`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 #include <stdio.h>
 #include <string.h>
 
 #include "abc_000_macro.h"
 #include "abc_000_warning.h"
 #include "abc_vec.h"
 
+#define STATIC static
+
 #if defined (WIN64_OS) || defined(WIN32_OS)
     #include <malloc.h> //alloca
 #else
     #include <alloca.h> //alloca
 #endif
 
 
@@ -142,57 +144,55 @@
     __m256i nvec    = set1_i32(n);
     __m256i maskmov = _mm256_cmpgt_epi32(nvec, maskNum);
     //__m256i maskmov = _mm256_sub_epi32(maskNum, nvec);    
     return maskmov;
 }
 
 static U64   masktemplate[8];
-static void  FillMaskTempalte( ) {
+static void  FillMaskTempalte(void) {
     for (int i=0; i<8;i++)     masktemplate[i] = (1ULL << (i * 8)) - 1;
     //{0x00|FF, 0x|FF|FF,0x|FF|FF|FF....}    
 }
+
 static INLINE __m256i GetMoveMask1(int n) {
     __m128i maskIdx = _mm_cvtsi64_si128(masktemplate[n]);
     __m256i mask    = _mm256_cvtepi8_epi32(maskIdx);
     return  mask;
 }
 
 #else
 
 static U64   masktemplate[8];
-static void  FillMaskTempalte( ) {
+static void  FillMaskTempalte(void) {
     for (int i=0; i<8;i++)     masktemplate[i] = (1ULL << (i * 8)) - 1;
     //{0x00|FF, 0x|FF|FF,0x|FF|FF|FF....}
 }
 
 #define GetMoveMask(n) ({__m128i maskIdx = _mm_cvtsi64_si128(masktemplate[n]); __m256i mask    = _mm256_cvtepi8_epi32(maskIdx); mask;})
 
 #endif
 //https://stackoverflow.com/questions/6996764/fastest-way-to-do-horizontal-sse-vector-sum-or-other-reduction
 //https://stackoverflow.com/questions/4120681/how-to-calculate-single-vector-dot-product-using-sse-intrinsic-functions-in-c/4121295#4121295
 
 
 // _mm512_reduce_add_ps: no a single instrution but an emulated sequence of instruction
 //https://stackoverflow.com/questions/26896432/horizontal-add-with-m512-avx512
 //https://stackoverflow.com/questions/55296777/summing-8-bit-integers-in-m512i-with-avx-intrinsics
-static INLINE F32  __attribute__((always_inline))  f32_hsum_slow(__m256 r)
-{   ///horizontal summing
-
- 
+static INLINE F32  __attribute__((always_inline))  f32_hsum_slow(__m256 r) { 
+    ///horizontal summing 
     //https://stackoverflow.com/questions/6996764/fastest-way-to-do-horizontal-sse-vector-sum-or-other-reduction   
     __m128 vlow  = _mm256_castps256_ps128(r);
     __m128 vhigh = _mm256_extractf128_ps(r, 1); // high 128
     __m128 v128  = _mm_add_ps(vlow, vhigh);     // add the low 128
                                                //float hsum_ps_sse3(__m128 v) {
     __m128 sums = _mm_hadd_ps(v128, v128);
     sums = _mm_hadd_ps(sums, sums);
     F32 sum = _mm_cvtss_f32(sums);    
     return sum;
 }
-
  
 static INLINE F32  __attribute__((always_inline)) f32_hsum ( __m256 r) {
     //https://stackoverflow.com/questions/6996764/fastest-way-to-do-horizontal-sse-vector-sum-or-other-reduction   
     __m128 vlow  = _mm256_castps256_ps128(r);
     __m128 vhigh = _mm256_extractf128_ps(r, 1); // high 128
     __m128 v128  = _mm_add_ps(vlow, vhigh);     // add the low 128
 
@@ -200,14 +200,15 @@
     __m128 shuf = _mm_movehdup_ps(v128);        // broadcast elements 3,1 to 2,0
     __m128 sums = _mm_add_ps(v128, shuf);
     shuf = _mm_movehl_ps(shuf, sums); // high half -> low half
     sums = _mm_add_ss(sums, shuf);
     F32 sum = _mm_cvtss_f32(sums);
     return sum;
 }
+
 static INLINE I32  __attribute__((always_inline)) i32_hsum(__m256i r)   {
     //https://stackoverflow.com/questions/6996764/fastest-way-to-do-horizontal-sse-vector-sum-or-other-reduction   
 
     __m128i vlow  = _mm256_castsi256_si128(r);
     __m128i vhigh = _mm256_extracti128_si256(r, 1); // high 128
     __m128i v128  = _mm_add_epi32(vlow, vhigh);     // add the low 128
 
@@ -233,30 +234,31 @@
         store(dst + i, load(src + i));
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), load(src + i));
     _mm256_zeroupper();
 }
 */
- void avx2_i32_add_val_inplace (const int c, const I32PTR x, const int N) {
+STATIC void avx2_i32_add_val_inplace (const int c, const I32PTR x, const int N) {
     __m256i  C = set1_i32(c);
     int i = 0;
     for (; i < N - (NF4-1); i += NF4) 
         storei(x + i,       addi32(loadi(x + i),       C) ),
         storei(x + i + NF,  addi32(loadi(x + i + NF),  C) ),
         storei(x + i + NF2, addi32(loadi(x + i + NF2), C) ),
         storei(x + i + NF3, addi32(loadi(x + i + NF3), C) );
     for (; i < N - (NF-1); i += NF)  
         storei(x + i, addi32(loadi(x + i), C) );
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstorei(x + i,  GetMoveMask(n),  addi32(loadi(x + i), C)  );
     _mm256_zeroupper();    
 }
-I32  avx2_i32_sum(const I32PTR x, const int N) {
+
+STATIC I32  avx2_i32_sum(const I32PTR x, const int N) {
     __m256i  S = set0i();
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256i s12   = addi32(loadi(x + i),        loadi(x + i + NF));
         __m256i s34   = addi32(loadi(x + i + NF2),  loadi(x + i + NF3));
          S = addi32(S, addi32(s12, s34));
     }
@@ -266,15 +268,16 @@
     if (n > 0) 
         S= addi32( S,  maskloadi(x + i, GetMoveMask(n) ) );
 
     I32 sum = i32_hsum(S);
      _mm256_zeroupper();
      return sum;
 }
-F32  avx2_f32_sum(const F32PTR x, const int N) {
+
+STATIC F32  avx2_f32_sum(const F32PTR x, const int N) {
     __m256  S = set0();
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 s12      = add(load(x + i),        load(x + i + NF) );
         __m256 s34      = add(load(x + i + NF2),  load(x + i + NF3));        
          S = add(S, add(s12, s34));
     }
@@ -282,15 +285,16 @@
     int n = N - i;
     if (n > 0)        S = add( S,  maskload(x + i, GetMoveMask(n) ) );
     F32 sum = f32_hsum(S);
      _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
      return sum;
 }
-void avx2_f32_fill_val(const F32 c, F32PTR x, int N) {    
+
+STATIC void avx2_f32_fill_val(const F32 c, F32PTR x, int N) {
     __m256  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store((x + i),    C);
         store((x + i+NF),  C);
         store((x + i+NF2), C);
         store((x + i+NF3), C);
@@ -299,15 +303,16 @@
         store((x+i), C);
     int n = N - i;
     if (n > 0) 
         maskstore(x + i, GetMoveMask(n), C);    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx2_f32_add_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
+
+STATIC void avx2_f32_add_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       //dst=dst-src
         store(dst + i,       add(load(src2 + i),     load(src1 + i)));
         store(dst + i + NF,   add(load(src2 + i + NF), load(src1 + i  + NF)));
         store(dst + i + NF2,  add(load(src2 + i + NF2), load(src1 + i + NF2)));
         store(dst + i + NF3,  add(load(src2 + i + NF3), load(src1 + i + NF3)));
     }
@@ -315,15 +320,16 @@
         store(dst + i,     add(load(src2 + i), load(src1 + i))  );    
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), add(load(src2 + i), load(src1 + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx2_f32_sub_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
+
+STATIC void avx2_f32_sub_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
     //dst=src2-src1
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       //dst=dst-src
         store(dst + i,       sub(load(src2 + i), load(src1 + i)));
         store(dst + i + NF,  sub(load(src2 + i + NF), load(src1 + i + NF)));
         store(dst + i + NF2, sub(load(src2 + i + NF2), load(src1 + i + NF2)));
         store(dst + i + NF3, sub(load(src2 + i + NF3), load(src1 + i + NF3)));
@@ -332,15 +338,16 @@
         store(dst + i, sub( load(src2 + i), load(src1 + i))  ); 
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), sub(load(src2 + i), load(src1 + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx2_f32_add_vec_inplace(const F32PTR src, const F32PTR dst, const int N) {
+
+STATIC void avx2_f32_add_vec_inplace(const F32PTR src, const F32PTR dst, const int N) {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(dst + i,           add(load(dst + i),       load(src + i)));
         store(dst + i + NF,      add(load(dst + i + NF),  load(src + i + NF)));
         store(dst + i + NF2,     add(load(dst + i + NF2), load(src + i + NF2)));
         store(dst + i + NF3,     add(load(dst + i + NF3), load(src + i + NF3)));
     }
@@ -349,15 +356,16 @@
     }
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), add(load(dst + i), load(src + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx2_f32_sub_vec_inplace(const F32PTR src, F32PTR dst, int N) {
+
+STATIC void avx2_f32_sub_vec_inplace(const F32PTR src, F32PTR dst, int N) {
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       //dst=dst-src
         store(dst + i,        sub(load(dst + i),      load(src + i)));
         store(dst + i + NF,   sub(load(dst + i + NF),  load(src + i + NF)));
         store(dst + i + NF2,  sub(load(dst + i + NF2), load(src + i + NF2)));
         store(dst + i + NF3,  sub(load(dst + i + NF3), load(src + i + NF3)));
     }
@@ -366,15 +374,16 @@
     }
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), sub(load(dst + i), load(src + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx2_f32_add_val_inplace(const F32 c, const F32PTR x, const int N) {
+
+STATIC void avx2_f32_add_val_inplace(const F32 c, const F32PTR x, const int N) {
     __m256  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) 
         store(x + i,          add(load( x + i),     C)   ),
         store(x + i + NF,     add(load(x + i + NF),  C) ),
         store(x + i + NF2,    add(load(x + i + NF2), C) ),
         store(x + i + NF3,    add(load(x + i + NF3), C) );
@@ -382,15 +391,16 @@
         store(x + i, add(load(x + i), C) );
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i,  GetMoveMask(n), add(load(x + i), C)  );
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
-void avx2_f32_subrev_val_inplace(const F32 c, const F32PTR x, const int N) {
+
+STATIC void avx2_f32_subrev_val_inplace(const F32 c, const F32PTR x, const int N) {
     __m256  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) 
         store(x + i,      sub(C, load( x + i))   ),
         store(x + i + NF,  sub(C, load(x + i + NF)) ),
         store(x + i + NF2, sub(C, load(x + i + NF2)) ),
         store(x + i + NF3, sub(C, load(x + i + NF3)) );
@@ -399,15 +409,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i,  GetMoveMask(n), sub(C, load(x + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
 
-void avx2_f32_mul_val_inplace(const F32 c, const F32PTR x, const int N) {
+STATIC void avx2_f32_mul_val_inplace(const F32 c, const F32PTR x, const int N) {
     __m256  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4)
         store(x + i,      mul(load(x + i), C)),
         store(x + i + NF, mul(load(x + i + NF), C)),
         store(x + i + NF2, mul(load(x + i + NF2), C)),
         store(x + i + NF3, mul(load(x + i + NF3), C));
@@ -415,15 +425,16 @@
         store(x + i, mul(load(x + i), C));
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i, GetMoveMask(n), mul(load(x + i), C));
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
-void avx2_f32_mul_vec_inplace(const F32PTR src, F32PTR dst, int N) {
+
+STATIC void avx2_f32_mul_vec_inplace(const F32PTR src, F32PTR dst, int N) {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(dst + i,       mul(load(dst + i),      load(src + i)));
         store(dst + i + NF,   mul(load(dst + i + NF),  load(src + i + NF)));
         store(dst + i + NF2,  mul(load(dst + i + NF2), load(src + i + NF2)));
         store(dst + i + NF3,  mul(load(dst + i + NF3), load(src + i + NF3)));
     }
@@ -433,15 +444,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), mul(load(dst + i), load(src + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
 
-void avx2_f32_mul_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
+STATIC void avx2_f32_mul_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       
         store(dst + i,       mul(load(src2 + i),      load(src1 + i)));
         store(dst + i + NF,  mul(load(src2 + i + NF),  load(src1 + i + NF)));
         store(dst + i + NF2,  mul(load(src2 + i + NF2), load(src1 + i + NF2)));
         store(dst + i + NF3,  mul(load(src2 + i + NF3), load(src1 + i + NF3)));
     }
@@ -451,15 +462,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), mul(load(src2 + i), load(src1 + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
 
-void avx2_f32_add_v_v2_vec_inplace(const F32PTR src, const F32PTR  v, const F32PTR  v2, int N) {
+STATIC void avx2_f32_add_v_v2_vec_inplace(const F32PTR src, const F32PTR  v, const F32PTR  v2, int N) {
 
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(v + i,  add(load(v + i), load(src + i)));
         store(v2 + i, add(load(v2 + i), mul(load(src + i), load(src + i))));
 
         store(v + i+NF,  add(load(v + i + NF),  load(src + i + NF)));
@@ -483,15 +494,16 @@
         maskstore(v + i, mask, add(    load(v + i),   load(src + i)  )                           );
         maskstore(v2 + i, mask, add(   load(v2 + i), mul(load(src + i), load(src + i)))     );
     }
     _mm256_zeroupper();
 
  
 }
-F32 avx2_f32_dot(F32PTR  x, F32PTR y, int N) {
+
+STATIC F32 avx2_f32_dot(F32PTR  x, F32PTR y, int N) {
 
     __m256 r = set0();    
     int i = 0;    
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 r0 = mul(load(x + i),     load(y + i)) ;
         __m256 r1 = mul(load(x + i+NF),   load(y + i+ NF));
         __m256 r2 = mul(load(x + i+ NF2),  load(y + i + NF2));
@@ -508,15 +520,16 @@
         __m256i mask = GetMoveMask(n);
         r = add(r,  mul(   maskload(x + i, mask), maskload(y + i, mask)   )   );
     }    
     F32 sum = f32_hsum(r);
      _mm256_zeroupper();    
     return sum;
 }
-F32 avx2_f32_dot2x1(F32PTR  x, F32PTR y, F32PTR v, int N, F32PTR res) {
+
+STATIC F32 avx2_f32_dot2x1(F32PTR  x, F32PTR y, F32PTR v, int N, F32PTR res) {
     __m256 RX = set0();
     __m256 RY = set0();
     int i = 0;    
     for (; i < N - (NF2-1); i += NF2) {
         __m256 x0 = mul(load(x + i),      load(v + i)) ;
         __m256 x1 = mul(load(x + i+NF),   load(v + i+ NF));
         __m256 y0 = mul(load(y + i),      load(v + i)) ;
@@ -542,15 +555,16 @@
     float sumY = f32_hsum(RY);
    
      _mm256_zeroupper();
     //for (; i < N; i++)     sum+=x[i] *y[i];
     res[0] = sumX;
     return sumY;
 }
-void avx2_f32_dot2x2(F32PTR  x, F32PTR y, F32PTR v, F32PTR w, int N, F32PTR res1, F32PTR res2) {
+
+STATIC void avx2_f32_dot2x2(F32PTR  x, F32PTR y, F32PTR v, F32PTR w, int N, F32PTR res1, F32PTR res2) {
     __m256 RX1 = set0();
     __m256 RX2 = set0();
     __m256 RY1 = set0();
     __m256 RY2 = set0();
     int i = 0;    
     
     for (; i  < N - (NF2-1); i += NF2) {
@@ -601,15 +615,16 @@
     //for (; i < N; i++)     sum+=x[i] *y[i];
     res1[0] = sumX1;
     res1[1] = sumY1;
     res2[0] = sumX2;
     res2[1] = sumY2;
     return;
 }
-F32 avx2_fma_f32_dot(F32PTR  x, F32PTR y, int N) {
+
+STATIC F32 avx2_fma_f32_dot(F32PTR  x, F32PTR y, int N) {
 
     __m256 r0 = set0();
     __m256 r1 = set0();
     __m256 r2 = set0();
     __m256 r3 = set0();
     
     int i = 0;    
@@ -633,15 +648,15 @@
      _mm256_zeroupper();
     return sum;
 }
 
 //https://stackoverflow.com/questions/1528727/why-is-sse-scalar-sqrtx-slower-than-rsqrtx-x
 //https://stackoverflow.com/questions/54642663/how-sqrt-of-gcc-works-after-compiled-which-method-of-root-is-used-newton-rap
 //https://stackoverflow.com/questions/31555260/fast-vectorized-rsqrt-and-reciprocal-with-sse-avx-depending-on-precision
-void avx2_f32_sqrt_vec_inplace(const F32PTR x, const int N)
+STATIC void avx2_f32_sqrt_vec_inplace(const F32PTR x, const int N)
 {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 r1 = load(x + i);          store(x + i,      _mm256_sqrt_ps(r1)  );
         __m256 r2 = load(x + i+NF);       store(x + i+ NF,  _mm256_sqrt_ps(r2) );
         __m256 r3 = load(x + i + NF2);    store(x + i+ NF2, _mm256_sqrt_ps(r3) );
         __m256 r4 = load(x + i + NF3);    store(x + i+ NF3, _mm256_sqrt_ps(r4) );
@@ -654,15 +669,16 @@
     if (n > 0) {
         __m256 r = load(x + i);
         maskstore(x + i, GetMoveMask(n), _mm256_sqrt_ps(r) );
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx2_f32_sqrt_vec(const F32PTR x, const F32PTR y, const int N)
+
+STATIC void avx2_f32_sqrt_vec(const F32PTR x, const F32PTR y, const int N)
 {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 r1 = load(x + i);          store(y + i,      _mm256_sqrt_ps(r1)  );
         __m256 r2 = load(x + i+NF);       store(y + i+ NF,  _mm256_sqrt_ps(r2) );
         __m256 r3 = load(x + i + NF2);    store(y + i+ NF2, _mm256_sqrt_ps(r3) );
         __m256 r4 = load(x + i + NF3);    store(y + i+ NF3, _mm256_sqrt_ps(r4) );     
@@ -677,15 +693,15 @@
         maskstore(y + i, GetMoveMask(n), _mm256_sqrt_ps(r) );
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
 
 #ifdef MSVC_COMPILER
-void avx2_f32_sin_vec_inplace_MSVC(const F32PTR x, const int N)
+STATIC void avx2_f32_sin_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m256 r = load(x + i);    store(x + i,   _mm256_sin_ps(r));
@@ -693,15 +709,16 @@
     int n = N - i;
     if (n > 0) {
         __m256 r = load(x + i);    maskstore(x + i, GetMoveMask(n), _mm256_sin_ps(r) );
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx2_f32_cos_vec_inplace_MSVC(const F32PTR x, const int N)
+
+STATIC void avx2_f32_cos_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m256 r = load(x + i);    store(x + i,   _mm256_cos_ps(r));
@@ -709,15 +726,16 @@
     int n = N - i;
     if (n > 0) {
         __m256 r = load(x + i);    maskstore(x + i, GetMoveMask(n), _mm256_cos_ps(r) );
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx2_f32_sincos_vec_inplace_MSVC(const F32PTR in_outsin, F32PTR outcos, const int N)
+
+STATIC void avx2_f32_sincos_vec_inplace_MSVC(const F32PTR in_outsin, F32PTR outcos, const int N)
 {
 //Compute the sine and cosine of packed single-precision (32-bit) floating-point elements in a expressed in radians,
 //store the sine in dst, and store the cosine into memory at mem_addr.
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m256 r = load(in_outsin + i);
         store(in_outsin + i, _mm256_sincos_ps(outcos+i,r));
@@ -729,15 +747,16 @@
         __m256  r = load(in_outsin + i);   
         maskstore(in_outsin + i, mask, _mm256_sincos_ps(&tmpcos, r) );
         maskstore(outcos  + i,   mask, tmpcos);
     }
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx2_f32_pow_vec_inplace_MSVC(F32PTR x, F32 pow, int N)
+
+STATIC void avx2_f32_pow_vec_inplace_MSVC(F32PTR x, F32 pow, int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     
     __m256 C = set1(pow);
 
@@ -748,15 +767,16 @@
     int n = N - i;
     if (n > 0) {
         __m256 r = load(x + i);  maskstore(x + i, GetMoveMask(n), _mm256_pow_ps(r, C));
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx2_f32_log_vec_inplace_MSVC(const F32PTR x, const int N)
+
+STATIC void avx2_f32_log_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m256 r = load(x + i);    store(x + i, _mm256_log_ps(r));
@@ -764,15 +784,16 @@
     int n = N - i;
     if (n > 0) {
         __m256 r = load(x + i);    maskstore(x + i, GetMoveMask(n), _mm256_log_ps(r));
     }
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx2_f32_exp_vec_inplace_MSVC(const F32PTR x, const int N)
+
+STATIC void avx2_f32_exp_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m256 r = load(x + i);    store(x + i, _mm256_exp_ps(r));
@@ -782,41 +803,43 @@
         __m256 r = load(x + i);    maskstore(x + i, GetMoveMask(n), _mm256_exp_ps(r));
     }
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
 #endif
 
-void avx2_f32_sin_vec_inplace(const F32PTR x, const int N)
+STATIC void avx2_f32_sin_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i,  sin256_ps(x + i) );    
     int n = N - i;
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), sin256_ps(x + i) );    
     _mm256_zeroupper();    
 }
-void avx2_f32_cos_vec_inplace(const F32PTR x, const int N)
+
+STATIC void avx2_f32_cos_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
      int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i, cos256_ps(x + i));    
     int n = N - i;
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), cos256_ps(x + i) );    
     _mm256_zeroupper();    
 }
-void avx2_f32_sincos_vec_inplace(const F32PTR in_outsin, F32PTR outcos, const int N) 
+
+STATIC void avx2_f32_sincos_vec_inplace(const F32PTR in_outsin, F32PTR outcos, const int N)
 {
 //Compute the sine and cosine of packed single-precision (32-bit) floating-point elements in a expressed in radians,
 //store the sine in dst, and store the cosine into memory at mem_addr.
     int i = 0;
     for (; i < N - (NF - 1); i += NF) 
         sincos256_ps(in_outsin + i, in_outsin + i, outcos + i);    
     int n = N - i;
@@ -848,16 +871,16 @@
         npositive = npositive >> 1;
     }
     if (n < 0) {
         res = _mm256_rcp_ps(res);
     }
     return res;
 }
-void avx2_f32_pow_vec_inplace(F32PTR x, F32 pow, int N)
-{
+
+STATIC void avx2_f32_pow_vec_inplace(F32PTR x, F32 pow, int N) {
          int   nInteger   = pow;
         float  nRemainder = pow - nInteger;
 
         if (nRemainder != 0) {
             int i = 0;
             for (; i < N - (NF - 1); i += NF) {
                 store(x + i, pow256(x+i, pow ) );
@@ -873,44 +896,44 @@
             }
             int n = N - i;
             if (n > 0)
                 maskstore(x + i, GetMoveMask(n), pow256_int(load(x + i), nInteger));         
         }
         _mm256_zeroupper();
 }
-void avx2_f32_log_vec_inplace(const F32PTR x, const int N)
+
+STATIC void avx2_f32_log_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
      int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i, log256_ps(x + i) );    
     int n = N - i;
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), log256_ps(x + i) );    
     _mm256_zeroupper();    
 }
-void avx2_f32_exp_vec_inplace(const F32PTR x, const int N)
+
+STATIC void avx2_f32_exp_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
      int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i, exp256_ps(x + i) );    
     int n = N - i;
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), exp256_ps(x + i) );
     _mm256_zeroupper();    
 }
 
-
-
-void  avx2_f32_avgstd(const F32PTR x, int N, F32PTR avg, F32PTR std) {
+STATIC void  avx2_f32_avgstd(const F32PTR x, int N, F32PTR avg, F32PTR std) {
     __m256  S    = set0();
     __m256  SS   = set0();
     int i = 0;
     for (; i < N - 15; i += 16) {
         __m256 s1  =  load(x + i);
         __m256 s2  =  load(x + i+8);
 
@@ -938,15 +961,16 @@
     F32 sumxx = f32_hsum(SS);
      _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
      F64 AVG = sumx / N;
      std[0] = sqrtf((sumxx - AVG * sumx) / (N - 1));// sqrtf((sumxx - AVG * AVG * N) / (N - 1));
      avg[0] =AVG;
 }
-void avx2_f32_sx_sxx_to_avgstd_inplace(F32PTR SX, F32PTR SXX, I32 Nsample, F32 scale, F32 offset, int N) {
+
+STATIC void avx2_f32_sx_sxx_to_avgstd_inplace(F32PTR SX, F32PTR SXX, I32 Nsample, F32 scale, F32 offset, int N) {
     /*
                    r_ippsMulC_32f_I(inv_sample* sd, resultChain.tY, N);
                    r_ippsMul_32f(resultChain.tY, resultChain.tY, MEMBUF1, N);
                    r_ippsMulC_32f_I(inv_sample* sd* sd, resultChain.tSD, N);
                    r_ippsSub_32f_I(MEMBUF1, resultChain.tSD, N);
                    r_ippsSqrt_32f_I(resultChain.tSD, N);
     */
@@ -986,15 +1010,15 @@
 }
 
 
 #ifdef WIN64_OS 
     #define WIN32_LEAN_AND_MEAN
     #include "windows.h"
 
-I32 avx2_f32_maxidx1(const F32PTR x, const int N, F32PTR val) {
+STATIC I32 avx2_f32_maxidx1(const F32PTR x, const int N, F32PTR val) {
 //https://stackoverflow.com/questions/23590610/find-index-of-maximum-element-in-x86-simd-vector    
     if (N < 8) {        
         int maxIdx = 0;
         F32 maxVal = x[0];        
         for (int i=1; i < N; i++) {
             if (maxVal < x[i])  maxVal = x[i], maxIdx = i;            
         }
@@ -1056,15 +1080,15 @@
     _mm256_store_si256(&ID.dummy, maxIdx);
     _mm256_zeroupper();     
     val[0] = max;
     return ID.idx[index>>2] ;
 }
 #endif
 
-I32 avx2_f32_maxidx(const F32PTR x, const int N, F32PTR val) {
+STATIC I32 avx2_f32_maxidx(const F32PTR x, const int N, F32PTR val) {
        
     __m128i _maskIdx    = _mm_cvtsi64_si128(0x0706050403020100);
     __m256i idx         = _mm256_cvtepu8_epi32(_maskIdx);
     __m256i EIGHT       = set1_i32(8);
 
     __m256  maxVec = set1(x[0]);
     __m256i maxIdx = set0i();
@@ -1092,15 +1116,15 @@
     }
     __m128 vlow     = _mm256_castps256_ps128(maxVec);
     __m128 vhigh    = _mm256_extractf128_ps(maxVec, 1); // high 128
     __m128i idxlow = _mm256_castsi256_si128(maxIdx);
     __m128i idxhigh = _mm256_extracti128_si256(maxIdx, 1); // high 128
 
     __m128 cmpmask  = _mm_cmp_ps(vlow, vhigh, _CMP_LE_OQ);  
-    __m128 max128 = _mm_blendv_ps(vlow, vhigh, cmpmask); //o: take a, 1: take from vec     
+    __m128 max128   = _mm_blendv_ps(vlow, vhigh, cmpmask); //o: take a, 1: take from vec     
     __m128i idx128  = _mm_blendv_epi8(idxlow, idxhigh, _mm_castps_si128(cmpmask)); //o: take a, 1: take from vec     
 
      F32 VAL[4];
      union {
         I32 idx[4];
         __m128i dummy;
      }ID;
@@ -1111,15 +1135,16 @@
      I32 i2 = VAL[2] > VAL[3] ? 2 : 3;
      I32 IDX = VAL[i1] > VAL[i2] ? i1 : i2;
 
      val[0] = VAL[IDX];
     //for (; i < N; i++)     sum+=x[i] *y[i];
     return ID.idx[IDX];
 }
-I32 avx2_f32_minidx(const F32PTR x, const int N, F32PTR val) {
+
+STATIC I32 avx2_f32_minidx(const F32PTR x, const int N, F32PTR val) {
     
     __m128i _maskIdx    = _mm_cvtsi64_si128(0x0706050403020100);
     __m256i idx         = _mm256_cvtepu8_epi32(_maskIdx);
     __m256i EIGHT       = set1_i32(8);
 
     __m256   minVec = set1(x[0]);
     __m256i  minIdx = set0i();
@@ -1171,15 +1196,15 @@
      I32 IDX = VAL[i1] < VAL[i2] ? i1 : i2;
 
      val[0] = VAL[IDX];
     //for (; i < N; i++)     sum+=x[i] *y[i];
     return ID.idx[IDX];
 }
 
-void avx2_f32_diff_back(const F32PTR  x, F32PTR result, const int N) {
+STATIC void avx2_f32_diff_back(const F32PTR  x, F32PTR result, const int N) {
     //skip the first elements because evaluation of diff0-x[0]-x[-1] needs an nonexistent element at -1
     //res[i]=x[i]-x[i-1]
 
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(result + i,        sub(load(x + i),         load(x + i-1)));
         store(result + i + NF,   sub(load(x + i + NF),    load(x + i + NF-1)));
@@ -1194,15 +1219,16 @@
         maskstore(result + i, GetMoveMask(n), sub(load(x + i), load(x + i-1))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 
     result[0] = result[1];
 
 }
-void avx2_f32_seq(F32PTR p, F32 x0, F32 dX, int N) {
+
+STATIC void avx2_f32_seq(F32PTR p, F32 x0, F32 dX, int N) {
    
     __m256 X;
     {    
         __m128i tmp     = _mm_cvtsi64_si128(0x0706050403020100);
         __m256i tmp256  = _mm256_cvtepu8_epi32(tmp);
         __m256  v1to7   = _mm256_cvtepi32_ps(tmp256);        
         __m256  DX      = mul(v1to7, set1(dX));
@@ -1218,15 +1244,15 @@
     int n = N - i;
     if (n > 0) {
         maskstore(p + i, GetMoveMask(n), X);
     }     
     _mm256_zeroupper();    
 }
 
-void avx2_i32_seq(I32PTR p, I32 x0, I32 dX, int N) {
+STATIC void avx2_i32_seq(I32PTR p, I32 x0, I32 dX, int N) {
 
     __m256i X;
     {
         __m128i tmp    = _mm_cvtsi64_si128(0x0706050403020100);
         __m256i v1to7  = _mm256_cvtepu8_epi32(tmp);
         //__m256  v1to7  = _mm256_cvtepi32_ps(tmp256);
         __m256i  DX     = _mm256_mullo_epi32(v1to7, set1_i32(dX)); //https://stackoverflow.com/questions/28479429/multiply-two-vectors-of-32bit-integers-producing-a-vector-of-32bit-result-eleme
@@ -1242,15 +1268,15 @@
     int n = N - i;
     if (n > 0) {
         maskstorei(p + i, GetMoveMask(n), X);
     }
     _mm256_zeroupper();
 }
 
-void avx2_f32_to_f64_inplace(F32PTR data32, int N) {
+STATIC void avx2_f32_to_f64_inplace(F32PTR data32, int N) {
 
     F64PTR data64 = data32;
     int i = N - 8;
     for (; i >= 0; i -= 8) {
         __m256 r = load(data32 + i);
         __m128 lowps    = _mm256_castps256_ps128(r);
         __m128 highps   = _mm256_extractf128_ps(r, 1);         // high 128
@@ -1263,15 +1289,16 @@
         __m128 r = _mm_loadu_ps(data32 + i);        
         _mm256_storeu_pd(data64 + i, _mm256_cvtps_pd(r));
     }
     i = i - 1;
     for (; i >= 0; --i)   data64[i] = data32[i];    
     _mm256_zeroupper();    
 }
-void avx2_f64_to_f32_inplace(F64PTR data64, int N) {
+
+STATIC void avx2_f64_to_f32_inplace(F64PTR data64, int N) {
 
     F32PTR data32 = data64;
     int i = 0;
     for (; i < N-7; i += 8) {    
         __m128  R1 = _mm256_cvtpd_ps(_mm256_loadu_pd(data64 + i));
         __m128  R2 = _mm256_cvtpd_ps(_mm256_loadu_pd(data64 + i + 4));
         _mm_storeu_ps(data32 + i,   R1);
@@ -1281,15 +1308,16 @@
         __m128  R1 = _mm256_cvtpd_ps(_mm256_loadu_pd(data64 + i));
         _mm_storeu_ps(data32 + i, R1);
     }    
     _mm256_zeroupper();
 
     for (; i <N; ++i)      data32[i] = data64[i];         
 }
-void avx2_i32_to_f32_scaleby_inplace(I32PTR x, int N, F32 scale) {
+
+STATIC void avx2_i32_to_f32_scaleby_inplace(I32PTR x, int N, F32 scale) {
     __m256  C = set1(scale);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4)
         store(x + i,      mul(_mm256_cvtepi32_ps(loadi(x + i)), C)),
         store(x + i + NF, mul(_mm256_cvtepi32_ps(loadi(x + i+NF)), C)),
         store(x + i + NF2, mul(_mm256_cvtepi32_ps(loadi(x + i+ NF2)), C)),
         store(x + i + NF3, mul(_mm256_cvtepi32_ps(loadi(x + i+ NF3)), C));
@@ -1298,15 +1326,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i, GetMoveMask(n), mul(_mm256_cvtepi32_ps(loadi(x + i)), C));
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
 
-void avx2_i32_increment_bycond_inplace(I32PTR x,  F32PTR cond, int N) {
+STATIC void avx2_i32_increment_bycond_inplace(I32PTR x,  F32PTR cond, int N) {
     __m256   C0 = set0();
     __m256i  C1 = set1_i32(1);
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {            
         __m256i mask = _mm256_castps_si256(  _mm256_cmp_ps( load(cond+i), C0, _CMP_GT_OQ) );
         __m256i vec = maskloadi(x + i, mask);
         vec = addi32(vec, C1);
@@ -1321,15 +1349,16 @@
         __m256i vec = maskloadi(x + i, mask);
         vec = addi32(vec, C1);
         maskstorei(x + i, mask, vec);
 
     }
     _mm256_zeroupper();
 }
-void avx2_i32_increment_vec2_bycond_inplace(I32PTR x, I32PTR y, F32PTR cond, int N) {
+
+STATIC void avx2_i32_increment_vec2_bycond_inplace(I32PTR x, I32PTR y, F32PTR cond, int N) {
     __m256   C0       = set0();
     __m256   Ceplison1 = set1(1e-10);
     __m256   Ceplison2 = set1(-1e-10);
     __m256i  C1       = set1_i32(1);
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {         
         __m256  data  = load(cond + i);
@@ -1356,15 +1385,16 @@
         mask2 = _mm256_and_si256(mask2, loadmask);
         __m256i vec2 = maskloadi(y + i, mask2);
         vec2 = addi32(vec2, C1);     maskstorei(y + i, mask2, vec2);        
 
     }
     _mm256_zeroupper();
 }
-I32  avx2_i08_sum_binvec(U08PTR binvec, I32 N) {
+
+STATIC I32  avx2_i08_sum_binvec(U08PTR binvec, I32 N) {
     //stackoverflow.com/questions/36998538/fastest-way-to-horizontally-sum-sse-unsigned-byte-vector
 	I32   SUM = 0;
 	I32	  i   = 0;
 	//|8bytees|8bytees|8bytees|8bytees|
     __m256i r   = set0i();
     I32  ite_read_for_sad = 0;
 	for (; i < N - (32*4-1); i+=32*4) {
@@ -1427,15 +1457,15 @@
 * > C : = alpha * op(A) * op(B) + beta * C,
 * > where  op(X) is one of
 * > op(X) = X or op(X) = X * *T,
 * > alpha and beta are scalars, and A, Band C are matrices, with op(A)
 * > an m by k matrix, op(B)  a  k by n matrixand C an m by n matrix.
 */
 
-void avx2_f32_gemm_XtY2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
+STATIC void avx2_f32_gemm_XtY2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
 { 
 	for (int col = 0; col < N; ++col) {
 		int row = 0;
 		for (; row < M - (2 - 1); row += 2) 
             C[row + 1] = avx2_f32_dot2x1(A + row * lda, A + (row + 1) * lda, B, K, C + row);
 			//f32_dot3x1(A + ROW * lda, A + (ROW + 1) * lda, A + (ROW + 2) * lda, B, K, C + ROW);			
 			//C[row] = f32_dot(A + row * lda, B, K);		
@@ -1443,15 +1473,15 @@
 			C[row] = avx2_f32_dot(A + row * lda, B, K);
 		B += ldb;
 		C += ldc;
 	}
  
 }
  
-void avx2_f32_gemm_XtY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void avx2_f32_gemm_XtY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 {
 	int COL;
  	for (COL = 0; COL < N-(2-1); COL+=2) {
 		int ROW;
 		for (ROW=0; ROW < M-(2-1); ROW+=2) {			
             avx2_f32_dot2x2(A+ROW*lda, A + (ROW+1)*lda, B, B+ldb, K, C+ROW, C +ldc+ROW);
 		}
@@ -1548,15 +1578,15 @@
             *(Crow + ldc * col) = avx2_f32_dot(B + col * ldb, Xrow, K);
         }
 
     }
 
 }
 */
-void avx2_f32_gemm_XY1x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
+STATIC void avx2_f32_gemm_XY1x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
 {
     // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
     // MSVC seems not to support it
 
     /*
     https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
     Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
@@ -1576,15 +1606,15 @@
         for (; col < N - 1; col += 2) 
             *(Crow + ldc * (col+1))=avx2_f32_dot2x1(B+col*ldb,B+col*ldb+ldb,Xrow,K, Crow+ldc*col);        
         if (col < N) 
             *(Crow+ldc*col)=avx2_f32_dot(B + col * ldb, Xrow, K);
     }  
 
 }
-void avx2_f32_gemm_XY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void avx2_f32_gemm_XY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 { // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
   // MSVC seems not to support it
   //    https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
   //   Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
    
     F32     XROW_FIXEXD[4096];
     F32PTR  Xrow = (2*K <= 4096) ? XROW_FIXEXD : alloca(2*K * sizeof(F32));
@@ -1614,15 +1644,15 @@
         for (; col < N - 1; col += 2)
              *(Crow + ldc * (col+1))=avx2_f32_dot2x1(B+col*ldb,B+(col+1)*ldb, Xrow1,K, Crow+col*ldc);              
         if (col < N)
             *(Crow + ldc * col ) = avx2_f32_dot(Xrow1, B+col*ldb,  K);            
 	}
 }
 
-void avx2_f32_gemm_XtYt2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void avx2_f32_gemm_XtYt2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 { // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
   // MSVC seems not to support it
   //    https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
   //   Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
    
     F32     YROW_FIXEXD[4096];
     F32PTR  Yrow = (2*K <= 4096) ? YROW_FIXEXD : alloca(2*K * sizeof(F32));
@@ -1687,14 +1717,15 @@
     float sumX = f32_hsum(RX);
     float sumY = f32_hsum(RY);
 
     _mm256_zeroupper();
     res[0] = sumX;
     return sumY;
 }
+
 static INLINE F32 __avx2_f32_dot_stride(F32PTR  x, F32PTR y, int N, __m256i mask, __m256i yoffset, I32 stride) {
 
     __m256 r = set0();    
     int i = 0;    
     for (; i < N - (NF - 1); i += NF) {
         __m256 Y = _mm256_i32gather_ps(y + i * stride, yoffset, 4);
         r = add(  r, mul( load(x + i), Y ) );
@@ -1704,15 +1735,16 @@
         __m256 Y = _mm256_mask_i32gather_ps(set0(), y + i * stride, yoffset, _mm256_castsi256_ps(mask), 4);
         r = add(r,  mul(   maskload(x + i, mask), Y  )   );
     }    
     F32 sum = f32_hsum(r);
      _mm256_zeroupper();    
     return sum;
 }
-void avx2_f32_gemm_XYt2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
+
+STATIC void avx2_f32_gemm_XYt2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
 {
     // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
     // MSVC seems not to support it
     /*
     https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
     Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
     */
@@ -1745,15 +1777,15 @@
             *(Crow + ldc * col) = __avx2_f32_dot_stride(Xrow1, B+col, K,mask,BOffset,ldb);
     }
 }
 
 
 ///////////////////////////////////////////////////////////////////////////
 
-void avx2_f32_gemv_Xy1x1_slow(int N, int K, F32PTR X, int lda, F32PTR y, F32PTR C)
+STATIC void avx2_f32_gemv_Xy1x1_slow(int N, int K, F32PTR X, int lda, F32PTR y, F32PTR C)
 {     
     I32     nRemainder = K % 8;
     __m256i mask       = GetMoveMask(nRemainder);
     __m256i Xoffset    = GetRowOffset(lda);    
     for (int row = 0; row < N ; ++row){
        C[row] =__avx2_f32_dot_stride(y, X + row, K, mask, Xoffset, lda);
     }
@@ -1835,15 +1867,16 @@
     {
         __m256 t1 = add(mul(load(x1 + i), C1), mul(load(x2 + i), C2)); 
         maskstore(y + i, GetMoveMask(n), add(t1, load(y + i)));      
     }  
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
-void avx2_f32_gemv_Xb(int N, int K, F32PTR X, int lda, F32PTR b, F32PTR C)
+
+STATIC void avx2_f32_gemv_Xb(int N, int K, F32PTR X, int lda, F32PTR b, F32PTR C)
 {
     //I32     nRemainder = K % 8;
     //__m256i mask    = GetMoveMask(nRemainder);
     //__m256i Xoffset = GetRowOffset(lda);
     memset(C, 0, sizeof(F32) * N);
     int row = 0;
     for (; row < N - (256 * 2 -1); row += 256*2) {
@@ -1875,34 +1908,34 @@
     https://stackoverflow.com/questions/18971401/sparse-array-compression-using-simd-avx2
     https://stackoverflow.com/questions/36932240/avx2-what-is-the-most-efficient-way-to-pack-left-based-on-a-mask
     AVX512 has the compress insturctions that allow copying scattered elements into a contiguous memory accroding to a mask
     https://stackoverflow.com/questions/25074197/compact-avx2-register-so-selected-integers-are-contiguous-according-to-mask
     */
     __m256  VALUE = set1(value);
 
-    int  cnt = 0;
-    int i = 0;
+    int cnt = 0;
+    int i   = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m256 cmpmask = _mm256_cmp_ps(load(x + i), VALUE, _CMP_LT_OQ);
-        int    mask = _mm256_movemask_ps(cmpmask);
-        int  segIdx = i;
+        int    mask    = _mm256_movemask_ps(cmpmask);
+        int    segIdx  = i;
         while (mask) {
             //https://stackoverflow.com/questions/20927710/quickly-count-number-of-zero-valued-bytes-in-an-array/20933337#20933337
             //Remove the branches to speed uo: if (keep)
             int keep = mask & 0x1L;
             indices[cnt] = segIdx++;
             cnt += keep;
             mask >>= 1L;
         }
     }
     int n = N - i;
     if (n > 0) {
         __m256i movemask = GetMoveMask(n);
         __m256  cmpmask = _mm256_cmp_ps(maskload(x + i, movemask), VALUE, _CMP_LT_OQ);
-        int    mask = _mm256_movemask_ps(_mm256_and_ps(cmpmask, _mm256_castsi256_ps(movemask)));
+        int     mask     = _mm256_movemask_ps(_mm256_and_ps(cmpmask, _mm256_castsi256_ps(movemask)));
         int  segIdx = i;
         while (mask) {
             //avoid branches: if (keep)
             int keep = mask & 0x1L;
             indices[cnt] = segIdx++;
             cnt += keep;
             mask = mask >> 1L;
@@ -2102,15 +2135,15 @@
     _mm256_zeroupper();
     return cnt;
 
 
     
 
 }
-I32 avx2_f32_findindex(F32PTR  x, I32PTR indices, F32 value, int N, CmpFlag flag) {
+STATIC I32 avx2_f32_findindex(F32PTR  x, I32PTR indices, F32 value, int N, CmpFlag flag) {
     /*
     https://stackoverflow.com/questions/18971401/sparse-array-compression-using-simd-avx2
     https://stackoverflow.com/questions/36932240/avx2-what-is-the-most-efficient-way-to-pack-left-based-on-a-mask
     AVX512 has the compress insturctions that allow copying scattered elements into a contiguous memory accroding to a mask
     https://stackoverflow.com/questions/25074197/compact-avx2-register-so-selected-integers-are-contiguous-according-to-mask
     */
 
@@ -2127,15 +2160,15 @@
         return _avx2_f32_findindex_EQ(x, indices, value, N);
 
     }
     return 0;
 }
 
 
-void  avx2_f32_scatter_val_byindex(F32PTR  x, I32PTR indices, F32 value, int N) {
+STATIC void  avx2_f32_scatter_val_byindex(F32PTR  x, I32PTR indices, F32 value, int N) {
 // No efficent avx2 version avaialble, so the generic version is used here
    
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
         x[indices[i]] = value;
@@ -2173,15 +2206,15 @@
     _mm256_zeroupper();
     for (; i < N; ++i)    x[indices[i]] = value;
     
 }
 
 
 
-void avx2_f32_scatter_vec_byindex(F32PTR  x, I32PTR indices, F32PTR values, int N) {
+STATIC void avx2_f32_scatter_vec_byindex(F32PTR  x, I32PTR indices, F32PTR values, int N) {
 
      int i = 0;
      #define f2i _mm_castps_si128
      #define i2f _mm_castsi128_ps
      
     for (; i < N - (NF - 1); i += NF) {
         __m256  value    = load(values + i); 
@@ -2204,15 +2237,15 @@
          _mm_store_ss(x + indices[i+2], i2f(  _mm_alignr_epi8(f2i(valueLow), f2i(valueLow),8) ));
          _mm_store_ss(x + indices[i+3], i2f(  _mm_alignr_epi8(f2i(valueLow), f2i(valueLow),12) ));
     }
     _mm256_zeroupper();
     for (; i < N; ++i)    x[indices[i]] = values[i];
     
 } 
-void avx2_f32_gatherVec_scatterVal_byindex(F32PTR  x, I32PTR indices, F32PTR values, F32 newValue, int N) {
+STATIC void avx2_f32_gatherVec_scatterVal_byindex(F32PTR  x, I32PTR indices, F32PTR values, F32 newValue, int N) {
 
      int i = 0;   
     for (; i < N - (NF - 1); i += NF) {
         __m256i index  = loadi(indices + i);   //   __m128i indlow = _mm256_castsi256_si128(index);
         v8sf  oldValues = _mm256_i32gather_ps(x, index, 4);
         store(values + i, oldValues);
         x[indices[i]]   = newValue;
@@ -2238,15 +2271,15 @@
     }    
     for (; i < N; ++i) {
         values[i] = x[indices[i]];
         x[indices[i]] = newValue;
     }
     
 } 
-void avx2_f32_gather2Vec_scatterVal_byindex(F32PTR  x, F32PTR  y, I32PTR indices, F32PTR values, F32 newValue, int N) {
+STATIC void avx2_f32_gather2Vec_scatterVal_byindex(F32PTR  x, F32PTR  y, I32PTR indices, F32PTR values, F32 newValue, int N) {
 
      int i = 0;   
     for (; i < N - (NF - 1); i += NF) {
         __m256i index   = loadi(indices + i);   //   __m128i indlow = _mm256_castsi256_si128(index);
         v8sf  oldXValues = _mm256_i32gather_ps(x, index, 4);
         store(values + i, oldXValues);
         v8sf  oldYValues = _mm256_i32gather_ps(y, index, 4);
@@ -2278,15 +2311,15 @@
         values[i] = x[indices[i]];
         values[N+i] = y[indices[i]];
         x[indices[i]] = newValue;
         y[indices[i]] = newValue;
     }
     
 } 
-void avx2_f32_scale_inplace(const F32 gain, const F32 offset,const F32PTR x, const int N) {
+STATIC void avx2_f32_scale_inplace(const F32 gain, const F32 offset,const F32PTR x, const int N) {
     __m256  G = set1(gain);
     __m256  O = set1(offset);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4)
         store(x + i,       add(mul(load(x + i),       G), O) ),
         store(x + i + NF,  add(mul(load(x + i + NF),  G), O)),
         store(x + i + NF2, add(mul(load(x + i + NF2), G), O)),
@@ -2296,15 +2329,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i, GetMoveMask(n), add(mul(load(x + i), G), O) );
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
 
-void avx2_f32_hinge_pos(const F32PTR X, const F32PTR Y, const F32 knot, const int N){    
+STATIC void avx2_f32_hinge_pos(const F32PTR X, const F32PTR Y, const F32 knot, const int N){
     __m256  O = set0();
     __m256  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 d1 = sub(load(X + i),    C);   store(Y + i,       _mm256_blendv_ps(O, d1, _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
         __m256 d2 = sub(load(X + i+NF), C);   store(Y + i + NF,  _mm256_blendv_ps(O, d2, _mm256_cmp_ps(d2, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
         __m256 d3 = sub(load(X + i+NF2), C);  store(Y + i + NF2, _mm256_blendv_ps(O, d3, _mm256_cmp_ps(d3, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
@@ -2316,15 +2349,15 @@
     
     int n = N - i;
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m256 d1 = sub(load(X + i), C);   maskstore(Y + i, GetMoveMask(n),_mm256_blendv_ps(O, d1, _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();    
 }
-void avx2_f32_hinge_neg(const F32PTR X, const F32PTR Y, const F32 knot, const int N){    
+STATIC void avx2_f32_hinge_neg(const F32PTR X, const F32PTR Y, const F32 knot, const int N){
     __m256  O = set0();
     __m256  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 d1 = sub(C, load(X + i));      store(Y + i,       _mm256_blendv_ps(O, d1, _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
         __m256 d2 = sub(C, load(X + i+NF));   store(Y + i + NF,  _mm256_blendv_ps(O, d2, _mm256_cmp_ps(d2, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
         __m256 d3 = sub(C, load(X + i+NF2));  store(Y + i + NF2, _mm256_blendv_ps(O, d3, _mm256_cmp_ps(d3, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
@@ -2337,15 +2370,15 @@
     int n = N - i;
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m256 d1 = sub(C,load(X + i));   maskstore(Y + i, GetMoveMask(n),_mm256_blendv_ps(O, d1, _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();    
 }
 
-void avx2_f32_step_pos(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
+STATIC void avx2_f32_step_pos(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
     __m256  O = set0();
     __m256  I = set1(1.0);
     __m256  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 d1 = sub(load(X + i),    C);   store(Z + i,       _mm256_blendv_ps(O, load(Y + i),       _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
         __m256 d2 = sub(load(X + i+NF), C);   store(Z + i + NF,  _mm256_blendv_ps(O, load(Y + i+NF),    _mm256_cmp_ps(d2, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
@@ -2358,15 +2391,15 @@
     
     int n = N - i;
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m256 d1 = sub(load(X + i), C);   maskstore(Z + i, GetMoveMask(n),_mm256_blendv_ps(O, load(Y + i), _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();    
 }
-void avx2_f32_step_neg(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
+STATIC  void avx2_f32_step_neg(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
     __m256  O = set0();
     __m256  I = set1(1.0);
     __m256  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m256 d1 = sub(load(X + i),    C);   store(Z + i,       _mm256_blendv_ps(load(Y + i ),      O, _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
         __m256 d2 = sub(load(X + i+NF), C);   store(Z + i + NF,  _mm256_blendv_ps(load(Y + i + NF),  O, _mm256_cmp_ps(d2, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
@@ -2379,15 +2412,15 @@
     
     int n = N - i;
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m256 d1 = sub(load(X + i), C);   maskstore(Z + i, GetMoveMask(n),_mm256_blendv_ps(load(Y + i), O, _mm256_cmp_ps(d1, O, _CMP_GE_OQ))); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();     
 }
-void SetupVectorFunction_AVX2() {
+ void SetupVectorFunction_AVX2() {
 
     FillMaskTempalte();
 
     i32_add_val_inplace = &avx2_i32_add_val_inplace;;
     i32_sum   = &avx2_i32_sum;
     f32_fill_val = &avx2_f32_fill_val;
     f32_sum  = &avx2_f32_sum;
```

### Comparing `Rbeast-0.1.13/ext_src/abc_vec_avx512.c` & `Rbeast-0.1.14/ext_src/abc_vec_avx512.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #include <stdio.h>
 #include <string.h>
 #include <math.h>         //sqrtf
 #include "abc_000_macro.h"
 #include "abc_000_warning.h"
 
+#define STATIC   static
+
 ///////////////////////////////////////////////////////////////////////////
 //stackoverflow.com/questions/2622017/suppressing-deprecated-warnings-in-xcode
 /*
 #ifdef CLANG_COMPILER
     #pragma clang diagnostic push
     #pragma clang diagnostic ignored "-Wdeprecated-declarations"
             //do something////
@@ -98,15 +100,15 @@
 
 // GCC will impiclty convert all the x+i read/write using aligned load/store while
 // MSVC and ICC use the unligned load/store.  So for GCC, we have to expliclty use 
 // the unaligned load/store to avoid seg faults. That is,
 // addi32(*((__m512i*) (x + i)), C)--> addi32 (loadu(x+i),C)
 
 static __mmask16 masktemplate[16];
-static INLINE void      FillMaskTemplate() {   for (I32 i = 0; i < 16; i++)    masktemplate[i] = (1UL << i) - 1UL;  }
+static INLINE void      FillMaskTemplate(void) {   for (I32 i = 0; i < 16; i++)    masktemplate[i] = (1UL << i) - 1UL;  }
 static INLINE __mmask16  __attribute__((always_inline)) GetMoveMask(int n)  {
     return masktemplate[n];
 }
 
 
 static INLINE F32 __attribute__((always_inline)) f32_hsum_m256( __m256 r)  {
     __m128 vlow  = _mm256_castps256_ps128(r);
@@ -146,30 +148,30 @@
     __m256i low = _mm512_castsi512_si256(r);
     __m256i high = _mm512_extracti32x8_epi32(r, 1);
     __m256i R = _mm256_add_epi32(low, high);
     return i32_hsum_m256(R);// SSE2 movd    
 }
 
 
- void avx512_i32_add_val_inplace(const int c, const I32PTR x, const int N) {
+STATIC void avx512_i32_add_val_inplace(const int c, const I32PTR x, const int N) {
     __m512i  C = set1_i32(c);
     int i = 0;
     for (; i < N - (NF4-1); i += NF4) 
         storei(x + i,       addi32(loadi(x + i),       C) ),
         storei(x + i + NF,  addi32(loadi(x + i + NF),  C) ),
         storei(x + i + NF2, addi32(loadi(x + i + NF2), C) ),
         storei(x + i + NF3, addi32(loadi(x + i + NF3), C) );
     for (; i < N - (NF-1); i += NF)  
         storei(x + i, addi32(loadi(x + i), C) );
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstorei(x + i,  GetMoveMask(n),  addi32(loadi(x + i), C)  );
     _mm256_zeroupper();    
 }
-I32  avx512_i32_sum(const I32PTR x, const int N) {
+STATIC I32  avx512_i32_sum(const I32PTR x, const int N) {
     __m512i  S = set0i();
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512i s12   = addi32(loadi(x + i),        loadi(x + i + NF));
         __m512i s34   = addi32(loadi(x + i + NF2),  loadi(x + i + NF3));
          S = addi32(S, addi32(s12, s34));
     }
@@ -179,15 +181,15 @@
     if (n > 0) 
         S= addi32( S,  maskloadi(x + i, GetMoveMask(n) ) );
 
     I32 sum = i32_hsum(S);
      _mm256_zeroupper();
      return sum;
 }
-F32  avx512_f32_sum(const I32PTR x, const int N) {
+STATIC F32  avx512_f32_sum(const I32PTR x, const int N) {
     __m512  S = set0();
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512 s12      = add(load(x + i),        load(x + i + NF) );
         __m512 s34      = add(load(x + i + NF2),  load(x + i + NF3));
          S = add(S, add(s12, s34));
     }
@@ -195,15 +197,15 @@
     int n = N - i;
     if (n > 0)        S = add( S,  maskload(x + i, GetMoveMask(n) ) );
     F32 sum = f32_hsum(S);
      _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
      return sum;
 }
-void avx512_f32_fill_val(const F32 c, F32PTR x, int N) {    
+STATIC void avx512_f32_fill_val(const F32 c, F32PTR x, int N) {
     __m512  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store((x + i),     C);
         store((x + i+NF),  C);
         store((x + i+NF2), C);
         store((x + i+NF3), C);
@@ -212,15 +214,15 @@
         store((x+i), C);
     int n = N - i;
     if (n > 0) 
         maskstore(x + i, GetMoveMask(n), C);    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx512_f32_add_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
+STATIC void avx512_f32_add_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       //dst=dst-src
         store(dst + i,        add(load(src2 + i),       load(src1 + i)));
         store(dst + i + NF,   add(load(src2 + i + NF),  load(src1 + i  + NF)));
         store(dst + i + NF2,  add(load(src2 + i + NF2), load(src1 + i + NF2)));
         store(dst + i + NF3,  add(load(src2 + i + NF3), load(src1 + i + NF3)));
     }
@@ -228,15 +230,15 @@
         store(dst + i,   add(load(src2 + i), load(src1 + i))  );    
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), add(load(src2 + i), load(src1 + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx512_f32_sub_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
+STATIC void avx512_f32_sub_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
     //dst=src2-src1
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       //dst=dst-src
         store(dst + i,       sub(load(src2 + i), load(src1 + i)));
         store(dst + i + NF,  sub(load(src2 + i + NF), load(src1 + i + NF)));
         store(dst + i + NF2, sub(load(src2 + i + NF2), load(src1 + i + NF2)));
         store(dst + i + NF3, sub(load(src2 + i + NF3), load(src1 + i + NF3)));
@@ -245,15 +247,17 @@
         store(dst + i, sub( load(src2 + i), load(src1 + i))  ); 
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), sub(load(src2 + i), load(src1 + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx512_f32_add_vec_inplace(const F32PTR src, const F32PTR dst, const int N) {
+
+
+STATIC void avx512_f32_add_vec_inplace(const F32PTR src, const F32PTR dst, const int N) {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(dst + i,           add(load(dst + i),          load(src + i)));
         store(dst + i + NF,      add(load(dst + i + NF),     load(src + i + NF)));
         store(dst + i + NF2,     add(load(dst + i + NF2),    load(src + i + NF2)));
         store(dst + i + NF3,     add(load(dst + i + NF3),    load(src + i + NF3)));
     }
@@ -262,15 +266,15 @@
     }
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), add(load(dst + i), load(src + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx512_f32_sub_vec_inplace(const F32PTR src, F32PTR dst, int N) {
+STATIC void avx512_f32_sub_vec_inplace(const F32PTR src, F32PTR dst, int N) {
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       //dst=dst-src
         store(dst + i,       sub(load(dst + i),      load(src + i)));
         store(dst + i + NF,   sub(load(dst + i + NF),  load(src + i + NF)));
         store(dst + i + NF2,  sub(load(dst + i + NF2), load(src + i + NF2)));
         store(dst + i + NF3,  sub(load(dst + i + NF3), load(src + i + NF3)));
     }
@@ -279,15 +283,15 @@
     }
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), sub(load(dst + i), load(src + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
-void avx512_f32_add_val_inplace(const F32 c, const F32PTR x, const int N) {
+STATIC void avx512_f32_add_val_inplace(const F32 c, const F32PTR x, const int N) {
     __m512  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) 
         store(x + i,        add(load( x + i),     C)   ),
         store(x + i + NF,    add(load(x + i + NF),  C) ),
         store(x + i + NF2,   add(load(x + i + NF2), C) ),
         store(x + i + NF3,    add(load(x + i + NF3), C) );
@@ -295,15 +299,15 @@
         store(x + i, add(load(x + i), C) );
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i,  GetMoveMask(n), add(load(x + i), C)  );
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
-void avx512_f32_subrev_val_inplace(const F32 c, const F32PTR x, const int N) {
+STATIC void avx512_f32_subrev_val_inplace(const F32 c, const F32PTR x, const int N) {
     __m512  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) 
         store(x + i,      sub(C, load( x + i))   ),
         store(x + i + NF,  sub(C, load(x + i + NF)) ),
         store(x + i + NF2, sub(C, load(x + i + NF2)) ),
         store(x + i + NF3, sub(C, load(x + i + NF3)) );
@@ -312,15 +316,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i,  GetMoveMask(n), sub(C, load(x + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
 
-void avx512_f32_mul_val_inplace(const F32 c, const F32PTR x, const int N) {
+STATIC void avx512_f32_mul_val_inplace(const F32 c, const F32PTR x, const int N) {
     __m512  C = set1(c);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4)
         store(x + i,      mul(load(x + i), C)),
         store(x + i + NF, mul(load(x + i + NF), C)),
         store(x + i + NF2, mul(load(x + i + NF2), C)),
         store(x + i + NF3, mul(load(x + i + NF3), C));
@@ -328,15 +332,15 @@
         store(x + i, mul(load(x + i), C));
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i, GetMoveMask(n), mul(load(x + i), C));
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
-void avx512_f32_mul_vec_inplace(const F32PTR src, F32PTR dst, int N) {
+STATIC void avx512_f32_mul_vec_inplace(const F32PTR src, F32PTR dst, int N) {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(dst + i,       mul(load(dst + i),      load(src + i)));
         store(dst + i + NF,   mul(load(dst + i + NF),  load(src + i + NF)));
         store(dst + i + NF2,  mul(load(dst + i + NF2), load(src + i + NF2)));
         store(dst + i + NF3,  mul(load(dst + i + NF3), load(src + i + NF3)));
     }
@@ -346,15 +350,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), mul(load(dst + i), load(src + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
 
-void avx512_f32_mul_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
+STATIC void avx512_f32_mul_vec(const F32PTR src1, const F32PTR src2, F32PTR dst, int N) {
    int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {       
         store(dst + i,       mul(load(src2 + i),      load(src1 + i)));
         store(dst + i + NF,  mul(load(src2 + i + NF),  load(src1 + i + NF)));
         store(dst + i + NF2,  mul(load(src2 + i + NF2), load(src1 + i + NF2)));
         store(dst + i + NF3,  mul(load(src2 + i + NF3), load(src1 + i + NF3)));
     }
@@ -364,15 +368,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(dst + i, GetMoveMask(n), mul(load(src2 + i), load(src1 + i))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 }
 
-void avx512_f32_add_v_v2_vec_inplace(const F32PTR src, const F32PTR  v, const F32PTR  v2, int N) {
+STATIC void avx512_f32_add_v_v2_vec_inplace(const F32PTR src, const F32PTR  v, const F32PTR  v2, int N) {
 
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(v + i,  add(load(v + i), load(src + i)));
         store(v2 + i, add(load(v2 + i), mul(load(src + i), load(src + i))));
 
         store(v + i+NF,  add(load(v + i + NF),  load(src + i + NF)));
@@ -396,15 +400,15 @@
         maskstore(v + i,  mask, add(   load(v + i),   load(src + i)  )                           );
         maskstore(v2 + i, mask, add(   load(v2 + i),  mul(load(src + i), load(src + i)))     );
     }
     _mm256_zeroupper();
 
  
 }
-F32 avx512_f32_dot(F32PTR  x, F32PTR y, int N) {
+STATIC F32 avx512_f32_dot(F32PTR  x, F32PTR y, int N) {
 
     __m512 r = set0();    
     int i = 0;    
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512 r0   = mul(load(x + i),      load(y + i )) ;
         __m512 r1   = mul(load(x + i+NF),   load(y + i+NF));
         __m512 r2   = mul(load(x + i+NF2),  load(y + i+NF2));
@@ -421,15 +425,15 @@
         __mmask16  mask = GetMoveMask(n);
         r = add(r,  mul(   maskload(x + i, mask), maskload(y + i, mask)   )   );
     }    
     F32 sum = f32_hsum(r);
      _mm256_zeroupper();    
     return sum;
 }
-F32 avx512_f32_dot2x1(F32PTR  x, F32PTR y, F32PTR v, int N, F32PTR res) {
+STATIC F32 avx512_f32_dot2x1(F32PTR  x, F32PTR y, F32PTR v, int N, F32PTR res) {
     __m512 RX = set0();
     __m512 RY = set0();
     int i = 0;    
     for (; i < N - (NF2-1); i += NF2) {
         __m512 x0 = mul(load(x + i),    load(v + i)) ;
         __m512 x1 = mul(load(x + i+NF),  load(v + i+NF));
         __m512 y0 = mul(load(y + i),    load(v + i)) ;
@@ -455,15 +459,15 @@
     float sumY = f32_hsum(RY);
    
      _mm256_zeroupper();
     //for (; i < N; i++)     sum+=x[i] *y[i];
     res[0] = sumX;
     return sumY;
 }
-void avx512_f32_dot2x2(F32PTR  x, F32PTR y, F32PTR v, F32PTR w, int N, F32PTR res1, F32PTR res2) {
+STATIC void avx512_f32_dot2x2(F32PTR  x, F32PTR y, F32PTR v, F32PTR w, int N, F32PTR res1, F32PTR res2) {
     __m512 RX1 = set0();
     __m512 RX2 = set0();
     __m512 RY1 = set0();
     __m512 RY2 = set0();
 
     int i = 0;    
     for (; i  < N - (NF2-1); i += NF2) {
@@ -514,15 +518,15 @@
     //for (; i < N; i++)     sum+=x[i] *y[i];
     res1[0] = sumX1;
     res1[1] = sumY1;
     res2[0] = sumX2;
     res2[1] = sumY2;
     return;
 }
-F32 avx512_fma_f32_dot(F32PTR  x, F32PTR y, int N) {
+STATIC F32 avx512_fma_f32_dot(F32PTR  x, F32PTR y, int N) {
 
     __m512 r0 = set0();
     __m512 r1 = set0();
     __m512 r2 = set0();
     __m512 r3 = set0();
     
     int i = 0;    
@@ -546,15 +550,15 @@
      _mm256_zeroupper();
     return sum;
 }
 
 //https://stackoverflow.com/questions/1528727/why-is-sse-scalar-sqrtx-slower-than-rsqrtx-x
 //https://stackoverflow.com/questions/54642663/how-sqrt-of-gcc-works-after-compiled-which-method-of-root-is-used-newton-rap
 //https://stackoverflow.com/questions/31555260/fast-vectorized-rsqrt-and-reciprocal-with-sse-avx-depending-on-precision
-void avx512_f32_sqrt_vec_inplace(const F32PTR x, const int N)
+STATIC void avx512_f32_sqrt_vec_inplace(const F32PTR x, const int N)
 {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         //__m512 r1 = load(x + i);          store( x + i,  mul(r1, _mm512_sqrt_ps(r1) ) );
         __m512 r1 = load(x + i);          store(x + i,      _mm512_sqrt_ps(r1) );
         __m512 r2 = load(x + i+NF);       store(x + i+NF,   _mm512_sqrt_ps(r2));
         __m512 r3 = load(x + i + NF2);    store(x + i+NF2,  _mm512_sqrt_ps(r3));
@@ -573,15 +577,15 @@
     // for (; i < N; i++)       x[i] = s;
 }
 //https://stackoverflow.com/questions/1528727/why-is-sse-scalar-sqrtx-slower-than-rsqrtx-x
 //https://stackoverflow.com/questions/35885170/handling-zeroes-in-mm256-rsqrt-ps
 //https://stackoverflow.com/questions/8924729/using-avx-intrinsics-instead-of-sse-does-not-improve-speed-why
 //x0 = vrsqrtps(a)
 //x1 = 0.5 * x0 * (3 - (a * x0) * x0)
-void avx512_f32_sqrt_vec(const F32PTR x, const F32PTR y, const int N)
+STATIC void avx512_f32_sqrt_vec(const F32PTR x, const F32PTR y, const int N)
 {
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512 r1 = load(x + i);          store(y + i,      _mm512_sqrt_ps(r1)  );
         __m512 r2 = load(x + i+NF);       store(y + i+ NF,  _mm512_sqrt_ps(r2)  );
         __m512 r3 = load(x + i + NF2);    store(y + i+ NF2, _mm512_sqrt_ps(r3)  );
         __m512 r4 = load(x + i + NF3);    store(y + i+ NF3, _mm512_sqrt_ps(r4)  );
@@ -597,15 +601,15 @@
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
 
 
 #ifdef MSVC_COMPILER
-void avx512_f32_sin_vec_inplace_MSVC(const F32PTR x, const int N)
+STATIC void avx512_f32_sin_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m512 r = load(x + i);    store(x + i,   _mm512_sin_ps(r));
@@ -613,15 +617,15 @@
     int n = N - i;
     if (n > 0) {
         __m512 r = load(x + i);    maskstore(x + i, GetMoveMask(n), _mm512_sin_ps(r) );
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx512_f32_cos_vec_inplace_MSVC(const F32PTR x, const int N)
+STATIC void avx512_f32_cos_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m512 r = load(x + i);    store(x + i, _mm512_cos_ps(r));
@@ -629,15 +633,15 @@
     int n = N - i;
     if (n > 0) {
         __m512 r = load(x + i);    maskstore(x + i, GetMoveMask(n), _mm512_cos_ps(r) );
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx512_f32_sincos_vec_inplace_MSVC(const F32PTR in_outsin, F32PTR outcos, const int N)
+STATIC void avx512_f32_sincos_vec_inplace_MSVC(const F32PTR in_outsin, F32PTR outcos, const int N)
 {
 //Compute the sine and cosine of packed single-precision (32-bit) floating-point elements in a expressed in radians,
 //store the sine in dst, and store the cosine into memory at mem_addr.
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m512 r = load(in_outsin + i);
         store(in_outsin + i, _mm512_sincos_ps(outcos+i,r));
@@ -649,15 +653,15 @@
         __m512  r = load(in_outsin + i);   
         maskstore(in_outsin + i, mask, _mm512_sincos_ps(&tmpcos, r) );
         maskstore(outcos  + i,   mask, tmpcos);
     }
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx512_f32_pow_vec_inplace_MSVC(F32PTR x, F32 pow, int N)
+STATIC void avx512_f32_pow_vec_inplace_MSVC(F32PTR x, F32 pow, int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     
     __m512 C = set1(pow);
 
@@ -668,15 +672,15 @@
     int n = N - i;
     if (n > 0) {
         __m512 r = load(x + i);  maskstore(x + i, GetMoveMask(n), _mm512_pow_ps(r, C));
     }    
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx512_f32_log_vec_inplace_MSVC(const F32PTR x, const int N)
+STATIC void avx512_f32_log_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m512 r = load(x + i);    store(x + i, _mm512_log_ps(r));
@@ -684,15 +688,15 @@
     int n = N - i;
     if (n > 0) {
         __m512 r = load(x + i);    maskstore(x + i, GetMoveMask(n), _mm512_log_ps(r));
     }
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
-void avx512_f32_exp_vec_inplace_MSVC(const F32PTR x, const int N)
+STATIC void avx512_f32_exp_vec_inplace_MSVC(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {
         __m512 r = load(x + i);    store(x + i, _mm512_exp_ps(r));
@@ -703,41 +707,41 @@
     }
     _mm256_zeroupper();
     // for (; i < N; i++)       x[i] = s;
 }
 #endif
 
 
-void avx512_f32_sin_vec_inplace(const F32PTR x, const int N)
+STATIC void avx512_f32_sin_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
     int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i,  sin512_ps(load(x + i)));    
     int n = N - i;
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), sin512_ps(load(x + i)) );
     _mm256_zeroupper();    
 }
-void avx512_f32_cos_vec_inplace(const F32PTR x, const int N)
+STATIC void avx512_f32_cos_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
      int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i, cos512_ps(load(x + i)));    
     int n = N - i;
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), cos512_ps(load(x + i)) );
     _mm256_zeroupper();    
 }
-void avx512_f32_sincos_vec_inplace(const F32PTR in_outsin, F32PTR outcos, const int N) 
+STATIC void avx512_f32_sincos_vec_inplace(const F32PTR in_outsin, F32PTR outcos, const int N)
 {
 //Compute the sine and cosine of packed single-precision (32-bit) floating-point elements in a expressed in radians,
 //store the sine in dst, and store the cosine into memory at mem_addr.
     int i = 0;
     for (; i < N - (NF - 1); i += NF) 
         sincos512_ps(load(in_outsin + i), in_outsin + i, outcos + i);    
     int n = N - i;
@@ -769,15 +773,15 @@
         npositive  = npositive >> 1;
     }
     if (n < 0) {
         res = _mm512_rcp14_ps(res);
     }
     return res;
 }
-void avx512_f32_pow_vec_inplace(F32PTR x, F32 pow, int N)
+STATIC void avx512_f32_pow_vec_inplace(F32PTR x, F32 pow, int N)
 {
          int   nInteger   = pow;
         float  nRemainder = pow - nInteger;
 
         if (nRemainder != 0) {
             int i = 0;
             for (; i < N - (NF - 1); i += NF) {
@@ -794,28 +798,28 @@
             }
             int n = N - i;
             if (n > 0)
                 maskstore(x + i, GetMoveMask(n), pow512_int(load(x + i), nInteger));         
         }
         _mm256_zeroupper();
 }
-void avx512_f32_log_vec_inplace(const F32PTR x, const int N)
+STATIC void avx512_f32_log_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
      int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i, log512_ps(load(x + i)));    
     int n = N - i;
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), log512_ps(load(x + i)) );
     _mm256_zeroupper();    
 }
-void avx512_f32_exp_vec_inplace(const F32PTR x, const int N)
+STATIC void avx512_f32_exp_vec_inplace(const F32PTR x, const int N)
 {
     //https://github.com/reyoung/avx_mathfun/blob/master/avx_mathfun.h
     //http://gruntthepeon.free.fr/ssemath/sse_mathfun.h
     //https://web.archive.org/web/20191019010229/http://software-lisc.fbk.eu/avx_mathfun/avx_mathfun.h
      int i = 0;
     for (; i < N - (NF - 1); i += NF)    
         store(x + i, exp512_ps(load(x + i)));    
@@ -823,15 +827,15 @@
     if (n > 0)
         maskstore(x + i, GetMoveMask(n), exp512_ps(load(x + i)) );
     _mm256_zeroupper();    
 }
 
 
 
-void  avx512_f32_avgstd(const F32PTR x, int N, F32PTR avg, F32PTR std) {
+STATIC void avx512_f32_avgstd(const F32PTR x, int N, F32PTR avg, F32PTR std) {
     __m512  S    = set0();
     __m512  SS   = set0();
     int i = 0;
     for (; i < N - (NF3-1); i += NF4) {
         __m512 s1  =  load(x + i);
         __m512 s2  =  load(x + i+NF);
         __m512 s3  =  load(x + i+NF2);
@@ -865,15 +869,15 @@
     F32 sumxx = f32_hsum(SS);
      _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
      F64 AVG = sumx / N;
      std[0] = sqrtf((sumxx - AVG * sumx) / (N - 1));// sqrtf((sumxx - AVG * AVG * N) / (N - 1));
      avg[0] = AVG;
 }
-void avx512_f32_sx_sxx_to_avgstd_inplace(F32PTR SX, F32PTR SXX, I32 Nsample, F32 scale, F32 offset, int N) {
+STATIC void avx512_f32_sx_sxx_to_avgstd_inplace(F32PTR SX, F32PTR SXX, I32 Nsample, F32 scale, F32 offset, int N) {
     /*
                    r_ippsMulC_32f_I(inv_sample* sd, resultChain.tY, N);
                    r_ippsMul_32f(resultChain.tY, resultChain.tY, MEMBUF1, N);
                    r_ippsMulC_32f_I(inv_sample* sd* sd, resultChain.tSD, N);
                    r_ippsSub_32f_I(MEMBUF1, resultChain.tSD, N);
                    r_ippsSqrt_32f_I(resultChain.tSD, N);
     */
@@ -984,15 +988,15 @@
     _mm256_store_si256(&ID.dummy, maxIdx);
     _mm256_zeroupper();     
     val[0] = max;
     return ID.idx[index>>2] ;
 }
 */
 
-I32 avx512_f32_maxidx(const F32PTR x, const int N, F32PTR val) {
+STATIC I32 avx512_f32_maxidx(const F32PTR x, const int N, F32PTR val) {
     //https://stackoverflow.com/questions/23590610/find-index-of-maximum-element-in-x86-simd-vector    
       
     __m128i _maskIdx    = _mm_cvtsi64_si128(0x0706050403020100);    
             _maskIdx    = _mm_insert_epi64(_maskIdx, 0x0F0E0D0C0B0A0908, 1);
     __m512i idx         = _mm512_cvtepu8_epi32(_maskIdx);
     __m512i Sixteen     = set1_i32(16);
 
@@ -1053,15 +1057,15 @@
      I32 i2 = VAL[2] > VAL[3] ? 2 : 3;
      I32 IDX = VAL[i1] > VAL[i2] ? i1 : i2;
 
      val[0] = VAL[IDX];
     //for (; i < N; i++)     sum+=x[i] *y[i];
     return ID.idx[IDX];
 }
-I32 avx512_f32_minidx(const F32PTR x, const int N, F32PTR val) {
+STATIC I32 avx512_f32_minidx(const F32PTR x, const int N, F32PTR val) {
     
     //https://stackoverflow.com/questions/23590610/find-index-of-maximum-element-in-x86-simd-vector    
       
     __m128i _maskIdx    = _mm_cvtsi64_si128(0x0706050403020100);    
             _maskIdx    = _mm_insert_epi64(_maskIdx, 0x0F0E0D0C0B0A0908, 1);
     __m512i idx         = _mm512_cvtepu8_epi32(_maskIdx);
     __m512i Sixteen     = set1_i32(16);
@@ -1123,15 +1127,15 @@
      I32 i2 = VAL[2] < VAL[3] ? 2 : 3;
      I32 IDX = VAL[i1] < VAL[i2] ? i1 : i2;
 
      val[0] = VAL[IDX];
     return ID.idx[IDX];
 }
 
-void avx512_f32_diff_back(const F32PTR  x, F32PTR result, const int N) {
+STATIC void avx512_f32_diff_back(const F32PTR  x, F32PTR result, const int N) {
     //skip the first elements because evaluation of diff0-x[0]-x[-1] needs an nonexistent element at -1
     //res[i]=x[i]-x[i-1]
 
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         store(result + i,        sub(load(x + i),         load(x + i-1)));
         store(result + i + NF,   sub(load(x + i + NF),    load(x + i + NF-1)));
@@ -1146,15 +1150,15 @@
         maskstore(result + i, GetMoveMask(n), sub(load(x + i), load(x + i-1))  );
     _mm256_zeroupper();
     //for (; i < N; i++)        dst[i] += src[i];
 
     result[0] = result[1];
 
 }
-void avx512_f32_seq(F32PTR p, F32 x0, F32 dX, int N) {
+STATIC void avx512_f32_seq(F32PTR p, F32 x0, F32 dX, int N) {
     
     __m512 X;
     {    
         /*
         __m128i tmp1 = _mm_cvtsi64_si128(0x0706050403020100);
         __m128i tmp2 = _mm_cvtsi64_si128(0x0F0E0D0C0B0A0908);
         __m256i tmp2561 = _mm256_cvtepu8_epi32(tmp1);
@@ -1179,15 +1183,15 @@
     } 
     int n = N - i;
     if (n > 0) {
         maskstore(p + i, GetMoveMask(n), X);
     }     
     _mm256_zeroupper();    
 }
-void avx512_i32_seq(I32PTR p, I32 x0, I32 dX, int N) {
+STATIC void avx512_i32_seq(I32PTR p, I32 x0, I32 dX, int N) {
     
     __m512i X;
     {    
         /*
         __m128i tmp1 = _mm_cvtsi64_si128(0x0706050403020100);
         __m128i tmp2 = _mm_cvtsi64_si128(0x0F0E0D0C0B0A0908);
         __m256i tmp2561 = _mm256_cvtepu8_epi32(tmp1);
@@ -1212,15 +1216,15 @@
     } 
     int n = N - i;
     if (n > 0) {
         maskstorei(p + i, GetMoveMask(n), X);
     }     
     _mm256_zeroupper();    
 }
-void avx512_f32_to_f64_inplace(F32PTR data32, int N) {
+STATIC void avx512_f32_to_f64_inplace(F32PTR data32, int N) {
 
     F64PTR data64 = data32;
     int i = N - 16;
     for (; i >= 0; i -= 16) {
         __m512 r        = load(data32 + i);
         __m256 lowps    = _mm512_castps512_ps256(r);
         __m256 highps   = _mm512_extractf32x8_ps(r, 1);         // high 128
@@ -1241,15 +1245,15 @@
         __m128 r = _mm_loadu_ps(data32 + i);        
         _mm256_storeu_pd(data64 + i, _mm256_cvtps_pd(r));
     }
     i = i - 1;
     for (; i >= 0; --i)   data64[i] = data32[i];    
     _mm256_zeroupper();    
 }
-void avx512_f64_to_f32_inplace(F64PTR data64, int N) {
+STATIC void avx512_f64_to_f32_inplace(F64PTR data64, int N) {
 
     F32PTR data32 = data64;
     int i = 0;
     for (; i < N-15; i += 16) {    
         __m256  R1 = _mm512_cvtpd_ps( _mm512_loadu_pd(data64 + i  )   );
         __m256  R2 = _mm512_cvtpd_ps( _mm512_loadu_pd(data64 + i+8)   );
         _mm256_storeu_ps(data32 + i,   R1);
@@ -1264,15 +1268,15 @@
     for (; i < N - 3; i +=4) {
         __m128  R1 = _mm256_cvtpd_ps(_mm256_loadu_pd(data64 + i));
         _mm_storeu_ps(data32 + i, R1);
     }    
     _mm256_zeroupper();
     for (; i <N; ++i)      data32[i] = data64[i];         
 }
-void avx512_i32_to_f32_scaleby_inplace(I32PTR x, int N, F32 scale) {
+STATIC void avx512_i32_to_f32_scaleby_inplace(I32PTR x, int N, F32 scale) {
     __m512  C = set1(scale);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4)
         store(x + i,       mul(_mm512_cvtepi32_ps(loadi(x + i    )), C)),
         store(x + i + NF,  mul(_mm512_cvtepi32_ps(loadi(x + i+NF )), C)),
         store(x + i + NF2, mul(_mm512_cvtepi32_ps(loadi(x + i+NF2)), C)),
         store(x + i + NF3, mul(_mm512_cvtepi32_ps(loadi(x + i+NF3)), C));
@@ -1281,15 +1285,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i, GetMoveMask(n), mul(_mm512_cvtepi32_ps(loadi(x + i)), C));
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
 
-void avx512_i32_increment_bycond_inplace(I32PTR x,  F32PTR cond, int N) {
+STATIC void avx512_i32_increment_bycond_inplace(I32PTR x,  F32PTR cond, int N) {
     __m512   C0 = set0();
     __m512i  C1 = set1_i32(1);
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {            
         __mmask16 mask   = _mm512_cmp_ps_mask( load(cond+i), C0, _CMP_GT_OQ) ;
         __m512i   vec    =  maskloadi(x + i, mask);
         vec = addi32(vec, C1);
@@ -1303,15 +1307,15 @@
          mask = mask & loadmask;
         __m512i vec = maskloadi(x + i, mask);
         vec = addi32(vec, C1);
         maskstorei(x + i, mask, vec);
     }
     _mm256_zeroupper();
 }
-void avx512_i32_increment_vec2_bycond_inplace(I32PTR x, I32PTR y, F32PTR cond, int N) {
+STATIC void avx512_i32_increment_vec2_bycond_inplace(I32PTR x, I32PTR y, F32PTR cond, int N) {
     __m512   C0        = set0();
     __m512   Ceplison1 = set1(1e-10);
     __m512   Ceplison2 = set1(-1e-10);
     __m512i  C1        = set1_i32(1);
     int i = 0;
     for (; i < N - (NF - 1); i += NF) {   
         __m512    data    = load(cond + i);
@@ -1337,15 +1341,15 @@
          mask2 = mask2 & loadmask;
         __m512i   vec2  = maskloadi(y + i, mask2);
         vec2 = addi32(vec2, C1);    maskstorei(y + i, mask2, vec2);
 
     }
     _mm256_zeroupper();
 }
-I32  avx512_i08_sum_binvec(U08PTR binvec, I32 N) {
+STATIC I32  avx512_i08_sum_binvec(U08PTR binvec, I32 N) {
     //stackoverflow.com/questions/36998538/fastest-way-to-horizontally-sum-sse-unsigned-byte-vector
 	I32   SUM = 0;
 	I32	  i   = 0;
 	//|8bytees|8bytees|8bytees|8bytees|
     __m512i r   = set0i();
     I32  ite_read_for_sad = 0;
 	for (; i < N - (64*4-1); i+=64*4) {
@@ -1427,32 +1431,31 @@
 * > C : = alpha * op(A) * op(B) + beta * C,
 * > where  op(X) is one of
 * > op(X) = X or op(X) = X * *T,
 * > alpha and beta are scalars, and A, Band C are matrices, with op(A)
 * > an m by k matrix, op(B)  a  k by n matrixand C an m by n matrix.
 */
 
-void avx512_f32_gemm_XtY2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
+STATIC void avx512_f32_gemm_XtY2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
 { 
 	for (int col = 0; col < N; ++col) {
 		int row = 0;
 		for (; row < M - (2 - 1); row += 2) 
             C[row + 1] = avx512_f32_dot2x1(A + row * lda, A + (row + 1) * lda, B, K, C + row);
 			//f32_dot3x1(A + ROW * lda, A + (ROW + 1) * lda, A + (ROW + 2) * lda, B, K, C + ROW);			
 			//C[row] = f32_dot(A + row * lda, B, K);		
 		if (row < M) 
 			C[row] = avx512_f32_dot(A + row * lda, B, K);
 		B += ldb;
 		C += ldc;
 	}
  
 }
- 
- 
-void avx512_f32_gemm_XtY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+  
+STATIC void avx512_f32_gemm_XtY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 {
 	int COL;
  	for (COL = 0; COL < N-(2-1); COL+=2) {
 		int ROW;
 		for (ROW=0; ROW < M-(2-1); ROW+=2) {			
             avx512_f32_dot2x2(A+ROW*lda, A + (ROW+1)*lda, B, B+ldb, K, C+ROW, C +ldc+ROW);
 		}
@@ -1553,15 +1556,15 @@
             *(Crow + ldc * col) = avx512_f32_dot(B + col * ldb, Xrow, K);
         }
 
     }
 
 }
 */
-void avx512_f32_gemm_XY1x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
+STATIC void avx512_f32_gemm_XY1x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
 {
     // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
     // MSVC seems not to support it
 
     /*
     https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
     Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
@@ -1581,15 +1584,15 @@
         for (; col < N - 1; col += 2) 
             *(Crow + ldc * (col+1))=avx512_f32_dot2x1(B+col*ldb,B+col*ldb+ldb,Xrow,K, Crow+ldc*col);        
         if (col < N) 
             *(Crow+ldc*col)=avx512_f32_dot(B + col * ldb, Xrow, K);
     }  
 
 }
-void avx512_f32_gemm_XY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void avx512_f32_gemm_XY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 { // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
   // MSVC seems not to support it
   //    https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
   //   Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
    
     F32     XROW_FIXEXD[4096*2];
     F32PTR  Xrow1 = (2*K <= 2*4096) ? XROW_FIXEXD : alloca(2*K*sizeof(F32));
@@ -1619,15 +1622,15 @@
         for (; col < N - 1; col += 2)
              *(Crow + ldc * (col+1))=avx512_f32_dot2x1(B+col*ldb,B+(col+1)*ldb, Xrow1,K, Crow+col*ldc);              
         if (col < N)
             *(Crow + ldc * col ) = avx512_f32_dot(Xrow1, B+col*ldb,  K);            
 	}
 }
 
-void avx512_f32_gemm_XtYt2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void avx512_f32_gemm_XtYt2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 { // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
   // MSVC seems not to support it
   //    https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
   //   Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
    
     F32     YROW_FIXEXD[4096*2];
     F32PTR  Yrow1 = (K <= 4096) ? YROW_FIXEXD : alloca(2*K * sizeof(F32));
@@ -1709,15 +1712,15 @@
         __m512 Y = _mm512_mask_i32gather_ps(set0(), mask, yoffset, y + i * ystride, 4);
         r = add(r,  mul(   maskload(x + i, mask), Y  )   );
     }    
     F32 sum = f32_hsum(r);
      _mm256_zeroupper();    
     return sum;
 }
-void avx512_f32_gemm_XYt2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
+STATIC void avx512_f32_gemm_XYt2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
 {
     // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
     // MSVC seems not to support it
     /*
     https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
     Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
     */
@@ -1749,15 +1752,15 @@
             Crow[ldc * col] = __avx512_f32_dot_stride(Xrow1, B+col, K,mask,BOffset,ldb);
     }
 }
 
 
 ///////////////////////////////////////////////////////////////////////////
 
-void avx512_f32_gemv_Xy1x1_slow(int N, int K, F32PTR X, int lda, F32PTR y, F32PTR C)
+STATIC void avx512_f32_gemv_Xy1x1_slow(int N, int K, F32PTR X, int lda, F32PTR y, F32PTR C)
 {     
     I32       nRemainder = K % NF;
     __mmask16 mask       = GetMoveMask(nRemainder);
     __m512i   Xoffset    = GetRowOffset(lda);    
     for (int row = 0; row < N ; ++row){
             C[row] =__avx512_f32_dot_stride(y, X+row, K, mask, Xoffset, lda);
     }
@@ -1862,15 +1865,15 @@
     int n = N - i;
     if (n > 0) { //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd 
         __m512 t1 = add(mul(load(x1 + i), C1), mul(load(x2 + i), C2)); 
         maskstore(y + i, GetMoveMask(n), add(t1, load(y + i)));      
     }  
     _mm256_zeroupper(); 
 }
-void avx512_f32_gemv_Xb(int N, int K, F32PTR X, int lda, F32PTR b, F32PTR C)
+STATIC void avx512_f32_gemv_Xb(int N, int K, F32PTR X, int lda, F32PTR b, F32PTR C)
 {
     //I32     nRemainder = K % 8;
     //__mmask16 mask    = GetMoveMask(nRemainder);
     //__m512i Xoffset = GetRowOffset(lda);
     memset(C, 0, sizeof(F32) * N);
     int row = 0;
     for (; row < N - (256 * 2 -1); row += 256*2) {
@@ -2106,15 +2109,15 @@
             mask = mask >> 1L;
         }
     }
     _mm256_zeroupper();
 
     return cnt;
 }
-I32 avx512_f32_findindex(F32PTR  x, I32PTR indices, F32 value, int N, CmpFlag flag) {
+STATIC I32 avx512_f32_findindex(F32PTR  x, I32PTR indices, F32 value, int N, CmpFlag flag) {
     /*
     https://stackoverflow.com/questions/18971401/sparse-array-compression-using-simd-avx2
     https://stackoverflow.com/questions/36932240/avx2-what-is-the-most-efficient-way-to-pack-left-based-on-a-mask
     AVX512 has the compress insturctions that allow copying scattered elements into a contiguous memory accroding to a mask
     https://stackoverflow.com/questions/25074197/compact-avx2-register-so-selected-integers-are-contiguous-according-to-mask
     */
     I32 cnt;
@@ -2133,15 +2136,15 @@
         cnt = _avx512_f32_findindex_cmp_eq(x, indices, value, N);  break; // cmpflag = _CMP_EQ_OQ; break;
     }
   
     return cnt;
 }
 
 
-void avx512_f32_scatter_val_byindex(F32PTR  x, I32PTR index, F32 value, int N) {
+STATIC void avx512_f32_scatter_val_byindex(F32PTR  x, I32PTR index, F32 value, int N) {
     
     __m512  vec = set1(value);
     int     i   = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512i indices1  = loadi(index +i);           _mm512_i32scatter_ps(x, indices1, vec , 4);        
         __m512i indices2  = loadi(index + i+NF);       _mm512_i32scatter_ps(x, indices2, vec, 4);
         __m512i indices3  = loadi(index + i+NF2);      _mm512_i32scatter_ps(x, indices3, vec, 4);
@@ -2157,15 +2160,15 @@
         _mm512_mask_i32scatter_ps(x, loadmask, indices1, vec, 4);  
     }
     _mm256_zeroupper();
   
     
 }
 
-void avx512_f32_scatter_vec_byindex(F32PTR  x, I32PTR index, F32PTR value, int N) {
+STATIC void avx512_f32_scatter_vec_byindex(F32PTR  x, I32PTR index, F32PTR value, int N) {
 
     int     i   = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512i indices1 = loadi(index +i);          __m512 vec1  = load(value + i);         _mm512_i32scatter_ps(x, indices1, vec1, 4);        
         __m512i indices2 = loadi(index + i+NF);      __m512 vec2 = load(value + i + NF);     _mm512_i32scatter_ps(x, indices2, vec2, 4);
         __m512i indices3 = loadi(index + i+NF2);     __m512 vec3 = load(value + i + NF2);    _mm512_i32scatter_ps(x, indices3, vec3, 4);
         __m512i indices4 = loadi(index + i+NF3);     __m512 vec4 = load(value + i + NF3);    _mm512_i32scatter_ps(x, indices4, vec4, 4);
@@ -2185,15 +2188,15 @@
   
     
 } 
 
 #define vf5 __m512
 #define vi5 __m512i
 
-void avx512_f32_gatherVec_scatterVal_byindex(F32PTR  x, I32PTR index, F32PTR value, F32 newValue, int N) {
+STATIC void avx512_f32_gatherVec_scatterVal_byindex(F32PTR  x, I32PTR index, F32PTR value, F32 newValue, int N) {
 
     __m512  vec = set1(newValue);
 
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         vi5  indices1  = loadi(index + i);       vf5  oldValue1 = _mm512_i32gather_ps(indices1, x, 4);
         store(value + i, oldValue1);             _mm512_i32scatter_ps(x, indices1, vec, 4);
@@ -2219,15 +2222,15 @@
         vf5  oldValue1 = _mm512_mask_i32gather_ps(set0(),loadmask, indices1, x, 4);
         maskstore(value + i, loadmask,oldValue1);            
         _mm512_mask_i32scatter_ps(x, loadmask, indices1, vec, 4);
     }
     _mm256_zeroupper();
 
 } 
-void avx512_f32_gather2Vec_scatterVal_byindex(F32PTR  x, F32PTR  y, I32PTR index, F32PTR value, F32 newValue, int N) {
+STATIC void avx512_f32_gather2Vec_scatterVal_byindex(F32PTR  x, F32PTR  y, I32PTR index, F32PTR value, F32 newValue, int N) {
 
      __m512  vec = set1(newValue);
 
     int i = 0;
     for (; i < N - (NF2 - 1); i += NF2) {
         vi5  indices1  = loadi(index + i);       vf5  oldX1 = _mm512_i32gather_ps(indices1, x, 4);   vf5  oldY1 = _mm512_i32gather_ps(indices1, y, 4);
         store(value +   i, oldX1);               _mm512_i32scatter_ps(x, indices1, vec, 4);
@@ -2254,15 +2257,15 @@
         maskstore(value +N +i, loadmask, oldY1);
         _mm512_mask_i32scatter_ps(x, loadmask, indices1, vec, 4);
         _mm512_mask_i32scatter_ps(y, loadmask, indices1, vec, 4);
     }
     _mm256_zeroupper();
 
 } 
-void avx512_f32_scale_inplace(const F32 gain, const F32 offset,const F32PTR x, const int N) {
+STATIC void avx512_f32_scale_inplace(const F32 gain, const F32 offset,const F32PTR x, const int N) {
     __m512  G = set1(gain);
     __m512  O = set1(offset);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4)
         store(x + i,       add(mul(load(x + i),       G), O) ),
         store(x + i + NF,  add(mul(load(x + i + NF),  G), O)),
         store(x + i + NF2, add(mul(load(x + i + NF2), G), O)),
@@ -2272,15 +2275,15 @@
     int n = N - i;
     if (n > 0) //TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd
         maskstore(x + i, GetMoveMask(n), add(mul(load(x + i), G), O) );
     _mm256_zeroupper();
     //for (; i < N; i++)         x[i] += c;
 }
 
- void avx512_f32_hinge_pos(const F32PTR X, const F32PTR Y, const F32 knot, const int N){    
+STATIC void avx512_f32_hinge_pos(const F32PTR X, const F32PTR Y, const F32 knot, const int N){
     __m512  O = set0();
     __m512  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512 d1 = sub(load(X + i),    C);   store(Y + i,       _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), O, d1)); //0: take a, 1: take from vec        
         __m512 d2 = sub(load(X + i+NF), C);   store(Y + i + NF,  _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d2, O, _CMP_GE_OQ), O, d2)); //0: take a, 1: take from vec        
         __m512 d3 = sub(load(X + i+NF2), C);  store(Y + i + NF2, _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d3, O, _CMP_GE_OQ), O, d3)); //0: take a, 1: take from vec        
@@ -2293,15 +2296,15 @@
     int n = N - i;
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m512 d1 = sub(load(X + i), C);  
         maskstore(Y + i, GetMoveMask(n), _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), O, d1) ); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();    
 }
- void avx512_f32_hinge_neg(const F32PTR X, const F32PTR Y, const F32 knot, const int N){    
+STATIC void avx512_f32_hinge_neg(const F32PTR X, const F32PTR Y, const F32 knot, const int N){
     __m512  O = set0();
     __m512  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512 d1 = sub(C, load(X + i)    );   store(Y + i,       _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), O, d1)); //0: take a, 1: take from vec        
         __m512 d2 = sub(C, load(X + i+NF) );   store(Y + i + NF,  _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d2, O, _CMP_GE_OQ), O, d2)); //0: take a, 1: take from vec        
         __m512 d3 = sub(C, load(X + i+NF2));   store(Y + i + NF2, _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d3, O, _CMP_GE_OQ), O, d3)); //0: take a, 1: take from vec        
@@ -2315,15 +2318,15 @@
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m512 d1 = sub(C, load(X + i));  
         maskstore(Y + i, GetMoveMask(n), _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), O, d1) ); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();    
 }
 
-  void avx512_f32_step_pos(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
+STATIC void avx512_f32_step_pos(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
     __m512  O = set0();
     __m512  I = set1(1.0);
     __m512  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512 d1 = sub(load(X + i),    C);   store(Z + i,       _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), O, load(Y + i ))); //0: take a, 1: take from vec        
         __m512 d2 = sub(load(X + i+NF), C);   store(Z + i + NF,  _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d2, O, _CMP_GE_OQ), O, load(Y + i + NF))); //0: take a, 1: take from vec        
@@ -2337,15 +2340,15 @@
     int n = N - i;
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m512 d1 = sub(load(X + i), C);  
         maskstore(Z + i, GetMoveMask(n), _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), O, load(Y + i  )) ); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();    
 }
-  void avx512_f32_step_neg(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
+STATIC void avx512_f32_step_neg(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N){
     __m512  O = set0();
     __m512  I = set1(1.0);
     __m512  C = set1(knot);
     int i = 0;
     for (; i < N - (NF4 - 1); i += NF4) {
         __m512 d1 = sub(load(X + i),    C);   store(Z + i,       _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), load(Y + i), O)); //0: take a, 1: take from vec        
         __m512 d2 = sub(load(X + i+NF), C);   store(Z + i + NF,  _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d2, O, _CMP_GE_OQ), load(Y + i+NF), O)); //0: take a, 1: take from vec        
@@ -2359,14 +2362,15 @@
     int n = N - i;
     if (n > 0) {//TODO:BUGGY, loadi should also been a masked load. If not, it may fail during the page bnd        
         __m512 d1 = sub(load(X + i), C);  
         maskstore(Z + i, GetMoveMask(n), _mm512_mask_blend_ps(_mm512_cmp_ps_mask(d1, O, _CMP_GE_OQ), load(Y + i), O) ); //0: take a, 1: take from vec        
     }
     _mm256_zeroupper();    
 }
+
 void SetupVectorFunction_AVX512() {
 
     FillMaskTemplate();
     i32_add_val_inplace = &avx512_i32_add_val_inplace;;
   
     i32_sum   = &avx512_i32_sum;                  
     f32_fill_val = &avx512_f32_fill_val;
```

### Comparing `Rbeast-0.1.13/ext_src/abc_vec_generic.c` & `Rbeast-0.1.14/ext_src/abc_vec_generic.c`

 * *Files 7% similar despite different names*

```diff
@@ -34,18 +34,19 @@
 
 #if defined(WIN64_OS) || defined(WIN32_OS)
     #include <malloc.h> //alloca
 #else
     #include <alloca.h> //alloca
 #endif
 
+#define STATIC static 
 
 //https://www.agner.org/optimize/vectorclass.pdf
 //When the data size is not a multiple of the vector size
-void  gen_i32_add_val_inplace(const int C, const I32PTR X, const int N) {
+STATIC void  gen_i32_add_val_inplace(const int C, const I32PTR X, const int N) {
 
 	#define UNROLL_NUMBER 4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 
 	I32 i = 0;
@@ -54,54 +55,54 @@
 		X[i+1]	+= C;
 		X[i+2]	+= C;
 		X[i+3]	+= C;
 	}
 	for (; i < N; ++i) X[i] += C;
 }
 
-I32   gen_i32_sum(const I32PTR X, const int N) //ippsSum_32s_Sfs(Src, N, Sum, ScaleFfactor);
+STATIC I32   gen_i32_sum(const I32PTR X, const int N) //ippsSum_32s_Sfs(Src, N, Sum, ScaleFfactor);
 {
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 sum=0;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER)  	sum += X[i] + X[i + 1] + X[i + 2] + X[i + 3];	
 	for (; i < N; ++i)								sum+=X[i];
 	
 	return sum;
 }
 
-void gen_f32_fill_val(const F32 C, F32PTR X, int N) {
+STATIC void gen_f32_fill_val(const F32 C, F32PTR X, int N) {
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		X[i]	 =  C;
 		X[i + 1] =  C;
 		X[i + 2] =  C;
 		X[i + 3] =  C;
 	}
 	for (; i < N; ++i) 		X[i] =  C;
 }
 
-F32 gen_f32_sum(const F32PTR X, int N ) {
+STATIC  F32 gen_f32_sum(const F32PTR X, int N ) {
      #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	F64 sum =	0;
 	I32 i	=	0;
 	for (; i < regularPart; i += UNROLL_NUMBER)  	sum = sum+ (X[i] + X[i + 1] + X[i + 2] + X[i + 3]);	
 	for (; i < N; ++i)								sum = sum + X[i];
 	
 	return (F32)sum;
 }
 
-void gen_f32_add_vec(const F32PTR SRC1, const F32PTR SRC2, F32PTR DST, int N) {
+STATIC void gen_f32_add_vec(const F32PTR SRC1, const F32PTR SRC2, F32PTR DST, int N) {
 #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		DST[i] = SRC2[i] + SRC1[i];
@@ -109,15 +110,15 @@
 		DST[i + 2] = SRC2[i + 2] + SRC1[i + 2];
 		DST[i + 3] = SRC2[i + 3] + SRC1[i + 3];
 	}
 	for (; i < N; ++i) DST[i] = SRC2[i] + SRC1[i];
 }
 
 //ippsMul_32f, (const Ipp32f*  pSrc1, const Ipp32f*  pSrc2, Ipp32f*  pDst, int len))
-void gen_f32_sub_vec(const F32PTR SRC1, const F32PTR SRC2, F32PTR DST, int N) {
+STATIC  void gen_f32_sub_vec(const F32PTR SRC1, const F32PTR SRC2, F32PTR DST, int N) {
 #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		DST[i] = SRC2[i] - SRC1[i];
@@ -125,15 +126,15 @@
 		DST[i + 2] = SRC2[i + 2] - SRC1[i + 2];
 		DST[i + 3] = SRC2[i + 3] - SRC1[i + 3];
 	}
 	for (; i < N; ++i) DST[i] = SRC2[i] - SRC1[i];
 }
 
 //ippsMul_32f, (const Ipp32f*  pSrc1, const Ipp32f*  pSrc2, Ipp32f*  pDst, int len))
-void gen_f32_add_vec_inplace(const F32PTR SRC, const F32PTR DST, const int N)
+STATIC  void gen_f32_add_vec_inplace(const F32PTR SRC, const F32PTR DST, const int N)
 {
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
@@ -142,15 +143,15 @@
 		DST[i+2] += SRC[i+2];
 		DST[i+3] += SRC[i+3];
 	}
 	for (; i < N; ++i) DST[i] += SRC[i];
 }
 
 //ippsMul_32f, (const Ipp32f*  pSrc1, const Ipp32f*  pSrc2, Ipp32f*  pDst, int len))
-void gen_f32_sub_vec_inplace(const F32PTR SRC, F32PTR DST, int N) {
+STATIC void gen_f32_sub_vec_inplace(const F32PTR SRC, F32PTR DST, int N) {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		DST[i]   -= SRC[i];
@@ -159,53 +160,53 @@
 		DST[i+3] -= SRC[i+3];
 	}
 	for (; i < N; ++i) DST[i] -= SRC[i];
 }
 
 
 //r_ippsSubCRev_32f_I(val, pSrcDst, N):  C-X
-void gen_f32_subrev_val_inplace(const F32 C, F32PTR X, int N) {
+STATIC void gen_f32_subrev_val_inplace(const F32 C, F32PTR X, int N) {
     const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		X[i]   = C-(X[i]);
 		X[i+1] = C-(X[i+1]);
 		X[i+2] = C - (X[i+2]);
 		X[i+3] = C - (X[i+3]);
 	}
 	for (; i < N; ++i) 		X[i] = C - (X[i]);
 }
 //X+C
-void gen_f32_add_val_inplace(const F32 C, F32PTR X, int N) {
+STATIC void gen_f32_add_val_inplace(const F32 C, F32PTR X, int N) {
     const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		X[i]   = X[i]+C;
 		X[i+1] = X[i+1] + C;
 		X[i+2] = X[i+2] + C;
 		X[i+3] = X[i+3] + C;
 	}
 	for (; i < N; ++i) 		X[i] = X[i] + C;
 }
 
 //F77__sscal(const int N, const F32 alpha, F32PTR X, const int incX);
-void gen_f32_mul_val_inplace(const F32 C, F32PTR X, const int N) {
+STATIC void gen_f32_mul_val_inplace(const F32 C, F32PTR X, const int N) {
     const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		X[i]   = X[i]*C;
 		X[i+1] = X[i+1]* C;
 		X[i+2] = X[i+2]* C;
 		X[i+3] = X[i+3]* C;
 	}
 	for (; i < N; ++i) 		X[i] = X[i]*C;
 }
 
 //F77__sscal(const int N, const F32 alpha, F32PTR X, const int incX);
-void gen_f32_mul_vec_inplace(const F32PTR SRC, F32PTR DST, int N) {
+STATIC void gen_f32_mul_vec_inplace(const F32PTR SRC, F32PTR DST, int N) {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		DST[i]   *= SRC[i];
@@ -213,15 +214,15 @@
 		DST[i+2] *= SRC[i+2];
 		DST[i+3] *= SRC[i+3];
 	}
 	for (; i < N; ++i) DST[i] *= SRC[i];
 }
 
 //F77__sscal(const int N, const F32 alpha, F32PTR X, const int incX);
-void gen_f32_mul_vec(const F32PTR SRC1, const F32PTR SRC2, F32PTR DST, int N) {
+STATIC void gen_f32_mul_vec(const F32PTR SRC1, const F32PTR SRC2, F32PTR DST, int N) {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		DST[i]   = SRC1[i]* SRC2[i];
@@ -229,15 +230,15 @@
 		DST[i+2] = SRC1[i + 2] * SRC2[i + 2];
 		DST[i+3] = SRC1[i + 3] * SRC2[i + 3];
 	}
 	for (; i < N; ++i) DST[i] = SRC1[i] * SRC2[i];
 }
 
 
-void gen_f32_add_v_v2_vec_inplace(const F32PTR SRC, const F32PTR x, F32PTR x2, int N) {
+STATIC void gen_f32_add_v_v2_vec_inplace(const F32PTR SRC, const F32PTR x, F32PTR x2, int N) {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		x[i]   += SRC[i] ; x2[i] += SRC[i]* SRC[i];
@@ -246,15 +247,15 @@
 		x[i + 3] += SRC[i + 3];		x2[i + 3] += SRC[i + 3] * SRC[i + 3];
 	}
 	for (; i < N; ++i) {
 		x[i] += SRC[i]; x2[i] += SRC[i] * SRC[i];
 	}
 }
 
-void gen_f32_sqrt_vec_inplace(const F32PTR X, const int N)
+STATIC void gen_f32_sqrt_vec_inplace(const F32PTR X, const int N)
 {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
@@ -262,30 +263,30 @@
 		X[i+1] = sqrtf(X[i+1]);
 		X[i+2] = sqrtf(X[i+2]);
 		X[i+3] = sqrtf(X[i+3]);
 	}
 	for (; i < N; ++i) 		X[i] = sqrtf(X[i]);
 }
 //vmsSin(const MKL_INT n, const F32  a[], F32  r[], MKL_INT64 mode))
-void gen_f32_cos_vec_inplace(const F32PTR X, const int N)
+STATIC  void gen_f32_cos_vec_inplace(const F32PTR X, const int N)
 {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		X[i]	= cosf(X[i]);
 		X[i+1] = cosf(X[i+1]);
 		X[i+2] = cosf(X[i+2]);
 		X[i+3] = cosf(X[i+3]);
 	}
 	for (; i < N; ++i) 		X[i] = cosf(X[i]);
 }
-void gen_f32_sin_vec_inplace(const F32PTR X, const int N)
+STATIC  void gen_f32_sin_vec_inplace(const F32PTR X, const int N)
 {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
@@ -294,15 +295,16 @@
 		X[i+2] = sinf(X[i+2]);
 		X[i+3] = sinf(X[i+3]);
 	}
 	for (; i < N; ++i) 		X[i] = sinf(X[i]);
 
     #undef  UNROLL_NUMBER 
 }
-void gen_f32_sincos_vec_inplace(const F32PTR in_outsin, F32PTR outcos, const int N)
+
+STATIC void gen_f32_sincos_vec_inplace(const F32PTR in_outsin, F32PTR outcos, const int N)
 {
 #define UNROLL_NUMBER  2
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
@@ -313,32 +315,34 @@
 	}
 	for (; i < N; ++i) {
 		outcos[i]	= cosf(in_outsin[i]);
 		in_outsin[i] = sinf(in_outsin[i]);
 	}
 #undef  UNROLL_NUMBER 
 }
+
 //vmsPowx(const MKL_INT n,  const F32  a[], const F32   b, F32  r[], MKL_INT64 mode))
-void gen_f32_pow_vec_inplace(F32PTR X, F32 pow, int N){
+STATIC void gen_f32_pow_vec_inplace(F32PTR X, F32 pow, int N){
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		X[i]   = powf(X[i], pow);
 		X[i+1] = powf(X[i+1], pow);
 		X[i+2] = powf(X[i+2], pow);
 		X[i+3] = powf(X[i+3], pow);
 	}
 	for (; i < N; ++i) 		X[i] = powf(X[i], pow);
 	#undef  UNROLL_NUMBER 
 }
+
 //vmsSin(const MKL_INT n, const F32  a[], F32  r[], MKL_INT64 mode))
-void gen_f32_log_vec_inplace(const F32PTR X, const int N)
+STATIC void gen_f32_log_vec_inplace(const F32PTR X, const int N)
 {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
@@ -346,16 +350,17 @@
 		X[i+1] = logf(X[i+1]);
 		X[i+2] = logf(X[i+2]);
 		X[i+3] = logf(X[i+3]);
 	}
 	for (; i < N; ++i) 		X[i] = logf(X[i]);
 	 #undef  UNROLL_NUMBER 
 }
-void gen_f32_exp_vec_inplace(const F32PTR X, const int N)
-{
+
+STATIC void gen_f32_exp_vec_inplace(const F32PTR X, const int N) {
+
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		X[i]   = expf(X[i]);
@@ -365,15 +370,15 @@
 	}
 	for (; i < N; ++i) 		X[i] = expf(X[i]);
 
 	#undef  UNROLL_NUMBER 
 }
 
 //ippsMul_32f, (const Ipp32f*  pSrc1, const Ipp32f*  pSrc2, Ipp32f*  pDst, int len))
-void gen_f32_sqrt_vec(const F32PTR X, F32PTR Y, int N) {
+STATIC void gen_f32_sqrt_vec(const F32PTR X, F32PTR Y, int N) {
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER);
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		Y[i]   = X[i]  *  X[i];
 		Y[i+1] = X[i+1] * X[i+1];
 		Y[i+2] = X[i+2] * X[i+2];
@@ -382,15 +387,15 @@
 	for (; i < N; ++i) Y[i] = X[i]*X[i];
 	#undef  UNROLL_NUMBER 
 }
 
 
 
 //void  F77__smnsd(F32* X, int N, F32PTR MEAN, F32PTR  STD);
-void  gen_f32_avgstd(const F32PTR X, int N, F32PTR avg, F32PTR std) {
+STATIC void  gen_f32_avgstd(const F32PTR X, int N, F32PTR avg, F32PTR std) {
      #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	// (AND-ing with -vectorsize will round down to nearest lower multiple of 
 	// vectorsize. This works only if vectorsize is a power of 2)
 	F64 sumx	=	0;
 	F64 sumxx	=	0;
 	I32 i		=	0;
@@ -404,15 +409,16 @@
 	}
 	
 	F64 AVG = sumx / N;
 	std[0] = sqrtf( (sumxx - AVG*sumx) / (N - 1));// sqrtf((sumxx - AVG * AVG * N) / (N - 1));
 	avg[0] = AVG;
 	#undef  UNROLL_NUMBER 
 }
-void gen_f32_sx_sxx_to_avgstd_inplace(F32PTR SX, F32PTR SXX, I32 Nsample, F32 scale, F32 offset, int N) {
+
+STATIC void gen_f32_sx_sxx_to_avgstd_inplace(F32PTR SX, F32PTR SXX, I32 Nsample, F32 scale, F32 offset, int N) {
 	//// sqrtf((sumxx - AVG * AVG * N) / (N - 1));
 	//=sqrt[SXX/N - AVG*AVG]
 
 	F32 inv_sample_scale   = 1./(F64) Nsample *scale;
 	F32 inv_sample_scale2  = 1./(F64)Nsample * scale*scale;
 	I32 i = 0;
 	for (; i < N; ++i) {
@@ -420,16 +426,17 @@
 		F32  sxx_n = SXX[i] * inv_sample_scale2;
 		SXX[i]	   = sqrtf(sxx_n - avg * avg);
 		SX[i]      = avg + offset;
 	}
 // sqrtf((sumxx - AVG * AVG * N) / (N - 1));
 	 
 }
+
 // the index is zero-based
-I32 gen_f32_maxidx_slow(const F32PTR  X, const int N, F32PTR val) {
+STATIC I32 gen_f32_maxidx_slow(const F32PTR  X, const int N, F32PTR val) {
 
 	F32 maxVal = X[0];
 	I32 maxIdx = 0;
 	for (I32 i = 1; i < N; i++) {
 		if (maxVal < X[i]) {
 			maxVal = X[i];
 			maxIdx = i;
@@ -437,15 +444,15 @@
 	}
 
 	*val = maxVal;
 	return maxIdx;
 }
 
 // the index is zero-based
-I32 gen_f32_maxidx(const F32PTR  X, const  int N, F32PTR val) {
+STATIC I32 gen_f32_maxidx(const F32PTR  X, const  int N, F32PTR val) {
 
 	#define UNROLL_NUMBER  2 // it would be even slower if changed to 4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 
 	F32 maxVal = X[0];
 	I32 maxIdx = 0;
 	I32 i = 0;
@@ -469,15 +476,15 @@
 	return maxIdx;
 
 	#undef UNROLL_NUMBER
 }
 
 // the index is zero-based
 //F77__sminidx(F32* X, int N, F32PTR val, int* idx);
-I32 gen_f32_minidx(const F32PTR  X, const int  N, F32PTR val) {
+STATIC I32 gen_f32_minidx(const F32PTR  X, const int  N, F32PTR val) {
 
 	#define UNROLL_NUMBER  2 // it would be even slower if changed to 4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 
 	F32 minVal = X[0];
 	I32 minIdx = 0;
 	I32 i = 0;
@@ -512,15 +519,15 @@
 The first elemn of result (d1=y1-y0 where y0 is non-existent) is borrowed from its 
 immediate right neighor: d1 =d2=x2-x1, so that diff=(d1=y2-y1, d2=y2-y1, d3=d3-d2...)
 
 *diff = *(diff + 1); //fill the leftmost
 
 */
 
-void gen_f32_diff_back(const F32PTR  X, F32PTR result, const int N) {
+STATIC void gen_f32_diff_back(const F32PTR  X, F32PTR result, const int N) {
 
 	#define UNROLL_NUMBER  4 // it would be even slower if changed to 4
 	
 	I32 i = 1;       //skip the first elements because evaluation of diff0-x[0]-x[-1] needs an nonexistent element at -1
 	for (; i < N-(UNROLL_NUMBER-1); i+= UNROLL_NUMBER) {		
 		result[i]		= X[i] - X[i-1];
 		result[i+1]		= X[i+1] - X[i];
@@ -533,15 +540,15 @@
 	}
 
 	result[0] = result[1];
 
 }
 
 
-void gen_f32_seq(F32PTR p, F32 x0, F32 dX, int N)
+STATIC void gen_f32_seq(F32PTR p, F32 x0, F32 dX, int N)
 { 
 	#define UNROLL_NUMBER  4 
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	int i		= 0;
 	const F32 dX2		= dX + dX;
 	const F32 dX3		= dX2 + dX;
 	for ( ; i < regularPart; i+= UNROLL_NUMBER) {
@@ -554,16 +561,16 @@
 	for (; i < N; ++i) {
 		p[i] = x0;
 		x0 += dX;
 	}
 #undef UNROLL_NUMBER
 }
 
-void gen_i32_seq(I32PTR p, I32 x0, I32 dX, int N)
-{
+STATIC  void gen_i32_seq(I32PTR p, I32 x0, I32 dX, int N) {
+
 #define UNROLL_NUMBER  4 
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	int i = 0;
 	const I32 dX2 = dX + dX;
 	const I32 dX3 = dX2 + dX;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		p[i]     = x0;
@@ -574,15 +581,16 @@
 	}
 	for (; i < N; ++i) {
 		p[i] = x0;
 		x0 += dX;
 	}
 #undef UNROLL_NUMBER
 }
-void gen_f32_to_f64_inplace(F32PTR data32, int N) {
+
+STATIC void gen_f32_to_f64_inplace(F32PTR data32, int N) {
 
 	#define UNROLL_NUMBER  4 
 
 	F64PTR data64 = (F64PTR) data32;	
 	//for (ptrdiff_t i = N-1; i >= 0; i--) 	data64[i] = (F64)data32[i];
 	
 	int i;
@@ -596,15 +604,15 @@
 	i = i + UNROLL_NUMBER;
 	for (int j = (i-1); j >= 0; --j) {
 		data64[j] = (F64)data32[j];
 	}
 
 }
 
-void gen_f64_to_f32_inplace(F64PTR data64, int N) {
+STATIC void gen_f64_to_f32_inplace(F64PTR data64, int N) {
 
 	#define UNROLL_NUMBER  4 
 
 	F32PTR data32 = (F64PTR) data64;	
 	//for (ptrdiff_t i = N-1; i >= 0; i--) 	data64[i] = (F64)data32[i];
 	
 	int i=0;
@@ -615,43 +623,43 @@
 		data32[i + 3] = data64[i + 3];
 	}	
 	for (; i < N; ++i) {
 		data32[i] = data64[i];
 	}
 }
 
-void gen_i32_to_f32_scaleby_inplace(I32PTR X, int N, F32 scale) {
+STATIC void gen_i32_to_f32_scaleby_inplace(I32PTR X, int N, F32 scale) {
     const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		*(F32PTR)(X+i)   = (F32)X[i]* scale;
 		*(F32PTR)(X+i+1) = (F32)X[i+1]* scale;
 		*(F32PTR)(X + i + 2) = (F32)X[i+2]* scale;
 		*(F32PTR)(X + i + 3) = (F32)X[i+3]* scale;
 	}
 	for (; i < N; ++i) 		*(F32PTR)(X+i) = X[i]*scale;
 
 }
 
-void gen_i32_increment_bycond_inplace(I32PTR x, F32PTR cond, int N) {
+STATIC void gen_i32_increment_bycond_inplace(I32PTR x, F32PTR cond, int N) {
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	// stackoverflow.com/questions/18481740/pointer-expressions-ptr-ptr-and-ptr
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		if (cond[i]   >0)  ++*(x+i);
 		if (cond[i+1] > 0) ++*(x+i+1);
 		if (cond[i+2] > 0) ++*(x+i+2);
 		if (cond[i+3] > 0) ++*(x+i + 3);;
 	}
 	for (; i < N; ++i) if (cond[i] > 0)  ++x[i]; 
 
 	
 }
 
-void gen_i32_increment_vec2_bycond_inplace(I32PTR x, I32PTR y, F32PTR cond, int N) {
+STATIC void gen_i32_increment_vec2_bycond_inplace(I32PTR x, I32PTR y, F32PTR cond, int N) {
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	// stackoverflow.com/questions/18481740/pointer-expressions-ptr-ptr-and-ptr
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		if (cond[i]   > 1e-10)  ++*(x+i);
 		if (cond[i+1] > 1e-10) ++*(x+i+1);
 		if (cond[i+2] > 1e-10) ++*(x+i+2);
@@ -665,15 +673,16 @@
 	for (; i < N; ++i) {
 		if (cond[i] > 1e-10)                  ++x[i];
 		if (cond[i] < 1e-10 && cond[i]>-1e-10) ++*(y+i);
 	}
 
 	
 }
-I32 gen_i08_sum_binvec(U08PTR binvec, I32 N) {
+
+STATIC I32 gen_i08_sum_binvec(U08PTR binvec, I32 N) {
 	I32   SUM = 0;
 	I32	  i   = 0;
 	U08PTR binvec_old = binvec;
 	//|8bytees|8bytees|8bytees|8bytees|
 	for (; i < N - (32-1); i+=32) {		
 		I64 sum  = *((I64PTR)binvec) + *((I64PTR)binvec + 1) + *((I64PTR)binvec + 2) + *((I64PTR)binvec + 3);
 		*((I32PTR)&sum) = *((I32PTR)&sum) + *((I32PTR)&sum + 1);
@@ -694,27 +703,28 @@
 		SUM = SUM + binvec_old[i];
 	}
 	return SUM;
 }
 
 
 //F77__sdot(const int N, const F32PTR x, const int incx, const F32PTR y, const int incy);
-F32  gen_f32_dot( const F32PTR x, const F32PTR y, const int N) {
+STATIC F32  gen_f32_dot( const F32PTR x, const F32PTR y, const int N) {
 	  #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	F32 sum = 0;
 	I32 i	= 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		sum += x[i] * y[i] + x[i+1] * y[i+1]+x[i + 2] * y[i + 2]+ x[i + 3] * y[i + 3];
 	}
 	for (; i < N; ++i) 		sum +=x[i]*y[i];
 
 	return sum;
 }
-F32  gen_f32_dot2x1( const F32PTR x, const F32PTR y, const F32PTR v, const int N, F32PTR res) {
+
+STATIC F32  gen_f32_dot2x1( const F32PTR x, const F32PTR y, const F32PTR v, const int N, F32PTR res) {
 	#define UNROLL_NUMBER 4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	F32 sumX = 0;
 	F32 sumY = 0;	
  
 		I32 i = 0;
 		for (; i < regularPart; i += UNROLL_NUMBER) {
@@ -726,15 +736,16 @@
 			sumY += y[i] * v[i];
 		}
 	 
 	
 	res[0] = sumX;
 	return sumY;
 }
-F32  gen_f32_dot2x1_dir( const F32PTR x, const F32PTR y, const F32PTR v, const int N, F32PTR res, int dir) {
+
+STATIC F32  gen_f32_dot2x1_dir( const F32PTR x, const F32PTR y, const F32PTR v, const int N, F32PTR res, int dir) {
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	F32 sumX = 0;
 	F32 sumY = 0;	
 	if (dir) {
 		I32 i = 0;
 		for (; i < regularPart; i += UNROLL_NUMBER) {
 			sumX += x[i] * v[i] + x[i + 1] * v[i + 1] + x[i + 2] * v[i + 2] + x[i + 3] * v[i + 3];
@@ -759,15 +770,16 @@
 	
 	}
 
 	
 	res[0] = sumX;
 	return sumY;
 }
-void gen_f32_dot2x2(const F32PTR x1, const F32PTR x2, const F32PTR y1, const F32PTR y2, const int N, F32PTR res1, F32PTR res2 ) {
+
+STATIC void gen_f32_dot2x2(const F32PTR x1, const F32PTR x2, const F32PTR y1, const F32PTR y2, const int N, F32PTR res1, F32PTR res2 ) {
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	F32 sum11 = 0;
 	F32 sum21 = 0;
 	F32 sum12 = 0;
 	F32 sum22 = 0;	
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
@@ -795,15 +807,15 @@
 * > C : = alpha * op(A) * op(B) + beta * C,
 * > where  op(X) is one of
 * > op(X) = X or op(X) = X * *T,
 * > alpha and beta are scalars, and A, Band C are matrices, with op(A)
 * > an m by k matrix, op(B)  a  k by n matrixand C an m by n matrix.
 */
  
-void gen_f32_gemm_XtY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void gen_f32_gemm_XtY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 {
 	int COL;
  	for (COL = 0; COL < N-(2-1); COL+=2) {
 		int ROW;
 		for (ROW=0; ROW < M-(2-1); ROW+=2) {			
             gen_f32_dot2x2(A+ROW*lda, A + (ROW+1)*lda, B, B+ldb, K, C+ROW, C +ldc+ROW);
 		}
@@ -837,15 +849,15 @@
 	}
 	for (; i < N; ++i) {
 		dst[i] = src[0];
 		src += stride;
 	}
 }
 
-void gen_f32_gemm_XY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void gen_f32_gemm_XY2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 { // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
   // MSVC seems not to support it
   //    https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
   //   Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
    
     F32     XROW_FIXEXD[4096];
     F32PTR  Xrow = (2*K <= 4096) ? XROW_FIXEXD : alloca(2*K * sizeof(F32));
@@ -872,15 +884,15 @@
         for (; col < N - 1; col += 2)
              *(Crow + ldc * (col+1))=gen_f32_dot2x1(B+col*ldb,B+(col+1)*ldb, Xrow1,K, Crow+col*ldc);              
         if (col < N)
             *(Crow + ldc * col ) = gen_f32_dot(Xrow1, B+col*ldb,  K);            
 	}
 }
 
-void gen_f32_gemm_XtYt2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
+STATIC void gen_f32_gemm_XtYt2x2(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb,  F32PTR C, int ldc)
 { // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
   // MSVC seems not to support it
   //    https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
   //   Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
    
     F32     YROW_FIXEXD[4096];
     F32PTR  Yrow = (2*K <= 4096) ? YROW_FIXEXD : alloca(2*K * sizeof(F32));
@@ -922,15 +934,16 @@
 	for (; i < N; ++i) {
 		sum += x[i] * y[0];
 		y += ystride;
 	}
 
 	return sum;
 }
-void gen_f32_gemm_XYt2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
+
+STATIC void  gen_f32_gemm_XYt2x1(int M, int N, int K, F32PTR A, int lda, F32PTR B, int ldb, F32PTR C, int ldc)
 {
     // F32 Xrow[K] : variable-length array defined in C99 but optional in C11
     // MSVC seems not to support it
     /*
     https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer
     Typically the compiler can keep track of stack depth on its own and does not need a frame pointer. The exception is if the function uses alloca which moves the stack pointer by a variable amount. Frame pointer omission does make debugging significantly harder. Local variables are harder to locate and stack traces are much harder to reconstruct without a frame pointer to help out. Also, accessing parameters can get more expensive since they are far away from the top of the stack and may require more expensive addressing mode
     */
@@ -945,30 +958,30 @@
         F32PTR Crow = C + row;
         int    col = 0;
         for (; col < N; col++)
             *(Crow + ldc * col) = __gen_f32_dot_stride(Xrow1, B+col, K,ldb);
     }
 }
 
-static  void gen_f32_axpy_inplace(const F32 c, const F32PTR x, F32PTR y, const int N) {
+STATIC   void gen_f32_axpy_inplace(const F32 c, const F32PTR x, F32PTR y, const int N) {
 #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		y[i] += x[i] * c;
 		y[i + 1] += x[i + 1] * c;
 		y[i + 2] += x[i + 2] * c;
 		y[i + 3] += x[i + 3] * c;
 	}
 	for (; i < N; ++i)
 		y[i] += x[i] * c;
 
 }
 
-static INLINE void _f32_axpy_inplace(const F32 c, const F32PTR x, F32PTR y, const int N) {
+STATIC  INLINE void _f32_axpy_inplace(const F32 c, const F32PTR x, F32PTR y, const int N) {
 #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 	I32 i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		y[i]     += x[i] * c;
 		y[i + 1] += x[i + 1] * c;
 		y[i + 2] += x[i + 2] * c;
@@ -988,15 +1001,16 @@
 		y[i+2] += x1[i+2] * a[0] + x2[i+2] * a[1];
 		y[i+3] += x1[i+3] * a[0] + x2[i+3] * a[1];		
 	}
 	for (;i<N; ++i)
 		y[i] += x1[i] * a[0] + x2[i] * a[1];
 
 }
-void gen_f32_gemv_Xb(int N, int K, F32PTR X, int lda, F32PTR b, F32PTR C)
+
+STATIC  void gen_f32_gemv_Xb(int N, int K, F32PTR X, int lda, F32PTR b, F32PTR C)
 {
 	memset(C, 0, sizeof(F32) * N);
 	int row = 0;
 	for (; row < N - (256 * 2 - 1); row += 256 * 2) {
 		int col = 0;
 		for (; col < K - 1; col += 2) {
 			_f32_axpy_inplace_x2(b + col, X + col * lda + row, X + (col + 1) * lda + row, C + row, 256 * 2);	
@@ -1018,15 +1032,15 @@
 
 }
 
 
 
 
 ////////////////////////////////////////////////////
-I32 gen_f32_findindex(F32PTR  x, I32PTR indices, F32 value, int N, CmpFlag flag) {
+STATIC I32 gen_f32_findindex(F32PTR  x, I32PTR indices, F32 value, int N, CmpFlag flag) {
    
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;
 
     int  cnt =0;
     int  i   =0;
     switch (flag) {
@@ -1086,42 +1100,42 @@
             }
             return cnt;
     }
 
 	return cnt;
 }
 
-void  gen_f32_scatter_val_byindex(F32PTR  x, I32PTR indices, F32 value, int N) {
+STATIC void  gen_f32_scatter_val_byindex(F32PTR  x, I32PTR indices, F32 value, int N) {
 
-#define UNROLL_NUMBER  4
+	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
 	int  i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		x[indices[i]] = value;
 		x[indices[i + 1]] = value;
 		x[indices[i + 2]] = value;
 		x[indices[i + 3]] = value;
 	}
 	for (; i < N; ++i)    x[indices[i]] = value;
 }
 
-void  gen_f32_scatter_vec_byindex(F32PTR  x, I32PTR indices, F32PTR values, int N) {
+STATIC void  gen_f32_scatter_vec_byindex(F32PTR  x, I32PTR indices, F32PTR values, int N) {
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
         x[indices[i]]   = values[i];
         x[indices[i+1]] = values[i+1];
         x[indices[i+2]] = values[i+2];
         x[indices[i+3]] = values[i+3];
     }   
     for (; i < N; ++i)    x[indices[i]] = values[i]; 
 }
 
-void gen_f32_gatherVec_scatterVal_byindex(F32PTR  x, I32PTR indices, F32PTR values, F32 newValue, int N) {
+STATIC void gen_f32_gatherVec_scatterVal_byindex(F32PTR  x, I32PTR indices, F32PTR values, F32 newValue, int N) {
    
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
         values[i] = x[indices[i]];
         values[i+1] = x[indices[i+1]];
@@ -1134,15 +1148,16 @@
         x[indices[i+3]] = newValue;
     }   
     for (; i < N; ++i) {
         values[i] = x[indices[i]];
         x[indices[i]] = newValue;
     }
 }
-void gen_f32_gather2Vec_scatterVal_byindex(F32PTR  x, F32PTR  y, I32PTR indices, F32PTR values, F32 newValue, int N){
+
+STATIC void gen_f32_gather2Vec_scatterVal_byindex(F32PTR  x, F32PTR  y, I32PTR indices, F32PTR values, F32 newValue, int N){
    
     #define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
         values[i]   = x[indices[i]];
         values[i+1] = x[indices[i+1]];
@@ -1163,15 +1178,15 @@
         values[i] = x[indices[i]];
         values[N + i] = y[indices[i]];
         x[indices[i]] = newValue;
         y[indices[i]] = newValue;
     }
 }
 
-void gen_f32_scale_inplace(const F32 gain, const F32 offset, const F32PTR x, const int N) {
+STATIC void gen_f32_scale_inplace(const F32 gain, const F32 offset, const F32PTR x, const int N) {
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
 		x[i] = x[i] * gain + offset;
 		x[i+1] = x[i+1] * gain + offset;
 		x[i+2] = x[i+2] * gain + offset;
@@ -1180,61 +1195,61 @@
 	for (; i < N; ++i) {
 		x[i] = x[i] * gain + offset;
 	}
 
 }
 
 
-void gen_f32_hinge_pos(const F32PTR X, const F32PTR Y, const F32 knot, const int N) {
+STATIC void gen_f32_hinge_pos(const F32PTR X, const F32PTR Y, const F32 knot, const int N) {
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
 		Y[i]   = X[i]   >= knot ? X[i]-knot:0;
 		Y[i+1] = X[i+1] >= knot ? X[i+1] - knot : 0;
 		Y[i+2] = X[i+2] >= knot ? X[i+2] - knot : 0;
 		Y[i+3] = X[i+3] >= knot ? X[i+3] - knot : 0;
     }   
 	for (; i < N; ++i) {
 		Y[i] = X[i] >= knot ? X[i] - knot : 0;
 	}
 }
 
-void gen_f32_hinge_neg(const F32PTR X, const F32PTR Y, const F32 knot, const int N) {
+STATIC void gen_f32_hinge_neg(const F32PTR X, const F32PTR Y, const F32 knot, const int N) {
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
 		Y[i]   = X[i]   <= knot ? knot - X[i]   : 0;
 		Y[i+1] = X[i+1] <= knot ? knot - X[i+1] : 0;
 		Y[i+2] = X[i+2] <= knot ? knot - X[i+2] : 0;
 		Y[i+3] = X[i+3] <= knot ? knot - X[i+3] : 0;
     }   
 	for (; i < N; ++i) {
 		Y[i] = X[i] <= knot ? knot - X[i] : 0;
 	}
 }
 
-void gen_f32_step_pos(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N) {
+STATIC void gen_f32_step_pos(const F32PTR X, const F32PTR Y, const F32PTR Z, const F32 knot, const int N) {
 	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
     int  i   = 0;
     for (; i < regularPart; i += UNROLL_NUMBER) {
 		Z[i]   = X[i]   >= knot ? Y[i] : 0;
 		Z[i+1] = X[i+1] >= knot ? Y[i+1] : 0;
 		Z[i+2] = X[i+2] >= knot ? Y[i+2] : 0;
 		Z[i+3] = X[i+3] >= knot ? Y[i+3] : 0;
     }   
 	for (; i < N; ++i) {
 		Z[i] = X[i] >= knot ? Y[i] : 0;
 	}
 }
 
-void gen_f32_step_neg(const F32PTR X, const F32PTR Y, const F32PTR Z,const F32 knot, const int N) {
-#define UNROLL_NUMBER  4
+STATIC void gen_f32_step_neg(const F32PTR X, const F32PTR Y, const F32PTR Z,const F32 knot, const int N) {
+	#define UNROLL_NUMBER  4
 	const int regularPart = N & (-UNROLL_NUMBER); // 4: 100 ; -4: ffff00;    
 	int  i = 0;
 	for (; i < regularPart; i += UNROLL_NUMBER) {
 		Z[i]     = X[i]     >= knot ? 0 : Y[i];
 		Z[i + 1] = X[i + 1] >= knot ? 0 : Y[i+1];
 		Z[i + 2] = X[i + 2] >= knot ? 0 : Y[i+2];
 		Z[i + 3] = X[i + 3] >= knot ? 0 : Y[i+3];
@@ -1243,15 +1258,15 @@
 		Z[i] = X[i] >= knot ? 0 : Y[i];
 	}
 }
 
 
 #include "abc_vec.h"
 
-void SetupVectorFunction_Generic() {
+  void SetupVectorFunction_Generic(void) {
 
 
     i32_add_val_inplace = &gen_i32_add_val_inplace;;
     i32_sum   = &gen_i32_sum;
     f32_fill_val = &gen_f32_fill_val;
     f32_sum  = &gen_f32_sum;
     f32_add_vec   = &gen_f32_add_vec;
```

### Comparing `Rbeast-0.1.13/ext_src/abc_win32_demo.c` & `Rbeast-0.1.14/ext_src/abc_win32_demo.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/abc_win32_demo.h` & `Rbeast-0.1.14/ext_src/abc_win32_demo.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_COREV4.c` & `Rbeast-0.1.14/ext_src/beastv2_COREV4.c`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #include "beastv2_prior_precfunc.h" 
 #include "beastv2_xxyy_allocmem.h" 
 #include "beastv2_io.h" 
 
 #define LOCAL(...) do{ __VA_ARGS__ } while(0);
 //extern MemPointers* mem;
 //time_t start, end; 
-int beast2_main_corev4()   {
+int beast2_main_corev4(void)   {
 
 	// A struct to track allocated pointers   
 	// Do not use 'const MemPointers MEM' bcz Clang will asssume other fields as zeros (e.g., alloc, and alloc0).
 	MemPointers MEM = (MemPointers){.init = mem_init,};
 	MEM.init(&MEM);
 	//MEM.checkHeader = 1;
 	//mem = &MEM;
@@ -50,15 +50,14 @@
 	const BEAST2_OPTIONS_PTR	opt   = GLOBAL_OPTIONS;
 	const BEAST2_EXTRA          extra = opt->extra;
 	
 	typedef int QINT;
 	//const   QINT  q = 1L;
 	const QINT  q   = opt->io.q;
 	
-
 	// Pre-allocate memory to save samples for calculating credibile intervals	
 	CI_PARAM     ciParam = {0,};
 	CI_RESULT    ci[MAX_NUM_BASIS];
 	if (extra.computeCredible) {
 		ConstructCIStruct(	opt->mcmc.credIntervalAlphaLevel, opt->mcmc.samples, opt->io.N*opt->io.q,  //for MRBEAST
 							opt->prior.numBasis,&MEM, &extra.fastCIComputation, &ciParam, ci );  
 	}
@@ -161,24 +160,25 @@
 	const U32  NUM_PIXELS    = opt->io.numOfPixels;
 	const U32  MCMC_SAMPLES  = opt->mcmc.samples;
 	const U32  MCMC_THINNING = opt->mcmc.thinningFactor;
 	const U32  MCMC_BURNIN   = opt->mcmc.burnin;
 	const U32  MCMC_CHAINNUM = opt->mcmc.chainNumber;
 	const U16  SEASON_BTYPE  = opt->prior.seasonBasisFuncType;
 	const U16  GROUP_MatxMat = (MODEL.sid <0 || opt->prior.seasonBasisFuncType != 3 )
+						       && (MODEL.vid < 0 || opt->prior.trendBasisFuncType != 3)
 							   && (MODEL.tid<0  || opt->prior.trendBasisFuncType!=2)
 		                       && ( MODEL.oid<0 || opt->prior.outlierBasisFuncType!=2);
 
 	NUM_OF_PROCESSED_GOOD_PIXELS  = 0; //this is a global variable.
 	NUM_OF_PROCESSED_PIXELS       = 0;  //this is also a global variable.
 	for (U32 pixelIndex = 1; pixelIndex <= NUM_PIXELS; pixelIndex++)
 	{
 		// Fecth a new time-series: set up Y, nMissing,  n, rowsMissing		
 		F32PTR MEMBUF           = Xnewterm; // Xnewterm is a temp mem buf.
-		BEAST2_fetch_next_timeSeries(&yInfo, pixelIndex,  MEMBUF, &(opt->io));
+		BEAST2_fetch_timeSeries(&yInfo, pixelIndex,  MEMBUF, &(opt->io));
 
 
 		F32PTR  Xtmp             = Xt_mars;
 		U08     skipCurrentPixel = BEAST2_preprocess_timeSeries(&yInfo, MODEL.b, Xtmp, opt);		
 	
 
 		#ifdef __DEBUG__
@@ -624,15 +624,15 @@
 				{
 					//Recover the orignal vaules for those rows corresponding to missing Y values
 					if (yInfo.nMissing > 0 && Knewterm > 0 /*&& basis->type != OUTLIERID*/)  //needed for basisFunction_OUliter=1						
 						f32_mat_multirows_set_by_submat(Xnewterm, Npad, Knewterm, Xt_zeroBackup, yInfo.rowsMissing, yInfo.nMissing);
 
 					// Inserting XnewTerms into Xt_mars
 					if (NewCol.k2_old != KOLD && NewCol.k2_new != NewCol.k2_old)
-						MoveCOLsWithinMatrix(Xt_mars, Npad, NewCol.k2_old+1, KOLD, NewCol.k2_new+1);
+						shift_lastcols_within_matrix(Xt_mars, Npad, NewCol.k2_old+1, KOLD, NewCol.k2_new+1);
 					if (Knewterm != 0)
 						SCPY(Knewterm*Npad, Xnewterm, Xt_mars + (NewCol.k1-1) * Npad);
 					
 					/****************************************************/
 					//Find the good positions of the proposed MOVE
 					//Then update the knotLists and order
 					/****************************************************/
@@ -925,15 +925,15 @@
 						//Counting probability of being breakpoints				
 						for (I32 i = 0; i < nKnot; i++) result->xProb[ KNOT[i]-1 ] += 1L;
 
 						//Summng up the harmonic orders or trend orders for individual seeasonal segments
 						if (result->xorder != NULL) {
 							TORDER_PTR  ORDER = basis->ORDER;
 							for (I32 i = 0; i <= nKnot; ++i) {
-								I16 r1 = KNOT[i-1], r2 = KNOT[i]-1;
+								I32 r1 = KNOT[i-1], r2 = KNOT[i]-1;
 								r_ippsAddC_32s_ISfs(ORDER[i], result->xorder+r1 - 1, r2 - r1 + 1, 0);
 							}
 						}
 
 						//Compute the averaged  signals
 						if (q == 1) {
 							//r_cblas_sgemv(CblasColMajor, CblasNoTrans, Npad, K_SN, 1.f, Xt_mars, Npad, MODEL.curr.beta_mean, 1L, 0.f, MEMBUF1, 1L);
@@ -1134,30 +1134,30 @@
 			/*****************************************************************************/
 
 			if (!skipCurrentPixel)
 			{
 				int   sum;
 				#define GetSum(arr) (r_ippsSum_32s_Sfs(arr, N, &sum, 0), sum) // parenthesis operator
 
-				I32   sMAXNUMKNOT = MODEL.sid >=0? MODEL.b[MODEL.sid].prior.maxKnotNum:-9999999;
+				I32   sMAXNUMKNOT = MODEL.sid >=0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum:-9999999; // the seasonal cmpt is always the first one
 				I32   tMAXNUMKNOT = MODEL.tid>=0?  MODEL.b[MODEL.tid].prior.maxKnotNum:-9999999;
 				I32   oMAXNUMKNOT = MODEL.oid>=0?  MODEL.b[MODEL.oid].prior.maxKnotNum:- 9999999;
 				F32   inv_sample  = 1.f / sample;			
 				
 
 				*resultChain.marg_lik = *resultChain.marg_lik * inv_sample;
 				// FOR MRBEAST
 				for (int col = 0; col < q; col++)	{ 
 					for (int i = 0; i < q; i++) {
 						resultChain.sig2[col*q+i] = resultChain.sig2[col*q+i] * inv_sample * yInfo.sd[col] * yInfo.sd[i];
 					}
 				}
 				
 
-				if (MODEL.sid >= 0) {
+				if (MODEL.sid >= 0 || MODEL.vid >= 0) {
 
 						*resultChain.sncp = GetSum(resultChain.scpOccPr)* inv_sample; 
 						i32_to_f32_scaleby_inplace(resultChain.sncpPr,	(sMAXNUMKNOT + 1), inv_sample);
 						i32_to_f32_scaleby_inplace(resultChain.scpOccPr, N,		           inv_sample);	
 					
 						//FOR MRBEAST
 						for (int i = 0; i < q; i++) {
@@ -1300,15 +1300,15 @@
 
 
 			/**************************************************/
 			//   Add up the individual chain to the Result
 			/**************************************************/
 			if (!skipCurrentPixel) 
 			{
-				I32   sMAXNUMKNOT = MODEL.sid >=0? MODEL.b[MODEL.sid].prior.maxKnotNum:-9999999;
+				I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 				I32   tMAXNUMKNOT = MODEL.tid>=0?  MODEL.b[MODEL.tid].prior.maxKnotNum:-9999999;
 				I32   oMAXNUMKNOT = MODEL.oid>=0?  MODEL.b[MODEL.oid].prior.maxKnotNum:- 9999999;
 
 				//https://stackoverflow.com/questions/13216423/error-pasting-and-red-does-not-give-a-valid-preprocessing-token
 				//#define _1(x)      *(result.##x) += *(resultChain.##x) // Working with MSVC but not GCC
 
 				#define _1(x)      *(result.x) += *(resultChain.x)
@@ -1321,15 +1321,15 @@
 				#define _skn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, sMAXNUMKNOT + 1)
 				#define _tkn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, tMAXNUMKNOT + 1)
 				#define _okn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, oMAXNUMKNOT + 1)
 
 				_1(marg_lik);
 				_q2(sig2);  //Fpr MRBEAST
 				
-				if (MODEL.sid >= 0) {					
+				if (MODEL.sid >= 0 || MODEL.vid >0) {
 					_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD);
 					if (extra.computeSeasonOrder)    _N(sorder);
 					if (extra.computeSeasonAmp)      _N(samp), _N(sampSD);
 					if (extra.computeCredible)       _2Nq(sCI);
 				}
 
 				if (MODEL.tid >= 0) {					
@@ -1378,15 +1378,15 @@
 				#undef _skn_1
 				#undef _tkn_1
 			    #undef _okn_1
 			}
 
 			// Jump out of the chainumber loop
 			if (skipCurrentPixel) {
-				r_warning("\nWARNING(#%d):The max number of bad iterations exceeded. Can't decompose the current time series\n", skipCurrentPixel);
+				q_warning("\nWARNING(#%d):The max number of bad iterations exceeded. Can't decompose the current time series\n", skipCurrentPixel);
 				break;
 			}
 		}
 		/*********************************/
 		// WHILE(chainNumber<chainNumber)
 		/*********************************/
 
@@ -1400,15 +1400,15 @@
 	/******************************************************/
 
 		// Average the results from multiple chains
 		if (MCMC_CHAINNUM >= 2 && !skipCurrentPixel)
 		{
 			I32  N = opt->io.N;			
 	
-			I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
+			I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 			I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
 			I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
 
 			const F32 invChainNumber = 1.f /(F32)MCMC_CHAINNUM;
 
 			#define _1(x)      *((F32PTR)result.x)*=invChainNumber
 			#define _N(x)      r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N)
@@ -1420,15 +1420,15 @@
 			#define _skn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, sMAXNUMKNOT + 1)
 			#define _tkn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, tMAXNUMKNOT + 1)
 			#define _okn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, oMAXNUMKNOT + 1)
 
 			F32 maxncpProb;	 
 			_1(marg_lik);			
 			_q2(sig2);
-			if (MODEL.sid >= 0) {
+			if (MODEL.sid >= 0 || MODEL.vid>0) {
 				_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD); 
 				if (extra.computeSeasonOrder)    _N(sorder);
 				if (extra.computeSeasonAmp)     {_N(samp), _N(sampSD);}
 				if (extra.computeCredible)       _2Nq(sCI);
  
 				*result.sncp_mode   = f32_maxidx(result.sncpPr,       sMAXNUMKNOT + 1, &maxncpProb);
 				*result.sncp_median = GetPercentileNcp(result.sncpPr, sMAXNUMKNOT + 1, 0.5);
@@ -1493,47 +1493,47 @@
 			#undef _2N
 			#undef _skn_1
 			#undef _tkn_1
 			#undef _okn_1
 		}
 		if (!skipCurrentPixel) {		
 			I32  N = opt->io.N;  
-			if (MODEL.sid >= 0) 							tsRemoveNaNs(result.sSD, N);
+			if (MODEL.sid >= 0||MODEL.vid>0) 				tsRemoveNaNs(result.sSD, N);
 			if (MODEL.tid >= 0)								tsRemoveNaNs(result.tSD, N);
 			if (MODEL.tid >= 0 && extra.computeTrendSlope)  tsRemoveNaNs(result.tslpSD, N);		 
 			if (MODEL.oid >= 0) 							tsRemoveNaNs(result.oSD, N);
 		}
 
 		// Compute Changepoints and their confidence intervals
 		if (!skipCurrentPixel)
 		{
 			I32     N         = opt->io.N;
 			F32     nan       = getNaN();     //A sloppy way to get a NAN
 
-			F32  	threshold = 0.001f;
+			F32  	threshold = 0.01f;
 			F32PTR	mem       = Xnewterm;  //Xnewterm must have a length larger than or equla to 5*N + max(sncp, tncp);
 			I32PTR  cptList   = (I32PTR)mem + 5LL * N;
 			F32PTR  cptCIList = (F32PTR)mem + 6LL * N;
 
 			I32   cptNumber;
 			I32   trueCptNumber;
 			F32   maxncpProb;
 			const F32 T0 = (F32)opt->io.meta.startTime;
 			const F32 dT = (F32)opt->io.meta.deltaTime;
 
-			I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
+			I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 			I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
 			I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
 
-			I32   sMINSEPDIST = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.minSepDist : -9999999;
+			I32   sMINSEPDIST = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.minSepDist : -9999999;
 			I32   tMINSEPDIST = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.minSepDist : -9999999;
-			I32   oMINSEPDIST = MODEL.oid >= 0 ? 1 : -9999999;
+			I32   oMINSEPDIST = MODEL.oid >= 0 ? 0 : -9999999;  //changed from 1 to 0 to pick up consecutive outlier spikes.
 
 			//--------------Season----------------------------
-			if (extra.computeSeasonChngpt && MODEL.sid >=0)  	{
+			if (extra.computeSeasonChngpt && (MODEL.sid >=0 || MODEL.vid>0 ))  	{
 				cptNumber      = sMAXNUMKNOT;
 				trueCptNumber = FindChangepoint((F32PTR)result.scpOccPr, mem, threshold, cptList, cptCIList, N, sMINSEPDIST, cptNumber);
 				//In the returned result, cptList is a list of detected changepoints, which are all zero-based indices.
 				//That is, a changepoint occurring at t1 has a value of 0.
 
 				for (int i = 0; i < trueCptNumber; i++) {
 					*(result.scp + i)	  = (F32)(*(cptList + i)) * dT + T0;
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_COREV4_gui.c` & `Rbeast-0.1.14/ext_src/beastv2_COREV4_gui.c`

 * *Files 12% similar despite different names*

```diff
@@ -38,31 +38,31 @@
 #ifdef WIN64_OS	
 #include "abc_win32_demo.h"
 #endif
 /*---------WINDOW-------------------------*/
 
 
 /*---------WINDOW-------------------------*/
-void beast2_main_corev4_gui()
+void beast2_main_corev4_gui(void)
 {
 #ifdef WIN64_OS	
 	/*---------WINDOW-------------------------*/
 
 	// A struct to track allocated pointers   
 	// Do not use 'const MemPointers MEM' bcz Clang will asssume other fields as zeros (e.g., alloc, and alloc0).
-	MemPointers MEM = (MemPointers){ .init = mem_init, };
+	MemPointers MEM = (MemPointers){.init = mem_init,};
 	MEM.init(&MEM);
 	//MEM.checkHeader = 1;
 	//mem = &MEM;
 
 	VSLStreamStatePtr stream;
 
 	// Get the Option parameters from the global pointer GLOBAL_OPTIONS, which was already 
 	// set prior to this point (e.g., time-series length N, and number of pixels).	
-	const BEAST2_OPTIONS_PTR	opt = GLOBAL_OPTIONS;
+	const BEAST2_OPTIONS_PTR	opt   = GLOBAL_OPTIONS;
 	const BEAST2_EXTRA          extra = opt->extra;
 
 	/*---------WINDOW-------------------------*/
 	if (gData.N <= 0)
 	{
 		EnterCriticalSection(&gData.cs);
 		gData.N = opt->io.N;
@@ -86,88 +86,87 @@
 		EnterCriticalSection(&gData.cs);
 		while (gData.plotData[0][0] == NULL)
 			SleepConditionVariableCS(&gData.cv, &gData.cs, INFINITE);
 		LeaveCriticalSection(&gData.cs);
 	}
 
 	/*---------WINDOW-------------------------*/
-
+	
 	typedef int QINT;
 	//const   QINT  q = 1L;
-	const QINT  q = opt->io.q;
-
-
+	const QINT  q   = opt->io.q;
+	
 	// Pre-allocate memory to save samples for calculating credibile intervals	
-	CI_PARAM     ciParam = { 0, };
+	CI_PARAM     ciParam = {0,};
 	CI_RESULT    ci[MAX_NUM_BASIS];
 	if (extra.computeCredible) {
-		ConstructCIStruct(opt->mcmc.credIntervalAlphaLevel, opt->mcmc.samples, opt->io.N * opt->io.q,  //for MRBEAST
-			opt->prior.numBasis, &MEM, &extra.fastCIComputation, &ciParam, ci);
+		ConstructCIStruct(	opt->mcmc.credIntervalAlphaLevel, opt->mcmc.samples, opt->io.N*opt->io.q,  //for MRBEAST
+							opt->prior.numBasis,&MEM, &extra.fastCIComputation, &ciParam, ci );  
 	}
 
 	// Allocate MEMORY FOR BASIS VARIABLE: Initialzie two pointers to BASIS
-	BEAST2_MODEL  MODEL = { 0, };
+	BEAST2_MODEL  MODEL = {0,};
 	AllocInitModelMEM(&MODEL, opt, &MEM);
 
 	//Initializing the random number generaotr	
-	LOCAL(
-		U64 seed = (opt->mcmc.seed == 0) ? TimerGetTickCount() : (opt->mcmc.seed + 0x4f352a3dc);
-	r_vslNewStream(&stream, VSL_BRNG_MT19937, seed);
+	LOCAL( 	
+		U64 seed = (opt->mcmc.seed == 0) ? TimerGetTickCount() : (opt->mcmc.seed+0x4f352a3dc);
+		r_vslNewStream(&stream, VSL_BRNG_MT19937, seed);   	
 	)
+	
 
-
-		const U32PTR  RND32 = MyALLOC(MEM, MAX_RAND_NUM, U32, 64);
-	const U16PTR  RND16 = MyALLOC(MEM, MAX_RAND_NUM * 2, U16, 64);
-	const U08PTR  RND08 = MyALLOC(MEM, MAX_RAND_NUM * 4, U08, 64);
-	const F32PTR  RNDGAMMA = MyALLOC(MEM, MAX_RAND_NUM, F32, 64);
-	const U32PTR  RND32_END = RND32 + MAX_RAND_NUM - 7;
-	const U16PTR  RND16_END = RND16 + MAX_RAND_NUM * 2 - 7;
-	const U08PTR  RND08_END = RND08 + MAX_RAND_NUM * 4 - 7 - 3;     //-3 bcz GenRandomBasis will also consume the stream bits
-	const F32PTR  RNDGAMMA_END = RNDGAMMA + MAX_RAND_NUM - MODEL.nPrec - 1L;
-
+	const U32PTR  RND32        = MyALLOC(MEM, MAX_RAND_NUM,     U32, 64);
+	const U16PTR  RND16        = MyALLOC(MEM, MAX_RAND_NUM * 2, U16, 64);
+	const U08PTR  RND08        = MyALLOC(MEM, MAX_RAND_NUM * 4, U08, 64);	
+	const F32PTR  RNDGAMMA     = MyALLOC(MEM, MAX_RAND_NUM,     F32, 64);	
+	const U32PTR  RND32_END    = RND32		+ MAX_RAND_NUM - 7;
+	const U16PTR  RND16_END    = RND16		+ MAX_RAND_NUM * 2 - 7;
+	const U08PTR  RND08_END    = RND08		+ MAX_RAND_NUM * 4 - 7 -3;     //-3 bcz GenRandomBasis will also consume the stream bits
+	const F32PTR  RNDGAMMA_END = RNDGAMMA	+ MAX_RAND_NUM - MODEL.nPrec-1L;
+		
 	// Allocate mem for current covariate/design matrix (Xt_mars), proposed new terms (Xnewterm),
 	// and subset matrix corresponding to rows of missing values.		
 	const F32PTR Xt_mars;
 	const F32PTR Xnewterm;      //will be re-used as a temp mem for multiple purposes
 	const F32PTR Xt_zeroBackup; //mem for saving Xrows of the missing rows	
-	AllocateXXXMEM(&Xt_mars, &Xnewterm, &Xt_zeroBackup, &MODEL, opt, &MEM);
+	AllocateXXXMEM(&Xt_mars, &Xnewterm, &Xt_zeroBackup,&MODEL,opt,&MEM);
 
 	// yInfo used to save the current time series to be processed
 	BEAST2_YINFO     yInfo;
 	AllocateYinfoMEM(&yInfo, opt, &MEM);
-
+	
 	// Allocate the output memory for a single chain (resultChain) and the averaged
 	// result of all chains ( result)
-	BEAST2_RESULT resultChain = { NULL, }, result = { NULL, };
-	BEAST2_Result_AllocMEM(&resultChain, opt, &MEM);
-	BEAST2_Result_AllocMEM(&result, opt, &MEM);
-
+	BEAST2_RESULT resultChain = { NULL,}, result={ NULL, };
+	BEAST2_Result_AllocMEM(&resultChain, opt, &MEM); 	
+	BEAST2_Result_AllocMEM(&result,      opt, &MEM);
+	
 	if (extra.computeCredible) {
-		I32  Npad = (opt->io.N + 7) / 8 * 8;
+		I32  Npad           = (opt->io.N + 7) / 8 * 8;
 		I32  XnewtermOffset = 0;
 		Npad = opt->io.N;    //Correct for the inconsitency of X and Y in gemm and gemv
 		for (I32 i = 0; i < MODEL.NUMBASIS; i++) {
-			if (MODEL.b[i].type == SEASONID || MODEL.b[i].type == DUMMYID || MODEL.b[i].type == SVDID)
-				ci[i].result = resultChain.sCI,		         //season		
-				ci[i].newDataRow = Xnewterm + XnewtermOffset;	 //season		
+			if (MODEL.b[i].type == SEASONID|| MODEL.b[i].type == DUMMYID || MODEL.b[i].type == SVDID)
+				ci[i].result     = resultChain.sCI,		         //season		
+			    ci[i].newDataRow = Xnewterm + XnewtermOffset;	 //season		
 			else if (MODEL.b[i].type == TRENDID)
-				ci[i].result = resultChain.tCI,               //trend			
-				ci[i].newDataRow = Xnewterm + XnewtermOffset;    //trend		
+				ci[i].result     = resultChain.tCI,               //trend			
+			    ci[i].newDataRow = Xnewterm  + XnewtermOffset;    //trend		
 			else if (MODEL.b[i].type == OUTLIERID)
-				ci[i].result = resultChain.oCI,               //outlier
-				ci[i].newDataRow = Xnewterm + XnewtermOffset;     //outlier       
+				ci[i].result     = resultChain.oCI,               //outlier
+			    ci[i].newDataRow = Xnewterm + XnewtermOffset;     //outlier       
 
 			XnewtermOffset += Npad * q;   //FOR MRBEAST
 		}
 	} //NUMVAR_FOR_CI=3
 
 	const CORESULT coreResults[MAX_NUM_BASIS];
 	SetupPointersForCoreResults(coreResults, MODEL.b, MODEL.NUMBASIS, &resultChain);
-
-	const BEAST2_HyperPar  hyperPar = { .alpha_1 = opt->prior.alpha1,.alpha_2 = opt->prior.alpha2,.del_1 = opt->prior.delta1,  .del_2 = opt->prior.delta2 };
+		 
+	const BEAST2_HyperPar  hyperPar = {.alpha_1=opt->prior.alpha1,.alpha_2=opt->prior.alpha2,.del_1=opt->prior.delta1,  .del_2=opt->prior.delta2};
 
 	/****************************************************************************/
 	//		THE OUTERMOST LOOP: Loop through all the time series one by one
 	/****************************************************************************/
 	// Get conversion factors from counts to seceonds
 	InitTimerFunc();
 	StartTimer();
@@ -179,84 +178,84 @@
 	// Print a blank line to be backspaced by the follow
 	if (extra.printProgressBar) {
 		F32 frac = 0.0; I32 firstTimeRun = 1;
 		printProgress(frac, extra.consoleWidth, Xnewterm, firstTimeRun);
 	}
 
 	//#define __DEBUG__
-#undef  __DEBUG__ 
+	#undef  __DEBUG__ 
 
-#ifdef __DEBUG__
-	// Allocate a mem block and memset it to zero
-	I32    N = opt->io.N;
-	I32    Npad = (N + 7) / 8 * 8; Npad = N;//Correct for the inconsitency of X and Y in gemm and gemv
-	F32PTR flagSat = MyALLOC0(MEM, N, I32, 64);
-	F32PTR Xdebug = MyALLOC0(MEM, Npad * (opt->prior.K_MAX + opt->prior.K_MAX), I32, 64); // one Kmax for Xt_mars, and another for Xtbackup
-#endif
-
-
-//#define XtX_ByGroup XtX_ByGroup_FULL
-//#define MatxMat     MatxMat_FULL
-//#define MatxVec     MatxVec_FULL
-
-// Calculate the total number of time sereies to be processed
-	const U32  NUM_PIXELS = opt->io.numOfPixels;
-	const U32  MCMC_SAMPLES = opt->mcmc.samples;
+	#ifdef __DEBUG__
+		// Allocate a mem block and memset it to zero
+		I32    N          = opt->io.N;
+		I32    Npad       = (N + 7) / 8 * 8; Npad =  N;//Correct for the inconsitency of X and Y in gemm and gemv
+		F32PTR flagSat    = MyALLOC0(MEM, N, I32, 64);
+		F32PTR Xdebug     = MyALLOC0(MEM, Npad*(opt->prior.K_MAX+ opt->prior.K_MAX), I32, 64); // one Kmax for Xt_mars, and another for Xtbackup
+	#endif
+
+
+	//#define XtX_ByGroup XtX_ByGroup_FULL
+	//#define MatxMat     MatxMat_FULL
+	//#define MatxVec     MatxVec_FULL
+
+	// Calculate the total number of time sereies to be processed
+	const U32  NUM_PIXELS    = opt->io.numOfPixels;
+	const U32  MCMC_SAMPLES  = opt->mcmc.samples;
 	const U32  MCMC_THINNING = opt->mcmc.thinningFactor;
-	const U32  MCMC_BURNIN = opt->mcmc.burnin;
+	const U32  MCMC_BURNIN   = opt->mcmc.burnin;
 	const U32  MCMC_CHAINNUM = opt->mcmc.chainNumber;
-	const U16  SEASON_BTYPE = opt->prior.seasonBasisFuncType;
-	const U16  GROUP_MatxMat = (MODEL.sid < 0 || opt->prior.seasonBasisFuncType != 3)
-		&& (MODEL.tid < 0 || opt->prior.trendBasisFuncType != 2)
-		&& (MODEL.oid < 0 || opt->prior.outlierBasisFuncType != 2);
+	const U16  SEASON_BTYPE  = opt->prior.seasonBasisFuncType;
+	const U16  GROUP_MatxMat = (MODEL.sid <0 || opt->prior.seasonBasisFuncType != 3 )
+						       && (MODEL.vid < 0 || opt->prior.trendBasisFuncType != 3)
+							   && (MODEL.tid<0  || opt->prior.trendBasisFuncType!=2)
+		                       && ( MODEL.oid<0 || opt->prior.outlierBasisFuncType!=2);
 
-	NUM_OF_PROCESSED_GOOD_PIXELS = 0; //this is a global variable.
-	NUM_OF_PROCESSED_PIXELS = 0;  //this is also a global variable.
+	NUM_OF_PROCESSED_GOOD_PIXELS  = 0; //this is a global variable.
+	NUM_OF_PROCESSED_PIXELS       = 0;  //this is also a global variable.
 	for (U32 pixelIndex = 1; pixelIndex <= NUM_PIXELS; pixelIndex++)
 	{
 		// Fecth a new time-series: set up Y, nMissing,  n, rowsMissing		
-		F32PTR MEMBUF = Xnewterm; // Xnewterm is a temp mem buf.
-		BEAST2_fetch_next_timeSeries(&yInfo, pixelIndex, MEMBUF, &(opt->io));
-
+		F32PTR MEMBUF           = Xnewterm; // Xnewterm is a temp mem buf.
+		BEAST2_fetch_timeSeries(&yInfo, pixelIndex,  MEMBUF, &(opt->io));
 
-		F32PTR  Xtmp = Xt_mars;
-		U08     skipCurrentPixel = BEAST2_preprocess_timeSeries(&yInfo, MODEL.b, Xtmp, opt);
 
+		F32PTR  Xtmp             = Xt_mars;
+		U08     skipCurrentPixel = BEAST2_preprocess_timeSeries(&yInfo, MODEL.b, Xtmp, opt);		
+	
 
-#ifdef __DEBUG__
-		I32 accS[5] = { 0, 0, 0, 0, 0 }, accT[5] = { 0, 0, 0, 0, 0 };
-		I32 flagS[5] = { 0, 0, 0, 0, 0 }, flagT[5] = { 0, 0, 0, 0, 0 };
-		for (int i = 0; i < yInfo.nMissing; i++) { flagSat[yInfo.rowsMissing[i]] = getNaN(); }
-#endif
-
-#define __START_IF_NOT_SKIP_TIMESESIRIES__    
-#define __END_IF_NOT_SKIP_TIMESESIRIES__                        
+		#ifdef __DEBUG__
+			I32 accS[5] = { 0, 0, 0, 0, 0 },  accT[5] = { 0, 0, 0, 0, 0 };
+			I32 flagS[5] = { 0, 0, 0, 0, 0 }, flagT[5] = { 0, 0, 0, 0, 0 };
+			for (int i = 0; i < yInfo.nMissing; i++) { flagSat[yInfo.rowsMissing[i]] = getNaN();}
+		#endif
 
+		#define __START_IF_NOT_SKIP_TIMESESIRIES__    
+		#define __END_IF_NOT_SKIP_TIMESESIRIES__                        
 
-		__START_IF_NOT_SKIP_TIMESESIRIES__
-			if (!skipCurrentPixel) {
 
-				if (q == 1) {  // for BEASTV4
+		__START_IF_NOT_SKIP_TIMESESIRIES__  
+		if (!skipCurrentPixel) {
 
-						// alpha2_star  = alpha_2 + 0.5(YtY-beta*X'Y) = 0.5* (  [YtY+2*alpha_2] - beta*X'Y  )
-						// YtY+2*alpha_2  is pre-cacluated here. THe "2" before alpha_2 is to undo the division
-						// later in the calcution of alpha2_star
-					yInfo.YtY_plus_alpha2Q[0] = yInfo.YtY_plus_alpha2Q[0] + 2 * hyperPar.alpha_2;
+		if (q == 1) {  // for BEASTV4
 
-					//Pre-compute alpha1_start, which depends only on n.
-					yInfo.alpha1_star = yInfo.n * 0.5 + hyperPar.alpha_1;
+				// alpha2_star  = alpha_2 + 0.5(YtY-beta*X'Y) = 0.5* (  [YtY+2*alpha_2] - beta*X'Y  )
+				// YtY+2*alpha_2  is pre-cacluated here. THe "2" before alpha_2 is to undo the division
+				// later in the calcution of alpha2_star
+				yInfo.YtY_plus_alpha2Q[0] = yInfo.YtY_plus_alpha2Q[0] + 2 * hyperPar.alpha_2;
+				
+				//Pre-compute alpha1_start, which depends only on n.
+				yInfo.alpha1_star = yInfo.n * 0.5 + hyperPar.alpha_1;    
 
-				}
-				else {	// For MRBEAST
+		}	else {	// For MRBEAST
 
 				 //YtY was computed from MV_Fetch; here alpaha_Q is added to its diagonal.			
-					f32_add_val_matrixdiag(yInfo.YtY_plus_alpha2Q, hyperPar.alpha_2, q);
+				f32_add_val_matrixdiag(yInfo.YtY_plus_alpha2Q, hyperPar.alpha_2, q);
 
-					yInfo.alpha1_star = yInfo.n * 0.5 + (hyperPar.alpha_1 + q - 1) * 0.5;
-				}
+				yInfo.alpha1_star = yInfo.n * 0.5 + (hyperPar.alpha_1 + q - 1) * 0.5;
+		}
 				/*---------WINDOW-------------------------*/
 				EnterCriticalSection(&gData.cs);
 				{
 					int idx;
 					int N = opt->io.N;
 					I32  Npad = (opt->io.N + 7) / 8 * 8;
 					r_ippsMaxIndx_32f(yInfo.Y, N, &gData.yMax, &idx);
@@ -308,949 +307,932 @@
 					LeaveCriticalSection(&gData.cs);
 				}
 				//For seme reason, the stewindowpos in beast2_winmain is not always working. Put hre
 				//Again
 				SetWindowPos(gData.hwnd, HWND_TOPMOST, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE);
 				/*---------WINDOW-------------------------*/
 
-				/****************************************************************************/
-				// GENERATE A STREAM OF RANDOM NUMBERS FOR FUTURE USE
-				/****************************************************************************/
-				BEAST2_RNDSTREAM  RND;
-				{
-					RND.rnd32 = RND32, RND.rnd16 = RND16, RND.rnd08 = RND08, RND.rndgamma = RNDGAMMA;
-					//vsRngUniform(VSL_RNG_METHOD_UNIFORM_STD_ACCURATE,  stream, MAX_RAND_NUM, rnd, 0, 1.0);		
-					r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, MAX_RAND_NUM, (U32PTR)RND32);
-					r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, MAX_RAND_NUM, (U32PTR)RND16);
-					r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, MAX_RAND_NUM, (U32PTR)RND08);
-					// rndgamma needed to resmaple Sig2, depending on n and alpha_1 
-					// Not used to sample prec bcz the degree of freedom there depends on the number of terms Kterms
-					r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, MAX_RAND_NUM, RNDGAMMA, (hyperPar.alpha_1 + yInfo.n * 0.5f), 0, 1);
-				}
-
-				// Clear up and zero out A(RESULT) for initialization	 
-				BEAST2_Result_FillMEM(&result, opt, 0);
-
-				// Make sure the initial preValues in MODEL.precVec contians no NANs as it will contain residual values
-				// from the previous time series
-				ReInit_PrecValues(&MODEL, opt);
-
-				/****************************************************************************/
-				//Iterate all the chains. The individual chain result will be saved into resultChain
-				/****************************************************************************/
-				for (U32 chainNumber = 0; chainNumber < MCMC_CHAINNUM; chainNumber++)
-				{
+		/****************************************************************************/
+		// GENERATE A STREAM OF RANDOM NUMBERS FOR FUTURE USE
+		/****************************************************************************/
+		BEAST2_RNDSTREAM  RND;
+		{
+			RND.rnd32 = RND32, RND.rnd16 = RND16, RND.rnd08 = RND08, RND.rndgamma = RNDGAMMA;
+			//vsRngUniform(VSL_RNG_METHOD_UNIFORM_STD_ACCURATE,  stream, MAX_RAND_NUM, rnd, 0, 1.0);		
+			r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, MAX_RAND_NUM, (U32PTR)RND32);
+			r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, MAX_RAND_NUM, (U32PTR)RND16);
+			r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, MAX_RAND_NUM, (U32PTR)RND08);
+			// rndgamma needed to resmaple Sig2, depending on n and alpha_1 
+			// Not used to sample prec bcz the degree of freedom there depends on the number of terms Kterms
+			r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, MAX_RAND_NUM, RNDGAMMA, ( hyperPar.alpha_1 + yInfo.n * 0.5f), 0, 1);
+		}
+	 
+		// Clear up and zero out A(RESULT) for initialization	 
+		BEAST2_Result_FillMEM(&result, opt, 0);		
+
+		// Make sure the initial preValues in MODEL.precVec contians no NANs as it will contain residual values
+		// from the previous time series
+		ReInit_PrecValues(&MODEL, opt);
+
+		/****************************************************************************/
+		//Iterate all the chains. The individual chain result will be saved into resultChain
+		/****************************************************************************/
+		for ( U32 chainNumber =0;  chainNumber < MCMC_CHAINNUM; chainNumber++)
+		{
 					/*---------WINDOW-------------------------*/
 					//A timer to compute elapsing time interval
 					LARGE_INTEGER tStart, tEnd, tFrequency;
 					QueryPerformanceCounter(&tStart);
 					QueryPerformanceFrequency(&tFrequency);
 					/*---------WINDOW-------------------------*/
-					const I32  N = opt->io.N;
-					//const I32  Npad   = (N + 7) / 8 * 8; 
-					const I32  Npad = N;//Correct for the inconsitency of X and Y in gemm and gemv
-					const I32  Npad16 = (N + 15) / 16 * 16;
-					/****************************************************************************/
-					//                 GENERATE AN INITIAL MODEL
-					/****************************************************************************/
-					{
-						// Generate random knots (numknot,KNOTs and ORDERS)				
-						GenarateRandomBasis(MODEL.b, MODEL.NUMBASIS, N, &RND);//CHANGE: nunKnot, ORDER, KNOT, K, KBase, Ks, Ke, or TERM_TYPE				
-
-						/*
-						MODEL.b[0].nKnot = 1;
-						MODEL.b[0].ORDER[0] = MODEL.b[0].ORDER[1] = 1;
-						MODEL.b[0].KNOT[0] = 500;
-						MODEL.b[0].KNOT[1] = N + 1;
-						// Get Ks and Ke for individula segments of each components
-						MODEL.b[0].CalcBasisKsKeK_TermType(&MODEL.b[0]);
-						*/
+			const I32  N      = opt->io.N; 
+			//const I32  Npad   = (N + 7) / 8 * 8; 
+			const I32  Npad   = N;//Correct for the inconsitency of X and Y in gemm and gemv
+			const I32  Npad16 = (N + 15) /16 * 16;	
+			/****************************************************************************/
+			//                 GENERATE AN INITIAL MODEL
+			/****************************************************************************/			
+			{   
+				// Generate random knots (numknot,KNOTs and ORDERS)				
+				GenarateRandomBasis(MODEL.b, MODEL.NUMBASIS, N, &RND);//CHANGE: nunKnot, ORDER, KNOT, K, KBase, Ks, Ke, or TERM_TYPE				
+				 
+				/*
+				MODEL.b[0].nKnot = 1;
+				MODEL.b[0].ORDER[0] = MODEL.b[0].ORDER[1] = 1;
+				MODEL.b[0].KNOT[0] = 500;
+				MODEL.b[0].KNOT[1] = N + 1;
+				// Get Ks and Ke for individula segments of each components
+				MODEL.b[0].CalcBasisKsKeK_TermType(&MODEL.b[0]);
+				*/
+
+				/*
+				for (int i = 0; i < MODEL.NUMBASIS; ++i) {
+					MODEL.b[i].nKnot = 0;
+					MODEL.b[i].KNOT[0] = N + 1;
+					MODEL.b[i].ORDER[0] = MODEL.b[i].prior.minOrder;
+					// Get Ks and Ke for individula segments of each components
+					MODEL.b[i].CalcBasisKsKeK_TermType(&MODEL.b[i]);
+				}
+				*/
+ 
+ 		
+				/////////////////////////////////
+				// Update the Kbase for the bases after the 1st one. The first one is fixed at Kbase=0.					
+				// Must be called after GenarateRandomBasis and before BEAST2_EvaluateModel
+				MODEL.b[0].Kbase = 0;                           // This is the first time and also the only time b[0].Kbase is specified
+				UpdateBasisKbase(MODEL.b, MODEL.NUMBASIS, 0);	//CHANGE: MODEL.b[i].Kbase for i>basisID				
+								
+				precFunc.GetNumTermsPerPrecGrp(&MODEL); //CHANGE: (1) nothing or (2) MODEL.curr.nTermsPerPrecGrp + MODEL.b[id].offsetPrec								
+				precFunc.GetXtXPrecDiag(&MODEL);        //CHANGE: (1)nothing or (2) MODEL.curr.precXtXDiag
+				
+				// Find candidate positions for SEASON AND TREND				
+				// nMissing & rowsMissing used for the outlier function
+				CvtKnotsToBinVec(MODEL.b, MODEL.NUMBASIS, N, &yInfo);
+
+				//Evaluate the initial model and compute its marg lik. CHANGE: DERIVE XMARS, K, BETA, BETA_MEAN, MARG_LIK
+				// Xtmars is a cotinguous mem block consiting of Xtmars, Xnewterm, and Xt_zerobackup. The first part will
+				// be filled with Xtmars, and the rest will be used as a temp block in this function call.
+				// We don't use Xnewterm  or Xt_zerobackup as a temp mem buf bcz the zeroOutXmars function may need a much
+				// larger  mem due to the many terms of the inital random model	
+				// basis->K won't be updated inside the function and the old values from CalcBasisKsKeK is kept
+				if (q == 1) {
+					BEAST2_EvaluateModel(&MODEL.curr, MODEL.b, Xt_mars, N, MODEL.NUMBASIS, &yInfo, &hyperPar, &opt->prior.precValue, &stream); 
+				} else 	{
+					MR_EvaluateModel(    &MODEL.curr, MODEL.b, Xt_mars, N, MODEL.NUMBASIS, &yInfo, &hyperPar, &opt->prior.precValue, &stream);
+				}
+		
+			}
+		
 
-						/*
-						for (int i = 0; i < MODEL.NUMBASIS; ++i) {
-							MODEL.b[i].nKnot = 0;
-							MODEL.b[i].KNOT[0] = N + 1;
-							MODEL.b[i].ORDER[0] = MODEL.b[i].prior.minOrder;
-							// Get Ks and Ke for individula segments of each components
-							MODEL.b[i].CalcBasisKsKeK_TermType(&MODEL.b[i]);
-						}
-						*/
+			{
+				// Clear up and zero out resultChain for initialization
+				BEAST2_Result_FillMEM(&resultChain, opt, 0);
+
+				// Reset all nots to ones bcz the real extrem positiosn won'tY be updated till samples > 1
+				memset(MODEL.extremePosVec, 1, N);
+				for (I32 i = 0; i < yInfo.nMissing; ++i) MODEL.extremePosVec[yInfo.rowsMissing[i]] = 0;
+				MODEL.extremPosNum = yInfo.n;
+			}
 
+			/**********************************************************************************************/
+			// PREPARE FOR THE START OF THE MAIN LOOP
+			// The proposed basis needs XtX and XtY of the current basis to compute XtX_prop and XtY_prop.
+			// Other varialbes (e.g., beta and cholXtX) are not cross-used by the basis and basis_prop
+			/**********************************************************************************************/
+			U32 ite            = 0;
+			U32 sample         = 0;
+
+			/*************************************************************/
+			// samplesInserted must be reset to zero at the start of each chain
+			/*************************************************************/
+			if (extra.computeCredible) { 
+				for (int i = 0; i < MODEL.NUMBASIS; i++) {
+					ci[i].samplesInserted = 0;
+				} 
+			} 
+
+			PROP_DATA PROPINFO = {.N=N,                   .Npad16 = Npad16,   .samples=&sample,
+				                  .keyresult=coreResults, .mem    = Xnewterm, .model  =&MODEL, 
+				                  .pRND =&RND,            .yInfo  =&yInfo,    .nSample_ExtremVecNeedUpdate =1L,       
+								  .sigFactor = opt->prior.sigFactor,          .outlierSigFactor = opt->prior.outlierSigFactor,
+			}; 
+
+			NEWTERM        NEW;     // moved here bvz its xcols has two fixed lements, N and Npad
+			NEWCOLINFO     NewCol; // moved here bvz its xcols has two fixed lements, N and Npad
+			NewCol.N    = N;
+			NewCol.Nlda = Npad;
+
+			I32 numBadIterations = 0;
+			while (sample < MCMC_SAMPLES)
+			{
+				ite++;
+				/**********************************************************************/
+				/*     Re-generate a pool of random numbers if almost used up          */
+				/***********************************************************************/
+				//vsRngUniform(VSL_RNG_METHOD_UNIFORM_STD_ACCURATE, stream, MAX_RAND_NUM, rnd32, 0.f, 1.0f);
+				if (RND.rnd32    >= RND32_END)    {r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, (RND.rnd32 - RND32), (U32PTR)RND32);	                               RND.rnd32    = RND32;   }
+				if (RND.rnd16    >= RND16_END)    {r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, ((char*)RND.rnd16 - (char*)RND16 + 3) / sizeof(U32), (U32PTR)RND16); RND.rnd16    = RND16;   }
+				if (RND.rnd08    >= RND08_END)    {r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, ((char*)RND.rnd08 - (char*)RND08 + 3) / sizeof(U32), (U32PTR)RND08); RND.rnd08    = RND08;   }
+				if (RND.rndgamma >= RNDGAMMA_END) {r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE,      stream, MAX_RAND_NUM, RNDGAMMA, (hyperPar.alpha_1+yInfo.n*0.5f), 0.f, 1.f);    RND.rndgamma = RNDGAMMA;}
+	
+				//  Choose a basis type	
+				BEAST2_BASIS_PTR basis = MODEL.b + MODEL.PickBasisID(&PROPINFO); //basisID = *RND.rnd08++ < 128;				
+				
+				// IMPLEMENT THE NEW PROPOSED BASIS	
+				//CHANGE: new.newKnot, numSeg, SEG/R1/2, orders2, newIdx, nKnot_new, jumpType,propinfo.pRND.rnd8/32				
+				basis->Propose(basis, &NEW, &NewCol, &PROPINFO); //info->mem=Xnewterm is used as a temp membuf here
+
+				#ifdef __DEBUG__
+					I32 basisIdx = basis - MODEL.b;		
+					flagSat[NEW.newKnot - 1] += basisIdx == 0 && (NEW.jumpType == BIRTH || NEW.jumpType == MOVE);					 
+					if (basisIdx == 0) ++(flagS[NEW.jumpType]);
+					else 		       ++(flagT[NEW.jumpType]); 
+				#endif
+
+				/**********************************************************************/
+				// Generate the new terms for the propsed step: To add or move a bk, two segments 
+				// are re-generated; to remove a bk or merge two bks, one segment are re-generated.	
+				/**********************************************************************/								
+				I32 Knewterm = 0;				
+				for (I32 i = 0; i < NEW.numSeg; i++) { 
+					// NEW.numSeg is 0 if removing terms for ChORDER(newOrder<oldeTerm)
+					// [1]..(1)....(2)...(sY-1)...N [N+1] 
+					I32 kterms   = NEW.SEG[i].K = basis->GenTerms(Xnewterm+Npad*Knewterm, N, &NEW.SEG[i], &(basis->bConst));					
+					Knewterm    += kterms;
+				} // Iterate through all the new segments
+
+				NewCol.k2_new = NewCol.k1 + Knewterm - 1L;	// if Knewterm=0 (i.e., delete terms), k2_new < k1_new
+				
+				//Get k1_old, k2_old, k1_new and k2_new
+				NewCol.k1     += basis->Kbase;		// k1=k1_new=k1_old
+				NewCol.k2_old += basis->Kbase;
+				NewCol.k2_new += basis->Kbase;
+
+				I32 KOLD     = MODEL.curr.K;                         // Total number of basis for the current model				
+				I32 KNEW     = KOLD + NewCol.k2_new - NewCol.k2_old; // Total number of bases in the proposed model	
+
+				NewCol.Knewterm = Knewterm;
+				NewCol.KOLD     = KOLD;
+				NewCol.KNEW     = KNEW;				
+
+				/*************************************************************************/
+				// Get XtX_prop: Copy parts of XtX to XtT_prop and fill new components 
+				/*************************************************************************/
+				// Set those rows of Xt_mars_newterms specfied by rowsMissing  to zeros
+				if (yInfo.nMissing > 0 && Knewterm > 0 /*&& basis->type != OUTLIERID*/)  //needed for basisFunction_OUliter=1
+				f32_mat_multirows_extract_set_by_scalar(Xnewterm,Npad,Knewterm,Xt_zeroBackup, yInfo.rowsMissing, yInfo.nMissing, 0.0f);
+
+
+				if (!GROUP_MatxMat) {
+					update_XtX_from_Xnewterm(Xt_mars, Xnewterm, MODEL.curr.XtX, MODEL.prop.XtX, &NewCol);
+					update_XtY_from_Xnewterm(yInfo.Y, Xnewterm, MODEL.curr.XtY, MODEL.prop.XtY, &NewCol, q);
+				}
+				else {
+				
+					/*************************************************************************/
+					//               The FIRST component:	
+					/*************************************************************************/
+					// There'sY no first component if k1_old/k1_new=1 for SEASON	
+					for (I32 i = 1; i < NewCol.k1; i++) SCPY(i, MODEL.curr.XtX + (i - 1L) * KOLD, MODEL.prop.XtX + (i - 1L) * KNEW);
+
+					/*************************************************************************/
+					//              The SECOND component
+					/*************************************************************************/
+					// No new cols/terms if flag=ChORDER && isInsert=0:the resampled basis has a higher order than the old basis
+					if (Knewterm != 0) {
 
-						/////////////////////////////////
-						// Update the Kbase for the bases after the 1st one. The first one is fixed at Kbase=0.					
-						// Must be called after GenarateRandomBasis and before BEAST2_EvaluateModel
-						MODEL.b[0].Kbase = 0;                           // This is the first time and also the only time b[0].Kbase is specified
-						UpdateBasisKbase(MODEL.b, MODEL.NUMBASIS, 0);	//CHANGE: MODEL.b[i].Kbase for i>basisID				
-
-						precFunc.GetNumTermsPerPrecGrp(&MODEL); //CHANGE: (1) nothing or (2) MODEL.curr.nTermsPerPrecGrp + MODEL.b[id].offsetPrec								
-						precFunc.GetXtXPrecDiag(&MODEL);        //CHANGE: (1)nothing or (2) MODEL.curr.precXtXDiag
-
-						// Find candidate positions for SEASON AND TREND				
-						// nMissing & rowsMissing used for the outlier function
-						CvtKnotsToBinVec(MODEL.b, MODEL.NUMBASIS, N, &yInfo);
-
-						//Evaluate the initial model and compute its marg lik. CHANGE: DERIVE XMARS, K, BETA, BETA_MEAN, MARG_LIK
-						// Xtmars is a cotinguous mem block consiting of Xtmars, Xnewterm, and Xt_zerobackup. The first part will
-						// be filled with Xtmars, and the rest will be used as a temp block in this function call.
-						// We don't use Xnewterm  or Xt_zerobackup as a temp mem buf bcz the zeroOutXmars function may need a much
-						// larger  mem due to the many terms of the inital random model	
-						// basis->K won't be updated inside the function and the old values from CalcBasisKsKeK is kept
-						if (q == 1) {
-							BEAST2_EvaluateModel(&MODEL.curr, MODEL.b, Xt_mars, N, MODEL.NUMBASIS, &yInfo, &hyperPar, &opt->prior.precValue, &stream);
-						}
-						else {
-							MR_EvaluateModel(&MODEL.curr, MODEL.b, Xt_mars, N, MODEL.NUMBASIS, &yInfo, &hyperPar, &opt->prior.precValue, &stream);
+						FILL0(MODEL.prop.XtX + (NewCol.k1 - 1) * KNEW, (KNEW - NewCol.k1 + 1) * KNEW); // zero out the cols from k1-th to the end
+						if (NewCol.k1 > 1) {
+							/*
+							I32 r1 = NEW.r1[0];
+							I32 r2 = NEW.r2[NEW.numSeg - 1];
+							I32 Nseg = r2 - r1 + 1;
+							r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, \
+								NEW.k1 - 1L, Knewterm, Nseg, 1.0f, \
+								Xt_mars  + r1-1L, Npad,
+								Xnewterm + r1-1L, Npad, 0.f, \
+								MODEL.prop.XtX + (NEW.k1 - 1L) * KNEW, KNEW); //0.f, MEMBUF1, k1_new - 1);
+							*/
+							// Xnewterm is pre-allocated with sufficent mem to ensure segInfo won't overflow in __GetMAXNumElemXnewTerm
+							BEAST2_BASESEG* _segInfo = (BEAST2_BASESEG*)(Xnewterm + Knewterm * Npad);
+							I32             _numBands = GetInfoBandList(_segInfo, &MODEL, NewCol.k1 - 1);
+							MatxMat(_segInfo, _numBands, Xt_mars,
+								NEW.SEG,   NEW.numSeg, Xnewterm,
+								MODEL.prop.XtX + (NewCol.k1 - 1L) * KNEW, N, KNEW);
 						}
 
-					}
-
-
-					{
-						// Clear up and zero out resultChain for initialization
-						BEAST2_Result_FillMEM(&resultChain, opt, 0);
+						/*
+						  r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans,
+						   Knewterm, Knewterm, Nseg, 1.0,
+						   Xnewterm + r1 - 1, Npad,
+						   Xnewterm + r1 - 1, Npad, 0.f,
+						   MODEL.prop.XtX + (NEW.k1-1) * KNEW + NEW.k1 - 1, KNEW);// MEMBUF2, K_newTerm);
+						*/
+						//XnewtermTXnewterm(&NEW, Xnewterm, MODEL.prop.XtX + (NEW.k1 - 1) * KNEW + NEW.k1 - 1, Npad, KNEW);
+						XtX_ByGroup(NEW.SEG, NEW.numSeg, Xnewterm, MODEL.prop.XtX + (NewCol.k1 - 1) * KNEW + NewCol.k1 - 1, N, KNEW);
 
-						// Reset all nots to ones bcz the real extrem positiosn won'tY be updated till samples > 1
-						memset(MODEL.extremePosVec, 1, N);
-						for (I32 i = 0; i < yInfo.nMissing; ++i) MODEL.extremePosVec[yInfo.rowsMissing[i]] = 0;
-						MODEL.extremPosNum = yInfo.n;
+						/* //After obtaining Xnewterm'*Xnewterm, insert it into XtX_prop at appropriate locations
+							for (rI32 i = k1_new, j = 1; i <= k2_new; i++, j++) {
+								if (k1_new != 1) r_cblas_scopy(k1_new - 1, MEMBUF1 + (j - 1)*(k1_new - 1), 1, XtX_prop + (i - 1)*KNEW, 1);
+								r_cblas_scopy(j, MEMBUF2 + (j - 1)*K_newTerm, 1, XtX_prop + (i - 1)*KNEW + k1_new - 1, 1);}
+						*/
 					}
-
-					/**********************************************************************************************/
-					// PREPARE FOR THE START OF THE MAIN LOOP
-					// The proposed basis needs XtX and XtY of the current basis to compute XtX_prop and XtY_prop.
-					// Other varialbes (e.g., beta and cholXtX) are not cross-used by the basis and basis_prop
-					/**********************************************************************************************/
-					U32 ite = 0;
-					U32 sample = 0;
-
-					/*************************************************************/
-					// samplesInserted must be reset to zero at the start of each chain
-					/*************************************************************/
-					if (extra.computeCredible) {
-						for (int i = 0; i < MODEL.NUMBASIS; i++) {
-							ci[i].samplesInserted = 0;
+					/*{ 
+					cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, k1_new - 1, K_newTerm, N, 1, X_mars, N, X_mars_prop + (k1_new - 1)*N, N, 0, GlobalMEMBuf_1st, k1_new - 1);
+					for (int i = k1_new, j = 1; i <= k2_new; i++, j++)
+					r_cblas_scopy(k1_new - 1, GlobalMEMBuf_1st + (j - 1)*(k1_new - 1), 1, XtX_prop + (i - 1)*KNEW, 1);
+					cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, K_newTerm, K_newTerm, N, 1, X_mars_prop + (k1_new - 1)*N, N, X_mars_prop + (k1_new - 1)*N, N, 0, GlobalMEMBuf_1st, K_newTerm);
+					for (int i = k1_new, j = 1; i <= k2_new; i++, j++)
+					r_cblas_scopy(j, GlobalMEMBuf_1st + (j - 1)*K_newTerm, 1, XtX_prop + (i - 1)*KNEW + k1_new - 1, 1);
+					}*/
+
+					/*************************************************************************/
+					//                  The THRID component: 
+					/*************************************************************************/
+					//There is no third componet if k2_old=KOLD 
+					if (NewCol.k2_old != KOLD) {
+						/*for (rI32  j = 1; i <= KOLD; i++, j++) {r_cblas_scopy(K_newTerm,  MEMBUF1 + (j - 1)*K_newTerm, 1, XtX_prop + (k - 1)*KNEW + k1_new - 1, 1),					*/
+						for (I32 kold = NewCol.k2_old + 1, knew = NewCol.k2_new + 1; kold <= KOLD; kold++, knew++) {
+							F32PTR ColStart_old = MODEL.curr.XtX + (kold - 1) * KOLD;
+							F32PTR ColStart_new = MODEL.prop.XtX + (knew - 1) * KNEW;
+							SCPY(NewCol.k1 - 1,        ColStart_old, ColStart_new); //the upper part of the third componet
+							SCPY(kold - NewCol.k2_old, ColStart_old + (NewCol.k2_old + 1) - 1, ColStart_new + (NewCol.k2_new + 1) - 1); // the bottom part of the 3rd cmpnt
+						}
+
+						// If there is a MIDDLE part of the componet (i.e, Knewterm>0); this part 
+						// will be missing if flag is resmaplingOder and isInsert = 0.
+						if (Knewterm != 0) {
+							/*
+							  rI32 r1 = NEW.r1[0];
+							  rI32 r2 = NEW.r2[NEW.numSeg - 1];
+							  rI32 Nseg = r2 - r1 + 1;
+							  r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans,
+								  Knewterm, (KOLD - NEW.k2_old), Nseg, 1,
+								  Xnewterm + r1 - 1, Npad,
+								  Xt_mars + (NEW.k2_old + 1 - 1) * Npad + r1 - 1, Npad, 0,
+								  MODEL.prop.XtX + (NEW.k2_new+1L-1L) * KNEW + NEW.k1 - 1, KNEW );//MEMBUF1, K_newTerm);
+							 */
+							BEAST2_BASESEG* _segInfo = (BEAST2_BASESEG*)(Xnewterm + Knewterm * Npad);
+							I32             _numBands = GetInfoBandList_post(_segInfo, &MODEL, NewCol.k2_old + 1);
+							MatxMat(NEW.SEG, NEW.numSeg, Xnewterm, _segInfo, _numBands, Xt_mars + NewCol.k2_old * Npad,
+									MODEL.prop.XtX + (NewCol.k2_new + 1 - 1) * KNEW + NewCol.k1 - 1, N, KNEW);
 						}
+
 					}
 
-					PROP_DATA PROPINFO = { .N = N,                   .Npad16 = Npad16,   .samples = &sample,
-										  .keyresult = coreResults, .mem = Xnewterm, .model = &MODEL,
-										  .pRND = &RND,            .yInfo = &yInfo,    .nSample_ExtremVecNeedUpdate = 1L,
-										  .sigFactor = opt->prior.sigFactor,          .outlierSigFactor = opt->prior.outlierSigFactor,
-					};
-
-					NEWTERM        NEW;     // moved here bvz its xcols has two fixed lements, N and Npad
-					NEWCOLINFO     NewCol; // moved here bvz its xcols has two fixed lements, N and Npad
-					NewCol.N = N;
-					NewCol.Nlda = Npad;
+					/*********************************************************************************/
+					//                 Compute XtY_prop from XtY
+					/********************************************************************************/
+					if (q == 1) {
 
-					I32 numBadIterations = 0;
-					while (sample < MCMC_SAMPLES)
-					{
-						ite++;
-						/**********************************************************************/
-						/*     Re-generate a pool of random numbers if almost used up          */
-						/***********************************************************************/
-						//vsRngUniform(VSL_RNG_METHOD_UNIFORM_STD_ACCURATE, stream, MAX_RAND_NUM, rnd32, 0.f, 1.0f);
-						if (RND.rnd32 >= RND32_END) { r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, (RND.rnd32 - RND32), (U32PTR)RND32);	                               RND.rnd32 = RND32; }
-						if (RND.rnd16 >= RND16_END) { r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, ((char*)RND.rnd16 - (char*)RND16 + 3) / sizeof(U32), (U32PTR)RND16); RND.rnd16 = RND16; }
-						if (RND.rnd08 >= RND08_END) { r_viRngUniformBits32(VSL_RNG_METHOD_UNIFORMBITS32_STD, stream, ((char*)RND.rnd08 - (char*)RND08 + 3) / sizeof(U32), (U32PTR)RND08); RND.rnd08 = RND08; }
-						if (RND.rndgamma >= RNDGAMMA_END) { r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, MAX_RAND_NUM, RNDGAMMA, (hyperPar.alpha_1 + yInfo.n * 0.5f), 0.f, 1.f);    RND.rndgamma = RNDGAMMA; }
-
-						//  Choose a basis type	
-						BEAST2_BASIS_PTR basis = MODEL.b + MODEL.PickBasisID(&PROPINFO); //basisID = *RND.rnd08++ < 128;				
-
-						// IMPLEMENT THE NEW PROPOSED BASIS	
-						//CHANGE: new.newKnot, numSeg, SEG/R1/2, orders2, newIdx, nKnot_new, jumpType,propinfo.pRND.rnd8/32				
-						basis->Propose(basis, &NEW, &NewCol, &PROPINFO); //info->mem=Xnewterm is used as a temp membuf here
-
-#ifdef __DEBUG__
-						I32 basisIdx = basis - MODEL.b;
-						flagSat[NEW.newKnot - 1] += basisIdx == 0 && (NEW.jumpType == BIRTH || NEW.jumpType == MOVE);
-						if (basisIdx == 0) ++(flagS[NEW.jumpType]);
-						else 		       ++(flagT[NEW.jumpType]);
-#endif
+						// Skipped if k1_old=1 when dealing with SEASON
+						if (NewCol.k1 > 1)         SCPY(NewCol.k1 - 1, MODEL.curr.XtY, MODEL.prop.XtY);
+						// New components : XnewTemrm*Y
+						if (Knewterm > 0)  	          MatxVec(NEW.SEG, NEW.numSeg, Xnewterm, yInfo.Y, MODEL.prop.XtY + NewCol.k1 - 1, N);
+						//this part will be skipped if k2_old=KOLD when dealing with TREND(Istrend==1)
+						if (NewCol.k2_old != KOLD) SCPY(KNEW - NewCol.k2_new, MODEL.curr.XtY + (NewCol.k2_old + 1L) - 1L, MODEL.prop.XtY + (NewCol.k2_new + 1) - 1);
 
-						/**********************************************************************/
-						// Generate the new terms for the propsed step: To add or move a bk, two segments 
-						// are re-generated; to remove a bk or merge two bks, one segment are re-generated.	
-						/**********************************************************************/
-						I32 Knewterm = 0;
-						for (I32 i = 0; i < NEW.numSeg; i++) {
-							// NEW.numSeg is 0 if removing terms for ChORDER(newOrder<oldeTerm)
-							// [1]..(1)....(2)...(sY-1)...N [N+1] 
-							I32 kterms = NEW.SEG[i].K = basis->GenTerms(Xnewterm + Npad * Knewterm, N, &NEW.SEG[i], &(basis->bConst));
-							Knewterm += kterms;
-						} // Iterate through all the new segments
-
-						NewCol.k2_new = NewCol.k1 + Knewterm - 1L;	// if Knewterm=0 (i.e., delete terms), k2_new < k1_new
-
-						//Get k1_old, k2_old, k1_new and k2_new
-						NewCol.k1 += basis->Kbase;		// k1=k1_new=k1_old
-						NewCol.k2_old += basis->Kbase;
-						NewCol.k2_new += basis->Kbase;
-
-						I32 KOLD = MODEL.curr.K;                         // Total number of basis for the current model				
-						I32 KNEW = KOLD + NewCol.k2_new - NewCol.k2_old; // Total number of bases in the proposed model	
-
-						NewCol.Knewterm = Knewterm;
-						NewCol.KOLD = KOLD;
-						NewCol.KNEW = KNEW;
-
-						/*************************************************************************/
-						// Get XtX_prop: Copy parts of XtX to XtT_prop and fill new components 
-						/*************************************************************************/
-						// Set those rows of Xt_mars_newterms specfied by rowsMissing  to zeros
-						if (yInfo.nMissing > 0 && Knewterm > 0 /*&& basis->type != OUTLIERID*/)  //needed for basisFunction_OUliter=1
-							f32_mat_multirows_extract_set_by_scalar(Xnewterm, Npad, Knewterm, Xt_zeroBackup, yInfo.rowsMissing, yInfo.nMissing, 0.0f);
-
-
-						if (!GROUP_MatxMat) {
-							update_XtX_from_Xnewterm(Xt_mars, Xnewterm, MODEL.curr.XtX, MODEL.prop.XtX, &NewCol);
-							update_XtY_from_Xnewterm(yInfo.Y, Xnewterm, MODEL.curr.XtY, MODEL.prop.XtY, &NewCol, q);
-						}
-						else {
+					}	else {
+						// FOR MrBEAST
 
-							/*************************************************************************/
-							//               The FIRST component:	
-							/*************************************************************************/
-							// There'sY no first component if k1_old/k1_new=1 for SEASON	
-							for (I32 i = 1; i < NewCol.k1; i++) SCPY(i, MODEL.curr.XtX + (i - 1L) * KOLD, MODEL.prop.XtX + (i - 1L) * KNEW);
-
-							/*************************************************************************/
-							//              The SECOND component
-							/*************************************************************************/
-							// No new cols/terms if flag=ChORDER && isInsert=0:the resampled basis has a higher order than the old basis
-							if (Knewterm != 0) {
-
-								FILL0(MODEL.prop.XtX + (NewCol.k1 - 1) * KNEW, (KNEW - NewCol.k1 + 1) * KNEW); // zero out the cols from k1-th to the end
-								if (NewCol.k1 > 1) {
-									/*
-									I32 r1 = NEW.r1[0];
-									I32 r2 = NEW.r2[NEW.numSeg - 1];
-									I32 Nseg = r2 - r1 + 1;
-									r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, \
-										NEW.k1 - 1L, Knewterm, Nseg, 1.0f, \
-										Xt_mars  + r1-1L, Npad,
-										Xnewterm + r1-1L, Npad, 0.f, \
-										MODEL.prop.XtX + (NEW.k1 - 1L) * KNEW, KNEW); //0.f, MEMBUF1, k1_new - 1);
-									*/
-									// Xnewterm is pre-allocated with sufficent mem to ensure segInfo won't overflow in __GetMAXNumElemXnewTerm
-									BEAST2_BASESEG* _segInfo = (BEAST2_BASESEG*)(Xnewterm + Knewterm * Npad);
-									I32             _numBands = GetInfoBandList(_segInfo, &MODEL, NewCol.k1 - 1);
-									MatxMat(_segInfo, _numBands, Xt_mars,
-										NEW.SEG, NEW.numSeg, Xnewterm,
-										MODEL.prop.XtX + (NewCol.k1 - 1L) * KNEW, N, KNEW);
-								}
-
-								/*
-								  r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans,
-								   Knewterm, Knewterm, Nseg, 1.0,
-								   Xnewterm + r1 - 1, Npad,
-								   Xnewterm + r1 - 1, Npad, 0.f,
-								   MODEL.prop.XtX + (NEW.k1-1) * KNEW + NEW.k1 - 1, KNEW);// MEMBUF2, K_newTerm);
-								*/
-								//XnewtermTXnewterm(&NEW, Xnewterm, MODEL.prop.XtX + (NEW.k1 - 1) * KNEW + NEW.k1 - 1, Npad, KNEW);
-								XtX_ByGroup(NEW.SEG, NEW.numSeg, Xnewterm, MODEL.prop.XtX + (NewCol.k1 - 1) * KNEW + NewCol.k1 - 1, N, KNEW);
-
-								/* //After obtaining Xnewterm'*Xnewterm, insert it into XtX_prop at appropriate locations
-									for (rI32 i = k1_new, j = 1; i <= k2_new; i++, j++) {
-										if (k1_new != 1) r_cblas_scopy(k1_new - 1, MEMBUF1 + (j - 1)*(k1_new - 1), 1, XtX_prop + (i - 1)*KNEW, 1);
-										r_cblas_scopy(j, MEMBUF2 + (j - 1)*K_newTerm, 1, XtX_prop + (i - 1)*KNEW + k1_new - 1, 1);}
-								*/
+						// Skipped if k1_old=1 when dealing with SEASON
+						if (NewCol.k1 > 1) {
+							for (I32 c = 0; c < q; ++c) {
+								SCPY(NewCol.k1 - 1, MODEL.curr.XtY + KOLD * c, MODEL.prop.XtY + KNEW * c);
 							}
-							/*{
-							cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, k1_new - 1, K_newTerm, N, 1, X_mars, N, X_mars_prop + (k1_new - 1)*N, N, 0, GlobalMEMBuf_1st, k1_new - 1);
-							for (int i = k1_new, j = 1; i <= k2_new; i++, j++)
-							r_cblas_scopy(k1_new - 1, GlobalMEMBuf_1st + (j - 1)*(k1_new - 1), 1, XtX_prop + (i - 1)*KNEW, 1);
-							cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, K_newTerm, K_newTerm, N, 1, X_mars_prop + (k1_new - 1)*N, N, X_mars_prop + (k1_new - 1)*N, N, 0, GlobalMEMBuf_1st, K_newTerm);
-							for (int i = k1_new, j = 1; i <= k2_new; i++, j++)
-							r_cblas_scopy(j, GlobalMEMBuf_1st + (j - 1)*K_newTerm, 1, XtX_prop + (i - 1)*KNEW + k1_new - 1, 1);
-							}*/
-
-							/*************************************************************************/
-							//                  The THRID component: 
-							/*************************************************************************/
-							//There is no third componet if k2_old=KOLD 
-							if (NewCol.k2_old != KOLD) {
-								/*for (rI32  j = 1; i <= KOLD; i++, j++) {r_cblas_scopy(K_newTerm,  MEMBUF1 + (j - 1)*K_newTerm, 1, XtX_prop + (k - 1)*KNEW + k1_new - 1, 1),					*/
-								for (I32 kold = NewCol.k2_old + 1, knew = NewCol.k2_new + 1; kold <= KOLD; kold++, knew++) {
-									F32PTR ColStart_old = MODEL.curr.XtX + (kold - 1) * KOLD;
-									F32PTR ColStart_new = MODEL.prop.XtX + (knew - 1) * KNEW;
-									SCPY(NewCol.k1 - 1, ColStart_old, ColStart_new); //the upper part of the third componet
-									SCPY(kold - NewCol.k2_old, ColStart_old + (NewCol.k2_old + 1) - 1, ColStart_new + (NewCol.k2_new + 1) - 1); // the bottom part of the 3rd cmpnt
-								}
-
-								// If there is a MIDDLE part of the componet (i.e, Knewterm>0); this part 
-								// will be missing if flag is resmaplingOder and isInsert = 0.
-								if (Knewterm != 0) {
-									/*
-									  rI32 r1 = NEW.r1[0];
-									  rI32 r2 = NEW.r2[NEW.numSeg - 1];
-									  rI32 Nseg = r2 - r1 + 1;
-									  r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans,
-										  Knewterm, (KOLD - NEW.k2_old), Nseg, 1,
-										  Xnewterm + r1 - 1, Npad,
-										  Xt_mars + (NEW.k2_old + 1 - 1) * Npad + r1 - 1, Npad, 0,
-										  MODEL.prop.XtX + (NEW.k2_new+1L-1L) * KNEW + NEW.k1 - 1, KNEW );//MEMBUF1, K_newTerm);
-									 */
-									BEAST2_BASESEG* _segInfo = (BEAST2_BASESEG*)(Xnewterm + Knewterm * Npad);
-									I32             _numBands = GetInfoBandList_post(_segInfo, &MODEL, NewCol.k2_old + 1);
-									MatxMat(NEW.SEG, NEW.numSeg, Xnewterm, _segInfo, _numBands, Xt_mars + NewCol.k2_old * Npad,
-										MODEL.prop.XtX + (NewCol.k2_new + 1 - 1) * KNEW + NewCol.k1 - 1, N, KNEW);
-								}
-
-							}
-
-							/*********************************************************************************/
-							//                 Compute XtY_prop from XtY
-							/********************************************************************************/
-							if (q == 1) {
-
-								// Skipped if k1_old=1 when dealing with SEASON
-								if (NewCol.k1 > 1)         SCPY(NewCol.k1 - 1, MODEL.curr.XtY, MODEL.prop.XtY);
-								// New components : XnewTemrm*Y
-								if (Knewterm > 0)  	          MatxVec(NEW.SEG, NEW.numSeg, Xnewterm, yInfo.Y, MODEL.prop.XtY + NewCol.k1 - 1, N);
-								//this part will be skipped if k2_old=KOLD when dealing with TREND(Istrend==1)
-								if (NewCol.k2_old != KOLD) SCPY(KNEW - NewCol.k2_new, MODEL.curr.XtY + (NewCol.k2_old + 1L) - 1L, MODEL.prop.XtY + (NewCol.k2_new + 1) - 1);
-
+						}
+						// New components : XnewTemrm*Y
+						if (Knewterm > 0) {
+							//MatxVec(NEW.SEG, NEW.numSeg, Xnewterm, yInfo.Y, MODEL.prop.XtY + NEW.k1 - 1, N);
+							r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, Knewterm, q, N, 1.f, Xnewterm, Npad, yInfo.Y, N, 0.f,
+								MODEL.prop.XtY + NewCol.k1 - 1, KNEW);
+						}
+						//this part will be skipped if k2_old=KOLD when dealing with TREND(Istrend==1)
+						if (NewCol.k2_old != KOLD) {
+							for (I32 c = 0; c < q; ++c) {
+								SCPY(KNEW - NewCol.k2_new, MODEL.curr.XtY + (NewCol.k2_old + 1L) - 1L + KOLD * c, MODEL.prop.XtY + (NewCol.k2_new + 1) - 1 + KNEW * c);
 							}
-							else {
-								// FOR MrBEAST
-
-								// Skipped if k1_old=1 when dealing with SEASON
-								if (NewCol.k1 > 1) {
-									for (I32 c = 0; c < q; ++c) {
-										SCPY(NewCol.k1 - 1, MODEL.curr.XtY + KOLD * c, MODEL.prop.XtY + KNEW * c);
-									}
-								}
-								// New components : XnewTemrm*Y
-								if (Knewterm > 0) {
-									//MatxVec(NEW.SEG, NEW.numSeg, Xnewterm, yInfo.Y, MODEL.prop.XtY + NEW.k1 - 1, N);
-									r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, Knewterm, q, N, 1.f, Xnewterm, Npad, yInfo.Y, N, 0.f,
-										MODEL.prop.XtY + NewCol.k1 - 1, KNEW);
-								}
-								//this part will be skipped if k2_old=KOLD when dealing with TREND(Istrend==1)
-								if (NewCol.k2_old != KOLD) {
-									for (I32 c = 0; c < q; ++c) {
-										SCPY(KNEW - NewCol.k2_new, MODEL.curr.XtY + (NewCol.k2_old + 1L) - 1L + KOLD * c, MODEL.prop.XtY + (NewCol.k2_new + 1) - 1 + KNEW * c);
-									}
-								}
-
-
-							} //if (q == 1) 
-
 						}
 
-						/*************************************************************/
-						// XtX_prop has been constructed. Now use it to get the marg lik
-						/***************************************************************/
-						if (1L) {
-							//Add precison values to the diagonal of XtX: post_P=XtX +diag(prec) 
-							/*
-							//Solve inv(Post_P)*XtY using  Post_P*b=XtY to get beta_mean
-							//lapack_int LAPACKE_spotrf(int matrix_layout, char uplo, lapack_int n, double * a, lapack_int lda);
-							r_LAPACKE_spotrf(LAPACK_COL_MAJOR, 'U', KNEW, MODEL.prop.cholXtX, KNEW); // Choleskey decomposition; only the upper triagnle elements are used
-							*/
-							for (I32 i = 1; i < NewCol.k1; i++)
-								SCPY(i, MODEL.curr.cholXtX + (i - 1) * KOLD, MODEL.prop.cholXtX + (i - 1) * KNEW);
 
-							precFunc.UpdateXtXPrec_nTermsPerGrp(&MODEL, basis, &NEW, &NewCol); //&NEW is used only for OrderWise
-							precFunc.chol_addCol(MODEL.prop.XtX + (NewCol.k1 - 1) * KNEW,
-								MODEL.prop.cholXtX,
-								MODEL.prop.precXtXDiag, KNEW, NewCol.k1, KNEW);
-							//chol_full_v2(MODEL.prop.XtX, MODEL.prop.cholXtX, KNEW, KNEW);
-						   /*
-							for (rI32 i = 1; i <= (NEW.k1_new - 1L); i++) 	r_cblas_scopy(i, MODEL.curr.cholXtX + (i - 1L) * KOLD, 1L, MODEL.prop.cholXtX + (i - 1L) * KNEW, 1L);
-							chol_addCol(MODEL.prop.cholXtX+ (NEW.k1_new - 1L)*KNEW, MODEL.prop.cholXtX, KNEW, NEW.k1_new, KNEW);
-							//chol_addCol(MODEL.prop.cholXtX + (1 - 1L) * KNEW, MODEL.prop.cholXtX, KNEW, 1, KNEW);
-							*/
+					} //if (q == 1) 
+				
+				}
 
-							/*{
-							//LAPACKE_dpotrs (int matrix_layout , char uplo , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
-							SCPY(KNEW, MODEL.prop.XtY, MODEL.prop.beta_mean);
-							r_LAPACKE_spotrs(LAPACK_COL_MAJOR, 'U', KNEW, 1, MODEL.prop.cholXtX, KNEW, MODEL.prop.beta_mean, KNEW);
-							}*/
-
-							// prop.K is needed for computing prop.marg_Lik
-							// In MODEL, basis's K is still the old ones. They will be updated only if the proposal is accetped
-							// via basis->CalcBasisKsKeK_TermType(basis). The Ks of the proposed bases are stored in MODEL.prop.ntermP				   
-							MODEL.prop.K = KNEW;
-							precFunc.ComputeMargLik(&MODEL.prop, &MODEL, &yInfo, &hyperPar);
-							//if (MODEL.prop.marg_lik != MODEL.prop.marg_lik || fabs(MODEL.prop.marg_lik )>FLOAT_MAX || MODEL.prop.alpha2_star <0.f) {					   				  
-
-							if (IsNaN(MODEL.prop.marg_lik) || IsInf(MODEL.prop.marg_lik)) {
-								if (++numBadIterations < 15) {
-
-									precFunc.IncreasePrecValues(&MODEL);
-									precFunc.GetXtXPrecDiag(&MODEL);
-									precFunc.chol_addCol(MODEL.curr.XtX, MODEL.curr.cholXtX, MODEL.curr.precXtXDiag, MODEL.curr.K, 1L, MODEL.curr.K);
-									precFunc.ComputeMargLik(&MODEL.curr, &MODEL, &yInfo, &hyperPar);
+				/*************************************************************/
+				// XtX_prop has been constructed. Now use it to get the marg lik
+				/***************************************************************/			
+				if (1L) {		
+					//Add precison values to the diagonal of XtX: post_P=XtX +diag(prec) 
+					/*
+					//Solve inv(Post_P)*XtY using  Post_P*b=XtY to get beta_mean
+					//lapack_int LAPACKE_spotrf(int matrix_layout, char uplo, lapack_int n, double * a, lapack_int lda);
+					r_LAPACKE_spotrf(LAPACK_COL_MAJOR, 'U', KNEW, MODEL.prop.cholXtX, KNEW); // Choleskey decomposition; only the upper triagnle elements are used
+					*/
+					for (I32 i=1; i<NewCol.k1; i++) 
+						SCPY(i, MODEL.curr.cholXtX+(i-1)*KOLD, MODEL.prop.cholXtX+(i-1)*KNEW);
+
+					precFunc.UpdateXtXPrec_nTermsPerGrp(&MODEL, basis, &NEW, &NewCol); //&NEW is used only for OrderWise
+					precFunc.chol_addCol(  MODEL.prop.XtX  + (NewCol.k1-1)*KNEW,
+							               MODEL.prop.cholXtX,
+							               MODEL.prop.precXtXDiag, KNEW, NewCol.k1, KNEW);
+					//chol_full_v2(MODEL.prop.XtX, MODEL.prop.cholXtX, KNEW, KNEW);
+			       /*
+					for (rI32 i = 1; i <= (NEW.k1_new - 1L); i++) 	r_cblas_scopy(i, MODEL.curr.cholXtX + (i - 1L) * KOLD, 1L, MODEL.prop.cholXtX + (i - 1L) * KNEW, 1L);
+					chol_addCol(MODEL.prop.cholXtX+ (NEW.k1_new - 1L)*KNEW, MODEL.prop.cholXtX, KNEW, NEW.k1_new, KNEW);
+					//chol_addCol(MODEL.prop.cholXtX + (1 - 1L) * KNEW, MODEL.prop.cholXtX, KNEW, 1, KNEW);
+					*/
+
+					/*{
+					//LAPACKE_dpotrs (int matrix_layout , char uplo , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );			
+					SCPY(KNEW, MODEL.prop.XtY, MODEL.prop.beta_mean);
+					r_LAPACKE_spotrs(LAPACK_COL_MAJOR, 'U', KNEW, 1, MODEL.prop.cholXtX, KNEW, MODEL.prop.beta_mean, KNEW);
+					}*/
+
+					// prop.K is needed for computing prop.marg_Lik
+					// In MODEL, basis's K is still the old ones. They will be updated only if the proposal is accetped
+					// via basis->CalcBasisKsKeK_TermType(basis). The Ks of the proposed bases are stored in MODEL.prop.ntermP				   
+				   MODEL.prop.K = KNEW;
+				   precFunc.ComputeMargLik(&MODEL.prop, &MODEL, &yInfo, &hyperPar);
+				   //if (MODEL.prop.marg_lik != MODEL.prop.marg_lik || fabs(MODEL.prop.marg_lik )>FLOAT_MAX || MODEL.prop.alpha2_star <0.f) {					   				  
+
+				   if ( IsNaN(MODEL.prop.marg_lik) || IsInf(MODEL.prop.marg_lik ) ) {
+					   if (++numBadIterations < 15) {
+					    	   
+						   precFunc.IncreasePrecValues(&MODEL);
+						   precFunc.GetXtXPrecDiag(&MODEL);
+						   precFunc.chol_addCol(MODEL.curr.XtX, MODEL.curr.cholXtX, MODEL.curr.precXtXDiag, MODEL.curr.K, 1L, MODEL.curr.K);
+						   precFunc.ComputeMargLik(&MODEL.curr, &MODEL, &yInfo, &hyperPar);
+
+						   #if !(defined(R_RELEASE) || defined(M_RELEASE))
+						   r_printf("prec: %.4f| marg_lik_prop: %.4f | marg_like_curr: %.4f \n", MODEL.precVec[0], MODEL.prop.marg_lik, MODEL.curr.marg_lik);
+						   #endif
+
+						   continue;
+					   }  else {
+						   skipCurrentPixel = 2;
+						   break;
+					   }					   
+				   }  else {
+					   numBadIterations = 0;
+				   } //if (marg_lik_prop != marg_lik_prop || alpha2_star_prop <0.f) 
+
+				   if (q == 1) {// added for MRBEAST
+					   MODEL.prop.alpha2Q_star[0] = max(MODEL.prop.alpha2Q_star[0], MIN_ALPHA2_VALUE);
+				   }
+				}
 
-#if !(defined(R_RELEASE) || defined(M_RELEASE))
-									r_printf("prec: %.4f| marg_lik_prop: %.4f | marg_like_curr: %.4f \n", MODEL.precVec[0], MODEL.prop.marg_lik, MODEL.curr.marg_lik);
-#endif
+			   /****************************************************************************************/
+			   /*    DETERMINE WHETHER OR NOT TO ACCCEPT THE PROPSOED STEP                              */
+			   /****************************************************************************************/
+			
+				// First, calcuate a factor adjusting the likelihood change
+				F32  factor;				
+				if   ( NEW.jumpType ==MOVE || basis->type ==OUTLIERID) 	factor = 0.;
+				else { factor = basis->ModelPrior(basis, &NewCol, &NEW); }
+
+				F32 delta_lik = MODEL.prop.marg_lik - MODEL.curr.marg_lik + factor;
+				
+				//acceptTheProposal = *(RND.rnd16)++ < fastexp(delta_lik) * 65535.0f;				
+				I08     acceptTheProposal;
+				if      (delta_lik >   0)   acceptTheProposal = 1;
+				else if (delta_lik < -23) 	acceptTheProposal = 0;				
+				else {				 
+					F32    expValue = fastexp(delta_lik);
+					if     (delta_lik > -0.5) 	acceptTheProposal = *(RND.rnd08)++ < expValue * 255.0f;
+					else if(delta_lik > -5  )   acceptTheProposal = *(RND.rnd16)++ < expValue * 65535.0f;
+					else						acceptTheProposal = *(RND.rnd32)++ < expValue * 4.294967296e+09;
+					 
+				}
+	 
 
-									continue;
-								}
-								else {
-									skipCurrentPixel = 2;
-									break;
-								}
-							}
-							else {
-								numBadIterations = 0;
-							} //if (marg_lik_prop != marg_lik_prop || alpha2_star_prop <0.f) 
+				if(acceptTheProposal) 
+				{
+					//Recover the orignal vaules for those rows corresponding to missing Y values
+					if (yInfo.nMissing > 0 && Knewterm > 0 /*&& basis->type != OUTLIERID*/)  //needed for basisFunction_OUliter=1						
+						f32_mat_multirows_set_by_submat(Xnewterm, Npad, Knewterm, Xt_zeroBackup, yInfo.rowsMissing, yInfo.nMissing);
+
+					// Inserting XnewTerms into Xt_mars
+					if (NewCol.k2_old != KOLD && NewCol.k2_new != NewCol.k2_old)
+						shift_lastcols_within_matrix(Xt_mars, Npad, NewCol.k2_old+1, KOLD, NewCol.k2_new+1);
+					if (Knewterm != 0)
+						SCPY(Knewterm*Npad, Xnewterm, Xt_mars + (NewCol.k1-1) * Npad);
+					
+					/****************************************************/
+					//Find the good positions of the proposed MOVE
+					//Then update the knotLists and order
+					/****************************************************/
+					basis->UpdateGoodVec(basis, &NEW, Npad16);
+					basis->CalcBasisKsKeK_TermType(basis);
+					UpdateBasisKbase(MODEL.b, MODEL.NUMBASIS, basis-MODEL.b);//basisIdx=basis-b Re-compute the K indices of the bases after the basisID 
+	
+					//Switching between Basis and Basis_prop
+					{
+						//http: //stackoverflow.com/questions/3647331/how-to-swap-two-numbers-without-using-temp-variables-or-arithmetic-operations
+						//basis  = ((I64)basis ^ (I64)basis_prop);basis_prop = ((I64)basis ^ (I64)basis_prop); basis      =  ((I64)basis ^ (I64)basis_prop);						
+					
+						#define Exchange(x,y)   {void * _restrict tmp; tmp=MODEL.x;  MODEL.x=MODEL.y; MODEL.y=tmp;}
+						Exchange(curr.XtX,       prop.XtX);
+						Exchange(curr.XtY,       prop.XtY);
+						Exchange(curr.beta_mean, prop.beta_mean);
+						//Exchange(curr.beta,      prop.beta);                    // no need to exchange
+						Exchange(curr.cholXtX,          prop.cholXtX);
+						Exchange(curr.precXtXDiag,      prop.precXtXDiag);        // needed for compontwise and orderwise
+						Exchange(curr.nTermsPerPrecGrp, prop.nTermsPerPrecGrp);   // needed for compontwise and orderwise
+
+						Exchange(curr.alpha2Q_star, prop.alpha2Q_star);           // changed for MRBEAST 
+						
+						MODEL.curr.marg_lik    = MODEL.prop.marg_lik;
+						MODEL.curr.K		   = MODEL.prop.K;  //GetNumOfXmarCols(&MODEL): this function should also give KNEW; if not, there must be something wrong!
+						#undef Exchange											
+					}
+					#ifdef __DEBUG__	
+					if (q == 1) {
+						//BEAST2_EvaluateModel(&MODEL.prop, MODEL.b, Xdebug, N, MODEL.NUMBASIS, &yInfo, &hyperPar, MODEL.precVec, &stream);											
+						//r_printf("ite:%d K: |%f|%f|diff:%f\n", ite, MODEL.curr.K, MODEL.curr.marg_lik, MODEL.prop.marg_lik, MODEL.prop.marg_lik - MODEL.curr.marg_lik);
+					    //r_printf(" %f[%f]-%f %f\n", (MODEL.curr.alpha2_star), (MODEL.prop.alpha2_star),	yInfo.alpha1_star* (log(MODEL.curr.alpha2_star) - log(MODEL.prop.alpha2_star)), yInfo.alpha1_star);
+						
+						/*
+						I32 K = MODEL.prop.K;
+						for (int i = 0; i < K; ++i) {
 
-							if (q == 1) {// added for MRBEAST
-								MODEL.prop.alpha2Q_star[0] = max(MODEL.prop.alpha2Q_star[0], MIN_ALPHA2_VALUE);
-							}
-						}
-
-						/****************************************************************************************/
-						/*    DETERMINE WHETHER OR NOT TO ACCCEPT THE PROPSOED STEP                              */
-						/****************************************************************************************/
-
-						 // First, calcuate a factor adjusting the likelihood change
-						F32  factor;
-						if (NEW.jumpType == MOVE || basis->type == OUTLIERID) 	factor = 0.;
-						else { factor = basis->ModelPrior(basis, &NewCol, &NEW); }
-
-						F32 delta_lik = MODEL.prop.marg_lik - MODEL.curr.marg_lik + factor;
-
-						//acceptTheProposal = *(RND.rnd16)++ < fastexp(delta_lik) * 65535.0f;				
-						I08     acceptTheProposal;
-						if (delta_lik > 0)   acceptTheProposal = 1;
-						else if (delta_lik < -23) 	acceptTheProposal = 0;
-						else {
-							F32    expValue = fastexp(delta_lik);
-							if (delta_lik > -0.5) 	acceptTheProposal = *(RND.rnd08)++ < expValue * 255.0f;
-							else if (delta_lik > -5)   acceptTheProposal = *(RND.rnd16)++ < expValue * 65535.0f;
-							else						acceptTheProposal = *(RND.rnd32)++ < expValue * 4.294967296e+09;
+							r_printf("%f %f %f | %f %f %f\n",
+								MODEL.prop.cholXtX[i * K + i], MODEL.curr.cholXtX[i * K + i],
+								MODEL.prop.cholXtX[i * K + i] - MODEL.curr.cholXtX[i * K + i],
+								MODEL.prop.XtX[i * K + i], MODEL.curr.XtX[i * K + i],
+								MODEL.prop.XtX[i * K + i] - MODEL.curr.XtX[i * K + i]);
 
 						}
+						r_printf("ite----%d\n", ite);
+						int a = 1;
+						 */
+					}
+					else {
+						MR_EvaluateModel(&MODEL.prop, MODEL.b, Xdebug, N, MODEL.NUMBASIS, &yInfo, &hyperPar, MODEL.precVec, &stream);
+						//r_printf("MRite%d |%f|%f|diff:%f -prec %f\n", ite, MODEL.curr.marg_lik, MODEL.prop.marg_lik, MODEL.prop.marg_lik - MODEL.curr.marg_lik, MODEL.precVec[0]);
+					 
+	                    /*
+						I32 K = MODEL.prop.K;
+						for (int i = 0; i < MODEL.prop.K; ++i) {
+						 
+								r_printf("%f %f %f | %f %f %f\n", 
+									MODEL.prop.cholXtX[i*K + i], MODEL.curr.cholXtX[i * K + i],
+									MODEL.prop.cholXtX[i * K + i] - MODEL.curr.cholXtX[i * K + i],
+									MODEL.prop.XtX[i * K + i], MODEL.curr.XtX[i * K + i],
+									MODEL.prop.XtX[i * K + i] - MODEL.curr.XtX[i * K + i]);
+						 
+						}
+						
+							r_printf("ite----%d\n",ite);
+							int a = 1;
+							*/ 
+					}
 
-#ifdef __DEBUG__
-						if (basisIdx == 0) ++(flagS[NEW.jumpType]);
-						else 		       ++(flagT[NEW.jumpType]);
-#endif
-
-						if (acceptTheProposal)
-						{
-#ifdef __DEBUG__
-							if (basisIdx == 0) ++(accS[NEW.jumpType]);
-							else 		       ++(accT[NEW.jumpType]);
-#endif
+					#endif
 
-							//Recover the orignal vaules for those rows corresponding to missing Y values
-							if (yInfo.nMissing > 0 && Knewterm > 0 /*&& basis->type != OUTLIERID*/)  //needed for basisFunction_OUliter=1						
-								f32_mat_multirows_set_by_submat(Xnewterm, Npad, Knewterm, Xt_zeroBackup, yInfo.rowsMissing, yInfo.nMissing);
-
-							// Inserting XnewTerms into Xt_mars
-							if (NewCol.k2_old != KOLD && NewCol.k2_new != NewCol.k2_old)
-								MoveCOLsWithinMatrix(Xt_mars, Npad, NewCol.k2_old + 1, KOLD, NewCol.k2_new + 1);
-							if (Knewterm != 0)
-								SCPY(Knewterm * Npad, Xnewterm, Xt_mars + (NewCol.k1 - 1) * Npad);
-
-
-							/****************************************************/
-							//Find the good positions of the proposed MOVE
-							//Then update the knotLists and order
-							/****************************************************/
-							basis->UpdateGoodVec(basis, &NEW, Npad16);
-							basis->CalcBasisKsKeK_TermType(basis);
-							UpdateBasisKbase(MODEL.b, MODEL.NUMBASIS, basis - MODEL.b);//basisIdx=basis-b Re-compute the K indices of the bases after the basisID 
-
-							//Switching between Basis and Basis_prop
-							{
-								//http: //stackoverflow.com/questions/3647331/how-to-swap-two-numbers-without-using-temp-variables-or-arithmetic-operations
-								//basis  = ((I64)basis ^ (I64)basis_prop);basis_prop = ((I64)basis ^ (I64)basis_prop); basis      =  ((I64)basis ^ (I64)basis_prop);						
-
-#define Exchange(x,y)   {void * _restrict tmp; tmp=MODEL.x;  MODEL.x=MODEL.y; MODEL.y=tmp;}
-								Exchange(curr.XtX, prop.XtX);
-								Exchange(curr.XtY, prop.XtY);
-								Exchange(curr.beta_mean, prop.beta_mean);
-								//Exchange(curr.beta,      prop.beta);                    // no need to exchange
-								Exchange(curr.cholXtX, prop.cholXtX);
-								Exchange(curr.precXtXDiag, prop.precXtXDiag);        // needed for compontwise and orderwise
-								Exchange(curr.nTermsPerPrecGrp, prop.nTermsPerPrecGrp);   // needed for compontwise and orderwise
-
-								Exchange(curr.alpha2Q_star, prop.alpha2Q_star);           // changed for MRBEAST 
-
-								MODEL.curr.marg_lik = MODEL.prop.marg_lik;
-								MODEL.curr.K = MODEL.prop.K;  //GetNumOfXmarCols(&MODEL): this function should also give KNEW; if not, there must be something wrong!
-#undef Exchange											
-							}
-#ifdef __DEBUG__	
-							if (q == 1) {
-								//BEAST2_EvaluateModel(&MODEL.prop, MODEL.b, Xdebug, N, MODEL.NUMBASIS, &yInfo, &hyperPar, MODEL.precVec, &stream);											
-								//r_printf("ite:%d K: |%f|%f|diff:%f\n", ite, MODEL.curr.K, MODEL.curr.marg_lik, MODEL.prop.marg_lik, MODEL.prop.marg_lik - MODEL.curr.marg_lik);
-								//r_printf(" %f[%f]-%f %f\n", (MODEL.curr.alpha2_star), (MODEL.prop.alpha2_star),	yInfo.alpha1_star* (log(MODEL.curr.alpha2_star) - log(MODEL.prop.alpha2_star)), yInfo.alpha1_star);
-
-								/*
-								I32 K = MODEL.prop.K;
-								for (int i = 0; i < K; ++i) {
-
-									r_printf("%f %f %f | %f %f %f\n",
-										MODEL.prop.cholXtX[i * K + i], MODEL.curr.cholXtX[i * K + i],
-										MODEL.prop.cholXtX[i * K + i] - MODEL.curr.cholXtX[i * K + i],
-										MODEL.prop.XtX[i * K + i], MODEL.curr.XtX[i * K + i],
-										MODEL.prop.XtX[i * K + i] - MODEL.curr.XtX[i * K + i]);
-
-								}
-								r_printf("ite----%d\n", ite);
-								int a = 1;
-								 */
-							}
-							else {
-								MR_EvaluateModel(&MODEL.prop, MODEL.b, Xdebug, N, MODEL.NUMBASIS, &yInfo, &hyperPar, MODEL.precVec, &stream);
-								//r_printf("MRite%d |%f|%f|diff:%f -prec %f\n", ite, MODEL.curr.marg_lik, MODEL.prop.marg_lik, MODEL.prop.marg_lik - MODEL.curr.marg_lik, MODEL.precVec[0]);
-
-								/*
-								I32 K = MODEL.prop.K;
-								for (int i = 0; i < MODEL.prop.K; ++i) {
-
-										r_printf("%f %f %f | %f %f %f\n",
-											MODEL.prop.cholXtX[i*K + i], MODEL.curr.cholXtX[i * K + i],
-											MODEL.prop.cholXtX[i * K + i] - MODEL.curr.cholXtX[i * K + i],
-											MODEL.prop.XtX[i * K + i], MODEL.curr.XtX[i * K + i],
-											MODEL.prop.XtX[i * K + i] - MODEL.curr.XtX[i * K + i]);
-
-								}
-
-									r_printf("ite----%d\n",ite);
-									int a = 1;
-									*/
-							}
+				    #ifdef __DEBUG__
+						if (basisIdx == 0) ++(accS[NEW.jumpType]);
+						else 		       ++(accT[NEW.jumpType]);
+					#endif
+
+				} //(*rnd32++ < exp(marg_lik_prop - basis->marg_lik))
+				
+
+				U08 bResampleParameter  = (ite >=100)         && (ite % 20 == 0)     ; //MCMC_BURIN>=150L
+				U08 bStoreCurrentSample = (ite > MCMC_BURNIN) && (ite % MCMC_THINNING == 0);
+
+				/****************************************************************************************/
+				// For buin-in iterations, we also want to sample parameters: added for cases when burn-in is very large
+				/****************************************************************************************/
+
+				/**********************/
+				//First, Re-SAMPLING SIG2
+				/**********************/
+				if (bResampleParameter || bStoreCurrentSample)	{		
+
+					if (q == 1) {
+						//vdRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, &sig2, (alpha_1+n/2), 0, 1.0/(alpha_1+basis->alpha2_star *0.5));
+						F32 sig2      = (*RND.rndgamma++) * 1.f / MODEL.curr.alpha2Q_star[0];
+						sig2          = 1.0f / sig2;					 
+						MODEL.sig2[0] = sig2 > MIN_SIG2_VALUE ? sig2 : MODEL.sig2[0];
+						//r_printf("ite-%d SIG %f %f\n", ite, MODEL.sig2,  MODEL.sig2*yInfo.sd*yInfo.sd);
+					}	else {
+						// For MRBEAST
+						F32PTR MEMBUF = Xnewterm;
+						local_pcg_invwishart_upper( &stream, MODEL.sig2, MODEL.sig2 +q*q, MEMBUF, q,
+							                        MODEL.curr.alpha2Q_star, hyperPar.alpha_1+ yInfo.n + q - 1);					
+					}
 
-#endif
+				}
+				/**********************/
+				//Re-sample beta to be used for either re-sampling prec (ite%20=0) or predicting Y (ite%thiningFactor=0)
+				/**********************/
+				if (bResampleParameter || (bStoreCurrentSample && extra.useMeanOrRndBeta)) {
+
+					if (q == 1) {
+						//Compute beta = beta_mean + Rsig2 * randn(p, 1);
+						//Usig2 = (1 / sqrt(sig2)) * U; 		beta = beta_mean + linsolve(Usig2, randn(p, 1), opts);
+						//status = vdRngGaussian( method, stream, n, r, a, sigma );
+						I32 K = MODEL.curr.K;
+						r_vsRngGaussian(VSL_RNG_METHOD_GAUSSIAN_ICDF, stream, K, MODEL.beta, 0, 1);
+						//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, 1, MODEL.curr.cholXtX, K, MODEL.curr.beta, K); // LAPACKE_strtrs (int matrix_layout , char uplo , char trans , char diag , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
+						solve_U_as_U_invdiag(MODEL.curr.cholXtX, MODEL.beta, K, K);
+						r_ippsMulC_32f_I(fastsqrt(MODEL.sig2[0]), MODEL.beta, K);
+						r_ippsAdd_32f_I(MODEL.curr.beta_mean, MODEL.beta, K);
+					} else {
+					    // for MRBEAST
+						F32PTR MEMBUF = Xnewterm;
+						I32    K      = MODEL.curr.K;
+
+						r_vsRngGaussian(VSL_RNG_METHOD_GAUSSIAN_ICDF, stream, K * q, MEMBUF, 0., 1.);
+						r_cblas_sgemm(CblasColMajor, CblasNoTrans, CblasNoTrans, K, q, q, 1.0, MEMBUF, K, MODEL.sig2, q, 0.f, MODEL.beta, K);
+						//LAPACKE_strtrs (int matrix_layout , char uplo , char trans , char diag , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
+						//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, 1, basis->post_P_U, K, beta, K);
+						//r_ippsMulC_32f_I(sqrtf(modelPar.sig2), beta, K);
+						//r_ippsAdd_32f_I(basis->beta_mean, beta, K);
+						
+						//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, q, post_P_U, K, beta, K);
+						//r_ippsAdd_32f_I(MODEL.curr.beta_mean, MODEL.beta, K * q);
+						solve_U_as_U_invdiag_multicols(MODEL.curr.cholXtX, MODEL.beta, K, K, q);
+						r_ippsAdd_32f_I(MODEL.curr.beta_mean, MODEL.beta, K * q);
+					}
 
+				}
 
-						} //(*rnd32++ < exp(marg_lik_prop - basis->marg_lik))
+				/**********************/
+				// Re-sample the precison parameters and re-calcuate marg_lik and beta
+				/**********************/
+				if (bResampleParameter && q==1) 
+				{
+				   /*
+					I32   K     = MODEL.K;
+					F32   sumq  = DOT(K, MODEL.curr.beta, MODEL.curr.beta);
+					r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, modelPar.prec, (hyperPar.del_1 + K * 0.5f), 0, 1.f);
+					modelPar.prec[2]     = modelPar.prec[1] = modelPar.prec[0] = (*modelPar.prec) / (hyperPar.del_2 + 0.5f * sumq / MODEL.sig2);
+					modelPar.LOG_PREC[2] = modelPar.LOG_PREC[1] = modelPar.LOG_PREC[0] = logf(modelPar.prec[0]);				
+					 
+					*/
+		   
+					/*
+					//X_mars_prop has been constructed. Now use it to calcuate its marginal likelihood
+					//Add precison values to the diagonal of XtX: post_P=XtX +diag(prec)				
+					SCPY(K * K, MODEL.curr.XtX, MODEL.curr.cholXtX);
+
+					{//Add precison values to the SEASONAL diagonal compoents		
+						//rU08PTR termType = MODEL.termType;			
+						for (rI32 i = 1, j = 0; i <= K; i++)						{
+							//MODEL.curr.cholXtX[j + (i)-1] += modelPar.prec[*termType++];
+							MODEL.curr.cholXtX[j + (i)-1] += modelPar.prec[0];
+							j += K;
+						}
+					}//Add precison values to the SEASONAL diagonal compoents
+
+					//Solve inv(Post_P)*XtY using  Post_P*b=XtY to get beta_mean
+					//lapack_int LAPACKE_spotrf(int matrix_layout, char uplo, lapack_int n, double * a, lapack_int lda);
+					r_LAPACKE_spotrf(LAPACK_COL_MAJOR, 'U', K, MODEL.curr.cholXtX, K); // Choleskey decomposition; only the upper triagnle elements are used
+					//chol_addCol(MODEL.curr.cholXtX, MODEL.curr.cholXtX, K, 1, K);
+
+					//LAPACKE_spotrs (int matrix_layout , char uplo , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );			
+					SCPY(K, MODEL.curr.XtY, MODEL.curr.beta_mean);
+					r_LAPACKE_spotrs(LAPACK_COL_MAJOR, 'U', K, 1, MODEL.curr.cholXtX, K, MODEL.curr.beta_mean, K);
+					*/
+
+					I32 ntries = 0;
+					do {
+						if (ntries++ == 0)	precFunc.ResamplePrecValues(&MODEL, &hyperPar, &stream);							
+						else				precFunc.IncreasePrecValues(&MODEL);											
+						precFunc.GetXtXPrecDiag( &MODEL);
+						precFunc.chol_addCol(    MODEL.curr.XtX, MODEL.curr.cholXtX, MODEL.curr.precXtXDiag, MODEL.curr.K, 1L, MODEL.curr.K);		
+						precFunc.ComputeMargLik( &MODEL.curr, &MODEL, &yInfo, &hyperPar);
+
+					} while (  IsNaN(MODEL.curr.marg_lik) && ntries < 20 );
+
+					if ( IsNaN(MODEL.curr.marg_lik) ) {
+						#if !(defined(R_RELEASE) || defined(M_RELEASE)) 
+						r_printf("skip3 | prec: %.4f| marg_lik_cur: %.4f \n",  MODEL.precVec[0], MODEL.curr.marg_lik);
+						#endif
+						skipCurrentPixel = 3;
+						break;
+					} 
 
+					/* No need to re-sample beta because it is not really used
+					r_vsRngGaussian(VSL_RNG_METHOD_GAUSSIAN_ICDF, stream, K, beta, 0, 1);
+					// LAPACKE_strtrs (int matrix_layout , char uplo , char trans , char diag , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
+					r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, 1, cholXtX, K, beta, K);
+					r_ippsMulC_32f_I(sqrtf(modelPar.sig2), beta, K);
+					r_ippsAdd_32f_I(beta_mean, beta, K);
+					*/
+					/* /FInally, re-sample sig2 based on the lastest alpha2_star
+					//vdRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, &sig2, (alpha_2+n/2), 0, 1.0/(alpha_1+basis->alpha2_star *0.5));
+					modelPar.sig2 = (*rndgamma++)*1.0f / (modelPar.alpha_1 + basis->alpha2_star *0.5f);
+					modelPar.sig2 = 1.f / modelPar.sig2;
+					*/
+				}
 
-						U08 bResampleParameter = (ite >= 100) && (ite % 20 == 0); //MCMC_BURIN>=150L
-						U08 bStoreCurrentSample = (ite > MCMC_BURNIN) && (ite % MCMC_THINNING == 0);
+				if (bResampleParameter && q>1) 
+				{
+					F32PTR MEMBUF = Xnewterm;					
+					I32    K      = MODEL.curr.K;
+					//FLOAT_SHARE.sumq = DOT(K, basis->beta, basis->beta);
+					//r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, modelPar.prec, (modelPar.alpha_2 + K *0.5f), 0, 1.f);
+					//modelPar.prec[2] = modelPar.prec[1] = (*modelPar.prec) / (modelPar.alpha_1 + 0.5f*FLOAT_SHARE.sumq / modelPar.sig2);
+
+					
+					I32 ntries = 0;
+					do {
+						if (ntries++ == 0) {
+							// Get trace( B*inv(SIG2)*B')						
+							//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', q, q, basis->alpha_Q_star, q, W_L, q);	
+							r_cblas_sgemm(CblasColMajor, CblasNoTrans, CblasNoTrans, K, q, q, 1.0, MODEL.beta, K, MODEL.sig2+q*q, q, 0.f, MEMBUF, K);
+							F32 sumq = DOT(K * q, MEMBUF, MEMBUF);
+							r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1L, MODEL.precVec, (hyperPar.del_1 + K * q * 0.5f), 0.f, 1.f);
+							MODEL.precVec[0]     = MODEL.precVec[0] / (hyperPar.del_2 + 0.5f * sumq);
+							MODEL.logPrecVec[0]  = logf(MODEL.precVec[0]);
+						} else {
+							precFunc.IncreasePrecValues(&MODEL);
+						}
+						//precFunc.ResamplePrecValues( &MODEL, &hyperPar,&stream);
+						precFunc.GetXtXPrecDiag(&MODEL);
+						precFunc.chol_addCol(MODEL.curr.XtX, MODEL.curr.cholXtX, MODEL.curr.precXtXDiag, K, 1, K);
+						precFunc.ComputeMargLik(&MODEL.curr, &MODEL, &yInfo, &hyperPar);
+					} while (IsNaN(MODEL.curr.marg_lik) && ntries < 20);
+
+					
+					if ( IsNaN(MODEL.curr.marg_lik) ) {
+						#if !(defined(R_RELEASE) || defined(M_RELEASE)) 
+							r_printf("skip4 | prec: %.4f| marg_lik_cur: %.4f \n",  MODEL.precVec[0], MODEL.curr.marg_lik);
+						#endif
+						skipCurrentPixel = 3;
+						break;
+					}  
 
-						/****************************************************************************************/
-						// For buin-in iterations, we also want to sample parameters: added for cases when burn-in is very large
-						/****************************************************************************************/
-
-						/**********************/
-						//First, Re-SAMPLING SIG2
-						/**********************/
-						if (bResampleParameter || bStoreCurrentSample) {
-
-							if (q == 1) {
-								//vdRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, &sig2, (alpha_1+n/2), 0, 1.0/(alpha_1+basis->alpha2_star *0.5));
-								F32 sig2 = (*RND.rndgamma++) * 1.f / MODEL.curr.alpha2Q_star[0];
-								sig2 = 1.0f / sig2;
-								MODEL.sig2[0] = sig2 > MIN_SIG2_VALUE ? sig2 : MODEL.sig2[0];
-								//r_printf("ite-%d SIG %f %f\n", ite, MODEL.sig2,  MODEL.sig2*yInfo.sd*yInfo.sd);
-							}
-							else {
-								// For MRBEAST
-								F32PTR MEMBUF = Xnewterm;
-								local_pcg_invwishart_upper(&stream, MODEL.sig2, MODEL.sig2 + q * q, MEMBUF, q,
-									MODEL.curr.alpha2Q_star, hyperPar.alpha_1 + yInfo.n + q - 1);
-							}
+				}
+ 
+				if (!bStoreCurrentSample) continue;
+				
+				/**********************************************/
+				//
+				//      Start to compute final results
+				//
+				/**********************************************/
+
+				sample++;
+
+				if (extra.printProgressBar && NUM_PIXELS == 1 && sample % 1000 == 0) {
+					F32 frac = (F32)(chainNumber * MCMC_SAMPLES + sample) / (MCMC_SAMPLES * MCMC_CHAINNUM);
+					printProgress(frac, extra.consoleWidth, Xnewterm, 0);
+				}
 
-						}
-						/**********************/
-						//Re-sample beta to be used for either re-sampling prec (ite%20=0) or predicting Y (ite%thiningFactor=0)
-						/**********************/
-						if (bResampleParameter || (bStoreCurrentSample && extra.useMeanOrRndBeta)) {
-
-							if (q == 1) {
-								//Compute beta = beta_mean + Rsig2 * randn(p, 1);
-								//Usig2 = (1 / sqrt(sig2)) * U; 		beta = beta_mean + linsolve(Usig2, randn(p, 1), opts);
-								//status = vdRngGaussian( method, stream, n, r, a, sigma );
-								I32 K = MODEL.curr.K;
-								r_vsRngGaussian(VSL_RNG_METHOD_GAUSSIAN_ICDF, stream, K, MODEL.beta, 0, 1);
-								//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, 1, MODEL.curr.cholXtX, K, MODEL.curr.beta, K); // LAPACKE_strtrs (int matrix_layout , char uplo , char trans , char diag , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
-								solve_U_as_U_invdiag(MODEL.curr.cholXtX, MODEL.beta, K, K);
-								r_ippsMulC_32f_I(fastsqrt(MODEL.sig2[0]), MODEL.beta, K);
-								r_ippsAdd_32f_I(MODEL.curr.beta_mean, MODEL.beta, K);
-							}
-							else {
-								// for MRBEAST
-								F32PTR MEMBUF = Xnewterm;
-								I32    K = MODEL.curr.K;
-
-								r_vsRngGaussian(VSL_RNG_METHOD_GAUSSIAN_ICDF, stream, K * q, MEMBUF, 0., 1.);
-								r_cblas_sgemm(CblasColMajor, CblasNoTrans, CblasNoTrans, K, q, q, 1.0, MEMBUF, K, MODEL.sig2, q, 0.f, MODEL.beta, K);
-								//LAPACKE_strtrs (int matrix_layout , char uplo , char trans , char diag , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
-								//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, 1, basis->post_P_U, K, beta, K);
-								//r_ippsMulC_32f_I(sqrtf(modelPar.sig2), beta, K);
-								//r_ippsAdd_32f_I(basis->beta_mean, beta, K);
-
-								//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, q, post_P_U, K, beta, K);
-								//r_ippsAdd_32f_I(MODEL.curr.beta_mean, MODEL.beta, K * q);
-								solve_U_as_U_invdiag_multicols(MODEL.curr.cholXtX, MODEL.beta, K, K, q);
-								r_ippsAdd_32f_I(MODEL.curr.beta_mean, MODEL.beta, K * q);
-							}
 
-						}
+				*resultChain.marg_lik += MODEL.curr.marg_lik;
 
-						/**********************/
-						// Re-sample the precison parameters and re-calcuate marg_lik and beta
-						/**********************/
-						if (bResampleParameter && q == 1)
-						{
-							/*
-							 I32   K     = MODEL.K;
-							 F32   sumq  = DOT(K, MODEL.curr.beta, MODEL.curr.beta);
-							 r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, modelPar.prec, (hyperPar.del_1 + K * 0.5f), 0, 1.f);
-							 modelPar.prec[2]     = modelPar.prec[1] = modelPar.prec[0] = (*modelPar.prec) / (hyperPar.del_2 + 0.5f * sumq / MODEL.sig2);
-							 modelPar.LOG_PREC[2] = modelPar.LOG_PREC[1] = modelPar.LOG_PREC[0] = logf(modelPar.prec[0]);
+				if (q == 1) {
+					resultChain.sig2[0] += MODEL.sig2[0];
+				}	else {
+					// For MRBEAST
+					F32PTR MEMBUF = Xnewterm;
+					r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, q, q, q, 1.f, MODEL.sig2, q, MODEL.sig2, q, 0.f, MEMBUF, q);
+					r_ippsAdd_32f_I(MEMBUF, resultChain.sig2,  q*q);
+				}
 
-							 */
+				F32PTR BETA = (extra.useMeanOrRndBeta == 0) ? MODEL.curr.beta_mean : MODEL.beta;
+				{
+					F32PTR MEMBUF1 = Xnewterm;					
 
-							 /*
-							 //X_mars_prop has been constructed. Now use it to calcuate its marginal likelihood
-							 //Add precison values to the diagonal of XtX: post_P=XtX +diag(prec)
-							 SCPY(K * K, MODEL.curr.XtX, MODEL.curr.cholXtX);
-
-							 {//Add precison values to the SEASONAL diagonal compoents
-								 //rU08PTR termType = MODEL.termType;
-								 for (rI32 i = 1, j = 0; i <= K; i++)						{
-									 //MODEL.curr.cholXtX[j + (i)-1] += modelPar.prec[*termType++];
-									 MODEL.curr.cholXtX[j + (i)-1] += modelPar.prec[0];
-									 j += K;
-								 }
-							 }//Add precison values to the SEASONAL diagonal compoents
-
-							 //Solve inv(Post_P)*XtY using  Post_P*b=XtY to get beta_mean
-							 //lapack_int LAPACKE_spotrf(int matrix_layout, char uplo, lapack_int n, double * a, lapack_int lda);
-							 r_LAPACKE_spotrf(LAPACK_COL_MAJOR, 'U', K, MODEL.curr.cholXtX, K); // Choleskey decomposition; only the upper triagnle elements are used
-							 //chol_addCol(MODEL.curr.cholXtX, MODEL.curr.cholXtX, K, 1, K);
-
-							 //LAPACKE_spotrs (int matrix_layout , char uplo , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
-							 SCPY(K, MODEL.curr.XtY, MODEL.curr.beta_mean);
-							 r_LAPACKE_spotrs(LAPACK_COL_MAJOR, 'U', K, 1, MODEL.curr.cholXtX, K, MODEL.curr.beta_mean, K);
-							 */
+					for (I32 i = 0; i < MODEL.NUMBASIS; ++i) 
+					{
+						BEAST2_BASIS_PTR  basis   = MODEL.b   + i;
+						CORESULT        * result  = coreResults+i;
 
-							I32 ntries = 0;
-							do {
-								if (ntries++ == 0)	precFunc.ResamplePrecValues(&MODEL, &hyperPar, &stream);
-								else				precFunc.IncreasePrecValues(&MODEL);
-								precFunc.GetXtXPrecDiag(&MODEL);
-								precFunc.chol_addCol(MODEL.curr.XtX, MODEL.curr.cholXtX, MODEL.curr.precXtXDiag, MODEL.curr.K, 1L, MODEL.curr.K);
-								precFunc.ComputeMargLik(&MODEL.curr, &MODEL, &yInfo, &hyperPar);
-
-							} while (IsNaN(MODEL.curr.marg_lik) && ntries < 20);
-
-							if (IsNaN(MODEL.curr.marg_lik)) {
-#if !(defined(R_RELEASE) || defined(M_RELEASE)) 
-								r_printf("skip3 | prec: %.4f| marg_lik_cur: %.4f \n", MODEL.precVec[0], MODEL.curr.marg_lik);
-#endif
-								skipCurrentPixel = 3;
-								break;
-							}
+						I32        nKnot  = basis->nKnot;
+						TKNOT_PTR  KNOT   = basis->KNOT;
 
-							/* No need to re-sample beta because it is not really used
-							r_vsRngGaussian(VSL_RNG_METHOD_GAUSSIAN_ICDF, stream, K, beta, 0, 1);
-							// LAPACKE_strtrs (int matrix_layout , char uplo , char trans , char diag , lapack_int n , lapack_int nrhs , const double * a , lapack_int lda , double * b , lapack_int ldb );
-							r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', K, 1, cholXtX, K, beta, K);
-							r_ippsMulC_32f_I(sqrtf(modelPar.sig2), beta, K);
-							r_ippsAdd_32f_I(beta_mean, beta, K);
-							*/
-							/* /FInally, re-sample sig2 based on the lastest alpha2_star
-							//vdRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, &sig2, (alpha_2+n/2), 0, 1.0/(alpha_1+basis->alpha2_star *0.5));
-							modelPar.sig2 = (*rndgamma++)*1.0f / (modelPar.alpha_1 + basis->alpha2_star *0.5f);
-							modelPar.sig2 = 1.f / modelPar.sig2;
-							*/
-						}
+						result->xNProb[nKnot] += 1L;
+						//Counting probability of being breakpoints				
+						for (I32 i = 0; i < nKnot; i++) result->xProb[ KNOT[i]-1 ] += 1L;
 
-						if (bResampleParameter && q > 1)
-						{
-							F32PTR MEMBUF = Xnewterm;
-							I32    K = MODEL.curr.K;
-							//FLOAT_SHARE.sumq = DOT(K, basis->beta, basis->beta);
-							//r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1, modelPar.prec, (modelPar.alpha_2 + K *0.5f), 0, 1.f);
-							//modelPar.prec[2] = modelPar.prec[1] = (*modelPar.prec) / (modelPar.alpha_1 + 0.5f*FLOAT_SHARE.sumq / modelPar.sig2);
-
-
-							I32 ntries = 0;
-							do {
-								if (ntries++ == 0) {
-									// Get trace( B*inv(SIG2)*B')						
-									//r_LAPACKE_strtrs(LAPACK_COL_MAJOR, 'U', 'N', 'N', q, q, basis->alpha_Q_star, q, W_L, q);	
-									r_cblas_sgemm(CblasColMajor, CblasNoTrans, CblasNoTrans, K, q, q, 1.0, MODEL.beta, K, MODEL.sig2 + q * q, q, 0.f, MEMBUF, K);
-									F32 sumq = DOT(K * q, MEMBUF, MEMBUF);
-									r_vsRngGamma(VSL_RNG_METHOD_GAMMA_GNORM_ACCURATE, stream, 1L, MODEL.precVec, (hyperPar.del_1 + K * q * 0.5f), 0.f, 1.f);
-									MODEL.precVec[0] = MODEL.precVec[0] / (hyperPar.del_2 + 0.5f * sumq);
-									MODEL.logPrecVec[0] = logf(MODEL.precVec[0]);
-								}
-								else {
-									precFunc.IncreasePrecValues(&MODEL);
-								}
-								//precFunc.ResamplePrecValues( &MODEL, &hyperPar,&stream);
-								precFunc.GetXtXPrecDiag(&MODEL);
-								precFunc.chol_addCol(MODEL.curr.XtX, MODEL.curr.cholXtX, MODEL.curr.precXtXDiag, K, 1, K);
-								precFunc.ComputeMargLik(&MODEL.curr, &MODEL, &yInfo, &hyperPar);
-							} while (IsNaN(MODEL.curr.marg_lik) && ntries < 20);
-
-
-							if (IsNaN(MODEL.curr.marg_lik)) {
-#if !(defined(R_RELEASE) || defined(M_RELEASE)) 
-								r_printf("skip4 | prec: %.4f| marg_lik_cur: %.4f \n", MODEL.precVec[0], MODEL.curr.marg_lik);
-#endif
-								skipCurrentPixel = 3;
-								break;
+						//Summng up the harmonic orders or trend orders for individual seeasonal segments
+						if (result->xorder != NULL) {
+							TORDER_PTR  ORDER = basis->ORDER;
+							for (I32 i = 0; i <= nKnot; ++i) {
+								I32 r1 = KNOT[i-1], r2 = KNOT[i]-1;
+								r_ippsAddC_32s_ISfs(ORDER[i], result->xorder+r1 - 1, r2 - r1 + 1, 0);
 							}
-
 						}
 
-						if (!bStoreCurrentSample) continue;
-
-						/**********************************************/
-						//
-						//      Start to compute final results
-						//
-						/**********************************************/
-
-						sample++;
-
-						if (extra.printProgressBar && NUM_PIXELS == 1 && sample % 1000 == 0) {
-							F32 frac = (F32)(chainNumber * MCMC_SAMPLES + sample) / (MCMC_SAMPLES * MCMC_CHAINNUM);
-							printProgress(frac, extra.consoleWidth, Xnewterm, 0);
-						}
-
-
-						*resultChain.marg_lik += MODEL.curr.marg_lik;
-
+						//Compute the averaged  signals
 						if (q == 1) {
-							resultChain.sig2[0] += MODEL.sig2[0];
-						}
-						else {
-							// For MRBEAST
-							F32PTR MEMBUF = Xnewterm;
-							r_cblas_sgemm(CblasColMajor, CblasTrans, CblasNoTrans, q, q, q, 1.f, MODEL.sig2, q, MODEL.sig2, q, 0.f, MEMBUF, q);
-							r_ippsAdd_32f_I(MEMBUF, resultChain.sig2, q * q);
-						}
-
-						F32PTR BETA = (extra.useMeanOrRndBeta == 0) ? MODEL.curr.beta_mean : MODEL.beta;
-						{
-							F32PTR MEMBUF1 = Xnewterm;
-
-							for (I32 i = 0; i < MODEL.NUMBASIS; ++i)
-							{
-								BEAST2_BASIS_PTR  basis = MODEL.b + i;
-								CORESULT* result = coreResults + i;
-
-								I32        nKnot = basis->nKnot;
-								TKNOT_PTR  KNOT = basis->KNOT;
-
-								result->xNProb[nKnot] += 1L;
-								//Counting probability of being breakpoints				
-								for (I32 i = 0; i < nKnot; i++) result->xProb[KNOT[i] - 1] += 1L;
-
-								//Summng up the harmonic orders or trend orders for individual seeasonal segments
-								if (result->xorder != NULL) {
-									TORDER_PTR  ORDER = basis->ORDER;
-									for (I32 i = 0; i <= nKnot; ++i) {
-										I16 r1 = KNOT[i - 1], r2 = KNOT[i] - 1;
-										r_ippsAddC_32s_ISfs(ORDER[i], result->xorder + r1 - 1, r2 - r1 + 1, 0);
-									}
-								}
-
-								//Compute the averaged  signals
-								if (q == 1) {
-									//r_cblas_sgemv(CblasColMajor, CblasNoTrans, Npad, K_SN, 1.f, Xt_mars, Npad, MODEL.curr.beta_mean, 1L, 0.f, MEMBUF1, 1L);
-									basis->ComputeY(Xt_mars, BETA, MEMBUF1, basis, Npad);
-									f32_add_v_v2_vec_inplace(MEMBUF1, result->x, result->xSD, N);
-									MEMBUF1 += Npad;
-								}
-								else {
-									// for MRBEAST
-									F32PTR 	X = Xt_mars + basis->Kbase * Npad;
-									F32PTR  beta = BETA + basis->Kbase;
-									I32     K = basis->K;
-									//r_cblas_sgemv(CblasColMajor, CblasNoTrans, Npad, K, 1.f, X, Npad, beta, 1L, 0.f, Y, 1L);
-									r_cblas_sgemm(CblasColMajor, CblasNoTrans, CblasNoTrans, N, q, K, 1.0f,
-										X, Npad, beta, MODEL.curr.K, 0.f, MEMBUF1, N);
-									f32_add_v_v2_vec_inplace(MEMBUF1, result->x, result->xSD, N * q);
-									MEMBUF1 += Npad * q;
-								}
-
-
-							}//for (rI32 i = 0; i < MODEL.NUMBASIS; i++)
-
-						}
-						/*********************************************************************/
-						// At this point, MEMBUF1=season, MEMBUF1+Npad=trend, and MEMBUF1+Npad+Npad=outlier;
-						/*********************************************************************/
-
-						/********************************************/
-						// Compute results for the seasonal cmpnt
-						/********************************************/
-						if (extra.computeSeasonAmp)
-						{
-							F32PTR           MEMBUF1 = Xnewterm + 3 * Npad;
-							F32PTR           MEMBUF2 = MODEL.prop.beta_mean; //re-used here as a temp mem buf.
-
-							BEAST2_BASIS_PTR basis = &MODEL.b[MODEL.sid];
-							I32             knotNum = basis->nKnot;
-							TKNOT_PTR       knotList = basis->KNOT;
-
-							//Summng up the per-segment harmonic magnitudes  	
-							F32PTR       beta = BETA;
-							TORDER_PTR   orderList = basis->ORDER;
-							F32PTR       SEASON_SQR_CSUM = basis->bConst.season.SQR_CSUM + 1L;  //SQR_CSUM has a row length of (N+1)
-							F32PTR       SEASON_SCALE = basis->bConst.season.SCALE_FACTOR;
-							if (SEASON_BTYPE == 0) {
-								for (I32 i = 0; i <= knotNum; i++) {
-									I32		r1 = knotList[i - 1];
-									I32		r2 = knotList[i] - 1;
-
-									F32PTR seasonSqrCsum = SEASON_SQR_CSUM;
-									I32    order2 = orderList[i] * 2L;
-									F32    amp = 0;
-									for (I32 j = 0; j < order2; j++) {
-										//TODO: re-check here
-										F32 scalingFactor = N / (seasonSqrCsum[r2 - 1] - seasonSqrCsum[(r1 - 1) - 1]);
-										F32 beta0 = beta[j] * SEASON_SCALE[j];
-										amp = amp + (beta0 * beta0) * scalingFactor;
-										seasonSqrCsum += (N + 1LL);
-									}
-									//r_ippsSubC_32f_I(-amp, resultChain.samp + r1 - 1, segLength, 0);
-									I32    segLength = r2 - r1 + 1L;
-									r_ippsSet_32f(amp, MEMBUF1 + r1 - 1, segLength);
-									beta += order2;
-								}
-							}
-							else {
-								for (I32 i = 0; i <= knotNum; i++) {
-									I32 r1 = knotList[i - 1];
-									I32 r2 = knotList[i] - 1;
-
-									F32PTR seasonSqrCsum = SEASON_SQR_CSUM;
-									I32    order2 = orderList[i] * 2L;
-									F32    amp = 0;
-									for (I32 j = 0; j < order2; j++) {
-										F32    beta0 = beta[j] * SEASON_SCALE[j];
-										amp += beta0 * beta0;
-									}
-
-									//r_ippsSubC_32f_I(-amp, resultChain.samp + r1 - 1, segLength, 0);
-									I32    segLength = r2 - r1 + 1L;
-									r_ippsSet_32f(amp, MEMBUF1 + r1 - 1, segLength);
-									beta += order2;
-								}
-							}
+							//r_cblas_sgemv(CblasColMajor, CblasNoTrans, Npad, K_SN, 1.f, Xt_mars, Npad, MODEL.curr.beta_mean, 1L, 0.f, MEMBUF1, 1L);
+							basis->ComputeY(Xt_mars, BETA, MEMBUF1, basis, Npad);
+							f32_add_v_v2_vec_inplace(MEMBUF1, result->x, result->xSD, N);
+							MEMBUF1 += Npad;
+						}	else {
+							// for MRBEAST
+							F32PTR 	X    = Xt_mars + basis->Kbase * Npad;
+							F32PTR  beta = BETA+basis->Kbase;
+							I32     K    = basis->K;
+							//r_cblas_sgemv(CblasColMajor, CblasNoTrans, Npad, K, 1.f, X, Npad, beta, 1L, 0.f, Y, 1L);
+							r_cblas_sgemm(CblasColMajor, CblasNoTrans, CblasNoTrans, N, q, K, 1.0f,
+									     	      X, Npad,beta, MODEL.curr.K, 0.f, MEMBUF1, N);
+							f32_add_v_v2_vec_inplace(MEMBUF1, result->x, result->xSD, N*q);
+							MEMBUF1 += Npad*q;
+						}
+	
+						
+					}//for (rI32 i = 0; i < MODEL.NUMBASIS; i++)
+				
+				}
+				/*********************************************************************/
+				// At this point, MEMBUF1=season, MEMBUF1+Npad=trend, and MEMBUF1+Npad+Npad=outlier;
+				/*********************************************************************/
+
+				/********************************************/
+				// Compute results for the seasonal cmpnt
+				/********************************************/
+				if(extra.computeSeasonAmp) 
+				{
+					F32PTR           MEMBUF1 = Xnewterm + 3*Npad;
+					F32PTR           MEMBUF2 = MODEL.prop.beta_mean; //re-used here as a temp mem buf.
 
-							r_ippsAdd_32f_I(MEMBUF1, resultChain.samp, N);
-							r_ippsMul_32f_I(MEMBUF1, MEMBUF1, N);
-							r_ippsAdd_32f_I(MEMBUF1, resultChain.sampSD, N); //added to the square of the samp for computering SD
-
-
-							if (extra.tallyPosNegSeasonJump)
-							{//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD					 
-								I32  posKnotNum = 0;
-								for (I32 i = 0; i < knotNum; i++) { // It must be i<KnotNum bcz of dealing with knots only 
-									I64 knot = knotList[i];
-									if (MEMBUF1[knot - 1] > MEMBUF1[knot - 1 - 1]) {
-										resultChain.spos_cpOccPr[knot - 1] += 1;
-										posKnotNum++;
-									}
-								}
-								resultChain.spos_ncpPr[posKnotNum] += 1L;
-								resultChain.sneg_ncpPr[knotNum - posKnotNum] += 1L;
-							}
+					BEAST2_BASIS_PTR basis    = &MODEL.b[MODEL.sid];
+					I32             knotNum  = basis->nKnot;
+					TKNOT_PTR       knotList = basis->KNOT;
+					
+					//Summng up the per-segment harmonic magnitudes  	
+					F32PTR       beta            = BETA;
+					TORDER_PTR   orderList       = basis->ORDER;
+					F32PTR       SEASON_SQR_CSUM = basis->bConst.season.SQR_CSUM +1L;  //SQR_CSUM has a row length of (N+1)
+					F32PTR       SEASON_SCALE    = basis->bConst.season.SCALE_FACTOR;
+					if (SEASON_BTYPE == 0) {
+						for (I32 i = 0; i <= knotNum; i++) {
+							I32		r1 = knotList[i - 1];
+							I32		r2 = knotList[i] - 1;
+							
+							F32PTR seasonSqrCsum = SEASON_SQR_CSUM;
+							I32    order2        = orderList[i] * 2L;
+							F32    amp           = 0;					 
+							for (I32 j = 0; j < order2; j++) {
+								//TODO: re-check here
+								F32 scalingFactor = N / (seasonSqrCsum[r2 - 1] - seasonSqrCsum[(r1 - 1) - 1]);
+								F32 beta0         = beta[j]* SEASON_SCALE[j];
+								amp               = amp + (beta0 * beta0) * scalingFactor;
+								seasonSqrCsum     += (N + 1LL);
+							}			 
+							//r_ippsSubC_32f_I(-amp, resultChain.samp + r1 - 1, segLength, 0);
+							I32    segLength = r2 - r1 + 1L;
+							r_ippsSet_32f(amp, MEMBUF1 + r1 - 1, segLength);
+							beta += order2;
+						}
+					} else {
+						for (I32 i = 0; i <= knotNum; i++) {
+							I32 r1 = knotList[i - 1];
+							I32 r2 = knotList[i] - 1;
+					
+							F32PTR seasonSqrCsum = SEASON_SQR_CSUM;
+							I32    order2        = orderList[i] * 2L;
+							F32    amp           = 0;		 
+							for (I32 j = 0; j < order2; j++) {
+								F32    beta0 = beta[j] * SEASON_SCALE[j];
+								amp += beta0 * beta0;
+							}					 
+
+							//r_ippsSubC_32f_I(-amp, resultChain.samp + r1 - 1, segLength, 0);
+							I32    segLength = r2 - r1 + 1L;
+							r_ippsSet_32f(amp, MEMBUF1 + r1 - 1, segLength);
+							beta += order2;
 						}
-
-						/********************************************/
-						// Compute results for the trend cmpnt
-						/********************************************/
-						if (extra.computeTrendSlope)
-						{
-							BEAST2_BASIS_PTR basis = &MODEL.b[MODEL.tid];
-							I32             knotNum = basis->nKnot;
-							TKNOT_PTR       knotList = basis->KNOT;
-
-							F32PTR TREND = Xnewterm + Npad * MODEL.tid;     //trend signal
-							F32PTR SLP = Xnewterm + 3 * Npad;				//temp mem
-
-																			// Compute the rate of change in trend based on beta. 
-							f32_diff_back(TREND, SLP, N);
-							f32_add_v_v2_vec_inplace(SLP, resultChain.tslp, resultChain.tslpSD, N); //added to the square of the trend signal for computing SD
-							//i32_increment_bycond_inplace(resultChain.tslpSgnPosPr, SLP, N); //increamnent tslpSingPr if SLP is larger than 0				 
-							i32_increment_vec2_bycond_inplace(resultChain.tslpSgnPosPr, resultChain.tslpSgnZeroPr, SLP, N); //increamnent tslpSingPr if SLP is larger than 0				 
-							if (extra.tallyPosNegTrendJump) {//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD					 
-								I32  posKnotNum = 0;
-								for (I32 i = 0; i < knotNum; i++) {  // It must be i<sKnotNum bcz of dealing with knots only 
-									I64 knot = knotList[i];
-									if (SLP[knot - 1] > 0) {
-										resultChain.tpos_cpOccPr[knot - 1] += 1;
-										posKnotNum++;
-									}
-								}
-								resultChain.tpos_ncpPr[posKnotNum] += 1L;
-								resultChain.tneg_ncpPr[knotNum - posKnotNum] += 1L;
+					}
+	
+					r_ippsAdd_32f_I(MEMBUF1, resultChain.samp,   N);
+					r_ippsMul_32f_I(MEMBUF1, MEMBUF1,            N);
+					r_ippsAdd_32f_I(MEMBUF1, resultChain.sampSD, N); //added to the square of the samp for computering SD
+
+					
+					if (extra.tallyPosNegSeasonJump)
+					{//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD					 
+						I32  posKnotNum = 0;
+						for (I32 i = 0; i < knotNum; i++) { // It must be i<KnotNum bcz of dealing with knots only 
+							I64 knot = knotList[i];
+							if (MEMBUF1[knot - 1] > MEMBUF1[knot - 1 - 1]) {
+								resultChain.spos_cpOccPr[knot - 1] += 1;
+								posKnotNum++;
 							}
-
-							if (extra.tallyIncDecTrendJump) {//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD					 						
-								I32  incKnotNum = 0;
-								for (I32 i = 0; i < knotNum; i++) {  // It must be i<sKnotNum bcz of dealing with knots only 
-									I64 knot = knotList[i];
-									if (knot >= 2 && SLP[(knot + 1) - 1] > SLP[(knot - 1) - 1]) {
-										resultChain.tinc_cpOccPr[knot - 1] += 1;
-										incKnotNum++;
-									}
-								}
-								resultChain.tinc_ncpPr[incKnotNum] += 1L;
-								resultChain.tdec_ncpPr[knotNum - incKnotNum] += 1L;
+						}
+						resultChain.spos_ncpPr[posKnotNum]           += 1L;
+						resultChain.sneg_ncpPr[knotNum - posKnotNum] += 1L;
+					}
+				}
+				
+				/********************************************/
+				// Compute results for the trend cmpnt
+				/********************************************/
+				if(extra.computeTrendSlope)
+				{
+					BEAST2_BASIS_PTR basis   = &MODEL.b[MODEL.tid];
+					I32             knotNum  = basis->nKnot;
+					TKNOT_PTR       knotList = basis->KNOT;
+
+					F32PTR TREND = Xnewterm + Npad * MODEL.tid;     //trend signal
+					F32PTR SLP   = Xnewterm + 3 * Npad;				//temp mem
+
+																	// Compute the rate of change in trend based on beta. 
+					f32_diff_back(TREND, SLP, N);
+					f32_add_v_v2_vec_inplace(SLP, resultChain.tslp, resultChain.tslpSD, N); //added to the square of the trend signal for computing SD
+					//i32_increment_bycond_inplace(resultChain.tslpSgnPosPr, SLP, N); //increamnent tslpSingPr if SLP is larger than 0				 
+					i32_increment_vec2_bycond_inplace(resultChain.tslpSgnPosPr, resultChain.tslpSgnZeroPr, SLP, N); //increamnent tslpSingPr if SLP is larger than 0				 
+					if (extra.tallyPosNegTrendJump ) {//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD					 
+						I32  posKnotNum = 0;
+						for (I32 i = 0; i < knotNum; i++) {  // It must be i<sKnotNum bcz of dealing with knots only 
+							I64 knot = knotList[i];
+							if (SLP[knot - 1] > 0) {
+								resultChain.tpos_cpOccPr[knot - 1] += 1;
+								posKnotNum++;
 							}
-
 						}
+						resultChain.tpos_ncpPr[posKnotNum]           += 1L;
+						resultChain.tneg_ncpPr[knotNum - posKnotNum] += 1L;
+					}
 
-						/********************************************/
-						// Compute results for the outlier cmpnt
-						/********************************************/
-						if (extra.tallyPosNegOutliers)
-						{//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD	
-							BEAST2_BASIS_PTR basis = &MODEL.b[MODEL.oid];
-							rI32             knotNum = basis->nKnot;
-							rTKNOT_PTR       knotList = basis->KNOT;
-
-							const F32PTR OUTLIIER = Xnewterm + Npad * MODEL.oid;
-
-							I32  posKnotNum = 0;
-							for (I32 i = 0; i < knotNum; i++) {  // It must be i<sKnotNum bcz of dealing with knots only 
-								I64 knot = knotList[i];
-								if (OUTLIIER[knot - 1] > 0) {
-									resultChain.opos_cpOccPr[knot - 1] += 1;
-									posKnotNum++;
-								}
+					if (extra.tallyIncDecTrendJump ){//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD					 						
+						I32  incKnotNum = 0;
+						for (I32 i = 0; i < knotNum; i++) {  // It must be i<sKnotNum bcz of dealing with knots only 
+							I64 knot = knotList[i];
+							if (knot >= 2 && SLP[(knot + 1) - 1] > SLP[(knot - 1) - 1]) {
+								resultChain.tinc_cpOccPr[knot - 1] += 1;
+								incKnotNum++;
 							}
-							resultChain.opos_ncpPr[posKnotNum] += 1L;
-							resultChain.oneg_ncpPr[knotNum - posKnotNum] += 1L;
 						}
+						resultChain.tinc_ncpPr[incKnotNum]         += 1L;
+						resultChain.tdec_ncpPr[knotNum-incKnotNum] += 1L;
+					}
+			
+				}
 
-						/*************************************************/
-						// Compute ci intervals: new row of data have already calculated
-						// and saved in Xnewterm, Xnewterm+Npad, and Xnweterm+2*Npad
-						/*************************************************/
-						if (extra.computeCredible) {
-
-							// when  *RND.rnd16++ <= ciParam.subsampleFraction_x_INT16MAX, samples are included;					
-							if (extra.fastCIComputation && !(*RND.rnd16++ < ciParam.subsampleFraction_x_INT16MAX)) {
-								//if (*rnd32++ < subsampleFraction*4.294967296000000e+09)
-								// The current sample not included. No need to insert it into the ci strips.
-								// So, just skip to the next iteration	
-							}
-							else {
-								// New row of data for slope, seasonal, and trend components: MEMBUF1=slope over time	 					    
-								for (int i = 0; i < MODEL.NUMBASIS; i++)
-									InsertNewRowToUpdateCI(&ciParam, &ci[i]);
-							}
+				/********************************************/
+				// Compute results for the outlier cmpnt
+				/********************************************/
+				if(extra.tallyPosNegOutliers)
+				{//NEWLY ADDEDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD	
+					BEAST2_BASIS_PTR basis    = &MODEL.b[MODEL.oid];
+					rI32             knotNum  = basis->nKnot;
+					rTKNOT_PTR       knotList = basis->KNOT;
+
+					const F32PTR OUTLIIER  = Xnewterm + Npad* MODEL.oid;
+	 
+					I32  posKnotNum = 0;
+					for (I32 i = 0; i < knotNum; i++) {  // It must be i<sKnotNum bcz of dealing with knots only 
+						I64 knot = knotList[i];
+						if (OUTLIIER[knot - 1] > 0) {
+							resultChain.opos_cpOccPr[knot - 1] += 1;
+							posKnotNum++;
+						}							
+					}
+					resultChain.opos_ncpPr[posKnotNum]			 += 1L;
+					resultChain.oneg_ncpPr[knotNum - posKnotNum] += 1L;								
+				}
 
-						} // if (extra.computeCredible)
+				/*************************************************/
+				// Compute ci intervals: new row of data have already calculated
+				// and saved in Xnewterm, Xnewterm+Npad, and Xnweterm+2*Npad
+				/*************************************************/
+				if (extra.computeCredible)	{ 	
+
+					// when  *RND.rnd16++ <= ciParam.subsampleFraction_x_INT16MAX, samples are included;					
+					if (extra.fastCIComputation &&  !(*RND.rnd16++  < ciParam.subsampleFraction_x_INT16MAX)  ){
+						//if (*rnd32++ < subsampleFraction*4.294967296000000e+09)
+				        // The current sample not included. No need to insert it into the ci strips.
+						// So, just skip to the next iteration	
+					} else {
+						// New row of data for slope, seasonal, and trend components: MEMBUF1=slope over time	 					    
+						for (int i = 0; i < MODEL.NUMBASIS; i++) 
+							InsertNewRowToUpdateCI(&ciParam, &ci[i]);						
+					}					
 
+				} // if (extra.computeCredible)
+				
 					/*---------WINDOW-------------------------*/
 						EnterCriticalSection(&gData.cs);
 
 						gData.ite = ite;
 						gData.sample = sample;
 						gData.tKnotNum = MODEL.b[1].nKnot;
 						gData.sKnotNum = MODEL.b[0].nKnot;;
@@ -1295,274 +1277,274 @@
 							r_vslDeleteStream(&stream);
 
 							return;
 						}
 
 						LeaveCriticalSection(&gData.cs);
 						/*---------WINDOW-------------------------*/
-					}//WHILE(sample<SAMPLE)
-
-					/*****************************************************************************/
-					//
-					// One chain is done; then start post-processing the result of the chain     
-					//
-					/*****************************************************************************/
-
-					if (!skipCurrentPixel)
-					{
-						int   sum;
-#define GetSum(arr) (r_ippsSum_32s_Sfs(arr, N, &sum, 0), sum) // parenthesis operator
+			}//WHILE(sample<SAMPLE)
 
-						I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
-						I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
-						I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
-						F32   inv_sample = 1.f / sample;
+			/*****************************************************************************/
+			//
+			// One chain is done; then start post-processing the result of the chain     
+			//
+			/*****************************************************************************/
+
+			if (!skipCurrentPixel)
+			{
+				int   sum;
+				#define GetSum(arr) (r_ippsSum_32s_Sfs(arr, N, &sum, 0), sum) // parenthesis operator
+
+				I32   sMAXNUMKNOT = MODEL.sid >=0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum:-9999999; // the seasonal cmpt is always the first one
+				I32   tMAXNUMKNOT = MODEL.tid>=0?  MODEL.b[MODEL.tid].prior.maxKnotNum:-9999999;
+				I32   oMAXNUMKNOT = MODEL.oid>=0?  MODEL.b[MODEL.oid].prior.maxKnotNum:- 9999999;
+				F32   inv_sample  = 1.f / sample;			
+				
+
+				*resultChain.marg_lik = *resultChain.marg_lik * inv_sample;
+				// FOR MRBEAST
+				for (int col = 0; col < q; col++)	{ 
+					for (int i = 0; i < q; i++) {
+						resultChain.sig2[col*q+i] = resultChain.sig2[col*q+i] * inv_sample * yInfo.sd[col] * yInfo.sd[i];
+					}
+				}
+				
 
+				if (MODEL.sid >= 0 || MODEL.vid >= 0) {
 
-						*resultChain.marg_lik = *resultChain.marg_lik * inv_sample;
-						// FOR MRBEAST
-						for (int col = 0; col < q; col++) {
-							for (int i = 0; i < q; i++) {
-								resultChain.sig2[col * q + i] = resultChain.sig2[col * q + i] * inv_sample * yInfo.sd[col] * yInfo.sd[i];
-							}
+						*resultChain.sncp = GetSum(resultChain.scpOccPr)* inv_sample; 
+						i32_to_f32_scaleby_inplace(resultChain.sncpPr,	(sMAXNUMKNOT + 1), inv_sample);
+						i32_to_f32_scaleby_inplace(resultChain.scpOccPr, N,		           inv_sample);	
+					
+						//FOR MRBEAST
+						for (int i = 0; i < q; i++) {
+							F32 offset = 0.0f;
+							f32_sx_sxx_to_avgstd_inplace(resultChain.sY + i * N, resultChain.sSD + i * N, sample, yInfo.sd[i], offset, N);
 						}
 
-
-						if (MODEL.sid >= 0) {
-
-							*resultChain.sncp = GetSum(resultChain.scpOccPr) * inv_sample;
-							i32_to_f32_scaleby_inplace(resultChain.sncpPr, (sMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.scpOccPr, N, inv_sample);
-
+						if (extra.computeSeasonOrder) i32_to_f32_scaleby_inplace(resultChain.sorder, N, inv_sample);
+						if (extra.computeSeasonAmp) {
 							//FOR MRBEAST
 							for (int i = 0; i < q; i++) {
 								F32 offset = 0.0f;
-								f32_sx_sxx_to_avgstd_inplace(resultChain.sY + i * N, resultChain.sSD + i * N, sample, yInfo.sd[i], offset, N);
-							}
-
-							if (extra.computeSeasonOrder) i32_to_f32_scaleby_inplace(resultChain.sorder, N, inv_sample);
-							if (extra.computeSeasonAmp) {
-								//FOR MRBEAST
-								for (int i = 0; i < q; i++) {
-									F32 offset = 0.0f;
-									f32_sx_sxx_to_avgstd_inplace(resultChain.samp + i * N, resultChain.sampSD + i * N, sample, yInfo.sd[i] * yInfo.sd[i], offset, N);
-								}
-							}
-							if (extra.computeCredible) {
-								//FOR MRBEAST
-								for (int i = 0; i < q; i++) {
-									r_ippsMulC_32f_I(yInfo.sd[i], resultChain.sCI + N * i, N);
-									r_ippsMulC_32f_I(yInfo.sd[i], resultChain.sCI + N * q + N * i, N);
-								}
-							}
+								f32_sx_sxx_to_avgstd_inplace(resultChain.samp+i*N, resultChain.sampSD + i*N, sample, yInfo.sd[i]* yInfo.sd[i], offset, N);
+							}							
 						}
-
-						///////////////TREND////////////////////////////////////////////////////
-						if (MODEL.tid >= 0) {
-							*resultChain.tncp = GetSum(resultChain.tcpOccPr) * inv_sample;
-							i32_to_f32_scaleby_inplace(resultChain.tncpPr, (tMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.tcpOccPr, N, inv_sample);
+						if (extra.computeCredible) {
 							//FOR MRBEAST
-							for (int i = 0; i < q; i++) {
-								F32 offset = 0.0f;
-								f32_sx_sxx_to_avgstd_inplace(resultChain.tY + i * N, resultChain.tSD + i * N, sample, yInfo.sd[i], yInfo.mean[i], N);
-							}
+							for (int i = 0; i < q; i++) {								
+								r_ippsMulC_32f_I(yInfo.sd[i], resultChain.sCI+      N*i, N);
+								r_ippsMulC_32f_I(yInfo.sd[i], resultChain.sCI+N*q + N*i, N);
+							}							
+						} 
+				}
 
+				///////////////TREND////////////////////////////////////////////////////
+				if (MODEL.tid >= 0) {
+						*resultChain.tncp = GetSum(resultChain.tcpOccPr)*inv_sample ;
+						i32_to_f32_scaleby_inplace(resultChain.tncpPr, (tMAXNUMKNOT + 1),	inv_sample);
+						i32_to_f32_scaleby_inplace(resultChain.tcpOccPr, N,					inv_sample);
+						//FOR MRBEAST
+						for (int i = 0; i < q; i++) {
+							F32 offset = 0.0f;
+							f32_sx_sxx_to_avgstd_inplace(resultChain.tY + i * N, resultChain.tSD + i * N, sample, yInfo.sd[i], yInfo.mean[i], N);
+						}
 
-							if (extra.computeTrendOrder) 	i32_to_f32_scaleby_inplace(resultChain.torder, N, inv_sample);
-							if (extra.computeTrendSlope) {
-								//FOR MRBEAST
-								for (int i = 0; i < q; i++) {
-									f32_sx_sxx_to_avgstd_inplace(resultChain.tslp + i * N, resultChain.tslpSD + i * N, sample, yInfo.sd[i] / opt->io.meta.deltaTime, 0, N);
-								}
-								i32_to_f32_scaleby_inplace(resultChain.tslpSgnPosPr, N * q, inv_sample);
-								i32_to_f32_scaleby_inplace(resultChain.tslpSgnZeroPr, N * q, inv_sample);
-							}
-							if (extra.computeCredible) {
-								//FOR MRBEAST
-								for (int i = 0; i < q; i++) {
-									f32_scale_inplace(yInfo.sd[i], yInfo.mean[i], resultChain.tCI + N * i, N);
-									f32_scale_inplace(yInfo.sd[i], yInfo.mean[i], resultChain.tCI + N * q + N * i, N);
-									//r_ippsMulC_32f_I(,    resultChain.tCI+(2*N)*i, N + N),
-									//r_ippsSubC_32f_I(-yInfo.mean[i], ); //ippsAddC_32f_I(yInfo.mean, result.tCI, N + N);
-								}
-							}
 
+						if (extra.computeTrendOrder) 	i32_to_f32_scaleby_inplace(resultChain.torder, N, inv_sample);						
+						if (extra.computeTrendSlope) {
+							//FOR MRBEAST
+							for (int i = 0; i < q; i++) {
+								f32_sx_sxx_to_avgstd_inplace(resultChain.tslp+i*N, resultChain.tslpSD+ i*N, sample, yInfo.sd[i]/opt->io.meta.deltaTime, 0, N);
+							}							
+							i32_to_f32_scaleby_inplace(resultChain.tslpSgnPosPr, N*q, inv_sample);
+							i32_to_f32_scaleby_inplace(resultChain.tslpSgnZeroPr, N*q, inv_sample);
 						}
-
-						///////////////OUTLIR////////////////////////////////////////////////////
-						if (MODEL.oid >= 0) {
-							*resultChain.oncp = inv_sample * GetSum(resultChain.ocpOccPr);
-							i32_to_f32_scaleby_inplace(resultChain.oncpPr, (oMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.ocpOccPr, N, inv_sample);
+						if (extra.computeCredible) {
 							//FOR MRBEAST
 							for (int i = 0; i < q; i++) {
-								f32_sx_sxx_to_avgstd_inplace(resultChain.oY + i * N, resultChain.oSD + i * N, sample, yInfo.sd[i], 0, N);
-							}
-							if (extra.computeCredible) {
-								//FOR MRBEAST
-								for (int i = 0; i < q; i++) {
-									r_ippsMulC_32f_I(yInfo.sd[i], resultChain.oCI + i * N, N);
-									r_ippsMulC_32f_I(yInfo.sd[i], resultChain.oCI + N * q + i * N, N);
-								}
-							}
+								f32_scale_inplace(yInfo.sd[i], yInfo.mean[i], resultChain.tCI +        N * i, N);
+								f32_scale_inplace(yInfo.sd[i], yInfo.mean[i], resultChain.tCI + N*q +  N * i, N);
+								//r_ippsMulC_32f_I(,    resultChain.tCI+(2*N)*i, N + N),
+								//r_ippsSubC_32f_I(-yInfo.mean[i], ); //ippsAddC_32f_I(yInfo.mean, result.tCI, N + N);
+							}							
 						}
+						
+				}
 
+				///////////////OUTLIR////////////////////////////////////////////////////
+				if (MODEL.oid >= 0) {					
+					 *resultChain.oncp = inv_sample * GetSum(resultChain.ocpOccPr);
+					 i32_to_f32_scaleby_inplace(resultChain.oncpPr,  (oMAXNUMKNOT + 1), inv_sample);
+					 i32_to_f32_scaleby_inplace(resultChain.ocpOccPr, N,                inv_sample);
+					 //FOR MRBEAST
+					 for (int i = 0; i < q; i++) {
+						 f32_sx_sxx_to_avgstd_inplace(resultChain.oY+i*N, resultChain.oSD+i*N, sample, yInfo.sd[i], 0, N);
+					 }					 
+					 if (extra.computeCredible) {
+						 //FOR MRBEAST
+						 for (int i = 0; i < q; i++) {
+							 r_ippsMulC_32f_I(yInfo.sd[i], resultChain.oCI +      i*N, N );
+							 r_ippsMulC_32f_I(yInfo.sd[i], resultChain.oCI + N*q+ i*N, N);
+						 }						 
+					 }	
+				}
 
-						//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
-						if (extra.tallyPosNegSeasonJump && MODEL.sid >= 0) {
-
-							GetSum(resultChain.spos_cpOccPr);
-							*resultChain.spos_ncp = inv_sample * sum; //NEWLY ADDED
-							*resultChain.sneg_ncp = *resultChain.sncp - *resultChain.spos_ncp; //NEWLY ADDED	
 
-							i32_to_f32_scaleby_inplace(resultChain.spos_ncpPr, (sMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.sneg_ncpPr, (sMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.spos_cpOccPr, N, inv_sample);
+				//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
+				if (extra.tallyPosNegSeasonJump && MODEL.sid>=0) {
 
-							SCPY(N, resultChain.scpOccPr, resultChain.sneg_cpOccPr); //NEWLY ADDED
-							r_ippsSub_32f_I((F32PTR)resultChain.spos_cpOccPr, (F32PTR)resultChain.sneg_cpOccPr, N);   //NEWLY ADDED
-						}
+					GetSum(resultChain.spos_cpOccPr);	
+					*resultChain.spos_ncp = inv_sample * sum; //NEWLY ADDED
+					*resultChain.sneg_ncp = *resultChain.sncp - *resultChain.spos_ncp; //NEWLY ADDED	
+
+					i32_to_f32_scaleby_inplace(resultChain.spos_ncpPr, (sMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.sneg_ncpPr, (sMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.spos_cpOccPr, N, inv_sample);
+ 
+					SCPY(N, resultChain.scpOccPr, resultChain.sneg_cpOccPr); //NEWLY ADDED
+					r_ippsSub_32f_I((F32PTR)resultChain.spos_cpOccPr, (F32PTR)resultChain.sneg_cpOccPr, N);   //NEWLY ADDED
+				}
 
-						//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
-						if (extra.tallyPosNegTrendJump) {
+				//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
+				if (extra.tallyPosNegTrendJump) {
 
-							GetSum(resultChain.tpos_cpOccPr);
-							*resultChain.tpos_ncp = inv_sample * sum; //NEWLY ADDED
-							*resultChain.tneg_ncp = *resultChain.tncp - *resultChain.tpos_ncp; //NEWLY ADDED	
+					GetSum(resultChain.tpos_cpOccPr);	
+					*resultChain.tpos_ncp = inv_sample * sum; //NEWLY ADDED
+					*resultChain.tneg_ncp = *resultChain.tncp - *resultChain.tpos_ncp; //NEWLY ADDED	
+
+					i32_to_f32_scaleby_inplace(resultChain.tpos_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.tneg_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.tpos_cpOccPr, N,				  inv_sample);
+ 
+					SCPY(N, resultChain.tcpOccPr, resultChain.tneg_cpOccPr); //NEWLY ADDED
+					r_ippsSub_32f_I((F32PTR)resultChain.tpos_cpOccPr, (F32PTR)resultChain.tneg_cpOccPr, N);   //NEWLY ADDED
+				}
 
-							i32_to_f32_scaleby_inplace(resultChain.tpos_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.tneg_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.tpos_cpOccPr, N, inv_sample);
 
-							SCPY(N, resultChain.tcpOccPr, resultChain.tneg_cpOccPr); //NEWLY ADDED
-							r_ippsSub_32f_I((F32PTR)resultChain.tpos_cpOccPr, (F32PTR)resultChain.tneg_cpOccPr, N);   //NEWLY ADDED
-						}
+				//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
+				if (extra.tallyIncDecTrendJump) {
 
+					GetSum(resultChain.tinc_cpOccPr);	   
+					*resultChain.tinc_ncp = inv_sample * sum; //NEWLY ADDED
+					*resultChain.tdec_ncp = *resultChain.tncp - *resultChain.tinc_ncp; //NEWLY ADDED	
+
+					i32_to_f32_scaleby_inplace(resultChain.tinc_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.tdec_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.tinc_cpOccPr, N, inv_sample);
 
-						//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
-						if (extra.tallyIncDecTrendJump) {
+					SCPY(N, resultChain.tcpOccPr, resultChain.tdec_cpOccPr); //NEWLY ADDED
+					r_ippsSub_32f_I((F32PTR)resultChain.tinc_cpOccPr, (F32PTR)resultChain.tdec_cpOccPr, N);   //NEWLY ADDED
+				}
 
-							GetSum(resultChain.tinc_cpOccPr);
-							*resultChain.tinc_ncp = inv_sample * sum; //NEWLY ADDED
-							*resultChain.tdec_ncp = *resultChain.tncp - *resultChain.tinc_ncp; //NEWLY ADDED	
 
-							i32_to_f32_scaleby_inplace(resultChain.tinc_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.tdec_ncpPr, (tMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.tinc_cpOccPr, N, inv_sample);
+				//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
+				if (extra.tallyPosNegOutliers && MODEL.oid >= 0) {
 
-							SCPY(N, resultChain.tcpOccPr, resultChain.tdec_cpOccPr); //NEWLY ADDED
-							r_ippsSub_32f_I((F32PTR)resultChain.tinc_cpOccPr, (F32PTR)resultChain.tdec_cpOccPr, N);   //NEWLY ADDED
-						}
+					GetSum(resultChain.opos_cpOccPr);	
+					*resultChain.opos_ncp = inv_sample * sum; //NEWLY ADDED
+					*resultChain.oneg_ncp = *resultChain.oncp - *resultChain.opos_ncp; //NEWLY ADDED	
+
+					i32_to_f32_scaleby_inplace(resultChain.opos_ncpPr, (oMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.oneg_ncpPr, (oMAXNUMKNOT + 1), inv_sample);
+					i32_to_f32_scaleby_inplace(resultChain.opos_cpOccPr, N, inv_sample);
 
+					SCPY(N, resultChain.ocpOccPr, resultChain.oneg_cpOccPr); //NEWLY ADDED
+					r_ippsSub_32f_I((F32PTR)resultChain.opos_cpOccPr, (F32PTR)resultChain.oneg_cpOccPr, N);   //NEWLY ADDED
+				}
 
-						//..tallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJumtallyPosNegSeasonJum.................
-						if (extra.tallyPosNegOutliers && MODEL.oid >= 0) {
+			}// Finish computing the result of the single chiain
 
-							GetSum(resultChain.opos_cpOccPr);
-							*resultChain.opos_ncp = inv_sample * sum; //NEWLY ADDED
-							*resultChain.oneg_ncp = *resultChain.oncp - *resultChain.opos_ncp; //NEWLY ADDED	
 
-							i32_to_f32_scaleby_inplace(resultChain.opos_ncpPr, (oMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.oneg_ncpPr, (oMAXNUMKNOT + 1), inv_sample);
-							i32_to_f32_scaleby_inplace(resultChain.opos_cpOccPr, N, inv_sample);
+			/**************************************************/
+			//   Add up the individual chain to the Result
+			/**************************************************/
+			if (!skipCurrentPixel) 
+			{
+				I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
+				I32   tMAXNUMKNOT = MODEL.tid>=0?  MODEL.b[MODEL.tid].prior.maxKnotNum:-9999999;
+				I32   oMAXNUMKNOT = MODEL.oid>=0?  MODEL.b[MODEL.oid].prior.maxKnotNum:- 9999999;
+
+				//https://stackoverflow.com/questions/13216423/error-pasting-and-red-does-not-give-a-valid-preprocessing-token
+				//#define _1(x)      *(result.##x) += *(resultChain.##x) // Working with MSVC but not GCC
+
+				#define _1(x)      *(result.x) += *(resultChain.x)
+				#define _N(x)      r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N)
+				#define _Nq(x)     r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N*q)
+				#define _q(x)      r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, q)
+				#define _q2(x)      r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, q*q)
+				#define _2N(x)     r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N+N)
+				#define _2Nq(x)     r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N*q+N*q)
+				#define _skn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, sMAXNUMKNOT + 1)
+				#define _tkn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, tMAXNUMKNOT + 1)
+				#define _okn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, oMAXNUMKNOT + 1)
+
+				_1(marg_lik);
+				_q2(sig2);  //Fpr MRBEAST
+				
+				if (MODEL.sid >= 0 || MODEL.vid >0) {
+					_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD);
+					if (extra.computeSeasonOrder)    _N(sorder);
+					if (extra.computeSeasonAmp)      _N(samp), _N(sampSD);
+					if (extra.computeCredible)       _2Nq(sCI);
+				}
 
-							SCPY(N, resultChain.ocpOccPr, resultChain.oneg_cpOccPr); //NEWLY ADDED
-							r_ippsSub_32f_I((F32PTR)resultChain.opos_cpOccPr, (F32PTR)resultChain.oneg_cpOccPr, N);   //NEWLY ADDED
-						}
+				if (MODEL.tid >= 0) {					
+					_1(tncp); _tkn_1(tncpPr);	   _N(tcpOccPr); _Nq(tY); _Nq(tSD);
+					if (extra.computeTrendOrder)   _N(torder);
+					if (extra.computeTrendSlope)   _N(tslp), _N(tslpSD),_N(tslpSgnPosPr), _N(tslpSgnZeroPr);
+					if (extra.computeCredible)     _2Nq(tCI);
+				}
 
-					}// Finish computing the result of the single chiain
+				if (MODEL.oid >= 0) {
+					_1(oncp); _okn_1(oncpPr);	_N(ocpOccPr); _Nq(oY); _Nq(oSD);
+					if (extra.computeCredible)   _2Nq(oCI);
+				}
 
+				if (extra.tallyPosNegSeasonJump && MODEL.sid >=0) {
+					_1(spos_ncp);         _1(sneg_ncp); //NEWLY ADDED					
+					_skn_1(spos_ncpPr);   _skn_1(sneg_ncpPr); //NEWLY ADDED
+					_N(spos_cpOccPr);     _N(sneg_cpOccPr); //NEWLY ADDED	
+				}
 
-					/**************************************************/
-					//   Add up the individual chain to the Result
-					/**************************************************/
-					if (!skipCurrentPixel)
-					{
-						I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
-						I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
-						I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
-
-						//https://stackoverflow.com/questions/13216423/error-pasting-and-red-does-not-give-a-valid-preprocessing-token
-						//#define _1(x)      *(result.##x) += *(resultChain.##x) // Working with MSVC but not GCC
-
-#define _1(x)      *(result.x) += *(resultChain.x)
-#define _N(x)      r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N)
-#define _Nq(x)     r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N*q)
-#define _q(x)      r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, q)
-#define _q2(x)      r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, q*q)
-#define _2N(x)     r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N+N)
-#define _2Nq(x)     r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, N*q+N*q)
-#define _skn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, sMAXNUMKNOT + 1)
-#define _tkn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, tMAXNUMKNOT + 1)
-#define _okn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, oMAXNUMKNOT + 1)
-
-						_1(marg_lik);
-						_q2(sig2);  //Fpr MRBEAST
-
-						if (MODEL.sid >= 0) {
-							_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD);
-							if (extra.computeSeasonOrder)    _N(sorder);
-							if (extra.computeSeasonAmp)      _N(samp), _N(sampSD);
-							if (extra.computeCredible)       _2Nq(sCI);
-						}
-
-						if (MODEL.tid >= 0) {
-							_1(tncp); _tkn_1(tncpPr);	   _N(tcpOccPr); _Nq(tY); _Nq(tSD);
-							if (extra.computeTrendOrder)   _N(torder);
-							if (extra.computeTrendSlope)   _N(tslp), _N(tslpSD), _N(tslpSgnPosPr), _N(tslpSgnZeroPr);
-							if (extra.computeCredible)     _2Nq(tCI);
-						}
-
-						if (MODEL.oid >= 0) {
-							_1(oncp); _okn_1(oncpPr);	_N(ocpOccPr); _Nq(oY); _Nq(oSD);
-							if (extra.computeCredible)   _2Nq(oCI);
-						}
-
-						if (extra.tallyPosNegSeasonJump && MODEL.sid >= 0) {
-							_1(spos_ncp);         _1(sneg_ncp); //NEWLY ADDED					
-							_skn_1(spos_ncpPr);   _skn_1(sneg_ncpPr); //NEWLY ADDED
-							_N(spos_cpOccPr);     _N(sneg_cpOccPr); //NEWLY ADDED	
-						}
-
-						if (extra.tallyPosNegTrendJump) {
-							_1(tpos_ncp);            _1(tneg_ncp); //NEWLY ADDED					
-							_tkn_1(tpos_ncpPr); _tkn_1(tneg_ncpPr); //NEWLY ADDED
-							_N(tpos_cpOccPr);         _N(tneg_cpOccPr); //NEWLY ADDED 
-						}
-
-						if (extra.tallyIncDecTrendJump) {
-							_1(tinc_ncp);         _1(tdec_ncp); //NEWLY ADDED					
-							_tkn_1(tinc_ncpPr); _tkn_1(tdec_ncpPr); //NEWLY ADDED
-							_N(tinc_cpOccPr);     _N(tdec_cpOccPr); //NEWLY ADDED
-						}
-
-						if (extra.tallyPosNegOutliers && MODEL.oid >= 0) {
-							_1(opos_ncp);            _1(oneg_ncp); //NEWLY ADDED					
-							_okn_1(opos_ncpPr);      _okn_1(oneg_ncpPr); //NEWLY ADDED
-							_N(opos_cpOccPr);        _N(oneg_cpOccPr); //NEWLY ADDED 
-						}
-
-#undef _1
-#undef _N
-#undef _Nq 
-#undef _q 
-#undef _q2
-#undef _2N
-#undef _2Nq
-#undef _skn_1
-#undef _tkn_1
-#undef _okn_1
-					}
+				if (extra.tallyPosNegTrendJump ) {
+					_1(tpos_ncp);            _1(tneg_ncp); //NEWLY ADDED					
+				    _tkn_1(tpos_ncpPr); _tkn_1(tneg_ncpPr); //NEWLY ADDED
+					_N(tpos_cpOccPr);         _N(tneg_cpOccPr); //NEWLY ADDED 
+				}
+				
+				if (extra.tallyIncDecTrendJump) {
+					_1(tinc_ncp);         _1(tdec_ncp); //NEWLY ADDED					
+					_tkn_1(tinc_ncpPr); _tkn_1(tdec_ncpPr); //NEWLY ADDED
+					_N(tinc_cpOccPr);     _N(tdec_cpOccPr); //NEWLY ADDED
+				}
+				
+				if (extra.tallyPosNegOutliers && MODEL.oid >= 0) {
+					_1(opos_ncp);            _1(oneg_ncp); //NEWLY ADDED					
+					_okn_1(opos_ncpPr);      _okn_1(oneg_ncpPr); //NEWLY ADDED
+					_N(opos_cpOccPr);        _N(oneg_cpOccPr); //NEWLY ADDED 
+				}	
+ 
+				#undef _1
+				#undef _N
+				#undef _Nq 
+				#undef _q 
+				#undef _q2
+				#undef _2N
+				#undef _2Nq
+				#undef _skn_1
+				#undef _tkn_1
+			    #undef _okn_1
+			}
 
-					// Jump out of the chainumber loop
-					if (skipCurrentPixel) {
-						r_warning("\nWARNING(#%d):The max number of bad iterations exceeded. Can't decompose the current time series\n", skipCurrentPixel);
-						break;
-					}
+			// Jump out of the chainumber loop
+			if (skipCurrentPixel) {
+				q_warning("\nWARNING(#%d):The max number of bad iterations exceeded. Can't decompose the current time series\n", skipCurrentPixel);
+				break;
+			}
 
 
 					/*---------WINDOW-------------------------*/
 					EnterCriticalSection(&gData.cs);
 
 					gData.curChainNumber = chainNumber;
 
@@ -1573,86 +1555,86 @@
 						gData.sN = 0;
 					}
 					gData.tN = *resultChain.tncp;
 					PostMessage(gData.hwnd, WM_USER + 2, 0, 0);
 
 					LeaveCriticalSection(&gData.cs);
 					/*---------WINDOW-------------------------*/
-				}
-				/*********************************/
-				// WHILE(chainNumber<chainNumber)
-				/*********************************/
+		}
+		/*********************************/
+		// WHILE(chainNumber<chainNumber)
+		/*********************************/
 
-				__END_IF_NOT_SKIP_TIMESESIRIES__
-			}
+		__END_IF_NOT_SKIP_TIMESESIRIES__  
+	}
 
-		/******************************************************/
-		//
-		// Finish all the chains and now acverage all of them
-		//
-		/******************************************************/
+	/******************************************************/
+	//
+	// Finish all the chains and now acverage all of them
+	//
+	/******************************************************/
 
-			// Average the results from multiple chains
+		// Average the results from multiple chains
 		if (MCMC_CHAINNUM >= 2 && !skipCurrentPixel)
 		{
-			I32  N = opt->io.N;
-
-			I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
+			I32  N = opt->io.N;			
+	
+			I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 			I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
 			I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
 
-			const F32 invChainNumber = 1.f / (F32)MCMC_CHAINNUM;
+			const F32 invChainNumber = 1.f /(F32)MCMC_CHAINNUM;
 
-#define _1(x)      *((F32PTR)result.x)*=invChainNumber
-#define _N(x)      r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N)
-#define _Nq(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x,N*q)
-#define _q(x)      r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x,q)
-#define _q2(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x,q*q)
-#define _2N(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N+N)
-#define _2Nq(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N*q+N*q)
-#define _skn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, sMAXNUMKNOT + 1)
-#define _tkn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, tMAXNUMKNOT + 1)
-#define _okn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, oMAXNUMKNOT + 1)
+			#define _1(x)      *((F32PTR)result.x)*=invChainNumber
+			#define _N(x)      r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N)
+			#define _Nq(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x,N*q)
+			#define _q(x)      r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x,q)
+			#define _q2(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x,q*q)
+			#define _2N(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N+N)
+			#define _2Nq(x)     r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N*q+N*q)
+			#define _skn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, sMAXNUMKNOT + 1)
+			#define _tkn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, tMAXNUMKNOT + 1)
+			#define _okn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, oMAXNUMKNOT + 1)
 
-			F32 maxncpProb;
-			_1(marg_lik);
+			F32 maxncpProb;	 
+			_1(marg_lik);			
 			_q2(sig2);
-			if (MODEL.sid >= 0) {
-				_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD);
+			if (MODEL.sid >= 0 || MODEL.vid>0) {
+				_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD); 
 				if (extra.computeSeasonOrder)    _N(sorder);
-				if (extra.computeSeasonAmp) { _N(samp), _N(sampSD); }
+				if (extra.computeSeasonAmp)     {_N(samp), _N(sampSD);}
 				if (extra.computeCredible)       _2Nq(sCI);
-
-				*result.sncp_mode = f32_maxidx(result.sncpPr, sMAXNUMKNOT + 1, &maxncpProb);
+ 
+				*result.sncp_mode   = f32_maxidx(result.sncpPr,       sMAXNUMKNOT + 1, &maxncpProb);
 				*result.sncp_median = GetPercentileNcp(result.sncpPr, sMAXNUMKNOT + 1, 0.5);
-				*result.sncp_pct90 = GetPercentileNcp(result.sncpPr, sMAXNUMKNOT + 1, 0.9);
-				*result.sncp_pct10 = GetPercentileNcp(result.sncpPr, sMAXNUMKNOT + 1, 0.1);
+				*result.sncp_pct90  = GetPercentileNcp(result.sncpPr, sMAXNUMKNOT + 1, 0.9);
+				*result.sncp_pct10  = GetPercentileNcp(result.sncpPr, sMAXNUMKNOT + 1, 0.1);
 			}
 
 			if (MODEL.tid >= 0) {
-				_1(tncp); _tkn_1(tncpPr);	     _N(tcpOccPr); _Nq(tY); _Nq(tSD);
+				_1(tncp); _tkn_1(tncpPr);	     _N(tcpOccPr); _Nq(tY); _Nq(tSD); 
 				if (extra.computeTrendOrder)     _N(torder);
-				if (extra.computeTrendSlope) { _N(tslp), _N(tslpSD), _N(tslpSgnPosPr), _N(tslpSgnZeroPr); }
+				if (extra.computeTrendSlope)    { _N(tslp), _N(tslpSD), _N(tslpSgnPosPr), _N(tslpSgnZeroPr);}
 				if (extra.computeCredible)       _2Nq(tCI);
 
-				*result.tncp_mode = f32_maxidx(result.tncpPr, tMAXNUMKNOT + 1, &maxncpProb);
+				*result.tncp_mode   = f32_maxidx(result.tncpPr,       tMAXNUMKNOT + 1, &maxncpProb);
 				*result.tncp_median = GetPercentileNcp(result.tncpPr, tMAXNUMKNOT + 1, 0.5);
-				*result.tncp_pct90 = GetPercentileNcp(result.tncpPr, tMAXNUMKNOT + 1, 0.9);
-				*result.tncp_pct10 = GetPercentileNcp(result.tncpPr, tMAXNUMKNOT + 1, 0.1);
+				*result.tncp_pct90  = GetPercentileNcp(result.tncpPr, tMAXNUMKNOT + 1, 0.9);
+				*result.tncp_pct10  = GetPercentileNcp(result.tncpPr, tMAXNUMKNOT + 1, 0.1);
 			}
 
 			if (MODEL.oid >= 0) {
-				_1(oncp); _okn_1(oncpPr);
+				_1(oncp); _okn_1(oncpPr);	   
 				_N(ocpOccPr); _Nq(oY); _Nq(oSD);
 				if (extra.computeCredible)      _2Nq(oCI);
 
-				*result.oncp_mode = f32_maxidx(result.oncpPr, oMAXNUMKNOT + 1, &maxncpProb);
+				*result.oncp_mode   = f32_maxidx(result.oncpPr,       oMAXNUMKNOT + 1, &maxncpProb);
 				*result.oncp_median = GetPercentileNcp(result.oncpPr, oMAXNUMKNOT + 1, 0.5);
-				*result.oncp_pct90 = GetPercentileNcp(result.oncpPr, oMAXNUMKNOT + 1, 0.9);
-				*result.oncp_pct10 = GetPercentileNcp(result.oncpPr, oMAXNUMKNOT + 1, 0.1);
+				*result.oncp_pct90  = GetPercentileNcp(result.oncpPr, oMAXNUMKNOT + 1, 0.9);
+				*result.oncp_pct10  = GetPercentileNcp(result.oncpPr, oMAXNUMKNOT + 1, 0.1);
 			}
 
 			/****************************************************************/
 
 			if (extra.tallyPosNegSeasonJump && MODEL.sid >= 0) {
 				_1(spos_ncp);             _1(sneg_ncp); //NEWLY ADDED					
 				_skn_1(spos_ncpPr);    _skn_1(sneg_ncpPr); //NEWLY ADDED
@@ -1675,115 +1657,115 @@
 
 			if (extra.tallyPosNegOutliers && MODEL.oid >= 0) {
 				_1(opos_ncp);            _1(oneg_ncp); //NEWLY ADDED					
 				_okn_1(opos_ncpPr); _okn_1(oneg_ncpPr); //NEWLY ADDED
 				_N(opos_cpOccPr);         _N(oneg_cpOccPr); //NEWLY ADDED 
 			}
 
-
-#undef _1
-#undef _N
-#undef _2N
-#undef _skn_1
-#undef _tkn_1
-#undef _okn_1
+ 
+			#undef _1
+			#undef _N
+			#undef _2N
+			#undef _skn_1
+			#undef _tkn_1
+			#undef _okn_1
 		}
-		if (!skipCurrentPixel) {
-			I32  N = opt->io.N;
-			if (MODEL.sid >= 0) 							tsRemoveNaNs(result.sSD, N);
+		if (!skipCurrentPixel) {		
+			I32  N = opt->io.N;  
+			if (MODEL.sid >= 0||MODEL.vid>0) 				tsRemoveNaNs(result.sSD, N);
 			if (MODEL.tid >= 0)								tsRemoveNaNs(result.tSD, N);
-			if (MODEL.tid >= 0 && extra.computeTrendSlope)  tsRemoveNaNs(result.tslpSD, N);
+			if (MODEL.tid >= 0 && extra.computeTrendSlope)  tsRemoveNaNs(result.tslpSD, N);		 
 			if (MODEL.oid >= 0) 							tsRemoveNaNs(result.oSD, N);
 		}
 
 		// Compute Changepoints and their confidence intervals
 		if (!skipCurrentPixel)
 		{
-			I32     N = opt->io.N;
-			F32     nan = getNaN();     //A sloppy way to get a NAN
+			I32     N         = opt->io.N;
+			F32     nan       = getNaN();     //A sloppy way to get a NAN
 
-			F32  	threshold = 0.001f;
-			F32PTR	mem = Xnewterm;  //Xnewterm must have a length larger than or equla to 5*N + max(sncp, tncp);
-			I32PTR  cptList = (I32PTR)mem + 5LL * N;
+			F32  	threshold = 0.01f;
+			F32PTR	mem       = Xnewterm;  //Xnewterm must have a length larger than or equla to 5*N + max(sncp, tncp);
+			I32PTR  cptList   = (I32PTR)mem + 5LL * N;
 			F32PTR  cptCIList = (F32PTR)mem + 6LL * N;
 
 			I32   cptNumber;
 			I32   trueCptNumber;
 			F32   maxncpProb;
 			const F32 T0 = (F32)opt->io.meta.startTime;
 			const F32 dT = (F32)opt->io.meta.deltaTime;
 
-			I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
+			I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 			I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
 			I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
 
-			I32   sMINSEPDIST = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.minSepDist : -9999999;
+			I32   sMINSEPDIST = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.minSepDist : -9999999;
 			I32   tMINSEPDIST = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.minSepDist : -9999999;
-			I32   oMINSEPDIST = MODEL.oid >= 0 ? 1 : -9999999;
+			I32   oMINSEPDIST = MODEL.oid >= 0 ? 0 : -9999999;  //changed from 1 to 0 to pick up consecutive outlier spikes.
 
 			//--------------Season----------------------------
-			if (extra.computeSeasonChngpt && MODEL.sid >= 0) {
-				cptNumber = sMAXNUMKNOT;
+			if (extra.computeSeasonChngpt && (MODEL.sid >=0 || MODEL.vid>0 ))  	{
+				cptNumber      = sMAXNUMKNOT;
 				trueCptNumber = FindChangepoint((F32PTR)result.scpOccPr, mem, threshold, cptList, cptCIList, N, sMINSEPDIST, cptNumber);
 				//In the returned result, cptList is a list of detected changepoints, which are all zero-based indices.
 				//That is, a changepoint occurring at t1 has a value of 0.
 
 				for (int i = 0; i < trueCptNumber; i++) {
-					*(result.scp + i) = (F32)(*(cptList + i)) * dT + T0;
-					*(result.scpPr + i) = (F32)mem[i];
+					*(result.scp + i)	  = (F32)(*(cptList + i)) * dT + T0;
+					*(result.scpPr + i)   = (F32)mem[i];
 					I32 cptLoc = cptList[i] == 0 ? 1 : cptList[i];
 					for (int j = 0; j < q; ++j) {
-						*(result.scpAbruptChange + j * sMAXNUMKNOT + i) = result.sY[j * N + cptLoc] - result.sY[j * N + cptLoc - 1];
-					}
+						*(result.scpAbruptChange +j*sMAXNUMKNOT + i) =	result.sY[j*N+cptLoc] - result.sY[j*N+cptLoc - 1];
+					}					
 				}
 				for (int i = trueCptNumber; i < sMAXNUMKNOT; i++) {
-					*(result.scp + i) = nan,
-						* (result.scpPr + i) = nan;
+					*(result.scp + i)             = nan,
+					*(result.scpPr + i)           = nan;
 					for (int j = 0; j < q; ++j) {
-						*(result.scpAbruptChange + j * sMAXNUMKNOT + i) = nan;
-					}
+						*(result.scpAbruptChange + j * sMAXNUMKNOT+ i) = nan;
+					}					
 				}
 				for (int i = 0; i < trueCptNumber; i++)
 					*(result.scpCI + i) = (F32)(*(cptCIList + i)) * dT + T0,
-					* (result.scpCI + sMAXNUMKNOT + i) = (F32)(*(cptCIList + trueCptNumber + i)) * dT + T0;
+					*(result.scpCI + sMAXNUMKNOT + i) = (F32)(*(cptCIList + trueCptNumber + i)) * dT + T0;
 				for (int i = trueCptNumber; i < sMAXNUMKNOT; i++)
 					*(result.scpCI + i) = nan,
-					* (result.scpCI + sMAXNUMKNOT + i) = nan;
+					*(result.scpCI + sMAXNUMKNOT + i) = nan;
 			}
 
 			//--------------Trend----------------------------
 			if (extra.computeTrendChngpt) {
-				cptNumber = tMAXNUMKNOT;
+				cptNumber     = tMAXNUMKNOT;
 				trueCptNumber = FindChangepoint((F32PTR)result.tcpOccPr, mem, threshold, cptList, cptCIList, N, tMINSEPDIST, cptNumber);
 				for (int i = 0; i < trueCptNumber; i++) {
-					*(result.tcp + i) = (F32)(*(cptList + i)) * dT + T0,
-						* (result.tcpPr + i) = (F32)mem[i];
+					*(result.tcp + i)          = (F32)(*(cptList + i)) * dT + T0,
+					*(result.tcpPr + i)         = (F32)mem[i];
 					I32 cptLoc = cptList[i] == 0 ? 1 : cptList[i];
 					for (int j = 0; j < q; ++j) {
-						*(result.tcpAbruptChange + j * tMAXNUMKNOT + i) = result.tY[j * N + cptLoc] - result.tY[j * N + cptLoc - 1];
+						*(result.tcpAbruptChange + j*tMAXNUMKNOT + i) = result.tY[j * N + cptLoc] - result.tY[j * N + cptLoc - 1];
 					}
 				}
 				for (int i = trueCptNumber; i < tMAXNUMKNOT; i++) {
-					*(result.tcp + i) = nan,
-						* (result.tcpPr + i) = nan;
+					*(result.tcp + i)   = nan,
+					*(result.tcpPr + i) = nan;
 					for (int j = 0; j < q; ++j) {
 						*(result.tcpAbruptChange + j * tMAXNUMKNOT + i) = nan;
-					}
-				}
+					}					
+				}					
 				for (int i = 0; i < trueCptNumber; i++)
 					*(result.tcpCI + i) = (F32)(*(cptCIList + i)) * dT + T0,
-					* (result.tcpCI + tMAXNUMKNOT + i) = (F32)(*(cptCIList + trueCptNumber + i)) * dT + T0;
+					*(result.tcpCI + tMAXNUMKNOT + i) = (F32)(*(cptCIList + trueCptNumber + i)) * dT + T0;
 				for (int i = trueCptNumber; i < tMAXNUMKNOT; i++)
 					*(result.tcpCI + i) = nan,
-					* (result.tcpCI + tMAXNUMKNOT + i) = nan;
+					*(result.tcpCI + tMAXNUMKNOT + i) = nan;
 			}
-
+	 
 
 			/**************************************************************************************************/
-#define GET_CHANGPOINTS(NcpProb, KNOTNUM, MINSEP, MAX_KNOTNUM, Y, CpOccPr, CP, CPPROB, CP_CHANGE, CP_CI)    \
+			#define GET_CHANGPOINTS(NcpProb, KNOTNUM, MINSEP, MAX_KNOTNUM, Y, CpOccPr, CP, CPPROB, CP_CHANGE, CP_CI)    \
 			cptNumber     = MAX_KNOTNUM;  \
 			trueCptNumber = FindChangepoint((F32PTR)CpOccPr, mem, threshold, cptList, cptCIList, N, MINSEP, cptNumber);\
 			for (int i = 0; i < trueCptNumber; i++) {\
 				*(CP + i)        = (F32) cptList[i]* dT + T0,\
 				*(CPPROB+ i)     = (F32) mem[i];\
 		         I32 cptLoc      = cptList[i] == 0 ? 1 : cptList[i];\
 				 *(CP_CHANGE + i) = Y[cptLoc] - Y[cptLoc - 1];\
@@ -1798,38 +1780,38 @@
 				*(CP_CI + MAX_KNOTNUM + i) = (F32)(*(cptCIList + trueCptNumber + i)) * dT + T0;\
 			for (int i = trueCptNumber; i < MAX_KNOTNUM; i++)\
 				*(CP_CI + i)               = nan,\
 				*(CP_CI + MAX_KNOTNUM + i) = nan;
 			/**************************************************************************************************/
 
 			if (extra.tallyPosNegSeasonJump && MODEL.sid >= 0) {
-				GET_CHANGPOINTS(result.spos_ncpPr, result.spos_ncp, sMINSEPDIST, sMAXNUMKNOT, result.samp,
+				GET_CHANGPOINTS(result.spos_ncpPr ,result.spos_ncp, sMINSEPDIST, sMAXNUMKNOT, result.samp,
 					result.spos_cpOccPr, result.spos_cp, result.spos_cpPr, result.spos_cpAbruptChange, result.spos_cpCI);
 
-				GET_CHANGPOINTS(result.sneg_ncpPr, result.sneg_ncp, sMINSEPDIST, sMAXNUMKNOT, result.samp,
+				GET_CHANGPOINTS(result.sneg_ncpPr,result.sneg_ncp, sMINSEPDIST, sMAXNUMKNOT, result.samp,
 					result.sneg_cpOccPr, result.sneg_cp, result.sneg_cpPr, result.sneg_cpAbruptChange, result.sneg_cpCI);
-			}
+			}			
 			if (extra.tallyPosNegTrendJump) {
 				GET_CHANGPOINTS(result.tpos_ncpPr, result.tpos_ncp, tMINSEPDIST, tMAXNUMKNOT, result.tY,
 					result.tpos_cpOccPr, result.tpos_cp, result.tpos_cpPr, result.tpos_cpAbruptChange, result.tpos_cpCI);
 
 				GET_CHANGPOINTS(result.tneg_ncpPr, result.tneg_ncp, tMINSEPDIST, tMAXNUMKNOT, result.tY,
 					result.tneg_cpOccPr, result.tneg_cp, result.tneg_cpPr, result.tneg_cpAbruptChange, result.tneg_cpCI);
 			}
 			if (extra.tallyIncDecTrendJump) {
-				GET_CHANGPOINTS(result.tinc_ncpPr, result.tinc_ncp, tMINSEPDIST, tMAXNUMKNOT, result.tslp,
+				GET_CHANGPOINTS(result.tinc_ncpPr,result.tinc_ncp, tMINSEPDIST, tMAXNUMKNOT, result.tslp,
 					result.tinc_cpOccPr, result.tinc_cp, result.tinc_cpPr, result.tinc_cpAbruptChange, result.tinc_cpCI);
 
-				GET_CHANGPOINTS(result.tdec_ncpPr, result.tdec_ncp, tMINSEPDIST, tMAXNUMKNOT, result.tslp,
+				GET_CHANGPOINTS(result.tdec_ncpPr,result.tdec_ncp, tMINSEPDIST, tMAXNUMKNOT, result.tslp,
 					result.tdec_cpOccPr, result.tdec_cp, result.tdec_cpPr, result.tdec_cpAbruptChange, result.tdec_cpCI);
 			}
 
 
 			/**************************************************************************************************/
-#define OGET_CHANGPOINTS(NcpProb, KNOTNUM,MINSEP, MAX_KNOTNUM, PROBCURVE, CP, CPPROB,CP_CI)    \
+			#define OGET_CHANGPOINTS(NcpProb, KNOTNUM,MINSEP, MAX_KNOTNUM, PROBCURVE, CP, CPPROB,CP_CI)    \
 			cptNumber     = MAX_KNOTNUM;  \
 			trueCptNumber = FindChangepoint((F32PTR)PROBCURVE, mem, threshold, cptList, cptCIList, N, MINSEP, cptNumber);\
 			for (int i = 0; i < trueCptNumber; i++) {\
 				*(CP + i)        = (F32) cptList[i]* dT + T0;\
 				*(CPPROB+ i)     = (F32) mem[i];\
 		         I32 cptLoc      = cptList[i] == 0 ? 1 : cptList[i];\
 			}\
@@ -1842,165 +1824,165 @@
 				*(CP_CI + MAX_KNOTNUM + i) = (F32)(*(cptCIList + trueCptNumber + i)) * dT + T0;\
 			for (int i = trueCptNumber; i < MAX_KNOTNUM; i++)\
 				*(CP_CI + i)               = nan,\
 				*(CP_CI + MAX_KNOTNUM + i) = nan;
 			/**************************************************************************************************/
 
 			if (extra.computeOutlierChngpt) {
-				OGET_CHANGPOINTS(result.oncpPr, result.oncp, oMINSEPDIST, oMAXNUMKNOT, result.ocpOccPr, result.ocp, result.ocpPr, result.ocpCI);
+				OGET_CHANGPOINTS(result.oncpPr,result.oncp, oMINSEPDIST, oMAXNUMKNOT, result.ocpOccPr, result.ocp, result.ocpPr, result.ocpCI);
 			}
 
-			if (extra.tallyPosNegOutliers && MODEL.oid >= 0) {
-				OGET_CHANGPOINTS(result.opos_ncpPr, result.opos_ncp, oMINSEPDIST, oMAXNUMKNOT,
+			if (extra.tallyPosNegOutliers && MODEL.oid >=0) {
+				OGET_CHANGPOINTS(result.opos_ncpPr,result.opos_ncp, oMINSEPDIST, oMAXNUMKNOT,
 					result.opos_cpOccPr, result.opos_cp, result.opos_cpPr, result.opos_cpCI);
 
-				OGET_CHANGPOINTS(result.oneg_ncpPr, result.oneg_ncp, oMINSEPDIST, oMAXNUMKNOT,
+				OGET_CHANGPOINTS(result.oneg_ncpPr,result.oneg_ncp, oMINSEPDIST, oMAXNUMKNOT,
 					result.oneg_cpOccPr, result.oneg_cp, result.oneg_cpPr, result.oneg_cpCI);
 			}
 
 
 		}
-
+		
 
 		// Recover the orignal Y values if the pixel is not skipped; the value will be needed below 
 		// to dump into the output and compute R2 and RMSE. Here Xnewterm is used a buff
 		// should not be touched until after the computation of R2 and RMSE
-		if (!skipCurrentPixel) {
-			I32  N = opt->io.N;
+		if ( !skipCurrentPixel) {	
+			I32  N  = opt->io.N;	
 			I32  Nq = N * q;  // For MRBEAST
 
 			for (int i = 0; i < q; ++i) {
-				memcpy(Xnewterm + N * i, yInfo.Y + N * i, sizeof(F32) * N);
-				f32_scale_inplace(yInfo.sd[i], yInfo.mean[i], Xnewterm + N * i, N);
+				memcpy(Xnewterm+N*i, yInfo.Y + N*i, sizeof(F32)* N);
+				f32_scale_inplace(yInfo.sd[i], yInfo.mean[i], Xnewterm+N*i, N);
 
 				F32PTR NULL_BUF_FOR_VALUES = (Xnewterm + N * i) + N;
 				if (yInfo.nMissing > 0) {
-					f32_gatherVec_scatterVal_byindex(Xnewterm + N * i, yInfo.rowsMissing, NULL_BUF_FOR_VALUES, getNaN(), yInfo.nMissing);
+					f32_gatherVec_scatterVal_byindex(Xnewterm + N*i, yInfo.rowsMissing, NULL_BUF_FOR_VALUES, getNaN(), yInfo.nMissing);
 				}
-			}
+			}			
 		}
 
 		if (opt->extra.dumpInputData && result.data != NULL) {
 			I32  N = opt->io.N;
 			I32  Nq = N * q;  // For MRBEAST
-			memcpy(result.data, Xnewterm, sizeof(F32) * Nq);
+			memcpy(result.data, Xnewterm, sizeof(F32)* Nq);
 		}
 
 		// Compute R2 and RMSE
 		// At this point, yInfo.Y is not used any longer, so is re-used
 		// to stote the sume of fitted S,T and/or O.
 		// Xnewterm still contains the orignal data and shiuldn't not be touched
-		if (!skipCurrentPixel) {
-
-			I32  N = opt->io.N;
+  		if (!skipCurrentPixel) { 
+			
+			I32  N  = opt->io.N ;
 			I32  Nq = N * q;  // For MRBEAST
 
-			I08 hasSeasonCmpnt = opt->prior.basisType[0] == SEASONID || opt->prior.basisType[0] == DUMMYID || opt->prior.basisType[0] == SVDID;
+			I08 hasSeasonCmpnt  = opt->prior.basisType[0] == SEASONID || opt->prior.basisType[0] == DUMMYID || opt->prior.basisType[0] == SVDID;
 			I08 hasOutlierCmpnt = opt->prior.basisType[opt->prior.numBasis - 1] == OUTLIERID;
-			I08 hasTrendCmpnt = 1;
+			I08 hasTrendCmpnt   = 1;
 			//Xnewterm is used at this point and should not be touched!
-			F32PTR BUF = yInfo.Y;
+			F32PTR BUF      = yInfo.Y;
 			f32_fill_val(0., BUF, Nq);
-
+	
 			if (hasTrendCmpnt)   f32_add_vec_inplace(result.tY, BUF, Nq);
 			if (hasSeasonCmpnt)  f32_add_vec_inplace(result.sY, BUF, Nq);
 			if (hasOutlierCmpnt) f32_add_vec_inplace(result.oY, BUF, Nq);
-
+		
 			for (int j = 0; j < q; ++j) {
 				//For MRBEAST
-				F32 r = f32_corr_rmse_nan(BUF + N * j, Xnewterm + N * j, N, &result.RMSE[j]);
+				F32 r = f32_corr_rmse_nan(BUF+N*j, Xnewterm + N*j, N, &result.RMSE[j]);
 				result.R2[j] = r * r;
 			}
-
+			
 		}
 
 		// Smooth the changepoint occurance probability curve
 		if (!skipCurrentPixel) {
 			I32  N = opt->io.N;
 
-			I08 hasSeasonCmpnt = opt->prior.basisType[0] == SEASONID || opt->prior.basisType[0] == DUMMYID || opt->prior.basisType[0] == SVDID;
+			I08 hasSeasonCmpnt  = opt->prior.basisType[0] == SEASONID || opt->prior.basisType[0] == DUMMYID || opt->prior.basisType[0] == SVDID;
 			I08 hasOutlierCmpnt = opt->prior.basisType[opt->prior.numBasis - 1] == OUTLIERID;
-			I08 hasTrendCmpnt = 1;
-
+			I08 hasTrendCmpnt   = 1;
+ 
 			F32PTR BUF = Xnewterm;
-			if (hasTrendCmpnt && opt->extra.smoothCpOccPrCurve) {
-				memcpy(BUF, result.tcpOccPr, sizeof(F32) * N);
-				f32_sumfilter(BUF, result.tcpOccPr, N, opt->prior.trendMinSepDist);
+			if (hasTrendCmpnt && opt->extra.smoothCpOccPrCurve) {	
+				memcpy(BUF, result.tcpOccPr, sizeof(F32)* N);
+				f32_sumfilter(BUF, result.tcpOccPr,N, opt->prior.trendMinSepDist);
 			}
 			if (hasSeasonCmpnt && opt->extra.smoothCpOccPrCurve) {
-				memcpy(BUF, result.scpOccPr, sizeof(F32) * N);
+				memcpy(BUF, result.scpOccPr, sizeof(F32)* N);
 				f32_sumfilter(BUF, result.scpOccPr, N, opt->prior.seasonMinSepDist);
-			}
+			}	
 		}
 
 
-		if (skipCurrentPixel) BEAST2_Result_FillMEM(&result, opt, getNaN());
+	    if (skipCurrentPixel) BEAST2_Result_FillMEM(&result, opt, getNaN());
 		/*********************************************/
 		//Write outputs to the mem array or files	
-		/*********************************************/
+		/*********************************************/	
 		if (!skipCurrentPixel) {
 			int N = opt->io.N;
 			for (int i = 0; i < q; ++i) {
 				if (yInfo.Yseason) {
-					//If Y has been deseaonalized, add it back
-					r_ippsAdd_32f_I(yInfo.Yseason + N * i, result.sY + N * i, N);
+				//If Y has been deseaonalized, add it back
+						r_ippsAdd_32f_I(yInfo.Yseason + N*i,   result.sY+N* i, N);
 					if (result.sCI) {
-						r_ippsAdd_32f_I(yInfo.Yseason + N * i, result.sCI + 2 * N * i, N);
-						r_ippsAdd_32f_I(yInfo.Yseason + N * i, result.sCI + 2 * N * i + N, N);
+						r_ippsAdd_32f_I(yInfo.Yseason + N * i, result.sCI + 2*N*i, N);
+						r_ippsAdd_32f_I(yInfo.Yseason + N * i, result.sCI + 2*N*i+ N, N);
 					}
 					if (extra.dumpInputData)
-						r_ippsAdd_32f_I(yInfo.Yseason + N * i, result.data + N * i, N);
+						r_ippsAdd_32f_I(yInfo.Yseason + N * i, result.data+N*i, N);
 				}
 				if (yInfo.Ytrend) {
-					//If Y has been detrended, add it back
-					r_ippsAdd_32f_I(yInfo.Ytrend + N * i, result.tY + N * i, N);
+				//If Y has been detrended, add it back
+						r_ippsAdd_32f_I(yInfo.Ytrend + N * i, result.tY + N*i, N);
 					if (result.tCI) {
-						r_ippsAdd_32f_I(yInfo.Ytrend + N * i, result.tCI + 2 * N * i, N);
-						r_ippsAdd_32f_I(yInfo.Ytrend + N * i, result.tCI + 2 * N * i + N, N);
+						r_ippsAdd_32f_I(yInfo.Ytrend + N * i, result.tCI+ 2*N*i,   N);
+						r_ippsAdd_32f_I(yInfo.Ytrend + N * i, result.tCI+ 2*N*i+N, N);
 					}
 					if (extra.dumpInputData)
 						r_ippsAdd_32f_I(yInfo.Ytrend + N * i, result.data + N * i, N);
 				}
 			} //for (int i = 0; i < q; ++i)
 		}
 
-
+	 
 		BEAST2_WriteOutput(opt, &result, pixelIndex);
-
-
+		 
+		  
 
 		//if (!skipCurrentPixel)	NUM_OF_PROCESSED_GOOD_PIXELS++; //avoid the branch
 		NUM_OF_PROCESSED_GOOD_PIXELS += !skipCurrentPixel;  //this is a global variable.
 		NUM_OF_PROCESSED_PIXELS++;							//this is also a global variable.
 
 
 		F64 elaspedTime = GetElaspedTimeFromBreakPoint();
-		if (NUM_OF_PROCESSED_GOOD_PIXELS > 0 && NUM_PIXELS > 1 && (pixelIndex % 50 == 0 || elaspedTime > 1)) {
-			F64 estTimeForCompletion = GetElapsedSecondsSinceStart() / NUM_OF_PROCESSED_GOOD_PIXELS * (NUM_PIXELS - pixelIndex);
+		if (NUM_OF_PROCESSED_GOOD_PIXELS > 0 && NUM_PIXELS > 1 && (pixelIndex % 50 == 0 || elaspedTime > 1)) 		{
+			F64 estTimeForCompletion = GetElapsedSecondsSinceStart()/NUM_OF_PROCESSED_GOOD_PIXELS * (NUM_PIXELS - pixelIndex);
 			printProgress2((F32)pixelIndex / NUM_PIXELS, estTimeForCompletion, extra.consoleWidth, Xnewterm, 0);
 			if (elaspedTime > 1) SetBreakPointForStartedTimer();
 		}
 
-#ifdef __DEBUG__
-		r_printf("TREND: birth%4d/%-5d|death%4d/%-5d|merge%4d/%-5d|move%4d/%-5d|chorder%4d/%-5d\n",
-			accT[0], flagT[0], accT[1], flagT[1], accT[2], flagT[2], accT[3], flagT[3], accT[4], flagT[4]);
+		#ifdef __DEBUG__
+		r_printf("TREND: birth%4d/%-5d|death%4d/%-5d|merge%4d/%-5d|move%4d/%-5d|chorder%4d/%-5d\n", 
+			      accT[0], flagT[0] , accT[1], flagT[1], accT[2], flagT[2], accT[3], flagT[3], accT[4], flagT[4]);
 		r_printf("SEASN: birth%4d/%-5d|death%4d/%-5d|merge%4d/%-5d|move%4d/%-5d|chorder%4d/%-5d\n",
-			accS[0], flagS[0], accS[1], flagS[1], accS[2], flagS[2], accS[3], flagS[3], accS[4], flagS[4]);
-#endif
+			      accS[0], flagS[0], accS[1], flagS[1], accS[2], flagS[2], accS[3], flagS[3], accS[4], flagS[4]);
+		#endif
 
 	} //for (U32 pixelIndex = 1; pixelIndex <= TOTALNUMPIXELS; pixelIndex++)
 
 
 	/***********************************************************/
 	// This is the ending bracekt of the iteration through pixels
 	/***********************************************************/
 
 	r_vslDeleteStream(&stream);
 	MEM.free_all(&MEM);
-
+ 
 	/*---------WINDOW-------------------------*/
 	PostMessage(gData.hwnd, WM_USER + 1, 0, 0);
 
 	EnterCriticalSection(&gData.cs);
 	gData.t = NULL;
 	gData.y = NULL;
 	gData.s = NULL;
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_COREV4_mthrd.c` & `Rbeast-0.1.14/ext_src/beastv2_COREV4_mthrd.c`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,16 @@
 			if (MODEL.b[i].type == SEASONID|| MODEL.b[i].type == DUMMYID || MODEL.b[i].type == SVDID)
 				ci[i].result     = resultChain.sCI,		         //season		
 			    ci[i].newDataRow = Xnewterm + XnewtermOffset;	 //season		
 			else if (MODEL.b[i].type == TRENDID)
 				ci[i].result     = resultChain.tCI,               //trend			
 			    ci[i].newDataRow = Xnewterm  + XnewtermOffset;    //trend		
 			else if (MODEL.b[i].type == OUTLIERID)
-				ci[i].result     = resultChain.oCI,      //outlier
-			    ci[i].newDataRow = Xnewterm + XnewtermOffset; //outlier       
+				ci[i].result     = resultChain.oCI,               //outlier
+			    ci[i].newDataRow = Xnewterm + XnewtermOffset;     //outlier       
 
 			XnewtermOffset += Npad * q;   //FOR MRBEAST
 		}
 	} //NUMVAR_FOR_CI=3
 
 	const CORESULT coreResults[MAX_NUM_BASIS];
 	SetupPointersForCoreResults(coreResults, MODEL.b, MODEL.NUMBASIS, &resultChain);
@@ -167,14 +167,15 @@
 	const U32  NUM_PIXELS    = opt->io.numOfPixels;
 	const U32  MCMC_SAMPLES  = opt->mcmc.samples;
 	const U32  MCMC_THINNING = opt->mcmc.thinningFactor;
 	const U32  MCMC_BURNIN   = opt->mcmc.burnin;
 	const U32  MCMC_CHAINNUM = opt->mcmc.chainNumber;
 	const U16  SEASON_BTYPE  = opt->prior.seasonBasisFuncType;
 	const U16  GROUP_MatxMat = (MODEL.sid <0 || opt->prior.seasonBasisFuncType != 3 )
+						       && (MODEL.vid < 0 || opt->prior.trendBasisFuncType != 3)
 							   && (MODEL.tid<0  || opt->prior.trendBasisFuncType!=2)
 		                       && ( MODEL.oid<0 || opt->prior.outlierBasisFuncType!=2);
 
 	/***********MULTITHREAD*******************/
 	//The next two global variables will be set in the main thread
 	//because if kept here, they can be wrongly initialized multiple times
 	//NUM_OF_PROCESSED_GOOD_PIXELS = 0; //this is a global variable.
@@ -189,15 +190,15 @@
 			pthread_mutex_unlock(&mutex);
 			continue;
 		}
 		pthread_mutex_unlock(&mutex);
 		/***********MULTITHREAD*******************/
 		// Fecth a new time-series: set up Y, nMissing,  n, rowsMissing		
 		F32PTR MEMBUF           = Xnewterm; // Xnewterm is a temp mem buf.
-		BEAST2_fetch_next_timeSeries(&yInfo, pixelIndex,  MEMBUF, &(opt->io));
+		BEAST2_fetch_timeSeries(&yInfo, pixelIndex,  MEMBUF, &(opt->io));
 
 
 		F32PTR  Xtmp             = Xt_mars;
 		U08     skipCurrentPixel = BEAST2_preprocess_timeSeries(&yInfo, MODEL.b, Xtmp, opt);		
 	
 
 		#ifdef __DEBUG__
@@ -598,15 +599,15 @@
 						   precFunc.ComputeMargLik(&MODEL.curr, &MODEL, &yInfo, &hyperPar);
 
 						   /***********MULTITHREAD*******************/
 						   //r_printf is not thread-safe.
 						   //#if !(defined(R_RELEASE) || defined(M_RELEASE))
 						   //r_printf("prec: %.4f| marg_lik_prop: %.4f | marg_like_curr: %.4f \n", MODEL.precVec[0], MODEL.prop.marg_lik, MODEL.curr.marg_lik);
 						   //#endif
-                           /***********MULTITHREAD*******************/
+                           			   /***********MULTITHREAD*******************/
 
 						   continue;
 					   }  else {
 						   skipCurrentPixel = 2;
 						   break;
 					   }					   
 				   }  else {
@@ -655,15 +656,15 @@
 
 					//Recover the orignal vaules for those rows corresponding to missing Y values
 					if (yInfo.nMissing > 0 && Knewterm > 0 /*&& basis->type != OUTLIERID*/)  //needed for basisFunction_OUliter=1						
 						f32_mat_multirows_set_by_submat(Xnewterm, Npad, Knewterm, Xt_zeroBackup, yInfo.rowsMissing, yInfo.nMissing);
 
 					// Inserting XnewTerms into Xt_mars
 					if (NewCol.k2_old != KOLD && NewCol.k2_new != NewCol.k2_old)
-						MoveCOLsWithinMatrix(Xt_mars, Npad, NewCol.k2_old+1, KOLD, NewCol.k2_new+1);
+						shift_lastcols_within_matrix(Xt_mars, Npad, NewCol.k2_old+1, KOLD, NewCol.k2_new+1);
 					if (Knewterm != 0)
 						SCPY(Knewterm*Npad, Xnewterm, Xt_mars + (NewCol.k1-1) * Npad);
 					
 					/****************************************************/
 					//Find the good positions of the proposed MOVE
 					//Then update the knotLists and order
 					/****************************************************/
@@ -952,15 +953,15 @@
 						//Counting probability of being breakpoints				
 						for (I32 i = 0; i < nKnot; i++) result->xProb[ KNOT[i]-1 ] += 1L;
 
 						//Summng up the harmonic orders or trend orders for individual seeasonal segments
 						if (result->xorder != NULL) {
 							TORDER_PTR  ORDER = basis->ORDER;
 							for (I32 i = 0; i <= nKnot; ++i) {
-								I16 r1 = KNOT[i-1], r2 = KNOT[i]-1;
+								I32 r1 = KNOT[i-1], r2 = KNOT[i]-1;
 								r_ippsAddC_32s_ISfs(ORDER[i], result->xorder+r1 - 1, r2 - r1 + 1, 0);
 							}
 						}
 
 						//Compute the averaged  signals
 						if (q == 1) {
 							//r_cblas_sgemv(CblasColMajor, CblasNoTrans, Npad, K_SN, 1.f, Xt_mars, Npad, MODEL.curr.beta_mean, 1L, 0.f, MEMBUF1, 1L);
@@ -1161,15 +1162,15 @@
 			/*****************************************************************************/
 
 			if (!skipCurrentPixel)
 			{
 				int   sum;
 				#define GetSum(arr) (r_ippsSum_32s_Sfs(arr, N, &sum, 0), sum) // parenthesis operator
 
-				I32   sMAXNUMKNOT = MODEL.sid >=0? MODEL.b[MODEL.sid].prior.maxKnotNum:-9999999;
+				I32   sMAXNUMKNOT = MODEL.sid >=0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum:-9999999; // the seasonal cmpt is always the first one
 				I32   tMAXNUMKNOT = MODEL.tid>=0?  MODEL.b[MODEL.tid].prior.maxKnotNum:-9999999;
 				I32   oMAXNUMKNOT = MODEL.oid>=0?  MODEL.b[MODEL.oid].prior.maxKnotNum:- 9999999;
 				F32   inv_sample  = 1.f / sample;			
 				
 
 				*resultChain.marg_lik = *resultChain.marg_lik * inv_sample;
 				// FOR MRBEAST
@@ -1327,15 +1328,15 @@
 
 
 			/**************************************************/
 			//   Add up the individual chain to the Result
 			/**************************************************/
 			if (!skipCurrentPixel) 
 			{
-				I32   sMAXNUMKNOT = MODEL.sid >=0? MODEL.b[MODEL.sid].prior.maxKnotNum:-9999999;
+				I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 				I32   tMAXNUMKNOT = MODEL.tid>=0?  MODEL.b[MODEL.tid].prior.maxKnotNum:-9999999;
 				I32   oMAXNUMKNOT = MODEL.oid>=0?  MODEL.b[MODEL.oid].prior.maxKnotNum:- 9999999;
 
 				//https://stackoverflow.com/questions/13216423/error-pasting-and-red-does-not-give-a-valid-preprocessing-token
 				//#define _1(x)      *(result.##x) += *(resultChain.##x) // Working with MSVC but not GCC
 
 				#define _1(x)      *(result.x) += *(resultChain.x)
@@ -1348,15 +1349,15 @@
 				#define _skn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, sMAXNUMKNOT + 1)
 				#define _tkn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, tMAXNUMKNOT + 1)
 				#define _okn_1(x)  r_ippsAdd_32f_I((F32PTR)resultChain.x, (F32PTR)result.x, oMAXNUMKNOT + 1)
 
 				_1(marg_lik);
 				_q2(sig2);  //Fpr MRBEAST
 				
-				if (MODEL.sid >= 0) {					
+				if (MODEL.sid >= 0 || MODEL.vid >0) {
 					_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD);
 					if (extra.computeSeasonOrder)    _N(sorder);
 					if (extra.computeSeasonAmp)      _N(samp), _N(sampSD);
 					if (extra.computeCredible)       _2Nq(sCI);
 				}
 
 				if (MODEL.tid >= 0) {					
@@ -1406,15 +1407,15 @@
 				#undef _tkn_1
 			    #undef _okn_1
 			}
 
 			/***********MULTITHREAD*******************/
 			// Jump out of the chainumber loop
 			if (skipCurrentPixel) {
-				//r_warning("WARNING(#%d):The max number of bad iterations exceeded. "
+				//q_warning("WARNING(#%d):The max number of bad iterations exceeded. "
 				//	     "Can't decompose the current time series\n", skipCurrentPixel);
 				break;
 			}
 			/***********MULTITHREAD*******************/
 		}
 		/*********************************/
 		// WHILE(chainNumber<chainNumber)
@@ -1430,15 +1431,15 @@
 	/******************************************************/
 
 		// Average the results from multiple chains
 		if (MCMC_CHAINNUM >= 2 && !skipCurrentPixel)
 		{
 			I32  N = opt->io.N;			
 	
-			I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
+			I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 			I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
 			I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
 
 			const F32 invChainNumber = 1.f /(F32)MCMC_CHAINNUM;
 
 			#define _1(x)      *((F32PTR)result.x)*=invChainNumber
 			#define _N(x)      r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, N)
@@ -1450,15 +1451,15 @@
 			#define _skn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, sMAXNUMKNOT + 1)
 			#define _tkn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, tMAXNUMKNOT + 1)
 			#define _okn_1(x)  r_ippsMulC_32f_I(invChainNumber, (F32PTR)result.x, oMAXNUMKNOT + 1)
 
 			F32 maxncpProb;	 
 			_1(marg_lik);			
 			_q2(sig2);
-			if (MODEL.sid >= 0) {
+			if (MODEL.sid >= 0 || MODEL.vid>0) {
 				_1(sncp); _skn_1(sncpPr);	     _N(scpOccPr); _Nq(sY); _Nq(sSD); 
 				if (extra.computeSeasonOrder)    _N(sorder);
 				if (extra.computeSeasonAmp)     {_N(samp), _N(sampSD);}
 				if (extra.computeCredible)       _2Nq(sCI);
  
 				*result.sncp_mode   = f32_maxidx(result.sncpPr,       sMAXNUMKNOT + 1, &maxncpProb);
 				*result.sncp_median = GetPercentileNcp(result.sncpPr, sMAXNUMKNOT + 1, 0.5);
@@ -1523,47 +1524,47 @@
 			#undef _2N
 			#undef _skn_1
 			#undef _tkn_1
 			#undef _okn_1
 		}
 		if (!skipCurrentPixel) {		
 			I32  N = opt->io.N;  
-			if (MODEL.sid >= 0) 							tsRemoveNaNs(result.sSD, N);
+			if (MODEL.sid >= 0||MODEL.vid>0) 				tsRemoveNaNs(result.sSD, N);
 			if (MODEL.tid >= 0)								tsRemoveNaNs(result.tSD, N);
 			if (MODEL.tid >= 0 && extra.computeTrendSlope)  tsRemoveNaNs(result.tslpSD, N);		 
 			if (MODEL.oid >= 0) 							tsRemoveNaNs(result.oSD, N);
 		}
 
 		// Compute Changepoints and their confidence intervals
 		if (!skipCurrentPixel)
 		{
 			I32     N         = opt->io.N;
 			F32     nan       = getNaN();     //A sloppy way to get a NAN
 
-			F32  	threshold = 0.001f;
+			F32  	threshold = 0.01f;
 			F32PTR	mem       = Xnewterm;  //Xnewterm must have a length larger than or equla to 5*N + max(sncp, tncp);
 			I32PTR  cptList   = (I32PTR)mem + 5LL * N;
 			F32PTR  cptCIList = (F32PTR)mem + 6LL * N;
 
 			I32   cptNumber;
 			I32   trueCptNumber;
 			F32   maxncpProb;
 			const F32 T0 = (F32)opt->io.meta.startTime;
 			const F32 dT = (F32)opt->io.meta.deltaTime;
 
-			I32   sMAXNUMKNOT = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.maxKnotNum : -9999999;
+			I32   sMAXNUMKNOT = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.maxKnotNum : -9999999;
 			I32   tMAXNUMKNOT = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.maxKnotNum : -9999999;
 			I32   oMAXNUMKNOT = MODEL.oid >= 0 ? MODEL.b[MODEL.oid].prior.maxKnotNum : -9999999;
 
-			I32   sMINSEPDIST = MODEL.sid >= 0 ? MODEL.b[MODEL.sid].prior.minSepDist : -9999999;
+			I32   sMINSEPDIST = MODEL.sid >= 0 || MODEL.vid >= 0 ? MODEL.b[0].prior.minSepDist : -9999999;
 			I32   tMINSEPDIST = MODEL.tid >= 0 ? MODEL.b[MODEL.tid].prior.minSepDist : -9999999;
-			I32   oMINSEPDIST = MODEL.oid >= 0 ? 1 : -9999999;
+			I32   oMINSEPDIST = MODEL.oid >= 0 ? 0 : -9999999;  //changed from 1 to 0 to pick up consecutive outlier spikes.
 
 			//--------------Season----------------------------
-			if (extra.computeSeasonChngpt && MODEL.sid >=0)  	{
+			if (extra.computeSeasonChngpt && (MODEL.sid >=0 || MODEL.vid>0 ))  	{
 				cptNumber      = sMAXNUMKNOT;
 				trueCptNumber = FindChangepoint((F32PTR)result.scpOccPr, mem, threshold, cptList, cptCIList, N, sMINSEPDIST, cptNumber);
 				//In the returned result, cptList is a list of detected changepoints, which are all zero-based indices.
 				//That is, a changepoint occurring at t1 has a value of 0.
 
 				for (int i = 0; i < trueCptNumber; i++) {
 					*(result.scp + i)	  = (F32)(*(cptList + i)) * dT + T0;
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_allocinitmem.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_allocinitmem.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_computexy_q.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_computexy_q.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_cvtKnotsToBinVec.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_cvtKnotsToBinVec.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_genrandbasis.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_genrandbasis.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_gensegment.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_gensegment.c`

 * *Files 1% similar despite different names*

```diff
@@ -194,30 +194,31 @@
 	F32PTR TERM       = SVD.TERMS     + N * (seg->ORDER1 - 1)  + seg->R1 - 1;
 	F32PTR svd_csum   = SVD.SQR_CSUM  + 1L + (N + 1) * (seg->ORDER1 - 1);
 	// !L is needed bcz each col is  padded with an exta zero at the beginning so 
 	// that season_csum[r2]-season_csum[r1-1] will be working
 
 	I32    k = 0;
 	for (I32 j = seg->ORDER1; j <= seg->ORDER2; j++){
-
-		F32   scalingFactor;
 		// there is only one term per order
 		r_cblas_scopy(Nseg, TERM, 1L, X + seg->R1 - 1, 1L);
-		scalingFactor = sqrtf(N / (svd_csum[seg->R2 - 1] - svd_csum[(seg->R1 - 1) - 1]));
-		r_cblas_sscal(Nseg, scalingFactor, X + seg->R1 - 1, 1L);
+		F32 csum_diff     = (svd_csum[seg->R2 - 1] - svd_csum[(seg->R1 - 1) - 1]);
+		F32 scalingFactor = csum_diff==0?0.0: sqrtf(N / csum_diff);  // Some hihger SVD terms may be zeros
+		//r_cblas_sscal(Nseg, scalingFactor, X + seg->R1 - 1, 1L);
 		
-		k       += 1;
+		k    += 1;
 		TERM += N ;
 		X    += Npad;
 		svd_csum += (N + 1L) ;	
 	}
 
+	
 	return k;
 #undef SEASON
 }
+
 static int SS_0( F32PTR X, I32 N, BEAST2_BASESEG_PTR seg, BASIS_CONST* ptr) {
 
 	#define SEASON  (*((SEASON_CONST*)ptr))
 
 	//...Calcuate new terms........	
 	I32     Npad = ((N + 7L) / 8L) * 8L;  Npad = N;//Correct for the inconsitency of X and Y in gemm and gemv
 	I32     Nseg = seg->R2 - seg->R1 + 1L;
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_pickcmptId.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_pickcmptId.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_proposeNew_q.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_proposeNew_q.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_updateKsKe_prec0123.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_updateKsKe_prec0123.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_basis_updategoodvec.c` & `Rbeast-0.1.14/ext_src/beastv2_basis_updategoodvec.c`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 	I32       MINSEP   = basis->prior.minSepDist;
 	TKNOT_PTR knotList = basis->KNOT;
 
 	MOVETYPE flag = new->jumpType;
 	if (flag == BIRTH) 
 		r_ippsSet_8u(0, goodVec + (newKnot - MINSEP) - 1, 2 * MINSEP + 1);	
 	else if (flag == DEATH) {//death						
-		I16 oldKnot = knotList[newIdx - 1]; //If flag=death, oldKnot was not assgined before until now
-		I16 r1      = knotList[(newIdx - 1) - 1];
-		I16 r2      = knotList[(newIdx + 1) - 1] - 1;
+		I32 oldKnot = knotList[newIdx - 1]; //If flag=death, oldKnot was not assgined before until now
+		I32 r1      = knotList[(newIdx - 1) - 1];
+		I32 r2      = knotList[(newIdx + 1) - 1] - 1;
 
 		r_ippsSet_8u(1, goodVec + (oldKnot - MINSEP) - 1,   2 * MINSEP + 1);
 		r_ippsSet_8u(0, goodVec + (r1)-1,                   MINSEP + 1);
 		r_ippsSet_8u(0, goodVec + (r2 - MINSEP + 1) - 1,    MINSEP);
 		//GOOD.tY.num = countOnes(N, GOOD.tY.binvec);//ippsSum_16s32s_Sfs(GOOD.tY.binvec, N, &GOOD.tY.num, 0);
 	}
 	else if (flag == MOVE) {//move
-		I16 oldKnot = knotList[newIdx - 1];
-		I16 r1      = knotList[(newIdx - 1) - 1];
-		I16 r2      = knotList[(newIdx + 1) - 1] - 1;
+		I32 oldKnot = knotList[newIdx - 1];
+		I32 r1      = knotList[(newIdx - 1) - 1];
+		I32 r2      = knotList[(newIdx + 1) - 1] - 1;
 
 		//If flag=move, oldKnot has been already assgined before.
 		r_ippsSet_8u(1, goodVec + (oldKnot - MINSEP) - 1, 2 * MINSEP + 1);
 		r_ippsSet_8u(0, goodVec + (newKnot - MINSEP) - 1, 2 * MINSEP + 1);
 		r_ippsSet_8u(0, goodVec + (r1)-1,                 MINSEP + 1);
 		r_ippsSet_8u(0, goodVec + (r2 - MINSEP + 1) - 1,  MINSEP);
 	}
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_func.h` & `Rbeast-0.1.14/ext_src/beastv2_func.h`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         for (rI32 i = startBasisIdx0 +1; i < MAX_NUM_BASIS; i++) {
             b[i].Kbase  = b[i-1].Kbase + b[i-1].K;
         }   
     }
 	*/
 }
 
- void MoveCOLsWithinMatrix(F32PTR X, I32 N, I32 Kstart, I32 Kend, I32 Knewstart);
+
  
  static void MatxVec_FULL(BEAST2_BASESEG* SEG, I32 numSeg, F32PTR X, F32PTR Y, F32PTR XtY, I32 N)
 {
 	// New components
 	 I32 Kterms = 0;
 	 for (int i = 0; i < numSeg; i++) {			 Kterms += SEG[i].K; 	 }
 	 I32 Npad = (N + 7) / 8 * 8; Npad = N;//Correct for the inconsitency of X and Y in gemm and gemv
@@ -125,11 +125,10 @@
 					X , Npad,
 					X , Npad, 0.,
 					XtX, Knew);
 
 }
 
 
-
 void MR_EvaluateModel(
 	BEAST2_MODELDATA* curmodel, BEAST2_BASIS_PTR b, F32PTR Xt_mars, I32 N, I32 NUMBASIS,
 	BEAST2_YINFO_PTR pyInfo, BEAST2_HyperPar* hyperPar, F32PTR precVec, VOID_PTR stream);
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_func_q.c` & `Rbeast-0.1.14/ext_src/beastv2_func_q.c`

 * *Files 2% similar despite different names*

```diff
@@ -407,50 +407,18 @@
 		}
 
 		Ksegcolcsum += Ksegcol;
 		XtX += Ksegcol*Knew;
 	}
 	
 }
-void MoveCOLsWithinMatrix(F32PTR X, I32 N, I32 Kstart, I32 Kend, I32 Knewstart) {
-
-	rI32 j = Knewstart - Kstart;
-	if (j < 0 || Knewstart > Kend)
-		// dst(k2_new):-----123455----
-		// src(k2_old):----------123455----
-
-		// dst(k2_new):----------------123455----
-		// src(k2_old):-----123455----
-		r_cblas_scopy((Kend-Kstart+1)*N, X+(Kstart-1)*N, 1, X+(Knewstart-1)*N, 1);
-	else
-	{
-		// dst(k2_new):-------------123456----
-		// src(k2_old):---------123456----
-
-		rI32 segStartIdx = Kend+1;
-		while (true) {
-			segStartIdx = segStartIdx - j;
-			if (segStartIdx > Kstart) {
-				r_cblas_scopy(j * N, X + (segStartIdx-1) * N, 1L, X + ((segStartIdx+j)- 1) * N, 1);
-			}
-			else {
-				j = (segStartIdx+j) - Kstart;
-				r_cblas_scopy(j *N, X + (Kstart - 1)*N, 1L, X+(Knewstart-1) * N, 1);
-				break;
-			}
-		}//while (true)
-
-	}//if (j < 0 || k2_new + 1 > Kold)
-}
  
 //https: //stackoverflow.com/questions/3174850/what-is-the-correct-type-for-array-indexes-in-c#
 //https: //stackoverflow.com/questions/797318/how-to-split-a-string-literal-across-multiple-lines-in-c-objective-c
- 
-
-/////////////////////////////////////////////////////////////////////////////////////////////////
+  
 /////////////////////////////////////////////////////////////////////////////////////////////////
 /////////////////////////////////////////////////////////////////////////////////////////////////
 /////////////////////////////////////////////////////////////////////////////////////////////////
 
 void MR_EvaluateModel(
 	BEAST2_MODELDATA *curmodel,  BEAST2_BASIS_PTR b, F32PTR Xt_mars, I32 N, I32 NUMBASIS,
 	BEAST2_YINFO_PTR yInfo,	 BEAST2_HyperPar *hyperPar, F32PTR precVec, VOID_PTR stream )
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_header.h` & `Rbeast-0.1.14/ext_src/beastv2_header.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #pragma once
 
 #include "abc_000_macro.h"
 #include "abc_datatype.h"   //#include <inttypes.h>  #include <stdint.h>
 #include "abc_ide_util.h"
+#include "abc_ts_func.h"
 #include "abc_mat.h"   //NEWXCOLINFO
 
 #ifndef SOLARIS_COMPILER
 
 #if R_INTERFACE==1 
 	#ifdef beta
 		#undef beta  //beta is refined to Rf_beta in Rmath.h, which causes errors in expanding model->beta
@@ -39,31 +40,29 @@
 #define rTORDER      register  TORDER
 
 /*************************************************/
 // Declarations of data types for input options
 /*************************************************/
 
 typedef struct BEAST2_METADATA {
-	VOID_PTR rawInput;
-	VOID_PTR rawTimeVec;	
-	I08      detrend;
-	I08      deseasonalize;
 	I08		 nrhs;
-	I08		 isMetaStruct;
-	I08		 isRegularOrdered;	
-	I08      seasonForm;
+	I08      detrend;
+	I08      deseasonalize;	
+ 	I08      seasonForm;
+	I08      IsPeriodEstimated;
 	I08      hasSeasonCmpnt;	
 	I08      hasOutlierCmpnt;	
 	
-	I08    whichDimIsTime;
-	F32    period;
-	F32    missingValue;
-	F32    startTime, deltaTime;	
-	F32    maxMissingRate;
-	F32PTR svdTerms;
+	I08     whichDimIsTime;
+	F32     period;
+	F32     missingValue;
+	F32     startTime, deltaTime;	
+	F32     maxMissingRate;
+	VOIDPTR svdTerms_Object;
+	VOIDPTR svdYseason_Object;
 } BEAST2_METADATA, * _restrict BEAST2_METADATA_PTR;
 
 
 // 0: Use a constant precison value
 // 1: Use a uniform precision value for all terms
 typedef enum { ConstPrec, UniformPrec, ComponentWise, OrderWise} PRECPRIOR_TYPE;
  
@@ -77,19 +76,20 @@
 
 	U08	  seasonBasisFuncType;
 	U08	  trendBasisFuncType;
 	U08	  outlierBasisFuncType;
 	U08	  modelPriorType;
 	U08   precPriorType;
 
-	U08   seasonMinOrder,   seasonMaxOrder;
-    U08   trendMinOrder,    trendMaxOrder;
-	I16   trendMinSepDist,  seasonMinSepDist;
-	U16   trendMinKnotNum,  seasonMinKnotNum;
-	U16   trendMaxKnotNum,  seasonMaxKnotNum;
+	I16   seasonMinOrder,   seasonMaxOrder;
+	I16   trendMinOrder,    trendMaxOrder;
+	I32   trendMinSepDist,  seasonMinSepDist;
+
+	I16   trendMinKnotNum,  seasonMinKnotNum;
+	I16   trendMaxKnotNum,  seasonMaxKnotNum;
 	I16   outlierMaxKnotNum;
 
 	U16   K_MAX;
  
 	F32   sigFactor;
 	F32   outlierSigFactor;
 
@@ -117,48 +117,44 @@
 	U16   numParThreads;
 	U16   numCPUCoresToUse;
 	U16   consoleWidth;
 	I08   whichOutputDimIsTime;
 	I08   removeSingletonDims;
 
 	I08   ncpStatMethod;
-	bool  computeCredible;
-	bool  fastCIComputation;
-	bool  computeSeasonOrder;
-	bool  computeTrendOrder;
-
-	bool  computeSeasonChngpt, computeTrendChngpt, computeOutlierChngpt;
-	bool  computeSeasonAmp;
-	bool  computeTrendSlope;	
+	Bool  computeCredible;
+	Bool  fastCIComputation;
+	Bool  computeSeasonOrder;
+	Bool  computeTrendOrder;
+
+	Bool  computeSeasonChngpt, computeTrendChngpt, computeOutlierChngpt;
+	Bool  computeSeasonAmp;
+	Bool  computeTrendSlope;	
 	
-	bool tallyPosNegSeasonJump;
-	bool tallyPosNegTrendJump;
-	bool tallyIncDecTrendJump;
-	bool tallyPosNegOutliers;
+	Bool tallyPosNegSeasonJump;
+	Bool tallyPosNegTrendJump;
+	Bool tallyIncDecTrendJump;
+	Bool tallyPosNegOutliers;
 
-	bool  printOptions;
-	bool  printProgressBar;
+	Bool  printOptions;
+	Bool  printProgressBar;
 
 } BEAST2_EXTRA, * _restrict BEAST2_EXTRA_PTR;
-
-typedef struct BEAST2_TIME {
-	I32PTR     sortedTimeIdx;
-	I32PTR     numPtsPerInterval;
-	I32        startIdxOfFirsInterval;
-} BEAST2_TIME;
-
+ 
 struct BEAST2_RESULT;
 typedef struct BEAST2_RESULT BEAST2_RESULT, * _restrict BEAST2_RESULT_PTR;
 typedef struct BEAST2_IO {
 	BEAST2_METADATA	meta;
-	BEAST2_TIME		T;
+	TimeVecInfo	T;
 
 	VOID_PTR		*pdata;
 	DATA_TYPE		*dtype;
 	I08				ndim;
+	I08             rowdim, coldim, timedim;
+	I32				imgdims[2];
 	I32				dims[3];
 	I32				numOfPixels;
 	// q is the number of time series;q=1 is for univaraite TS in BEASTv4.
 	// q is added to ensure a consistent API inteface btw BEAST and MRBEAST
 	// For irregular time seires, Nraw is obtained from ndims[whichDimIsTime=1]
 	I32				N ,q; 
 
@@ -322,15 +318,15 @@
 } NEWTERM, * _restrict NEWTERM_PTR;
 
  
 
 //period is used as "basis->bConst.dummy.period" in the following functons: computeXY,Alloc_Init_PrecPrior,DD_CalcBasisKsKeK_prec0123
 //TERMS needed only if meta->io.deseasonlaized=TRUE
 typedef struct DUMMY_CONS { F32PTR TERMS; F32PTR SQRT_N_div_n; I32 period; }          DUMMY_CONST;
-typedef struct SVD_CONS {  F32PTR TERMS; F32PTR SQR_CSUM;}                            SVD_CONST;
+typedef struct SVD_CONS     { F32PTR TERMS; F32PTR SQR_CSUM;}                            SVD_CONST;
 typedef struct SEASON_CONST { F32PTR TERMS, SQR_CSUM, SCALE_FACTOR;}				    SEASON_CONST;
 typedef struct TREND_CONS   { F32PTR TERMS, COEFF_A, COEFF_B, INV_SQR;}	               TREND_CONST;
 typedef struct OUTLIER_CONS { F32    SQRTN, SQRTN_1; }		                           OUTLIER_CONST;
  
 typedef union  {
 	SVD_CONST     svd;
 	DUMMY_CONST   dummy;
@@ -452,8 +448,8 @@
  
 
 #elif defined(SOLARIS_COMPILER)
 #include "beastv2_header_solaris.h"
 #endif
 
 
-#define AggregatedMemAlloc 1L
+#define AggregatedMemAlloc 0L
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_header_solaris.h` & `Rbeast-0.1.14/ext_src/beastv2_header_solaris.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #pragma once
 
 #include "abc_000_macro.h"
 #include "abc_datatype.h"   //#include <inttypes.h>  #include <stdint.h>
 #include "abc_ide_util.h"
+#include "abc_ts_func.h"
 #include "abc_mat.h"   //NEWXCOLINFO
 
 
 #if R_INTERFACE==1 
-	#ifdef beta
-		#undef beta  //beta is refined to Rf_beta in Rmath.h, which causes errors in expanding model->beta
-	#endif
+#ifdef beta
+#undef beta  //beta is refined to Rf_beta in Rmath.h, which causes errors in expanding model->beta
+#endif
 #endif
 
 #define _IN_ 
 #define _OUT_
 
 #define MAX_RAND_NUM	  5000L
 #define MAX_NUM_BASIS     3
@@ -26,73 +27,71 @@
 #define SEASONID   0
 #define TRENDID    1
 #define OUTLIERID  2 //oooooooooooooooooooo
 #define DUMMYID    3
 #define SVDID      4
 #define A(xxx)     BEAST2_##xxx
 
-typedef U32 TKNOT,  *_restrict TKNOT_PTR;
-typedef U08 TORDER, *_restrict TORDER_PTR;
+typedef U32 TKNOT, * _restrict TKNOT_PTR;
+typedef U08 TORDER, * _restrict TORDER_PTR;
 #define rTKNOT_PTR   register  TKNOT_PTR
 #define rTORDER_PTR  register  TORDER_PTR
 #define rTKNOT       register  TKNOT
 #define rTORDER      register  TORDER
 
 /*************************************************/
 // Declarations of data types for input options
 /*************************************************/
 
 typedef struct BEAST2_METADATA {
-	VOID_PTR rawInput;
-	VOID_PTR rawTimeVec;	
 	I08      detrend;
 	I08      deseasonalize;
 	I08		 nrhs;
-	I08		 isMetaStruct;
-	I08		 isRegularOrdered;	
 	I08      seasonForm;
-	I08      hasSeasonCmpnt;	
-	I08      hasOutlierCmpnt;	
-	
-	I08    whichDimIsTime;
-	F32    period;
-	F32    missingValue;
-	F32    startTime, deltaTime;	
-	F32    maxMissingRate;
-	F32PTR svdTerms;
+	I08      hasSeasonCmpnt;
+	I08      hasOutlierCmpnt;
+
+	I08     whichDimIsTime;
+	F32     period;
+	F32     missingValue;
+	F32     startTime, deltaTime;
+	F32     maxMissingRate;
+	VOIDPTR svdTerms_Object;
+	VOIDPTR svdYseason_Object;
 } BEAST2_METADATA, * _restrict BEAST2_METADATA_PTR;
 
 
 // 0: Use a constant precison value
 // 1: Use a uniform precision value for all terms
-typedef enum { ConstPrec, UniformPrec, ComponentWise, OrderWise} PRECPRIOR_TYPE;
- 
+typedef enum { ConstPrec, UniformPrec, ComponentWise, OrderWise } PRECPRIOR_TYPE;
+
 typedef struct BEAST2_HyperPar {
 	F32 alpha_1, alpha_2, del_1, del_2;
 } BEAST2_HyperPar, * _restrict BEAST2_HyperPar_PTR;
 
 typedef struct BEAST2_PRIOR {
 	I08	  basisType[MAX_NUM_BASIS];			//'ST','STO','TO','T', ...
 	I08	  numBasis;
 
 	U08	  seasonBasisFuncType;
 	U08	  trendBasisFuncType;
 	U08	  outlierBasisFuncType;
 	U08	  modelPriorType;
 	U08   precPriorType;
 
-	U08   seasonMinOrder,   seasonMaxOrder;
-    U08   trendMinOrder,    trendMaxOrder;
-	I16   trendMinSepDist,  seasonMinSepDist;
-	U16   trendMinKnotNum,  seasonMinKnotNum;
-	U16   trendMaxKnotNum,  seasonMaxKnotNum;
+	I16   seasonMinOrder, seasonMaxOrder;
+	I16   trendMinOrder, trendMaxOrder;
+	I32   trendMinSepDist, seasonMinSepDist;
+
+	I16   trendMinKnotNum, seasonMinKnotNum;
+	I16   trendMaxKnotNum, seasonMaxKnotNum;
 	I16   outlierMaxKnotNum;
 
 	U16   K_MAX;
- 
+
 	F32   sigFactor;
 	F32   outlierSigFactor;
 
 	F32   sig2;
 	F32	  precValue;
 	F32   alpha1, alpha2, delta1, delta2;
 } BEAST2_PRIOR, * _restrict BEAST2_PRIOR_PTR;
@@ -103,67 +102,64 @@
 	F32   ridgeFactor;
 	F32   trendResamplingOrderProb;
 	F32   seasonResamplingOrderProb;
 	U16   maxMoveStepSize;
 	U32   burnin, samples, chainNumber;
 	U16   thinningFactor;
 } BEAST2_MCMC, * _restrict BEAST2_MCMC_PTR;
- 
+
 typedef struct BEAST2_EXTRA {
 	I08   smoothCpOccPrCurve;
 	I08   useMeanOrRndBeta;
 	I08   dumpInputData;
 	U08   numThreadsPerCPU;
 	U16   numParThreads;
 	U16   numCPUCoresToUse;
 	U16   consoleWidth;
 	I08   whichOutputDimIsTime;
 	I08   removeSingletonDims;
 
 	I08   ncpStatMethod;
-	bool  computeCredible;
-	bool  fastCIComputation;
-	bool  computeSeasonOrder;
-	bool  computeTrendOrder;
-
-	bool  computeSeasonChngpt, computeTrendChngpt, computeOutlierChngpt;
-	bool  computeSeasonAmp;
-	bool  computeTrendSlope;	
-	
-	bool tallyPosNegSeasonJump;
-	bool tallyPosNegTrendJump;
-	bool tallyIncDecTrendJump;
-	bool tallyPosNegOutliers;
+	Bool  computeCredible;
+	Bool  fastCIComputation;
+	Bool  computeSeasonOrder;
+	Bool  computeTrendOrder;
+
+	Bool  computeSeasonChngpt, computeTrendChngpt, computeOutlierChngpt;
+	Bool  computeSeasonAmp;
+	Bool  computeTrendSlope;
+
+	Bool tallyPosNegSeasonJump;
+	Bool tallyPosNegTrendJump;
+	Bool tallyIncDecTrendJump;
+	Bool tallyPosNegOutliers;
 
-	bool  printOptions;
-	bool  printProgressBar;
+	Bool  printOptions;
+	Bool  printProgressBar;
 
 } BEAST2_EXTRA, * _restrict BEAST2_EXTRA_PTR;
 
-typedef struct BEAST2_TIME {
-	I32PTR     sortedTimeIdx;
-	I32PTR     numPtsPerInterval;
-	I32        startIdxOfFirsInterval;
-} BEAST2_TIME;
 
 struct BEAST2_RESULT;
 typedef struct BEAST2_RESULT BEAST2_RESULT, * _restrict BEAST2_RESULT_PTR;
 typedef struct BEAST2_IO {
 	BEAST2_METADATA	meta;
-	BEAST2_TIME		T;
+	TimeVecInfo  	T;
 
-	VOID_PTR		*pdata;
-	DATA_TYPE		*dtype;
+	VOID_PTR* pdata;
+	DATA_TYPE* dtype;
 	I08				ndim;
+	I08             rowdim, coldim, timedim;
+	I32				imgdims[2];
 	I32				dims[3];
 	I32				numOfPixels;
 	// q is the number of time series;q=1 is for univaraite TS in BEASTv4.
 	// q is added to ensure a consistent API inteface btw BEAST and MRBEAST
 	// For irregular time seires, Nraw is obtained from ndims[whichDimIsTime=1]
-	I32				N ,q; 
+	I32				N, q;
 
 	struct {
 		BEAST2_RESULT* result;
 		DATA_TYPE      dtype;
 		U08            whichDimIsTime;
 	} out;
 
@@ -178,38 +174,38 @@
 
 typedef struct BEAST2_YINFO {
 	// maen, sd, and YtT are all scalars but pointers are used to maintan 
 	// a consitent API with MRBEAST
 	F32PTR    Yseason;
 	F32PTR    Ytrend;
 
-	F32PTR     mean, sd;	
+	F32PTR     mean, sd;
 	F32PTR     YtY_plus_alpha2Q;
 	F32        alpha1_star;
-	TKNOT      n, nMissing;		
+	TKNOT      n, nMissing;
 	//q is added for MRBEAST and used in ComputeLik, PropseNew/__CalcAbsDeviation(compute deviaiton and extrempos)
-    //, MR_EvaluateModel,
-	I32        q; 
+	//, MR_EvaluateModel,
+	I32        q;
 	I32PTR     rowsMissing;
 	F32PTR     Y;
-	
+
 } BEAST2_YINFO, * _restrict BEAST2_YINFO_PTR;
 
 typedef struct BEAST2_RESULT {
 	F32PTR  time;
 	F32PTR  data;
 	F32PTR  marg_lik, sig2, R2, RMSE;
 	F32PTR  sncp, sncp_median, sncp_mode, sncp_pct90, sncp_pct10;
 	I32PTR  sncpPr, scpOccPr;
 	F32PTR  sY, sSD;
 	F32PTR  sCI;            //computeCI
 	I32PTR  sorder;         //computeOrder
 	F32PTR  samp, sampSD;   //computeAmp
 	F32PTR  scp, scpCI, scpPr, scpAbruptChange; //computeChangpt
- 
+
 	F32PTR  tncp, tncp_median, tncp_mode, tncp_pct90, tncp_pct10;
 	I32PTR  tncpPr, tcpOccPr;
 	F32PTR  tY, tSD;
 	F32PTR  tCI;            //computeCI
 	I32PTR  torder;         //computeOrder
 	F32PTR  tslp, tslpSD;   //computeSlp
 	I32PTR  tslpSgnPosPr;   //computeSlp
@@ -219,148 +215,148 @@
 
 	F32PTR  oncp, oncp_median, oncp_mode, oncp_pct90, oncp_pct10;
 	I32PTR  oncpPr, ocpOccPr;
 	F32PTR  oY, oSD;
 	F32PTR  oCI;                 //computeCI
 	F32PTR  ocp, ocpCI, ocpPr;  //computeChangpt	
 
-    //tallyPosNegSeasonJump
-	F32PTR  spos_ncp,     sneg_ncp;
-	I32PTR  spos_ncpPr,    sneg_ncpPr;
-	I32PTR  spos_cpOccPr,  sneg_cpOccPr;
-	F32PTR  spos_cp,    sneg_cp;
+	//tallyPosNegSeasonJump
+	F32PTR  spos_ncp, sneg_ncp;
+	I32PTR  spos_ncpPr, sneg_ncpPr;
+	I32PTR  spos_cpOccPr, sneg_cpOccPr;
+	F32PTR  spos_cp, sneg_cp;
 	F32PTR  spos_cpPr, sneg_cpPr;
 	F32PTR  spos_cpAbruptChange, sneg_cpAbruptChange;
 	F32PTR  spos_cpCI, sneg_cpCI;
 
 	//tallyPosNegTrendJump
-	F32PTR  tpos_ncp,      tneg_ncp;
-	I32PTR  tpos_ncpPr,  tneg_ncpPr;
-	I32PTR  tpos_cpOccPr,   tneg_cpOccPr;
-	F32PTR  tpos_cp,     tneg_cp;
+	F32PTR  tpos_ncp, tneg_ncp;
+	I32PTR  tpos_ncpPr, tneg_ncpPr;
+	I32PTR  tpos_cpOccPr, tneg_cpOccPr;
+	F32PTR  tpos_cp, tneg_cp;
 	F32PTR  tpos_cpPr, tneg_cpPr;
 	F32PTR  tpos_cpAbruptChange, tneg_cpAbruptChange;
-	F32PTR  tpos_cpCI,  tneg_cpCI;
+	F32PTR  tpos_cpCI, tneg_cpCI;
 
 	//tallyIncDecTrendJump
-	F32PTR  tinc_ncp,     tdec_ncp;
+	F32PTR  tinc_ncp, tdec_ncp;
 	I32PTR  tinc_ncpPr, tdec_ncpPr;
-	I32PTR  tinc_cpOccPr,  tdec_cpOccPr;
-	F32PTR  tinc_cp,     tdec_cp;
+	I32PTR  tinc_cpOccPr, tdec_cpOccPr;
+	F32PTR  tinc_cp, tdec_cp;
 	F32PTR  tinc_cpPr, tdec_cpPr;
 	F32PTR  tinc_cpAbruptChange, tdec_cpAbruptChange;
 	F32PTR  tinc_cpCI, tdec_cpCI;
 
 	//tallyPosNegOutliers
 	F32PTR  opos_ncp, oneg_ncp;
 	I32PTR  opos_ncpPr, oneg_ncpPr;
 	I32PTR  opos_cpOccPr, oneg_cpOccPr;
 	F32PTR  opos_cp, oneg_cp;
-	F32PTR  opos_cpPr, oneg_cpPr;	
+	F32PTR  opos_cpPr, oneg_cpPr;
 	F32PTR  opos_cpCI, oneg_cpCI;
 
 
 } BEAST2_RESULT, * _restrict BEAST2_RESULT_PTR;
 
 typedef struct CORESULT {
 	I32PTR xNProb, xProb, xorder;
 	F32PTR x, xSD;
 } CORESULT, * _restrict CORESULT_PTR;
 
 typedef struct BEAST2_RNDSTREAM {
 	F32PTR  rndgamma;
 	U32PTR  rnd32;
 	U16PTR  rnd16;
-	U08PTR  rnd08;	
+	U08PTR  rnd08;
 } BEAST2_RNDSTREAM, * _restrict BEAST2_RANDSEEDPTR;
 
 
 struct BEAST2_BASIS;
 struct BEAST2_MODEL;
-typedef struct BEAST2_BASIS  * _restrict BEAST2_BASIS_PTR;
+typedef struct BEAST2_BASIS* _restrict BEAST2_BASIS_PTR;
 typedef struct BEAST2_MODEL BEAST2_MODEL, * _restrict BEAST2_MODEL_PTR;
-typedef struct PROPOSE_STRUCT {	
-	I32PTR             samples;	
+typedef struct PROPOSE_STRUCT {
+	I32PTR             samples;
 	CORESULT_PTR       keyresult;
 	F32PTR             mem;
 	BEAST2_MODEL_PTR   model;
 	BEAST2_RANDSEEDPTR pRND;
 	BEAST2_YINFO_PTR   yInfo;
 	I32                nSample_ExtremVecNeedUpdate;
 	I32                N, Npad16;
-	F32                sigFactor;	
+	F32                sigFactor;
 	F32                outlierSigFactor;
-} PROP_DATA, *_restrict PROP_DATA_PTR;
+} PROP_DATA, * _restrict PROP_DATA_PTR;
+
 
 
- 
 typedef struct BEAST2_BASESEG {
 	I32 R1, R2, K;
 	//solaris: union {
 		//solaris: struct {
-			I16 ORDER1, ORDER2; 
-		//solaris: };
-		I32     outlierKnot; //used only for the outlier component
+	I16 ORDER1, ORDER2;
+	//solaris: };
+	I32     outlierKnot; //used only for the outlier component
 	//solaris:};
 } BEAST2_BASESEG, * _restrict BEAST2_BASESEG_PTR;
 
 typedef struct _NEWTERM {
 
 	BEAST2_BASESEG  SEG[2];
 	//solaris: union {
-		TKNOT          newKnot;
-		//solaris: struct { 
-			TORDER oldOrder, newOrder; 
-		//solaris: };
+	TKNOT          newKnot;
+	//solaris: struct { 
+	TORDER oldOrder, newOrder;
 	//solaris: };
+//solaris: };
 
 	I16 nKnot_new;
 	I16 newIdx;
- 
+
 	NEWCOLINFO xcols;
 
 	U08 numSeg;
 	I08 jumpType;
 	//I16 Knewterm; //not used
 	//U08 basisID;	//not used
 } NEWTERM, * _restrict NEWTERM_PTR;
 
- 
+
 
 //period is used as "basis->bConst.dummy.period" in the following functons: computeXY,Alloc_Init_PrecPrior,DD_CalcBasisKsKeK_prec0123
 //TERMS needed only if meta->io.deseasonlaized=TRUE
 typedef struct DUMMY_CONS { F32PTR TERMS; F32PTR SQRT_N_div_n; I32 period; }          DUMMY_CONST;
-typedef struct SVD_CONS {  F32PTR TERMS; F32PTR SQR_CSUM;}                            SVD_CONST;
-typedef struct SEASON_CONST { F32PTR TERMS, SQR_CSUM, SCALE_FACTOR;}				    SEASON_CONST;
-typedef struct TREND_CONS   { F32PTR TERMS, COEFF_A, COEFF_B, INV_SQR;}	               TREND_CONST;
+typedef struct SVD_CONS { F32PTR TERMS; F32PTR SQR_CSUM; }                            SVD_CONST;
+typedef struct SEASON_CONST { F32PTR TERMS, SQR_CSUM, SCALE_FACTOR; }				    SEASON_CONST;
+typedef struct TREND_CONS { F32PTR TERMS, COEFF_A, COEFF_B, INV_SQR; }	               TREND_CONST;
 typedef struct OUTLIER_CONS { F32    SQRTN, SQRTN_1; }		                           OUTLIER_CONST;
- 
-typedef union  {
+
+typedef union {
 	SVD_CONST     svd;
 	DUMMY_CONST   dummy;
 	SEASON_CONST  season;
 	TREND_CONST   trend;
 	OUTLIER_CONST outlier;
 } BASIS_CONST;
 
 //https://gcc.gnu.org/onlinedocs/gcc/Unnamed-Fields.html
 
-typedef int  (*pfnGenTerms)(F32PTR X, I32 N, BEAST2_BASESEG*, BASIS_CONST * ptr);
-typedef struct PROP_PROB_STRUCT {U08 birth, death, merge, move;} PROP_PROB_STRUCT;
+typedef int  (*pfnGenTerms)(F32PTR X, I32 N, BEAST2_BASESEG*, BASIS_CONST* ptr);
+typedef struct PROP_PROB_STRUCT { U08 birth, death, merge, move; } PROP_PROB_STRUCT;
 typedef struct BEAST2_BASIS {
 
 	BASIS_CONST  bConst;
 	struct {
 		void        (*Propose)(BEAST2_BASIS_PTR, NEWTERM_PTR, NEWCOLINFO_PTR, PROP_DATA*);
 		pfnGenTerms GenTerms;
 		int         (*CalcBasisKsKeK_TermType)(BEAST2_BASIS_PTR  basis);
 		void        (*UpdateGoodVec)(BEAST2_BASIS_PTR basis, NEWTERM_PTR new, I32 Npad16_not_used);
 		void        (*ComputeY)(F32PTR X, F32PTR beta, F32PTR Y, BEAST2_BASIS_PTR basis, I32 Npad);
-		F32         (*ModelPrior)(BEAST2_BASIS_PTR basis, NEWCOLINFO_PTR newcol, NEWTERM_PTR new);
-	};	
+		F32(*ModelPrior)(BEAST2_BASIS_PTR basis, NEWCOLINFO_PTR newcol, NEWTERM_PTR new);
+	};
 
 	F32PTR   scalingFactor;
 	F64PTR   priorMat;
 	F64PTR   priorVec;
 
 	struct {
 		TKNOT  minSepDist;
@@ -376,82 +372,81 @@
 	TKNOT_PTR   KNOT;
 	TORDER_PTR	ORDER;  // not used for the dummpy basis
 	/*
 	union {
 		TORDER_PTR	ORDER;  // not used for the dummpy basis
 		I32			period; // only used for the dummy basiss
 	};
-	*/	
+	*/
 	I16PTR     ks, ke;
 	U08PTR     termType;
 	U08PTR08   goodvec;
 
 	I16      nPrec;
 	I16      offsetPrec;
 
 	I32      goodNum;
 	I16      nKnot;
 	I16      K, Kbase;
 	U08      type;
 
 } BEAST2_BASIS, * _restrict BEAST2_BASIS_PTR;
- 
+
 
 typedef struct {
 	F32PTR XtX, XtY, cholXtX, beta_mean;
 	F32PTR precXtXDiag;
 	I16PTR nTermsPerPrecGrp;
 
 	F32PTR   alpha2Q_star;  // made to be a pointer for MRBEAST
 
 	F32    marg_lik;
 	I32    K;
 
-    /*
+	/*
 	union {
 		F32      alpha2_star;
 		F32PTR   alphaQ_star; // added for MRBEAST
 	};
 	*/
-} BEAST2_MODELDATA, *_restrict  BEAST2_MODELDATA_PTR;
+} BEAST2_MODELDATA, * _restrict  BEAST2_MODELDATA_PTR;
 
 typedef struct BEAST2_MODEL {
-	I32 (*PickBasisID)(PROP_DATA_PTR );
+	I32(*PickBasisID)(PROP_DATA_PTR);
 
-	F32PTR  beta;	
+	F32PTR  beta;
 	F32PTR	sig2; // for MRBEAST
-	
+
 	/////////////////////////////	
 	I08PTR08 extremePosVec;
 	F32PTR   deviation;
 	F32PTR   avgDeviation;  // Changed to a pointer for a consistent API with MRBEAST
 	I32      extremPosNum;
-	
+
 	I16     nPrec;
 	F32PTR  precVec;
-	F32PTR  logPrecVec;	
- 
+	F32PTR  logPrecVec;
+
 	/////////////////
 	/*
 	F32PTR XtX,  XtY, cholXtX,  beta_mean,  beta;
 	F32PTR precXtXDiag;
 	I08PTR nTermsPerPrecGrp;
 	*/
 	//F32PTR XtX_prop, XtY_prop, cholXtX_prop, beta_mean_prop, beta_prop;
 	BEAST2_MODELDATA curr, prop;
 
 	I32          NUMBASIS;
-	I08          vid,did, sid, tid, oid;
-	BEAST2_BASIS *b;	
+	I08          vid, did, sid, tid, oid;
+	BEAST2_BASIS* b;
 
 } BEAST2_MODEL, * _restrict BEAST2_MODEL_PTR;
 
 
 
 typedef struct {
 	I32              minSepDist;
 	BEAST2_YINFO_PTR yInfo;
 } KNOT2BINVEC, * _restrict KNOT2BINVEC_PTR;
 
- 
- 
- 
+
+
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_io.h` & `Rbeast-0.1.14/ext_src/beastv2_io.h`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 extern void BEAST2_DeallocateTimeSeriesIO(BEAST2_IO_PTR T);
 
 
 /****************beastv2_in_readts******************/
 //Need to check to make sure Xnewterm/GlobalMEMBuf is big enough to handle ts aggregration. 
 //Raw ts may be longer than the aggregated ts but Xnewterm is allocated based on the length 
 // of the aggegrate ts			
-extern void  BEAST2_fetch_next_timeSeries(A(YINFO_PTR)  yInfo, int pixelIndex, F32PTR GlobalMEMBuf, A(IO_PTR)  io);
+extern void  BEAST2_fetch_timeSeries(A(YINFO_PTR)  yInfo, int pixelIndex, F32PTR GlobalMEMBuf, A(IO_PTR)  io);
 extern I08 BEAST2_preprocess_timeSeries(A(YINFO_PTR)  yInfo, BEAST2_BASIS_PTR basis, F32PTR Xtmp, BEAST2_OPTIONS_PTR opt);
 
 /****************beastv2_out_allocmem******************/
 extern void* BEAST2_Output_AllocMEM(BEAST2_OPTIONS_PTR  opt);
 extern void  BEAST2_Result_FillMEM(BEAST2_RESULT_PTR  result, BEAST2_OPTIONS_PTR  opt, const F32 nan);
 extern void  BEAST2_Result_AllocMEM(BEAST2_RESULT_PTR  result, BEAST2_OPTIONS_PTR  opt, MemPointers* _restrict MEM);
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_io_in_args.c` & `Rbeast-0.1.14/ext_src/beastv2_io_in_args.c`

 * *Files 6% similar despite different names*

```diff
@@ -6,776 +6,639 @@
 #include <stdio.h>
 #include <string.h>
 #include <time.h>
 
 #include "abc_datatype.h"
 #include "abc_blas_lapack_lib.h"
 #include "abc_ide_util.h"  //printf
-#include "abc_common.h"  //strcicmp
+#include "abc_common.h"    //strcicmp
 #include "abc_ts_func.h"
 #include "abc_date.h"
 #include "beastv2_func.h"    
 #include "beastv2_io.h"
+ 
+#define CondErrMsgRet0(cond, ...)   if(cond) { r_error(__VA_ARGS__); return 0;}
+#define CondErrActionRet0(cond, Action, ...)   if(cond) { (Action) ;r_error(__VA_ARGS__); return 0;}
+#define ifelse(cond, a, b)  ((cond)?(a):(b))
+static int  GetArg_0th_Data(VOIDPTR prhs[], int nrhs, BEAST2_IO_PTR _OUT_ io) {
 
-#define IsAlmostInteger(x)  ( fabs(x-round(x)) <1e-3 )
-static int  GetArg_1st_MetaData(VOIDPTR prhs[], int nrhs, BEAST2_METADATA_PTR meta)
-{
-	
 	// Check the number of inputs:  the first arg is the algorithm name.
-	if (nrhs < 2L) {	
-		r_error("ERROR: At least one input argument is needed!\n");
+	CondErrMsgRet0( nrhs < 2L, "ERROR: At least one input argument is needed!\n" );
+
+	VOIDPTR DATA  = prhs[1];
+	int     numel = GetNumberOfElements(DATA);
+	// Check if the input 'data' is numeric and lengthy enough 	
+	if (IsEmpty(DATA) || (/*beg*/ !(IsNumeric(DATA) && numel > 2) && !(IsStruct(DATA) && numel >= 1) && !IsCell(DATA) /*end*/) ) {
+		/* IsCell  true Only for Matlab*/
+		// Yobj has multivariate time series if it is a struct variable
+		r_error("ERROR: The input data should be numeric and must be long enough.\n");
 		return 0;
 	}
-
-	meta->rawInput     = prhs[1];	
-	
  
+	/*****************************************************************************************/
+	/* If pY is not a string but a matrix or vector  find the dimesions, and configure io-*/
+	/*****************************************************************************************/
+	I32       q = 0;
+	VOID_PTR  Y = NULL;
+	if ((IsStruct(DATA) && numel >= 1) || IsCell(DATA)) {
+		// For MRBEAST only: Yobj is a struct variable with multivariate time series						
+		q = numel;
+		// Mem to be dellocated in DeallocatTimeSeriesIO
+		io->pdata = malloc(sizeof(VOID_PTR) * q);
+		io->dtype = malloc(sizeof(DATA_TYPE) * q);
+		//TODO: For MRBEAST,the dimensions of all elments are assumed to be the same
+		// A sanity check needs to be done to ensure that is the case.
+		for (int i = 0; i < q; i++) {
+			Y = GetFieldByIdx(DATA, i);
+			io->pdata[i] = GetData(Y);
+			io->dtype[i] = GetDataType(Y);
+		}		
+	} else {
+		//DATA is a vector of numeric type, and not a struct variable with multivariate time series			
+		q = 1;
+		//Mem to be dellocated in DeallocatTimeSeriesIO
+		io->pdata   = malloc(sizeof(VOID_PTR) * q);
+		io->dtype    = malloc(sizeof(DATA_TYPE) * q);
+		io->pdata[0] = GetData(DATA);
+		io->dtype[0] = GetDataType(DATA);
+		Y = DATA;
+	}
+	for (int i = 0; i < q; i++) {
+		CondErrMsgRet0( io->dtype[i] == DATA_UNKNOWN, "ERROR: The input data has an uknown numeric type!\n");		
+	}
+	io->q = q;
 
-	I08 metaProcessed = 0;
-	if (nrhs < 3) {
-		meta->isMetaStruct		= 0;
-		meta->isRegularOrdered  = 1; //We asumme the data is regular if no meta is supplied
-		meta->hasSeasonCmpnt    = 1;
-		meta->hasOutlierCmpnt   = 0;
-		meta->seasonForm        ='S';
-		meta->detrend           = 0;
-		meta->deseasonalize     = 0;
-		meta->period			= getNaN();
-
-		meta->startTime = 1.f;
-		meta->deltaTime = 1.f;	
-		meta->missingValue = getNaN();// FLOAT_MAX;
-		meta->maxMissingRate = 0.75;
-		meta->whichDimIsTime = -1; //Not used
-		meta->rawTimeVec      = NULL;
-
-		metaProcessed = 1;
-	}
-
-	if (nrhs >= 3 && IsNumeric(prhs[2L])) {
-
-		VOIDPTR pmeta = prhs[2L];
-
-		meta->isMetaStruct = 0;
-		meta->isRegularOrdered = 1L; //We asumme the data is regular if meta is a scalar numeric value.
-		meta->hasSeasonCmpnt   = 1L;
-		meta->hasOutlierCmpnt  = 0L;
-		meta->seasonForm        ='S';
-		meta->detrend           = 0;
-		meta->deseasonalize     = 0;
-
-		meta->period    = GetScalar(pmeta);
-		meta->startTime = 1.f;
-		meta->deltaTime = 1.f;
-		meta->missingValue = getNaN();// FLOAT_MAX;
-		meta->maxMissingRate = 0.75;
-		meta->whichDimIsTime = -1; //Not used
-		meta->rawTimeVec     = NULL;
+	/*************************************************/
+	/* Get the dimension of the input              */
+	/*************************************************/
+	io->timedim = UnknownStatus;   // A filler to indicate hte status is undetermined
+	I32 ndims = GetNumOfDim(Y);	
+	if (ndims == 0 ||	 // the input is a vector: ndims == 0  is possible only for R vectors (not  Matlab)
+		ndims == 1)      // the input is a vector: ndims == 1  is possible only for Python vectors (not R or matlab)
+	{
+		I32 N = GetNumberOfElements(Y);
+		io->ndim    = 1L;
+		io->dims[0] = N;
+		io->dims[1] = 1L;
+		io->dims[2] = 1L; 
+		io->timedim = 1L; 		
+	}
+	else if (ndims == 2) {
+		// Matlab: a vector or matrix;
+		// R:      a matrix or a vector with a dim attribute.
+		int N = GetDim1(Y);
+		int M = GetDim2(Y);
 
-		metaProcessed = 1;
+		if (min(N, M) == 1L) {
+			//PY is a vector
+			N = max(N, M),
+			io->ndim   = 1L;
+			io->dims[0] = N;
+			io->dims[1] = 1L;
+			io->dims[2] = 1L;
+			io->timedim = 1L;
+		} else {
+			//PY is a matrix
+			io->ndim = 2L;
+			io->dims[0] = N;
+			io->dims[1] = M;
+			io->dims[2] = 1L; // for 2d matrix input, the last dimenion is always set to 1L 
+		}//PY is a matrix
+	}
+	else if (ndims == 3) {
+		// If the input is a 3D array
+		io->ndim = 3L;
+		GetDimensions(Y, io->dims, 3L);	
+	}
+	else {
+		r_printf("ERROR: The maximum dimension allowed is 3 when data is a 3D stack of images over time, but the input has a dimension of %d.\n", ndims);
+		return 0;
 	}
 
-	if (nrhs >= 3 && IsStruct(prhs[2L])  ) {
+	return 1;
+}
+
+static float ParsePeriod(BEAST2_IO_PTR _OUT_ io);
+static int   Parse_whichDimIsTime(BEAST2_IO_PTR _OUT_ io, int Nrawtime, int userWhichDim);
 
-		meta->isMetaStruct = 1;
+static int  GetArg_1st_MetaData(VOIDPTR prhs[], int nrhs, BEAST2_IO_PTR _OUT_ io) {
 	
-		VOIDPTR pmeta = prhs[2L];
-		VOIDPTR tmp;
 
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		meta->isRegularOrdered = (tmp = GetField123Check(pmeta, "isRegularOrdered",2)) ? GetScalar(tmp) : 1L;
-		if (tmp == NULL)
-			r_warning("WARNING: metadata$isRegularOrdered is not specified. A default 'metadata$isRegularOrdered=TRUE' is assumed.\n");
+	BEAST2_METADATA_PTR meta = &io->meta;
+	meta->nrhs = nrhs;
 
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		// Get the season string to determine the number and types of season components: harnomic or dummy
-		
-		
-		if ((tmp = GetField123Check(pmeta, "season",2)) != NULL && IsChar(tmp)) {			
-			char season[20 + 1];
-			GetCharArray(tmp, season, 20);
-			ToUpper(season);
-
-			char a = season[0], b = season[1];
-			if      (a=='N' && b=='O') 		meta->hasSeasonCmpnt = 0;							    //none
-			else if (a=='H' && b=='A') 		meta->hasSeasonCmpnt = 1, meta->seasonForm = 'S'; 	//harmonic
-			else if (a=='D' && b=='U')		meta->hasSeasonCmpnt = 1, meta->seasonForm = 'D';			//dummy
-			else if (a=='S' && b=='V')		meta->hasSeasonCmpnt = 1, meta->seasonForm = 'V';			//svd			
+	/**********************************/
+	// Get the type of metadata
+	/**********************************/
+	int METADATA_NONE          = _False_;
+	int METADATA_NumericScalar = _False_;
+	int METADATA_NumericVector = _False_;
+	int METADATA_CharVector    = _False_;
+	int METADATA_CharScaler    = _False_;
+	int METADATA_Struct        = _False_;
+	int METADATA_OTHER         = _False_;
+
+	VOIDPTR pmeta              = (nrhs < 3) ? NULL : prhs[2L];
+	VOIDPTR TIMEobj            = NULL;
+	int     userWhichDimIsTime = UnknownStatus;
+	if ( pmeta==NULL || IsEmpty(pmeta) ) {
+		METADATA_NONE       = _True_;
+	} else if ( IsNumeric(pmeta) ) {
+		int  numel = GetNumberOfElements(pmeta);
+		if      (numel == 0) METADATA_NONE          = _True_;
+		else if (numel == 1) METADATA_NumericScalar = _True_;
+		else if (numel > 1 ) METADATA_NumericVector = _True_, TIMEobj = pmeta;
+		else 			     METADATA_OTHER         = _True_;
+	} else if ( IsChar(pmeta) ) {
+		int numel = GetNumberOfElements(pmeta);
+		if      (numel == 0) METADATA_NONE          = _True_;
+		else if (numel == 1) METADATA_CharScaler    = _True_;
+		else if (numel > 1 ) METADATA_CharVector    = _True_, TIMEobj = pmeta;
+		else 			     METADATA_OTHER         = _True_;
+	} else if (IsStruct(pmeta) ) {
+		METADATA_Struct      = _True_;
+		TIMEobj              =  GetField123Check(pmeta, "time", 2) ; // if time is NULL or empty []	VOIDPTR  tmp;
+		VOIDPTR  tmp;
+		userWhichDimIsTime  = (tmp = GetField123Check(pmeta, "whichDimIsTime", 2)) ? GetScalar(tmp) : UnknownStatus;
+	} else {
+		METADATA_OTHER = _True_;
+	}
+	CondErrMsgRet0(METADATA_OTHER == _True_, "ERROR: The 'metadata' parameter given is of unsupported type.\n");
+
+	//*****************************************************************
+	// Determnie if it has a seaosn component or not: Moved here
+	// becuase period is needed in TSaggragatePrepare()
+	//*****************************************************************	
+	meta->hasSeasonCmpnt = UnknownStatus;
+	I08 ISDATE   = UnknownStatus;
+	F32 START    = getNaN();
+	F32 DT       = getNaN();
+	F32 PERIOD   = getNaN();
+	//////////////////////////////////////////////////////////////////////////////////
+	if (METADATA_NONE || METADATA_NumericScalar || METADATA_CharVector || METADATA_CharScaler ||  METADATA_NumericVector) {
+		//meta->isRegularOrdered  = 1; // We asumme the data is regular/orderred if no meta is supplied
+	 
+		START  = getNaN();
+		DT     = getNaN();
+		PERIOD = getNaN();
+		if (METADATA_NumericScalar) {
+			PERIOD = GetScalar(pmeta);
+			if (!IsNaN(PERIOD) ) {
+				if (PERIOD <= 0.) {
+					q_warning("WARNING: A negative or zero value of period (%g) means no periodic/seasonal component in the input time series!\n", meta->period);
+				} else{ //meta->period > 0;
+					CondErrMsgRet0(!_IsAlmostInteger(PERIOD),
+						"ERROR: When metadata is supplied as a single number %g, it must be an integer to specify the period of the regular time seires!\n", meta->period);
+					PERIOD = round(PERIOD);
+				}
+			}
+			meta->hasSeasonCmpnt = PERIOD <= 0.0? _False_ :_True_; // Period may be still a NAN  if meta is a NAN
+		}	else if (METADATA_CharScaler) {
+		// there is only one possibiliyt: Period nyst be the string 'none"
+			char period[10+1];
+			GetCharArray(pmeta, period, 10L);
+			CondErrMsgRet0( strcicmp(period, "none") != 0, "ERROR: When metadata is supplied as a string to speciify period, it can only be 'none'!\n");
+ 			meta->hasSeasonCmpnt = _False_;
+			PERIOD               = 0.0;
+		}	else {
+			// has a seasonal component with period still being NAN and to be determined
+			meta->hasSeasonCmpnt = _True_;
+		}
+		meta->seasonForm        = ifelse( meta->hasSeasonCmpnt, 'S','N');
+
+		meta->hasOutlierCmpnt   = _False_;		
+		meta->detrend           = _False_;
+		meta->deseasonalize     = _False_;
+		meta->missingValue      = getNaN();// FLOAT_MAX;
+		meta->maxMissingRate    = 0.75f;
+	}
+	else if (METADATA_Struct) {
+	//*****************************************************************
+	// Determnie if it has a seaosn component or not when  METADATA_Struct =1
+	//*****************************************************************	
+		VOIDPTR  tmp;
+
+		//  Deermine the startTime property
+		tmp = GetField123Check(pmeta, "startTime", 2); // IsEmpty is checked inside GetField123Check
+		TimeScalarInfo timevalue;
+		Parse_SingelDateObject(tmp, &timevalue);
+		START = timevalue.value;
+		if (timevalue.unit == 'Y')  ISDATE = _True_;
+		CondErrMsgRet0(timevalue.unit == 'B', "ERROR: cannot interpret the metadata$startTime input,'\n");
+
+		//  Deermine the deltaTime property		
+		tmp = GetField123Check(pmeta, "deltaTime", 3);
+		Parse_TimeIntervalObject(tmp, &timevalue);
+		DT  = timevalue.fyear;
+		if (timevalue.unit != 'U' && timevalue.unit != 'B') ISDATE = _True_;
+		CondErrMsgRet0(timevalue.unit == 'B', "ERROR: cannot interpret the metadata$deltaTime input,'\n");
+		CondErrMsgRet0(DT             <= 0,   "ERROR: metadata$deltaTime must be a positive time interval!\n");
+
+		//  Deermine the period property
+		tmp = GetField123Check(pmeta, "period", 2);
+		Parse_TimeIntervalObject(tmp, &timevalue);
+		PERIOD  = timevalue.fyear;
+		if (timevalue.unit != 'U' && timevalue.unit != 'B') ISDATE = _True_;
+		CondErrMsgRet0(timevalue.unit == 'B', "ERROR: cannot interpret the metadata$period input,'\n");
+
+		if (PERIOD<=0) {
+			meta->hasSeasonCmpnt = _False_;
+			q_warning("WARNING: A negative or zero value of period (%g) indicates no periodic/seasonal component in the input time series!\n", PERIOD);
+		}
+		if (PERIOD > 0 && PERIOD /DT >= 2.0) {
+			meta->hasSeasonCmpnt = _True_;			
+		}
+		if (PERIOD > 0 && PERIOD /DT < 2.0) {
+			meta->hasSeasonCmpnt = _False_;
+			q_warning("WARNING: The value metadata$period/metadata$deltTime=%g/%g=%g is unreasonalbe for a siginal with seasonal componet, so no seasonal component is "
+				"assumed and the trend-only model is fitted. Perios is also set to 0.0\n", PERIOD, DT, PERIOD/DT);
+			PERIOD = 0;
+		}
+
+		/////////////////////////////////////////////////////////// 
+		//   Get the season string to determine the number and types of season components: harnomic or dummy
+		////////////////////////////////////////////////////////// 
+		tmp = ( tmp=GetField123Check(pmeta, "season", 2) , tmp && !IsChar(tmp) ? NULL : tmp);
+		char season[20 + 1];
+		GetCharArray(tmp, season, 20); // Will check if tmp is NULL inside the function
+		ToUpper(season);
+		char a = season[0], b = season[1];
+	
+	   if (meta->hasSeasonCmpnt == _False_ && a != 'N' && a != '\0' ) {
+		   // period has been set and used to determine hasSeasonCMpnt or not
+			   q_warning("WARNING: A confilict found between metadata$season=%s and period=%g. '%s' suggests a time series with periodic variations but "
+				         "period=%g or period='none' suggests a trend-only time series without any periodic variations. The season parameter is "
+				         "ignored and no seasonal component is assumed for the input.\n", season, PERIOD, season, PERIOD);
+		} else if  (tmp  && IsChar(tmp) ) {			
+			// tmp may be an empty string "" (a=0).
+			int  hasSeasonCmpt_bySeasonStr = _True_;			
+			if    ((a=='N' && b=='O') || a == '\0')		hasSeasonCmpt_bySeasonStr = _False_;								//none
+			else if (a=='H' && b=='A') 					hasSeasonCmpt_bySeasonStr = _True_, meta->seasonForm = 'S';    	//harmonic
+			else if (a=='D' && b=='U')					hasSeasonCmpt_bySeasonStr = _True_, meta->seasonForm = 'D';		//dummy
+			else if (a=='S' && b=='V')					hasSeasonCmpt_bySeasonStr = _True_, meta->seasonForm = 'V';		//svd			
 			else {
-				meta->hasSeasonCmpnt = 1;
-				meta->seasonForm     = 'S';  //the default form is harmonic
-				r_warning("WARNING: metadata$season=%s is specified but has an unrecongizable string. A default metadata$season='harmonic' is used instead.\n", season);
+				hasSeasonCmpt_bySeasonStr = _True_;
+				meta->seasonForm          = 'S';  //the default form is harmonic
+				q_warning("WARNING: metadata$season='%s' has an unrecongizable string. The default season='harmonic' is used instead.\n", season);
 			}
 
-			if (meta->seasonForm == 'V') meta->svdTerms = GetFieldCheck(pmeta, "svdTerms");
-
-		} else  {
-			meta->hasSeasonCmpnt = 1;
-			meta->seasonForm     = 'S';
-			r_warning("WARNING: metadata$season is either missing or not given as a valid specifier string (e.g., none, harmonic, or dummy). A default "
-				      "metadata$season='harmonic' is assumed.\n");
-		}	
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		meta->hasOutlierCmpnt = (tmp = GetField123Check(pmeta, "hasOutlierCmpnt",2)) ? GetScalar(tmp) : 0L;
-
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		meta->detrend         = (tmp = GetField123Check(pmeta, "detrend"      ,3)) ?  GetScalar(tmp) : 0L;
-		meta->deseasonalize   = (tmp = GetField123Check(pmeta, "deseasonalize",3)) ?  GetScalar(tmp) : 0L;
- 
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		meta->period = (tmp = GetField123Check(pmeta, "period",2)) ? GetScalar(tmp) : getNaN();
-		if (!meta->hasSeasonCmpnt && tmp != NULL)
-			r_warning("WARNING: For metadata$season='none' (i.e., no periodic component in the time series), metadata$period is ignored!\n");
-
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		I08 isDefaultStartTime = 0;
-		tmp = GetField123Check(pmeta, "startTime",2);
-		if     (tmp && IsClass(tmp,"Date")) 		{
-			// this branch is true only for R and Matlab's IsClass always return FALSE
-			// in R, tmp is an integer array
-			int   days      = GetScalar(tmp);
-			meta->startTime = fractional_civil_from_days(days);
-		}
-		else if (tmp && IsNumeric(tmp)) {
-			I32 n = GetNumberOfElements(tmp);
-			if (n==1)
-				meta->startTime = GetScalar(tmp);
-			else if (n == 2) {
-				F32 Y = GetNumericElement(tmp, 0);
-				F32 M = GetNumericElement(tmp, 1);
-				meta->startTime = YMDtoF32time(Y, M, 15);
-				r_warning("WARNING: Your metadata$startTime (%f, %f) is interpreted as (Year: %d, Month: %d, Day: 15) and converted to "
-					       "a numeric value of %f. If not making sense, make sure to supply a correct start time: "
-					       "startTime can take a numeric scalar, a vector of two values (year, month), or a vector of three values (year, month,day).",
-					       Y,M, (int)Y, (int)M, meta->startTime);
-			}
-			else if (n == 3) {
-				F32 Y = GetNumericElement(tmp, 0);
-				F32 M = GetNumericElement(tmp, 1);
-				F32 D = GetNumericElement(tmp, 2);
-				meta->startTime = (F32) YMDtoF32time((int)Y, (int)M, (int)D);
-				r_warning("WARNING: Your metadata$startTime (%f, %f, %f) is interpreted as (Year: %d, Month: %d, Day: %d) and converted to "
-					"a numeric value of %f. If not making sense, make sure to supply a correct start time: "
-					"startTime can take a numeric scalar, a vector of two values (year, month), or a vector of three values (year, month,day).",
-					Y, M,D, (int)Y, (int)M, (int)D, meta->startTime);
+			if (meta->hasSeasonCmpnt == _True_ && hasSeasonCmpt_bySeasonStr == _False_) {
+				hasSeasonCmpt_bySeasonStr = _True_;
+				meta->seasonForm          = 'S';
+				q_warning("WARNING: A confilict found between metadata$season='none' and period=%g. season='none' suggests a time series with "
+					       "no periodic variations but period=%g suggests otherwise. The season='none' parameter is ignored and "
+					      "the data is assumed to have a seasonal component.\n", PERIOD, PERIOD);
 			}
-			else { 
-				r_error("ERROR: Your metadata$startTime is a vector of more than three elements. A valid 'startTime' should be either a numeric scalar,"
-					     "a vector of two values (year, month), or a vector of three values (year, month,day)."	);
-				return 0;
+			meta->hasSeasonCmpnt = hasSeasonCmpt_bySeasonStr;
+		} 	else	{
+			if (meta->hasSeasonCmpnt == UnknownStatus || meta->hasSeasonCmpnt == _True_) {
+				meta->hasSeasonCmpnt = _True_;
+				meta->seasonForm     = 'S';
+				q_warning("WARNING: metadata$season is either missing or not given as a valid specifier string (e.g., none, harmonic, or dummy). A default season='harmonic' is assumed.\n");
 			}
-			
-		} else {
-			meta->startTime = 1L;
-			isDefaultStartTime = 1L;
+		}	
+
+		if (meta->seasonForm == 'V') {
+			meta->svdTerms_Object   = GetFieldCheck(pmeta, "svdTerms");
+			meta->svdYseason_Object = GetFieldCheck(pmeta, "svdYseason");
 		}
 
-		////////////////////////////P//////////////////////////////////////////////////////////////////
-		I08 isDefaultDeltaTime = 0;
-		meta->deltaTime = (tmp = GetField123Check(pmeta, "deltaTime",3)) ? GetScalar(tmp) : getNaN();			
-		if (!meta->isRegularOrdered && IsNaN(meta->deltaTime) ) {
-			r_error("ERROR: when metadata$isRegualrOrdered=FALSE, the input data is considered irregular/unordered in time AND "
-			 	   "metadata$deltaTime must be specified for BEAST to pre-process and aggregate the irregular input to a regular time series spaced at deltaTime.\n");
-			return 0;
-		} 
-		if (meta->deltaTime <= 0  ) {
-			r_error("ERROR: metadata$deltaTime must be a positive time interval!\n");
-			return 0;
+		meta->hasOutlierCmpnt = (tmp = GetField123Check(pmeta, "hasOutlierCmpnt", 2)) ? GetScalar(tmp) : _False_;
+		meta->detrend         = (tmp = GetField123Check(pmeta, "detrend"      ,3)) ?  GetScalar(tmp)   : _False_;
+		meta->deseasonalize   = (tmp = GetField123Check(pmeta, "deseasonalize",3)) ?  GetScalar(tmp)   : _False_;
+		meta->missingValue	  = (tmp = GetField123Check(pmeta, "missingValue",0))   ? GetScalar(tmp)   : getNaN();// FLOAT_MAX;
+		meta->maxMissingRate  = (tmp = GetField123Check(pmeta, "maxMissingRate",0)) ? GetScalar(tmp)   : 0.75;
+	} //else if (nrhs >= 3)
+	else {
+		CondErrMsgRet0(  _True_, "ERROR: The 'metadata' parameter given is of unsupported type.\n");
+	}
+
+	////////////////////////////////////////////////////////////////////////////////
+	// Sanity check
+	CondErrMsgRet0(meta->hasSeasonCmpnt == UnknownStatus, "ERROR: Cnnot determine whether the input time series has a seasonal/periodic componnet or net.\n");
+	if (meta->hasSeasonCmpnt == 0) PERIOD = 0;        //just double check to make sure it is the case that period=0 for trend-only data
+	if (DT  < 0.)      DT     = getNaN(); //dT should never < 0 at this point, but just double check.
+	////////////////////////////////////////////////////////////////////////////////
+
+	/**********************************/
+    // If there is a time object suppiked
+	/**********************************/
+	TimeVecInfo tvec = { 0 };
+	TimeVec_init(&tvec);
+
+     if (TIMEobj) { 
+		//  Allocated mem that needs to be freeed explicilty for tvec.fyear, but noo mem allocated if TIMEObj
+		//  is NULL, which means that the ts is regular/ordered, as dertermined by start and dt only
+		int Nrawtime = TimeVec_from_TimeObject(TIMEobj, &tvec);        // isDate may be updated inside based on the TimeObj
+	    if(tvec.isDate == 1) ISDATE =_True_;                            // this is the LAST chance to decide whether the time is date
+	   
+		// Nawtime must be larger than 1L.
+		CondErrMsgRet0( Nrawtime<=1, "ERROR: Unable to read and intepret 'time' or 'metadata$time'!\n");
+
+		// io->timedim and meta->whichDim are filled insside
+		// Nrawtime>1: we know the time series length
+		userWhichDimIsTime=Parse_whichDimIsTime(io, Nrawtime, userWhichDimIsTime);  
+		CondErrMsgRet0(userWhichDimIsTime <= 0, "ERROR: Unable to dtermine which dimo of the input data refers to the time'!\n");
+	
+	} else {
+	 /**********************************/
+    // TIMEobj=NULLL If there is no time object suppiled; it must be a regular ts
+	// Assume it is a regular time series
+	/**********************************/
+		int Nrawtime = 0;
+
+		// io->timedim and meta->whichDim are filled insside
+		// Nrawtime>0: we know the time series length
+		userWhichDimIsTime = Parse_whichDimIsTime(io, Nrawtime, userWhichDimIsTime);
+		CondErrMsgRet0(userWhichDimIsTime <= 0, "ERROR: Unable to dtermine which dimo of the input data refers to the time'!\n");
+
+		int isDefaultDeltaTime = 0;
+		int isDefaultStartTime = 0;
+		if (IsNaN(START)) {
+			START              = 1.f;
+			isDefaultStartTime = 1L;
 		}
-		if (meta->isRegularOrdered && IsNaN(meta->deltaTime)) {
-			meta->deltaTime    = 1.f;
-			isDefaultDeltaTime = 1;		
+		if (IsNaN(DT)) {
+			DT   = 1.f;
+			isDefaultDeltaTime = 1L;
 		}
-		
-		if (meta->isRegularOrdered ) {
-			if (isDefaultDeltaTime && isDefaultStartTime) {
-				r_warning("WARNING: when metadata$isRegualrOrdered=TRUE, the input data is assumed to be regular and ordered in time AND the times of "
-					"individual datapoints are determined fully by 'metadata$startTime' and 'metadata$deltaTime'. But metadata$startTime and deltaTime "
-					"are missing and a default value 1 is used for both!\n");
+
+		char *warningMsg= "WARNING: If the input data is regular and ordered in time, the times of individual datapoints are determined fully by 'metadata$startTime' and 'metadata$deltaTime'.";
+		if (isDefaultDeltaTime && isDefaultStartTime) {
+			q_warning("%s But startTime and deltaTime are missing and a default value 1 is used for both!\n", warningMsg);
+			if (ISDATE == _True_) { // as determined from the period field
+				q_warning("WARNING! The default sartTime=1 and deltaTime=1  are used, but the 'period' field specifies that the time is date\n");
 			}
-			else if (isDefaultStartTime) {
-				r_warning("WARNING: when metadata$isRegualrOrdered=TRUE, the input data is assumed to be regular and ordered in time AND the times of "
-					"individual datapoints are determined fully by 'metadata$startTime' and 'metadata$deltaTime'. But startTime is missing "
-					"and a default value 1 is used!\n");
+		} else if (isDefaultStartTime) {
+			q_warning("%s But startTime is missing and a default value 1 is used!\n", warningMsg);
+			if (ISDATE == _True_) { // as determined from the period field
+				q_warning("WARNING! The default startTime=1 is used, but the 'period' field specifies that the time is date\n");
+			}
+		} else if (isDefaultDeltaTime) {
+			q_warning("%s But deltaTime is missing and a default value 1 is used!\n", warningMsg);
+			if (ISDATE == _True_) { // as determined from the period field
+				q_warning("WARNING! The default deltaTime=1 is used, but the 'period' field specifies that the time is date\n");
 			}
-			else if (isDefaultDeltaTime) {
-				r_warning("WARNING: when metadata$isRegualrOrdered=TRUE, the input data is assumed to be regular and ordered in time AND the times of "
-					"individual datapoints are determined fully by 'metadata$startTime' and 'metadata$deltaTime'. But deltaTime is missing and a default"
-					" value 1 is used!\n");	
-			}			
 		}
-		
 
- 
+		int N = io->dims[userWhichDimIsTime - 1];   // filled in Parse_whichDimIsTime;
 
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		meta->rawTimeVec = (tmp = GetField123Check(pmeta, "time",2)) ? tmp : NULL;
-		if (meta->isRegularOrdered && tmp)
-			r_warning("WARNING: metadata$time is specified but ignored. For regular ordered time series, 'metadata$startTime=%f' and 'metadata$deltaTime=%f' "
-					  "alone are enough to determine the times for all data points. \n", meta->startTime, meta->deltaTime);
-		if (!meta->isRegularOrdered && tmp == NULL) {
-			r_error("ERROR: metadata$isRegualrOrdered=0 (false) indicates that the input data is irregular or unordered in time; 'metadata$time' must be "
-				     "also supplied to specify the times at which individual data points are collected.\n");
-			return 0;
+		TimeVec_from_StartDeltaTime(&tvec, START, DT, N, ISDATE);         // isDate is not updated inise		
+		PERIOD          = tvec.isDateNum == 1 ? PERIOD * 365 : PERIOD; // time unit may be changed to datenum inside the function above
+		START           = tvec.data_start;   // time unit might have been changed
+		DT              = tvec.data_dt;      // time unit might have been changed
+	}
+	// No change to update IsData any longer, so if it is still undetermined, then, it is not date
+	ISDATE = ISDATE == UnknownStatus ? _False_ : ISDATE; 
+
+	// Sorted_time_indices are allocated here taht need to be de-allocated explicilty
+	TimeVec_SortCheckRegularOrder(&tvec); // Update data_start and data_dT
+
+	tvec.isDate       = ISDATE;
+	tvec.data_period  = PERIOD;
+	tvec.out.start    = START; // may be still NA in the case of TimeObj != NULL
+	tvec.out.dT       = DT;  // may be still NA in the case of TimeObj != NULL
+
+	// datt_period may be changed inside when f32time is converted to days
+   // out.start may be adjustd slightly to better match the real start of the time series
+	TimeVec_UpdateUserStartDt(&tvec); // PERIOD may be needed in this function to get a better estiamte of dT
+	                                  
+	if (TIMEobj && IsNaN(DT)) {
+	// When TIMEObj is not NULL and dT is not available from the input
+	//FOr regular inpus: q_warning("WARNING: The input time series is regular and metadata$deltaTime/deltat is missing, the regular time interval %g is used. If not making sense, "
+	//      "please specify metadata$deltaTime/deltat explicitly. \n", io->T.dT);
+		F32 dT_new = tvec.out.dT;
+		if (io->T.isRegular == 0) {
+			if (ISDATE && io->T.out.asDailyTS==1) {
+				q_warning("WARNING: The input time series is irregular (or may span across leap years) and BEAST needs to aggregate/resample it into regular data "
+					"at a user-specified interval 'metadata$deltaTime/deltat' (for faster computation). But deltaTime is missing, a best guess of it %g year = %g months = %g days is used. "
+					"If not making sense, please specify metadata$deltaTime/deltat explicitly. \n", dT_new, dT_new * 12, dT_new * 365.0);
+			} else {
+				q_warning("WARNING: The input data is irregular and for faster computaiton, BEAST needs to aggregate/resample it into regular data "
+					"at a user-specified interval 'metadata$deltaTime/deltat' But deltaTime is missing, a best guess of it %g is used. "
+					"If not making sense, please specify metadata$deltaTime/deltat explicitly. \n", dT_new);
+			}
 		}
-
-		//////////////////////////////////////////////////////////////////////////////////////////////
-		meta->missingValue			= (tmp = GetField123Check(pmeta, "missingValue",2))   ? GetScalar(tmp) : getNaN();// FLOAT_MAX;
-		meta->maxMissingRate 		= (tmp = GetField123Check(pmeta, "maxMissingRate",2)) ? GetScalar(tmp) : 0.75;
-		meta->whichDimIsTime		= (tmp = GetField123Check(pmeta, "whichDimIsTime",2)) ? GetScalar(tmp) : -1;
-
-		metaProcessed = 1;
-
-	} //else if (nrhs >= 3)
-
-	if (metaProcessed == 0 ) {
-		r_error("ERROR: The 'metadata' parameter given is of unsupported type.\n");
-		return 0;
 	}
-
-	/*************************************************/
-	// Convert period to the unit of deltaTime
-	/*************************************************/
-	if (meta->hasSeasonCmpnt) {	
-		meta->period = meta->period / meta->deltaTime;
-		F32 period   = meta->period;
-		if (period == 0) {
-			r_error("ERROR: Your input parameters are \"metadata$period=0\" and \"metadata$season='%s'\". BEAST can't handle a time series with no perodicity. "
-				"If you mean to handle a trend-only time series, please use the trend-only version of the BEAST algorithm by specifying metadata$season='none'."
-				, meta->seasonForm == 'S' ? "harmonic" : "dummy" );
+	PERIOD = tvec.data_period;
+	START  = tvec.out.start;
+	DT     = tvec.out.dT;;
+
+	io->N = tsAggegrationPrepare(&tvec);
+
+	/////////////////////////////////////////////////////////
+	// PERIOD is still uknown. Guess it via auto-correlation
+	// Up to this point, if period=NAN, it will be further determined via auto-correlaton, It must be an intger
+	/////////////////////////////////////////////////////////	
+	meta->IsPeriodEstimated = 0;
+	if ( meta->hasSeasonCmpnt && IsNaN(PERIOD)) {		
+		io->T = tvec; // TODO: must update io->T because it is needed inside ParsePeriod
+		F32  estPeriod = ParsePeriod(io);
+		char* season;
+		char* msg;
+		season =io->meta.seasonForm == 'S' ?      "harmonic" :
+			    io->meta.seasonForm == 'V' ?     "svd":
+			                                     "dummy";
+		msg   = "suggests that the time series has a periodic/seasonal component. \"metadata$period\" is needed but missing.";
+		if (estPeriod > 0) {
+			q_warning( "WARNING: metadata$season='%s' %s A BEST GUESS of numbers of datapoints per period is %d, giving period = num_sample_per_period * deltaTime "
+				"= %d*%g = %g. Please make sure this estimate makes sense; otherwise, the BEAST decomposition result will be incorrect.\n",
+				season,  msg,  (int)estPeriod, (int)estPeriod, DT, DT * estPeriod);
+		}	else {
+			r_error("ERROR: metadata$season='%s' %s BEAST tried to estimate it via an auotcorrelation method but failed to get a reliable estimate. "
+				"Please specify the period value EXPLICILTY. Or if your input has no periodic/seasonal component at all, "
+				" set metadata$season='none' or period=0, which will fit a trend-only model.\n", season, msg);
 			return 0;
 		}
+		meta->IsPeriodEstimated = 1;
+		PERIOD = estPeriod * DT; // Convert period to the unit of deltaTime
+	}
 
-		if (meta->seasonForm == 'D' && !IsNaN(period) && !IsAlmostInteger(period)  ) {
-			r_error("ERROR: Your input parameters are \"metadata$period=%f\" and \"metadata$season='%s'\". For a dummy seasonal component, "
-				"period must be a multiple of deltaTime by an INTEGER number. Your period/deltaTime is %f.",	
-				 period*meta->deltaTime, "dummy", period );
-			return 0;
-		}
-	
+ 
+	// Another check on PERIOD: make sure there are at least 2 point per period
+	if (meta->hasSeasonCmpnt == 1) {	
+		F32 freq = PERIOD / DT;
+		CondErrMsgRet0(freq <= 0, "ERROR: BEAST can't handle a time series with a periodic componnet (\"metadata$season='%s'\") but with metadata$period=%g or period='none' specified. If you mean to "
+				    "handle trend-only time series, use the trend-only BEAST version by specifying metadata$season='none'.", meta->seasonForm == 'S' ? "harmonic" : "dummy" ,PERIOD);
+		CondErrMsgRet0(freq <2, "ERROR: BEAST can't handle a time series with a periodic componnet (\"metadata$season='%s'\") but with metadata$period=%g and metadata$deltaTime=%g specified, "
+			                    "which gives only 'period/deltatime=%g' data points per period, If you mean to "
+							    "handle trend-only time series, use the trend-only BEAST version by specifying metadata$season='none'.", meta->seasonForm == 'S' ? "harmonic" : "dummy", PERIOD, DT, PERIOD/DT);
+		CondErrMsgRet0(meta->seasonForm == 'D' && !IsNaN(freq) && !_IsAlmostInteger(freq), "ERROR: For a dummy seasonal component (\"metadata$season='dummy'\"), metadata$period=%g must be a multiple of metadata$deltaTime by an INTEGER number. "
+			"Your period/deltaTime ratio is %g.", freq* DT, freq);
+		CondErrMsgRet0(meta->seasonForm == 'V' && !IsNaN(freq) && !_IsAlmostInteger(freq), "ERROR: For a SVD seasonal component (\"metadata$season='dummy'\"), metadata$period=%g must be a multiple of metadata$deltaTime by an INTEGER number. "
+			"Your period/deltaTime ratio is %g.", freq* DT, freq);	 
 	}
 
-	// Up to this point, if period=NAN, it will be further determined in ParseInputData
 
+	meta->startTime   = START;  //shound't be NAN
+	meta->deltaTime   = DT;     //shound't be NAN
+	meta->period      = PERIOD/DT;
 
+	TimeVec_kill_fyearArray(&tvec); // Deallocate f64time only; the other allocate mem is still needed
+	io->T = tvec;
 
-	meta->nrhs = nrhs;
+ 
 	return 1;
 }
 
-static INLINE I32 __GetRawTimeDimension(BEAST2_IO_PTR io) {
-	 return io->dims[io->meta.whichDimIsTime - 1];
-}
-
-static int  ___PraseMetaData_RegularTS_Dim123(A(METADATA_PTR) meta, BEAST2_IO_PTR io) {
-	/*  If the input is regular time series */ 
-	if (meta->nrhs < 3 && io->ndim >=2 ) {
-		// No metadata input
-		r_error("ERROR: For a 2D matrix or 3D stack input, 'metadata$whichDimIsTime' must be given to specify which dim of the input refers to time.\n");
-		return 0;
-	} 
-	if (meta->isMetaStruct==0 && io->ndim >= 2) {
-		r_error("ERROR: For a 2D matrix or 3D stack input, the 'metadata' argument must be a LIST (for R) or STRUCT (for Matlab) variable "
-			    "(e.g., metedata$period' and 'metadata$whichDimIsTime) providing additional info on the 2D or 3D input.\n");
-		return 0;
-	}
-	io->N = __GetRawTimeDimension(io);
-	return 1L;
-}
-
-
-
-int __ReadRawTime(F32PTR time, VOID_PTR timeField, const I32 Nraw) {		
-	// time should have been pre-allocated, with a length of Nraw
-
-	// TimeField is not a struct variable
-	if ( IsStruct(timeField)==0 ) {	
-
-		if (IsNumeric(timeField)==0) {
-			r_error("ERROR: metadata$time is not numeric. If times are strings, please use metadata$time$dateStr and metadata$time$strFmt to specify data observation times.\n");
-			return 0;
-		} else {
-			I32  Ntime = GetNumberOfElements(timeField);
-			if ( Ntime != Nraw ) {
-				r_error("ERROR: 'metadata$time' (%d) must be of the same length as the time dim of the input data (%d).\n", Ntime, Nraw);
-				return 0;			
-			}
-					
-			if ( IsClass(timeField, "Date")) {
-				// this branch is true only for R and Matlab's IsClass always return FALSE
-				// in R, tmp is an integer array
-				F64PTR days = GetData(timeField);
-				for (int i = 0; i < Ntime; ++i) {
-					time[i] = fractional_civil_from_days((int)days[i]);
-				}	
-				return 1L;
-			}
-			else {
-				if (CopyNumericArrToF32Arr(time, timeField, Ntime))
-					return 1L;
-				else {
-					r_error("ERROR: metadata$time has an unsupported data format or type.\n");
-					return 0;
-				}			
-			}
+static int Parse_whichDimIsTime(BEAST2_IO_PTR _OUT_ io, int Nrawtime, int userWhichDim) {
+	   // Nrawtime = 0 when TIMEObject is NULL (only start and dt are provided)
+	   // Nrawtime >1 when TIMEObjc is not NULL (metadata$time is provided)
 
+		int whichDim_final = userWhichDim;
 
-				
+		if ( io->ndim == 1 && userWhichDim != UnknownStatus && userWhichDim != 1) {
+			q_warning("WARNING: metadata$whichDimIsTime = %d is ignored because 'whichDimIsTime' is used only for 2D matrix or 3D array inputs but your input is a 1D vector.\n", userWhichDim);
+            // in this cse, io->timedim has been assigned 1 in Get_DATA
 		}
-		
-	}
+    
 
-   // TimeField is a struct variable
-	VOIDPTR yr  = GetField123Check(timeField, "year",1);
-	VOIDPTR mn  = GetField123Check(timeField, "month",1);
-	VOIDPTR day = GetField123Check(timeField, "day",3);
-	VOIDPTR doy = GetField123Check(timeField, "doy",3);
+		if (Nrawtime > 0) {
+			// TImeobjec is not NULL: We know the the length of the time dim
 
-	int isTimeProcessed = 0;
-	if (!isTimeProcessed && yr && mn && IsNumeric(yr) && IsNumeric(mn)  && GetNumberOfElements(yr)==Nraw && GetNumberOfElements(mn) == Nraw) 	{
-	
-		F32PTR yr32  = time;
-		F32PTR mn32  = malloc(sizeof(F32) *2*Nraw); // one for mn32 and another for day32
-		F32PTR day32 = mn32+Nraw;
-
-		if (!CopyNumericArrToF32Arr(yr32, yr, Nraw)) {
-			r_error("ERROR: metadata$time$year has an unsupported data format or type.\n");
-			free(mn32);
-			return 0;
-		}
-		if (!CopyNumericArrToF32Arr(mn32, mn, Nraw)) {
-			r_error("ERROR: metadata$time$month has an unsupported data format or type.\n");
-			free(mn32);
-			return 0;
-		}
- 
-		if (day && IsNumeric(day) && GetNumberOfElements(day) == Nraw) {
-		// time$day is present
-			if (!CopyNumericArrToF32Arr(day32,day, Nraw)) {
-				r_error("ERROR: metadata$time$day has an unsupported data format or type.\n");
-				free(mn32);
-				return 0;
+			int matcheNumDims = (Nrawtime == io->dims[0]) + (Nrawtime == io->dims[1]) + (Nrawtime == io->dims[2]);
+			if (matcheNumDims == 0) {
+				r_error("ERROR: The input data must have the same length as the time in metadata.\n");
+				return -1;
 			}
-			
-			for (int i = 0; i < Nraw; ++i) {
-				yr32[i] = YMDtoF32time(yr32[i], mn32[i], day32[i]);
-				if (yr32[i] < -1e9) {
-					r_error("ERROR: The (%d)-ith date (metadata$time$year=%d,metadata$time$month=%d, and metadata$time$day=%d) is not valid.\n",i+1, (int) yr32[i], (int)mn32[i], (int)day32[i] );
-					free(mn32);
-					return 0;
+			else if (matcheNumDims == 1) {
+				int  timeDimMatched;
+				if (Nrawtime == io->dims[0])  timeDimMatched = 1;
+				if (Nrawtime == io->dims[1])  timeDimMatched = 2;
+				if (Nrawtime == io->dims[2])  timeDimMatched = 3;
+				if (userWhichDim != UnknownStatus && userWhichDim != timeDimMatched) {
+					q_warning("WARNING: the specified metadata$whichDimIsTime=%d is ignored; 'whichDimIsTime=%d' is instead used based on the match between the input data and time.\n", userWhichDim, timeDimMatched);
 				}
+				whichDim_final = timeDimMatched;
 			}
-			
-		} else {
-			// time$day is not present
-			r_warning("WARNING: metadata$time$day is not specified, so only time$year and time$month are used!\n");
-
-			for (int i = 0; i < Nraw; ++i) {
-				yr32[i] = YMDtoF32time(yr32[i], mn32[i], 15);
-				if (yr32[i] < -1e9) {
-					r_error("ERROR: The (%d)-ith date (metadata$time$year=%d,and metadata$time$month=%d) is not valid.\n", i+1, (int)yr32[i], (int)mn32[i]);
-					free(mn32);
+			else { // matcheNumDims =2 or 3
+				if (userWhichDim == UnknownStatus || (io->ndim == 2 && userWhichDim != 1 && userWhichDim != 2)) {
+					r_error("ERROR: For a 2D matrix input of size [%d x %d] (i.e., multiple time series), metadata$whichDimIsTime must be given "
+						"to tell which dim of the matrix  refers to time. It must take a value out of 1 or 2 only.\n", io->dims[0], io->dims[1]);
 					return 0;
 				}
-			}			
-		}
-
-		isTimeProcessed = 1;
-		free(mn32);
-		return 1L;
-
-	}  
-
-	if (!isTimeProcessed && yr && doy && IsNumeric(yr) && IsNumeric(doy) && GetNumberOfElements(yr) == Nraw && GetNumberOfElements(doy) == Nraw)
-	{
-		F32PTR yr32  = time;
-		F32PTR doy32 = malloc(sizeof(F32) * Nraw); 
-
-		if (!CopyNumericArrToF32Arr(yr32, yr, Nraw)) {
-			r_error("ERROR: metadata$time$year has an unsupported data format or type.\n");
-			free(doy32);
-			return 0L;
-		}
-		if (!CopyNumericArrToF32Arr(doy32, doy, Nraw)) {
-			r_error("ERROR: metadata$time$doy has an unsupported data format or type.\n");
-			free(doy32);
-			return 0L;
-		}
- 
-		for (int i = 0; i < Nraw; ++i) {
-			yr32[i] = YDOYtoF32time(yr32[i], doy32[i] );
-			if (yr32[i] < -1e9) {
-				r_error("ERROR: The (%d)-ith date (metadata$time$year=%d,and metadata$time$doy=%d) is not valid.\n", i + 1, (int)yr32[i], (int)doy32[i] );
-				free(doy32);
-				return 0;
-			}
-		}
-
-		isTimeProcessed = 1;
-		free(doy32);
-		return 1L;
-	}
-
-
-	VOIDPTR datestr = GetField123Check(timeField, "dateStr",3);
-	VOIDPTR strfmt  = GetField123Check(timeField, "strFmt",3); 
-	if (!isTimeProcessed && datestr && strfmt && IsChar(datestr) && IsChar(strfmt) && GetNumberOfElements(datestr)==Nraw ) 	{		
-
-		char STRFmt[255 + 1];
-		GetCharArray(strfmt, STRFmt, 255);
-		
-		DateFmtPattern1 fmt1;	
-		if (GetStrPattern_fmt1(STRFmt, &fmt1)) {
-			
-			for (int i = 0; i < Nraw; ++i) {	
-				char TMP[255 + 1];
-				if (!GetCharVecElem(datestr, i, TMP, 255)) {
-					r_error("ERROR: Unable to read the %d-ith date string from metadata$time$dateStr.\n", i + 1);
-					return 0L;
-				}
-				time[i] = Str2F32time_fmt1(TMP, &fmt1);
-				if (time[i] < -1e9) {
-					r_error("ERROR: The %d-th string ($metadata$time$dateStr=\"%s\") is invalid, incompatiable with the specified "
-							" metadata$time$strFmat=\"%s\".\n", i + 1, TMP, STRFmt);
-					return 0L;
-				}
-			}	
-		}
-	 
-		DateFmtPattern2 fmt2;	
-		if (GetStrPattern_fmt2(STRFmt, &fmt2)) {
-			
-			for (int i = 0; i < Nraw; ++i) {	
-				char TMP[255 + 1];
-				if (!GetCharVecElem(datestr, i, TMP, 255)) {
-					r_error("ERROR: Unable to read the %d-ith date string from metadata$time$dateStr.\n", i + 1);
-					return 0L;
+				if (userWhichDim == UnknownStatus || (io->ndim == 3 && userWhichDim != 1 && userWhichDim != 2 && userWhichDim != 3)) {
+					r_error("ERROR: For a 3D array input of size [%d x %d x %d] (i.e., stacked time series images), metadata$whichDimIsTime must be given "
+						"to tell which dim of the 3D array  refers to time. It must take a value out of 1, 2 or 3 only.\n", io->dims[0], io->dims[1], io->dims[2]);
+					return 0;
 				}
-				time[i] = Str2F32time_fmt2(TMP, &fmt2);
-				if (time[i] < -1e9) {
-					r_error("ERROR: The %d-th string (metadata$time$dateStr=\"%s\") is invalid, incompatiable with the specified "
-							" metadata$time$strFmat=\"%s\".\n", i + 1, TMP, STRFmt);
-					return 0L;
+				if (io->dims[userWhichDim] != Nrawtime) {
+					r_error("ERROR: The length of the time dimension of the input (whichDimIsTime=%d) doesn't match the length of time/metadata$time (i.e., %d!=%d).\n", userWhichDim, io->dims[userWhichDim], Nrawtime);
+					return 0;
 				}
-			}	
-		}
-
+				whichDim_final = userWhichDim;
+			}
+		}	
+		else {
+		// Nraw=0
 
-		DateFmtPattern3 fmt3;	
-		if (GetStrPattern_fmt3(STRFmt, &fmt3)) {
-			
-			for (int i = 0; i < Nraw; ++i) {	
-				char TMP[255 + 1];
-				if (!GetCharVecElem(datestr, i, TMP, 255)) {
-					r_error("ERROR: Unable to read the %d-ith date string from metadata$time$dateStr.\n", i + 1);
-					return 0L;
+			if (io->timedim == UnknownStatus) {
+				// io->timedim has been determined for 1D signals; this branch is only for 2D or 3D data 
+				if (userWhichDim == UnknownStatus || (io->ndim == 2 && userWhichDim != 1 && userWhichDim != 2)) {
+					r_error("ERROR: For a 2D matrix input of size [%d x %d] (e.g., multiple time series), metadata$whichDimIsTime must be given "
+						"to tell which matrix dim refers to time. It must take a value out of 1 or 2 only.\n", io->dims[0], io->dims[1]);
+					return 0;
 				}
-				time[i] = Str2F32time_fmt3(TMP, &fmt3);
-				if (time[i] < -1e9) {
-					r_error("ERROR: The %d-th string ($metadata$time$dateStr=\"%s\") is invalid, incompatiable with the specified "
-							" metadata$time$strFmat=\"%s\".\n", i + 1, TMP, STRFmt);
-					return 0L;
+				if (userWhichDim == UnknownStatus || (io->ndim == 3 && userWhichDim != 1 && userWhichDim != 2 && userWhichDim != 3)) {
+					r_error("ERROR: For a 3D array input of size [%d x %d x %d] (i.e., stacked time series images), metadata$whichDimIsTime must be given "
+						"to tell which aray dim refers to time. It must take a value out of 1, 2 or 3 only.\n", io->dims[0], io->dims[1], io->dims[2]);
+					return 0;
 				}
-			}	
-		}
-		return 1L;
-
-	}
-	 
-
-	return 0L;
-}
-static int  ___PraseMetaData_IrregularTS_Dim123(BEAST2_METADATA_PTR meta, BEAST2_IO_PTR io) {
-	// If the input time series data are irregular
-	if (meta->nrhs < 3 || meta->isMetaStruct==0) {
-		r_printf("ERROR: For irregular time series (i.e., metadata$isRegularOdered=FALSE), the argument 'metadata' must be supplied and it should be a LIST (for R) or struct (for Matlab) variable!");
-		return 0;
-	}
-	if (meta->rawTimeVec == NULL) {
-		r_printf("ERROR: For irregular time series (i.e., metadata$isRegularOdered=FALSE), metadata$time must be given to "
-			     "specify the times at which data points are collected.");
-		return 0;
-	}
-
-	/************************************************************/
-	// REad the raw time and gather the info needed for aggragration
-	/************************************************************/
-	I32    Nraw = __GetRawTimeDimension(io);
-	F32PTR time = malloc(sizeof(F32) * Nraw);	
-	// Nraw must is the same as the length of rawTimeVec, to be checked in __ReadRawTime		
-	if (__ReadRawTime(time, meta->rawTimeVec, Nraw)) {
-		F32  dT = meta->deltaTime;
-		io->N   = tsAggegrationPrepare(
-					time, Nraw, dT, &io->T.sortedTimeIdx, &io->T.numPtsPerInterval,
-					&io->T.startIdxOfFirsInterval, &meta->startTime
-				); // meta->stattTime may be adjustd slightly to better match the real start of the time series
-		free(time);
-	} else {
-		free(time);
-		r_error("ERROR: Unable to read and intepret 'metadata$time'!\n");
-		return 0;
-	}
-
-	// Npad:N_extended; the mutiples of 8 closest to N, defined for 32-byte alginment	
-	//opt->Npad16 = (N+15)/16 *16;   //(I32)ceil((F32)N / 16.f) * 16;
-	return 1L;
-}
-static int ParseInputData( BEAST2_IO_PTR _OUT_ io){
-
-		// Check if the input 'data' is numeric and lengthy enough
-		VOIDPTR DATA  =	 io->meta.rawInput;
-		int     numel =  GetNumberOfElements(DATA);
-		if (!(IsDouble(DATA) && numel > 2) && 	!(IsSingle(DATA) && numel > 2) &&
-			!(IsInt32(DATA)  && numel > 2) &&	!(IsInt16(DATA) && numel > 2) &&
-			!(IsInt64(DATA) && numel > 2)  && !(IsStruct(DATA) && numel >= 1 ) &&
-			!(IsCell(DATA) ) /*Only true for Matlab*/      // Y=rawInput is a struct variable with multivariate time series
-		   ) {   
-			r_error("ERROR: The input data should be numeric and must be long enough.\n");
-			return 0;
-		}
-
-		/*************************************************/
-		/* If pY is not a string but a matrix or vector  */
-		/* find the dimesions, and configure io-*/
-		/*************************************************/
-		I32       q;
-		VOID_PTR  Y;
-		if ( (IsStruct(DATA) && numel >= 1) || IsCell(DATA)) {
-			// For MRBEAST only
-			// rawInput is a struct variable with multivariate time series						
-			q = numel;
-
-			//Mem to be dellocated in DeallocatTimeSeriesIO
-			io->pdata = malloc(sizeof(VOID_PTR) * q);
-			io->dtype = malloc(sizeof(DATA_TYPE) * q);
-			//TODO: For MRBEAST, here the data type an dimensions of all elments are assumed to be the same
-			// A sanity check needs to be done to ensure that is the case.
-			for (I32 i = 0; i < q; i++) {
-				 Y           = GetFieldByIdx(DATA, i);
-				io->pdata[i] = GetData(Y);
-				io->dtype[i] = GetDataType(Y);
-			}		
-			//Aded for MRBEAST
-			
-		} else {
-		    //rawIinput is a vector of numeric type, and not a struct variable with multivariate time series			
-			q = 1;
-			//Mem to be dellocated in DeallocatTimeSeriesIO
-			io->pdata    = malloc(sizeof(VOID_PTR) * q);
-			io->dtype    = malloc(sizeof(DATA_TYPE) * q);
-			io->pdata[0] = GetData(DATA);
-			io->dtype[0] = GetDataType(DATA);
-			Y = DATA;
-		}				
-		for (I32 i = 0; i < q; i++) {
-			if (io->dtype[i] == DATA_UNKNOWN) {
-				r_error("ERROR: The input data has an uknown numeric type!\n");
-				return 0;
+				whichDim_final = userWhichDim;
+			}	else {
+				// it can be only 1
+				whichDim_final = io->timedim;
 			}
+		
 		}
-		io->q = q;
-		/*************************************************/
-		/* Get the dimension of the input              */		
-		/*************************************************/
-		I32 ndims = GetNumOfDim(Y);
-		if (ndims == 0) {
-			// the input is a vector: this branch is possible only for R vectors (not  Matlab)
-			I32 N = GetNumberOfElements(Y);
-
-			io->numOfPixels = 1L;
-			io->ndim		= 1L;
-			io->dims[0]		= N;
-			io->dims[1]		= 1L;
-			
-			if (io->meta.whichDimIsTime != -1) 
-				r_warning("WARNING: metadata$whichDimIsTime=%d is ignored because 'whichDimIsTime' is used only if the input "
-					      "is a 2D matrix or 3D array but your input is a 1D vector.\n", io->meta.whichDimIsTime);
-
-			//TODO: always set it to 1 for 1D and 2D inputs
-			// If hte input is a vector, the time dim is always 1
-			io->meta.whichDimIsTime = 1L;
-		} 
-		else if (ndims == 1) {
-			// the input is a vector: this branch is possible only for Python vectors (not R or matlab)
-			I32 N = GetNumberOfElements(Y);
-
-			io->numOfPixels = 1L;
-			io->ndim     = 1L;
-			io->dims[0]  = N;
-			io->dims[1]  = 1L;
-
-			if (io->meta.whichDimIsTime != -1)
-				r_warning("WARNING: metadata$whichDimIsTime=%d is ignored because 'whichDimIsTime' is used only if the input "
-					"is a 2D matrix or 3D array but your input is a 1D vector.\n", io->meta.whichDimIsTime);
-
-			//TODO: always set it to 1 for 1D and 2D inputs
-			// If hte input is a vector, the time dim is always 1
-			io->meta.whichDimIsTime = 1L;
-		}
-		//ndims is impossible to be 1L
-		else if (ndims == 2) { 
-		// Matlab: a vector or matrix;
-		// R:      a matrix or a vector with a dim attribute.
 
-			int N = GetDim1(Y);
-			int M = GetDim2(Y);
-
-			if (min(N, M) == 1L)  //PY is a vector
-			{
-				N = max(N, M),
-				io->numOfPixels = 1,
-				io->ndim      = 1L,
-				io->dims[0]   = N,
-				io->dims[1]   = 1L,
-				io->meta.whichDimIsTime = 1L;
-
-				// If hte input is a vector, the time dim is always 1
-				if (io->meta.whichDimIsTime != -1)
-					r_warning("WARNING: metadata$whichDimIsTime=%d is ignored because 'whichDimIsTime' is used only if the input "
-						"is a 2D matrix or 3D array but your input is a 1D vector.\n", io->meta.whichDimIsTime);
-			}
-			else                 //PY is a matrix
-			{
-				io->ndim	= 2L,
-				io->dims[0] = N,
-				io->dims[1] = M;
+		io->timedim = io->meta.whichDimIsTime = whichDim_final;
 
+		if (io->meta.whichDimIsTime == 1) { io->rowdim = 2, io->coldim = 3, io->timedim = 1; }
+		if (io->meta.whichDimIsTime == 2) { io->rowdim = 1, io->coldim = 3, io->timedim = 2; }
+		if (io->meta.whichDimIsTime == 3) { io->rowdim = 1, io->coldim = 2, io->timedim = 3; }
+
+		io->imgdims[0]  = io->dims[io->rowdim - 1];
+		io->imgdims[1]  = io->dims[io->coldim - 1];
+		io->numOfPixels = (I64)io->dims[0] * io->dims[1] * io->dims[2] / io->dims[io->timedim - 1L];
 
-				I32 whichDimIsTime = io->meta.whichDimIsTime;
-				if (whichDimIsTime == -1 || (whichDimIsTime != 1 && whichDimIsTime != 2 )) {
-					r_error("ERROR: For a 2D matrix input of size [%d x %d] (i.e., multiple time series), metadata$whichDimIsTime must be given "
-						    "to tell which dim of the matrix  refers to time. It must take a value out of 1 or 2 only.\n", N, M);
-					return 0;
-				}
-
-				io->numOfPixels = (I64)io->dims[0] * io->dims[1]  / io->dims[io->meta.whichDimIsTime - 1L];
-			}//PY is a matrix
-
-			
-		}
-		else if (ndims == 3) {
-			// If the input is a 3D array
-			io->ndim = 3L;
-			GetDimensions(Y, io->dims, 3L);
-
-			I32 whichDimIsTime = io->meta.whichDimIsTime;
-			if (whichDimIsTime == -1 ||	(whichDimIsTime!=1 && whichDimIsTime!=2 && whichDimIsTime!=3 )  ) {
-				r_error("ERROR: For a 3D array input of size [%d x %d x %d] (i.e., stacked time series images), metadata$whichDimIsTime must be given "
-					     "to tell which dim of the 3D array  refers to time. It must take a value out of 1, 2 or 3 only.\n", 
-					     io->dims[0], io->dims[1], io->dims[2]);
-				return 0;	}
-
-			io->numOfPixels = (I64)io->dims[0] * io->dims[1] * io->dims[2] / io->dims[io->meta.whichDimIsTime - 1L];
-		}
-		else {
-			r_printf("ERROR: The maximum dimension allowed is 3 when the data is a 3D stack of images over time,"
-				    " but the input data has a dimension of %d .\n", ndims);
-			return 0;
-		}
-
-	
+		//int N = io->dims[io->timedim - 1L];
+		return whichDim_final;		
+}
 
+ static float ParsePeriod(BEAST2_IO_PTR _OUT_ io ) {
+		
 		/*************************************************/
-		// Check and get the values for period, startTime, deltaTime
-		// or period_in_time
+		// There is a seasonal componet, and we need to check and get period	 
 		/*************************************************/
-		int res = io->meta.isRegularOrdered? ___PraseMetaData_RegularTS_Dim123(  &io->meta, io):
-											 ___PraseMetaData_IrregularTS_Dim123(&io->meta, io); //set io->N
-		if (res == 0)
-			return 0;
-
-		// Period is not needed for trend-only data
-		// or if there is a season compnt and the period is already a valid value
-		if ( !io->meta.hasSeasonCmpnt   || io->meta.period > 0)
-			return 1;
+		//if ( io->meta.hasSeasonCmpnt==0 ||    // Period is not needed for trend-only data
+		//	 io->meta.period        > 0    )  // or if there is a season compnt and the period is already a valid value			 
 
-
-		// There is a seasonal componet, and we need to check and get period	 
 		/*************************************************/
 		//  if period<=0 or IsNan(period)
 		//  Determine the period perameter via auto-correlation
 		/*************************************************/
-		BEAST2_YINFO yInfo;
+		BEAST2_YINFO Yinfo;
 		F32PTR       MEMBUF;
-		I32   N    = io->N;
-		I32   Nraw = __GetRawTimeDimension(io);
-		F32PTR tmp = malloc(sizeof(F32)*(N*q +N+q +q +q*q +Nraw )); //alocate mem for yInfo and MEMBUF
-
-		yInfo.Y               = tmp;
-		yInfo.rowsMissing     = tmp+N*q;
-		yInfo.mean            = tmp + N * q+N;
-		yInfo.sd                = tmp + N * q +N+q;
-		yInfo.YtY_plus_alpha2Q  = tmp + N * q +N+q+q;
+		int    N    = io->N;		
+		int    q    = io->q;
+		int    Nraw = io->dims[io->timedim - 1];
+		F32PTR tmp  = malloc(sizeof(F32)*(N*q +N+q +q +q*q +Nraw )); //alocate mem for yInfo and MEMBUF
+
+		Yinfo.Y                 = tmp;
+		Yinfo.rowsMissing       = tmp+N*q;
+		Yinfo.mean              = tmp + N * q+N;
+		Yinfo.sd                = tmp + N * q +N+q;
+		Yinfo.YtY_plus_alpha2Q  = tmp + N * q +N+q+q;
 		MEMBUF                  = tmp + N * q +N+q+q+q*q; //needed only for irregular time series
 
-		F32 period              = -1;
 		F32 nan                 = getNaN();
+		F32 period              = nan;
 		I32 goodPixelVisited    = 0;
 		I32 MaxNumPixelVisisted = 200;
-
 		// THe pixel index is 1-based and not zero-based
 		for (int i = 1; i <= io->numOfPixels; ++i) {
 
-			BEAST2_fetch_next_timeSeries(&yInfo, i, MEMBUF, io);
-			// yInfo has been fillted above and now compaute mean, std, and YtY			
-			int    N = io->N;
-			int    q = io->q;
-			//Normalize Y with NaN ommitted and then pre-comoute Y'*Y: YtY_plus_Q using gemm
-			yInfo.nMissing = f32_normalize_multicols_zeroout_nans(yInfo.Y, yInfo.rowsMissing, N, N, q, yInfo.mean, yInfo.sd);
-			U08 skipCurrentPixel = yInfo.nMissing > (N * io->meta.maxMissingRate) ? 1 : 0;
+			BEAST2_fetch_timeSeries(&Yinfo, i, MEMBUF, io);
+			// yInfo has been fillted above and now compaute mean, std, and YtY						
+			// Normalize Y with NaN ommitted and then pre-comoute Y'*Y: YtY_plus_Q using gemm
+			Yinfo.nMissing = f32_normalize_multicols_zeroout_nans(Yinfo.Y, Yinfo.rowsMissing, N, N, q, Yinfo.mean, Yinfo.sd);
+
+			U08 skipCurrentPixel = Yinfo.nMissing > (N * io->meta.maxMissingRate);
 			if (skipCurrentPixel) {
 				continue;
-			}
-		
+			}		
 			
 			for (int j = 0; j < q; ++j) {
-				F32PTR y = yInfo.Y + j * N;
-				for (int k = 0; k < yInfo.nMissing; ++k) {y[yInfo.rowsMissing[k]] = nan;}
 
-				F32 curPeriod = DeterminePeriod(y, N);  // return -1 if failing to estimate the period
-				if (j == 0){ //if it is the 1st out of the q time series				
-					period = curPeriod;
-					if (period < 0) {
-						break;
-					}
+				F32PTR y = Yinfo.Y + j * N;
+				for (int k = 0; k < Yinfo.nMissing; ++k) {
+					y[Yinfo.rowsMissing[k]] = nan;
+				}
+
+				F32 jthPeriod = DeterminePeriod(y, N);  // return -1 if failing to estimate the period
+				if (j == 0) { 
+					//if it is the 1st out of the q time series	
+					period = jthPeriod;
+					if (period < 0)	break;					
 				} else {
-					if (period != curPeriod) {
+					if (jthPeriod != period ) {
 						//if a later time series dones't give the same period as the first one
-						period = -1;
+						period = nan;
 						break;
 					}
 				}
 			}
 
-			if (period > 0) {
-				break;
-			}
-
-			if (++goodPixelVisited > MaxNumPixelVisisted)
-				break;
+			if (period > 0   )                           	break;
+			if (++goodPixelVisited > MaxNumPixelVisisted) 	break;
 		}
 		free(tmp);
-		
-
-		if (period > 0) {
-			r_warning("WARNING: When metadata$season='%s' (i.e., the time series has a periodic component), \"metadata$period\" "
-				"MUST be known in advance and specified by the user but it is missing. A BEST GUESS of it is %f (period=freq*deltaTime=%d*%f) and "
-				"will be used. Please make sure this estimate makes sense; otherwise, the BEAST decomposition result will be incorrect.\n",
-				io->meta.seasonForm == 'S' ? "harmonic" : "dummy", period* io->meta.deltaTime, (int)period, io->meta.deltaTime);
-		} else {
-			r_error("ERROR: When metadata$season='%s' (i.e., a periodic component present in the input time series), the \"metadata$period\" parameter "
-				"must be known in advance and specified by the user but it is missing. BEAST tried to estimate it via an auotcorrelation method but failed to "
-				"get a reliable estimate. Please specify the value for metadata$period EXPLICILTY. Or if your input has no periodic component at all, "
-				" set  metadata$season='none', which will fit a trend-only model.\n", io->meta.seasonForm == 'S' ? "harmonic" : "dummy");
-			return 0;
-		}
-
-		io->meta.period = period;
-		return 1;
-
+ 
+	return period;
 }
 
 static int __GetPrecPriorType( VOID_PTR S ) {
 
 	VOID_PTR  tmp = GetField123Check(S, "precPriorType",5);
 	
 	if (tmp == NULL)
@@ -785,33 +648,33 @@
 	if (IsNumeric(tmp)) {
 		I32 value = GetScalar(tmp);
 		if (value == 0) return ConstPrec;
 		if (value == 1) return UniformPrec;
 		if (value == 2) return ComponentWise;
 		if (value == 3) return OrderWise;
 
-		r_warning("WARNING: The arg prior$precPriorType=(%d) is not a valid value; the default prior$precPriorType='%s' is assumed instread!", value, "uniform");
+		q_warning("WARNING: The arg prior$precPriorType=(%d) is not a valid value; the default prior$precPriorType='%s' is assumed instread!", value, "uniform");
 		return UniformPrec;
 	} 
 	else if (IsChar(tmp)) {
 		char str[60+1];
 		GetCharArray(tmp,str, 60);
 		ToUpper(str);
 		char a = str[0];
 		char c = str[2];
 		if (a =='U')				return UniformPrec;
 		if (a == 'O')				return OrderWise;
 		if (a == 'C' && c == 'M')	return ComponentWise;
 		if (a == 'C' && c == 'N')	return ConstPrec;	
 
-		r_warning("WARNING: The arg prior$precPriorType=(%s) is not recongizable; the default prior$precPriorType='%s' is assumed instread!", str, "uniform");
+		q_warning("WARNING: The arg prior$precPriorType=(%s) is not recongizable; the default prior$precPriorType='%s' is assumed instread!", str, "uniform");
 		return UniformPrec;
 	}
 	
-	r_warning("WARNING: The arg prior$precPriorType has an supported format or value; the default prior$precPriorType='%s' is assumed instread!",  "uniform");
+	q_warning("WARNING: The arg prior$precPriorType has an supported format or value; the default prior$precPriorType='%s' is assumed instread!",  "uniform");
 	return UniformPrec;
 }
 
 static int  GetArg_2nd_Prior__(VOIDPTR prhs[], int nrhs, BEAST2_PRIOR_PTR prior, BEAST2_IO_PTR io)
 {	 
 	// Before running this fuction,  period and N must have been determined
 
@@ -841,95 +704,105 @@
 
 	if (nrhs < 4) 	
 		memset(&m, 1L, sizeof(struct PRIOR_MISSING));
 
 	if (nrhs >= 4) {		 
 		VOIDPTR S = prhs[3L];
 		if (!IsStruct(S)) {
-			r_warning("WARNING: The arg 'prior' is ignored because it is not a List/Struct variable.");
+			q_warning("WARNING: The arg 'prior' is ignored because it is not a List/Struct variable.");
 			memset(&m, 1L, sizeof(struct PRIOR_MISSING));
 		}
 		else {
 			VOIDPTR tmp;
-			o.seasonMinOrder    = (tmp = GetField123Check(S, "seasonMinOrder",10)) ?    GetScalar(tmp) : (m.seasonMinOrder = 1);
-			o.seasonMaxOrder    = (tmp = GetField123Check(S, "seasonMaxOrder", 10)) ?   GetScalar(tmp) : (m.seasonMaxOrder = 1);
-			o.trendMinOrder     = (tmp = GetField123Check(S, "trendMinOrder", 10)) ?    GetScalar(tmp) : (m.trendMinOrder = 1);
-			o.trendMaxOrder     = (tmp = GetField123Check(S, "trendMaxOrder", 10)) ?    GetScalar(tmp) : (m.trendMaxOrder = 1);
+			if (io->meta.hasSeasonCmpnt) {
+				o.seasonMinOrder = (tmp = GetField123Check(S, "seasonMinOrder", 10)) ? GetScalar(tmp) : (m.seasonMinOrder = 1);
+				o.seasonMaxOrder = (tmp = GetField123Check(S, "seasonMaxOrder", 10)) ? GetScalar(tmp) : (m.seasonMaxOrder = 1);
+				o.seasonMinSepDist = (tmp = GetField123Check(S, "seasonMinSepDist", 10)) ? GetScalar(tmp) : (m.seasonMinSepDist = 1);
+				o.seasonMinKnotNum = (tmp = GetField123Check(S, "seasonMinKnotNum", 10)) ? GetScalar(tmp) : (m.seasonMinKnotNum = 1);
+				o.seasonMaxKnotNum = (tmp = GetField123Check(S, "seasonMaxKnotNum", 10)) ? GetScalar(tmp) : (m.seasonMaxKnotNum = 1);
+			}
+
+			o.trendMinOrder     = (tmp = GetField123Check(S, "trendMinOrder",  10)) ?   GetScalar(tmp) : (m.trendMinOrder = 1);
+			o.trendMaxOrder     = (tmp = GetField123Check(S, "trendMaxOrder",  10)) ?   GetScalar(tmp) : (m.trendMaxOrder = 1);
 			o.trendMinSepDist   = (tmp = GetField123Check(S, "trendMinSepDist", 10)) ?  GetScalar(tmp) : (m.trendMinSepDist = 1);
-			o.seasonMinSepDist  = (tmp = GetField123Check(S, "seasonMinSepDist", 10)) ? GetScalar(tmp) : (m.seasonMinSepDist = 1);
-			o.trendMinKnotNum   = (tmp = GetField123Check(S, "trendMinKnotNum", 10)) ?  GetScalar(tmp) : (m.trendMinKnotNum = 1);
-			o.seasonMinKnotNum  = (tmp = GetField123Check(S, "seasonMinKnotNum", 10)) ? GetScalar(tmp) : (m.seasonMinKnotNum = 1);
+			o.trendMinKnotNum   = (tmp = GetField123Check(S, "trendMinKnotNum", 10)) ?  GetScalar(tmp) : (m.trendMinKnotNum = 1);			
 			o.trendMaxKnotNum   = (tmp = GetField123Check(S, "trendMaxKnotNum", 10)) ?  GetScalar(tmp) : (m.trendMaxKnotNum = 1);
-			o.seasonMaxKnotNum  = (tmp = GetField123Check(S, "seasonMaxKnotNum", 10)) ? GetScalar(tmp) : (m.seasonMaxKnotNum = 1);
-			o.outlierMaxKnotNum = (tmp = GetField123Check(S, "outlierMaxKnotNum", 10))? GetScalar(tmp) : (m.outlierMaxKnotNum = 1);
-			o.K_MAX             = (tmp = GetField123Check(S, "K_MAX",1)) ?			GetScalar(tmp) : (m.K_MAX = 1);
+			
+			if (io->meta.hasOutlierCmpnt) {
+				o.outlierMaxKnotNum = (tmp = GetField123Check(S, "outlierMaxKnotNum", 10)) ? GetScalar(tmp) : (m.outlierMaxKnotNum = 1);
+				o.outlierSigFactor = (tmp = GetFieldCheck(S, "outlierSigFactor")) ? GetScalar(tmp) : (m.outlierSigFactor = 1);
+			}
 
 			o.sigFactor         = (tmp = GetFieldCheck(S,  "sigFactor")) ?			GetScalar(tmp) : (m.sigFactor        = 1);
-			o.outlierSigFactor  = (tmp = GetFieldCheck(S,  "outlierSigFactor")) ?	GetScalar(tmp) : (m.outlierSigFactor = 1);
 
 			o.sig2              = (tmp = GetField123Check(S, "sig2",2)) ?				GetScalar(tmp) : (m.sig2 = 1);
 			o.precValue		    = (tmp = GetField123Check(S, "precValue",5)) ?		GetScalar(tmp) : (m.precValue = 1);
 			o.alpha1			= (tmp = GetField123Check(S, "alpha1",0)) ?			GetScalar(tmp) : (m.alpha1 = 1);
 			o.alpha2			= (tmp = GetField123Check(S, "alpha2",0)) ?			GetScalar(tmp) : (m.alpha2 = 1);
 			o.delta1			= (tmp = GetField123Check(S, "delta1",0)) ?			GetScalar(tmp) : (m.delta1 = 1);
 			o.delta2			= (tmp = GetField123Check(S, "delta2",0)) ?			GetScalar(tmp) : (m.delta2 = 1);
 
-		
-			o.seasonBasisFuncType	= (tmp = GetField123Check(S, "seasonBasisFuncType",10)) ?  GetScalar(tmp) : (m.seasonBasisFuncType = 1);
-			o.trendBasisFuncType	= (tmp = GetField123Check(S, "trendBasisFuncType", 10)) ?   GetScalar(tmp) : (m.trendBasisFuncType = 1);
-			o.outlierBasisFuncType	= (tmp = GetField123Check(S, "outlierBasisFuncType", 10)) ? GetScalar(tmp) : (m.outlierBasisFuncType = 1);
+			o.K_MAX = (tmp = GetField123Check(S, "K_MAX", 1)) ? GetScalar(tmp) : (m.K_MAX = 1);
+
+			if (io->meta.hasSeasonCmpnt)  o.seasonBasisFuncType	  = (tmp = GetField123Check(S, "seasonBasisFuncType",10)) ?  GetScalar(tmp) : (m.seasonBasisFuncType = 1);
+			if (1L)                       o.trendBasisFuncType	  = (tmp = GetField123Check(S, "trendBasisFuncType", 10)) ?   GetScalar(tmp) : (m.trendBasisFuncType = 1);
+			if (io->meta.hasOutlierCmpnt) o.outlierBasisFuncType  = (tmp = GetField123Check(S, "outlierBasisFuncType", 10)) ? GetScalar(tmp) : (m.outlierBasisFuncType = 1);
 			o.modelPriorType		= (tmp = GetField123Check(S, "modelPriorType",  10)) ?		GetScalar(tmp) : (m.modelPriorType = 1);
 			
 			//o.precPriorType		    = (tmp = GetFieldCheck(S, "precPriorType")) ?	    GetScalar(tmp) : (m.precPriorType = 1);
 			o.precPriorType = __GetPrecPriorType(S);
 
 		
 		}
 
 	} // if (nrhs >= 4)
 
 	o.numBasis       = 1L + io->meta.hasSeasonCmpnt + io->meta.hasOutlierCmpnt;
 	I32  basisIdx    = 0;	
 	if (io->meta.hasSeasonCmpnt) {
-		I08  seasonFrom = io->meta.seasonForm;
+		I08      seasonFrom = io->meta.seasonForm;
 		if      (seasonFrom == 'S')	o.basisType[basisIdx++] = SEASONID;
 		else if (seasonFrom == 'D') o.basisType[basisIdx++] = DUMMYID;
 		else if (seasonFrom == 'V') o.basisType[basisIdx++] = SVDID;
 		else {
-			r_error("ERROR: the seasonform character is unrecognized. It must be one of 'S', 'D', or 'V'. \n");
+			r_error("ERROR: the season character is unrecognized. Valid values are 'none', 'harmonic', 'dummy', and 'svd'. \n");
 			return 0;
 		}
 	}
 	o.basisType[basisIdx++] = TRENDID;
 	if (io->meta.hasOutlierCmpnt) o.basisType[basisIdx++] = OUTLIERID;
 		
 	/**************************/
 	//Put here because the following setup need the values of period and N (time-series length).
 	//These two values have been determined in ParseInputData. 
 	I32 period = io->meta.period;
 	I32 N      = io->N;
 	/**************************/
 
-	if (m.seasonMinOrder)    o.seasonMinOrder   = 1L;				   o.seasonMinOrder   = min(o.seasonMinOrder, period / 2 - 1);    o.seasonMinOrder = max(o.seasonMinOrder, 1L);
-	if (m.seasonMaxOrder)    o.seasonMaxOrder   = (period/2 - 1);      o.seasonMaxOrder   = min(o.seasonMaxOrder, (period / 2 - 1));  o.seasonMaxOrder = max(o.seasonMaxOrder, o.seasonMinOrder);
-	if (m.trendMinOrder)     o.trendMinOrder    = 0L;				   o.trendMinOrder	  = max(o.trendMinOrder, 0L);
-	if (m.trendMaxOrder)     o.trendMaxOrder    = 1L;				   o.trendMaxOrder	  = max(o.trendMaxOrder, o.trendMinOrder);
-	if (m.seasonMinSepDist || o.seasonMinSepDist == 0)				   o.seasonMinSepDist = period / 2;       o.seasonMinSepDist = max(o.seasonMinSepDist, o.seasonMaxOrder);		 o.seasonMinSepDist = min(o.seasonMinSepDist, N / 2 - 1); // TODO:N/2-1 can be negtative, and then forced into a lager postive U16 integer
-	
-	if (m.trendMinSepDist || o.trendMinSepDist == 0)   o.trendMinSepDist = io->meta.hasSeasonCmpnt? period / 2: 3 ;
-	o.trendMinSepDist = max(o.trendMinSepDist, (o.trendMaxOrder+1));
-	o.trendMinSepDist = min(o.trendMinSepDist, N / 2 - 1);
-	
-	
-	if (m.seasonMinKnotNum)  o.seasonMinKnotNum = 0;                   o.seasonMinKnotNum = max(min(o.seasonMaxKnotNum, o.seasonMinKnotNum), 0);
-	if (m.trendMinKnotNum)   o.trendMinKnotNum  = 0;	               o.trendMinKnotNum  = max( min(o.trendMaxKnotNum,  o.trendMinKnotNum),0);
+	if (io->meta.hasSeasonCmpnt) {
+		if (io->meta.seasonForm == 'S') {
+			if (m.seasonMinOrder)      o.seasonMinOrder = 1L;				   o.seasonMinOrder = min(o.seasonMinOrder, period / 2 - 1);    o.seasonMinOrder = max(o.seasonMinOrder, 1L);
+			if (m.seasonMaxOrder)      o.seasonMaxOrder = (period / 2 - 1);    o.seasonMaxOrder = min(o.seasonMaxOrder, (period / 2 - 1));  o.seasonMaxOrder = max(o.seasonMaxOrder, o.seasonMinOrder);
+		}	else if (io->meta.seasonForm == 'V') {
+			if (m.seasonMinOrder)      o.seasonMinOrder = 1L;				   o.seasonMinOrder = min(o.seasonMinOrder, period - 1);   o.seasonMinOrder = max(o.seasonMinOrder, 1L);
+			if (m.seasonMaxOrder)      o.seasonMaxOrder = (period / 2 - 1);    o.seasonMaxOrder = min(o.seasonMaxOrder, period );  o.seasonMaxOrder = max(o.seasonMaxOrder, o.seasonMinOrder);
+		}
+		
+		if (m.seasonMinSepDist || o.seasonMinSepDist <= 0)   o.seasonMinSepDist = period / 2;          o.seasonMinSepDist = max(o.seasonMinSepDist, o.seasonMaxOrder);		 o.seasonMinSepDist = min(o.seasonMinSepDist, N / 2 - 1); // TODO:N/2-1 can be negtative, and then forced into a lager postive U16 integer
+		if (m.seasonMinKnotNum)                              o.seasonMinKnotNum = 0;                   o.seasonMinKnotNum = max(min(o.seasonMaxKnotNum, o.seasonMinKnotNum), 0);
+		if (m.seasonMaxKnotNum)                              o.seasonMaxKnotNum = min(floor(N / (o.seasonMinSepDist + 1) - 1.f), 5);  o.seasonMaxKnotNum = min(o.seasonMaxKnotNum, floor(N / (o.seasonMinSepDist + 1) - 1.f));   o.seasonMaxKnotNum = max(o.seasonMaxKnotNum, o.seasonMinKnotNum);
+	}
 	
-	if (m.seasonMaxKnotNum)  o.seasonMaxKnotNum  = min(floor(N / (o.seasonMinSepDist + 1) - 1.f), 5);  o.seasonMaxKnotNum = min(o.seasonMaxKnotNum, floor(N / (o.seasonMinSepDist + 1) - 1.f));
-	if (m.trendMaxKnotNum)   o.trendMaxKnotNum   = min( floor(N/(o.trendMinSepDist  + 1) - 1.f),  10); o.trendMaxKnotNum  = min(o.trendMaxKnotNum,  floor(N / (o.trendMinSepDist + 1) - 1.f));	
-	if (m.outlierMaxKnotNum) o.outlierMaxKnotNum = o.trendMaxKnotNum;                                  o.outlierMaxKnotNum = max(o.outlierMaxKnotNum, 1L); // at least has one; otherwise, the program crahses if hasOUtliercomponet=1
+	if (m.trendMinOrder)                             o.trendMinOrder    = 0L;				                      o.trendMinOrder	  = max(o.trendMinOrder, 0L);
+	if (m.trendMaxOrder)                             o.trendMaxOrder    = 1L;				                      o.trendMaxOrder	  = max(o.trendMaxOrder, o.trendMinOrder);	
+	if (m.trendMinSepDist || o.trendMinSepDist <= 0) o.trendMinSepDist = io->meta.hasSeasonCmpnt? period / 2: 3 ; o.trendMinSepDist = max(o.trendMinSepDist, o.trendMaxOrder + 1);	o.trendMinSepDist = min(o.trendMinSepDist, N / 2 - 1);
+	if (m.trendMinKnotNum)                           o.trendMinKnotNum = 0;	                                      o.trendMinKnotNum = max(min(o.trendMaxKnotNum, o.trendMinKnotNum), 0);
+	if (m.trendMaxKnotNum)                           o.trendMaxKnotNum = min(floor(N / (o.trendMinSepDist + 1) - 1.f), 10); o.trendMaxKnotNum = min(o.trendMaxKnotNum, floor(N / (o.trendMinSepDist + 1) - 1.f)); o.trendMaxKnotNum = max(o.trendMaxKnotNum, o.trendMinKnotNum);
+
+	if (m.outlierMaxKnotNum) o.outlierMaxKnotNum = o.trendMaxKnotNum;      o.outlierMaxKnotNum = max(o.outlierMaxKnotNum, 1L); // at least has one; otherwise, the program crahses if hasOUtliercomponet=1
 	
 	if (m.K_MAX )            o.K_MAX            = 500;                  
 	if (m.sigFactor)         o.sigFactor        = 1.8;            o.sigFactor        = max(o.sigFactor,        1.02);
 	if (m.outlierSigFactor)  o.outlierSigFactor = 2.5;            o.outlierSigFactor = max(o.outlierSigFactor, 1.5);
 
 	if (m.sig2 )             o.sig2      = 0.2f;				  o.sig2             = max(o.sig2,      0.01);
 	if (m.precValue)         o.precValue = 1.5f;				  o.precValue        = max(o.precValue, 0.01);
@@ -956,15 +829,14 @@
 	if (m.outlierBasisFuncType) {
 		if      (o.precPriorType == UniformPrec)		o.outlierBasisFuncType = 0;
 		else if (o.precPriorType == ConstPrec)          o.outlierBasisFuncType = 0;
 		else if (o.precPriorType == ComponentWise)      o.outlierBasisFuncType = 1;
 		else if (o.precPriorType == OrderWise)          o.outlierBasisFuncType = 1;
 	}	 
 	if (m.modelPriorType)			o.modelPriorType        = 1L;
-	
 
 	return 1;
 
 #undef o
 }
 
 static int  GetArg_3rd_MCMC___(VOIDPTR prhs[], int nrhs, BEAST2_MCMC_PTR mcmc,  BEAST2_OPTIONS_PTR opt)
@@ -987,51 +859,51 @@
 	if (nrhs < 5) 
 		memset(&m, 1L, sizeof(struct MCMC_MISSING));
 
 	if (nrhs >= 5) {
 
 		VOIDPTR S = prhs[4L];
 		if (!IsStruct(S)) {
-			r_warning("WARNING: The arg 'mcmc' is ignored because it is not a LIST variable.");
+			q_warning("WARNING: The arg 'mcmc' is ignored because it is not a LIST variable.");
 			memset(&m, 1L, sizeof(struct MCMC_MISSING));
 		} else {
 			VOIDPTR tmp;
 			o.maxMoveStepSize = (tmp = GetField123Check(S, "maxMoveStepSize",2))? GetScalar(tmp) : (m.maxMoveStepSize = 1);
-			o.samples         = (tmp = GetField123Check(S, "samples", 2)) ?        GetScalar(tmp) : (m.samples = 1);
+			o.samples         = (tmp = GetField123Check(S, "samples", 3)) ?        GetScalar(tmp) : (m.samples = 1);
 			o.thinningFactor  = (tmp = GetField123Check(S, "thinningFactor", 2)) ? GetScalar(tmp) : (m.thinningFactor = 1);
 			o.burnin          = (tmp = GetField123Check(S, "burnin", 2)) ?         GetScalar(tmp) : (m.burnin = 1);
 			o.chainNumber     = (tmp = GetField123Check(S, "chainNumber", 2)) ?    GetScalar(tmp) : (m.chainNumber = 1);
-			o.seed			  = (tmp = GetField123Check(S, "seed", 2)) ?			GetScalar(tmp) : (m.seed = 1);
+			o.seed			  = (tmp = GetField123Check(S, "seed", 4)) ?			GetScalar(tmp) : (m.seed = 1);
 			o.ridgeFactor	  = (tmp = GetField123Check(S, "ridgeFactor", 2)) ?	GetScalar(tmp) : (m.ridgeFactor = 1);
 
-			o.trendResamplingOrderProb  = (tmp = GetField123Check(S, "trendResamplingOrderProb",  2)) ? GetScalar(tmp) : (m.trendResamplingOrderProb = 1);
-			o.seasonResamplingOrderProb = (tmp = GetField123Check(S, "seasonResamplingOrderProb", 2)) ? GetScalar(tmp) : (m.seasonResamplingOrderProb = 1);
+			o.trendResamplingOrderProb  = (tmp = GetField123Check(S, "trendResamplingOrderProb",  5)) ? GetScalar(tmp) : (m.trendResamplingOrderProb = 1);
+			o.seasonResamplingOrderProb = (tmp = GetField123Check(S, "seasonResamplingOrderProb", 5)) ? GetScalar(tmp) : (m.seasonResamplingOrderProb = 1);
 			o.credIntervalAlphaLevel    = (tmp = GetField123Check(S, "credIntervalAlphaLevel",    2)) ? GetScalar(tmp) : (m.credIntervalAlphaLevel = 1);
 		}
 
 	} // if (nrhs >= 5)
-
  
 	//r_printf("move :%d  %d %d\n", o.maxMoveStepSize, opt->io.meta.hasSeasonCmpnt , opt->prior.trendMinSepDist  );
 	if (m.maxMoveStepSize || o.maxMoveStepSize==0) o.maxMoveStepSize = opt->io.meta.hasSeasonCmpnt? opt->io.meta.period: (opt->prior.trendMinSepDist + 1);
 	if (m.samples         || o.samples==0)		   o.samples		 = 3000;        o.samples		  = max(o.samples, 800);
 	if (m.thinningFactor  || o.thinningFactor==0)  o.thinningFactor  = 1L;			o.thinningFactor = max(o.thinningFactor, 1L);
 	if (m.burnin          || o.burnin==0)          o.burnin		     = 150L;		o.burnin		  = max(o.burnin, 150L);
 	if (m.chainNumber || o.chainNumber==0)         o.chainNumber	 = 3;			o.chainNumber	  = max(o.chainNumber, 1L);
 	if (m.seed)            o.seed			 = 0L;
 	if (m.credIntervalAlphaLevel)      o.credIntervalAlphaLevel	 = .95;
 	if (m.ridgeFactor)     o.ridgeFactor	 = 0.0001f;
 
 	if (m.trendResamplingOrderProb)  o.trendResamplingOrderProb  = .1f;
 	if (m.seasonResamplingOrderProb) o.seasonResamplingOrderProb = .17f;
-
+ 
 	return 1;
 
 #undef o
 }
+
 static int  GetArg_4th_EXTRA__(VOIDPTR prhs[], int nrhs, BEAST2_EXTRA_PTR extra, I32 whichDimIsTime, I32 ndims)
 {
 	// Before running this function, meta.whichDimIsTime must be first obtained
 
 	#define o (*extra)
 	struct OUTFLAGS_MISSING {
 		I08   numThreadsPerCPU;
@@ -1070,15 +942,15 @@
 
 	if (nrhs < 6) 
 		memset(&m, 1L, sizeof(struct OUTFLAGS_MISSING));	
 
 	if (nrhs >= 6) {
 		VOIDPTR S = prhs[5L];
 		if (!IsStruct(S)) {
-			r_warning("WARNING: The arg 'extra' is ignored because it is not a LIST variable.");
+			q_warning("WARNING: The arg 'extra' is ignored because it is not a LIST variable.");
 			memset(&m, 1L, sizeof(struct OUTFLAGS_MISSING));
 		}
 		else {
 			VOIDPTR tmp;
 			o.whichOutputDimIsTime = (tmp = GetField123Check(S, "whichOutputDimIsTime",2)) ?	GetScalar(tmp) : (m.whichOutputDimIsTime = 1);
 			o.removeSingletonDims  = (tmp = GetField123Check(S, "removeSingletonDims", 8)) ? GetScalar(tmp) : (m.removeSingletonDims = 1);			
 			o.numThreadsPerCPU     = (tmp = GetField123Check(S, "numThreadsPerCPU", 4)) ? GetScalar(tmp) : (m.numThreadsPerCPU = 1);
@@ -1097,16 +969,14 @@
 			_2(computeCredible,  fastCIComputation);
 
 			_2(computeSeasonOrder,   computeTrendOrder);
 			_3(computeSeasonChngpt,  computeTrendChngpt, computeOutlierChngpt);
 			_2(computeSeasonAmp,     computeTrendSlope);
 			_4(tallyPosNegSeasonJump, tallyPosNegTrendJump, tallyIncDecTrendJump, tallyPosNegOutliers);
 			_1(useMeanOrRndBeta);
-
-		 
 				 
 		} // if (!IsStruct(S)) : S is a struct
 	} // if (nrhs >= 5)
 
 	if (m.whichOutputDimIsTime)		o.whichOutputDimIsTime = whichDimIsTime;
 	if (m.removeSingletonDims)		o.removeSingletonDims  = 1;
 
@@ -1118,15 +988,14 @@
 	if (m.numThreadsPerCPU)      o.numThreadsPerCPU    = 2;
 	if (m.numParThreads)         o.numParThreads		= 0;
 	if (m.numCPUCoresToUse)      o.numCPUCoresToUse	= 0;	
 	if (m.consoleWidth||o.consoleWidth<=0)  o.consoleWidth= GetConsoleWidth(); 	o.consoleWidth = max(o.consoleWidth, 40);
 	if (m.printProgressBar)      o.printProgressBar	= 1;
 	if (m.printOptions)          o.printOptions		= 1;
 
-
 	if (m.computeCredible)       o.computeCredible		= 0L;
 	if (m.fastCIComputation)     o.fastCIComputation	= 1L;
 
 	if (m.computeSeasonOrder)    o.computeSeasonOrder	= 0L;
 	if (m.computeTrendOrder)     o.computeTrendOrder	= 0L;
 
 	if (m.computeSeasonChngpt)   o.computeSeasonChngpt	= 1L;
@@ -1155,14 +1024,15 @@
 }
 
 I32 PostCheckArgs(A(OPTIONS_PTR) opt) {
 
 	I08 hasSeasonCmpnt   = opt->prior.basisType[0] == SEASONID || opt->prior.basisType[0] == DUMMYID || opt->prior.basisType[0] == SVDID;
 	I08 hasHarmonicCmpnt = opt->prior.basisType[0] == SEASONID ;
 	I08 hasDummyCmpnt    = opt->prior.basisType[0] == DUMMYID;
+	I08 hasSVDCmpnt      = opt->prior.basisType[0] == SVDID;
 	I08 hasOutlierCmpnt  = opt->prior.basisType[opt->prior.numBasis - 1] == OUTLIERID;
 	I08 hasTrendCmpnt    = 1;
 	I08 hasAlways        = 1;
 
 	// Period must be an integer when Dummy is used
 	if (hasDummyCmpnt) opt->io.meta.period = ceil(opt->io.meta.period);
 
@@ -1185,18 +1055,20 @@
 		opt->extra.computeSeasonChngpt   = 0;
 		opt->extra.computeSeasonAmp      = 0;
 		opt->extra.tallyPosNegSeasonJump = 0;
 	}
 	if (hasDummyCmpnt) {
 		opt->extra.computeSeasonOrder	    = 0;	
 		opt->extra.computeSeasonAmp         = 0; //TODO: remove this restriction
-		opt->mcmc.seasonResamplingOrderProb = 0;
 		opt->prior.seasonMinOrder           = 0;
 		opt->prior.seasonMaxOrder           = 0;		
 	}
+	if (hasSVDCmpnt) { 
+		opt->extra.computeSeasonAmp = 0; //TODO: remove this restriction 
+	}
 	if (!hasOutlierCmpnt) {
 		opt->extra.computeOutlierChngpt = 0;
 		opt->extra.tallyPosNegOutliers  = 0;
 	}
 
 	BEAST2_PRIOR_PTR PRIOR = &opt->prior;
 	#define prior (*PRIOR)
@@ -1204,45 +1076,45 @@
 	I08  isSeasonCmpntFixed = prior.seasonMaxOrder == prior.seasonMinOrder && prior.seasonMaxKnotNum == 0 && prior.seasonMinKnotNum == 0;
 	if (hasDummyCmpnt) isSeasonCmpntFixed = prior.seasonMaxKnotNum == 0 && prior.seasonMinKnotNum == 0;
 	#undef prior
 
 	//if numbasis == 2 and hasOutlier == 1, then the first cmpt must not be fixed
 	if (opt->prior.numBasis == 2 ) {
 		if (hasTrendCmpnt  && hasOutlierCmpnt && isTrendCmpntFixed) {
-			r_warning("WARNING: The options 'trendMaxOrder==trendMaxOrder && trendMaxKnotNum==0 && trendMinKnotNum==0' will"
+			q_warning("WARNING: The options 'trendMaxOrder==trendMaxOrder && trendMaxKnotNum==0 && trendMinKnotNum==0' will"
 				     " fix the trend to a global curve.\n");					 
 		}
 		if (hasHarmonicCmpnt && hasOutlierCmpnt && isSeasonCmpntFixed) {
-			r_warning("WARNING: The options 'seasonMaxOrder==seasonMaxOrder && seasonMaxKnotNum==0 && seasonMinKnotNum==0' will"
+			q_warning("WARNING: The options 'seasonMaxOrder==seasonMaxOrder && seasonMaxKnotNum==0 && seasonMinKnotNum==0' will"
 				    " fix the season component to a global curve.\n");		 
 		}
 		if (hasDummyCmpnt && hasOutlierCmpnt && isSeasonCmpntFixed) {
 			// for the dummy cmpnt, maxOrder and minOrder are both set to zeros.
-			r_warning("WARNING: The options 'seasonMaxKnotNum==0 && seasonMinKnotNum==0' will"
+			q_warning("WARNING: The options 'seasonMaxKnotNum==0 && seasonMinKnotNum==0' will"
 				    " fix the dummy season component to a global curve.\n");			
 		}
 	}
 	if (hasTrendCmpnt && hasDummyCmpnt & isTrendCmpntFixed && isSeasonCmpntFixed) {		
-		r_warning("WARNING: The options 'trendMaxOrder==trendMaxOrder && trendMaxKnotNum==0 && trendMinKnotNum==0 && "
+		q_warning("WARNING: The options 'trendMaxOrder==trendMaxOrder && trendMaxKnotNum==0 && trendMinKnotNum==0 && "
 			    " seasonMaxKnotNum==0 && seasonMinKnotNum==0' will"
 			    " fix the model structures of the trend and dummy season components.\n");
  
 	}
 	if (hasTrendCmpnt && hasHarmonicCmpnt & isTrendCmpntFixed && isSeasonCmpntFixed) {
-		r_warning("WARNING: The options 'trendMaxOrder==trendMaxOrder && trendMaxKnotNum==0 && trendMinKnotNum==0 && "
+		q_warning("WARNING: The options 'trendMaxOrder==trendMaxOrder && trendMaxKnotNum==0 && trendMinKnotNum==0 && "
 			    "seasonMaxOrder==seasonMaxOrder && seasonMaxKnotNum==0 && seasonMinKnotNum==0' will"
 			    " fix the model structures of the trend and harmonic season components.\n"); 
 	}
 
 	I32 KMAX=0;
 	for (I32 i = 0; i < PRIOR->numBasis; i++) {		
 		I08 type = PRIOR->basisType[i];
 		if (type == SEASONID)			KMAX += (PRIOR->seasonMaxOrder*2) * (PRIOR->seasonMaxKnotNum + 1);
-		if (type == DUMMYID)			KMAX += (opt->io.meta.period)    * (PRIOR->seasonMaxKnotNum + 1);
-		if (type == SVDID)			    KMAX += (opt->io.meta.period) * (PRIOR->seasonMaxKnotNum + 1);
+		if (type == DUMMYID)			KMAX += (opt->io.meta.period)     * (PRIOR->seasonMaxKnotNum + 1);
+		if (type == SVDID)			    KMAX += (opt->io.meta.period)     * (PRIOR->seasonMaxKnotNum + 1);
 		if (type == TRENDID)			KMAX += (PRIOR->trendMaxOrder +1) * (PRIOR->trendMaxKnotNum + 1);
 		if (type == OUTLIERID)			KMAX += PRIOR->outlierMaxKnotNum;
 	}
 	PRIOR->K_MAX = min(PRIOR->K_MAX, KMAX);
 
 	
 	// The initial model is generated in "basis_genrandombasis". We cacluat the number of terms for it
@@ -1279,51 +1151,53 @@
 
 	opt->io.out.dtype          = IsRinterface() ? DATA_DOUBLE : DATA_FLOAT;
 	opt->io.out.whichDimIsTime = opt->extra.whichOutputDimIsTime;
 
     // no need to use componetwise if there is only one componet
 	if (opt->prior.precPriorType == ComponentWise && opt->prior.numBasis == 1) {
 		opt->prior.precPriorType = UniformPrec;
-		r_warning("WARNING: prior$precPriorType is changed from 'componentwise' to 'uniform' because the model specified only has one component.\n");
+		//q_warning("WARNING: prior$precPriorType is changed from 'componentwise' to 'uniform' because the model specified only has a trend component.\n");
 	}
 	return 1;
 }
 
-int BEAST2_GetArgs(VOIDPTR prhs[], int nrhs, A(OPTIONS_PTR) opt)
-{
-	int  failed = !GetArg_1st_MetaData(prhs, nrhs, &opt->io.meta)		 || 
-				  !ParseInputData(&opt->io)								 || 
-			      !GetArg_2nd_Prior__(prhs, nrhs, &opt->prior, &opt->io)   ||
-			      !GetArg_3rd_MCMC___(prhs, nrhs, &opt->mcmc,  opt)     ||
+int BEAST2_GetArgs(VOIDPTR prhs[], int nrhs, A(OPTIONS_PTR) opt) {
+
+  
+
+	int  failed = !GetArg_0th_Data(prhs, nrhs, &opt->io)                 ||
+		          !GetArg_1st_MetaData(prhs, nrhs, &opt->io)		      || 				  
+			      !GetArg_2nd_Prior__(prhs, nrhs, &opt->prior, &opt->io)  ||
+			      !GetArg_3rd_MCMC___(prhs, nrhs, &opt->mcmc,  opt)       ||
 			      !GetArg_4th_EXTRA__(prhs, nrhs, &opt->extra, opt->io.meta.whichDimIsTime,opt->io.ndim) ;
 	int success = !failed;	
 	if (success) 	success=PostCheckArgs(opt); 	
 	if (success) 	BEAST2_print_options(opt);	
+
 	return success;
 }
 
 
 void BEAST2_DeallocateTimeSeriesIO(BEAST2_IO_PTR  o) {
 	// Free mems allocated in the "tsAggegrationPrepare" function
-	if (o->T.numPtsPerInterval != NULL) {
-		free(o->T.numPtsPerInterval);
-		o->T.numPtsPerInterval = NULL;
-	}
-	if (o->T.sortedTimeIdx != NULL) {
-		free(o->T.sortedTimeIdx);
-		o->T.sortedTimeIdx = NULL;
+	if (o->T.out.numPtsPerInterval != NULL) {
+		free(o->T.out.numPtsPerInterval);
+		o->T.out.numPtsPerInterval = NULL;
 	}
+	TimeVec_kill(&o->T);
+
 	if (o->pdata != NULL) {
 		free(o->pdata);
 		o->pdata = NULL;
 	}
 	if (o->dtype != NULL) {
 		free(o->dtype);
 		o->dtype = NULL;
 	}
 	if (o->out.result != NULL) {
 		free(o->out.result);
 		o->out.result = NULL;
 	}
+ 
 }
 
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_io_out_allocmem_q.c` & `Rbeast-0.1.14/ext_src/beastv2_io_out_allocmem_q.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #include "abc_000_warning.h"
 #include "abc_001_config.h"
 
 #include <string.h>   // memset and memcpy
 
 #include "abc_ide_util.h"
 #include "abc_vec.h"
+#include "abc_date.h"
 #include "abc_mem.h"
 #include "beastv2_io.h"
 
 
 static void __RemoveFieldsGivenFlags_Trend(A(OPTIONS_PTR)  opt, FIELD_ITEM * fieldList, int nfields) {
 
 	I08 hasSeasonCmpnt  = opt->prior.basisType[0] == SEASONID || opt->prior.basisType[0] == DUMMYID || opt->prior.basisType[0] == SVDID;
@@ -175,90 +176,63 @@
 	#undef _3
 	#undef _4
     #undef _5
 	#undef _6
 	#undef _7
 }
 
-static void __ExtendDims_SwitchTimeDim_1D2D(FIELD_ITEM* fld, int outTimDim, int numTS) {
-	
-	int ndim = fld->ndim;
-	if (ndim > 2 || outTimDim >2  ||  (numTS==1 && outTimDim!=1)) {
-		// newDimT should be always 1 if the number of pixels is 1
-		r_printf("__ExtendDims_SwitchTimeDim_1D2D:there must be something wrong!");
-	}
-
-	if        (outTimDim == 1) {
-	    // Apend the nuMTS at the end
-		fld->dims[ndim] = numTS;
-		fld->ndim++;
-	} else if (outTimDim == 2) {
-	   // Insert the numTS at the start
-		for (int i = ndim - 1; i >= 0; i--) { fld->dims[i + 1] = fld->dims[i]; }
-		fld->dims[0] = numTS;
-		fld->ndim++;;
-	}  
-}
 
-static void __ExtendDims_SwitchTimeDim_3D(FIELD_ITEM* fld, int outTimDim, int ROW, int COL) {
- 
-	int ndim = fld->ndim;
-	if (ndim > 2 || outTimDim >3) {
-		r_printf("__ExtendDims_SwitchTimeDim_1D2D:there must be something wrong!");
-	}
-
-	if  (outTimDim == 1) {
-	    // Apend the nuMTS at the end
-		fld->dims[ndim  ] = ROW;
-		fld->dims[ndim+1] = COL;
-		fld->ndim  +=2;
-	} else if (outTimDim == 3) {
-	   // Insert the numTS at the start
-		for (int i = ndim - 1; i >= 0; i--) {fld->dims[i + 2] = fld->dims[i];}
-		fld->dims[0] = ROW;
-		fld->dims[1] = COL;
-		fld->ndim += 2;
-	} else if (outTimDim == 2) {
-		// Insert ROW at the start and the COL at the end
-		for (int i = ndim - 1; i >= 0; i--) {fld->dims[i +1 ] = fld->dims[i];}
-		fld->dims[0]      = ROW;
-		fld->dims[ndim+1] = COL;
-		fld->ndim += 2;
+static void   __AddSpatialDimension(int ROW, int COL, int whichOutDimIsTime, FIELD_ITEM * fieldList, int nfields) {
+	  
+  	if (whichOutDimIsTime == 1) {
+		// Apend the nuMTS at the end
+		for (int i = 0; i < nfields; i++) {
+			FIELD_ITEM * fld  = fieldList + i;
+			int          ndim = fld->ndim;
+			fld->dims[ndim]     = ROW;
+			fld->dims[ndim + 1] = COL;
+			fld->ndim += 2;
+		}
+		return;
 	}
 
-}
-
-static void   ExtendDims_SwitchTimeDim_AllFields(BEAST2_IO_PTR  io, FIELD_ITEM * fieldList, int nfields) {
-
-	/***************************************/
-	// If the inputs is a ts or a 2D matrix
-	/***************************************/
-	if (io->ndim == 1 || io->ndim == 2) {		
-		// When numTS=1, outWhichDimIsTIms should be always 1.
+	if (whichOutDimIsTime == 2) {
+		// Insert ROW at the start and the COL at the end
 		for (int i = 0; i < nfields; i++) {
-			__ExtendDims_SwitchTimeDim_1D2D(fieldList + i, io->out.whichDimIsTime, io->numOfPixels);
+			FIELD_ITEM * fld  = fieldList + i;
+			int          ndim = fld->ndim;
+			for (int i = ndim - 1; i >= 0; i--) { 
+				fld->dims[i + 1] = fld->dims[i]; 
+			}
+			fld->dims[0]         = ROW;
+			fld->dims[ndim + 1]  = COL;
+			fld->ndim           += 2;
 		}
+		return;
 	}
-	// if the input is a 3D stack
-	else if (io->ndim == 3) {		
-		int   ROW, COL;
-		switch (io->meta.whichDimIsTime) {
-			case 1:	ROW = io->dims[1], COL = io->dims[2]; break;
-			case 2:	ROW = io->dims[0], COL = io->dims[2]; break;
-			case 3:	ROW = io->dims[0], COL = io->dims[1]; break;
-		}
+
+	if (whichOutDimIsTime == 3) {
+		// Insert the numTS at the start
 		for (int i = 0; i < nfields; i++) {
-			__ExtendDims_SwitchTimeDim_3D(fieldList + i, io->out.whichDimIsTime, ROW, COL);
+			FIELD_ITEM * fld  = fieldList + i;
+			int          ndim = fld->ndim;
+			for (int i = ndim - 1; i >= 0; i--) {
+				fld->dims[i + 2] = fld->dims[i]; 
+			}
+			fld->dims[0] = ROW;
+			fld->dims[1] = COL;
+			fld->ndim    += 2;
 		}
-	
+		return;
 	}
+	 
 }
 
 
-static  I32 __MR_ExtendFieldsToMultiVaraiteTS(FIELD_ITEM *flist, I32 N, I32 q) {
+static  I32  __MR_ExtendFieldsToMultiVaraiteTS(FIELD_ITEM *flist, I32 N, I32 q) {
 
 	if (q == 1) 
 		return 0;
 
 	//char* nms[] = { "Y1","Y2" ,"Y3", };
 
 	I32 nptr       = 0;
@@ -267,15 +241,15 @@
 
 		if (flist[i].extra == 0 || flist[i].ptr == NULL)
 			continue;
 
 		nptr_dummy++;
 		FIELD_ITEM qList[100] = { { /*fielditem*/{/*char*/0,},}, };
 		for (int j = 0; j < q; j++) {
-			sprintf(qList[j].name, "Y%d", j+1); 	//strcpy(qList[j].name, nms[j]);
+			snprintf(qList[j].name, 63, "Y%d", j+1); 	//strcpy(qList[j].name, nms[j]);
 			qList[j].extra = 0;
 			qList[j].type  = flist[i].type;
 			qList[j].ndim  = flist[i].ndim;
 			memcpy(&qList[j].dims, &flist[i].dims, sizeof(I32) * 5);
 	
 			if (flist[i].ptr != NULL)
 				qList[j].ptr = (char*)(flist[i].ptr) + sizeof(BEAST2_RESULT) * j;
@@ -295,55 +269,21 @@
 	}
  
  
 	 UNPROTECT(nptr_dummy); //nptr_dummy=0: added here to trick R's ptr checker
 	 return nptr;
 }
 
-
-static void __RemoveSingltonDims(FIELD_ITEM* flist, I32 nlist) {
-	// 1 x1 ->1
-	// 2x1x1x2-> 2x2
-	// 1x10 -> 10
-
-	// 10 : in R, this will be created as a vector, and in Matlab 
-	// be created as a column vector.
-	for (int i = 0; i < nlist; i++) {
-
-		if ( flist[i].ndim == 1) continue;
-		
-		int goodN       = 0;
-		int goodDims[4];
-		// FInd all the non-one dims
-		for (int j = 0; j < flist[i].ndim; j++) {
-			if (flist[i].dims[j]!= 1) {
-				goodDims[goodN++] = flist[i].dims[j];
-			}
-		}
-
-		// Re-assign the non-one dims
-		if (goodN == 0) {
-			// it is 1x 1 x1 ..,
-			flist[i].ndim    = 1;
-			flist[i].dims[0] = 1;
-		} else {
-			flist[i].ndim = goodN;
-			for (int j = 0; j < goodN; j++) {
-				flist[i].dims[j] = goodDims[j];
-			}
-		}
-	}
-
-}
+ 
 static void* __BEAST2_Output_AllocMEM_Trend(A(OPTIONS_PTR)  opt) {
 
 	const BEAST2_IO_PTR      io = &opt->io;
 	const BEAST2_RESULT_PTR  mat = io->out.result;
-	DATA_TYPE   dtype = io->out.dtype; // DATA_FLOAT or DATA_DOUBLE                            
-	const int   N = io->N;
+	DATA_TYPE   dtype     = io->out.dtype; // DATA_FLOAT or DATA_DOUBLE                            
+	const int   N         = io->N;
 	const int   mxKnotNum = opt->prior.trendMaxKnotNum;
 	//https://stackoverflow.com/questions/2124339/c-preprocessor-va-args-number-of-arguments
 	#define NUMARGS(...)                 (sizeof((int[]){__VA_ARGS__})/sizeof(int))
 	#define NARGS(...)                   (sizeof((int[]){0, ##__VA_ARGS__})/sizeof(int)-1)
 	#define _(name, ...)                 {#name, dtype, NUMARGS(__VA_ARGS__),{__VA_ARGS__},(void ** )&mat->t##name }
 	#define _1(name, ...)                _(name, __VA_ARGS__)  
 	#define _2(name1,name2, ...)         _(name1, __VA_ARGS__),  _(name2, __VA_ARGS__)   
@@ -388,18 +328,18 @@
 			 _q2(inc_ncpPr,    dec_ncpPr,    mxKnotNum + 1),
 			 _q2(inc_cpOccPr,  dec_cpOccPr,  N),
 			 _q6(inc_cp,    dec_cp, inc_cpPr, dec_cpPr, inc_cpAbruptChange, dec_cpAbruptChange, mxKnotNum),
 			 _q2(inc_cpCI,  dec_cpCI,        mxKnotNum,2),
 	};
 
 	I32 nfields = sizeof(fieldList) / sizeof(FIELD_ITEM);
-	ExtendDims_SwitchTimeDim_AllFields(io, fieldList, nfields);
+	__AddSpatialDimension(io->dims[io->rowdim-1], io->dims[io->coldim - 1], io->out.whichDimIsTime, fieldList, nfields);
 	__RemoveFieldsGivenFlags_Trend(opt, fieldList, nfields);
 	if (opt->extra.removeSingletonDims) {
-		__RemoveSingltonDims(fieldList, nfields);
+		RemoveSingltonDims(fieldList, nfields);
 	}
 
 	// Do nothing if io->q is 1L;  within the function, newly created lists are protected
 	I32       nptr = __MR_ExtendFieldsToMultiVaraiteTS(fieldList, nfields, io->q); 
 	VOID_PTR  out  = PROTECT(CreateStructVar(fieldList, nfields));
 					 UNPROTECT(1L);
 	UNPROTECT(nptr); 
@@ -470,18 +410,18 @@
 			_q2(pos_ncpPr,  neg_ncpPr,    mxKnotNum+ 1),
 			_q2(pos_cpOccPr,neg_cpOccPr,  N),
 			_q6(pos_cp,     neg_cp,   pos_cpPr, neg_cpPr, pos_cpAbruptChange, neg_cpAbruptChange, mxKnotNum),
 			_q2(pos_cpCI,   neg_cpCI, mxKnotNum,2)				
 	};
 
 	I32 nfields = sizeof(fieldList) / sizeof(FIELD_ITEM);
-	ExtendDims_SwitchTimeDim_AllFields(io, fieldList, nfields);
+	__AddSpatialDimension(io->dims[io->rowdim - 1], io->dims[io->coldim - 1], io->out.whichDimIsTime, fieldList, nfields);
 	__RemoveFieldsGivenFlags_Season(opt, fieldList, nfields);
 	if (opt->extra.removeSingletonDims) {
-		__RemoveSingltonDims(fieldList, nfields);
+		RemoveSingltonDims(fieldList, nfields);
 	}
 
 	// Do nothing if io->q is 1L;  within the function, newly created lists are protected
 	I32       nptr = __MR_ExtendFieldsToMultiVaraiteTS(fieldList, nfields, io->q); 
 	VOID_PTR  out  = PROTECT(CreateStructVar(fieldList, nfields));
 					 UNPROTECT(1L);
 	UNPROTECT(nptr); 
@@ -502,14 +442,15 @@
 	#undef _q2
 	#undef _q3
 	#undef _q4
     #undef _q5
 	#undef _q6
 	#undef _q7
 }
+
 static void* __BEAST2_Output_AllocMEM_Outlier(A(OPTIONS_PTR)  opt)
 {
 	const BEAST2_IO_PTR      io     = &opt->io;
 	const BEAST2_RESULT_PTR  mat    = io->out.result;
 	DATA_TYPE   dtype        = io->out.dtype; // DATA_FLOAT or DATA_DOUBLE                            
 	const int   N	         = io->N;
 	const int   mxKnotNum	 = opt->prior.outlierMaxKnotNum;	
@@ -552,18 +493,18 @@
 			_q2(pos_ncpPr,   neg_ncpPr,    mxKnotNum + 1),
 			_q2(pos_cpOccPr, neg_cpOccPr,  N),
 			_q4(pos_cp,      neg_cp, pos_cpPr, neg_cpPr, mxKnotNum),
 			_q2(pos_cpCI,    neg_cpCI,     mxKnotNum,2),
 	};
 
 	I32 nfields = sizeof(fieldList) / sizeof(FIELD_ITEM);
-	ExtendDims_SwitchTimeDim_AllFields(io, fieldList, nfields);
+	__AddSpatialDimension(io->dims[io->rowdim - 1], io->dims[io->coldim - 1], io->out.whichDimIsTime, fieldList, nfields);
 	__RemoveFieldsGivenFlags_Outlier(opt, fieldList, nfields);
 	if (opt->extra.removeSingletonDims) {
-		__RemoveSingltonDims(fieldList, nfields);
+		RemoveSingltonDims(fieldList, nfields);
 	}
 
 	// Do nothing if io->q is 1L;  within the function, newly created lists are protected
 	I32       nptr = __MR_ExtendFieldsToMultiVaraiteTS(fieldList, nfields, io->q); 
 	VOID_PTR  out  = PROTECT(CreateStructVar(fieldList, nfields));
 					 UNPROTECT(1L);
 	UNPROTECT(nptr); 
@@ -587,16 +528,16 @@
     #undef _q5
 	#undef _q6
 	#undef _q7
 }
 
 
 
-void* BEAST2_Output_AllocMEM(A(OPTIONS_PTR)  opt) 
-{	
+void* BEAST2_Output_AllocMEM(A(OPTIONS_PTR)  opt)  {	
+
 	//Moved from glue_code to accomodate multivriate time series
 	if (opt->io.out.result) {
 		// Added to accomodate the beast_thread() for Win GUI where Output_AllocMem is called each time a thread is created.
 		free(opt->io.out.result);
 	}
 	opt->io.out.result = malloc(sizeof(BEAST2_RESULT) * opt->io.q);
 	memset(opt->io.out.result, 0, sizeof(BEAST2_RESULT) * opt->io.q);
@@ -661,24 +602,24 @@
 		{"whichOutDimIsTime", DATA_INT32,  2,  {1,1,},   &whichDimIsTime },
 		{"nrows",             DATA_INT32,  2,  {1,1,},   &nrows },
 		{"ncols",             DATA_INT32,  2,  {1,1,},   &ncols },
 	};
 	I32    nfields = sizeof(fieldList) / sizeof(FIELD_ITEM);
 
 	int sig2_index = 6 - 1;
-	ExtendDims_SwitchTimeDim_AllFields(io, &fieldList[sig2_index], 1L); //1L means only one field to be adjusted
+	__AddSpatialDimension(io->dims[io->rowdim - 1], io->dims[io->coldim - 1], io->out.whichDimIsTime, &fieldList[sig2_index], 1L); //1L means only one field to be adjusted
 	// Adjust the dimension of out$data based on the input dimesion and the outputtimedim
 	// to make it compatible with whichOutputDimIsTime.
 	// Change the data field by adding the extra dims and swithcing for the outputTimeDim
-	ExtendDims_SwitchTimeDim_AllFields(io, &fieldList[1], 1L);
+	__AddSpatialDimension(io->dims[io->rowdim - 1], io->dims[io->coldim - 1], io->out.whichDimIsTime, &fieldList[1], 1L);
 	if (!opt->extra.dumpInputData) {  		 
 		RemoveField(fieldList, nfields, "data"); mat->data = NULL;
 	}
 	if (opt->extra.removeSingletonDims) {
-		__RemoveSingltonDims(fieldList, nfields);
+		RemoveSingltonDims(fieldList, nfields);
 	}
 
 	VOID_PTR  out;
 	// Extend it if and only if q >1
 	I32       nptr1 = __MR_ExtendFieldsToMultiVaraiteTS(fieldList, nfields, io->q);  nprt += nptr1;
 	if (ROW * COL == 1) {
 		// No need to inclulde whichTimeDim and ncols and nrows if there is only one ts
@@ -693,15 +634,22 @@
 
 	AddStringAttribute(out,  "class",          "beast");	
 	if (hasSeasonCmpnt && !hasDummyCmpnt) AddStringAttribute(out,  "season_type",  "harmonic");
 	if (hasSeasonCmpnt &&  hasDummyCmpnt) AddStringAttribute(out,  "season_type",  "dummy");
 	if (!hasSeasonCmpnt )                 AddStringAttribute(out,  "season_type",  "none");
 	//AddIntegerAttribute(out, "hasOutlier", hasOutlierCmpnt);	
  
-	f32_seq(mat->time, io->meta.startTime, io->meta.deltaTime, N);
+	if (io->T.out.asDailyTS) {
+		for (int i = 0; i < N; i++) {
+			mat->time[i]=FracYear_from_DateNum(io->meta.startTime+ io->meta.deltaTime*i);
+		} 
+	}	else {
+		f32_seq(mat->time, io->meta.startTime, io->meta.deltaTime, N);
+	}    
+
 	if (dtype == DATA_DOUBLE)  f32_to_f64_inplace(mat->time, N);
 	//r_ippsMulC_32f_I(io->meta.deltaTime, mat->time, N);
 	//r_ippsSubC_32f_I(-(io->meta.startTime - io->meta.deltaTime), mat->time, N);
  
 
 	UNPROTECT(nprt);
 	return out;
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_io_out_tsextractprint.c` & `Rbeast-0.1.14/ext_src/beastv2_io_out_tsextractprint.c`

 * *Files 14% similar despite different names*

```diff
@@ -8,62 +8,50 @@
 #include "abc_ide_util.h"
 #include "abc_ts_func.h"
 #include "abc_common.h"  //WriteF32ArrayToStrideMEM
 #include "abc_vec.h"  //WriteF32ArrayToStrideMEM
 #include "beastv2_io.h"
  
 
-static void GetOutputOffsetStride_V2(int ROW, int COL, int whichDimIsTime, I64 idx, I64 Nvec, I64* pStride, I64* pOffset)
-{
-	//index should be 1-based.
-	I64 stride, offset;
-	if (ROW*COL==1)  
-	// A 1d vcetor: io->ndim == 1
-		stride = 1L, offset = (idx - 1) * Nvec;
-	else if (ROW==1 || COL==1) {
-	// A 2 D mat input:io->ndim == 2L
-	//TODO: buggy: a edge case may be  a 3D input of 1x1 in dimension
-
-		I32 nPixel = ROW * COL;
-		if(whichDimIsTime ==1)
-			stride = 1L, offset = (idx - 1) * Nvec;
-		else {
-			stride = nPixel;
-			offset = (idx - 1);
-		}
-	} else  { 
-	// A 3D stack input: io->ndim == 3L
-
-		switch (whichDimIsTime) {
-		case 1:
-			stride = 1L;
-			offset = (idx - 1) * Nvec;
-			break;
-		case 2: {
-			int c = (idx - 1) / ROW;
-			int r = idx - c * ROW;
-			c = c + 1;
-			stride = ROW;
-			offset = (c - 1) * (Nvec * ROW) + r - 1;
-			break;	}
-		case 3: {
-			int c = (idx - 1) / ROW;
-			int r = idx - c * ROW;
-			c = c + 1;
-			stride = ROW * COL;
-			offset = (c - 1) * ROW + r - 1;
-			break;	}
-		} // switch ( io->whichDimIsTime)	 
 
-	} // (io->ndim == 3L)
+static void __convert_index_to_datasubs3(int rows, int cols, int timedim, int index, int dims[], int subs3[]) {
+
+	int subs2[2];
+	int imgdims[] = { rows, cols };
+	ind2sub(imgdims, 2L, index, subs2);
+
+
+	if (timedim == 1) {
+		subs3[0] = 1;  // can fill any value
+		subs3[1] = subs2[0]; 
+		subs3[2] = subs2[1]; 
+		
+		dims[1] = rows;
+		dims[2] = cols;
+	}
+	else if (timedim == 2) {
+		subs3[1] = 1;  // can fill any value
+		subs3[0] = subs2[0]; 
+		subs3[2] = subs2[1]; 
+
+		dims[0] = rows;
+		dims[2] = cols;
+	}
+	else if (timedim == 3) {
+		subs3[2] = 1;  // can fill any value
+		subs3[0] = subs2[0];
+		subs3[1] = subs2[1];
+
+		dims[0] = rows;
+		dims[1] = cols;
+	}
 
-	*pStride = stride;
-	*pOffset = offset;
 }
 
+
 void* BEAST2_TsExtract(void *o, void * pindex ) {
  
 
 	VOID_PTR    tmp;	
 	
 	// Get basic dimension parameters from 0
 	DATA_TYPE   dtype;
@@ -305,87 +293,92 @@
 	out = PROTECT(CreateStructVar(fieldListBEAST, nfieldsBEAST));          nprt++;
 	AddStringAttribute(out,  "class",          "beast");	
 	
 
 	/************************************************/
 	// Copy elements to the newly created array
 	/************************************************/
+	int subs3[3];
+	int dims[3];
+	__convert_index_to_datasubs3(ROW, COL, whichDimTim, index, dims, subs3);
+
+
 	I64 stride, offset;
 
 	if (hasTrendCmpnt) {
 		fieldList = fieldListT;
 		nfields   = nfieldsT;
 		VOID_PTR cmpnt = GetField(o, "trend");
 		for (int i = 0; i < nfields; i++) {
 
 			if (fieldList[i].ptr == NULL) {
 				continue;
 			}			
-			int Nvec = fieldList[i].ndim == 1 ? fieldList[i].dims[0] : fieldList[i].dims[0] * fieldList[i].dims[1];			
-			GetOutputOffsetStride_V2(ROW, COL, whichDimTim,  index, Nvec, &stride, &offset);
+			dims[whichDimTim - 1] = fieldList[i].ndim == 1 ? fieldList[i].dims[0] : fieldList[i].dims[0] * fieldList[i].dims[1];			 
+			int Nvec = ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
 
 			VOID_PTR newData = GetData(  GetField(trend, fieldList[i].name) );
 			VOID_PTR oldData = GetData(  GetField(cmpnt, fieldList[i].name));
-			WriteStrideMEMToArrMEM(newData, oldData, Nvec, stride, offset, dtype);	
+			arr_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		}
 	
 	}
 	if (hasSeasonCmpnt) {
 		fieldList = fieldListS;
 		nfields   = nfieldsS;
 		VOID_PTR cmpnt = GetField(o, "season");
 		for (int i = 0; i < nfields; i++) {
 
 			if (fieldList[i].ptr == NULL) {
 				continue;
 			}			
-			int Nvec = fieldList[i].ndim == 1 ? fieldList[i].dims[0] : fieldList[i].dims[0] * fieldList[i].dims[1];			
-			GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
+			dims[whichDimTim - 1] = fieldList[i].ndim == 1 ? fieldList[i].dims[0] : fieldList[i].dims[0] * fieldList[i].dims[1];
+			int Nvec = ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
 
 			VOID_PTR newData = GetData(  GetField(season, fieldList[i].name) );
 			VOID_PTR oldData = GetData(  GetField(cmpnt, fieldList[i].name));
-			WriteStrideMEMToArrMEM(newData, oldData, Nvec, stride, offset, dtype);
+			arr_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		}
 	}
 	if (hasOutlierCmpnt) {
 		fieldList = fieldListO;
 		nfields   = nfieldsO;
 		VOID_PTR cmpnt = GetField(o, "outlier");
 		for (int i = 0; i < nfields; i++) {
 
 			if (fieldList[i].ptr == NULL) {
 				continue;
 			}			
-			int Nvec = fieldList[i].ndim == 1 ? fieldList[i].dims[0] : fieldList[i].dims[0] * fieldList[i].dims[1];			
-			GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
+			dims[whichDimTim - 1] = fieldList[i].ndim == 1 ? fieldList[i].dims[0] : fieldList[i].dims[0] * fieldList[i].dims[1];
+			int Nvec = ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
 
 			VOID_PTR newData = GetData(  GetField(outlier, fieldList[i].name) );
 			VOID_PTR oldData = GetData(  GetField(cmpnt, fieldList[i].name));
-			WriteStrideMEMToArrMEM(newData, oldData, Nvec, stride, offset, dtype);
+			arr_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		}
 	}
 
 	// Ti,e
 	{
 		VOID_PTR newData = GetData(GetField(out, fieldListBEAST[0].name));
 		VOID_PTR oldData = GetData(GetField(o, fieldListBEAST[0].name));
-		WriteStrideMEMToArrMEM(newData, oldData, N, 1, 0, dtype);
+		arr_from_strided_mem(newData, oldData, N, 1, 0, dtype);
 
 		for (int i = 1; i < 6; i++) {
 
 			if (fieldListBEAST[i].ptr == NULL) {
 				continue;
 			}
 
-			int Nvec = fieldListBEAST[i].ndim == 1 ? fieldListBEAST[i].dims[0] : fieldListBEAST[i].dims[0] * fieldListBEAST[i].dims[1];
-			GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
+			dims[whichDimTim - 1] = fieldListBEAST[i].ndim == 1 ? fieldListBEAST[i].dims[0] : fieldListBEAST[i].dims[0] * fieldListBEAST[i].dims[1];
+			int Nvec = ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
 
 			VOID_PTR newData = GetData(GetField(out, fieldListBEAST[i].name));
 			VOID_PTR oldData = GetData(GetField(o, fieldListBEAST[i].name));
-			WriteStrideMEMToArrMEM(newData, oldData, Nvec, stride, offset, dtype);
+			arr_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		}
 
 	}
 
 
 
 	UNPROTECT(nprt);
@@ -499,17 +492,17 @@
 	F32PTR newData = tmpbuf;
 	int    maxLen = max(maxKnotNumT, max(maxKnotNumS, maxKnotNumO)) + 1;
 	if (maxLen > 100) {
 		newData     = malloc(sizeof(F32) * maxLen);
 		isallocated = 1;
 	}
 
-	I64  stride, offset;
+
 	char s1[] = "                                                ";
-	int  nChar = strlen(s1);
+	int  nChar = (int) strlen(s1);
 
 	#define cat r_printf
 
 #if R_INTERFACE == 1
 	#define boldStart  "\033[1;31m" 
     #define boldEnd    "\033[0m" 
 #elif P_INTERFACE == 1
@@ -517,14 +510,20 @@
 	#define boldEnd    "\033[0m" 
 #else
 	#define boldStart  "<strong>" 
     #define boldEnd   "</strong>" 
 #endif
 
 
+	int subs3[3];
+	int dims[3];
+	__convert_index_to_datasubs3(ROW, COL, whichDimTim, index, dims, subs3);
+
+	I64  stride, offset;
+
 	cat(boldStart);
 	cat("#####################################################################\n");
 	cat("#                      Seasonal  Changepoints                       #\n");
 	cat("#####################################################################\n");
 	cat(boldEnd);
 
 	if (!hasSeasonCmpnt) {
@@ -533,18 +532,19 @@
 		
 	if (hasSeasonCmpnt) {
 
 		int      maxKnotNum = maxKnotNumS;
 		VOID_PTR cmpnt      = GetField(o, "season");
 
 	
-		int      Nvec       = maxKnotNum +1L;
-		GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
+		int      Nvec       = dims[whichDimTim-1]= maxKnotNum +1L;
+		ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+
 		VOID_PTR oldData  = GetData(GetField(cmpnt, "ncpPr"));
-		CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 maxPr;
 		I32 maxIx = f32_maxidx(newData, Nvec, &maxPr);
 		Nvec = min(Nvec, 99);
 		cat(".-------------------------------------------------------------------.\n");
 		cat("| Ascii plot of probability distribution for number of chgpts (ncp) |\n");
 		cat(".-------------------------------------------------------------------.\n");
 		for ( int i=0; i<Nvec; i++) {
@@ -552,25 +552,25 @@
 			slen = ceil(newData[i] / maxPr * (nChar - 1));
 			slen = max(1, slen);
 			memset(s1, ' ', nChar);
 			memset(s1, '*', slen);
 		    cat("|Pr(ncp = %-2d)=%.3f|%s|\n", i, newData[i], s1);
 		}
 
-		Nvec    = 1;	GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
-		oldData = GetData(GetField(cmpnt, "ncp"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		Nvec    = dims[whichDimTim - 1]=1;	ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+		oldData = GetData(GetField(cmpnt, "ncp"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_median")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_median")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_median = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_pct90")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_pct90")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_pct90 = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_pct10")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_pct10")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_pct10 = newData[0];
 
 		cat(".-------------------------------------------------------------------.\n"); 
 		cat("|    Summary for number of Seasonal ChangePoints (scp)              |\n");
 		cat(".-------------------------------------------------------------------.\n");
 		cat("|ncp_max    = %-4d | MaxSeasonKnotNum: A parameter you set          |\n",     maxKnotNum);
 		cat("|ncp_mode   = %-4d | Pr(ncp=%2d)=%3.2f: There is a %3.1f%% probability  |\n", maxIx, min(maxIx, 99), maxPr, maxPr * 100);
@@ -586,19 +586,19 @@
 		cat("'-------------------------------------------------------------------'\n");
 		cat("|scp#              |time (cp)                  |prob(cpPr)          |\n");
 		cat("|------------------|---------------------------|--------------------|\n");
 
 		F32 cp[200];
 		F32 cpPr[200];
 		if (GetData(GetField(cmpnt, "cp"))) {
-			Nvec    = maxKnotNum;	GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
-			oldData = GetData(GetField(cmpnt, "cp"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);		
+			Nvec = dims[whichDimTim - 1] = maxKnotNum;	ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+			oldData = GetData(GetField(cmpnt, "cp"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);		
 			memcpy(cp, newData, sizeof(F32)* min(200, Nvec));
 
-			oldData = GetData(GetField(cmpnt, "cpPr"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+			oldData = GetData(GetField(cmpnt, "cpPr"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 			memcpy(cpPr, newData, sizeof(F32) * min(200, Nvec));
 
 			Nvec = min(200L, Nvec);
 
 			int ncp_all=0;
 			for (int i = 0; i < Nvec; i++) {
 				ncp_all = ncp_all + (cp[i] == cp[i]);
@@ -620,18 +620,19 @@
 	cat("#####################################################################\n");
 	cat(boldEnd);
 
 	if (hasTrendCmpnt) {
 		int      maxKnotNum = maxKnotNumT;
 		VOID_PTR cmpnt      = GetField(o, "trend");
 
-		int      Nvec       = maxKnotNum +1L;
-		GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
+		int      Nvec;
+		Nvec = dims[whichDimTim - 1] = maxKnotNum + 1L;	
+		ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
 		VOID_PTR oldData  = GetData(GetField(cmpnt, "ncpPr"));
-		CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 maxPr;
 		I32 maxIx = f32_maxidx(newData, Nvec, &maxPr);
 		Nvec = min(Nvec, 99);
 		cat(".-------------------------------------------------------------------.\n");
 		cat("| Ascii plot of probability distribution for number of chgpts (ncp) |\n");
 		cat(".-------------------------------------------------------------------.\n");
 		for ( int i=0; i<Nvec; i++) {
@@ -639,25 +640,25 @@
 			slen = ceil(newData[i] / maxPr * (F32)(nChar - 1));
 			slen = max(1, slen);
 			memset(s1, ' ', nChar);
 			memset(s1, '*', slen);
 		    cat("|Pr(ncp = %-2d)=%.3f|%s|\n", i, newData[i], s1);
 		}
 
-		Nvec    = 1;	GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
-		oldData = GetData(GetField(cmpnt, "ncp"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+ 		Nvec = dims[whichDimTim - 1] = 1L;	ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+		oldData = GetData(GetField(cmpnt, "ncp"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_median")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_median")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_median = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_pct90")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_pct90")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_pct90 = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_pct10")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_pct10")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_pct10 = newData[0];
 
 		cat(".-------------------------------------------------------------------.\n");
 		cat("|    Summary for number of Trend ChangePoints (tcp)                 |\n");
 		cat(".-------------------------------------------------------------------.\n");
 		cat("|ncp_max    = %-4d | MaxTrendKnotNum: A parameter you set           |\n", maxKnotNum);
 		cat("|ncp_mode   = %-4d | Pr(ncp=%2d)=%3.2f: There is a %3.1f%% probability  |\n", maxIx, min(maxIx, 99), maxPr, maxPr * 100);
@@ -674,19 +675,19 @@
 		cat("|tcp#              |time (cp)                  |prob(cpPr)          |\n");
 		cat("|------------------|---------------------------|--------------------|\n");
 
 		F32 cp[200];
 		F32 cpPr[200];
 
 		if (GetData(GetField(cmpnt, "cp"))) {
-			Nvec    = maxKnotNum;	GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
-			oldData = GetData(GetField(cmpnt, "cp"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);		
+			Nvec = dims[whichDimTim - 1] = maxKnotNum;	ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+			oldData = GetData(GetField(cmpnt, "cp"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);		
 			memcpy(cp, newData, sizeof(F32)* min(200, Nvec));
 
-			oldData = GetData(GetField(cmpnt, "cpPr"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+			oldData = GetData(GetField(cmpnt, "cpPr"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 			memcpy(cpPr, newData, sizeof(F32) * min(200, Nvec));
 
 			Nvec = min(200L, Nvec);
 
 			int ncp_all=0;
 			for (int i = 0; i < Nvec; i++) {
 				ncp_all = ncp_all + (cp[i] == cp[i]);
@@ -706,18 +707,19 @@
 		cat("#                      Outlier  Changepoints                        #\n");
 		cat("#####################################################################\n");
 		cat(boldEnd);
 		int      maxKnotNum = maxKnotNumO;
 		VOID_PTR cmpnt      = GetField(o, "outlier");
 
 
-		int      Nvec       = maxKnotNum +1L;
-		GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
+		int     Nvec   ;
+		Nvec = dims[whichDimTim - 1] = maxKnotNum + 1L;	ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+
 		VOID_PTR oldData = GetData(GetField(cmpnt, "ncpPr"));
-		CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 maxPr;
 		I32 maxIx = f32_maxidx(newData, Nvec, &maxPr);
 		Nvec = min(Nvec, 99);
 		cat(".-------------------------------------------------------------------.\n");
 		cat("| Ascii plot of probability distribution for number of chgpts (ncp) |\n");
 		cat(".-------------------------------------------------------------------.\n");
 		for ( int i=0; i<Nvec; i++) {
@@ -725,25 +727,25 @@
 			slen = ceil(newData[i] / maxPr * (nChar - 1));
 			slen = max(1, slen);
 			memset(s1, ' ', nChar);
 			memset(s1, '*', slen);
 		    cat("|Pr(ncp = %-2d)=%.3f|%s|\n", i, newData[i], s1);
 		}
 
-		Nvec    = 1;	GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
-		oldData = GetData(GetField(cmpnt, "ncp"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		Nvec = dims[whichDimTim - 1] = 1L;	ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+		oldData = GetData(GetField(cmpnt, "ncp"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_median")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_median")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_median = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_pct90")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_pct90")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_pct90 = newData[0];
 
-		oldData = GetData(GetField(cmpnt, "ncp_pct10")); 	CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+		oldData = GetData(GetField(cmpnt, "ncp_pct10")); 	f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 		F32 ncp_pct10 = newData[0];
 
 		cat(".-------------------------------------------------------------------.\n");
 		cat("|    Summary for number of Outlier ChangePoints (ocp)               |\n");
 		cat(".-------------------------------------------------------------------.\n");
 		cat("|ncp_max    = %-4d | MaxOutlierKnotNum: A parameter you set         |\n", maxKnotNum);
 		cat("|ncp_mode   = %-4d | Pr(ncp=%2d)=%3.2f: There is a %3.1f%% probability  |\n", maxIx, min(maxIx, 99), maxPr, maxPr * 100);
@@ -761,19 +763,19 @@
 		cat("|------------------|---------------------------|--------------------|\n");
 
 
 		F32 cp[200];
 		F32 cpPr[200];
 
 		if (GetData(GetField(cmpnt, "cp"))) {
-			Nvec    = maxKnotNum;	GetOutputOffsetStride_V2(ROW, COL, whichDimTim, index, Nvec, &stride, &offset);
-			oldData = GetData(GetField(cmpnt, "cp"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);		
+			Nvec = dims[whichDimTim - 1] = maxKnotNum;	ndarray_get1d_stride_offset(dims, 3L, subs3, whichDimTim, &stride, &offset);
+			oldData = GetData(GetField(cmpnt, "cp"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);		
 			memcpy(cp, newData, sizeof(F32)* min(200, Nvec));
 
-			oldData = GetData(GetField(cmpnt, "cpPr"));		  CopyStrideMEMToF32Arr(newData, oldData, Nvec, stride, offset, dtype);
+			oldData = GetData(GetField(cmpnt, "cpPr"));		  f32_from_strided_mem(newData, oldData, Nvec, stride, offset, dtype);
 			memcpy(cpPr, newData, sizeof(F32) * min(200, Nvec));
 
 			Nvec = min(200L, Nvec);
 
 			int ncp_all=0;
 			for (int i = 0; i < Nvec; i++) {
 				ncp_all = ncp_all + (cp[i] == cp[i]);
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_model_allocinit_q.c` & `Rbeast-0.1.14/ext_src/beastv2_model_allocinit_q.c`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 	MODEL.b = MyALLOC(*MEM, NumBasis, BEAST2_BASIS, 64);
 
 	for (int i = 0; i < NumBasis; i++)
 		MODEL.b[i].type = opt->prior.basisType[i];
 		
 
 	I32 isComponentFixed[3] = {0,0,0};
-	MODEL.did = MODEL.sid = MODEL.tid = MODEL.oid = -1;
+	MODEL.did = MODEL.sid = MODEL.tid = MODEL.oid = MODEL.vid= -1;
 	for (int i = 0; i < NumBasis; i++) 	{
 
 		BEAST2_BASIS_PTR	basis	= MODEL.b + i;
 		I08					type	= basis->type;
 
 		void (*AllocInitBasisMEM)(BEAST2_BASIS_PTR, I32,I32, MemPointers*)= Get_AllocInitBasis(type);
 
@@ -536,26 +536,27 @@
 			// Pre-calcalte terms for SEASON AND TRENDS Bases:Precaluating SEASON AND TREND terms 
 			/*************************************************************************************************/
 			// When deseaonalize=TRUE, the full set of cos/sin are needed to compute seasonality 		
 			SVD_CONST* SVD = &basis->bConst;
 			I32 sMAXORDER  = opt->io.meta.deseasonalize? opt->io.meta.period: basis->prior.maxOrder;
 			SVD->TERMS     = MyALLOC(*MEM, N*sMAXORDER ,              F32, 64);
 			SVD->SQR_CSUM  = MyALLOC(*MEM, (N + 1L) * sMAXORDER ,     F32, 64);
-			CopyNumericArrToF32Arr(SVD->TERMS, opt->io.meta.svdTerms, N* sMAXORDER);
-			{
+			if(opt->io.meta.svdTerms_Object)	{
+				CopyNumericObjToF32Arr(SVD->TERMS, opt->io.meta.svdTerms_Object, N* sMAXORDER);
 				F32PTR ptr  = SVD->TERMS;
 				F32PTR ptr1 = SVD->SQR_CSUM; 
 
 				for (I32 order = 1; order <= sMAXORDER; order++) {				 
 						*ptr1 = 0.f;						
 						f32_copy(ptr, ptr1 + 1, N);         f32_cumsumsqr_inplace(ptr1 + 1, N);
 						ptr  +=  N;
 						ptr1 += N + 1;
 				} // or (rI32 order = 1; order <= maxSeasonOrder; order++)
 			}
+ 
 			/****************************************************************************/
 			//				Pre-compute the scaling factor
 			/****************************************************************************/
 			I32 sMAXNUMKNOT = basis->prior.maxKnotNum;
 			I32 sMINSEPDIST = basis->prior.minSepDist;
 			F32PTR scaleFactor = MyALLOC(*MEM, sMAXNUMKNOT + 1, F32, 0);
 			{
```

### Comparing `Rbeast-0.1.13/ext_src/beastv2_prior_model.c` & `Rbeast-0.1.14/ext_src/beastv2_prior_model.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_prior_precfunc.c` & `Rbeast-0.1.14/ext_src/beastv2_prior_precfunc.c`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_prior_precfunc.h` & `Rbeast-0.1.14/ext_src/beastv2_prior_precfunc.h`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/ext_src/beastv2_xxyy_allocmem_q.c` & `Rbeast-0.1.14/ext_src/beastv2_xxyy_allocmem_q.c`

 * *Files 16% similar despite different names*

```diff
@@ -8,44 +8,42 @@
 #include "abc_001_config.h"
 #include "abc_rand.h"
 #include "abc_mat.h"
 #include "beastv2_func.h"
 
 #include "abc_ide_util.h" //printf
 
-#define max(a,b)            (((a) > (b)) ? (a) : (b))
-#define max3(a,b,c)         max( max(a,b), c)
-#define max4(a,b,c,d)       max( max3(a,b,c),d)
-#define min(a,b)            (((a) < (b)) ? (a) : (b))
-
-
 
 static I32 __GetNumElem_of_XnewTerm(BEAST2_MODEL_PTR model, BEAST2_OPTIONS_PTR opt,   I32 * MAX_COL) {
 	#define MODEL (*model)
-	/////////////////////////////////////////////////////////////////////////////////////////////////
+
 	// For some proposal moves, two new segments will be generated..
      #define MAX_NUM_NEW_SEG 2
 	I32 MXNCOL_PERSEG1 = MODEL.sid >= 0 ? (MODEL.b[MODEL.sid].prior.maxOrder)*2L : -9999;  	// mem to save one season term	
 	I32 MXNCOL_PERSEG2 = MODEL.tid >= 0 ? (MODEL.b[MODEL.tid].prior.maxOrder+1L) : -9999;    // mem to save one trend term	
 	I32 MXNCOL_PERSEG3 = MODEL.did >= 0 ? opt->io.meta.period : -9999;                       // mem to save one dummyterm   
+	I32 MXNCOL_PERSEG4 = MODEL.vid >= 0 ? MODEL.b[MODEL.tid].prior.maxOrder : -9999;    // mem to save one trend term	
 
 	I32 MAXNUMCOL_Xnewterm = max3(MXNCOL_PERSEG1, MXNCOL_PERSEG2, MXNCOL_PERSEG3) * MAX_NUM_NEW_SEG;
 	/////////////////////////////////////////////////////////////////////////////////////////////////
 
 
 	/////////////////////////////////////////////////////////////////////////////////////////////////
-	// Extra mem for storing BASESEG
+	// Extra mem for storing BASESEG: used in GetInfoBandList() of beastv4_Core
 	I32 MAX_TOTAL_SEGNUM = 0;
-	for (int i = 0; i < MODEL.NUMBASIS; i++)	MAX_TOTAL_SEGNUM += (MODEL.b[i].prior.maxKnotNum + 1);
+	for (int i = 0; i < MODEL.NUMBASIS; i++) { 
+		MAX_TOTAL_SEGNUM += (MODEL.b[i].prior.maxKnotNum + 1);
+	}
 	I32 MAX_NUMELEM_SEGINFO = MAX_TOTAL_SEGNUM * (sizeof(BEAST2_BASESEG)/4);
 	/////////////////////////////////////////////////////////////////////////////////////////////////
 
 
 	/////////////////////////////////////////////////////////////////////////////////////////////////
 	//Xnewterm must have a length larger than or equla to 5*N + max(sncp, tncp);
+	// used in FindChangepoint() of beastv3_core()
 	I32 MAX_MEM_FOR_CHANGEPOINTS = 6 * opt->io.N;
 	/////////////////////////////////////////////////////////////////////////////////////////////////
 	
 	/////////////////////////////////////////////////////////////////////////////////////////////////
 	// The length of the raw data of input time series  which differs from N for irregular TS
 	// Xnewterm is used as temp mem for fetch_next_timeSeries)(&yInfo, pixelIndex, MEMBUF, opt);
 	I32 Nraw = opt->io.dims[ opt->io.meta.whichDimIsTime-1L];
@@ -57,90 +55,105 @@
 
 	//Xnewterm is also needed to store the recoverd original Y data values to be dumped into the output
 	//varaible o.data and to compute R2 and RMSE.
 	I32 MAX_COLS_YPRED = opt->io.q * MODEL.NUMBASIS;
 	/////////////////////////////////////////////////////////////////////////////////////////////////
 
 
-	I32 Npad = ((opt->io.N + 7) / 8) * 8;  Npad = opt->io.N;//Correct for the inconsitency of X and Y in gemm and gemv
+	I32 Npad = RoundTo8(opt->io.N);
+	Npad = opt->io.N;//Correct for the inconsitency of X and Y in gemm and gemv
 	I32 TOTAL_NUM = max4( MAXNUMCOL_Xnewterm* Npad + MAX_NUMELEM_SEGINFO, 
 		                  MAX_MEM_FOR_CHANGEPOINTS,
 		                  MAX_COLS_YPRED*Npad,
 		                  Nraw);
 		
-		
 	*MAX_COL = MAXNUMCOL_Xnewterm;
 	return TOTAL_NUM;
 
     #undef MODEL
 }
 /*************************************************/
 //Arrays that have a leading dimension of Npad:
 // Xt_mars, and Xnewterm
 // Y has a leading dimension of N, as in fetech_next_time-series
 /*************************************************/
 
 void AllocateXXXMEM( F32PTR * Xt_mars, F32PTR*  Xnewterm, F32PTR*  Xt_zeroBackup,
 	                 BEAST2_MODEL_PTR model, BEAST2_OPTIONS_PTR opt, MemPointers * MEM) 
 {	
-#define RoundTo64(N)  ((N+63)/64*64)
 
 	I32 N         = opt->io.N;
-	I32 Npad      = ((N + 7) / 8) * 8;
+	I32 Npad      = RoundTo8(N);
 	I32 K_MAX     = opt->prior.K_MAX;
-	I64 szXtmars  = Npad * K_MAX;
+	I64 SIZE_Xtmars  = Npad * K_MAX;
 
 	I32 XNEW_MAX_NUMCOL;
 	I32 XNEW_TOTAL_NUM    = __GetNumElem_of_XnewTerm(model, opt, &XNEW_MAX_NUMCOL);
 	I32 MAXNUM_MISSINGROW = N * opt->io.meta.maxMissingRate + 1;
 
-	I64 szXnewterm     =  XNEW_TOTAL_NUM;
-	I64 szXtzeroBackup =  MAXNUM_MISSINGROW * XNEW_MAX_NUMCOL;
+	I64 SIZE_Xnewterm     =  XNEW_TOTAL_NUM;
+	I64 SIZE_XtzeroBackup =  MAXNUM_MISSINGROW * XNEW_MAX_NUMCOL;
+
 
+	I32 SIZE_Total = RoundTo64(SIZE_Xtmars) + RoundTo64(SIZE_Xnewterm) + RoundTo64(SIZE_XtzeroBackup);
 
-	I32 szTotal = RoundTo64(szXtmars) + RoundTo64(szXnewterm) + RoundTo64(szXtzeroBackup);
+	typedef struct SVDBasisMEM SVDBasisMEM;
+	I64 Get_Alloc_SVDBasisMEM(int N, int P, SVDBasisMEM * s, VOID_PTR bufBase); // from beastv2_svdbasis
+	I32 SIZE_svdASISMEM =0;  // Needed for computing svd basis terms	
+	if (opt->io.meta.seasonForm == 'V') {
+		int P = opt->io.meta.period;
+		SIZE_svdASISMEM =Get_Alloc_SVDBasisMEM(N, P, NULL, NULL);
+	}
+	SIZE_Total = max(SIZE_Total, SIZE_svdASISMEM);
 
-	*Xt_mars       = MyALLOC(*MEM, szTotal, F32, 64);
-	*Xnewterm      = *Xt_mars  + RoundTo64(szXtmars) ;
-	*Xt_zeroBackup = *Xnewterm + RoundTo64(szXnewterm);
+	*Xt_mars       = MyALLOC(*MEM, SIZE_Total, F32, 64);
+	*Xnewterm      = *Xt_mars  + RoundTo64(SIZE_Xtmars) ;
+	*Xt_zeroBackup = *Xnewterm + RoundTo64(SIZE_Xnewterm);
 	//Xt_mars		= MyALLOC(MEM, Npad * MAX_K, F32, 64); 
 	//Xnewterm		= MyALLOC(MEM, TOTAL_NUM, F32, 64);
 	//Xt_zeroBackup = MyALLOC(MEM, MAXNUM_MISSINGROW *MAX_NUMCOL, F32, 64);
 }
 
 
 void AllocateYinfoMEM(BEAST2_YINFO_PTR yInfo, BEAST2_OPTIONS_PTR opt, MemPointers* MEM) {
 	I32  N    = opt->io.N;	//I32  Npad = ((N+7)/8) * 8;
 	I32  q    = opt->io.q;  //q=1 for BEASTV2
 	I32  qxq = q*q;
 	//Important: In fetch_next_timeSeries (__NormalizeF32ArrayWithNaNOmitted_zerobased), it is possible
 	// that all the points are bad indices, so the space for rowMissing should be at least of length N.
 	I32  MAXNUM_MISSINGROW = N;  //N * opt->io.meta.maxMissingRate + 1L;
 
+
+	MemNode nodes[10];
+	int     nNodes = 0;
+
 	// Sizes: Y[Npad], sd[q], mean[q], YtY_plus_alpha2Q[q*q]
-	yInfo->Y                = MyALLOC(*MEM, N*q+ qxq +q +q,              F32, 64);
-	yInfo->YtY_plus_alpha2Q = yInfo->Y                + N*q;
-	yInfo->mean             = yInfo->YtY_plus_alpha2Q + qxq;
-	yInfo->sd               = yInfo->mean + q;
+	nodes[nNodes++] = (MemNode){ .addr=&yInfo->Y,                .size =sizeof(F32)*N*q,  .align = 64,.offset_from_origin=0};
+	nodes[nNodes++] = (MemNode){ .addr=&yInfo->YtY_plus_alpha2Q, .size = sizeof(F32)*q*q, .align = 4,.offset_from_origin = 0 };
+	nodes[nNodes++] = (MemNode){ .addr=&yInfo->mean,             .size = sizeof(F32)*q,   .align = 4,.offset_from_origin = 0 };
+	nodes[nNodes++] = (MemNode){ .addr=&yInfo->sd,               .size = sizeof(F32)*q,   .align = 4,.offset_from_origin = 0 };
+
+
 
 	// yInfo.rowsMissing: THE INDEX OF ROWS WITH MISSING DATA	
-	yInfo->rowsMissing     = MyALLOC(*MEM, MAXNUM_MISSINGROW, U32, 64);	 	
+	nodes[nNodes++] = (MemNode){ .addr = &yInfo->rowsMissing,    .size = sizeof(U32) * MAXNUM_MISSINGROW,   .align =64,.offset_from_origin = 0 };
 
 	//added for MRBEAST and used in ComputeLik, PropseNew/__CalcAbsDeviation(compute deviaiton and extrempos)
 	//, MR_EvaluateModel,
 	yInfo->q               = q;
 
 	if (opt->io.meta.deseasonalize) {
-		yInfo->Yseason= MyALLOC(*MEM, N * q , F32, 0);
+		nodes[nNodes++] = (MemNode){ .addr = &yInfo->Yseason,    .size = sizeof(F32) * N * q,   .align = 4,.offset_from_origin = 0 };
 	} else {
 		yInfo->Yseason = NULL;
 	}
 
 	if (opt->io.meta.detrend) {
-		yInfo->Ytrend = MyALLOC(*MEM, N * q, F32, 0);
-	}
-	else {
+		nodes[nNodes++] = (MemNode){ .addr = &yInfo->Ytrend,    .size = sizeof(F32) * N * q,   .align = 4,.offset_from_origin = 0 }; 
+	} else {
 		yInfo->Ytrend = NULL;
 	}
+	nodes[nNodes++] = (MemNode){ .addr =NULL };
+	MEM->alloclist(MEM, nodes, AggregatedMemAlloc,NULL);
 }
 
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/ext_src/globalvars.c` & `Rbeast-0.1.14/ext_src/globalvars.c`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 #include "abc_000_warning.h"
 //Added before globalvar.h bcz abc_pthread is included, which has a few static functions not already 
 // used. We want to force -Wno-unused-function
 #include "globalvars.h"
 
 VOID_PTR  GLOBAL_OPTIONS;
 VOID_PTR  GLOBAL_RESULT;
-
+VOID_PTR  GLOBAL_DATA0;
 
 pthread_t       *thread_id;
 pthread_mutex_t  mutex;
 pthread_cond_t   condVar;
 
 
 volatile F32    PERCENT_COMPLETED;
 volatile F32    REMAINING_TIME;
 volatile I32    NEXT_PIXEL_INDEX;
 volatile I32    NUM_OF_PROCESSED_PIXELS;
 volatile I32    NUM_OF_PROCESSED_GOOD_PIXELS;
  
 
-int  IS_CPU_INSTRUCTON_SET = 0;
+
+char GLOBAL_QUIET_MODE = 0;
 
 #include "abc_000_warning.h"
```

### Comparing `Rbeast-0.1.13/py_src/Rbeast/__init__.py` & `Rbeast-0.1.14/py_src/Rbeast/__init__.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/beast.py` & `Rbeast-0.1.14/py_src/Rbeast/beast.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/beast123.py` & `Rbeast-0.1.14/py_src/Rbeast/beast123.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/beast_irreg.py` & `Rbeast-0.1.14/py_src/Rbeast/beast_irreg.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/cvt_to_numpy.py` & `Rbeast-0.1.14/py_src/Rbeast/cvt_to_numpy.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/data/beach.csv` & `Rbeast-0.1.14/py_src/Rbeast/data/beach.csv`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/data/ndvi.npy` & `Rbeast-0.1.14/py_src/Rbeast/data/ndvi.npy`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/data/ndvi_filename.txt` & `Rbeast-0.1.14/py_src/Rbeast/data/ndvi_filename.txt`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/data/ndvi_fyear.npy` & `Rbeast-0.1.14/py_src/Rbeast/data/ndvi_fyear.npy`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/data/nile.csv` & `Rbeast-0.1.14/py_src/Rbeast/data/nile.csv`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/extractbeast.py` & `Rbeast-0.1.14/py_src/Rbeast/extractbeast.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/load_example.py` & `Rbeast-0.1.14/py_src/Rbeast/load_example.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/plotbeast.py` & `Rbeast-0.1.14/py_src/Rbeast/plotbeast.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/py_src/Rbeast/printbeast.py` & `Rbeast-0.1.14/py_src/Rbeast/printbeast.py`

 * *Files identical despite different names*

### Comparing `Rbeast-0.1.13/setup.py` & `Rbeast-0.1.14/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import os,sys,glob
+import os, sys, glob
 from   setuptools import setup, find_packages, Extension,find_namespace_packages
 
-
 #import numpy as np
 
-# setup should isstall numpy but numpy is needed to get the numpy headers  in np.get_include()
-# and run the setup before it is installed -- chichen-and-egg problems
+# chichen-and-egg problems:  setup should install numpy but numpy is needed to get the numpy headers in np.get_include()
+# and run the setup before it is installed
 # 
 # https://stackoverflow.com/questions/56008251/setup-requires-does-not-seem-to-install-dependencies
 # https://stackoverflow.com/questions/35516059/python-is-not-installing-dependencies-listed-in-install-requires-of-setuptools
 # https://stackoverflow.com/questions/19919905/how-to-bootstrap-numpy-installation-in-setup-py/21621689
 
 # A few solutions: https://stackoverflow.com/questions/19919905/how-to-bootstrap-numpy-installation-in-setup-py/21621689
 # This should now (since 2018-ish) be solved by adding numpy as a buildsystem dependency in pyproject.toml, 
@@ -36,39 +35,40 @@
 
 def is_platform_windows():
     return sys.platform == "win32" or sys.platform == "cygwin"
 
 def is_platform_mac():
     return sys.platform == "darwin"
     
-filenames    = glob.glob('ext_src/*.c');
-filenames.append("ext_src/abc_ioFlushcpp.cpp")
 
 extralibs  = []
 if is_platform_windows():
    extralibs=["kernel32", "user32", "gdi32" ]
+
+filenames    = glob.glob('ext_src/*.c');
+filenames.append("ext_src/abc_ioFlushcpp.cpp")
       
 modules = Extension(
             "Rbeast.Rbeast",
             sources       = filenames,
-            include_dirs  = [get_numpy_include(), "ext_src/"],      #[np.get_include(), "ext_src/"],
-            define_macros = [('P_RELEASE','1'),('R_INTERFACE','0')],
+            include_dirs  = [get_numpy_include(), "ext_src/"],      # [ np.get_include(), "ext_src/"],
+            define_macros = [('P_RELEASE','1'),('RRR_INTERFACE','0')],
             libraries     = extralibs
         )
         
 #packages = find_packages( include=['exampleproject','exampleproject.*','data'],  exclude=['figures', 'output', 'notebooks'])
 #packages = find_packages( exclude=['figures', 'output', 'notebooks'])           
 #packages = find_packages( exclude=['tests'])           
 packages = find_packages( include =['Rbeast'],exclude=['Rbeast.src'])     
 packages = find_namespace_packages(where='./py_src', exclude=['build','tests','extension_src'])
 #print(packages)
 #print(packages)
 setup(
     name             = "Rbeast",   
-    version          = '0.1.13',
+    version          = '0.1.14',
     description      = "Bayesian changepoint detection and time series decomposition",
     author           = "Kaiguang Zhao",
     author_email     = 'zhao.1423@osu.edu',
     url              = 'https://github.com/zhaokg/Rbeast',    
     keywords         = ['changepoint', 'structural breaks','time series decomposition' 'time series analysis', 'trend analysis'],
     python_requires  = '>=3.5',  
     long_description = read('README.md'),
@@ -76,24 +76,25 @@
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",        
         "Programming Language :: Python :: 3.9",                
         "Programming Language :: Python :: 3.10",                        
         "Programming Language :: Python :: 3.11",   
+        "Programming Language :: Python :: 3.12",   
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Hydrology",
         "Topic :: Scientific/Engineering :: Atmospheric Science",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
     ],    
-    #setup_requires  = ['numpy'], #deprecated in favor of pyproject.toml
-    install_requires     = ['numpy', 'matplotlib>=2.2.0'],
-    #entry_points={  'console_scripts': ['mycommand=exampleproject.data:main1'] },    
+    #setup_requires      = ['numpy'],           # Deprecated in favor of pyproject.toml
+    install_requires     =  ['numpy>=1.18', 'matplotlib>=2.2.0'], # ['numpy>=1.10', 'matplotlib>=2.2.0'],
+    #entry_points        ={  'console_scripts': ['mycommand=exampleproject.data:main1'] },    
     packages             = packages,    
     package_dir          = {"Rbeast": "py_src/Rbeast","Rbeast.data": "py_src/Rbeast/data", '': '.'},      
     include_package_data = True,      
     package_data         = {'Rbeast': ['data/nile.csv'],'Rbeast.data': ['beach.csv'] ,'Rbeast': ['data/*.npy','data/*.txt','data/*.csv']},
     exclude_package_data = {'': ['*.c','*.cpp']},       
     ext_modules          = [modules]
 )
```

