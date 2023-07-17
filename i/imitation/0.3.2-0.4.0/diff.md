# Comparing `tmp/imitation-0.3.2.tar.gz` & `tmp/imitation-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imitation-0.3.2.tar", last modified: Sun Nov 27 19:48:55 2022, max compression
+gzip compressed data, was "imitation-0.4.0.tar", last modified: Mon Jul 17 23:06:30 2023, max compression
```

## Comparing `imitation-0.3.2.tar` & `imitation-0.4.0.tar`

### file list

```diff
@@ -1,262 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.742641 imitation-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.698640 imitation-0.3.2/.circleci/
--rw-r--r--   0 runner    (1001) docker     (122)    12313 2022-11-27 19:48:43.000000 imitation-0.3.2/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)      862 2022-11-27 19:48:43.000000 imitation-0.3.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-11-27 19:48:43.000000 imitation-0.3.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)     2190 2022-11-27 19:48:43.000000 imitation-0.3.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-27 19:48:43.000000 imitation-0.3.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.698640 imitation-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.698640 imitation-0.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2022-11-27 19:48:43.000000 imitation-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      355 2022-11-27 19:48:43.000000 imitation-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-11-27 19:48:43.000000 imitation-0.3.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.698640 imitation-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1986 2022-11-27 19:48:43.000000 imitation-0.3.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2190 2022-11-27 19:48:43.000000 imitation-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2022-11-27 19:48:43.000000 imitation-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2022-11-27 19:48:43.000000 imitation-0.3.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2022-11-27 19:48:43.000000 imitation-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     8445 2022-11-27 19:48:55.742641 imitation-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7541 2022-11-27 19:48:43.000000 imitation-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.702641 imitation-0.3.2/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (122)      897 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_airl_seals_ant_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_airl_seals_half_cheetah_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_airl_seals_hopper_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_airl_seals_swimmer_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_airl_seals_walker_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)      972 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_bc_seals_ant_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)      977 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_bc_seals_half_cheetah_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)      977 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_bc_seals_hopper_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)      976 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_bc_seals_swimmer_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)      979 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_bc_seals_walker_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_dagger_seals_ant_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_dagger_seals_half_cheetah_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_dagger_seals_hopper_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_dagger_seals_swimmer_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_dagger_seals_walker_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1507 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_gail_seals_ant_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_gail_seals_half_cheetah_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_gail_seals_hopper_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_gail_seals_swimmer_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/example_gail_seals_walker_best_hp_eval.json
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2022-11-27 19:48:43.000000 imitation-0.3.2/benchmarking/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.706641 imitation-0.3.2/ci/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1173 2022-11-27 19:48:43.000000 imitation-0.3.2/ci/Xdummy-entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2022-11-27 19:48:43.000000 imitation-0.3.2/ci/build_and_activate_venv.ps1
--rwxr-xr-x   0 runner    (1001) docker     (122)      648 2022-11-27 19:48:43.000000 imitation-0.3.2/ci/build_and_activate_venv.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     2866 2022-11-27 19:48:43.000000 imitation-0.3.2/ci/check_typeignore.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5196 2022-11-27 19:48:43.000000 imitation-0.3.2/ci/clean_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6518 2022-11-27 19:48:43.000000 imitation-0.3.2/ci/xorg.conf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.706641 imitation-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      737 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.690641 imitation-0.3.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.706641 imitation-0.3.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.690641 imitation-0.3.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.706641 imitation-0.3.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (122)      106 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (122)      553 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.710641 imitation-0.3.2/docs/algorithms/
--rw-r--r--   0 runner    (1001) docker     (122)     2732 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/algorithms/airl.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/algorithms/bc.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2477 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/algorithms/dagger.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1655 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/algorithms/density.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2569 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/algorithms/gail.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/algorithms/mce_irl.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3579 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/algorithms/preference_comparisons.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3915 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.710641 imitation-0.3.2/docs/development/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.710641 imitation-0.3.2/docs/development/contributing/
--rw-r--r--   0 runner    (1001) docker     (122)     2848 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/development/contributing/code-of-conduct.rst
--rw-r--r--   0 runner    (1001) docker     (122)      654 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/development/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6237 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/development/contributing/ways-to-contribute.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/development/developer.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/development/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)      254 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/development/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.710641 imitation-0.3.2/docs/experts/
--rw-r--r--   0 runner    (1001) docker     (122)     4851 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/experts/loading-experts.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.710641 imitation-0.3.2/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/getting-started/first-steps.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/getting-started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5663 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/getting-started/variable-horizon.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/getting-started/what-is-imitation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      795 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.714640 imitation-0.3.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (122)     5890 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/1_train_bc.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3751 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/2_train_dagger.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5996 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/3_train_gail.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5497 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/4_train_airl.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5968 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/5_train_preference_comparisons.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9001 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/5a_train_preference_comparisons_with_cnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8777 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/6_train_mce.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5601 2022-11-27 19:48:43.000000 imitation-0.3.2/docs/tutorials/7_train_density.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.714640 imitation-0.3.2/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2022-11-27 19:48:43.000000 imitation-0.3.2/examples/quickstart.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      796 2022-11-27 19:48:43.000000 imitation-0.3.2/examples/quickstart.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.718641 imitation-0.3.2/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     1865 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/bc_benchmark.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     2639 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/benchmark_and_table.sh
--rw-r--r--   0 runner    (1001) docker     (122)      631 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/common.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/convert_traj.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2871 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/dagger_benchmark.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     3562 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/imit_benchmark.sh
--rw-r--r--   0 runner    (1001) docker     (122)      765 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/imit_benchmark_config.csv
--rw-r--r--   0 runner    (1001) docker     (122)       53 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/imit_table_cheetahs.csv
--rw-r--r--   0 runner    (1001) docker     (122)       71 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/imit_table_mvp_seals_config.csv
--rwxr-xr-x   0 runner    (1001) docker     (122)     1844 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/rollouts_from_policies.sh
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/rollouts_from_policies_config.csv
--rwxr-xr-x   0 runner    (1001) docker     (122)     2821 2022-11-27 19:48:43.000000 imitation-0.3.2/experiments/transfer_learn_benchmark.sh
--rw-r--r--   0 runner    (1001) docker     (122)       37 2022-11-27 19:48:43.000000 imitation-0.3.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)      570 2022-11-27 19:48:43.000000 imitation-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      172 2022-11-27 19:48:43.000000 imitation-0.3.2/readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.718641 imitation-0.3.2/runners/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1308 2022-11-27 19:48:43.000000 imitation-0.3.2/runners/build_push_image.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1297 2022-11-27 19:48:43.000000 imitation-0.3.2/runners/launch_docker-dev.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1291 2022-11-27 19:48:55.742641 imitation-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     9806 2022-11-27 19:48:43.000000 imitation-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.694640 imitation-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.718641 imitation-0.3.2/src/imitation/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.722641 imitation-0.3.2/src/imitation/algorithms/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.722641 imitation-0.3.2/src/imitation/algorithms/adversarial/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/adversarial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5092 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/adversarial/airl.py
--rw-r--r--   0 runner    (1001) docker     (122)    27136 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/adversarial/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     6086 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/adversarial/gail.py
--rw-r--r--   0 runner    (1001) docker     (122)    11372 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    18649 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/bc.py
--rw-r--r--   0 runner    (1001) docker     (122)    26475 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/dagger.py
--rw-r--r--   0 runner    (1001) docker     (122)    17005 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/density.py
--rw-r--r--   0 runner    (1001) docker     (122)    21103 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/mce_irl.py
--rw-r--r--   0 runner    (1001) docker     (122)    75364 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/algorithms/preference_comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.722641 imitation-0.3.2/src/imitation/data/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14491 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/data/buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)    26242 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/data/rollout.py
--rw-r--r--   0 runner    (1001) docker     (122)    19124 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/data/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     7693 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/data/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.722641 imitation-0.3.2/src/imitation/policies/
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4442 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/policies/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2628 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/policies/exploration_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     3530 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/policies/replay_buffer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     7594 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/policies/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.722641 imitation-0.3.2/src/imitation/regularization/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11139 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/regularization/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5483 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/regularization/updaters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.726641 imitation-0.3.2/src/imitation/rewards/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/rewards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/rewards/reward_function.py
--rw-r--r--   0 runner    (1001) docker     (122)    38132 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/rewards/reward_nets.py
--rw-r--r--   0 runner    (1001) docker     (122)     4580 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/rewards/reward_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     8287 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/rewards/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.726641 imitation-0.3.2/src/imitation/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      212 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11059 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.730641 imitation-0.3.2/src/imitation/scripts/common/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5721 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3254 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/demonstrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/expert.py
--rw-r--r--   0 runner    (1001) docker     (122)     5474 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/reward.py
--rw-r--r--   0 runner    (1001) docker     (122)     6970 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/rl.py
--rw-r--r--   0 runner    (1001) docker     (122)     3394 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/train.py
--rw-r--r--   0 runner    (1001) docker     (122)     2165 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/common/wb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.730641 imitation-0.3.2/src/imitation/scripts/config/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/analyze.py
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/eval_policy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     5168 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/train_adversarial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/train_imitation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/train_preference_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (122)     3639 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/config/train_rl.py
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/convert_trajs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4909 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/eval_policy.py
--rw-r--r--   0 runner    (1001) docker     (122)     9508 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     7167 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/train_adversarial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6509 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/train_imitation.py
--rw-r--r--   0 runner    (1001) docker     (122)    12320 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/train_preference_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (122)     7064 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/scripts/train_rl.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.730641 imitation-0.3.2/src/imitation/testing/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6561 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/testing/expert_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (122)     2395 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/testing/reward_improvement.py
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/testing/reward_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.734641 imitation-0.3.2/src/imitation/util/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15243 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)    12532 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/util/networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3074 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/util/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     4458 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/util/sacred.py
--rw-r--r--   0 runner    (1001) docker     (122)    12025 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/util/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2022-11-27 19:48:43.000000 imitation-0.3.2/src/imitation/util/video_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.718641 imitation-0.3.2/src/imitation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8445 2022-11-27 19:48:55.000000 imitation-0.3.2/src/imitation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7473 2022-11-27 19:48:55.000000 imitation-0.3.2/src/imitation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 19:48:55.000000 imitation-0.3.2/src/imitation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      462 2022-11-27 19:48:55.000000 imitation-0.3.2/src/imitation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2145 2022-11-27 19:48:55.000000 imitation-0.3.2/src/imitation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-11-27 19:48:55.000000 imitation-0.3.2/src/imitation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.734641 imitation-0.3.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.734641 imitation-0.3.2/tests/algorithms/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2437 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    12682 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/test_adversarial.py
--rw-r--r--   0 runner    (1001) docker     (122)     5212 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    11496 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/test_bc.py
--rw-r--r--   0 runner    (1001) docker     (122)    14144 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/test_dagger.py
--rw-r--r--   0 runner    (1001) docker     (122)     5182 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/test_density_baselines.py
--rw-r--r--   0 runner    (1001) docker     (122)    15154 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/test_mce_irl.py
--rw-r--r--   0 runner    (1001) docker     (122)    32416 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/algorithms/test_preference_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1411 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.734641 imitation-0.3.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)     9737 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/data/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)    13009 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/data/test_rollout.py
--rw-r--r--   0 runner    (1001) docker     (122)    15771 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/data/test_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     8199 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/data/test_wrappers.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      353 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/generate_test_data.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/policies/
--rw-r--r--   0 runner    (1001) docker     (122)     4736 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/policies/test_exploration_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     6431 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/policies/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/policies/test_replay_buffer_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/rewards/
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/rewards/test_reward_fn.py
--rw-r--r--   0 runner    (1001) docker     (122)    29677 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/rewards/test_reward_nets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/rewards/test_reward_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/scripts/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/scripts/common/test_rewards.py
--rw-r--r--   0 runner    (1001) docker     (122)    34549 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/scripts/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (122)     3296 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)      684 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)    16754 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/test_regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.694640 imitation-0.3.2/tests/testdata/expert_models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.694640 imitation-0.3.2/tests/testdata/expert_models/cartpole_0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.694640 imitation-0.3.2/tests/testdata/expert_models/cartpole_0/policies/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/testdata/expert_models/cartpole_0/policies/final/
--rw-r--r--   0 runner    (1001) docker     (122)    39774 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/testdata/expert_models/cartpole_0/policies/final/model.zip
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/testdata/expert_models/cartpole_0/rollouts/
--rw-r--r--   0 runner    (1001) docker     (122)   415849 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/testdata/expert_models/cartpole_0/rollouts/final.npz
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.694640 imitation-0.3.2/tests/testdata/expert_models/pendulum_0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.738641 imitation-0.3.2/tests/testdata/expert_models/pendulum_0/rollouts/
--rw-r--r--   0 runner    (1001) docker     (122)   247960 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/testdata/expert_models/pendulum_0/rollouts/final.npz
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/testdata/imit_benchmark_config.csv
--rw-r--r--   0 runner    (1001) docker     (122)    15058 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/testdata/old_format_rollout.pkl
--rw-r--r--   0 runner    (1001) docker     (122)       50 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/testdata/rollouts_from_policies_config.csv
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:48:55.742641 imitation-0.3.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (122)     9862 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/util/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)    10106 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/util/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/util/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     3544 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/util/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3814 2022-11-27 19:48:43.000000 imitation-0.3.2/tests/util/test_wb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.355242 imitation-0.4.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-17 23:06:19.000000 imitation-0.4.0/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-17 23:06:19.000000 imitation-0.4.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 23:06:19.000000 imitation-0.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-17 23:06:19.000000 imitation-0.4.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-17 23:06:19.000000 imitation-0.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.355242 imitation-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.355242 imitation-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 23:06:19.000000 imitation-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 23:06:19.000000 imitation-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 23:06:19.000000 imitation-0.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.355242 imitation-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-17 23:06:19.000000 imitation-0.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-17 23:06:19.000000 imitation-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-17 23:06:19.000000 imitation-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-17 23:06:19.000000 imitation-0.4.0/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-17 23:06:19.000000 imitation-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-17 23:06:19.000000 imitation-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-17 23:06:30.383243 imitation-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-17 23:06:19.000000 imitation-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.359243 imitation-0.4.0/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_airl_seals_ant_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_airl_seals_half_cheetah_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_airl_seals_hopper_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_airl_seals_swimmer_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_airl_seals_walker_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_bc_seals_ant_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_bc_seals_half_cheetah_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_bc_seals_hopper_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_bc_seals_swimmer_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_bc_seals_walker_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_dagger_seals_ant_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_dagger_seals_half_cheetah_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_dagger_seals_hopper_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_dagger_seals_swimmer_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_dagger_seals_walker_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_gail_seals_ant_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_gail_seals_half_cheetah_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_gail_seals_hopper_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_gail_seals_swimmer_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/example_gail_seals_walker_best_hp_eval.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/fast_dagger_seals_cartpole.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-17 23:06:19.000000 imitation-0.4.0/benchmarking/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.359243 imitation-0.4.0/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-17 23:06:19.000000 imitation-0.4.0/ci/Xdummy-entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-17 23:06:19.000000 imitation-0.4.0/ci/build_and_activate_venv.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1182 2023-07-17 23:06:19.000000 imitation-0.4.0/ci/build_and_activate_venv.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2866 2023-07-17 23:06:19.000000 imitation-0.4.0/ci/check_typeignore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5196 2023-07-17 23:06:19.000000 imitation-0.4.0/ci/clean_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-17 23:06:19.000000 imitation-0.4.0/ci/xorg.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.359243 imitation-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.343242 imitation-0.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.359243 imitation-0.4.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.347242 imitation-0.4.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.359243 imitation-0.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.363242 imitation-0.4.0/docs/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/algorithms/airl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/algorithms/bc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/algorithms/dagger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/algorithms/density.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/algorithms/gail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/algorithms/mce_irl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/algorithms/preference_comparisons.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.363242 imitation-0.4.0/docs/development/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.363242 imitation-0.4.0/docs/development/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/development/contributing/code-of-conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/development/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/development/contributing/ways-to-contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/development/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/development/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/development/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.363242 imitation-0.4.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/getting-started/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/getting-started/first_steps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/getting-started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/getting-started/what_is_imitation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.363242 imitation-0.4.0/docs/main-concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/main-concepts/experts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/main-concepts/reward_networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/main-concepts/trajectories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/main-concepts/variable_horizon.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.363242 imitation-0.4.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/1_train_bc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/2_train_dagger.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/3_train_gail.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/4_train_airl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/5_train_preference_comparisons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/5a_train_preference_comparisons_with_cnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/6_train_mce.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/7_train_density.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/8_train_custom_env.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16589 2023-07-17 23:06:19.000000 imitation-0.4.0/docs/tutorials/9_compare_baselines.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.367242 imitation-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-17 23:06:19.000000 imitation-0.4.0/examples/quickstart.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-07-17 23:06:19.000000 imitation-0.4.0/examples/quickstart.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.367242 imitation-0.4.0/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1885 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/bc_benchmark.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2639 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/benchmark_and_table.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/common.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/convert_traj.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/dagger_benchmark.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3582 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/imit_benchmark.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/imit_benchmark_config.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/imit_table_cheetahs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/imit_table_mvp_seals_config.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/rollouts_from_policies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/rollouts_from_policies_config.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2841 2023-07-17 23:06:19.000000 imitation-0.4.0/experiments/transfer_learn_benchmark.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 23:06:19.000000 imitation-0.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 23:06:19.000000 imitation-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-17 23:06:19.000000 imitation-0.4.0/readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.367242 imitation-0.4.0/runners/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1308 2023-07-17 23:06:19.000000 imitation-0.4.0/runners/build_push_image.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-17 23:06:19.000000 imitation-0.4.0/runners/launch_docker-dev.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-17 23:06:30.383243 imitation-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-17 23:06:19.000000 imitation-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.347242 imitation-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.367242 imitation-0.4.0/src/imitation/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.371243 imitation-0.4.0/src/imitation/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.371243 imitation-0.4.0/src/imitation/algorithms/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/adversarial/airl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27233 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/adversarial/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/adversarial/gail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28090 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/dagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/mce_irl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75455 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/algorithms/preference_comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.371243 imitation-0.4.0/src/imitation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/data/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/data/huggingface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27416 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/data/rollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/data/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/data/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.371243 imitation-0.4.0/src/imitation/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/policies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/policies/exploration_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/policies/replay_buffer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/policies/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.371243 imitation-0.4.0/src/imitation/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/regularization/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/regularization/updaters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.371243 imitation-0.4.0/src/imitation/rewards/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/rewards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/rewards/reward_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/rewards/reward_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/rewards/reward_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/rewards/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.375243 imitation-0.4.0/src/imitation/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.375243 imitation-0.4.0/src/imitation/scripts/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/eval_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/train_adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/train_imitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/train_preference_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/config/train_rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/convert_trajs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/eval_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.375243 imitation-0.4.0/src/imitation/scripts/ingredients/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/demonstrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/expert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/policy_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/ingredients/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/train_adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/train_imitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/train_preference_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/scripts/train_rl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.375243 imitation-0.4.0/src/imitation/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/testing/expert_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/testing/hypothesis_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/testing/reward_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/testing/reward_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.379243 imitation-0.4.0/src/imitation/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/util/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/util/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/util/sacred.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-17 23:06:19.000000 imitation-0.4.0/src/imitation/util/video_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.367242 imitation-0.4.0/src/imitation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-17 23:06:29.000000 imitation-0.4.0/src/imitation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-17 23:06:30.000000 imitation-0.4.0/src/imitation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:06:29.000000 imitation-0.4.0/src/imitation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 23:06:29.000000 imitation-0.4.0/src/imitation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-17 23:06:29.000000 imitation-0.4.0/src/imitation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 23:06:29.000000 imitation-0.4.0/src/imitation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.379243 imitation-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.379243 imitation-0.4.0/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/test_adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/test_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/test_dagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/test_density_baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/test_mce_irl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32521 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/algorithms/test_preference_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.379243 imitation-0.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/data/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/data/test_huggingface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/data/test_rollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/data/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/data/test_wrappers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      353 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/generate_test_data.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.379243 imitation-0.4.0/tests/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/policies/test_exploration_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/policies/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/policies/test_replay_buffer_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/rewards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/rewards/test_reward_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30105 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/rewards/test_reward_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/rewards/test_reward_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/scripts/ingredients/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/scripts/ingredients/test_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36425 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/scripts/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/test_benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/test_regularization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.351242 imitation-0.4.0/tests/testdata/expert_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.351242 imitation-0.4.0/tests/testdata/expert_models/cartpole_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.351242 imitation-0.4.0/tests/testdata/expert_models/cartpole_0/policies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/testdata/expert_models/cartpole_0/policies/final/
+-rw-r--r--   0 runner    (1001) docker     (123)    59287 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/testdata/expert_models/cartpole_0/policies/final/model.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/testdata/expert_models/cartpole_0/rollouts/
+-rw-r--r--   0 runner    (1001) docker     (123)   415849 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/testdata/expert_models/cartpole_0/rollouts/final.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.351242 imitation-0.4.0/tests/testdata/expert_models/pendulum_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/testdata/expert_models/pendulum_0/rollouts/
+-rw-r--r--   0 runner    (1001) docker     (123)   247960 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/testdata/expert_models/pendulum_0/rollouts/final.npz
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/testdata/imit_benchmark_config.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/testdata/npz_format_rollout.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/testdata/pickle_format_rollout.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/testdata/rollouts_from_policies_config.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:06:30.383243 imitation-0.4.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/util/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/util/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/util/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/util/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-17 23:06:19.000000 imitation-0.4.0/tests/util/test_wb_logger.py
```

### Comparing `imitation-0.3.2/.circleci/config.yml` & `imitation-0.4.0/.circleci/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 executors:
   unit-test-linux:
     <<: *defaults
     resource_class: xlarge
     environment:
       # more CPUs visible but we're throttled to 8, which breaks auto-detect
       NUM_CPUS: 8
+      # Prevent git lfs from downloading files upon checkout
+      # (we want to do this explicitly, so we can cache them)
+      # see https://naiyer.dev/post/2020/09/05/using-git-lfs-in-ci/ for details
+      GIT_LFS_SKIP_SMUDGE: 1
   static-analysis-xlarge:
     <<: *defaults
     # darglint is slow enough that we benefit from xlarge even for linting.
     # However, there's little benefit from larger parallelization (I think there's
     # a handful of files with long docstrings causing the bulk of the time).
     resource_class: xlarge
     environment:
@@ -42,28 +46,40 @@
   dependencies-linux:
     # You must still manually update the Docker image if any
     # binary (non-Python) dependencies change.
     description: "Check out and update Python dependencies on Linux."
     steps:
       - checkout
 
+      # Download and cache git-lfs files
+      - run: git lfs ls-files -l | cut -d' ' -f1 | sort > .lfs-assets-id
+      - restore_cache:
+          keys:
+            - v1-lfscache-{{ checksum ".lfs-assets-id" }}
+            - v1-lfscache-
+      - run: git lfs pull
+      - save_cache:
+          paths:
+            - .git/lfs
+          key: v1-lfscache-{{ checksum ".lfs-assets-id" }}
+
       # Download and cache dependencies
       - restore_cache:
           keys:
-            - v6-linux-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
+            - v7linux-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
 
       - run:
           name: install dependencies
           # Only create venv if it's not been restored from cache
           command: "[[ -d /venv ]] || ./ci/build_and_activate_venv.sh /venv"
 
       - save_cache:
           paths:
             - /venv
-          key: v6-linux-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
+          key: v7linux-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
 
       - run:
           name: install imitation
           command: pip install --upgrade --force-reinstall --no-deps .
 
       - run:
           name: print installed packages
@@ -76,27 +92,27 @@
           name: install macOS packages
           command: HOMEBREW_NO_AUTO_UPDATE=1 brew install coreutils parallel gnu-getopt
 
       - checkout
 
       - restore_cache:
           keys:
-            - v6-macos-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
+            - v7macos-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
 
       - run:
           name: install dependencies
           # Only create venv if it's not been restored from cache.
           # We use python3.9 on macOS due to a bug with importing `ray` in python3.8:
           # https://github.com/ray-project/ray/issues/27380
           command: "[[ -d ~/venv ]] || ./ci/build_and_activate_venv.sh ~/venv python3.9"
 
       - save_cache:
           paths:
             - ~/venv
-          key: v6-macos-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
+          key: v7macos-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.sh" }}
 
       - run:
           name: install imitation
           command: |
             source ~/venv/bin/activate
             pip install --upgrade --force-reinstall --no-deps .
 
@@ -118,21 +134,22 @@
           shell: powershell.exe
 
       - checkout
 
       # Download and cache dependencies
       - restore_cache:
           keys:
-            - v6-win-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.ps1" }}
+            - v10win-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.ps1" }}
 
       - run:
           name: install python and binary dependencies
           command: |
             choco install --side-by-side -y python --version=3.8.10
             choco install -y ffmpeg
+            choco install -y openssl
           shell: powershell.exe
 
       - run:
           name: upgrade pip
           command: |
               python -m pip install --upgrade pip
           shell: powershell.exe
@@ -147,15 +164,15 @@
           # Only create venv if it's not been restored from cache
           command: if (-not (Test-Path venv)) { .\ci\build_and_activate_venv.ps1 -venv venv }
           shell: powershell.exe
 
       - save_cache:
           paths:
             - .\venv
-          key: v6-win-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.ps1" }}
+          key: v10win-dependencies-{{ checksum "setup.py" }}-{{ checksum "ci/build_and_activate_venv.ps1" }}
 
       - run:
           name: install imitation
           command: |
             .\venv\Scripts\activate
             pip install --upgrade --force-reinstall --no-deps .
           shell: powershell.exe
@@ -308,16 +325,16 @@
 
       - restore-pytest-cache
 
       - run:
           name: run tests
           command: |
             Xdummy-entrypoint.py pytest -n ${NUM_CPUS} --cov=/venv/lib/python3.8/site-packages/imitation \
-                   --cov=tests --junitxml=/tmp/test-reports/junit.xml \
-                    -vv tests/
+                  --cov=tests --junitxml=/tmp/test-reports/junit.xml \
+                  --durations=500 -vv tests/
             mv .coverage .coverage.imitation
             coverage combine  # rewrite paths from virtualenv to src/
 
       - codecov/upload
       - save-pytest-cache
       - store-test-output-unix
```

### Comparing `imitation-0.3.2/.codecov.yml` & `imitation-0.4.0/.codecov.yml`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/.dockerignore` & `imitation-0.4.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/.github/workflows/publish-to-pypi.yml` & `imitation-0.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/.gitignore` & `imitation-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/.pre-commit-config.yaml` & `imitation-0.4.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - id: check-added-large-files
 - repo: https://github.com/psf/black
   rev: 22.6.0
   hooks:
   - id: black
   - id: black-jupyter
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 # Python static analysis
 - repo: https://github.com/pycqa/flake8
   rev: '5.0.4'
   hooks:
   - id: flake8
```

### Comparing `imitation-0.3.2/Dockerfile` & `imitation-0.4.0/Dockerfile`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Based on OpenAI's mujoco-py Dockerfile
 
 # base stage contains just binary dependencies.
 # This is used in the CI build.
-FROM nvidia/cuda:11.6.2-cudnn8-runtime-ubuntu20.04 AS base
+FROM nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu20.04 AS base
 ARG DEBIAN_FRONTEND=noninteractive
 
 RUN apt-get update -q \
     && apt-get install -y --no-install-recommends \
     build-essential \
     curl \
     wget \
     ffmpeg \
     git \
+    git-lfs \
+    ssh \
     libgl1-mesa-dev \
     libgl1-mesa-glx \
     libglew-dev \
     libosmesa6-dev \
     net-tools \
     parallel \
     python3.8 \
@@ -28,19 +30,22 @@
     virtualenv \
     xpra \
     xserver-xorg-dev \
     patchelf  \
     && apt-get clean \
     && rm -rf /var/lib/apt/lists/*
 
+RUN git lfs install
+
 ENV LANG C.UTF-8
 
 # Set the PATH to the venv before we create the venv, so it's visible in base.
 # This is since we may create the venv outside of Docker, e.g. in CI
 # or by binding it in for local development.
+ENV VIRTUAL_ENV=/venv
 ENV PATH="/venv/bin:$PATH"
 ENV LD_LIBRARY_PATH /usr/local/nvidia/lib64:${LD_LIBRARY_PATH}
 
 # Run Xdummy mock X server by default so that rendering will work.
 COPY ci/xorg.conf /etc/dummy_xorg.conf
 COPY ci/Xdummy-entrypoint.py /usr/bin/Xdummy-entrypoint.py
 ENTRYPOINT ["/usr/bin/Xdummy-entrypoint.py"]
@@ -53,15 +58,20 @@
 WORKDIR /imitation
 # Copy over just setup.py and dependencies (__init__.py and README.md)
 # to avoid rebuilding venv when requirements have not changed.
 COPY ./setup.py ./setup.py
 COPY ./README.md ./README.md
 COPY ./src/imitation/__init__.py ./src/imitation/__init__.py
 COPY ci/build_and_activate_venv.sh ./ci/build_and_activate_venv.sh
-RUN    ci/build_and_activate_venv.sh /venv \
+
+# Pass mock value for version because .git is not present in the Docker container
+# at this stage, so setuptools-scm cannot determine version automatically.
+# setuptools-scm will compute it correctly when it comes to building and installing
+# imitation, as .git will then be present.
+RUN SETUPTOOLS_SCM_PRETEND_VERSION="dummy" ci/build_and_activate_venv.sh /venv \
     && rm -rf $HOME/.cache/pip
 
 # full stage contains everything.
 # Can be used for deployment and local testing.
 FROM python-req as full
 
 # Delay copying (and installing) the code until the very end
```

### Comparing `imitation-0.3.2/LICENSE` & `imitation-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/PKG-INFO` & `imitation-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: imitation
-Version: 0.3.2
-Summary: Implementation of modern reward and imitation learning algorithms.
-Home-page: https://github.com/HumanCompatibleAI/imitation
-Author: Center for Human-Compatible AI and Google
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: parallel
-Provides-Extra: mujoco
-Provides-Extra: atari
-License-File: LICENSE
-
 [![CircleCI](https://circleci.com/gh/HumanCompatibleAI/imitation.svg?style=svg)](https://circleci.com/gh/HumanCompatibleAI/imitation)
 [![Documentation Status](https://readthedocs.org/projects/imitation/badge/?version=latest)](https://imitation.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/HumanCompatibleAI/imitation/branch/master/graph/badge.svg)](https://codecov.io/gh/HumanCompatibleAI/imitation)
 [![PyPI version](https://badge.fury.io/py/imitation.svg)](https://badge.fury.io/py/imitation)
 
 # Imitation Learning Baseline Implementations
 
@@ -92,21 +67,21 @@
 
 We provide several CLI scripts as a front-end to the algorithms implemented in `imitation`. These use [Sacred](https://github.com/idsia/sacred) for configuration and replicability.
 
 From [examples/quickstart.sh:](examples/quickstart.sh)
 
 ```bash
 # Train PPO agent on pendulum and collect expert demonstrations. Tensorboard logs saved in quickstart/rl/
-python -m imitation.scripts.train_rl with pendulum common.fast train.fast rl.fast fast common.log_dir=quickstart/rl/
+python -m imitation.scripts.train_rl with pendulum environment.fast policy_evaluation.fast rl.fast fast logging.log_dir=quickstart/rl/
 
 # Train GAIL from demonstrations. Tensorboard logs saved in output/ (default log directory).
-python -m imitation.scripts.train_adversarial gail with pendulum common.fast demonstrations.fast train.fast rl.fast fast demonstrations.rollout_path=quickstart/rl/rollouts/final.npz
+python -m imitation.scripts.train_adversarial gail with pendulum environment.fast demonstrations.fast policy_evaluation.fast rl.fast fast demonstrations.path=quickstart/rl/rollouts/final.npz demonstrations.source=local
 
 # Train AIRL from demonstrations. Tensorboard logs saved in output/ (default log directory).
-python -m imitation.scripts.train_adversarial airl with pendulum common.fast demonstrations.fast train.fast rl.fast fast demonstrations.rollout_path=quickstart/rl/rollouts/final.npz
+python -m imitation.scripts.train_adversarial airl with pendulum environment.fast demonstrations.fast policy_evaluation.fast rl.fast fast demonstrations.path=quickstart/rl/rollouts/final.npz demonstrations.source=local
 ```
 
 Tips:
 
 - Remove the "fast" options from the commands above to allow training run to completion.
 - `python -m imitation.scripts.train_rl print_config` will list Sacred script options. These configuration options are documented in each script's docstrings.
 
@@ -119,21 +94,23 @@
 ### Density reward baseline
 
 We also implement a density-based reward baseline. You can find an [example notebook here](docs/tutorials/7_train_density.ipynb).
 
 # Citations (BibTeX)
 
 ```
-@misc{wang2020imitation,
-  author = {Wang, Steven and Toyer, Sam and Gleave, Adam and Emmons, Scott},
-  title = {The {\tt imitation} Library for Imitation Learning and Inverse Reinforcement Learning},
-  year = {2020},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/HumanCompatibleAI/imitation}},
+@misc{gleave2022imitation,
+  author = {Gleave, Adam and Taufeeque, Mohammad and Rocamonde, Juan and Jenner, Erik and Wang, Steven H. and Toyer, Sam and Ernestus, Maximilian and Belrose, Nora and Emmons, Scott and Russell, Stuart},
+  title = {imitation: Clean Imitation Learning Implementations},
+  year = {2022},
+  howPublished = {arXiv:2211.11972v1 [cs.LG]},
+  archivePrefix = {arXiv},
+  eprint = {2211.11972},
+  primaryClass = {cs.LG},
+  url = {https://arxiv.org/abs/2211.11972},
 }
 ```
 
 # Contributing
 
 See [Contributing to imitation][contributing] for more information.
```

### Comparing `imitation-0.3.2/README.md` & `imitation-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: imitation
+Version: 0.4.0
+Summary: Implementation of modern reward and imitation learning algorithms.
+Home-page: https://github.com/HumanCompatibleAI/imitation
+Author: Center for Human-Compatible AI and Google
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: docs
+Provides-Extra: parallel
+Provides-Extra: mujoco
+Provides-Extra: atari
+License-File: LICENSE
+
 [![CircleCI](https://circleci.com/gh/HumanCompatibleAI/imitation.svg?style=svg)](https://circleci.com/gh/HumanCompatibleAI/imitation)
 [![Documentation Status](https://readthedocs.org/projects/imitation/badge/?version=latest)](https://imitation.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/HumanCompatibleAI/imitation/branch/master/graph/badge.svg)](https://codecov.io/gh/HumanCompatibleAI/imitation)
 [![PyPI version](https://badge.fury.io/py/imitation.svg)](https://badge.fury.io/py/imitation)
 
 # Imitation Learning Baseline Implementations
 
@@ -67,21 +92,21 @@
 
 We provide several CLI scripts as a front-end to the algorithms implemented in `imitation`. These use [Sacred](https://github.com/idsia/sacred) for configuration and replicability.
 
 From [examples/quickstart.sh:](examples/quickstart.sh)
 
 ```bash
 # Train PPO agent on pendulum and collect expert demonstrations. Tensorboard logs saved in quickstart/rl/
-python -m imitation.scripts.train_rl with pendulum common.fast train.fast rl.fast fast common.log_dir=quickstart/rl/
+python -m imitation.scripts.train_rl with pendulum environment.fast policy_evaluation.fast rl.fast fast logging.log_dir=quickstart/rl/
 
 # Train GAIL from demonstrations. Tensorboard logs saved in output/ (default log directory).
-python -m imitation.scripts.train_adversarial gail with pendulum common.fast demonstrations.fast train.fast rl.fast fast demonstrations.rollout_path=quickstart/rl/rollouts/final.npz
+python -m imitation.scripts.train_adversarial gail with pendulum environment.fast demonstrations.fast policy_evaluation.fast rl.fast fast demonstrations.path=quickstart/rl/rollouts/final.npz demonstrations.source=local
 
 # Train AIRL from demonstrations. Tensorboard logs saved in output/ (default log directory).
-python -m imitation.scripts.train_adversarial airl with pendulum common.fast demonstrations.fast train.fast rl.fast fast demonstrations.rollout_path=quickstart/rl/rollouts/final.npz
+python -m imitation.scripts.train_adversarial airl with pendulum environment.fast demonstrations.fast policy_evaluation.fast rl.fast fast demonstrations.path=quickstart/rl/rollouts/final.npz demonstrations.source=local
 ```
 
 Tips:
 
 - Remove the "fast" options from the commands above to allow training run to completion.
 - `python -m imitation.scripts.train_rl print_config` will list Sacred script options. These configuration options are documented in each script's docstrings.
 
@@ -94,21 +119,23 @@
 ### Density reward baseline
 
 We also implement a density-based reward baseline. You can find an [example notebook here](docs/tutorials/7_train_density.ipynb).
 
 # Citations (BibTeX)
 
 ```
-@misc{wang2020imitation,
-  author = {Wang, Steven and Toyer, Sam and Gleave, Adam and Emmons, Scott},
-  title = {The {\tt imitation} Library for Imitation Learning and Inverse Reinforcement Learning},
-  year = {2020},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/HumanCompatibleAI/imitation}},
+@misc{gleave2022imitation,
+  author = {Gleave, Adam and Taufeeque, Mohammad and Rocamonde, Juan and Jenner, Erik and Wang, Steven H. and Toyer, Sam and Ernestus, Maximilian and Belrose, Nora and Emmons, Scott and Russell, Stuart},
+  title = {imitation: Clean Imitation Learning Implementations},
+  year = {2022},
+  howPublished = {arXiv:2211.11972v1 [cs.LG]},
+  archivePrefix = {arXiv},
+  eprint = {2211.11972},
+  primaryClass = {cs.LG},
+  url = {https://arxiv.org/abs/2211.11972},
 }
 ```
 
 # Contributing
 
 See [Contributing to imitation][contributing] for more information.
```

### Comparing `imitation-0.3.2/benchmarking/README.md` & `imitation-0.4.0/benchmarking/README.md`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/benchmarking/example_airl_seals_ant_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_gail_seals_half_cheetah_best_hp_eval.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48636363636363633%*

 * *Differences: {"'algorithm_kwargs'": "{'gen_replay_buffer_capacity': 512, 'n_disc_updates_per_round': 8}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/HalfCheetah-v0')])",*

 * * "'policy'": "OrderedDict([('policy_cls', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.FeedForward32Policy')])), ('policy_kwargs', "*

 * *             "OrderedDict([('features_extractor_class', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.No […]*

```diff
@@ -1,63 +1,67 @@
 {
     "algorithm_kwargs": {
         "demo_batch_size": 8192,
-        "gen_replay_buffer_capacity": 8192,
-        "n_disc_updates_per_round": 16
+        "gen_replay_buffer_capacity": 512,
+        "n_disc_updates_per_round": 8
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Ant-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/HalfCheetah-v0"
+    },
+    "policy": {
+        "policy_cls": {
+            "py/type": "imitation.policies.base.FeedForward32Policy"
+        },
+        "policy_kwargs": {
+            "features_extractor_class": {
+                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
+            },
+            "features_extractor_kwargs": {
+                "normalize_class": {
+                    "py/type": "imitation.util.networks.RunningNorm"
+                }
+            }
+        }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     },
     "reward": {
         "add_std_alpha": null,
         "ensemble_size": null,
         "net_cls": {
-            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
+            "py/type": "imitation.rewards.reward_nets.BasicRewardNet"
         },
         "net_kwargs": {
             "normalize_input_layer": {
                 "py/type": "imitation.util.networks.RunningNorm"
             }
         },
         "normalize_output_layer": {
             "py/type": "imitation.util.networks.RunningNorm"
         }
     },
     "rl": {
-        "batch_size": 8192,
+        "batch_size": 4096,
         "rl_cls": {
             "py/type": "stable_baselines3.ppo.ppo.PPO"
         },
         "rl_kwargs": {
-            "batch_size": 16,
-            "clip_range": 0.3,
-            "ent_coef": 3.27750078482474e-06,
-            "gae_lambda": 0.8,
-            "gamma": 0.995,
-            "learning_rate": 3.249429831179079e-05,
-            "max_grad_norm": 0.9,
-            "n_epochs": 10,
-            "vf_coef": 0.4351450387648799
+            "batch_size": 64,
+            "clip_range": 0.1,
+            "ent_coef": 3.992371122209408e-06,
+            "gae_lambda": 0.95,
+            "gamma": 0.95,
+            "learning_rate": 0.00026250519057717037,
+            "max_grad_norm": 0.8,
+            "n_epochs": 5,
+            "vf_coef": 0.11483689492120866
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
-        "policy_cls": {
-            "py/type": "imitation.policies.base.FeedForward32Policy"
-        },
-        "policy_kwargs": {
-            "features_extractor_class": {
-                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
-            },
-            "features_extractor_kwargs": {
-                "normalize_class": {
-                    "py/type": "imitation.util.networks.RunningNorm"
-                }
-            }
-        }
-    }
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_airl_seals_half_cheetah_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_airl_seals_half_cheetah_best_hp_eval.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5151515151515151%*

 * *Differences: {"'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/HalfCheetah-v0')])",*

 * * "'policy'": "OrderedDict([('policy_cls', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.FeedForward32Policy')])), ('policy_kwargs', "*

 * *             "OrderedDict([('features_extractor_class', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.NormalizeFeaturesExtractor')])), "*

 * *             "('features_extractor_kwargs', OrderedDict([('n […]*

```diff
@@ -1,19 +1,39 @@
 {
     "algorithm_kwargs": {
         "demo_batch_size": 2048,
         "gen_replay_buffer_capacity": 512,
         "n_disc_updates_per_round": 16
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/HalfCheetah-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/HalfCheetah-v0"
+    },
+    "policy": {
+        "policy_cls": {
+            "py/type": "imitation.policies.base.FeedForward32Policy"
+        },
+        "policy_kwargs": {
+            "features_extractor_class": {
+                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
+            },
+            "features_extractor_kwargs": {
+                "normalize_class": {
+                    "py/type": "imitation.util.networks.RunningNorm"
+                }
+            }
+        }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     },
     "reward": {
         "add_std_alpha": null,
         "ensemble_size": null,
         "net_cls": {
             "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
         },
@@ -39,25 +59,9 @@
             "gamma": 0.95,
             "learning_rate": 0.00047248619386801587,
             "max_grad_norm": 0.8,
             "n_epochs": 5,
             "vf_coef": 0.11483689492120866
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
-        "policy_cls": {
-            "py/type": "imitation.policies.base.FeedForward32Policy"
-        },
-        "policy_kwargs": {
-            "features_extractor_class": {
-                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
-            },
-            "features_extractor_kwargs": {
-                "normalize_class": {
-                    "py/type": "imitation.util.networks.RunningNorm"
-                }
-            }
-        }
-    }
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_airl_seals_hopper_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_gail_seals_walker_best_hp_eval.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.44621913580246914%*

 * *Differences: {"'algorithm_kwargs'": "{'demo_batch_size': 512, 'gen_replay_buffer_capacity': 16384}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Walker2d-v0')])",*

 * * "'expert'": "OrderedDict([('loader_kwargs', OrderedDict([('gym_id', 'seals/Walker2d-v0'), "*

 * *             "('organization', 'HumanCompatibleAI')]))])",*

 * * "'policy'": "OrderedDict([('policy_cls', 'MlpPolicy'), ('policy_kwargs', "*

 * *             "OrderedDict([('activation_fn', OrderedDict([ […]*

```diff
@@ -1,55 +1,29 @@
 {
     "algorithm_kwargs": {
-        "demo_batch_size": 2048,
-        "gen_replay_buffer_capacity": 8192,
+        "demo_batch_size": 512,
+        "gen_replay_buffer_capacity": 16384,
         "n_disc_updates_per_round": 16
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Hopper-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
     },
-    "reward": {
-        "add_std_alpha": null,
-        "ensemble_size": null,
-        "net_cls": {
-            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
-        },
-        "net_kwargs": {
-            "normalize_input_layer": {
-                "py/type": "imitation.util.networks.RunningNorm"
-            }
-        },
-        "normalize_output_layer": {
-            "py/type": "imitation.util.networks.RunningNorm"
-        }
+    "environment": {
+        "gym_id": "seals/Walker2d-v0"
     },
-    "rl": {
-        "batch_size": 8192,
-        "rl_cls": {
-            "py/type": "stable_baselines3.ppo.ppo.PPO"
-        },
-        "rl_kwargs": {
-            "batch_size": 512,
-            "clip_range": 0.1,
-            "ent_coef": 0.009709494745755033,
-            "gae_lambda": 0.98,
-            "gamma": 0.995,
-            "learning_rate": 0.0005807211840258373,
-            "max_grad_norm": 0.9,
-            "n_epochs": 20,
-            "vf_coef": 0.20315938606555833
+    "expert": {
+        "loader_kwargs": {
+            "gym_id": "seals/Walker2d-v0",
+            "organization": "HumanCompatibleAI"
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
+    "policy": {
         "policy_cls": "MlpPolicy",
         "policy_kwargs": {
             "activation_fn": {
                 "py/type": "torch.nn.modules.activation.ReLU"
             },
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
@@ -68,9 +42,45 @@
                     "vf": [
                         64,
                         64
                     ]
                 }
             ]
         }
-    }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
+    },
+    "reward": {
+        "add_std_alpha": null,
+        "ensemble_size": null,
+        "net_cls": {
+            "py/type": "imitation.rewards.reward_nets.BasicRewardNet"
+        },
+        "net_kwargs": {
+            "normalize_input_layer": {
+                "py/type": "imitation.util.networks.RunningNorm"
+            }
+        },
+        "normalize_output_layer": {
+            "py/type": "imitation.util.networks.RunningNorm"
+        }
+    },
+    "rl": {
+        "batch_size": 16384,
+        "rl_cls": {
+            "py/type": "stable_baselines3.ppo.ppo.PPO"
+        },
+        "rl_kwargs": {
+            "batch_size": 128,
+            "clip_range": 0.4,
+            "ent_coef": 0.0007566389899529574,
+            "gae_lambda": 0.92,
+            "gamma": 0.98,
+            "learning_rate": 1.943992487657563e-05,
+            "max_grad_norm": 0.6,
+            "n_epochs": 20,
+            "vf_coef": 0.6167177795726859
+        }
+    },
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_airl_seals_swimmer_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_airl_seals_walker_best_hp_eval.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.53125%*

 * *Differences: {"'algorithm_kwargs'": "{'demo_batch_size': 512}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Walker2d-v0')])",*

 * * "'expert'": "{'loader_kwargs': {'gym_id': 'seals/Walker2d-v0', delete: ['env_name']}}",*

 * * "'policy'": "OrderedDict([('policy_cls', 'MlpPolicy'), ('policy_kwargs', "*

 * *             "OrderedDict([('activation_fn', OrderedDict([('py/type', "*

 * *             "'torch.nn.modules.activation.ReLU')])), ('features_extractor_class', "*

 * *  […]*

```diff
@@ -1,61 +1,29 @@
 {
     "algorithm_kwargs": {
-        "demo_batch_size": 128,
+        "demo_batch_size": 512,
         "gen_replay_buffer_capacity": 16384,
         "n_disc_updates_per_round": 16
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Swimmer-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Walker2d-v0"
     },
     "expert": {
         "loader_kwargs": {
-            "env_name": "seals/Swimmer-v0",
+            "gym_id": "seals/Walker2d-v0",
             "organization": "HumanCompatibleAI"
         }
     },
-    "reward": {
-        "add_std_alpha": null,
-        "ensemble_size": null,
-        "net_cls": {
-            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
-        },
-        "net_kwargs": {
-            "normalize_input_layer": {
-                "py/type": "imitation.util.networks.RunningNorm"
-            }
-        },
-        "normalize_output_layer": {
-            "py/type": "imitation.util.networks.RunningNorm"
-        }
-    },
-    "rl": {
-        "batch_size": 16384,
-        "rl_cls": {
-            "py/type": "stable_baselines3.ppo.ppo.PPO"
-        },
-        "rl_kwargs": {
-            "batch_size": 64,
-            "clip_range": 0.1,
-            "ent_coef": 0.006137718463434523,
-            "gae_lambda": 0.95,
-            "gamma": 0.999,
-            "learning_rate": 0.0013390060486393868,
-            "max_grad_norm": 2,
-            "n_epochs": 5,
-            "vf_coef": 0.6162112311062333
-        }
-    },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
+    "policy": {
         "policy_cls": "MlpPolicy",
         "policy_kwargs": {
             "activation_fn": {
                 "py/type": "torch.nn.modules.activation.ReLU"
             },
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
@@ -74,9 +42,45 @@
                     "vf": [
                         64,
                         64
                     ]
                 }
             ]
         }
-    }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
+    },
+    "reward": {
+        "add_std_alpha": null,
+        "ensemble_size": null,
+        "net_cls": {
+            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
+        },
+        "net_kwargs": {
+            "normalize_input_layer": {
+                "py/type": "imitation.util.networks.RunningNorm"
+            }
+        },
+        "normalize_output_layer": {
+            "py/type": "imitation.util.networks.RunningNorm"
+        }
+    },
+    "rl": {
+        "batch_size": 16384,
+        "rl_cls": {
+            "py/type": "stable_baselines3.ppo.ppo.PPO"
+        },
+        "rl_kwargs": {
+            "batch_size": 128,
+            "clip_range": 0.4,
+            "ent_coef": 0.002003867232707145,
+            "gae_lambda": 0.92,
+            "gamma": 0.98,
+            "learning_rate": 3.052170958603811e-05,
+            "max_grad_norm": 0.6,
+            "n_epochs": 20,
+            "vf_coef": 0.6167177795726859
+        }
+    },
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_airl_seals_walker_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_airl_seals_swimmer_best_hp_eval.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.53125%*

 * *Differences: {"'algorithm_kwargs'": "{'demo_batch_size': 128}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Swimmer-v0')])",*

 * * "'expert'": "{'loader_kwargs': {'gym_id': 'seals/Swimmer-v0', delete: ['env_name']}}",*

 * * "'policy'": "OrderedDict([('policy_cls', 'MlpPolicy'), ('policy_kwargs', "*

 * *             "OrderedDict([('activation_fn', OrderedDict([('py/type', "*

 * *             "'torch.nn.modules.activation.ReLU')])), ('features_extractor_class', "*

 * *    […]*

```diff
@@ -1,61 +1,29 @@
 {
     "algorithm_kwargs": {
-        "demo_batch_size": 512,
+        "demo_batch_size": 128,
         "gen_replay_buffer_capacity": 16384,
         "n_disc_updates_per_round": 16
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Walker2d-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Swimmer-v0"
     },
     "expert": {
         "loader_kwargs": {
-            "env_name": "seals/Walker2d-v0",
+            "gym_id": "seals/Swimmer-v0",
             "organization": "HumanCompatibleAI"
         }
     },
-    "reward": {
-        "add_std_alpha": null,
-        "ensemble_size": null,
-        "net_cls": {
-            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
-        },
-        "net_kwargs": {
-            "normalize_input_layer": {
-                "py/type": "imitation.util.networks.RunningNorm"
-            }
-        },
-        "normalize_output_layer": {
-            "py/type": "imitation.util.networks.RunningNorm"
-        }
-    },
-    "rl": {
-        "batch_size": 16384,
-        "rl_cls": {
-            "py/type": "stable_baselines3.ppo.ppo.PPO"
-        },
-        "rl_kwargs": {
-            "batch_size": 128,
-            "clip_range": 0.4,
-            "ent_coef": 0.002003867232707145,
-            "gae_lambda": 0.92,
-            "gamma": 0.98,
-            "learning_rate": 3.052170958603811e-05,
-            "max_grad_norm": 0.6,
-            "n_epochs": 20,
-            "vf_coef": 0.6167177795726859
-        }
-    },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
+    "policy": {
         "policy_cls": "MlpPolicy",
         "policy_kwargs": {
             "activation_fn": {
                 "py/type": "torch.nn.modules.activation.ReLU"
             },
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
@@ -74,9 +42,45 @@
                     "vf": [
                         64,
                         64
                     ]
                 }
             ]
         }
-    }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
+    },
+    "reward": {
+        "add_std_alpha": null,
+        "ensemble_size": null,
+        "net_cls": {
+            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
+        },
+        "net_kwargs": {
+            "normalize_input_layer": {
+                "py/type": "imitation.util.networks.RunningNorm"
+            }
+        },
+        "normalize_output_layer": {
+            "py/type": "imitation.util.networks.RunningNorm"
+        }
+    },
+    "rl": {
+        "batch_size": 16384,
+        "rl_cls": {
+            "py/type": "stable_baselines3.ppo.ppo.PPO"
+        },
+        "rl_kwargs": {
+            "batch_size": 64,
+            "clip_range": 0.1,
+            "ent_coef": 0.006137718463434523,
+            "gae_lambda": 0.95,
+            "gamma": 0.999,
+            "learning_rate": 0.0013390060486393868,
+            "max_grad_norm": 2,
+            "n_epochs": 5,
+            "vf_coef": 0.6162112311062333
+        }
+    },
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_bc_seals_ant_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_bc_seals_walker_best_hp_eval.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 32), ('l2_weight', 0.0014680228143404998), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.0003034620018780926)])), ('train_kwargs', "*

 * *         "OrderedDict([('log_interval', 500), ('n_batches', None), ('n_epochs', 20)]))])",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Walker2d-v0')])",*

 * * "'policy'": "Order […]*

```diff
@@ -1,44 +1,48 @@
 {
-    "bc_kwargs": {
-        "batch_size": 16,
-        "l2_weight": 2.350251568550711e-05,
+    "bc": {
+        "batch_size": 32,
+        "l2_weight": 0.0014680228143404998,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
-            "lr": 0.0017601048183920826
+            "lr": 0.0003034620018780926
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 20
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 5
-    },
-    "common": {
-        "env_name": "seals/Ant-v0"
-    },
     "dagger": {
         "rollout_round_min_episodes": null,
-        "total_timesteps": 100000.0,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "environment": {
+        "gym_id": "seals/Walker2d-v0"
+    },
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_bc_seals_half_cheetah_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_bc_seals_half_cheetah_best_hp_eval.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 64), ('l2_weight', 0.005728455628518169), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.008056922426724927)])), ('train_kwargs', "*

 * *         "OrderedDict([('log_interval', 500), ('n_batches', None), ('n_epochs', 20)]))])",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/HalfCheetah-v0')])",*

 * * "'policy'": "Orde […]*

```diff
@@ -1,44 +1,48 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 64,
         "l2_weight": 0.005728455628518169,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
             "lr": 0.008056922426724927
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 20
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 20
-    },
-    "common": {
-        "env_name": "seals/HalfCheetah-v0"
-    },
     "dagger": {
         "rollout_round_min_episodes": null,
         "total_timesteps": 60000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "environment": {
+        "gym_id": "seals/HalfCheetah-v0"
+    },
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_bc_seals_hopper_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_bc_seals_hopper_best_hp_eval.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 64), ('l2_weight', 1.3610189916104634e-06), "*

 * *         "('optimizer_cls', OrderedDict([('py/type', 'torch.optim.adam.Adam')])), "*

 * *         "('optimizer_kwargs', OrderedDict([('lr', 0.0007172435323620212)])), ('train_kwargs', "*

 * *         "OrderedDict([('log_interval', 500), ('n_batches', None), ('n_epochs', 20)]))])",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Hopper-v0')])",*

 * * "'policy'": "Ordere […]*

```diff
@@ -1,44 +1,48 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 64,
         "l2_weight": 1.3610189916104634e-06,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
             "lr": 0.0007172435323620212
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 20
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 20
-    },
-    "common": {
-        "env_name": "seals/Hopper-v0"
-    },
     "dagger": {
         "rollout_round_min_episodes": null,
-        "total_timesteps": 100000.0,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "environment": {
+        "gym_id": "seals/Hopper-v0"
+    },
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_bc_seals_swimmer_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_dagger_seals_swimmer_best_hp_eval.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.14791666666666664%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 16), ('l2_weight', 0.0001), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.001)])), ('train_kwargs', OrderedDict([('log_interval', 500), "*

 * *         "('n_batches', None), ('n_epochs', 1)]))])",*

 * * "'dagger'": "{'rollout_round_min_episodes': 3, 'beta_schedule': OrderedDict([('py/object', "*

 * *             "'imitation.algorithms.dagger.LinearBetaSchedule'), ('rampdown_rounds', 15)])}",*

 * *  […]*

```diff
@@ -1,44 +1,52 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 16,
-        "l2_weight": 4.37857842825771e-05,
+        "l2_weight": 0.0001,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
-            "lr": 0.0016370547173923296
+            "lr": 0.001
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 1
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 10
-    },
-    "common": {
-        "env_name": "seals/Swimmer-v0"
-    },
     "dagger": {
-        "rollout_round_min_episodes": null,
-        "total_timesteps": 100000.0,
+        "beta_schedule": {
+            "py/object": "imitation.algorithms.dagger.LinearBetaSchedule",
+            "rampdown_rounds": 15
+        },
+        "rollout_round_min_episodes": 3,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Swimmer-v0"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_bc_seals_walker_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_dagger_seals_walker_best_hp_eval.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.14791666666666664%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 16), ('l2_weight', 0.0001), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.001)])), ('train_kwargs', OrderedDict([('log_interval', 500), "*

 * *         "('n_batches', None), ('n_epochs', 5)]))])",*

 * * "'dagger'": "{'rollout_round_min_episodes': 5, 'beta_schedule': "*

 * *             "OrderedDict([('decay_probability', 0.7), ('py/object', "*

 * *             "'imitation.algorithms.dagger.Exponent […]*

```diff
@@ -1,44 +1,52 @@
 {
-    "bc_kwargs": {
-        "batch_size": 32,
-        "l2_weight": 0.0014680228143404998,
+    "bc": {
+        "batch_size": 16,
+        "l2_weight": 0.0001,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
-            "lr": 0.0003034620018780926
+            "lr": 0.001
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 5
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 20
-    },
-    "common": {
-        "env_name": "seals/Walker2d-v0"
-    },
     "dagger": {
-        "rollout_round_min_episodes": null,
-        "total_timesteps": 100000.0,
+        "beta_schedule": {
+            "decay_probability": 0.7,
+            "py/object": "imitation.algorithms.dagger.ExponentialBetaSchedule"
+        },
+        "rollout_round_min_episodes": 5,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Walker2d-v0"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_dagger_seals_ant_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_dagger_seals_ant_best_hp_eval.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 16), ('l2_weight', 0.0001), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.001)])), ('train_kwargs', OrderedDict([('log_interval', 500), "*

 * *         "('n_batches', None), ('n_epochs', 10)]))])",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Ant-v0')])",*

 * * "'policy'": "OrderedDict([('policy_cls', OrderedDict([ […]*

```diff
@@ -1,48 +1,52 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 16,
         "l2_weight": 0.0001,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
             "lr": 0.001
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 10
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 10
-    },
-    "common": {
-        "env_name": "seals/Ant-v0"
-    },
     "dagger": {
         "beta_schedule": {
             "py/object": "imitation.algorithms.dagger.LinearBetaSchedule",
             "rampdown_rounds": 15
         },
         "rollout_round_min_episodes": 5,
-        "total_timesteps": 100000.0,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "environment": {
+        "gym_id": "seals/Ant-v0"
+    },
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_dagger_seals_half_cheetah_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_dagger_seals_hopper_best_hp_eval.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15416666666666665%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 16), ('l2_weight', 0.0001), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.001)])), ('train_kwargs', OrderedDict([('log_interval', 500), "*

 * *         "('n_batches', None), ('n_epochs', 1)]))])",*

 * * "'dagger'": "{'rollout_round_min_episodes': 10, 'total_timesteps': 100000}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id' […]*

```diff
@@ -1,48 +1,52 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 16,
         "l2_weight": 0.0001,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
             "lr": 0.001
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 1
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 5
-    },
-    "common": {
-        "env_name": "seals/HalfCheetah-v0"
-    },
     "dagger": {
         "beta_schedule": {
             "decay_probability": 0.7,
             "py/object": "imitation.algorithms.dagger.ExponentialBetaSchedule"
         },
-        "rollout_round_min_episodes": 5,
-        "total_timesteps": 60000,
+        "rollout_round_min_episodes": 10,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "environment": {
+        "gym_id": "seals/Hopper-v0"
+    },
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_dagger_seals_hopper_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_dagger_seals_half_cheetah_best_hp_eval.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15416666666666665%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 16), ('l2_weight', 0.0001), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.001)])), ('train_kwargs', OrderedDict([('log_interval', 500), "*

 * *         "('n_batches', None), ('n_epochs', 5)]))])",*

 * * "'dagger'": "{'rollout_round_min_episodes': 5, 'total_timesteps': 60000}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id',  […]*

```diff
@@ -1,48 +1,52 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 16,
         "l2_weight": 0.0001,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
             "lr": 0.001
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 5
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 1
-    },
-    "common": {
-        "env_name": "seals/Hopper-v0"
-    },
     "dagger": {
         "beta_schedule": {
             "decay_probability": 0.7,
             "py/object": "imitation.algorithms.dagger.ExponentialBetaSchedule"
         },
-        "rollout_round_min_episodes": 10,
-        "total_timesteps": 100000.0,
+        "rollout_round_min_episodes": 5,
+        "total_timesteps": 60000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "environment": {
+        "gym_id": "seals/HalfCheetah-v0"
+    },
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_dagger_seals_swimmer_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_bc_seals_swimmer_best_hp_eval.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.14791666666666664%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 16), ('l2_weight', 4.37857842825771e-05), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.0016370547173923296)])), ('train_kwargs', "*

 * *         "OrderedDict([('log_interval', 500), ('n_batches', None), ('n_epochs', 10)]))])",*

 * * "'dagger'": "{'rollout_round_min_episodes': None, delete: ['beta_schedule']}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'envir […]*

```diff
@@ -1,48 +1,48 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 16,
-        "l2_weight": 0.0001,
+        "l2_weight": 4.37857842825771e-05,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
-            "lr": 0.001
+            "lr": 0.0016370547173923296
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 10
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 1
-    },
-    "common": {
-        "env_name": "seals/Swimmer-v0"
-    },
     "dagger": {
-        "beta_schedule": {
-            "py/object": "imitation.algorithms.dagger.LinearBetaSchedule",
-            "rampdown_rounds": 15
-        },
-        "rollout_round_min_episodes": 3,
-        "total_timesteps": 100000.0,
+        "rollout_round_min_episodes": null,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Swimmer-v0"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_dagger_seals_walker_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_bc_seals_ant_best_hp_eval.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.14791666666666664%*

 * *Differences: {"'bc'": "OrderedDict([('batch_size', 16), ('l2_weight', 2.350251568550711e-05), ('optimizer_cls', "*

 * *         "OrderedDict([('py/type', 'torch.optim.adam.Adam')])), ('optimizer_kwargs', "*

 * *         "OrderedDict([('lr', 0.0017601048183920826)])), ('train_kwargs', "*

 * *         "OrderedDict([('log_interval', 500), ('n_batches', None), ('n_epochs', 5)]))])",*

 * * "'dagger'": "{'rollout_round_min_episodes': None, delete: ['beta_schedule']}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'envir […]*

```diff
@@ -1,48 +1,48 @@
 {
-    "bc_kwargs": {
+    "bc": {
         "batch_size": 16,
-        "l2_weight": 0.0001,
+        "l2_weight": 2.350251568550711e-05,
         "optimizer_cls": {
             "py/type": "torch.optim.adam.Adam"
         },
         "optimizer_kwargs": {
-            "lr": 0.001
+            "lr": 0.0017601048183920826
+        },
+        "train_kwargs": {
+            "log_interval": 500,
+            "n_batches": null,
+            "n_epochs": 5
         }
     },
-    "bc_train_kwargs": {
-        "log_interval": 500,
-        "n_batches": null,
-        "n_epochs": 5
-    },
-    "common": {
-        "env_name": "seals/Walker2d-v0"
-    },
     "dagger": {
-        "beta_schedule": {
-            "decay_probability": 0.7,
-            "py/object": "imitation.algorithms.dagger.ExponentialBetaSchedule"
-        },
-        "rollout_round_min_episodes": 5,
-        "total_timesteps": 100000.0,
+        "rollout_round_min_episodes": null,
+        "total_timesteps": 100000,
         "use_offline_rollouts": false
     },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Ant-v0"
     },
-    "train": {
-        "n_episodes_eval": 50,
+    "policy": {
         "policy_cls": {
             "py/type": "imitation.policies.base.FeedForward32Policy"
         },
         "policy_kwargs": {
             "features_extractor_class": {
                 "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
             },
             "features_extractor_kwargs": {
                 "normalize_class": {
                     "py/type": "imitation.util.networks.RunningNorm"
                 }
             }
         }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     }
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_gail_seals_ant_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_gail_seals_ant_best_hp_eval.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5151515151515151%*

 * *Differences: {"'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Ant-v0')])",*

 * * "'policy'": "OrderedDict([('policy_cls', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.FeedForward32Policy')])), ('policy_kwargs', "*

 * *             "OrderedDict([('features_extractor_class', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.NormalizeFeaturesExtractor')])), "*

 * *             "('features_extractor_kwargs', OrderedDict([('normalize […]*

```diff
@@ -1,19 +1,39 @@
 {
     "algorithm_kwargs": {
         "demo_batch_size": 32,
         "gen_replay_buffer_capacity": 16384,
         "n_disc_updates_per_round": 8
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Ant-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Ant-v0"
+    },
+    "policy": {
+        "policy_cls": {
+            "py/type": "imitation.policies.base.FeedForward32Policy"
+        },
+        "policy_kwargs": {
+            "features_extractor_class": {
+                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
+            },
+            "features_extractor_kwargs": {
+                "normalize_class": {
+                    "py/type": "imitation.util.networks.RunningNorm"
+                }
+            }
+        }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     },
     "reward": {
         "add_std_alpha": null,
         "ensemble_size": null,
         "net_cls": {
             "py/type": "imitation.rewards.reward_nets.BasicRewardNet"
         },
@@ -39,25 +59,9 @@
             "gamma": 0.995,
             "learning_rate": 2.428297806883194e-05,
             "max_grad_norm": 0.9,
             "n_epochs": 10,
             "vf_coef": 0.4351450387648799
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
-        "policy_cls": {
-            "py/type": "imitation.policies.base.FeedForward32Policy"
-        },
-        "policy_kwargs": {
-            "features_extractor_class": {
-                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
-            },
-            "features_extractor_kwargs": {
-                "normalize_class": {
-                    "py/type": "imitation.util.networks.RunningNorm"
-                }
-            }
-        }
-    }
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_gail_seals_half_cheetah_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_gail_seals_hopper_best_hp_eval.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4966329966329966%*

 * *Differences: {"'algorithm_kwargs'": "{'demo_batch_size': 128, 'gen_replay_buffer_capacity': 4096}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Hopper-v0')])",*

 * * "'policy'": "OrderedDict([('policy_cls', 'MlpPolicy'), ('policy_kwargs', "*

 * *             "OrderedDict([('activation_fn', OrderedDict([('py/type', "*

 * *             "'torch.nn.modules.activation.ReLU')])), ('features_extractor_class', "*

 * *             "OrderedDict([('py/type', 'imitation.polici […]*

```diff
@@ -1,19 +1,52 @@
 {
     "algorithm_kwargs": {
-        "demo_batch_size": 8192,
-        "gen_replay_buffer_capacity": 512,
+        "demo_batch_size": 128,
+        "gen_replay_buffer_capacity": 4096,
         "n_disc_updates_per_round": 8
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/HalfCheetah-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Hopper-v0"
+    },
+    "policy": {
+        "policy_cls": "MlpPolicy",
+        "policy_kwargs": {
+            "activation_fn": {
+                "py/type": "torch.nn.modules.activation.ReLU"
+            },
+            "features_extractor_class": {
+                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
+            },
+            "features_extractor_kwargs": {
+                "normalize_class": {
+                    "py/type": "imitation.util.networks.RunningNorm"
+                }
+            },
+            "net_arch": [
+                {
+                    "pi": [
+                        64,
+                        64
+                    ],
+                    "vf": [
+                        64,
+                        64
+                    ]
+                }
+            ]
+        }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     },
     "reward": {
         "add_std_alpha": null,
         "ensemble_size": null,
         "net_cls": {
             "py/type": "imitation.rewards.reward_nets.BasicRewardNet"
         },
@@ -28,36 +61,20 @@
     },
     "rl": {
         "batch_size": 4096,
         "rl_cls": {
             "py/type": "stable_baselines3.ppo.ppo.PPO"
         },
         "rl_kwargs": {
-            "batch_size": 64,
+            "batch_size": 512,
             "clip_range": 0.1,
-            "ent_coef": 3.992371122209408e-06,
-            "gae_lambda": 0.95,
-            "gamma": 0.95,
-            "learning_rate": 0.00026250519057717037,
-            "max_grad_norm": 0.8,
-            "n_epochs": 5,
-            "vf_coef": 0.11483689492120866
+            "ent_coef": 0.001255299425412744,
+            "gae_lambda": 0.98,
+            "gamma": 0.995,
+            "learning_rate": 4.3984856156897565e-05,
+            "max_grad_norm": 0.9,
+            "n_epochs": 20,
+            "vf_coef": 0.20315938606555833
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
-        "policy_cls": {
-            "py/type": "imitation.policies.base.FeedForward32Policy"
-        },
-        "policy_kwargs": {
-            "features_extractor_class": {
-                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
-            },
-            "features_extractor_kwargs": {
-                "normalize_class": {
-                    "py/type": "imitation.util.networks.RunningNorm"
-                }
-            }
-        }
-    }
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_gail_seals_hopper_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_airl_seals_hopper_best_hp_eval.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48173400673400674%*

 * *Differences: {"'algorithm_kwargs'": "{'demo_batch_size': 2048, 'gen_replay_buffer_capacity': 8192, "*

 * *                       "'n_disc_updates_per_round': 16}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Hopper-v0')])",*

 * * "'policy'": "OrderedDict([('policy_cls', 'MlpPolicy'), ('policy_kwargs', "*

 * *             "OrderedDict([('activation_fn', OrderedDict([('py/type', "*

 * *             "'torch.nn.modules.activation.ReLU')])), ('features_extractor_class', […]*

```diff
@@ -1,76 +1,80 @@
 {
     "algorithm_kwargs": {
-        "demo_batch_size": 128,
-        "gen_replay_buffer_capacity": 4096,
-        "n_disc_updates_per_round": 8
+        "demo_batch_size": 2048,
+        "gen_replay_buffer_capacity": 8192,
+        "n_disc_updates_per_round": 16
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Hopper-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Hopper-v0"
+    },
+    "policy": {
+        "policy_cls": "MlpPolicy",
+        "policy_kwargs": {
+            "activation_fn": {
+                "py/type": "torch.nn.modules.activation.ReLU"
+            },
+            "features_extractor_class": {
+                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
+            },
+            "features_extractor_kwargs": {
+                "normalize_class": {
+                    "py/type": "imitation.util.networks.RunningNorm"
+                }
+            },
+            "net_arch": [
+                {
+                    "pi": [
+                        64,
+                        64
+                    ],
+                    "vf": [
+                        64,
+                        64
+                    ]
+                }
+            ]
+        }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
     },
     "reward": {
         "add_std_alpha": null,
         "ensemble_size": null,
         "net_cls": {
-            "py/type": "imitation.rewards.reward_nets.BasicRewardNet"
+            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
         },
         "net_kwargs": {
             "normalize_input_layer": {
                 "py/type": "imitation.util.networks.RunningNorm"
             }
         },
         "normalize_output_layer": {
             "py/type": "imitation.util.networks.RunningNorm"
         }
     },
     "rl": {
-        "batch_size": 4096,
+        "batch_size": 8192,
         "rl_cls": {
             "py/type": "stable_baselines3.ppo.ppo.PPO"
         },
         "rl_kwargs": {
             "batch_size": 512,
             "clip_range": 0.1,
-            "ent_coef": 0.001255299425412744,
+            "ent_coef": 0.009709494745755033,
             "gae_lambda": 0.98,
             "gamma": 0.995,
-            "learning_rate": 4.3984856156897565e-05,
+            "learning_rate": 0.0005807211840258373,
             "max_grad_norm": 0.9,
             "n_epochs": 20,
             "vf_coef": 0.20315938606555833
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
-        "policy_cls": "MlpPolicy",
-        "policy_kwargs": {
-            "activation_fn": {
-                "py/type": "torch.nn.modules.activation.ReLU"
-            },
-            "features_extractor_class": {
-                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
-            },
-            "features_extractor_kwargs": {
-                "normalize_class": {
-                    "py/type": "imitation.util.networks.RunningNorm"
-                }
-            },
-            "net_arch": [
-                {
-                    "pi": [
-                        64,
-                        64
-                    ],
-                    "vf": [
-                        64,
-                        64
-                    ]
-                }
-            ]
-        }
-    }
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_gail_seals_swimmer_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_gail_seals_swimmer_best_hp_eval.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5416666666666666%*

 * *Differences: {"'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Swimmer-v0')])",*

 * * "'expert'": "{'loader_kwargs': {'gym_id': 'seals/Swimmer-v0', delete: ['env_name']}}",*

 * * "'policy'": "OrderedDict([('policy_cls', 'MlpPolicy'), ('policy_kwargs', "*

 * *             "OrderedDict([('activation_fn', OrderedDict([('py/type', "*

 * *             "'torch.nn.modules.activation.ReLU')])), ('features_extractor_class', "*

 * *             "OrderedDict([('py/type', 'imitation.poli […]*

```diff
@@ -1,26 +1,59 @@
 {
     "algorithm_kwargs": {
         "demo_batch_size": 32,
         "gen_replay_buffer_capacity": 4096,
         "n_disc_updates_per_round": 16
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Swimmer-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Swimmer-v0"
     },
     "expert": {
         "loader_kwargs": {
-            "env_name": "seals/Swimmer-v0",
+            "gym_id": "seals/Swimmer-v0",
             "organization": "HumanCompatibleAI"
         }
     },
+    "policy": {
+        "policy_cls": "MlpPolicy",
+        "policy_kwargs": {
+            "activation_fn": {
+                "py/type": "torch.nn.modules.activation.ReLU"
+            },
+            "features_extractor_class": {
+                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
+            },
+            "features_extractor_kwargs": {
+                "normalize_class": {
+                    "py/type": "imitation.util.networks.RunningNorm"
+                }
+            },
+            "net_arch": [
+                {
+                    "pi": [
+                        64,
+                        64
+                    ],
+                    "vf": [
+                        64,
+                        64
+                    ]
+                }
+            ]
+        }
+    },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
+    },
     "reward": {
         "add_std_alpha": null,
         "ensemble_size": null,
         "net_cls": {
             "py/type": "imitation.rewards.reward_nets.BasicRewardNet"
         },
         "net_kwargs": {
@@ -45,38 +78,9 @@
             "gamma": 0.999,
             "learning_rate": 2.0190030388504567e-05,
             "max_grad_norm": 2,
             "n_epochs": 5,
             "vf_coef": 0.6162112311062333
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
-        "policy_cls": "MlpPolicy",
-        "policy_kwargs": {
-            "activation_fn": {
-                "py/type": "torch.nn.modules.activation.ReLU"
-            },
-            "features_extractor_class": {
-                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
-            },
-            "features_extractor_kwargs": {
-                "normalize_class": {
-                    "py/type": "imitation.util.networks.RunningNorm"
-                }
-            },
-            "net_arch": [
-                {
-                    "pi": [
-                        64,
-                        64
-                    ],
-                    "vf": [
-                        64,
-                        64
-                    ]
-                }
-            ]
-        }
-    }
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/example_gail_seals_walker_best_hp_eval.json` & `imitation-0.4.0/benchmarking/example_airl_seals_ant_best_hp_eval.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4458333333333333%*

 * *Differences: {"'algorithm_kwargs'": "{'demo_batch_size': 8192, 'gen_replay_buffer_capacity': 8192}",*

 * * "'demonstrations'": "{'source': 'huggingface', 'algo_name': 'ppo'}",*

 * * "'environment'": "OrderedDict([('gym_id', 'seals/Ant-v0')])",*

 * * "'policy'": "OrderedDict([('policy_cls', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.FeedForward32Policy')])), ('policy_kwargs', "*

 * *             "OrderedDict([('features_extractor_class', OrderedDict([('py/type', "*

 * *             "'imitation.policies.base.NormalizeFeatur […]*

```diff
@@ -1,82 +1,67 @@
 {
     "algorithm_kwargs": {
-        "demo_batch_size": 512,
-        "gen_replay_buffer_capacity": 16384,
+        "demo_batch_size": 8192,
+        "gen_replay_buffer_capacity": 8192,
         "n_disc_updates_per_round": 16
     },
     "checkpoint_interval": 0,
-    "common": {
-        "env_name": "seals/Walker2d-v0"
-    },
     "demonstrations": {
-        "n_expert_demos": null
-    },
-    "expert": {
-        "loader_kwargs": {
-            "env_name": "seals/Walker2d-v0",
-            "organization": "HumanCompatibleAI"
+        "algo_name": "ppo",
+        "n_expert_demos": null,
+        "source": "huggingface"
+    },
+    "environment": {
+        "gym_id": "seals/Ant-v0"
+    },
+    "policy": {
+        "policy_cls": {
+            "py/type": "imitation.policies.base.FeedForward32Policy"
+        },
+        "policy_kwargs": {
+            "features_extractor_class": {
+                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
+            },
+            "features_extractor_kwargs": {
+                "normalize_class": {
+                    "py/type": "imitation.util.networks.RunningNorm"
+                }
+            }
         }
     },
+    "policy_evaluation": {
+        "n_episodes_eval": 50
+    },
     "reward": {
         "add_std_alpha": null,
         "ensemble_size": null,
         "net_cls": {
-            "py/type": "imitation.rewards.reward_nets.BasicRewardNet"
+            "py/type": "imitation.rewards.reward_nets.BasicShapedRewardNet"
         },
         "net_kwargs": {
             "normalize_input_layer": {
                 "py/type": "imitation.util.networks.RunningNorm"
             }
         },
         "normalize_output_layer": {
             "py/type": "imitation.util.networks.RunningNorm"
         }
     },
     "rl": {
-        "batch_size": 16384,
+        "batch_size": 8192,
         "rl_cls": {
             "py/type": "stable_baselines3.ppo.ppo.PPO"
         },
         "rl_kwargs": {
-            "batch_size": 128,
-            "clip_range": 0.4,
-            "ent_coef": 0.0007566389899529574,
-            "gae_lambda": 0.92,
-            "gamma": 0.98,
-            "learning_rate": 1.943992487657563e-05,
-            "max_grad_norm": 0.6,
-            "n_epochs": 20,
-            "vf_coef": 0.6167177795726859
+            "batch_size": 16,
+            "clip_range": 0.3,
+            "ent_coef": 3.27750078482474e-06,
+            "gae_lambda": 0.8,
+            "gamma": 0.995,
+            "learning_rate": 3.249429831179079e-05,
+            "max_grad_norm": 0.9,
+            "n_epochs": 10,
+            "vf_coef": 0.4351450387648799
         }
     },
-    "total_timesteps": 10000000.0,
-    "train": {
-        "n_episodes_eval": 50,
-        "policy_cls": "MlpPolicy",
-        "policy_kwargs": {
-            "activation_fn": {
-                "py/type": "torch.nn.modules.activation.ReLU"
-            },
-            "features_extractor_class": {
-                "py/type": "imitation.policies.base.NormalizeFeaturesExtractor"
-            },
-            "features_extractor_kwargs": {
-                "normalize_class": {
-                    "py/type": "imitation.util.networks.RunningNorm"
-                }
-            },
-            "net_arch": [
-                {
-                    "pi": [
-                        64,
-                        64
-                    ],
-                    "vf": [
-                        64,
-                        64
-                    ]
-                }
-            ]
-        }
-    }
+    "total_timesteps": 10000000
 }
```

### Comparing `imitation-0.3.2/benchmarking/util.py` & `imitation-0.4.0/benchmarking/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
     import json
 
     with open(file) as f:
         config = json.load(f)
     # remove key 'agent_path'
     config.pop("agent_path")
     config.pop("seed")
-    config.get("demonstrations", {}).pop("rollout_path")
+    config.get("demonstrations", {}).pop("path")
     config.get("expert", {}).get("loader_kwargs", {}).pop("path", None)
-    env_name = config.pop("common").pop("env_name")
-    config["common"] = {"env_name": env_name}
+    env_name = config.pop("environment").pop("gym_id")
+    config["environment"] = {"gym_id": env_name}
     config.pop("show_config", None)
 
     remove_empty_dicts(config)
     # files are of the format
     # /path/to/file/example_<algo>_<env>_best_hp_eval/<other_info>/sacred/1/config.json
     # we want to write to /<write_path>/<algo>_<env>.json
     with open(write_path / f"{file.parents[3].name}.json", "w") as f:
```

### Comparing `imitation-0.3.2/ci/Xdummy-entrypoint.py` & `imitation-0.4.0/ci/Xdummy-entrypoint.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/ci/check_typeignore.py` & `imitation-0.4.0/ci/check_typeignore.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/ci/clean_notebooks.py` & `imitation-0.4.0/ci/clean_notebooks.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/ci/xorg.conf` & `imitation-0.4.0/ci/xorg.conf`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/Makefile` & `imitation-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/_templates/autosummary/class.rst` & `imitation-0.4.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/_templates/autosummary/module.rst` & `imitation-0.4.0/docs/_templates/autosummary/module.rst`

 * *Files 22% similar despite different names*

```diff
@@ -18,20 +18,14 @@
    .. rubric:: {{ _('Functions') }}
    .. testsetup::
       :skipif: skip_doctests
 
       # import all functions from module since examples don't import them
       from {{ fullname }} import *
 
-   .. doctest::
-
-      # empty test needed in case the module has no example usage.
-      # otherwise, testsetup throws an error
-      pass
-
    .. autosummary::
    {% for item in functions %}
       {{ item }}
    {%- endfor %}
    {% endif %}
    {% endblock %}
```

### Comparing `imitation-0.3.2/docs/algorithms/airl.rst` & `imitation-0.4.0/docs/algorithms/airl.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 `AIRL <https://arxiv.org/abs/1710.11248>`_, similar to :ref:`GAIL <gail docs>`,
 adversarially trains a policy against a discriminator that aims to distinguish the expert
 demonstrations from the learned policy. Unlike GAIL, AIRL recovers a reward function
 that is more generalizable to changes in environment dynamics.
 
 The expert policy must be stochastic.
 
-Notes
------
-- AIRL paper: `Learning Robust Rewards with Adversarial Inverse Reinforcement Learning <https://arxiv.org/abs/1710.11248>`_
+
+.. note::
+    AIRL paper: `Learning Robust Rewards with Adversarial Inverse Reinforcement Learning <https://arxiv.org/abs/1710.11248>`_
 
 Example
 =======
 
 Detailed example notebook: :doc:`../tutorials/4_train_airl`
 
 .. testcode::
```

### Comparing `imitation-0.3.2/docs/algorithms/bc.rst` & `imitation-0.4.0/docs/algorithms/bc.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/algorithms/dagger.rst` & `imitation-0.4.0/docs/algorithms/dagger.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 policy using supervised learning on a dataset of observation-action pairs from expert demonstrations
 (like :ref:`behavioral cloning <behavioral cloning docs>`), runs the policy to gather
 observations, queries the expert for good actions on those observations, and adds the
 newly labeled observations to the dataset. DAgger improves on behavioral cloning by
 training on a dataset that better resembles the observations the trained policy is
 likely to encounter, but it requires querying the expert online.
 
-Notes
------
-- DAgger paper: `A Reduction of Imitation Learning and Structured Prediction to No-Regret Online Learning <https://arxiv.org/abs/1011.0686>`_
+.. note::
+    DAgger paper: `A Reduction of Imitation Learning and Structured Prediction to No-Regret Online Learning <https://arxiv.org/abs/1011.0686>`_
 
 Example
 =======
 
 Detailed example notebook: :doc:`../tutorials/2_train_dagger`
 
 .. testcode::
```

### Comparing `imitation-0.3.2/docs/algorithms/gail.rst` & `imitation-0.4.0/docs/algorithms/gail.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 Generative Adversarial Imitation Learning (GAIL)
 ================================================
 
 `GAIL <https://arxiv.org/abs/1606.03476>`_ learns a policy by simultaneously training it
 with a discriminator that aims to distinguish expert trajectories against
 trajectories from the learned policy.
 
-Notes
------
-- GAIL paper: `Generative Adversarial Imitation Learning <https://arxiv.org/abs/1606.03476>`_
+.. note::
+    GAIL paper: `Generative Adversarial Imitation Learning <https://arxiv.org/abs/1606.03476>`_
 
 Example
 =======
 
 Detailed example notebook: :doc:`../tutorials/3_train_gail`
 
 .. testcode::
```

### Comparing `imitation-0.3.2/docs/algorithms/mce_irl.rst` & `imitation-0.4.0/docs/algorithms/mce_irl.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/algorithms/preference_comparisons.rst` & `imitation-0.4.0/docs/algorithms/preference_comparisons.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 .. _preference comparisons docs:
 
 ======================
-Preference comparisons
+Preference Comparisons
 ======================
 
 The preference comparison algorithm learns a reward function from preferences between pairs of trajectories.
 The comparisons are modeled as being generated from a Bradley-Terry (or Boltzmann rational) model,
 where the probability of preferring trajectory A over B is proportional to the exponential of the
 difference between the return of trajectory A minus B. In other words, the difference in returns forms a logit
 for a binary classification problem, and accordingly the reward function is trained using a cross-entropy loss
 to predict the preference comparison.
 
-Notes
------
-- Our implementation is based on the  `Deep Reinforcement Learning from Human Preferences <https://arxiv.org/pdf/1706.03741.pdf>`_ algorithm.
-
-- An ensemble of reward networks can also be trained instead of a single network. The uncertainty in the preference between the member networks can be used to actively select preference queries.
+.. note::
+    - Our implementation is based on the  `Deep Reinforcement Learning from Human Preferences <https://arxiv.org/pdf/1706.03741.pdf>`_ algorithm.
+    - An ensemble of reward networks can also be trained instead of a single network. The uncertainty in the preference between the member networks can be used to actively select preference queries.
 
 Example
 =======
 
 Detailed example notebook: :doc:`../tutorials/5_train_preference_comparisons`
 
 .. testcode::
```

### Comparing `imitation-0.3.2/docs/conf.py` & `imitation-0.4.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 napoleon_numpy_docstring = False
 autosummary_generate = True
 
 nb_execution_mode = os.getenv("NB_EXECUTION_MODE", "cache")
 nb_execution_timeout = 120
 nb_merge_streams = True
 nb_output_stderr = "remove"
+# Enable LaTeX macros in markdown cells
+myst_enable_extensions = [
+    "amsmath",
+    "dollarmath",
+]
 
 # skip_doctests is checked in our :skipif: directives in doctest examples
 doctest_global_setup = """
 import os
 
 skip_doctests = os.getenv("SKIP_DOCTEST")
 """
```

### Comparing `imitation-0.3.2/docs/development/contributing/code-of-conduct.rst` & `imitation-0.4.0/docs/development/contributing/code-of-conduct.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/development/contributing/index.rst` & `imitation-0.4.0/docs/development/contributing/index.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/development/contributing/ways-to-contribute.rst` & `imitation-0.4.0/docs/development/contributing/ways-to-contribute.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/development/developer.rst` & `imitation-0.4.0/docs/development/developer.rst`

 * *Files 6% similar despite different names*

```diff
@@ -97,33 +97,37 @@
   The default reward function of the environment is overridden with the passed reward function,
   and the original rewards are stored in the ``info_dict`` with the ``original_env_rew`` key.
   This class is used to override the original reward function of an environment with a learned
   reward function from the reward learning algorithms like preference comparisons.
 
 The ``imitation.rewards.serialize`` module contains functions to load serialized reward functions.
 
+For more see the :ref:`Reward Networks Tutorial <reward-net docs>`.
+
 Scripts
 -------
 
 We use Sacred to provide a command-line interface to run the experiments. The scripts to run the end-to-end experiments are
 available in ``scripts/``. You can take a look at the following doc links to understand how to use Sacred:
 
 - `Experiment Overview <https://sacred.readthedocs.io/en/stable/experiment.html>`_: Explains how to create and run experiments. Each script, defined in ``scripts/``, has a corresponding experiment object, defined in ``scripts/config``, with the experiment object and Python source files named after the algorithm(s) supported. For example, the ``train_rl_ex`` object is defined in ``scripts.config.train_rl`` and its main function is in ``scripts.train_rl``.
 
-- `Ingredients <https://sacred.readthedocs.io/en/stable/ingredients.html>`_: Explains how to use ingredients to avoid code duplication across experiments. The ingredients used in our experiments are defined in ``scripts/common/``:
+- `Ingredients <https://sacred.readthedocs.io/en/stable/ingredients.html>`_: Explains how to use ingredients to avoid code duplication across experiments. The ingredients used in our experiments are defined in ``scripts/ingredients/``:
 
   .. autosummary::
-    imitation.scripts.common.common
-    imitation.scripts.common.demonstrations
-    imitation.scripts.common.reward
-    imitation.scripts.common.rl
-    imitation.scripts.common.train
-    imitation.scripts.common.wb
+    imitation.scripts.ingredients.logging
+    imitation.scripts.ingredients.demonstrations
+    imitation.scripts.ingredients.environment
+    imitation.scripts.ingredients.expert
+    imitation.scripts.ingredients.reward
+    imitation.scripts.ingredients.rl
+    imitation.scripts.ingredients.policy
+    imitation.scripts.ingredients.wb
 
-- `Configurations <https://sacred.readthedocs.io/en/stable/configuration.html>`_: Explains how to use configurations to parametrize runs. The configurations for different algorithms are defined in their file in ``scripts/``. Some of the commonly used configs and ingredients used across algorithms are defined in ``scripts/common/``.
+- `Configurations <https://sacred.readthedocs.io/en/stable/configuration.html>`_: Explains how to use configurations to parametrize runs. The configurations for different algorithms are defined in their file in ``scripts/``. Some of the commonly used configs and ingredients used across algorithms are defined in ``scripts/ingredients/``.
 
 - `Command-Line Interface <https://sacred.readthedocs.io/en/stable/command_line.html>`_: Explains how to run the experiments through the command-line interface. Also, note the section on how to `print configs <https://sacred.readthedocs.io/en/stable/command_line.html#print-config>`_ to verify the configurations used for the run.
 
 - `Controlling Randomness <https://sacred.readthedocs.io/en/stable/randomness.html>`_: Explains how to control randomness by seeding experiments through Sacred.
 
 Util
 ----
```

### Comparing `imitation-0.3.2/docs/experts/loading-experts.rst` & `imitation-0.4.0/docs/main-concepts/experts.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-===============
-Loading Experts
-===============
+=======
+Experts
+=======
 
 The algorithms in the imitation library are all about learning from some kind of
 expert.
 In many cases this expert is a piece of software itself.
 The `imitation` library natively supports experts trained using the
 `stable-baselines3 <https://github.com/DLR-RM/stable-baselines3>`_ reinforcement
 learning library.
@@ -22,19 +22,20 @@
 
 The Python interface provides a :func:`~imitation.policies.serialize.load_policy`
 function to which you pass a `policy_type`, a VecEnv and any extra kwargs to pass to the
 corresponding policy loader.
 
 .. code-block:: python
 
+    import numpy as np
     from imitation.policies.serialize import load_policy
     from imitation.util import util
 
-    venv = util.make_vec_env("your-env", n_envs=4)
-    local_policy = load_policy("ppo", venv, loader_kwargs={"path": "path/to/model.zip"})
+    venv = util.make_vec_env("your-env", n_envs=4, rng=np.random.default_rng())
+    local_policy = load_policy("ppo", venv, path="path/to/model.zip")
 
 To load a policy from disk, use either `ppo` or `sac` as the policy type.
 The path is specified by `path` in the `loader_kwargs` and it should either point
 to a zip file containing the policy or a directory containing a `model.zip` file that
 was created by stable-baselines3.
 
 In the command line interface the `expert.policy_type` and `expert.loader_kwargs`
@@ -57,23 +58,23 @@
 By default, the policies are loaded from the
 `HumanCompatibleAI organization <https://huggingface.co/HumanCompatibleAI>`_, but you
 can override this by setting the `organization` parameter in the `loader_kwargs`.
 When using the Python API, you also have to specify the environment name as `env_name`.
 
 .. code-block:: python
 
+    import numpy as np
     from imitation.policies.serialize import load_policy
     from imitation.util import util
 
-    venv = util.make_vec_env("your-env", n_envs=4)
+    venv = util.make_vec_env("your-env", n_envs=4, rng=np.random.default_rng())
     remote_policy = load_policy(
         "ppo-huggingface",
-        loader_kwargs=dict(
-            organization="your-org",
-            env_name="your-env"
+        organization="your-org",
+        env_name="your-env"
         )
     )
 
 In the command line interface, the `env-name` is automatically injected into the
 `loader_kwargs` and does not need to be defined explicitly.
 In this example, to train AIRL on a PPO expert that was loaded from `your-org` on
 HuggingFace:
```

### Comparing `imitation-0.3.2/docs/getting-started/first-steps.rst` & `imitation-0.4.0/docs/getting-started/first_steps.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/getting-started/installation.rst` & `imitation-0.4.0/docs/getting-started/installation.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/getting-started/variable-horizon.rst` & `imitation-0.4.0/docs/main-concepts/variable_horizon.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 ================================================
 Limitations on Horizon Length
 ================================================
 
-Variable Horizon Environments Considered Harmful
-================================================
+.. warning:: Variable Horizon Environments Considered Harmful
+
 
 Reinforcement learning (RL) algorithms are commonly trained and evaluated in *variable horizon* environments.
 In these environments, the episode ends when some termination condition is reached (rather than after a fixed number of steps).
 This typically corresponds to success, such as reaching the top of the mountain in ``MountainCar``, or to failure, such as the pole falling down in ``CartPole``.
 A variable horizon will tend to speed up RL training, by increasing the proportion of samples where the agent's actions still have a meaningful impact on the reward, pruning out states that are already a foregone conclusion.
 
 However, termination conditions must be carefully hand-designed for each environment.
```

### Comparing `imitation-0.3.2/docs/getting-started/what-is-imitation.rst` & `imitation-0.4.0/docs/getting-started/what_is_imitation.rst`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/index.rst` & `imitation-0.4.0/docs/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-.. imitation documentation master file, created by
-   sphinx-quickstart on Wed Jun 26 10:19:27 2019.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
 =========
 Imitation
 =========
 
 **Imitation provides clean implementations of imitation and reward learning algorithms**, under a unified and user-friendly API.
 Currently, we have implementations of Behavioral Cloning, `DAgger <https://arxiv.org/pdf/1011.0686.pdf>`_
 (with synthetic examples), density-based reward modeling, `Maximum Causal Entropy Inverse Reinforcement Learning <https://www.cs.cmu.edu/~bziebart/publications/maximum-causal-entropy.pdf>`_,
@@ -23,24 +18,50 @@
 - Built on and compatible with Stable Baselines 3 (SB3).
 - Modular Pytorch implementations of Behavioral Cloning, DAgger, GAIL, and AIRL that can
   train arbitrary SB3 policies.
 - GAIL and AIRL have customizable reward and discriminator networks.
 - Scripts to train policies using SB3 and save rollouts from these policies as synthetic "expert" demonstrations.
 - Data structures and scripts for loading and storing expert demonstrations.
 
+Citing imitation
+~~~~~~~~~~~~~~~~
+
+If you use ``imitation`` in your research project, please cite our paper to help us track our impact and enable readers to more easily replicate your results. You may use the following BibTeX::
+
+    @misc{gleave2022imitation,
+      author = {Gleave, Adam and Taufeeque, Mohammad and Rocamonde, Juan and Jenner, Erik and Wang, Steven H. and Toyer, Sam and Ernestus, Maximilian and Belrose, Nora and Emmons, Scott and Russell, Stuart},
+      title = {imitation: Clean Imitation Learning Implementations},
+      year = {2022},
+      howPublished = {arXiv:2211.11972v1 [cs.LG]},
+      archivePrefix = {arXiv},
+      eprint = {2211.11972},
+      primaryClass = {cs.LG},
+      url = {https://arxiv.org/abs/2211.11972},
+    }
 
 .. toctree::
    :maxdepth: 2
    :caption: Getting Started
    :hidden:
 
+   getting-started/what_is_imitation
    getting-started/installation
-   getting-started/what-is-imitation
-   getting-started/variable-horizon
-   getting-started/first-steps
+   getting-started/first_steps
+   getting-started/cli
+
+.. toctree::
+    :maxdepth: 2
+    :caption: Main Concepts
+    :hidden:
+
+    main-concepts/experts
+    main-concepts/trajectories
+    main-concepts/reward_networks
+    main-concepts/variable_horizon
+
 
 .. toctree::
    :maxdepth: 2
    :caption: Algorithms
    :hidden:
 
    algorithms/bc
@@ -60,22 +81,16 @@
    tutorials/2_train_dagger
    tutorials/3_train_gail
    tutorials/4_train_airl
    tutorials/5_train_preference_comparisons
    tutorials/5a_train_preference_comparisons_with_cnn
    tutorials/6_train_mce
    tutorials/7_train_density
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Experts
-   :hidden:
-
-   experts/loading-experts
-
+   tutorials/8_train_custom_env
+   tutorials/9_compare_baselines
 
 API Reference
 ~~~~~~~~~~~~~
 
 .. autosummary::
    :toctree: _api
    :caption: API Reference
```

### Comparing `imitation-0.3.2/docs/make.bat` & `imitation-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/tutorials/1_train_bc.ipynb` & `imitation-0.4.0/docs/tutorials/1_train_bc.ipynb`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/tutorials/2_train_dagger.ipynb` & `imitation-0.4.0/docs/tutorials/2_train_dagger.ipynb`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/tutorials/3_train_gail.ipynb` & `imitation-0.4.0/docs/tutorials/3_train_gail.ipynb`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/tutorials/4_train_airl.ipynb` & `imitation-0.4.0/docs/tutorials/4_train_airl.ipynb`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/docs/tutorials/5_train_preference_comparisons.ipynb` & `imitation-0.4.0/docs/tutorials/5_train_preference_comparisons.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995454545454545%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(3, 'learned_reward_venv = RewardVecEnvWrapper(venv, "*

 * *            "reward_net.predict_processed)')], delete: [3]}}}"}*

```diff
@@ -123,15 +123,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from imitation.rewards.reward_wrapper import RewardVecEnvWrapper\n",
                 "\n",
                 "\n",
-                "learned_reward_venv = RewardVecEnvWrapper(venv, reward_net.predict)"
+                "learned_reward_venv = RewardVecEnvWrapper(venv, reward_net.predict_processed)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we can train an agent, that only sees those learned reward."
```

### Comparing `imitation-0.3.2/docs/tutorials/5a_train_preference_comparisons_with_cnn.ipynb` & `imitation-0.4.0/docs/tutorials/5a_train_preference_comparisons_with_cnn.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993884952766532%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(14, '\\n'), (15, '# GOTCHA: When using the "*

 * *            "NormalizedRewardNet wrapper, you should deactivate updating\\n'), (16, '# during "*

 * *            "evaluation by passing update_stats=False to the predict_processed method.\\n'), (17, "*

 * *            "'learned_reward_venv = RewardVecEnvWrapper(venv, "*

 * *            "shaped_reward_net.predict_processed)')], delete: [14]}}, 11: {'source': {insert: [(0, "*

 * *            "'## Generating rollouts\\n')], delete: [0]}}}"}*

```diff
@@ -161,15 +161,18 @@
                 "\n",
                 "\n",
                 "shaped_reward_net = ShapedRewardNet(\n",
                 "    base=reward_net,\n",
                 "    potential=value_potential,\n",
                 "    discount_factor=0.99,\n",
                 ")\n",
-                "learned_reward_venv = RewardVecEnvWrapper(venv, shaped_reward_net.predict)"
+                "\n",
+                "# GOTCHA: When using the NormalizedRewardNet wrapper, you should deactivate updating\n",
+                "# during evaluation by passing update_stats=False to the predict_processed method.\n",
+                "learned_reward_venv = RewardVecEnvWrapper(venv, shaped_reward_net.predict_processed)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "41efea37",
             "metadata": {},
             "source": [
@@ -218,15 +221,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "hZ9um7u1V0h1",
             "metadata": {},
             "source": [
-                "# Generating rollouts\n",
+                "## Generating rollouts\n",
                 "When generating rollouts in image environments, be sure to use the agent's get_env() function rather than using the original environment.\n",
                 "\n",
                 "The learner re-arranges the observations space to put the channel environment in the first dimension, and get_env() will correctly provide a wrapped environment doing this.\n",
                 "\n"
             ]
         },
         {
```

### Comparing `imitation-0.3.2/docs/tutorials/6_train_mce.ipynb` & `imitation-0.4.0/docs/tutorials/6_train_mce.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999285714285715%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(17, 'env_creator = partial(CliffWorldEnv, height=4, "*

 * *            "horizon=40, width=7, use_xy_obs=True)\\n')], delete: [17]}}}"}*

```diff
@@ -36,15 +36,15 @@
                 "    mce_occupancy_measures,\n",
                 "    mce_partition_fh,\n",
                 "    TabularPolicy,\n",
                 ")\n",
                 "from imitation.data import rollout\n",
                 "from imitation.rewards import reward_nets\n",
                 "\n",
-                "env_creator = partial(CliffWorldEnv, height=4, horizon=8, width=7, use_xy_obs=True)\n",
+                "env_creator = partial(CliffWorldEnv, height=4, horizon=40, width=7, use_xy_obs=True)\n",
                 "env_single = env_creator()\n",
                 "\n",
                 "state_env_creator = lambda: base_envs.ExposePOMDPStateWrapper(env_creator())\n",
                 "\n",
                 "# This is just a vectorized environment because `generate_trajectories` expects one\n",
                 "state_venv = DummyVecEnv([state_env_creator] * 4)"
             ]
```

### Comparing `imitation-0.3.2/docs/tutorials/7_train_density.ipynb` & `imitation-0.4.0/docs/tutorials/7_train_density.ipynb`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/examples/quickstart.py` & `imitation-0.4.0/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/experiments/README.md` & `imitation-0.4.0/experiments/README.md`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/experiments/bc_benchmark.sh` & `imitation-0.4.0/experiments/bc_benchmark.sh`

 * *Files 6% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 eval set -- "$TEMP"
 
 while true; do
   case "$1" in
     -f | --fast)
       # Fast mode (debug)
       SEEDS=(0)
-      extra_configs=("${extra_configs[@]}" common.fast demonstrations.fast train.fast fast)
+      extra_configs=("${extra_configs[@]}" environment.fast demonstrations.fast policy_evaluation.fast fast)
       shift
       ;;
     --paper)  # Table benchmark settings
       ENVS=(seals_cartpole seals_mountain_car seals_half_cheetah)
       shift
       ;;
     -w | --wandb)
-      # activate wandb logging by adding 'wandb' format string to common.log_format_strs
-      extra_configs=("${extra_configs[@]}" "common.wandb_logging")
+      # activate wandb logging by adding 'wandb' format string to logging.log_format_strs
+      extra_configs=("${extra_configs[@]}" "logging.wandb_logging")
       shift
       ;;
     --run_name)
       extra_options=("${extra_options[@]}" --name "$2")
       shift 2
       ;;
     -T | --tmux)
@@ -66,10 +66,10 @@
   --capture=sys \
   "${extra_options[@]}" \
   bc \
   with \
   '{env_config_name}' \
   "${extra_configs[@]}" \
   'seed={seed}' \
-  common.log_root="${OUTPUT_DIR}" \
+  logging.log_root="${OUTPUT_DIR}" \
   ::: env_config_name "${ENVS[@]}" \
   ::: seed "${SEEDS[@]}"
```

### Comparing `imitation-0.3.2/experiments/benchmark_and_table.sh` & `imitation-0.4.0/experiments/benchmark_and_table.sh`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/experiments/common.sh` & `imitation-0.4.0/experiments/common.sh`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/experiments/convert_traj.py` & `imitation-0.4.0/experiments/convert_traj.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import argparse
 import os
 from pathlib import Path
 from typing import Sequence
 
 import numpy as np
 
-from imitation.data import rollout, types
+from imitation.data import rollout, serialize, types
 
 
 def convert_trajs_to_sb(trajs: Sequence[types.TrajectoryWithRew]) -> dict:
     """Converts Trajectories into the dict format used by Stable Baselines GAIL."""
     trans = rollout.flatten_trajectories_with_rew(trajs)
     return dict(
         acs=trans.acts,
@@ -28,15 +28,15 @@
     parser.add_argument("dst_path", type=str)
     args = parser.parse_args()
 
     src_path = Path(args.src_path)
     dst_path = Path(args.dst_path)
 
     assert src_path.is_file()
-    src_trajs = types.load_with_rewards(src_path)
+    src_trajs = serialize.load_with_rewards(src_path)
     dst_trajs = convert_trajs_to_sb(src_trajs)
     os.makedirs(dst_path.parent, exist_ok=True)
     with open(dst_path, "wb") as f:
         np.savez_compressed(f, **dst_trajs)
 
     print(f"Dumped rollouts to {dst_path}")
```

### Comparing `imitation-0.3.2/experiments/dagger_benchmark.sh` & `imitation-0.4.0/experiments/dagger_benchmark.sh`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 eval set -- "$TEMP"
 
 while true; do
   case "$1" in
     # Fast mode (debug)
     -f | --fast)
       SEEDS=(0)
-      extra_configs=("${extra_configs[@]}" common.fast demonstrations.fast train.fast fast)
+      extra_configs=("${extra_configs[@]}" environment.fast demonstrations.fast policy_evaluation.fast fast)
       shift
       ;;
     --paper)  # Table benchmark settings
       ENVS=(seals_cartpole seals_mountain_car seals_half_cheetah)
       shift
       ;;
     -w | --wandb)
-      # activate wandb logging by adding 'wandb' format string to common.log_format_strs
-      extra_configs=("${extra_configs[@]}" "common.wandb_logging")
+      # activate wandb logging by adding 'wandb' format string to logging.log_format_strs
+      extra_configs=("${extra_configs[@]}" "logging.wandb_logging")
       shift
       ;;
     -T | --tmux)
       extra_parallel_options=("${extra_parallel_options[@]}" --tmux)
       shift
       ;;
     --run_name)
@@ -80,15 +80,15 @@
   "${extra_parallel_options[@]}" \
   python -m imitation.scripts.train_imitation \
   --capture=sys \
   "${extra_options[@]}" \
   dagger \
   with \
   '{env_config_name}' \
-  common.log_dir="${LOG_ROOT}/{env_config_name}_{seed}" \
+  logging.log_dir="${LOG_ROOT}/{env_config_name}_{seed}" \
   dagger.expert_policy_type='ppo' \
   seed='{seed}' \
   "${extra_configs[@]}" \
   ::: env_config_name "${ENVS[@]}" \
   ::: seed "${SEEDS[@]}"
 
 # Directory path is really long. Enter the directory to shorten results output,
```

### Comparing `imitation-0.3.2/experiments/imit_benchmark.sh` & `imitation-0.4.0/experiments/imit_benchmark.sh`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 
 while true; do
   case "$1" in
     # Fast mode (debug)
     -f | --fast)
       CONFIG_CSV="tests/testdata/imit_benchmark_config.csv"
       SEEDS=(0)
-      extra_configs=("${extra_configs[@]}" common.fast demonstrations.fast rl.fast train.fast fast)
+      extra_configs=("${extra_configs[@]}" environment.fast demonstrations.fast rl.fast policy_evaluation.fast fast)
       shift
       ;;
     -w | --wandb)
-      # activate wandb logging by adding 'wandb' format string to common.log_format_strs
-      extra_configs=("${extra_configs[@]}" "common.wandb_logging")
+      # activate wandb logging by adding 'wandb' format string to logging.log_format_strs
+      extra_configs=("${extra_configs[@]}" "logging.wandb_logging")
       shift
       ;;
     --mvp_seals)
       CONFIG_CSV="experiments/imit_table_mvp_seals_config.csv"
       shift
       ;;
     --cheetah)
@@ -101,15 +101,15 @@
   "${extra_parallel_options[@]}" \
   python -m imitation.scripts.train_adversarial \
   --capture=sys \
   "${extra_options[@]}" \
   "${ALGORITHM}" \
   with \
   '{env_config_name}' seed='{seed}' \
-  common.log_dir="${LOG_ROOT}/{env_config_name}_{seed}/n_expert_demos_{n_expert_demos}" \
+  logging.log_dir="${LOG_ROOT}/{env_config_name}_{seed}/n_expert_demos_{n_expert_demos}" \
   demonstrations.n_expert_demos='{n_expert_demos}' \
   checkpoint_interval=0 \
   "${extra_configs[@]}" \
   :::: $CONFIG_CSV \
   ::: seed "${SEEDS[@]}"
 
 # Print the name of each stderr output file the line containing "Result"
```

### Comparing `imitation-0.3.2/experiments/imit_benchmark_config.csv` & `imitation-0.4.0/experiments/imit_benchmark_config.csv`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/experiments/rollouts_from_policies.sh` & `imitation-0.4.0/experiments/rollouts_from_policies.sh`

 * *Files 9% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 echo "Writing logs in ${OUTPUT_DIR}, and saving rollouts in ${OUTPUT_DIR}/expert_models/*/rollouts/"
 
 parallel -j 25% --header : --results "${OUTPUT_DIR}/parallel/" --colsep , \
   python -m imitation.scripts.eval_policy \
   --capture=sys \
   with \
   '{env_config_name}' \
-  common.log_root="${OUTPUT_DIR}" \
+  logging.log_root="${OUTPUT_DIR}" \
   rollout_save_path="${OUTPUT_DIR}/expert_models/{env_config_name}_0/rollouts/final.npz" \
   eval_n_episodes='{n_demonstrations}' \
   eval_n_timesteps=None \
   :::: ${CONFIG_CSV}
```

### Comparing `imitation-0.3.2/experiments/transfer_learn_benchmark.sh` & `imitation-0.4.0/experiments/transfer_learn_benchmark.sh`

 * *Files 7% similar despite different names*

```diff
@@ -25,20 +25,20 @@
   case "$1" in
     # Fast mode (debug)
     -f | --fast)
       CONFIG_CSV="tests/testdata/imit_benchmark_config.csv"
       REWARD_MODELS_DIR="tests/testdata/reward_models"
       NEED_TEST_FILES="true"
       SEEDS=(0)
-      extra_configs=("${extra_configs[@]}" common.fast rl.fast train.fast fast)
+      extra_configs=("${extra_configs[@]}" environment.fast rl.fast policy_evaluation.fast fast)
       shift
       ;;
     -w | --wandb)
-      # activate wandb logging by adding 'wandb' format string to common.log_format_strs
-      extra_configs=("${extra_configs[@]}" "common.wandb_logging")
+      # activate wandb logging by adding 'wandb' format string to logging.log_format_strs
+      extra_configs=("${extra_configs[@]}" "logging.wandb_logging")
       shift
       ;;
     --gail)
       ALGORITHM="gail"
       shift
       ;;
     --airl)
@@ -84,15 +84,15 @@
 echo "Writing logs in ${LOG_ROOT}"
 parallel -j 25% --header : --results "${LOG_ROOT}/parallel/" --colsep , --progress \
   python -m imitation.scripts.train_rl \
   --capture=sys \
   "${extra_options[@]}" \
   with \
   '{env_config_name}' seed='{seed}' \
-  common.log_dir="${LOG_ROOT}/${ALGORITHM}/{env_config_name}_{seed}/n_expert_demos_{n_expert_demos}" \
+  logging.log_dir="${LOG_ROOT}/${ALGORITHM}/{env_config_name}_{seed}/n_expert_demos_{n_expert_demos}" \
   reward_type="RewardNet_unshaped" \
   reward_path="${REWARD_MODELS_DIR}/${ALGORITHM}/${TIMESTAMP}-${BASHPID}/{env_config_name}_0/n_expert_demos_{n_expert_demos}/checkpoints/final/reward_test.pt" \
   "${extra_configs[@]}" \
   :::: ${CONFIG_CSV} \
   ::: seed "${SEEDS[@]}"
 
 pushd "$LOG_ROOT"
```

### Comparing `imitation-0.3.2/runners/build_push_image.sh` & `imitation-0.4.0/runners/build_push_image.sh`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/runners/launch_docker-dev.sh` & `imitation-0.4.0/runners/launch_docker-dev.sh`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/setup.cfg` & `imitation-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/setup.py` & `imitation-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 IS_NOT_WINDOWS = os.name != "nt"
 
 PARALLEL_REQUIRE = ["ray[debug,tune]~=2.0.0"]
 ATARI_REQUIRE = [
     "opencv-python",
     "ale-py==0.7.4",
     "pillow",
-    "autorom[accept-rom-license]~=0.4.2",
+    "autorom[accept-rom-license]~=0.6.0",
 ]
 PYTYPE = ["pytype==2022.7.26"] if IS_NOT_WINDOWS else []
-STABLE_BASELINES3 = "stable-baselines3>=1.6.1"
+STABLE_BASELINES3 = "stable-baselines3>=1.7.0,<2.0.0"
 # pinned to 0.21 until https://github.com/DLR-RM/stable-baselines3/pull/780 goes
 # upstream.
 GYM_VERSION_SPECIFIER = "==0.21.0"
 
 # Note: the versions of the test and doc requirements should be tightly pinned to known
 #   working versions to make our CI/CD pipeline as stable as possible.
 TESTS_REQUIRE = (
@@ -201,19 +201,18 @@
         "matplotlib",
         "numpy>=1.15",
         "torch>=1.4.0",
         "tqdm",
         "scikit-learn>=0.21.2",
         "seals>=0.1.5",
         STABLE_BASELINES3,
-        # TODO(adam) switch to upstream release if they make it
-        #  See https://github.com/IDSIA/sacred/issues/879
-        "chai-sacred>=0.8.3",
+        "sacred>=0.8.4",
         "tensorboard>=1.14",
         "huggingface_sb3>=2.2.1",
+        "datasets>=2.8.0",
     ],
     tests_require=TESTS_REQUIRE,
     extras_require={
         # recommended packages for development
         "dev": [
             "autopep8",
             "ipdb",
```

### Comparing `imitation-0.3.2/src/imitation/algorithms/adversarial/airl.py` & `imitation-0.4.0/src/imitation/algorithms/adversarial/airl.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/algorithms/adversarial/common.py` & `imitation-0.4.0/src/imitation/algorithms/adversarial/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         self._disc_step = 0
         self.n_disc_updates_per_round = n_disc_updates_per_round
 
         self.debug_use_ground_truth = debug_use_ground_truth
         self.venv = venv
         self.gen_algo = gen_algo
         self._reward_net = reward_net.to(gen_algo.device)
-        self._log_dir = types.parse_path(log_dir)
+        self._log_dir = util.parse_path(log_dir)
 
         # Create graph for optimising/recording stats on discriminator
         self._disc_opt_cls = disc_opt_cls
         self._disc_opt_kwargs = disc_opt_kwargs or {}
         self._init_tensorboard = init_tensorboard
         self._init_tensorboard_graph = init_tensorboard_graph
         self._disc_opt = self._disc_opt_cls(
@@ -497,15 +497,16 @@
                 mean_actions,
                 log_std,
             )
             # SAC applies a squashing function to bound the actions to a finite range
             # `acts_th` need to be scaled accordingly before computing log prob.
             # Scale actions only if the policy squashes outputs.
             assert self.policy.squash_output
-            scaled_acts_th = self.policy.scale_action(acts_th)
+            scaled_acts = self.policy.scale_action(acts_th.numpy(force=True))
+            scaled_acts_th = th.as_tensor(scaled_acts, device=mean_actions.device)
             log_policy_act_prob_th = distribution.log_prob(scaled_acts_th)
         else:
             return None
         return log_policy_act_prob_th
 
     def _make_disc_train_batches(
         self,
```

### Comparing `imitation-0.3.2/src/imitation/algorithms/adversarial/gail.py` & `imitation-0.4.0/src/imitation/algorithms/adversarial/gail.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/algorithms/base.py` & `imitation-0.4.0/src/imitation/algorithms/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,17 @@
             horizons.add(self._horizon)
 
         if len(horizons) > 1:
             raise ValueError(
                 f"Episodes of different length detected: {horizons}. "
                 "Variable horizon environments are discouraged -- "
                 "termination conditions leak information about reward. See "
-                "https://imitation.readthedocs.io/en/latest/guide/variable_horizon.html"
-                " for more information. If you are SURE you want to run imitation on a "
+                "https://imitation.readthedocs.io/en/latest/getting-started/"
+                "variable-horizon.html for more information. "
+                "If you are SURE you want to run imitation on a "
                 "variable horizon task, then please pass in the flag: "
                 "`allow_variable_horizon=True`.",
             )
         elif len(horizons) == 1:
             self._horizon = horizons.pop()
 
     def __getstate__(self):
@@ -150,15 +151,15 @@
                 keywords to arrays containing observations, etc).
             custom_logger: Where to log to; if None (default), creates a new logger.
             allow_variable_horizon: If False (default), algorithm will raise an
                 exception if it detects trajectories of different length during
                 training. If True, overrides this safety check. WARNING: variable
                 horizon episodes leak information about the reward via termination
                 condition, and can seriously confound evaluation. Read
-                https://imitation.readthedocs.io/en/latest/guide/variable_horizon.html
+                https://imitation.readthedocs.io/en/latest/getting-started/variable-horizon.html
                 before overriding this.
         """
         super().__init__(
             custom_logger=custom_logger,
             allow_variable_horizon=allow_variable_horizon,
         )
```

### Comparing `imitation-0.3.2/src/imitation/algorithms/bc.py` & `imitation-0.4.0/src/imitation/algorithms/bc.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 
 
 @dataclasses.dataclass(frozen=True)
 class BCTrainingMetrics:
     """Container for the different components of behavior cloning loss."""
 
     neglogp: th.Tensor
-    entropy: th.Tensor
-    ent_loss: th.Tensor
+    entropy: Optional[th.Tensor]
+    ent_loss: th.Tensor  # set to 0 if entropy is None
     prob_true_act: th.Tensor
     l2_norm: th.Tensor
     l2_loss: th.Tensor
     loss: th.Tensor
 
 
 @dataclasses.dataclass(frozen=True)
@@ -115,22 +115,22 @@
             consists of.
         """
         obs = util.safe_to_tensor(obs)
         acts = util.safe_to_tensor(acts)
         _, log_prob, entropy = policy.evaluate_actions(obs, acts)
         prob_true_act = th.exp(log_prob).mean()
         log_prob = log_prob.mean()
-        entropy = entropy.mean()
+        entropy = entropy.mean() if entropy is not None else None
 
         l2_norms = [th.sum(th.square(w)) for w in policy.parameters()]
         l2_norm = sum(l2_norms) / 2  # divide by 2 to cancel with gradient of square
         # sum of list defaults to float(0) if len == 0.
         assert isinstance(l2_norm, th.Tensor)
 
-        ent_loss = -self.ent_weight * entropy
+        ent_loss = -self.ent_weight * (entropy if entropy is not None else th.zeros(1))
         neglogp = -log_prob
         l2_loss = self.l2_weight * l2_norm
         loss = neglogp + ent_loss + l2_loss
 
         return BCTrainingMetrics(
             neglogp=neglogp,
             entropy=entropy,
@@ -215,15 +215,15 @@
         rollout_stats: Mapping[str, float],
     ):
         self._logger.record("batch_size", batch_size)
         self._logger.record("bc/epoch", self._current_epoch)
         self._logger.record("bc/batch", batch_num)
         self._logger.record("bc/samples_so_far", num_samples_so_far)
         for k, v in training_metrics.__dict__.items():
-            self._logger.record(f"bc/{k}", float(v))
+            self._logger.record(f"bc/{k}", float(v) if v is not None else None)
 
         for k, v in rollout_stats.items():
             if "return" in k and "monitor" not in k:
                 self._logger.record("rollout/" + k, v)
         self._logger.dump(self._tensorboard_step)
         self._tensorboard_step += 1
 
@@ -486,8 +486,8 @@
 
     def save_policy(self, policy_path: types.AnyPath) -> None:
         """Save policy to a path. Can be reloaded by `.reconstruct_policy()`.
 
         Args:
             policy_path: path to save policy to.
         """
-        th.save(self.policy, types.parse_path(policy_path))
+        th.save(self.policy, util.parse_path(policy_path))
```

### Comparing `imitation-0.3.2/src/imitation/algorithms/dagger.py` & `imitation-0.4.0/src/imitation/algorithms/dagger.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 policy.
 """
 
 import abc
 import logging
 import os
 import pathlib
+import uuid
 from typing import Any, Callable, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import torch as th
 from stable_baselines3.common import policies, utils, vec_env
 from stable_baselines3.common.vec_env.base_vec_env import VecEnvStepReturn
 from torch.utils import data as th_data
 
 from imitation.algorithms import base, bc
-from imitation.data import rollout, types
+from imitation.data import rollout, serialize, types
 from imitation.util import logger as imit_logger
 from imitation.util import util
 
 
 class BetaSchedule(abc.ABC):
     """Computes beta (% of time demonstration action used) from training round."""
 
@@ -62,14 +63,43 @@
             beta linearly decreasing from `1` to `0` between round `0` and
             `self.rampdown_rounds`. After that, it is 0.
         """
         assert round_num >= 0
         return min(1, max(0, (self.rampdown_rounds - round_num) / self.rampdown_rounds))
 
 
+class ExponentialBetaSchedule(BetaSchedule):
+    """Exponentially decaying schedule for beta."""
+
+    def __init__(self, decay_probability: float):
+        """Builds ExponentialBetaSchedule.
+
+        Args:
+            decay_probability: the decay factor for beta.
+
+        Raises:
+            ValueError: if `decay_probability` not within (0, 1].
+        """
+        if not (0 < decay_probability <= 1):
+            raise ValueError("decay_probability lies outside the range (0, 1].")
+        self.decay_probability = decay_probability
+
+    def __call__(self, round_num: int) -> float:
+        """Computes beta value.
+
+        Args:
+            round_num: the current round number.
+
+        Returns:
+            beta as `self.decay_probability ^ round_num`
+        """
+        assert round_num >= 0
+        return self.decay_probability**round_num
+
+
 def reconstruct_trainer(
     scratch_dir: types.AnyPath,
     venv: vec_env.VecEnv,
     custom_logger: Optional[imit_logger.HierarchicalLogger] = None,
     device: Union[th.device, str] = "auto",
 ) -> "DAggerTrainer":
     """Reconstruct trainer from the latest snapshot in some working directory.
@@ -85,35 +115,40 @@
         custom_logger: Where to log to; if None (default), creates a new logger.
         device: device on which to load the trainer.
 
     Returns:
         A deserialized `DAggerTrainer`.
     """
     custom_logger = custom_logger or imit_logger.configure()
-    scratch_dir = types.parse_path(scratch_dir)
+    scratch_dir = util.parse_path(scratch_dir)
     checkpoint_path = scratch_dir / "checkpoint-latest.pt"
     trainer = th.load(checkpoint_path, map_location=utils.get_device(device))
     trainer.venv = venv
     trainer._logger = custom_logger
     return trainer
 
 
 def _save_dagger_demo(
     trajectory: types.Trajectory,
+    trajectory_index: int,
     save_dir: types.AnyPath,
+    rng: np.random.Generator,
     prefix: str = "",
 ) -> None:
-    save_dir = types.parse_path(save_dir)
+    save_dir = util.parse_path(save_dir)
     assert isinstance(trajectory, types.Trajectory)
     actual_prefix = f"{prefix}-" if prefix else ""
-    timestamp = util.make_unique_timestamp()
-    filename = f"{actual_prefix}dagger-demo-{timestamp}.npz"
-
+    randbits = int.from_bytes(rng.bytes(16), "big")
+    random_uuid = uuid.UUID(int=randbits, version=4).hex
+    filename = f"{actual_prefix}dagger-demo-{trajectory_index}-{random_uuid}.npz"
     npz_path = save_dir / filename
-    types.save(npz_path, [trajectory])
+    assert (
+        not npz_path.exists()
+    ), "The following DAgger demonstration path already exists: {0}".format(npz_path)
+    serialize.save(npz_path, [trajectory])
     logging.info(f"Saved demo at '{npz_path}'")
 
 
 class InteractiveTrajectoryCollector(vec_env.VecEnvWrapper):
     """DAgger VecEnvWrapper for querying and saving expert actions.
 
     Every call to `.step(actions)` accepts and saves expert actions to `self.save_dir`,
@@ -242,16 +277,16 @@
         fresh_demos = self.traj_accum.add_steps_and_auto_finish(
             obs=next_obs,
             acts=self._last_user_actions,
             rews=rews,
             infos=infos,
             dones=dones,
         )
-        for traj in fresh_demos:
-            _save_dagger_demo(traj, self.save_dir)
+        for traj_index, traj in enumerate(fresh_demos):
+            _save_dagger_demo(traj, traj_index, self.save_dir, self.rng)
 
         return next_obs, rews, dones, infos
 
 
 class NeedsDemosException(Exception):
     """Signals demos need to be collected for current round before continuing."""
 
@@ -315,15 +350,15 @@
             custom_logger: Where to log to; if None (default), creates a new logger.
         """
         super().__init__(custom_logger=custom_logger)
 
         if beta_schedule is None:
             beta_schedule = LinearBetaSchedule(15)
         self.beta_schedule = beta_schedule
-        self.scratch_dir = types.parse_path(scratch_dir)
+        self.scratch_dir = util.parse_path(scratch_dir)
         self.venv = venv
         self.round_num = 0
         self._last_loaded_round = -1
         self._all_demos = []
         self.rng = rng
 
         utils.check_for_correct_spaces(
@@ -361,22 +396,28 @@
         return self.bc_trainer.batch_size
 
     def _load_all_demos(self) -> Tuple[types.Transitions, List[int]]:
         num_demos_by_round = []
         for round_num in range(self._last_loaded_round + 1, self.round_num + 1):
             round_dir = self._demo_dir_path_for_round(round_num)
             demo_paths = self._get_demo_paths(round_dir)
-            self._all_demos.extend(types.load(p)[0] for p in demo_paths)
+            self._all_demos.extend(serialize.load(p)[0] for p in demo_paths)
             num_demos_by_round.append(len(demo_paths))
         logging.info(f"Loaded {len(self._all_demos)} total")
         demo_transitions = rollout.flatten_trajectories(self._all_demos)
         return demo_transitions, num_demos_by_round
 
     def _get_demo_paths(self, round_dir: pathlib.Path) -> List[pathlib.Path]:
-        return [round_dir / p for p in os.listdir(round_dir) if p.endswith(".npz")]
+        # listdir returns filenames in an arbitrary order that depends on the
+        # file system implementation:
+        # https://stackoverflow.com/questions/31534583/is-os-listdir-deterministic
+        # To ensure the order is consistent across file systems,
+        # we sort by the filename.
+        filenames = sorted(os.listdir(round_dir))
+        return [round_dir / f for f in filenames if f.endswith(".npz")]
 
     def _demo_dir_path_for_round(self, round_num: Optional[int] = None) -> pathlib.Path:
         if round_num is None:
             round_num = self.round_num
         return self.scratch_dir / "demos" / f"round-{round_num:03d}"
 
     def _try_load_demos(self) -> None:
@@ -566,18 +607,20 @@
         # TODO(shwang):
         #   Might welcome Transitions and DataLoaders as sources of expert data
         #   in the future too, but this will require some refactoring, so for
         #   now we just have `expert_trajs`.
         if expert_trajs is not None:
             # Save each initial expert trajectory into the "round 0" demonstration
             # data directory.
-            for traj in expert_trajs:
+            for traj_index, traj in enumerate(expert_trajs):
                 _save_dagger_demo(
                     traj,
+                    traj_index,
                     self._demo_dir_path_for_round(),
+                    self.rng,
                     prefix="initial_data",
                 )
 
     def train(
         self,
         total_timesteps: int,
         *,
```

### Comparing `imitation-0.3.2/src/imitation/algorithms/density.py` & `imitation-0.4.0/src/imitation/algorithms/density.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/algorithms/mce_irl.py` & `imitation-0.4.0/src/imitation/algorithms/mce_irl.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/algorithms/preference_comparisons.py` & `imitation-0.4.0/src/imitation/algorithms/preference_comparisons.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,17 @@
         # First, we compute the difference of the returns of
         # the two fragments. We have a special case for a discount
         # factor of 1 to avoid unnecessary computation (especially
         # since this is the default setting).
         if self.discount_factor == 1:
             returns_diff = (rews2 - rews1).sum(axis=0)  # type: ignore[call-overload]
         else:
-            discounts = self.discount_factor ** th.arange(len(rews1))
+            device = rews1.device
+            assert device == rews2.device
+            discounts = self.discount_factor ** th.arange(len(rews1), device=device)
             if self.ensemble_model is not None:
                 discounts = discounts.reshape(-1, 1)
             returns_diff = (discounts * (rews2 - rews1)).sum(axis=0)
         # Clip to avoid overflows (which in particular may occur
         # in the backwards pass even if they do not in the forward pass).
         returns_diff = th.clip(returns_diff, -self.threshold, self.threshold)
         # We take the softmax of the returns. model_probability
```

### Comparing `imitation-0.3.2/src/imitation/data/buffer.py` & `imitation-0.4.0/src/imitation/data/buffer.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/data/rollout.py` & `imitation-0.4.0/src/imitation/data/rollout.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Callable,
     Dict,
     Hashable,
     List,
     Mapping,
     Optional,
     Sequence,
+    Tuple,
     Union,
 )
 
 import numpy as np
 from stable_baselines3.common.base_class import BaseAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.utils import check_for_correct_spaces
@@ -258,46 +259,62 @@
             if not cond(trajs):
                 return False
         return True
 
     return sample_until
 
 
-# A PolicyCallable is a function that takes an array of observations
-# and returns an array of corresponding actions.
-PolicyCallable = Callable[[np.ndarray], np.ndarray]
+# A PolicyCallable is a function that takes an array of observations, an optional
+# array of states, and an optional array of episode starts and returns an array of
+# corresponding actions.
+PolicyCallable = Callable[
+    [np.ndarray, Optional[Tuple[np.ndarray, ...]], Optional[np.ndarray]],
+    Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]],
+]
 AnyPolicy = Union[BaseAlgorithm, BasePolicy, PolicyCallable, None]
 
 
 def policy_to_callable(
     policy: AnyPolicy,
     venv: VecEnv,
     deterministic_policy: bool = False,
 ) -> PolicyCallable:
     """Converts any policy-like object into a function from observations to actions."""
+    get_actions: PolicyCallable
     if policy is None:
 
-        def get_actions(states):
-            acts = [venv.action_space.sample() for _ in range(len(states))]
-            return np.stack(acts, axis=0)
+        def get_actions(
+            observations: np.ndarray,
+            states: Optional[Tuple[np.ndarray, ...]],
+            episode_starts: Optional[np.ndarray],
+        ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
+            acts = [venv.action_space.sample() for _ in range(len(observations))]
+            return np.stack(acts, axis=0), None
 
     elif isinstance(policy, (BaseAlgorithm, BasePolicy)):
         # There's an important subtlety here: BaseAlgorithm and BasePolicy
         # are themselves Callable (which we check next). But in their case,
         # we want to use the .predict() method, rather than __call__()
         # (which would call .forward()). So this elif clause must come first!
 
-        def get_actions(states):
+        def get_actions(
+            observations: np.ndarray,
+            states: Optional[Tuple[np.ndarray, ...]],
+            episode_starts: Optional[np.ndarray],
+        ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
+            assert isinstance(policy, (BaseAlgorithm, BasePolicy))
             # pytype doesn't seem to understand that policy is a BaseAlgorithm
             # or BasePolicy here, rather than a Callable
-            acts, _ = policy.predict(  # pytype: disable=attribute-error
-                states,
+            (acts, states) = policy.predict(  # pytype: disable=attribute-error
+                observations,
+                state=states,
+                episode_start=episode_starts,
                 deterministic=deterministic_policy,
             )
-            return acts
+            return acts, states
 
     elif callable(policy):
         # When a policy callable is passed, by default we will use it directly.
         # We are not able to change the determinism of the policy when it is a
         # callable that only takes in the states.
         if deterministic_policy:
             raise ValueError(
@@ -398,16 +415,18 @@
     # since longer episodes are more likely to still be active, i.e. in the process
     # of being sampled from. To avoid this, we continue sampling until all epsiodes
     # are complete.
     #
     # To start with, all environments are active.
     active = np.ones(venv.num_envs, dtype=bool)
     assert isinstance(obs, np.ndarray), "Dict/tuple observations are not supported."
+    state = None
+    dones = np.zeros(venv.num_envs, dtype=bool)
     while np.any(active):
-        acts = get_actions(obs)
+        acts, state = get_actions(obs, state, dones)
         obs, rews, dones, infos = venv.step(acts)
         assert isinstance(obs, np.ndarray)
 
         # If an environment is inactive, i.e. the episode completed for that
         # environment after `sample_until(trajectories)` was true, then we do
         # *not* want to add any subsequent trajectories from it. We avoid this
         # by just making it never done.
@@ -606,14 +625,19 @@
     unwrap: bool = True,
     exclude_infos: bool = True,
     verbose: bool = True,
     **kwargs: Any,
 ) -> Sequence[types.TrajectoryWithRew]:
     """Generate policy rollouts.
 
+    This method is a wrapper of generate_trajectories that allows
+    the user to additionally replace the rewards and observations with the original
+    values if the environment is wrapped, to exclude the infos from the
+    trajectories, and to print summary statistics of the rollout.
+
     The `.infos` field of each Trajectory is set to `None` to save space.
 
     Args:
         policy: Can be any of the following:
             1) A stable_baselines3 policy or algorithm trained on the gym environment.
             2) A Callable that takes an ndarray of observations and returns an ndarray
             of corresponding actions.
```

### Comparing `imitation-0.3.2/src/imitation/data/wrappers.py` & `imitation-0.4.0/src/imitation/data/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             env: Environment to wrap.
         """
         super().__init__(env)
         self._obs = None
         self._rews = None
 
     def reset(self, **kwargs):
-        new_obs = super().reset()
+        new_obs = super().reset(**kwargs)
         self._obs = [new_obs]
         self._rews = []
         return new_obs
 
     def step(self, action):
         obs, rew, done, info = self.env.step(action)
         self._obs.append(obs)
```

### Comparing `imitation-0.3.2/src/imitation/policies/base.py` & `imitation-0.4.0/src/imitation/policies/base.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/policies/exploration_wrapper.py` & `imitation-0.4.0/src/imitation/util/video_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,78 @@
-"""Wrapper to turn a policy into a more exploratory version."""
+"""Wrapper to record rendered video frames from an environment."""
 
-import numpy as np
-from stable_baselines3.common import vec_env
+import pathlib
+from typing import Optional
 
-from imitation.data import rollout
-from imitation.util import util
+import gym
+from gym.wrappers.monitoring import video_recorder
 
 
-class ExplorationWrapper:
-    """Wraps a PolicyCallable to create a partially randomized version.
+class VideoWrapper(gym.Wrapper):
+    """Creates videos from wrapped environment by calling render after each timestep."""
 
-    This wrapper randomly switches between two policies: the wrapped policy,
-    and a random one. After each action, the current policy is kept
-    with a certain probability. Otherwise, one of these two policies is chosen
-    at random (without any dependence on what the current policy is).
-
-    The random policy uses the `action_space.sample()` method.
-    """
+    episode_id: int
+    video_recorder: Optional[video_recorder.VideoRecorder]
+    single_video: bool
+    directory: pathlib.Path
 
     def __init__(
         self,
-        policy: rollout.AnyPolicy,
-        venv: vec_env.VecEnv,
-        random_prob: float,
-        switch_prob: float,
-        rng: np.random.Generator,
-        deterministic_policy: bool = False,
+        env: gym.Env,
+        directory: pathlib.Path,
+        single_video: bool = True,
     ):
-        """Initializes the ExplorationWrapper.
+        """Builds a VideoWrapper.
 
         Args:
-            policy: The policy to randomize.
-            venv: The environment to use (needed for sampling random actions).
-            random_prob: The probability of picking the random policy when switching.
-            switch_prob: The probability of switching away from the current policy.
-            rng: The random state to use for seeding the environment and for
-                switching policies.
-            deterministic_policy: Whether to make the policy deterministic when not
-                exploring. This must be False when ``policy`` is a ``PolicyCallable``.
+            env: the wrapped environment.
+            directory: the output directory.
+            single_video: if True, generates a single video file, with episodes
+                concatenated. If False, a new video file is created for each episode.
+                Usually a single video file is what is desired. However, if one is
+                searching for an interesting episode (perhaps by looking at the
+                metadata), then saving to different files can be useful.
+        """
+        super().__init__(env)
+        self.episode_id = 0
+        self.video_recorder = None
+        self.single_video = single_video
+
+        self.directory = directory
+        self.directory.mkdir(parents=True, exist_ok=True)
+
+    def _reset_video_recorder(self) -> None:
+        """Creates a video recorder if one does not already exist.
+
+        Called at the start of each episode (by `reset`). When a video recorder is
+        already present, it will only create a new one if `self.single_video == False`.
         """
-        policy_callable = rollout.policy_to_callable(policy, venv, deterministic_policy)
-        self.wrapped_policy = policy_callable
-        self.random_prob = random_prob
-        self.switch_prob = switch_prob
-        self.venv = venv
-
-        self.rng = rng
-        seed = util.make_seeds(self.rng)
-        self.venv.action_space.seed(seed)
-
-        self.current_policy = policy_callable
-        # Choose the initial policy at random
-        self._switch()
-
-    def _random_policy(self, obs: np.ndarray) -> np.ndarray:
-        acts = [self.venv.action_space.sample() for _ in range(len(obs))]
-        return np.stack(acts, axis=0)
-
-    def _switch(self) -> None:
-        """Pick a new policy at random."""
-        if self.rng.random() < self.random_prob:
-            self.current_policy = self._random_policy
-        else:
-            self.current_policy = self.wrapped_policy
-
-    def __call__(self, obs: np.ndarray) -> np.ndarray:
-        acts = self.current_policy(obs)
-        if self.rng.random() < self.switch_prob:
-            self._switch()
-        return acts
+        if self.video_recorder is not None:
+            # Video recorder already started.
+            if not self.single_video:
+                # We want a new video for each episode, so destroy current recorder.
+                self.video_recorder.close()
+                self.video_recorder = None
+
+        if self.video_recorder is None:
+            # No video recorder -- start a new one.
+            self.video_recorder = video_recorder.VideoRecorder(
+                env=self.env,
+                base_path=str(self.directory / f"video.{self.episode_id:06}"),
+                metadata={"episode_id": self.episode_id},
+            )
+
+    def reset(self):
+        self._reset_video_recorder()
+        self.episode_id += 1
+        return self.env.reset()
+
+    def step(self, action):
+        res = self.env.step(action)
+        self.video_recorder.capture_frame()
+        return res
+
+    def close(self) -> None:
+        if self.video_recorder is not None:
+            self.video_recorder.close()
+            self.video_recorder = None
+        super().close()
```

### Comparing `imitation-0.3.2/src/imitation/policies/replay_buffer_wrapper.py` & `imitation-0.4.0/src/imitation/policies/replay_buffer_wrapper.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/policies/serialize.py` & `imitation-0.4.0/src/imitation/policies/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 import logging
 import pathlib
 from typing import Callable, Type, TypeVar
 
 import huggingface_sb3 as hfsb3
 from stable_baselines3.common import base_class, callbacks, policies, vec_env
 
-from imitation.data import types
 from imitation.policies import base
-from imitation.util import registry
+from imitation.util import registry, util
 
 Algorithm = TypeVar("Algorithm", bound=base_class.BaseAlgorithm)
 
 # Note: a VecEnv will always be passed first and then any kwargs. There is just no
 # proper way to specify this in python yet. For details see
 # https://stackoverflow.com/questions/61569324/type-annotation-for-callable-that-takes-kwargs
 # TODO(juan) this can be fixed using ParamSpec
@@ -48,15 +47,15 @@
         FileNotFoundError: If `path` is not a directory containing a `model.zip` file.
         FileExistsError: If `path` contains a `vec_normalize.pkl` file (unsupported).
 
     Returns:
         The deserialized RL algorithm.
     """
     logging.info(f"Loading Stable Baselines policy for '{cls}' from '{path}'")
-    path_obj = types.parse_path(path)
+    path_obj = util.parse_path(path)
 
     if path_obj.is_dir():
         path_obj = path_obj / "model.zip"
         if not path_obj.exists():
             raise FileNotFoundError(
                 f"Expected '{path}' to be a directory containing a 'model.zip' file.",
             )
```

### Comparing `imitation-0.3.2/src/imitation/regularization/regularizers.py` & `imitation-0.4.0/src/imitation/regularization/regularizers.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/regularization/updaters.py` & `imitation-0.4.0/src/imitation/regularization/updaters.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/rewards/reward_function.py` & `imitation-0.4.0/src/imitation/rewards/reward_function.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/rewards/reward_nets.py` & `imitation-0.4.0/src/imitation/rewards/reward_nets.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/rewards/reward_wrapper.py` & `imitation-0.4.0/src/imitation/rewards/reward_wrapper.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/rewards/serialize.py` & `imitation-0.4.0/src/imitation/rewards/serialize.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/scripts/analyze.py` & `imitation-0.4.0/src/imitation/scripts/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import warnings
 from typing import Any, Callable, Iterable, List, Mapping, Optional, Sequence, Set
 
 import pandas as pd
 from sacred.observers import FileStorageObserver
 
 import imitation.util.sacred as sacred_util
-from imitation.data import types
 from imitation.scripts.config.analyze import analysis_ex
+from imitation.util import util
 from imitation.util.sacred import dict_get_nested as get
 
 
 @analysis_ex.capture
 def _gather_sacred_dicts(
     source_dirs: Sequence[str],
     run_name: Optional[str],
@@ -42,15 +42,15 @@
 
     Returns:
         A list of `SacredDicts` corresponding to the selected Sacred directories.
     """
     # e.g. chain.from_iterable([["pathone", "pathtwo"], [], ["paththree"]]) =>
     # ("pathone", "pathtwo", "paththree")
     sacred_dirs = itertools.chain.from_iterable(
-        sacred_util.filter_subdirs(types.parse_path(source_dir))
+        sacred_util.filter_subdirs(util.parse_path(source_dir))
         for source_dir in source_dirs
     )
     sacred_dicts_list = []
 
     for sacred_dir in sacred_dirs:
         try:
             sacred_dicts_list.append(sacred_util.SacredDicts.load_from_dir(sacred_dir))
@@ -62,15 +62,15 @@
         sacred_dicts = filter(
             lambda sd: get(sd.run, "experiment.name") == run_name,
             sacred_dicts,
         )
 
     if env_name is not None:
         sacred_dicts = filter(
-            lambda sd: get(sd.config, "common.env_name") == env_name,
+            lambda sd: get(sd.config, "environment.gym_id") == env_name,
             sacred_dicts,
         )
 
     if skip_failed_runs:
         sacred_dicts = filter(
             lambda sd: get(sd.run, "status") != "FAILED",
             sacred_dicts,
@@ -198,15 +198,15 @@
 
 # This dict maps column names to functions that get table entries, given the
 # row's unique SacredDicts object.
 table_entry_fns: sd_to_table_entry_type = {
     "status": lambda sd: get(sd.run, "status"),
     "exp_command": _get_exp_command,
     "algo": _get_algo_name,
-    "env_name": lambda sd: get(sd.config, "common.env_name"),
+    "env_name": lambda sd: get(sd.config, "environment.gym_id"),
     "n_expert_demos": lambda sd: get(sd.config, "demonstrations.n_expert_demos"),
     "run_name": lambda sd: get(sd.run, "experiment.name"),
     "expert_return_summary": lambda sd: _return_summaries(sd)["expert_return_summary"],
     "imit_return_summary": lambda sd: _return_summaries(sd)["imit_return_summary"],
     "imit_expert_ratio": lambda sd: _return_summaries(sd)["imit_expert_ratio"],
 }
```

### Comparing `imitation-0.3.2/src/imitation/scripts/common/reward.py` & `imitation-0.4.0/src/imitation/scripts/ingredients/reward.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Common configuration elements for reward network training."""
+"""This ingredient provides a reward network."""
 
 import logging
 import typing
 from typing import Any, Mapping, Optional, Type
 
 import sacred
 from stable_baselines3.common import vec_env
```

### Comparing `imitation-0.3.2/src/imitation/scripts/common/rl.py` & `imitation-0.4.0/src/imitation/scripts/ingredients/rl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Common configuration elements for reinforcement learning."""
+"""This ingredient provides a reinforcement learning algorithm from stable-baselines3.
+
+The algorithm instance is either freshly constructed or loaded from a file.
+"""
 
 import logging
 import warnings
 from typing import Any, Dict, Mapping, Optional, Type
 
 import sacred
 import stable_baselines3 as sb3
@@ -13,20 +16,20 @@
     on_policy_algorithm,
     vec_env,
 )
 
 from imitation.policies import serialize
 from imitation.policies.replay_buffer_wrapper import ReplayBufferRewardWrapper
 from imitation.rewards.reward_function import RewardFn
-from imitation.scripts.common import common
-from imitation.scripts.common.train import train_ingredient
+from imitation.scripts.ingredients import logging as logging_ingredient
+from imitation.scripts.ingredients.policy import policy_ingredient
 
 rl_ingredient = sacred.Ingredient(
     "rl",
-    ingredients=[train_ingredient, common.common_ingredient],
+    ingredients=[policy_ingredient, logging_ingredient.logging_ingredient],
 )
 logger = logging.getLogger(__name__)
 
 
 @rl_ingredient.config
 def config():
     rl_cls = None
@@ -51,17 +54,21 @@
         )
     return res
 
 
 @rl_ingredient.named_config
 def fast():
     batch_size = 2
-    # SB3 RL seems to need batch size of 2, otherwise it runs into numeric
-    # issues when computing multinomial distribution during predict()
-    rl_kwargs = dict(batch_size=2)
+    rl_kwargs = dict(
+        # SB3 RL seems to need batch size of 2, otherwise it runs into numeric
+        # issues when computing multinomial distribution during predict()
+        batch_size=2,
+        # Setting n_epochs=1 speeds up thing a lot
+        n_epochs=1,
+    )
     locals()  # quieten flake8
 
 
 @rl_ingredient.named_config
 def sac():
     # For recommended SAC hyperparams in each environment, see:
     # https://github.com/DLR-RM/rl-baselines3-zoo/blob/master/hyperparams/sac.yml
@@ -101,26 +108,26 @@
 
 @rl_ingredient.capture
 def make_rl_algo(
     venv: vec_env.VecEnv,
     rl_cls: Type[base_class.BaseAlgorithm],
     batch_size: int,
     rl_kwargs: Mapping[str, Any],
-    train: Mapping[str, Any],
+    policy: Mapping[str, Any],
     _seed: int,
     relabel_reward_fn: Optional[RewardFn] = None,
 ) -> base_class.BaseAlgorithm:
     """Instantiates a Stable Baselines3 RL algorithm.
 
     Args:
         venv: The vectorized environment to train on.
         rl_cls: Type of a Stable Baselines3 RL algorithm.
         batch_size: The batch size of the RL algorithm.
         rl_kwargs: Keyword arguments for RL algorithm constructor.
-        train: Configuration for the train ingredient. We need the
+        policy: Configuration for the policy ingredient. We need the
             policy_cls and policy_kwargs component.
         relabel_reward_fn: Reward function used for reward relabeling
             in replay or rollout buffers of RL algorithms.
 
     Returns:
         The RL algorithm.
 
@@ -129,14 +136,19 @@
         TypeError: `rl_cls` is neither `OnPolicyAlgorithm` nor `OffPolicyAlgorithm`.
     """
     if batch_size % venv.num_envs != 0:
         raise ValueError(
             f"num_envs={venv.num_envs} must evenly divide batch_size={batch_size}.",
         )
     rl_kwargs = dict(rl_kwargs)
+
+    # TODO: this is a hack and an indicator that the rl ingredient should be refactored
+    if rl_cls == sb3.SAC:
+        del rl_kwargs["n_epochs"]
+
     # If on-policy, collect `batch_size` many timesteps each update.
     # If off-policy, train on `batch_size` many timesteps each update.
     # These are different notion of batches, but this seems the closest
     # possible translation, and I would expect the appropriate hyperparameter
     # to be similar between them.
     if issubclass(rl_cls, on_policy_algorithm.OnPolicyAlgorithm):
         assert "n_steps" not in rl_kwargs, (
@@ -151,20 +163,20 @@
         rl_kwargs = _maybe_add_relabel_buffer(
             rl_kwargs=rl_kwargs,
             relabel_reward_fn=relabel_reward_fn,
         )
     else:
         raise TypeError(f"Unsupported RL algorithm '{rl_cls}'")
     rl_algo = rl_cls(
-        policy=train["policy_cls"],
+        policy=policy["policy_cls"],
         # Note(yawen): Copy `policy_kwargs` as SB3 may mutate the config we pass.
         # In particular, policy_kwargs["use_sde"] may be changed in rl_cls.__init__()
         # for certain algorithms, such as Soft Actor Critic. See:
         # https://github.com/DLR-RM/stable-baselines3/blob/30772aa9f53a4cf61571ee90046cdc454c1b11d7/sb3/common/off_policy_algorithm.py#L145
-        policy_kwargs=dict(train["policy_kwargs"]),
+        policy_kwargs=dict(policy["policy_kwargs"]),
         env=venv,
         seed=_seed,
         **rl_kwargs,
     )
     logger.info(f"RL algorithm: {type(rl_algo)}")
     logger.info(f"Policy network summary:\n {rl_algo.policy}")
     return rl_algo
@@ -176,14 +188,19 @@
     agent_path: str,
     venv: vec_env.VecEnv,
     rl_cls: Type[base_class.BaseAlgorithm],
     rl_kwargs: Mapping[str, Any],
     relabel_reward_fn: Optional[RewardFn] = None,
 ) -> base_class.BaseAlgorithm:
     rl_kwargs = dict(rl_kwargs)
+
+    # TODO: this is a hack and an indicator that the rl ingredient should be refactored
+    if rl_cls == sb3.SAC:
+        del rl_kwargs["n_epochs"]
+
     if issubclass(rl_cls, off_policy_algorithm.OffPolicyAlgorithm):
         rl_kwargs = _maybe_add_relabel_buffer(
             rl_kwargs=rl_kwargs,
             relabel_reward_fn=relabel_reward_fn,
         )
     agent = serialize.load_stable_baselines_model(
         cls=rl_cls,
```

### Comparing `imitation-0.3.2/src/imitation/scripts/common/train.py` & `imitation-0.4.0/src/imitation/scripts/ingredients/policy_evaluation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,73 @@
-"""Common configuration elements for training imitation algorithms."""
+"""This ingredient performs evaluation of learned policy.
 
-import logging
-from typing import Any, Mapping, Union
+It takes care of the right wrappers, does some rollouts
+and computes statistics of the rollouts.
+"""
 
+from typing import Mapping, Union
+
+import numpy as np
 import sacred
 from stable_baselines3.common import base_class, policies, vec_env
 
-import imitation.util.networks
 from imitation.data import rollout
-from imitation.policies import base
-from imitation.scripts.common import common
 
-train_ingredient = sacred.Ingredient("train", ingredients=[common.common_ingredient])
-logger = logging.getLogger(__name__)
+policy_evaluation_ingredient = sacred.Ingredient("policy_evaluation")
 
 
-@train_ingredient.config
+@policy_evaluation_ingredient.config
 def config():
-    # Training
-    policy_cls = base.FeedForward32Policy
-    policy_kwargs = {}
-
-    # Evaluation
     n_episodes_eval = 50  # Num of episodes for final mean ground truth return
-
     locals()  # quieten flake8
 
 
-@train_ingredient.named_config
+@policy_evaluation_ingredient.named_config
 def fast():
     n_episodes_eval = 1  # noqa: F841
 
 
-@train_ingredient.named_config
-def sac():
-    policy_cls = base.SAC1024Policy  # noqa: F841
-
-
-NORMALIZE_RUNNING_POLICY_KWARGS = {
-    "features_extractor_class": base.NormalizeFeaturesExtractor,
-    "features_extractor_kwargs": {
-        "normalize_class": imitation.util.networks.RunningNorm,
-    },
-}
-
-
-@train_ingredient.named_config
-def normalize_running():
-    policy_kwargs = NORMALIZE_RUNNING_POLICY_KWARGS  # noqa: F841
-
-
-# Default config for CNN Policies
-@train_ingredient.named_config
-def cnn_policy():
-    policy_cls = policies.ActorCriticCnnPolicy  # noqa: F841
-
-
-@train_ingredient.capture
+@policy_evaluation_ingredient.capture
 def eval_policy(
     rl_algo: Union[base_class.BaseAlgorithm, policies.BasePolicy],
     venv: vec_env.VecEnv,
     n_episodes_eval: int,
+    _rnd: np.random.Generator,
 ) -> Mapping[str, float]:
     """Evaluation of imitation learned policy.
 
     Has the side effect of setting `rl_algo`'s environment to `venv`
     if it is a `BaseAlgorithm`.
 
     Args:
         rl_algo: Algorithm to evaluate.
         venv: Environment to evaluate on.
         n_episodes_eval: The number of episodes to average over when calculating
             the average episode reward of the imitation policy for return.
+        _rnd: Random number generator provided by Sacred.
 
     Returns:
         A dictionary with two keys. "imit_stats" gives the return value of
         `rollout_stats()` on rollouts test-reward-wrapped environment, using the final
         policy (remember that the ground-truth reward can be recovered from the
         "monitor_return" key). "expert_stats" gives the return value of
-        `rollout_stats()` on the expert demonstrations loaded from `rollout_path`.
+        `rollout_stats()` on the expert demonstrations loaded from `path`.
     """
-    rng = common.make_rng()
     sample_until_eval = rollout.make_min_episodes(n_episodes_eval)
     if isinstance(rl_algo, base_class.BaseAlgorithm):
         # Set RL algorithm's env to venv, removing any cruft wrappers that the RL
         # algorithm's environment may have accumulated.
         rl_algo.set_env(venv)
         # Generate trajectories with the RL algorithm's env - SB3 may apply wrappers
         # under the hood to get it to work with the RL algorithm (e.g. transposing
-        # images so they can be fed into CNNs).
+        # images, so they can be fed into CNNs).
         train_env = rl_algo.get_env()
         assert train_env is not None
     else:
         train_env = venv
     trajs = rollout.generate_trajectories(
         rl_algo,
         train_env,
         sample_until=sample_until_eval,
-        rng=rng,
+        rng=_rnd,
     )
     return rollout.rollout_stats(trajs)
-
-
-@train_ingredient.capture
-def suppress_sacred_error(policy_kwargs: Mapping[str, Any]):
-    """No-op so Sacred recognizes `policy_kwargs` is used (in `rl` and elsewhere)."""
```

### Comparing `imitation-0.3.2/src/imitation/scripts/common/wb.py` & `imitation-0.4.0/src/imitation/scripts/ingredients/wb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Weights & Biases configuration elements for scripts."""
+"""This ingredient provides Weights & Biases logging."""
 
 import logging
 from typing import Any, Mapping, Optional
 
 import sacred
 
-wandb_ingredient = sacred.Ingredient("common.wandb")
+wandb_ingredient = sacred.Ingredient("logging.wandb")
 logger = logging.getLogger(__name__)
 
 
 @wandb_ingredient.config
 def wandb_config():
     # Other users can overwrite this function to customize their wandb.init() call.
     wandb_tag = None  # User-specified tag for this run
@@ -42,15 +42,15 @@
         wandb_additional_info: User-specific additional info to add to wandb experiment
             ``config``.
         log_dir: W&B logs will be stored in directory `{log_dir}/wandb/`.
 
     Raises:
         ModuleNotFoundError: wandb is not installed.
     """
-    env_name = _run.config["common"]["env_name"]
+    env_name = _run.config["environment"]["gym_id"]
     root_seed = _run.config["seed"]
 
     updated_wandb_kwargs: Mapping[str, Any] = {
         **wandb_kwargs,
         "name": f"{wandb_name_prefix}-{env_name}-seed{root_seed}",
         "tags": [env_name, f"seed{root_seed}"] + ([wandb_tag] if wandb_tag else []),
         "dir": log_dir,
```

### Comparing `imitation-0.3.2/src/imitation/scripts/config/analyze.py` & `imitation-0.4.0/src/imitation/scripts/config/analyze.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/scripts/config/parallel.py` & `imitation-0.4.0/src/imitation/scripts/config/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,21 @@
                     "learning_rate": tune.grid_search(
                         [3e-4 * x for x in (1 / 3, 1 / 2)],
                     ),
                 },
             },
         },
     }
-    base_named_configs = ["cartpole", "common.fast", "train.fast", "rl.fast", "fast"]
+    base_named_configs = [
+        "cartpole",
+        "environment.fast",
+        "policy_evaluation.fast",
+        "rl.fast",
+        "fast",
+    ]
     base_config_updates = {
         "rollout_save_final": False,
     }
 
 
 @parallel_ex.named_config
 def example_cartpole_rl():
```

### Comparing `imitation-0.3.2/src/imitation/scripts/config/train_preference_comparisons.py` & `imitation-0.4.0/src/imitation/scripts/config/train_preference_comparisons.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Configuration for imitation.scripts.train_preference_comparisons."""
 
 import sacred
 
 from imitation.algorithms import preference_comparisons
-from imitation.scripts.common import common, reward, rl, train
+from imitation.scripts.ingredients import environment
+from imitation.scripts.ingredients import logging as logging_ingredient
+from imitation.scripts.ingredients import policy_evaluation, reward, rl
 
 train_preference_comparisons_ex = sacred.Experiment(
     "train_preference_comparisons",
     ingredients=[
-        common.common_ingredient,
+        logging_ingredient.logging_ingredient,
+        environment.environment_ingredient,
         reward.reward_ingredient,
         rl.rl_ingredient,
-        train.train_ingredient,
+        policy_evaluation.policy_evaluation_ingredient,
     ],
 )
 
 
 MUJOCO_SHARED_LOCALS = dict(rl=dict(rl_kwargs=dict(ent_coef=0.1)))
 ANT_SHARED_LOCALS = dict(
     total_timesteps=int(3e7),
@@ -59,64 +62,64 @@
 
     checkpoint_interval = 0  # Num epochs between saving (<0 disables, =0 final only)
     query_schedule = "hyperbolic"
 
 
 @train_preference_comparisons_ex.named_config
 def cartpole():
-    common = dict(env_name="CartPole-v1")
+    environment = dict(gym_id="CartPole-v1")
     allow_variable_horizon = True
 
 
 @train_preference_comparisons_ex.named_config
 def seals_ant():
     locals().update(**MUJOCO_SHARED_LOCALS)
     locals().update(**ANT_SHARED_LOCALS)
-    common = dict(env_name="seals/Ant-v0")
+    environment = dict(gym_id="seals/Ant-v0")
 
 
 @train_preference_comparisons_ex.named_config
 def half_cheetah():
     locals().update(**MUJOCO_SHARED_LOCALS)
-    common = dict(env_name="HalfCheetah-v2")
+    environment = dict(gym_id="HalfCheetah-v2")
     rl = dict(batch_size=16384, rl_kwargs=dict(batch_size=1024))
 
 
 @train_preference_comparisons_ex.named_config
 def seals_hopper():
     locals().update(**MUJOCO_SHARED_LOCALS)
-    common = dict(env_name="seals/Hopper-v0")
+    environment = dict(gym_id="seals/Hopper-v0")
 
 
 @train_preference_comparisons_ex.named_config
 def seals_humanoid():
     locals().update(**MUJOCO_SHARED_LOCALS)
-    common = dict(env_name="seals/Humanoid-v0")
+    environment = dict(gym_id="seals/Humanoid-v0")
     total_timesteps = int(4e6)
 
 
 @train_preference_comparisons_ex.named_config
 def seals_cartpole():
-    common = dict(env_name="seals/CartPole-v0")
+    environment = dict(gym_id="seals/CartPole-v0")
 
 
 @train_preference_comparisons_ex.named_config
 def pendulum():
-    common = dict(env_name="Pendulum-v1")
+    environment = dict(gym_id="Pendulum-v1")
 
 
 @train_preference_comparisons_ex.named_config
 def mountain_car():
-    common = dict(env_name="MountainCar-v0")
+    environment = dict(gym_id="MountainCar-v0")
     allow_variable_horizon = True
 
 
 @train_preference_comparisons_ex.named_config
 def seals_mountain_car():
-    common = dict(env_name="seals/MountainCar-v0")
+    environment = dict(gym_id="seals/MountainCar-v0")
 
 
 @train_preference_comparisons_ex.named_config
 def fast():
     # Minimize the amount of computation. Useful for test cases.
     total_timesteps = 50
     total_comparisons = 5
```

### Comparing `imitation-0.3.2/src/imitation/scripts/config/train_rl.py` & `imitation-0.4.0/src/imitation/scripts/config/train_rl.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Configuration settings for train_rl, training a policy with RL."""
 
 import sacred
 
-from imitation.scripts.common import common, rl, train
+from imitation.scripts.ingredients import environment
+from imitation.scripts.ingredients import logging as logging_ingredient
+from imitation.scripts.ingredients import policy_evaluation, rl
 
 train_rl_ex = sacred.Experiment(
     "train_rl",
     ingredients=[
-        common.common_ingredient,
-        train.train_ingredient,
+        logging_ingredient.logging_ingredient,
+        environment.environment_ingredient,
         rl.rl_ingredient,
+        policy_evaluation.policy_evaluation_ingredient,
     ],
 )
 
 
 @train_rl_ex.config
 def train_rl_defaults():
     total_timesteps = int(1e6)  # Number of training timesteps in model.learn()
@@ -45,95 +48,95 @@
 
 
 # Standard Gym env configs
 
 
 @train_rl_ex.named_config
 def acrobot():
-    common = dict(env_name="Acrobot-v1")
+    environment = dict(gym_id="Acrobot-v1")
 
 
 @train_rl_ex.named_config
 def ant():
-    common = dict(env_name="Ant-v2")
+    environment = dict(gym_id="Ant-v2")
     rl = dict(batch_size=16384)
     total_timesteps = int(5e6)
 
 
 @train_rl_ex.named_config
 def cartpole():
-    common = dict(env_name="CartPole-v1")
+    environment = dict(gym_id="CartPole-v1")
     total_timesteps = int(1e5)
 
 
 @train_rl_ex.named_config
 def seals_cartpole():
-    common = dict(env_name="seals/CartPole-v0")
+    environment = dict(gym_id="seals/CartPole-v0")
     total_timesteps = int(1e6)
 
 
 @train_rl_ex.named_config
 def half_cheetah():
-    common = dict(env_name="HalfCheetah-v3")
+    environment = dict(gym_id="HalfCheetah-v3")
     total_timesteps = int(5e6)  # does OK after 1e6, but continues improving
 
 
 @train_rl_ex.named_config
 def seals_hopper():
-    common = dict(env_name="seals/Hopper-v0")
+    environment = dict(gym_id="seals/Hopper-v0")
 
 
 @train_rl_ex.named_config
 def seals_humanoid():
-    common = dict(env_name="seals/Humanoid-v0")
+    environment = dict(gym_id="seals/Humanoid-v0")
     rl = dict(batch_size=16384)
     total_timesteps = int(10e6)  # fairly discontinuous, needs at least 5e6
 
 
 @train_rl_ex.named_config
 def mountain_car():
-    common = dict(env_name="MountainCar-v0")
+    environment = dict(gym_id="MountainCar-v0")
 
 
 @train_rl_ex.named_config
 def seals_mountain_car():
-    common = dict(env_name="seals/MountainCar-v0")
+    environment = dict(gym_id="seals/MountainCar-v0")
 
 
 @train_rl_ex.named_config
 def pendulum():
-    common = dict(env_name="Pendulum-v1")
+    environment = dict(gym_id="Pendulum-v1")
     rl = dict(
         batch_size=4096,
         rl_kwargs=dict(
             gamma=0.9,
             learning_rate=1e-3,
         ),
     )
     total_timesteps = int(2e5)
 
 
 @train_rl_ex.named_config
 def reacher():
-    common = dict(env_name="Reacher-v2")
+    environment = dict(gym_id="Reacher-v2")
 
 
 @train_rl_ex.named_config
 def seals_ant():
-    common = dict(env_name="seals/Ant-v0")
+    environment = dict(gym_id="seals/Ant-v0")
 
 
 @train_rl_ex.named_config
 def seals_swimmer():
-    common = dict(env_name="seals/Swimmer-v0")
+    environment = dict(gym_id="seals/Swimmer-v0")
 
 
 @train_rl_ex.named_config
 def seals_walker():
-    common = dict(env_name="seals/Walker2d-v0")
+    environment = dict(gym_id="seals/Walker2d-v0")
 
 
 # Debug configs
 
 
 @train_rl_ex.named_config
 def fast():
```

### Comparing `imitation-0.3.2/src/imitation/scripts/convert_trajs.py` & `imitation-0.4.0/src/imitation/scripts/convert_trajs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,61 @@
-"""Converts old-style pickle trajectories to new-style NPZ trajectories.
+"""Converts old-style pickle or npz trajectories to new-style HuggingFace datasets.
 
 See https://github.com/HumanCompatibleAI/imitation/pull/448 for a description
 of the new trajectory format.
 
 This script takes as command-line input multiple paths to saved trajectories,
-in the old .pkl or new .npz format. It then saves each sequence in the new .npz
-format. The path is the same as the original but with an ".npz" extension
-(i.e. "A.pkl" -> "A.npz", "A.npz" -> "A.npz", "A" -> "A.npz", "A.foo" -> "A.foo.npz").
+in the old .pkl or .npz format. It then saves each sequence in the new HuggingFace
+datasets format. The path is the same as the original but a directory without an
+extension (i.e. "A.pkl" -> "A/", "A.npz" -> "A/", "A/" -> "A/", "A.foo" -> "A/").
 """
 
+import pathlib
 import warnings
 
-from imitation.data import types
+from imitation.data import huggingface_utils, serialize, types
+from imitation.util import util
 
 
-def update_traj_file_in_place(path_str: str, /) -> None:
-    """Modifies trajectories pickle file in-place to update data to new format.
+def update_traj_file_in_place(path_str: types.AnyPath, /) -> pathlib.Path:
+    """Converts pickle or npz file to the new HuggingFace format.
 
     The new data is saved as `Sequence[imitation.types.TrajectoryWithRew]`.
 
     Args:
-        path_str: Path to a pickle file containing
+        path_str: Path to a pickle or npz file containing
             `Sequence[imitation.types.Trajectory]`
             or `Sequence[imitation.old_types.TrajectoryWithRew]`.
+
+    Returns:
+        The path to the converted trajectory dataset.
     """
-    path = types.parse_path(path_str)
+    path = util.parse_path(path_str)
     with warnings.catch_warnings():
         # Filter out DeprecationWarning because we expect to load old trajectories here.
         warnings.filterwarnings(
             "ignore",
-            message="Loading old version of Trajectory.*",
+            message="Loading old .* version of Trajectories.*",
             category=DeprecationWarning,
         )
-        trajs = types.load(path)
+        trajs = serialize.load(path)
 
-    ext = path.suffix
-    new_ext = ".npz" if ext in (".pkl", ".npz") else ext + ".npz"
-    types.save(path.with_suffix(new_ext), trajs)
+    if isinstance(
+        trajs,
+        huggingface_utils.TrajectoryDatasetSequence,
+    ):
+        warnings.warn(f"File {path} is already in the new format. Skipping.")
+        return path
+    else:
+        converted_path = path.with_suffix("")
+        serialize.save(converted_path, trajs)
+        return converted_path
 
 
-def main():
+def main():  # pragma: no cover
     import sys
 
     if len(sys.argv) <= 1:
         print("Supply at least one path to pickled trajectories.")
     else:
         for path in sys.argv[1:]:
             update_traj_file_in_place(path)
```

### Comparing `imitation-0.3.2/src/imitation/scripts/eval_policy.py` & `imitation-0.4.0/src/imitation/scripts/eval_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 import logging
 import pathlib
 import time
 from typing import Any, Mapping, Optional
 
 import gym
+import numpy as np
 from sacred.observers import FileStorageObserver
 from stable_baselines3.common.vec_env import VecEnvWrapper
 
-from imitation.data import rollout, types
+from imitation.data import rollout, serialize
 from imitation.policies.exploration_wrapper import ExplorationWrapper
 from imitation.rewards import reward_wrapper
 from imitation.rewards.serialize import load_reward
-from imitation.scripts.common import common, expert
 from imitation.scripts.config.eval_policy import eval_policy_ex
+from imitation.scripts.ingredients import environment, expert
+from imitation.scripts.ingredients import logging as logging_ingredient
 from imitation.util import video_wrapper
 
 
 class InteractiveRender(VecEnvWrapper):
     """Render the wrapped environment(s) on screen."""
 
     def __init__(self, venv, fps):
@@ -48,21 +50,22 @@
         return video_wrapper.VideoWrapper(env, directory=directory, **kwargs)
 
     return f
 
 
 @eval_policy_ex.main
 def eval_policy(
-    _run,
     eval_n_timesteps: Optional[int],
     eval_n_episodes: Optional[int],
     render: bool,
     render_fps: int,
     videos: bool,
     video_kwargs: Mapping[str, Any],
+    _run,
+    _rnd: np.random.Generator,
     reward_type: Optional[str] = None,
     reward_path: Optional[str] = None,
     rollout_save_path: Optional[str] = None,
     explore_kwargs: Optional[Mapping[str, Any]] = None,
 ):
     """Rolls a policy out in an environment, collecting statistics.
 
@@ -71,56 +74,56 @@
             one of `eval_n_episodes` and `eval_n_timesteps`.
         eval_n_episodes: Minimum number of episodes to evaluate for. Set exactly
             one of `eval_n_episodes` and `eval_n_timesteps`.
         render: If True, renders interactively to the screen.
         render_fps: The target number of frames per second to render on screen.
         videos: If True, saves videos to `log_dir`.
         video_kwargs: Keyword arguments passed through to `video_wrapper.VideoWrapper`.
+        _rnd: Random number generator provided by Sacred.
         reward_type: If specified, overrides the environment reward with
             a reward of this.
         reward_path: If reward_type is specified, the path to a serialized reward
             of `reward_type` to override the environment reward with.
         rollout_save_path: where to save rollouts used for computing stats to disk;
             if None, then do not save.
         explore_kwargs: keyword arguments to an exploration wrapper to apply before
             rolling out, not including policy_callable, venv, and rng; if None, then
             do not wrap.
 
     Returns:
         Return value of `imitation.util.rollout.rollout_stats()`.
     """
-    rng = common.make_rng()
-    log_dir = common.make_log_dir()
+    log_dir = logging_ingredient.make_log_dir()
     sample_until = rollout.make_sample_until(eval_n_timesteps, eval_n_episodes)
     post_wrappers = [video_wrapper_factory(log_dir, **video_kwargs)] if videos else None
-    with common.make_venv(post_wrappers=post_wrappers) as venv:
+    with environment.make_venv(post_wrappers=post_wrappers) as venv:
         if render:
             venv = InteractiveRender(venv, render_fps)
 
         if reward_type is not None:
             reward_fn = load_reward(reward_type, reward_path, venv)
             venv = reward_wrapper.RewardVecEnvWrapper(venv, reward_fn)
             logging.info(f"Wrapped env in reward {reward_type} from {reward_path}.")
 
         policy = expert.get_expert_policy(venv)
         if explore_kwargs is not None:
             policy = ExplorationWrapper(
                 policy,
                 venv,
-                rng=rng,
+                rng=_rnd,
                 **explore_kwargs,
             )
             log_str = (
                 f"Wrapped policy in ExplorationWrapper with kwargs {explore_kwargs}"
             )
             logging.info(log_str)
-        trajs = rollout.generate_trajectories(policy, venv, sample_until, rng=rng)
+        trajs = rollout.generate_trajectories(policy, venv, sample_until, rng=_rnd)
 
     if rollout_save_path:
-        types.save(log_dir / rollout_save_path.replace("{log_dir}/", ""), trajs)
+        serialize.save(log_dir / rollout_save_path.replace("{log_dir}/", ""), trajs)
 
     return rollout.rollout_stats(trajs)
 
 
 def main_console():
     observer_path = pathlib.Path.cwd() / "output" / "sacred" / "eval_policy"
     observer = FileStorageObserver(observer_path)
```

### Comparing `imitation-0.3.2/src/imitation/scripts/parallel.py` & `imitation-0.4.0/src/imitation/scripts/parallel.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/scripts/train_adversarial.py` & `imitation-0.4.0/src/imitation/scripts/train_adversarial.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 from sacred.observers import FileStorageObserver
 
 from imitation.algorithms.adversarial import airl as airl_algo
 from imitation.algorithms.adversarial import common
 from imitation.algorithms.adversarial import gail as gail_algo
 from imitation.data import rollout
 from imitation.policies import serialize
-from imitation.scripts.common import common as common_config
-from imitation.scripts.common import demonstrations, reward, rl, train
 from imitation.scripts.config.train_adversarial import train_adversarial_ex
+from imitation.scripts.ingredients import demonstrations, environment
+from imitation.scripts.ingredients import logging as logging_ingredient
+from imitation.scripts.ingredients import policy_evaluation, reward, rl
 
 logger = logging.getLogger("imitation.scripts.train_adversarial")
 
 
 def save(trainer: common.AdversarialTrainer, save_path: pathlib.Path):
     """Save discriminator and generator."""
     # We implement this here and not in Trainer since we do not want to actually
@@ -101,23 +102,28 @@
     Returns:
         A dictionary with two keys. "imit_stats" gives the return value of
         `rollout_stats()` on rollouts test-reward-wrapped environment, using the final
         policy (remember that the ground-truth reward can be recovered from the
         "monitor_return" key). "expert_stats" gives the return value of
         `rollout_stats()` on the expert demonstrations.
     """
+    # This allows to specify total_timesteps and checkpoint_interval in scientific
+    # notation, which is interpreted as a float by python.
+    total_timesteps = int(total_timesteps)
+    checkpoint_interval = int(checkpoint_interval)
+
     if show_config:
         # Running `train_adversarial print_config` will show unmerged config.
         # So, support showing merged config from `train_adversarial {airl,gail}`.
         sacred.commands.print_config(_run)
 
-    custom_logger, log_dir = common_config.setup_logging()
+    custom_logger, log_dir = logging_ingredient.setup_logging()
     expert_trajs = demonstrations.get_expert_trajectories()
 
-    with common_config.make_venv() as venv:
+    with environment.make_venv() as venv:
         reward_net = reward.make_reward_net(venv)
         relabel_reward_fn = functools.partial(
             reward_net.predict_processed,
             update_stats=False,
         )
 
         if agent_path is None:
@@ -148,15 +154,15 @@
         )
 
         def callback(round_num: int, /) -> None:
             if checkpoint_interval > 0 and round_num % checkpoint_interval == 0:
                 save(trainer, log_dir / "checkpoints" / f"{round_num:05d}")
 
         trainer.train(total_timesteps, callback)
-        imit_stats = train.eval_policy(trainer.policy, trainer.venv_train)
+        imit_stats = policy_evaluation.eval_policy(trainer.policy, trainer.venv_train)
 
     # Save final artifacts.
     if checkpoint_interval >= 0:
         save(trainer, log_dir / "checkpoints" / "final")
 
     return {
         "imit_stats": imit_stats,
```

### Comparing `imitation-0.3.2/src/imitation/scripts/train_imitation.py` & `imitation-0.4.0/src/imitation/scripts/train_rl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,179 +1,172 @@
-"""Trains DAgger on synthetic demonstrations generated from an expert policy."""
+"""Uses RL to train a policy from scratch, saving rollouts and policy.
+
+This can be used:
+    1. To train a policy on a ground-truth reward function, as a source of
+       synthetic "expert" demonstrations to train IRL or imitation learning
+       algorithms.
+    2. To train a policy on a learned reward function, to solve a task or
+       as a way of evaluating the quality of the learned reward function.
+"""
 
 import logging
-import os.path as osp
 import pathlib
 import warnings
-from typing import Any, Mapping, Optional, Sequence, Type, cast
+from typing import Any, Mapping, Optional
 
+import numpy as np
 from sacred.observers import FileStorageObserver
-from stable_baselines3.common import policies, utils, vec_env
+from stable_baselines3.common import callbacks
+from stable_baselines3.common.vec_env import VecNormalize
 
-from imitation.algorithms import bc as bc_algorithm
-from imitation.algorithms.dagger import SimpleDAggerTrainer
-from imitation.data import rollout, types
-from imitation.scripts.common import common, demonstrations, expert, train
-from imitation.scripts.config.train_imitation import train_imitation_ex
-
-logger = logging.getLogger(__name__)
-
-
-@train_imitation_ex.capture(prefix="train")
-def make_policy(
-    venv: vec_env.VecEnv,
-    policy_cls: Type[policies.BasePolicy],
-    policy_kwargs: Mapping[str, Any],
+import imitation.data.serialize as data_serialize
+import imitation.policies.serialize as policies_serialize
+from imitation.data import rollout, wrappers
+from imitation.rewards.reward_wrapper import RewardVecEnvWrapper
+from imitation.rewards.serialize import load_reward
+from imitation.scripts.config.train_rl import train_rl_ex
+from imitation.scripts.ingredients import environment
+from imitation.scripts.ingredients import logging as logging_ingredient
+from imitation.scripts.ingredients import policy_evaluation, rl
+
+
+@train_rl_ex.main
+def train_rl(
+    *,
+    total_timesteps: int,
+    normalize_reward: bool,
+    normalize_kwargs: dict,
+    reward_type: Optional[str],
+    reward_path: Optional[str],
+    load_reward_kwargs: Optional[Mapping[str, Any]],
+    rollout_save_final: bool,
+    rollout_save_n_timesteps: Optional[int],
+    rollout_save_n_episodes: Optional[int],
+    policy_save_interval: int,
+    policy_save_final: bool,
     agent_path: Optional[str],
-) -> policies.BasePolicy:
-    """Makes policy.
-
-    Args:
-        venv: Vectorized environment we will be imitating demos from.
-        policy_cls: Type of a Stable Baselines3 policy architecture.
-            Specify only if policy_path is not specified.
-        policy_kwargs: Keyword arguments for policy constructor.
-            Specify only if policy_path is not specified.
-        agent_path: Path to serialized policy. If provided, then load the
-            policy from this path. Otherwise, make a new policy.
-            Specify only if policy_cls and policy_kwargs are not specified.
+    _rnd: np.random.Generator,
+) -> Mapping[str, float]:
+    """Trains an expert policy from scratch and saves the rollouts and policy.
+
+    Checkpoints:
+      At applicable training steps `step` (where step is either an integer or
+      "final"):
 
-    Returns:
-        A Stable Baselines3 policy.
-    """
-    policy_kwargs = dict(policy_kwargs)
-    if issubclass(policy_cls, policies.ActorCriticPolicy):
-        policy_kwargs.update(
-            {
-                "observation_space": venv.observation_space,
-                "action_space": venv.action_space,
-                # parameter mandatory for ActorCriticPolicy, but not used by BC
-                "lr_schedule": utils.get_schedule_fn(1),
-            },
-        )
-    policy: policies.BasePolicy
-    if agent_path is not None:
-        warnings.warn(
-            "When agent_path is specified, policy_cls and policy_kwargs are ignored.",
-            RuntimeWarning,
-        )
-        policy = bc_algorithm.reconstruct_policy(agent_path)
-    else:
-        policy = policy_cls(**policy_kwargs)
-    logger.info(f"Policy network summary:\n {policy}")
-    return policy
-
-
-@train_imitation_ex.capture
-def train_imitation(
-    _run,
-    bc_kwargs: Mapping[str, Any],
-    bc_train_kwargs: Mapping[str, Any],
-    dagger: Mapping[str, Any],
-    use_dagger: bool,
-    agent_path: Optional[str],
-) -> Mapping[str, Mapping[str, float]]:
-    """Runs DAgger (if `use_dagger`) or BC (otherwise) training.
+        - Policies are saved to `{log_dir}/policies/{step}/`.
+        - Rollouts are saved to `{log_dir}/rollouts/{step}.npz`.
 
     Args:
-        bc_kwargs: Keyword arguments passed through to `bc.BC` constructor.
-        bc_train_kwargs: Keyword arguments passed through to `BC.train()` method.
-        dagger: Arguments for DAgger training.
-        use_dagger: If True, train using DAgger; otherwise, use BC.
-        agent_path: Path to serialized policy. If provided, then load the
-            policy from this path. Otherwise, make a new policy.
-            Specify only if policy_cls and policy_kwargs are not specified.
+        total_timesteps: Number of training timesteps in `model.learn()`.
+        normalize_reward: Applies normalization and clipping to the reward function by
+            keeping a running average of training rewards. Note: this is may be
+            redundant if using a learned reward that is already normalized.
+        normalize_kwargs: kwargs for `VecNormalize`.
+        reward_type: If provided, then load the serialized reward of this type,
+            wrapping the environment in this reward. This is useful to test
+            whether a reward model transfers. For more information, see
+            `imitation.rewards.serialize.load_reward`.
+        reward_path: A specifier, such as a path to a file on disk, used by
+            reward_type to load the reward model. For more information, see
+            `imitation.rewards.serialize.load_reward`.
+        load_reward_kwargs: Additional kwargs to pass to `predict_processed`.
+            Examples are 'alpha' for :class: `AddSTDRewardWrapper` and 'update_stats'
+            for :class: `NormalizedRewardNet`.
+        rollout_save_final: If True, then save rollouts right after training is
+            finished.
+        rollout_save_n_timesteps: The minimum number of timesteps saved in every
+            file. Could be more than `rollout_save_n_timesteps` because
+            trajectories are saved by episode rather than by transition.
+            Must set exactly one of `rollout_save_n_timesteps`
+            and `rollout_save_n_episodes`.
+        rollout_save_n_episodes: The number of episodes saved in every
+            file. Must set exactly one of `rollout_save_n_timesteps` and
+            `rollout_save_n_episodes`.
+        policy_save_interval: The number of training updates between in between
+            intermediate rollout saves. If the argument is nonpositive, then
+            don't save intermediate updates.
+        policy_save_final: If True, then save the policy right after training is
+            finished.
+        agent_path: Path to load warm-started agent.
+        _rnd: Random number generator provided by Sacred.
 
     Returns:
-        Statistics for rollouts from the trained policy and demonstration data.
+        The return value of `rollout_stats()` using the final policy.
     """
-    rng = common.make_rng()
-    custom_logger, log_dir = common.setup_logging()
-
-    with common.make_venv() as venv:
-        imit_policy = make_policy(venv, agent_path=agent_path)
-
-        expert_trajs: Optional[Sequence[types.Trajectory]] = None
-        if not use_dagger or dagger["use_offline_rollouts"]:
-            expert_trajs = demonstrations.get_expert_trajectories()
-
-        bc_trainer = bc_algorithm.BC(
-            observation_space=venv.observation_space,
-            action_space=venv.action_space,
-            policy=imit_policy,
-            demonstrations=expert_trajs,
-            custom_logger=custom_logger,
-            rng=rng,
-            **bc_kwargs,
-        )
-        bc_train_kwargs = dict(log_rollouts_venv=venv, **bc_train_kwargs)
-        if bc_train_kwargs["n_epochs"] is None and bc_train_kwargs["n_batches"] is None:
-            if use_dagger:
-                bc_train_kwargs["n_epochs"] = 4
-            else:
-                bc_train_kwargs["n_batches"] = 50_000
-
-        if use_dagger:
-            expert_policy = expert.get_expert_policy(venv)
-            model = SimpleDAggerTrainer(
-                venv=venv,
-                scratch_dir=osp.join(log_dir, "scratch"),
-                expert_trajs=expert_trajs,
-                expert_policy=expert_policy,
-                custom_logger=custom_logger,
-                bc_trainer=bc_trainer,
-                rng=rng,
+    custom_logger, log_dir = logging_ingredient.setup_logging()
+    rollout_dir = log_dir / "rollouts"
+    policy_dir = log_dir / "policies"
+    rollout_dir.mkdir(parents=True, exist_ok=True)
+    policy_dir.mkdir(parents=True, exist_ok=True)
+
+    post_wrappers = [lambda env, idx: wrappers.RolloutInfoWrapper(env)]
+    with environment.make_venv(post_wrappers=post_wrappers) as venv:
+        callback_objs = []
+        if reward_type is not None:
+            reward_fn = load_reward(
+                reward_type,
+                reward_path,
+                venv,
+                **load_reward_kwargs,
             )
-            model.train(
-                total_timesteps=int(dagger["total_timesteps"]),
-                bc_train_kwargs=bc_train_kwargs,
+            venv = RewardVecEnvWrapper(venv, reward_fn)
+            callback_objs.append(venv.make_log_callback())
+            logging.info(f"Wrapped env in reward {reward_type} from {reward_path}.")
+
+        if normalize_reward:
+            # Normalize reward. Reward scale effectively changes the learning rate,
+            # so normalizing it makes training more stable. Note we do *not* normalize
+            # observations here; use the `NormalizeFeaturesExtractor` instead.
+            venv = VecNormalize(venv, norm_obs=False, **normalize_kwargs)
+            if reward_type == "RewardNet_normalized":
+                warnings.warn(
+                    "Applying normalization to already normalized reward function. \
+                    Consider setting normalize_reward as False",
+                    RuntimeWarning,
+                )
+
+        if policy_save_interval > 0:
+            save_policy_callback: callbacks.EventCallback = (
+                policies_serialize.SavePolicyCallback(policy_dir)
             )
-            # TODO(adam): add checkpointing to DAgger?
-            save_locations = model.save_trainer()
-            print(f"Model saved to {save_locations}")
-        else:
-            bc_trainer.train(**bc_train_kwargs)
-            # TODO(adam): add checkpointing to BC?
-            bc_trainer.save_policy(policy_path=osp.join(log_dir, "final.th"))
-
-        imit_stats = train.eval_policy(imit_policy, venv)
-
-    stats = {"imit_stats": imit_stats}
-    trajectories = model._all_demos if use_dagger else expert_trajs
-    assert trajectories is not None
-    if all(isinstance(t, types.TrajectoryWithRew) for t in trajectories):
-        expert_stats = rollout.rollout_stats(
-            cast(Sequence[types.TrajectoryWithRew], trajectories),
-        )
-        stats["expert_stats"] = expert_stats
-    return stats
-
-
-@train_imitation_ex.command
-def bc() -> Mapping[str, Mapping[str, float]]:
-    """Run BC experiment using a Sacred interface to BC.
-
-    Returns:
-        Statistics for rollouts from the trained policy and expert data.
-    """
-    return train_imitation(use_dagger=False)
-
+            save_policy_callback = callbacks.EveryNTimesteps(
+                policy_save_interval,
+                save_policy_callback,
+            )
+            callback_objs.append(save_policy_callback)
+        callback = callbacks.CallbackList(callback_objs)
 
-@train_imitation_ex.command
-def dagger() -> Mapping[str, Mapping[str, float]]:
-    """Run synthetic DAgger experiment using a Sacred interface to SimpleDAggerTrainer.
+        if agent_path is None:
+            rl_algo = rl.make_rl_algo(venv)
+        else:
+            rl_algo = rl.load_rl_algo_from_path(agent_path=agent_path, venv=venv)
+        rl_algo.set_logger(custom_logger)
+        rl_algo.learn(total_timesteps, callback=callback)
+
+        # Save final artifacts after training is complete.
+        if rollout_save_final:
+            save_path = rollout_dir / "final.npz"
+            sample_until = rollout.make_sample_until(
+                rollout_save_n_timesteps,
+                rollout_save_n_episodes,
+            )
+            data_serialize.save(
+                save_path,
+                rollout.rollout(rl_algo, rl_algo.get_env(), sample_until, rng=_rnd),
+            )
+        if policy_save_final:
+            output_dir = policy_dir / "final"
+            policies_serialize.save_stable_model(output_dir, rl_algo)
 
-    Returns:
-        Statistics for rollouts from the trained policy and expert data.
-    """
-    return train_imitation(use_dagger=True)
+        # Final evaluation of expert policy.
+        return policy_evaluation.eval_policy(rl_algo, venv)
 
 
 def main_console():
-    observer_path = pathlib.Path.cwd() / "output" / "sacred" / "train_dagger"
+    observer_path = pathlib.Path.cwd() / "output" / "sacred" / "train_rl"
     observer = FileStorageObserver(observer_path)
-    train_imitation_ex.observers.append(observer)
-    train_imitation_ex.run_commandline()
+    train_rl_ex.observers.append(observer)
+    train_rl_ex.run_commandline()
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     main_console()
```

### Comparing `imitation-0.3.2/src/imitation/scripts/train_preference_comparisons.py` & `imitation-0.4.0/src/imitation/scripts/train_preference_comparisons.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 can be called directly.
 """
 
 import functools
 import pathlib
 from typing import Any, Mapping, Optional, Type, Union
 
+import numpy as np
 import torch as th
 from sacred.observers import FileStorageObserver
 from stable_baselines3.common import type_aliases
 
+import imitation.data.serialize as data_serialize
+import imitation.policies.serialize as policies_serialize
 from imitation.algorithms import preference_comparisons
-from imitation.data import types
-from imitation.policies import serialize
-from imitation.scripts.common import common, reward
-from imitation.scripts.common import rl as rl_common
-from imitation.scripts.common import train
 from imitation.scripts.config.train_preference_comparisons import (
     train_preference_comparisons_ex,
 )
+from imitation.scripts.ingredients import environment
+from imitation.scripts.ingredients import logging as logging_ingredient
+from imitation.scripts.ingredients import policy_evaluation, reward
+from imitation.scripts.ingredients import rl as rl_common
 
 
 def save_model(
     agent_trainer: preference_comparisons.AgentTrainer,
     save_path: pathlib.Path,
 ):
     """Save the model as `model.zip`."""
-    serialize.save_stable_model(
+    policies_serialize.save_stable_model(
         output_dir=save_path / "policy",
         model=agent_trainer.algorithm,
     )
 
 
 def save_checkpoint(
     trainer: preference_comparisons.PreferenceComparisons,
@@ -78,14 +80,15 @@
     active_selection: bool,
     active_selection_oversampling: int,
     uncertainty_on: str,
     fragmenter_kwargs: Mapping[str, Any],
     allow_variable_horizon: bool,
     checkpoint_interval: int,
     query_schedule: Union[str, type_aliases.Schedule],
+    _rnd: np.random.Generator,
 ) -> Mapping[str, Any]:
     """Train a reward model using preference comparisons.
 
     Args:
         total_timesteps: number of environment interaction steps
         total_comparisons: number of preferences to gather in total
         num_iterations: number of times to train the agent against the reward model
@@ -137,25 +140,37 @@
             iterations and after training is complete. If 0, then only save weights
             after training is complete. If <0, then don't save weights at all.
         query_schedule: one of ("constant", "hyperbolic", "inverse_quadratic").
             A function indicating how the total number of preference queries should
             be allocated to each iteration. "hyperbolic" and "inverse_quadratic"
             apportion fewer queries to later iterations when the policy is assumed
             to be better and more stable.
+        _rnd: Random number generator provided by Sacred.
 
     Returns:
         Rollout statistics from trained policy.
 
     Raises:
         ValueError: Inconsistency between config and deserialized policy normalization.
     """
-    custom_logger, log_dir = common.setup_logging()
-    rng = common.make_rng()
+    # This allows to specify total_timesteps, total_comparisons etc. in scientific
+    # notation, which is interpreted as a float by python.
+    total_timesteps = int(total_timesteps)
+    total_comparisons = int(total_comparisons)
+    num_iterations = int(num_iterations)
+    comparison_queue_size = (
+        int(comparison_queue_size) if comparison_queue_size is not None else None
+    )
+    fragment_length = int(fragment_length)
+    active_selection_oversampling = int(active_selection_oversampling)
+    checkpoint_interval = int(checkpoint_interval)
+
+    custom_logger, log_dir = logging_ingredient.setup_logging()
 
-    with common.make_venv() as venv:
+    with environment.make_venv() as venv:
         reward_net = reward.make_reward_net(venv)
         relabel_reward_fn = functools.partial(
             reward_net.predict_processed,
             update_stats=False,
         )
         if agent_path is None:
             agent = rl_common.make_rl_algo(venv, relabel_reward_fn=relabel_reward_fn)
@@ -170,15 +185,15 @@
             # Setting the logger here is not necessary (PreferenceComparisons takes care
             # of it automatically) but it avoids creating unnecessary loggers.
             agent_trainer = preference_comparisons.AgentTrainer(
                 algorithm=agent,
                 reward_fn=reward_net,
                 venv=venv,
                 exploration_frac=exploration_frac,
-                rng=rng,
+                rng=_rnd,
                 custom_logger=custom_logger,
                 **trajectory_generator_kwargs,
             )
             # Stable Baselines will automatically occupy GPU 0 if it is available.
             # Let's use the same device as the SB3 agent for the reward model.
             reward_net = reward_net.to(agent_trainer.algorithm.device)
             trajectory_generator: preference_comparisons.TrajectoryGenerator = (
@@ -186,24 +201,26 @@
             )
         else:
             if exploration_frac > 0:
                 raise ValueError(
                     "exploration_frac can't be set when a trajectory dataset is used",
                 )
             trajectory_generator = preference_comparisons.TrajectoryDataset(
-                trajectories=types.load_with_rewards(trajectory_path),
-                rng=rng,
+                trajectories=data_serialize.load_with_rewards(
+                    trajectory_path,
+                ),
+                rng=_rnd,
                 custom_logger=custom_logger,
                 **trajectory_generator_kwargs,
             )
 
         fragmenter: preference_comparisons.Fragmenter = (
             preference_comparisons.RandomFragmenter(
                 **fragmenter_kwargs,
-                rng=rng,
+                rng=_rnd,
                 custom_logger=custom_logger,
             )
         )
         preference_model = preference_comparisons.PreferenceModel(
             **preference_model_kwargs,
             model=reward_net,
         )
@@ -213,24 +230,24 @@
                 base_fragmenter=fragmenter,
                 fragment_sample_factor=active_selection_oversampling,
                 uncertainty_on=uncertainty_on,
                 custom_logger=custom_logger,
             )
         gatherer = gatherer_cls(
             **gatherer_kwargs,
-            rng=rng,
+            rng=_rnd,
             custom_logger=custom_logger,
         )
 
         loss = preference_comparisons.CrossEntropyRewardLoss()
 
         reward_trainer = preference_comparisons._make_reward_trainer(
             preference_model,
             loss,
-            rng,
+            _rnd,
             reward_trainer_kwargs,
         )
 
         main_trainer = preference_comparisons.PreferenceComparisons(
             trajectory_generator,
             reward_net,
             num_iterations=num_iterations,
@@ -259,15 +276,15 @@
             total_comparisons,
             callback=save_callback,
         )
 
         # Storing and evaluating policy only useful if we generated trajectory data
         if bool(trajectory_path is None):
             results = dict(results)
-            results["rollout"] = train.eval_policy(agent, venv)
+            results["rollout"] = policy_evaluation.eval_policy(agent, venv)
 
     if save_preferences:
         main_trainer.dataset.save(log_dir / "preferences.pkl")
 
     # Save final artifacts.
     if checkpoint_interval >= 0:
         save_checkpoint(
```

### Comparing `imitation-0.3.2/src/imitation/testing/expert_trajectories.py` & `imitation-0.4.0/src/imitation/testing/expert_trajectories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Test utilities to conveniently generate expert trajectories."""
 import math
 import pathlib
 import pickle
+import shutil
 import warnings
 from os import PathLike
 from pathlib import Path
 from typing import Sequence
 
 import huggingface_sb3 as hfsb3
 import numpy as np
 from filelock import FileLock
 from torch.utils import data as th_data
 
+import imitation.data.serialize as data_serialize
+import imitation.policies.serialize as policies_serialize
 from imitation.data import rollout, types, wrappers
-from imitation.policies import serialize
 from imitation.util import util
 
 
 def generate_expert_trajectories(
     env_id: str,
     num_trajectories: int,
     rng: np.random.Generator,
@@ -36,15 +38,15 @@
     """
     env = util.make_vec_env(
         env_id,
         post_wrappers=[lambda e, _: wrappers.RolloutInfoWrapper(e)],
         rng=rng,
     )
     try:
-        expert = serialize.load_policy("ppo-huggingface", env, env_name=env_id)
+        expert = policies_serialize.load_policy("ppo-huggingface", env, env_name=env_id)
         return rollout.rollout(
             expert,
             env,
             rollout.make_sample_until(min_episodes=num_trajectories),
             rng=rng,
         )
     finally:
@@ -68,38 +70,44 @@
 
     Returns:
         A list of trajectories with rewards.
     """
     environment_cache_path = pathlib.Path(cache_path) / hfsb3.EnvironmentName(env_id)
     environment_cache_path.mkdir(parents=True, exist_ok=True)
 
-    trajectories_path = environment_cache_path / "rollout.npz"
+    trajectories_path = environment_cache_path / "rollout"
 
     # Note: we cast to str here because FileLock doesn't support pathlib.Path.
-    with FileLock(str(environment_cache_path / "rollout.npz.lock")):
+    with FileLock(str(environment_cache_path / "rollout.lock")):
         try:
-            trajectories = types.load_with_rewards(trajectories_path)
+            trajectories = data_serialize.load_with_rewards(trajectories_path)
         except (FileNotFoundError, pickle.PickleError) as e:  # pragma: no cover
             generation_reason = (
                 "the cache is cold"
                 if isinstance(e, FileNotFoundError)
                 else "trajectory file format in the cache is outdated"
             )
             warnings.warn(
                 f"Generating expert trajectories for {env_id} because "
                 f"{generation_reason}.",
             )
             trajectories = generate_expert_trajectories(env_id, num_trajectories, rng)
-            types.save(trajectories_path, trajectories)
+            data_serialize.save(trajectories_path, trajectories)
 
     if len(trajectories) >= num_trajectories:
         return trajectories[:num_trajectories]
     else:  # pragma: no cover
         # If it is not enough, just throw away the cache and generate more.
-        trajectories_path.unlink()
+        if trajectories_path.is_dir():
+            # rmtree won't remove directory on Windows
+            # until the last handle to the directory is closed
+            del trajectories
+            shutil.rmtree(trajectories_path)
+        else:
+            trajectories_path.unlink()
         return lazy_generate_expert_trajectories(
             cache_path,
             env_id,
             num_trajectories,
             rng,
         )
```

### Comparing `imitation-0.3.2/src/imitation/testing/reward_improvement.py` & `imitation-0.4.0/src/imitation/testing/reward_improvement.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/testing/reward_nets.py` & `imitation-0.4.0/src/imitation/testing/reward_nets.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/util/logger.py` & `imitation-0.4.0/src/imitation/util/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sys
 import tempfile
 from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, Union
 
 import stable_baselines3.common.logger as sb_logger
 
 from imitation.data import types
+from imitation.util import util
 
 
 def make_output_format(
     _format: str,
     log_dir: str,
     log_suffix: str = "",
     max_length: int = 50,
@@ -265,20 +266,19 @@
         subdir = os.path.join(*self._accumulate_prefixes, name)
 
         if subdir in self._cached_loggers:
             logger = self._cached_loggers[subdir]
         else:
             default_logger_dir = self.default_logger.dir
             assert default_logger_dir is not None
-            folder = types.parse_path(default_logger_dir) / "raw" / subdir
+            folder = util.parse_path(default_logger_dir) / "raw" / subdir
             folder.mkdir(exist_ok=True, parents=True)
             output_formats = _build_output_formats(folder, self.format_strs)
             logger = sb_logger.Logger(str(folder), list(output_formats))
             self._cached_loggers[subdir] = logger
-
         try:
             self.current_logger = logger
             self._subdir = subdir
             self._name = name
             self._update_name_to_maps()
             yield
         finally:
@@ -398,20 +398,20 @@
         format_strs: An list of output format strings. For details on available
             output formats see `stable_baselines3.logger.make_output_format`.
 
     Returns:
         The configured HierarchicalLogger instance.
     """
     if folder is None:
-        tempdir = types.parse_path(tempfile.gettempdir())
+        tempdir = util.parse_path(tempfile.gettempdir())
         now = datetime.datetime.now()
         timestamp = now.strftime("imitation-%Y-%m-%d-%H-%M-%S-%f")
         folder = tempdir / timestamp
     else:
-        folder = types.parse_path(folder)
+        folder = util.parse_path(folder)
     if format_strs is None:
         format_strs = ["stdout", "log", "csv"]
     output_formats = _build_output_formats(folder, format_strs)
     default_logger = sb_logger.Logger(str(folder), list(output_formats))
     hier_format_strs = [f for f in format_strs if f != "wandb"]
     hier_logger = HierarchicalLogger(default_logger, hier_format_strs)
     return hier_logger
```

### Comparing `imitation-0.3.2/src/imitation/util/networks.py` & `imitation-0.4.0/src/imitation/util/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,29 +82,34 @@
             # Do not backpropagate through updating running mean and variance.
             # These updates are in-place and not differentiable. The gradient
             # is not needed as the running mean and variance are updated
             # directly by this function, and not by gradient descent.
             with th.no_grad():
                 self.update_stats(x)
 
+        # Note: this is different from the behavior in stable-baselines, see
+        # https://github.com/HumanCompatibleAI/imitation/issues/442
         return (x - self.running_mean) / th.sqrt(self.running_var + self.eps)
 
     @abc.abstractmethod
     def update_stats(self, batch: th.Tensor) -> None:
         """Update `self.running_mean`, `self.running_var` and `self.count`."""
 
 
 class RunningNorm(BaseNorm):
     """Normalizes input to mean 0 and standard deviation 1 using a running average.
 
     Similar to BatchNorm, LayerNorm, etc. but whereas they only use statistics from
     the current batch at train time, we use statistics from all batches.
 
-    This should closely replicate the common practice in RL of normalizing environment
-    observations, such as using `VecNormalize` in Stable Baselines.
+    This should replicate the common practice in RL of normalizing environment
+    observations, such as using ``VecNormalize`` in Stable Baselines. Note that
+    the behavior of this class is slightly different from `VecNormalize`, e.g.,
+    it works with the current reward instead of return estimate, and subtracts the mean
+    reward whereas ``VecNormalize`` only rescales it.
     """
 
     def update_stats(self, batch: th.Tensor) -> None:
         """Update `self.running_mean`, `self.running_var` and `self.count`.
 
         Uses Chan et al (1979), "Updating Formulae and a Pairwise Algorithm for
         Computing Sample Variances." to update the running moments in a numerically
```

### Comparing `imitation-0.3.2/src/imitation/util/registry.py` & `imitation-0.4.0/src/imitation/util/registry.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/src/imitation/util/sacred.py` & `imitation-0.4.0/src/imitation/util/sacred.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Callable, NamedTuple, Optional, Sequence
 
 import sacred
 import sacred.observers
 import sacred.run
 
 from imitation.data import types
+from imitation.util import util
 
 
 class SacredDicts(NamedTuple):
     """Each dict `foo` is loaded from `f"{sacred_dir}/foo.json"`."""
 
     sacred_dir: pathlib.Path
     config: dict
@@ -73,15 +74,15 @@
                         f"Found nested directories: {dirpath} and {other_dirpath}",
                     )
     return list(filtered_dirs)
 
 
 def build_sacred_symlink(log_dir: types.AnyPath, run: sacred.run.Run) -> None:
     """Constructs a symlink "{log_dir}/sacred" => "${SACRED_PATH}"."""
-    log_dir = types.parse_path(log_dir)
+    log_dir = util.parse_path(log_dir)
 
     sacred_dir = get_sacred_dir_from_run(run)
     if sacred_dir is None:
         warnings.warn(RuntimeWarning("Couldn't find sacred directory."))
         return
     symlink_path = log_dir / "sacred"
     target_path = pathlib.Path(os.path.relpath(sacred_dir, start=log_dir))
@@ -111,15 +112,15 @@
             raise e
 
 
 def get_sacred_dir_from_run(run: sacred.run.Run) -> Optional[pathlib.Path]:
     """Returns path to the sacred directory, or None if not found."""
     for obs in run.observers:
         if isinstance(obs, sacred.observers.FileStorageObserver):
-            return types.parse_path(obs.dir)
+            return util.parse_path(obs.dir)
     return None
 
 
 def dict_get_nested(d: dict, nested_key: str, *, sep=".", default=None) -> Any:
     curr = d
     for key in nested_key.split(sep):
         if isinstance(curr, dict) and key in curr:
```

### Comparing `imitation-0.3.2/src/imitation.egg-info/PKG-INFO` & `imitation-0.4.0/src/imitation.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imitation
-Version: 0.3.2
+Version: 0.4.0
 Summary: Implementation of modern reward and imitation learning algorithms.
 Home-page: https://github.com/HumanCompatibleAI/imitation
 Author: Center for Human-Compatible AI and Google
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -92,21 +92,21 @@
 
 We provide several CLI scripts as a front-end to the algorithms implemented in `imitation`. These use [Sacred](https://github.com/idsia/sacred) for configuration and replicability.
 
 From [examples/quickstart.sh:](examples/quickstart.sh)
 
 ```bash
 # Train PPO agent on pendulum and collect expert demonstrations. Tensorboard logs saved in quickstart/rl/
-python -m imitation.scripts.train_rl with pendulum common.fast train.fast rl.fast fast common.log_dir=quickstart/rl/
+python -m imitation.scripts.train_rl with pendulum environment.fast policy_evaluation.fast rl.fast fast logging.log_dir=quickstart/rl/
 
 # Train GAIL from demonstrations. Tensorboard logs saved in output/ (default log directory).
-python -m imitation.scripts.train_adversarial gail with pendulum common.fast demonstrations.fast train.fast rl.fast fast demonstrations.rollout_path=quickstart/rl/rollouts/final.npz
+python -m imitation.scripts.train_adversarial gail with pendulum environment.fast demonstrations.fast policy_evaluation.fast rl.fast fast demonstrations.path=quickstart/rl/rollouts/final.npz demonstrations.source=local
 
 # Train AIRL from demonstrations. Tensorboard logs saved in output/ (default log directory).
-python -m imitation.scripts.train_adversarial airl with pendulum common.fast demonstrations.fast train.fast rl.fast fast demonstrations.rollout_path=quickstart/rl/rollouts/final.npz
+python -m imitation.scripts.train_adversarial airl with pendulum environment.fast demonstrations.fast policy_evaluation.fast rl.fast fast demonstrations.path=quickstart/rl/rollouts/final.npz demonstrations.source=local
 ```
 
 Tips:
 
 - Remove the "fast" options from the commands above to allow training run to completion.
 - `python -m imitation.scripts.train_rl print_config` will list Sacred script options. These configuration options are documented in each script's docstrings.
 
@@ -119,21 +119,23 @@
 ### Density reward baseline
 
 We also implement a density-based reward baseline. You can find an [example notebook here](docs/tutorials/7_train_density.ipynb).
 
 # Citations (BibTeX)
 
 ```
-@misc{wang2020imitation,
-  author = {Wang, Steven and Toyer, Sam and Gleave, Adam and Emmons, Scott},
-  title = {The {\tt imitation} Library for Imitation Learning and Inverse Reinforcement Learning},
-  year = {2020},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/HumanCompatibleAI/imitation}},
+@misc{gleave2022imitation,
+  author = {Gleave, Adam and Taufeeque, Mohammad and Rocamonde, Juan and Jenner, Erik and Wang, Steven H. and Toyer, Sam and Ernestus, Maximilian and Belrose, Nora and Emmons, Scott and Russell, Stuart},
+  title = {imitation: Clean Imitation Learning Implementations},
+  year = {2022},
+  howPublished = {arXiv:2211.11972v1 [cs.LG]},
+  archivePrefix = {arXiv},
+  eprint = {2211.11972},
+  primaryClass = {cs.LG},
+  url = {https://arxiv.org/abs/2211.11972},
 }
 ```
 
 # Contributing
 
 See [Contributing to imitation][contributing] for more information.
```

### Comparing `imitation-0.3.2/src/imitation.egg-info/SOURCES.txt` & `imitation-0.4.0/src/imitation.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .codecov.yml
 .coveragerc
 .dockerignore
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
+CITATION.bib
 Dockerfile
 LICENSE
 README.md
 mypy.ini
 pyproject.toml
 readthedocs.yml
 setup.cfg
@@ -34,26 +35,28 @@
 benchmarking/example_dagger_seals_swimmer_best_hp_eval.json
 benchmarking/example_dagger_seals_walker_best_hp_eval.json
 benchmarking/example_gail_seals_ant_best_hp_eval.json
 benchmarking/example_gail_seals_half_cheetah_best_hp_eval.json
 benchmarking/example_gail_seals_hopper_best_hp_eval.json
 benchmarking/example_gail_seals_swimmer_best_hp_eval.json
 benchmarking/example_gail_seals_walker_best_hp_eval.json
+benchmarking/fast_dagger_seals_cartpole.json
 benchmarking/util.py
 ci/Xdummy-entrypoint.py
 ci/build_and_activate_venv.ps1
 ci/build_and_activate_venv.sh
 ci/check_typeignore.py
 ci/clean_notebooks.py
 ci/xorg.conf
 docs/.gitignore
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
+docs/requirements.txt
 docs/_static/css/custom.css
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/algorithms/airl.rst
 docs/algorithms/bc.rst
 docs/algorithms/dagger.rst
@@ -63,33 +66,39 @@
 docs/algorithms/preference_comparisons.rst
 docs/development/developer.rst
 docs/development/license.rst
 docs/development/release-notes.rst
 docs/development/contributing/code-of-conduct.rst
 docs/development/contributing/index.rst
 docs/development/contributing/ways-to-contribute.rst
-docs/experts/loading-experts.rst
-docs/getting-started/first-steps.rst
+docs/getting-started/cli.rst
+docs/getting-started/first_steps.rst
 docs/getting-started/installation.rst
-docs/getting-started/variable-horizon.rst
-docs/getting-started/what-is-imitation.rst
+docs/getting-started/what_is_imitation.rst
+docs/main-concepts/experts.rst
+docs/main-concepts/reward_networks.rst
+docs/main-concepts/trajectories.rst
+docs/main-concepts/variable_horizon.rst
 docs/tutorials/1_train_bc.ipynb
 docs/tutorials/2_train_dagger.ipynb
 docs/tutorials/3_train_gail.ipynb
 docs/tutorials/4_train_airl.ipynb
 docs/tutorials/5_train_preference_comparisons.ipynb
 docs/tutorials/5a_train_preference_comparisons_with_cnn.ipynb
 docs/tutorials/6_train_mce.ipynb
 docs/tutorials/7_train_density.ipynb
+docs/tutorials/8_train_custom_env.ipynb
+docs/tutorials/9_compare_baselines.ipynb
 examples/quickstart.py
 examples/quickstart.sh
 experiments/.gitignore
 experiments/README.md
 experiments/bc_benchmark.sh
 experiments/benchmark_and_table.sh
+experiments/commands.py
 experiments/common.sh
 experiments/convert_traj.py
 experiments/dagger_benchmark.sh
 experiments/imit_benchmark.sh
 experiments/imit_benchmark_config.csv
 experiments/imit_table_cheetahs.csv
 experiments/imit_table_mvp_seals_config.csv
@@ -115,15 +124,17 @@
 src/imitation/algorithms/preference_comparisons.py
 src/imitation/algorithms/adversarial/__init__.py
 src/imitation/algorithms/adversarial/airl.py
 src/imitation/algorithms/adversarial/common.py
 src/imitation/algorithms/adversarial/gail.py
 src/imitation/data/__init__.py
 src/imitation/data/buffer.py
+src/imitation/data/huggingface_utils.py
 src/imitation/data/rollout.py
+src/imitation/data/serialize.py
 src/imitation/data/types.py
 src/imitation/data/wrappers.py
 src/imitation/policies/__init__.py
 src/imitation/policies/base.py
 src/imitation/policies/exploration_wrapper.py
 src/imitation/policies/replay_buffer_wrapper.py
 src/imitation/policies/serialize.py
@@ -140,69 +151,76 @@
 src/imitation/scripts/convert_trajs.py
 src/imitation/scripts/eval_policy.py
 src/imitation/scripts/parallel.py
 src/imitation/scripts/train_adversarial.py
 src/imitation/scripts/train_imitation.py
 src/imitation/scripts/train_preference_comparisons.py
 src/imitation/scripts/train_rl.py
-src/imitation/scripts/common/__init__.py
-src/imitation/scripts/common/common.py
-src/imitation/scripts/common/demonstrations.py
-src/imitation/scripts/common/expert.py
-src/imitation/scripts/common/reward.py
-src/imitation/scripts/common/rl.py
-src/imitation/scripts/common/train.py
-src/imitation/scripts/common/wb.py
 src/imitation/scripts/config/__init__.py
 src/imitation/scripts/config/analyze.py
 src/imitation/scripts/config/eval_policy.py
 src/imitation/scripts/config/parallel.py
 src/imitation/scripts/config/train_adversarial.py
 src/imitation/scripts/config/train_imitation.py
 src/imitation/scripts/config/train_preference_comparisons.py
 src/imitation/scripts/config/train_rl.py
+src/imitation/scripts/ingredients/__init__.py
+src/imitation/scripts/ingredients/bc.py
+src/imitation/scripts/ingredients/demonstrations.py
+src/imitation/scripts/ingredients/environment.py
+src/imitation/scripts/ingredients/expert.py
+src/imitation/scripts/ingredients/logging.py
+src/imitation/scripts/ingredients/policy.py
+src/imitation/scripts/ingredients/policy_evaluation.py
+src/imitation/scripts/ingredients/reward.py
+src/imitation/scripts/ingredients/rl.py
+src/imitation/scripts/ingredients/wb.py
 src/imitation/testing/__init__.py
 src/imitation/testing/expert_trajectories.py
+src/imitation/testing/hypothesis_strategies.py
 src/imitation/testing/reward_improvement.py
 src/imitation/testing/reward_nets.py
 src/imitation/util/__init__.py
 src/imitation/util/logger.py
 src/imitation/util/networks.py
 src/imitation/util/registry.py
 src/imitation/util/sacred.py
 src/imitation/util/util.py
 src/imitation/util/video_wrapper.py
 tests/conftest.py
 tests/generate_test_data.sh
+tests/test_benchmarking.py
 tests/test_examples.py
 tests/test_experiments.py
 tests/test_regularization.py
 tests/algorithms/__init__.py
 tests/algorithms/conftest.py
 tests/algorithms/test_adversarial.py
 tests/algorithms/test_base.py
 tests/algorithms/test_bc.py
 tests/algorithms/test_dagger.py
 tests/algorithms/test_density_baselines.py
 tests/algorithms/test_mce_irl.py
 tests/algorithms/test_preference_comparisons.py
 tests/data/test_buffer.py
+tests/data/test_huggingface_utils.py
 tests/data/test_rollout.py
 tests/data/test_types.py
 tests/data/test_wrappers.py
 tests/policies/test_exploration_wrapper.py
 tests/policies/test_policies.py
 tests/policies/test_replay_buffer_wrapper.py
 tests/rewards/test_reward_fn.py
 tests/rewards/test_reward_nets.py
 tests/rewards/test_reward_wrapper.py
 tests/scripts/test_scripts.py
-tests/scripts/common/test_rewards.py
+tests/scripts/ingredients/test_rewards.py
 tests/testdata/imit_benchmark_config.csv
-tests/testdata/old_format_rollout.pkl
+tests/testdata/npz_format_rollout.npz
+tests/testdata/pickle_format_rollout.pkl
 tests/testdata/rollouts_from_policies_config.csv
 tests/testdata/expert_models/cartpole_0/policies/final/model.zip
 tests/testdata/expert_models/cartpole_0/rollouts/final.npz
 tests/testdata/expert_models/pendulum_0/rollouts/final.npz
 tests/util/test_logger.py
 tests/util/test_networks.py
 tests/util/test_registry.py
```

### Comparing `imitation-0.3.2/src/imitation.egg-info/requires.txt` & `imitation-0.4.0/src/imitation.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 pyglet==1.5.27
 matplotlib
 numpy>=1.15
 torch>=1.4.0
 tqdm
 scikit-learn>=0.21.2
 seals>=0.1.5
-stable-baselines3>=1.6.1
-chai-sacred>=0.8.3
+stable-baselines3<2.0.0,>=1.7.0
+sacred>=0.8.4
 tensorboard>=1.14
 huggingface_sb3>=2.2.1
+datasets>=2.8.0
 
 [atari]
 opencv-python
 ale-py==0.7.4
 pillow
-autorom[accept-rom-license]~=0.4.2
+autorom[accept-rom-license]~=0.6.0
 
 [dev]
 autopep8
 ipdb
 isort~=5.0
 codespell
 sphinx-autobuild
@@ -50,15 +51,15 @@
 wandb==0.12.21
 setuptools_scm~=7.0.5
 pre-commit>=2.20.0
 ray[debug,tune]~=2.0.0
 opencv-python
 ale-py==0.7.4
 pillow
-autorom[accept-rom-license]~=0.4.2
+autorom[accept-rom-license]~=0.6.0
 pytype==2022.7.26
 sphinx~=5.1.1
 sphinx-autodoc-typehints~=1.19.1
 sphinx-rtd-theme~=1.0.0
 sphinxcontrib-napoleon==0.7
 furo==2022.6.21
 sphinx-copybutton==0.5.0
@@ -75,15 +76,15 @@
 sphinx-copybutton==0.5.0
 sphinx-github-changelog~=1.2.0
 myst-nb==0.16.0
 ipykernel~=6.15.2
 opencv-python
 ale-py==0.7.4
 pillow
-autorom[accept-rom-license]~=0.4.2
+autorom[accept-rom-license]~=0.6.0
 
 [mujoco]
 gym[classic_control,mujoco]==0.21.0
 
 [parallel]
 ray[debug,tune]~=2.0.0
 
@@ -115,9 +116,9 @@
 wandb==0.12.21
 setuptools_scm~=7.0.5
 pre-commit>=2.20.0
 ray[debug,tune]~=2.0.0
 opencv-python
 ale-py==0.7.4
 pillow
-autorom[accept-rom-license]~=0.4.2
+autorom[accept-rom-license]~=0.6.0
 pytype==2022.7.26
```

### Comparing `imitation-0.3.2/tests/algorithms/conftest.py` & `imitation-0.4.0/tests/algorithms/conftest.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/algorithms/test_adversarial.py` & `imitation-0.4.0/tests/algorithms/test_adversarial.py`

 * *Files 4% similar despite different names*

```diff
@@ -395,17 +395,17 @@
     obs, acts, next_obs, dones = trainer_diverse_env.reward_train.preprocess(
         trans.obs,
         trans.acts,
         trans.next_obs,
         trans.dones,
     )
     log_act_prob_non_none = np.log(0.1 + 0.9 * np.random.rand(n_timesteps))
-    log_act_prob_non_none = th.as_tensor(log_act_prob_non_none).to(obs.device)
+    log_act_prob_non_none_th = th.as_tensor(log_act_prob_non_none).to(obs.device)
 
-    for log_act_prob in [None, log_act_prob_non_none]:
+    for log_act_prob in [None, log_act_prob_non_none_th]:
         maybe_error_ctx: contextlib.AbstractContextManager
         if isinstance(trainer_diverse_env, airl.AIRL) and log_act_prob is None:
             maybe_error_ctx = pytest.raises(TypeError, match="Non-None.*required.*")
         else:
             maybe_error_ctx = contextlib.nullcontext()
 
         with maybe_error_ctx:
@@ -429,7 +429,38 @@
         disc_logits_expert_is_high,
         labels_expert_is_one,
         disc_loss,
     )
     for k, v in stats.items():
         assert isinstance(k, str)
         assert isinstance(v, float)
+
+
+@pytest.mark.skipif(not th.cuda.is_available(), reason="requires GPU")
+def test_regression_gail_with_sac(
+    pendulum_expert_trajectories,
+    pendulum_venv,
+):  # pragma: no cover
+    """GAIL with a SAC learner on GPU used to crash when training (see #655).
+
+    This is a minimal test to reproduce it.
+
+    Args:
+        pendulum_expert_trajectories: expert trajectories for Pendulum env.
+        pendulum_venv: the Pendulum environment.
+    """
+    learner = stable_baselines3.SAC(
+        env=pendulum_venv,
+        policy=stable_baselines3.sac.policies.SACPolicy,
+    )
+    reward_net = reward_nets.BasicRewardNet(
+        pendulum_venv.observation_space,
+        pendulum_venv.action_space,
+    )
+    gail_trainer = gail.GAIL(
+        demonstrations=pendulum_expert_trajectories,
+        demo_batch_size=1024,
+        venv=pendulum_venv,
+        gen_algo=learner,
+        reward_net=reward_net,
+    )
+    gail_trainer.train(8)
```

### Comparing `imitation-0.3.2/tests/algorithms/test_base.py` & `imitation-0.4.0/tests/algorithms/test_base.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/algorithms/test_bc.py` & `imitation-0.4.0/tests/algorithms/test_bc.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 @hypothesis.given(
     env_name=env_names,
     bc_args=bc_args,
     train_args=bc_train_args,
     expert_data_type=expert_data_types,
     rng=rngs,
 )
-@hypothesis.settings(deadline=20000, max_examples=50)
+@hypothesis.settings(deadline=20000, max_examples=15)
 def test_smoke_bc_training(
     env_name: str,
     bc_args: dict,
     train_args: dict,
     expert_data_type: str,
     rng: np.random.Generator,
     pytestconfig: pytest.Config,
@@ -165,15 +165,15 @@
         **bc_args,
         demonstrations=make_expert_transition_loader(
             cache_dir=cache.mkdir("experts"),
             batch_size=bc_args["batch_size"],
             expert_data_type=expert_data_type,
             env_name=env_name,
             rng=rng,
-            num_trajectories=3,  # Only use 3 trajectories to speed up the test
+            num_trajectories=2,  # Only use 2 trajectories to speed up the test
         ),
     )
     # WHEN
     trainer.train(**train_args)
 
 
 #####################
@@ -182,29 +182,26 @@
 
 
 def test_that_bc_improves_rewards(
     cartpole_bc_trainer: bc.BC,
     cartpole_venv: vec_env.VecEnv,
 ):
     # GIVEN
-    # TODO(https://github.com/HumanCompatibleAI/imitation/issues/600): the upstream
-    # annotation for this function is overly-conservative but passing the policy at
-    # runtime works, the ignore can be removed once fixed upstream.
     novice_rewards, _ = evaluation.evaluate_policy(
-        cartpole_bc_trainer.policy,  # type: ignore[arg-type]
+        cartpole_bc_trainer.policy,
         cartpole_venv,
         15,
         return_episode_rewards=True,
     )
     assert isinstance(novice_rewards, list)
 
     # WHEN
     cartpole_bc_trainer.train(n_epochs=1)
     rewards_after_training, _ = evaluation.evaluate_policy(
-        cartpole_bc_trainer.policy,  # type: ignore[arg-type]
+        cartpole_bc_trainer.policy,
         cartpole_venv,
         15,
         return_episode_rewards=True,
     )
 
     # THEN
     assert isinstance(rewards_after_training, list)
```

### Comparing `imitation-0.3.2/tests/algorithms/test_dagger.py` & `imitation-0.4.0/tests/algorithms/test_dagger.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import gym
 import numpy as np
 import pytest
 import torch.random
 from stable_baselines3.common import evaluation, policies
 
 from imitation.algorithms import bc, dagger
-from imitation.data import rollout, types
+from imitation.data import rollout, serialize, types
 from imitation.data.types import TrajectoryWithRew
 from imitation.policies import base
 from imitation.testing import reward_improvement
 from imitation.util import util
 
 
 @pytest.fixture(params=[True, False])
@@ -29,20 +29,47 @@
     keep_trajs = request.param
     if keep_trajs:
         return pendulum_expert_trajectories
     else:
         return None
 
 
-def test_beta_schedule():
-    one_step_sched = dagger.LinearBetaSchedule(1)
-    three_step_sched = dagger.LinearBetaSchedule(3)
-    for i in range(10):
-        assert np.allclose(one_step_sched(i), 1 if i == 0 else 0)
-        assert np.allclose(three_step_sched(i), (3 - i) / 3 if i <= 2 else 0)
+@pytest.mark.parametrize("num_rampdown_rounds", [1, 2, 3, 10])
+def test_linear_beta_schedule(num_rampdown_rounds):
+    # GIVEN
+    sched = dagger.LinearBetaSchedule(num_rampdown_rounds)
+    idx_after_rampdown = num_rampdown_rounds + 1
+
+    # WHEN
+    betas = [sched(i) for i in range(num_rampdown_rounds + 10)]
+
+    # THEN
+    assert np.allclose(
+        betas[:idx_after_rampdown],
+        np.linspace(1, 0, idx_after_rampdown),
+    )
+    assert np.allclose(betas[idx_after_rampdown:], 0)
+
+
+@pytest.mark.parametrize("decay_probability", [0.1, 0.5, 0.9, 1])
+def test_exponential_beta_schedule(decay_probability):
+    # GIVEN
+    sched = dagger.ExponentialBetaSchedule(decay_probability)
+
+    # WHEN
+    betas = [sched(i) for i in range(10)]
+
+    # THEN
+    assert np.allclose(betas, decay_probability ** np.arange(10))
+
+
+@pytest.mark.parametrize("decay_probability", [-0.1, 0, 1.1, 2])
+def test_forbidden_decay_probability_on_exp_beta_schedule(decay_probability):
+    with pytest.raises(ValueError):
+        dagger.ExponentialBetaSchedule(decay_probability)
 
 
 def test_traj_collector_seed(tmpdir, pendulum_venv, rng):
     collector = dagger.InteractiveTrajectoryCollector(
         venv=pendulum_venv,
         get_robot_acts=lambda o: [
             pendulum_venv.action_space.sample() for _ in range(len(o))
@@ -96,19 +123,76 @@
     assert 388 * pendulum_venv.num_envs <= robot_calls <= 612 * pendulum_venv.num_envs
 
     # All user/expert actions are zero. Therefore, all collected actions should be
     # zero.
     file_paths = glob.glob(os.path.join(tmpdir, "dagger-demo-*.npz"))
     assert num_episodes == 5 * pendulum_venv.num_envs
     assert len(file_paths) == num_episodes
-    trajs = [types.load(p)[0] for p in file_paths]
+    trajs = [serialize.load(p)[0] for p in file_paths]
     nonzero_acts = sum(np.sum(traj.acts != 0) for traj in trajs)
     assert nonzero_acts == 0
 
 
+def test_traj_collector_reproducible(tmpdir, pendulum_venv):
+    # We run the collector twice with the same random seeds and
+    # check that the following 2 properties hold:
+    # 1) The files written in the first run have the same filenames
+    #    as the files written in the second run.
+    # 2) Each file in the first run stores the same trajectory as
+    #    the file with the same filename in the second run.
+    filename_to_traj_dicts = []
+    with torch.random.fork_rng():
+        for run_idx in range(2):
+            # Reset the random seeds.
+            save_dir = os.path.join(tmpdir, "run{0}".format(run_idx))
+            rng = np.random.default_rng(12345)
+            pendulum_venv.seed(12345)
+            pendulum_venv.action_space.seed(12345)
+
+            # Run the collector.
+            collector = dagger.InteractiveTrajectoryCollector(
+                venv=pendulum_venv,
+                get_robot_acts=lambda o: [
+                    pendulum_venv.action_space.sample() for _ in range(len(o))
+                ],
+                beta=0.5,
+                save_dir=save_dir,
+                rng=rng,
+            )
+            collector.reset()
+            zero_acts = np.zeros(
+                (pendulum_venv.num_envs,) + pendulum_venv.action_space.shape,
+                dtype=pendulum_venv.action_space.dtype,
+            )
+            for i in range(1000):
+                _, _, dones, _ = collector.step(zero_acts)
+
+            # Get the observations from all the collected trajectories.
+            file_paths = glob.glob(os.path.join(save_dir, "dagger-demo-*.npz"))
+            filename_to_traj_dict = {}
+            for fp in file_paths:
+                traj = serialize.load_with_rewards(fp)[0]
+                # For the purposes of testing, we remove `infos` from the
+                # trajectory, because `infos` contains the time that it
+                # takes to complete an episode, which we expect to differ
+                # slightly between runs.
+                traj_without_infos = types.TrajectoryWithRew(
+                    obs=traj.obs,
+                    acts=traj.acts,
+                    infos=None,
+                    terminal=traj.terminal,
+                    rews=traj.rews,
+                )
+                filename = os.path.basename(fp)
+                filename_to_traj_dict[filename] = traj_without_infos
+            filename_to_traj_dicts.append(filename_to_traj_dict)
+
+    assert filename_to_traj_dicts[0] == filename_to_traj_dicts[1]
+
+
 def _build_dagger_trainer(
     tmpdir,
     venv,
     beta_schedule,
     expert_policy,
     pendulum_expert_rollouts: List[TrajectoryWithRew],
     custom_logger,
@@ -278,57 +362,119 @@
         torch.random.manual_seed(42)
         pendulum_venv.action_space.seed(42)
 
         trainer = init_trainer_fn()
         novice_rewards, _ = evaluation.evaluate_policy(
             trainer.policy,
             pendulum_venv,
-            15,
-            deterministic=False,
+            25,
+            deterministic=True,
             return_episode_rewards=True,
         )
         # note a randomly initialised policy does well for some seeds -- so may
         # want to adjust this check if changing seed. Pendulum return can range
         # from -1,200 to -130 (approx.), per Figure 3 in this PDF (on page 3):
         # https://arxiv.org/pdf/2106.09556.pdf
         assert np.mean(novice_rewards) < -1000
-        # Train for 10 iterations. (6 or less causes test to fail on some configs.)
+        # Train for 5 iterations. (4 or fewer causes test to fail on some configs.)
         # see https://github.com/HumanCompatibleAI/imitation/issues/580 for details
-        for i in range(10):
+        for i in range(5):
             # roll out a few trajectories for dataset, then train for a few steps
             collector = trainer.create_trajectory_collector()
-            for _ in range(5):
+            for _ in range(4):
                 obs = collector.reset()
                 dones = [False] * pendulum_venv.num_envs
                 while not np.any(dones):
                     expert_actions, _ = pendulum_expert_policy.predict(
                         obs,
                         deterministic=True,
                     )
                     obs, _, dones, _ = collector.step(expert_actions)
             trainer.extend_and_update(dict(n_epochs=1))
         # make sure we're doing better than a random policy would
         rewards_after_training, _ = evaluation.evaluate_policy(
             trainer.policy,
             pendulum_venv,
-            15,
+            25,
+            deterministic=True,
             return_episode_rewards=True,
         )
 
     assert reward_improvement.is_significant_reward_improvement(
         novice_rewards,
         rewards_after_training,
     )
     assert reward_improvement.mean_reward_improved_by(
         novice_rewards,
         rewards_after_training,
         300,
     )
 
 
+@pytest.mark.parametrize(
+    "init_trainer_fn",
+    [_build_dagger_trainer, _build_simple_dagger_trainer],
+)
+def test_trainer_reproducible(
+    init_trainer_fn,
+    tmpdir,
+    pendulum_venv,
+    pendulum_expert_policy,
+    custom_logger,
+):
+    # Check that we get the same results if we run the trainer
+    # twice with the same random seeds.
+    # In particular, check that the trajectories from rolling out
+    # the trained policy are the same in each run.
+    run_trajs = []
+    with torch.random.fork_rng():
+        for run_idx in range(2):
+            # Reset the random seeds.
+            run_dir = os.path.join(tmpdir, "run{0}".format(run_idx))
+            torch.random.manual_seed(12345)
+            rng = np.random.default_rng(12345)
+            pendulum_venv.seed(12345)
+            pendulum_venv.action_space.seed(12345)
+
+            beta_schedule = None
+            maybe_pendulum_expert_trajectories = None
+            trainer = init_trainer_fn(
+                run_dir,
+                pendulum_venv,
+                beta_schedule,
+                pendulum_expert_policy,
+                maybe_pendulum_expert_trajectories,
+                custom_logger,
+                rng,
+            )
+
+            for i in range(2):
+                collector = trainer.create_trajectory_collector()
+                obs = collector.reset()
+                dones = [False] * pendulum_venv.num_envs
+                while not np.any(dones):
+                    expert_actions, _ = pendulum_expert_policy.predict(
+                        obs,
+                        deterministic=True,
+                    )
+                    obs, _, dones, _ = collector.step(expert_actions)
+                trainer.extend_and_update(dict(n_epochs=1))
+
+            trajs = rollout.rollout(
+                trainer.policy,
+                pendulum_venv,
+                rollout.make_sample_until(min_episodes=2),
+                rng,
+            )
+            run_trajs.append(trajs)
+
+    assert len(run_trajs) == 2
+    assert run_trajs[0] == run_trajs[1]
+
+
 def test_trainer_save_reload(tmpdir, init_trainer_fn, pendulum_venv):
     trainer = init_trainer_fn()
     trainer.round_num = 3
     trainer.save_trainer()
     loaded_trainer = dagger.reconstruct_trainer(trainer.scratch_dir, venv=pendulum_venv)
     assert loaded_trainer.round_num == trainer.round_num
```

### Comparing `imitation-0.3.2/tests/algorithms/test_density_baselines.py` & `imitation-0.4.0/tests/algorithms/test_density_baselines.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,16 @@
     density_type,
     is_stationary,
     pendulum_venv,
     pendulum_expert_trajectories: Sequence[TrajectoryWithRew],
     rng,
 ):
     # use only a subset of trajectories
-    expert_trajectories_all = pendulum_expert_trajectories[:8]
-    n_experts = len(expert_trajectories_all)
-    expert_trajectories_train = expert_trajectories_all[: n_experts // 2]
+    n_experts = len(pendulum_expert_trajectories)
+    expert_trajectories_train = pendulum_expert_trajectories[: n_experts // 2]
     reward_fn = DensityAlgorithm(
         demonstrations=expert_trajectories_train,
         density_type=density_type,
         kernel="gaussian",
         venv=pendulum_venv,
         is_stationary=is_stationary,
         kernel_bandwidth=0.2,
@@ -72,15 +71,15 @@
     sample_until = rollout.make_min_episodes(15)
     random_trajectories = rollout.generate_trajectories(
         random_policy,
         pendulum_venv,
         sample_until=sample_until,
         rng=rng,
     )
-    expert_trajectories_test = expert_trajectories_all[n_experts // 2 :]
+    expert_trajectories_test = pendulum_expert_trajectories[n_experts // 2 :]
     random_returns = score_trajectories(random_trajectories, reward_fn)
     expert_returns = score_trajectories(expert_trajectories_test, reward_fn)
     assert reward_improvement.is_significant_reward_improvement(
         random_returns,
         expert_returns,
     )
 
@@ -107,15 +106,20 @@
 
 
 def test_density_with_other_trajectory_types(
     pendulum_expert_trajectories: Sequence[TrajectoryWithRew],
     pendulum_venv,
     rng,
 ):
-    rl_algo = stable_baselines3.PPO(policies.ActorCriticPolicy, pendulum_venv)
+    rl_algo = stable_baselines3.PPO(
+        policies.ActorCriticPolicy,
+        pendulum_venv,
+        n_steps=10,  # small value to make test faster
+        n_epochs=2,  # small value to make test faster
+    )
     rollouts = pendulum_expert_trajectories[:2]
     transitions = rollout.flatten_trajectories_with_rew(rollouts)
     transitions_mappings = [
         asdict(transitions),
     ]
 
     minimal_transitions = types.TransitionsMinimal(
```

### Comparing `imitation-0.3.2/tests/algorithms/test_mce_irl.py` & `imitation-0.4.0/tests/algorithms/test_mce_irl.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,14 +310,54 @@
 
     mask = (1 - states).astype(bool)
     actions, timesteps = tabular.predict(states, timesteps, mask)
     np.testing.assert_array_equal(np.zeros((5,)), actions)
     np.testing.assert_equal(timesteps[0], 2 - mask.astype(int))
 
 
+def test_tabular_policy_rollouts(rng):
+    """Tests that rolling out a tabular policy that varies at each timestep works."""
+    state_space = gym.spaces.Discrete(5)
+    action_space = gym.spaces.Discrete(3)
+    mdp = ReasonablePOMDP()
+    state_env = base_envs.ExposePOMDPStateWrapper(mdp)
+    state_venv = vec_env.DummyVecEnv([lambda: state_env])
+
+    # alternate actions every step
+    subpolicy = np.stack([np.eye(action_space.n)] * state_space.n, axis=1)
+
+    # repeat 7 times for a total of 21 (greater than 20)
+    pi = np.repeat(
+        subpolicy,
+        ((mdp.horizon + action_space.n - 1) // action_space.n),
+        axis=0,
+    )
+
+    tabular = TabularPolicy(
+        state_space=state_space,
+        action_space=action_space,
+        pi=pi,
+        rng=rng,
+    )
+
+    trajs = rollout.generate_trajectories(
+        tabular,
+        state_venv,
+        sample_until=rollout.make_min_episodes(1),
+        rng=rng,
+    )
+
+    # pi[t,s,a] is the same for every state, so drop that dimension
+    exposed_actions_onehot = pi[:, 0, :]
+    exposed_actions = exposed_actions_onehot.nonzero()[1]
+
+    # check that the trajectory chooses the same actions as the policy
+    assert (trajs[0].acts == exposed_actions[: len(trajs[0].acts)]).all()
+
+
 def test_tabular_policy_randomness(rng):
     state_space = gym.spaces.Discrete(2)
     action_space = gym.spaces.Discrete(2)
     pi = np.array(
         [
             [
                 [0.5, 0.5],
```

### Comparing `imitation-0.3.2/tests/algorithms/test_preference_comparisons.py` & `imitation-0.4.0/tests/algorithms/test_preference_comparisons.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import imitation.testing.reward_nets as testing_reward_nets
 from imitation.algorithms import preference_comparisons
 from imitation.data import types
 from imitation.data.types import TrajectoryWithRew
 from imitation.regularization import regularizers, updaters
 from imitation.rewards import reward_nets
+from imitation.testing import reward_improvement
 from imitation.util import networks, util
 
 UNCERTAINTY_ON = ["logit", "probability", "label"]
 
 
 @pytest.fixture
 def venv(rng):
@@ -1060,31 +1061,34 @@
         custom_logger=custom_logger,
     )
 
     # Get initial agent performance
     novice_agent_rewards, _ = evaluation.evaluate_policy(
         agent_trainer.algorithm.policy,
         action_is_reward_venv,
-        15,
+        25,
         return_episode_rewards=True,
     )
 
     # Train for a short period of time, and then again.
     # We expect the reward network to have a better estimate of the reward
     # after this training, and thus `later_rewards` should have lower loss.
     first_reward_network_stats = main_trainer.train(20, 20)
 
-    later_reward_network_stats = main_trainer.train(1000, 20)
+    later_reward_network_stats = main_trainer.train(50, 20)
     assert (
         first_reward_network_stats["reward_loss"]
         > later_reward_network_stats["reward_loss"]
     )
 
     # The agent should have also improved
     trained_agent_rewards, _ = evaluation.evaluate_policy(
         agent_trainer.algorithm.policy,
         action_is_reward_venv,
-        15,
+        25,
         return_episode_rewards=True,
     )
 
-    assert np.mean(trained_agent_rewards) > np.mean(novice_agent_rewards)
+    assert reward_improvement.is_significant_reward_improvement(
+        novice_agent_rewards,
+        trained_agent_rewards,
+    )
```

### Comparing `imitation-0.3.2/tests/conftest.py` & `imitation-0.4.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 @pytest.fixture()
 def custom_logger(tmpdir: str) -> logger.HierarchicalLogger:
     return logger.configure(tmpdir)
 
 
 @pytest.fixture()
 def rng() -> np.random.Generator:
-    return np.random.default_rng()
+    return np.random.default_rng(seed=0)
```

### Comparing `imitation-0.3.2/tests/data/test_buffer.py` & `imitation-0.4.0/tests/data/test_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         # Are samples right data type?
         assert sample.obs.dtype == dtype
         assert sample.acts.dtype == dtype
         assert sample.next_obs.dtype == dtype
         assert info_vals.dtype == dtype
         assert sample.dones.dtype == bool
-        assert sample.infos.dtype == np.object
+        assert sample.infos.dtype == object
 
         # Are samples in range?
         _check_bound(i + chunk_len, capacity, sample.obs)
         _check_bound(i + chunk_len, capacity, sample.next_obs, 3 * capacity)
         _check_bound(i + chunk_len, capacity, sample.acts, 6 * capacity)
         _check_bound(i + chunk_len, capacity, info_vals, 9 * capacity)
```

### Comparing `imitation-0.3.2/tests/data/test_rollout.py` & `imitation-0.4.0/tests/data/test_rollout.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     if policy_type == "policy":
         policy = RandomPolicy(venv.observation_space, venv.action_space)
     elif policy_type == "callable":
         random_policy = RandomPolicy(venv.observation_space, venv.action_space)
 
         # Simple way to get a valid callable: just use a policies .predict() method
         # (still tests another code path inside generate_trajectories)
-        def policy(x):
-            return random_policy.predict(x)[0]
+        def policy(x, state, mask):
+            return random_policy.predict(x, state, mask)
 
     elif policy_type == "random":
         policy = None
     else:  # pragma: no cover
         raise ValueError(f"Unknown policy_type '{policy_type}'")
     sample_until = rollout.make_min_episodes(min_episodes)
     trajectories = rollout.generate_trajectories(
```

### Comparing `imitation-0.3.2/tests/data/test_types.py` & `imitation-0.4.0/tests/data/test_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import pickle
 from typing import Any, Callable, Sequence
 
 import gym
 import numpy as np
 import pytest
 
-from imitation.data import types
+from imitation.data import serialize, types
+from imitation.util import util
 
 SPACES = [
     gym.spaces.Discrete(3),
     gym.spaces.MultiDiscrete((3, 4)),
     gym.spaces.Box(-1, 1, shape=(1,)),
     gym.spaces.Box(-1, 1, shape=(2,)),
     gym.spaces.Box(-np.inf, np.inf, shape=(2,)),
@@ -39,15 +40,15 @@
     length: int,
 ) -> types.Trajectory:
     """Fixture to generate trajectory of length `length` iid sampled from spaces."""
     if length == 0:
         pytest.skip()
     obs = np.array([obs_space.sample() for _ in range(length + 1)])
     acts = np.array([act_space.sample() for _ in range(length)])
-    infos = np.array([{i: i} for i in range(length)])
+    infos = np.array([{f"key{i}": i} for i in range(length)])
     return types.Trajectory(obs=obs, acts=acts, infos=infos, terminal=True)
 
 
 @pytest.fixture
 def trajectory_rew(trajectory: types.Trajectory) -> types.TrajectoryWithRew:
     """Like `trajectory` but with reward randomly sampled from a Gaussian."""
     rews = np.random.randn(len(trajectory))
@@ -214,41 +215,41 @@
             chdir_context = pushd(tmpdir)
             save_dir_str = ""
         else:
             chdir_context = contextlib.nullcontext()
             save_dir_str = tmpdir
 
         with chdir_context:
-            save_dir = types.parse_path(save_dir_str)
+            save_dir = util.parse_path(save_dir_str)
             trajs = [trajectory_rew if use_rewards else trajectory]
             save_path = save_dir / "trajs"
 
             if use_pickle:
                 # Pickle format
                 with open(save_path, "wb") as f:
                     pickle.dump(trajs, f)
             else:
-                # .npz format
-                types.save(save_path, trajs)
+                # HuggingFace Dataset Format
+                serialize.save(save_path, trajs)
 
                 # Test that heterogeneous lists of trajectories throw an error
                 if use_rewards:
                     with pytest.raises(ValueError):
-                        types.save(save_path, [trajectory, trajectory_rew])
+                        serialize.save(save_path, [trajectory, trajectory_rew])
 
             loaded_trajs: Sequence[types.Trajectory]
             if type_safe:
                 if use_rewards:
-                    loaded_trajs = types.load_with_rewards(save_path)
+                    loaded_trajs = serialize.load_with_rewards(save_path)
                 else:
                     with pytest.raises(ValueError):
-                        types.load_with_rewards(save_path)
-                    loaded_trajs = types.load(save_path)
+                        serialize.load_with_rewards(save_path)
+                    loaded_trajs = serialize.load(save_path)
             else:
-                loaded_trajs = types.load(save_path)
+                loaded_trajs = serialize.load(save_path)
 
             assert len(trajs) == len(loaded_trajs)
             for t1, t2 in zip(trajs, loaded_trajs):
                 assert t1 == t2
 
     def test_invalid_trajectories(
         self,
@@ -393,43 +394,43 @@
 def test_parse_path():
     if os.name == "nt":  # pragma: no cover
         pytest.skip(
             "Windows uses path.WindowsPath instead when paths are resolved, which"
             "cannot be compared directly to pathlib.Path objects.",
         )
     # absolute paths
-    assert types.parse_path("/foo/bar") == pathlib.Path("/foo/bar")
-    assert types.parse_path(pathlib.Path("/foo/bar")) == pathlib.Path("/foo/bar")
-    assert types.parse_path(b"/foo/bar") == pathlib.Path("/foo/bar")
+    assert util.parse_path("/foo/bar") == pathlib.Path("/foo/bar")
+    assert util.parse_path(pathlib.Path("/foo/bar")) == pathlib.Path("/foo/bar")
+    assert util.parse_path(b"/foo/bar") == pathlib.Path("/foo/bar")
 
     # relative paths. implicit conversion to cwd
-    assert types.parse_path("foo/bar") == pathlib.Path.cwd() / "foo/bar"
-    assert types.parse_path(pathlib.Path("foo/bar")) == pathlib.Path.cwd() / "foo/bar"
-    assert types.parse_path(b"foo/bar") == pathlib.Path.cwd() / "foo/bar"
+    assert util.parse_path("foo/bar") == pathlib.Path.cwd() / "foo/bar"
+    assert util.parse_path(pathlib.Path("foo/bar")) == pathlib.Path.cwd() / "foo/bar"
+    assert util.parse_path(b"foo/bar") == pathlib.Path.cwd() / "foo/bar"
 
     # relative paths. conversion using custom base directory
     base_dir = pathlib.Path("/foo/bar")
-    assert types.parse_path("baz", base_directory=base_dir) == base_dir / "baz"
+    assert util.parse_path("baz", base_directory=base_dir) == base_dir / "baz"
     assert (
-        types.parse_path(pathlib.Path("baz"), base_directory=base_dir)
+        util.parse_path(pathlib.Path("baz"), base_directory=base_dir)
         == base_dir / "baz"
     )
-    assert types.parse_path(b"baz", base_directory=base_dir) == base_dir / "baz"
+    assert util.parse_path(b"baz", base_directory=base_dir) == base_dir / "baz"
 
     # pass a relative path but disallowing relative paths. should raise error.
     with pytest.raises(ValueError, match="Path .* is not absolute"):
-        types.parse_path("foo/bar", allow_relative=False)
+        util.parse_path("foo/bar", allow_relative=False)
 
     # pass a base direectory but disallowing relative paths. should raise error.
     with pytest.raises(
         ValueError,
         match="If `base_directory` is specified, then `allow_relative` must be True.",
     ):
-        types.parse_path(
+        util.parse_path(
             "foo/bar",
             base_directory=pathlib.Path("/foo/bar"),
             allow_relative=False,
         )
 
     # Parse optional path. Works the same way but passes None down the line.
-    assert types.parse_optional_path(None) is None
-    assert types.parse_optional_path("/foo/bar") == types.parse_path("/foo/bar")
+    assert util.parse_optional_path(None) is None
+    assert util.parse_optional_path("/foo/bar") == util.parse_path("/foo/bar")
```

### Comparing `imitation-0.3.2/tests/data/test_wrappers.py` & `imitation-0.4.0/tests/data/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/policies/test_exploration_wrapper.py` & `imitation-0.4.0/tests/policies/test_exploration_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """Tests ExplorationWrapper."""
 
 import numpy as np
+import pytest
 import seals  # noqa: F401
 
 from imitation.policies import exploration_wrapper
 from imitation.util import util
 
 
-def constant_policy(obs):
-    return np.zeros(len(obs), dtype=int)
+def constant_policy(obs, state, mask):
+    del state, mask  # Unused
+    return np.zeros(len(obs), dtype=int), None
+
+
+def fake_stateful_policy(obs, state, mask):
+    del state, mask  # Unused
+    return np.zeros(len(obs), dtype=int), (np.zeros(1),)
 
 
 def make_wrapper(random_prob, switch_prob, rng):
     venv = util.make_vec_env(
         "seals/CartPole-v0",
         n_envs=1,
         rng=rng,
@@ -88,25 +95,25 @@
     Args:
         rng (np.random.Generator): random number generator.
     """
     wrapper, venv = make_wrapper(random_prob=0.5, switch_prob=0.0, rng=rng)
     policy = wrapper.current_policy
 
     obs = np.random.rand(100, 2)
-    for action in wrapper(obs):
+    for action in wrapper(obs, None, None)[0]:
         assert venv.action_space.contains(action)
         assert wrapper.current_policy == policy
 
     def _always_switch(random_prob, num_steps):
         wrapper, _ = make_wrapper(random_prob=random_prob, switch_prob=1.0, rng=rng)
         num_random = 0
         num_constant = 0
         for _ in range(num_steps):
             obs = np.random.rand(1, 2)
-            wrapper(obs)
+            wrapper(obs, None, None)
             if wrapper.current_policy == wrapper._random_policy:
                 num_random += 1
             elif wrapper.current_policy == constant_policy:
                 num_constant += 1
             else:  # pragma: no cover
                 raise ValueError("Unknown policy")
         return num_random, num_constant
@@ -133,9 +140,38 @@
 
 def test_valid_output(rng):
     """Ensure that we test both the random and the wrapped policy at least once."""
     for random_prob in [0.0, 0.5, 1.0]:
         wrapper, venv = make_wrapper(random_prob=random_prob, switch_prob=0.5, rng=rng)
         np.random.seed(0)
         obs = np.random.rand(100, 2)
-        for action in wrapper(obs):
+        for action in wrapper(obs, None, None)[0]:
             assert venv.action_space.contains(action)
+
+
+def test_throws_for_stateful_policy(rng):
+    venv = util.make_vec_env(
+        "seals/CartPole-v0",
+        n_envs=1,
+        rng=rng,
+    )
+    wrapper = exploration_wrapper.ExplorationWrapper(
+        policy=fake_stateful_policy,
+        venv=venv,
+        random_prob=0,
+        switch_prob=0,
+        rng=rng,
+    )
+
+    np.random.seed(0)
+    obs = np.random.rand(100, 2)
+    with pytest.raises(
+        ValueError,
+        match="Exploration wrapper does not support stateful policies.",
+    ):
+        wrapper(obs, (np.ones_like(obs)), None)
+
+    with pytest.raises(
+        ValueError,
+        match="Exploration wrapper does not support stateful policies.",
+    ):
+        wrapper(obs, None, None)
```

### Comparing `imitation-0.3.2/tests/policies/test_policies.py` & `imitation-0.4.0/tests/policies/test_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import gym
 import numpy as np
 import pytest
 import torch as th
 from stable_baselines3.common import preprocessing
 from torch import nn
 
-from imitation.data import rollout, types
+from imitation.data import rollout
 from imitation.policies import base, serialize
 from imitation.util import registry, util
 
 SIMPLE_DISCRETE_ENV = "CartPole-v0"  # Discrete(2) action space
 SIMPLE_CONTINUOUS_ENV = "MountainCarContinuous-v0"  # Box(1) action space
 SIMPLE_ENVS = [SIMPLE_DISCRETE_ENV, SIMPLE_CONTINUOUS_ENV]
 HARDCODED_TYPES = ["random", "zero"]
@@ -54,15 +54,15 @@
 def test_save_stable_model_errors_and_warnings(
     tmpdir,
     policy_env_name_pair,
     rng,
 ):
     """Check errors and warnings in `save_stable_model()`."""
     policy, env_name = policy_env_name_pair
-    tmpdir = types.parse_path(tmpdir)
+    tmpdir = util.parse_path(tmpdir)
     venv = util.make_vec_env(env_name, rng=rng)
 
     # Trigger FileNotFoundError for no model.{zip,pkl}
     dir_a = tmpdir / "a"
     dir_a.mkdir()
     with pytest.raises(FileNotFoundError, match=".*Expected.*model.zip.*"):
         serialize.load_policy(policy, venv, path=str(dir_a))
@@ -99,15 +99,15 @@
         model,
         venv,
         n_timesteps=1000,
         deterministic_policy=True,
         rng=np.random.default_rng(0),
     )
 
-    serialize.save_stable_model(types.parse_path(tmpdir), model)
+    serialize.save_stable_model(util.parse_path(tmpdir), model)
     loaded = serialize.load_policy(model_name, venv, path=tmpdir)
     venv.env_method("seed", 0)
     venv.reset()
     new_rollout = rollout.generate_transitions(
         loaded,
         venv,
         n_timesteps=1000,
```

### Comparing `imitation-0.3.2/tests/policies/test_replay_buffer_wrapper.py` & `imitation-0.4.0/tests/policies/test_replay_buffer_wrapper.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/rewards/test_reward_fn.py` & `imitation-0.4.0/tests/rewards/test_reward_fn.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/rewards/test_reward_nets.py` & `imitation-0.4.0/tests/rewards/test_reward_nets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests `imitation.rewards.reward_nets` and `imitation.rewards.serialize`."""
 
+import functools
 import logging
 import os
 import tempfile
 from typing import Callable, Tuple
 from unittest import mock
 
 import gym
@@ -34,19 +35,37 @@
     "RewardNet_shaped",
     "RewardNet_unshaped",
 ]
 
 
 # Reward net classes, allowed kwargs
 MAKE_REWARD_NET = [
-    reward_nets.BasicRewardNet,
-    reward_nets.BasicShapedRewardNet,
-    testing_reward_nets.make_ensemble,
+    functools.partial(
+        reward_nets.BasicRewardNet,
+        hid_sizes=(3,),
+    ),
+    functools.partial(
+        reward_nets.BasicShapedRewardNet,
+        reward_hid_sizes=(3,),
+        potential_hid_sizes=(3,),
+    ),
+    functools.partial(
+        testing_reward_nets.make_ensemble,
+        hid_sizes=(3,),
+    ),
+]
+MAKE_IMAGE_REWARD_NET = [
+    functools.partial(
+        reward_nets.CnnRewardNet,
+        hid_channels=(3, 3, 3),
+        kernel_size=3,
+        padding=0,
+        stride=3,
+    ),
 ]
-MAKE_IMAGE_REWARD_NET = [reward_nets.CnnRewardNet]
 
 MakePredictProcessedWrapper = Callable[
     [reward_nets.RewardNet],
     reward_nets.PredictProcessedWrapper,
 ]
 MAKE_PREDICT_PROCESSED_WRAPPERS = [
     lambda base: reward_nets.NormalizedRewardNet(base, networks.RunningNorm),
@@ -453,19 +472,22 @@
     normalize_rewards,
     tmpdir,
     rng,
 ):
     """Does output of deserialized reward network match that of original?"""
     logging.info(f"Testing {net_cls}")
 
+    ep_steps = 5
+
     venv = util.make_vec_env(
         env_name,
         n_envs=1,
         parallel=False,
         rng=rng,
+        max_episode_steps=ep_steps + 1,
     )
     original = net_cls(venv.observation_space, venv.action_space, **net_kwargs)
     if normalize_rewards:
         original = reward_nets.NormalizedRewardNet(original, networks.RunningNorm)
     random = base.RandomPolicy(venv.observation_space, venv.action_space)
 
     tmppath = os.path.join(tmpdir, "reward.pt")
@@ -474,15 +496,15 @@
 
     assert original.observation_space == loaded.observation_space
     assert original.action_space == loaded.action_space
 
     transitions = rollout.generate_transitions(
         random,
         venv,
-        n_timesteps=100,
+        n_timesteps=ep_steps,
         rng=rng,
     )
 
     if isinstance(original, reward_nets.NormalizedRewardNet):
         wrapped_rew_fn = serialize.load_reward("RewardNet_normalized", tmppath, venv)
         unwrapped_rew_fn = serialize.load_reward(
             "RewardNet_unnormalized",
```

### Comparing `imitation-0.3.2/tests/rewards/test_reward_wrapper.py` & `imitation-0.4.0/tests/rewards/test_reward_wrapper.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/scripts/common/test_rewards.py` & `imitation-0.4.0/tests/scripts/ingredients/test_rewards.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Tests for imitation.scripts.common.make_reward."""
+"""Tests for imitation.scripts.ingredients.reward."""
 from typing import Any, Mapping
 
 import pytest
 
 from imitation.rewards import reward_nets
-from imitation.scripts.common import reward
+from imitation.scripts.ingredients import reward
 from imitation.util import networks
 
 
 @pytest.fixture
 def member_config() -> Mapping[str, Any]:
     return {
         "net_cls": reward_nets.BasicRewardNet,
```

### Comparing `imitation-0.3.2/tests/scripts/test_scripts.py` & `imitation-0.4.0/tests/scripts/test_scripts.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 import pathlib
 import pickle
 import platform
 import shutil
 import sys
 import tempfile
 from collections import Counter
-from typing import Any, Dict, List, Mapping, Optional
+from typing import Any, Dict, Generator, List, Mapping, Optional
 from unittest import mock
 
 import numpy as np
 import pandas as pd
 import pytest
 import ray.tune as tune
 import sacred
 import sacred.utils
 import stable_baselines3
 import torch as th
 from stable_baselines3.common import buffers
 from stable_baselines3.her.her_replay_buffer import HerReplayBuffer
 
-from imitation.data import types
+from imitation.data import serialize
 from imitation.rewards import reward_nets
 from imitation.scripts import (
     analyze,
     convert_trajs,
     eval_policy,
     parallel,
     train_adversarial,
@@ -49,30 +49,31 @@
     parallel,
     train_adversarial,
     train_imitation,
     train_preference_comparisons,
     train_rl,
 ]
 
-TEST_DATA_PATH = types.parse_path("tests/testdata")
+TEST_DATA_PATH = util.parse_path("tests/testdata")
 
 if not TEST_DATA_PATH.exists():  # pragma: no cover
     raise RuntimeError(
         "Folder with test data has not been found. Make sure you are "
         "running tests relative to the base imitation project folder.",
     )
 
 CARTPOLE_TEST_DATA_PATH = TEST_DATA_PATH / "expert_models/cartpole_0/"
 CARTPOLE_TEST_ROLLOUT_PATH = CARTPOLE_TEST_DATA_PATH / "rollouts/final.npz"
 CARTPOLE_TEST_POLICY_PATH = CARTPOLE_TEST_DATA_PATH / "policies/final"
 
 PENDULUM_TEST_DATA_PATH = TEST_DATA_PATH / "expert_models/pendulum_0/"
 PENDULUM_TEST_ROLLOUT_PATH = PENDULUM_TEST_DATA_PATH / "rollouts/final.npz"
 
-OLD_FMT_ROLLOUT_TEST_DATA_PATH = TEST_DATA_PATH / "old_format_rollout.pkl"
+PICKLE_FMT_ROLLOUT_TEST_DATA_PATH = TEST_DATA_PATH / "pickle_format_rollout.pkl"
+NPZ_FMT_ROLLOUT_TEST_DATA_PATH = TEST_DATA_PATH / "npz_format_rollout.npz"
 
 
 @pytest.fixture(autouse=True)
 def sacred_capture_use_sys():
     """Set Sacred capture mode to "sys" because default "fd" option leads to error.
 
     See https://github.com/IDSIA/sacred/issues/289.
@@ -93,27 +94,37 @@
     argv = ["sacred-pytest-stub", "print_config"]
     with mock.patch.object(sys, "argv", argv):
         script_mod.main_console()
 
 
 ALGO_FAST_CONFIGS = {
     "adversarial": [
-        "common.fast",
+        "environment.fast",
         "demonstrations.fast",
         "rl.fast",
-        "train.fast",
+        "policy_evaluation.fast",
         "fast",
     ],
-    "eval_policy": ["common.fast", "fast"],
-    "imitation": ["common.fast", "demonstrations.fast", "train.fast", "fast"],
-    "preference_comparison": ["common.fast", "rl.fast", "train.fast", "fast"],
-    "rl": ["common.fast", "rl.fast", "train.fast", "fast"],
+    "eval_policy": ["environment.fast", "fast"],
+    "imitation": [
+        "environment.fast",
+        "demonstrations.fast",
+        "policy_evaluation.fast",
+        "fast",
+    ],
+    "preference_comparison": [
+        "environment.fast",
+        "rl.fast",
+        "policy_evaluation.fast",
+        "fast",
+    ],
+    "rl": ["environment.fast", "rl.fast", "fast"],
 }
 
-RL_SAC_NAMED_CONFIGS = ["rl.sac", "train.sac"]
+RL_SAC_NAMED_CONFIGS = ["rl.sac", "policy.sac"]
 
 
 @pytest.fixture(
     params=[
         "plain",
         "with_expert_trajectories",
         "warmstart",
@@ -130,25 +141,25 @@
             # don't interact with warm starting an agent.
             "save_preferences": True,
             "gatherer_kwargs": {"sample": False},
             "agent_path": CARTPOLE_TEST_POLICY_PATH,
             # FIXME(yawen): the policy we load was trained on 8 parallel environments
             #  and for some reason using it breaks if we use just 1 (like would be the
             #  default with the fast named_config)
-            "common": dict(num_vec=8),
+            "environment": dict(num_vec=8),
         },
         with_checkpoints={
             # Test that we can save checkpoints
             "checkpoint_interval": 1,
         },
     )[request.param]
 
 
 def test_train_preference_comparisons_main(tmpdir, preference_comparison_config):
-    config_updates = dict(common=dict(log_root=tmpdir))
+    config_updates = dict(logging=dict(log_root=tmpdir))
     sacred.utils.recursive_update(config_updates, preference_comparison_config)
     run = train_preference_comparisons.train_preference_comparisons_ex.run(
         # Note: we have to use the cartpole and not the seals_cartpole config because
         #  the seals_cartpole config needs rollouts with a fixed horizon,
         #  and the saved trajectory rollouts are variable horizon.
         named_configs=["cartpole"] + ALGO_FAST_CONFIGS["preference_comparison"],
         config_updates=config_updates,
@@ -159,52 +170,52 @@
 
 @pytest.mark.parametrize(
     "env_name",
     ["seals_cartpole", "mountain_car", "seals_mountain_car"],
 )
 def test_train_preference_comparisons_envs_no_crash(tmpdir, env_name):
     """Test envs specified in imitation.scripts.config.train_preference_comparisons."""
-    config_updates = dict(common=dict(log_root=tmpdir))
+    config_updates = dict(logging=dict(log_root=tmpdir))
     run = train_preference_comparisons.train_preference_comparisons_ex.run(
         named_configs=[env_name] + ALGO_FAST_CONFIGS["preference_comparison"],
         config_updates=config_updates,
     )
     assert run.status == "COMPLETED"
     assert isinstance(run.result, dict)
 
 
 def test_train_preference_comparisons_sac(tmpdir):
-    config_updates = dict(common=dict(log_root=tmpdir))
+    config_updates = dict(logging=dict(log_root=tmpdir))
     run = train_preference_comparisons.train_preference_comparisons_ex.run(
         # make sure rl.sac named_config is called after rl.fast to overwrite
         # rl_kwargs.batch_size to None
         named_configs=["pendulum"]
         + ALGO_FAST_CONFIGS["preference_comparison"]
         + RL_SAC_NAMED_CONFIGS,
         config_updates=config_updates,
     )
     assert run.config["rl"]["rl_cls"] is stable_baselines3.SAC
     assert run.status == "COMPLETED"
     assert isinstance(run.result, dict)
 
     # Make sure rl.sac named_config is called after rl.fast to overwrite
     # rl_kwargs.batch_size to None
-    with pytest.raises(Exception, match=".*set 'batch_size' at top-level.*"):
+    with pytest.raises(Exception, match="set 'batch_size' at top-level"):
         train_preference_comparisons.train_preference_comparisons_ex.run(
             named_configs=["pendulum"]
             + RL_SAC_NAMED_CONFIGS
             + ALGO_FAST_CONFIGS["preference_comparison"],
             config_updates=config_updates,
         )
 
 
 def test_train_preference_comparisons_sac_reward_relabel(tmpdir):
     def _run_reward_relabel_sac_preference_comparisons(buffer_cls):
         config_updates = dict(
-            common=dict(log_root=tmpdir),
+            logging=dict(log_root=tmpdir),
             rl=dict(
                 rl_kwargs=dict(
                     replay_buffer_class=buffer_cls,
                     replay_buffer_kwargs=dict(handle_timeout_termination=True),
                 ),
             ),
         )
@@ -218,30 +229,30 @@
         )
         return run
 
     run = _run_reward_relabel_sac_preference_comparisons(buffers.ReplayBuffer)
     assert run.status == "COMPLETED"
     del run
 
-    with pytest.raises(AssertionError, match=".*only ReplayBuffer is supported.*"):
+    with pytest.raises(AssertionError, match="only ReplayBuffer is supported"):
         _run_reward_relabel_sac_preference_comparisons(buffers.DictReplayBuffer)
-    with pytest.raises(AssertionError, match=".*only ReplayBuffer is supported.*"):
+    with pytest.raises(AssertionError, match="only ReplayBuffer is supported"):
         _run_reward_relabel_sac_preference_comparisons(HerReplayBuffer)
 
 
 @pytest.mark.parametrize(
     "named_configs",
     (
         [],
         ["reward.normalize_output_running"],
         ["reward.normalize_output_disable"],
     ),
 )
 def test_train_preference_comparisons_reward_named_config(tmpdir, named_configs):
-    config_updates = dict(common=dict(log_root=tmpdir))
+    config_updates = dict(logging=dict(log_root=tmpdir))
     run = train_preference_comparisons.train_preference_comparisons_ex.run(
         named_configs=["seals_cartpole"]
         + ALGO_FAST_CONFIGS["preference_comparison"]
         + named_configs,
         config_updates=config_updates,
     )
     if "reward.normalize_output_running" in named_configs:
@@ -256,16 +267,16 @@
 
 def test_train_dagger_main(tmpdir):
     with pytest.warns(None) as record:
         run = train_imitation.train_imitation_ex.run(
             command_name="dagger",
             named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
             config_updates=dict(
-                common=dict(log_root=tmpdir),
-                demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+                logging=dict(log_root=tmpdir),
+                demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
             ),
         )
     for warning in record:
         # PyTorch wants writeable arrays.
         # See https://github.com/HumanCompatibleAI/imitation/issues/219
         assert not (
             warning.category == UserWarning
@@ -276,72 +287,94 @@
 
 
 def test_train_dagger_warmstart(tmpdir):
     run = train_imitation.train_imitation_ex.run(
         command_name="dagger",
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
         config_updates=dict(
-            common=dict(log_root=tmpdir),
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+            logging=dict(log_root=tmpdir),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
         ),
     )
     assert run.status == "COMPLETED"
 
-    log_dir = types.parse_path(run.config["common"]["log_dir"])
+    log_dir = util.parse_path(run.config["logging"]["log_dir"])
     policy_path = log_dir / "scratch" / "policy-latest.pt"
     run_warmstart = train_imitation.train_imitation_ex.run(
         command_name="dagger",
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
         config_updates=dict(
-            common=dict(log_root=tmpdir),
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
-            agent_path=policy_path,
+            logging=dict(log_root=tmpdir),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
+            bc=dict(agent_path=policy_path),
         ),
     )
     assert run_warmstart.status == "COMPLETED"
     assert isinstance(run_warmstart.result, dict)
 
 
 def test_train_bc_main_with_none_demonstrations_raises_value_error(tmpdir):
-    with pytest.raises(ValueError, match=".*n_expert_demos.*rollout_path.*"):
+    with pytest.raises(ValueError, match="n_expert_demos must be specified"):
         train_imitation.train_imitation_ex.run(
             command_name="bc",
             named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
             config_updates=dict(
-                common=dict(log_root=tmpdir),
+                logging=dict(log_root=tmpdir),
                 demonstrations=dict(n_expert_demos=None),
             ),
         )
 
 
+def test_train_bc_main_with_demonstrations_from_huggingface(tmpdir):
+    train_imitation.train_imitation_ex.run(
+        command_name="bc",
+        named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
+        config_updates=dict(
+            logging=dict(log_root=tmpdir),
+            demonstrations=dict(
+                source="huggingface",
+                algo_name="ppo",
+            ),
+        ),
+    )
+
+
 @pytest.fixture(
     params=[
         "expert_from_path",
         "expert_from_huggingface",
         "random_expert",
         "zero_expert",
     ],
 )
 def bc_config(tmpdir, request):
-    expert_config = dict(
-        expert_from_path=dict(
+    environment_named_config = "seals_cartpole"
+
+    if request.param == "expert_from_path":
+        expert_config = dict(
             policy_type="ppo",
             loader_kwargs=dict(path=CARTPOLE_TEST_POLICY_PATH / "model.zip"),
-        ),
-        expert_from_huggingface=dict(policy_type="ppo-huggingface"),
-        random_expert=dict(policy_type="random"),
-        zero_expert=dict(policy_type="zero"),
-    )[request.param]
+        )
+        # Note: we don't have a seals_cartpole expert in our testdata folder,
+        # so we use the cartpole environment in this case.
+        environment_named_config = "cartpole"
+    elif request.param == "expert_from_huggingface":
+        expert_config = dict(policy_type="ppo-huggingface")
+    elif request.param == "random_expert":
+        expert_config = dict(policy_type="random")
+    elif request.param == "zero_expert":
+        expert_config = dict(policy_type="zero")
+
     return dict(
         command_name="bc",
-        named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
+        named_configs=[environment_named_config] + ALGO_FAST_CONFIGS["imitation"],
         config_updates=dict(
-            common=dict(log_root=tmpdir),
+            logging=dict(log_root=tmpdir),
             expert=expert_config,
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
         ),
     )
 
 
 def test_train_bc_main(bc_config):
     run = train_imitation.train_imitation_ex.run(**bc_config)
     assert run.status == "COMPLETED"
@@ -349,81 +382,81 @@
 
 
 def test_train_bc_warmstart(tmpdir):
     run = train_imitation.train_imitation_ex.run(
         command_name="bc",
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
         config_updates=dict(
-            common=dict(log_root=tmpdir),
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+            logging=dict(log_root=tmpdir),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
             expert=dict(policy_type="ppo-huggingface"),
         ),
     )
     assert run.status == "COMPLETED"
     assert isinstance(run.result, dict)
 
-    policy_path = types.parse_path(run.config["common"]["log_dir"]) / "final.th"
+    policy_path = util.parse_path(run.config["logging"]["log_dir"]) / "final.th"
     run_warmstart = train_imitation.train_imitation_ex.run(
         command_name="bc",
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
         config_updates=dict(
-            common=dict(log_root=tmpdir),
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
-            agent_path=policy_path,
+            logging=dict(log_root=tmpdir),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
+            bc=dict(agent_path=policy_path),
         ),
     )
 
     assert run_warmstart.status == "COMPLETED"
     assert isinstance(run_warmstart.result, dict)
 
 
 @pytest.fixture(params=["cold_start", "warm_start"])
 def rl_train_ppo_config(request, tmpdir):
-    config = dict(common=dict(log_root=tmpdir))
+    config = dict(logging=dict(log_root=tmpdir))
     if request.param == "warm_start":
         # FIXME(yawen): the policy we load was trained on 8 parallel environments
         #  and for some reason using it breaks if we use just 1 (like would be the
         #  default with the fast named_config)
         config["agent_path"] = CARTPOLE_TEST_POLICY_PATH / "model.zip"
-        config["common"] = dict(num_vec=8)
+        config["environment"] = dict(num_vec=8)
     return config
 
 
 def test_train_rl_main(tmpdir, rl_train_ppo_config):
     """Smoke test for imitation.scripts.train_rl."""
-    config_updates = dict(common=dict(log_root=tmpdir))
+    config_updates = dict(logging=dict(log_root=tmpdir))
     sacred.utils.recursive_update(config_updates, rl_train_ppo_config)
     run = train_rl.train_rl_ex.run(
         named_configs=["cartpole"] + ALGO_FAST_CONFIGS["rl"],
         config_updates=config_updates,
     )
     assert run.status == "COMPLETED"
     assert isinstance(run.result, dict)
 
 
 def test_train_rl_wb_logging(tmpdir):
-    """Smoke test for imitation.scripts.common.common.wandb_logging."""
-    with pytest.raises(Exception, match=".*api_key not configured.*"):
+    """Smoke test for imitation.scripts.ingredients.logging.wandb_logging."""
+    with pytest.raises(Exception, match="api_key not configured"):
         train_rl.train_rl_ex.run(
             named_configs=["cartpole"]
             + ALGO_FAST_CONFIGS["rl"]
-            + ["common.wandb_logging"],
+            + ["logging.wandb_logging"],
             config_updates=dict(
-                common=dict(log_root=tmpdir),
+                logging=dict(log_root=tmpdir),
             ),
         )
 
 
 def test_train_rl_sac(tmpdir):
     run = train_rl.train_rl_ex.run(
         # make sure rl.sac named_config is called after rl.fast to overwrite
         # rl_kwargs.batch_size to None
         named_configs=["pendulum"] + ALGO_FAST_CONFIGS["rl"] + RL_SAC_NAMED_CONFIGS,
         config_updates=dict(
-            common=dict(log_root=tmpdir),
+            logging=dict(log_root=tmpdir),
         ),
     )
     assert run.config["rl"]["rl_cls"] is stable_baselines3.SAC
     assert run.status == "COMPLETED"
     assert isinstance(run.result, dict)
 
 
@@ -443,15 +476,15 @@
         ],
     )
 
 
 @pytest.mark.parametrize("config", EVAL_POLICY_CONFIGS)
 def test_eval_policy(config, tmpdir):
     """Smoke test for imitation.scripts.eval_policy."""
-    config_updates = dict(common=dict(log_root=tmpdir))
+    config_updates = dict(logging=dict(log_root=tmpdir))
     config_updates.update(config)
     run = eval_policy.eval_policy_ex.run(
         config_updates=config_updates,
         named_configs=ALGO_FAST_CONFIGS["eval_policy"],
     )
     assert run.status == "COMPLETED"
     wrapped_reward = "reward_type" in config
@@ -482,27 +515,27 @@
     _check_rollout_stats(imit_stats)
 
 
 @pytest.mark.parametrize(
     "named_configs",
     (
         [],
-        ["train.normalize_running", "reward.normalize_input_running"],
+        ["policy.normalize_running", "reward.normalize_input_running"],
         ["reward.normalize_input_disable"],
     ),
 )
 @pytest.mark.parametrize("command", ("airl", "gail"))
 def test_train_adversarial(tmpdir, named_configs, command):
     """Smoke test for imitation.scripts.train_adversarial."""
     named_configs = (
         named_configs + ["seals_cartpole"] + ALGO_FAST_CONFIGS["adversarial"]
     )
     config_updates = {
-        "common": dict(log_root=tmpdir),
-        "demonstrations": dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+        "logging": dict(log_root=tmpdir),
+        "demonstrations": dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
         # TensorBoard logs to get extra coverage
         "algorithm_kwargs": dict(init_tensorboard=True),
     }
     run = train_adversarial.train_adversarial_ex.run(
         command_name=command,
         named_configs=named_configs,
         config_updates=config_updates,
@@ -511,24 +544,24 @@
     _check_train_ex_result(run.result)
 
 
 @pytest.mark.parametrize("command", ("airl", "gail"))
 def test_train_adversarial_warmstart(tmpdir, command):
     named_configs = ["cartpole"] + ALGO_FAST_CONFIGS["adversarial"]
     config_updates = {
-        "common": dict(log_root=tmpdir),
-        "demonstrations": dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+        "logging": dict(log_root=tmpdir),
+        "demonstrations": dict(path=CARTPOLE_TEST_ROLLOUT_PATH, source="local"),
     }
     run = train_adversarial.train_adversarial_ex.run(
         command_name=command,
         named_configs=named_configs,
         config_updates=config_updates,
     )
 
-    log_dir = types.parse_path(run.config["common"]["log_dir"])
+    log_dir = util.parse_path(run.config["logging"]["log_dir"])
     policy_path = log_dir / "checkpoints" / "final" / "gen_policy"
 
     run_warmstart = train_adversarial.train_adversarial_ex.run(
         command_name=command,
         named_configs=named_configs,
         config_updates={
             "agent_path": policy_path,
@@ -545,16 +578,16 @@
     """Smoke test for imitation.scripts.train_adversarial."""
     # Make sure rl.sac named_config is called after rl.fast to overwrite
     # rl_kwargs.batch_size to None
     named_configs = (
         ["pendulum"] + ALGO_FAST_CONFIGS["adversarial"] + RL_SAC_NAMED_CONFIGS
     )
     config_updates = {
-        "common": dict(log_root=tmpdir),
-        "demonstrations": dict(rollout_path=PENDULUM_TEST_ROLLOUT_PATH),
+        "logging": dict(log_root=tmpdir),
+        "demonstrations": dict(path=PENDULUM_TEST_ROLLOUT_PATH),
     }
     run = train_adversarial.train_adversarial_ex.run(
         command_name=command,
         named_configs=named_configs,
         config_updates=config_updates,
     )
     assert run.config["rl"]["rl_cls"] is stable_baselines3.SAC
@@ -563,39 +596,39 @@
 
 
 def test_train_adversarial_algorithm_value_error(tmpdir):
     """Error on bad algorithm arguments."""
     base_named_configs = ["cartpole"] + ALGO_FAST_CONFIGS["adversarial"]
     base_config_updates = collections.ChainMap(
         {
-            "common": dict(log_root=tmpdir),
-            "demonstrations": dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+            "logging": dict(log_root=tmpdir),
+            "demonstrations": dict(path=CARTPOLE_TEST_ROLLOUT_PATH, source="local"),
         },
     )
 
-    with pytest.raises(TypeError, match=".*BAD_VALUE.*"):
+    with pytest.raises(TypeError, match="BAD_VALUE"):
         train_adversarial.train_adversarial_ex.run(
             command_name="gail",
             named_configs=base_named_configs,
             config_updates=base_config_updates.new_child(
                 dict(algorithm_kwargs={"BAD_VALUE": "bar"}),
             ),
         )
 
-    with pytest.raises(FileNotFoundError, match=".*BAD_VALUE.*"):
+    with pytest.raises(FileNotFoundError, match="BAD_VALUE"):
         train_adversarial.train_adversarial_ex.run(
             command_name="gail",
             named_configs=base_named_configs,
             config_updates=base_config_updates.new_child(
-                {"demonstrations.rollout_path": "path/BAD_VALUE"},
+                {"demonstrations.path": "path/BAD_VALUE"},
             ),
         )
 
     n_traj = 1234567
-    with pytest.raises(ValueError, match=f".*{n_traj}.*"):
+    with pytest.raises(ValueError, match=f"{n_traj}"):
         train_adversarial.train_adversarial_ex.run(
             command_name="gail",
             named_configs=base_named_configs,
             config_updates=base_config_updates.new_child(
                 {"demonstrations.n_expert_demos": n_traj},
             ),
         )
@@ -605,48 +638,48 @@
     """Transfer learning smoke test.
 
     Saves a dummy AIRL test reward, then loads it for transfer learning.
 
     Args:
         tmpdir: Temporary directory to save results to.
     """
-    tmpdir_path = types.parse_path(tmpdir)
+    tmpdir_path = util.parse_path(tmpdir)
     log_dir_train = tmpdir_path / "train"
     run = train_adversarial.train_adversarial_ex.run(
         command_name="airl",
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["adversarial"],
         config_updates=dict(
-            common=dict(log_dir=log_dir_train),
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+            logging=dict(log_dir=log_dir_train),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
         ),
     )
     assert run.status == "COMPLETED"
     _check_train_ex_result(run.result)
 
     _check_rollout_stats(run.result["imit_stats"])
 
     log_dir_data = tmpdir_path / "train_rl"
     reward_path = log_dir_train / "checkpoints" / "final" / "reward_test.pt"
     run = train_rl.train_rl_ex.run(
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["rl"],
         config_updates=dict(
-            common=dict(log_dir=log_dir_data),
+            logging=dict(log_dir=log_dir_data),
             reward_type="RewardNet_unshaped",
             reward_path=reward_path,
         ),
     )
     assert run.status == "COMPLETED"
     _check_rollout_stats(run.result)
 
 
 @pytest.mark.parametrize(
     "named_configs_dict",
     (
         dict(pc=[], rl=[]),
-        dict(pc=["rl.sac", "train.sac"], rl=["rl.sac", "train.sac"]),
+        dict(pc=["rl.sac", "policy.sac"], rl=["rl.sac", "policy.sac"]),
         dict(pc=["reward.reward_ensemble"], rl=[]),
     ),
 )
 def test_preference_comparisons_transfer_learning(
     tmpdir: str,
     named_configs_dict: Mapping[str, List[str]],
 ) -> None:
@@ -654,22 +687,22 @@
 
     Saves a preference comparisons ensemble reward, then loads it for transfer learning.
 
     Args:
         tmpdir: Temporary directory to save results to.
         named_configs_dict: Named configs for preference_comparisons and rl.
     """
-    tmpdir_path = types.parse_path(tmpdir)
+    tmpdir_path = util.parse_path(tmpdir)
 
     log_dir_train = tmpdir_path / "train"
     run = train_preference_comparisons.train_preference_comparisons_ex.run(
         named_configs=["pendulum"]
         + ALGO_FAST_CONFIGS["preference_comparison"]
         + named_configs_dict["pc"],
-        config_updates=dict(common=dict(log_dir=log_dir_train)),
+        config_updates=dict(logging=dict(log_dir=log_dir_train)),
     )
     assert run.status == "COMPLETED"
 
     if "reward.reward_ensemble" in named_configs_dict["pc"]:
         assert run.config["reward"]["net_cls"] is reward_nets.RewardEnsemble
         assert run.config["reward"]["add_std_alpha"] == 0.0
         reward_type = "RewardNet_std_added"
@@ -680,15 +713,15 @@
 
     log_dir_data = tmpdir_path / "train_rl"
     reward_path = log_dir_train / "checkpoints" / "final" / "reward_net.pt"
     agent_path = log_dir_train / "checkpoints" / "final" / "policy"
     run = train_rl.train_rl_ex.run(
         named_configs=["pendulum"] + ALGO_FAST_CONFIGS["rl"] + named_configs_dict["rl"],
         config_updates=dict(
-            common=dict(log_dir=log_dir_data),
+            logging=dict(log_dir=log_dir_data),
             reward_type=reward_type,
             reward_path=reward_path,
             load_reward_kwargs=load_reward_kwargs,
             agent_path=agent_path,
         ),
     )
     assert run.status == "COMPLETED"
@@ -709,20 +742,20 @@
     net = reward_nets.NormalizedRewardNet(basic_reward_net, networks.RunningNorm)
     tmppath = os.path.join(tmpdir, "reward.pt")
     th.save(net, tmppath)
 
     log_dir_data = os.path.join(tmpdir, "train_rl")
     with pytest.warns(
         RuntimeWarning,
-        match=r"Applying normalization to already normalized reward function.*",
+        match=r"Applying normalization to already normalized reward function",
     ):
         train_rl.train_rl_ex.run(
             named_configs=["cartpole"] + ALGO_FAST_CONFIGS["rl"],
             config_updates=dict(
-                common=dict(log_dir=log_dir_data),
+                logging=dict(log_dir=log_dir_data),
                 reward_type="RewardNet_normalized",
                 normalize_reward=True,
                 reward_path=tmppath,
             ),
         )
 
 
@@ -735,17 +768,18 @@
     )
     net = reward_nets.CnnRewardNet(venv.observation_space, venv.action_space)
     tmppath = os.path.join(tmpdir, "reward.pt")
     th.save(net, tmppath)
 
     log_dir_data = os.path.join(tmpdir, "train_rl")
     run = train_rl.train_rl_ex.run(
-        named_configs=["train.cnn_policy"] + ALGO_FAST_CONFIGS["rl"],
+        named_configs=["policy.cnn_policy"] + ALGO_FAST_CONFIGS["rl"],
         config_updates=dict(
-            common=dict(log_dir=log_dir_data, env_name="AsteroidsNoFrameskip-v4"),
+            environment=dict(gym_id="AsteroidsNoFrameskip-v4"),
+            logging=dict(log_dir=log_dir_data),
             reward_path=tmppath,
         ),
     )
     assert run.status == "COMPLETED"
     assert isinstance(run.result, dict)
 
 
@@ -762,15 +796,15 @@
         },
     ),
     dict(
         sacred_ex_name="train_adversarial",
         base_named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["adversarial"],
         base_config_updates={
             # Need absolute path because raylet runs in different working directory.
-            "demonstrations.rollout_path": CARTPOLE_TEST_ROLLOUT_PATH.absolute(),
+            "demonstrations.path": CARTPOLE_TEST_ROLLOUT_PATH.absolute(),
         },
         search_space={
             "command_name": tune.grid_search(["gail", "airl"]),
         },
     ),
 ]
 
@@ -784,108 +818,108 @@
 
 @pytest.mark.parametrize("config_updates", PARALLEL_CONFIG_UPDATES)
 def test_parallel(config_updates, tmpdir):
     """Hyperparam tuning smoke test."""
     # CI server only has 2 cores
     config_updates = dict(config_updates)
     config_updates.update(PARALLEL_CONFIG_LOW_RESOURCE)
-    config_updates.setdefault("base_config_updates", {})["common.log_root"] = tmpdir
+    config_updates.setdefault("base_config_updates", {})["logging.log_root"] = tmpdir
     run = parallel.parallel_ex.run(config_updates=config_updates)
     assert run.status == "COMPLETED"
 
 
 def test_parallel_arg_errors(tmpdir):
     """Error on bad algorithm arguments."""
     config_updates = dict(PARALLEL_CONFIG_LOW_RESOURCE)
-    config_updates.setdefault("base_config_updates", {})["common.log_root"] = tmpdir
+    config_updates.setdefault("base_config_updates", {})["logging.log_root"] = tmpdir
     config_updates = collections.ChainMap(config_updates)
 
-    with pytest.raises(TypeError, match=".*Sequence.*"):
+    with pytest.raises(TypeError, match="Sequence"):
         parallel.parallel_ex.run(
             config_updates=config_updates.new_child(dict(base_named_configs={})),
         )
 
-    with pytest.raises(TypeError, match=".*Mapping.*"):
+    with pytest.raises(TypeError, match="Mapping"):
         parallel.parallel_ex.run(
             config_updates=config_updates.new_child(dict(base_config_updates=())),
         )
 
-    with pytest.raises(TypeError, match=".*Sequence.*"):
+    with pytest.raises(TypeError, match="Sequence"):
         parallel.parallel_ex.run(
             config_updates=config_updates.new_child(
                 dict(search_space={"named_configs": {}}),
             ),
         )
 
-    with pytest.raises(TypeError, match=".*Mapping.*"):
+    with pytest.raises(TypeError, match="Mapping"):
         parallel.parallel_ex.run(
             config_updates=config_updates.new_child(
                 dict(search_space={"config_updates": ()}),
             ),
         )
 
 
 def _generate_test_rollouts(tmpdir: str, env_named_config: str) -> pathlib.Path:
-    tmpdir_path = types.parse_path(tmpdir)
+    tmpdir_path = util.parse_path(tmpdir)
     train_rl.train_rl_ex.run(
         named_configs=[env_named_config] + ALGO_FAST_CONFIGS["rl"],
         config_updates=dict(
-            common=dict(log_dir=tmpdir),
+            logging=dict(log_dir=tmpdir),
         ),
     )
-    rollout_path = tmpdir_path / "rollouts/final.npz"
-    return rollout_path.absolute()
+    path = tmpdir_path / "rollouts/final.npz"
+    return path.absolute()
 
 
 def test_parallel_train_adversarial_custom_env(tmpdir):
     if os.name == "nt":  # pragma: no cover
         pytest.skip(
             "`ray.init()` times out when this test runs concurrently with other "
             "test_parallel tests on Windows (e.g., `pytest -n auto -k test_parallel`)",
         )
 
     env_named_config = "pendulum"
-    rollout_path = _generate_test_rollouts(tmpdir, env_named_config)
+    path = _generate_test_rollouts(tmpdir, env_named_config)
 
     config_updates = dict(
         sacred_ex_name="train_adversarial",
         n_seeds=1,
         base_named_configs=[env_named_config] + ALGO_FAST_CONFIGS["adversarial"],
         base_config_updates=dict(
-            common=dict(log_root=tmpdir),
-            demonstrations=dict(rollout_path=rollout_path),
+            logging=dict(log_root=tmpdir),
+            demonstrations=dict(path=path),
         ),
         search_space=dict(command_name="gail"),
     )
     config_updates.update(PARALLEL_CONFIG_LOW_RESOURCE)
     run = parallel.parallel_ex.run(config_updates=config_updates)
     assert run.status == "COMPLETED"
 
 
 def _run_train_adv_for_test_analyze_imit(run_name, sacred_logs_dir, log_dir):
     run = train_adversarial.train_adversarial_ex.run(
         command_name="gail",
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["adversarial"],
         config_updates=dict(
-            common=dict(log_root=log_dir),
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+            logging=dict(log_root=log_dir),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
             checkpoint_interval=-1,
         ),
         options={"--name": run_name, "--file_storage": sacred_logs_dir},
     )
     return run
 
 
 def _run_train_bc_for_test_analyze_imit(run_name, sacred_logs_dir, log_dir):
     run = train_imitation.train_imitation_ex.run(
         command_name="bc",
         named_configs=["seals_cartpole"] + ALGO_FAST_CONFIGS["imitation"],
         config_updates=dict(
-            common=dict(log_dir=log_dir),
-            demonstrations=dict(rollout_path=CARTPOLE_TEST_ROLLOUT_PATH),
+            logging=dict(log_dir=log_dir),
+            demonstrations=dict(path=CARTPOLE_TEST_ROLLOUT_PATH),
         ),
         options={"--name": run_name, "--file_storage": sacred_logs_dir},
     )
     return run
 
 
 @pytest.mark.parametrize("run_names", ([], list("adab")))
@@ -893,15 +927,15 @@
     "run_sacred_fn",
     (
         _run_train_adv_for_test_analyze_imit,
         _run_train_bc_for_test_analyze_imit,
     ),
 )
 def test_analyze_imitation(tmpdir: str, run_names: List[str], run_sacred_fn):
-    sacred_logs_dir = tmpdir_path = types.parse_path(tmpdir)
+    sacred_logs_dir = tmpdir_path = util.parse_path(tmpdir)
 
     # Generate sacred logs (other logs are put in separate tmpdir for deletion).
     for run_name in run_names:
         with tempfile.TemporaryDirectory(prefix="junk") as log_dir:
             run = run_sacred_fn(run_name, sacred_logs_dir, log_dir)
             assert run.status == "COMPLETED"
 
@@ -947,36 +981,71 @@
         ),
     )
     assert run.status == "COMPLETED"
     assert isinstance(run.result, dict)
     assert run.result["n_tb_dirs"] == 2
 
 
-def test_convert_trajs(tmpdir: str):
-    """Tests that convert_trajs is idempotent and does not change the data."""
-    shutil.copy(OLD_FMT_ROLLOUT_TEST_DATA_PATH, tmpdir)
-    tmp_path = os.path.join(tmpdir, os.path.basename(OLD_FMT_ROLLOUT_TEST_DATA_PATH))
-    with open(tmp_path, "rb") as f:
-        pickle.load(f)  # check it's in pickle format to start with
-    args = ["convert_trajs.py", tmp_path]
-    with mock.patch.object(sys, "argv", args):
-        convert_trajs.main()
-
-    npz_tmp_path = tmp_path.replace(".pkl", ".npz")
-    np.load(npz_tmp_path, allow_pickle=True)  # check it's now in npz format
-
-    shutil.copy(npz_tmp_path, npz_tmp_path + ".orig")
-    args = ["convert_trajs.py", npz_tmp_path]
-    with mock.patch.object(sys, "argv", args):
-        convert_trajs.main()
-
-    assert filecmp.cmp(
-        npz_tmp_path,
-        npz_tmp_path + ".orig",
-    ), "convert_trajs not idempotent"
+def test_pickle_fmt_rollout_test_data_is_pickle():
+    # WHEN
+    with open(PICKLE_FMT_ROLLOUT_TEST_DATA_PATH, "rb") as f:
+        pickle.load(f)
+
+    # THEN
+    # No exception raised
+
+
+def test_npz_fmt_rollout_test_data_is_npz():
+    # WHEN
+    np.load(NPZ_FMT_ROLLOUT_TEST_DATA_PATH, allow_pickle=False)
+
+    # THEN
+    # No exception raised
+
+
+@pytest.fixture(
+    params=[PICKLE_FMT_ROLLOUT_TEST_DATA_PATH, NPZ_FMT_ROLLOUT_TEST_DATA_PATH],
+    ids=["pickle", "npz"],
+)
+def old_rollouts_file_in_tmp(tmpdir, request) -> Generator[str, None, None]:
+    old_rollouts_file = request.param
+    shutil.copy(old_rollouts_file, tmpdir)
+    yield os.path.join(tmpdir, os.path.basename(old_rollouts_file))
+
 
-    from_pkl = types.load(tmp_path)
-    from_npz = types.load(npz_tmp_path)
+@pytest.fixture()
+def new_rollouts_file_in_tmp(tmpdir) -> Generator[pathlib.Path, None, None]:
+    # Note: here we just convert some old rollouts to the new format, so we don't need
+    #  to keep trajectories in the new format in the testdata folder
+    npz_rollouts_in_tmp = shutil.copy(NPZ_FMT_ROLLOUT_TEST_DATA_PATH, tmpdir)
+    yield convert_trajs.update_traj_file_in_place(npz_rollouts_in_tmp)
 
-    assert len(from_pkl) == len(from_npz)
-    for t_pkl, t_npz in zip(from_pkl, from_npz):
-        assert t_pkl == t_npz
+
+def test_converted_trajectories_equal_original(old_rollouts_file_in_tmp: str):
+    # GIVEN
+    old_trajs = serialize.load(old_rollouts_file_in_tmp)
+
+    # WHEN
+    converted_path = convert_trajs.update_traj_file_in_place(old_rollouts_file_in_tmp)
+
+    # THEN
+    converted_trajs = serialize.load(converted_path)
+
+    assert len(old_trajs) == len(converted_trajs)
+    for t_old, t_converted in zip(old_trajs, converted_trajs):
+        assert t_old == t_converted
+
+
+def test_convert_trajs_from_current_format_is_idempotent(
+    new_rollouts_file_in_tmp: pathlib.Path,
+):
+    # GIVEN
+    original_path = new_rollouts_file_in_tmp.with_suffix(".orig")
+
+    # WHEN
+    shutil.copytree(new_rollouts_file_in_tmp, original_path)
+    converted_path = convert_trajs.update_traj_file_in_place(new_rollouts_file_in_tmp)
+
+    # THEN
+    assert (
+        filecmp.dircmp(converted_path, original_path).diff_files == []
+    ), "convert_trajs not idempotent"
```

### Comparing `imitation-0.3.2/tests/test_examples.py` & `imitation-0.4.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/test_regularization.py` & `imitation-0.4.0/tests/test_regularization.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/testdata/expert_models/cartpole_0/policies/final/model.zip` & `imitation-0.4.0/tests/testdata/expert_models/cartpole_0/policies/final/model.zip`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 39774 bytes, number of entries: 6
-?rw-------  2.0 unx    14858 b- stor 22-Apr-22 12:52 data
+Zip file size: 59287 bytes, number of entries: 6
+?rw-------  2.0 unx    14327 b- stor 23-May-03 11:47 data
 ?rw-------  2.0 unx      431 b- stor 80-Jan-01 00:00 pytorch_variables.pth
-?rw-------  2.0 unx     8964 b- stor 80-Jan-01 00:00 policy.pth
-?rw-------  2.0 unx    14645 b- stor 80-Jan-01 00:00 policy.optimizer.pth
-?rw-------  2.0 unx        5 b- stor 22-Apr-22 12:52 _stable_baselines3_version
-?rw-------  2.0 unx      201 b- stor 22-Apr-22 12:52 system_info.txt
-6 files, 39104 bytes uncompressed, 39104 bytes compressed:  0.0%
+?rw-------  2.0 unx    14145 b- stor 80-Jan-01 00:00 policy.pth
+?rw-------  2.0 unx    29433 b- stor 80-Jan-01 00:00 policy.optimizer.pth
+?rw-------  2.0 unx        5 b- stor 23-May-03 11:47 _stable_baselines3_version
+?rw-------  2.0 unx      216 b- stor 23-May-03 11:47 system_info.txt
+6 files, 58557 bytes uncompressed, 58557 bytes compressed:  0.0%
```

#### data

##### Pretty-printed

 * *Similarity: 0.9138471177944861%*

 * *Differences: {"'_last_obs'": "{':serialized:': "*

 * *                "'gAWV9QAAAAAAAACMEm51bXB5LmNvcmUubnVtZXJpY5SMC19mcm9tYnVmZmVylJOUKJaAAAAAAAAAALBNoD6Y8r2+gPc/vFoBAD+0Dog9rRFkvilCqzu9+NI+BJ62PerNv7wzZnI7ceiJPK5GhT7QBF6+hPh5u1brGj7c7AQ+Ln/vPEmxkzu7bVu9+3icPJVl4zx+Rt475MggPI4rnD738iM8/PlOvWimoz1Q3YU+24dkvIlqgzykviK8lIwFbnVtcHmUjAVkdHlwZZSTlIwCZjSUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYksISwSGlIwBQ5R0lFKULg=='}",*

 * * "'_last_original_obs'": "{':serialized:': "*

 * *                         "'gAWV9QAAAAAAAACMEm51bXB5LmNvcmUubnVtZ […]*

```diff
@@ -2,53 +2,54 @@
     "_current_progress_remaining": -0.0035199999999999676,
     "_episode_num": 0,
     "_last_episode_starts": {
         ":serialized:": "gAWVewAAAAAAAACMEm51bXB5LmNvcmUubnVtZXJpY5SMC19mcm9tYnVmZmVylJOUKJYIAAAAAAAAAAAAAAAAAAAAlIwFbnVtcHmUjAVkdHlwZZSTlIwCYjGUiYiHlFKUKEsDjAF8lE5OTkr/////Sv////9LAHSUYksIhZSMAUOUdJRSlC4=",
         ":type:": "<class 'numpy.ndarray'>"
     },
     "_last_obs": {
-        ":serialized:": "gAWV9QAAAAAAAACMEm51bXB5LmNvcmUubnVtZXJpY5SMC19mcm9tYnVmZmVylJOUKJaAAAAAAAAAAP1e8L871hy/6ooKPB1D7z4ijIW81V1YvoFZk7vniTA+yLQFvr3hRL7doNa7uHHuPSu7Xb9zfNi+nxKiu6Hjhj4ckLW/kKqivjEMjLvlj8o70F9Kv7EIo74B0uW76vbqPT6T8r9OqRC/l5bXvIUFlD7iqmG/OFIwvn5tITznnBy+lIwFbnVtcHmUjAVkdHlwZZSTlIwCZjSUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYksISwSGlIwBQ5R0lFKULg==",
+        ":serialized:": "gAWV9QAAAAAAAACMEm51bXB5LmNvcmUubnVtZXJpY5SMC19mcm9tYnVmZmVylJOUKJaAAAAAAAAAALBNoD6Y8r2+gPc/vFoBAD+0Dog9rRFkvilCqzu9+NI+BJ62PerNv7wzZnI7ceiJPK5GhT7QBF6+hPh5u1brGj7c7AQ+Ln/vPEmxkzu7bVu9+3icPJVl4zx+Rt475MggPI4rnD738iM8/PlOvWimoz1Q3YU+24dkvIlqgzykviK8lIwFbnVtcHmUjAVkdHlwZZSTlIwCZjSUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYksISwSGlIwBQ5R0lFKULg==",
         ":type:": "<class 'numpy.ndarray'>"
     },
     "_last_original_obs": {
-        ":serialized:": "gAWV9QAAAAAAAACMEm51bXB5LmNvcmUubnVtZXJpY5SMC19mcm9tYnVmZmVylJOUKJaAAAAAAAAAANAuqDz4GQe9ejDSOzmn7DzKRQG9Syg0u785TL0Wxjw9gQQnvV/2E73JCcg8gc5FPS2WKr0rlCm9GGecvD7VyDyiM9q8AwlrvA5qEDzAXBC9RJgwPWe7OTx9dUK8RnEMvXXwN72kGxg9qsxmu7Qjv7mNMGS8zYgiPT58HD1nB5y8lIwFbnVtcHmUjAVkdHlwZZSTlIwCZjSUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYksISwSGlIwBQ5R0lFKULg==",
+        ":serialized:": "gAWV9QAAAAAAAACMEm51bXB5LmNvcmUubnVtZXJpY5SMC19mcm9tYnVmZmVylJOUKJaAAAAAAAAAAKtxOL2bDPm8TePkPAi7MT0qGT09rz+IPEizkrzyuRO92XdEPZVTXTxnUam8PU+Zuzx4Mj2YG6U6i2PJPFyEMD3FZR89jIvHvElWyrxEfki9K3AuvYEfLz2Olx89/XWHPH0V3LvxTYo8g/UYvXF9gTw710C99D5BPWBHSD0VlCQ9lIwFbnVtcHmUjAVkdHlwZZSTlIwCZjSUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYksISwSGlIwBQ5R0lFKULg==",
         ":type:": "<class 'numpy.ndarray'>"
     },
     "_n_updates": 490,
     "_num_timesteps_at_start": 0,
+    "_stats_window_size": 100,
     "_total_timesteps": 100000,
     "action_noise": null,
     "action_space": {
-        ":serialized:": "gAWVNQsAAAAAAACME2d5bS5zcGFjZXMuZGlzY3JldGWUjAhEaXNjcmV0ZZSTlCmBlH2UKIwBbpRLAowGX3NoYXBllCmMBWR0eXBllIwFbnVtcHmUjAVkdHlwZZSTlIwCaTiUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYowKX25wX3JhbmRvbZSMFG51bXB5LnJhbmRvbS5fcGlja2xllIwSX19yYW5kb21zdGF0ZV9jdG9ylJOUjAdNVDE5OTM3lIWUUpR9lCiMDWJpdF9nZW5lcmF0b3KUaBSMBXN0YXRllH2UKIwDa2V5lIwSbnVtcHkuY29yZS5udW1lcmljlIwLX2Zyb21idWZmZXKUk5QolsAJAAAAAAAAAAAAgDB7o6CniLOKTNzKIPVbV/zHdtv7FMLFp28bL8uc9jPFJAET2fIVTRroV/vCkccOMTnOc1+OcovNcQIJSnBDD2j3r1ECM6cD38obyBzAkvKGK3SFVtBjEH8kfRhWzLKyVIKZEL6l8LmdxoUifXYzW76dN6Lr/r0VrAjvyYCYqLPtjm07hEejps7ZRNAyM4OorO7+ZeEbux1IRexQdiYBOCHgkJPGuNa9XmL546wIaBvc3IDc8HbPssECyaSIN+atF7JmTV/IHmkb8GYbgSkPnWRxqe3VWFrQqWZjd61n+X/hsSrCRbK8JNbh6kffI1XlMKqNrp/Iniju7or2dEcCCo0xsKpKPigOxcVWYjjTc3YNQBzR0ln95YuW2y21VhNB7P+PWtbw3S+kGunh9bIh8sKYM0QSsIQ7Dt1ABsBkb7MVLVw9TEo9n9PGtD4atKgjG7Achvepxxyju8gkOZr7wudQ9YCNxiMch6ZHvbUO6SH5PHbuSUMDuE2yMuiiD9tzqS6Hr90EXTIZJwE6VP1vVoGWka5ecF5i22SbmElGvcnc/rrYqLfTWU/gBqTY+Kq2JlRrT7pfm+O7ymic7ENmRAGE/ybjY3LffevpHSBO/Nx0Db11GI0eTr2j3DhEvbx5QkKmQ1uWOOjyooYURFiTHuJJtMItODs6UCGVs8cyzIM92u7+eWslWSV5WR2DdbyO/xYbaDgVmp2Ytb6YeMOD+PKhYMEw7hPjFUYwbnVqEkmvhEE3tCa5uAXWYWueFRPlEishyhLCGEbzDcd+OprADENfVsrWbF8VJGLun/7d27+L9pLCQAbPmjy7c3Je1nasHBlVEbRBV6mUbI5QPDo9JZt0fcsWcA752anc+XbyqsItOW4k7WtXkWzZ5/P3Df+isFIda56/eMlEhS7zCG7681mQZhSN/h8dJPl7NiOl5WXOyPQc7J9oHz5zCVTbMQtoW90a4HQUq9O9GWkMMEk+GUTwJs/cwItvhVNS0Ul4nycaoDoQb17X8exEHxj3RAd+I0DM/ZYfOMPXdls4gA0aOOv+2yGkBijkwm0AQs8KNTjEeeY4RMQ3D2aX5+Qm3NCkw0RjXn3kJcTi6LyvLIDgQFnTgh9iUliVVGA7CCquevLGwegnY8x2CC4qS/ILMzmkbzxP7/Qxfad9CGSIZ7QGgSZe/Yy0ePx7q0I8gvsZwWJqs5KV3MIghecK+XVOBMysH8rVxADm9MT7T5OOUDscnsogv1HrDCMgebsAE8rVGAcEeTaVuw3Hbg0E8r3i+Lg5T0d5oJurKcVyvA5nuSx71gVt3PAE971HRNVy5uT4iVQHP1bKyn2VTNXSGy/M0cXDc+rp1lAHuMNIjXMQDxB1blLEyUXM4rsns+cTa2R9UrTUml8uDHXLZc80FSbgTgLQeTJUVJ6K39GxRC/Jxkr7aQEkyF1hb/XpmlOTr5mGMF7HUNnx3HrAPUMS4bHWOHyz730DCyVWnCeCDmzPwc03tJszFll0ringJZ6yuJ+5+M6y6E4M6tCKcgpELGbh4EGUnUrcmSL4W9zhThkS3O0odgTYUKUaFdODEJQm3gqMFpdTp9M3VN9+yd+3iwtnKYOmc1X5VbKPcJ9gifKN6WJDg7tu8f5jbg7CjkIwYT8affJvvepA5hUqCv+PxV3uZ84ZU3NSDi4l21dpoCNTWtPLWuhFUScDHg3qouvYVAgBJQzf5ANpqyRQ/lCxltcGqLp7Ks5ReKZmFjaRQZ0YKA4rKOGjbSa4m5+G+t4loBirjK9KxkDh+bn85oxN0cJQ4tpsFzAVFVXkjdPWWrjEuvag+kfOVqx8AptTJ4N/75ls6+ROQeY0VvGU9s3qsnipdwgs1q0kc9dse6+UEojVGpjj3JFeGQpRwRKUHJDllpu+WKbup6urLVJ1L73I0qv1nyy5ARtNl01DmKFqtt3eT6ct7oj2VhXIBlnjsb2u7BX0KsWZdFygB3o/m2rxzHt5FtvZu/k4tKEVEENVklMniGIrHz9hiMWaS9FW+rJNa5zHYUXxKty8edRcv9WNCr2AA8kEd20MIJGhz0QvMVfaUNezzPzBeuyL4quLWhdc9X07PGRMZqOIDM2NLLdCD0karnY2O/4U/zP+s+xbKs0jGbKBFjGelHQXaqHpv96qroHX5Nj2OfAAmp9K+pI7kr023K7EW98L3Dx7oojunQbQI3cva8oWwDp7nxH135D2ULo090jOwnKsIs0d0dxcivyT9FK5696gPrMtz1HgJJMBeidAOdOEO+n+3vi5natbtMPXeK/0M693/R1lf5aSB2Ob18lxiz74l6KfAG02eYRou/Od354kNhRkz7UvVye1JZFyjEfyGT9UGJRcojeUe5mz/Y+xsEUPgBLSWDZFp/3QSz0fp/cLFQJg025QkQeeYvCNDOFo5SH6AwzYgcz0SsgXDywsUpvb2KYX18UkDhkXAB5HUkUux19aBui6tlU1PaE/4+Mf+nhBUKd5tmRqG5pJHBZklrkJIYzJvERD0h8XjQikrcEYJrArkwgpI6MtRzYU+PAzgPd5kN7aAljGpohWrVIY3vCkq3uoSfz434kgCFmn7FB8gnOev6NX/bhz3raL1hrHOgsCWfm0NrPzd3RgHX/TXD4d0PIH7JQeI2chPOWx+mLDaAjhY9JZkpEAu5UDDKrSdxtduuYwPX/5ZIFvLvPZsyHktqNPUdAPNrzuyjTRDJbl4EYkl3St42qL9QF4UQ1xVbjCijJcUd3sRd7cWkOA5WMqlZSAhuwuB+IebSgrb4fuYJ4E7DNThwlKiI1UEmhZ8XoUMC8eteVift+xnpcRhlhCoBvDVy2beZgpPczLoaPUaC2fgFhZ5kC8F7C3YZxp4IpUpx0f3Wrvb4RxOuBtrVgFwng42YAhcSi4k6h1/yiiSwp99ksGSwhVsPHHb9+FJSxpjrpmh3BS73Hd+7J6eOvCZC1QCLDskUJIr+qH55GdFvYr0iLrUOniuWgzO5CKVeuBS/kPcqpNApgfEWQw29kXxK8TVDDcoco3jLxcxtr2I/Y5taJ6Bh19jcGBYwTEUVfDDJQo1ii/FGzmEvgpFHrJWvHaYisXpM0I9wkAzNLPh6aW5tCZZxlpwgsRQwLb+uOwfFz69hNV0Qp02rrju4km/aLN8kXnItgzWFg42gEOnWG1683GNgBnCj2WtluunWcZW3k3pKw8dgYag4+VM0lR/TsWuL2n6MkAcqpHlvknVMRo9e24Mg52x/2fhXpBSEVzqZUo59r3C67yzD/5/pJs2Os8iYoqhGTGokx/cU0xzvYJ7J7/FCwwBc313DPNIpRiVOpBoKHedVfzlGgKjAJ1NJSJiIeUUpQoSwNoDk5OTkr/////Sv////9LAHSUYk1wAoWUjAFDlHSUUpSMA3Bvc5RNcAJ1jAloYXNfZ2F1c3OUSwCMBWdhdXNzlEcAAAAAAAAAAHVidWIu",
+        ":serialized:": "gAWVWAsAAAAAAACME2d5bS5zcGFjZXMuZGlzY3JldGWUjAhEaXNjcmV0ZZSTlCmBlH2UKIwBbpRLAowGX3NoYXBllCmMBWR0eXBllIwFbnVtcHmUjAVkdHlwZZSTlIwCaTiUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYowKX25wX3JhbmRvbZSMFG51bXB5LnJhbmRvbS5fcGlja2xllIwSX19yYW5kb21zdGF0ZV9jdG9ylJOUjAdNVDE5OTM3lGgRjBRfX2JpdF9nZW5lcmF0b3JfY3RvcpSTlIaUUpR9lCiMDWJpdF9nZW5lcmF0b3KUjAdNVDE5OTM3lIwFc3RhdGWUfZQojANrZXmUjBJudW1weS5jb3JlLm51bWVyaWOUjAtfZnJvbWJ1ZmZlcpSTlCiWwAkAAAAAAAAAAACAL6geVY99W9iSOzOWX9wrwN4FaLkPb2FZlBpCIpEHdBWzqlLtIYXarg6AcO3nEotLleYiTB0R4F/9jDkfX2ordCLarhDXHVyPZn+mE2XT9I7dQtWO+NHtHSE9czp/UwGsramimSmrHXwKvNbn35mA2So0GVDh6QIxxaSoWWgVkpXJuSefhx4jr6/wmkXlWWLsKKqb+TeP3dtskyx9qGuN2SHXNSV3Yd0eZA39YdxfFSLFLf3OTIUQIiNZMrdnL1YmZZzpp5xoMJHPMMRXic78u8/K8gB3i2zdBINDg0be00Bb2tJTx7iLxY/pssSFWqGA+yHQwSrDqJ9bBQ7QAvB49qmVylLpfq3dHCqn9fsXVkRWdZq/2s1Fce4EZDYIX96om6x6QASNm+aTintwxk0UOBNSWDfIQUOLepbRR81cAdS3wVrjhSWcbUhXygNnwkd8Ujl0XZLoL2TYyVLu0knP7+kClwWRHReKkrxwIzKwH92XJ+mEUYkB1Fmx0C4LZzm41BNNTVKzrg5UiF9rxKEuNIQvbuI6MLxwtdDpplvX47Jj2n00lSX+uDj1koOAZYIEgRJyctaoMLlH63X63OF2ZFDSWlJ2T8NnfqLYZO1WDdNVNwoqdvwBhEmMCeRnxHeGq85bAzeP3dhOhfm0o2vyZ4CS+Lr/QcbXnX8LufszGA58XjHUyiBPzmQLmWEF09MrAcFO0bColnX7zuWD+eiKUi1XeABy0rn3p+hNHsiJ6EiqUKUOaKj+mCBx36L0ztUVykbSQoVgxS1Sd15b1c20s7revzy9k9NmdDkKHBOB6rp7cY0hlEgy7f1j9o2ZP9YW/cCjNpywXikl8Yhca9pADvpafknQx6xMq3mgJj4F6Eo3HNSh1MOhLik16uPfmu9k372LFmuGHuOurjd0Uxrp/G6gJlWGDWoafdW2+Qx0TTIDUyccjMJroBv/f8ZHPHFxjiWurCVFj5J848pWT5PjpcjRmobCNSZpkqy1UgQxuLoaLR025Rnd3AmolFjA8YFNP579uNh4z2doGIslWNItwbyd+zca1znow0vQlvioXYIudfRkyaOugLRoZrliHwvJKYtn3MtLqjdgnAsxumAXZG40OjzxwInDjLrubvn5fX6OWu2ukWCDP1xVUMXWENE+5ipR0485uyq6DemEXJfrgui/EWkvCpOj4Q32d9sjMlPQ03fWh6XXuCKsPRc+fWS0xu6UjELvj+1OPo6ulMfE8L/TkEhCrrkRV3rY9wdtQ+J9vROgo7ZgJ/jcYdHF3zDtLO8GzxDu/mJKJzFrJHuAVg/ypw11zJD0zF9Hec7qjzZXqI78UVTDGP9229u6wt1UtXBY+VLDu3BBkzn/VXvRkQU8qtlzezcY9zm6T/gbZCyejKPy0zxzL5xKfNAMYx2b1rlohWL1qzJ4F48WZ2dOZVHCuwBRCpSRK8uVJOvF6YZxNBtDX7tuehLWvjEUo4JHe7zZsggbJRH94CCqnG3C+7g4g4E2ZpCYWPV76xZAjKcnCzoz42ULqBWJMXk839cvdSSmg4hPxDmCqXp+zY0DcnWEdJ0yDfW9VFYHHVoBVkOV6imG8peL741LL63FfkcxmMXQNe7XNg5STfHxtGkOPOOQf6eC0IUOrM4ieoP8WiCn5IzUSHbAypEU4hFiydWvVzW4fq3nKhaYWab/a/WMgDk1SgiDa52e0JuUkmwI4SKiXMuGZVXl2x4g+72qp4Mdt9WyCRU/77mqYyo3+4oVSeMb4+SfsGJxAMxncw2MFPMiTcCz+uV2Bl7BW2Xy7JFNSY1LGtDhmWHGbcWP9ndWPuHr+0Bq9IkgPbqCRgXVhoOWvzOwQEIDx2NUnmyHh7Tb71P9w9RlmUNlVp2DirBnrhLFdjGYMso3jUpEm7VGpL3DFHBOKLo4s1SbtCy8owMlIgNO7eBe+8B4BrZEMTnlVA/5nJ/Ti7bQ8xk47pH5glxBzsuXRHGNW8TK9A+t6ZW93yeXltprdoxZYLzRkbD/ElXKqhOE+3kjKEceqHQQ7DjgbStKVMbAfkQLiMdJ+GlROeKbrYMhJHEUatKWxFQakqEz8yJb/HAi7tNQ+4j02hjx2aVPJ14sU3Y7qhRt4kOXebrsDM0mqK+UKYf89OoVTIBC7JeXTb+aqCO6HOKSQgou6dQuukAKV0MQEDOZ3XvGS3rNPkRVHulujfcD7dbk7Gt3RGoEKmjhTZPLtfXwvB1nhzJCJQVbjgWxPmmqoVrd4uxcBlVb1fQdvsfGyRGPRUSd2xD2K7PVARJTrzfit84d9RtBc4kJnfijlpD9mUcwmsPTmyG77SOgSQcA8lrESZyuinZ0DnC56hpmxFLU/1TSEI1vos555qOZEUzxH0bhaEM1w/iId5sRylLfZ9DVGgWjrYyn0yfzLx70MfDW4x0lk7SNsc1CiDtyWyPeUqD9HH10N/ZGoJi/42sZq8/MzrYvHoVazAiyHTojvnXVBU1vs3ygRHu182d4w80WXrdqo5Yi4ODRxqB8mnDaUtdV1qZyBYqqvtbE07C7ZocgWRuNz6ESpkkI/hcrlXyTKc2AVnHKWzcpbOaO9p/NneqvV93r4QqwPNovVuLpdlQslGyICbCatx2J+U+qfqB8cVp0X3/6rg2B9O5A7DFK4g1G4i6/5QWePtZT0PCEbsaDW3MNr3fWTxLyqzR6rQoHiwqNUcGDCm+c+/2VW3GhdtnH8oSbDujP62Q32625xxgHBop1hXplNxBBxK8zmMsFRqH5DWv+/7c9jFRCSt+iCEf2ARyHGPcrvlLzvd1QedEJOhwJedtienWnz8dQRJ1lyO0TpJocJKMfvM5QF7jwgvnm36+UljA61a4KquwILSwKQoC7U4tcN7kclK8rDDXlPlqUGOGt08aAD3igbOKq7wR+O7fh7oN0uMv69b/SvrdNEM7cAoqDE7yGfX9MQ/J+xhyeIWPYkc+FhQAs+yLDEUh5NBvvvGx/Jv1OkE+rXdvMucLUNJXw8RFscbPZHe7Ziw66lR3XXr7iSGeVHcHwaet9o0ttUL05fASEplE3qQd1n3U7xjhfECrbjr0mtFNIYEN2/F+aXxl++tCooem6+g0U9KATkdyhLjmimwfsoeGV+O5MVqGC5kp66dRNLyZsyBpLUOwl5BZMBP8Y05ABxqbDcsX7bphBJ5E5l0K1cyWaBZcDBJOSJsSIs8du1tIHu6Te5bOwkRlFKSBBfTO+vagiLqiHYet2DqIaRmsotliTYwLHqK9kdOZ8YyTvfyLaKQEpr8Ojlq8vVBA8+cy2I4oBK+YrgENE00SmEcYqMf0ntolbTmDUYaFv91TVUxGUaAqMAnU0lImIh5RSlChLA2gOTk5OSv////9K/////0sAdJRiTXAChZSMAUOUdJRSlIwDcG9zlE1wAnWMCWhhc19nYXVzc5RLAIwFZ2F1c3OURwAAAAAAAAAAdWJ1Yi4=",
         ":type:": "<class 'gym.spaces.discrete.Discrete'>",
         "_np_random": "RandomState(MT19937)",
         "_shape": [],
         "dtype": "int64",
         "n": 2
     },
     "batch_size": 64,
     "clip_range": {
-        ":serialized:": "gAWVkwIAAAAAAACMF2Nsb3VkcGlja2xlLmNsb3VkcGlja2xllIwNX2J1aWx0aW5fdHlwZZSTlIwKTGFtYmRhVHlwZZSFlFKUKGgCjAhDb2RlVHlwZZSFlFKUKEsBSwBLAEsBSwFLE0MEiABTAJROhZQpjAFflIWUjGMvaG9tZS9tL0RvY3VtZW50cy9DSEFJL2ltaXRhdGlvbi92ZW52L2xpYi9weXRob24zLjgvc2l0ZS1wYWNrYWdlcy9zdGFibGVfYmFzZWxpbmVzMy9jb21tb24vdXRpbHMucHmUjARmdW5jlEuAQwIAAZSMA3ZhbJSFlCl0lFKUfZQojAtfX3BhY2thZ2VfX5SMGHN0YWJsZV9iYXNlbGluZXMzLmNvbW1vbpSMCF9fbmFtZV9flIwec3RhYmxlX2Jhc2VsaW5lczMuY29tbW9uLnV0aWxzlIwIX19maWxlX1+UaA11Tk5oAIwQX21ha2VfZW1wdHlfY2VsbJSTlClSlIWUdJRSlIwcY2xvdWRwaWNrbGUuY2xvdWRwaWNrbGVfZmFzdJSMEl9mdW5jdGlvbl9zZXRzdGF0ZZSTlGgffZR9lChoF2gOjAxfX3F1YWxuYW1lX1+UjBljb25zdGFudF9mbi48bG9jYWxzPi5mdW5jlIwPX19hbm5vdGF0aW9uc19flH2UjA5fX2t3ZGVmYXVsdHNfX5ROjAxfX2RlZmF1bHRzX1+UTowKX19tb2R1bGVfX5RoGIwHX19kb2NfX5ROjAtfX2Nsb3N1cmVfX5RoAIwKX21ha2VfY2VsbJSTlEc/yZmZmZmZmoWUUpSFlIwXX2Nsb3VkcGlja2xlX3N1Ym1vZHVsZXOUXZSMC19fZ2xvYmFsc19flH2UdYaUhlIwLg==",
+        ":serialized:": "gAWVlQIAAAAAAACMF2Nsb3VkcGlja2xlLmNsb3VkcGlja2xllIwOX21ha2VfZnVuY3Rpb26Uk5QoaACMDV9idWlsdGluX3R5cGWUk5SMCENvZGVUeXBllIWUUpQoSwFLAEsASwFLAUsTQwSIAFMAlE6FlCmMAV+UhZSMYy9ob21lL20vRG9jdW1lbnRzL0NIQUkvaW1pdGF0aW9uL3ZlbnYvbGliL3B5dGhvbjMuOC9zaXRlLXBhY2thZ2VzL3N0YWJsZV9iYXNlbGluZXMzL2NvbW1vbi91dGlscy5weZSMBGZ1bmOUS4JDAgABlIwDdmFslIWUKXSUUpR9lCiMC19fcGFja2FnZV9flIwYc3RhYmxlX2Jhc2VsaW5lczMuY29tbW9ulIwIX19uYW1lX1+UjB5zdGFibGVfYmFzZWxpbmVzMy5jb21tb24udXRpbHOUjAhfX2ZpbGVfX5RoDHVOTmgAjBBfbWFrZV9lbXB0eV9jZWxslJOUKVKUhZR0lFKUjBxjbG91ZHBpY2tsZS5jbG91ZHBpY2tsZV9mYXN0lIwSX2Z1bmN0aW9uX3NldHN0YXRllJOUaB59lH2UKGgWaA2MDF9fcXVhbG5hbWVfX5SMGWNvbnN0YW50X2ZuLjxsb2NhbHM+LmZ1bmOUjA9fX2Fubm90YXRpb25zX1+UfZSMDl9fa3dkZWZhdWx0c19flE6MDF9fZGVmYXVsdHNfX5ROjApfX21vZHVsZV9flGgXjAdfX2RvY19flE6MC19fY2xvc3VyZV9flGgAjApfbWFrZV9jZWxslJOURz/JmZmZmZmahZRSlIWUjBdfY2xvdWRwaWNrbGVfc3VibW9kdWxlc5RdlIwLX19nbG9iYWxzX1+UfZR1hpSGUjAu",
         ":type:": "<class 'function'>"
     },
     "clip_range_vf": null,
     "ent_coef": 0.0,
     "ep_info_buffer": {
-        ":serialized:": "gAWVRAwAAAAAAACMC2NvbGxlY3Rpb25zlIwFZGVxdWWUk5QpS2SGlFKUKH2UKIwBcpRHQH9AAAAAAACMAWyUTfQBjAF0lEdATYklVtGd7XV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQE12fT1CgK51fZQoaAZHQH9AAAAAAABoB030AWgIR0BNqcwQDmr9dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdATpS/bj94vHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQE6vU83dbgV1fZQoaAZHQH9AAAAAAABoB030AWgIR0BO2Zy2hIvrdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAT5NwJgLJCHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQE+vGDL8rI51fZQoaAZHQH9AAAAAAABoB030AWgIR0BP3r/sE7nxdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAT8oHxBmf5HV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQE/+W2w3YL91fZQoaAZHQH9AAAAAAABoB030AWgIR0BQdD4YaYNRdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAUIGs+3YthHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFCYy1/lQuV1fZQoaAZHQH9AAAAAAABoB030AWgIR0BQkacmShaldX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAUQOaiKziTHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFEbx9XtBv91fZQoaAZHQH9AAAAAAABoB030AWgIR0BREPjCHh0hdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAUSm+XZ5AyHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFGeGH58BuJ1fZQoaAZHQH9AAAAAAABoB030AWgIR0BRq2V3Ux20dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAUcB2wFC9iHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFG5k+5e7cx1fZQoaAZHQH9AAAAAAABoB030AWgIR0BSK4YrJ8v3dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAUkLJPqLS/nV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFI4Pwd8zAN1fZQoaAZHQH9AAAAAAABoB030AWgIR0BSUdXT3IuHdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAUsQqNIbwSnV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFLRb9If8uV1fZQoaAZHQH9AAAAAAABoB030AWgIR0BS5cQ2/BWQdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAUt7aBZpztHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFLtSDRMN+d1fZQoaAZHQH9AAAAAAABoB030AWgIR0BTZzXvphWpdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAU1xhXr+o+HV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFN0tXgccVB1fZQoaAZHQH9AAAAAAABoB030AWgIR0BT6tLYf4h2dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAU/gfeUILPXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFQQnSv1UVB1fZQoaAZHQH9AAAAAAABoB030AWgIR0BUCrteD3/QdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVBlUaQ3gk3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFSOIjGDL8t1fZQoaAZHQH9AAAAAAABoB030AWgIR0BUgs6BAfMfdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVJmbwz+FUXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFUXDhcZ9/l1fZQoaAZHQH9AAAAAAABoB030AWgIR0BVJEyP+4smdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVTlW4mTkhnV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFUyqJ/G2kV1fZQoaAZHQH9AAAAAAABoB030AWgIR0BVQRs/IKc/dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVbYmb9ZRsXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFWtC0WuX/p1fZQoaAZHQH9AAAAAAABoB030AWgIR0BVxwvHtF8YdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVkX+NtIkJXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFZTQnx8UmF1fZQoaAZHQH9AAAAAAABoB030AWgIR0BWaAiA2AG0dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVmEo/iYLLXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFZvRArxy4p1fZQoaAZHQH9AAAAAAABoB030AWgIR0BW4C7btZ3cdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVtX5CWu5jHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFbu9jgAIY51fZQoaAZHQH9AAAAAAABoB030AWgIR0BXZFr6+FlDdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAV3GYMOPNmnV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFeI4MWoFV11fZQoaAZHQH9AAAAAAABoB030AWgIR0BXg52yLQ5WdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAV5IjY7JXAHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFeqWhRIjGF1fZQoaAZHQH9AAAAAAABoB030AWgIR0BYDZ0CA+Y/dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWCc1JlJ6IHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFirP4EfT1F1fZQoaAZHQH9AAAAAAABoB030AWgIR0BYuLdepn6EdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWM0xqO938nV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFjHiBXjlxR1fZQoaAZHQH9AAAAAAABoB030AWgIR0BY1oUSIxgzdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWO4Difg75nV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFlRFocrAgx1fZQoaAZHQH9AAAAAAABoB030AWgIR0BZa1vIfbKzdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWY1XNke6qnV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFn5QVsUIs11fZQoaAZHQHqAAAAAAABoB02oAWgIR0BZ/ZAhStNjdX2UKGgGR0B4IAAAAAAAaAdNggFoCEdAWftqi48U23V9lChoBkdAfQAAAAAAAGgHTdABaAhHQFn9AgxJul51fZQoaAZHQHxQAAAAAABoB03FAWgIR0BaHq8Yht+DdX2UKGgGR0B8wAAAAAAAaAdNzAFoCEdAWhQd2gWadHV9lChoBkdAfMAAAAAAAGgHTcwBaAhHQFqAWp6yB091fZQoaAZHQHpwAAAAAABoB02nAWgIR0BapEygwoLHdX2UKGgGR0B7YAAAAAAAaAdNtgFoCEdAWqu4RVZLZnV9lChoBkdAfQAAAAAAAGgHTdABaAhHQFqfW56MR6F1fZQoaAZHQHqAAAAAAABoB02oAWgIR0Bap9EG7jDLdX2UKGgGR0B88AAAAAAAaAdNzwFoCEdAWwieTV2A5XV9lChoBkdAe9AAAAAAAGgHTb0BaAhHQFsnam4y44J1fZQoaAZHQHkgAAAAAABoB02SAWgIR0BbFa//NqxkdX2UKGgGR0B9IAAAAAAAaAdN0gFoCEdAW5Rf6XSjQHV9lChoBkdAd9AAAAAAAGgHTX0BaAhHQFumW1c+qzZ1fZQoaAZHQHjAAAAAAABoB02MAWgIR0BbrjFId2gWdX2UKGgGR0B8wAAAAAAAaAdNzAFoCEdAW8B2cJ+lTHV9lChoBkdAfHAAAAAAAGgHTccBaAhHQFuzXUYsNDt1fZQoaAZHQHugAAAAAABoB026AWgIR0Bbw3EAHVwxdX2UKGgGR0B5sAAAAAAAaAdNmwFoCEdAXDKsEJSiunV9lChoBkdAeSAAAAAAAGgHTZIBaAhHQFweKKYRdyF1fZQoaAZHQHngAAAAAABoB02eAWgIR0BcRxeXzDoAdX2UKGgGR0B8wAAAAAAAaAdNzAFoCEdAXGLXrdFfA3VlLg==",
+        ":serialized:": "gAWVRAwAAAAAAACMC2NvbGxlY3Rpb25zlIwFZGVxdWWUk5QpS2SGlFKUKH2UKIwBcpRHQH9AAAAAAACMAWyUTfQBjAF0lEdAU1gbkwN9Y3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFNUsTWXkYJ1fZQoaAZHQH9AAAAAAABoB030AWgIR0BTxclkYoAodX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAU+EE8q4H5nV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFPPqZ+hGpd1fZQoaAZHQH9AAAAAAABoB030AWgIR0BTycoMKCxvdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVAmgte2NN3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFTM/DtPYWd1fZQoaAZHQH9AAAAAAABoB030AWgIR0BVPqyKNyYHdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVUDTfBN21XV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFWfSLZSNwR1fZQoaAZHQH9AAAAAAABoB030AWgIR0BVuofCAMDwdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVanPE87p3XV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFWjiDdxhlV1fZQoaAZHQH9AAAAAAABoB030AWgIR0BV4gbuMMqjdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVfKNLlFMI3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFYwahHskY51fZQoaAZHQH9AAAAAAABoB030AWgIR0BWLOwkgOjJdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVnlBPbfxc3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFaUsGxD9fl1fZQoaAZHQH9AAAAAAABoB030AWgIR0BWg+M6zVtodX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVn2tSydFv3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFa8M3IdU851fZQoaAZHQH9AAAAAAABoB030AWgIR0BWyrjDKoycdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAVwhGkN4JNXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFcEy8SPEKp1fZQoaAZHQH9AAAAAAABoB030AWgIR0BXT/CqIacadX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAV2sn0Cih4HV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFdZoCdSVGF1fZQoaAZHQH9AAAAAAABoB030AWgIR0BXU1Y2bXpXdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAV5LVhCtzS3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFeg2F36hxp1fZQoaAZHQH9AAAAAAABoB030AWgIR0BX3hJd0JWvdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAV9svWYnfEXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFgmsBQvYe11fZQoaAZHQH9AAAAAAABoB030AWgIR0BYQelbeMyadX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWDDF6zE74nV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFgqzcAR02d1fZQoaAZHQH9AAAAAAABoB030AWgIR0BYaV9Brvb5dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWDNy2hIvrXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFi8/pt78el1fZQoaAZHQH9AAAAAAABoB030AWgIR0BYuW4uscQzdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWQnW6K+BYnV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFklDZ13dKx1fZQoaAZHQH9AAAAAAABoB030AWgIR0BZE3t4RmK7dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWQ1dAxBVuXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFlMH2ys0YV1fZQoaAZHQH9AAAAAAABoB030AWgIR0BZFQLux8lYdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWZf101ZTynV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFmUY287IT51fZQoaAZHQH9AAAAAAABoB030AWgIR0BZ5GjO9nK5dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWf+vC/GlynV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFnuGVRk3CN1fZQoaAZHQH9AAAAAAABoB030AWgIR0BZ5+1jRUm2dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWia6FuejEnV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFnwJl8PWhB1fZQoaAZHQH9AAAAAAABoB030AWgIR0Bacuj7ALy+dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWm/ynUDuB3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFq9BZIQOFx1fZQoaAZHQH9AAAAAAABoB030AWgIR0Ba2HbmEGqxdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWsfCO3lS0nV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFrCD7655JN1fZQoaAZHQH9AAAAAAABoB030AWgIR0BbAHn2ZiNLdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAWsldxAB1cXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFtPKtga3ql1fZQoaAZHQH9AAAAAAABoB030AWgIR0BbTBRIjGDMdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAW5qtyPuG9HV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFu19AHE/B51fZQoaAZHQH9AAAAAAABoB030AWgIR0BbpptNzr/sdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAW6EJqqOtGXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFvgJ7sv7Fd1fZQoaAZHQH9AAAAAAABoB030AWgIR0Bbqog3cYZVdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAXIwgkka/AXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQFyM2uPmxMZ1fZQoaAZHQH9AAAAAAABoB030AWgIR0Bddmpda+vhdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAXZH7bcoH9nV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF2CM6BAfMh1fZQoaAZHQH9AAAAAAABoB030AWgIR0BdfGEwnH/+dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAXbr0se4kNXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF2DaxX4j8l1fZQoaAZHQH9AAAAAAABoB030AWgIR0BeC07r9l3AdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAXgfILgGbC3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF4MWiUPhAJ1fZQoaAZHQH9AAAAAAABoB030AWgIR0BeJ5flZHNHdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAXlzU1AJLNHV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF5W0qH446x1fZQoaAZHQH9AAAAAAABoB030AWgIR0BelZQ+EAYIdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAXl8pnYg7o3V9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF7yBSk0rLB1fZQoaAZHQH9AAAAAAABoB030AWgIR0Be7obCJoCddX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAXvXJdSl3yXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF8RBMSK3ux1fZQoaAZHQH9AAAAAAABoB030AWgIR0BfS8Q7LdN4dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAX0XlLeyiVXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF+EWrOqvNh1fZQoaAZHQH9AAAAAAABoB030AWgIR0BfTqL0jC53dX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAX+HNke6qbXV9lChoBkdAf0AAAAAAAGgHTfQBaAhHQF/gqt5le4V1fZQoaAZHQH9AAAAAAABoB030AWgIR0BgCbS1E3KkdX2UKGgGR0B/QAAAAAAAaAdN9AFoCEdAYBfpgTh5xHVlLg==",
         ":type:": "<class 'collections.deque'>"
     },
     "ep_success_buffer": {
         ":serialized:": "gAWVIAAAAAAAAACMC2NvbGxlY3Rpb25zlIwFZGVxdWWUk5QpS2SGlFKULg==",
         ":type:": "<class 'collections.deque'>"
     },
     "gae_lambda": 0.95,
     "gamma": 0.99,
     "learning_rate": 0.0003,
     "lr_schedule": {
-        ":serialized:": "gAWVkwIAAAAAAACMF2Nsb3VkcGlja2xlLmNsb3VkcGlja2xllIwNX2J1aWx0aW5fdHlwZZSTlIwKTGFtYmRhVHlwZZSFlFKUKGgCjAhDb2RlVHlwZZSFlFKUKEsBSwBLAEsBSwFLE0MEiABTAJROhZQpjAFflIWUjGMvaG9tZS9tL0RvY3VtZW50cy9DSEFJL2ltaXRhdGlvbi92ZW52L2xpYi9weXRob24zLjgvc2l0ZS1wYWNrYWdlcy9zdGFibGVfYmFzZWxpbmVzMy9jb21tb24vdXRpbHMucHmUjARmdW5jlEuAQwIAAZSMA3ZhbJSFlCl0lFKUfZQojAtfX3BhY2thZ2VfX5SMGHN0YWJsZV9iYXNlbGluZXMzLmNvbW1vbpSMCF9fbmFtZV9flIwec3RhYmxlX2Jhc2VsaW5lczMuY29tbW9uLnV0aWxzlIwIX19maWxlX1+UaA11Tk5oAIwQX21ha2VfZW1wdHlfY2VsbJSTlClSlIWUdJRSlIwcY2xvdWRwaWNrbGUuY2xvdWRwaWNrbGVfZmFzdJSMEl9mdW5jdGlvbl9zZXRzdGF0ZZSTlGgffZR9lChoF2gOjAxfX3F1YWxuYW1lX1+UjBljb25zdGFudF9mbi48bG9jYWxzPi5mdW5jlIwPX19hbm5vdGF0aW9uc19flH2UjA5fX2t3ZGVmYXVsdHNfX5ROjAxfX2RlZmF1bHRzX1+UTowKX19tb2R1bGVfX5RoGIwHX19kb2NfX5ROjAtfX2Nsb3N1cmVfX5RoAIwKX21ha2VfY2VsbJSTlEc/M6kqMFUyYYWUUpSFlIwXX2Nsb3VkcGlja2xlX3N1Ym1vZHVsZXOUXZSMC19fZ2xvYmFsc19flH2UdYaUhlIwLg==",
+        ":serialized:": "gAWVlQIAAAAAAACMF2Nsb3VkcGlja2xlLmNsb3VkcGlja2xllIwOX21ha2VfZnVuY3Rpb26Uk5QoaACMDV9idWlsdGluX3R5cGWUk5SMCENvZGVUeXBllIWUUpQoSwFLAEsASwFLAUsTQwSIAFMAlE6FlCmMAV+UhZSMYy9ob21lL20vRG9jdW1lbnRzL0NIQUkvaW1pdGF0aW9uL3ZlbnYvbGliL3B5dGhvbjMuOC9zaXRlLXBhY2thZ2VzL3N0YWJsZV9iYXNlbGluZXMzL2NvbW1vbi91dGlscy5weZSMBGZ1bmOUS4JDAgABlIwDdmFslIWUKXSUUpR9lCiMC19fcGFja2FnZV9flIwYc3RhYmxlX2Jhc2VsaW5lczMuY29tbW9ulIwIX19uYW1lX1+UjB5zdGFibGVfYmFzZWxpbmVzMy5jb21tb24udXRpbHOUjAhfX2ZpbGVfX5RoDHVOTmgAjBBfbWFrZV9lbXB0eV9jZWxslJOUKVKUhZR0lFKUjBxjbG91ZHBpY2tsZS5jbG91ZHBpY2tsZV9mYXN0lIwSX2Z1bmN0aW9uX3NldHN0YXRllJOUaB59lH2UKGgWaA2MDF9fcXVhbG5hbWVfX5SMGWNvbnN0YW50X2ZuLjxsb2NhbHM+LmZ1bmOUjA9fX2Fubm90YXRpb25zX1+UfZSMDl9fa3dkZWZhdWx0c19flE6MDF9fZGVmYXVsdHNfX5ROjApfX21vZHVsZV9flGgXjAdfX2RvY19flE6MC19fY2xvc3VyZV9flGgAjApfbWFrZV9jZWxslJOURz8zqSowVTJhhZRSlIWUjBdfY2xvdWRwaWNrbGVfc3VibW9kdWxlc5RdlIwLX19nbG9iYWxzX1+UfZR1hpSGUjAu",
         ":type:": "<class 'function'>"
     },
     "max_grad_norm": 0.5,
     "n_envs": 8,
     "n_epochs": 10,
     "n_steps": 256,
     "normalize_advantage": true,
@@ -66,27 +67,22 @@
         "high": "[4.8000002e+00 3.4028235e+38 4.1887903e-01 3.4028235e+38]",
         "low": "[-4.8000002e+00 -3.4028235e+38 -4.1887903e-01 -3.4028235e+38]"
     },
     "policy_class": {
         ":serialized:": "gAWVMwAAAAAAAACMF2ltaXRhdGlvbi5wb2xpY2llcy5iYXNllIwTRmVlZEZvcndhcmQzMlBvbGljeZSTlC4=",
         ":type:": "<class 'abc.ABCMeta'>",
         "__abstractmethods__": "frozenset()",
-        "__doc__": "A feed forward policy network with two hidden layers of 32 units.\n\n    This matches the IRL policies in the original AIRL paper.\n\n    Note: This differs from stable_baselines3 ActorCriticPolicy in two ways: by\n    having 32 rather than 64 units, and by having policy and value networks\n    share weights except at the final layer.\n    ",
-        "__init__": "<function FeedForward32Policy.__init__ at 0x7f9b68959280>",
+        "__doc__": "A feed forward policy network with two hidden layers of 32 units.\n\n    This matches the IRL policies in the original AIRL paper.\n\n    Note: This differs from stable_baselines3 ActorCriticPolicy in two ways: by\n    having 32 rather than 64 units, and by having policy and value networks\n    share weights except at the final layer, where there are different linear heads.\n    ",
+        "__init__": "<function FeedForward32Policy.__init__ at 0x7f8560c56a60>",
         "__module__": "imitation.policies.base",
-        "_abc_impl": "<_abc_data object at 0x7f9b68950a80>"
-    },
-    "policy_kwargs": {
-        ":serialized:": "gAWV8QAAAAAAAACMH3NhY3JlZC5jb25maWcuY3VzdG9tX2NvbnRhaW5lcnOUjAxSZWFkT25seURpY3SUk5R9lCiMGGZlYXR1cmVzX2V4dHJhY3Rvcl9jbGFzc5SMF2ltaXRhdGlvbi5wb2xpY2llcy5iYXNllIwaTm9ybWFsaXplRmVhdHVyZXNFeHRyYWN0b3KUk5SMGWZlYXR1cmVzX2V4dHJhY3Rvcl9rd2FyZ3OUaAJ9lIwPbm9ybWFsaXplX2NsYXNzlIwXaW1pdGF0aW9uLnV0aWwubmV0d29ya3OUjAtSdW5uaW5nTm9ybZSTlHOFlFKUdYWUUpQu",
-        ":type:": "<class 'sacred.config.custom_containers.ReadOnlyDict'>",
-        "features_extractor_class": "<class 'imitation.policies.base.NormalizeFeaturesExtractor'>",
-        "features_extractor_kwargs": "{'normalize_class': <class 'imitation.util.networks.RunningNorm'>}"
+        "_abc_impl": "<_abc_data object at 0x7f8560c514e0>"
     },
+    "policy_kwargs": {},
     "sde_sample_freq": -1,
-    "seed": 703960862,
-    "start_time": 1650624603.5629442,
+    "seed": 929991016,
+    "start_time": 1683107121387198012,
     "target_kl": null,
     "tensorboard_log": null,
     "use_sde": false,
     "verbose": 0,
     "vf_coef": 0.5
 }
```

#### policy.pth

##### zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 8964 bytes, number of entries: 13
--rw----     0.0 fat     1588 bl stor 80-000-00 00:00 archive/data.pkl
--rw----     0.0 fat       16 bl stor 80-000-00 00:00 archive/data/0
--rw----     0.0 fat       16 bl stor 80-000-00 00:00 archive/data/1
--rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/10
--rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/2
--rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/3
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/4
--rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/5
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/6
--rw----     0.0 fat      256 bl stor 80-000-00 00:00 archive/data/7
--rw----     0.0 fat        8 bl stor 80-000-00 00:00 archive/data/8
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/9
+Zip file size: 14145 bytes, number of entries: 14
+-rw----     0.0 fat     1891 bl stor 80-000-00 00:00 archive/data.pkl
+-rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/0
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/1
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/10
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/11
+-rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/2
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/3
+-rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/4
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/5
+-rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/6
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/7
+-rw----     0.0 fat      256 bl stor 80-000-00 00:00 archive/data/8
+-rw----     0.0 fat        8 bl stor 80-000-00 00:00 archive/data/9
 -rw----     0.0 fat        2 bl stor 80-000-00 00:00 archive/version
-13 files, 6886 bytes uncompressed, 6886 bytes compressed:  0.0%
+14 files, 12017 bytes uncompressed, 12017 bytes compressed:  0.0%
```

##### zipnote «TEMP»/diffoscope_3cnx63wy_/tmp2dorepu8_.zip

```diff
@@ -6,14 +6,17 @@
 
 Filename: archive/data/1
 Comment: 
 
 Filename: archive/data/10
 Comment: 
 
+Filename: archive/data/11
+Comment: 
+
 Filename: archive/data/2
 Comment: 
 
 Filename: archive/data/3
 Comment: 
 
 Filename: archive/data/4
```

##### archive/data.pkl

```diff
@@ -1,100 +1,119 @@
 00000000: 8002 6363 6f6c 6c65 6374 696f 6e73 0a4f  ..ccollections.O
 00000010: 7264 6572 6564 4469 6374 0a71 0029 5271  rderedDict.q.)Rq
-00000020: 0128 5829 0000 0066 6561 7475 7265 735f  .(X)...features_
-00000030: 6578 7472 6163 746f 722e 6e6f 726d 616c  extractor.normal
-00000040: 697a 652e 7275 6e6e 696e 675f 6d65 616e  ize.running_mean
-00000050: 7102 6374 6f72 6368 2e5f 7574 696c 730a  q.ctorch._utils.
-00000060: 5f72 6562 7569 6c64 5f74 656e 736f 725f  _rebuild_tensor_
-00000070: 7632 0a71 0328 2858 0700 0000 7374 6f72  v2.q.((X....stor
-00000080: 6167 6571 0463 746f 7263 680a 466c 6f61  ageq.ctorch.Floa
-00000090: 7453 746f 7261 6765 0a71 0558 0100 0000  tStorage.q.X....
-000000a0: 3071 0658 0300 0000 6370 7571 074b 0474  0q.X....cpuq.K.t
-000000b0: 7108 514b 004b 0485 7109 4b01 8571 0a89  q.QK.K..q.K..q..
-000000c0: 6800 2952 710b 7471 0c52 710d 5828 0000  h.)Rq.tq.Rq.X(..
-000000d0: 0066 6561 7475 7265 735f 6578 7472 6163  .features_extrac
-000000e0: 746f 722e 6e6f 726d 616c 697a 652e 7275  tor.normalize.ru
-000000f0: 6e6e 696e 675f 7661 7271 0e68 0328 2868  nning_varq.h.((h
-00000100: 0468 0558 0100 0000 3171 0f68 074b 0474  .h.X....1q.h.K.t
-00000110: 7110 514b 004b 0485 7111 4b01 8571 1289  q.QK.K..q.K..q..
-00000120: 6800 2952 7113 7471 1452 7115 5822 0000  h.)Rq.tq.Rq.X"..
-00000130: 0066 6561 7475 7265 735f 6578 7472 6163  .features_extrac
-00000140: 746f 722e 6e6f 726d 616c 697a 652e 636f  tor.normalize.co
-00000150: 756e 7471 1668 0328 2868 0463 746f 7263  untq.h.((h.ctorc
-00000160: 680a 496e 7453 746f 7261 6765 0a71 1758  h.IntStorage.q.X
-00000170: 0100 0000 3271 1868 074b 0174 7119 514b  ....2q.h.K.tq.QK
-00000180: 0029 2989 6800 2952 711a 7471 1b52 711c  .)).h.)Rq.tq.Rq.
-00000190: 5821 0000 006d 6c70 5f65 7874 7261 6374  X!...mlp_extract
-000001a0: 6f72 2e73 6861 7265 645f 6e65 742e 302e  or.shared_net.0.
-000001b0: 7765 6967 6874 711d 6803 2828 6804 6805  weightq.h.((h.h.
-000001c0: 5801 0000 0033 711e 6807 4b80 7471 1f51  X....3q.h.K.tq.Q
-000001d0: 4b00 4b20 4b04 8671 204b 044b 0186 7121  K.K K..q K.K..q!
-000001e0: 8968 0029 5271 2274 7123 5271 2458 1f00  .h.)Rq"tq#Rq$X..
-000001f0: 0000 6d6c 705f 6578 7472 6163 746f 722e  ..mlp_extractor.
-00000200: 7368 6172 6564 5f6e 6574 2e30 2e62 6961  shared_net.0.bia
-00000210: 7371 2568 0328 2868 0468 0558 0100 0000  sq%h.((h.h.X....
-00000220: 3471 2668 074b 2074 7127 514b 004b 2085  4q&h.K tq'QK.K .
-00000230: 7128 4b01 8571 2989 6800 2952 712a 7471  q(K..q).h.)Rq*tq
-00000240: 2b52 712c 5821 0000 006d 6c70 5f65 7874  +Rq,X!...mlp_ext
-00000250: 7261 6374 6f72 2e73 6861 7265 645f 6e65  ractor.shared_ne
-00000260: 742e 322e 7765 6967 6874 712d 6803 2828  t.2.weightq-h.((
-00000270: 6804 6805 5801 0000 0035 712e 6807 4d00  h.h.X....5q.h.M.
-00000280: 0474 712f 514b 004b 204b 2086 7130 4b20  .tq/QK.K K .q0K 
-00000290: 4b01 8671 3189 6800 2952 7132 7471 3352  K..q1.h.)Rq2tq3R
-000002a0: 7134 581f 0000 006d 6c70 5f65 7874 7261  q4X....mlp_extra
-000002b0: 6374 6f72 2e73 6861 7265 645f 6e65 742e  ctor.shared_net.
-000002c0: 322e 6269 6173 7135 6803 2828 6804 6805  2.biasq5h.((h.h.
-000002d0: 5801 0000 0036 7136 6807 4b20 7471 3751  X....6q6h.K tq7Q
-000002e0: 4b00 4b20 8571 384b 0185 7139 8968 0029  K.K .q8K..q9.h.)
-000002f0: 5271 3a74 713b 5271 3c58 1100 0000 6163  Rq:tq;Rq<X....ac
-00000300: 7469 6f6e 5f6e 6574 2e77 6569 6768 7471  tion_net.weightq
-00000310: 3d68 0328 2868 0468 0558 0100 0000 3771  =h.((h.h.X....7q
-00000320: 3e68 074b 4074 713f 514b 004b 024b 2086  >h.K@tq?QK.K.K .
-00000330: 7140 4b20 4b01 8671 4189 6800 2952 7142  q@K K..qA.h.)RqB
-00000340: 7471 4352 7144 580f 0000 0061 6374 696f  tqCRqDX....actio
-00000350: 6e5f 6e65 742e 6269 6173 7145 6803 2828  n_net.biasqEh.((
-00000360: 6804 6805 5801 0000 0038 7146 6807 4b02  h.h.X....8qFh.K.
-00000370: 7471 4751 4b00 4b02 8571 484b 0185 7149  tqGQK.K..qHK..qI
-00000380: 8968 0029 5271 4a74 714b 5271 4c58 1000  .h.)RqJtqKRqLX..
-00000390: 0000 7661 6c75 655f 6e65 742e 7765 6967  ..value_net.weig
-000003a0: 6874 714d 6803 2828 6804 6805 5801 0000  htqMh.((h.h.X...
-000003b0: 0039 714e 6807 4b20 7471 4f51 4b00 4b01  .9qNh.K tqOQK.K.
-000003c0: 4b20 8671 504b 204b 0186 7151 8968 0029  K .qPK K..qQ.h.)
-000003d0: 5271 5274 7153 5271 5458 0e00 0000 7661  RqRtqSRqTX....va
-000003e0: 6c75 655f 6e65 742e 6269 6173 7155 6803  lue_net.biasqUh.
-000003f0: 2828 6804 6805 5802 0000 0031 3071 5668  ((h.h.X....10qVh
-00000400: 074b 0174 7157 514b 004b 0185 7158 4b01  .K.tqWQK.K..qXK.
-00000410: 8571 5989 6800 2952 715a 7471 5b52 715c  .qY.h.)RqZtq[Rq\
-00000420: 757d 715d 5809 0000 005f 6d65 7461 6461  u}q]X...._metada
-00000430: 7461 715e 6800 2952 715f 2858 0000 0000  taq^h.)Rq_(X....
-00000440: 7160 7d71 6158 0700 0000 7665 7273 696f  q`}qaX....versio
-00000450: 6e71 624b 0173 5812 0000 0066 6561 7475  nqbK.sX....featu
-00000460: 7265 735f 6578 7472 6163 746f 7271 637d  res_extractorqc}
-00000470: 7164 6862 4b01 7358 1a00 0000 6665 6174  qdhbK.sX....feat
-00000480: 7572 6573 5f65 7874 7261 6374 6f72 2e66  ures_extractor.f
-00000490: 6c61 7474 656e 7165 7d71 6668 624b 0173  lattenqe}qfhbK.s
-000004a0: 581c 0000 0066 6561 7475 7265 735f 6578  X....features_ex
-000004b0: 7472 6163 746f 722e 6e6f 726d 616c 697a  tractor.normaliz
-000004c0: 6571 677d 7168 6862 4b01 7358 0d00 0000  eqg}qhhbK.sX....
-000004d0: 6d6c 705f 6578 7472 6163 746f 7271 697d  mlp_extractorqi}
-000004e0: 716a 6862 4b01 7358 1800 0000 6d6c 705f  qjhbK.sX....mlp_
-000004f0: 6578 7472 6163 746f 722e 7368 6172 6564  extractor.shared
-00000500: 5f6e 6574 716b 7d71 6c68 624b 0173 581a  _netqk}qlhbK.sX.
-00000510: 0000 006d 6c70 5f65 7874 7261 6374 6f72  ...mlp_extractor
-00000520: 2e73 6861 7265 645f 6e65 742e 3071 6d7d  .shared_net.0qm}
-00000530: 716e 6862 4b01 7358 1a00 0000 6d6c 705f  qnhbK.sX....mlp_
-00000540: 6578 7472 6163 746f 722e 7368 6172 6564  extractor.shared
-00000550: 5f6e 6574 2e31 716f 7d71 7068 624b 0173  _net.1qo}qphbK.s
-00000560: 581a 0000 006d 6c70 5f65 7874 7261 6374  X....mlp_extract
-00000570: 6f72 2e73 6861 7265 645f 6e65 742e 3271  or.shared_net.2q
-00000580: 717d 7172 6862 4b01 7358 1a00 0000 6d6c  q}qrhbK.sX....ml
-00000590: 705f 6578 7472 6163 746f 722e 7368 6172  p_extractor.shar
-000005a0: 6564 5f6e 6574 2e33 7173 7d71 7468 624b  ed_net.3qs}qthbK
-000005b0: 0173 5818 0000 006d 6c70 5f65 7874 7261  .sX....mlp_extra
-000005c0: 6374 6f72 2e70 6f6c 6963 795f 6e65 7471  ctor.policy_netq
-000005d0: 757d 7176 6862 4b01 7358 1700 0000 6d6c  u}qvhbK.sX....ml
-000005e0: 705f 6578 7472 6163 746f 722e 7661 6c75  p_extractor.valu
-000005f0: 655f 6e65 7471 777d 7178 6862 4b01 7358  e_netqw}qxhbK.sX
-00000600: 0a00 0000 6163 7469 6f6e 5f6e 6574 7179  ....action_netqy
-00000610: 7d71 7a68 624b 0173 5809 0000 0076 616c  }qzhbK.sX....val
-00000620: 7565 5f6e 6574 717b 7d71 7c68 624b 0173  ue_netq{}q|hbK.s
-00000630: 7573 622e                                usb.
+00000020: 0128 5821 0000 006d 6c70 5f65 7874 7261  .(X!...mlp_extra
+00000030: 6374 6f72 2e70 6f6c 6963 795f 6e65 742e  ctor.policy_net.
+00000040: 302e 7765 6967 6874 7102 6374 6f72 6368  0.weightq.ctorch
+00000050: 2e5f 7574 696c 730a 5f72 6562 7569 6c64  ._utils._rebuild
+00000060: 5f74 656e 736f 725f 7632 0a71 0328 2858  _tensor_v2.q.((X
+00000070: 0700 0000 7374 6f72 6167 6571 0463 746f  ....storageq.cto
+00000080: 7263 680a 466c 6f61 7453 746f 7261 6765  rch.FloatStorage
+00000090: 0a71 0558 0100 0000 3071 0658 0300 0000  .q.X....0q.X....
+000000a0: 6370 7571 074b 8074 7108 514b 004b 204b  cpuq.K.tq.QK.K K
+000000b0: 0486 7109 4b04 4b01 8671 0a89 6800 2952  ..q.K.K..q..h.)R
+000000c0: 710b 7471 0c52 710d 581f 0000 006d 6c70  q.tq.Rq.X....mlp
+000000d0: 5f65 7874 7261 6374 6f72 2e70 6f6c 6963  _extractor.polic
+000000e0: 795f 6e65 742e 302e 6269 6173 710e 6803  y_net.0.biasq.h.
+000000f0: 2828 6804 6805 5801 0000 0031 710f 6807  ((h.h.X....1q.h.
+00000100: 4b20 7471 1051 4b00 4b20 8571 114b 0185  K tq.QK.K .q.K..
+00000110: 7112 8968 0029 5271 1374 7114 5271 1558  q..h.)Rq.tq.Rq.X
+00000120: 2100 0000 6d6c 705f 6578 7472 6163 746f  !...mlp_extracto
+00000130: 722e 706f 6c69 6379 5f6e 6574 2e32 2e77  r.policy_net.2.w
+00000140: 6569 6768 7471 1668 0328 2868 0468 0558  eightq.h.((h.h.X
+00000150: 0100 0000 3271 1768 074d 0004 7471 1851  ....2q.h.M..tq.Q
+00000160: 4b00 4b20 4b20 8671 194b 204b 0186 711a  K.K K .q.K K..q.
+00000170: 8968 0029 5271 1b74 711c 5271 1d58 1f00  .h.)Rq.tq.Rq.X..
+00000180: 0000 6d6c 705f 6578 7472 6163 746f 722e  ..mlp_extractor.
+00000190: 706f 6c69 6379 5f6e 6574 2e32 2e62 6961  policy_net.2.bia
+000001a0: 7371 1e68 0328 2868 0468 0558 0100 0000  sq.h.((h.h.X....
+000001b0: 3371 1f68 074b 2074 7120 514b 004b 2085  3q.h.K tq QK.K .
+000001c0: 7121 4b01 8571 2289 6800 2952 7123 7471  q!K..q".h.)Rq#tq
+000001d0: 2452 7125 5820 0000 006d 6c70 5f65 7874  $Rq%X ...mlp_ext
+000001e0: 7261 6374 6f72 2e76 616c 7565 5f6e 6574  ractor.value_net
+000001f0: 2e30 2e77 6569 6768 7471 2668 0328 2868  .0.weightq&h.((h
+00000200: 0468 0558 0100 0000 3471 2768 074b 8074  .h.X....4q'h.K.t
+00000210: 7128 514b 004b 204b 0486 7129 4b04 4b01  q(QK.K K..q)K.K.
+00000220: 8671 2a89 6800 2952 712b 7471 2c52 712d  .q*.h.)Rq+tq,Rq-
+00000230: 581e 0000 006d 6c70 5f65 7874 7261 6374  X....mlp_extract
+00000240: 6f72 2e76 616c 7565 5f6e 6574 2e30 2e62  or.value_net.0.b
+00000250: 6961 7371 2e68 0328 2868 0468 0558 0100  iasq.h.((h.h.X..
+00000260: 0000 3571 2f68 074b 2074 7130 514b 004b  ..5q/h.K tq0QK.K
+00000270: 2085 7131 4b01 8571 3289 6800 2952 7133   .q1K..q2.h.)Rq3
+00000280: 7471 3452 7135 5820 0000 006d 6c70 5f65  tq4Rq5X ...mlp_e
+00000290: 7874 7261 6374 6f72 2e76 616c 7565 5f6e  xtractor.value_n
+000002a0: 6574 2e32 2e77 6569 6768 7471 3668 0328  et.2.weightq6h.(
+000002b0: 2868 0468 0558 0100 0000 3671 3768 074d  (h.h.X....6q7h.M
+000002c0: 0004 7471 3851 4b00 4b20 4b20 8671 394b  ..tq8QK.K K .q9K
+000002d0: 204b 0186 713a 8968 0029 5271 3b74 713c   K..q:.h.)Rq;tq<
+000002e0: 5271 3d58 1e00 0000 6d6c 705f 6578 7472  Rq=X....mlp_extr
+000002f0: 6163 746f 722e 7661 6c75 655f 6e65 742e  actor.value_net.
+00000300: 322e 6269 6173 713e 6803 2828 6804 6805  2.biasq>h.((h.h.
+00000310: 5801 0000 0037 713f 6807 4b20 7471 4051  X....7q?h.K tq@Q
+00000320: 4b00 4b20 8571 414b 0185 7142 8968 0029  K.K .qAK..qB.h.)
+00000330: 5271 4374 7144 5271 4558 1100 0000 6163  RqCtqDRqEX....ac
+00000340: 7469 6f6e 5f6e 6574 2e77 6569 6768 7471  tion_net.weightq
+00000350: 4668 0328 2868 0468 0558 0100 0000 3871  Fh.((h.h.X....8q
+00000360: 4768 074b 4074 7148 514b 004b 024b 2086  Gh.K@tqHQK.K.K .
+00000370: 7149 4b20 4b01 8671 4a89 6800 2952 714b  qIK K..qJ.h.)RqK
+00000380: 7471 4c52 714d 580f 0000 0061 6374 696f  tqLRqMX....actio
+00000390: 6e5f 6e65 742e 6269 6173 714e 6803 2828  n_net.biasqNh.((
+000003a0: 6804 6805 5801 0000 0039 714f 6807 4b02  h.h.X....9qOh.K.
+000003b0: 7471 5051 4b00 4b02 8571 514b 0185 7152  tqPQK.K..qQK..qR
+000003c0: 8968 0029 5271 5374 7154 5271 5558 1000  .h.)RqStqTRqUX..
+000003d0: 0000 7661 6c75 655f 6e65 742e 7765 6967  ..value_net.weig
+000003e0: 6874 7156 6803 2828 6804 6805 5802 0000  htqVh.((h.h.X...
+000003f0: 0031 3071 5768 074b 2074 7158 514b 004b  .10qWh.K tqXQK.K
+00000400: 014b 2086 7159 4b20 4b01 8671 5a89 6800  .K .qYK K..qZ.h.
+00000410: 2952 715b 7471 5c52 715d 580e 0000 0076  )Rq[tq\Rq]X....v
+00000420: 616c 7565 5f6e 6574 2e62 6961 7371 5e68  alue_net.biasq^h
+00000430: 0328 2868 0468 0558 0200 0000 3131 715f  .((h.h.X....11q_
+00000440: 6807 4b01 7471 6051 4b00 4b01 8571 614b  h.K.tq`QK.K..qaK
+00000450: 0185 7162 8968 0029 5271 6374 7164 5271  ..qb.h.)RqctqdRq
+00000460: 6575 7d71 6658 0900 0000 5f6d 6574 6164  eu}qfX...._metad
+00000470: 6174 6171 6768 0029 5271 6828 5800 0000  ataqgh.)Rqh(X...
+00000480: 0071 697d 716a 5807 0000 0076 6572 7369  .qi}qjX....versi
+00000490: 6f6e 716b 4b01 7358 1200 0000 6665 6174  onqkK.sX....feat
+000004a0: 7572 6573 5f65 7874 7261 6374 6f72 716c  ures_extractorql
+000004b0: 7d71 6d68 6b4b 0173 581a 0000 0066 6561  }qmhkK.sX....fea
+000004c0: 7475 7265 735f 6578 7472 6163 746f 722e  tures_extractor.
+000004d0: 666c 6174 7465 6e71 6e7d 716f 686b 4b01  flattenqn}qohkK.
+000004e0: 7358 1500 0000 7069 5f66 6561 7475 7265  sX....pi_feature
+000004f0: 735f 6578 7472 6163 746f 7271 707d 7171  s_extractorqp}qq
+00000500: 686b 4b01 7358 1d00 0000 7069 5f66 6561  hkK.sX....pi_fea
+00000510: 7475 7265 735f 6578 7472 6163 746f 722e  tures_extractor.
+00000520: 666c 6174 7465 6e71 727d 7173 686b 4b01  flattenqr}qshkK.
+00000530: 7358 1500 0000 7666 5f66 6561 7475 7265  sX....vf_feature
+00000540: 735f 6578 7472 6163 746f 7271 747d 7175  s_extractorqt}qu
+00000550: 686b 4b01 7358 1d00 0000 7666 5f66 6561  hkK.sX....vf_fea
+00000560: 7475 7265 735f 6578 7472 6163 746f 722e  tures_extractor.
+00000570: 666c 6174 7465 6e71 767d 7177 686b 4b01  flattenqv}qwhkK.
+00000580: 7358 0d00 0000 6d6c 705f 6578 7472 6163  sX....mlp_extrac
+00000590: 746f 7271 787d 7179 686b 4b01 7358 1800  torqx}qyhkK.sX..
+000005a0: 0000 6d6c 705f 6578 7472 6163 746f 722e  ..mlp_extractor.
+000005b0: 706f 6c69 6379 5f6e 6574 717a 7d71 7b68  policy_netqz}q{h
+000005c0: 6b4b 0173 581a 0000 006d 6c70 5f65 7874  kK.sX....mlp_ext
+000005d0: 7261 6374 6f72 2e70 6f6c 6963 795f 6e65  ractor.policy_ne
+000005e0: 742e 3071 7c7d 717d 686b 4b01 7358 1a00  t.0q|}q}hkK.sX..
+000005f0: 0000 6d6c 705f 6578 7472 6163 746f 722e  ..mlp_extractor.
+00000600: 706f 6c69 6379 5f6e 6574 2e31 717e 7d71  policy_net.1q~}q
+00000610: 7f68 6b4b 0173 581a 0000 006d 6c70 5f65  .hkK.sX....mlp_e
+00000620: 7874 7261 6374 6f72 2e70 6f6c 6963 795f  xtractor.policy_
+00000630: 6e65 742e 3271 807d 7181 686b 4b01 7358  net.2q.}q.hkK.sX
+00000640: 1a00 0000 6d6c 705f 6578 7472 6163 746f  ....mlp_extracto
+00000650: 722e 706f 6c69 6379 5f6e 6574 2e33 7182  r.policy_net.3q.
+00000660: 7d71 8368 6b4b 0173 5817 0000 006d 6c70  }q.hkK.sX....mlp
+00000670: 5f65 7874 7261 6374 6f72 2e76 616c 7565  _extractor.value
+00000680: 5f6e 6574 7184 7d71 8568 6b4b 0173 5819  _netq.}q.hkK.sX.
+00000690: 0000 006d 6c70 5f65 7874 7261 6374 6f72  ...mlp_extractor
+000006a0: 2e76 616c 7565 5f6e 6574 2e30 7186 7d71  .value_net.0q.}q
+000006b0: 8768 6b4b 0173 5819 0000 006d 6c70 5f65  .hkK.sX....mlp_e
+000006c0: 7874 7261 6374 6f72 2e76 616c 7565 5f6e  xtractor.value_n
+000006d0: 6574 2e31 7188 7d71 8968 6b4b 0173 5819  et.1q.}q.hkK.sX.
+000006e0: 0000 006d 6c70 5f65 7874 7261 6374 6f72  ...mlp_extractor
+000006f0: 2e76 616c 7565 5f6e 6574 2e32 718a 7d71  .value_net.2q.}q
+00000700: 8b68 6b4b 0173 5819 0000 006d 6c70 5f65  .hkK.sX....mlp_e
+00000710: 7874 7261 6374 6f72 2e76 616c 7565 5f6e  xtractor.value_n
+00000720: 6574 2e33 718c 7d71 8d68 6b4b 0173 580a  et.3q.}q.hkK.sX.
+00000730: 0000 0061 6374 696f 6e5f 6e65 7471 8e7d  ...action_netq.}
+00000740: 718f 686b 4b01 7358 0900 0000 7661 6c75  q.hkK.sX....valu
+00000750: 655f 6e65 7471 907d 7191 686b 4b01 7375  e_netq.}q.hkK.su
+00000760: 7362 2e                                  sb.
```

##### archive/data/0

```diff
@@ -1 +1,32 @@
-00000000: d20c 49bf 59b7 fdbd 746d 6638 b9b9 143a  ..I.Y...tmf8...:
+00000000: 03d1 13bf 34cf 19bf f82b bbbe b90f c9be  ....4....+......
+00000010: e2ba 943e 96c0 c13d 8c64 1b3f 5985 c53e  ...>...=.d.?Y..>
+00000020: fa00 193e f1ca d2be 62fb d2be cd15 1ebe  ...>....b.......
+00000030: 0751 31bf 4526 91be d29e 263d 981d 113f  .Q1.E&....&=...?
+00000040: 07a8 56be 18e3 b2be 3d2e 08bf 0e8a a6be  ..V.....=.......
+00000050: de0c 67bd 46b9 093d f6a7 183f 3fd9 a83e  ..g.F..=...??..>
+00000060: 3124 9b3e 9fef 563d ce94 5c3f 7fff 223e  1$.>..V=..\?..">
+00000070: 0976 c8be ff70 833e ad9a 3c3f 13e9 183f  .v...p.>..<?...?
+00000080: 4583 01be dc43 453e 12f0 9a3f 8ad6 cb3e  E....CE>...?...>
+00000090: 10d7 98be 3051 a23e 4877 a93f 990a 1f3d  ....0Q.>Hw.?...=
+000000a0: ef43 a9be 7d86 8d3e d74d 9ebe df31 cdbc  .C..}..>.M...1..
+000000b0: 971e b73e 831d f7bd 27a0 a63e 6a27 663e  ...>....'..>j'f>
+000000c0: cceb 3abc c2ac b83e 19f9 903e 985e 423e  ..:....>...>.^B>
+000000d0: cce9 5e3e 90c8 be3d b83b 3b3f 25c9 fb3e  ..^>...=.;;?%..>
+000000e0: a925 ebbc 69f6 6a3e 9aa3 23bf 8d29 e8be  .%..i.j>..#..)..
+000000f0: 8ed1 8fbd c7d0 033f a1b5 403f 91c8 263e  .......?..@?..&>
+00000100: 2bd0 c4be 1d56 17bf 5811 5abf 91bf 20bf  +....V..X.Z... .
+00000110: 10b3 eabe ba00 9abe dafb 3dbf 2a89 afbe  ..........=.*...
+00000120: 0b66 40be c1e2 babe 9fe6 31bf 32eb b9be  .f@.......1.2...
+00000130: 6c3d a73e 5e84 a0bd 5281 0b3f 4af2 123f  l=.>^...R..?J..?
+00000140: dd4f c4bd a06f f23e 4e25 bb3e 6104 b13e  .O...o.>N%.>a..>
+00000150: ac8b 0dbd ceab 02bf 7fab e6be 9939 3d3e  .............9=>
+00000160: 22f5 203e 4981 813d ed00 5a3f 3a79 013f  ". >I..=..Z?:y.?
+00000170: 31fb 823e bea4 73be 48c4 b1be afd1 cbbe  1..>..s.H.......
+00000180: 9287 79bd 2de1 143e 410c 48bf e944 9fbe  ..y.-..>A.H..D..
+00000190: d2ee a7be e882 a63e 4d28 363f 7f95 7c3e  .......>M(6?..|>
+000001a0: 916a 3c3c e682 f03e 1c31 043f c181 133f  .j<<...>.1.?...?
+000001b0: 1ebd dcbc 00bb 78be bbf5 2e3f dc9a 1c3e  ......x....?...>
+000001c0: b490 97be 4f15 babe 5bdb d33e a5e8 363e  ....O...[..>..6>
+000001d0: 2da9 9d3c afce 653d fa09 043f 5b8d 573e  -..<..e=...?[.W>
+000001e0: 0542 7fbe a32a 6a3e ead7 bd3e 776b b43e  .B...*j>...>wk.>
+000001f0: 1d72 473e 4dfa 53be def7 e1be 7d47 31be  .rG>M.S.....}G1.
```

##### archive/data/1

```diff
@@ -1 +1,8 @@
-00000000: 5d33 e03e 60c7 0a3e 0f79 af3a 2f8d f23d  ]3.>`..>.y.:/..=
+00000000: af36 603b 9ea0 86bc bff7 883c 05c8 24bd  .6`;.......<..$.
+00000010: 6f64 933c 5bec 0dbc bed9 80bb 0ba8 a2bc  od.<[...........
+00000020: 812f 61bc ac2e b2bc 3d40 0ebd 9709 de3c  ./a.....=@.....<
+00000030: 41ca 31bc 16b3 5dbc cac9 023c dcbc aabc  A.1...]....<....
+00000040: c667 a83b befb b93b 7e9b b03b ca5f 84bc  .g.;...;~..;._..
+00000050: 35ba 113b 8a6b 773b 050b a4bc fcee 473c  5..;.kw;......G<
+00000060: 3ae0 223c c90f dabc f0df efbb 812b a53c  :."<.........+.<
+00000070: dbb7 0bbd 3d2e 85bb abe0 27bc 9dbe 4a3c  ....=.....'...J<
```

##### archive/data/10

```diff
@@ -1 +1,8 @@
-00000000: 9909 e83d                                ...=
+00000000: fa27 a83d 47fe 643e 9f65 89be 23ef b5be  .'.=G.d>.e..#...
+00000010: 7313 523e eaef 333e 62b9 773e ac2a 843e  s.R>..3>b.w>.*.>
+00000020: 3e3b f03e 81c7 0d3e 55e5 bb3e 38c8 a1be  >;.>...>U..>8...
+00000030: 98b3 e13e ff73 703e 4b73 3abe 795e 963e  ...>.sp>Ks:.y^.>
+00000040: 7f1d 873e 06e6 d53c d269 7dbc e477 0ebf  ...>...<.i}..w..
+00000050: 99c9 70be 697e 373d 0988 9d3e 82a4 ba3e  ..p.i~7=...>...>
+00000060: bc9a 0a3e 453c b63e 2da5 ebbe 259f 273e  ...>E<.>-...%.'>
+00000070: 40e4 95be 0f4a 733e 1a11 23be 5bcc 5cbe  @....Js>..#.[.\.
```

##### archive/data/2

```diff
@@ -1 +1,256 @@
-00000000: 0050 0f00                                .P..
+00000000: 5038 94bd d0d1 5d3e a157 80bd da8b 8a3e  P8....]>.W.....>
+00000010: 6c28 65bf 667d 35bd e2ba c13e 79c9 013f  l(e.f}5....>y..?
+00000020: f84b 6e3f 3f31 213e 60ed bfbe 2c97 903e  .Kn??1!>`...,..>
+00000030: 70cd 113e 044f a53e 6fc9 933d fbca cd3e  p..>.O.>o..=...>
+00000040: 5830 50bf 550d 05bf f4a8 4bbf 07da bd3e  X0P.U.....K....>
+00000050: f51b bb3e 9dcd 10bf 1759 c23e 3fd8 e73d  ...>.....Y.>?..=
+00000060: 4cf5 a9be 1f4d a93d ddbf d83e 5784 953c  L....M.=...>W..<
+00000070: eed5 63bd bb81 b13e 113f 68be 1a6d 103e  ..c....>.?h..m.>
+00000080: 4ceb 063e 1363 8d3e f3f7 f43e 9ddd c53d  L..>.c.>...>...=
+00000090: 8670 86be 376f 9cbe 34e3 b4bd c126 f73d  .p..7o..4....&.=
+000000a0: 1400 24be e3f8 57be ac0e 233e fc7f 1ebf  ..$...W...#>....
+000000b0: 887f 5a3d cd6e 9d3d 7f09 c3bd 9a42 c1be  ..Z=.n.=.....B..
+000000c0: e950 993e 85b5 87bd 47dd ab3e 7daf d7be  .P.>....G..>}...
+000000d0: a4c5 2e3e 8f3c 273e bfa4 c5be a672 18bd  ...>.<'>.....r..
+000000e0: 47e3 32bd 82c9 09bf 76de e03e f801 24ba  G.2.....v..>..$.
+000000f0: 3a2a bfbc 7761 563e dc2c 55bc f7c9 d03d  :*..waV>.,U....=
+00000100: 51b6 95be 14be 193e 38d1 9c3e bdbb 593d  Q......>8..>..Y=
+00000110: ef03 dcbd 0703 b7bd d76a c43d ae85 1cbf  .........j.=....
+00000120: 9385 ebbe a53f ac3d 7500 c8be 0b5b ffbd  .....?.=u....[..
+00000130: ae2b 82be db7c 0fbf 4f76 16be 1121 0bbe  .+...|..Ov...!..
+00000140: 0969 613c 2e66 913e 80d2 c33e 72d9 c2be  .ia<.f.>...>r...
+00000150: 9f41 a2be a8d7 d6be 3cd0 3d3e c140 093f  .A......<.=>.@.?
+00000160: 1da7 9d3e 3762 a3be 50e6 47be 8766 47be  ...>7b..P.G..fG.
+00000170: c9f7 05be c691 1abe 2b03 bfbb 5a38 103f  ........+...Z8.?
+00000180: e883 da3d a48c bdbd ef2a d3be 60a7 9c3e  ...=.....*..`..>
+00000190: e586 8b3e c5ee 463c 5b85 94be 15ae 3dbe  ...>..F<[.....=.
+000001a0: 0072 9bbe a8d8 14be d5d6 3b3d f153 e1bd  .r........;=.S..
+000001b0: 9a1b 87bd 93c8 0a3c f0da c5be afed 5bbe  .......<......[.
+000001c0: b11c f9bd b9d5 123d c807 32be 3886 ee3d  .......=..2.8..=
+000001d0: fb39 4b3c 0568 383c 6694 ccbd 8c9d f33e  .9K<.h8<f......>
+000001e0: 79a5 bfbd d25c 03bf f773 17bd 2bc9 16bf  y....\...s..+...
+000001f0: 9860 703e 1c35 e73d 6781 35be 25fd 03bf  .`p>.5.=g.5.%...
+00000200: e596 68be 0be3 0abf 2f41 63be b85e acbe  ..h...../Ac..^..
+00000210: 3e72 1e3c 3135 92be 3026 083c c083 d1bc  >r.<15..0&.<....
+00000220: 6bce a13c 2496 89be 0123 f73c 8e76 32be  k..<$....#.<.v2.
+00000230: f851 0cbe 93bb 3bbe 9f6d 9d3d 0f95 42bf  .Q....;..m.=..B.
+00000240: 0999 763e c39a b2bd 02f8 c0bc 5e0f 12bd  ..v>........^...
+00000250: f6fc 47be e896 edb9 76f0 043f 557f 9bbc  ..G.....v..?U...
+00000260: 2e87 8abe e148 d53d 08b9 bb3e 2562 37be  .....H.=...>%b7.
+00000270: ce91 99bb d3ea 0cbe a629 263d c8de 213e  .........)&=..!>
+00000280: 4f49 62bf 9c34 ec3e c97f 3dbf f297 bfbe  OIb..4.>..=.....
+00000290: ae48 22bf c833 9b3e 5491 d03e 3a69 1e3f  .H"..3.>T..>:i.?
+000002a0: 6ce9 a33e e2ff 923e a056 bdbe a337 18bc  l..>...>.V...7..
+000002b0: aa51 113f 2867 3a3f 5ebc eabe da3a 393f  .Q.?(g:?^....:9?
+000002c0: 8971 56bf c274 2ebf ffc9 73bf 0fe7 a13e  .qV..t....s....>
+000002d0: ed2e 543e e7e1 02be cba8 553e fd8a 88bd  ..T>......U>....
+000002e0: f18d 1b3d 472a cb3d f358 803f a8b0 d73e  ...=G*.=.X.?...>
+000002f0: cc61 9abd 200a 0dbd 4b68 2b3e d50a 853d  .a.. ...Kh+>...=
+00000300: ddb0 383f 8a29 57bf 6c0a 383e 63d3 2b3e  ..8?.)W.l.8>c.+>
+00000310: 5a4e 2c3f 7a07 6fbe 7787 23bf 0b35 253e  ZN,?z.o.w.#..5%>
+00000320: 0fe8 43bf 020d e1be 09a3 8a3e d75b c23d  ..C........>.[.=
+00000330: a86b f3be e6df 36bf b0fa 0abe d64e e5be  .k....6......N..
+00000340: 1b07 883e 4f8d 763f 59ee 0c3f c31e 60bf  ...>O.v?Y..?..`.
+00000350: d6fc 2ebf cd6a 953e 0741 06bf 81e0 563e  .....j.>.A....V>
+00000360: 703e 2b3e c2f1 19be 094f f3be b609 7b3e  p>+>.....O....{>
+00000370: dff5 90bd b9e8 923d 54ce 82be 4ad7 aa3e  .......=T...J..>
+00000380: d79d 803e 5dbb 7ebe 67bb a43d 04e4 5ebe  ...>].~.g..=..^.
+00000390: 6e78 2a3d 71c9 febe 1b89 e3be b7d6 4fbf  nx*=q.........O.
+000003a0: a709 02bf 2b58 0abf e577 65be 6c39 c5be  ....+X...we.l9..
+000003b0: a5a4 c6be ae44 b03d 1bd4 083f 12dd 40be  .....D.=...?..@.
+000003c0: f9fb 3bbe 59a6 823e e3f7 5d3e 0614 6b3e  ..;.Y..>..]>..k>
+000003d0: 1670 85be c73b 1f3e 073d 83be 1608 803d  .p...;.>.=.....=
+000003e0: 6554 ed3e 1c7d babe 29a5 87be 8508 3fbd  eT.>.}..).....?.
+000003f0: 0f83 10bf b593 14bd 45a9 f5be bdb4 ff3e  ........E......>
+00000400: c523 babd 4b35 683e e2eb 1c3e fb4b 54be  .#..K5h>...>.KT.
+00000410: ea62 033e 28a7 40be 6ee1 003e d4c0 a93e  .b.>(.@.n..>...>
+00000420: f423 37bd 7046 b33d 3a25 d93e ad63 cebd  .#7.pF.=:%.>.c..
+00000430: 81a6 f1be 21af 25bd aa46 94be 4049 e33e  ....!.%..F..@I.>
+00000440: c8cd 20bd 371c 1d3c 4c0b 35bc aeb2 353f  .. .7..<L.5...5?
+00000450: 986f 0cbd 911e 9ebe 12d9 943e a7e5 8c3e  .o.........>...>
+00000460: ab5d 15be 175b 443d cdd3 753e aa93 023e  .]...[D=..u>...>
+00000470: ada9 03bf a7bc 923e 0432 303e 7034 0fbe  .......>.20>p4..
+00000480: c3e7 36bd 7666 b0bd 75d4 913c 5a02 c4be  ..6.vf..u..<Z...
+00000490: 0ee8 6dbe b298 7bbc 9387 133e 518f 1ebe  ..m...{....>Q...
+000004a0: f796 18bd 9547 883e 7885 8f3c fb71 12be  .....G.>x..<.q..
+000004b0: 9487 ad3d 0c40 33be 4244 033f f6d3 9d3e  ...=.@3.BD.?...>
+000004c0: b1be 13bf ed0e 3b3e dc8b 7b3e 4703 f83b  ......;>..{>G..;
+000004d0: ec35 283c f78f 313e f607 613d ce64 813e  .5(<..1>..a=.d.>
+000004e0: 4268 d9be 62a3 0c3d 12a2 a13e a91b 563e  Bh..b..=...>..V>
+000004f0: 0819 043f 00b7 5a3e 627f 3e3d 3871 d4be  ...?..Z>b.>=8q..
+00000500: c4f0 843e 6386 5fbe 6431 85be 22a6 143e  ...>c._.d1.."..>
+00000510: 4fbb b8be 9e6d a43e 6bef 8c3e 22b1 5abc  O....m.>k..>".Z.
+00000520: 94d8 fcbe 4115 f8be bbe7 99bd f9e9 52be  ....A.........R.
+00000530: 84af a3be 9296 67be 5ff3 a93d 678b 013e  ......g._..=g..>
+00000540: c696 083f e605 bc3e e310 16be d589 933b  ...?...>.......;
+00000550: 6eb2 913e 0d5e 84be 9e84 26bc 5f99 a0be  n..>.^....&._...
+00000560: 838f b63d 0715 063d ac9c 283d 1db3 b33d  ...=...=..(=...=
+00000570: 8bfa 803e 9cd2 3cbb d8a9 c33d e4c9 2cbe  ...>..<....=..,.
+00000580: 39c7 0ebe f5e7 993e d3ab fdbe 373e be3e  9......>....7>.>
+00000590: 641f b2be c17c ea3e 5908 d5bc be32 5f3d  d....|.>Y....2_=
+000005a0: 1123 203f 8aeb 983e 58e0 4e3c 66f4 e3be  .# ?...>X.N<f...
+000005b0: bec4 34be f8f1 133e 4e79 eabe ca79 e7bd  ..4....>Ny...y..
+000005c0: b521 00bf 4bb3 eaba dff1 16be c48f 853d  .!..K..........=
+000005d0: b931 723e 97a0 193e 18d5 263d 7e59 6fbe  .1r>...>..&=~Yo.
+000005e0: bc99 f1be eec4 163f 0a7f 89bd 14b2 da3e  .......?.......>
+000005f0: 122a 4cbe e34c cfbd 859f e03e 4310 d4be  .*L..L.....>C...
+00000600: d703 fc3c 7757 513e 6a9e 6cbe 1ab0 b83e  ...<wWQ>j.l....>
+00000610: 21e2 32bd 5ec1 093e a227 1b3f 5066 9e3e  !.2.^..>.'.?Pf.>
+00000620: a637 a93e 16a1 b83d d85e 833e 18ed 80be  .7.>...=.^.>....
+00000630: 1a7b 973e d636 e33e c8f1 58be 5287 273e  .{.>.6.>..X.R.'>
+00000640: 690b 1ebf 8e8d a1be 3a8c cbbd 8dbf 443e  i.......:.....D>
+00000650: 8c9d 503e d232 a83d 9501 5f3f 1d60 70be  ..P>.2.=.._?.`p.
+00000660: 01a2 fd3e 25e7 183e ec32 f33d a5c5 b53e  ...>%..>.2.=...>
+00000670: fab7 e73e 70f8 553e 75db 2d3e 5195 1bbe  ...>p.U>u.->Q...
+00000680: a601 ff3e 7a71 d73e aa2e a5be 0a33 6b3d  ...>zq.>.....3k=
+00000690: c48b e83e f80c 0cbe 50b0 c03e c667 49be  ...>....P..>.gI.
+000006a0: 620c 6c3d 0782 8cbe 145d 26be 9fdc 90bd  b.l=.....]&.....
+000006b0: 8d6c d83d 048a f2be 653a 2f3e f488 033c  .l.=....e:/>...<
+000006c0: 985c 323e 80db 6abe 7fb2 203e 4d82 9ebe  .\2>..j... >M...
+000006d0: ce2b a0be 77d1 223c 7a12 85bd f16a 7b3d  .+..w."<z....j{=
+000006e0: 7d38 2fbc ee52 093e eab7 943e a5cf 613c  }8/..R.>...>..a<
+000006f0: 21d6 bfbe 6c0b 65bd 2255 cdbe aa4d 41be  !...l.e."U...MA.
+00000700: 1944 0b3f 3082 113f 7a78 d3bd c57c 1bbf  .D.?0..?zx...|..
+00000710: a9ed 55be 387a 173e fc0c 8fbe 8987 0ebd  ..U.8z.>........
+00000720: 6983 353c 6426 afbe 6322 6e3e 21a3 223d  i.5<d&..c"n>!."=
+00000730: b11c a5bd 324e 6e3c 2d90 373e 400b 9ebd  ....2Nn<-.7>@...
+00000740: 15ea b63d 8b5e c53d e820 69be 254a 9bbe  ...=.^.=. i.%J..
+00000750: b03b 95bc 6816 313e c038 103e 6bc2 c23e  .;..h.1>.8.>k..>
+00000760: b1c1 ad3d 7ece 2ebd e662 5abe 1e71 53be  ...=~....bZ..qS.
+00000770: 709c ff3d 09dd 5bbd 6232 ba3e 0433 983e  p..=..[.b2.>.3.>
+00000780: f51b 38bd dce5 2c3e 2915 a93d d3a0 3dbd  ..8...,>)..=..=.
+00000790: 802c 363e 7166 6bbe 6738 793d 2118 3dbe  .,6>qfk.g8y=!.=.
+000007a0: e1cb c9be 6da9 c1bd f4ab aabe f732 d83e  ....m........2.>
+000007b0: 0954 acbe 6d6e c63a 67fd a23e 9ec3 0fbf  .T..mn.:g..>....
+000007c0: 1c6e 9f3d 26ef 8dbe a778 42be b727 31be  .n.=&....xB..'1.
+000007d0: 019b e13d 2e82 aabd 918c 8abe d421 f03d  ...=.........!.=
+000007e0: 3c62 443e 6c52 56be ce00 b5bd 5b1c 143f  <bD>lRV.....[..?
+000007f0: 802c f03c 707e 7e3e dcc7 c03e d7dc a5be  .,.<p~~>...>....
+00000800: cc36 073f 69af 1cbf 28cc 723e 5d5e acbe  .6.?i...(.r>]^..
+00000810: 29e0 223e 879e cabe 0c20 c8bc 3d14 203d  ).">..... ..=. =
+00000820: ea69 d9be b429 bbbe e120 94be a3b6 86be  .i...)... ......
+00000830: 594e 21be eeeb b73d d10b ffbd 03dd 1bbe  YN!....=........
+00000840: 6d8a 633e 4f83 44be 1361 2d3f 1f69 a8be  m.c>O.D..a-?.i..
+00000850: 7727 5dbd 88e1 73be 171d 9bbe 10db 0b3f  w']...s........?
+00000860: 1f66 b03d a763 cfbc 1e53 30bf 33ff 68bd  .f.=.c...S0.3.h.
+00000870: 5cac d4bd c94e efbe b3f9 d8bc e5a0 7cbd  \....N........|.
+00000880: 89b5 6fbe ef99 883e de13 b5be 5b25 683e  ..o....>....[%h>
+00000890: 8555 c2be d0de 8fbe cffd d73d 3e78 d0bc  .U.........=>x..
+000008a0: b4cb f03b 45d9 2d3e 8f25 103d ee3c ef3d  ...;E.->.%.=.<.=
+000008b0: c6f1 503f ced9 f63e 3330 20be a1c7 b73e  ..P?...>30 ....>
+000008c0: 6d02 483d f9ad b33d 6206 9bbe cf84 de3b  m.H=...=b......;
+000008d0: ec77 603e 7eba ecbd 8eff 173f ce30 82bd  .w`>~......?.0..
+000008e0: ce61 23bf 8795 2e3e ea39 c1bd 72cb e23e  .a#....>.9..r..>
+000008f0: a676 3fbe 7dbb ba3e da04 8b3d 3b8c 26be  .v?.}..>...=;.&.
+00000900: 55b1 ac3e 634c 8fbe c283 523e dcad bbbe  U..>cL....R>....
+00000910: c675 493c e7c9 873e 4575 d53e aa95 14bf  .uI<...>Eu.>....
+00000920: 37cb d7bd ed2a 933b 1033 b63e a853 2a3e  7....*.;.3.>.S*>
+00000930: 3aab 54bd bf82 80bd cee8 80be 9da0 e1bd  :.T.............
+00000940: 2bd5 3fbd 354e a0bd 360e 0bbb 0f8a cabd  +.?.5N..6.......
+00000950: 0ca9 9c3b fd35 45bd 0ced 6ebe 035f 60be  ...;.5E...n.._`.
+00000960: bf76 82be 8364 1abf 18dc acbd 2ce5 713e  .v...d......,.q>
+00000970: 3180 f8bd 5cfa 8dbe 5562 80be 00a6 2f3e  1...\...Ub..../>
+00000980: 42cd 48be fb2b 4f3e ee66 5d3e afdf 25be  B.H..+O>.f]>..%.
+00000990: 03eb 15bd 2d46 833e ed35 273e 3daf 0c3f  ....-F.>.5'>=..?
+000009a0: 8caa e0be 78af bb3c 7a16 41be 5dcf 99be  ....x..<z.A.]...
+000009b0: 32f5 53bd 6cc0 4bbe 7f88 c13e 7145 41be  2.S.l.K....>qEA.
+000009c0: d49f c6bd 9431 b1ba 94bc 1dbe 9424 f7bd  .....1.......$..
+000009d0: 0899 1ebe 4b27 4e3e 1f8b 1c3e c88e 72be  ....K'N>...>..r.
+000009e0: 6147 17be 318b a7be 14bd 12bf fbf5 2cbe  aG..1.........,.
+000009f0: 8efe 84be 124d b7bd a61a bebe 9cc8 56be  .....M........V.
+00000a00: 5237 41bf 187f 853e 83e6 11be 2208 1d3e  R7A....>...."..>
+00000a10: 12a4 84be 6dbb 8f3d 0a50 f13e 2fc9 d63d  ....m..=.P.>/..=
+00000a20: 947e 5c3e bce5 3dbe 247f ea3e a0e7 3a3e  .~\>..=.$..>..:>
+00000a30: d397 8bbd 691e ce3e 900e 193e ab4e 263e  ....i..>...>.N&>
+00000a40: cc04 ccbe 4538 c4bd 97cc 8bbe 2631 f4bd  ....E8......&1..
+00000a50: 03c5 2d3f 8ac7 adbd d9b8 6c3a b635 c13e  ..-?......l:.5.>
+00000a60: b525 49bc 399e cb3e 9ad2 963e a86f 103d  .%I.9..>...>.o.=
+00000a70: 93a8 b3bd de7d c0bd 38fb cdbe de8d 423c  .....}..8.....B<
+00000a80: 6241 f5be 14f9 0f3f 2a98 933e 799a 78bd  bA.....?*..>y.x.
+00000a90: 6829 f4be 0698 76be 1d89 8e3e 8c55 3cbd  h)....v....>.U<.
+00000aa0: 5a63 7d3e 9d1d e3be ac33 66be 6e60 c73e  Zc}>.....3f.n`.>
+00000ab0: 72f1 98bd 8c73 0a3f 0e63 a4be 946f 053f  r....s.?.c...o.?
+00000ac0: 6d8b 1fbf 0670 7dbe 1fdc c8be 2989 3f3c  m....p}.....).?<
+00000ad0: 9c2d 95be 3054 36be 0af9 b73e d7bd ffbe  .-..0T6....>....
+00000ae0: 80d4 81be b895 383e 464a ba3e 6333 25be  ......8>FJ.>c3%.
+00000af0: 740f 273e 12d7 48be 6c62 b33d d93e e2be  t.'>..H.lb.=.>..
+00000b00: 5c0b 053d a6c3 603e b926 e4be 0760 49bd  \..=..`>.&...`I.
+00000b10: 7e64 783b 58b9 6b3b 7fb4 823d 0c9e 053d  ~dx;X.k;...=...=
+00000b20: 9318 8ebe daa6 963d 5771 933d fb04 4d3e  .......=Wq.=..M>
+00000b30: 4602 debe 9518 ff3e 3f77 5a3e 48e8 56be  F......>?wZ>H.V.
+00000b40: ac23 443e 252d 023c acf1 273f fe8e 0abd  .#D>%-.<..'?....
+00000b50: 51f7 dcbe 311e 88be b7ea 54be 45fe b4bd  Q...1.....T.E...
+00000b60: bfbc 45be c724 0dbe d024 10be b6d8 3fbe  ..E..$...$....?.
+00000b70: f5f8 383e bcca 263e dc0d 88be b4f6 c93e  ..8>..&>.......>
+00000b80: ce00 b5bd 2962 5f3e 8f86 16bf efce 4a3e  ....)b_>......J>
+00000b90: 8840 15bf ee91 b0bd c180 a23e d616 f03e  .@.........>...>
+00000ba0: 90c3 853e 6545 473f 51ce b23d e61a e93e  ...>eEG?Q..=...>
+00000bb0: 3e66 7e3e df79 b63e c29b f7bd 2709 da3e  >f~>.y.>....'..>
+00000bc0: 1580 39bf fe93 84be cf2d 81be bc59 a53c  ..9......-...Y.<
+00000bd0: 45a4 5f3f b455 ec3d 2f4d 073f 40f8 00bf  E._?.U.=/M.?@...
+00000be0: 1e15 adbc 83aa 483e a833 353f 6bb2 b3be  ......H>.35?k...
+00000bf0: 7250 e1be 3365 01be 5c75 093f 5360 acbe  rP..3e..\u.?S`..
+00000c00: 3ef7 853e c41e c4be 561a 0b3e fcd4 223e  >..>....V..>..">
+00000c10: 6785 543e 084b 44be 956f 31be bd7d 21be  g.T>.KD..o1..}!.
+00000c20: 946d 60bc 1363 09bf 21d1 01be cfe1 fe3d  .m`..c..!......=
+00000c30: d6dc dfbe b286 b4be 99eb bb3e e94f 97be  ...........>.O..
+00000c40: 1b68 593f 0f4c 353f 7721 453f 463d cabd  .hY?.L5?w!E?F=..
+00000c50: b911 2abf e3ab f93e 2489 87be 824e 103f  ..*....>$....N.?
+00000c60: 9db8 773e cbab 70bf 2ce7 eebe f536 483e  ..w>..p.,....6H>
+00000c70: b974 01be ee07 12bf 3550 aabd f707 af3c  .t......5P.....<
+00000c80: f51c 7abd d8f0 47bd dc76 1bbe 1563 4b3d  ..z...G..v...cK=
+00000c90: f1a5 3ebf 0aa8 613e 78e1 2abd a68d ab3d  ..>...a>x.*....=
+00000ca0: 230d 133e 8df8 893e 6c43 003f ef12 bb3d  #..>...>lC.?...=
+00000cb0: 60cd b93e 5106 48ba 66f3 5f3c e141 eebd  `..>Q.H.f._<.A..
+00000cc0: f2d0 25be e500 68be 18c1 a93a 7e26 f53d  ..%...h....:~&.=
+00000cd0: bbbf f4be 1e5d d0be 5660 93bd 1970 e5bc  .....]..V`...p..
+00000ce0: 17ad d63e b273 563e 7390 b53d 53c2 3f3c  ...>.sV>s..=S.?<
+00000cf0: 0ab7 4dbe f94c 2c3e 4a2d ff3c 472f 01bf  ..M..L,>J-.<G/..
+00000d00: 866e 88bd 82e7 08be c02d 9c3d 5920 c0be  .n.......-.=Y ..
+00000d10: b185 cc3c e564 a93e 1358 413e 0f39 b9bd  ...<.d.>.XA>.9..
+00000d20: 91ce 293e 5afa c9be 2c31 c8be 0475 483e  ..)>Z...,1...uH>
+00000d30: 60bb 9f3d c5c4 3e3d d499 9abe b075 03be  `..=..>=.....u..
+00000d40: 3f3f 0a3e c984 b43e d108 ef3e 9980 cabd  ??.>...>...>....
+00000d50: 8fee 213e 9243 a73e f02a a1bd a871 2f3c  ..!>.C.>.*...q/<
+00000d60: 3869 373e f6fa 243d 8ca1 aabd 9010 58be  8i7>..$=......X.
+00000d70: 2434 5ebe d025 353f d325 b6bd ecd5 21be  $4^..%5?.%....!.
+00000d80: fb5b 88be 1665 f7bd b427 80be 2f0d a23e  .[...e...'../..>
+00000d90: d367 de3d d1bd cd3c ed0b d73e aeca 1d3e  .g.=...<...>...>
+00000da0: 5d09 413e 4946 9fbe b702 5d3e 59ac d2bd  ].A>IF....]>Y...
+00000db0: 0765 863e b0c4 15be 6e54 3d3e e6d2 703e  .e.>....nT=>..p>
+00000dc0: e2a9 bfbe 49a0 5bbe 3719 b9bc 6d80 8c3d  ....I.[.7...m..=
+00000dd0: 50a3 babd 3776 77bd 8a67 93be e884 32be  P...7vw..g....2.
+00000de0: 7cdb 98be c808 87bd 15a3 38be 9fe3 56be  |.........8...V.
+00000df0: fe80 6abd 65f4 963e 8a42 4e3f 7fc0 6b3e  ..j.e..>.BN?..k>
+00000e00: db7e c5bd 18c5 dcbe 9ff2 6ebd 4409 babd  .~........n.D...
+00000e10: c13a bf3e 4d06 3c3c 02ac e9be 8667 64be  .:.>M.<<.....gd.
+00000e20: 51df 8b3e 6853 613d 7563 943e b17c 78be  Q..>hSa=uc.>.|x.
+00000e30: c238 f4be dffb 33bb d709 4e3e d945 963e  .8....3...N>.E.>
+00000e40: 5dc9 b93e e189 bcbd 7547 7b3d 8f7d 40bf  ]..>....uG{=.}@.
+00000e50: 3892 b9bd 5016 febd eef5 313e 6bda 93bd  8...P.....1>k...
+00000e60: e5dd 4d3e a577 c6be 77a4 87be 32a0 26bc  ..M>.w..w...2.&.
+00000e70: f42e 2bbe 8bc1 793e 1508 cabc f6c0 0abe  ..+...y>........
+00000e80: 1e65 803e 0168 40be 322f a7bd 2d89 9cbe  .e.>.h@.2/..-...
+00000e90: 4bdd 083f cbd4 26bf 0d59 e4bc 632e 773b  K..?..&..Y..c.w;
+00000ea0: c7ee 3b3e b11b b03d 49af 3c3e d307 9ebe  ..;>...=I.<>....
+00000eb0: 6a15 b7bd 6e1d adbe 0e9e 15bd 6037 fbbe  j...n.......`7..
+00000ec0: 7d21 9f3e 49d1 833f cf04 063e 9972 57be  }!.>I..?...>.rW.
+00000ed0: 1880 f8bd 81ff 91be 2cca 0dbf eff2 13be  ........,.......
+00000ee0: e1f3 b33e 274f 75be 0bf5 04bf 10c6 aebd  ...>'Ou.........
+00000ef0: 71eb 323e e1d1 12be 114c 42bd a969 9fbd  q.2>.....LB..i..
+00000f00: 63ba f1bb 543b 103e 1cb9 79bc 800f f93c  c...T;.>..y....<
+00000f10: a12c b53e 74bd f93e c304 e0be 1589 733e  .,.>t..>......s>
+00000f20: cc8d 273e 73c6 7abe 37af b63b f3d8 c83d  ..'>s.z.7..;...=
+00000f30: f59c a63e 55b9 613d f5a7 043e da1c 2cbe  ...>U.a=...>..,.
+00000f40: 9a6a b9be 6cad 4d3e c241 a53e bdab 823d  .j..l.M>.A.>...=
+00000f50: fe92 af3e b2ac 30bf b927 893e 892f 40be  ...>..0..'.>./@.
+00000f60: 527d 06be 707a 2bbe eaf5 733e dc66 4d3e  R}..pz+...s>.fM>
+00000f70: 328c c8bd 974d 35be 8b0a d03d e29e 00be  2....M5....=....
+00000f80: 8b4d 4abe e82c 1f3e 10bb bbbe 0767 21be  .MJ..,.>.....g!.
+00000f90: 8f1f 5abe afb9 aebe 24a8 b6be 9ff5 913d  ..Z.....$......=
+00000fa0: 4513 43ba cea9 74be 77c6 253e 8a7d 3f3e  E.C...t.w.%>.}?>
+00000fb0: 114c 45bd bf12 35bf 9bea 94be 9f38 7c3d  .LE...5......8|=
+00000fc0: c7ab c43c 2901 b6be 7eb5 c73e 18b7 f53d  ...<)...~..>...=
+00000fd0: 0739 bd3e 2b2b 143e 6caf 8bbc 6170 8abe  .9.>++.>l...ap..
+00000fe0: e5eb 8f3d 402a 20be ba32 a3be 7cc9 5a3e  ...=@* ..2..|.Z>
+00000ff0: 5214 913e c34f 1c3d e847 88be 624b bc3d  R..>.O.=.G..bK.=
```

##### archive/data/3

```diff
@@ -1,32 +1,8 @@
-00000000: c2a8 503e 5cf8 543d 67ca 3e3d 1dd1 78be  ..P>\.T=g.>=..x.
-00000010: 27a7 703e 59f1 94be 3e7b 04bc 73f0 6dbd  '.p>Y...>{..s.m.
-00000020: bb60 d13e df59 a6bd 5680 8f3c cbb5 c93d  .`.>.Y..V..<...=
-00000030: ae35 9a3d eb1e e4bd 0948 b33d 365f 963c  .5.=.....H.=6_.<
-00000040: 01c8 ff3d 664a d93d 163b eabd 2f2c 99bb  ...=fJ.=.;../,..
-00000050: f223 cb3e 6811 253e daf5 d53d b4cf c63c  .#.>h.%>...=...<
-00000060: dcbe 0abe d538 b8bc 785a 5bbe 1879 94be  .....8..xZ[..y..
-00000070: 7d05 acbd 1a9d 11be 0910 9b3e a1a6 fa3c  }..........>...<
-00000080: 1184 fe3d 6903 77bd d16d 013e 877d cdbd  ...=i.w..m.>.}..
-00000090: f9e9 4e3e 3652 87bd 3b90 a4bd 9e22 95bb  ..N>6R..;...."..
-000000a0: c0ce 36be 3d4c 21be 49b7 6e3e f2bd d8bd  ..6.=L!.I.n>....
-000000b0: 410f a3bd cbbc c7be 9636 b8be 3313 efbd  A........6..3...
-000000c0: dbe8 4cbd 0be8 013e a2d6 f93e bd17 923e  ..L....>...>...>
-000000d0: cdfc 353d 95bd 093e 8fa2 00bf 48e4 a2be  ..5=...>....H...
-000000e0: 7ff6 8e3e 16a6 613e d44f c33e da54 323e  ...>..a>.O.>.T2>
-000000f0: 30d2 b2be 1ee2 7bbe d7db c23d 8693 a83d  0.....{....=...=
-00000100: 0701 44bd 82ae bdbe 7222 d7be 8caa 713b  ..D.....r"....q;
-00000110: f63c d53c 9fa3 a23e 3232 a9be 43e0 733e  .<.<...>22..C.s>
-00000120: 20d2 6b3e 84a0 ddbd d2e7 b63d 25d8 cc3e   .k>.......=%..>
-00000130: f80b 543e c5ea 22be a6b5 f23e 11c2 cb3e  ..T>.."....>...>
-00000140: e302 1a3e 8a37 21bf fbf3 07bc 37a8 d2be  ...>.7!.....7...
-00000150: 1bda 77be 9b71 a73e b572 013f d164 623d  ..w..q.>.r.?.db=
-00000160: 7554 f03e 7115 08bf ace2 d73d 5830 bcbe  uT.>q......=X0..
-00000170: 9f42 b8be b93a 8f3c a5ae cabe ba70 d73a  .B...:.<.....p.:
-00000180: 1eda 3e3c 5ba7 6abc 1de6 f2bd 3394 f7be  ..><[.j.....3...
-00000190: 8da4 e93d e868 4e3e 3f9a 12be 1d76 b13d  ...=.hN>?....v.=
-000001a0: 4312 9b3d b2a5 d73e 6624 053e 519d cb3e  C..=...>f$.>Q..>
-000001b0: 8aed a8be e486 9b3e 0e7c bfbd 08db 2a3e  .......>.|....*>
-000001c0: c8e4 a03e a497 dcbc 276e d6bc c5c0 5c3e  ...>....'n....\>
-000001d0: 82ad 453e 0d7b fc3c 9ca8 40bd 8c1d 2a3d  ..E>.{.<..@...*=
-000001e0: c679 873e 62b9 cc3a 55cc 273e ba66 253b  .y.>b..:U.'>.f%;
-000001f0: 1eee b1bd 0ce5 ea3e 2f76 1f3e 7344 fe3e  .......>/v.>sD.>
+00000000: e28f 84bc 25f1 2c3c 6678 d43c e3f7 b53c  ....%.,<fx.<...<
+00000010: 9bea 013d d0b8 9a3a 6f60 ab3b bb66 063d  ...=...:o`.;.f.=
+00000020: 5d71 b4bc e103 0ebd 2a39 5e3c 0390 c7bc  ]q......*9^<....
+00000030: 7770 b4bc 9e88 d03b 7639 bd3c 29a9 5a3d  wp.....;v9.<).Z=
+00000040: d9c7 8f3c a8a8 83bc 77c8 4e3d 19db a83c  ...<....w.N=...<
+00000050: b697 57bc a632 debc bb3b 8cba 6528 0dbc  ..W..2...;..e(..
+00000060: b741 123c f097 79bc fe96 743d 7523 2abc  .A.<..y...t=u#*.
+00000070: 2adf c33b 9108 b33c 83b9 a3bc 71ef da3c  *..;...<....q..<
```

##### archive/data/4

```diff
@@ -1,8 +1,32 @@
-00000000: b67d 41be a003 f8bd d899 e8bd 8be1 30be  .}A...........0.
-00000010: 748d b5bd a91d 5abb 7ea9 9cbd 2798 213e  t.....Z.~...'.!>
-00000020: a80d 253e bce9 ea3d cda2 08be a514 1fbe  ..%>...=........
-00000030: f0fc 87bd 27e4 cebd e8a4 11be be27 c13e  ....'........'.>
-00000040: 4636 7f3e 0d45 9d3c 6a35 97bd 573f 2b3d  F6.>.E.<j5..W?+=
-00000050: d002 483e cbf8 833e fda5 21be b4d5 87be  ..H>...>..!.....
-00000060: 6b49 ce3d f3fc 803e 7ada 53be 4ca9 85be  kI.=...>z.S.L...
-00000070: 45f8 043e 860d 143e 4802 1b3e 2ab3 2e3e  E..>...>H..>*..>
+00000000: 709b 863d e899 8ebe 403d f2ba 6e39 fd3c  p..=....@=..n9.<
+00000010: cb84 c13e cb22 3fbc e8cb 17be 8b13 f4bd  ...>."?.........
+00000020: 3928 51bf f945 2a3d 30dc 0fbe 2caa ad3e  9(Q..E*=0...,..>
+00000030: 5291 b03e f0d2 b1bb c141 1b3f e5eb 2e3e  R..>.....A.?...>
+00000040: ceff 793e ce3b 70be c722 1f3f ee73 533e  ..y>.;p..".?.sS>
+00000050: aa82 87be 15a7 c3be 7333 353f d186 343d  ........s35?..4=
+00000060: 4761 973d 71d5 ba3e b36b f83e 726b 0e3e  Ga.=q..>.k.>rk.>
+00000070: 4753 043e 0295 8b3e a751 aebd 2b91 91bc  GS.>...>.Q..+...
+00000080: 00b1 c93e 7aa4 723d 7b30 e63e a1b7 e43d  ...>z.r={0.>...=
+00000090: 96bf cabe dfa9 c73a e62f f1bd 9a2a 5dbd  .......:./...*].
+000000a0: 5dff 20bf 9316 94be 7280 35bf e6bb 193d  ]. .....r.5....=
+000000b0: ebd8 293e 30d5 d7bd c78d 35bf 256d e1bd  ..)>0.....5.%m..
+000000c0: 8980 663e c599 cbbd 8a88 083f 4971 3f3e  ..f>.......?Iq?>
+000000d0: 87d6 98be 6038 68bd ebed c1bc 7d86 083e  ....`8h.....}..>
+000000e0: 5da4 eabe 856d 8dbd 82f6 2dbf f632 a73e  ]....m....-..2.>
+000000f0: 9965 edbd 3df3 82be 3fb5 76be daab 95be  .e..=...?.v.....
+00000100: ecbf e43e 3af6 48bd e49b 653f 1d74 373d  ...>:.H...e?.t7=
+00000110: 26b0 283e 9c85 c2be 1f25 ef3d ed94 a2be  &.(>.....%.=....
+00000120: e698 58be ae29 1ebd 9c55 b0be 95fc 3ebd  ..X..)...U....>.
+00000130: 013c bfbe 414e f3bd a083 0ebf b685 6bbe  .<..AN........k.
+00000140: cb20 0bbf 5533 a1bd 90bd 82be 277c c1be  . ..U3......'|..
+00000150: 2d90 87be 7e00 373e 11df 47be 5e65 05be  -...~.7>..G.^e..
+00000160: 1989 95be 14b5 8e3d 462f 25be 9151 b73d  .......=F/%..Q.=
+00000170: 08e8 c9be 92d4 3b3f d08d 963e 89d5 553e  ......;?...>..U>
+00000180: 185e 1a3e b6a9 ff3c 8dde 513c 2102 ee3e  .^.>...<..Q<!..>
+00000190: f8e3 413e da28 863e e4ef 113f 20a9 cf3e  ..A>.(.>...? ..>
+000001a0: c9e2 2d3f 13c6 ac3c 8c61 82bd 6da2 9abd  ..-?...<.a..m...
+000001b0: 2517 fc3e 9714 a23e 18fd 623e 40e7 793e  %..>...>..b>@.y>
+000001c0: e86c 65be ebc4 a53d 679f 373f d758 0dbe  .le....=g.7?.X..
+000001d0: 9d6d 8dbe 981f ae3e ba02 e73a 9655 8c3e  .m.....>...:.U.>
+000001e0: 5369 bf3e d8ed 973e ec35 2e3f 6f21 043e  Si.>...>.5.?o!.>
+000001f0: 6e01 9a3d ad0d 8dbe 2e37 23bf a956 b5be  n..=.....7#..V..
```

##### archive/data/5

```diff
@@ -1,256 +1,8 @@
-00000000: 1d31 143f 237f 483d 480d abbd 88b5 e83c  .1.?#.H=H......<
-00000010: 42eb 713e 5211 b33d d33f 213d 435f 0a3e  B.q>R..=.?!=C_.>
-00000020: 2ee7 3bbf 66cf efbe 1386 8c3e 89b1 8c3d  ..;.f......>...=
-00000030: 8fb9 053f a208 4bbd 8c73 c3be df8a 45be  ...?..K..s....E.
-00000040: 3b81 843d fb27 25be 9a64 873e f923 01be  ;..=.'%..d.>.#..
-00000050: 9d2a 58bf 2283 8abc ab28 14be ce64 733e  .*X."....(...ds>
-00000060: 02f4 3cbe 0e23 523e 158c 2f3f c684 913e  ..<..#R>../?...>
-00000070: 643e 15bf f093 08bf d040 14bf 9395 e83d  d>.......@.....=
-00000080: 9a66 f3be 53b4 a23e 704c c2be 838a cabe  .f..S..>pL......
-00000090: cb58 49be 261e 9dbd dd52 83bd f5ea 863d  .XI.&....R.....=
-000000a0: 15f0 d23d 02ac a83d 6bf3 22be f29d a5bd  ...=...=k.".....
-000000b0: 69c1 3bbc 1d00 3cbe 2a17 75be 8f5d 1d3e  i.;...<.*.u..].>
-000000c0: dbb7 bbbd f88b 123e eca7 5fbe afc6 7e3d  .......>.._...~=
-000000d0: fb2c 32bf 8e67 2a3e e146 88be 2db9 21bc  .,2..g*>.F..-.!.
-000000e0: 3511 ed3e 993b 123c 0ed2 803e 11c9 b83e  5..>.;.<...>...>
-000000f0: 4379 debe 07d4 1ebe 61fd 97be 3614 d73e  Cy......a...6..>
-00000100: b738 5abe 2d5c 85be 0cc4 84be 3d9d cc3e  .8Z.-\......=..>
-00000110: c082 793e 8f55 633e b103 3d3d 19bf 5c3d  ..y>.Uc>..==..\=
-00000120: 8bf0 703e 5d82 bf3e e84e 683e c03a 143d  ..p>]..>.Nh>.:.=
-00000130: 095c 1dbe 474c 7dbe fa11 e1be b6ea 94bd  .\..GL}.........
-00000140: d029 953e 114e c23a ae3d 1e3c 6743 353e  .).>.N.:.=.<gC5>
-00000150: 1461 fa3d 49e0 d43d 0a07 273f 463f 7f3d  .a.=I..=..'?F?.=
-00000160: 734d 093e 496c ce3e a13d 42be 6115 b53d  sM.>Il.>.=B.a..=
-00000170: 392e 4c3e 2512 283f 45a7 273e cf75 cd3d  9.L>%.(?E.'>.u.=
-00000180: e02f 8fbe 2db8 dc3d 4f47 fabc dd2f f4bd  ./..-..=OG.../..
-00000190: 9e51 5dbe b0e9 c63e dcdf aabe 9183 d5bc  .Q]....>........
-000001a0: 6993 b93d 67ab 7a3c 65bf 863d 97d2 d2bc  i..=g.z<e..=....
-000001b0: 97a7 bd3e d130 59be 1213 7f3e 48d1 89be  ...>.0Y....>H...
-000001c0: 62df 66be 538b 05bf a131 3a3f ea3c e63e  b.f.S....1:?.<.>
-000001d0: 694f d3be 2c1d 42be f28d 24bd 8cd8 903e  iO..,.B...$....>
-000001e0: 21e3 c2bc 67c1 89be 59e5 833e d775 3b3e  !...g...Y..>.u;>
-000001f0: 9430 f03e 7082 a83e 4b72 30bc 7249 17bd  .0.>p..>Kr0.rI..
-00000200: 0299 be3b ddf3 cc3e a326 663d 7254 2c3e  ...;...>.&f=rT,>
-00000210: edb8 2fbe 57cb 7c3e 0273 b53e bd40 b4be  ../.W.|>.s.>.@..
-00000220: cdca 91be e4de 103f 555b d0be 59c9 8d3e  .......?U[..Y..>
-00000230: 2e9c 54be 9c9e 1f3e 28b3 07bf c84e 34bf  ..T....>(....N4.
-00000240: a69c 513d f76a b0be dac4 07bf 44ef 92be  ..Q=.j......D...
-00000250: 219f 2a3e 013e 69be b7f1 78bc c66f ba3d  !.*>.>i...x..o.=
-00000260: 23e8 1fbe 291d 30be d9b9 1abe f1ad 9f3c  #...).0........<
-00000270: cf1a 4b3e 9c12 01be 256c 2c3d 4400 b7be  ..K>....%l,=D...
-00000280: 7f49 773e 6a0b df3c d659 16bf 7a07 f9bd  .Iw>j..<.Y..z...
-00000290: 53b0 ec3d 98db c53e 78cf 02be 6b1b a5be  S..=...>x...k...
-000002a0: 3c53 bdbd c685 7abd 0d03 38be d205 e7be  <S....z...8.....
-000002b0: 7642 f1be fa02 093f 7bb9 89be 3d36 253d  vB.....?{...=6%=
-000002c0: 7fbb 4e3e 0055 0cbd 5251 e7bd 2b25 ddbe  ..N>.U..RQ..+%..
-000002d0: 9f33 ce3d dfbd 6cbe b6c3 843d a075 dd3e  .3.=..l....=.u.>
-000002e0: 0005 863e 26cb b63b 70a2 44bf 7f29 263e  ...>&..;p.D..)&>
-000002f0: 0e4a 8fbe c474 00bd e430 bebe f96b 28bf  .J...t...0...k(.
-00000300: cd5c 59be 945f 5c3d ad9f 163d 9eb9 7dbe  .\Y.._\=...=..}.
-00000310: a110 7a3d 8d68 713e 7dfa acbe 9c66 6bbd  ..z=.hq>}....fk.
-00000320: 6334 72bd 6bfa 803e 14d5 623e 9b6b e63e  c4r.k..>..b>.k.>
-00000330: 53f8 10bd e597 82be 498e 4ebd ba6c f13d  S.......I.N..l.=
-00000340: 346d a1bb ffd1 82be f7e7 96bb 0d0f ecbe  4m..............
-00000350: af54 0e3f 9961 ecbe 7c92 c23d bb31 c0be  .T.?.a..|..=.1..
-00000360: a6f8 1fbb 1af9 25bd 9a92 14bf 990f cabe  ......%.........
-00000370: 85e0 a3be 2c42 ec3e 5049 52be 2770 623e  ....,B.>PIR.'pb>
-00000380: 9764 d63d a4d1 713d 12e9 df3b 0794 ec3c  .d.=..q=...;...<
-00000390: a0a7 fdbd 1b10 4ebd a9cb 24be 7fad af3e  ......N...$....>
-000003a0: 9ec5 9fbe c8fc 3c3e 0a45 d0be cc56 b6be  ......<>.E...V..
-000003b0: 8673 91bb dcd6 23bf ff7e 91be c98b b1bb  .s....#..~......
-000003c0: 327b fabc f47f b83e cd4a 7e3d b6c8 cdbd  2{.....>.J~=....
-000003d0: 1d3e e43d e155 9a3d 3443 cebe 8837 803e  .>.=.U.=4C...7.>
-000003e0: de75 063f 6c89 063d c328 e6be 9729 9fbe  .u.?l..=.(...)..
-000003f0: b2dd dd3d 0f88 ab3e 5fc8 683e 4fd2 7a3c  ...=...>_.h>O.z<
-00000400: 79da 03bd 940a e03e fde7 57bd a16d f73e  y......>..W..m.>
-00000410: 0c7d 0a3c 2a9c ba3e a383 9bbd 8abf 793d  .}.<*..>......y=
-00000420: 7c6f 02be 2aca 11bf 3d3e 003f d32e 1a3f  |o..*...=>.?...?
-00000430: 34bf 4ebe 8035 fe3d 9bec 4a3e 7733 1abe  4.N..5.=..J>w3..
-00000440: f905 1abe cf82 433e 3aab 92be 6a04 593e  ......C>:...j.Y>
-00000450: 3694 89be 9a01 94be 8d44 e5bd a5cc fd3d  6........D.....=
-00000460: 5b3f 5f3e 456f bf3d 1290 a7bd 7859 70be  [?_>Eo.=....xYp.
-00000470: 6ca8 863d f447 c1be 66ba 2f3d 1e40 69be  l..=.G..f./=.@i.
-00000480: 8afc 53be 3b41 b9be 871c b6bc c887 1e3e  ..S.;A.........>
-00000490: 357f 18bf aaae 8f3e 4428 f3bd 92fe 933d  5......>D(.....=
-000004a0: 95d0 923e 72fb 6abe 45f6 ed3d 7aad 0abf  ...>r.j.E..=z...
-000004b0: f4d5 273f 4e28 14bf 2428 3fbd 108f 98bd  ..'?N(..$(?.....
-000004c0: fb97 74bb 8a42 2ebe 80ee ab3c 5f03 8abd  ..t..B.....<_...
-000004d0: 8796 ecbe 05d6 163d ba3a 3bbe 3794 4cbe  .......=.:;.7.L.
-000004e0: 8df7 9ebe 9421 3a3e d95f 9cbe 3b8b 9f3d  .....!:>._..;..=
-000004f0: 642b fa3c 3714 6abe fae8 3e3e caab 5b3f  d+.<7.j...>>..[?
-00000500: 95bb bcbd d6d6 01bf 6e41 af3d 1e3f b83d  ........nA.=.?.=
-00000510: 8980 78bd 4f7c 9d3c 4e09 25bf 2234 b63e  ..x.O|.<N.%."4.>
-00000520: 6735 8c3d 3d56 3abe 8c26 fabe 32a0 ee3c  g5.==V:..&..2..<
-00000530: 5489 0fbe 0a5a 4e3e bf13 74be eeed 3f3c  T....ZN>..t...?<
-00000540: 3a80 d4bc 8e10 9cbd c9fc 12bd d4d4 d6bc  :...............
-00000550: b135 abbd 92e1 c6be 933d d1bb 0571 c6be  .5.......=...q..
-00000560: d91c 2a3d f95a cebd ccb4 dd3d b27e d93e  ..*=.Z.....=.~.>
-00000570: edb2 963e 305b 19be f466 fdbc eef0 583e  ...>0[...f....X>
-00000580: eaf9 dfbc df33 203e 2e5a 11bd a108 30bc  .....3 >.Z....0.
-00000590: bce0 833e 102f c2bd 5f6e 84be b171 0c3e  ...>./.._n...q.>
-000005a0: bedd 22be 3431 323d e8b0 113e fd6b 003e  ..".412=...>.k.>
-000005b0: 16d6 9a3d 72fc 8dbe 986d ca3c e4e8 4d3e  ...=r....m.<..M>
-000005c0: 1ec9 1c3f ac6d dfbd 5f6a 09be 560c bebd  ...?.m.._j..V...
-000005d0: dcac 9abe 21fa a83e c50f 0d3f f890 96be  ....!..>...?....
-000005e0: b4ec 443c 511c abbe c8ed fcbd 097d 9fbe  ..D<Q........}..
-000005f0: 8a58 063e a61e 16bf 6c96 0e3e 6906 e6be  .X.>....l..>i...
-00000600: 6568 50bd f41f d1be 4869 a03e ea79 c73d  ehP.....Hi.>.y.=
-00000610: 8a11 ebbd 7a72 1d3d 4651 52be 8471 1abf  ....zr.=FQR..q..
-00000620: 2c9e e93d 5137 d93c 1ec8 113a 7978 a83e  ,..=Q7.<...:yx.>
-00000630: d05f 8fbe 2deb 9dbd e8dc ffbe 0fbe 323e  ._..-.........2>
-00000640: 5f84 a2bd 927f 8fbe f464 413e 5d7b 15be  _........dA>]{..
-00000650: 8ddb 583e 10fe fc3d d70e 12be 5e79 8f3e  ..X>...=....^y.>
-00000660: ba06 ff3e 50d5 ce3d 3739 43bc b71c e0bd  ...>P..=79C.....
-00000670: ee1c b1be 5765 a6be 93cd b43e 8e42 b1be  ....We.....>.B..
-00000680: 225d a33e 5602 4d3e cb67 233e 86a9 d83b  "].>V.M>.g#>...;
-00000690: 4152 97bd 6e56 98be c421 333c 203e 21be  AR..nV...!3< >!.
-000006a0: a76a 14be 5aea 1d3e edbc 463e e4e6 163d  .j..Z..>..F>...=
-000006b0: da6a e2bd 3a00 e2be 2ee2 c23e 521a c23d  .j..:......>R..=
-000006c0: 82ce f4b8 c0b8 89bd 98b3 f0bd 7691 9e3a  ............v..:
-000006d0: 4b7c a7be a0b8 9abe 82c9 303e 08a1 133e  K|........0>...>
-000006e0: dd2f 473e 8890 9d3e 8ecb 253d 655d 3d3f  ./G>...>..%=e]=?
-000006f0: 4f59 84bd 3a90 f5be e9df b3be 4324 103d  OY..:.......C$.=
-00000700: 1775 823e 7ce4 84be f7d1 bcbe 3303 0cbf  .u.>|.......3...
-00000710: b363 9abe 2f83 92bd c0b5 523d 71c4 993e  .c../.....R=q..>
-00000720: 6732 3b3e 40d2 0f3e b1d2 0ebb 560d ea3e  g2;>@..>....V..>
-00000730: 9bd7 343d fa0b 033f 9832 f0be f992 1ebc  ..4=...?.2......
-00000740: 6031 823e 9bd6 bc3a 1a0f cbbe c830 e3be  `1.>...:.....0..
-00000750: bc5c 9c3c cf04 62bd 07dd d83d 4593 383f  .\.<..b....=E.8?
-00000760: 4746 133f aa97 17be 9afe 8bbe 182e 19be  GF.?............
-00000770: af0c afbc 6d15 593b aaeb f1bd 1799 113e  ....m.Y;.......>
-00000780: 14b0 0a3d 8035 90bd 3506 c53b efdb 9abd  ...=.5..5..;....
-00000790: 0ae2 07bc a311 f53c 64f5 883e d473 4dbd  .......<d..>.sM.
-000007a0: 3374 bbbe 39e0 4bbf fda5 acbd bb41 2d3e  3t..9.K......A->
-000007b0: 9f80 923d 4ec1 17bf 69d9 513c 229a 133e  ...=N...i.Q<"..>
-000007c0: b3a0 13bf 20cc 4e3e 8611 51be 50c1 b0be  .... .N>..Q.P...
-000007d0: 0772 07bf 2daa 10bd 104a 073f ef5c 183f  .r..-....J.?.\.?
-000007e0: e256 b8be 0a40 b8be df9f 053f d804 453e  .V...@.....?..E>
-000007f0: e142 0fbd 523a c9be f06c 0ebf 0722 4bbe  .B..R:...l..."K.
-00000800: 1866 c83e 6e11 8abd cc70 133e ce35 6b3e  .f.>n....p.>.5k>
-00000810: cd8c e1be 419f 9d3d c429 b3be 20bd 8f3c  ....A..=.).. ..<
-00000820: ac70 db3e c9ad 223e bcb3 6a3e 8ea9 c6bd  .p.>..">..j>....
-00000830: 2bc6 32be ff5d 5b3d 72d8 16bd 7386 87be  +.2..][=r...s...
-00000840: 4a03 37bd 2c3e d23e 2bcd 19be 7fc9 903d  J.7.,>.>+......=
-00000850: 181b 31be fb56 14be d1c4 223d 1636 5b3e  ..1..V...."=.6[>
-00000860: a977 b3be d8d5 2bbe 59d7 623d c674 953b  .w....+.Y.b=.t.;
-00000870: ce9f 95be 4f3a e23d 539f a63d 18fa 093c  ....O:.=S..=...<
-00000880: 21f9 e93d f44e 163e cbc2 c8be 1c70 33be  !..=.N.>.....p3.
-00000890: b0b5 413d b5f1 f6bd fb85 bbbe cfe8 e13d  ..A=...........=
-000008a0: 81d8 433c 4b63 88bc 27b8 063f d470 37be  ..C<Kc..'..?.p7.
-000008b0: e210 babe 9904 66be 457e 06bf 506f 1dbd  ......f.E~..Po..
-000008c0: 8dd8 86be 22cf 09bd b7ba 083e 1f16 a5be  ...."......>....
-000008d0: 8f85 ab3d 3415 a13e 15af f0be c2a4 28be  ...=4..>......(.
-000008e0: f961 49be c942 36be 6a0d 0a3e f4cd 763e  .aI..B6.j..>..v>
-000008f0: 6209 003f 4f10 3f3d 26c5 dd3d 45ce c53e  b..?O.?=&..=E..>
-00000900: a67a 643e 4226 71be 5643 ce3e 02d6 b73d  .zd>B&q.VC.>...=
-00000910: 3ea1 763e 6b3e f53d 154f 523e 0710 7d3e  >.v>k>.=.OR>..}>
-00000920: 05bb 61bf dbe2 7dbe e6b3 493e c0e9 9d3e  ..a...}...I>...>
-00000930: 489d b93d 1f3b 21be 8007 bc3e e573 a2bd  H..=.;!....>.s..
-00000940: 8991 f0bd f32a 0c3e e745 4e3d f4ce 32be  .....*.>.EN=..2.
-00000950: ce5a abbf 3630 a93e 9663 81be eb45 063f  .Z..60.>.c...E.?
-00000960: 65f2 4cbe aa02 3bbf 8629 113e 6abe 753f  e.L...;..).>j.u?
-00000970: 11d3 d0be a769 98be f14a 8dbe a34c 823e  .....i...J...L.>
-00000980: ede7 8f3e 5f5a 933e f8aa 8bbe 2737 39bc  ...>_Z.>....'79.
-00000990: 98e6 ae3c c07d 0f3f 60b2 e43d 6628 bc3d  ...<.}.?`..=f(.=
-000009a0: b61f 7c3f 8961 283f 59ca 05bf bdd3 ae3e  ..|?.a(?Y......>
-000009b0: d200 2cbe 9361 6e3d e84b 03be 7e17 383f  ..,..an=.K..~.8?
-000009c0: f937 89bd c075 0fbe 1fc3 643e efce 9bbd  .7...u....d>....
-000009d0: e695 413f 0834 033e 6f63 92bd 68f7 9fbe  ..A?.4.>oc..h...
-000009e0: 15e4 01be ee8b c33e 4b7a 0ebf 7c8c a6be  .......>Kz..|...
-000009f0: 9473 a63e 2b18 753e 4840 083f 1949 debc  .s.>+.u>H@.?.I..
-00000a00: 8a90 32be 683f a53e 7084 c13e 93f4 8b3e  ..2.h?.>p..>...>
-00000a10: 18fb b7be 2371 d23d 7d46 663e a3c0 ec3e  ....#q.=}Ff>...>
-00000a20: 2118 03be b2d6 843e b8a7 303e d1b8 85bd  !......>..0>....
-00000a30: 9646 31be 3a38 c93e 5850 cc3c 49e8 abbd  .F1.:8.>XP.<I...
-00000a40: f59b 92be b5a5 5f3e 1c22 113f 6839 cbbe  ......_>.".?h9..
-00000a50: a341 0a3e 1993 563c 6a1d 173f 8a05 5dbe  .A.>..V<j..?..].
-00000a60: 2d70 d73d fa84 173e 3a68 943d 504d b2bd  -p.=...>:h.=PM..
-00000a70: a817 b7bd dc78 6dbe f12a 883c 339a e0be  .....xm..*.<3...
-00000a80: 099b 79bd 624b c3bd 464c 9b3e 5c87 4e3c  ..y.bK..FL.>\.N<
-00000a90: d7c7 46be 5bf9 113f 3b74 6a3b 4888 8c3e  ..F.[..?;tj;H..>
-00000aa0: 79ef 5b3f c03d bb3e 42a6 97be 42e1 06be  y.[?.=.>B...B...
-00000ab0: 79e9 1abf 023c 08be 1cc3 0abd 9508 3b3e  y....<........;>
-00000ac0: 83c6 143f a85d 71be 67fb dabd b1fa 183d  ...?.]q.g......=
-00000ad0: 7f1a 3e3f c446 4a3e 8f37 98be 7e49 00bf  ..>?.FJ>.7..~I..
-00000ae0: 3abf 423e bd01 aa3e bad5 9d3c 7f77 2dbf  :.B>...>...<.w-.
-00000af0: 94fd a03e e420 303f ba75 78be 8f1f 5cbe  ...>. 0?.ux...\.
-00000b00: e7fe b1bc 68b1 48be fc35 bf3d e4fc 8ebe  ....h.H..5.=....
-00000b10: 5fb9 443e 4f5f c53d 949d 3cbe bc14 a23e  _.D>O_.=..<....>
-00000b20: 9467 133f 8b63 ad3e ad32 54be 36db 863e  .g.?.c.>.2T.6..>
-00000b30: 6e48 b13d c2d0 48bd 7d5c c7be f52c a6be  nH.=..H.}\...,..
-00000b40: 657f 9fbe b58a d33d dcac 3cbd de84 ec3e  e......=..<....>
-00000b50: 36ca 403f ec91 2d3e ada4 17be 9b27 aabe  6.@?..->.....'..
-00000b60: a8de 693d 537b e13e c54c 30bf f164 0dbe  ..i=S{.>.L0..d..
-00000b70: ebdf 513e 6ba1 1c3e b6d7 6abe d5f8 c3be  ..Q>k..>..j.....
-00000b80: 3730 29bd eb61 ed3e 5419 443e c476 633e  70)..a.>T.D>.vc>
-00000b90: b74d 363c b060 babe 3449 debe 4164 49be  .M6<.`..4I..AdI.
-00000ba0: 2962 243d e01d d5be 40cf b5be 9af6 ad3e  )b$=....@......>
-00000bb0: 1ec5 033d b52b 753e 9459 6c3e fd6e aebe  ...=.+u>.Yl>.n..
-00000bc0: 72b3 8a3d cb3b 80bd 747a df3c c1fc ecbe  r..=.;..tz.<....
-00000bd0: 7a5d 90be cedd 093f 8ae4 413e 7049 193e  z].....?..A>pI.>
-00000be0: c773 3bbe 4bea b23e 2163 8abd 0679 f73d  .s;.K..>!c...y.=
-00000bf0: 8fda 0ebe b945 913e 2362 1dbd 4a8c ddbd  .....E.>#b..J...
-00000c00: 0995 debd 5484 8c3e 6b43 a4bd 08a7 44be  ....T..>kC....D.
-00000c10: 7c83 0e3e 01ce 6f3d 6bf9 cd3e b962 c3bd  |..>..o=k..>.b..
-00000c20: 2965 6f3e c504 fbbe e4e4 aabd 1fe0 b83e  )eo>...........>
-00000c30: 3409 b3bb 8335 f8bd 5581 6dbe 80b8 96be  4....5..U.m.....
-00000c40: 8dd3 f53e bdc2 f63e 6f00 733e 6f6d 2fbe  ...>...>o.s>om/.
-00000c50: 0979 313e 2173 9fbe b730 583d 5855 dcbd  .y1>!s...0X=XU..
-00000c60: 09e2 473c 0b42 a9be 992c a3bb dc91 c53e  ..G<.B...,.....>
-00000c70: 4666 e5be b005 c1bc 850e 853e be10 e2be  Ff.........>....
-00000c80: c59f bfbd d19e 21be ff2d 5bbe 9e37 f63c  ......!..-[..7.<
-00000c90: 3e50 663e 74eb f8be 70bb 673e fbef 28be  >Pf>t...p.g>..(.
-00000ca0: c48e e5bd d039 8b3e 31d5 0fbe f73b b33e  .....9.>1....;.>
-00000cb0: 8811 f8be 9d48 023e 6a1b 46be 7970 7abd  .....H.>j.F.ypz.
-00000cc0: 3af0 d8bd 590a 403e 1755 5c3e e363 0bbe  :...Y.@>.U\>.c..
-00000cd0: 7ade 41bf b51c d9be a3bd b4bd 858b a93d  z.A............=
-00000ce0: 6f1e babe eaef 4c3c 17f1 23be 7ebd d0be  o.....L<..#.~...
-00000cf0: fdbd 4bbe d3ad 813d 9070 03be 3fba fcbe  ..K....=.p..?...
-00000d00: cc7c c7be 0bd2 64be 8326 bebe ae1c c83d  .|....d..&.....=
-00000d10: 5c24 a73d af7a 4c3e c529 97be b3bd f23e  \$.=.zL>.).....>
-00000d20: 7b5c 903d 725a 9d3d 2975 70be 38ab 47be  {\.=rZ.=)up.8.G.
-00000d30: a3cd 43be 6041 babe 14da 923e b07b 9dbe  ..C.`A.....>.{..
-00000d40: 895a 16be 0bf4 82be d82c 313e a0ba c83e  .Z.......,1>...>
-00000d50: 034e 6d3e 763b ab3e 0456 bcbd 6ec7 483e  .Nm>v;.>.V..n.H>
-00000d60: 9c77 91be cb70 3bbd 7568 5a3e 4786 93bd  .w...p;.uhZ>G...
-00000d70: f609 d0be 8308 c3be 70a0 e13d 3a03 5f3f  ........p..=:._?
-00000d80: 7efb b0bd d36c 02be 6d50 9d3d ce30 06be  ~....l..mP.=.0..
-00000d90: 80ba c53d 59a3 c73d 9e27 773d 0a99 09bf  ...=Y..=.'w=....
-00000da0: 541a e03d aa0c 103e d6e1 9e3d 254d a13d  T..=...>...=%M.=
-00000db0: 40d9 04be 5753 d93d b0b6 963e 83a5 c7be  @...WS.=...>....
-00000dc0: 8ea1 183e 1262 083f a0a2 a73e 6b39 93be  ...>.b.?...>k9..
-00000dd0: 3da4 a4bc b87c 773e 2551 ddbb 2685 713c  =....|w>%Q..&.q<
-00000de0: e663 eb3d 91f4 6bbd 6172 cfbc 4d2d f0bd  .c.=..k.ar..M-..
-00000df0: fc3d a73e f6e8 d7be ea62 f8be c56b d83d  .=.>.....b...k.=
-00000e00: 9976 f83e 70a7 27be 12cf 22bf cbbb dd3e  .v.>p.'..."....>
-00000e10: a5b8 a6be 8faf 61be 0a31 2f3e dd95 053d  ......a..1/>...=
-00000e20: 6d76 e03d 0d22 9d3c 37c9 5bbe 1c1e ad3e  mv.=.".<7.[....>
-00000e30: 279c d2bc bf53 25be fe44 b23e 0aba a5be  '....S%..D.>....
-00000e40: aab7 7c3d 0ce0 29be 1325 913e 91bf febd  ..|=..)..%.>....
-00000e50: 2e31 973e eba7 c8bd 2f92 d03c 0dd9 a8be  .1.>..../..<....
-00000e60: 7ace ac3e 6718 56bd 6743 ac3b 1e72 0bbe  z..>g.V.gC.;.r..
-00000e70: f6c1 8e3d 79be 883d b6de 28bd 63bf 4bbe  ...=y..=..(.c.K.
-00000e80: 14cd 1ebe 06a0 e9bd 023d 9ebc ca9f b1be  .........=......
-00000e90: 2f81 293e ade8 1bbc e616 8bbd 4419 d53e  /.)>........D..>
-00000ea0: b97c d33e c147 323e 25f3 2e3d 3adc 55be  .|.>.G2>%..=:.U.
-00000eb0: ebac 0ebe 4275 13be b411 883e 51eb 0fbe  ....Bu.....>Q...
-00000ec0: 97cc 4b3e 178d 8bbe a4f8 06be 0b53 bebe  ..K>.........S..
-00000ed0: 4f13 8b3e 6c33 abbe c70a 5fbe 7a4a 513e  O..>l3...._.zJQ>
-00000ee0: a41d 2ebd a16f fc3e 1930 d3bd 681f 1abe  .....o.>.0..h...
-00000ef0: 7b69 503e e369 953c 586c 003f 9110 b4be  {iP>.i.<Xl.?....
-00000f00: 4321 b73d a565 f73e f0e0 ea3e 50d3 2f3f  C!.=.e.>...>P./?
-00000f10: 5132 393f eb92 01be d25d fb3d f336 043d  Q29?.....].=.6.=
-00000f20: cdb4 493f 0cb4 1f3e fa0c 12be f2cd b6bd  ..I?...>........
-00000f30: 012d 80bd 38bf 343e 66ba 35bd f398 e8bd  .-..8.4>f.5.....
-00000f40: d5dc 88bc c3b4 83be 13e6 373e a4ea 32be  ..........7>..2.
-00000f50: ed87 b33e 349a d5be ef91 9b3e b0d1 97bd  ...>4......>....
-00000f60: f3f0 c53e dda8 70be 72cf 2dbe ee58 e3be  ...>..p.r.-..X..
-00000f70: 2944 793e e0c1 823d 094d f2bb c91b d8bd  )Dy>...=.M......
-00000f80: 8ac9 afbe e9a8 34be d819 8dbe d421 d43e  ......4......!.>
-00000f90: be81 713e 1f09 f03d 526c 3dbe 6e6c 9dbd  ..q>...=Rl=.nl..
-00000fa0: 7a36 74be 1249 3c3e a13c 443e d892 8e3d  z6t..I<>.<D>...=
-00000fb0: 3398 223f 765e e93c e312 9c3e 0a5e f93c  3."?v^.<...>.^.<
-00000fc0: 71b5 5dbe a041 d13e 73d5 87be 6329 d6be  q.]..A.>s...c)..
-00000fd0: c178 afbe 8d1c 643d 41f8 99be 7310 1b3e  .x....d=A...s..>
-00000fe0: 60ec 69bd b6a8 20be b561 223f 8f60 d13e  `.i... ..a"?.`.>
-00000ff0: ec82 5ebe 2053 11be c26d 37be 70a2 9ebe  ..^. S...m7.p...
+00000000: e437 083d 7a34 253e 4dec afbd 18e9 59be  .7.=z4%>M.....Y.
+00000010: 1dec bebd 62bc c13d ac74 16be c561 3fbd  ....b..=.t...a?.
+00000020: 138a c4bd a5ce 0d3e be84 a3bc 5d80 333e  .......>....].3>
+00000030: 3ff3 063e c6b0 423e 246c d43d ef10 243e  ?..>..B>$l.=..$>
+00000040: fede fdbd c4d7 a8bd 06e0 b63d 49df b7bd  ...........=I...
+00000050: a320 f3bd 43fd 94bd 4984 a03d 3143 bc3d  . ..C...I..=1C.=
+00000060: 6619 8dbd e99a 80be 6ce9 1e3e 0914 dfbd  f.......l..>....
+00000070: 64b0 afbd a2a6 dd3d 5839 ba3d 9b98 91bd  d......=X9.=....
```

##### archive/data/6

```diff
@@ -1,8 +1,256 @@
-00000000: 423e 8bbe 8bf6 c93d ffc4 dc3d c1cd bfbd  B>.....=...=....
-00000010: a364 acbd 347c 1d3d 57f3 ee3d 40c7 1f3e  .d..4|.=W..=@..>
-00000020: a78b f4bd 9059 c73d fc37 aa3d a1a9 91bd  .....Y.=.7.=....
-00000030: d512 6e3d bf84 04be a0c4 833d 1717 56be  ..n=.......=..V.
-00000040: 3b57 06bd cc78 113e 922b 79be 7b47 693e  ;W...x.>.+y.{Gi>
-00000050: 7fbd d9bd 137d 823e 150a 333e e8fc debd  .....}.>..3>....
-00000060: de28 eabd bfaf e2bd fc50 9f3d a95c ffbd  .(.......P.=.\..
-00000070: d71e 343d 8aad 193d c070 a2bd 10f6 e7bd  ..4=...=.p......
+00000000: 1db5 2ebe 6ea2 133e 6b9f a1bc 5a3f c2be  ....n..>k...Z?..
+00000010: 7a82 1abe be03 a13e aa4c d63c 2ef8 cb3e  z......>.L.<...>
+00000020: d7d4 cbbe dfb9 98be a191 e0bd ffa1 18be  ................
+00000030: 541e 223e a886 4c3e 80d4 d13d 51d9 9dbb  T.">..L>...=Q...
+00000040: 7293 943e 5165 a8be f7ef a1be ca99 16bf  r..>Qe..........
+00000050: 651a 88be 5d38 05be 91e8 003f 0fa3 363e  e...]8.....?..6>
+00000060: 3bbe 193d 97fd cdbe 4166 323d b0a2 92bd  ;..=....Af2=....
+00000070: ceba 4f3e 4d19 0d3f 13c5 ad3e ffe9 66bf  ..O>M..?...>..f.
+00000080: 66bd 263e eb01 13bd 7b98 b73e 7700 a1be  f.&>....{..>w...
+00000090: 8d77 a0be 0e17 98bc f6c2 ccbe 8aaa 22bd  .w............".
+000000a0: bb76 81bf db60 263f 0fbd 8a3e 867c 053f  .v...`&?...>.|.?
+000000b0: 7202 443d 03f9 9c3e f411 bf3e 67c6 a73d  r.D=...>...>g..=
+000000c0: 44f0 46bf ea1a d13e 0fe9 cf3e 9fba e33d  D.F....>...>...=
+000000d0: 9a2d 3f3d 7da2 8e3e f22c 8f3e 1031 62be  .-?=}..>.,.>.1b.
+000000e0: 453d c1be b2b4 a4bd 5529 f7ba 8691 8dbe  E=......U)......
+000000f0: 15cd 76be 993d 0f3f 14ed c63e f494 36be  ..v..=.?...>..6.
+00000100: 954c 90bd 9a11 ddbe 0ccf e53e 7aa5 b3bd  .L.........>z...
+00000110: 417a 19be 0e28 c63e b5b1 ca3d 39de 013f  Az...(.>...=9..?
+00000120: 8fa0 aebc 285e 683e b9bd cf3e 414c a6bc  ....(^h>...>AL..
+00000130: b61d 38bf dfff babd b4c6 873e ccfc 51be  ..8........>..Q.
+00000140: 7af2 29bf 1927 6e3c 6c3b f5bc 1081 383e  z.)..'n<l;....8>
+00000150: 3d92 913e f4d2 2cbd 1f6e b13d ce42 873d  =..>..,..n.=.B.=
+00000160: b6a0 5c3d 7355 9d3e 2da4 5ebf eb6f 463e  ..\=sU.>-.^..oF>
+00000170: 5a3e b03e 338a f4bd 8d39 f8be 3b76 dcbd  Z>.>3....9..;v..
+00000180: 822b 063e ede5 f3be a616 74bc 93cd 083f  .+.>......t....?
+00000190: 41bd ef3e 317e 3abf 638a 603e 5b94 033f  A..>1~:.c.`>[..?
+000001a0: adae 483f 7eb9 5abf 9cc4 fdbe e3f6 d2be  ..H?~.Z.........
+000001b0: 8c89 803e 7179 27bf 87b6 d5be ce30 36be  ...>qy'......06.
+000001c0: 8cde 013f c70e 8abe ca2e f4be c524 edbe  ...?.........$..
+000001d0: aec4 c7bd 6144 213e 5153 cbbe 359d 82be  ....aD!>QS..5...
+000001e0: 3b0d fc3d e5b4 a93e 5f47 90be ab33 803f  ;..=...>_G...3.?
+000001f0: 66f4 643d 4d40 e9be a732 013f d7c9 4e3e  f.d=M@...2.?..N>
+00000200: 9bd4 3a3d 7ab4 9fbe 5b55 98be 656c dabe  ..:=z...[U..el..
+00000210: ade2 5c3b 6014 0abc f248 26bf 8a88 90be  ..\;`....H&.....
+00000220: 1b70 d63d 949a 013f 45f1 a33e 96d3 393e  .p.=...?E..>..9>
+00000230: ced0 4bbd e716 433e 0db9 d73c 6acd 84bc  ..K...C>...<j...
+00000240: 0bda a5be 1a57 b63e 0eee 293d b96d 22be  .....W.>..)=.m".
+00000250: 953d 0a3f 7f07 633e 13aa ed3e fe2a 123d  .=.?..c>...>.*.=
+00000260: 4a6a 443e 8b49 e7be 038c 80be 78b7 14bf  JjD>.I......x...
+00000270: e2c8 b3be 2833 fd3e 0ba2 3ebd 3642 ed3d  ....(3.>..>.6B.=
+00000280: 2e9b e33e 40e3 553e 173a e3be d192 33be  ...>@.U>.:....3.
+00000290: cf05 de3d 69a7 a0bd d056 58be 65e0 44be  ...=i....VX.e.D.
+000002a0: ffab ee3d 90b0 49be 2029 1cbe 75fd a43e  ...=..I. )..u..>
+000002b0: 86fe f3bd 804d a0be eed4 953e ad8b 50be  .....M.....>..P.
+000002c0: 9822 d53e 382f 8e3e b3d5 003f f520 17be  .".>8/.>...?. ..
+000002d0: ca50 5fbe 63fe c8bd 66e5 e3be 114b 203e  .P_.c...f....K >
+000002e0: e9a5 8f3e d5f4 87be 2bc8 473e 529e a73e  ...>....+.G>R..>
+000002f0: f37d b43e e4e3 6fbd 4b03 f43e 0bc5 a1be  .}.>..o.K..>....
+00000300: b49b 8e3c 1a8c 76be daf0 10bf 03e0 32bd  ...<..v.......2.
+00000310: 7247 973e 4fa1 523e e3b9 323e 4c91 c73e  rG.>O.R>..2>L..>
+00000320: 10a5 c3bd 91f8 a5bd d708 27bf d4f0 f63d  ..........'....=
+00000330: 6dc9 113e 299f fd3e e237 1c3e 2c23 e6bc  m..>)..>.7.>,#..
+00000340: e44c 0dbe 321a 393e 8b5b 593d ebf6 debe  .L..2.9>.[Y=....
+00000350: 777f a3be a90f 593e 2826 0abe d38b 9f3d  w.....Y>(&.....=
+00000360: 5923 353e 7a59 4c3e b1df 9d3e 345b 69be  Y#5>zYL>...>4[i.
+00000370: 76c1 bc3e 0dd9 893e ebaa 68bd b013 523e  v..>...>..h...R>
+00000380: d975 913e 1cc5 ae3d ca15 b5be 764d 80be  .u.>...=....vM..
+00000390: 1437 a5be 6375 253e cf8e 763e 41eb 4dbd  .7..cu%>..v>A.M.
+000003a0: 2818 713e 0656 683d ac90 fdbe 813d 8a3e  (.q>.Vh=.....=.>
+000003b0: a3d1 063f ad9b ed3e 4447 2abe 38a9 5dbe  ...?...>DG*.8.].
+000003c0: a8ea b63e c177 e2bd eb98 68be f3e0 adbe  ...>.w....h.....
+000003d0: c087 9fbd f15a 88bd 2c50 d3be d7f6 953e  .....Z..,P.....>
+000003e0: 4ca1 38bd c4d1 803e 3c06 c23b 909c a23e  L.8....><..;...>
+000003f0: 7a1d 1dbf 3df0 b6be a2a3 bd3e 95d1 ddbe  z...=......>....
+00000400: c422 2a3e 3d97 bf3e 0b10 edbe bc3d 00bf  ."*>=..>.....=..
+00000410: 8fba 803d d665 0bbe 098f adbe 4ebc 303e  ...=.e......N.0>
+00000420: ff5c 8abe d231 1a3f 7b10 d13e ce0a 083f  .\...1.?{..>...?
+00000430: a020 31bd ae4f c63e 0cec eb3e 5f85 493e  . 1..O.>...>_.I>
+00000440: ee2b 37bf 7f88 823c 0d76 1d3f 3d5d a13d  .+7....<.v.?=].=
+00000450: 817c 783d 7983 6abe ef7a 993e ab01 e4be  .|x=y.j..z.>....
+00000460: 12ed d0be 476d 23bf a99d 043f 6e94 c3be  ....Gm#....?n...
+00000470: b031 25bf 4968 94be fd90 97be 4f59 263e  .1%.Ih......OY&>
+00000480: 2e2d 7dbe 4514 02bf d293 26be 57af 64be  .-}.E.....&.W.d.
+00000490: 76f0 e9be c39b 933e bcb6 793e 5d71 c1bc  v......>..y>]q..
+000004a0: 0e5a c63d e0da bc3e be85 2cbd d9f1 88bc  .Z.=...>..,.....
+000004b0: 1f7e bbbe 01fe d3be f1e8 293d 3335 3fbd  .~........)=35?.
+000004c0: 3e68 873d ec65 2cbe afb0 133f a0a3 4d3d  >h.=.e,....?..M=
+000004d0: bd83 a1be 27cc 6b3e edc8 1f3e 5a2b 80be  ....'.k>...>Z+..
+000004e0: 41b6 8dbe 080b 82bd 4e66 823c 3432 dbbe  A.......Nf.<42..
+000004f0: 6703 58be e026 793e e9d9 debd 3b84 17be  g.X..&y>....;...
+00000500: 0d41 373e 1ce7 edbd f03c 483e 18b6 0fbe  .A7>.....<H>....
+00000510: 61c1 ab3e 96d5 ce3e 744d b8bd 8880 85bd  a..>...>tM......
+00000520: 4101 7bbe f8cd bc3e d722 013f 28c1 b33e  A.{....>.".?(..>
+00000530: 9bb9 d33e c21d 8a3e f1b4 583e 3764 f73b  ...>...>..X>7d.;
+00000540: 4412 23be 6b41 acbe 6a19 a33e 3cb1 4a3d  D.#.kA..j..><.J=
+00000550: a519 89be ce94 853e d4ad c63e a26c 1c3f  .......>...>.l.?
+00000560: 934a 22bf dcef 71be b6e7 ccbe ed99 d3be  .J"...q.........
+00000570: 5f0a 303e d104 8b3e f51d 493e f537 973c  _.0>...>..I>.7.<
+00000580: 98d7 12be c0d4 223e f28c 69bc c37a dbbe  ......">..i..z..
+00000590: 3d26 523e 868d 4f3e ed34 d5bd 472b a8bc  =&R>..O>.4..G+..
+000005a0: f6b4 b33d fa30 9fbd a2b4 99bd 2cb7 133f  ...=.0......,..?
+000005b0: 47e5 51bc 93ee 05be a41e 10bf 795a 0d3d  G.Q.........yZ.=
+000005c0: 902c 623e 9aa3 cabd 1adf 37bc bcba d23d  .,b>......7....=
+000005d0: d041 883d 145b 003f 1bc7 cb3e 9773 7abe  .A.=.[.?...>.sz.
+000005e0: 40a9 3c3e e736 da3d ae5b 7d3e a1e5 0b3f  @.<>.6.=.[}>...?
+000005f0: 89f0 053e 16bb cdbe 398c 2dbe 4c25 753d  ...>....9.-.L%u=
+00000600: 9d67 ac3e c124 db3e 0344 babe 6536 be3d  .g.>.$.>.D..e6.=
+00000610: 3cd3 1cbd 6382 d63e fcf9 f9bc 4b25 97be  <...c..>....K%..
+00000620: 4e7e cebe 6f6b 00be 69b4 8ebe 0320 a3bd  N~..ok..i.... ..
+00000630: f76d e23d 3fb3 8fbe 108f 0dbe 5798 0bbf  .m.=?.......W...
+00000640: f864 d6be 3090 9bbe c7f7 6b3e afea c9be  .d..0.....k>....
+00000650: 739e a93e aaab 93bc 4fff 393e 67b6 66bd  s..>....O.9>g.f.
+00000660: 4cfb b3bc f8e9 4c3e 2869 45bc ad15 c6be  L.....L>(iE.....
+00000670: d9d0 86bd 78d3 003e 5411 423e ed34 a9bd  ....x..>T.B>.4..
+00000680: 8ca1 6dbe 6751 b83e a8de c33e bc84 05bf  ..m.gQ.>...>....
+00000690: d92d 883e dd84 be3e 4cc3 ef3e eae9 cebd  .-.>...>L..>....
+000006a0: 44ff ec3c d090 493f 3645 8ebe 8497 6ebe  D..<..I?6E....n.
+000006b0: 6e0f b9bd 0eb6 843e 41c2 dd3e b2d4 b5be  n......>A..>....
+000006c0: 45ca c8bd aa82 67be 64a3 183e 1017 f5be  E.....g.d..>....
+000006d0: e5d1 173c 3a34 8abe 0332 113f 00a5 273f  ...<:4...2.?..'?
+000006e0: c1e6 d03b c61c 70bd 7d18 2e3e edec 553d  ...;..p.}..>..U=
+000006f0: 0b8c 263c 0749 2f3f 4b66 163f cb20 a2bd  ..&<.I/?Kf.?. ..
+00000700: 0a71 353e b5a1 e53d d73b 28be 5ac1 023e  .q5>...=.;(.Z..>
+00000710: dde3 1ebd 4841 a8be 8274 b83d 3b24 9e3e  ....HA...t.=;$.>
+00000720: c27e fb3d 62f7 373e f0cd f63e a1e7 b9be  .~.=b.7>...>....
+00000730: 5bdb ac3d 96d2 173e c4d9 b1be 99ba 91be  [..=...>........
+00000740: 8039 233f 0532 f0be eb47 a5bd 7983 d3be  .9#?.2...G..y...
+00000750: bb7e 073e e397 26bd e567 babe 508d 6ebd  .~.>..&..g..P.n.
+00000760: 2556 ba3b cf36 e43e 6eef 86bc ea34 093f  %V.;.6.>n....4.?
+00000770: 4b86 bc3e a7e0 b03e 1a66 69be b92b cfbd  K..>...>.fi..+..
+00000780: 77c5 573e 35c8 d73e 024d 30bf 049e 81be  w.W>5..>.M0.....
+00000790: 934f 203d aef8 183e 4815 b5be d587 b83e  .O =...>H......>
+000007a0: 16af 81be 4693 dcbc 37ba 31bd 5938 283e  ....F...7.1.Y8(>
+000007b0: 1691 93bd 875f 89be 2648 71be 2007 d23e  ....._..&Hq. ..>
+000007c0: 6a4e f33e 3ec0 973d 0908 ccbd 7f90 6cbe  jN.>>..=......l.
+000007d0: e458 d5be f8e1 c2be 1a86 0dbe a8fe 4cbd  .X............L.
+000007e0: f2dc 0e3e fcf6 403e 5154 f13d cbb7 89be  ...>..@>QT.=....
+000007f0: f63c e5be 4ab6 d0be 9abb 293f 880e 163f  .<..J.....)?...?
+00000800: ab8a 0abd e073 4238 8e1d debd a200 8dbe  .....sB8........
+00000810: 1480 283e 9b44 0bbf 5d5a 4b3e b6c5 013e  ..(>.D..]ZK>...>
+00000820: 353f fbbd 0f64 e43e 3854 0f3c 7b43 57be  5?...d.>8T.<{CW.
+00000830: 3e28 c9bc 6f24 d3be 2a70 babd 7ca5 1a3d  >(..o$..*p..|..=
+00000840: 4d50 a8be 6242 a03d 3a4e 4abe ad6c c13d  MP..bB.=:NJ..l.=
+00000850: e56c c2bc 8bb5 783e db5f e33d 7244 853e  .l....x>._.=rD.>
+00000860: 058c 073e 944d 853e ce27 393e ba79 1dbf  ...>.M.>.'9>.y..
+00000870: bc6e ac3e e7c4 e4be 4d53 6a3c 36f3 ffbe  .n.>....MSj<6...
+00000880: d2e4 91be 6375 b13e d8bb 0cbf fa7b 473e  ....cu.>.....{G>
+00000890: ae65 373e a01d 92be a5b5 803e f6f8 bcbe  .e7>.......>....
+000008a0: cb1d 8cbd 428c bebd 73c3 57bd 5c16 cb3e  ....B...s.W.\..>
+000008b0: 9168 01bf 254e 8c3e 20f9 5b3d 3cc2 5d3e  .h..%N.> .[=<.]>
+000008c0: a12f 57bd e30f 0dbe a509 57bd 1bbd 5bbe  ./W.......W...[.
+000008d0: ee71 c33c deb1 ce3c b1a2 603d 5633 77bd  .q.<...<..`=V3w.
+000008e0: 23d8 56be 34a9 3bbe 0c8d f6be 529b 28be  #.V.4.;.....R.(.
+000008f0: f40b 6d3d ceb3 16be f72e 233e 7ebf 0dbe  ..m=......#>~...
+00000900: 1e13 60be 74ab 77be 961b 8dbd cf31 8e3e  ..`.t.w......1.>
+00000910: fbe6 a43d df7c a03e 1f67 ab3e 0c85 b6be  ...=.|.>.g.>....
+00000920: 5407 67be 0f0f d53e 7a24 353e 1603 893e  T.g....>z$5>...>
+00000930: a9a7 133e 6b69 33bd 60e4 aa3e 8a9a 413e  ...>ki3.`..>..A>
+00000940: faf9 3c3d c7a0 ecbe 3776 86be f163 d0be  ..<=....7v...c..
+00000950: e52f 6c3c 3777 e33d 87ef 39be 415c 13be  ./l<7w.=..9.A\..
+00000960: 05ae 013f 408b 403e 7cb3 473e d640 22bd  ...?@.@>|.G>.@".
+00000970: 9689 d23d 194f 673e f6d7 003f b8fd 51be  ...=.Og>...?..Q.
+00000980: fc94 11be c8c0 153b 79ba 73be 62fb 0a3f  .......;y.s.b..?
+00000990: ce11 4c3f bdcb 24be aac0 c53e edec 563e  ..L?..$....>..V>
+000009a0: 85f5 d43d e6d8 60be 14f7 efbe 9eba 5fbe  ...=..`......._.
+000009b0: a40b a8bd ff01 1ebf 140e 1abf 7b78 05bf  ............{x..
+000009c0: eb8e 5a3f d4f7 d73e 18c2 2fbf 11e9 07ba  ..Z?...>../.....
+000009d0: de39 32be b2e1 a1bb 9052 34bf d5f4 cbbe  .92......R4.....
+000009e0: c249 6ebe 6bfc 5b3d 5ffa 8abd 1008 ec3e  .In.k.[=_......>
+000009f0: 29fd 34be 5743 92be 9475 1ebe c0bc 1fbb  ).4.WC...u......
+00000a00: f96a c0be 68a3 373e b300 43be 7371 ad3d  .j..h.7>..C.sq.=
+00000a10: e5c4 b6bd b00e ddbe 3db8 c83e 269c 9cbd  ........=..>&...
+00000a20: 7cf0 613e 005c dbbe 3c39 4e3e f2cd 80be  |.a>.\..<9N>....
+00000a30: b979 023e aae4 60bc b064 f2be 2adb d9be  .y.>..`..d..*...
+00000a40: acd9 903d b35c c03e e81d ebbc 8352 74bd  ...=.\.>.....Rt.
+00000a50: ba2d 37bf b363 903d 9588 08bd 5da1 04bb  .-7..c.=....]...
+00000a60: 017e c33e 305c d43e f482 71be 40a7 fe3e  .~.>0\.>..q.@..>
+00000a70: 0d06 63bd 6447 5c3c 98cd 043d dce8 b03d  ..c.dG\<...=...=
+00000a80: 5093 dd3e f647 c13d 4c6f c0be 8f0b 3e3d  P..>.G.=Lo....>=
+00000a90: 6c29 f13c 8859 383e 7f6d 2a3e 8615 9d3d  l).<.Y8>.m*>...=
+00000aa0: 7162 b13d dc70 9d3d f48a 483e c76b 8abe  qb.=.p.=..H>.k..
+00000ab0: 4792 5bbe a82b 4abd bf00 733e 2164 b13d  G.[..+J...s>!d.=
+00000ac0: 5e08 aabe e816 f4bd 1701 d8be 2057 4e3f  ^........... WN?
+00000ad0: 9316 68bd 5023 d33e bf5a 543e 4276 4b3d  ..h.P#.>.ZT>BvK=
+00000ae0: af1e 773d 77dd edbc 3f55 8c3c 9eef 9a3e  ..w=w...?U.<...>
+00000af0: 6f70 03be cb19 d73e 292a 69bd 8ca0 93bb  op.....>)*i.....
+00000b00: bffa 633d 18be 9b3e fca0 acbe 9ae2 2c3f  ..c=...>......,?
+00000b10: 928f b6bd 8ed6 c03e 5945 a3bd be21 1c3e  .......>YE...!.>
+00000b20: 738c 133e cb1e 7b3e c021 03be a157 27be  s..>..{>.!...W'.
+00000b30: 881a 623e bbca 34bd a3ce d2be 3f0b 043e  ..b>..4.....?..>
+00000b40: cde9 adbc e1de 403e 2946 423d 5f21 49bf  ......@>)FB=_!I.
+00000b50: f505 dabe 5e93 ab3d 6c6c 75bd 577b 943e  ....^..=llu.W{.>
+00000b60: 0b8a 353e 2c50 04bf 9699 b63e 4e42 ac3e  ..5>,P.....>NB.>
+00000b70: 2d84 09be c507 b1be c7cb bc3e 4088 5fbe  -..........>@._.
+00000b80: 4f0c 4abe 4e32 443e 97ad 16bf f844 8a3d  O.J.N2D>.....D.=
+00000b90: 7639 4cbe b153 b13d 2183 d0be ef6c 85be  v9L..S.=!....l..
+00000ba0: 25dd a83e b9c7 c03d 6729 a1be 9430 153d  %..>...=g)...0.=
+00000bb0: ee32 cd3e 3df1 67be 1fd6 953e 532f 9bbd  .2.>=.g....>S/..
+00000bc0: 8713 193e e5b7 1c3e 2306 e3be 59dc ebbe  ...>...>#...Y...
+00000bd0: 6f9e babe 5d28 a9be d712 553e 66d1 28be  o...](....U>f.(.
+00000be0: 9d12 12bf 6ca2 903e cd57 8d3e e84c 9d3e  ....l..>.W.>.L.>
+00000bf0: 2d6f 983e 5ecf 15be 7076 973e 124f 06bd  -o.>^...pv.>.O..
+00000c00: 2ac7 d53c 2147 14bf c09d 9fbe ae60 b3be  *..<!G.......`..
+00000c10: e18c 8eb9 d2d9 f03d a37f 903e 566d b0be  .......=...>Vm..
+00000c20: 60e5 3ebf 6386 0b3e a7bf 563e 6499 36bd  `.>.c..>..V>d.6.
+00000c30: 4246 113e f06e 88bd 6261 94bd ec98 463e  BF.>.n..ba....F>
+00000c40: acdf bfbe ab61 1b3e 2aad 403e fb32 133e  .....a.>*.@>.2.>
+00000c50: 3942 8c3e 4a97 0bbf 7f67 a53e 1946 543e  9B.>J....g.>.FT>
+00000c60: 218b 88bd c86a a1be 4cf9 503d b0f0 213e  !....j..L.P=..!>
+00000c70: 55bb 9b3d 0021 04bc f754 24be eef7 0c3e  U..=.!...T$....>
+00000c80: 83e6 043f 4a61 da3e 8353 2dbe 71bb 21be  ...?Ja.>.S-.q.!.
+00000c90: 9e20 a03d cadf 8d3d 06d5 c73e 1de9 84bd  . .=...=...>....
+00000ca0: 0697 ea3e 8c00 e9bd c42f 50be c781 b53e  ...>...../P....>
+00000cb0: f33d 863e cac0 95be 9580 e0be 1d9a 383f  .=.>..........8?
+00000cc0: 0b0f 353c d72e b03e efe5 62bd 53c3 26bf  ..5<...>..b.S.&.
+00000cd0: b8d3 5cbe 5416 aebe 25c5 56be 1a29 2cbe  ..\.T...%.V..),.
+00000ce0: 3b57 55be a9f2 9b3d 8da2 1b3e d2f4 1abc  ;WU....=...>....
+00000cf0: 75d1 34bd 75ac a23e 0097 323e 1a54 16be  u.4.u..>..2>.T..
+00000d00: a00f 483e 1111 34be 9027 2cbe c509 0b3f  ..H>..4..',....?
+00000d10: 03e5 1b3e eddb 96bd 5e71 513f 05e6 9f3e  ...>....^qQ?...>
+00000d20: 4845 503f 78ae 43bf f846 8fbd 5a06 f4be  HEP?x.C..F..Z...
+00000d30: ecda 04bd c533 adbc 9c88 22bf 4e0c 12bf  .....3....".N...
+00000d40: 4c8b 573f 90da c03e 811e 1dbf a89f 2fbe  L.W?...>....../.
+00000d50: 03d2 843c e795 59bd 561b 9bbe 24ce 0dbf  ...<..Y.V...$...
+00000d60: 9fb7 e8bc fd0d 753e 8dde 573e a4a6 9f3e  ......u>..W>...>
+00000d70: 02f2 ee3e adbd 29bf e427 5a3f be4a 563d  ...>..)..'Z?.JV=
+00000d80: 29e9 273e 4f36 ab3d efb6 9fbe cc32 c83e  ).'>O6.=.....2.>
+00000d90: 1d3b a1bc ebf5 4bbe 0d88 debd ad9e 433e  .;....K.......C>
+00000da0: 01da c23e d574 67be 3438 27be 8d42 5a3f  ...>.tg.48'..BZ?
+00000db0: 6f33 0a3e 18c3 e2bd 3029 0abf 1237 cbbe  o3.>....0)...7..
+00000dc0: 4f82 963d 5814 99be 906a 8ebe b771 39be  O..=X....j...q9.
+00000dd0: f00f dfbe 9a83 29bf ea54 adbd a35a 003e  ......)..T...Z.>
+00000de0: 7300 d83d bfc7 14bd a475 233f 3140 27bc  s..=.....u#?1@'.
+00000df0: 3fad c6bd 683d 103e 0be8 b03e 2769 13bd  ?...h=.>...>'i..
+00000e00: 9fd4 08bf d60e 68bd 1a29 91be df8a 223f  ......h..)...."?
+00000e10: 2266 ea3e b3cd a33c 25a2 453e 3a1b fb3e  "f.>...<%.E>:..>
+00000e20: 2d76 173f 1e19 25bf 158a b1bc 2d81 43be  -v.?..%.....-.C.
+00000e30: c606 2c3e 4691 85be 7fce 8fbe 8c94 cc3a  ..,>F..........:
+00000e40: 142b 143f 092c 8b3e 6399 bbbc 216d 8b3d  .+.?.,.>c...!m.=
+00000e50: 14fc ba3e 83f1 1cbe 4256 81be 289e 313e  ...>....BV..(.1>
+00000e60: 0b47 9e3d a17f 403f f789 203e e5b9 063f  .G.=..@?.. >...?
+00000e70: cd6a debd ce4d 51bd 94a4 b33e abff ecbe  .j...MQ....>....
+00000e80: b168 0e3e f8fb 3a3b fe22 75bd fd52 273e  .h.>..:;."u..R'>
+00000e90: 25f2 8e3c c0f5 fe3d ddcd 4bbe a78f 6abd  %..<...=..K...j.
+00000ea0: b4fa acbd 2eeb 383f 98d5 1abf 8d5f cabd  ......8?....._..
+00000eb0: 3513 57bb f01c 003f a63d aabe f587 1e3e  5.W....?.=.....>
+00000ec0: 3bf3 fa3d 8ff5 4bbe ff3f 653e 8a1f e23d  ;..=..K..?e>...=
+00000ed0: bbca 56be e733 d5be 0fa9 d33e 6822 7c3d  ..V..3.....>h"|=
+00000ee0: 86de ec3d f71c 353d 7c6b 5dbe fdf0 633c  ...=..5=|k]...c<
+00000ef0: 90aa 933e f361 a73e 6880 fb3e 5aac c1be  ...>.a.>h..>Z...
+00000f00: 34a7 3f3d ead4 0f3e 566c fb3d d53d 993e  4.?=...>Vl.=.=.>
+00000f10: 76c5 b0be 4dd9 79be 5355 a83e c8b0 c53e  v...M.y.SU.>...>
+00000f20: 36f6 c3bd 7919 2f3e b1c9 d93d 4794 8e3e  6...y./>...=G..>
+00000f30: b494 c63e d02c 98be 9763 d73e 0dc7 48bd  ...>.,...c.>..H.
+00000f40: 999e 563e 8efc 8b3e 8298 243e 1659 fb3e  ..V>...>..$>.Y.>
+00000f50: afb6 d23e ff55 0e3e 2226 e33e a005 43be  ...>.U.>"&.>..C.
+00000f60: 008b 8d3e 4360 15be 0348 02bf 91eb ebbd  ...>C`...H......
+00000f70: 4e14 843d e1f9 f5bd a829 1ebf 24fb a63e  N..=.....)..$..>
+00000f80: 49de f7be a823 763e d21a 26be cffa a5be  I....#v>..&.....
+00000f90: c599 d1bc e1af 8e3d d5d3 bbbd e8c3 803e  .......=.......>
+00000fa0: 7aa2 8e3e 4dfc 33bc 6124 91bc 943c e9bc  z..>M.3.a$...<..
+00000fb0: 05aa 0d3f 9750 26be b637 8bbe d53a adbb  ...?.P&..7...:..
+00000fc0: 3c11 a1be b5c0 35be 499d 623d eec1 d33e  <.....5.I.b=...>
+00000fd0: bafa 543d 7467 d4bd a8c7 1ebf 13dc 9bbe  ..T=tg..........
+00000fe0: 9fe4 ab3d 09c1 c2be 97b8 9dbe 057c bd3c  ...=.........|.<
+00000ff0: 7bfa 7b3e 2bb8 333b ba9c 2c3e 0b9e 933d  {.{>+.3;..,>...=
```

##### archive/data/7

```diff
@@ -1,16 +1,8 @@
-00000000: cf53 213d 3bdd bebc 8118 2f3e 7013 66be  .S!=;...../>p.f.
-00000010: 9a41 ab3e a46d 9a3e 0c9b a93d e854 7fbd  .A.>.m.>...=.T..
-00000020: 0c93 3e3e f58c a7be f501 8d3c 16a5 31bd  ..>>.......<..1.
-00000030: 49da 233e 92eb 18bd e19d 4a3e ecf5 923b  I.#>......J>...;
-00000040: eefd ab3a e438 d5bd 6d27 6a3d 46d1 9bbc  ...:.8..m'j=F...
-00000050: cd38 0b3e 8df1 1bbd 2181 70bd 2627 303e  .8.>....!.p.&'0>
-00000060: f908 0e3e 0b52 163e deee 87be 32c1 db3d  ...>.R.>....2..=
-00000070: acff 553d 90ff 183e 90b0 f43d 404a f4bd  ..U=...>...=@J..
-00000080: 6558 22bd d54c a43c 8872 31be d493 663e  eX"..L.<.r1...f>
-00000090: fcd6 abbe 0ad0 99be 28d8 a4bd 0af4 7c3d  ........(.....|=
-000000a0: 7366 3bbe 10b8 a63e 3055 67bc 9036 2a3d  sf;....>0Ug..6*=
-000000b0: 93fe 28be 2487 183d 286f 49be ed65 1dbb  ..(.$..=(oI..e..
-000000c0: a375 3fba da0f c83d 7a06 58bd c430 a53c  .u?....=z.X..0.<
-000000d0: 0135 0bbe 98f4 1d3d 43e6 793d 2c36 32be  .5.....=C.y=,62.
-000000e0: ee50 11be 4ba2 19be 8694 883e 44b4 d9bd  .P..K......>D...
-000000f0: 2a85 69bd f6db 17be 7e19 f5bd f68d f43d  *.i.....~......=
+00000000: 003c 243e 7e29 ed3d 0e78 0fbd ad08 5fbe  .<$>~).=.x...._.
+00000010: 5842 f73d a55b 5b3d a109 a83c 9a3d df3d  XB.=.[[=...<.=.=
+00000020: d5c2 ae3d c4bc 2ebd 2da6 1d3e 3b11 94bc  ...=....-..>;...
+00000030: 2925 cdbc 011c 0d3e 6f09 bcbb 5f22 863d  )%.....>o..._".=
+00000040: 2a33 69bd 70ad 2ebd 8b40 503c 2d2a 11be  *3i.p....@P<-*..
+00000050: fbe1 84bd aa8a a7bb b5c6 ae3d 3279 a33d  ...........=2y.=
+00000060: 0c45 b83c 2168 463d ce23 19be 57b8 d83d  .E.<!hF=.#..W..=
+00000070: 8ba7 f6bd 5fa9 bc3c 8170 65bd b6d7 1c3d  ...._..<.pe....=
```

##### archive/data/8

```diff
@@ -1 +1,16 @@
-00000000: ac73 c9bb aa73 c93b                      .s...s.;
+00000000: 6026 87be be41 0c3e ff7c 873d 996d 903d  `&...A.>.|.=.m.=
+00000010: 93ff 6d3c f7c0 aebe 3191 9b3e 052a 013e  ..m<....1..>.*.>
+00000020: 8979 e2bd 7fe7 babd 25df 343d b52c e1bd  .y......%.4=.,..
+00000030: c5ec eabd 4f7d de3c 1f0c 6c3d 21d8 903d  ....O}.<..l=!..=
+00000040: 7bcb dc3d d08e bbbd 003d ac3d c8f6 5d3c  {..=.....=.=..]<
+00000050: 3363 eabd 2da6 19be 87fb e73c bed9 6dbe  3c..-......<..m.
+00000060: b8e6 873e 5a73 92bd 7a9b fe3c 3c39 3bbd  ...>Zs..z..<<9;.
+00000070: 237b d03c 163b 063e 9d2b 3dbd 21ec 273c  #{.<.;.>.+=.!.'<
+00000080: 289e 843e c69f 0bbe 57ed 77bd c5e8 90bd  (..>....W.w.....
+00000090: bdc9 69bc a5b8 ac3e 24bc 9cbe 186d 01be  ..i....>$....m..
+000000a0: ebc7 ed3d c60f bc3d 02fc 2fbd 5ad1 de3d  ...=...=../.Z..=
+000000b0: 94d5 e63d 5d8e dabc 699e 66bd 6c93 8ebd  ...=]...i.f.l...
+000000c0: 6b3b dcbd 4ccb ba3d 3808 a2bd 7ffe 35bc  k;..L..=8.....5.
+000000d0: bb7e ea3d c882 193e 9832 d6bc 9043 6f3e  .~.=...>.2...Co>
+000000e0: a494 88be 6afd 8e3d e74d d6bc f1e3 3e3d  ....j..=.M....>=
+000000f0: ec22 debc 86e4 06be 79aa 363d 7609 58bc  ."......y.6=v.X.
```

##### archive/data/9

```diff
@@ -1,8 +1 @@
-00000000: b8a9 b5be 00b3 b13e cedf 7d3e ea82 513e  .......>..}>..Q>
-00000010: e8c5 2b3e 2f4c 473d 1e3a 343e 7e4f 243e  ..+>/LG=.:4>~O$>
-00000020: 508e b0be 29a7 0d3d 43de 8f3d 89b9 efbe  P...)..=C..=....
-00000030: 1826 953d 7d2c 93be 4405 873d 40db e9be  .&.=},..D..=@...
-00000040: 509a 9c3e a38e 283e 6e6c 24bf 1f9c c23e  P..>..(>nl$....>
-00000050: bd3e b1be 9cd8 0a3f 08b7 993e c9c2 52be  .>.....?...>..R.
-00000060: d9a7 1ebe 598f 8a3d f491 0b3d 1a9d 90bd  ....Y..=...=....
-00000070: 9e11 643e 08a9 7b3e 0357 7ebe cd50 a6be  ..d>..{>.W~..P..
+00000000: a7c1 8a3c 9ac1 8abc                      ...<....
```

#### policy.optimizer.pth

##### zipinfo {}

```diff
@@ -1,20 +1,40 @@
-Zip file size: 14645 bytes, number of entries: 18
--rw----     0.0 fat     1279 bl stor 80-000-00 00:00 archive/data.pkl
--rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/0
+Zip file size: 29433 bytes, number of entries: 38
+-rw----     0.0 fat     2354 bl stor 80-000-00 00:00 archive/data.pkl
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/0
 -rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/1
--rw----     0.0 fat        8 bl stor 80-000-00 00:00 archive/data/10
--rw----     0.0 fat        8 bl stor 80-000-00 00:00 archive/data/11
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/12
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/13
--rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/14
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/10
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/11
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/12
+-rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/13
+-rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/14
 -rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/15
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/2
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/3
--rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/4
--rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/5
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/6
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/7
--rw----     0.0 fat      256 bl stor 80-000-00 00:00 archive/data/8
--rw----     0.0 fat      256 bl stor 80-000-00 00:00 archive/data/9
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/16
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/17
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/18
+-rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/19
+-rw----     0.0 fat      512 bl stor 80-000-00 00:00 archive/data/2
+-rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/20
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/21
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/22
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/23
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/24
+-rw----     0.0 fat      256 bl stor 80-000-00 00:00 archive/data/25
+-rw----     0.0 fat      256 bl stor 80-000-00 00:00 archive/data/26
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/27
+-rw----     0.0 fat        8 bl stor 80-000-00 00:00 archive/data/28
+-rw----     0.0 fat        8 bl stor 80-000-00 00:00 archive/data/29
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/3
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/30
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/31
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/32
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/33
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/34
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/35
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/4
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 archive/data/5
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/6
+-rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/7
+-rw----     0.0 fat     4096 bl stor 80-000-00 00:00 archive/data/8
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 archive/data/9
 -rw----     0.0 fat        2 bl stor 80-000-00 00:00 archive/version
-18 files, 11801 bytes uncompressed, 11801 bytes compressed:  0.0%
+38 files, 22652 bytes uncompressed, 22652 bytes compressed:  0.0%
```

##### zipnote «TEMP»/diffoscope_3cnx63wy_/tmpfi2aeasw_.zip

```diff
@@ -21,20 +21,80 @@
 
 Filename: archive/data/14
 Comment: 
 
 Filename: archive/data/15
 Comment: 
 
+Filename: archive/data/16
+Comment: 
+
+Filename: archive/data/17
+Comment: 
+
+Filename: archive/data/18
+Comment: 
+
+Filename: archive/data/19
+Comment: 
+
 Filename: archive/data/2
 Comment: 
 
+Filename: archive/data/20
+Comment: 
+
+Filename: archive/data/21
+Comment: 
+
+Filename: archive/data/22
+Comment: 
+
+Filename: archive/data/23
+Comment: 
+
+Filename: archive/data/24
+Comment: 
+
+Filename: archive/data/25
+Comment: 
+
+Filename: archive/data/26
+Comment: 
+
+Filename: archive/data/27
+Comment: 
+
+Filename: archive/data/28
+Comment: 
+
+Filename: archive/data/29
+Comment: 
+
 Filename: archive/data/3
 Comment: 
 
+Filename: archive/data/30
+Comment: 
+
+Filename: archive/data/31
+Comment: 
+
+Filename: archive/data/32
+Comment: 
+
+Filename: archive/data/33
+Comment: 
+
+Filename: archive/data/34
+Comment: 
+
+Filename: archive/data/35
+Comment: 
+
 Filename: archive/data/4
 Comment: 
 
 Filename: archive/data/5
 Comment: 
 
 Filename: archive/data/6
```

##### archive/data.pkl

```diff
@@ -1,80 +1,148 @@
 00000000: 8002 7d71 0028 5805 0000 0073 7461 7465  ..}q.(X....state
 00000010: 7101 7d71 0228 4b00 7d71 0328 5804 0000  q.}q.(K.}q.(X...
-00000020: 0073 7465 7071 044d 403d 5807 0000 0065  .stepq.M@=X....e
-00000030: 7870 5f61 7667 7105 6374 6f72 6368 2e5f  xp_avgq.ctorch._
-00000040: 7574 696c 730a 5f72 6562 7569 6c64 5f74  utils._rebuild_t
-00000050: 656e 736f 725f 7632 0a71 0628 2858 0700  ensor_v2.q.((X..
-00000060: 0000 7374 6f72 6167 6571 0763 746f 7263  ..storageq.ctorc
-00000070: 680a 466c 6f61 7453 746f 7261 6765 0a71  h.FloatStorage.q
-00000080: 0858 0100 0000 3071 0958 0300 0000 6370  .X....0q.X....cp
-00000090: 7571 0a4b 8074 710b 514b 004b 204b 0486  uq.K.tq.QK.K K..
-000000a0: 710c 4b04 4b01 8671 0d89 6363 6f6c 6c65  q.K.K..q..ccolle
-000000b0: 6374 696f 6e73 0a4f 7264 6572 6564 4469  ctions.OrderedDi
-000000c0: 6374 0a71 0e29 5271 0f74 7110 5271 1158  ct.q.)Rq.tq.Rq.X
-000000d0: 0a00 0000 6578 705f 6176 675f 7371 7112  ....exp_avg_sqq.
-000000e0: 6806 2828 6807 6808 5801 0000 0031 7113  h.((h.h.X....1q.
-000000f0: 680a 4b80 7471 1451 4b00 4b20 4b04 8671  h.K.tq.QK.K K..q
-00000100: 154b 044b 0186 7116 8968 0e29 5271 1774  .K.K..q..h.)Rq.t
-00000110: 7118 5271 1975 4b01 7d71 1a28 6804 4d40  q.Rq.uK.}q.(h.M@
-00000120: 3d68 0568 0628 2868 0768 0858 0100 0000  =h.h.((h.h.X....
-00000130: 3271 1b68 0a4b 2074 711c 514b 004b 2085  2q.h.K tq.QK.K .
-00000140: 711d 4b01 8571 1e89 680e 2952 711f 7471  q.K..q..h.)Rq.tq
-00000150: 2052 7121 6812 6806 2828 6807 6808 5801   Rq!h.h.((h.h.X.
-00000160: 0000 0033 7122 680a 4b20 7471 2351 4b00  ...3q"h.K tq#QK.
-00000170: 4b20 8571 244b 0185 7125 8968 0e29 5271  K .q$K..q%.h.)Rq
-00000180: 2674 7127 5271 2875 4b02 7d71 2928 6804  &tq'Rq(uK.}q)(h.
-00000190: 4d40 3d68 0568 0628 2868 0768 0858 0100  M@=h.h.((h.h.X..
-000001a0: 0000 3471 2a68 0a4d 0004 7471 2b51 4b00  ..4q*h.M..tq+QK.
-000001b0: 4b20 4b20 8671 2c4b 204b 0186 712d 8968  K K .q,K K..q-.h
-000001c0: 0e29 5271 2e74 712f 5271 3068 1268 0628  .)Rq.tq/Rq0h.h.(
-000001d0: 2868 0768 0858 0100 0000 3571 3168 0a4d  (h.h.X....5q1h.M
-000001e0: 0004 7471 3251 4b00 4b20 4b20 8671 334b  ..tq2QK.K K .q3K
-000001f0: 204b 0186 7134 8968 0e29 5271 3574 7136   K..q4.h.)Rq5tq6
-00000200: 5271 3775 4b03 7d71 3828 6804 4d40 3d68  Rq7uK.}q8(h.M@=h
-00000210: 0568 0628 2868 0768 0858 0100 0000 3671  .h.((h.h.X....6q
-00000220: 3968 0a4b 2074 713a 514b 004b 2085 713b  9h.K tq:QK.K .q;
-00000230: 4b01 8571 3c89 680e 2952 713d 7471 3e52  K..q<.h.)Rq=tq>R
-00000240: 713f 6812 6806 2828 6807 6808 5801 0000  q?h.h.((h.h.X...
-00000250: 0037 7140 680a 4b20 7471 4151 4b00 4b20  .7q@h.K tqAQK.K 
-00000260: 8571 424b 0185 7143 8968 0e29 5271 4474  .qBK..qC.h.)RqDt
-00000270: 7145 5271 4675 4b04 7d71 4728 6804 4d40  qERqFuK.}qG(h.M@
-00000280: 3d68 0568 0628 2868 0768 0858 0100 0000  =h.h.((h.h.X....
-00000290: 3871 4868 0a4b 4074 7149 514b 004b 024b  8qHh.K@tqIQK.K.K
-000002a0: 2086 714a 4b20 4b01 8671 4b89 680e 2952   .qJK K..qK.h.)R
-000002b0: 714c 7471 4d52 714e 6812 6806 2828 6807  qLtqMRqNh.h.((h.
-000002c0: 6808 5801 0000 0039 714f 680a 4b40 7471  h.X....9qOh.K@tq
-000002d0: 5051 4b00 4b02 4b20 8671 514b 204b 0186  PQK.K.K .qQK K..
-000002e0: 7152 8968 0e29 5271 5374 7154 5271 5575  qR.h.)RqStqTRqUu
-000002f0: 4b05 7d71 5628 6804 4d40 3d68 0568 0628  K.}qV(h.M@=h.h.(
-00000300: 2868 0768 0858 0200 0000 3130 7157 680a  (h.h.X....10qWh.
-00000310: 4b02 7471 5851 4b00 4b02 8571 594b 0185  K.tqXQK.K..qYK..
-00000320: 715a 8968 0e29 5271 5b74 715c 5271 5d68  qZ.h.)Rq[tq\Rq]h
-00000330: 1268 0628 2868 0768 0858 0200 0000 3131  .h.((h.h.X....11
-00000340: 715e 680a 4b02 7471 5f51 4b00 4b02 8571  q^h.K.tq_QK.K..q
-00000350: 604b 0185 7161 8968 0e29 5271 6274 7163  `K..qa.h.)Rqbtqc
-00000360: 5271 6475 4b06 7d71 6528 6804 4d40 3d68  RqduK.}qe(h.M@=h
-00000370: 0568 0628 2868 0768 0858 0200 0000 3132  .h.((h.h.X....12
-00000380: 7166 680a 4b20 7471 6751 4b00 4b01 4b20  qfh.K tqgQK.K.K 
-00000390: 8671 684b 204b 0186 7169 8968 0e29 5271  .qhK K..qi.h.)Rq
-000003a0: 6a74 716b 5271 6c68 1268 0628 2868 0768  jtqkRqlh.h.((h.h
-000003b0: 0858 0200 0000 3133 716d 680a 4b20 7471  .X....13qmh.K tq
-000003c0: 6e51 4b00 4b01 4b20 8671 6f4b 204b 0186  nQK.K.K .qoK K..
-000003d0: 7170 8968 0e29 5271 7174 7172 5271 7375  qp.h.)RqqtqrRqsu
-000003e0: 4b07 7d71 7428 6804 4d40 3d68 0568 0628  K.}qt(h.M@=h.h.(
-000003f0: 2868 0768 0858 0200 0000 3134 7175 680a  (h.h.X....14quh.
-00000400: 4b01 7471 7651 4b00 4b01 8571 774b 0185  K.tqvQK.K..qwK..
-00000410: 7178 8968 0e29 5271 7974 717a 5271 7b68  qx.h.)RqytqzRq{h
-00000420: 1268 0628 2868 0768 0858 0200 0000 3135  .h.((h.h.X....15
-00000430: 717c 680a 4b01 7471 7d51 4b00 4b01 8571  q|h.K.tq}QK.K..q
-00000440: 7e4b 0185 717f 8968 0e29 5271 8074 7181  ~K..q..h.)Rq.tq.
-00000450: 5271 8275 7558 0c00 0000 7061 7261 6d5f  Rq.uuX....param_
-00000460: 6772 6f75 7073 7183 5d71 847d 7185 2858  groupsq.]q.}q.(X
-00000470: 0200 0000 6c72 7186 473f 33a9 2a30 5532  ....lrq.G?3.*0U2
-00000480: 6158 0500 0000 6265 7461 7371 8747 3fec  aX....betasq.G?.
-00000490: cccc cccc cccd 473f eff7 ced9 1687 2b86  ......G?......+.
-000004a0: 7188 5803 0000 0065 7073 7189 473e e4f8  q.X....epsq.G>..
-000004b0: b588 e368 f158 0c00 0000 7765 6967 6874  ...h.X....weight
-000004c0: 5f64 6563 6179 718a 4b00 5807 0000 0061  _decayq.K.X....a
-000004d0: 6d73 6772 6164 718b 8958 0600 0000 7061  msgradq..X....pa
-000004e0: 7261 6d73 718c 5d71 8d28 4b00 4b01 4b02  ramsq.]q.(K.K.K.
-000004f0: 4b03 4b04 4b05 4b06 4b07 6575 6175 2e    K.K.K.K.K.euau.
+00000020: 0073 7465 7071 0463 746f 7263 682e 5f75  .stepq.ctorch._u
+00000030: 7469 6c73 0a5f 7265 6275 696c 645f 7465  tils._rebuild_te
+00000040: 6e73 6f72 5f76 320a 7105 2828 5807 0000  nsor_v2.q.((X...
+00000050: 0073 746f 7261 6765 7106 6374 6f72 6368  .storageq.ctorch
+00000060: 0a46 6c6f 6174 5374 6f72 6167 650a 7107  .FloatStorage.q.
+00000070: 5801 0000 0030 7108 5803 0000 0063 7075  X....0q.X....cpu
+00000080: 7109 4b01 7471 0a51 4b00 2929 8963 636f  q.K.tq.QK.)).cco
+00000090: 6c6c 6563 7469 6f6e 730a 4f72 6465 7265  llections.Ordere
+000000a0: 6444 6963 740a 710b 2952 710c 7471 0d52  dDict.q.)Rq.tq.R
+000000b0: 710e 5807 0000 0065 7870 5f61 7667 710f  q.X....exp_avgq.
+000000c0: 6805 2828 6806 6807 5801 0000 0031 7110  h.((h.h.X....1q.
+000000d0: 6809 4b80 7471 1151 4b00 4b20 4b04 8671  h.K.tq.QK.K K..q
+000000e0: 124b 044b 0186 7113 8968 0b29 5271 1474  .K.K..q..h.)Rq.t
+000000f0: 7115 5271 1658 0a00 0000 6578 705f 6176  q.Rq.X....exp_av
+00000100: 675f 7371 7117 6805 2828 6806 6807 5801  g_sqq.h.((h.h.X.
+00000110: 0000 0032 7118 6809 4b80 7471 1951 4b00  ...2q.h.K.tq.QK.
+00000120: 4b20 4b04 8671 1a4b 044b 0186 711b 8968  K K..q.K.K..q..h
+00000130: 0b29 5271 1c74 711d 5271 1e75 4b01 7d71  .)Rq.tq.Rq.uK.}q
+00000140: 1f28 6804 6805 2828 6806 6807 5801 0000  .(h.h.((h.h.X...
+00000150: 0033 7120 6809 4b01 7471 2151 4b00 2929  .3q h.K.tq!QK.))
+00000160: 8968 0b29 5271 2274 7123 5271 2468 0f68  .h.)Rq"tq#Rq$h.h
+00000170: 0528 2868 0668 0758 0100 0000 3471 2568  .((h.h.X....4q%h
+00000180: 094b 2074 7126 514b 004b 2085 7127 4b01  .K tq&QK.K .q'K.
+00000190: 8571 2889 680b 2952 7129 7471 2a52 712b  .q(.h.)Rq)tq*Rq+
+000001a0: 6817 6805 2828 6806 6807 5801 0000 0035  h.h.((h.h.X....5
+000001b0: 712c 6809 4b20 7471 2d51 4b00 4b20 8571  q,h.K tq-QK.K .q
+000001c0: 2e4b 0185 712f 8968 0b29 5271 3074 7131  .K..q/.h.)Rq0tq1
+000001d0: 5271 3275 4b02 7d71 3328 6804 6805 2828  Rq2uK.}q3(h.h.((
+000001e0: 6806 6807 5801 0000 0036 7134 6809 4b01  h.h.X....6q4h.K.
+000001f0: 7471 3551 4b00 2929 8968 0b29 5271 3674  tq5QK.)).h.)Rq6t
+00000200: 7137 5271 3868 0f68 0528 2868 0668 0758  q7Rq8h.h.((h.h.X
+00000210: 0100 0000 3771 3968 094d 0004 7471 3a51  ....7q9h.M..tq:Q
+00000220: 4b00 4b20 4b20 8671 3b4b 204b 0186 713c  K.K K .q;K K..q<
+00000230: 8968 0b29 5271 3d74 713e 5271 3f68 1768  .h.)Rq=tq>Rq?h.h
+00000240: 0528 2868 0668 0758 0100 0000 3871 4068  .((h.h.X....8q@h
+00000250: 094d 0004 7471 4151 4b00 4b20 4b20 8671  .M..tqAQK.K K .q
+00000260: 424b 204b 0186 7143 8968 0b29 5271 4474  BK K..qC.h.)RqDt
+00000270: 7145 5271 4675 4b03 7d71 4728 6804 6805  qERqFuK.}qG(h.h.
+00000280: 2828 6806 6807 5801 0000 0039 7148 6809  ((h.h.X....9qHh.
+00000290: 4b01 7471 4951 4b00 2929 8968 0b29 5271  K.tqIQK.)).h.)Rq
+000002a0: 4a74 714b 5271 4c68 0f68 0528 2868 0668  JtqKRqLh.h.((h.h
+000002b0: 0758 0200 0000 3130 714d 6809 4b20 7471  .X....10qMh.K tq
+000002c0: 4e51 4b00 4b20 8571 4f4b 0185 7150 8968  NQK.K .qOK..qP.h
+000002d0: 0b29 5271 5174 7152 5271 5368 1768 0528  .)RqQtqRRqSh.h.(
+000002e0: 2868 0668 0758 0200 0000 3131 7154 6809  (h.h.X....11qTh.
+000002f0: 4b20 7471 5551 4b00 4b20 8571 564b 0185  K tqUQK.K .qVK..
+00000300: 7157 8968 0b29 5271 5874 7159 5271 5a75  qW.h.)RqXtqYRqZu
+00000310: 4b04 7d71 5b28 6804 6805 2828 6806 6807  K.}q[(h.h.((h.h.
+00000320: 5802 0000 0031 3271 5c68 094b 0174 715d  X....12q\h.K.tq]
+00000330: 514b 0029 2989 680b 2952 715e 7471 5f52  QK.)).h.)Rq^tq_R
+00000340: 7160 680f 6805 2828 6806 6807 5802 0000  q`h.h.((h.h.X...
+00000350: 0031 3371 6168 094b 8074 7162 514b 004b  .13qah.K.tqbQK.K
+00000360: 204b 0486 7163 4b04 4b01 8671 6489 680b   K..qcK.K..qd.h.
+00000370: 2952 7165 7471 6652 7167 6817 6805 2828  )RqetqfRqgh.h.((
+00000380: 6806 6807 5802 0000 0031 3471 6868 094b  h.h.X....14qhh.K
+00000390: 8074 7169 514b 004b 204b 0486 716a 4b04  .tqiQK.K K..qjK.
+000003a0: 4b01 8671 6b89 680b 2952 716c 7471 6d52  K..qk.h.)RqltqmR
+000003b0: 716e 754b 057d 716f 2868 0468 0528 2868  qnuK.}qo(h.h.((h
+000003c0: 0668 0758 0200 0000 3135 7170 6809 4b01  .h.X....15qph.K.
+000003d0: 7471 7151 4b00 2929 8968 0b29 5271 7274  tqqQK.)).h.)Rqrt
+000003e0: 7173 5271 7468 0f68 0528 2868 0668 0758  qsRqth.h.((h.h.X
+000003f0: 0200 0000 3136 7175 6809 4b20 7471 7651  ....16quh.K tqvQ
+00000400: 4b00 4b20 8571 774b 0185 7178 8968 0b29  K.K .qwK..qx.h.)
+00000410: 5271 7974 717a 5271 7b68 1768 0528 2868  RqytqzRq{h.h.((h
+00000420: 0668 0758 0200 0000 3137 717c 6809 4b20  .h.X....17q|h.K 
+00000430: 7471 7d51 4b00 4b20 8571 7e4b 0185 717f  tq}QK.K .q~K..q.
+00000440: 8968 0b29 5271 8074 7181 5271 8275 4b06  .h.)Rq.tq.Rq.uK.
+00000450: 7d71 8328 6804 6805 2828 6806 6807 5802  }q.(h.h.((h.h.X.
+00000460: 0000 0031 3871 8468 094b 0174 7185 514b  ...18q.h.K.tq.QK
+00000470: 0029 2989 680b 2952 7186 7471 8752 7188  .)).h.)Rq.tq.Rq.
+00000480: 680f 6805 2828 6806 6807 5802 0000 0031  h.h.((h.h.X....1
+00000490: 3971 8968 094d 0004 7471 8a51 4b00 4b20  9q.h.M..tq.QK.K 
+000004a0: 4b20 8671 8b4b 204b 0186 718c 8968 0b29  K .q.K K..q..h.)
+000004b0: 5271 8d74 718e 5271 8f68 1768 0528 2868  Rq.tq.Rq.h.h.((h
+000004c0: 0668 0758 0200 0000 3230 7190 6809 4d00  .h.X....20q.h.M.
+000004d0: 0474 7191 514b 004b 204b 2086 7192 4b20  .tq.QK.K K .q.K 
+000004e0: 4b01 8671 9389 680b 2952 7194 7471 9552  K..q..h.)Rq.tq.R
+000004f0: 7196 754b 077d 7197 2868 0468 0528 2868  q.uK.}q.(h.h.((h
+00000500: 0668 0758 0200 0000 3231 7198 6809 4b01  .h.X....21q.h.K.
+00000510: 7471 9951 4b00 2929 8968 0b29 5271 9a74  tq.QK.)).h.)Rq.t
+00000520: 719b 5271 9c68 0f68 0528 2868 0668 0758  q.Rq.h.h.((h.h.X
+00000530: 0200 0000 3232 719d 6809 4b20 7471 9e51  ....22q.h.K tq.Q
+00000540: 4b00 4b20 8571 9f4b 0185 71a0 8968 0b29  K.K .q.K..q..h.)
+00000550: 5271 a174 71a2 5271 a368 1768 0528 2868  Rq.tq.Rq.h.h.((h
+00000560: 0668 0758 0200 0000 3233 71a4 6809 4b20  .h.X....23q.h.K 
+00000570: 7471 a551 4b00 4b20 8571 a64b 0185 71a7  tq.QK.K .q.K..q.
+00000580: 8968 0b29 5271 a874 71a9 5271 aa75 4b08  .h.)Rq.tq.Rq.uK.
+00000590: 7d71 ab28 6804 6805 2828 6806 6807 5802  }q.(h.h.((h.h.X.
+000005a0: 0000 0032 3471 ac68 094b 0174 71ad 514b  ...24q.h.K.tq.QK
+000005b0: 0029 2989 680b 2952 71ae 7471 af52 71b0  .)).h.)Rq.tq.Rq.
+000005c0: 680f 6805 2828 6806 6807 5802 0000 0032  h.h.((h.h.X....2
+000005d0: 3571 b168 094b 4074 71b2 514b 004b 024b  5q.h.K@tq.QK.K.K
+000005e0: 2086 71b3 4b20 4b01 8671 b489 680b 2952   .q.K K..q..h.)R
+000005f0: 71b5 7471 b652 71b7 6817 6805 2828 6806  q.tq.Rq.h.h.((h.
+00000600: 6807 5802 0000 0032 3671 b868 094b 4074  h.X....26q.h.K@t
+00000610: 71b9 514b 004b 024b 2086 71ba 4b20 4b01  q.QK.K.K .q.K K.
+00000620: 8671 bb89 680b 2952 71bc 7471 bd52 71be  .q..h.)Rq.tq.Rq.
+00000630: 754b 097d 71bf 2868 0468 0528 2868 0668  uK.}q.(h.h.((h.h
+00000640: 0758 0200 0000 3237 71c0 6809 4b01 7471  .X....27q.h.K.tq
+00000650: c151 4b00 2929 8968 0b29 5271 c274 71c3  .QK.)).h.)Rq.tq.
+00000660: 5271 c468 0f68 0528 2868 0668 0758 0200  Rq.h.h.((h.h.X..
+00000670: 0000 3238 71c5 6809 4b02 7471 c651 4b00  ..28q.h.K.tq.QK.
+00000680: 4b02 8571 c74b 0185 71c8 8968 0b29 5271  K..q.K..q..h.)Rq
+00000690: c974 71ca 5271 cb68 1768 0528 2868 0668  .tq.Rq.h.h.((h.h
+000006a0: 0758 0200 0000 3239 71cc 6809 4b02 7471  .X....29q.h.K.tq
+000006b0: cd51 4b00 4b02 8571 ce4b 0185 71cf 8968  .QK.K..q.K..q..h
+000006c0: 0b29 5271 d074 71d1 5271 d275 4b0a 7d71  .)Rq.tq.Rq.uK.}q
+000006d0: d328 6804 6805 2828 6806 6807 5802 0000  .(h.h.((h.h.X...
+000006e0: 0033 3071 d468 094b 0174 71d5 514b 0029  .30q.h.K.tq.QK.)
+000006f0: 2989 680b 2952 71d6 7471 d752 71d8 680f  ).h.)Rq.tq.Rq.h.
+00000700: 6805 2828 6806 6807 5802 0000 0033 3171  h.((h.h.X....31q
+00000710: d968 094b 2074 71da 514b 004b 014b 2086  .h.K tq.QK.K.K .
+00000720: 71db 4b20 4b01 8671 dc89 680b 2952 71dd  q.K K..q..h.)Rq.
+00000730: 7471 de52 71df 6817 6805 2828 6806 6807  tq.Rq.h.h.((h.h.
+00000740: 5802 0000 0033 3271 e068 094b 2074 71e1  X....32q.h.K tq.
+00000750: 514b 004b 014b 2086 71e2 4b20 4b01 8671  QK.K.K .q.K K..q
+00000760: e389 680b 2952 71e4 7471 e552 71e6 754b  ..h.)Rq.tq.Rq.uK
+00000770: 0b7d 71e7 2868 0468 0528 2868 0668 0758  .}q.(h.h.((h.h.X
+00000780: 0200 0000 3333 71e8 6809 4b01 7471 e951  ....33q.h.K.tq.Q
+00000790: 4b00 2929 8968 0b29 5271 ea74 71eb 5271  K.)).h.)Rq.tq.Rq
+000007a0: ec68 0f68 0528 2868 0668 0758 0200 0000  .h.h.((h.h.X....
+000007b0: 3334 71ed 6809 4b01 7471 ee51 4b00 4b01  34q.h.K.tq.QK.K.
+000007c0: 8571 ef4b 0185 71f0 8968 0b29 5271 f174  .q.K..q..h.)Rq.t
+000007d0: 71f2 5271 f368 1768 0528 2868 0668 0758  q.Rq.h.h.((h.h.X
+000007e0: 0200 0000 3335 71f4 6809 4b01 7471 f551  ....35q.h.K.tq.Q
+000007f0: 4b00 4b01 8571 f64b 0185 71f7 8968 0b29  K.K..q.K..q..h.)
+00000800: 5271 f874 71f9 5271 fa75 7558 0c00 0000  Rq.tq.Rq.uuX....
+00000810: 7061 7261 6d5f 6772 6f75 7073 71fb 5d71  param_groupsq.]q
+00000820: fc7d 71fd 2858 0200 0000 6c72 71fe 473f  .}q.(X....lrq.G?
+00000830: 33a9 2a30 5532 6158 0500 0000 6265 7461  3.*0U2aX....beta
+00000840: 7371 ff47 3fec cccc cccc cccd 473f eff7  sq.G?.......G?..
+00000850: ced9 1687 2b86 7200 0100 0058 0300 0000  ....+.r....X....
+00000860: 6570 7372 0101 0000 473e e4f8 b588 e368  epsr....G>.....h
+00000870: f158 0c00 0000 7765 6967 6874 5f64 6563  .X....weight_dec
+00000880: 6179 7202 0100 004b 0058 0700 0000 616d  ayr....K.X....am
+00000890: 7367 7261 6472 0301 0000 8958 0800 0000  sgradr.....X....
+000008a0: 6d61 7869 6d69 7a65 7204 0100 0089 5807  maximizer.....X.
+000008b0: 0000 0066 6f72 6561 6368 7205 0100 004e  ...foreachr....N
+000008c0: 580a 0000 0063 6170 7475 7261 626c 6572  X....capturabler
+000008d0: 0601 0000 8958 0e00 0000 6469 6666 6572  .....X....differ
+000008e0: 656e 7469 6162 6c65 7207 0100 0089 5805  entiabler.....X.
+000008f0: 0000 0066 7573 6564 7208 0100 004e 5806  ...fusedr....NX.
+00000900: 0000 0070 6172 616d 7372 0901 0000 5d72  ...paramsr....]r
+00000910: 0a01 0000 284b 004b 014b 024b 034b 044b  ....(K.K.K.K.K.K
+00000920: 054b 064b 074b 084b 094b 0a4b 0b65 7561  .K.K.K.K.K.K.eua
+00000930: 752e                                     u.
```

##### archive/data/0

```diff
@@ -1,32 +1 @@
-00000000: df59 a53b 2527 fd3a efb0 05b9 c339 1e39  .Y.;%'.:.....9.9
-00000010: 9f24 023c e280 4b3b befb 09ba 15c4 793a  .$.<..K;......y:
-00000020: 046c 9cba 72ab fc39 a5c1 5a3a c1c4 1aba  .l..r..9..Z:....
-00000030: 4e5a 033b 4d98 e13a 29a9 b339 0795 f1b9  NZ.;M..:)..9....
-00000040: f0d6 aa3b 916e 2b3b 8562 95b9 ea07 9ab9  ...;.n+;.b......
-00000050: d02d e33a f9cc c6b7 f3c1 bcb9 42d4 373a  .-.:........B.7:
-00000060: 4364 233c b852 823b aff1 83ba d748 ab39  Cd#<.R.;.....H.9
-00000070: 2adf 31bc 5226 6ebb 2570 863a df4d a4ba  *.1.R&n.%p.:.M..
-00000080: 6fc2 193b 3d3f 0cbb ed2b 33b9 3568 8b3b  o..;=?...+3.5h.;
-00000090: 38e2 d03b addd 67ba 5d0b 85ba d39e 8b3b  8..;..g.]......;
-000000a0: c027 bdbb 8e99 ffb9 631b 1f3a 8c6f 1abb  .'......c..:.o..
-000000b0: 1b14 9c3c a4d7 d93b ff99 d2ba 298e ff3a  ...<...;....)..:
-000000c0: 964a e4bc 92c3 fabb 47ce 4b3b fa53 72bb  .J......G.K;.Sr.
-000000d0: 4c90 913c 2339 b53b d852 9fba 9234 1d3b  L..<#9.;.R...4.;
-000000e0: 298d 48bc 4edb 6abb add6 7f3a 13fe b0ba  ).H.N.j....:....
-000000f0: dd80 4abb 71fc 8cba 4a7b 9fb9 7798 84ba  ..J.q...J{..w...
-00000100: 24f7 2b3c f450 603b 41b3 28ba 704a 5b3a  $.+<.P`;A.(.pJ[:
-00000110: 1f75 ab39 86ca 503a 477f a639 8a3a 67ba  .u.9..P:G..9.:g.
-00000120: 4fda 9abb fe1f b3ba f3f7 043a 0827 5bb8  O..........:.'[.
-00000130: 980e 94bc 2359 f2bb 8966 973a 33da 75b8  ....#Y...f.:3.u.
-00000140: 9026 223c ceaa 0c38 9225 8fba 67c8 a13b  .&"<...8.%..g..;
-00000150: 2636 3abc 2a48 66bb 7e5c b93a ab1b fcba  &6:.*Hf.~\.:....
-00000160: fb86 ba3b 895c 623b 1a4e c739 8efd 24ba  ...;.\b;.N.9..$.
-00000170: 9055 783b 0b27 203b 0ff6 57ba 035f 43ba  .Ux;.' ;..W.._C.
-00000180: 26d7 303c ac4f 453b ac8e 54ba 7b7e bd3a  &.0<.OE;..T.{~.:
-00000190: bbf2 fa3b 6248 873a 4475 8eba e68b 073b  ...;bH.:Du.....;
-000001a0: db3c 7ebc 40d2 85bb 095a a53a 76a3 fdba  .<~.@....Z.:v...
-000001b0: 8368 ffbb 9421 64ba 49f9 2f3a 0794 5abb  .h...!d.I./:..Z.
-000001c0: 693a ecba bac5 02bb ad24 e337 dbc8 0a3b  i:.......$.7...;
-000001d0: ae5a 383c 6773 623a 0f9a 0dbb 4385 8f3b  .Z8<gsb:....C..;
-000001e0: f4fe 403b 70e9 40b9 bde2 26ba 66d8 c83a  ..@;p.@...&.f..:
-000001f0: 4152 12bd dcc6 3fbc 1155 513b 5a4e 7dbb  AR....?..UQ;ZN}.
+00000000: 0000 7546                                ..uF
```

##### archive/data/1

```diff
@@ -1,32 +1,32 @@
-00000000: f36d 7d39 fad5 e837 dbbd 0637 d7f0 0338  .m}9...7...7...8
-00000010: 7ceb aa3a 95a0 2139 4c31 1b38 3530 3b39  |..:..!9L1.850;9
-00000020: eda0 2639 7bfe f937 33da c836 8d5e 0238  ..&9{..73..6.^.8
-00000030: c40a aa39 7fd6 3e38 c3ab 4437 ad00 7838  ...9..>8..D7..x8
-00000040: 626b 843a 6e6c 0539 1ec7 e737 b880 1839  bk.:nl.9...7...9
-00000050: 0c7f ac38 ed29 3c37 9864 5036 b5f1 7437  ...8.)<7.dP6..t7
-00000060: 27b2 de3a 58ff 4e39 2f5c 4238 636c 5b39  '..:X.N9/\B8cl[9
-00000070: 0927 1d3b a599 7b39 0205 8738 6312 9239  .'.;..{9...8c..9
-00000080: 4b1a e03b b03e 713a cb4b 6039 b9eb 873a  K..;.>q:.K`9...:
-00000090: 4dd7 363b c038 df39 7505 dd38 edaf 053a  M.6;.8.9u..8...:
-000000a0: 466f 293a 923a db38 e919 ea37 974d 0339  Fo):.:.8...7.M.9
-000000b0: 9df7 b63b 7a39 fd39 6676 1039 386d 453a  ...;z9.9fv.98mE:
-000000c0: 79a0 f23b feb8 603a 7df3 5b39 d61a 803a  y..;..`:}.[9...:
-000000d0: c2cc 943b b0d5 ee39 cf6a 1039 71ac 0e3a  ...;...9.j.9q..:
-000000e0: 2afb 9b3a 319b 1f39 1b25 3538 1db1 4739  *..:1..9.%58..G9
-000000f0: 3107 3639 30b5 a937 ae6b 0737 ab0a 3a38  1.690..7.k.7..:8
-00000100: d4ba 533a 419e 8938 0373 ba37 f188 dc38  ..S:A..8.s.7...8
-00000110: c3d2 703a 07dc ee38 1965 ce37 603a 1139  ..p:...8.e.7`:.9
-00000120: db49 a339 1950 8e38 a953 4b37 9df5 5d38  .I.9.P.8.SK7..]8
-00000130: 22fb 993b 4319 1d3a 0678 0d39 54a1 023a  "..;C..:.x.9T..:
-00000140: 1b58 1a3c 58a7 953a 63dd aa39 87d3 c43a  .X.<X..:c..9...:
-00000150: f79b 883a 255c 3939 73bb 0c38 11e3 1939  ...:%\99s..8...9
-00000160: 75a6 003a 953a b238 8248 a337 3cb0 cd38  u..:.:.8.H.7<..8
-00000170: c94d eb3a d80d 6739 e054 6038 bbc4 6739  .M.:..g9.T`8..g9
-00000180: 44dc 8e3a 203a 0e39 cbb3 1f38 3d81 f138  D..: :.9...8=..8
-00000190: 9216 8c3a a101 2a39 467a 2d38 6c5f 4739  ...:..*9Fz-8l_G9
-000001a0: cdc5 2f3b 10e8 b439 a128 b638 42d9 c739  ../;...9.(.8B..9
-000001b0: 1421 0f3b a23b a739 5eb2 9f38 3c41 c039  .!.;.;.9^..8<A.9
-000001c0: c4e8 863a 99a7 4739 1b0f 0d38 cfa5 3539  ...:..G9...8..59
-000001d0: a436 803b 05ed 113a 4815 1c39 f51d 3d3a  .6.;...:H..9..=:
-000001e0: 7d8e 323a ec37 b538 e94e ba37 c66d cd38  }.2:.7.8.N.7.m.8
-000001f0: 275b 6a3c a28d d53a 155c d039 b853 e63a  '[j<...:.\.9.S.:
+00000000: 0e1c 0e3a 3cf5 24ba a30e 57b8 3cdc a43a  ...:<.$...W.<..:
+00000010: 4d5d 24ba de89 0d3a 0573 5c38 fb77 89ba  M]$....:.s\8.w..
+00000020: 0cb6 ed39 0fe3 b4b9 345b 3eb8 239d 233a  ...9....4[>.#.#:
+00000030: c5fa 3ab8 2bf5 6bb8 828b b537 a6c3 0039  ..:.+.k....7...9
+00000040: d322 4d3a 537f 39ba 6aac 87b8 6eaa b03a  ."M:S.9.j...n..:
+00000050: 6962 89b9 8d0a 4439 b3e6 0538 c7b8 c4b9  ib....D9...8....
+00000060: 48a0 08ba 76e1 ef39 adf4 4b38 76fd 67ba  H...v..9..K8v.g.
+00000070: 5dd9 f3b9 62a6 9439 21e8 8038 28ca 07ba  ]...b..9!..8(...
+00000080: 1768 2aba 34c2 063a 4b0f 9b38 e444 83ba  .h*.4..:K..8.D..
+00000090: 9fae 04ba 2da3 d239 68a9 7838 97ed 2dba  ....-..9h.x8..-.
+000000a0: 1f14 2039 e337 13b9 7cad d536 e722 ac39  .. 9.7..|..6.".9
+000000b0: 58ed 17b9 46f6 3039 0dfa 9337 412e 95b9  X...F.09...7A...
+000000c0: d765 04ba 8106 e839 957e 5038 effb 56ba  .e.....9.~P8..V.
+000000d0: 03f4 39ba a97d 233a 2fbf 7038 a9da 9eba  ..9..}#:/.p8....
+000000e0: 477f 9539 b7ab 02b9 6c67 02b8 4829 8139  G..9....lg..H).9
+000000f0: 5f6c 23ba b4eb 363a 5ca8 7e38 6002 a7ba  _l#...6:\.~8`...
+00000100: 0f8b 753a 6b99 64ba d0b9 b7b8 032b d23a  ..u:k.d......+.:
+00000110: 5128 523a cf2e 3dba e723 80b8 ced3 b73a  Q(R:..=..#.....:
+00000120: ec53 6a3a 6f53 45ba 65ae 9cb8 9ddf bc3a  .Sj:oSE.e......:
+00000130: 80c2 f7b9 c1f4 053a 5349 2a38 4b3d 82ba  .......:SI*8K=..
+00000140: e379 30ba 7bcb f239 b9a9 8638 db35 56ba  .y0.{..9...8.5V.
+00000150: 8d3b 9939 f8c2 94b9 ef7c cbb7 873b 0c3a  .;.9.....|...;.:
+00000160: 9162 27ba 48c5 053a aa3a 9138 f2fb 78ba  .b'.H..:.:.8..x.
+00000170: d40a c239 4966 5bb9 7770 2db8 0e21 b239  ...9If[.wp-..!.9
+00000180: 6f39 7e39 516c 56b9 a571 09b8 ce8b c839  o9~9QlV..q.....9
+00000190: 9f4c d5b9 e4c3 d939 a9a3 8038 7594 31ba  .L.....9...8u.1.
+000001a0: ba24 61ba 3d00 3d3a 4e30 9738 6e77 b0ba  .$a.=.=:N0.8nw..
+000001b0: e73f 91b7 f43e 0538 9868 1337 63e3 d7b8  .?...>.8.h.7c...
+000001c0: f3d4 9337 cf11 90b8 c230 4836 8e4f d138  ...7.....0H6.O.8
+000001d0: 6b63 69b9 0003 0139 97ac d537 5fa9 59b9  kci....9...7_.Y.
+000001e0: 3ca3 78b9 f01d 2239 23e2 0e38 d7a2 86b9  <.x..."9#..8....
+000001f0: d07e 3639 15b8 1eb9 c3ed 07b8 305f 8639  .~69........0_.9
```

##### archive/data/10

```diff
@@ -1 +1,8 @@
-00000000: ff81 2bbc 0082 2b3c                      ..+...+<
+00000000: 1412 7eba 2d25 af38 f99e 0639 e01f 2538  ..~.-%.8...9..%8
+00000010: 9705 1d37 c262 8aba a3bf 703a 447d 9839  ...7.b....p:D}.9
+00000020: 4fc0 b0b8 dd14 5cb8 48f1 bb37 19c9 8db9  O.....\.H..7....
+00000030: f5a8 deb9 1f88 dd37 9a5c 4138 b434 2f38  .......7.\A8.4/8
+00000040: 7ed5 b639 0ca3 35b9 ddf4 8b38 b4ab 0f37  ~..9..5....8...7
+00000050: 050c eeb8 b1a2 b0b9 49d0 9737 8695 50ba  ........I..7..P.
+00000060: 2d16 683a 3fec 59b8 3caf 8637 16f9 0ab8  -.h:?.Y.<..7....
+00000070: 7d5f 6c38 3bfa c739 f75a 02b8 0a07 f136  }_l8;..9.Z.....6
```

##### archive/data/11

```diff
@@ -1 +1,8 @@
-00000000: 4007 8c3a 4207 8c3a                      @..:B..:
+00000000: 1217 9039 7d33 b438 9601 7137 6e2d cf37  ...9}3.8..q7n-.7
+00000010: f915 a535 35b8 d039 a7ec ab39 a503 5d38  ...55..9...9..]8
+00000020: 5416 5938 d626 3038 2c2b fa36 cda0 3938  T.Y8.&08,+.6..98
+00000030: 5265 4e38 daaf 0b36 1f51 8137 d276 bb37  ReN8...6.Q.7.v.7
+00000040: 136c 3c38 355d 0d38 6018 ef37 edb3 5d35  .l<85].8`..7..]5
+00000050: cdc9 4a38 4fb9 a838 3fdb 0036 90fc 6939  ..J8O..8?..6..i9
+00000060: 6517 9f39 3bb1 c137 1252 8a36 9d2b f936  e..9;..7.R.6.+.6
+00000070: f304 0436 5d0e 8338 b9ed 0437 ab7f b535  ...6]..8...7...5
```

##### archive/data/12

```diff
@@ -1,8 +1 @@
-00000000: 48fd c2ba b847 08bb f557 f33a b0c7 2e3b  H....G...W.:...;
-00000010: 2205 93b8 e06c 58bb 5edf 663a 2ca1 d139  "....lX.^.f:,..9
-00000020: a8d5 d8b9 ee9b 8139 221d 953a 7850 4cb9  .......9"..:xPL.
-00000030: f483 bbba 7a93 9fba 1f1d 24bb 08fd edba  ....z.....$.....
-00000040: a0ee 183a 9457 16ba 3aab 95ba 74be b93a  ...:.W..:...t..:
-00000050: 8c66 313a e707 b93a 4b0c bc3a 61cc 5ab8  .f1:...:K..:a.Z.
-00000060: e250 13ba 4ace c9b9 62d3 163a 5220 4d3a  .P..J...b..:R M:
-00000070: 4c75 53b9 db53 113a 1c22 073b c427 17bb  LuS..S.:.".;.'..
+00000000: 0000 7546                                ..uF
```

##### archive/data/13

```diff
@@ -1,8 +1,32 @@
-00000000: eb42 c838 c2cd 9739 d945 3638 f8b1 7c39  .B.8...9.E68..|9
-00000010: 31b0 dc38 45d4 3739 69a2 ca38 dd0c 1f39  1..8E.79i..8...9
-00000020: 7976 0839 ebde 0139 7d9a 8337 2310 1c38  yv.9...9}..7#..8
-00000030: e710 f438 8345 4e38 09a4 9b39 3cbc c338  ...8.EN8...9<..8
-00000040: 0015 5a39 4926 2e39 93d2 f038 e8dc cd38  ..Z9I&.9...8...8
-00000050: 7c67 6039 2ade ed38 8585 af38 97f4 5738  |g`9*..8...8..W8
-00000060: 970b 1038 fe27 5d38 bc8a e238 b0b1 ef38  ...8.']8...8...8
-00000070: 0e62 b537 3b6d 5538 37cb a839 943c 8b38  .b.7;mU87..9.<.8
+00000000: 7dcd 1ebb 70e1 b0ba c2c5 29b8 1b4e 3e3b  }...p.....)..N>;
+00000010: 3e01 9cba 9bfd 3cba df97 3bb8 6d92 ca3a  >.....<...;.m..:
+00000020: bf9f bd3a 77ff 4e3a 6099 fe38 cdbc bcba  ...:w.N:`..8....
+00000030: 34c0 5c3b 1342 ed3a 9d9b 0ab8 e030 95bb  4.\;.B.:.....0..
+00000040: 647a e93a 641b 703a af88 ecb7 5692 1cbb  dz.:d.p:....V...
+00000050: be58 33bb a66a b5ba b561 1238 cad9 5a3b  .X3..j...a.8..Z;
+00000060: d805 2d3b 25ec d13a 001a 6636 3b55 73bb  ..-;%..:..f6;Us.
+00000070: 196a 273b aab3 ac3a d954 d1b7 ac99 50bb  .j';...:.T....P.
+00000080: b89a 823b b7fd 0b3b c371 5bb8 6acc aebb  ...;...;.q[.j...
+00000090: f52e b3bb 4fdb 3fbb 88aa 4638 48cc e73b  ....O.?...F8H..;
+000000a0: 18ae f939 df6a a037 7f11 4338 4c5f 6339  ...9.j.7..C8L_c9
+000000b0: b1de 16bb 3f55 b5ba 18f9 2cb8 10ac 513b  ....?U....,...Q;
+000000c0: fb51 45ba 1172 d1b9 1665 15b8 15cb 323a  .QE..r...e....2:
+000000d0: e492 1dbb 9d5f a2ba d823 5738 c8d4 503b  ....._...#W8..P;
+000000e0: 95c8 54bb e376 e1ba 53ef 4938 8d7f 933b  ..T..v..S.I8...;
+000000f0: 6fdc e8ba 1b7b 8dba e85b 0fb7 16ca 253b  o....{...[....%;
+00000100: 9bd7 a53b 290b 363b 3153 80b8 9732 e1bb  ...;).6;1S...2..
+00000110: acb2 903a 4405 e839 e5cb 08b8 edb8 a8ba  ...:D..9........
+00000120: 93d4 60bb e48f f8ba 093c 1338 a65c 9a3b  ..`......<.8.\.;
+00000130: e5ce 223b 0861 953a debc 9338 6648 14bb  ..";.a.:...8fH..
+00000140: ebd5 6e3a eded 093a ff9a 6138 c7a2 5fba  ..n:...:..a8.._.
+00000150: e061 913a e0db 243a 0b89 3838 0955 a1ba  .a.:..$:..88.U..
+00000160: 30f1 7dbb 22a0 02bb d1f3 6b38 956b a33b  0.}.".....k8.k.;
+00000170: ec83 46bb dc6a c1ba cfe4 3338 bfee 6c3b  ..F..j....38..l;
+00000180: 9b43 cd3a 67f9 6a3a d00c b137 3ec0 03bb  .C.:g.j:...7>...
+00000190: cf6b 013b 5e8c 943a dcfc fc36 606e 39bb  .k.;^..:...6`n9.
+000001a0: d843 a1ba c9b7 38ba cbb1 a9b8 c3fb b33a  .C....8........:
+000001b0: 7695 b13b 95b6 433b 99c8 ceb7 dbb7 e7bb  v..;..C;........
+000001c0: 2b86 833a bab1 303a e888 5a38 63eb c1ba  +..:..0:..Z8c...
+000001d0: 2c48 59bb 3aa8 c2ba ae4d 8d38 14b1 803b  ,HY.:....M.8...;
+000001e0: 83d6 e5ba 4e59 2dba ef1e 88b8 4672 a13a  ....NY-.....Fr.:
+000001f0: 9fbe b23a a3e6 1e3a a559 a8b7 2cfb b2ba  ...:...:.Y..,...
```

##### archive/data/14

```diff
@@ -1 +1,32 @@
-00000000: 6dab 673a                                m.g:
+00000000: 1955 9738 c498 4538 6193 4e35 add5 9e38  .U.8..E8a.N5...8
+00000010: 5f5b bd37 840c 9237 150e 9c34 decf ec37  _[.7...7...4...7
+00000020: 5be1 c337 1d98 0238 3139 1635 1305 5938  [..7...819.5..Y8
+00000030: 6453 4939 8c0f c738 ad5a bc35 5c77 1c39  dSI9...8.Z.5\w.9
+00000040: 7bcb 6d38 705a e037 8846 e034 4a0a 3038  {.m8pZ.7.F.4J.08
+00000050: 2a0a d738 d7cd 6438 93ec 6035 9123 b638  *..8..d8..`5.#.8
+00000060: 2bab df38 202f 6b38 5273 5c35 4085 ba38  +..8 /k8Rs\5@..8
+00000070: 6785 ba38 b4f7 4338 5f18 3d35 8cb5 9b38  g..8..C8_.=5...8
+00000080: de29 8439 8c28 0139 9568 eb35 031d 4b39  .).9.(.9.h.5..K9
+00000090: 3537 f139 cba2 7939 7ffd 6d36 18ec c439  57.9..y9..m6...9
+000000a0: b961 ad36 a6a7 3337 5746 3c34 5dc5 9437  .a.6..37WF<4]..7
+000000b0: 00d7 b538 e422 4f38 b445 4d35 9d72 a438  ...8."O8.EM5.r.8
+000000c0: 0747 a736 9936 de36 2c35 f433 d38c 3637  .G.6.6.6,5.3..67
+000000d0: cad6 d938 f57d 5838 c257 4f35 c0ad a938  ...8.}X8.WO5...8
+000000e0: 3dc9 5c39 2148 cf38 0e90 cd35 66dc 2139  =.\9!H.8...5f.!9
+000000f0: 5d96 4538 fce3 ce37 8c90 be34 09c3 2438  ].E8...7...4..$8
+00000100: 857b df39 b040 5d39 e450 4e36 fdda ad39  .{.9.@]9.PN6...9
+00000110: b4fd 2738 27de b037 89e9 c734 18fd 0838  ..'8'..7...4...8
+00000120: 542d 4a39 1255 ca38 e863 ba35 7c2d 1f39  T-J9.U.8.c.5|-.9
+00000130: a1e4 8638 19a0 8138 6f26 9035 523e d238  ...8...8o&.5R>.8
+00000140: 3ddb 1a37 a1a6 4d37 2462 6e34 844a a737  =..7..M7$bn4.J.7
+00000150: e5b7 7637 148c 6437 3bdc 7a34 4f84 b937  ..v7..d7;.z4O..7
+00000160: 6a46 8439 6686 0539 4c3f 0036 f7c2 5139  jF.9f..9L?.6..Q9
+00000170: 7ecf 2539 1b1e ac38 3b79 bb35 9ea1 0839  ~.%9...8;y.5...9
+00000180: 6dd2 0038 747e 8f37 97f2 8e34 be5c e437  m..8t~.7...4.\.7
+00000190: eb35 8e38 24fb 0c38 f61c 0135 d3d3 5e38  .5.8$..8...5..^8
+000001a0: 9ac9 9937 2b7b a237 32c0 b534 3666 0538  ...7+{.72..46f.8
+000001b0: 3bbb d639 b3c0 5d39 4611 4d36 3a8e af39  ;..9..]9F.M6:..9
+000001c0: cd0e 9a37 2975 3f37 794c 4f34 541e 9837  ...7)u?7yLO4T..7
+000001d0: 0fef 5839 51b9 e038 19e8 e535 d90f 3039  ..X9Q..8...5..09
+000001e0: f729 f337 e7a2 1438 aa98 2635 f3a1 7238  .).7...8..&5..r8
+000001f0: 6008 2138 4b3c ca37 a07a eb34 092f 1f38  `.!8K<.7.z.4./.8
```

##### archive/data/15

```diff
@@ -1 +1 @@
-00000000: 5081 e739                                P..9
+00000000: 0000 7546                                ..uF
```

##### archive/data/2

```diff
@@ -1,8 +1,32 @@
-00000000: 2a5f cbba 34f4 aebb 1211 b6ba 982c 37bb  *_..4........,7.
-00000010: 4b96 5abb 4a6f 14ba df9b 9dbb 9c66 883b  K.Z.Jo.......f.;
-00000020: 4593 85bb 2178 42bb bbcb 303b 8cd3 16bc  E...!xB...0;....
-00000030: 67cd 3d3c c58e 04bc 42a9 663b fd2b af3a  g.=<....B.f;.+.:
-00000040: bc85 b0bb b685 c539 4f50 aa38 a781 f73b  .......9OP.8...;
-00000050: 255e d4bb b121 b13b 7c76 a5bb 4008 ccb9  %^...!.;|v..@...
-00000060: 0300 91bb e766 85bb 12d9 c23b 17f3 dc3b  .....f.....;...;
-00000070: 1f39 81ba bf09 acbb 6a11 1abb a844 883c  .9......j....D.<
+00000000: e74d cb39 4dc0 2839 df7b 6536 039f 5739  .M.9M.(9.{e6..W9
+00000010: 6dff a039 4d9c 0239 1de2 3636 7594 2339  m..9M..9..66u.#9
+00000020: a5a2 2c39 9fd4 9238 99f3 cb35 937c ba38  ..,9...8...5.|.8
+00000030: 67e4 f336 3621 2936 a346 9533 54cb 6936  g..66!)6.F.3T.i6
+00000040: 5da1 013a b7a3 5039 30c1 8e36 2925 8339  ]..:..P90..6)%.9
+00000050: 6d54 9238 e691 e937 b4e2 2c35 5775 1338  mT.8...7..,5Wu.8
+00000060: 627a 8139 147b d438 c7aa 1436 080c 0639  bz.9.{.8...6...9
+00000070: 6a2d 5439 2546 af38 117e fe35 5957 de38  j-T9%F.8.~.5YW.8
+00000080: 768f e539 f4e3 3e39 c118 8836 ebce 7039  v..9..>9...6..p9
+00000090: 2eb6 8939 d9eb f038 6e72 2536 7f22 1a39  ...9...8nr%6.".9
+000000a0: 48d7 7836 f0ed e235 1f50 0833 fcf4 1436  H.x6...5.P.3...6
+000000b0: b41a 0938 f376 5737 af97 9434 20cc 8837  ...8.vW7...4 ..7
+000000c0: 346a 7939 80e2 cd38 d019 0c36 3717 0339  4jy9...8...67..9
+000000d0: 5d77 d039 ab72 2939 52bc 6e36 c46a 5439  ]w.9.r)9R.n6.jT9
+000000e0: 7eca 2238 d8a1 7737 ba8a be34 9432 9b37  ~."8..w7...4.2.7
+000000f0: 37b3 053a 5deb 5e39 b514 9936 5146 8e39  7..:].^9...6QF.9
+00000100: 441c 5e3a 31ab b539 a558 f736 0cc6 e639  D.^:1..9.X.6...9
+00000110: 254b fa39 f42c 5039 ca29 8f36 9cab 8239  %K.9.,P9.).6...9
+00000120: 885e 1d3a 967e 7f39 50ef ad36 2206 a139  .^.:.~.9P..6"..9
+00000130: 771c 8139 65f7 c838 541d 0f36 3f0b fd38  w..9e..8T..6?..8
+00000140: d493 9b39 1195 fe38 df77 2b36 120d 2239  ...9...8.w+6.."9
+00000150: 1c5f a838 e974 0638 8286 3c35 078b 2c38  ._.8.t.8..<5..,8
+00000160: 053b cc39 356c 2039 b826 6836 ed0e 4a39  .;.95l 9.&h6..J9
+00000170: 1c88 c238 d054 2138 a870 6335 a6dd 4c38  ...8.T!8.pc5..L8
+00000180: 728e b238 7b03 0e38 d1c1 4e35 0278 3438  r..8{..8..N5.x48
+00000190: e704 a639 4abf 0e39 cd83 4336 3d3a 3939  ...9J..9..C6=:99
+000001a0: 0dc7 0e3a 2c1c 6839 1842 9e36 43ed 9139  ...:,.h9.B.6C..9
+000001b0: e4cc ca36 21bf 1636 4e61 8133 d0ce 3d36  ...6!..6Na.3..=6
+000001c0: 2b1c 4635 06bb bc34 4e8a 9831 f59a ff34  +.F5...4N..1...4
+000001d0: a00b 1938 46b7 6537 0593 a334 8cf9 9137  ...8F.e7...4...7
+000001e0: 0e7b 8438 f49a de37 1df7 1a35 e8b0 0e38  .{.8...7...5...8
+000001f0: 2bfa 8c38 bf43 f037 fbc2 2a35 3a85 1b38  +..8.C.7..*5:..8
```

##### archive/data/3

```diff
@@ -1,8 +1 @@
-00000000: cad8 9138 8103 a339 981b 3c38 c701 a338  ...8...9..<8...8
-00000010: 0676 6539 3374 be37 53a0 ce39 5692 0e3a  .ve93t.7S..9V..:
-00000020: 2e23 b33a 352f 1e3a 26a2 2739 1376 a33a  .#.:5/.:&.'9.v.:
-00000030: 1c33 da3a 5984 963a 2973 bc39 3f29 8738  .3.:Y..:)s.9?).8
-00000040: ff64 4139 82d0 4439 c2d0 cb38 12bd 923a  .dA9..D9...8...:
-00000050: 6aee f93a 1dc3 9439 4f7c 1b39 f28b d439  j..:...9O|.9...9
-00000060: 8826 a039 7ec8 6c39 2b6a 283a 13bc f539  .&.9~.l9+j(:...9
-00000070: d35c 6539 da41 593a c024 1d39 d2cf 5a3b  .\e9.AY:.$.9..Z;
+00000000: 0000 7546                                ..uF
```

##### archive/data/4

```diff
@@ -1,256 +1,8 @@
-00000000: 8916 1839 6d3b 63b8 8349 98b8 9b95 a1b8  ...9m;c..I......
-00000010: c44c e538 5fd7 ba36 4a1c e938 3a7f 00b9  .L.8_..6J..8:...
-00000020: cd22 ce38 f4a8 bc38 3381 21b9 6459 52b9  .".8...83.!.dYR.
-00000030: b865 45b9 23ad 8e39 4412 da36 97c2 5c38  .eE.#..9D..6..\8
-00000040: 8afb 1cb9 0b1e 0239 95d7 68b9 db0a 9bb9  .......9..h.....
-00000050: 390e 72b8 dde2 0438 671c 0eb8 71b1 fbb8  9.r....8g...q...
-00000060: 6d11 9c39 6980 5639 2f01 4d36 c5fb dfb8  m..9i.V9/.M6....
-00000070: 6ebd 03b7 b71b f938 5834 ee38 e807 0bb8  n......8X4.8....
-00000080: 6dd3 e1b9 1d2c 29b8 36f0 2eb9 767c 6bb9  m....,).6...v|k.
-00000090: a7ed 43b9 9129 3cb9 e723 24b9 a169 8939  ..C..)<..#$..i.9
-000000a0: 2920 5e39 5df2 7239 bdcd 47b9 1b6d ab38  ) ^9].r9..G..m.8
-000000b0: c5c3 58b9 319f 86b9 7a95 ebb9 15f8 303a  ..X.1...z.....0:
-000000c0: 5695 343a d7b7 9cb6 34d3 e038 17da 7839  V.4:....4..8..x9
-000000d0: 882e 103a 835d f338 20e8 e5b8 1192 9ab9  ...:.].8 .......
-000000e0: 81eb 93b8 831a a539 8423 00ba 84a3 06ba  .......9.#......
-000000f0: a3cb 8d39 f746 6639 372f 3339 62f9 f038  ...9.Ff97/39b..8
-00000100: b881 123b 4f78 d93a d621 543b 9a26 663a  ...;Ox.:.!T;.&f:
-00000110: 734f f03a 6120 553b d3e8 67ba c535 05bb  sO.:a U;..g..5..
-00000120: d4a8 d538 445c ae3a d36b fcba 225a 58ba  ...8D\.:.k.."ZX.
-00000130: 93d9 c7b9 76e7 cd3a e528 3d3b fa0c 71bb  ....v..:.(=;..q.
-00000140: 7ba7 eeba d70f db3a dc4a 063b 467e 603a  {......:.J.;F~`:
-00000150: b2b9 b1ba c827 2bbb 3918 2a3b fccc d1ba  .....'+.9.*;....
-00000160: b980 fbb9 9f90 7a3a 6e77 1f3b e470 6cba  ......z:nw.;.pl.
-00000170: ee86 173b 3754 b63a 731f ce3a 59d5 5fb7  ...;7T.:s..:Y._.
-00000180: ee4a a3ba 2afd 3aba cc76 c5ba a5ff 9db9  .J..*.:..v......
-00000190: d04d 5eba ef32 ddba 4424 a239 9b38 573a  .M^..2..D$.9.8W:
-000001a0: ba09 a3b9 1060 37ba f53f 6f3a 9a30 453a  .....`7..?o:.0E:
-000001b0: dc2e 8339 f6b3 43ba b2a6 c1ba 0c67 da3a  ...9..C......g.:
-000001c0: 3cab 923a 3045 19ba 0e8f 1aba f4a0 55b9  <..:0E........U.
-000001d0: 1577 d339 76e4 6d3a 2980 b8ba f344 8c3a  .w.9v.m:)....D.:
-000001e0: f701 97b9 610f 1bba 2c06 75ba ddd2 343a  ....a...,.u...4:
-000001f0: 1720 8aba d2a3 46ba 8ae4 7bba 6340 1239  . ....F...{.c@.9
-00000200: e431 193b 8928 023b 56f6 7e3b 566c 8e3a  .1.;.(.;V.~;Vl.:
-00000210: 4d02 053b cf4a 783b a05b bdba 99ae 0cbb  M..;.Jx;.[......
-00000220: 124f bd38 7d72 d03a 85f5 13bb 491f 88ba  .O.8}r.:....I...
-00000230: 610d 9bb8 6b20 a63a 3394 6e3b a090 87bb  a...k .:3.n;....
-00000240: d9bd 0bbb 9235 033b f24c 3d3b 3579 d63a  .....5.;.L=;5y.:
-00000250: cb33 ddba 2bdf 42bb 3e14 3b3b 905b 00bb  .3..+.B.>.;;.[..
-00000260: 0f17 91ba 37b4 953a 12a0 493b 4751 8bba  ....7..:..I;GQ..
-00000270: 195d 413b cbf6 db3a b891 f83a 30e4 e539  .]A;...:...:0..9
-00000280: 1730 2c3b f4ea ed3a f2b9 6f3b 0623 823a  .0,;...:..o;.#.:
-00000290: a77f 043b b202 743b 480b 93ba f793 08bb  ...;..t;H.......
-000002a0: 2fc8 9a39 c488 c23a 5637 08bb 6d91 b3ba  /..9...:V7..m...
-000002b0: 8dd4 feb8 d389 c53a c00e 633b bae8 84bb  .......:..c;....
-000002c0: 0197 20bb 22f0 db3a 8f54 143b 1636 973a  .. ."..:.T.;.6.:
-000002d0: 3bea ceba 1f2a 26bb e2a6 403b 54ca 08bb  ;....*&...@;T...
-000002e0: dbf4 cfb9 cbe4 8f3a 5b7a 383b d28a 94ba  .......:[z8;....
-000002f0: 9936 2c3b 8a44 d23a dd29 003b b248 1839  .6,;.D.:.).;.H.9
-00000300: a5fe 653a fa64 2c3a 10e7 ad3a 334c a239  ..e:.d,:...:3L.9
-00000310: f2e8 3b3a 2d6d b63a 92bc d8b9 5e21 45ba  ..;:-m.:....^!E.
-00000320: a050 0939 383e 1c3a 8eef 56ba 25a1 d9b9  .P.98>.:..V.%...
-00000330: 6005 13b9 ca9f 113a 302e 9a3a 8be0 bdba  `......:0..:....
-00000340: ce03 30ba 5392 273a b16c 573a f1a7 de39  ..0.S.':.lW:...9
-00000350: 842e e6b9 b724 77ba c688 8e3a b026 53ba  .....$w....:.&S.
-00000360: def3 34b9 100b f439 53e1 6f3a a383 05ba  ..4....9S.o:....
-00000370: ae51 833a 5a57 253a 18fb 403a 7af7 2d38  .Q.:ZW%:..@:z.-8
-00000380: 12fb 06ba 52d6 92b9 a877 16ba 3398 43b9  ....R....w..3.C.
-00000390: 0254 bfb9 8f5a 1cba 68dc ce38 0b14 ce39  .T...Z..h..8...9
-000003a0: a4e8 abb7 073a 4bb9 1748 9c39 5f8e 8239  .....:K..H.9_..9
-000003b0: 0757 e137 ae96 b7b9 7354 25ba 1fa4 3d3a  .W.7....sT%...=:
-000003c0: dacb 0c3a dacd 8cb9 1862 83b9 4870 0eb8  ...:.....b..Hp..
-000003d0: ab14 b639 4ae9 d639 cb5c fcb9 22b1 9239  ...9J..9.\.."..9
-000003e0: 1489 10b8 3c5b 0db9 2612 08ba 0b67 b738  ....<[..&....g.8
-000003f0: b75d a9b9 7fcc 63b9 f7e3 93b9 5ae1 1638  .]....c.....Z..8
-00000400: e402 db3a cc9e 863a eba8 063b 5cab 2d3a  ...:...:...;\.-:
-00000410: 863a a43a 7d12 073b 69b1 f1b9 7387 b3ba  .:.:}..;i...s...
-00000420: 1cd0 6937 9084 3a3a 754e 8fba dbb8 41ba  ..i7..::uN....A.
-00000430: 6216 bbb8 4a53 923a 51dc 0c3b 7705 24bb  b...JS.:Q..;w.$.
-00000440: a0aa dfba 2d2e 863a 556c 933a ce63 b139  ....-..:Ul.:.c.9
-00000450: c94b 9dba 3ecd cdba c317 d63a 845b 70ba  .K..>......:.[p.
-00000460: 2812 04b9 c68c fd39 33a4 ef3a 31a8 a1b9  (......93..:1...
-00000470: 84de a43a a110 4c3a c86d 793a 52ae 10b8  ...:..L:.my:R...
-00000480: 8b59 13bb 2a34 efba 9195 68bb dae2 83ba  .Y..*4....h.....
-00000490: 291e f6ba 98ac 65bb d12e a83a 28ff 003b  ).....e....:(..;
-000004a0: d78a f1b8 607f beba 181e 063b 4af7 843a  ....`......;J..:
-000004b0: 5fd0 9138 ff68 a0ba e224 5dbb 144e 7d3b  _..8.h...$]..N};
-000004c0: 09c8 073b 58aa e9ba 05e2 27bb 8de9 b8ba  ...;X.....'.....
-000004d0: a59e c93a 11b3 303b f4dc 2fbb 9d34 ee3a  ...:..0;../..4.:
-000004e0: caa8 6b3a 8af4 87ba 4b20 37bb 07dd 803a  ..k:....K 7....:
-000004f0: c666 2ebb a37e c9ba 7d0c e7ba ca4a b5b9  .f...~..}....J..
-00000500: e416 5139 1149 4e39 edbe c639 e725 c738  ..Q9.IN9...9.%.8
-00000510: f1b8 4039 ac28 c239 5a00 23b9 d20c 48b9  ..@9.(.9Z.#...H.
-00000520: 39dd b537 c5a9 3139 3edd 6fb9 f79b b5b8  9..7..19>.o.....
-00000530: d0f8 6eb7 8a08 cc38 1bb8 a739 5c6c c4b9  ..n....8...9\l..
-00000540: 7f42 1db9 6361 4339 383f 9e39 92a3 4a39  .B..caC98?.9..J9
-00000550: 1e18 fab8 82f6 94b9 5d19 9639 8444 62b9  ........]..9.Db.
-00000560: 697d 05b9 422f 0039 da48 8a39 79ee 15b9  i}..B/.9.H.9y...
-00000570: d763 a339 90e8 3739 2653 4e39 e8f5 3b38  .c.9..79&SN9..;8
-00000580: d799 08ba b48b 3fba 4547 b9ba 085c 97b9  ......?.EG...\..
-00000590: d475 1fba c9ca b1ba 7541 363a e53c 213a  .u......uA6:.<!:
-000005a0: 101a e1b8 d330 39ba 9793 733a 61b2 7339  .....09...s:a.s9
-000005b0: 666c a538 25d7 3bb9 9210 89ba 1cf0 9f3a  fl.8%.;........:
-000005c0: 5489 7839 d863 40ba c343 a6ba f2f1 6eba  T.x9.c@..C....n.
-000005d0: c80e 9639 9a84 8b3a da83 82ba 5bce 623a  ...9...:....[.b:
-000005e0: 0ad4 2a3a 35ee 0eba cab7 63ba 0690 2f3a  ..*:5.....c.../:
-000005f0: 7fb3 aaba 8503 3dba a158 48ba 459f 94b9  ......=..XH.E...
-00000600: e2aa b43a 6f63 853a eb44 073b 08cf 0a3a  ...:oc.:.D.;...:
-00000610: 6460 8e3a 43ed 093b 9705 37ba 1ba5 8eba  d`.:C..;..7.....
-00000620: 351b 4e39 3f29 643a 88cd 9bba de70 4aba  5.N9?)d:.....pJ.
-00000630: a236 54b8 832e 3c3a c9bb 003b 3747 0fbb  .6T...<:...;7G..
-00000640: 5b7b a9ba e181 743a 481a af3a 321c 453a  [{....t:H..:2.E:
-00000650: c26c 51ba f6df b4ba 7204 d63a 6dae a2ba  .lQ.....r..:m...
-00000660: 1dbd a3b9 f451 2d3a 1376 c93a b00a 3bba  .....Q-:.v.:..;.
-00000670: d93e c93a 74c4 753a e103 953a d816 1d39  .>.:t.u:...:...9
-00000680: 17e7 e8b9 1759 14ba f1ad 85ba e931 92b9  .....Y.......1..
-00000690: 33e6 edb9 ad13 72ba e681 e439 72ae 003a  3.....r....9r..:
-000006a0: b42a e1b5 51d6 e3b9 1f52 173a f444 a338  .*..Q....R.:.D.8
-000006b0: 9c84 2c38 bfa0 56b9 d96d 48ba 3854 7a3a  ..,8..V..mH.8Tz:
-000006c0: 2791 8539 a3eb ffb9 5738 6aba fd65 19ba  '..9....W8j..e..
-000006d0: f2a3 8d39 88ef 623a db00 49ba 0e60 fc39  ...9..b:..I..`.9
-000006e0: 4687 e739 334e 89b9 3251 2eba 62bc b539  F..93N..2Q..b..9
-000006f0: 24d2 5dba a5ec e0b9 5fe8 eeb9 604f c6b8  $.]....._...`O..
-00000700: dbb8 fe39 eaea b339 83ab 433a e650 2639  ...9...9..C:.P&9
-00000710: fc1e b839 b487 503a 6309 a5b9 4174 9ab9  ...9..P:c...At..
-00000720: cd51 0a39 f738 b339 3df3 e2b9 d46e c6b9  .Q.9.8.9=....n..
-00000730: 9b9f 1f38 29f4 0039 caef 4c3a b138 47ba  ...8)..9..L:.8G.
-00000740: fd16 12ba 2fbd 9839 53ef 033a 581a c239  ..../..9S..:X..9
-00000750: 0d0a 76b9 05c2 c6b9 6fa5 163a 2c1f 09ba  ..v.....o..:,...
-00000760: 237f 00b9 f52a 9539 f494 0a3a e9e9 b2b9  #....*.9...:....
-00000770: c258 1f3a dc39 c539 1fcd f639 79a0 0739  .X.:.9.9...9y..9
-00000780: d31a a0b9 e974 0aba dc50 6aba 29ae aeb9  .....t...Pj.)...
-00000790: 96f9 9eb9 0461 42ba 2766 d939 7f3f af39  .....aB.'f.9.?.9
-000007a0: 574b e338 d6d1 82b9 3b72 a039 56c2 f4b8  WK.8....;r.9V...
-000007b0: 2850 15b9 3d5b d836 1eb3 28ba eb09 693a  (P..=[.6..(...i:
-000007c0: 4df9 1e39 5b61 92b9 8623 65ba 1839 2eba  M..9[a...#e..9..
-000007d0: 97b0 6d39 56ec 473a c92c 35ba 00ee 8239  ..m9V.G:.,5....9
-000007e0: bd4d 163a e916 4437 a7a7 18ba 7a29 0e39  .M.:..D7....z).9
-000007f0: 57e5 29ba 8b3f 64b9 d16a 83b9 f45e 6db8  W.)..?d..j...^m.
-00000800: b5d8 37b7 4c61 2d39 1700 ab39 25ce 8ab5  ..7.La-9...9%...
-00000810: 082e d338 5779 ac39 5daa 88b9 f1df afb8  ...8Wy.9].......
-00000820: 1a7b a838 4a21 8539 71cf a3b9 0e3a 0bb8  .{.8J!.9q....:..
-00000830: 76ee 86b8 088e 8bb8 bae2 1039 cf5f 2eb9  v..........9._..
-00000840: 4760 2d39 7abe 5f39 09d0 dc39 70b5 c639  G`-9z._9...9p..9
-00000850: 0b38 9938 ac10 73b9 3515 4d39 4040 a0b9  .8.8..s.5.M9@@..
-00000860: 73e5 8bb9 7f6d 7f39 167d c838 ca76 a7b9  s....m.9.}.8.v..
-00000870: 9f1b e839 3a6b 8639 df7b 8039 0215 2539  ...9:k.9.{.9..%9
-00000880: 8bd5 16ba 6520 bab9 ea71 43ba a1e0 8bb9  ....e ...qC.....
-00000890: 4ae2 cab9 bc2b 44ba a9f0 6f39 fd23 c839  J....+D...o9.#.9
-000008a0: 6aa4 0eb6 f5e3 4eb9 4f81 9739 cbfa a039  j.....N.O..9...9
-000008b0: 9b97 0bb9 7330 77b9 fac9 63ba edd2 6c3a  ....s0w...c...l:
-000008c0: 75d3 353a 702b 89b9 764f edb9 c210 87b9  u.5:p+..vO......
-000008d0: 5170 e539 c23e e539 5667 17ba 9b16 b139  Qp.9.>.9Vg.....9
-000008e0: 0637 0839 9e1c bdb8 aa34 34ba 8743 8038  .7.9.....44..C.8
-000008f0: 93f3 dbb9 98d7 6cb9 c878 acb9 ba4a 5ab8  ......l..x...JZ.
-00000900: b166 ac35 6375 67b9 198f cbb9 fb8b 8bb9  .f.5cug.........
-00000910: 2347 9d37 24df 7fb9 3f22 7339 6159 1b36  #G.7$...?"s9aY.6
-00000920: ae02 8539 2651 1439 c9d3 4bb9 917e 9fb9  ...9&Q.9..K..~..
-00000930: 73e2 c6b9 5815 a639 fdba 9bb9 a48a 0e3a  s...X..9.......:
-00000940: a864 1d38 7281 a638 5110 10ba a40a 10ba  .d.8r..8Q.......
-00000950: 7443 3339 1b87 9a39 a240 71b9 4fd3 6ab9  tC39...9.@q.O.j.
-00000960: 3d01 1d3a b154 cf39 a182 a7b9 de20 9eb9  =..:.T.9..... ..
-00000970: 7973 d7b8 c011 4439 0cf3 2e39 30c8 61b8  ys....D9...90.a.
-00000980: ad4c 8b38 8395 7539 2a4d cf39 16ae 4739  .L.8..u9*M.9..G9
-00000990: de0e 9538 5f59 9939 f2f2 5eb9 d291 bab8  ...8_Y.9..^.....
-000009a0: 339f 07b9 f4d5 b837 ce9f 9ab7 f019 2d39  3......7......-9
-000009b0: c5de 3939 188a 07b9 0634 9139 367d e6b9  ..99.....4.96}..
-000009c0: b874 dab7 0b8b 6738 730a f639 49d3 d439  .t....g8s..9I..9
-000009d0: 0c6c f1b8 1afd b0b9 19b6 8f39 19ef a237  .l.........9...7
-000009e0: 9187 d3b9 16c5 1ab9 b30d 8f39 fbd8 9238  ...........9...8
-000009f0: 5df0 7339 d148 ceb6 ecb5 8236 ae5b 3638  ].s9.H.....6.[68
-00000a00: 98de 403a 282f c439 d78e 533a 20de c339  ..@:(/.9..S: ..9
-00000a10: 1f88 dd39 9929 533a 54c8 4cb9 e06a dab9  ...9.)S:T.L..j..
-00000a20: 4a06 8db8 cca0 ac38 2dd6 20b9 8924 bfb9  J......8-. ..$..
-00000a30: c30d 9c39 fa8e 8539 5d2a 8d3a 2a9c 94ba  ...9...9]*.:*...
-00000a40: e91d 83ba 7676 4439 d9fe de39 678b 6939  ....vvD9...9g.i9
-00000a50: f17d 24ba 107a dbb9 20a9 263a 5e95 83b9  .}$..z.. .&:^...
-00000a60: 9f2c 03b9 bb4a a4b8 2ca9 643a f4d1 1139  .,...J..,.d:...9
-00000a70: 4a04 9939 0819 f338 7d53 8c39 15f2 a137  J..9...8}S.9...7
-00000a80: ec50 5a38 b40c 8839 3508 ea39 bb30 7b39  .PZ8...95..9.0{9
-00000a90: bb79 3238 e2a8 a739 39b0 78b9 5946 6eb8  .y28...99.x.YFn.
-00000aa0: 0ebd 35b9 7a5b 0eb8 7f0d 8c38 c3ee 6c39  ..5.z[.....8..l9
-00000ab0: 7b8f 8e39 3972 66b9 a7ca a739 5c95 08ba  {..99rf....9\...
-00000ac0: 71ad 00b8 77aa 84b7 dac0 0b3a 3122 043a  q...w......:1".:
-00000ad0: 9875 00b9 55c7 b1b9 ff24 a839 9916 9138  .u..U....$.9...8
-00000ae0: 9ad6 02ba ae9e 88b9 65b3 9e39 b988 1339  ........e..9...9
-00000af0: 8698 5839 ae5c 97b8 02f3 38b8 adcc fc37  ..X9.\....8....7
-00000b00: b6f1 07ba 7370 44b9 7a26 d2b9 322f 01b9  ....spD.z&..2/..
-00000b10: 1c4c c3b9 4cd0 edb9 a03d 1eb8 9c0d e539  .L..L....=.....9
-00000b20: 7c2f acb7 6a20 2fb9 1126 9e39 0a63 8939  |/..j /..&.9.c.9
-00000b30: 2394 1939 4838 04ba 9efa 00ba aa22 203a  #..9H8......." :
-00000b40: ccbb 0c3a ed0d a0b9 1083 2db8 8fc1 6839  ...:......-...h9
-00000b50: ed78 c239 a52a bb39 e86d b4b9 b236 4939  .x.9.*.9.m...6I9
-00000b60: 8b6d 51b9 e8fa 38b9 02d3 eab9 d996 2838  .mQ...8.......(8
-00000b70: 41f0 4ab9 1c6c 4eb9 7672 6db9 cd9d b238  A.J..lN.vrm....8
-00000b80: 5a69 bf3a 9d2a 713a d4e4 f53a 4e4e 1a3a  Zi.:.*q:...:NN.:
-00000b90: 6232 8f3a 6797 f93a 02fb 01ba bf86 98ba  b2.:g..:........
-00000ba0: 622f 2738 dca1 2b3a 0aba 80ba cf74 37ba  b/'8..+:.....t7.
-00000bb0: 3c80 67b6 cca7 673a e9d2 013b 7655 13bb  <.g...g:...;vU..
-00000bc0: 70cd c6ba 8d3f 693a 2dec 8e3a 3824 eb39  p....?i:-..:8$.9
-00000bd0: f174 88ba ebdd aeba c800 c13a 8160 6dba  .t.........:.`m.
-00000be0: 009e 56b9 157d ea39 f480 d73a 6548 adb9  ..V..}.9...:eH..
-00000bf0: be5c 9b3a 61d5 3c3a 0090 6b3a 4e3b 4338  .\.:a.<:..k:N;C8
-00000c00: b81d e73a 90a3 963a fac7 143b 11d1 473a  ...:...:...;..G:
-00000c10: 17f8 b23a bb5f 123b a0e0 15ba c59e c5ba  ...:._.;........
-00000c20: 5b6d 32b8 e70d 473a e318 9bba b015 41ba  [m2...G:......A.
-00000c30: 3e83 d4b7 9dbe 913a b789 163b 82ed 35bb  >......:...;..5.
-00000c40: 7086 e9ba e585 963a ae2e b43a 9eee 073a  p......:...:...:
-00000c50: bfd5 b3ba 7430 e8ba bdef e43a 7834 7aba  ....t0.....:x4z.
-00000c60: ed92 acb9 4703 f939 5b10 073b 0200 99b9  ....G..9[..;....
-00000c70: fb6b b93a ae70 583a 82ee 823a 4b0c d437  .k.:.pX:...:K..7
-00000c80: 50d1 f53a 8e37 b03a 471c 2c3b 312a 5e3a  P..:.7.:G.,;1*^:
-00000c90: d9ec c53a 845a 283b c4b9 4aba 4045 d9ba  ...:.Z(;..J.@E..
-00000ca0: 27a7 dab7 86ba 743a dd45 b8ba f909 48ba  '.....t:.E....H.
-00000cb0: 6e85 88b7 e05b 933a 05a1 253b 87a9 4bbb  n....[.:..%;..K.
-00000cc0: 9e47 ecba a947 ad3a dcb4 e43a 14c0 533a  .G...G.:...:..S:
-00000cd0: 5037 bcba 3242 06bb d7c0 023b 4c7f 99ba  P7..2B.....;L...
-00000ce0: 5591 12ba 4f89 193a 0883 153b ff24 f7b9  U...O..:...;.$..
-00000cf0: 9a7b e63a 7bee 823a de1f 9b3a 680d e138  .{.:{..:...:h..8
-00000d00: c1e7 0fbb 4da5 daba c74b 57bb 0aee 73ba  ....M....KW...s.
-00000d10: 570d eaba 97fb 57bb 29ae 913a b716 f73a  W.....W.)..:...:
-00000d20: 4150 fdb8 06d2 adba 516c f73a 51a7 833a  AP......Ql.:Q..:
-00000d30: 6ed0 c838 8954 a6ba 2ffc 4ebb 8bef 6f3b  n..8.T../.N...o;
-00000d40: 6f84 043b 05f6 d6ba d23f 14bb e9d3 9bba  o..;.....?......
-00000d50: f524 c13a 1ed8 203b b2ab 25bb e813 df3a  .$.:.. ;..%....:
-00000d60: fadc 383a 9ee7 7aba 650e 2bbb 3fd1 673a  ..8:..z.e.+.?.g:
-00000d70: da2a 1dbb 7d2c b9ba d48d d7ba 42d8 84b9  .*..},......B...
-00000d80: fc93 183a 999b d439 a201 5b3a 516c 8539  ...:...9..[:Ql.9
-00000d90: 93d6 ec39 270c 5b3a 9767 90b9 3b49 f6b9  ...9'.[:.g..;I..
-00000da0: 915b 4f37 3406 9b39 bca1 e4b9 bf3a 9ab9  .[O74..9.....:..
-00000db0: 3e7c 1138 5510 9c39 af95 683a 7988 7bba  >|.8U..9..h:y.{.
-00000dc0: 8b9a 25ba eb06 d039 68b7 123a db04 9d39  ..%....9h..:...9
-00000dd0: ed0e e7b9 f189 17ba bf01 223a bff5 d2b9  ..........":....
-00000de0: e0aa 40b9 a5ad 5539 e1f4 3d3a 3a26 22b9  ..@...U9..=::&".
-00000df0: d084 133a 1dbc a939 7d6c cf39 bff6 a938  ...:...9}l.9...8
-00000e00: 7a76 253a ebfb 303a 3995 a83a f6fc a839  zv%:..0:9..:...9
-00000e10: 179c 1f3a 24c5 a03a f0be 0fba d410 25ba  ...:$..:......%.
-00000e20: 95f2 8b38 798f 173a 0a8b 4bba 8908 8cb9  ...8y..:..K.....
-00000e30: e16d 42b8 9fe4 9939 39df 8a3a 01a5 9fba  .mB....99..:....
-00000e40: 517e eeb9 5949 273a a759 8a3a 5ca2 343a  Q~..YI':.Y.:\.4:
-00000e50: 6a1d ceb9 a3ed 80ba edad 793a 4f46 3cba  j.........y:OF<.
-00000e60: 921e f1b9 e2af d939 8bb5 683a 021e ffb9  .......9..h:....
-00000e70: 89ef 8c3a 4c09 1c3a e786 2c3a 861e 3139  ...:L..:..,:..19
-00000e80: c6e9 e03a 3f24 c83a da36 3c3b 6404 4d3a  ...:?$.:.6<;d.M:
-00000e90: 31e9 c53a 8412 343b b34d 7cba b512 d7ba  1..:..4;.M|.....
-00000ea0: 52f9 b538 c71f a03a 5055 dfba a5f9 1fba  R..8...:PU......
-00000eb0: fba9 85b9 cc52 8e3a 5cf9 1f3b 3307 42bb  .....R.:\..;3.B.
-00000ec0: 0515 afba e9c2 bf3a 8153 073b e24b 8c3a  .......:.S.;.K.:
-00000ed0: a55e 8bba d7c9 1abb cb76 123b 6390 bbba  .^.......v.;c...
-00000ee0: dac6 31ba d873 5f3a f768 083b 363b 6aba  ..1..s_:.h.;6;j.
-00000ef0: 48ce 0f3b 68cb a43a 5331 b63a 4490 f238  H..;h..:S1.:D..8
-00000f00: 23cf 173a c0fe 6b39 13cb 153a e9cb ab39  #..:..k9...:...9
-00000f10: 5374 ac39 8be3 113a f072 ccb8 fb8c c3b9  St.9...:.r......
-00000f20: ff5d 42b9 78e1 9cb8 bbef 25b7 77fc 6fb9  .]B.x.....%.w.o.
-00000f30: 9f91 a939 1ef3 4e39 f5cb 5d3a 5197 87ba  ...9..N9..]:Q...
-00000f40: bce4 69ba 04b4 2f39 ee79 a739 026a 0239  ..i.../9.y.9.j.9
-00000f50: ad25 37ba 5007 a6b9 718d b039 d37a 4238  .%7.P...q..9.zB8
-00000f60: c866 56b9 6415 55b9 69f2 533a 8581 c739  .fV.d.U.i.S:...9
-00000f70: 5b06 a638 be9d 45b8 a59a 2c38 6757 6b38  [..8..E...,8gWk8
-00000f80: 7aec ddba 1600 abba ba42 24bb d1e0 36ba  z........B$...6.
-00000f90: 1e65 b7ba 6ecf 23bb 5156 2e3a edc0 ce3a  .e..n.#.QV.:...:
-00000fa0: c04b 10b8 3750 83ba 6047 be3a 8331 073a  .K..7P..`G.:.1.:
-00000fb0: 27dc a039 3e35 9fba 2e93 0dbb 8640 3c3b  '..9>5.......@<;
-00000fc0: 7eee a83a 117a a6ba 8d9c d0ba 908e 2dba  ~..:.z........-.
-00000fd0: 0240 843a 6e8b 083b 607f 05bb ab98 983a  .@.:n..;`......:
-00000fe0: 9fcf d339 4e24 30ba f45b f1ba b64b 2c3a  ...9N$0..[...K,:
-00000ff0: ca2a e7ba 8e43 87ba 9da1 97ba abab 8738  .*...C.........8
+00000000: a644 2c3b c293 37bb ad15 003b ef33 adb9  .D,;..7....;.3..
+00000010: e76c 633b 9941 a3ba 475a 1abb d065 0cbb  .lc;.A..GZ...e..
+00000020: 45c9 45bb 1266 13bb 1b8d 0a3a 3332 43ba  E.E..f.....:32C.
+00000030: dd1e 14bb 5d7f 4ebb aec5 9e3a 86d9 41bb  ....].N....:..A.
+00000040: bbcf 893b 0c62 663b 0d11 7e3b 8a34 15bb  ...;.bf;..~;.4..
+00000050: 4bd0 39bb 9c27 aa3a 6d20 42bb 33ec ce3a  K.9..'.:m B.3..:
+00000060: 0b99 9f3a 1592 06bb ad7b 74bb 7009 4fb9  ...:.....{t.p.O.
+00000070: c9a9 4138 9072 79ba 96c9 92ba 0b11 7a3a  ..A8.ry.......z:
```

##### archive/data/5

```diff
@@ -1,256 +1,8 @@
-00000000: 05d0 5b37 5656 d836 435e 8f37 2a09 4036  ..[7VV.6C^.7*.@6
-00000010: 1ac7 c436 8b57 cd37 c350 6b36 0389 cd36  ...6.W.7.Pk6...6
-00000020: 1453 b034 0b64 1a36 a91a 7a36 add3 5736  .S.4.d.6..z6..W6
-00000030: b28f f535 6fb4 c836 0a47 8437 0fb9 d537  ...5o..6.G.7...7
-00000040: 902c 2237 b4f6 4436 c395 1937 d975 d736  .,"7..D6...7.u.6
-00000050: c1eb 3136 f02f 5237 936d 9437 0f3d 1137  ..16./R7.m.7.=.7
-00000060: 6687 9936 7a82 3c35 e14d 1537 85ce 5736  f..6z.<5.M.7..W6
-00000070: d2f1 0d37 b328 2436 9e15 d736 917b 1836  ...7.($6...6.{.6
-00000080: cae7 3236 9f17 5c35 a132 3536 3c50 0135  ..26..\5.256<P.5
-00000090: e6ae 8b35 d8da af36 7f5c 3835 3675 9f35  ...5...6.\856u.5
-000000a0: 8483 b334 4a9f 2835 00c2 7035 4dbb 7635  ...4J.(5..p5M.v5
-000000b0: 18f4 3335 4ac4 c735 29c6 3e36 89a2 b136  ..35J..5).>6...6
-000000c0: 0ef7 3636 b919 3335 0d1c d335 71ce b535  ..66..35...5q..5
-000000d0: c9e0 df35 8261 f735 48d5 3c36 e4a4 1736  ...5.a.5H.<6...6
-000000e0: 630b aa35 3d85 1935 cc17 0636 b3c6 d435  c..5=..5...6...5
-000000f0: a598 dd35 750c 3935 cff4 bd35 e558 0b35  ...5u.95...5.X.5
-00000100: 53dc 1c38 8f02 bd37 6db0 7338 b3e4 2537  S..8...7m.s8..%7
-00000110: a019 9337 5849 9d38 d03d 5c37 4abd 9537  ...7XI.8.=\7J..7
-00000120: 123d ad35 a247 0d37 edcb 5937 1299 2537  .=.5.G.7..Y7..%7
-00000130: ae70 9b36 8c3c 6d37 4da6 5738 14b5 a538  .p.6.<m7M.W8...8
-00000140: fa85 f537 d94d 2d37 2adb 1438 e065 c237  ...7.M-7*..8.e.7
-00000150: 62e3 2b37 fbbe 3238 472c 6638 32f5 e937  b.+7..28G,f82..7
-00000160: 225c 8237 8730 2c36 e09d 0638 3369 3e37  "\.7.0,6...83i>7
-00000170: 4a07 0538 87c3 0f37 3f3c ab37 ae5d ad36  J..8...7?<.7.].6
-00000180: 1784 ac37 b090 b336 b7d6 8637 e8d4 2336  ...7...6...7..#6
-00000190: 7532 f936 0ff7 f837 b764 ed35 ceb5 0837  u2.6...7.d.5...7
-000001a0: 6d31 b735 1ab8 4a36 60e6 9136 33fe ce36  m1.5..J6`..63..6
-000001b0: e785 f535 b617 2737 97db 9537 7ff5 0638  ...5..'7...7...8
-000001c0: 77c2 9b37 4f0b 4136 ab61 b936 3404 8d36  w..7O.A6.a.64..6
-000001d0: 8497 d336 a3e7 4437 1cdb b137 6a5b 5937  ...6..D7...7j[Y7
-000001e0: 30b1 b736 bbb0 0936 b230 1237 abef f136  0..6...6.0.7...6
-000001f0: 43be f336 4e22 5e36 8d26 0f37 f1a0 7d36  C..6N"^6.&.7..}6
-00000200: feb3 d338 b40d 8f38 7ed9 2d39 607d 0238  ...8...8~.-9`}.8
-00000210: 5e17 3d38 a4a4 6039 fe85 2e38 ddae 3138  ^.=8..`9...8..18
-00000220: 0613 bd36 5d55 d737 1565 0e38 faff ef37  ...6]U.7.e.8...7
-00000230: ea51 4c37 fac3 db37 b85b 1a39 3e95 6439  .QL7...7.[.9>.d9
-00000240: 0a63 b538 bea7 da37 7398 e738 cba8 9838  .c.8...7s..8...8
-00000250: 0902 1438 f668 0039 00a4 2939 0dda bd38  ...8.h.9..)9...8
-00000260: 8dfe 3f38 9969 1337 9d10 c238 8d2f 3b38  ..?8.i.7...8./;8
-00000270: d80b cb38 e63b d437 7519 8338 a9cc 7237  ...8.;.7u..8..r7
-00000280: 9695 9b38 a5d4 0338 aad9 af38 d7fe 6937  ...8...8...8..i7
-00000290: 11b0 fe37 5b4b 0539 a6c7 2837 239e 0738  ...7[K.9..(7#..8
-000002a0: a78d 6b36 d335 5537 3c1c a037 377c 9537  ..k6.5U7<..77|.7
-000002b0: b198 9d36 50f4 de37 c372 a538 f1f4 0c39  ...6P..7.r.8...9
-000002c0: 9e9e 7538 af4c 7337 e779 1538 9305 8a37  ..u8.Ls7.y.8...7
-000002d0: cc9e a937 defe 8838 5075 c538 7587 4d38  ...7...8Pu.8u.M8
-000002e0: b472 6337 27aa cb36 046e 3338 44fa ce37  .rc7'..6.n38D..7
-000002f0: 80a8 2438 ff78 5e37 8d8f 1138 a95f 3637  ..$8.x^7...8._67
-00000300: 1c9e 1a37 20cd da36 6dac 7737 efd3 4236  ...7 ..6m.w7..B6
-00000310: 3e9e 8a36 42d6 a637 311e 7536 fd04 8c36  >..6B..71.u6...6
-00000320: ffac 9834 1ad9 0b36 e070 3f36 75c7 f135  ...4...6.p?6u..5
-00000330: 1fe3 a435 bcd2 6536 a552 4c37 89a5 a337  ...5..e6.RL7...7
-00000340: d0e2 d136 27f9 1e36 e8a9 2437 7e13 db36  ...6'..6..$7~..6
-00000350: 5488 fd35 ff3d 5237 62ad 7f37 c0e1 ee36  T..5.=R7b..7...6
-00000360: aaf5 8e36 b73c 3335 2f2f e636 7656 6c36  ...6.<35//.6vVl6
-00000370: 549f 0a37 47b8 0336 e704 b136 033e f735  T..7G..6...6.>.5
-00000380: f8a5 7736 9b3e 0a36 02fd b136 4071 7735  ..w6.>.6...6@qw5
-00000390: cf1f db35 fe71 f936 b597 9d35 a321 de35  ...5.q.6...5.!.5
-000003a0: 09c9 2e34 5d2a 5435 cd88 9b35 5038 8135  ...4]*T5...5P8.5
-000003b0: ccf4 0f35 e4b5 c835 ac36 9f36 afe1 f936  ...5...5.6.6...6
-000003c0: cff0 3f36 0de4 6b35 55d6 4f36 6c9f 0c36  ..?6..k5U.O6l..6
-000003d0: ce6c 8535 96b9 8236 2fe4 b436 b508 4236  .l.5...6/..6..B6
-000003e0: a801 c135 d89b a634 4b48 3a36 5277 b135  ...5...4KH:6Rw.5
-000003f0: d711 3f36 1dc1 5a35 607a 0936 4513 2735  ..?6..Z5`z.6E.'5
-00000400: b185 0738 bb75 9137 c259 4538 118c 0337  ...8.u.7.YE8...7
-00000410: 413a 7137 d0de 8538 7f81 2f37 ccb1 6f37  A:q7...8../7..o7
-00000420: 145f df35 541b f336 158d 3437 d956 2537  ._.5T..6..47.V%7
-00000430: 4e73 9b36 83e9 4f37 6037 3738 c6cc 8938  Ns.6..O7`778...8
-00000440: 42ea e637 cd70 0337 ecce e637 cd35 9c37  B..7.p.7...7.5.7
-00000450: 1295 2c37 0db5 0438 baa0 4038 2afd dd37  ..,7...8..@8*..7
-00000460: 2424 5737 44e0 4736 cf4b e137 eabf 4337  $$W7D.G6.K.7..C7
-00000470: 0d45 d637 630b 0037 8a80 9937 0808 9336  .E.7c..7...7...6
-00000480: 03df cc38 bf77 8638 54aa 2439 1c79 f237  ...8.w.8T.$9.y.7
-00000490: 8073 3638 71d8 5739 39f6 1d38 4181 2c38  .s68q.W99..8A.,8
-000004a0: 608a af36 673e ca37 b40f 0738 22f6 e437  `..6g>.7...8"..7
-000004b0: 6d92 1e37 4fff c637 24fe 1139 957b 5b39  m..7O..7$..9.{[9
-000004c0: ab2b ac38 1732 cf37 ed6a d638 4caa 8938  .+.8.2.7.j.8L..8
-000004d0: 02df 0a38 864f f338 9709 2239 672a b438  ...8.O.8.."9g*.8
-000004e0: 7b0c 2a38 e0e1 0737 7a2d b538 71ff 2f38  {.*8...7z-.8q./8
-000004f0: eef8 bd38 0c9b c837 fa5d 7938 370d 6337  ...8...7.]y87.c7
-00000500: 017b 8435 4893 1635 c7c4 bb35 4b1d 8d34  .{.5H..5...5K..4
-00000510: 31d5 e634 3450 0636 a228 b334 7998 f334  1..44P.6.(.4y..4
-00000520: 69bb 3533 16af 5734 ae58 9d34 8480 7a34  i.53..W4.X.4..z4
-00000530: 8e0b 3534 8162 e834 eaa5 a635 aa66 0836  ..54.b.4...5.f.6
-00000540: e628 4e35 715c 8234 503e 6835 82fc 2335  .(N5q\.4P>h5..#5
-00000550: 9cb3 9834 e514 9635 e415 c035 d8a5 4135  ...4...5...5..A5
-00000560: 029d e234 0821 b633 2cc3 4635 0b7f bf34  ...4.!.3,.F5...4
-00000570: 7051 4a35 b8d1 5634 4b38 0c35 95c6 4234  pQJ5..V4K8.5..B4
-00000580: 8ffb f137 7029 8237 c63d 2638 7448 f336  ...7p).7.=&8tH.6
-00000590: 5ac3 5237 2c1f 7538 be2c 1d37 ea65 5937  Z.R7,.u8.,.7.eY7
-000005a0: 51f8 a235 da39 bf36 e06e 0e37 1e33 ea36  Q..5.9.6.n.7.3.6
-000005b0: 789e a636 eb17 4e37 a920 1638 20e1 7438  x..6..N7. .8 .t8
-000005c0: 2362 bb37 5a38 eb36 06e8 ca37 60d8 8e37  #b.7Z8.6...7`..7
-000005d0: 3d59 0337 08fc 0138 2e28 2b38 8e2e b037  =Y.7...8.(+8...7
-000005e0: b396 4e37 64e5 1336 0022 b137 4c66 2137  ..N7d..6.".7Lf!7
-000005f0: 7f58 b337 228f c336 29d8 7d37 04c4 be36  .X.7"..6).}7...6
-00000600: 73a3 b637 862e 3037 58dc d837 becb 9f36  s..7..07X..7...6
-00000610: 1ac0 1037 275e 2238 c501 9736 ec2f 1737  ...7'^"8...6./.7
-00000620: 8cd4 a735 fce4 8936 cd80 ba36 aee9 b836  ...5...6...6...6
-00000630: ee3b 0036 54cb 0237 cb55 c737 94e0 2738  .;.6T..7.U.7..'8
-00000640: fb46 9537 6623 8f36 e2a4 6a37 2889 0a37  .F.7f#.6..j7(..7
-00000650: 3a79 d836 a8ea b037 27bc f537 c396 8337  :y.6...7'..7...7
-00000660: fcad d336 a79c 0a36 98c4 5837 5393 1237  ...6...6..X7S..7
-00000670: 3b50 6037 1a3b 8936 11cd 3537 6ae8 7936  ;P`7.;.6..57j.y6
-00000680: bfce 3637 8ed9 c536 6b37 7b37 cf15 3736  ..67...6k7{7..76
-00000690: 93ab 9f36 e731 b537 64a2 6f36 f466 a636  ...6.1.7d.o6.f.6
-000006a0: ca26 bf34 c3d3 0836 248e 4f36 0437 3236  .&.4...6$.O6.726
-000006b0: 67fe fa35 740a a636 1c42 6437 15be b737  g..5t..6.Bd7...7
-000006c0: 140b 0c37 6bfb 2d36 e682 1737 0e31 dc36  ...7k.-6...7.1.6
-000006d0: 18e0 3136 b897 4237 9a60 8137 af98 0037  ..16..B7.`.7...7
-000006e0: adfc 9936 23bb 3e35 e3c0 0337 2212 5d36  ...6#.>5...7".]6
-000006f0: 95da 0337 c7dd 0a36 cc8e bb36 5022 0c36  ...7...6...6P".6
-00000700: 43bf aa36 3fab ba35 ad45 7336 8a2d 5e35  C..6?..5.Es6.-^5
-00000710: 82d4 e335 4efa f136 6f78 4d35 eea2 1036  ...5N..6oxM5...6
-00000720: 482f 8635 2b19 ac35 4292 b935 a04d 0136  H/.5+..5B..5.M.6
-00000730: b21a 8935 ff5a 3b36 d016 8d36 7b25 0f37  ...5.Z;6...6{%.7
-00000740: d89d ce36 077a 8835 6e1d 2036 042b 0336  ...6.z.5n. 6.+.6
-00000750: e71f 8b36 9014 6d36 1da3 ab36 77b8 9936  ...6..m6...6w..6
-00000760: 4ff6 2936 1940 a735 a2b7 5c36 dbb3 8b36  O.)6.@.5..\6...6
-00000770: ef4b 2d36 cadb ab35 ada4 2a36 1a14 8835  .K-6...5..*6...5
-00000780: d5e3 a637 7d0e 2c37 f8f9 e137 f023 9c36  ...7}.,7...7.#.6
-00000790: bb1b 1637 63a7 2038 8386 c636 7f9c 1c37  ...7c. 8...6...7
-000007a0: b833 1435 5c13 7036 da6e c036 cd1f a636  .3.5\.p6.n.6...6
-000007b0: 4ada 5636 2eff 1937 1c4e cf37 4870 2638  J.V6...7.N.7Hp&8
-000007c0: 91f5 7837 b92d 9d36 0df5 7d37 e6c3 3537  ..x7.-.6..}7..57
-000007d0: cda2 9236 b2ce a737 daa5 e637 afff 6137  ...6...7...7..a7
-000007e0: 5979 0037 38ac 9335 f9f8 6e37 14f3 aa36  Yy.78..5..n7...6
-000007f0: 4b5b 6337 24d8 7b36 30df 2637 04be 7136  K[c7$.{60.&7..q6
-00000800: de4a 8f36 4f25 ea35 81e7 b036 aa71 5e35  .J.6O%.5...6.q^5
-00000810: db31 f535 3b4a 0a37 27b5 a635 d50f 0636  .1.5;J.7'..5...6
-00000820: a964 b634 8b80 8235 a7a2 c935 f2ba b535  .d.4...5...5...5
-00000830: d70e 8335 69fe 2236 1414 a636 9e50 0c37  ...5i."6...6.P.7
-00000840: d6d8 7c36 ce7a 8e35 72d4 4736 cc1b 2336  ..|6.z.5r.G6..#6
-00000850: 2688 df35 a26c 6c36 6235 b136 4126 6136  &..5.ll6b5.6A&a6
-00000860: 7571 0836 bbed 2e35 6746 4f36 681e f135  uq.6...5gFO6h..5
-00000870: 45e5 4436 59cf 8d35 9ac6 1736 a1c7 5735  E.D6Y..5...6..W5
-00000880: a0dc ac36 1006 4836 898b fe36 d0ce bc35  ...6..H6...6...5
-00000890: 983f 1236 5e66 3437 7a2f fd35 9ae3 1236  .?.6^f47z/.5...6
-000008a0: 5af4 f434 65a9 b235 9e49 e735 b894 d235  Z..4e..5.I.5...5
-000008b0: 509e 7e35 20db 0136 3ea2 e636 d9b1 3237  P.~5 ..6>..6..27
-000008c0: 4e54 9c36 408c ab35 143f a336 4397 6336  NT.6@..5.?.6C.c6
-000008d0: 8d5c 1636 8619 bb36 374a 0237 495c a536  .\.6...67J.7I\.6
-000008e0: fcae 1b36 2f57 3c35 17f9 9136 e17b 3d36  ...6/W<5...6.{=6
-000008f0: dbd8 9636 14f8 b435 9246 5836 1b38 6835  ...6...5.FX6.8h5
-00000900: 51ca 2338 3ab7 a537 8175 5938 692c 1337  Q.#8:..7.uY8i,.7
-00000910: 8e3a 9337 8bef 9938 77f1 3837 a1ab 9837  .:.7...8w.87...7
-00000920: f3ba 8735 7f5e ed36 b7f8 3d37 6d6e 2337  ...5.^.6..=7mn#7
-00000930: bcc9 c036 6958 9537 e3cf 4738 be8f 9f38  ...6iX.7..G8...8
-00000940: db03 f137 b828 1437 4997 ed37 6c94 a837  ...7.(.7I..7l..7
-00000950: a1ad 0137 157a 1f38 90e5 6038 49bd df37  ...7.z.8..`8I..7
-00000960: 9259 6b37 a370 1436 2b66 e137 0b51 2837  .Yk7.p.6+f.7.Q(7
-00000970: 0cb2 da37 ca1e fc36 a1cc a437 008e e836  ...7...6...7...6
-00000980: 6b43 5e37 051c e536 5236 9537 21dd 4c36  kC^7...6R6.7!.L6
-00000990: 0135 c836 5dd7 d337 41e5 8036 5ae9 d036  .5.6]..7A..6Z..6
-000009a0: 7469 be34 981d 2136 31bb 8036 5fcb 5936  ti.4..!61..6_.Y6
-000009b0: a37a 0a36 6c41 ce36 100f 8837 0995 da37  .z.6lA.6...7...7
-000009c0: 0f80 2237 af53 4d36 958e 2537 7101 ec36  .."7.SM6..%7q..6
-000009d0: 56c3 3336 638c 5e37 e519 9a37 cf2f 1737  V.36c.^7...7./.7
-000009e0: 08a9 a536 b2a9 4935 060b 1a37 94dd 6636  ...6..I5...7..f6
-000009f0: 4a12 1637 b586 2936 7c9a df36 3aef 2136  J..7..)6|..6:.!6
-00000a00: f0b7 0137 2e94 b036 ee7d 5b37 ad49 2736  ...7...6.}[7.I'6
-00000a10: 5539 6936 31e6 9937 88d0 7b36 10c3 7336  U9i61..7..{6..s6
-00000a20: b9fc 7835 b206 2936 879b 5736 c662 1f36  ..x5..)6..W6.b.6
-00000a30: f9c4 0136 45f4 5e36 fdf3 3937 3e64 9437  ...6E.^6..97>d.7
-00000a40: 2496 f136 389a 2736 3cfb 1c37 a72b e036  $..68.'6<..7.+.6
-00000a50: fcc5 9536 2919 2c37 e4cc 5437 6949 0c37  ...6).,7..T7iI.7
-00000a60: cedc 9f36 2c6b c635 976f 0137 d033 b836  ...6,k.5.o.7.3.6
-00000a70: a13a 0e37 5a65 2736 c784 b636 3c9d ce35  .:.7Ze'6...6<..5
-00000a80: 775b fc37 61be 8037 6a8c 2638 852e e736  w[.7a..7j.&8...6
-00000a90: 2059 6037 45f8 6e38 c288 0e37 3840 6937   Y`7E.n8...78@i7
-00000aa0: e519 4f35 8375 b336 d4e7 0d37 cf23 f536  ..O5.u.6...7.#.6
-00000ab0: 1b96 9936 7df0 6737 f9c2 1838 000c 7638  ...6}.g7...8..v8
-00000ac0: dff6 b837 7563 e236 8e03 b737 76a8 8237  ...7uc.6...7v..7
-00000ad0: 8091 c836 f7f3 f837 ef46 2e38 f45f aa37  ...6...7.F.8._.7
-00000ae0: 7fa0 3737 7d1e e135 b467 aa37 5926 0337  ..77}..5.g.7Y&.7
-00000af0: a0bf a637 8adf bb36 db81 7b37 c020 ba36  ...7...6..{7. .6
-00000b00: 4781 7637 701b 0837 3eff a837 844d 7536  G.v7p..7>..7.Mu6
-00000b10: 01ea d436 0311 f437 675f 8e36 1040 d636  ...6...7g_.6.@.6
-00000b20: 6f01 c334 50e7 3136 e6ef 8236 1dae 5f36  o..4P.16...6.._6
-00000b30: 0103 0036 e410 bf36 3abc 9737 87ae f237  ...6...6:..7...7
-00000b40: ab1d 3137 e825 4f36 810f 3f37 fe8f fd36  ..17.%O6..?7...6
-00000b50: ae31 3736 79bf 8137 415b b437 367c 2f37  .176y..7A[.76|/7
-00000b60: c795 a636 1d72 5535 f02f 2337 054e 9136  ...6.rU5./#7.N.6
-00000b70: 7930 2b37 12ec 3436 b760 0037 1da4 3736  y0+7..46.`.7..76
-00000b80: 673d 1a38 fbaa b937 e944 6138 1570 2637  g=.8...7.Da8.p&7
-00000b90: f270 8437 1170 9d38 91b4 4337 8380 8137  .p.7.p.8..C7...7
-00000ba0: 5f05 d235 aaf7 0437 73e8 3437 1b1e 1637  _..5...7s.47...7
-00000bb0: f401 8b36 6c0c 4237 7597 4638 1787 9b38  ...6l.B7u.F8...8
-00000bc0: a86a eb37 66de 0937 8f5b 0738 d2fb aa37  .j.7f..7.[.8...7
-00000bd0: bb54 1c37 50ed 2d38 ff93 6c38 729a f837  .T.7P.-8..l8r..7
-00000be0: ff65 5a37 b460 3f36 ed45 e037 1b3f 7037  .eZ7.`?6.E.7.?p7
-00000bf0: 3f2a f537 ec62 0437 3d4d af37 9d44 d436  ?*.7.b.7=M.7.D.6
-00000c00: 299e 1438 82f3 ae37 0bb3 5738 6fc6 1837  )..8...7..W8o..7
-00000c10: df44 8337 5e0e 9438 d401 3337 1fd8 8337  .D.7^..8..37...7
-00000c20: fc05 b435 dbb9 0137 ab89 3837 8488 0a37  ...5...7..87...7
-00000c30: c30e 6136 6cf1 4437 353b 3d38 3f60 9638  ..a6l.D75;=8?`.8
-00000c40: 9c94 e237 492b 0e37 3274 fe37 eb54 9c37  ...7I+.72t.7.T.7
-00000c50: 5ae1 1e37 484d 2638 86cf 5d38 b03b e137  Z..7HM&8..]8.;.7
-00000c60: cd29 4c37 df27 3536 3649 db37 8a79 5937  .)L7.'566I.7.yY7
-00000c70: 4940 ea37 9b04 0137 cb4c a237 f0fe bb36  I@.7...7.L.7...6
-00000c80: e01e 0c38 7742 b037 06a6 5638 d1c5 1737  ...8wB.7..V8...7
-00000c90: 0a5a 8037 dae3 8e38 aea0 3837 12b0 8137  .Z.7...8..87...7
-00000ca0: f9eb 9a35 b74c 0337 3112 3b37 65ef fb36  ...5.L.71.;7e..6
-00000cb0: 49df 4736 2add 3137 60ca 3738 75c7 9238  I.G6*.17`.78u..8
-00000cc0: 5e83 d537 b6b7 1137 d878 0338 2fd1 9e37  ^..7...7.x.8/..7
-00000cd0: 8cc8 1f37 6fc9 2838 3351 5538 e5bc d137  ...7o.(83QU8...7
-00000ce0: af0a 4d37 470f 2436 e97c de37 8108 4d37  ..M7G.$6.|.7..M7
-00000cf0: f676 f037 48ad 0037 8b78 9a37 ea0f ac36  .v.7H..7.x.7...6
-00000d00: 6336 9a38 2360 4d38 2cae f838 288b b537  c6.8#`M8,..8(..7
-00000d10: 8a32 0b38 650a 2339 2598 e237 2c74 0638  .2.8e.#9%..7,t.8
-00000d20: 149e 7636 f290 9937 0466 cf37 7bca 9f37  ..v6...7.f.7{..7
-00000d30: 228d e236 5729 9437 b4bb d738 b17e 2539  "..6W).7...8.~%9
-00000d40: bd8e 7838 5b36 a137 fc00 9f38 2cfa 4238  ..x8[6.7...8,.B8
-00000d50: 0949 c737 1dd4 bd38 c12f f638 882f 8438  .I.7...8./.8./.8
-00000d60: ffac e937 18d1 ca36 b899 8438 3381 0338  ...7...6...83..8
-00000d70: cfad 8e38 70db 9637 45a2 3938 9fe3 2e37  ...8p..7E.98...7
-00000d80: c1c7 1037 12f6 b336 0ad1 5337 6af8 2636  ...7...6..S7j.&6
-00000d90: bdb0 6a36 6f7b 9337 891e 4836 0cbb 5936  ..j6o{.7..H6..Y6
-00000da0: b783 ff34 34b7 0136 ddad 1f36 fac2 1a36  ...44..6...6...6
-00000db0: 8f6e 9335 1442 2636 953c 3e37 0fe8 8f37  .n.5.B&6.<>7...7
-00000dc0: c48c ed36 f3be e535 42ea 0537 90c5 b236  ...6...5B..7...6
-00000dd0: 7ddb 2036 a421 2137 dd2e 6437 4547 ff36  }. 6.!!7..d7EG.6
-00000de0: d6a4 6136 2ae0 5635 2121 d336 eb4c 8436  ..a6*.V5!!.6.L.6
-00000df0: 082e ed36 79a7 fd35 2f4e ad36 5da5 cd35  ...6y..5/N.6]..5
-00000e00: 32c8 0e37 7d0c a836 0c47 5637 33d2 1936  2..7}..6.GV73..6
-00000e10: 0a9d 8136 94bd 9237 03e4 5036 779e 8736  ...6...7..P6w..6
-00000e20: 985e c634 f348 0036 5068 3e36 6497 1136  .^.4.H.6Ph>6d..6
-00000e30: f87a c435 4105 7836 d99b 3d37 f14c 9737  .z.5A.x6..=7.L.7
-00000e40: 61b1 e836 2cd5 1a36 f487 0637 4222 bd36  a..6,..6...7B".6
-00000e50: d02c 3636 62cc 2337 a26e 5037 7464 d736  .,66b.#7.nP7td.6
-00000e60: 3d48 7e36 0252 4b35 3522 ec36 285d 4e36  =H~6.RK55".6(]N6
-00000e70: 8fb0 ee36 3ea4 0036 6ea9 9b36 49c2 b635  ...6>..6n..6I..5
-00000e80: e35c 1238 7ff2 a437 e05d 5138 4fa7 1137  .\.8...7.]Q8O..7
-00000e90: 68ce 8137 673e 8d38 f15c 3437 7d17 8437  h..7g>.8.\47}..7
-00000ea0: 51eb a235 16bf f436 ea18 3637 63ce 1437  Q..5...6..67c..7
-00000eb0: de92 7f36 4a27 5637 362d 3c38 11e2 9338  ...6J'V76-<8...8
-00000ec0: 6ffb e737 57be 0f37 c0c7 f737 9c9f a037  o..7W..7...7...7
-00000ed0: 0740 1b37 6404 1d38 4197 5038 d24d d437  .@.7d..8A.P8.M.7
-00000ee0: 0739 5537 43ce 2136 f94a df37 c3d3 3a37  .9U7C.!6.J.7..:7
-00000ef0: 4e74 e137 2d96 f636 a39b 9937 11b8 ad36  Nt.7-..6...7...6
-00000f00: 82eb eb35 f4ad 7635 db2f 2336 79f5 0a35  ...5..v5./#6y..5
-00000f10: 7ee4 3b35 c81a 7f36 3446 5735 0a10 6535  ~.;5...64FW5..e5
-00000f20: 4040 d834 67a2 2735 4916 3e35 6042 4235  @@.4g.'5I.>5`BB5
-00000f30: 2ffa 1e35 6087 7235 9fb6 1b36 d3a0 8836  /..5`.r5...6...6
-00000f40: cb15 1936 4c4c 2835 7b1f 0636 f825 cc35  ...6LL(5{..6.%.5
-00000f50: ca86 0036 f2fa 0836 fe97 1c36 69a8 0f36  ...6...6...6i..6
-00000f60: a334 ad35 f700 0835 4e8e 0936 d53c f735  .4.5...5N..6.<.5
-00000f70: b0e9 f035 8066 2535 13a8 a235 9e9a d234  ...5.f%5...5...4
-00000f80: 6f2a d937 d6e9 8837 d908 2a38 8296 f336  o*.7...7..*8...6
-00000f90: 3823 4937 f56e 5f38 d94c 2037 3096 4c37  8#I7.n_8.L 70.L7
-00000fa0: 14c5 4535 6a51 bc36 3e0c 0f37 2d9d d036  ..E5jQ.6>..7-..6
-00000fb0: 701b 7536 66be 2937 d000 1438 507e 6538  p.u6f.)7...8P~e8
-00000fc0: 6e48 a037 5233 ea36 6cef d337 038d 8e37  nH.7R3.6l..7...7
-00000fd0: fe4f c936 5ebb 0238 c8b4 2538 fea0 a137  .O.6^..8..%8...7
-00000fe0: 5e87 3a37 eba2 df35 b952 b137 ac34 0537  ^.:7...5.R.7.4.7
-00000ff0: f630 b837 8b86 bc36 e426 6f37 787a 8f36  .0.7...6.&o7xz.6
+00000000: 8f90 623b d554 323b 5e0e c63a 3f74 8b38  ..b;.T2;^..:?t.8
+00000010: f2df 8d3b c514 263a 010f 103b 4ee7 f33a  ...;..&:...;N..:
+00000020: b972 823b e64e 213b b05e 0a38 1e4d 9539  .r.;.N!;.^.8.M.9
+00000030: 6071 0b3b 42c3 673b 80ad b739 235e 963b  `q.;B.g;...9#^.;
+00000040: 2abe f43b 1625 8c3b bdea ac3b bd13 0d3b  *..;.%.;...;...;
+00000050: d9e7 2c3b 1fc6 3b3a 6552 613b d3e6 5d3a  ..,;..;:eRa;..]:
+00000060: 8f22 463a 01a0 3e3b ea6c 9d3b 6228 6738  ."F:..>;.l.;b(g8
+00000070: f976 c936 70fa a139 83d4 183a 9d63 253a  .v.6p..9...:.c%:
```

##### archive/data/6

```diff
@@ -1,8 +1 @@
-00000000: 8a66 1539 926a d13a c132 73bb b869 973a  .f.9.j.:.2s..i.:
-00000010: 6de1 84bb fb3c 82bb 13c7 93ba 2a1f 723a  m....<......*.r:
-00000020: ef30 4ebb e687 773b fc12 9cb9 f9ff 143a  .0N...w;.......:
-00000030: 6800 fdba ee8c 5f3a 0909 d5b9 50f0 8b3a  h....._:....P..:
-00000040: 9d21 c639 c91c 953a a188 813a 00b3 26ba  .!.9...:...:..&.
-00000050: 08dc e5ba 885b 57ba daf1 623a 6597 2dbb  .....[W...b:e.-.
-00000060: ba3a 6bbb 50e5 75bb f7fa 6e3b 5028 8aba  .:k.P.u...n;P(..
-00000070: 00b7 7fba b8aa 40bb d363 ebba f8f2 413b  ......@..c....A;
+00000000: 0000 7546                                ..uF
```

##### archive/data/7

```diff
@@ -1,8 +1,256 @@
-00000000: 734f 1a38 54ea 3d37 a03c fc38 0149 6e38  sO.8T.=7.<.8.In8
-00000010: 2245 c539 b039 6939 b609 0338 47de 4237  "E.9.9i9...8G.B7
-00000020: fdb0 d938 baf7 b939 bdf9 6136 fde7 c538  ...8...9..a6...8
-00000030: 0db4 9438 a4d9 0d38 eb7e de37 9e59 7538  ...8...8.~.7.Yu8
-00000040: bafe 7337 2c67 a937 0832 e738 1d5e 1f38  ..s7,g.7.2.8.^.8
-00000050: ab35 1a38 33e9 b338 a61f 3338 055c fa38  .5.83..8..38.\.8
-00000060: e445 ee38 a483 eb38 43ea 8a39 e064 f937  .E.8...8C..9.d.7
-00000070: 88ca f937 6767 e638 f178 4337 4a65 ad38  ...7gg.8.xC7Je.8
+00000000: 041d 1e39 5390 1bb9 71ac a0b8 24b7 fdb5  ...9S...q...$...
+00000010: 6949 8f38 8e29 8bb8 5d4e c1b8 c1d3 a6b7  iI.8.)..]N......
+00000020: b338 f8b7 4705 2139 80aa 2439 9b95 4bb9  .8..G.!9..$9..K.
+00000030: 5d51 8d37 eea1 2eb9 cac7 2e39 bc4f ad38  ]Q.7.......9.O.8
+00000040: 1e0c 3739 4526 1a39 3d9f ac38 9647 82b9  ..79E&.9=..8.G..
+00000050: 3098 d6b6 dd25 19b9 cbea 1fb9 4b9e 2337  0....%......K.#7
+00000060: 1082 ea38 fcc4 ba38 dcd9 c4b8 a1c7 b8b8  ...8...8........
+00000070: 92a1 26b6 0175 4bb8 579f 5033 d437 38b8  ..&..uK.W.P3.78.
+00000080: 8a06 de36 aa34 0738 fe4d 7b37 6775 a138  ...6.4.8.M{7gu.8
+00000090: e40c c8b6 ad77 0d38 3765 ce36 2213 4c38  .....w.87e.6".L8
+000000a0: d5d2 de37 e9d1 d9b7 2e38 b5b7 9a19 0d38  ...7.....8.....8
+000000b0: af45 ecb6 0be3 4038 9ea8 8bb8 59f9 d3b7  .E....@8....Y...
+000000c0: 0ad1 c5b7 7aef 15b7 be3e 27b7 dfe7 9338  ....z....>'....8
+000000d0: b544 b136 b27e 8838 ad5f 4c38 c3e3 fbb7  .D.6.~.8._L8....
+000000e0: 5b90 31b8 184d 3d36 ffb7 0238 66eb 1138  [.1..M=6...8f..8
+000000f0: 110b 3c38 a5c2 9337 8a0b d437 e8ec 85b6  ..<8...7...7....
+00000100: d3d9 04b7 ea90 4636 b303 1837 f640 7db7  ......F6...7.@}.
+00000110: 35aa 8635 96f4 4db6 b231 3835 a0ef 39b7  5..5..M..185..9.
+00000120: e477 1eb7 5f36 9eb7 d11f 38b7 afa5 4237  .w.._6....8...B7
+00000130: 3742 8bb6 9a0c 2536 22ea c2b5 2b0f 39b7  7B....%6"...+.9.
+00000140: 15ac 89b6 67bd 98b6 52cc 0235 49d2 0f37  ....g...R..5I..7
+00000150: 6412 78b6 9ca2 1037 2442 47b4 0465 d336  d.x....7$BG..e.6
+00000160: dd9f 9c35 8cc5 66b7 3a56 b8b5 1a54 4e35  ...5..f.:V...TN5
+00000170: 2b46 15b7 5649 feb5 17d9 d7b6 bd91 0237  +F..VI.........7
+00000180: 867d a136 8e31 8737 6533 0237 c74d 2c38  .}.6.1.7e3.7.M,8
+00000190: b5bb 27b6 ad85 9237 87e8 2f36 295e d637  ..'....7../6)^.7
+000001a0: 12d2 6637 7104 5cb7 e935 33b7 9885 8c37  ..f7q.\..53....7
+000001b0: 13f6 81b6 b88f c337 338e 10b8 f4b2 5eb7  .......73.....^.
+000001c0: 94b8 39b7 f663 73b6 8248 98b6 68c0 1638  ..9..cs..H..h..8
+000001d0: cb67 2636 23a8 0e38 5291 d037 7e0d 84b7  .g&6#..8R..7~...
+000001e0: cc4d b7b7 bf83 f235 2c94 8337 86a3 9737  .M.....5,..7...7
+000001f0: f93d c937 390b 1737 85d7 5e37 cb6e 16b6  .=.79..7..^7.n..
+00000200: a38a 5b35 b06e 3f36 8c62 ce35 15e0 ed36  ..[5.n?6.b.5...6
+00000210: 0182 c7b4 6d8a 4b36 705e d834 d473 9236  ....m.K6p^.4.s.6
+00000220: 27fc 1636 9f3d 33b6 ad1a 09b6 c800 5236  '..6.=3.......R6
+00000230: 87fb 4fb5 4792 8a36 b44d cdb6 41ee 2cb6  ..O.G..6.M..A.,.
+00000240: f93b 03b6 d16c 29b5 6857 47b5 2ca6 d936  .;...l).hWG.,..6
+00000250: 518f c734 87bb d036 d246 9236 4c98 35b6  Q..4...6.F.6L.5.
+00000260: 1c4a 80b6 91fc d133 dba7 3736 4153 5736  .J.....3..76ASW6
+00000270: 7c6f 8a36 2723 cf35 a811 1836 bfcf 91b4  |o.6'#.5...6....
+00000280: 814a 4a39 6192 72b9 7322 b5b8 0bd7 f6b8  .JJ9a.r.s"......
+00000290: 887b e938 b633 0db9 f554 0cb9 aab9 ebb8  .{.8.3...T......
+000002a0: ae65 ceb8 2a75 3a39 1f3c 5439 8300 8cb9  .e..*u:9.<T9....
+000002b0: d619 3237 3d36 8eb9 fbee 9639 a5d3 ca38  ..27=6.....9...8
+000002c0: f57c 8b39 4db1 5839 73e9 0b39 2855 cbb9  .|.9M.X9s..9(U..
+000002d0: 91ae 10b8 f7d0 71b9 9017 89b9 94a5 8938  ......q........8
+000002e0: 88cf 4e39 9e1c 9d38 d5fb 36b9 ad5c 1cb9  ..N9...8..6..\..
+000002f0: 711b 89b8 5b93 bfb8 5196 47b8 c904 00b8  q...[...Q.G.....
+00000300: a59c 27b9 4852 4e39 b3c9 9838 971b e738  ..'.HRN9...8...8
+00000310: fb94 c4b8 3080 f638 8e15 ea38 289b d738  ....0..8...8(..8
+00000320: 4638 b638 b504 1eb9 b647 33b9 8bf6 6d39  F8.8.....G3...m9
+00000330: 236f 16b7 f9c5 7339 d9af 82b9 ba32 aeb8  #o....s9.....2..
+00000340: 99fb 6cb9 856d 35b9 2476 edb8 865a ae39  ..l..m5.$v...Z.9
+00000350: b031 0438 088d 5239 499f 6b39 1a67 7eb8  .1.8..R9I.k9.g~.
+00000360: 944d 32b9 10d9 7db8 51f3 1e39 44ca 0739  .M2...}.Q..9D..9
+00000370: b915 7d38 a373 a538 253e 3c38 7293 c737  ..}8.s.8%><8r..7
+00000380: 62c5 a1b7 1166 31b7 8153 8737 e218 99b8  b....f1..S.7....
+00000390: 09be 0237 bded cfb7 7a0f acb6 8fc5 54b8  ...7....z.....T.
+000003a0: 0984 22b8 d22e 1db8 3a68 7fb7 a993 3c37  ..".....:h....<7
+000003b0: 7a18 03b7 5590 97b7 dd3f f737 0b48 94b7  z...U....?.7.H..
+000003c0: b3ef 8e36 0767 4eb6 5053 0f37 55d0 65b7  ...6.gN.PS.7U.e.
+000003d0: 0190 48b7 a2fc f1b6 43dc dbb7 79f2 f537  ..H.....C...y..7
+000003e0: 11bd d337 270d 17b8 122d a0b7 61e7 85b7  ...7'....-..a...
+000003f0: 8383 36b8 e0e6 72b7 1bd3 e6b7 a6bb b437  ..6...r........7
+00000400: 78df 36b6 4f5d ecb7 5293 59b7 d754 81b8  x.6.O]..R.Y..T..
+00000410: fc57 c936 4903 ecb7 ad14 dab6 e69f 25b8  .W.6I.........%.
+00000420: 4f89 b8b7 e574 bf37 9b85 a537 af77 fbb7  O....t.7...7.w..
+00000430: f044 c036 e9ac 25b8 4482 6a38 0ced b137  .D.6..%.D.j8...7
+00000440: d3ba b737 5585 2137 b93f 1f37 37dc 7cb8  ...7U.!7.?.77.|.
+00000450: 4ef7 99b6 1ee9 62b8 41fc 2db8 ba1e cc37  N.....b.A.-....7
+00000460: 07aa 1538 7568 92b5 f98d dfb7 49ca f5b7  ...8uh......I...
+00000470: 2548 16b8 7cf2 7ab7 72fd aab7 0fa8 3236  %H..|.z.r.....26
+00000480: 6c36 d0b6 da08 b2b7 738a 30b7 ab57 60b8  l6......s.0..W`.
+00000490: c314 5736 4d11 bfb7 c075 72b6 105e 0ab8  ..W6M....ur..^..
+000004a0: 0b01 95b7 42ae 9337 05a7 7137 4bc7 bab7  ....B..7..q7K...
+000004b0: 84b7 b136 0f44 00b8 e4b5 3d38 6dd7 9437  ...6.D....=8m..7
+000004c0: fac1 7137 f19b a436 6470 c436 6f34 46b8  ..q7...6dp.6o4F.
+000004d0: f769 42b6 64c3 3bb8 d0a3 08b8 dee6 a937  .iB.d.;........7
+000004e0: 6cc0 f037 00d8 fdb5 1fd9 a9b7 6f77 c7b7  l..7........ow..
+000004f0: cc80 03b8 9925 45b7 71fc 8eb7 4f89 3136  .....%E.q...O.16
+00000500: 8740 3e36 5d99 3137 f0df 9236 ed4a e537  .@>6].17...6.J.7
+00000510: caae 08b6 a80e 4337 ede3 f835 ec24 9237  ......C7...5.$.7
+00000520: 1f6e 2137 1797 fdb6 54dd d8b6 5bd5 3037  .n!7....T...[.07
+00000530: 9517 09b6 dd77 8037 84c4 bbb7 bf9d 02b7  .....w.7........
+00000540: fb1e 01b7 2528 2db6 5fa3 63b6 7d64 c237  ....%(-._.c.}d.7
+00000550: 8179 1436 a7ec b337 57a2 8937 d752 34b7  .y.6...7W..7.R4.
+00000560: 84e7 6fb7 8206 0436 d4c7 3437 031b 4437  ..o....6..47..D7
+00000570: bac5 8337 8e8f cb36 524c 1937 3679 02b6  ...7...6RL.76y..
+00000580: d382 bb37 4ee0 92b6 20d8 97b7 bc47 4138  ...7N... ....GA8
+00000590: 34f3 8fb5 21ae 3837 cdfb 40b6 d9c4 0538  4...!.87..@....8
+000005a0: 42ae c937 0fc9 2238 ca27 c037 5b84 c1b7  B..7.."8.'.7[...
+000005b0: 90a9 0037 2abb 97b5 0f74 abb6 c100 ab37  ...7*....t.....7
+000005c0: ed7b 1937 8c10 4b37 d6e6 09b5 32b1 40b7  .{.7..K7....2.@.
+000005d0: 9c7f 0f37 0965 20b7 d7e5 b136 35f9 9bb7  ...7.e ....65...
+000005e0: fb16 f9b6 69f4 0438 4edc cb36 3f7a 4336  ....i..8N..6?zC6
+000005f0: a4a0 e237 7878 c836 1534 9937 6503 99b7  ...7xx.6.4.7e...
+00000600: 6ef6 5138 5f6e c1b7 d003 f1b7 dee5 8438  n.Q8_n.........8
+00000610: 6e08 1b37 6960 ee36 fbb4 93b7 a09a 2738  n..7i`.6......'8
+00000620: 2848 d437 3545 7e38 24f8 4038 a1d4 50b8  (H.75E~8$.@8..P.
+00000630: 6581 1e37 2f8b a6b7 1db9 1a37 84b0 fa37  e..7/......7...7
+00000640: 2391 0e38 56d0 1538 ca27 3e37 6800 24b8  #..8V..8.'>7h.$.
+00000650: 5d3a 1937 6049 b0b7 fd29 2db7 2bc0 c9b7  ]:.7`I...)-.+...
+00000660: 67b3 3436 75f9 4b38 960c 43b6 7f9d a3b6  g.46u.K8..C.....
+00000670: 39a5 1938 8fe8 cf35 ce63 cc37 8f8c e4b7  9..8...5.c.7....
+00000680: 8dbb 6eb2 96bc c036 cbb3 5236 bc56 3b37  ..n....6..R6.V;7
+00000690: 445d 96b5 e2b2 b336 c80f b235 3486 ed36  D].....6...54..6
+000006a0: 438f 7a36 744d c0b6 d397 9bb6 27ed e036  C.z6tM......'..6
+000006b0: 3f66 bab5 3983 0537 19c0 3ab7 7c39 a4b6  ?f..9..7..:.|9..
+000006c0: 9f89 9bb6 ed5f 14b6 3f3b fab5 fcec 5037  ....._..?;....P7
+000006d0: f2f5 3d35 075d 3c37 eb0c 0937 c6c5 93b6  ..=5.]<7...7....
+000006e0: b170 e9b6 af3b 38b5 119d ae36 a57d c436  .p...;8....6.}.6
+000006f0: 570d d836 f721 3e36 f6bb 7236 dc5b c9b2  W..6.!>6..r6.[..
+00000700: 0589 ed35 c00f 3937 3642 d436 f8e9 cd37  ...5..976B.6...7
+00000710: ce1d d5b5 8a7f 3837 dcca f335 147b 7e37  ......87...5.{~7
+00000720: cb4d 0037 d7b7 3eb7 150c 10b7 7761 5537  .M.7..>.....waU7
+00000730: 5c91 4cb6 7693 8337 0ac9 beb7 3b63 2bb7  \.L.v..7....;c+.
+00000740: 7fad 07b7 2156 53b6 90bc 4ab6 7c7d d037  ....!VS...J.|}.7
+00000750: a81f a735 c2ca c437 ff98 8837 fab7 1eb7  ...5...7...7....
+00000760: 2360 6cb7 51e1 54b5 b1ee 2b37 d5a1 4737  #`l.Q.T...+7..G7
+00000770: bfd7 6e37 8cee bc36 e146 0337 fc3e c3b4  ..n7...6.F.7.>..
+00000780: b098 d636 a4df 5e37 03ad 0b37 3573 1938  ...6..^7...75s.8
+00000790: e291 29b5 2b4f 7837 96fc c335 9054 b237  ..).+Ox7...5.T.7
+000007a0: 52a9 3337 4523 5fb7 f5e3 29b7 541e 7b37  R.37E#_...).T.{7
+000007b0: c3b7 9db6 7d36 a437 ccd3 feb7 307b 66b7  ....}6.7....0{f.
+000007c0: 08c8 f6b6 ad54 dfb5 889e 1fb6 5e46 0338  .....T......^F.8
+000007d0: 120f 2935 4995 0438 034a af37 f9fa 58b7  ..)5I..8.J.7..X.
+000007e0: 1e41 9fb7 59a0 3934 fbb6 4937 558a 8837  .A..Y.94..I7U..7
+000007f0: 81a0 b537 b938 f736 3c2e 3537 19b3 91b5  ...7.8.6<.57....
+00000800: e1b0 2ab8 d5e9 0538 cd1f e537 a196 d4b7  ..*....8...7....
+00000810: 1ce6 44b7 7bac e836 b98f a937 6903 81b7  ..D.{..6...7i...
+00000820: 6f0d 0cb7 a87a 61b8 e519 40b8 5890 5c38  o....za...@.X.\8
+00000830: 64c6 1ab7 6e5d 0d38 19d4 03b8 3e81 fcb7  d...n].8....>...
+00000840: 4700 1fb8 5d58 14b8 84eb 78b7 c933 6d38  G...]X....x..3m8
+00000850: 44b9 bbb6 2d24 1938 28ae e537 75a4 2337  D...-$.8(..7u.#7
+00000860: f9ba 9eb7 c9f9 1bb8 f6ca 5f37 8502 9037  .........._7...7
+00000870: 48b9 61b7 0b49 cf36 f845 40b7 eaf9 a737  H.a..I.6.E@....7
+00000880: b77d 8337 483a c9b7 4253 87b7 b8a5 65b7  .}.7H:..BS....e.
+00000890: a1a4 f036 9421 66b7 0727 31b7 da55 19b7  ...6.!f..'1..U..
+000008a0: 8c2d a7b6 c958 0238 1051 db37 b28e 0ab8  .-...X.8.Q.7....
+000008b0: 926d c636 4c58 f4b7 84b0 1038 ed69 ac37  .m.6LX.....8.i.7
+000008c0: 1652 ca37 160d 9837 0e80 2337 aac8 43b8  .R.7...7..#7..C.
+000008d0: 55b4 ca34 c142 17b8 b0d0 e4b7 07f6 bb36  U..4.B.........6
+000008e0: 57d5 b337 170e 7737 7eff 85b7 2533 98b7  W..7..w7~...%3..
+000008f0: f9fc 0bb7 d89c 0ab7 4c66 60b6 b41c efb6  ........Lf`.....
+00000900: abbb b736 34da 3837 46a4 1937 848f ef37  ...64.87F..7...7
+00000910: 2cad 2135 af8d 4537 d3da ce34 79c0 8537  ,.!5..E7...4y..7
+00000920: a359 e336 243f 81b7 a4b3 2fb7 478e 7437  .Y.6$?..../.G.t7
+00000930: 308d afb6 c8be 8937 29a8 d9b7 6a28 74b7  0......7)...j(t.
+00000940: 6ef7 c0b6 ec49 81b5 8dbb 8bb5 d44d e937  n....I.......M.7
+00000950: af5a f4b4 5afe f537 d2cd 8e37 42bf 25b7  .Z..Z..7...7B.%.
+00000960: 7947 82b7 aa89 2db6 2c14 1e37 92b3 6b37  yG....-.,..7..k7
+00000970: 5f76 8e37 d941 bb36 72dd 0637 3ab5 2835  _v.7.A.6r..7:.(5
+00000980: c9c7 2635 5725 1c36 f6f5 ac35 30c1 be36  ..&5W%.6...50..6
+00000990: 2db8 9eb4 6d71 2436 77b8 a734 db60 6b36  -...mq$6w..4.`k6
+000009a0: f398 ee35 eaea 18b6 d026 e5b5 ab9e 2e36  ...5.....&.....6
+000009b0: fbc4 2cb5 a108 6236 b205 a7b6 964f 10b6  ..,...b6.....O..
+000009c0: b1b6 d9b5 819b 0db5 5d09 22b5 287f b236  ........].".(..6
+000009d0: 2b46 a334 a35a ab36 c96c 6d36 379b 12b6  +F.4.Z.6.lm67...
+000009e0: 0a6c 4fb6 d3f7 8a32 5d2d 1636 e7ed 2e36  .lO....2]-.6...6
+000009f0: 9b12 5d36 53c3 a635 4fec f435 f1eb 48b4  ..]6S..5O..5..H.
+00000a00: a4fd de36 af2e 18b8 c24a 71b7 a64c 82b8  ...6.....Jq..L..
+00000a10: 0800 3d37 03e9 06b8 f7a8 4ab7 4e36 32b8  ..=7......J.N62.
+00000a20: af5f d7b7 c563 e237 0852 d937 8750 21b8  ._...c.7.R.7.P!.
+00000a30: 4449 a036 3357 4bb8 f69a 8538 b81a b937  DI.63WK....8...7
+00000a40: b6c2 0938 d22f 9a37 de6b 8137 e11f 97b8  ...8./.7.k.7....
+00000a50: d7ef e5b6 b021 75b8 b5b0 51b8 d447 db37  .....!u...Q..G.7
+00000a60: a2eb 2d38 d71a 4b35 3d6f 0bb8 b3ba 0ab8  ..-8..K5=o......
+00000a70: c95c 16b8 6cbd 97b7 7f0e b6b7 3211 0736  .\..l.......2..6
+00000a80: 52f3 3438 62e3 9eb8 32e5 f5b7 a3d4 a2b8  R.48b...2.......
+00000a90: 51ea 0138 2aa0 62b8 870a 1cb8 c974 75b8  Q..8*.b......tu.
+00000aa0: 5dd4 2fb8 5e1a 6e38 1c37 8438 aeec b3b8  ]./.^.n8.7.8....
+00000ab0: 20d9 d536 d05c c5b8 8807 e938 a2c4 1d38   ..6.\.....8...8
+00000ac0: e44a a738 a6fa 6b38 744e 2538 40d5 0eb9  .J.8..k8tN%8@...
+00000ad0: a57a 55b7 fc08 c6b8 624b c4b8 075e 1238  .zU.....bK...^.8
+00000ae0: af1d 9c38 5598 8237 6a5d 82b8 9c1b 77b8  ...8U..7j]....w.
+00000af0: bc92 35b8 1c0f 0db8 0c39 e8b7 49ad 8eb6  ..5......9..I...
+00000b00: 29a3 ca35 4828 c436 9d7e 5436 27d6 6a37  )..5H(.6.~T6'.j7
+00000b10: 01b4 58b5 cb2e cc36 ae46 8a35 cdbe 0f37  ..X....6.F.5...7
+00000b20: dc52 9836 46ac b2b6 05f3 8fb6 364e d736  .R.6F.......6N.6
+00000b30: 46e1 d6b5 9563 0c37 42ee 4eb7 d5ca adb6  F....c.7B.N.....
+00000b40: 8f78 85b6 fe50 c3b5 656d cfb5 70b4 5b37  .x...P..em..p.[7
+00000b50: 6218 2535 e67d 5037 4b33 1437 7998 b0b6  b.%5.}P7K3.7y...
+00000b60: f287 02b7 b9ca a533 85ac b436 18cd da36  .......3...6...6
+00000b70: f5ae 0a37 1357 5236 c775 9336 3138 fbb4  ...7.WR6.u.618..
+00000b80: 320b bf38 7ccd 95b8 d91b a2b8 e599 ba38  2..8|..........8
+00000b90: 79a4 a637 62da c2b6 a2c6 5cb8 9b0c 8a38  y..7b.....\....8
+00000ba0: ceb6 0f38 70e4 0d39 c710 fb38 c260 06b9  ...8p..9...8.`..
+00000bb0: 68a6 0638 40d8 93b8 c006 8938 bd95 ac38  h..8@......8...8
+00000bc0: b922 9a38 6a43 ad38 976c d437 d477 04b9  .".8jC.8.l.7.w..
+00000bd0: 6248 0838 b96e b1b8 a17a 64b8 ef2d 3ab8  bH.8.n...zd..-:.
+00000be0: 1645 2b38 cc4c dd38 2e96 09b7 b32b 27b8  .E+8.L.8.....+'.
+00000bf0: 42f2 1e38 27a2 1ab7 c397 4338 80c4 77b8  B..8'.....C8..w.
+00000c00: 19b0 f6b8 66c7 e438 c61c b238 5719 68b8  ....f..8...8W.h.
+00000c10: f070 26b8 4fb8 0638 7b40 9938 2c91 14b8  .p&.O..8{@.8,...
+00000c20: ba8b 28b7 02c0 20b9 0be7 17b9 1725 2d39  ..(... ......%-9
+00000c30: a8f5 feb7 31a2 f338 71e0 f0b8 6d67 bfb8  ....1..8q...mg..
+00000c40: f0a0 f5b8 041a eeb8 a803 4cb8 44b9 4539  ..........L.D.E9
+00000c50: 09e5 b9b7 9a41 fc38 6b62 d238 bc1c d937  .....A.8kb.8...7
+00000c60: e373 9eb8 0d2a e0b8 5073 2e38 ea84 8738  .s...*..Ps.8...8
+00000c70: d207 a1b7 d582 dd37 5dce 03b8 74ef 7138  .......7]...t.q8
+00000c80: 9d03 92b6 5b9d 8eb7 1dd4 25b7 8c8b 27b8  ....[.....%...'.
+00000c90: f8a4 0d36 5609 91b7 8ef2 68b6 74b8 c5b7  ...6V.....h.t...
+00000ca0: 6b42 53b7 acdf 8537 ff11 5e37 d9b2 9fb7  kBS....7..^7....
+00000cb0: 0db7 ac36 8ed9 c9b7 a5a7 1538 cde6 8237  ...6.......8...7
+00000cc0: 86f2 3737 72e0 9536 4fe1 8b36 8186 1eb8  ..77r..6O..6....
+00000cd0: ad98 62b5 7e54 17b8 d702 d5b7 7bda 6e37  ..b.~T......{.n7
+00000ce0: 30ea bd37 f721 4f35 1e1b 75b7 2ff4 9fb7  0..7.!O5..u./...
+00000cf0: 6e2f c8b7 b225 16b7 6eb9 45b7 ec20 4235  n/...%..n.E.. B5
+00000d00: 51e4 2036 d8f2 da36 ee3f 6e36 2ea5 8e37  Q. 6...6.?n6...7
+00000d10: 28c8 46b5 a48c ed36 c078 9135 165c 2a37  (.F....6.x.5.\*7
+00000d20: 68fe b536 d4dd bdb6 423b 9cb6 b18b ea36  h..6....B;.....6
+00000d30: 8535 ffb5 2f56 1e37 f8ee 6eb7 4eed c4b6  .5../V.7..n.N...
+00000d40: 2732 87b6 715d adb5 2964 d0b5 9c05 7737  '2..q]..)d....w7
+00000d50: 4763 1835 a97d 6f37 fa48 2937 eebb ceb6  Gc.5.}o7.H)7....
+00000d60: 9dc3 17b7 5524 d534 d00c c836 427b fe36  ....U$.4...6B{.6
+00000d70: 17d7 2837 0e47 7336 2864 ad36 3f37 3bb5  ..(7.Gs6(d.6?7;.
+00000d80: fcfb 23b6 a5c1 24b7 3626 bcb6 3558 c0b7  ..#...$.6&..5X..
+00000d90: e538 a835 bec8 28b7 679c f3b5 8d01 69b7  .8.5..(.g.....i.
+00000da0: ffe5 f5b6 8974 1c37 773a fd36 3326 39b7  .....t.7w:.63&9.
+00000db0: a88c 4036 b7ce 6ab7 db34 ad37 eceb 1637  ..@6..j..4.7...7
+00000dc0: 2c19 dd36 3e7c 2936 9c89 2736 0adb b8b7  ,..6>|)6..'6....
+00000dd0: fb39 50b5 f7f7 afb7 42fc 76b7 1397 0e37  .9P.....B.v....7
+00000de0: b557 5a37 66a0 9f34 7932 13b7 fa5e 38b7  .WZ7f..4y2...^8.
+00000df0: 29fb 64b7 63ec adb6 66e6 ecb6 64fa 0d35  ).d.c...f...d..5
+00000e00: eee2 adb6 ed43 1937 b136 a136 9e27 0f37  .....C.7.6.6.'.7
+00000e10: 3a30 52b6 e789 cf36 390d 8936 bad0 c836  :0R....69..6...6
+00000e20: c66b 7f36 5abe 1bb7 ec71 12b7 d78b 4037  .k.6Z....q....@7
+00000e30: e12f ccb5 271e 3f37 fbf8 66b7 9d8a d2b6  ./..'.?7..f.....
+00000e40: f5e0 1cb7 b07f ddb6 6055 8db6 5b29 9137  ........`U..[).7
+00000e50: 865a 6f35 1e7b 5a37 4dd2 3937 00eb 72b6  .Zo5.{Z7M.97..r.
+00000e60: 345c 14b7 79a3 69b6 5788 ed36 823e f636  4\..y.i.W..6.>.6
+00000e70: 0110 9e36 22d2 7a36 cc22 3636 ced5 be35  ...6".z6."66...5
+00000e80: eecd 50b8 2180 8c38 3875 fe37 80ff 3138  ..P.!..88u.7..18
+00000e90: 7776 ecb7 37a9 2b38 6c96 1738 1a19 1238  wv..7.+8l..8...8
+00000ea0: b75b e537 fd2d 79b8 c14e 84b8 15a3 ab38  .[.7.-y..N.....8
+00000eb0: aa49 ebb6 627a a838 ea0e bdb8 f113 18b8  .I..bz.8........
+00000ec0: b7d3 9ab8 a2a4 6bb8 e715 15b8 216a f738  ......k.....!j.8
+00000ed0: ef99 0337 b9ed a338 285b a238 590b abb7  ...7...8([.8Y...
+00000ee0: 9d1e 7cb8 fe56 d4b7 ec21 5238 035a 4a38  ..|..V...!R8.ZJ8
+00000ef0: 67fa c437 05cd df37 1746 7737 1c3e 3237  g..7...7.Fw7.>27
+00000f00: c7f4 28b6 d3e4 1eb7 9f79 b0b6 7dab beb7  ..(......y..}...
+00000f10: 6ace a435 687d 25b7 70b7 d6b5 4397 68b7  j..5h}%.p...C.h.
+00000f20: 11df f3b6 f6d1 1437 32ad ec36 594e 30b7  .......72..6YN0.
+00000f30: 31aa 3336 c8e9 63b7 077d a837 5f15 1037  1.36..c..}.7_..7
+00000f40: d4c3 d636 4827 1a36 df9b 2336 1817 b3b7  ...6H'.6..#6....
+00000f50: bd50 7eb5 98e7 aab7 b046 70b7 f204 0f37  .P~......Fp....7
+00000f60: 3fd4 5337 a0cf 62af 7227 12b7 8c49 32b7  ?.S7..b.r'...I2.
+00000f70: d00a 61b7 4dc9 a9b6 8488 eeb6 dd54 3935  ..a.M........T95
+00000f80: 396f 3435 08ff 3236 e7f9 b035 36f4 da36  9o45..26...56..6
+00000f90: 2504 e6b4 ad2a 3d36 bae8 fb34 3e2f 8836  %....*=6...4>/.6
+00000fa0: ae6a 1236 a2ec 16b6 b2e0 f5b5 1184 3d36  .j.6..........=6
+00000fb0: 31d1 2db5 6565 8036 b73f bcb6 1378 14b6  1.-.ee.6.?...x..
+00000fc0: df04 fbb5 b8af 33b5 19c1 4cb5 8b87 c636  ......3...L....6
+00000fd0: 6633 cc34 a572 ba36 e22b 8836 eac2 27b6  f3.4.r.6.+.6..'.
+00000fe0: 9474 6eb6 074c 4e34 5f02 2b36 c182 4536  .tn..LN4_.+6..E6
+00000ff0: 4d03 8036 28c6 c335 01fa 0c36 c399 a4b4  M..6(..5...6....
```

##### archive/data/8

```diff
@@ -1,16 +1,256 @@
-00000000: df48 1f3a 0b5e 2cbc cef3 9bb9 8300 423c  .H.:.^,.......B<
-00000010: 3091 ad3b 26c7 12bc 00f2 bdbb 962a d4bb  0..;&........*..
-00000020: 8838 ac3b c38e abbb 5482 153b 9213 a5bb  .8.;....T..;....
-00000030: c9fe 07bc 0358 f73a 6a10 63bc e36e 02b9  .....X.:j.c..n..
-00000040: 89d3 e33b 9141 08bc 8ace 32b8 53ca 12ba  ...;.A....2.S...
-00000050: ef42 173c 9a11 77ba f96e 87bb d8a8 c43b  .B.<..w..n.....;
-00000060: 1cba b8ba 42a9 e93a 86cb 7ebb f273 053c  ....B..:..~..s.<
-00000070: 2f7d f939 4151 4bba ed29 283c e260 583a  /}.9AQK..)(<.`X:
-00000080: d248 1fba 0b5e 2c3c dbf3 9b39 8100 42bc  .H...^,<...9..B.
-00000090: 3391 adbb 25c7 123c fef1 bd3b 982a d43b  3...%..<...;.*.;
-000000a0: 8838 acbb c48e ab3b 5682 15bb 9413 a53b  .8.....;V......;
-000000b0: c9fe 073c 0358 f7ba 6b10 633c e96e 0239  ...<.X..k.c<.n.9
-000000c0: 8bd3 e3bb 9241 083c bdcf 3238 5bca 123a  .....A.<..28[..:
-000000d0: f242 17bc 9711 773a fa6e 873b d9a8 c4bb  .B....w:.n.;....
-000000e0: 1eba b83a 46a9 e9ba 8ccb 7e3b f373 05bc  ...:F.....~;.s..
-000000f0: 3f7d f9b9 3951 4b3a f029 28bc d560 58ba  ?}..9QK:.)(..`X.
+00000000: 3950 2637 97fa 1336 0e00 1336 8789 0138  9P&7...6...6...8
+00000010: a5ad 2e35 3528 f135 2d33 0836 e45b 2537  ...55(.5-3.6.[%7
+00000020: 2530 2036 606f cb36 7350 ac36 4f43 bd36  %0 6`o.6sP.6OC.6
+00000030: f31c 0a35 adfe 2736 8d2b ca36 9be0 1e36  ...5..'6.+.6...6
+00000040: 88f6 7736 beaf a836 935d 4735 91fd db36  ..w6...6.]G5...6
+00000050: 84bd 5135 4c6d d936 9908 3036 e43b 8736  ..Q5Lm.6..06.;.6
+00000060: 5ce1 2b36 f0a5 c336 cede 3835 6459 fd35  \.+6...6..85dY.5
+00000070: bb98 2237 d5ae d034 de73 6d36 80e5 0c36  .."7...4.sm6...6
+00000080: a299 4e36 0965 6c35 d7f2 4535 4ec5 1c37  ..N6.el5..E5N..7
+00000090: d75a 7334 6ffe 2435 8ac5 3b35 947a 4b36  .Zs4o.$5..;5.zK6
+000000a0: e1d5 4d35 9e83 0636 6f94 ec35 5e2d 0736  ..M5...6o..5^-.6
+000000b0: 661b 3434 84cd 8b35 51b1 1236 d39f 5635  f.44...5Q..6..V5
+000000c0: 7fc3 ae35 4d0d e035 70eb 8f34 1a46 2d36  ...5M..5p..4.F-6
+000000d0: 8e16 8534 f5cd 1536 8467 8f35 8513 a635  ...4...6.g.5...5
+000000e0: a4f6 8035 33fe f535 ddea 9534 e040 3a35  ...53..5...4.@:5
+000000f0: d3a7 4636 a06a 2034 3eae 9135 a823 3035  ..F6.j 4>..5.#05
+00000100: 99ab fb34 bd0c 3534 a48e 1134 ee91 9835  ...4..54...4...5
+00000110: 7670 2d33 a77a 9233 ac12 0934 d7e7 bf34  vp-3.z.3...4...4
+00000120: 2ef7 b533 8e7a c134 cb2d b134 9f72 cd34  ...3.z.4.-.4.r.4
+00000130: 2575 ff32 a469 4534 be85 a134 3373 1a34  %u.2.iE4...43s.4
+00000140: 16c0 8034 d0da 9b34 d844 5433 c18f f734  ...4...4.DT3...4
+00000150: b43c 2e33 9769 b034 39be 3334 9f1c 2234  .<.3.i.49.34.."4
+00000160: 7556 1134 b0e7 9b34 b20d 1733 8d14 d633  uV.4...4...3...3
+00000170: ebf7 bb34 fb69 9d32 7681 1234 4acb d933  ...4.i.2v..4J..3
+00000180: 236e 6635 3bfc 8534 79cf 5e34 d1ec 2f36  #nf5;..4y.^4../6
+00000190: 8872 8933 50b2 3b34 4ae7 5134 acbd 6335  .r.3P.;4J.Q4..c5
+000001a0: d761 6834 54fb 1635 63fe 0435 9fa4 1735  .ah4T..5c..5...5
+000001b0: d2e8 4c33 7bb4 9f34 fb7e 2735 3f46 7334  ..L3{..4.~'5?Fs4
+000001c0: af82 c434 c91e fa34 8a7f a233 ed55 4535  ...4...4...3.UE5
+000001d0: 3fe5 9633 45bf 2a35 c74a a434 33b0 b934  ?..3E.*5.J.43..4
+000001e0: 5b81 9334 b707 0935 98d9 ac33 0079 5734  [..4...5...3.yW4
+000001f0: 1786 6035 1468 3833 c2d6 a234 7dad 4434  ..`5.h83...4}.D4
+00000200: e379 2133 4f96 5432 d9f8 3132 ae81 fd33  .y!3O.T2..12...3
+00000210: 15d0 4a31 3433 1132 549c 1832 cf30 2233  ..J143.2T..2.0"3
+00000220: f026 2a32 0e47 e832 0bed ca32 a3c5 e632  .&*2.G.2...2...2
+00000230: 56f1 2e31 1cde 8232 c972 0833 3614 4b32  V..1...2.r.36.K2
+00000240: c81b 9032 3d97 b232 a683 6e31 aac6 2133  ...2=..2..n1..!3
+00000250: 1f0d 7531 f6f7 0c33 ab34 8732 395f 8432  ..u1...3.4.29_.2
+00000260: 2e50 7132 36de c532 8086 8a31 57e3 3832  .Pq26..2...1W.82
+00000270: 613f 2633 81ae 1431 713c 6832 e42e 0f32  a?&3...1q<h2...2
+00000280: 5ba6 6437 52cc 4236 f88f 5136 2f5f 4638  [.d7R.B6..Q6/_F8
+00000290: 01c1 5335 5017 4736 c4f1 3036 7776 8137  ..S5P.G6..06wv.7
+000002a0: 40a4 8236 a599 0e37 4912 eb36 c001 fc36  @..6...7I..6...6
+000002b0: 3fa5 4c35 49d2 6e36 ee56 2037 9b0d 6736  ?.L5I.n6.V 7..g6
+000002c0: 824d 9836 526d dc36 f360 6c35 0ca8 1c37  .M.6Rm.6.`l5...7
+000002d0: c701 9f35 a38e 2737 cc87 8636 a168 d236  ...5..'7...6.h.6
+000002e0: 6e79 8836 e4b9 0d37 a1dd 9635 0c13 4936  ny.6...7...5..I6
+000002f0: 37cd 7c37 c34c 2d35 e24f b736 606e 4e36  7.|7.L-5.O.6`nN6
+00000300: 49b7 3e37 92b6 2036 a822 2a36 9015 2438  I.>7.. 6."*6..$8
+00000310: 2031 3435 2b5c 2436 558c 1236 c133 5537   145+\$6U..6.3U7
+00000320: ebf1 5636 98ff e836 35cc c036 e15d cf36  ..V6...65..6.].6
+00000330: 2c44 2635 412d 4536 d027 0437 5721 3c36  ,D&5A-E6.'.7W!<6
+00000340: 3adb 8036 e78b b736 c5de 4a35 bfa9 0037  :..6...6..J5...7
+00000350: 6bcf 8035 94e3 0937 7bba 5d36 bdf6 ac36  k..5...7{.]6...6
+00000360: 92c1 6036 e103 e836 695e 7c35 3ca6 2536  ..`6...6i^|5<.%6
+00000370: 5c2d 5137 d732 0f35 c992 9636 bdd5 2836  \-Q7.2.5...6..(6
+00000380: be97 d735 7dc6 2f35 e1e1 0735 7228 6d36  ...5}./5...5r(m6
+00000390: 8b0d 2234 5414 6134 ab17 0135 d5d0 8f35  .."4T.a4...5...5
+000003a0: 22af 8034 371f b035 9215 a735 24e6 c235  "..47..5...5$..5
+000003b0: 58ac ef33 a25e 3e35 b679 8e35 1260 1135  X..3.^>5.y.5.`.5
+000003c0: 2673 7235 d86b 8e35 9d6e 4a34 b9cf ed35  &sr5.k.5.nJ4...5
+000003d0: ce06 1b34 9bbf 9f35 39e4 2735 0e70 f834  ...4...59.'5.p.4
+000003e0: 1a83 0135 1bf4 8535 928e 0034 f445 c034  ...5...5...4.E.4
+000003f0: 22cd 9035 227b 8233 6827 e334 f02b b934  "..5"{.3h'.4.+.4
+00000400: 54bc 0336 2770 0e35 974a f034 b759 c536  T..6'p.5.J.4.Y.6
+00000410: 049d 1734 9af0 c734 98aa ec34 e873 0036  ...4...4...4.s.6
+00000420: 4308 ff34 2f24 a535 9519 9235 8c18 a735  C..4/$.5...5...5
+00000430: 8a9a d433 2351 2535 0543 ae35 bf01 ff34  ...3#Q%5.C.5...4
+00000440: 14bb 5a35 38f8 8d35 75dd 3334 4c87 cd35  ..Z58..5u.34L..5
+00000450: 3af5 1f34 25c6 b135 54cd 2835 40e8 5135  :..4%..5T.(5@.Q5
+00000460: c999 1835 893e 9b35 0f63 3134 a8f6 d634  ...5.>.5.c14...4
+00000470: 7c2d f635 8f6c bd33 dc1a 3835 9c59 dd34  |-.5.l.3..85.Y.4
+00000480: 3725 c835 d253 e534 f188 bf34 86e5 9736  7%.5.S.4...4...6
+00000490: d83b ed33 7e1e a034 aa34 b634 4b83 c435  .;.3~..4.4.4K..5
+000004a0: d4f5 c734 c617 8235 b8d2 6535 04cf 8235  ...4...5..e5...5
+000004b0: 2a0a af33 0bed 0735 8c3e 8e35 cda6 cf34  *..3...5.>.5...4
+000004c0: f69f 2a35 1b27 5935 ca48 0d34 4cf3 a735  ..*5.'Y5.H.4L..5
+000004d0: 3618 0134 30ed 9035 d67d 0b35 be88 2035  6..40..5.}.5.. 5
+000004e0: 97b0 fa34 b0c9 6d35 32f8 1234 4bf0 b434  ...4..m52..4K..4
+000004f0: 0102 c135 f0df 9c33 f8cd 0c35 e37b aa34  ...5...3...5.{.4
+00000500: fd33 9634 01d8 a233 c93f 8833 e731 6435  .3.4...3.?.3.1d5
+00000510: 13b9 ad32 dc80 6a33 db63 8633 9ab5 9334  ...2..j3.c.3...4
+00000520: 10c4 9333 89db 3a34 5fb7 2534 1a5a 3d34  ...3..:4_.%4.Z=4
+00000530: d398 7432 a89b bf33 d950 4c34 5d57 9233  ..t2...3.PL4]W.3
+00000540: f1c2 f933 740d 2134 654d cf32 4729 6d34  ...3t.!4eM.2G)m4
+00000550: e13c b632 a1d7 4f34 836a c533 9dc5 f033  .<.2..O4.j.3...3
+00000560: a615 b333 ec92 2f34 7f55 d132 9e63 7c33  ...3../4.U.2.c|3
+00000570: 4655 8f34 a5d0 5f32 21ad d233 97ab 7a33  FU.4.._2!..3..z3
+00000580: 0f2c bf35 ea94 0b35 b5c8 e034 e361 6236  .,.5...5...4.ab6
+00000590: 8cd0 0534 ae8c 5334 da25 d434 68ae 8c35  ...4..S4.%.4h..5
+000005a0: 8414 8234 ba94 9435 2dee 8835 6b91 9e35  ...4...5-..5k..5
+000005b0: b6e2 c533 40e0 1635 2584 7135 faf7 ee34  ...3@..5%.q5...4
+000005c0: 43c2 4635 9dbf 6f35 a23d 2434 86f8 bd35  C.F5..o5.=$4...5
+000005d0: f17f 0534 9c22 8635 b0a4 0735 1e6a ef34  ...4.".5...5.j.4
+000005e0: 1917 d934 d79d 6c35 6c72 dc33 1d94 a034  ...4..l5lr.3...4
+000005f0: 3bd4 8a35 c6aa 6433 d616 d934 f6fe a434  ;..5..d3...4...4
+00000600: 772a e235 de5d 0e35 a681 f634 2bcc 8736  w*.5.].5...4+..6
+00000610: 2a49 1334 bdfb 6434 3046 eb34 63a2 ad35  *I.4..d40F.4c..5
+00000620: 3a6d 9f34 8c20 a735 051d 9635 3a81 ab35  :m.4. .5...5:..5
+00000630: b3e3 d333 9e28 1335 633c 7035 2b11 fd34  ...3.(.5c<p5+..4
+00000640: f8c5 5935 b827 8835 5c55 3134 7815 bd35  ..Y5.'.5\U14x..5
+00000650: f2c8 1934 2c6d 8735 af41 0235 ae15 1435  ...4,m.5.A.5...5
+00000660: 6759 d534 b7c0 8c35 5743 df33 9ba1 9e34  gY.4...5WC.3...4
+00000670: 2f87 a235 ee63 6433 4e6c 0635 3a8f c534  /..5.cd3Nl.5:..4
+00000680: 01ad b333 6f3a b932 2085 9932 debf 7f34  ...3o:.2 ..2...4
+00000690: b1aa cf31 d06d 7132 554f a232 f08c a733  ...1.mq2UO.2...3
+000006a0: 4fb6 a032 0330 5833 bd6d 4233 bcb6 5f33  O..2.0X3.mB3.._3
+000006b0: 60bd 7d31 4d58 cc32 9df2 4e33 9c85 9b32  `.}1MX.2..N3...2
+000006c0: 672f 1533 9d93 4333 03e2 f431 b205 7f33  g/.3..C3...1...3
+000006d0: eefb c631 b9fa 5233 83a7 ca32 cc2f 0933  ...1..R3...2./.3
+000006e0: b9a6 b432 2b73 5033 03aa d331 7431 7832  ...2+sP3...1t1x2
+000006f0: 2cbd 9b33 fb65 5d31 0a95 f132 2715 9332  ,..3.e]1...2'..2
+00000700: dd71 0f35 a6ff 2c34 dfd2 0f34 9d68 d435  .q.5..,4...4.h.5
+00000710: de37 2f33 4f8e df33 4876 0634 dd6e 0835  .7/3O..3Hv.4.n.5
+00000720: 1fe7 0934 faf0 c134 a86b ab34 1ace c334  ...4...4.k.4...4
+00000730: 1a2d 0433 4426 4b34 64f1 cd34 2045 1d34  .-.3D&K4d..4 E.4
+00000740: 721e 7c34 0ce2 9e34 1f8e 5033 8d39 fc34  r.|4...4..P3.9.4
+00000750: 1190 3e33 7708 d534 85f9 4c34 4b84 5f34  ..>3w..4..L4K._4
+00000760: 80b7 3534 53a4 ab34 01f0 4e33 09e6 0434  ..54S..4..N3...4
+00000770: 5850 0735 6dd8 dd32 c2bf 4434 b960 f533  XP.5m..2..D4.`.3
+00000780: cda3 4d35 f50e 7134 f556 4334 292c 1e36  ..M5..q4.VC4),.6
+00000790: 36db 7a33 153b 2a34 088c 3a34 21ce 4635  6.z3.;*4..:4!.F5
+000007a0: 4d1b 4a34 a04b 0335 c14d eb34 8d27 0635  M.J4.K.5.M.4.'.5
+000007b0: d069 3933 1130 9234 bb3e 1b35 9cb3 5b34  .i93.0.4.>.5..[4
+000007c0: 379d b234 87ea dd34 8d99 9633 0dea 3335  7..4...4...3..35
+000007d0: e339 8133 5643 1f35 c453 9734 ef31 a134  .9.3VC.5.S.4.1.4
+000007e0: f6b1 8834 0200 eb34 957c 9a33 688f 4734  ...4...4.|.3h.G4
+000007f0: 80b2 4c35 c0a3 2833 abb2 8c34 4465 2834  ..L5..(3...4De(4
+00000800: 9753 da35 9e02 f334 cd8b d534 89dd 9036  .S.5...4...4...6
+00000810: 3dee 0434 10e2 7f34 d863 d034 407a b835  =..4...4.c.4@z.5
+00000820: 3dde ac34 486e 9235 3c2b 8235 7a07 9435  =..4Hn.5<+.5z..5
+00000830: b3bb ba33 ec42 0135 cb53 7235 c0f5 dd34  ...3.B.5.Sr5...4
+00000840: 8ff0 4035 b805 7735 2582 1d34 3dd9 a535  ..@5..w5%..4=..5
+00000850: 2434 0934 e485 8435 b898 f234 ced0 1935  $4.4...5...4...5
+00000860: 8008 d434 1847 8235 88f2 dd33 7854 9b34  ...4.G.5...3xT.4
+00000870: a3f4 b035 adf8 6f33 3975 0935 ed17 b834  ...5..o39u.5...4
+00000880: 04fc a535 d729 b834 73a0 9d34 b476 6c36  ...5.).4s..4.vl6
+00000890: 126a c533 bc41 6334 26b5 9934 f861 9735  .j.3.Ac4&..4.a.5
+000008a0: 2eca 9134 e288 5735 ab35 3f35 f159 5a35  ...4..W5.5?5.YZ5
+000008b0: 7dfa 8b33 726f ce34 ee85 4f35 8f54 a734  }..3ro.4..O5.T.4
+000008c0: b367 0e35 592f 3735 3c63 e933 8657 8235  .g.5Y/75<c.3.W.5
+000008d0: 063b cd33 6e57 5b35 3e70 cb34 a93c f934  .;.3nW[5>p.4.<.4
+000008e0: 5d38 b534 47b5 4335 8697 c633 0b8f 8234  ]8.4G.C5...3...4
+000008f0: 83ba 9235 c45a 5633 bd38 dc34 cef2 8a34  ...5.ZV3.8.4...4
+00000900: d5c7 8035 9b5f a334 dffb 8234 7752 3b36  ...5._.4...4wR;6
+00000910: 5484 a333 6e1c 4834 eb7e 7634 f03c 6b35  T..3n.H4.~v4.<k5
+00000920: f36c 6d34 1377 2f35 94b8 1d35 f25b 3535  .lm4.w/5...5.[55
+00000930: efa3 7333 ec3f c134 9c9a 3f35 88e1 9134  ..s3.?.4..?5...4
+00000940: 35c5 eb34 4fb1 1035 8f31 c533 e8b4 6e35  5..4O..5.1.3..n5
+00000950: 61de a633 f432 4735 7070 c134 45ee bf34  a..3.2G5pp.4E..4
+00000960: 9ac6 a934 d487 1635 e5bf ba33 1bc8 7934  ...4...5...3..y4
+00000970: 2e4c 7135 c719 4b33 e3dc a834 341f 5634  .Lq5..K3...44.V4
+00000980: 36ef d732 ba86 0f32 158a ee31 8356 a733  6..2...2...1.V.3
+00000990: c7e5 0831 96c1 be31 0d5d cd31 02cc d532  ...1...1.].1...2
+000009a0: 4104 e031 085c 9c32 22de 8832 7fae 9b32  A..1.\.2"..2...2
+000009b0: 4ad5 e830 018d 2f32 c0a2 b432 e9c2 0732  J..0../2...2...2
+000009c0: 6791 4232 8b4a 7032 98fd 2031 4919 d932  g.B2.Jp2.. 1I..2
+000009d0: 44d1 2231 3efc ba32 2c45 3432 2472 2e32  D."1>..2,E42$r.2
+000009e0: dedc 1f32 6d4d 8432 9f1b 3731 d3c6 f431  ...2mM.2..71...1
+000009f0: eaab db32 dee6 c330 b237 1932 46ec be31  ...2...0.7.2F..1
+00000a00: 8d1e ef35 d3b7 0435 9c71 e234 d7e8 b536  ...5...5.q.4...6
+00000a10: fe47 0634 61bf ba34 a3eb d934 2dfe ef35  .G.4a..4...4-..5
+00000a20: c93c f034 9725 9b35 37f4 8835 9607 9c35  .<.4.%.57..5...5
+00000a30: 16b6 c533 aab6 1a35 3637 a235 ec43 ee34  ...3...567.5.C.4
+00000a40: 37ca 4435 64ba 8135 b06c 1f34 db82 c035  7.D5d..5.l.4...5
+00000a50: 914f 1734 4670 a435 724d 1e35 286c 4435  .O.4Fp.5rM.5(lD5
+00000a60: 285e 0e35 b1c3 9135 735b 2734 b031 c834  (^.5...5s['4.1.4
+00000a70: e361 e235 68b6 b133 6263 2c35 3ce3 cf34  .a.5h..3bc,5<..4
+00000a80: 65a1 4636 5337 1b35 944d 1835 0200 2637  e.F6S7.5.M.5..&7
+00000a90: 65e0 4b34 6476 2135 8ae5 1735 3950 5436  e.K4dv!5...59PT6
+00000aa0: 68d7 5235 147e d435 583b b735 0d7d c635  h.R5.~.5X;.5.}.5
+00000ab0: e8b6 1334 92b7 3b35 e400 fc35 6810 2635  ...4..;5...5h.&5
+00000ac0: 78e7 8b35 a928 bf35 f859 6a34 c750 ee35  x..5.(.5.Yj4.P.5
+00000ad0: 934e 6a34 426f 0136 a07b 5335 8db7 ab35  .Nj4Bo.6.{S5...5
+00000ae0: 31f9 5535 6a86 de35 fc07 8134 db8d 1b35  1.U5j..5...4...5
+00000af0: 249c 5136 2019 0c34 adec 9435 c3b3 2135  $.Q6 ..4...5..!5
+00000b00: f18a 9f33 1431 a532 d77e 8132 d5e0 6934  ...3.1.2.~.2..i4
+00000b10: 552c b931 9ff1 6432 9d03 8d32 58f2 9833  U,.1..d2...2X..3
+00000b20: c654 9332 c9c7 3833 8b0f 2833 8438 4233  .T.2..83..(3.8B3
+00000b30: 5d6e 5331 cb08 bb32 95a7 4233 f7b7 8432  ]nS1...2..B3...2
+00000b40: 9228 0233 385b 2b33 e46a d631 362e 6733  .(.38[+3.j.16.g3
+00000b50: 4ae2 a631 a93a 4333 95e8 bd32 5511 f732  J..1.:C3...2U..2
+00000b60: 7e4e a932 ae3b 3433 7ff1 c831 abb8 6a32  ~N.2.;43...1..j2
+00000b70: 3b93 9033 3346 5131 3941 d832 76af 7d32  ;..33FQ19A.2v.}2
+00000b80: 0da4 0537 5e08 1c36 3e0c fa35 ddf1 b837  ...7^..6>..5...7
+00000b90: a069 2635 7a2f b135 e5fd fb35 50ac e036  .i&5z/.5...5P..6
+00000ba0: ffe1 d035 8426 aa36 8308 9b36 0b08 b336  ...5.&.6...6...6
+00000bb0: 0f81 e034 bf07 3036 5674 ad36 4e09 0936  ...4..06Vt.6N..6
+00000bc0: 0c4a 6f36 9f5e 9536 7fa1 4535 29d0 dd36  .Jo6.^.6..E5)..6
+00000bd0: 10d4 1335 3b41 ba36 31a5 2b36 739c 3736  ...5;A.61.+6s.76
+00000be0: 7fce 1736 54ec 9336 0440 0e35 7c0c de35  ...6T..6.@.5|..5
+00000bf0: a59d ea36 d4f7 a934 960f 2236 ec9c d035  ...6...4.."6...5
+00000c00: 4d26 3737 98d5 4c36 f88d 2b36 29b9 0538  M&77..L6..+6)..8
+00000c10: a61c 5535 b179 0336 c22a 2736 fd9b 2737  ..U5.y.6.*'6..'7
+00000c20: 3f4e 2036 ef56 ea36 0c25 d136 400b ef36  ?N 6.V.6.%.6@..6
+00000c30: eb60 1935 92cc 6a36 45c5 f336 6818 3a36  .`.5..j6E..6h.:6
+00000c40: b1e5 9a36 57b1 c736 337d 7a35 656b 1437  ...6W..63}z5ek.7
+00000c50: 7317 5535 4f8b 0037 6719 6b36 dfdc 8836  s.U5O..7g.k6...6
+00000c60: 13a3 5436 73a3 d236 339d 5235 60bd 1a36  ..T6s..63.R5`..6
+00000c70: 2035 2937 c56a f734 bcd5 7036 a7aa 1536   5)7.j.4..p6...6
+00000c80: 495b 5e35 13b8 6f34 7ab6 4234 7728 2a36  I[^5..o4z.B4w(*6
+00000c90: a126 8333 0ba9 3034 163f 4434 a4ad 5a35  .&.3..04.?D4..Z5
+00000ca0: 0b93 5c34 60b3 0635 5e23 f034 9aca 0835  ..\4`..5^#.4...5
+00000cb0: 1ffa 2e33 6641 8e34 357e 1835 064b 5134  ...3fA.45~.5.KQ4
+00000cc0: 841b ba34 36d0 ec34 5954 9b33 b79e 2e35  ...46..4YT.3...5
+00000cd0: 5fa9 8333 be8a 1935 5eac 9334 07bf b134  _..3...5^..4...4
+00000ce0: 5abc 8534 0bfb fd34 8033 a033 f160 4034  Z..4...4.3.3.`@4
+00000cf0: 5ceb 5735 c726 2a33 6455 9b34 bb4b 3634  \.W5.&*3dU.4.K64
+00000d00: 0c1b 1934 2e51 2e33 f3d6 1033 1730 ef34  ...4.Q.3...3.0.4
+00000d10: 2086 3532 2583 0033 358f 0833 3ed8 1734   .52%..35..3>..4
+00000d20: ab49 1b33 25fd c233 a685 ad33 6566 c433  .I.3%..3...3ef.3
+00000d30: 2c6c 0932 7e40 5433 51a7 e533 769c 2133  ,l.2~@T3Q..3v.!3
+00000d40: d3ff 8133 df4f a333 0be2 5932 c2c3 0234  ...3.O.3..Y2...4
+00000d50: 420e 4332 246e ea33 8ca6 5d33 cfa6 7633  B.C2$n.3..]3..v3
+00000d60: 7ee9 4933 1ea7 b133 53b2 6832 ff2d 1233  ~.I3...3S.h2.-.3
+00000d70: cf21 1a34 a039 fc31 c226 5733 b141 ff32  .!.4.9.1.&W3.A.2
+00000d80: 3c0a 9834 f470 a533 215b 8633 af3f 5f35  <..4.p.3![.3.?_5
+00000d90: 2208 b232 d02d 6033 bc0e 8933 04dd 9034  "..2.-`3...3...4
+00000da0: 42f5 8d33 4c75 3a34 f802 2734 d3a3 4034  B..3Lu:4..'4..@4
+00000db0: 478c 6732 8034 be33 d18f 4434 ab43 8d33  G.g2.4.3..D4.C.3
+00000dc0: c05e ff33 19e2 2434 261c d232 989e 6b34  .^.3..$4&..2..k4
+00000dd0: 8e10 ae32 b99a 4734 1c90 c033 fbf4 eb33  ...2..G4...3...3
+00000de0: d224 ac33 c894 2f34 3d99 c632 3b99 7133  .$.3../4=..2;.q3
+00000df0: 2bee 8a34 4dba 5332 baf8 ce33 f606 7933  +..4M.S2...3..y3
+00000e00: a137 ac33 0f7a 8e32 251c 8032 e85d 7d34  .7.3.z.2%..2.]}4
+00000e10: 6318 bd31 13e0 5d32 97b8 8f32 27df a433  c..1..]2...2'..3
+00000e20: 3545 9c32 fb47 3933 b5f6 2433 e03b 3933  5E.2.G93..$3.;93
+00000e30: b342 5531 5d44 9832 a1e4 2b33 16a0 7b32  .BU1]D.2..+3..{2
+00000e40: 8c8e 0433 e2ff 3133 e62a dc31 b12f 4033  ...3..13.*.1./@3
+00000e50: 89a9 b431 d17f 3033 fe29 9b32 1fe5 0633  ...1..03.).2...3
+00000e60: e6b4 9232 3102 4133 2f20 b931 d99b 4b32  ...21.A3/ .1..K2
+00000e70: 4dbc 9833 e6de 3b31 58cd ec32 0b7e 8932  M..3..;1X..2.~.2
+00000e80: 23c3 1c36 a30a ed34 e169 ec34 0c4e fa36  #..6...4.i.4.N.6
+00000e90: b457 2434 a715 e534 7651 f334 32ca 1f36  .W$4...4vQ.42..6
+00000ea0: f18b 1b35 bd41 a735 1b7d 9035 4282 9c35  ...5.A.5.}.5B..5
+00000eb0: 7a97 de33 ab16 0735 b5af b035 72a2 f934  z..3...5...5r..4
+00000ec0: 5567 6135 0454 9935 807e 3c34 417b ad35  Uga5.T.5.~<4A{.5
+00000ed0: 70b5 3434 3197 b835 a596 1335 ac05 8235  p.441..5...5...5
+00000ee0: cb3b 1535 a1f1 ae35 9564 3534 774c da34  .;.5...5.d54wL.4
+00000ef0: 58bf 1b36 fecf c133 c0d3 6235 1261 fd34  X..6...3..b5.a.4
+00000f00: 1314 9b34 100d af33 f48c 8e33 90fd 6535  ...4...3...3..e5
+00000f10: 17c4 b832 e3a6 6c33 9ebf 8c33 307b 9434  ...2..l3...30{.4
+00000f20: 7a88 9333 19e9 4334 a551 2e34 f47e 4834  z..3..C4.Q.4.~H4
+00000f30: 8403 7d32 b8fa cb33 33e6 5234 cce0 9833  ..}2...33.R4...3
+00000f40: 9eec 0334 66b4 2834 dba3 d932 c798 7c34  ...4f.(4...2..|4
+00000f50: 5d1b bb32 6238 5734 124e cf33 5bc1 f133  ]..2b8W4.N.3[..3
+00000f60: 771c b933 2859 3434 2adc d432 27bd 8433  w..3(Y44*..2'..3
+00000f70: 81ff 9034 d4b6 6332 981f d433 e161 8033  ...4..c2...3.a.3
+00000f80: aaea 2033 86b4 6132 d481 4132 6195 0434  .. 3..a2..A2a..4
+00000f90: 3088 4d31 3eab 2032 082f 1832 b556 2833  0.M1>. 2./.2.V(3
+00000fa0: 85e0 3732 15dd f732 2cae d432 b6bb ee32  ..72...2,..2...2
+00000fb0: f95d 4831 60c7 8f32 b7fc 1833 927c 6432  .]H1`..2...3.|d2
+00000fc0: 18b7 9132 2c0d b132 9c20 7231 de9a 3133  ...2,..2. r1..13
+00000fd0: 4604 8931 62ce 1e33 9ad3 9632 383c 8932  F..1b..3...28<.2
+00000fe0: e594 8732 ddfa ca32 753b 9c31 452f 5532  ...2...2u;.1E/U2
+00000ff0: ed15 3333 cbcf 2831 d873 7032 cca6 1432  ..33..(1.sp2...2
```

##### archive/data/9

```diff
@@ -1,16 +1 @@
-00000000: ca62 4f39 561d 3b3a d924 df38 6668 2d3a  .bO9V.;:.$.8fh-:
-00000010: 2e0c 4739 9995 d239 c671 8939 248d be39  ..G9...9.q.9$..9
-00000020: f6eb 9439 6e96 6639 1533 1638 cc69 c138  ...9n.f9.3.8.i.8
-00000030: 7b87 a739 20a2 e538 94ea 4a3a f870 4039  {..9 ..8..J:.p@9
-00000040: 479e ee39 3c74 da39 3fd0 6a39 d845 5239  G..9<t.9?.j9.ER9
-00000050: 0b36 0b3a 691c 6b39 41f6 4a39 d288 1339  .6.:i.k9A.J9...9
-00000060: 9c99 8738 8cd6 f138 a105 3839 363e 9439  ...8...8..896>.9
-00000070: d5a4 3738 d383 ef38 ffb2 4c3a 4fe2 2039  ..78...8..L:O. 9
-00000080: cb62 4f39 551d 3b3a d724 df38 6668 2d3a  .bO9U.;:.$.8fh-:
-00000090: 2e0c 4739 9795 d239 c771 8939 248d be39  ..G9...9.q.9$..9
-000000a0: f4eb 9439 6e96 6639 1733 1638 cd69 c138  ...9n.f9.3.8.i.8
-000000b0: 7b87 a739 20a2 e538 93ea 4a3a f770 4039  {..9 ..8..J:.p@9
-000000c0: 4a9e ee39 3a74 da39 40d0 6a39 d545 5239  J..9:t.9@.j9.ER9
-000000d0: 0c36 0b3a 691c 6b39 43f6 4a39 d288 1339  .6.:i.k9C.J9...9
-000000e0: 9b99 8738 8fd6 f138 a105 3839 343e 9439  ...8...8..894>.9
-000000f0: d2a4 3738 d283 ef38 00b3 4c3a 4ce2 2039  ..78...8..L:L. 9
+00000000: 0000 7546                                ..uF
```

#### _stable_baselines3_version

```diff
@@ -1 +1 @@
-1.5.0
+1.8.0
```

#### system_info.txt

```diff
@@ -1,7 +1,7 @@
-OS: Linux-5.4.0-104-generic-x86_64-with-glibc2.29 #118-Ubuntu SMP Wed Mar 2 19:02:41 UTC 2022
-Python: 3.8.10
-Stable-Baselines3: 1.5.0
-PyTorch: 1.10.2+cu102
-GPU Enabled: False
-Numpy: 1.21.5
-Gym: 0.21.0
+- OS: Linux-5.4.0-148-generic-x86_64-with-glibc2.29 # 165-Ubuntu SMP Tue Apr 18 08:53:12 UTC 2023
+- Python: 3.8.10
+- Stable-Baselines3: 1.8.0
+- PyTorch: 2.0.0+cu117
+- GPU Enabled: False
+- Numpy: 1.24.3
+- Gym: 0.21.0
```

### Comparing `imitation-0.3.2/tests/testdata/expert_models/cartpole_0/rollouts/final.npz` & `imitation-0.4.0/tests/testdata/expert_models/cartpole_0/rollouts/final.npz`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/testdata/expert_models/pendulum_0/rollouts/final.npz` & `imitation-0.4.0/tests/testdata/expert_models/pendulum_0/rollouts/final.npz`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/util/test_logger.py` & `imitation-0.4.0/tests/util/test_logger.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/util/test_networks.py` & `imitation-0.4.0/tests/util/test_networks.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/util/test_registry.py` & `imitation-0.4.0/tests/util/test_registry.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/util/test_util.py` & `imitation-0.4.0/tests/util/test_util.py`

 * *Files identical despite different names*

### Comparing `imitation-0.3.2/tests/util/test_wb_logger.py` & `imitation-0.4.0/tests/util/test_wb_logger.py`

 * *Files identical despite different names*

