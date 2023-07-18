# Comparing `tmp/solvis-0.8.0.tar.gz` & `tmp/solvis-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvis-0.8.0.tar", max compression
+gzip compressed data, was "solvis-0.8.1.tar", max compression
```

## Comparing `solvis-0.8.0.tar` & `solvis-0.8.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    34523 2023-07-17 22:16:26.018770 solvis-0.8.0/LICENSE
--rw-r--r--   0        0        0     2733 2023-07-17 22:16:26.018770 solvis-0.8.0/README.md
--rw-r--r--   0        0        0     2593 2023-07-17 22:16:26.022770 solvis-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      259 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/__init__.py
--rw-r--r--   0        0        0      369 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/config.py
--rw-r--r--   0        0        0     8314 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/geometry.py
--rw-r--r--   0        0        0     2512 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/get_secret.py
--rw-r--r--   0        0        0      155 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/__init__.py
--rw-r--r--   0        0        0     4119 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/composite_solution.py
--rw-r--r--   0        0        0     7983 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/fault_system_solution.py
--rw-r--r--   0        0        0     4750 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/fault_system_solution_file.py
--rw-r--r--   0        0        0     2576 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/inversion_solution.py
--rw-r--r--   0        0        0     8911 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/inversion_solution_file.py
--rw-r--r--   0        0        0     5859 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/inversion_solution_operations.py
--rw-r--r--   0        0        0     3053 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/solution_surfaces_builder.py
--rw-r--r--   0        0        0     3005 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/typing.py
--rw-r--r--   0        0        0     2106 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/solvis.py
--rw-r--r--   0        0        0        0 2023-07-17 22:16:26.022770 solvis-0.8.0/test/__init__.py
--rw-r--r--   0        0        0     6174 2023-07-17 22:16:26.022770 solvis-0.8.0/test/conftest.py
--rw-r--r--   0        0        0  1390671 2023-07-17 22:16:26.026770 solvis-0.8.0/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip
--rw-r--r--   0        0        0   306556 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/CrustalSmallSolution_compat.zip
--rw-r--r--   0        0        0   306556 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/CrustalSmallSolution_non_compat.zip
--rw-r--r--   0        0        0   329085 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/HikurangiSmallSolution_compat.zip
--rw-r--r--   0        0        0   329085 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/HikurangiSmallSolution_non_compat.zip
--rw-r--r--   0        0        0      791 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/MiniInversionSolution/README
--rw-r--r--   0        0        0      470 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/MiniInversionSolution/modules.json
--rw-r--r--   0        0        0    21893 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv
--rw-r--r--   0        0        0  1678031 2023-07-17 22:16:26.034770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson
--rw-r--r--   0        0        0   425032 2023-07-17 22:16:26.038770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv
--rw-r--r--   0        0        0   654267 2023-07-17 22:16:26.042770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv
--rw-r--r--   0        0        0  2486065 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson
--rw-r--r--   0        0        0   156269 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/indices.csv
--rw-r--r--   0        0        0       36 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/info.txt
--rw-r--r--   0        0        0    15992 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json
--rw-r--r--   0        0        0     2495 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json
--rw-r--r--   0        0        0    22534 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv
--rw-r--r--   0        0        0     2385 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/modules.json
--rw-r--r--   0        0        0   485782 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/plausibility.json
--rw-r--r--   0        0        0    77673 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/properties.csv
--rw-r--r--   0        0        0    26727 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json
--rw-r--r--   0        0        0    52224 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv
--rw-r--r--   0        0        0  2688710 2023-07-17 22:16:26.062770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson
--rw-r--r--   0        0        0    36289 2023-07-17 22:16:26.062770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv
--rw-r--r--   0        0        0  1055188 2023-07-17 22:16:26.066770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv
--rw-r--r--   0        0        0  1028684 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv
--rw-r--r--   0        0        0      173 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/build_info.json
--rw-r--r--   0        0        0      670 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/modules.json
--rw-r--r--   0        0        0     7958 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/rates.csv
--rw-r--r--   0        0        0  1055188 2023-07-17 22:16:26.078770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv
--rw-r--r--   0        0        0   450515 2023-07-17 22:16:26.078770 solvis-0.8.0/test/fixtures/ModularAlpineVernonInversionSolution.zip
--rw-r--r--   0        0        0   842948 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip
--rw-r--r--   0        0        0   214824 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/PuysegurSmallSolution_compat.zip
--rw-r--r--   0        0        0   214824 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/PuysegurSmallSolution_non_compat.zip
--rw-r--r--   0        0        0   466256 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/hik_fault_sections.geojson
--rw-r--r--   0        0        0   241379 2023-07-17 22:16:26.086770 solvis-0.8.0/test/fixtures/puy_fault_sections.geojson
--rw-r--r--   0        0        0     1540 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_circle_polygon.py
--rw-r--r--   0        0        0     3359 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry.py
--rw-r--r--   0        0        0    11190 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_dip.py
--rw-r--r--   0        0        0     8559 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_distance.py
--rw-r--r--   0        0        0     2827 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_performance.py
--rw-r--r--   0        0        0     4444 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_subduction.py
--rw-r--r--   0        0        0     6809 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_composite_solution.py
--rw-r--r--   0        0        0     4432 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_dataframe_serialisation.py
--rw-r--r--   0        0        0    10643 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_fault_system_solution.py
--rw-r--r--   0        0        0     4314 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_inversion_solution.py
--rw-r--r--   0        0        0     5201 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_new_inversion_solution.py
--rw-r--r--   0        0        0     1905 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_solution_surfaces_builder.py
--rw-r--r--   0        0        0     1206 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_solvis.py
--rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 solvis-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-18 00:00:42.922290 solvis-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2733 2023-07-18 00:00:42.922290 solvis-0.8.1/README.md
+-rw-r--r--   0        0        0     2593 2023-07-18 00:00:42.922290 solvis-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/__init__.py
+-rw-r--r--   0        0        0      369 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/config.py
+-rw-r--r--   0        0        0     8314 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/geometry.py
+-rw-r--r--   0        0        0     2512 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/get_secret.py
+-rw-r--r--   0        0        0      155 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/__init__.py
+-rw-r--r--   0        0        0     4119 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/composite_solution.py
+-rw-r--r--   0        0        0     7983 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/fault_system_solution.py
+-rw-r--r--   0        0        0     4750 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/fault_system_solution_file.py
+-rw-r--r--   0        0        0     2576 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/inversion_solution.py
+-rw-r--r--   0        0        0     8911 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/inversion_solution_file.py
+-rw-r--r--   0        0        0     5859 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/inversion_solution_operations.py
+-rw-r--r--   0        0        0     3053 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/solution_surfaces_builder.py
+-rw-r--r--   0        0        0     3005 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/inversion_solution/typing.py
+-rw-r--r--   0        0        0     2106 2023-07-18 00:00:42.926290 solvis-0.8.1/solvis/solvis.py
+-rw-r--r--   0        0        0        0 2023-07-18 00:00:42.926290 solvis-0.8.1/test/__init__.py
+-rw-r--r--   0        0        0     6174 2023-07-18 00:00:42.926290 solvis-0.8.1/test/conftest.py
+-rw-r--r--   0        0        0  1390671 2023-07-18 00:00:42.930290 solvis-0.8.1/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip
+-rw-r--r--   0        0        0   306556 2023-07-18 00:00:42.930290 solvis-0.8.1/test/fixtures/CrustalSmallSolution_compat.zip
+-rw-r--r--   0        0        0   306556 2023-07-18 00:00:42.934290 solvis-0.8.1/test/fixtures/CrustalSmallSolution_non_compat.zip
+-rw-r--r--   0        0        0   329085 2023-07-18 00:00:42.934290 solvis-0.8.1/test/fixtures/HikurangiSmallSolution_compat.zip
+-rw-r--r--   0        0        0   329085 2023-07-18 00:00:42.934290 solvis-0.8.1/test/fixtures/HikurangiSmallSolution_non_compat.zip
+-rw-r--r--   0        0        0      791 2023-07-18 00:00:42.934290 solvis-0.8.1/test/fixtures/MiniInversionSolution/README
+-rw-r--r--   0        0        0      470 2023-07-18 00:00:42.934290 solvis-0.8.1/test/fixtures/MiniInversionSolution/modules.json
+-rw-r--r--   0        0        0    21893 2023-07-18 00:00:42.934290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv
+-rw-r--r--   0        0        0  1678031 2023-07-18 00:00:42.938290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson
+-rw-r--r--   0        0        0   425032 2023-07-18 00:00:42.942290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv
+-rw-r--r--   0        0        0   654267 2023-07-18 00:00:42.946290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv
+-rw-r--r--   0        0        0  2486065 2023-07-18 00:00:42.954290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson
+-rw-r--r--   0        0        0   156269 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/indices.csv
+-rw-r--r--   0        0        0       36 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/info.txt
+-rw-r--r--   0        0        0    15992 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json
+-rw-r--r--   0        0        0     2495 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json
+-rw-r--r--   0        0        0    22534 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv
+-rw-r--r--   0        0        0     2385 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/modules.json
+-rw-r--r--   0        0        0   485782 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/plausibility.json
+-rw-r--r--   0        0        0    77673 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/properties.csv
+-rw-r--r--   0        0        0    26727 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json
+-rw-r--r--   0        0        0    52224 2023-07-18 00:00:42.958290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv
+-rw-r--r--   0        0        0  2688710 2023-07-18 00:00:42.970290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson
+-rw-r--r--   0        0        0    36289 2023-07-18 00:00:42.970290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv
+-rw-r--r--   0        0        0  1055188 2023-07-18 00:00:42.974290 solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv
+-rw-r--r--   0        0        0  1028684 2023-07-18 00:00:42.978290 solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv
+-rw-r--r--   0        0        0      173 2023-07-18 00:00:42.978290 solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/build_info.json
+-rw-r--r--   0        0        0      670 2023-07-18 00:00:42.978290 solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/modules.json
+-rw-r--r--   0        0        0     7958 2023-07-18 00:00:42.978290 solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/rates.csv
+-rw-r--r--   0        0        0  1055188 2023-07-18 00:00:42.986290 solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv
+-rw-r--r--   0        0        0   450515 2023-07-18 00:00:42.986290 solvis-0.8.1/test/fixtures/ModularAlpineVernonInversionSolution.zip
+-rw-r--r--   0        0        0   842948 2023-07-18 00:00:42.990290 solvis-0.8.1/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip
+-rw-r--r--   0        0        0   214824 2023-07-18 00:00:42.990290 solvis-0.8.1/test/fixtures/PuysegurSmallSolution_compat.zip
+-rw-r--r--   0        0        0   214824 2023-07-18 00:00:42.990290 solvis-0.8.1/test/fixtures/PuysegurSmallSolution_non_compat.zip
+-rw-r--r--   0        0        0   466256 2023-07-18 00:00:42.990290 solvis-0.8.1/test/fixtures/hik_fault_sections.geojson
+-rw-r--r--   0        0        0   241379 2023-07-18 00:00:42.994290 solvis-0.8.1/test/fixtures/puy_fault_sections.geojson
+-rw-r--r--   0        0        0     1540 2023-07-18 00:00:42.994290 solvis-0.8.1/test/geometry/test_circle_polygon.py
+-rw-r--r--   0        0        0     3359 2023-07-18 00:00:42.994290 solvis-0.8.1/test/geometry/test_geometry.py
+-rw-r--r--   0        0        0    11190 2023-07-18 00:00:42.994290 solvis-0.8.1/test/geometry/test_geometry_dip.py
+-rw-r--r--   0        0        0     8559 2023-07-18 00:00:42.994290 solvis-0.8.1/test/geometry/test_geometry_distance.py
+-rw-r--r--   0        0        0     2827 2023-07-18 00:00:42.994290 solvis-0.8.1/test/geometry/test_geometry_performance.py
+-rw-r--r--   0        0        0     4444 2023-07-18 00:00:42.994290 solvis-0.8.1/test/geometry/test_geometry_subduction.py
+-rw-r--r--   0        0        0     6809 2023-07-18 00:00:42.994290 solvis-0.8.1/test/test_composite_solution.py
+-rw-r--r--   0        0        0     4432 2023-07-18 00:00:42.994290 solvis-0.8.1/test/test_dataframe_serialisation.py
+-rw-r--r--   0        0        0    10643 2023-07-18 00:00:42.994290 solvis-0.8.1/test/test_fault_system_solution.py
+-rw-r--r--   0        0        0     4314 2023-07-18 00:00:42.994290 solvis-0.8.1/test/test_inversion_solution.py
+-rw-r--r--   0        0        0     5201 2023-07-18 00:00:42.994290 solvis-0.8.1/test/test_new_inversion_solution.py
+-rw-r--r--   0        0        0     1905 2023-07-18 00:00:42.994290 solvis-0.8.1/test/test_solution_surfaces_builder.py
+-rw-r--r--   0        0        0     1206 2023-07-18 00:00:42.994290 solvis-0.8.1/test/test_solvis.py
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 solvis-0.8.1/PKG-INFO
```

### Comparing `solvis-0.8.0/LICENSE` & `solvis-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/README.md` & `solvis-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/pyproject.toml` & `solvis-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solvis"
-version = "0.8.0"
+version = "0.8.1"
 description = "analysis of opensha modular solution files."
 authors = ["Chris Chamberlain <chrisbc@artisan.co.nz>"]
 license = "AGPL3"
 readme = "README.md"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `solvis-0.8.0/solvis/geometry.py` & `solvis-0.8.1/solvis/geometry.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/get_secret.py` & `solvis-0.8.1/solvis/get_secret.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/composite_solution.py` & `solvis-0.8.1/solvis/inversion_solution/composite_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/fault_system_solution.py` & `solvis-0.8.1/solvis/inversion_solution/fault_system_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/fault_system_solution_file.py` & `solvis-0.8.1/solvis/inversion_solution/fault_system_solution_file.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/inversion_solution.py` & `solvis-0.8.1/solvis/inversion_solution/inversion_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/inversion_solution_file.py` & `solvis-0.8.1/solvis/inversion_solution/inversion_solution_file.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/inversion_solution_operations.py` & `solvis-0.8.1/solvis/inversion_solution/inversion_solution_operations.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/solution_surfaces_builder.py` & `solvis-0.8.1/solvis/inversion_solution/solution_surfaces_builder.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/inversion_solution/typing.py` & `solvis-0.8.1/solvis/inversion_solution/typing.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/solvis/solvis.py` & `solvis-0.8.1/solvis/solvis.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/conftest.py` & `solvis-0.8.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip` & `solvis-0.8.1/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/CrustalSmallSolution_compat.zip` & `solvis-0.8.1/test/fixtures/CrustalSmallSolution_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/CrustalSmallSolution_non_compat.zip` & `solvis-0.8.1/test/fixtures/CrustalSmallSolution_non_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/HikurangiSmallSolution_compat.zip` & `solvis-0.8.1/test/fixtures/HikurangiSmallSolution_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/HikurangiSmallSolution_non_compat.zip` & `solvis-0.8.1/test/fixtures/HikurangiSmallSolution_non_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/README` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/README`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/indices.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/indices.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/modules.json` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/modules.json`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/plausibility.json` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/plausibility.json`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/properties.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/properties.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/modules.json` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/modules.json`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/rates.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/rates.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv` & `solvis-0.8.1/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/ModularAlpineVernonInversionSolution.zip` & `solvis-0.8.1/test/fixtures/ModularAlpineVernonInversionSolution.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip` & `solvis-0.8.1/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/PuysegurSmallSolution_compat.zip` & `solvis-0.8.1/test/fixtures/PuysegurSmallSolution_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/PuysegurSmallSolution_non_compat.zip` & `solvis-0.8.1/test/fixtures/PuysegurSmallSolution_non_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/hik_fault_sections.geojson` & `solvis-0.8.1/test/fixtures/hik_fault_sections.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/fixtures/puy_fault_sections.geojson` & `solvis-0.8.1/test/fixtures/puy_fault_sections.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/geometry/test_circle_polygon.py` & `solvis-0.8.1/test/geometry/test_circle_polygon.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/geometry/test_geometry.py` & `solvis-0.8.1/test/geometry/test_geometry.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/geometry/test_geometry_dip.py` & `solvis-0.8.1/test/geometry/test_geometry_dip.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/geometry/test_geometry_distance.py` & `solvis-0.8.1/test/geometry/test_geometry_distance.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/geometry/test_geometry_performance.py` & `solvis-0.8.1/test/geometry/test_geometry_performance.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/geometry/test_geometry_subduction.py` & `solvis-0.8.1/test/geometry/test_geometry_subduction.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/test_composite_solution.py` & `solvis-0.8.1/test/test_composite_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/test_dataframe_serialisation.py` & `solvis-0.8.1/test/test_dataframe_serialisation.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/test_fault_system_solution.py` & `solvis-0.8.1/test/test_fault_system_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/test_inversion_solution.py` & `solvis-0.8.1/test/test_inversion_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/test_new_inversion_solution.py` & `solvis-0.8.1/test/test_new_inversion_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/test_solution_surfaces_builder.py` & `solvis-0.8.1/test/test_solution_surfaces_builder.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/test/test_solvis.py` & `solvis-0.8.1/test/test_solvis.py`

 * *Files identical despite different names*

### Comparing `solvis-0.8.0/PKG-INFO` & `solvis-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvis
-Version: 0.8.0
+Version: 0.8.1
 Summary: analysis of opensha modular solution files.
 License: AGPL3
 Author: Chris Chamberlain
 Author-email: chrisbc@artisan.co.nz
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

