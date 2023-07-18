# Comparing `tmp/savic-0.0.3.tar.gz` & `tmp/savic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "savic-0.0.3.tar", last modified: Sat May 13 21:59:11 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `savic-0.0.3.tar` & `savic-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 21:59:11.145744 savic-0.0.3/
--rw-rw-rw-   0        0        0      755 2023-05-13 21:59:11.145244 savic-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-13 21:58:23.000000 savic-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-13 21:59:11.144744 savic-0.0.3/savic.egg-info/
--rw-rw-rw-   0        0        0      755 2023-05-13 21:59:11.000000 savic-0.0.3/savic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-13 21:59:11.000000 savic-0.0.3/savic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 21:59:11.000000 savic-0.0.3/savic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-13 21:59:11.000000 savic-0.0.3/savic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 21:59:11.000000 savic-0.0.3/savic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 21:59:11.145744 savic-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1310 2023-05-13 21:58:51.000000 savic-0.0.3/setup.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_C.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_CA.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_CB.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_CBA.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Core.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_CoreAlpha.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_CoreBeam.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_CoreBeamAlpha.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Input_Sort.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_C.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_CA.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_CB.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_CBA.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_C.py
+-rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_CA.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_CB.py
+-rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_CBA.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_C/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_CA/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_CB/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_CBA/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/tutorial/00_dummy.txt
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 savic-0.9.0/LICENSE
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 savic-0.9.0/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 savic-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 savic-0.9.0/PKG-INFO
```

