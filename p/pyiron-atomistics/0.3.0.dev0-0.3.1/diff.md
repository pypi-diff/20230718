# Comparing `tmp/pyiron-atomistics-0.3.0.dev0.tar.gz` & `tmp/pyiron-atomistics-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron-atomistics-0.3.0.dev0.tar", last modified: Thu Jul  6 07:54:58 2023, max compression
+gzip compressed data, was "pyiron-atomistics-0.3.1.tar", last modified: Tue Jul 18 08:24:17 2023, max compression
```

## Comparing `pyiron-atomistics-0.3.0.dev0.tar` & `pyiron-atomistics-0.3.1.tar`

### file list

```diff
@@ -1,151 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/structurecontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.592846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/convergence_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32965 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/murnaghan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/quasi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/sqsmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)   128325 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/atomsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20288 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/has_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyironase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/sparse_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    22405 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/structurestorage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34986 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/bader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/murnaghan_dft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/dos.py
--rw-r--r--   0 runner    (1001) docker     (123)    29606 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/electronic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/gpaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/pyiron_ase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/activation_relaxation_technique.py
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/quasi_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/scipy_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/sxextoptint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44523 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    41465 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    25776 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    26176 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99408 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/funct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/randomatomistic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/hessian.py
--rw-r--r--   0 runner    (1001) docker     (123)    51129 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/interfacemethod.py
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/sxphonons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   101289 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/metadyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/oszicar.py
--rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/outcar.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/procar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)    34363 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vaspsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-06 07:54:55.000000 pyiron-atomistics-0.3.0.dev0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 07:54:55.000000 pyiron-atomistics-0.3.0.dev0/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-06 07:54:55.000000 pyiron-atomistics-0.3.0.dev0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.790257 pyiron-atomistics-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-18 08:24:17.790257 pyiron-atomistics-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.790257 pyiron-atomistics-0.3.1/pyiron_atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 08:24:17.790257 pyiron-atomistics-0.3.1/pyiron_atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.766257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.766257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/generic/object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.766257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41952 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/structurecontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.770257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/convergence_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33764 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/quasi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/sqsmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.774257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124204 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.774257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/atomsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20288 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/has_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/pyironase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22356 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/structurestorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.774257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.774257 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/volumetric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/volumetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/volumetric/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.774257 pyiron-atomistics-0.3.1/pyiron_atomistics/calphy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/calphy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34986 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/calphy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.774257 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/bader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.778257 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/job/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.778257 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/convergence_encut_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/convergence_encut_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/murnaghan_dft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.778257 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29606 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/electronic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.778257 pyiron-atomistics-0.3.1/pyiron_atomistics/gpaw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/gpaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/gpaw/gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/gpaw/pyiron_ase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.778257 pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/activation_relaxation_technique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/quasi_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/scipy_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/sxextoptint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.782257 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44366 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41929 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25776 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26226 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.782257 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99824 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.782257 pyiron-atomistics-0.3.1/pyiron_atomistics/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/table/funct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.786257 pyiron-atomistics-0.3.1/pyiron_atomistics/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/testing/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/testing/randomatomistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.786257 pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51126 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/interfacemethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/sxphonons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.786257 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101263 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14988 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/metadyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/oszicar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/procar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34363 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/vaspsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-18 08:24:13.000000 pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.766257 pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-18 08:24:17.000000 pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-18 08:24:17.000000 pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:24:17.000000 pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-18 08:24:17.000000 pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 08:24:17.000000 pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 08:24:17.790257 pyiron-atomistics-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-18 08:24:17.000000 pyiron-atomistics-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:24:17.790257 pyiron-atomistics-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-18 08:24:14.000000 pyiron-atomistics-0.3.1/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 08:24:14.000000 pyiron-atomistics-0.3.1/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-18 08:24:14.000000 pyiron-atomistics-0.3.1/versioneer.py
```

### Comparing `pyiron-atomistics-0.3.0.dev0/LICENSE` & `pyiron-atomistics-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/PKG-INFO` & `pyiron-atomistics-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-atomistics
-Version: 0.3.0.dev0
+Version: 0.3.1
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron-atomistics-0.3.0.dev0/README.rst` & `pyiron-atomistics-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/__init__.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/_tests.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/object_type.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/generic/object_type.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/atomistic.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/atomistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -755,15 +755,15 @@
                 pbc=self.structure.pbc,
             )
         else:
             snapshot = self.structure.copy()
             if cell is not None:
                 snapshot.cell = cell
             if indices is not None:
-                snapshot.indices = indices
+                snapshot.set_array("indices", indices)
         if self.output.positions is not None:
             if wrap_atoms:
                 snapshot.positions = self.output.positions[frame]
                 snapshot.center_coordinates_in_unit_cell()
             elif len(self.output.unwrapped_positions) > max([frame, 0]):
                 snapshot.positions = self.output.unwrapped_positions[frame]
             else:
@@ -878,15 +878,15 @@
 
     def __getitem__(self, item):
         if isinstance(item, numbers.Integral):
             new_structure = self._structure.copy()
             if self._cells is not None:
                 new_structure.cell = self._cells[item]
             if self._indices is not None:
-                new_structure.indices = self._indices[item]
+                new_structure.set_array("indices", self._indices[item])
             new_structure.positions = self._positions[item]
             # This step is necessary for using ase.io.write for trajectories
             new_structure.arrays["positions"] = new_structure.positions
             # new_structure.arrays['cells'] = new_structure.cell
             return new_structure
         elif isinstance(item, (list, np.ndarray, slice)):
             snapshots = np.arange(len(self), dtype=int)[item]
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactive.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactivewrapper.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/potentials.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/potentials.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/sqs.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/sqs.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/structurecontainer.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/job/structurecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/convergence_volume.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/convergence_volume.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/elastic.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/elastic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/murnaghan.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/murnaghan.py`

 * *Files 3% similar despite different names*

```diff
@@ -675,14 +675,18 @@
             ["x", "y", "z"],
             "Axes along which the strain will be applied",
         )
         self.input["strains"] = (
             None,
             "List of strains that should be calculated.  If given vol_range and num_points take no effect.",
         )
+        self.input["allow_aborted"] = (
+            0,
+            "The number of child jobs that are allowed to abort, before the whole job is considered aborted.",
+        )
 
         self.debye_model = DebyeModel(self)
         self.fit_module = EnergyVolumeFit()
 
         self.fit_dict = None
         self._debye_T = None
         self._job_generator = MurnaghanJobGenerator(self)
@@ -805,27 +809,40 @@
             vol_lst = ham["output/generic/volume"]
             arg_lst = np.argsort(vol_lst)
 
             self._output["volume"] = vol_lst[arg_lst]
             self._output["energy"] = erg_lst[arg_lst]
         else:
             erg_lst, vol_lst, err_lst, id_lst = [], [], [], []
+            allowed_aborted_children = self.input.get("allow_aborted", 0)
             for job_id in self.child_ids:
                 ham = self.project_hdf5.inspect(job_id)
+                if ham.status == "aborted":
+                    if allowed_aborted_children == 0:
+                        raise ValueError(f"Child {ham.name}({job_id}) is aborted!")
+                    allowed_aborted_children -= 1
+                    continue
                 if "energy_tot" in ham["output/generic"].list_nodes():
                     energy = ham["output/generic/energy_tot"][-1]
                 elif "energy_pot" in ham["output/generic"].list_nodes():
                     energy = ham["output/generic/energy_pot"][-1]
                 else:
                     raise ValueError("Neither energy_pot or energy_tot was found.")
                 volume = ham["output/generic/volume"][-1]
                 erg_lst.append(np.mean(energy))
                 err_lst.append(np.var(energy))
                 vol_lst.append(volume)
                 id_lst.append(job_id)
+            aborted_children = (
+                self.input.get("allow_aborted") - allowed_aborted_children
+            )
+            if aborted_children > 0:
+                self.logger.warning(
+                    f"{aborted_children} aborted, but proceeding anyway."
+                )
             vol_lst = np.array(vol_lst)
             erg_lst = np.array(erg_lst)
             err_lst = np.array(err_lst)
             id_lst = np.array(id_lst)
             arg_lst = np.argsort(vol_lst)
 
             self._output["volume"] = vol_lst[arg_lst]
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/parallel.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/phonopy.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/phonopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         """
         Args:
             structure (pyiron.atomistics.structure.atoms): input structure
 
         Returns:
             structure (pyiron_atomistics.atomistics.structure.atoms): output structure with magnetic moments
         """
-        if any(self._master.structure.get_initial_magnetic_moments() != None):
+        if self._master.structure.has("initial_magmoms"):
             magmoms = self._master.structure.get_initial_magnetic_moments()
             magmoms = np.tile(
                 magmoms,
                 np.prod(np.diagonal(self._master._phonopy_supercell_matrix())).astype(
                     int
                 ),
             )
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/quasi.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/quasi.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/serial.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/serial.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/sqsmaster.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/sqsmaster.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/structure.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/master/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/analyse.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/analyse.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atom.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/atom.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from pyiron_atomistics.atomistics.structure.periodic_table import (
     PeriodicTable,
     ChemicalElement,
 )
-from pyiron_atomistics.atomistics.structure.sparse_list import SparseArrayElement
 from ase.atom import Atom as ASEAtom
 
 __author__ = "Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Aug 1, 2020"
 
 
-class Atom(ASEAtom, SparseArrayElement):
+class Atom(ASEAtom):
     """
     Class for representing a single atom derived from the `ASE atom class`_.
 
     Args:
         symbol (str/pyiron_atomistics.atomistics.structure.periodic_table.ChemcicalElement): Symbol or elecment object
         position (list/numpy.ndarray): Position of atom in cartesian coordinates
         tag (str): Tag assigned to structure
@@ -55,30 +54,27 @@
         pse=None,
         element=None,
         **qwargs
     ):
         if element is None:
             element = symbol
 
-        SparseArrayElement.__init__(self, **qwargs)
-        # super(SparseArrayElement, self).__init__(**qwargs)
-        # verify that element is given (as string, ChemicalElement object or nucleus number
         if pse is None:
             pse = PeriodicTable()
 
         if element is None or element == "X":
             if "Z" in qwargs:
                 el_symbol = pse.atomic_number_to_abbreviation(qwargs["Z"])
-                self._lists["element"] = pse.element(el_symbol)
+                qwargs["element"] = pse.element(el_symbol)
         else:
             if isinstance(element, str):
                 el_symbol = element
-                self._lists["element"] = pse.element(el_symbol)
+                qwargs["element"] = pse.element(el_symbol)
             elif isinstance(element, ChemicalElement):
-                self._lists["element"] = element
+                qwargs["element"] = element
             else:
                 raise ValueError("Unknown element type")
 
         # KeyError handling required for user defined elements
         try:
             ASEAtom.__init__(
                 self,
@@ -107,14 +103,20 @@
                 index=index,
             )
 
         # ASE compatibility for tags
         for key, val in qwargs.items():
             self.data[key] = val
 
+    def __getattr__(self, key):
+        try:
+            return self.data[key]
+        except KeyError:
+            raise AttributeError(key)
+
     @property
     def mass(self):
         """
         Gives the atomic mass of the atom
 
         Returns:
             float: The atomic mass in a.u.
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atoms.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from structuretoolkit.visualize import plot3d
 from pyiron_atomistics.atomistics.structure.atom import (
     Atom,
     ase_to_pyiron as ase_to_pyiron_atom,
 )
 from pyiron_atomistics.atomistics.structure.pyscal import pyiron_to_pyscal_system
 from pyiron_atomistics.atomistics.structure.analyse import Analyse
-from pyiron_atomistics.atomistics.structure.sparse_list import SparseArray, SparseList
 from pyiron_atomistics.atomistics.structure.periodic_table import (
     PeriodicTable,
     ChemicalElement,
 )
 from pyiron_base import state, deprecate
 from pymatgen.io.ase import AseAtomsAdaptor
 from collections.abc import Sequence
@@ -112,18 +111,15 @@
             or info is not None
         ):
             state.logger.debug("Not supported parameter used!")
 
         self._is_scaled = False
 
         self._species = list()
-        self.indices = np.array([])
-        self.constraints = None
         self._pse = PeriodicTable()
-        self._tag_list = SparseArray()
 
         el_index_lst = list()
         element_list = None
         if numbers is not None:  # for ASE compatibility
             if not (elements is None):
                 raise AssertionError()
             elements = self.numbers_to_elements(numbers)
@@ -177,21 +173,20 @@
             el_index_lst = indices
             if species is None:
                 raise ValueError(
                     "species must be given if indices is given, but is None."
                 )
             self.set_species(species)
 
-        self.indices = np.array(el_index_lst, dtype=int)
+        indices = np.array(el_index_lst, dtype=int)
 
         el_lst = [
             el.Abbreviation if el.Parent is None else el.Parent for el in self.species
         ]
-        symbols = np.array([el_lst[el] for el in self.indices])
-        self._tag_list._length = len(symbols)
+        symbols = np.array([el_lst[el] for el in indices])
         super(Atoms, self).__init__(
             symbols=symbols,
             positions=positions,
             numbers=None,
             tags=tags,
             momenta=momenta,
             masses=masses,
@@ -202,14 +197,16 @@
             pbc=pbc,
             celldisp=celldisp,
             constraint=constraint,
             calculator=calculator,
             info=info,
         )
 
+        self.set_array("indices", indices)
+
         self.bonds = None
         self.units = {"length": "A", "mass": "u"}
         self.set_initial_magnetic_moments(magmoms)
         self._high_symmetry_points = None
         self._high_symmetry_path = None
         self.dimension = dimension
         if len(self.positions) > 0:
@@ -269,15 +266,14 @@
     def species(self):
         """
         list: A list of atomistics.structure.periodic_table.ChemicalElement instances
 
         """
         return self._species
 
-    # @species.setter
     def set_species(self, value):
         """
         Setting the species list
 
         Args:
             value (list): A list atomistics.structure.periodic_table.ChemicalElement instances
 
@@ -398,26 +394,30 @@
                     if v not in self.get_high_symmetry_points().keys():
                         raise ValueError(
                             "'{}' is not a valid high symmetry point".format(v)
                         )
 
         self._high_symmetry_path.update(path)
 
+    @deprecate(
+        "Use Atoms.set_array() instead: e.g. Atoms.set_array('selective_dynamics', np.repeat([[True, True, False]], len(Atoms), axis=0))"
+    )
     def add_tag(self, **qwargs):
         """
         Add tags to the atoms object.
 
         Examples:
 
             For selective dynamics::
 
             >>> self.add_tag(selective_dynamics=[False, False, False])
 
         """
-        self._tag_list.add_tag(**qwargs)
+        for tag, value in qwargs.items():
+            self.set_array(tag, np.repeat([value], len(self), axis=0))
 
     # @staticmethod
     def numbers_to_elements(self, numbers):
         """
         Convert atomic numbers in element objects (needed for compatibility with ASE)
 
         Args:
@@ -461,18 +461,18 @@
                 if isinstance(el.tags, dict):
                     with hdf_structure.open("new_species") as hdf_species:
                         el.to_hdf(hdf_species)
             hdf_structure["species"] = [el.Abbreviation for el in self.species]
             hdf_structure["indices"] = self.indices
 
             with hdf_structure.open("tags") as hdf_tags:
-                for tag in self._tag_list.keys():
-                    tag_value = self._tag_list[tag]
-                    if isinstance(tag_value, SparseList):
-                        tag_value.to_hdf(hdf_tags, tag)
+                for tag, value in self.arrays.items():
+                    if tag in ["positions", "numbers", "indices"]:
+                        continue
+                    hdf_tags[tag] = value.tolist()
             hdf_structure["units"] = self.units
             hdf_structure["dimension"] = self.dimension
 
             if self.cell is not None:
                 with hdf_structure.open("cell") as hdf_cell:
                     # Convert ASE cell object to numpy array before storing
                     hdf_cell["cell"] = np.array(self.cell)
@@ -519,16 +519,15 @@
                 if "new_species" in hdf_atoms.list_groups():
                     with hdf_atoms.open("new_species") as hdf_species:
                         self._pse.from_hdf(hdf_species)
 
                 el_object_list = [
                     self.convert_element(el, self._pse) for el in hdf_atoms["species"]
                 ]
-                self.indices = hdf_atoms["indices"]
-                self._tag_list._length = len(self.indices)
+                self.arrays["indices"] = hdf_atoms["indices"]
 
                 self.set_species(el_object_list)
                 self.bonds = None
 
                 tr_dict = {1: True, 0: False}
                 self.dimension = hdf_atoms["dimension"]
                 self.units = hdf_atoms["units"]
@@ -556,32 +555,25 @@
                     self.bonds = hdf_atoms["explicit_bonds"]
                 if "spins" in hdf_atoms.list_nodes():
                     self.spins = hdf_atoms["spins"]
                 if "tags" in hdf_atoms.list_groups():
                     with hdf_atoms.open("tags") as hdf_tags:
                         tags = hdf_tags.list_nodes()
                         for tag in tags:
+                            if tag in ["initial_magmoms"]:
+                                continue
                             # tr_dict = {'0': False, '1': True}
                             if isinstance(hdf_tags[tag], (list, np.ndarray)):
                                 my_list = hdf_tags[tag]
-                                self._tag_list[tag] = SparseList(
-                                    my_list, length=len(self)
-                                )
-
-                            else:
+                            else:  # legacy of SparseList
                                 my_dict = hdf_tags.get_pandas(tag).to_dict()
-                                my_dict = {
-                                    i: val
-                                    for i, val in zip(
-                                        my_dict["index"], my_dict["values"]
-                                    )
-                                }
-                                self._tag_list[tag] = SparseList(
-                                    my_dict, length=len(self)
-                                )
+                                my_list = np.array(my_dict["values"])[
+                                    np.argsort(my_dict["index"])
+                                ]
+                            self.set_array(tag, np.asarray(my_list))
 
                 if "bonds" in hdf_atoms.list_nodes():
                     self.bonds = hdf_atoms["explicit_bonds"]
 
                 self._high_symmetry_points = None
                 if "high_symmetry_points" in hdf_atoms.list_nodes():
                     self._high_symmetry_points = hdf_atoms["high_symmetry_points"]
@@ -614,37 +606,35 @@
                 with hdf_atoms.open("species") as hdf_species:
                     self._pse.from_hdf(hdf_species)
             chemical_symbols = np.array(hdf_atoms["elements"], dtype=str)
             el_object_list = [
                 self.convert_element(el, self._pse) for el in chemical_symbols
             ]
             self.set_species(list(set(el_object_list)))
-            self.indices = [self._species_to_index_dict[el] for el in el_object_list]
-            self._tag_list._length = len(self)
+            self.set_array(
+                "indices", [self._species_to_index_dict[el] for el in el_object_list]
+            )
             self.bonds = None
             if "explicit_bonds" in hdf_atoms.list_nodes():
                 # print "bonds: "
                 self.bonds = hdf_atoms["explicit_bonds"]
 
             if "tags" in hdf_atoms.list_groups():
                 with hdf_atoms.open("tags") as hdf_tags:
                     tags = hdf_tags.list_nodes()
                     for tag in tags:
                         # tr_dict = {'0': False, '1': True}
                         if isinstance(hdf_tags[tag], (list, np.ndarray)):
                             my_list = hdf_tags[tag]
-                            self._tag_list[tag] = SparseList(my_list, length=len(self))
-
                         else:
                             my_dict = hdf_tags.get_pandas(tag).to_dict()
-                            my_dict = {
-                                i: val
-                                for i, val in zip(my_dict["index"], my_dict["values"])
-                            }
-                            self._tag_list[tag] = SparseList(my_dict, length=len(self))
+                            my_list = np.array(my_dict["values"])[
+                                np.argsort(my_dict["index"])
+                            ]
+                        self.set_array(tag, my_list)
 
             self.cell = None
             if "cell" in hdf_atoms.list_groups():
                 with hdf_atoms.open("cell") as hdf_cell:
                     self.cell = hdf_cell["cell"]
                     self.pbc = hdf_cell["pbc"]
 
@@ -703,15 +693,15 @@
         """
         Returns the keys of the stored tags of the structure
 
         Returns:
             dict_keys: Keys of the stored tags
 
         """
-        return self._tag_list.keys()
+        return self.arrays.keys()
 
     def convert_element(self, el, pse=None):
         """
         Convert a string or an atom instance into a ChemicalElement instance
 
         Args:
             el (str/atomistics.structure.atom.Atom): String or atom instance from which the element should
@@ -829,15 +819,15 @@
                 sym_list, return_index=True, return_inverse=True
             )
             new_species = new_species[ind].copy()
             parent_basis.set_species(list(new_species))
             indices_copy = parent_basis.indices.copy()
             for i, ind_ind in enumerate(inv_ind):
                 indices_copy[parent_basis.indices == i] = ind_ind
-            parent_basis.indices = indices_copy
+            parent_basis.set_array("indices", indices_copy)
             return parent_basis
         parent_basis.set_species(list(new_species))
         return parent_basis
 
     def get_chemical_elements(self):
         """
         Returns the list of chemical element instances
@@ -1063,14 +1053,15 @@
         )
 
         struc_new._set_high_symmetry_points(sp_dict["point_coords"])
         struc_new._set_high_symmetry_path({"full": sp_dict["path"]})
 
         return struc_new
 
+    @deprecate("Use Atoms.repeat")
     def set_repeat(self, vec):
         self *= vec
 
     def repeat_points(self, points, rep, centered=False):
         """
         Return points with repetition given according to periodic boundary conditions
 
@@ -1612,15 +1603,15 @@
                 delete_species_indices.append(i)
             else:
                 retain_species_indices.append(i)
         for i in delete_species_indices:
             new_indices[new_indices >= i] += -1
         new_species = np.array(new_species)[retain_species_indices]
         self.set_species(new_species)
-        self.indices = new_indices
+        self.set_array("indices", new_indices)
 
     @deprecate(
         "Use neigh.cluster_analysis() instead (after calling neigh = structure.get_neighbors())",
         version="1.0.0",
     )
     def cluster_analysis(
         self, id_list, neighbors=None, radius=None, return_cluster_sizes=False
@@ -2018,26 +2009,33 @@
         Args:
             other (pyiron_atomistics.atomistics.structure.atoms.Atoms/ase.atoms.Atoms): Structure to append
 
         Returns:
             pyiron.atomistics.structure.atoms.Atoms: The extended structure
 
         """
-        old_indices = self.indices
         if isinstance(other, Atom):
             other = self.__class__([other])
         elif isinstance(other, ASEAtom):
             other = self.__class__([ase_to_pyiron_atom(other)])
         if not isinstance(other, Atoms) and isinstance(other, ASEAtoms):
             warnings.warn(
                 "Converting ase structure to pyiron before appending the structure"
             )
             other = ase_to_pyiron(other)
 
-        new_indices = other.indices.copy()
+        d = self._store_elements.copy()
+        d.update(other._store_elements.copy())
+        chem, new_indices = np.unique(
+            self.get_chemical_symbols().tolist()
+            + other.get_chemical_symbols().tolist(),
+            return_inverse=True,
+        )
+        new_species = [d[c] for c in chem]
+
         super(Atoms, self).extend(other=other)
         if isinstance(other, Atoms):
             if not np.allclose(self.cell, other.cell):
                 warnings.warn(
                     "You are adding structures with different cell shapes. "
                     "Taking the cell and pbc of the first structure:{}".format(
                         self.cell
@@ -2046,36 +2044,17 @@
             if not np.array_equal(self.pbc, other.pbc):
                 warnings.warn(
                     "You are adding structures with different periodic boundary conditions. "
                     "Taking the cell and pbc of the first structure:{}".format(
                         self.cell
                     )
                 )
-            sum_atoms = self
-            # sum_atoms = copy(self)
-            sum_atoms._tag_list = sum_atoms._tag_list + other._tag_list
-            sum_atoms.indices = np.append(sum_atoms.indices, other.indices)
-            new_species_lst = copy(sum_atoms.species)
-            ind_conv = {}
-            for ind_old, el in enumerate(other.species):
-                if el.Abbreviation in sum_atoms._store_elements.keys():
-                    ind_new = sum_atoms._species_to_index_dict[
-                        sum_atoms._store_elements[el.Abbreviation]
-                    ]
-                    ind_conv[ind_old] = ind_new
-                else:
-                    new_species_lst.append(el)
-                    ind_conv[ind_old] = len(new_species_lst) - 1
-
-            for key, val in ind_conv.items():
-                new_indices[new_indices == key] = val + 1000
-            new_indices = np.mod(new_indices, 1000)
-            sum_atoms.indices[len(old_indices) :] = new_indices
-            sum_atoms.set_species(new_species_lst)
-            if not len(set(sum_atoms.indices)) == len(sum_atoms.species):
+            self.set_array("indices", new_indices)
+            self.set_species(new_species)
+            if not len(set(self.indices)) == len(self.species):
                 raise ValueError("Adding the atom instances went wrong!")
         return self
 
     __iadd__ = extend
 
     def __copy__(self):
         """
@@ -2093,47 +2072,33 @@
         for key, val in self.__dict__.items():
             if key not in ase_keys:
                 atoms_new.__dict__[key] = copy(val)
         atoms_new._analyse = Analyse(atoms_new)
         return atoms_new
 
     def __delitem__(self, key):
-        if isinstance(key, (int, np.integer)):
-            key = [key]
-        key = np.array(key).flatten()
-        new_length = len(self) - len(np.arange(len(self))[np.asarray(key)])
-        super(Atoms, self).__delitem__(key)
-        self.indices = np.delete(self.indices, key, axis=0)
-        del self._tag_list[key]
-        self._tag_list._length = new_length
-        deleted_species_indices = list()
-        retain_species_indices = list()
-        new_indices = self.indices.copy()
-        for i, el in enumerate(self.species):
-            if len(self.select_index(el)) == 0:
-                deleted_species_indices.append(i)
-                new_indices[new_indices >= i] += -1
-            else:
-                retain_species_indices.append(i)
-        new_species = np.array(self.species).copy()[retain_species_indices]
-        self.set_species(new_species)
-        self.indices = new_indices
+        super().__delitem__(np.array([key]).flatten())
+        unique_ind, new_ind = np.unique(self.indices, return_inverse=True)
+        self.set_array("indices", new_ind)
+        self.set_species(np.array(self.species)[unique_ind])
 
     def __eq__(self, other):
         return super(Atoms, self).__eq__(other) and np.array_equal(
             self.get_chemical_symbols(), other.get_chemical_symbols()
         )
 
     def __ne__(self, other):
         return not self == other
 
     def __getitem__(self, item):
         new_dict = dict()
         if isinstance(item, int):
-            for key, value in self._tag_list.items():
+            for key, value in self.arrays.items():
+                if key in ["positions", "numbers", "indices"]:
+                    continue
                 if item < len(value):
                     if value[item] is not None:
                         new_dict[key] = value[item]
             element = self.species[self.indices[item]]
             index = item
             position = self.positions[item]
             return Atom(
@@ -2145,39 +2110,36 @@
                 **new_dict,
             )
 
         new_array = super(Atoms, self).__getitem__(item)
         new_array.dimension = self.dimension
         if isinstance(item, tuple):
             item = list(item)
-        new_indices = self.indices[item].copy()
-        new_species_indices, new_proper_indices = np.unique(
-            new_indices, return_inverse=True
+        new_species_indices, new_indices = np.unique(
+            self.indices[item], return_inverse=True
         )
         new_species = [self.species[ind] for ind in new_species_indices]
         new_array.set_species(new_species)
-        new_array.indices = new_proper_indices
-        new_array._tag_list = self._tag_list[item]
-        # new_array._tag_list._length = self._tag_list._length
-        new_array._tag_list._length = len(new_array)
+        new_array.arrays["indices"] = new_indices
         if isinstance(new_array, Atom):
             natoms = len(self)
             if item < -natoms or item >= natoms:
                 raise IndexError("Index out of range.")
             new_array.index = item
         return new_array
 
     def __getattr__(self, item):
-        if item in self._tag_list.keys():
-            return self._tag_list._lists[item]
-        return object.__getattribute__(self, item)
+        try:
+            return self.arrays[item]
+        except KeyError:
+            return object.__getattribute__(self, item)
 
     def __dir__(self):
         new_dir = super().__dir__()
-        for key in self._tag_list.keys():
+        for key in self.arrays.keys():
             new_dir.append(key)
         return new_dir
 
     # def __len__(self):
     #     return len(self.indices)
 
     def __repr__(self):
@@ -2186,17 +2148,17 @@
         out_str = ""
         for el, pos in zip(self.get_chemical_symbols(), self.positions):
             out_str += el + ": " + str(pos) + "\n"
         if len(self.get_tags()) > 0:
             tags = self.get_tags()
             out_str += "tags: \n"  # + ", ".join(tags) + "\n"
             for tag in tags:
-                out_str += (
-                    "    " + str(tag) + ": " + self._tag_list[tag].__str__() + "\n"
-                )
+                if tag in ["positions", "numbers"]:
+                    continue
+                out_str += "    " + str(tag) + ": " + self.arrays[tag].__str__() + "\n"
         if self.cell is not None:
             out_str += "pbc: " + str(self.pbc) + "\n"
             out_str += "cell: \n"
             out_str += str(self.cell) + "\n"
         return out_str
 
     def __str__(self):
@@ -2306,75 +2268,24 @@
                     delete_indices = list()
                     new_indices = self.indices.copy()
                     for i, rep in enumerate(replace_list):
                         if i != ind and rep:
                             delete_indices.append(i)
                             # del new_species[i]
                             new_indices[new_indices >= i] -= 1
-                    self.indices = new_indices.copy()
+                    self.set_array("indices", new_indices.copy())
                     new_species = np.array(new_species)[
                         np.setdiff1d(np.arange(len(new_species)), delete_indices)
                     ].tolist()
                     self.set_species(new_species)
         else:
             raise NotImplementedError()
         # For ASE compatibility
         self.numbers = self.get_atomic_numbers()
 
-    def __imul__(self, vec):
-        if isinstance(vec, (int, np.integer)):
-            vec = [vec] * self.dimension
-        initial_length = len(self)
-        if not hasattr(vec, "__len__"):
-            raise ValueError(
-                "Box repetition must be an integer or a list/ndarray of integers and not",
-                type(vec),
-            )
-
-        if len(vec) != self.dimension:
-            raise AssertionError(
-                "Dimension of box repetition not consistent: ",
-                len(vec),
-                "!=",
-                self.dimension,
-            )
-
-        i_vec = np.array([vec[0], 1, 1])
-        if self.dimension > 1:
-            i_vec[1] = vec[1]
-        if self.dimension > 2:
-            i_vec[2] = vec[2]
-
-        if not self.dimension == 3:
-            raise NotImplementedError()
-        mx, my, mz = i_vec
-        # Our position repeat algorithm is faster than ASE (no nested loops)
-        nx_lst, ny_lst, nz_lst = np.arange(mx), np.arange(my), np.arange(mz)
-        positions = self.get_scaled_positions(wrap=False)
-        lat = np.array(np.meshgrid(nx_lst, ny_lst, nz_lst)).T.reshape(-1, 3)
-        lat_new = np.repeat(lat, len(positions), axis=0)
-        new_positions = np.tile(positions, (len(lat), 1)) + lat_new
-        new_positions /= np.array(i_vec)
-        self.set_cell((self.cell.T * np.array(vec)).T, scale_atoms=True)
-        # ASE compatibility
-        for name, a in self.arrays.items():
-            self.arrays[name] = np.tile(
-                a, (np.product(vec),) + (1,) * (len(a.shape) - 1)
-            )
-        self.arrays["positions"] = np.dot(new_positions, self.cell)
-        self.indices = np.tile(self.indices, len(lat))
-        self._tag_list._length = len(self)
-        scale = i_vec[0] * i_vec[1] * i_vec[2]
-        for tag in self._tag_list.keys():
-            self._tag_list[tag] *= scale
-        # Repeating ASE constraints
-        if self.constraints is not None:
-            self.constraints = [c.repeat(vec, initial_length) for c in self.constraints]
-        return self
-
     @staticmethod
     def convert_formula(elements):
         """
         Convert a given chemical formula into a list of elements
 
         Args:
             elements (str): A string of the required chamical formula (eg. H2O)
@@ -2409,15 +2320,15 @@
                     for el in el_fac[1:]:
                         el_list.append(el)
                     num_list = ""
 
         return el_list
 
     def get_constraint(self):
-        if "selective_dynamics" in self._tag_list._lists.keys():
+        if "selective_dynamics" in self.arrays.keys():
             from ase.constraints import FixAtoms
 
             return FixAtoms(
                 indices=[
                     atom_ind
                     for atom_ind in range(len(self))
                     if not any(self.selective_dynamics[atom_ind])
@@ -2429,15 +2340,15 @@
     def set_constraint(self, constraint=None):
         super(Atoms, self).set_constraint(constraint)
         if constraint is not None:
             if constraint.todict()["name"] != "FixAtoms":
                 raise ValueError(
                     "Only FixAtoms is supported as ASE compatible constraint."
                 )
-            if "selective_dynamics" not in self._tag_list._lists.keys():
+            if "selective_dynamics" not in self.arrays.keys():
                 self.add_tag(selective_dynamics=None)
             for atom_ind in range(len(self)):
                 if atom_ind in constraint.index:
                     self.selective_dynamics[atom_ind] = [False, False, False]
                 else:
                     self.selective_dynamics[atom_ind] = [True, True, True]
 
@@ -2504,17 +2415,17 @@
     def get_initial_magnetic_moments(self):
         """
         Get array of initial magnetic moments.
 
         Returns:
             numpy.array()
         """
-        if "spin" in self._tag_list._lists.keys():
-            return np.asarray(self.spin.list())
-        else:
+        try:
+            return self.arrays["spin"]
+        except KeyError:
             spin_lst = [
                 element.tags["spin"] if "spin" in element.tags.keys() else None
                 for element in self.get_chemical_elements()
             ]
             if any(spin_lst):
                 if (
                     (
@@ -2625,18 +2536,16 @@
                         )
                     )
                 magmoms = [magmoms[c] for c in self.get_chemical_symbols()]
             elif not isinstance(magmoms, (np.ndarray, Sequence)):
                 magmoms = len(self) * [magmoms]
             if len(magmoms) != len(self):
                 raise ValueError("magmoms can be collinear or non-collinear.")
-            if "spin" not in self._tag_list._lists.keys():
-                self.add_tag(spin=None)
-            for ind, spin in enumerate(magmoms):
-                self.spin[ind] = spin  # For self._tag_list.spin
+            self.set_array("spin", None)
+            self.set_array("spin", np.array(magmoms))
         self.spins = magmoms  # For self.array['initial_magmoms']
 
     def rotate(
         self, a=0.0, v=None, center=(0, 0, 0), rotate_cell=False, index_list=None
     ):
         """
         Rotate atoms based on a vector and an angle, or two vectors. This function is completely adopted from ASE code
@@ -3206,21 +3115,21 @@
             cell=cell,
             magmoms=spins,
         )
     if hasattr(ase_obj, "constraints") and len(ase_obj.constraints) != 0:
         for constraint in ase_obj.constraints:
             constraint_dict = constraint.todict()
             if constraint_dict["name"] == "FixAtoms":
-                if "selective_dynamics" not in pyiron_atoms._tag_list.keys():
+                if "selective_dynamics" not in pyiron_atoms.arrays.keys():
                     pyiron_atoms.add_tag(selective_dynamics=[True, True, True])
                 pyiron_atoms.selective_dynamics[
                     constraint_dict["kwargs"]["indices"]
                 ] = [False, False, False]
             elif constraint_dict["name"] == "FixScaled":
-                if "selective_dynamics" not in pyiron_atoms._tag_list.keys():
+                if "selective_dynamics" not in pyiron_atoms.arrays.keys():
                     pyiron_atoms.add_tag(selective_dynamics=[True, True, True])
                 pyiron_atoms.selective_dynamics[
                     constraint_dict["kwargs"]["a"]
                 ] = constraint_dict["kwargs"]["mask"]
             else:
                 warnings.warn("Unsupported ASE constraint: " + constraint_dict["name"])
     return pyiron_atoms
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/aimsgb.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/ase.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/ase.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/atomsk.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/atomsk.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/compound.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/compound.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/materialsproject.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factories/materialsproject.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factory.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/has_structure.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/has_structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/neighbors.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/periodic_table.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/periodic_table.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/phonopy.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyironase.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/pyironase.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyscal.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/pyscal.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/structurestorage.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/structure/structurestorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,17 +208,15 @@
                                         string
             **kwargs: additional arrays to store for structure
         """
 
         if structure.has("initial_magmoms"):
             arrays["spins"] = structure.spins
         if "selective_dynamics" in structure.get_tags():
-            arrays["selective_dynamics"] = getattr(
-                structure, "selective_dynamics"
-            ).list()
+            arrays["selective_dynamics"] = structure.selective_dynamics
 
         self.add_chunk(
             len(structure),
             identifier=identifier,
             symbols=np.array(structure.symbols),
             positions=structure.positions,
             cell=[structure.cell.array],
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/generic.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/atomistics/volumetric/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/job.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/calphy/job.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/bader.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/bader.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/generic.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_parallel.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/convergence_encut_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_serial.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/convergence_encut_serial.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/murnaghan_dft.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/master/murnaghan_dft.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/bandstructure.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/dos.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/dos.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/electronic.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/dft/waves/electronic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/gpaw.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/gpaw/gpaw.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/pyiron_ase.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/gpaw/pyiron_ase.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                 atoms = Atoms(
                     symbols=np.array([el_lst[el] for el in indices]),
                     positions=positions,
                     cell=self.output.cells[frame],
                     pbc=self.structure.pbc,
                 )
                 # Update indicies to match the indicies in the cache.
-                atoms.indices = indices
+                atoms.set_array("indices", indices)
                 return atoms
             else:
                 return None
         else:
             if (
                 self.get("output/generic/cells") is not None
                 and len(self.get("output/generic/cells")) != 0
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/activation_relaxation_technique.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/activation_relaxation_technique.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/quasi_newton.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/quasi_newton.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/scipy_minimizer.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/scipy_minimizer.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/sxextoptint.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/interactive/sxextoptint.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import warnings
 from pyiron_base import state, GenericParameters, Executable, deprecate
 from pyiron_atomistics.atomistics.job.interactivewrapper import (
     InteractiveWrapper,
     ReferenceJobOutput,
 )
 from pyiron_atomistics.atomistics.job.interactive import InteractiveInterface
-from pyiron_atomistics.sphinx.base import InputWriter
+from pyiron_atomistics.sphinx.base import get_structure_group
 
 __author__ = "Jan Janssen, Osamu Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -42,15 +42,14 @@
         ionic_energy=None,
         ionic_forces=None,
         ionic_energy_tolerance=1.0e-3,
         ionic_force_tolerance=1.0e-2,
         max_step_length=1.0e-1,
         soft_mode_damping=1,
         executable=None,
-        ssa=False,
     ):
         if ionic_forces is not None:
             ionic_force_tolerance = ionic_forces
         if ionic_energy is not None:
             ionic_energy_tolerance = ionic_energy
         super().__init__()
 
@@ -72,57 +71,43 @@
             executable=executable,
             maxDist=maxDist,
             ionic_steps=ionic_steps,
             ionic_energy_tolerance=ionic_energy_tolerance,
             ionic_force_tolerance=ionic_force_tolerance,
             max_step_length=max_step_length,
             soft_mode_damping=soft_mode_damping,
-            selective_dynamics="selective_dynamics" in structure._tag_list.keys(),
-            ssa=ssa,
+            selective_dynamics="selective_dynamics" in structure.arrays.keys(),
         )
         self._cell = structure.cell
-        if ssa:
-            self._elements = structure.get_parent_symbols()
-        else:
-            magmom = structure.get_initial_magnetic_moments()
-            magmom[magmom != None] = np.round(magmom[magmom != None], decimals=1)
-            magmom = np.char.mod("%s", magmom)
-            self._elements = np.char.add(structure.get_parent_symbols(), magmom)
-            self._elements = np.char.replace(self._elements, "-", "m")
-            self._elements = np.char.replace(self._elements, ".", "p")
+        magmom = structure.get_initial_magnetic_moments()
+        magmom[magmom != None] = np.round(magmom[magmom != None], decimals=1)
+        magmom = np.char.mod("%s", magmom)
+        self._elements = np.char.add(structure.get_parent_symbols(), magmom)
+        self._elements = np.char.replace(self._elements, "-", "m")
+        self._elements = np.char.replace(self._elements, ".", "p")
         self._positions = structure.positions
         self._converged = False
 
     def _start_process(
         self,
         structure,
         executable,
         maxDist=5,
         ionic_steps=1000,
         ionic_energy_tolerance=1.0e-3,
         ionic_force_tolerance=1.0e-2,
         max_step_length=1.0e-1,
         soft_mode_damping=1,
         selective_dynamics=False,
-        ssa=False,
     ):
         if selective_dynamics:
-            input_writer_obj = InputWriter()
-            input_writer_obj.structure = structure
-            if ssa:
-                input_writer_obj.structure.set_initial_magnetic_moments(
-                    len(structure) * [None]
-                )
-            input_writer_obj.write_structure(
-                file_name="structure.sx",
-                cwd=self.working_directory,
-                structure_str=None,
-                symmetry_enabled=True,
-                keep_angstrom=True,
-            )
+            structure_to_write = structure.copy()
+            file_name = posixpath.join(self.working_directory, "input.sx")
+            with open(file_name, "w") as f:
+                f.write(get_structure_group(structure, keep_angstrom=True).to_sphinx())
         self._write_input(
             working_directory=self.working_directory,
             maxDist=maxDist,
             ionic_steps=ionic_steps,
             ionic_energy_tolerance=ionic_energy_tolerance,
             ionic_force_tolerance=ionic_force_tolerance,
             max_step_length=max_step_length,
@@ -328,15 +313,14 @@
             maxDist=int(self.input["maxDist"]),
             ionic_steps=int(self.input["ionic_steps"]),
             ionic_energy_tolerance=float(self.input["ionic_energy_tolerance"]),
             ionic_force_tolerance=float(self.input["ionic_force_tolerance"]),
             max_step_length=float(self.input["max_step_length"]),
             soft_mode_damping=float(self.input["soft_mode_damping"]),
             executable=self.executable.executable_path,
-            ssa=self.input["ssa"],
         )
         self.status.running = True
         self._logger.info("job status: %s", self.status)
         new_positions = self.ref_job.structure.positions
         self.ref_job_initialize()
         while (
             self._interactive_number_of_steps < self.input["ionic_steps"]
@@ -404,15 +388,14 @@
         """
         file_content = (
             "ionic_steps = 1000 // maximum number of ionic steps\n"
             "ionic_energy_tolerance = 1.0e-3\n"
             "ionic_force_tolerance = 1.0e-2\n"
             "maxDist = 5 // maximum possible distance for considering neighbors\n"
             "max_step_length = 1.0e-1 // maximum displacement at each step\n"
-            "ssa = False // ignore different magnetic moment values when internal symmetries are considered\n"
             "soft_mode_damping = 1.0 // Tikhonov damper\n"
         )
         self.load_string(file_content)
 
 
 class SxExtOptOutput(ReferenceJobOutput):
     def __init__(self, job):
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/base.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -969,18 +969,16 @@
         ):
             raise ValueError(
                 "The selected potentials do not support the given combination of elements."
             )
         return lmp_structure
 
     def _set_selective_dynamics(self):
-        if "selective_dynamics" in self.structure._tag_list.keys():
-            if self.structure.selective_dynamics._default is None:
-                self.structure.selective_dynamics._default = [True, True, True]
-            sel_dyn = np.logical_not(self.structure.selective_dynamics.list())
+        if "selective_dynamics" in self.structure.arrays.keys():
+            sel_dyn = np.logical_not(self.structure.selective_dynamics)
             # Enter loop only if constraints present
             if len(np.argwhere(np.any(sel_dyn, axis=1)).flatten()) != 0:
                 all_indices = np.arange(len(self.structure), dtype=int)
                 constraint_xyz = np.argwhere(np.all(sel_dyn, axis=1)).flatten()
                 not_constrained_xyz = np.setdiff1d(all_indices, constraint_xyz)
                 # LAMMPS starts counting from 1
                 constraint_xyz += 1
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/control.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -760,21 +760,30 @@
                 key = key.replace("**", "^")
             self._measure_mean_value(name, key, every, atom)
         else:
             raise NotImplementedError(key + " is not implemented")
 
     def energy_pot_per_atom(self):
         """
-        Enable the output of atomic energies.  This will add an additional key 'energy_pot_per_atom' to the HDF output.
+        Enable the output of per atom potential energies.  This will add an additional key 'energy_pot_per_atom' to the HDF output.
         """
         if self["compute___energy_pot_per_atom"] is None:
             self["compute___energy_pot_per_atom"] = "all pe/atom"
             self["dump___1"] += " c_energy_pot_per_atom"
             self["dump_modify___1"] = self["dump_modify___1"][:-1] + ' %20.15g"'
 
+    def energy_kin_per_atom(self):
+        """
+        Enable the output of per atom kinetic energies.  This will add an additional key 'energy_kin_per_atom' to the HDF output.
+        """
+        if self["compute___energy_kin_per_atom"] is None:
+            self["compute___energy_kin_per_atom"] = "all ke/atom"
+            self["dump___1"] += " c_energy_kin_per_atom"
+            self["dump_modify___1"] = self["dump_modify___1"][:-1] + ' %20.15g"'
+
     def _set_group_by_id(self, group_name, ids):
         if len(ids) < 1:
             raise ValueError(
                 "Group ids must have at least length one, but got {}".format(ids)
             )
         if np.any(
             [
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/interactive.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/lammps.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/output.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/output.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/potential.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/structure.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/units.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/lammps/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 _conversion_dict["volume"] = ["volume", "volumes"]
 _conversion_dict["pressure"] = ["pressure", "pressures", "mean_pressures"]
 _conversion_dict["time"] = ["time"]
 _conversion_dict["energy"] = [
     "energy_tot",
     "energy_pot",
     "energy_pot_per_atom",
+    "energy_kin_per_atom",
     "mean_energy_pot",
 ]
 _conversion_dict["temperature"] = ["temperature", "temperatures"]
 _conversion_dict["velocity"] = ["velocity", "velocities", "mean_velocities"]
 _conversion_dict["mass"] = ["mass"]
 _conversion_dict["charge"] = ["charges", "charge"]
 _conversion_dict["force"] = ["forces", "force", "mean_forces"]
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/project.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,17 @@
         """
         job = self.inspect(job_specifier)
         snapshot = Atoms().from_hdf(job["input"], "structure")
         if "output" in job.project_hdf5.list_groups() and iteration_step != 0:
             snapshot.cell = job.get("output/generic/cells")[iteration_step]
             snapshot.positions = job.get("output/generic/positions")[iteration_step]
             if "indices" in job.get("output/generic").list_nodes():
-                snapshot.indices = job.get("output/generic/indices")[iteration_step]
+                snapshot.set_array(
+                    "indices", job.get("output/generic/indices")[iteration_step]
+                )
             if (
                 "dft" in job["output/generic"].list_groups()
                 and "atom_spins" in job["output/generic/dft"].list_nodes()
             ):
                 snapshot.set_initial_magnetic_moments(
                     job.get("output/generic/dft/atom_spins")[iteration_step]
                 )
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/base.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,17 @@
         return self._generic_input["fix_spin_constraint"]
 
     @fix_spin_constraint.setter
     def fix_spin_constraint(self, boolean):
         if not isinstance(boolean, bool):
             raise ValueError("fix_spin_constraint has to be a boolean")
         self._generic_input["fix_spin_constraint"] = boolean
-        self.structure.add_tag(spin_constraint=boolean)
+        self.structure.set_array(
+            "spin_constraint", np.array(len(self.structure) * [boolean])
+        )
 
     @plane_wave_cutoff.setter
     def plane_wave_cutoff(self, val):
         """
         Function to setup the energy cut-off for the SPHInX job in eV.
 
         Args:
@@ -330,60 +332,19 @@
     def get_structure_group(self, keep_angstrom=False):
         """
         create a SPHInX Group object based on self.structure
 
         Args:
             keep_angstrom (bool): Store distances in Angstroms or Bohr
         """
-        if keep_angstrom:
-            structure_group = Group({"cell": np.array(self.structure.cell)})
-        else:
-            structure_group = Group(
-                {
-                    "cell": np.array(self.structure.cell * 1 / BOHR_TO_ANGSTROM),
-                }
-            )
-        if "selective_dynamics" in self.structure._tag_list.keys():
-            selective_dynamics_list = self.structure.selective_dynamics.list()
-        else:
-            selective_dynamics_list = [3 * [False]] * len(self.structure.positions)
-        species = structure_group.create_group("species")
-        for elm_species in self.structure.get_species_objects():
-            if elm_species.Parent:
-                element = elm_species.Parent
-            else:
-                element = elm_species.Abbreviation
-            species.append(Group({"element": '"' + str(element) + '"'}))
-            elm_list = np.array(
-                self.structure.get_chemical_symbols() == elm_species.Abbreviation
-            )
-            atom_group = species[-1].create_group("atom")
-            for elm_pos, elm_magmon, selective in zip(
-                self.structure.positions[elm_list],
-                np.array(self.structure.get_initial_magnetic_moments())[elm_list],
-                np.array(selective_dynamics_list)[elm_list],
-            ):
-                atom_group.append(Group())
-                if self._spin_enabled:
-                    atom_group[-1]["label"] = '"spin_' + str(elm_magmon) + '"'
-                if keep_angstrom:
-                    atom_group[-1]["coords"] = np.array(elm_pos)
-                else:
-                    atom_group[-1]["coords"] = np.array(elm_pos * 1 / BOHR_TO_ANGSTROM)
-                if all(selective):
-                    atom_group[-1]["movable"] = True
-                elif any(selective):
-                    for ss, xx in zip(selective, ["X", "Y", "Z"]):
-                        if ss:
-                            atom_group[-1]["movable" + xx] = True
-        if not self.fix_symmetry:
-            structure_group.symmetry = Group(
-                {"operator": {"S": "[[1,0,0],[0,1,0],[0,0,1]]"}}
-            )
-        return structure_group
+        return get_structure_group(
+            structure=self.structure,
+            use_symmetry=self.fix_symmetry,
+            keep_angstrom=keep_angstrom,
+        )
 
     def load_default_input(self):
         """
         Set defaults for generic parameters and create SPHInX input groups.
         """
 
         sph = self.input.create_group("sphinx")
@@ -1851,14 +1812,74 @@
                 print(addon + " output:\n\n")
             print(out.stdout)
             if out.returncode != 0:
                 print(out.stderr)
         return out if debug else None
 
 
+def get_structure_group(structure, use_symmetry=True, keep_angstrom=False):
+    """
+    create a SPHInX Group object based on structure
+
+    Args:
+        structure (pyiron_atomistics.atomistics.structure.atoms) structure
+        use_symmetry (bool): Whether or not consider internal symmetry
+        keep_angstrom (bool): Store distances in Angstroms or Bohr
+
+    Returns:
+        (Group): structure group
+    """
+    if keep_angstrom:
+        structure_group = Group({"cell": np.array(structure.cell)})
+    else:
+        structure_group = Group(
+            {
+                "cell": np.array(structure.cell * 1 / BOHR_TO_ANGSTROM),
+            }
+        )
+    if "selective_dynamics" in structure.arrays:
+        selective_dynamics_list = list(structure.selective_dynamics)
+    else:
+        selective_dynamics_list = [3 * [False]] * len(structure.positions)
+    species = structure_group.create_group("species")
+    for elm_species in structure.get_species_objects():
+        if elm_species.Parent:
+            element = elm_species.Parent
+        else:
+            element = elm_species.Abbreviation
+        species.append(Group({"element": '"' + str(element) + '"'}))
+        elm_list = np.array(
+            structure.get_chemical_symbols() == elm_species.Abbreviation
+        )
+        atom_group = species[-1].create_group("atom")
+        for elm_pos, elm_magmon, selective in zip(
+            structure.positions[elm_list],
+            np.array(structure.get_initial_magnetic_moments())[elm_list],
+            np.array(selective_dynamics_list)[elm_list],
+        ):
+            atom_group.append(Group())
+            if structure.has("initial_magmoms"):
+                atom_group[-1]["label"] = '"spin_' + str(elm_magmon) + '"'
+            if keep_angstrom:
+                atom_group[-1]["coords"] = np.array(elm_pos)
+            else:
+                atom_group[-1]["coords"] = np.array(elm_pos * 1 / BOHR_TO_ANGSTROM)
+            if all(selective):
+                atom_group[-1]["movable"] = True
+            elif any(selective):
+                for ss, xx in zip(selective, ["X", "Y", "Z"]):
+                    if ss:
+                        atom_group[-1]["movable" + xx] = True
+    if not use_symmetry:
+        structure_group.symmetry = Group(
+            {"operator": {"S": "[[1,0,0],[0,1,0],[0,0,1]]"}}
+        )
+    return structure_group
+
+
 class InputWriter(object):
     """
     The SPHInX Input writer is called to write the
     SPHInX specific input files.
     """
 
     def __init__(self):
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/interactive.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/potential.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/sphinx.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/structure.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/util.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/util.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/volumetric_data.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/sphinx/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/datamining.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/table/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/funct.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/table/funct.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/executable.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/testing/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/randomatomistic.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/testing/randomatomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/hessian.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/hessian.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/interfacemethod.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/interfacemethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     Args:
         basis (pyiron_atomistics.structure.atoms.Atoms): Atomistic structure object
 
     Returns:
         Atoms: Atomistic structure object with selective dynamics set to True
     """
-    if "selective_dynamics" in basis._tag_list.keys():
+    if "selective_dynamics" in basis.arrays.keys():
         for ind in range(len(basis)):
             basis.selective_dynamics[ind] = [True, True, True]
     return basis
 
 
 def set_server(job, project_parameter):
     """
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/sxphonons.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/thermodynamics/sxphonons.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/toolkit.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/base.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
                 raise IOError("Unable to read output structure")
         return input_structure
 
     def write_magmoms(self):
         """
         Write the magnetic moments in INCAR from that assigned to the species
         """
-        if any(self.structure.get_initial_magnetic_moments().flatten()):
+        if self.structure.has("initial_magmoms"):
             if "ISPIN" not in self.input.incar._dataset["Parameter"]:
                 self.input.incar["ISPIN"] = 2
             if self.input.incar["ISPIN"] != 1:
                 final_cmd = "   ".join(
                     [
                         " ".join([str(spinmom) for spinmom in spin])
                         if isinstance(spin, (list, np.ndarray))
@@ -1794,15 +1794,15 @@
             )
 
         self.input.incar["LAMBDA"] = lamb
         self.set_rwigs(rwigs_dict)
 
     def validate_ready_to_run(self):
         super(VaspBase, self).validate_ready_to_run()
-        if "spin_constraint" in self.structure._tag_list.keys():
+        if "spin_constraint" in self.structure.arrays.keys():
             raise NotImplementedError(
                 "The spin_constraint tag is not supported by VASP."
             )
 
     def list_potentials(self):
         """
         Lists all the possible POTCAR files for the elements in the structure depending on the XC functional
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/interactive.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 
     def _run_if_new(self, debug=False):
         if (
             self.server.run_mode.interactive
             or self.server.run_mode.interactive_non_modal
         ):
             self.interactive_prepare()
-        return super(VaspInteractive, self)._run_if_new(debug=debug)
+        super(VaspInteractive, self)._run_if_new(debug=debug)
 
     def interactive_prepare(self):
         """
         Modifies/adds tags in the INCAR file that make it possible to run VASP interactively
         """
         self._check_incar_parameter(parameter="INTERACTIVE", value=True)
         self._check_incar_parameter(parameter="IBRION", value=-1)
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/metadyn.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/metadyn.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/oszicar.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/oszicar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/outcar.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/outcar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/potential.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/procar.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/procar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/report.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/report.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/structure.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasp.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasprun.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vaspsol.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/vaspsol.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/volumetric_data.py` & `pyiron-atomistics-0.3.1/pyiron_atomistics/vasp/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/PKG-INFO` & `pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-atomistics
-Version: 0.3.0.dev0
+Version: 0.3.1
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/SOURCES.txt` & `pyiron-atomistics-0.3.1/pyiron_atomistics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 pyiron_atomistics/atomistics/structure/factory.py
 pyiron_atomistics/atomistics/structure/has_structure.py
 pyiron_atomistics/atomistics/structure/neighbors.py
 pyiron_atomistics/atomistics/structure/periodic_table.py
 pyiron_atomistics/atomistics/structure/phonopy.py
 pyiron_atomistics/atomistics/structure/pyironase.py
 pyiron_atomistics/atomistics/structure/pyscal.py
-pyiron_atomistics/atomistics/structure/sparse_list.py
 pyiron_atomistics/atomistics/structure/structurestorage.py
 pyiron_atomistics/atomistics/structure/factories/__init__.py
 pyiron_atomistics/atomistics/structure/factories/aimsgb.py
 pyiron_atomistics/atomistics/structure/factories/ase.py
 pyiron_atomistics/atomistics/structure/factories/atomsk.py
 pyiron_atomistics/atomistics/structure/factories/compound.py
 pyiron_atomistics/atomistics/structure/factories/materialsproject.py
```

### Comparing `pyiron-atomistics-0.3.0.dev0/setup.py` & `pyiron-atomistics-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,22 @@
         "*test_integration*", 
         "*.github*"
     ]),
     install_requires=[
         'ase>=3.22.1',
         'defusedxml>=0.7.1',
         'h5py>=3.9.0',
-        'matplotlib>=3.7.1',
+        'matplotlib>=3.7.2',
         'mendeleev>=0.14.0',
         'mp-api>=0.33.3',
         'numpy>=1.24.3',
         'pandas>=2.0.3',
         'phonopy>=2.20.0',
         'pint>=0.22',
-        'pyiron_base>=0.6.1',
+        'pyiron_base>=0.6.3',
         'pymatgen>=2023.6.28',
         'scipy>=1.11.1',
         'seekpath>=2.1.0',
         'scikit-learn>=1.3.0',
         'spglib>=2.0.2',
         'structuretoolkit>=0.0.5'
     ],
```

### Comparing `pyiron-atomistics-0.3.0.dev0/tests/test_project.py` & `pyiron-atomistics-0.3.1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/tests/test_toolkit.py` & `pyiron-atomistics-0.3.1/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0.dev0/versioneer.py` & `pyiron-atomistics-0.3.1/versioneer.py`

 * *Files identical despite different names*

