# Comparing `tmp/stk-2023.7.5.3.tar.gz` & `tmp/stk-2023.7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stk-2023.7.5.3.tar", last modified: Wed Jul  5 17:32:09 2023, max compression
+gzip compressed data, was "stk-2023.7.6.0.tar", last modified: Thu Jul  6 10:12:01 2023, max compression
```

## Comparing `stk-2023.7.5.3.tar` & `stk-2023.7.6.0.tar`

### file list

```diff
@@ -1,341 +1,1320 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.755530 stk-2023.7.5.3/
--rw-r--r--   0 root         (0) root         (0)     1098 2023-07-05 17:31:57.000000 stk-2023.7.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6103 2023-07-05 17:32:09.755530 stk-2023.7.5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5735 2023-07-05 17:31:57.000000 stk-2023.7.5.3/README.rst
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-05 17:31:57.000000 stk-2023.7.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 17:32:09.755530 stk-2023.7.5.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.699529 stk-2023.7.5.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.707529 stk-2023.7.5.3/src/stk/
--rw-r--r--   0 root         (0) root         (0)    14877 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.711529 stk-2023.7.5.3/src/stk/_internal/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/atom.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/atom_info.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/bond.py
--rw-r--r--   0 root         (0) root         (0)     2649 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/bond_info.py
--rw-r--r--   0 root         (0) root         (0)    37484 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/building_block.py
--rw-r--r--   0 root         (0) root         (0)    14393 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/constructed_molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.711529 stk-2023.7.5.3/src/stk/_internal/construction_result/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_result/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3700 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_result/construction_result.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_result/periodic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.711529 stk-2023.7.5.3/src/stk/_internal/construction_state/
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11906 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/construction_state.py
--rw-r--r--   0 root         (0) root         (0)    10688 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/graph_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.711529 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5684 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/deletions_summary.py
--rw-r--r--   0 root         (0) root         (0)     9278 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/molecule_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.711529 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py
--rw-r--r--   0 root         (0) root         (0)     7311 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.711529 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py
--rw-r--r--   0 root         (0) root         (0)     1319 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py
--rw-r--r--   0 root         (0) root         (0)     5218 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.715529 stk-2023.7.5.3/src/stk/_internal/databases/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/constructed_molecule.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.715529 stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27693 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/constructed_molecule.py
--rw-r--r--   0 root         (0) root         (0)    17958 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/molecule.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/utilities.py
--rw-r--r--   0 root         (0) root         (0)     6457 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/value.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/databases/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.715529 stk-2023.7.5.3/src/stk/_internal/ea/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.715529 stk-2023.7.5.3/src/stk/_internal/ea/crossover/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/crossover/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8967 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/crossover/genetic_recombination.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/crossover/molecule_crosser.py
--rw-r--r--   0 root         (0) root         (0)     7633 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/crossover/random.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/crossover/record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.715529 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.715529 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/implementations/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/implementations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/implementations/serial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.719529 stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      637 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py
--rw-r--r--   0 root         (0) root         (0)     9713 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/fitness_function.py
--rw-r--r--   0 root         (0) root         (0)    11219 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/property_vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.719529 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5818 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/add.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/multiply.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/null.py
--rw-r--r--   0 root         (0) root         (0)     7166 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/power.py
--rw-r--r--   0 root         (0) root         (0)     4105 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/sequence.py
--rw-r--r--   0 root         (0) root         (0)     7017 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/shift_up.py
--rw-r--r--   0 root         (0) root         (0)     4455 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/sum.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.719529 stk-2023.7.5.3/src/stk/_internal/ea/molecule_records/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/molecule_records/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/molecule_records/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.719529 stk-2023.7.5.3/src/stk/_internal/ea/mutation/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/mutation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/mutation/mutator.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/mutation/random.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/mutation/random_building_block.py
--rw-r--r--   0 root         (0) root         (0)     3253 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/mutation/random_topology_graph.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/mutation/record.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/mutation/similar_building_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.719529 stk-2023.7.5.3/src/stk/_internal/ea/plotters/
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/plotters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13994 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/plotters/progress.py
--rw-r--r--   0 root         (0) root         (0)     7603 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/plotters/selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.723529 stk-2023.7.5.3/src/stk/_internal/ea/selection/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7886 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.723529 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/above_average.py
--rw-r--r--   0 root         (0) root         (0)     5939 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/best.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/filter_batches.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/filter_molecules.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/remove_batches.py
--rw-r--r--   0 root         (0) root         (0)     2629 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/remove_molecules.py
--rw-r--r--   0 root         (0) root         (0)     6006 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/roulette.py
--rw-r--r--   0 root         (0) root         (0)     7396 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/selector.py
--rw-r--r--   0 root         (0) root         (0)     7125 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py
--rw-r--r--   0 root         (0) root         (0)     4934 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/tournament.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.723529 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/utilities/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/worst.py
--rw-r--r--   0 root         (0) root         (0)    25498 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/elements.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.727530 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4502 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/alcohol_factory.py
--rw-r--r--   0 root         (0) root         (0)     4376 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/aldehyde_factory.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/amide_factory.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/boronic_acid_factory.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/bromo_factory.py
--rw-r--r--   0 root         (0) root         (0)     4534 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py
--rw-r--r--   0 root         (0) root         (0)     4280 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/dibromo_factory.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/difluoro_factory.py
--rw-r--r--   0 root         (0) root         (0)     4412 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/diol_factory.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/fluoro_factory.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/functional_group_factory.py
--rw-r--r--   0 root         (0) root         (0)     2702 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/iodo_factory.py
--rw-r--r--   0 root         (0) root         (0)     4602 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/primary_amino_factory.py
--rw-r--r--   0 root         (0) root         (0)     1326 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/ring_amine_factory.py
--rw-r--r--   0 root         (0) root         (0)     4411 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/secondary_amino_factory.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/smarts.py
--rw-r--r--   0 root         (0) root         (0)     4479 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py
--rw-r--r--   0 root         (0) root         (0)     4228 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/thioacid_factory.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/thiol_factory.py
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_group_factories/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.731530 stk-2023.7.5.3/src/stk/_internal/functional_groups/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3224 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/alcohol.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/aldehyde.py
--rw-r--r--   0 root         (0) root         (0)     4507 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/alkene.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/alkyne.py
--rw-r--r--   0 root         (0) root         (0)     4815 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/amide.py
--rw-r--r--   0 root         (0) root         (0)     4869 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/boronic_acid.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/bromo.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/carboxylic_acid.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/dibromo.py
--rw-r--r--   0 root         (0) root         (0)     3218 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/difluoro.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/diol.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/fluoro.py
--rw-r--r--   0 root         (0) root         (0)    11798 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/functional_group.py
--rw-r--r--   0 root         (0) root         (0)     4825 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/generic_functional_group.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/iodo.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/primary_amino.py
--rw-r--r--   0 root         (0) root         (0)     4671 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/ring_amine.py
--rw-r--r--   0 root         (0) root         (0)     3382 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/secondary_amino.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/single_atom.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/thioacid.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/functional_groups/thiol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.731530 stk-2023.7.5.3/src/stk/_internal/json_serde/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/json_serde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9926 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/json_serde/constructed_molecule.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/json_serde/molecule.py
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/json_serde/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.731530 stk-2023.7.5.3/src/stk/_internal/key_makers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/key_makers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/key_makers/inchi.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/key_makers/inchi_key.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/key_makers/molecule.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/key_makers/smiles.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/key_makers/utilities.py
--rw-r--r--   0 root         (0) root         (0)    25466 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.735530 stk-2023.7.5.3/src/stk/_internal/optimizers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/collapser.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/mchammer.py
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/null.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3839 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/periodic_collapser.py
--rw-r--r--   0 root         (0) root         (0)     4456 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/spinner.py
--rw-r--r--   0 root         (0) root         (0)     2118 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/optimizers/utilities.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/periodic_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.735530 stk-2023.7.5.3/src/stk/_internal/reaction_factories/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reaction_factories/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reaction_factories/dative_reaction_factory.py
--rw-r--r--   0 root         (0) root         (0)     6034 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reaction_factories/generic_reaction_factory.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reaction_factories/reaction_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.735530 stk-2023.7.5.3/src/stk/_internal/reactions/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.735530 stk-2023.7.5.3/src/stk/_internal/reactions/dative_reaction/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/dative_reaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/dative_reaction/dative_reaction.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/dative_reaction/utilities.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/one_one_reaction.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/one_two_reaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.735530 stk-2023.7.5.3/src/stk/_internal/reactions/reaction/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/reaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/reaction/new_atom.py
--rw-r--r--   0 root         (0) root         (0)     3615 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/reaction/reaction.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/reaction/reaction_result.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/ring_amine_reaction.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/reactions/two_two_reaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.739530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.743530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42840 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/cage.py
--rw-r--r--   0 root         (0) root         (0)     8079 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/cage_construction_state.py
--rw-r--r--   0 root         (0) root         (0)     8062 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py
--rw-r--r--   0 root         (0) root         (0)     6824 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py
--rw-r--r--   0 root         (0) root         (0)     5631 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/five_plus_ten.py
--rw-r--r--   0 root         (0) root         (0)     5034 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_eight.py
--rw-r--r--   0 root         (0) root         (0)     4120 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_four.py
--rw-r--r--   0 root         (0) root         (0)     4907 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_six.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py
--rw-r--r--   0 root         (0) root         (0)     7536 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m12l24.py
--rw-r--r--   0 root         (0) root         (0)    13449 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m24l48.py
--rw-r--r--   0 root         (0) root         (0)     5151 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py
--rw-r--r--   0 root         (0) root         (0)     8175 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py
--rw-r--r--   0 root         (0) root         (0)     7429 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m3l6.py
--rw-r--r--   0 root         (0) root         (0)     7982 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l4_square.py
--rw-r--r--   0 root         (0) root         (0)     7987 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     9248 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py
--rw-r--r--   0 root         (0) root         (0)     8786 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py
--rw-r--r--   0 root         (0) root         (0)     5904 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l8.py
--rw-r--r--   0 root         (0) root         (0)     6744 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m6l12_cube.py
--rw-r--r--   0 root         (0) root         (0)     9469 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py
--rw-r--r--   0 root         (0) root         (0)     9502 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m8l6_cube.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/one_plus_one.py
--rw-r--r--   0 root         (0) root         (0)     6788 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/six_plus_eight.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/six_plus_nine.py
--rw-r--r--   0 root         (0) root         (0)     6684 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py
--rw-r--r--   0 root         (0) root         (0)     8949 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py
--rw-r--r--   0 root         (0) root         (0)     4697 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/three_plus_six.py
--rw-r--r--   0 root         (0) root         (0)    11770 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py
--rw-r--r--   0 root         (0) root         (0)    10975 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/two_plus_four.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/two_plus_three.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/two_plus_two.py
--rw-r--r--   0 root         (0) root         (0)    11358 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.747530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/
--rw-r--r--   0 root         (0) root         (0)      412 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27030 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/cof.py
--rw-r--r--   0 root         (0) root         (0)     1934 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/edge.py
--rw-r--r--   0 root         (0) root         (0)     8245 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/hexagonal.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/honeycomb.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/kagome.py
--rw-r--r--   0 root         (0) root         (0)     3904 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py
--rw-r--r--   0 root         (0) root         (0)    12091 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py
--rw-r--r--   0 root         (0) root         (0)     8737 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py
--rw-r--r--   0 root         (0) root         (0)    10199 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_kagome.py
--rw-r--r--   0 root         (0) root         (0)     7760 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py
--rw-r--r--   0 root         (0) root         (0)     8551 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_square.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/square.py
--rw-r--r--   0 root         (0) root         (0)    11377 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/vertices.py
--rw-r--r--   0 root         (0) root         (0)     5569 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/edge.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/edge_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.747530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/host_guest/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/host_guest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17325 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/host_guest/complex.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/host_guest/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.747530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/macrocycle/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/macrocycle/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18837 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/macrocycle/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.751530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py
--rw-r--r--   0 root         (0) root         (0)     2919 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py
--rw-r--r--   0 root         (0) root         (0)    26537 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/octahedral.py
--rw-r--r--   0 root         (0) root         (0)     3944 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/square_planar.py
--rw-r--r--   0 root         (0) root         (0)     4667 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.751530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.751530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/linear/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/linear/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24349 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/linear/linear.py
--rw-r--r--   0 root         (0) root         (0)     6057 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/linear/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.751530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/rotaxane/
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/rotaxane/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20644 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/rotaxane/vertices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.751530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2131 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/parallel.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/serial.py
--rw-r--r--   0 root         (0) root         (0)    19701 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.751530 stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/edge_sorter.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/sorter.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/topology_graphs/vertex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.751530 stk-2023.7.5.3/src/stk/_internal/utilities/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/molecule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.755530 stk-2023.7.5.3/src/stk/_internal/utilities/updaters/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/updaters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/updaters/mae.py
--rw-r--r--   0 root         (0) root         (0)      745 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/updaters/mdl_mol.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/updaters/pdb.py
--rw-r--r--   0 root         (0) root         (0)     5796 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/updaters/turbomole.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/updaters/xyz.py
--rw-r--r--   0 root         (0) root         (0)    23774 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.755530 stk-2023.7.5.3/src/stk/_internal/utilities/writers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/writers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/writers/mdl_mol.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/writers/pdb.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/utilities/writers/xyz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.755530 stk-2023.7.5.3/src/stk/_internal/writers/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/writers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/writers/mdl_mol.py
--rw-r--r--   0 root         (0) root         (0)     6082 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/writers/pdb.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/writers/turbomole.py
--rw-r--r--   0 root         (0) root         (0)     2904 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/_internal/writers/xyz.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-07-05 17:32:09.000000 stk-2023.7.5.3/src/stk/_version.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/cage.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/cof.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/host_guest.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/macrocycle.py
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/metal_complex.py
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/polymer.py
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-05 17:31:57.000000 stk-2023.7.5.3/src/stk/rotaxane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:09.707529 stk-2023.7.5.3/src/stk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6103 2023-07-05 17:32:09.000000 stk-2023.7.5.3/src/stk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15113 2023-07-05 17:32:09.000000 stk-2023.7.5.3/src/stk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:32:09.000000 stk-2023.7.5.3/src/stk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-05 17:32:09.000000 stk-2023.7.5.3/src/stk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-05 17:32:09.000000 stk-2023.7.5.3/src/stk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.096314 stk-2023.7.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.948313 stk-2023.7.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-06 10:11:05.000000 stk-2023.7.6.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.948313 stk-2023.7.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-06 10:11:05.000000 stk-2023.7.6.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-06 10:11:05.000000 stk-2023.7.6.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-06 10:11:05.000000 stk-2023.7.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 10:11:05.000000 stk-2023.7.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-06 10:11:05.000000 stk-2023.7.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-06 10:12:01.096314 stk-2023.7.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-06 10:11:05.000000 stk-2023.7.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.948313 stk-2023.7.6.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.948313 stk-2023.7.6.0/benchmarks/cof/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/benchmarks/cof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-06 10:11:05.000000 stk-2023.7.6.0/benchmarks/cof/benchmark_kagome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.948313 stk-2023.7.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.952313 stk-2023.7.6.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.952313 stk-2023.7.6.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   505277 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/_static/stk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.952313 stk-2023.7.6.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26916 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/basic_ea_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    45165 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/basic_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/cage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/cof.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/constructed_molecule_databases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/construction_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/crossover.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/fitness_calculators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/fitness_normalizers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/functional_group_factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/functional_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25425 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/intermediate_ea_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/key_makers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/metal_complex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/molecule_databases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/mutation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/optimizers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/plotters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/polymer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/reaction_factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/reactions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/selection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/value_databases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/video_tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 10:11:05.000000 stk-2023.7.6.0/docs/source/writers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-06 10:11:05.000000 stk-2023.7.6.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-06 10:11:05.000000 stk-2023.7.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:12:01.096314 stk-2023.7.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.932312 stk-2023.7.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.952313 stk-2023.7.6.0/src/stk/
+-rw-r--r--   0 runner    (1001) docker     (123)    14877 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/atom_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/bond_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37484 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/building_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/constructed_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/construction_result/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_result/construction_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_result/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/construction_state/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/construction_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/graph_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/deletions_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/molecule_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/constructed_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27693 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/constructed_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/databases/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.956313 stk-2023.7.6.0/src/stk/_internal/ea/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.960313 stk-2023.7.6.0/src/stk/_internal/ea/crossover/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/crossover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/crossover/genetic_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/crossover/molecule_crosser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/crossover/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/crossover/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.960313 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.960313 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.960313 stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/fitness_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/property_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.960313 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/shift_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.960313 stk-2023.7.6.0/src/stk/_internal/ea/molecule_records/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/molecule_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/molecule_records/molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.960313 stk-2023.7.6.0/src/stk/_internal/ea/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/mutation/mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/mutation/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/mutation/random_building_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/mutation/random_topology_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/mutation/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/mutation/similar_building_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.964313 stk-2023.7.6.0/src/stk/_internal/ea/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/plotters/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/plotters/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.964313 stk-2023.7.6.0/src/stk/_internal/ea/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.964313 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/above_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/best.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/filter_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/filter_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/remove_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/remove_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/roulette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/tournament.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.964313 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/worst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.968313 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/alcohol_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/aldehyde_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/amide_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/boronic_acid_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/bromo_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/dibromo_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/difluoro_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/diol_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/fluoro_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/functional_group_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/iodo_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/primary_amino_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/ring_amine_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/secondary_amino_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/smarts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/thioacid_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/thiol_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_group_factories/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.968313 stk-2023.7.6.0/src/stk/_internal/functional_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/aldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/alkene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/alkyne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/amide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/boronic_acid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/bromo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/carboxylic_acid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/dibromo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/difluoro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/diol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/fluoro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/functional_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/generic_functional_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/iodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/primary_amino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/ring_amine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/secondary_amino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/single_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/thioacid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/functional_groups/thiol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.968313 stk-2023.7.6.0/src/stk/_internal/json_serde/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/json_serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/json_serde/constructed_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/json_serde/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/json_serde/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.972313 stk-2023.7.6.0/src/stk/_internal/key_makers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/key_makers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/key_makers/inchi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/key_makers/inchi_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/key_makers/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/key_makers/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/key_makers/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25466 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.972313 stk-2023.7.6.0/src/stk/_internal/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/collapser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/mchammer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/periodic_collapser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/optimizers/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/periodic_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.972313 stk-2023.7.6.0/src/stk/_internal/reaction_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reaction_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reaction_factories/dative_reaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reaction_factories/generic_reaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reaction_factories/reaction_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.972313 stk-2023.7.6.0/src/stk/_internal/reactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.972313 stk-2023.7.6.0/src/stk/_internal/reactions/dative_reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/dative_reaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/dative_reaction/dative_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/dative_reaction/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/one_one_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/one_two_reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.972313 stk-2023.7.6.0/src/stk/_internal/reactions/reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/reaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/reaction/new_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/reaction/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/reaction/reaction_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/ring_amine_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/reactions/two_two_reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.972313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.980313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/cage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/cage_construction_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/five_plus_ten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_eight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m12l24.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m24l48.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m3l6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l4_square.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m6l12_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m8l6_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/one_plus_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/six_plus_eight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/six_plus_nine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/three_plus_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/two_plus_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/two_plus_three.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/two_plus_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/vertices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.980313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/cof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/hexagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/kagome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_kagome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_square.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/square.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/edge_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.980313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/host_guest/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/host_guest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/host_guest/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/host_guest/vertices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.980313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/macrocycle/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/macrocycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/macrocycle/vertices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26537 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/octahedral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/square_planar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/vertices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24349 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/linear/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/linear/vertices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/rotaxane/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/rotaxane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/rotaxane/vertices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/edge_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/topology_graphs/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/utilities/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/updaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/updaters/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/updaters/mdl_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/updaters/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/updaters/turbomole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/updaters/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.984313 stk-2023.7.6.0/src/stk/_internal/utilities/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/writers/mdl_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/writers/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/utilities/writers/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/src/stk/_internal/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/writers/mdl_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/writers/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/writers/turbomole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/_internal/writers/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 10:12:00.000000 stk-2023.7.6.0/src/stk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/cage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/cof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/host_guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/macrocycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/metal_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/polymer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-06 10:11:05.000000 stk-2023.7.6.0/src/stk/rotaxane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.952313 stk-2023.7.6.0/src/stk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-06 10:12:00.000000 stk-2023.7.6.0/src/stk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    68946 2023-07-06 10:12:00.000000 stk-2023.7.6.0/src/stk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:12:00.000000 stk-2023.7.6.0/src/stk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 10:12:00.000000 stk-2023.7.6.0/src/stk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 10:12:00.000000 stk-2023.7.6.0/src/stk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/constructed_molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/constructed_molecule/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/fixtures/constructed_molecule_mongo_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/fixtures/constructed_molecule_mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/get_all/test_get_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/constructed_molecule/mongo_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/mongo_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/mongo_db/test_constructed_molecule_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/mongo_db/test_constructed_molecule_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/mongo_db/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/constructed_molecule/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.988313 stk-2023.7.6.0/tests/databases/molecule/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/fixtures/molecule_mongo_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/databases/molecule/get_all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/get_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/get_all/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/get_all/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/databases/molecule/get_all/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/get_all/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/get_all/fixtures/molecule_mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/get_all/test_get_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/databases/molecule/mongo_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/mongo_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/mongo_db/test_molecule_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/mongo_db/test_molecule_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/mongo_db/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/molecule/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/databases/value/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/databases/value/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/fixtures/mongo_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/databases/value/mongo_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/mongo_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/mongo_db/test_value_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/mongo_db/test_value_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/mongo_db/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/databases/value/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/drop_test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/ea/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/ea/crossover/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/ea/crossover/crossers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/crossers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/crossers/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/crossers/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/ea/crossover/crossers/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/crossers/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/crossers/fixtures/genetic_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/crossers/fixtures/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/crossover/crossers/test_cross.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/ea/fitness_calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.992313 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/fixtures/fitness_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/fixtures/property_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/fixtures/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_caching/test_caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/fixtures/fitness_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/fixtures/property_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_calculator/test_get_fitness_value/test_get_fitness_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/fitness_normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/divide_by_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/replace_fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/shift_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/fixtures/sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/fitness_normalizer/test_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/mutation/mutator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/mutation/mutator/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/fixtures/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/fixtures/random_building_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/fixtures/random_topology_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/fixtures/similar_building_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/mutation/mutator/test_mutate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:00.996313 stk-2023.7.6.0/tests/ea/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/plotters/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/progress/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/progress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/progress/test_progress_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/plotters/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/selection/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/selection/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/plotters/selection/test_selection_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/selection/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/selection/selector/select/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/above_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/best.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/filter_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/filter_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/remove_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/remove_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/fixtures/worst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_1/test_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/fixtures/roulette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/fixtures/stochastic_universal_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/fixtures/tournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/ea/selection/selector/select/select_2/test_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.000313 stk-2023.7.6.0/tests/molecular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.004313 stk-2023.7.6.0/tests/molecular/atoms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.004313 stk-2023.7.6.0/tests/molecular/atoms/atom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/test_get_atomic_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/test_get_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/test_with_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.004313 stk-2023.7.6.0/tests/molecular/atoms/atom_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom_info/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom_info/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom_info/test_get_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom_info/test_get_building_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/atoms/atom_info/test_get_building_block_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.004313 stk-2023.7.6.0/tests/molecular/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.004313 stk-2023.7.6.0/tests/molecular/bonds/bond/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/test_get_atom1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/test_get_atom2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/test_get_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/test_get_periodicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/test_is_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.004313 stk-2023.7.6.0/tests/molecular/bonds/bond/with_atoms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/with_atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/with_atoms/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/with_atoms/test_with_atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.008313 stk-2023.7.6.0/tests/molecular/bonds/bond/with_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/with_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/with_ids/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond/with_ids/test_with_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.008313 stk-2023.7.6.0/tests/molecular/bonds/bond_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond_info/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond_info/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond_info/test_get_bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond_info/test_get_building_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/bonds/bond_info/test_get_building_block_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.008313 stk-2023.7.6.0/tests/molecular/functional_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.008313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/aldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/alkene.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/alkyne.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/amide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/boronic_acid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/bromo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/carboxylic_acid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/dibromo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/difluoro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/diol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/fluoro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/iodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/primary_amino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/ring_amine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/secondary_amino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/single_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/thioacid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/fixtures/thiol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/test_get_atom_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/test_get_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/test_get_core_atom_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/test_get_placer_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_atoms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_atoms/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_atoms/test_with_atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_ids/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/functional_group/with_ids/test_with_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/test_get_bonder_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/test_get_bonders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/test_get_deleter_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/test_get_deleters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/test_get_num_bonders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_atoms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_atoms/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_atoms/test_with_atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_ids/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/generic_functional_group/with_ids/test_with_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.012313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/case_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.016313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/functional_group_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/functional_group_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/functional_group_factory/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/functional_group_factory/test_get_functional_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.016313 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/generic_functional_group_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/generic_functional_group_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14146 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/generic_functional_group_factory/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/generic_functional_group_factory/test_get_functional_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/functional_groups/functional_group_factory/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.016313 stk-2023.7.6.0/tests/molecular/key_makers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/key_makers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/key_makers/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/key_makers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/key_makers/test_get_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/key_makers/test_get_key_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.016313 stk-2023.7.6.0/tests/molecular/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.016313 stk-2023.7.6.0/tests/molecular/molecules/building_block/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.016313 stk-2023.7.6.0/tests/molecular/molecules/building_block/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/fixtures/default_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/fixtures/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/fixtures/init_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/fixtures/init_from_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/fixtures/init_from_rdkit_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/test_get_core_atom_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/test_get_functional_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/test_get_num_functional_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/test_get_num_placers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/test_get_placer_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/building_block/test_with_functional_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.020313 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.020313 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/fixtures/cof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/fixtures/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/test_get_atom_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/test_get_bond_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/test_get_building_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/constructed_molecule/test_get_num_building_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.020313 stk-2023.7.6.0/tests/molecular/molecules/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.020313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/building_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.020313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/cage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.020313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m12l24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m24l48.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m2l4_lantern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m3l3_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m3l6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m4l4_square.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m4l4_tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m4l6_tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m4l6_tetrahedron_spacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m4l8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m6l12_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m6l2l3_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/metal_topologies/m8l6_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.024313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_four/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_four/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_four/six_plus_eight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.024313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_three/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_three/four_plus_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_three/one_plus_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/three_plus_three/two_plus_two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.024313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_five/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_five/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_five/twelve_plus_thirty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.024313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/eight_plus_sixteen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/five_plus_ten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/four_plus_eight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/six_plus_twelve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/ten_plus_twenty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/three_plus_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_four/two_plus_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.024313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/eight_plus_twelve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/four_plus_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/four_plus_six_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/six_plus_nine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/twenty_plus_thirty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cage/two_plus_three/two_plus_three.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/cof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/hexagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/kagome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/linkerless_honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/periodic_hexagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/periodic_honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/periodic_kagome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/periodic_linkerless_honeycomb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/periodic_square.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/cof/square.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/host_guest/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/host_guest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/host_guest/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/host_guest/host_guest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/macrocycle/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/macrocycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/macrocycle/macrocycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/metal_complex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/octahedral/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/octahedral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/octahedral/octahedral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/octahedral/octahedral_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/octahedral/octahedral_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/paddlewheel/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/paddlewheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/paddlewheel/paddlewheel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/porphyrin/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/porphyrin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/porphyrin/porphyrin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/square_planar/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/square_planar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/square_planar/bidentate_square_planar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/square_planar/cis_protected_square_planar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/metal_complex/square_planar/square_planar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.028313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/polymer/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/polymer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/polymer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/polymer/polymer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.040313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/building_block0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/building_block1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/building_block2.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/building_block3.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/building_block4.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/building_block5.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/building_block6.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_eight_plus_sixteen0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_eight_plus_twelve0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_eight_plus_twelve1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_five_plus_ten0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_four_plus_eight0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_four_plus_four0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_four_plus_six0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_four_plus_six_20.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_one_plus_one0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_six_plus_eight0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_six_plus_nine0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_six_plus_twelve0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_ten_plus_twenty0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_three_plus_six0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_twelve_plus_thirty0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_twenty_plus_thirty0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_two_plus_four0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_two_plus_three0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cage_two_plus_two0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_hexagonal0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    37712 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_hexagonal1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_hexagonal2.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_hexagonal3.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_honeycomb0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_honeycomb1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_honeycomb2.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_kagome0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_linkerless_honeycomb0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_hexagonal0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_hexagonal1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_honeycomb0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_honeycomb1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_kagome0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_kagome1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_linkerless_honeycomb0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_linkerless_honeycomb1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_square0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_periodic_square1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/cof_square0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/host_guest_complex0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/host_guest_complex1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/host_guest_complex2.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/host_guest_complex3.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/macrocycle_macrocycle0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/macrocycle_macrocycle1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m12l240.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m24l480.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m2l4_lantern0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m3l3_triangle0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m3l3_triangle1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m3l3_triangle2.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m3l3_triangle3.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m3l60.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m4l4_square0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m4l4_square1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m4l4_tetrahedron0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m4l6_tetrahedron0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m4l6_tetrahedron_spacer0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m4l80.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m6l12_cube0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m6l2l3_prism0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_cage_m8l6_cube0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_bidentate_square_planar0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_bidentate_square_planar1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_cis_protected_square_planar0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_cis_protected_square_planar1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_octahedral0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_octahedral1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_octahedral_delta0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_octahedral_delta1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_octahedral_lambda0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_octahedral_lambda1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_paddlewheel0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_paddlewheel1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_porphyrin0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_porphyrin1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_square_planar0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/metal_complex_square_planar1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/polymer_linear0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/polymer_linear1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/polymer_linear2.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/polymer_linear3.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/position_matrices/rotaxane_nrotaxane0.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.040313 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/rotaxane/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/rotaxane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/rotaxane/nrotaxane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/fixtures/rotaxane/rotaxane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.040313 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_1/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_1/test_get_atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_atoms/get_atoms_2/test_get_atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_bonds/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_bonds/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_bonds/test_get_bonds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_canonical_atom_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_canonical_atom_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_canonical_atom_ids/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_canonical_atom_ids/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_canonical_atom_ids/test_get_canonical_atom_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_centroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_centroid/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_centroid/test_get_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_centroid/test_get_centroid_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_direction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_direction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_direction/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_direction/test_get_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_direction/test_get_direction_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_maximum_diameter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_maximum_diameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_maximum_diameter/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_maximum_diameter/test_get_maximum_diameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_maximum_diameter/test_get_maximum_diameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_maximum_diameter/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_1/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_1/test_get_num_atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_atoms/get_num_atoms_2/test_get_num_atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.044314 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_1/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_1/test_get_num_bonds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_num_bonds/get_num_bonds_2/test_get_num_bonds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_plane_normal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_plane_normal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_plane_normal/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_plane_normal/test_get_plane_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_plane_normal/test_get_plane_normal_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/get_plane_normal/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/test_dump_molecular_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/test_get_atomic_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/test_get_position_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/test_to_rdkit_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/test_with_position_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_canonical_atom_ordering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_canonical_atom_ordering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_canonical_atom_ordering/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_canonical_atom_ordering/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_canonical_atom_ordering/test_with_canonical_atom_ordering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_centroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_centroid/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_centroid/test_with_centroid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_displacement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_displacement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_displacement/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_displacement/test_with_displacement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_about_axis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_about_axis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_about_axis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_about_axis/test_with_rotation_about_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.048313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_between_vectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_between_vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_between_vectors/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_between_vectors/test_with_rotation_between_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.052313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_to_minimize_angle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_to_minimize_angle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_to_minimize_angle/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_rotation_to_minimize_angle/test_with_rotation_to_minimize_angle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.052313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.052313 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_1/test_with_structure_from_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.056314 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.060314 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN.coord
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN.mae
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN_with_cell.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN_with_cell1.coord
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file/NCCN_with_cell2.coord
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/with_structure_from_file/with_structure_from_file_2/test_with_structure_from_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.060314 stk-2023.7.6.0/tests/molecular/molecules/molecule/write/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/write/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/molecule/write/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.060314 stk-2023.7.6.0/tests/molecular/molecules/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/utilities/building_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/utilities/constructed_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/utilities/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/molecules/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.064314 stk-2023.7.6.0/tests/molecular/periodic_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_get_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_get_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_get_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_get_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_get_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_get_cell_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/periodic_info/test_get_gamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.064314 stk-2023.7.6.0/tests/molecular/reactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.064314 stk-2023.7.6.0/tests/molecular/reactions/reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.068314 stk-2023.7.6.0/tests/molecular/reactions/reaction/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/fixtures/dative_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/fixtures/one_one_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/fixtures/one_two_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/fixtures/two_two_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/test_get_deleted_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/test_get_deleted_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/test_get_new_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/test_get_new_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.068314 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.068314 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/fixtures/dative_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/fixtures/one_one_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/fixtures/one_two_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/fixtures/two_two_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/fixtures/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/reactions/reaction_factory/test_get_reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.072314 stk-2023.7.6.0/tests/molecular/topology_graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.072314 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/test_with_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.072314 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_atom_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_bond_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_building_block_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_building_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_edge_functional_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_position_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_vertex_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/check_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/construction_state/with_placement_results/test_with_placement_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.072314 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/test_get_periodicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/test_get_vertex1_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/test_get_vertex2_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/test_get_vertex_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/test_is_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.076314 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/with_scale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/with_scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/with_scale/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/with_scale/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/edge/with_scale/test_with_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.076314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/_test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/_test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/_test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/_test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/_test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/_test_with_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/case_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.076314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.076314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cage/test_with_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.076314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.080314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/fixtures/cof1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/fixtures/cof2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/fixtures/cof3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/cof/test_with_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.080314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/host_guest/test_with_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.080314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/linear/test_with_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.080314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/macrocycle/test_with_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/metal_complex/test_with_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/test_get_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/test_get_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/test_get_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/test_with_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/cases/rotaxane/test_with_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/_test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/case_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/fixtures/angled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/fixtures/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/fixtures/nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/fixtures/unaligning.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cage/test_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/fixtures/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/fixtures/nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/fixtures/unaligning.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/cof/test_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.084314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.088314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/fixtures/guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/fixtures/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/host_guest/test_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.088314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.088314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/center.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/head_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/head_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/head_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/tail_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/tail_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/tail_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/fixtures/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/linear/test_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.088314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.088314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/fixtures/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/fixtures/no_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/fixtures/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/macrocycle/test_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.088314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.088314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/fixtures/bidentate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/fixtures/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/fixtures/monodentate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/metal_complex/test_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/fixtures/axle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/fixtures/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/placement/cases/rotaxane/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/topology_graphs/vertex/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/molecular/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/molecular/writers/mdl_mol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/mdl_mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/mdl_mol/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/mdl_mol/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/mdl_mol/test_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/mdl_mol/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/molecular/writers/pdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/pdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/pdb/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/pdb/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/pdb/test_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/pdb/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/molecular/writers/turbomole/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/turbomole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/turbomole/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/turbomole/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/turbomole/test_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/turbomole/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/molecular/writers/xyz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/xyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/xyz/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/xyz/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/xyz/test_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/molecular/writers/xyz/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/mongo-config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/serialization/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.092314 stk-2023.7.6.0/tests/serialization/json/from_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/from_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/from_json/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/from_json/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/from_json/test_from_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.096314 stk-2023.7.6.0/tests/serialization/json/to_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/to_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/to_json/case_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/to_json/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/serialization/json/to_json/test_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.096314 stk-2023.7.6.0/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:12:01.096314 stk-2023.7.6.0/tests/utilities/molecular/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/utilities/molecular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/utilities/molecular/constructed_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/utilities/molecular/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-06 10:11:05.000000 stk-2023.7.6.0/tests/utilities/molecular/utilities.py
```

### Comparing `stk-2023.7.5.3/LICENSE` & `stk-2023.7.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/PKG-INFO` & `stk-2023.7.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stk
-Version: 2023.7.5.3
+Version: 2023.7.6.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>, Andrew Tarzia <andrew.tarzia@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/stk
 Project-URL: documentation, https://stk.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `stk-2023.7.5.3/README.rst` & `stk-2023.7.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/pyproject.toml` & `stk-2023.7.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/__init__.py` & `stk-2023.7.6.0/src/stk/__init__.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/atom.py` & `stk-2023.7.6.0/src/stk/_internal/atom.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/atom_info.py` & `stk-2023.7.6.0/src/stk/_internal/atom_info.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/bond.py` & `stk-2023.7.6.0/src/stk/_internal/bond.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/bond_info.py` & `stk-2023.7.6.0/src/stk/_internal/bond_info.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/building_block.py` & `stk-2023.7.6.0/src/stk/_internal/building_block.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/constructed_molecule.py` & `stk-2023.7.6.0/src/stk/_internal/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_result/construction_result.py` & `stk-2023.7.6.0/src/stk/_internal/construction_result/construction_result.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_result/periodic.py` & `stk-2023.7.6.0/src/stk/_internal/construction_result/periodic.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/construction_state.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/construction_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/graph_state.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/graph_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/deletions_summary.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/deletions_summary.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/molecule_state.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/molecule_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/atom_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/bond_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/placements_summary/placements_summary.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/atom_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/bond_batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py` & `stk-2023.7.6.0/src/stk/_internal/construction_state/molecule_state/reactions_summary/reactions_summary.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/databases/constructed_molecule.py` & `stk-2023.7.6.0/src/stk/_internal/databases/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/databases/molecule.py` & `stk-2023.7.6.0/src/stk/_internal/databases/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/constructed_molecule.py` & `stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/molecule.py` & `stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/utilities.py` & `stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/databases/mongo_db/value.py` & `stk-2023.7.6.0/src/stk/_internal/databases/mongo_db/value.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/databases/value.py` & `stk-2023.7.6.0/src/stk/_internal/databases/value.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/crossover/genetic_recombination.py` & `stk-2023.7.6.0/src/stk/_internal/ea/crossover/genetic_recombination.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/crossover/molecule_crosser.py` & `stk-2023.7.6.0/src/stk/_internal/ea/crossover/molecule_crosser.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/crossover/random.py` & `stk-2023.7.6.0/src/stk/_internal/ea/crossover/random.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/crossover/record.py` & `stk-2023.7.6.0/src/stk/_internal/ea/crossover/record.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py` & `stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/evolutionary_algorithm.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py` & `stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/implementation.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py` & `stk-2023.7.6.0/src/stk/_internal/ea/evolutionary_algorithm/implementations/parallel.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/fitness_calculator.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/fitness_function.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/fitness_function.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_calculators/property_vector.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_calculators/property_vector.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/add.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/add.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/divide_by_mean.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/fitness_normalizer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/multiply.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/multiply.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/power.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/power.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/replace_fitness.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/sequence.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/sequence.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/shift_up.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/shift_up.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/fitness_normalizers/sum.py` & `stk-2023.7.6.0/src/stk/_internal/ea/fitness_normalizers/sum.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/generation.py` & `stk-2023.7.6.0/src/stk/_internal/ea/generation.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/molecule_records/molecule.py` & `stk-2023.7.6.0/src/stk/_internal/ea/molecule_records/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/mutation/mutator.py` & `stk-2023.7.6.0/src/stk/_internal/ea/mutation/mutator.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/mutation/random.py` & `stk-2023.7.6.0/src/stk/_internal/ea/mutation/random.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/mutation/random_building_block.py` & `stk-2023.7.6.0/src/stk/_internal/ea/mutation/random_building_block.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/mutation/random_topology_graph.py` & `stk-2023.7.6.0/src/stk/_internal/ea/mutation/random_topology_graph.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/mutation/record.py` & `stk-2023.7.6.0/src/stk/_internal/ea/mutation/record.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/mutation/similar_building_block.py` & `stk-2023.7.6.0/src/stk/_internal/ea/mutation/similar_building_block.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/plotters/progress.py` & `stk-2023.7.6.0/src/stk/_internal/ea/plotters/progress.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/plotters/selection.py` & `stk-2023.7.6.0/src/stk/_internal/ea/plotters/selection.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/batch.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/batch.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/above_average.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/above_average.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/best.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/best.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/filter_batches.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/filter_batches.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/filter_molecules.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/remove_batches.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/remove_batches.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/remove_molecules.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/remove_molecules.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/roulette.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/roulette.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/selector.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/stochastic_universal_sampling.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/tournament.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/tournament.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/utilities/yielded_batches.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/ea/selection/selectors/worst.py` & `stk-2023.7.6.0/src/stk/_internal/ea/selection/selectors/worst.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/elements.py` & `stk-2023.7.6.0/src/stk/_internal/elements.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/alcohol_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/alcohol_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/aldehyde_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/aldehyde_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/amide_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/amide_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/boronic_acid_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/boronic_acid_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/bromo_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/bromo_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/carboxylic_acid_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/dibromo_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/dibromo_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/difluoro_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/difluoro_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/diol_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/diol_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/fluoro_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/fluoro_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/functional_group_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/functional_group_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/iodo_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/iodo_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/primary_amino_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/primary_amino_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/ring_amine_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/ring_amine_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/secondary_amino_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/secondary_amino_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/smarts.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/smarts.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/terminal_alkene_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/terminal_alkyne_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/thioacid_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/thioacid_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/thiol_factory.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/thiol_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_group_factories/utilities.py` & `stk-2023.7.6.0/src/stk/_internal/functional_group_factories/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/alcohol.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/alcohol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/aldehyde.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/aldehyde.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/alkene.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/alkene.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/alkyne.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/alkyne.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/amide.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/amide.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/boronic_acid.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/boronic_acid.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/bromo.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/bromo.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/carboxylic_acid.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/carboxylic_acid.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/dibromo.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/dibromo.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/difluoro.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/difluoro.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/diol.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/diol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/fluoro.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/fluoro.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/functional_group.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/functional_group.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/generic_functional_group.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/generic_functional_group.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/iodo.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/iodo.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/primary_amino.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/primary_amino.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/ring_amine.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/ring_amine.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/secondary_amino.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/secondary_amino.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/single_atom.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/single_atom.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/thioacid.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/thioacid.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/functional_groups/thiol.py` & `stk-2023.7.6.0/src/stk/_internal/functional_groups/thiol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/json_serde/constructed_molecule.py` & `stk-2023.7.6.0/src/stk/_internal/json_serde/constructed_molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/json_serde/molecule.py` & `stk-2023.7.6.0/src/stk/_internal/json_serde/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/json_serde/utilities.py` & `stk-2023.7.6.0/src/stk/_internal/json_serde/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/key_makers/inchi.py` & `stk-2023.7.6.0/src/stk/_internal/key_makers/inchi.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/key_makers/inchi_key.py` & `stk-2023.7.6.0/src/stk/_internal/key_makers/inchi_key.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/key_makers/molecule.py` & `stk-2023.7.6.0/src/stk/_internal/key_makers/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/key_makers/smiles.py` & `stk-2023.7.6.0/src/stk/_internal/key_makers/smiles.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/key_makers/utilities.py` & `stk-2023.7.6.0/src/stk/_internal/key_makers/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/molecule.py` & `stk-2023.7.6.0/src/stk/_internal/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/optimizers/collapser.py` & `stk-2023.7.6.0/src/stk/_internal/optimizers/collapser.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/optimizers/mchammer.py` & `stk-2023.7.6.0/src/stk/_internal/optimizers/mchammer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/optimizers/optimizer.py` & `stk-2023.7.6.0/src/stk/_internal/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/optimizers/periodic_collapser.py` & `stk-2023.7.6.0/src/stk/_internal/optimizers/periodic_collapser.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/optimizers/spinner.py` & `stk-2023.7.6.0/src/stk/_internal/optimizers/spinner.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/optimizers/utilities.py` & `stk-2023.7.6.0/src/stk/_internal/optimizers/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/periodic_info.py` & `stk-2023.7.6.0/src/stk/_internal/periodic_info.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reaction_factories/dative_reaction_factory.py` & `stk-2023.7.6.0/src/stk/_internal/reaction_factories/dative_reaction_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reaction_factories/generic_reaction_factory.py` & `stk-2023.7.6.0/src/stk/_internal/reaction_factories/generic_reaction_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reaction_factories/reaction_factory.py` & `stk-2023.7.6.0/src/stk/_internal/reaction_factories/reaction_factory.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/dative_reaction/dative_reaction.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/dative_reaction/dative_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/one_one_reaction.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/one_one_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/one_two_reaction.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/one_two_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/reaction/new_atom.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/reaction/new_atom.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/reaction/reaction.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/reaction/reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/reaction/reaction_result.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/reaction/reaction_result.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/ring_amine_reaction.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/ring_amine_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/reactions/two_two_reaction.py` & `stk-2023.7.6.0/src/stk/_internal/reactions/two_two_reaction.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/cage.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/cage.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/cage_construction_state.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/cage_construction_state.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/eight_plus_sixteen.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/eight_plus_twelve.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/five_plus_ten.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/five_plus_ten.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_eight.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_eight.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_four.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_four.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_six.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_six.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/four_plus_six_2.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m12l24.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m12l24.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m24l48.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m24l48.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m2l4_lantern.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m3l3_triangle.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m3l6.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m3l6.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l4_square.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l4_square.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l4_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l6_tetrahedron_spacer.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m4l8.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m4l8.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m6l12_cube.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m6l12_cube.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m6l2l3_prism.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/m8l6_cube.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/m8l6_cube.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/one_plus_one.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/one_plus_one.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/six_plus_eight.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/six_plus_eight.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/six_plus_nine.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/six_plus_nine.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/six_plus_twelve.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/ten_plus_twenty.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/three_plus_six.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/three_plus_six.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/twelve_plus_thirty.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/twenty_plus_thirty.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/two_plus_four.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/two_plus_four.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/two_plus_three.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/two_plus_three.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/two_plus_two.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/two_plus_two.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cage/vertices.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cage/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/cof.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/cof.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/edge.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/edge.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/hexagonal.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/hexagonal.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/honeycomb.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/kagome.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/kagome.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/linkerless_honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_hexagonal.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_kagome.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_kagome.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_linkerless_honeycomb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/periodic_square.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/periodic_square.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/square.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/square.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/cof/vertices.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/cof/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/edge.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/edge.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/edge_group.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/edge_group.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/host_guest/complex.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/host_guest/complex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/host_guest/vertices.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/host_guest/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/macrocycle/macrocycle.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/macrocycle/vertices.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/macrocycle/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/bidentate_square_planar.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/cis_protected_square_planar.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/metal_complex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/octahedral.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/octahedral.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_delta.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/octahedral_lambda.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/paddlewheel.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/porphyrin.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/square_planar.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/square_planar.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/metal_complex/vertices.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/metal_complex/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/linear/linear.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/linear/linear.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/polymer/linear/vertices.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/polymer/linear/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/rotaxane/nrotaxane.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/rotaxane/vertices.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/rotaxane/vertices.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/parallel.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/parallel.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/serial.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/serial.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/topology_graph.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/topology_graph/utilities.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/topology_graph/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/edge_sorter.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/edge_sorter.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/functional_group_sorter.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/utilities/sorter.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/utilities/sorter.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/topology_graphs/vertex.py` & `stk-2023.7.6.0/src/stk/_internal/topology_graphs/vertex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/molecule.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/molecule.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/updaters/mae.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/updaters/mae.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/updaters/mdl_mol.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/updaters/mdl_mol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/updaters/pdb.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/updaters/pdb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/updaters/turbomole.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/updaters/turbomole.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/updaters/xyz.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/updaters/xyz.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/utilities.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/writers/mdl_mol.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/writers/mdl_mol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/writers/pdb.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/writers/pdb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/utilities/writers/xyz.py` & `stk-2023.7.6.0/src/stk/_internal/utilities/writers/xyz.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/writers/mdl_mol.py` & `stk-2023.7.6.0/src/stk/_internal/writers/mdl_mol.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/writers/pdb.py` & `stk-2023.7.6.0/src/stk/_internal/writers/pdb.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/writers/turbomole.py` & `stk-2023.7.6.0/src/stk/_internal/writers/turbomole.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/_internal/writers/xyz.py` & `stk-2023.7.6.0/src/stk/_internal/writers/xyz.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/cage.py` & `stk-2023.7.6.0/src/stk/cage.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/cof.py` & `stk-2023.7.6.0/src/stk/cof.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk/metal_complex.py` & `stk-2023.7.6.0/src/stk/metal_complex.py`

 * *Files identical despite different names*

### Comparing `stk-2023.7.5.3/src/stk.egg-info/PKG-INFO` & `stk-2023.7.6.0/src/stk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stk
-Version: 2023.7.5.3
+Version: 2023.7.6.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>, Andrew Tarzia <andrew.tarzia@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/stk
 Project-URL: documentation, https://stk.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
```

