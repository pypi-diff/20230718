# Comparing `tmp/bbrc-bx-0.5.1.tar.gz` & `tmp/bbrc-bx-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrc-bx-0.5.1.tar", last modified: Tue Jul 11 17:09:34 2023, max compression
+gzip compressed data, was "bbrc-bx-0.5.2.tar", last modified: Tue Jul 18 13:57:07 2023, max compression
```

## Comparing `bbrc-bx-0.5.1.tar` & `bbrc-bx-0.5.2.tar`

### file list

```diff
@@ -1,106 +1,105 @@
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/MANIFEST.in
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    20834 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    16563 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/README.md
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bbrc_bx.egg-info/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    20834 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2443 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/SOURCES.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/dependency_links.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/requires.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/top_level.txt
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bin/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bin/bx
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bin/dump
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       22 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/__init__.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/ants.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/archiving.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/ashs.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/bamos.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3957 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/basil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/braak.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/cache.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/cat12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1276 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/command.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3477 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/dartel.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/aal2/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/aal2/AAL2.nii
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/braak/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/braak/Braak_III_IV.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/braak/Braak_I_II.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/braak/Braak_V_VI.nii.gz
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/dickerson/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/dickerson/ad/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.tpole.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/readme.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.tpole.label
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/dickerson/aging/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/logo
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/masks/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   902981 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/data/masks/fdg_aging_mask.nii
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/mrtrix3/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6193 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/data/mrtrix3/fs_default.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/dcm.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/donsurf.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    13464 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/download.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/dtifit.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3118 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/dump.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/freesurfer.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/id.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    75188 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/lists.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3200 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/mrtrix3.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/nifti.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8829 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/parse.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8455 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/pet.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2882 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/qsmxt.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/scandates.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/signature.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/spm12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/validation.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/xnat.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/requirements.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/setup.cfg
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/setup.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.046810 bbrc-bx-0.5.2/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/MANIFEST.in
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21746 2023-07-18 13:57:07.046810 bbrc-bx-0.5.2/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17339 2023-07-18 13:56:17.000000 bbrc-bx-0.5.2/README.md
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bbrc_bx.egg-info/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21746 2023-07-18 13:57:07.000000 bbrc-bx-0.5.2/bbrc_bx.egg-info/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2423 2023-07-18 13:57:07.000000 bbrc-bx-0.5.2/bbrc_bx.egg-info/SOURCES.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2023-07-18 13:57:07.000000 bbrc-bx-0.5.2/bbrc_bx.egg-info/dependency_links.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-07-18 13:57:07.000000 bbrc-bx-0.5.2/bbrc_bx.egg-info/requires.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2023-07-18 13:57:07.000000 bbrc-bx-0.5.2/bbrc_bx.egg-info/top_level.txt
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bin/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bin/bx
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bin/dump
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bx/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       22 2023-07-18 13:56:17.000000 bbrc-bx-0.5.2/bx/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/ants.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/archiving.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/ashs.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/bamos.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3957 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/basil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/braak.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/cache.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/cat12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1276 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/command.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3477 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/bx/dartel.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bx/data/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bx/data/aal2/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/aal2/AAL2.nii
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bx/data/braak/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/braak/Braak_III_IV.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/braak/Braak_I_II.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/braak/Braak_V_VI.nii.gz
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bx/data/dickerson/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.036810 bbrc-bx-0.5.2/bx/data/dickerson/ad/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.tpole.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/readme.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.tpole.label
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.046810 bbrc-bx-0.5.2/bx/data/dickerson/aging/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/data/logo
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 13:57:07.046810 bbrc-bx-0.5.2/bx/data/masks/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   902981 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/bx/data/masks/fdg_aging_mask.nii
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/dcm.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/donsurf.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    13464 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/bx/download.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/dtifit.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3118 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/bx/dump.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/freesurfer.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/id.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    75188 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/bx/lists.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2521 2023-07-18 13:56:17.000000 bbrc-bx-0.5.2/bx/mrtrix3.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/nifti.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8829 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/parse.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8455 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/bx/pet.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2882 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/bx/qsmxt.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/scandates.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/signature.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/spm12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/validation.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3517 2023-07-18 13:56:17.000000 bbrc-bx-0.5.2/bx/xcpd.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-02-09 15:02:03.000000 bbrc-bx-0.5.2/bx/xnat.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-07-18 13:56:17.000000 bbrc-bx-0.5.2/requirements.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2023-07-18 13:57:07.046810 bbrc-bx-0.5.2/setup.cfg
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-07-11 17:06:38.000000 bbrc-bx-0.5.2/setup.py
```

### Comparing `bbrc-bx-0.5.1/PKG-INFO` & `bbrc-bx-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5.1
+Version: 0.5.2
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.1/bx-v0.5.1.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.2/bx-v0.5.2.tar.gz
 Description: # bx
         
         [![pipeline status](https://gitlab.com/bbrc/xnat/bx/badges/master/pipeline.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![coverage report](https://gitlab.com/bbrc/xnat/bx/badges/master/coverage.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![downloads](https://img.shields.io/pypi/dm/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![python versions](https://img.shields.io/pypi/pyversions/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![pypi version](https://img.shields.io/pypi/v/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
@@ -221,15 +221,15 @@
         
         FreeSurfer v6.0.0
         
             Available subcommands:
              `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
              `aseg`:			create an Excel table with all `aseg` measurements
              `aparc`:			create an Excel table with all `aparc` measurements
-             hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+             `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
              `snapshot`:		download a snapshot from the `recon-all` pipeline
              `report`:			download the validation report issued by bbrc-validator
              `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx freesurfer6 <subcommand> <resource_id>
         
@@ -237,15 +237,15 @@
         
         FreeSurfer v6.0.0 (-hires option)
         
             Available subcommands:
              `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
              `aseg`:			create an Excel table with all `aseg` measurements
              `aparc`:			create an Excel table with all `aparc` measurements
-             hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+             `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
              `snapshot`:		download a snapshot from the `recon-all` pipeline
              `report`:			download the validation report issued by bbrc-validator
              `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx freesurfer6hires <subcommand> <resource_id>
         
@@ -253,20 +253,20 @@
         
         FreeSurfer v7.1.1
         
             Available subcommands:
              `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
              `aseg`:			create an Excel table with all `aseg` measurements
              `aparc`:			create an Excel table with all `aparc` measurements
-             amygNucVolumes:	save an Excel table with amygdalar volumes
+             `amygNucVolumes`:	save an Excel table with amygdalar volumes
              `brainstem`:		save an Excel table with brainstem substructures volumes
              `thalamus`:		save an Excel table with thalamic nuclei volumes
-             hypothalamus:		save an Excel table with hypothalamic subunits volumes
+             `hypothalamus`:	save an Excel table with hypothalamic subunits volumes
              `jack`:			compute the cortical AD signature with FS7 results
-             hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+             `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
              `snapshot`:		download a snapshot from the `recon-all` pipeline
              `report`:			download the validation report issued by bbrc-validator
              `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx freesurfer7 <subcommand> <resource_id>
         
@@ -301,15 +301,15 @@
              bx lists <subcommand>
         
         ### **`MRTRIX3`**:
         
         MRtrix3 - Diffusion MRI tractography and structural connectivity.
         
             Available subcommands:
-             connectome:	download the structural connectivity matrices (Desikan-Killiany atlas)
+             `connectome`:	download the structural connectivity matrices (Desikan-Killiany atlas)
              `files`:		download all MRTRIX3 outputs (streamlines, segmentations, everything...)
              `report`:		download the validation report issued by `MRtrix3Validator`
              `snapshot`:	download snapshots from the MRTRIX3 pipeline
              `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx mrtrix3 <subcommand> <resource_id>
@@ -348,15 +348,15 @@
             - Landau et al., Ann Neurol., 2012
         
         ### **`FTM`**:
         
         18F-flutemetamol PET imaging data
         
             Available subcommands:
-             centiloids:	creates an Excel table with centiloid scales
+             `centiloids`:	creates an Excel table with centiloid scales
              `maps`:		download the normalized FTM maps
              `tests`:		collect all automatic tests outcomes from `PetSessionValidator`
              `mri`:			creates an Excel table with details from associated MRI sessions
         
             Usage:
              bx ftm <subcommand> <resource_id>
         
@@ -438,18 +438,35 @@
              `report`:		download the validation report issued by `SPM12Validator`
              `tests`:		creates an Excel table with all automatic tests outcomes from `SPM12`
              `rc`:			downloads rc* files (DARTEL imports)
         
             Usage:
              bx spm12 <subcommand> <resource_id>
         
+        ### **`XCPD`**:
+        
+        XCP-D - Resting State fMRI postprocessing and functional connectivity.
+        
+            Available subcommands:
+             `conmat`:          download the functional connectivity matrix (Desikan-Killiany atlas)
+             `timeseries`:      download the parcellated BOLD time-series (Desikan-Killiany atlas)
+             `files`:           download all XCP_D outputs (denoised BOLD data, segmentations, everything...)
+             `report`:          download the validation report issued by `XCPDValidator`
+             `snapshot`:        download snapshots from the XCPD pipeline
+             `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+        
+            Usage:
+             bx xcpd <subcommand> <resource_id>
+        
+            References:
+            - Ciric R, et al., Nat Protoc 13 (2018).
         
         ## Dependencies
         
-        Requires [`bbrc-pyxnat>=1.4.2`](https://gitlab.com/pyxnat/pyxnat/tree/bbrc) and
+        Requires [`bbrc-pyxnat>=1.6.1`](https://gitlab.com/pyxnat/pyxnat/tree/bbrc) and
         the librairies listed in `requirements.txt`.
         
         
         ## Install
         
         ```
         pip install bbrc-bx
```

### Comparing `bbrc-bx-0.5.1/README.md` & `bbrc-bx-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 
 FreeSurfer v6.0.0
 
     Available subcommands:
      `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
      `aseg`:			create an Excel table with all `aseg` measurements
      `aparc`:			create an Excel table with all `aparc` measurements
-     hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+     `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
      `snapshot`:		download a snapshot from the `recon-all` pipeline
      `report`:			download the validation report issued by bbrc-validator
      `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx freesurfer6 <subcommand> <resource_id>
 
@@ -228,15 +228,15 @@
 
 FreeSurfer v6.0.0 (-hires option)
 
     Available subcommands:
      `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
      `aseg`:			create an Excel table with all `aseg` measurements
      `aparc`:			create an Excel table with all `aparc` measurements
-     hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+     `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
      `snapshot`:		download a snapshot from the `recon-all` pipeline
      `report`:			download the validation report issued by bbrc-validator
      `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx freesurfer6hires <subcommand> <resource_id>
 
@@ -244,20 +244,20 @@
 
 FreeSurfer v7.1.1
 
     Available subcommands:
      `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
      `aseg`:			create an Excel table with all `aseg` measurements
      `aparc`:			create an Excel table with all `aparc` measurements
-     amygNucVolumes:	save an Excel table with amygdalar volumes
+     `amygNucVolumes`:	save an Excel table with amygdalar volumes
      `brainstem`:		save an Excel table with brainstem substructures volumes
      `thalamus`:		save an Excel table with thalamic nuclei volumes
-     hypothalamus:		save an Excel table with hypothalamic subunits volumes
+     `hypothalamus`:	save an Excel table with hypothalamic subunits volumes
      `jack`:			compute the cortical AD signature with FS7 results
-     hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+     `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
      `snapshot`:		download a snapshot from the `recon-all` pipeline
      `report`:			download the validation report issued by bbrc-validator
      `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx freesurfer7 <subcommand> <resource_id>
 
@@ -292,15 +292,15 @@
      bx lists <subcommand>
 
 ### **`MRTRIX3`**:
 
 MRtrix3 - Diffusion MRI tractography and structural connectivity.
 
     Available subcommands:
-     connectome:	download the structural connectivity matrices (Desikan-Killiany atlas)
+     `connectome`:	download the structural connectivity matrices (Desikan-Killiany atlas)
      `files`:		download all MRTRIX3 outputs (streamlines, segmentations, everything...)
      `report`:		download the validation report issued by `MRtrix3Validator`
      `snapshot`:	download snapshots from the MRTRIX3 pipeline
      `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
      bx mrtrix3 <subcommand> <resource_id>
@@ -339,15 +339,15 @@
     - Landau et al., Ann Neurol., 2012
 
 ### **`FTM`**:
 
 18F-flutemetamol PET imaging data
 
     Available subcommands:
-     centiloids:	creates an Excel table with centiloid scales
+     `centiloids`:	creates an Excel table with centiloid scales
      `maps`:		download the normalized FTM maps
      `tests`:		collect all automatic tests outcomes from `PetSessionValidator`
      `mri`:			creates an Excel table with details from associated MRI sessions
 
     Usage:
      bx ftm <subcommand> <resource_id>
 
@@ -429,18 +429,35 @@
      `report`:		download the validation report issued by `SPM12Validator`
      `tests`:		creates an Excel table with all automatic tests outcomes from `SPM12`
      `rc`:			downloads rc* files (DARTEL imports)
 
     Usage:
      bx spm12 <subcommand> <resource_id>
 
+### **`XCPD`**:
+
+XCP-D - Resting State fMRI postprocessing and functional connectivity.
+
+    Available subcommands:
+     `conmat`:          download the functional connectivity matrix (Desikan-Killiany atlas)
+     `timeseries`:      download the parcellated BOLD time-series (Desikan-Killiany atlas)
+     `files`:           download all XCP_D outputs (denoised BOLD data, segmentations, everything...)
+     `report`:          download the validation report issued by `XCPDValidator`
+     `snapshot`:        download snapshots from the XCPD pipeline
+     `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx xcpd <subcommand> <resource_id>
+
+    References:
+    - Ciric R, et al., Nat Protoc 13 (2018).
 
 ## Dependencies
 
-Requires [`bbrc-pyxnat>=1.4.2`](https://gitlab.com/pyxnat/pyxnat/tree/bbrc) and
+Requires [`bbrc-pyxnat>=1.6.1`](https://gitlab.com/pyxnat/pyxnat/tree/bbrc) and
 the librairies listed in `requirements.txt`.
 
 
 ## Install
 
 ```
 pip install bbrc-bx
```

### Comparing `bbrc-bx-0.5.1/bbrc_bx.egg-info/PKG-INFO` & `bbrc-bx-0.5.2/bbrc_bx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5.1
+Version: 0.5.2
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.1/bx-v0.5.1.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.2/bx-v0.5.2.tar.gz
 Description: # bx
         
         [![pipeline status](https://gitlab.com/bbrc/xnat/bx/badges/master/pipeline.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![coverage report](https://gitlab.com/bbrc/xnat/bx/badges/master/coverage.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![downloads](https://img.shields.io/pypi/dm/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![python versions](https://img.shields.io/pypi/pyversions/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![pypi version](https://img.shields.io/pypi/v/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
@@ -221,15 +221,15 @@
         
         FreeSurfer v6.0.0
         
             Available subcommands:
              `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
              `aseg`:			create an Excel table with all `aseg` measurements
              `aparc`:			create an Excel table with all `aparc` measurements
-             hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+             `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
              `snapshot`:		download a snapshot from the `recon-all` pipeline
              `report`:			download the validation report issued by bbrc-validator
              `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx freesurfer6 <subcommand> <resource_id>
         
@@ -237,15 +237,15 @@
         
         FreeSurfer v6.0.0 (-hires option)
         
             Available subcommands:
              `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
              `aseg`:			create an Excel table with all `aseg` measurements
              `aparc`:			create an Excel table with all `aparc` measurements
-             hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+             `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
              `snapshot`:		download a snapshot from the `recon-all` pipeline
              `report`:			download the validation report issued by bbrc-validator
              `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx freesurfer6hires <subcommand> <resource_id>
         
@@ -253,20 +253,20 @@
         
         FreeSurfer v7.1.1
         
             Available subcommands:
              `files`:			download all `recon-all` outputs (segmentation maps, files, everything...)
              `aseg`:			create an Excel table with all `aseg` measurements
              `aparc`:			create an Excel table with all `aparc` measurements
-             amygNucVolumes:	save an Excel table with amygdalar volumes
+             `amygNucVolumes`:	save an Excel table with amygdalar volumes
              `brainstem`:		save an Excel table with brainstem substructures volumes
              `thalamus`:		save an Excel table with thalamic nuclei volumes
-             hypothalamus:		save an Excel table with hypothalamic subunits volumes
+             `hypothalamus`:	save an Excel table with hypothalamic subunits volumes
              `jack`:			compute the cortical AD signature with FS7 results
-             hippoSfVolumes:	save an Excel table with hippocampal subfield volumes
+             `hippoSfVolumes`:	save an Excel table with hippocampal subfield volumes
              `snapshot`:		download a snapshot from the `recon-all` pipeline
              `report`:			download the validation report issued by bbrc-validator
              `tests`:			create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx freesurfer7 <subcommand> <resource_id>
         
@@ -301,15 +301,15 @@
              bx lists <subcommand>
         
         ### **`MRTRIX3`**:
         
         MRtrix3 - Diffusion MRI tractography and structural connectivity.
         
             Available subcommands:
-             connectome:	download the structural connectivity matrices (Desikan-Killiany atlas)
+             `connectome`:	download the structural connectivity matrices (Desikan-Killiany atlas)
              `files`:		download all MRTRIX3 outputs (streamlines, segmentations, everything...)
              `report`:		download the validation report issued by `MRtrix3Validator`
              `snapshot`:	download snapshots from the MRTRIX3 pipeline
              `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
         
             Usage:
              bx mrtrix3 <subcommand> <resource_id>
@@ -348,15 +348,15 @@
             - Landau et al., Ann Neurol., 2012
         
         ### **`FTM`**:
         
         18F-flutemetamol PET imaging data
         
             Available subcommands:
-             centiloids:	creates an Excel table with centiloid scales
+             `centiloids`:	creates an Excel table with centiloid scales
              `maps`:		download the normalized FTM maps
              `tests`:		collect all automatic tests outcomes from `PetSessionValidator`
              `mri`:			creates an Excel table with details from associated MRI sessions
         
             Usage:
              bx ftm <subcommand> <resource_id>
         
@@ -438,18 +438,35 @@
              `report`:		download the validation report issued by `SPM12Validator`
              `tests`:		creates an Excel table with all automatic tests outcomes from `SPM12`
              `rc`:			downloads rc* files (DARTEL imports)
         
             Usage:
              bx spm12 <subcommand> <resource_id>
         
+        ### **`XCPD`**:
+        
+        XCP-D - Resting State fMRI postprocessing and functional connectivity.
+        
+            Available subcommands:
+             `conmat`:          download the functional connectivity matrix (Desikan-Killiany atlas)
+             `timeseries`:      download the parcellated BOLD time-series (Desikan-Killiany atlas)
+             `files`:           download all XCP_D outputs (denoised BOLD data, segmentations, everything...)
+             `report`:          download the validation report issued by `XCPDValidator`
+             `snapshot`:        download snapshots from the XCPD pipeline
+             `tests`:           create an Excel table with all automatic tests outcomes from bbrc-validator
+        
+            Usage:
+             bx xcpd <subcommand> <resource_id>
+        
+            References:
+            - Ciric R, et al., Nat Protoc 13 (2018).
         
         ## Dependencies
         
-        Requires [`bbrc-pyxnat>=1.4.2`](https://gitlab.com/pyxnat/pyxnat/tree/bbrc) and
+        Requires [`bbrc-pyxnat>=1.6.1`](https://gitlab.com/pyxnat/pyxnat/tree/bbrc) and
         the librairies listed in `requirements.txt`.
         
         
         ## Install
         
         ```
         pip install bbrc-bx
```

### Comparing `bbrc-bx-0.5.1/bbrc_bx.egg-info/SOURCES.txt` & `bbrc-bx-0.5.2/bbrc_bx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 bx/parse.py
 bx/pet.py
 bx/qsmxt.py
 bx/scandates.py
 bx/signature.py
 bx/spm12.py
 bx/validation.py
+bx/xcpd.py
 bx/xnat.py
 bx/data/logo
 bx/data/aal2/AAL2.nii
 bx/data/braak/Braak_III_IV.nii.gz
 bx/data/braak/Braak_I_II.nii.gz
 bx/data/braak/Braak_V_VI.nii.gz
 bx/data/dickerson/ad/lh.adsig.annot
@@ -84,9 +85,8 @@
 bx/data/dickerson/aging/rh.cmfg.label
 bx/data/dickerson/aging/rh.cuneus.label
 bx/data/dickerson/aging/rh.ifg.label
 bx/data/dickerson/aging/rh.loccip.label
 bx/data/dickerson/aging/rh.msfg.label
 bx/data/dickerson/aging/rh.precent.label
 bx/data/dickerson/aging/rh.smg.label
-bx/data/masks/fdg_aging_mask.nii
-bx/data/mrtrix3/fs_default.txt
+bx/data/masks/fdg_aging_mask.nii
```

### Comparing `bbrc-bx-0.5.1/bin/bx` & `bbrc-bx-0.5.2/bin/bx`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bin/dump` & `bbrc-bx-0.5.2/bin/dump`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/ants.py` & `bbrc-bx-0.5.2/bx/ants.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/archiving.py` & `bbrc-bx-0.5.2/bx/archiving.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/ashs.py` & `bbrc-bx-0.5.2/bx/ashs.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/bamos.py` & `bbrc-bx-0.5.2/bx/bamos.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/basil.py` & `bbrc-bx-0.5.2/bx/basil.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/braak.py` & `bbrc-bx-0.5.2/bx/braak.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/cache.py` & `bbrc-bx-0.5.2/bx/cache.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/cat12.py` & `bbrc-bx-0.5.2/bx/cat12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/command.py` & `bbrc-bx-0.5.2/bx/command.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/dartel.py` & `bbrc-bx-0.5.2/bx/dartel.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/aal2/AAL2.nii` & `bbrc-bx-0.5.2/bx/data/aal2/AAL2.nii`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/braak/Braak_III_IV.nii.gz` & `bbrc-bx-0.5.2/bx/data/braak/Braak_III_IV.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/braak/Braak_I_II.nii.gz` & `bbrc-bx-0.5.2/bx/data/braak/Braak_I_II.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/braak/Braak_V_VI.nii.gz` & `bbrc-bx-0.5.2/bx/data/braak/Braak_V_VI.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.annot` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ag.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ifs.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.itg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.mtl.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.precun.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.sfg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.smg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.spl.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.tpole.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/lh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.annot` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ag.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ifs.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.itg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.mtl.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.precun.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.sfg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.smg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.spl.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.tpole.label` & `bbrc-bx-0.5.2/bx/data/dickerson/ad/rh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ag.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.calcarine.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cfusi.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cinsula.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cmfg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cuneus.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ifg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.loccip.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.msfg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.precent.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.smg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ag.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.calcarine.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cfusi.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cinsula.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cmfg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cuneus.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ifg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.loccip.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.msfg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.precent.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.smg.label` & `bbrc-bx-0.5.2/bx/data/dickerson/aging/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/data/masks/fdg_aging_mask.nii` & `bbrc-bx-0.5.2/bx/data/masks/fdg_aging_mask.nii`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/dcm.py` & `bbrc-bx-0.5.2/bx/dcm.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/donsurf.py` & `bbrc-bx-0.5.2/bx/donsurf.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/download.py` & `bbrc-bx-0.5.2/bx/download.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/dtifit.py` & `bbrc-bx-0.5.2/bx/dtifit.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/dump.py` & `bbrc-bx-0.5.2/bx/dump.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/freesurfer.py` & `bbrc-bx-0.5.2/bx/freesurfer.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/id.py` & `bbrc-bx-0.5.2/bx/id.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/lists.py` & `bbrc-bx-0.5.2/bx/lists.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/mrtrix3.py` & `bbrc-bx-0.5.2/bx/xcpd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,93 @@
 from bx.command import Command
 from bx import download as dl
-import os
 import logging as log
 
 
-class MRtrix3Command(Command):
-    """MRtrix3 - Diffusion MRI tractography and structural connectivity.
+class XCPDCommand(Command):
+    """XCP-D - Resting State fMRI postprocessing and functional connectivity.
 
     Available subcommands:
-     connectome:\tdownload the structural connectivity matrices (Desikan-Killiany atlas)
-     files:\t\tdownload all MRTRIX3 outputs (streamlines, segmentations, everything...)
-     report:\t\tdownload the validation report issued by `MRtrix3Validator`
-     snapshot:\t\tdownload snapshots from the MRTRIX3 pipeline
+     conmat:\t\tdownload the functional connectivity matrix (Desikan-Killiany atlas)
+     timeseries:\tdownload the parcellated BOLD time-series (Desikan-Killiany atlas)
+     files:\t\tdownload all XCP_D outputs (denoised BOLD data, segmentations, everything...)
+     report:\t\tdownload the validation report issued by `XCPDValidator`
+     snapshot:\t\tdownload snapshots from the XCPD pipeline
      tests:\t\tcreate an Excel table with all automatic tests outcomes from bbrc-validator
 
     Usage:
-     bx mrtrix3 <subcommand> <resource_id>
+     bx xcpd <subcommand> <resource_id>
 
     References:
-    - Tournier JD et al., NeuroImage 202 (2019).
+    - Ciric R, et al., Nat Protoc 13 (2018).
     """
     nargs = 2
-    resource_name = 'MRTRIX3'
-    subcommands = ['connectome', 'files', 'report', 'snapshot', 'tests']
-    validator = 'MRtrix3Validator'
-    url = 'https://gitlab.com/bbrc/xnat/docker-images/-/tree/master/mrtrix3'
+    resource_name = 'XCP_D'
+    subcommands = ['conmat', 'timeseries', 'files', 'report', 'snapshot', 'tests']
+    validator = 'XCPDValidator'
+    url = 'https://gitlab.com/bbrc/xnat/docker-images/-/tree/master/xcp_d'
 
     def __init__(self, *args, **kwargs):
-        super(MRtrix3Command, self).__init__(*args, **kwargs)
+        super(XCPDCommand, self).__init__(*args, **kwargs)
 
     def parse(self):
         subcommand = self.args[0]
         id = self.args[1]
 
-        if subcommand == 'connectome':
-            self.run_id(id, download_connectome, resource_name=self.resource_name,
+        if subcommand == 'conmat':
+            self.run_id(id, download_conmat, resource_name=self.resource_name,
+                        destdir=self.destdir)
+        elif subcommand == 'timeseries':
+            self.run_id(id, download_ts, resource_name=self.resource_name,
                         destdir=self.destdir)
-
         elif subcommand in ['files', 'report', 'snapshot']:
             self.run_id(id, dl.download, resource_name=self.resource_name,
                         validator=self.validator, destdir=self.destdir,
                         subcommand=subcommand)
 
         elif subcommand == 'tests':
             version = ['f0eefa95', '*']
             from bx import validation as val
             df = self.run_id(id, val.validation_scores,
                              validator=self.validator,
                              version=version, max_rows=25)
             self.to_excel(df)
 
 
-def download_connectome(x, experiments, resource_name, destdir):
-    import bx
-    import pandas as pd
+def download_conmat(x, experiments, resource_name, destdir, atlas='DK'):
     import os.path as op
     from tqdm import tqdm
-    from io import StringIO
 
-    labels_fp = op.join(op.dirname(bx.__file__), 'data',
-                        'mrtrix3', 'fs_default.txt')
+    for e in tqdm(experiments):
+        log.debug('Experiment %s:' % e['ID'])
+
+        r = x.select.experiment(e['ID']).resource(resource_name)
+        try:
+            df = r.conmat(atlas)
+        except StopIteration:
+            log.error('Failed for %s. Skipping it.' % e['ID'])
+            continue
 
-    with open(labels_fp, mode='r') as f:
-        data = [ln.split() for ln in f.read().splitlines()
-                if ln and ln[0] not in ['#', '0'] and '-Proper ' not in ln]
-    cols = ['label_index', 'label_code', 'label', 'R', 'G', 'B', 'n_colors']
-    dk_lut = pd.DataFrame(data, columns=cols)
+        fn = '{}_{}_{}_xcpd_{}_conmat.xlsx'.format(e['subject_label'],
+                                                   e['label'], e['ID'],
+                                                   atlas)
+        df.to_excel(op.join(destdir, fn))
 
-    filename = 'connectome.csv'
+
+def download_ts(x, experiments, resource_name, destdir, atlas='DK'):
+    import os.path as op
+    from tqdm import tqdm
 
     for e in tqdm(experiments):
         log.debug('Experiment %s:' % e['ID'])
 
         r = x.select.experiment(e['ID']).resource(resource_name)
-        f = r.file(filename)
-
-        fn = '{}_{}_{}_mrtrix3_connectome.xlsx'.format(e['subject_label'],
-                                                       e['label'], e['ID'])
-        if f.exists():
-            content = x.get(f._uri).content.decode('utf-8')
-            df = pd.read_csv(StringIO(content), names=dk_lut.label, header=None)
-            df.index = df.columns
-            df.to_excel(op.join(destdir, fn))
-
-        else:
+        try:
+            df = r.timeseries(atlas)
+        except StopIteration:
             log.error('Failed for %s. Skipping it.' % e['ID'])
+            continue
+
+        fn = '{}_{}_{}_xcpd_{}_timeseries.xlsx'.format(e['subject_label'],
+                                                       e['label'], e['ID'],
+                                                       atlas)
+        df.to_excel(op.join(destdir, fn), index=False)
```

### Comparing `bbrc-bx-0.5.1/bx/nifti.py` & `bbrc-bx-0.5.2/bx/nifti.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/parse.py` & `bbrc-bx-0.5.2/bx/parse.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/pet.py` & `bbrc-bx-0.5.2/bx/pet.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/qsmxt.py` & `bbrc-bx-0.5.2/bx/qsmxt.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/scandates.py` & `bbrc-bx-0.5.2/bx/scandates.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/signature.py` & `bbrc-bx-0.5.2/bx/signature.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/spm12.py` & `bbrc-bx-0.5.2/bx/spm12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/validation.py` & `bbrc-bx-0.5.2/bx/validation.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/bx/xnat.py` & `bbrc-bx-0.5.2/bx/xnat.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5.1/setup.py` & `bbrc-bx-0.5.2/setup.py`

 * *Files identical despite different names*

