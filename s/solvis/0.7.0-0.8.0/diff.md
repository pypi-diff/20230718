# Comparing `tmp/solvis-0.7.0.tar.gz` & `tmp/solvis-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvis-0.7.0.tar", max compression
+gzip compressed data, was "solvis-0.8.0.tar", max compression
```

## Comparing `solvis-0.7.0.tar` & `solvis-0.8.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0    34523 2023-04-26 23:13:11.534536 solvis-0.7.0/LICENSE
--rw-r--r--   0        0        0     2733 2023-04-26 23:13:11.534536 solvis-0.7.0/README.md
--rw-r--r--   0        0        0     2517 2023-04-26 23:13:11.538535 solvis-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      239 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/__init__.py
--rw-r--r--   0        0        0      369 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/config.py
--rw-r--r--   0        0        0     8314 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/geometry.py
--rw-r--r--   0        0        0     2512 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/get_secret.py
--rw-r--r--   0        0        0      155 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/__init__.py
--rw-r--r--   0        0        0     4119 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/composite_solution.py
--rw-r--r--   0        0        0     7983 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/fault_system_solution.py
--rw-r--r--   0        0        0     4750 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/fault_system_solution_file.py
--rw-r--r--   0        0        0     2576 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/inversion_solution.py
--rw-r--r--   0        0        0     8832 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/inversion_solution_file.py
--rw-r--r--   0        0        0     5860 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/inversion_solution_operations.py
--rw-r--r--   0        0        0     3053 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/solution_surfaces_builder.py
--rw-r--r--   0        0        0     3005 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/inversion_solution/typing.py
--rw-r--r--   0        0        0     1809 2023-04-26 23:13:11.538535 solvis-0.7.0/solvis/solvis.py
--rw-r--r--   0        0        0        0 2023-04-26 23:13:11.538535 solvis-0.7.0/test/__init__.py
--rw-r--r--   0        0        0     6174 2023-04-26 23:13:11.538535 solvis-0.7.0/test/conftest.py
--rw-r--r--   0        0        0  1390671 2023-04-26 23:13:11.542536 solvis-0.7.0/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip
--rw-r--r--   0        0        0   306556 2023-04-26 23:13:11.546536 solvis-0.7.0/test/fixtures/CrustalSmallSolution_compat.zip
--rw-r--r--   0        0        0   306556 2023-04-26 23:13:11.546536 solvis-0.7.0/test/fixtures/CrustalSmallSolution_non_compat.zip
--rw-r--r--   0        0        0   329085 2023-04-26 23:13:11.546536 solvis-0.7.0/test/fixtures/HikurangiSmallSolution_compat.zip
--rw-r--r--   0        0        0   329085 2023-04-26 23:13:11.546536 solvis-0.7.0/test/fixtures/HikurangiSmallSolution_non_compat.zip
--rw-r--r--   0        0        0      791 2023-04-26 23:13:11.546536 solvis-0.7.0/test/fixtures/MiniInversionSolution/README
--rw-r--r--   0        0        0      470 2023-04-26 23:13:11.546536 solvis-0.7.0/test/fixtures/MiniInversionSolution/modules.json
--rw-r--r--   0        0        0    21893 2023-04-26 23:13:11.546536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv
--rw-r--r--   0        0        0  1678031 2023-04-26 23:13:11.554536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson
--rw-r--r--   0        0        0   425032 2023-04-26 23:13:11.554536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv
--rw-r--r--   0        0        0   654267 2023-04-26 23:13:11.558536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv
--rw-r--r--   0        0        0  2486065 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson
--rw-r--r--   0        0        0   156269 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/indices.csv
--rw-r--r--   0        0        0       36 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/info.txt
--rw-r--r--   0        0        0    15992 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json
--rw-r--r--   0        0        0     2495 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json
--rw-r--r--   0        0        0    22534 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv
--rw-r--r--   0        0        0     2385 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/modules.json
--rw-r--r--   0        0        0   485782 2023-04-26 23:13:11.566536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/plausibility.json
--rw-r--r--   0        0        0    77673 2023-04-26 23:13:11.570536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/properties.csv
--rw-r--r--   0        0        0    26727 2023-04-26 23:13:11.570536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json
--rw-r--r--   0        0        0    52224 2023-04-26 23:13:11.570536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv
--rw-r--r--   0        0        0  2688710 2023-04-26 23:13:11.578536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson
--rw-r--r--   0        0        0    36289 2023-04-26 23:13:11.578536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv
--rw-r--r--   0        0        0  1055188 2023-04-26 23:13:11.582536 solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv
--rw-r--r--   0        0        0  1028684 2023-04-26 23:13:11.590536 solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv
--rw-r--r--   0        0        0      173 2023-04-26 23:13:11.590536 solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/build_info.json
--rw-r--r--   0        0        0      670 2023-04-26 23:13:11.590536 solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/modules.json
--rw-r--r--   0        0        0     7958 2023-04-26 23:13:11.590536 solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/rates.csv
--rw-r--r--   0        0        0  1055188 2023-04-26 23:13:11.594536 solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv
--rw-r--r--   0        0        0   450515 2023-04-26 23:13:11.594536 solvis-0.7.0/test/fixtures/ModularAlpineVernonInversionSolution.zip
--rw-r--r--   0        0        0   842948 2023-04-26 23:13:11.598536 solvis-0.7.0/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip
--rw-r--r--   0        0        0   214824 2023-04-26 23:13:11.598536 solvis-0.7.0/test/fixtures/PuysegurSmallSolution_compat.zip
--rw-r--r--   0        0        0   214824 2023-04-26 23:13:11.598536 solvis-0.7.0/test/fixtures/PuysegurSmallSolution_non_compat.zip
--rw-r--r--   0        0        0   466256 2023-04-26 23:13:11.602536 solvis-0.7.0/test/fixtures/hik_fault_sections.geojson
--rw-r--r--   0        0        0   241379 2023-04-26 23:13:11.602536 solvis-0.7.0/test/fixtures/puy_fault_sections.geojson
--rw-r--r--   0        0        0     1540 2023-04-26 23:13:11.602536 solvis-0.7.0/test/geometry/test_circle_polygon.py
--rw-r--r--   0        0        0     3359 2023-04-26 23:13:11.602536 solvis-0.7.0/test/geometry/test_geometry.py
--rw-r--r--   0        0        0    11190 2023-04-26 23:13:11.602536 solvis-0.7.0/test/geometry/test_geometry_dip.py
--rw-r--r--   0        0        0     8559 2023-04-26 23:13:11.602536 solvis-0.7.0/test/geometry/test_geometry_distance.py
--rw-r--r--   0        0        0     2827 2023-04-26 23:13:11.602536 solvis-0.7.0/test/geometry/test_geometry_performance.py
--rw-r--r--   0        0        0     4444 2023-04-26 23:13:11.602536 solvis-0.7.0/test/geometry/test_geometry_subduction.py
--rw-r--r--   0        0        0     6809 2023-04-26 23:13:11.602536 solvis-0.7.0/test/test_composite_solution.py
--rw-r--r--   0        0        0     4432 2023-04-26 23:13:11.602536 solvis-0.7.0/test/test_dataframe_serialisation.py
--rw-r--r--   0        0        0    10643 2023-04-26 23:13:11.602536 solvis-0.7.0/test/test_fault_system_solution.py
--rw-r--r--   0        0        0     4314 2023-04-26 23:13:11.602536 solvis-0.7.0/test/test_inversion_solution.py
--rw-r--r--   0        0        0     5201 2023-04-26 23:13:11.602536 solvis-0.7.0/test/test_new_inversion_solution.py
--rw-r--r--   0        0        0     1905 2023-04-26 23:13:11.602536 solvis-0.7.0/test/test_solution_surfaces_builder.py
--rw-r--r--   0        0        0     4344 1970-01-01 00:00:00.000000 solvis-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-17 22:16:26.018770 solvis-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2733 2023-07-17 22:16:26.018770 solvis-0.8.0/README.md
+-rw-r--r--   0        0        0     2593 2023-07-17 22:16:26.022770 solvis-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/__init__.py
+-rw-r--r--   0        0        0      369 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/config.py
+-rw-r--r--   0        0        0     8314 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/geometry.py
+-rw-r--r--   0        0        0     2512 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/get_secret.py
+-rw-r--r--   0        0        0      155 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/__init__.py
+-rw-r--r--   0        0        0     4119 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/composite_solution.py
+-rw-r--r--   0        0        0     7983 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/fault_system_solution.py
+-rw-r--r--   0        0        0     4750 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/fault_system_solution_file.py
+-rw-r--r--   0        0        0     2576 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/inversion_solution.py
+-rw-r--r--   0        0        0     8911 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/inversion_solution_file.py
+-rw-r--r--   0        0        0     5859 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/inversion_solution_operations.py
+-rw-r--r--   0        0        0     3053 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/solution_surfaces_builder.py
+-rw-r--r--   0        0        0     3005 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/inversion_solution/typing.py
+-rw-r--r--   0        0        0     2106 2023-07-17 22:16:26.022770 solvis-0.8.0/solvis/solvis.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:16:26.022770 solvis-0.8.0/test/__init__.py
+-rw-r--r--   0        0        0     6174 2023-07-17 22:16:26.022770 solvis-0.8.0/test/conftest.py
+-rw-r--r--   0        0        0  1390671 2023-07-17 22:16:26.026770 solvis-0.8.0/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip
+-rw-r--r--   0        0        0   306556 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/CrustalSmallSolution_compat.zip
+-rw-r--r--   0        0        0   306556 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/CrustalSmallSolution_non_compat.zip
+-rw-r--r--   0        0        0   329085 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/HikurangiSmallSolution_compat.zip
+-rw-r--r--   0        0        0   329085 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/HikurangiSmallSolution_non_compat.zip
+-rw-r--r--   0        0        0      791 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/MiniInversionSolution/README
+-rw-r--r--   0        0        0      470 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/MiniInversionSolution/modules.json
+-rw-r--r--   0        0        0    21893 2023-07-17 22:16:26.030770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv
+-rw-r--r--   0        0        0  1678031 2023-07-17 22:16:26.034770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson
+-rw-r--r--   0        0        0   425032 2023-07-17 22:16:26.038770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv
+-rw-r--r--   0        0        0   654267 2023-07-17 22:16:26.042770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv
+-rw-r--r--   0        0        0  2486065 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson
+-rw-r--r--   0        0        0   156269 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/indices.csv
+-rw-r--r--   0        0        0       36 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/info.txt
+-rw-r--r--   0        0        0    15992 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json
+-rw-r--r--   0        0        0     2495 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json
+-rw-r--r--   0        0        0    22534 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv
+-rw-r--r--   0        0        0     2385 2023-07-17 22:16:26.050770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/modules.json
+-rw-r--r--   0        0        0   485782 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/plausibility.json
+-rw-r--r--   0        0        0    77673 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/properties.csv
+-rw-r--r--   0        0        0    26727 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json
+-rw-r--r--   0        0        0    52224 2023-07-17 22:16:26.054770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv
+-rw-r--r--   0        0        0  2688710 2023-07-17 22:16:26.062770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson
+-rw-r--r--   0        0        0    36289 2023-07-17 22:16:26.062770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv
+-rw-r--r--   0        0        0  1055188 2023-07-17 22:16:26.066770 solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv
+-rw-r--r--   0        0        0  1028684 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv
+-rw-r--r--   0        0        0      173 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/build_info.json
+-rw-r--r--   0        0        0      670 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/modules.json
+-rw-r--r--   0        0        0     7958 2023-07-17 22:16:26.074770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/rates.csv
+-rw-r--r--   0        0        0  1055188 2023-07-17 22:16:26.078770 solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv
+-rw-r--r--   0        0        0   450515 2023-07-17 22:16:26.078770 solvis-0.8.0/test/fixtures/ModularAlpineVernonInversionSolution.zip
+-rw-r--r--   0        0        0   842948 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip
+-rw-r--r--   0        0        0   214824 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/PuysegurSmallSolution_compat.zip
+-rw-r--r--   0        0        0   214824 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/PuysegurSmallSolution_non_compat.zip
+-rw-r--r--   0        0        0   466256 2023-07-17 22:16:26.082770 solvis-0.8.0/test/fixtures/hik_fault_sections.geojson
+-rw-r--r--   0        0        0   241379 2023-07-17 22:16:26.086770 solvis-0.8.0/test/fixtures/puy_fault_sections.geojson
+-rw-r--r--   0        0        0     1540 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_circle_polygon.py
+-rw-r--r--   0        0        0     3359 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry.py
+-rw-r--r--   0        0        0    11190 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_dip.py
+-rw-r--r--   0        0        0     8559 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_distance.py
+-rw-r--r--   0        0        0     2827 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_performance.py
+-rw-r--r--   0        0        0     4444 2023-07-17 22:16:26.086770 solvis-0.8.0/test/geometry/test_geometry_subduction.py
+-rw-r--r--   0        0        0     6809 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_composite_solution.py
+-rw-r--r--   0        0        0     4432 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_dataframe_serialisation.py
+-rw-r--r--   0        0        0    10643 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_fault_system_solution.py
+-rw-r--r--   0        0        0     4314 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_inversion_solution.py
+-rw-r--r--   0        0        0     5201 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_new_inversion_solution.py
+-rw-r--r--   0        0        0     1905 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_solution_surfaces_builder.py
+-rw-r--r--   0        0        0     1206 2023-07-17 22:16:26.086770 solvis-0.8.0/test/test_solvis.py
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 solvis-0.8.0/PKG-INFO
```

### Comparing `solvis-0.7.0/LICENSE` & `solvis-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/README.md` & `solvis-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/pyproject.toml` & `solvis-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solvis"
-version = "0.7.0"
+version = "0.8.0"
 description = "analysis of opensha modular solution files."
 authors = ["Chris Chamberlain <chrisbc@artisan.co.nz>"]
 license = "AGPL3"
 readme = "README.md"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -20,26 +20,29 @@
     {include = "test", format = "sdist" }
 ]
 
 [tool.poetry.scripts]
 cli = 'scripts.cli:cli'
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-pandas = "^1.3.4"
-python-dateutil = "^2.8.2"
+boto3 = {version = "^1.26.82", optional = true, extras = ["scripts"]}
 click = "^8.1.3"
 click-plugins = "^1.1.1"
-geopandas = "^0.12.2"
-pytz = "2021.3"
-pyproj = "^3.3"
-pyvista = {version = "^0.37.0", optional = true, extras = ["vtk"]}
 nshm-toshi-client = {version = "^1.0.0", optional = true, extras = ["scripts"]}
-boto3 = {version = "^1.26.82", optional = true, extras = ["scripts"]}
 nzshm-model = {version = "^0.3.0", optional = true, extras = ["scripts"]}
+pyproj = "^3.3"
+python = ">=3.9,<4.0"
+python-dateutil = "^2.8.2"
+pytz = "2021.3"
+pyvista = {version = "^0.37.0", optional = true, extras = ["vtk"]}
+
+# see https://github.com/orgs/python-poetry/discussions/7937
+urllib3 = "<2" 
+geopandas = "^0.13.2"
+numpy = "<1.25"
 
 [tool.poetry.group.dev.dependencies]
 black  = { version = "^22.3"}
 bump2version = "^1.0.1"
 isort  = { version = "^5.8.0"}
 flake8  = { version = "^3.9.2"}
 flake8-docstrings = { version = "^1.6.0", optional = true }
```

### Comparing `solvis-0.7.0/solvis/geometry.py` & `solvis-0.8.0/solvis/geometry.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/get_secret.py` & `solvis-0.8.0/solvis/get_secret.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/inversion_solution/composite_solution.py` & `solvis-0.8.0/solvis/inversion_solution/composite_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/inversion_solution/fault_system_solution.py` & `solvis-0.8.0/solvis/inversion_solution/fault_system_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/inversion_solution/fault_system_solution_file.py` & `solvis-0.8.0/solvis/inversion_solution/fault_system_solution_file.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/inversion_solution/inversion_solution.py` & `solvis-0.8.0/solvis/inversion_solution/inversion_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/inversion_solution/inversion_solution_file.py` & `solvis-0.8.0/solvis/inversion_solution/inversion_solution_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,16 @@
             else:
                 tic = time.perf_counter()
                 self._archive = zipfile.ZipFile(self._archive_path)
                 toc = time.perf_counter()
                 log.debug('archive time to open zipfile %s %2.3f seconds' % (self._archive_path, toc - tic))
         return self._archive
 
-    def _dataframe_from_csv(self, prop, path, dtype={}):
+    def _dataframe_from_csv(self, prop, path, dtype=None):
+        log.debug('_dataframe_from_csv( %s, %s, %s )' % (prop, path, dtype))
         if not isinstance(prop, pd.DataFrame):
             tic = time.perf_counter()
             data = self.archive.open(path)
             toc = time.perf_counter()
             log.debug('dataframe_from_csv() time to open datafile %s %2.3f seconds' % (path, toc - tic))
             tic = time.perf_counter()
             prop = pd.read_csv(data, dtype=dtype)
```

### Comparing `solvis-0.7.0/solvis/inversion_solution/inversion_solution_operations.py` & `solvis-0.8.0/solvis/inversion_solution/inversion_solution_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     @property
     def fault_sections(self) -> gpd.GeoDataFrame:
         tic = time.perf_counter()
         fault_sections = self._geodataframe_from_geojson(self._fault_sections, self.FAULTS_PATH)
         toc = time.perf_counter()
         log.debug('fault_sections: time to load fault_sections: %2.3f seconds' % (toc - tic))
-
         return fault_sections
 
     @property
     def rupture_sections(self) -> gpd.GeoDataFrame:
 
         if self._rupture_sections is not None:
             return self._rupture_sections  # pragma: no cover
```

### Comparing `solvis-0.7.0/solvis/inversion_solution/solution_surfaces_builder.py` & `solvis-0.8.0/solvis/inversion_solution/solution_surfaces_builder.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/inversion_solution/typing.py` & `solvis-0.8.0/solvis/inversion_solution/typing.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/solvis/solvis.py` & `solvis-0.8.0/solvis/solvis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 #!python3
 
 # from functools import partial
 from pathlib import Path
-from typing import Union
+from typing import Callable, Iterable, List, Union
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
 from solvis.inversion_solution.typing import InversionSolutionProtocol
 
 
+def parent_fault_names(
+    sol: InversionSolutionProtocol, sort: Union[None, Callable[[Iterable], List]] = sorted
+) -> List[str]:
+    if sort:
+        return sort(sol.fault_sections.ParentName.unique())
+    return list(sol.fault_sections.ParentName.unique())
+
+
 # filtered_rupture_sections (with geometry)
 def section_participation(sol: InversionSolutionProtocol, df_ruptures: pd.DataFrame = None):
     sr = sol.rs_with_rates
     if df_ruptures is not None:
-        filtered_sections_with_rates_df = sr[(sr.rupture.isin(list(df_ruptures))) & (sr['Annual Rate'] > 0)]
+        filtered_sections_with_rates_df = sr[(sr["Rupture Index"].isin(list(df_ruptures))) & (sr['Annual Rate'] > 0)]
     else:
         filtered_sections_with_rates_df = sr
 
     # print("Pivot table (note precision is not lost!!)")
     # participation (sum of rate) for every rupture though a point
     section_sum_of_rates_df = filtered_sections_with_rates_df.pivot_table(
         values='Annual Rate', index=['section'], aggfunc=np.sum
```

### Comparing `solvis-0.7.0/test/conftest.py` & `solvis-0.8.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip` & `solvis-0.8.0/test/fixtures/AveragedHikurangiInversionSolution-QXV0b21hdGlvblRhc2s6MTA3MzMy.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/CrustalSmallSolution_compat.zip` & `solvis-0.8.0/test/fixtures/CrustalSmallSolution_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/CrustalSmallSolution_non_compat.zip` & `solvis-0.8.0/test/fixtures/CrustalSmallSolution_non_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/HikurangiSmallSolution_compat.zip` & `solvis-0.8.0/test/fixtures/HikurangiSmallSolution_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/HikurangiSmallSolution_non_compat.zip` & `solvis-0.8.0/test/fixtures/HikurangiSmallSolution_non_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/README` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/README`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/average_slips.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/fault_sections.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_association_fracts.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_node_sect_associations.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/grid_region.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/indices.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/indices.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/inversion_target_mfds.json`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/logic_tree_branch.json`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/mod_sect_min_mags.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/modules.json` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/modules.json`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/plausibility.json` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/plausibility.json`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/properties.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/properties.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/regional_inversion_target_mfds.json`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_areas.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_polygons.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sect_slip_rates.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/ruptures/sub_seismo_on_fault_mfds.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/annealing_progress.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/modules.json` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/modules.json`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/rates.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/rates.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv` & `solvis-0.8.0/test/fixtures/MiniInversionSolution/solution/sub_seismo_on_fault_mfds.csv`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/ModularAlpineVernonInversionSolution.zip` & `solvis-0.8.0/test/fixtures/ModularAlpineVernonInversionSolution.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip` & `solvis-0.8.0/test/fixtures/PuysegurInversionSolution-QXV0b21hdGlvblRhc2s6MTExMDA1.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/PuysegurSmallSolution_compat.zip` & `solvis-0.8.0/test/fixtures/PuysegurSmallSolution_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/PuysegurSmallSolution_non_compat.zip` & `solvis-0.8.0/test/fixtures/PuysegurSmallSolution_non_compat.zip`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/hik_fault_sections.geojson` & `solvis-0.8.0/test/fixtures/hik_fault_sections.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/fixtures/puy_fault_sections.geojson` & `solvis-0.8.0/test/fixtures/puy_fault_sections.geojson`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/geometry/test_circle_polygon.py` & `solvis-0.8.0/test/geometry/test_circle_polygon.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/geometry/test_geometry.py` & `solvis-0.8.0/test/geometry/test_geometry.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/geometry/test_geometry_dip.py` & `solvis-0.8.0/test/geometry/test_geometry_dip.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/geometry/test_geometry_distance.py` & `solvis-0.8.0/test/geometry/test_geometry_distance.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/geometry/test_geometry_performance.py` & `solvis-0.8.0/test/geometry/test_geometry_performance.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/geometry/test_geometry_subduction.py` & `solvis-0.8.0/test/geometry/test_geometry_subduction.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/test_composite_solution.py` & `solvis-0.8.0/test/test_composite_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/test_dataframe_serialisation.py` & `solvis-0.8.0/test/test_dataframe_serialisation.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/test_fault_system_solution.py` & `solvis-0.8.0/test/test_fault_system_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/test_inversion_solution.py` & `solvis-0.8.0/test/test_inversion_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/test_new_inversion_solution.py` & `solvis-0.8.0/test/test_new_inversion_solution.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/test/test_solution_surfaces_builder.py` & `solvis-0.8.0/test/test_solution_surfaces_builder.py`

 * *Files identical despite different names*

### Comparing `solvis-0.7.0/PKG-INFO` & `solvis-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 Metadata-Version: 2.1
 Name: solvis
-Version: 0.7.0
+Version: 0.8.0
 Summary: analysis of opensha modular solution files.
 License: AGPL3
 Author: Chris Chamberlain
 Author-email: chrisbc@artisan.co.nz
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: scripts
 Provides-Extra: test
 Provides-Extra: vtk
 Requires-Dist: boto3[scripts] (>=1.26.82,<2.0.0) ; extra == "scripts"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-plugins (>=1.1.1,<2.0.0)
-Requires-Dist: geopandas (>=0.12.2,<0.13.0)
+Requires-Dist: geopandas (>=0.13.2,<0.14.0)
 Requires-Dist: nshm-toshi-client[scripts] (>=1.0.0,<2.0.0) ; extra == "scripts"
+Requires-Dist: numpy (<1.25)
 Requires-Dist: nzshm-model[scripts] (>=0.3.0,<0.4.0) ; extra == "scripts"
-Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: pyproj (>=3.3,<4.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (==2021.3)
 Requires-Dist: pyvista[vtk] (>=0.37.0,<0.38.0) ; extra == "vtk"
+Requires-Dist: urllib3 (<2)
 Description-Content-Type: text/markdown
 
 # solvis
 
 [![pypi](https://img.shields.io/pypi/v/solvis.svg)](https://pypi.org/project/solvis/)
 [![python](https://img.shields.io/pypi/pyversions/solvis.svg)](https://pypi.org/project/solvis/)
 [![Build Status](https://github.com/GNS-Science/solvis/actions/workflows/dev.yml/badge.svg)](https://github.com/GNS-Science/solvis/actions/workflows/dev.yml)
```

