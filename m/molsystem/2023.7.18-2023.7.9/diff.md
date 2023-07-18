# Comparing `tmp/molsystem-2023.7.18.tar.gz` & `tmp/molsystem-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molsystem-2023.7.18.tar", last modified: Tue Jul 18 18:48:34 2023, max compression
+gzip compressed data, was "molsystem-2023.7.9.tar", last modified: Mon Jul 10 17:31:09 2023, max compression
```

## Comparing `molsystem-2023.7.18.tar` & `molsystem-2023.7.9.tar`

### file list

```diff
@@ -1,106 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.560005 molsystem-2023.7.18/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 18:48:21.000000 molsystem-2023.7.18/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-18 18:48:21.000000 molsystem-2023.7.18/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-18 18:48:21.000000 molsystem-2023.7.18/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-18 18:48:21.000000 molsystem-2023.7.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-18 18:48:21.000000 molsystem-2023.7.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-18 18:48:34.560005 molsystem-2023.7.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-18 18:48:21.000000 molsystem-2023.7.18/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.540005 molsystem-2023.7.18/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.544005 molsystem-2023.7.18/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.544005 molsystem-2023.7.18/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.544005 molsystem-2023.7.18/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.544005 molsystem-2023.7.18/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.544005 molsystem-2023.7.18/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 18:48:21.000000 molsystem-2023.7.18/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.564005 molsystem-2023.7.18/molsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 18:48:34.564005 molsystem-2023.7.18/molsystem/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    33626 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/cms_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/configuration_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.552005 molsystem-2023.7.18/molsystem/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/data/standard_properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/frozencolumn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/inchi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/molfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/openbabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    28940 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/rdkit_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    32852 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/system_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/system_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-07-18 18:48:21.000000 molsystem-2023.7.18/molsystem/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.552005 molsystem-2023.7.18/molsystem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-18 18:48:34.000000 molsystem-2023.7.18/molsystem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-18 18:48:34.000000 molsystem-2023.7.18/molsystem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:48:34.000000 molsystem-2023.7.18/molsystem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 18:48:34.000000 molsystem-2023.7.18/molsystem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:48:34.000000 molsystem-2023.7.18/molsystem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 18:48:34.560005 molsystem-2023.7.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-18 18:48:21.000000 molsystem-2023.7.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.560005 molsystem-2023.7.18/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:48:34.560005 molsystem-2023.7.18/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269083 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/data/1n9v.cif
--rw-r--r--   0 runner    (1001) docker     (123)  1055288 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/data/aa-variants-v1.cif
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/data/acy.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)   117392 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/data/aminoacids.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/data/hoh.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_angiotensin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_configuration_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_inchi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_molfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_openbabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_property_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_rdkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_system_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-18 18:48:21.000000 molsystem-2023.7.18/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-18 18:48:21.000000 molsystem-2023.7.18/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.740878 molsystem-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 17:30:46.000000 molsystem-2023.7.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-10 17:30:46.000000 molsystem-2023.7.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-10 17:30:46.000000 molsystem-2023.7.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-10 17:30:46.000000 molsystem-2023.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-10 17:30:46.000000 molsystem-2023.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-10 17:31:09.740878 molsystem-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-10 17:30:46.000000 molsystem-2023.7.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.744878 molsystem-2023.7.9/molsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 17:31:09.744878 molsystem-2023.7.9/molsystem/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33626 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cms_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/configuration_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.732878 molsystem-2023.7.9/molsystem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/data/standard_properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/frozencolumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/molfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28940 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/rdkit_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32852 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.732878 molsystem-2023.7.9/molsystem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 17:31:09.740878 molsystem-2023.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-10 17:30:46.000000 molsystem-2023.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.736878 molsystem-2023.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.740878 molsystem-2023.7.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269083 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/1n9v.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  1055288 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/aa-variants-v1.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/acy.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)   117392 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/aminoacids.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/hoh.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_angiotensin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_configuration_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_molfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_property_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_system_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-10 17:30:46.000000 molsystem-2023.7.9/versioneer.py
```

### Comparing `molsystem-2023.7.18/CONTRIBUTING.rst` & `molsystem-2023.7.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/HISTORY.rst` & `molsystem-2023.7.9/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 =======
 History
 =======
 
-2023.7.18 -- Added support for InChI and InChIKeys
-
 2023.7.9 -- Added JSON properties
-    * Added properties stored as JSON, which allows, vectors, tensors, etc.
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
       
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.7.18/LICENSE` & `molsystem-2023.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/PKG-INFO` & `molsystem-2023.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2023.7.18
+Version: 2023.7.9
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -110,18 +110,16 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.18 -- Added support for InChI and InChIKeys
-
 2023.7.9 -- Added JSON properties
-    * Added properties stored as JSON, which allows, vectors, tensors, etc.
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
       
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.7.18/README.rst` & `molsystem-2023.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/Makefile` & `molsystem-2023.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/_static/SEAMM inverted.png` & `molsystem-2023.7.9/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/_static/SEAMM logo.png` & `molsystem-2023.7.9/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/_static/molssi_main_logo.png` & `molsystem-2023.7.9/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/_static/molssi_main_logo_inverted_white.png` & `molsystem-2023.7.9/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/_static/molssi_square.png` & `molsystem-2023.7.9/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/_static/nsf.png` & `molsystem-2023.7.9/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/conf.py` & `molsystem-2023.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/developer_guide/installation.rst` & `molsystem-2023.7.9/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/getting_started/index.rst` & `molsystem-2023.7.9/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/index.rst` & `molsystem-2023.7.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/make.bat` & `molsystem-2023.7.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/docs/user_guide/index.rst` & `molsystem-2023.7.9/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/__init__.py` & `molsystem-2023.7.9/molsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/atoms.py` & `molsystem-2023.7.9/molsystem/atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/bonds.py` & `molsystem-2023.7.9/molsystem/bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/cell.py` & `molsystem-2023.7.9/molsystem/cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/cif.py` & `molsystem-2023.7.9/molsystem/cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/cms_schema.py` & `molsystem-2023.7.9/molsystem/cms_schema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/column.py` & `molsystem-2023.7.9/molsystem/column.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/configuration.py` & `molsystem-2023.7.9/molsystem/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from .atoms import _Atoms
 from .bonds import _Bonds
 from .cell import _Cell
 from .cif import CIFMixin
 from .cms_schema import CMSSchemaMixin
 from .configuration_properties import _ConfigurationProperties
-from .inchi import InChIMixin
 from .molfile import MolFileMixin
 from .openbabel import OpenBabelMixin
 from .rdkit_ import RDKitMixin
 from .pdb import PDBMixin
 from .qcschema import QCSchemaMixin
 from .smiles import SMILESMixin
 from .subsets import _Subsets
@@ -30,15 +29,14 @@
 
 
 class _Configuration(
     PDBMixin,
     MolFileMixin,
     CIFMixin,
     CMSSchemaMixin,
-    InChIMixin,
     SMILESMixin,
     TopologyMixin,
     OpenBabelMixin,
     RDKitMixin,
     QCSchemaMixin,
     object,
 ):
```

### Comparing `molsystem-2023.7.18/molsystem/configuration_properties.py` & `molsystem-2023.7.9/molsystem/configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/data/standard_properties.csv` & `molsystem-2023.7.9/molsystem/data/standard_properties.csv`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/elements.py` & `molsystem-2023.7.9/molsystem/elements.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/frozencolumn.py` & `molsystem-2023.7.9/molsystem/frozencolumn.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/molfile.py` & `molsystem-2023.7.9/molsystem/molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/openbabel.py` & `molsystem-2023.7.9/molsystem/openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/pdb.py` & `molsystem-2023.7.9/molsystem/pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/properties.py` & `molsystem-2023.7.9/molsystem/properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/qcschema.py` & `molsystem-2023.7.9/molsystem/qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/rdkit_.py` & `molsystem-2023.7.9/molsystem/rdkit_.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/smiles.py` & `molsystem-2023.7.9/molsystem/smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/subset.py` & `molsystem-2023.7.9/molsystem/subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 import logging
 
 from .atoms import _SubsetAtoms
 from .bonds import _SubsetBonds
-from .inchi import InChIMixin
 from .openbabel import OpenBabelMixin
 from .smiles import SMILESMixin
 from .template import _Template
 
 logger = logging.getLogger(__name__)
 
 
-class _Subset(InChIMixin, SMILESMixin, OpenBabelMixin, object):
+class _Subset(SMILESMixin, OpenBabelMixin, object):
     """A class providing the API for a subset.
 
     Parameters
     ----------
     sid : int
         The id of the subset in the subset table.
     logger : logging.Logger = logger
```

### Comparing `molsystem-2023.7.18/molsystem/subsets.py` & `molsystem-2023.7.9/molsystem/subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/symmetry.py` & `molsystem-2023.7.9/molsystem/symmetry.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/system.py` & `molsystem-2023.7.9/molsystem/system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/system_db.py` & `molsystem-2023.7.9/molsystem/system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/system_properties.py` & `molsystem-2023.7.9/molsystem/system_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/table.py` & `molsystem-2023.7.9/molsystem/table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/template.py` & `molsystem-2023.7.9/molsystem/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 import logging
 
-from .inchi import InChIMixin
 from .openbabel import OpenBabelMixin
 from .smiles import SMILESMixin
 
 logger = logging.getLogger(__name__)
 
 
-class _Template(InChIMixin, SMILESMixin, OpenBabelMixin, object):
+class _Template(SMILESMixin, OpenBabelMixin, object):
     """A class providing the API for templates.
 
     There are two types of templates:
 
     simple
         Which have a category and name, which together are unique.
     full
```

### Comparing `molsystem-2023.7.18/molsystem/templates.py` & `molsystem-2023.7.9/molsystem/templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem/topology.py` & `molsystem-2023.7.9/molsystem/topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/molsystem.egg-info/PKG-INFO` & `molsystem-2023.7.9/molsystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2023.7.18
+Version: 2023.7.9
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -110,18 +110,16 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
-2023.7.18 -- Added support for InChI and InChIKeys
-
 2023.7.9 -- Added JSON properties
-    * Added properties stored as JSON, which allows, vectors, tensors, etc.
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
       
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.7.18/molsystem.egg-info/SOURCES.txt` & `molsystem-2023.7.9/molsystem.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 molsystem/cif.py
 molsystem/cms_schema.py
 molsystem/column.py
 molsystem/configuration.py
 molsystem/configuration_properties.py
 molsystem/elements.py
 molsystem/frozencolumn.py
-molsystem/inchi.py
 molsystem/molfile.py
 molsystem/openbabel.py
 molsystem/pdb.py
 molsystem/properties.py
 molsystem/qcschema.py
 molsystem/rdkit_.py
 molsystem/smiles.py
@@ -67,15 +66,14 @@
 tests/test_angiotensin.py
 tests/test_atoms.py
 tests/test_bonds.py
 tests/test_cell.py
 tests/test_cif.py
 tests/test_configuration_properties.py
 tests/test_configurations.py
-tests/test_inchi.py
 tests/test_molfile.py
 tests/test_openbabel.py
 tests/test_pdb.py
 tests/test_properties.py
 tests/test_property_timings.py
 tests/test_rdkit.py
 tests/test_smiles.py
```

### Comparing `molsystem-2023.7.18/setup.py` & `molsystem-2023.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/conftest.py` & `molsystem-2023.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/data/1n9v.cif` & `molsystem-2023.7.9/tests/data/1n9v.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/data/aa-variants-v1.cif` & `molsystem-2023.7.9/tests/data/aa-variants-v1.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/data/acy.mmcif` & `molsystem-2023.7.9/tests/data/acy.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/data/aminoacids.mmcif` & `molsystem-2023.7.9/tests/data/aminoacids.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/data/hoh.mmcif` & `molsystem-2023.7.9/tests/data/hoh.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_angiotensin.py` & `molsystem-2023.7.9/tests/test_angiotensin.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_atoms.py` & `molsystem-2023.7.9/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_bonds.py` & `molsystem-2023.7.9/tests/test_bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_cell.py` & `molsystem-2023.7.9/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_cif.py` & `molsystem-2023.7.9/tests/test_cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_configuration_properties.py` & `molsystem-2023.7.9/tests/test_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_configurations.py` & `molsystem-2023.7.9/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_inchi.py` & `molsystem-2023.7.9/tests/test_smiles.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,72 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest  # noqa: F401
 
-"""Tests for handling InChI."""
+"""Tests for handling SMILES."""
 
 
-def test_to_inchi(AceticAcid):
-    """Create a InChI string from a system"""
-    correct = "InChI=1S/C2H4O2/c1-2(3)4/h1H3,(H,3,4)"
-    inchi = AceticAcid.to_inchi()
+def test_to_smiles(AceticAcid):
+    """Create a SMILES string from a system"""
+    correct = "CC(=O)O"
+    smiles = AceticAcid.to_smiles()
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
-def test_to_inchikey(AceticAcid):
-    """Create a InChIKey string from a system"""
-    correct = "QTBSBXVTEAMEQO-UHFFFAOYSA-N"
-    inchi = AceticAcid.to_inchi(key=True)
+def test_to_smiles_with_name(AceticAcid):
+    """Create a SMILES string from a system"""
+    correct = "CC(=O)O"
+    smiles = AceticAcid.smiles
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
-def test_to_inchi_with_name(AceticAcid):
-    """Create a InChI string from a system, adding the name"""
-    correct = "InChI=1S/C2H4O2/c1-2(3)4/h1H3,(H,3,4)"
-    inchi = AceticAcid.inchi
+def test_to_canonical_smiles(AceticAcid):
+    """Create a SMILES string from a system"""
+    correct = "CC(=O)O"
+    smiles = AceticAcid.to_smiles(canonical=True)
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
 def test_several_molecules(CH3COOH_3H2O):
     """System with acetic acid and 3 waters"""
     system = CH3COOH_3H2O
-    correct = "InChI=1S/C2H4O2.3H2O/c1-2(3)4;;;/h1H3,(H,3,4);3*1H2"
+    correct = "CC(=O)O.O.O.O"
+
+    smiles = system.to_smiles()
+
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
+
+
+def test_several_molecules_canonical(CH3COOH_3H2O):
+    """System with acetic acid and 3 waters"""
+    system = CH3COOH_3H2O
+    correct = "CC(=O)O.O.O.O"
 
-    inchi = system.to_inchi()
+    smiles = system.to_smiles(canonical=True)
 
-    if inchi != correct:
-        print(inchi)
-    assert inchi == correct
+    if smiles != correct:
+        print(smiles)
+    assert smiles == correct
 
 
-def test_from_inchi(configuration):
-    """Create a configuration from InChI"""
+def test_from_smiles(configuration):
+    """Create a configuration from SMILES"""
     correct = "CC(=O)O"
-    configuration.from_inchi(
-        "InChI=1S/C2H4O2/c1-2(3)4/h1H3,(H,3,4)", name="acetic acid"
-    )
+    configuration.from_smiles("OC(=O)C", name="acetic acid")
     result = configuration.to_smiles(canonical=True)
 
     if result != correct:
         print(result)
 
     assert result == correct
```

### Comparing `molsystem-2023.7.18/tests/test_molfile.py` & `molsystem-2023.7.9/tests/test_molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_openbabel.py` & `molsystem-2023.7.9/tests/test_openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_pdb.py` & `molsystem-2023.7.9/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_properties.py` & `molsystem-2023.7.9/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_property_timings.py` & `molsystem-2023.7.9/tests/test_property_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_rdkit.py` & `molsystem-2023.7.9/tests/test_rdkit.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_subsets.py` & `molsystem-2023.7.9/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_system.py` & `molsystem-2023.7.9/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_system_db.py` & `molsystem-2023.7.9/tests/test_system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_table.py` & `molsystem-2023.7.9/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_templates.py` & `molsystem-2023.7.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_timings.py` & `molsystem-2023.7.9/tests/test_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/tests/test_topology.py` & `molsystem-2023.7.9/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.7.18/versioneer.py` & `molsystem-2023.7.9/versioneer.py`

 * *Files identical despite different names*

