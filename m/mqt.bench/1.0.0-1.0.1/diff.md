# Comparing `tmp/mqt.bench-1.0.0.tar.gz` & `tmp/mqt.bench-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt.bench-1.0.0.tar", last modified: Sun Jul  2 15:00:45 2023, max compression
+gzip compressed data, was "mqt.bench-1.0.1.tar", last modified: Tue Jul 18 06:32:22 2023, max compression
```

## Comparing `mqt.bench-1.0.0.tar` & `mqt.bench-1.0.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.353476 mqt.bench-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.353476 mqt.bench-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.357476 mqt.bench-1.0.0/img/
--rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/arch.png
--rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/level_4.png
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/mqt_light.png
--rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/img/mqtbench.png
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.349476 mqt.bench-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.349476 mqt.bench-1.0.0/src/mqt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.361476 mqt.bench-1.0.0/src/mqt/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmark_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/ae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/dj.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/graphstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qft.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qftentangled.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_nature/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.365476 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeinexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/qwalk.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/realamprandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/shor.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/su2random.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/twolocalrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/vqe.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/benchmarks/wstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.385477 mqt.bench-1.0.0/src/mqt/bench/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123) 15925096 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation_visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.385477 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/
--rw-r--r--   0 runner    (1001) docker     (123)    16460 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/pie.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/qubit_dist.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/evaluation/results/violins.pdf
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/qiskit_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/tket_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/bench/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/MQTBench_all.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/qasm_output/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/files/qasm_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/static/tum_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/src/mqt/benchviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/benchmark_description.html
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/description.html
--rw-r--r--   0 runner    (1001) docker     (123)    28232 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/src/mqt/benchviewer/templates/legal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.357476 mqt.bench-1.0.0/src/mqt.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-02 15:00:45.000000 mqt.bench-1.0.0/src/mqt.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:45.389477 mqt.bench-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27066 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-02 15:00:34.000000 mqt.bench-1.0.0/tests/test_benchviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.580695 mqt.bench-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.540694 mqt.bench-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.540694 mqt.bench-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-07-18 06:32:22.580695 mqt.bench-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.544694 mqt.bench-1.0.1/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/arch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/level_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/level_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/level_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/level_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/mqt_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/img/mqtbench.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:32:22.580695 mqt.bench-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.536694 mqt.bench-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.536694 mqt.bench-1.0.1/src/mqt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.548694 mqt.bench-1.0.1/src/mqt/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmark_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.552694 mqt.bench-1.0.1/src/mqt/bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/graphstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qftentangled.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.552694 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.552694 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.552694 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_nature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.552694 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qpeexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qpeinexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/qwalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/realamprandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/shor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/su2random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/twolocalrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/vqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/benchmarks/wstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.572695 mqt.bench-1.0.1/src/mqt/bench/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123) 15925096 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/evaluation/evaluation_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/evaluation/evaluation_visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.576695 mqt.bench-1.0.1/src/mqt/bench/evaluation/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/evaluation/results/pie.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/evaluation/results/qubit_dist.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/evaluation/results/violins.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/qiskit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/tket_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/bench/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.576695 mqt.bench-1.0.1/src/mqt/benchviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.576695 mqt.bench-1.0.1/src/mqt/benchviewer/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.576695 mqt.bench-1.0.1/src/mqt/benchviewer/static/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/static/files/MQTBench_all.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.576695 mqt.bench-1.0.1/src/mqt/benchviewer/static/files/qasm_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/static/files/qasm_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/static/tum_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.576695 mqt.bench-1.0.1/src/mqt/benchviewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/templates/benchmark_description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/templates/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28232 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/src/mqt/benchviewer/templates/legal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.548694 mqt.bench-1.0.1/src/mqt.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-07-18 06:32:22.000000 mqt.bench-1.0.1/src/mqt.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-18 06:32:22.000000 mqt.bench-1.0.1/src/mqt.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:32:22.000000 mqt.bench-1.0.1/src/mqt.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-18 06:32:22.000000 mqt.bench-1.0.1/src/mqt.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 06:32:22.000000 mqt.bench-1.0.1/src/mqt.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 06:32:22.000000 mqt.bench-1.0.1/src/mqt.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:22.580695 mqt.bench-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27066 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-18 06:32:09.000000 mqt.bench-1.0.1/tests/test_benchviewer.py
```

### Comparing `mqt.bench-1.0.0/.github/dependabot.yml` & `mqt.bench-1.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/.github/release-drafter.yml` & `mqt.bench-1.0.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/.github/workflows/codeql.yml` & `mqt.bench-1.0.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/.github/workflows/coverage.yml` & `mqt.bench-1.0.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/.github/workflows/deploy.yml` & `mqt.bench-1.0.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/.gitignore` & `mqt.bench-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/.pre-commit-config.yaml` & `mqt.bench-1.0.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -66,21 +66,21 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, javascript, json]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+    rev: v0.0.275
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         files: ^(src|tests|setup.py)
         args: []
         additional_dependencies:
           - importlib_resources
           - pytest
```

### Comparing `mqt.bench-1.0.0/LICENSE` & `mqt.bench-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/PKG-INFO` & `mqt.bench-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.0.0
+Version: 1.0.1
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -246,19 +246,19 @@
 - `level`: `0` or `"alg"`, `1` or `"indep"`, `2` or `"nativegates"`, `3` or `"mapped"`
 - `circuit_size`: for most of the cases this is equal to number of qubits
   (all scalable benchmarks except `"qwalk-v-chain"` and `"grover-v-chain"`) while for all other the qubit number is higher
 - `compiler`: `"qiskit"` or `"tket"`
 - `compiler_settings`: Optimization level for `"qiskit"` (`0`-`3`), placement for `"tket"` (`lineplacement` or `graphplacement`), exemplary shown:
 
 ```python
-from mqt.bench import CompilerSettings
+from mqt.bench import CompilerSettings, QiskitSettings, TKETSettings
 
 compiler_settings = CompilerSettings(
-    qiskit={"optimization_level": 1},
-    tket={"placement": "lineplacement"},
+    qiskit=QiskitSettings(optimization_level=1),
+    tket=TKETSettings(placement="lineplacement"),
 )
 ```
 
 - `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, `"oqc"`, or `"quantinuum"`
 - `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"rigetti_aspen_m2"`, `"ionq_harmony"`, `"ionq_aria1"`, `"oqc_lucy"`, or `"quantinuum_h2"`
 
 Hereby, the mappings between shortened `benchmark_name` and actual benchmarks are:
```

### Comparing `mqt.bench-1.0.0/README.md` & `mqt.bench-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -194,19 +194,19 @@
 - `level`: `0` or `"alg"`, `1` or `"indep"`, `2` or `"nativegates"`, `3` or `"mapped"`
 - `circuit_size`: for most of the cases this is equal to number of qubits
   (all scalable benchmarks except `"qwalk-v-chain"` and `"grover-v-chain"`) while for all other the qubit number is higher
 - `compiler`: `"qiskit"` or `"tket"`
 - `compiler_settings`: Optimization level for `"qiskit"` (`0`-`3`), placement for `"tket"` (`lineplacement` or `graphplacement`), exemplary shown:
 
 ```python
-from mqt.bench import CompilerSettings
+from mqt.bench import CompilerSettings, QiskitSettings, TKETSettings
 
 compiler_settings = CompilerSettings(
-    qiskit={"optimization_level": 1},
-    tket={"placement": "lineplacement"},
+    qiskit=QiskitSettings(optimization_level=1),
+    tket=TKETSettings(placement="lineplacement"),
 )
 ```
 
 - `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, `"oqc"`, or `"quantinuum"`
 - `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"rigetti_aspen_m2"`, `"ionq_harmony"`, `"ionq_aria1"`, `"oqc_lucy"`, or `"quantinuum_h2"`
 
 Hereby, the mappings between shortened `benchmark_name` and actual benchmarks are:
```

### Comparing `mqt.bench-1.0.0/config.json` & `mqt.bench-1.0.1/config.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/arch.png` & `mqt.bench-1.0.1/img/arch.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/level_1.png` & `mqt.bench-1.0.1/img/level_1.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/level_2.png` & `mqt.bench-1.0.1/img/level_2.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/level_3.png` & `mqt.bench-1.0.1/img/level_3.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/level_4.png` & `mqt.bench-1.0.1/img/level_4.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/mqt_dark.png` & `mqt.bench-1.0.1/img/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/mqt_light.png` & `mqt.bench-1.0.1/img/mqt_light.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/img/mqtbench.png` & `mqt.bench-1.0.1/img/mqtbench.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/pyproject.toml` & `mqt.bench-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 keywords = ["MQT",  "quantum computing", "benchmarking", "performance", "testing"]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dynamic = ["version"]
 
 dependencies = [
-    "pytket-qiskit>=0.40.0,<0.41.0",  #  manages the dependencies for qiskit and tket in a combined fashion
+    "pytket-qiskit>=0.40.0,<0.42.0",  #  manages the dependencies for qiskit and tket in a combined fashion
     "qiskit[all]",  # this is merely to get the [all] dependencies. The versioning is covered by pytket-qiskit
     "pandas>=1.0.0",
     "flask>=2.0.0",
     "networkx>=2.0.0",
     "scipy<1.11.0",
     "pyscf>=2.1.0",
     "packaging>=21.0",
```

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmark_generator.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmark_generator.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/ae.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/ae.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/dj.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/dj.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/ghz.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/ghz.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/graphstate.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/graphstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/grover.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/grover.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qaoa.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qft.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qft.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qftentangled.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qftentangled.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeexact.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qpeexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qpeinexact.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qpeinexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/qwalk.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/qwalk.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from qiskit import AncillaRegister, QuantumCircuit, QuantumRegister
 
 
 def create_circuit(
     n: int,
     ancillary_mode: str = "noancilla",
     depth: int = 3,
-    coin_state_preparation: QuantumCircuit = None,
+    coin_state_preparation: QuantumCircuit | None = None,
 ) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Walk algorithm.
 
     Keyword arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     depth -- number of quantum steps
     coin_state_preparation -- optional quantum circuit for state preparation
```

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/random.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/random.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/realamprandom.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/realamprandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/shor.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/shor.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/su2random.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/su2random.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/twolocalrandom.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/twolocalrandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/vqe.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/vqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/benchmarks/wstate.py` & `mqt.bench-1.0.1/src/mqt/bench/benchmarks/wstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation.py` & `mqt.bench-1.0.1/src/mqt/bench/evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation_data.pkl` & `mqt.bench-1.0.1/src/mqt/bench/evaluation/evaluation_data.pkl`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/evaluation/evaluation_visualization.ipynb` & `mqt.bench-1.0.1/src/mqt/bench/evaluation/evaluation_visualization.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991593567251462%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(2, 'data = [perc_washington, perc_rigetti, perc_quantinuum, "*

 * *            "perc_montreal, perc_ionq_aria1, perc_ionq_harmony, perc_oqc]\\n')], delete: [2]}}, "*

 * *            "insert: [(14, OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'238ae571'), ('metadata', OrderedDict()), ('outputs', []), ('source', [])]))]}"}*

```diff
@@ -123,15 +123,15 @@
             "execution_count": null,
             "id": "089acc25",
             "metadata": {},
             "outputs": [],
             "source": [
                 "font = {\"size\": 12}\n",
                 "matplotlib.rc(\"font\", **font)\n",
-                "data = [perc_washington, perc_rigetti, perc_montreal, perc_quantinuum, perc_ionq_aria1, perc_ionq_harmony, perc_oqc]\n",
+                "data = [perc_washington, perc_rigetti, perc_quantinuum, perc_montreal, perc_ionq_aria1, perc_ionq_harmony, perc_oqc]\n",
                 "colors = [\"#B7E6A5\", \"#7CCBA2\", \"#46AEA0\", \"#089099\", \"#02818B\", \"#026688\", \"#025582\"]\n",
                 "labels = [\n",
                 "    \"IBMQ Washington (127)\",\n",
                 "    \"Rigetti Aspen M2 (80)\",\n",
                 "    \"Quantinuum H2 (32)\",\n",
                 "    \"IBMQ Montreal (27)\",\n",
                 "    \"IonQ Aria 1 (25)\",\n",
@@ -234,14 +234,22 @@
                 "    pc.set_facecolor(color)\n",
                 "\n",
                 "ax.set_xticks(pos)\n",
                 "plt.xticks(rotation=0)\n",
                 "ax.set_xticklabels(labels)\n",
                 "plt.savefig(\"results/violins.pdf\", format=\"pdf\", bbox_inches=\"tight\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "238ae571",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `mqt.bench-1.0.0/src/mqt/bench/evaluation/results/pie.pdf` & `mqt.bench-1.0.1/src/mqt/bench/evaluation/results/pie.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,23 +1,22 @@
 IBMQ Washington (127)
 Rigetti Aspen M2 (80)
 
 32.8%
 24.3%
-11.4%
+12.5%
 
 Quantinuum H2 (32)
 
-12.5%
-
-IBMQ Montreal (27)
+11.4%
 
 3.6%
 5.2%
 10.3%
 
 OQC Lucy (8)
 IonQ Harmony (11)
 
 IonQ Aria 1 (25)
+IBMQ Montreal (27)
```

### Comparing `mqt.bench-1.0.0/src/mqt/bench/evaluation/results/qubit_dist.pdf` & `mqt.bench-1.0.1/src/mqt/bench/evaluation/results/qubit_dist.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/evaluation/results/violins.pdf` & `mqt.bench-1.0.1/src/mqt/bench/evaluation/results/violins.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/qiskit_helper.py` & `mqt.bench-1.0.1/src/mqt/bench/qiskit_helper.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/tket_helper.py` & `mqt.bench-1.0.1/src/mqt/bench/tket_helper.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/bench/utils.py` & `mqt.bench-1.0.1/src/mqt/bench/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,17 +137,15 @@
             c_map_rigetti.append([m - 7, m + 6])
 
     for n in range(5):
         c_map_rigetti.append([n * 8 + 3, n * 8 + 5 * 8])
         c_map_rigetti.append([n * 8 + 4, n * 8 + 7 + 5 * 8])
 
     inverted = [[item[1], item[0]] for item in c_map_rigetti]
-    c_map_rigetti = c_map_rigetti + inverted
-
-    return c_map_rigetti
+    return c_map_rigetti + inverted
 
 
 def get_fully_connected_cmap(num_qubits: int) -> list[list[int]]:
     c_map = []
     for i in range(0, num_qubits):
         for j in range(0, num_qubits):
             if i != j:
```

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/backend.py` & `mqt.bench-1.0.1/src/mqt/benchviewer/backend.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/main.py` & `mqt.bench-1.0.1/src/mqt/benchviewer/main.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/static/favicon.ico` & `mqt.bench-1.0.1/src/mqt/benchviewer/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/static/mqt_dark.png` & `mqt.bench-1.0.1/src/mqt/benchviewer/static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/static/tum_logo.svg` & `mqt.bench-1.0.1/src/mqt/benchviewer/static/tum_logo.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/templates/benchmark_description.html` & `mqt.bench-1.0.1/src/mqt/benchviewer/templates/benchmark_description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/templates/description.html` & `mqt.bench-1.0.1/src/mqt/benchviewer/templates/description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/templates/index.html` & `mqt.bench-1.0.1/src/mqt/benchviewer/templates/index.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt/benchviewer/templates/legal.html` & `mqt.bench-1.0.1/src/mqt/benchviewer/templates/legal.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/src/mqt.bench.egg-info/PKG-INFO` & `mqt.bench-1.0.1/src/mqt.bench.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.0.0
+Version: 1.0.1
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -246,19 +246,19 @@
 - `level`: `0` or `"alg"`, `1` or `"indep"`, `2` or `"nativegates"`, `3` or `"mapped"`
 - `circuit_size`: for most of the cases this is equal to number of qubits
   (all scalable benchmarks except `"qwalk-v-chain"` and `"grover-v-chain"`) while for all other the qubit number is higher
 - `compiler`: `"qiskit"` or `"tket"`
 - `compiler_settings`: Optimization level for `"qiskit"` (`0`-`3`), placement for `"tket"` (`lineplacement` or `graphplacement`), exemplary shown:
 
 ```python
-from mqt.bench import CompilerSettings
+from mqt.bench import CompilerSettings, QiskitSettings, TKETSettings
 
 compiler_settings = CompilerSettings(
-    qiskit={"optimization_level": 1},
-    tket={"placement": "lineplacement"},
+    qiskit=QiskitSettings(optimization_level=1),
+    tket=TKETSettings(placement="lineplacement"),
 )
 ```
 
 - `gate_set_name`: `"ibm"`, `"rigetti"`, `"ionq"`, `"oqc"`, or `"quantinuum"`
 - `device_name`: `"ibm_washington"`, `"ibm_montreal"`, `"rigetti_aspen_m2"`, `"ionq_harmony"`, `"ionq_aria1"`, `"oqc_lucy"`, or `"quantinuum_h2"`
 
 Hereby, the mappings between shortened `benchmark_name` and actual benchmarks are:
```

### Comparing `mqt.bench-1.0.0/src/mqt.bench.egg-info/SOURCES.txt` & `mqt.bench-1.0.1/src/mqt.bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/tests/test_bench.py` & `mqt.bench-1.0.1/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.0/tests/test_benchviewer.py` & `mqt.bench-1.0.1/tests/test_benchviewer.py`

 * *Files identical despite different names*

