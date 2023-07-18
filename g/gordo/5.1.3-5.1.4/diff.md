# Comparing `tmp/gordo-5.1.3.tar.gz` & `tmp/gordo-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gordo-5.1.3.tar", last modified: Tue Jul  4 10:20:56 2023, max compression
+gzip compressed data, was "gordo-5.1.4.tar", last modified: Tue Jul 18 13:45:08 2023, max compression
```

## Comparing `gordo-5.1.3.tar` & `gordo-5.1.4.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.060648 gordo-5.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 10:18:37.000000 gordo-5.1.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 10:18:37.000000 gordo-5.1.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 10:18:37.000000 gordo-5.1.3/.github/dependabot.yml 
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-04 10:18:37.000000 gordo-5.1.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-04 10:18:37.000000 gordo-5.1.3/.github/workflows/master-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-04 10:18:37.000000 gordo-5.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-04 10:18:37.000000 gordo-5.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-04 10:18:37.000000 gordo-5.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/.trivyignore
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-04 10:18:37.000000 gordo-5.1.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-04 10:18:37.000000 gordo-5.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-04 10:18:37.000000 gordo-5.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-04 10:20:56.060648 gordo-5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-04 10:18:37.000000 gordo-5.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 10:18:37.000000 gordo-5.1.3/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/benchmarks/load_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-04 10:18:37.000000 gordo-5.1.3/benchmarks/load_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-04 10:18:37.000000 gordo-5.1.3/benchmarks/load_test/load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-04 10:18:37.000000 gordo-5.1.3/benchmarks/load_test/task_set.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-04 10:18:37.000000 gordo-5.1.3/benchmarks/test_ml_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 10:18:37.000000 gordo-5.1.3/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/_static/Gordo_C4.README
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/_static/Gordo_C4.svg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/_static/_placeholder.txt
--rw-r--r--   0 runner    (1001) docker     (123)   113230 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/_static/architecture_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/_static/architecture_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/_static/argo_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/_static/endpoint-metadata.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/docs/api/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/loader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.044648 gordo-5.1.3/docs/api/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/model-factories.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/register.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/transformer-funcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/model/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/machine/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/reporters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/serializer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/docs/api/server/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/server/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/server/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/server/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/server/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/server/properties.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/server/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/server/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/api/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/docs/general/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/general/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/general/cluster_deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/general/endpoints.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/general/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/docs/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/ml/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/ml/model_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/ml/model_output.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-04 10:18:37.000000 gordo-5.1.3/docs/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    42032 2023-07-04 10:18:37.000000 gordo-5.1.3/examples/Gordo-Workflow-High-Level.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-07-04 10:18:37.000000 gordo-5.1.3/examples/Pipelines-with-Gordo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-04 10:18:37.000000 gordo-5.1.3/examples/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-04 10:18:37.000000 gordo-5.1.3/examples/model-configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-04 10:18:37.000000 gordo-5.1.3/examples/test-project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-04 10:18:37.000000 gordo-5.1.3/functions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 10:20:55.000000 gordo-5.1.3/gordo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26331 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/builder/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/builder/local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/cli/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/cli/exceptions_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/cli/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/anomaly/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/anomaly/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/machine/model/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/factories/feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/factories/lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/factories/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/machine/model/transformer_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/transformer_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/transformer_funcs/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/machine/model/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/transformers/imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/machine/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/reporters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/reporters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/reporters/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/reporters/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/serializer/from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/serializer/into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/serializer/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/serializer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/server/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/blueprints/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/blueprints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/model_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/server/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/prometheus/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/prometheus/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/prometheus/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/util/disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/util/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/util/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/workflow/config_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/config_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/config_elements/normalized_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/config_elements/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/workflow/workflow_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/workflow_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/workflow_generator/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.052647 gordo-5.1.3/gordo/workflow/workflow_generator/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/workflow_generator/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70808 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-04 10:18:37.000000 gordo-5.1.3/gordo/workflow/workflow_generator/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.048647 gordo-5.1.3/gordo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-04 10:20:55.000000 gordo-5.1.3/gordo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-04 10:20:56.000000 gordo-5.1.3/gordo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:20:55.000000 gordo-5.1.3/gordo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-04 10:20:55.000000 gordo-5.1.3/gordo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-04 10:20:55.000000 gordo-5.1.3/gordo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 10:20:55.000000 gordo-5.1.3/gordo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:20:55.000000 gordo-5.1.3/gordo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-04 10:18:37.000000 gordo-5.1.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-04 10:18:37.000000 gordo-5.1.3/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 10:18:37.000000 gordo-5.1.3/requirements/docs_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-04 10:18:37.000000 gordo-5.1.3/requirements/full_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 10:18:37.000000 gordo-5.1.3/requirements/mlflow_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 10:18:37.000000 gordo-5.1.3/requirements/postgres_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-04 10:18:37.000000 gordo-5.1.3/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 10:18:37.000000 gordo-5.1.3/requirements/test_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-04 10:18:37.000000 gordo-5.1.3/requirements/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.040647 gordo-5.1.3/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.040647 gordo-5.1.3/resources/grafana/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/resources/grafana/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-07-04 10:18:37.000000 gordo-5.1.3/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 10:18:37.000000 gordo-5.1.3/resources/grafana/dashboards/how_to_modify_dashboard.md
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-07-04 10:18:37.000000 gordo-5.1.3/resources/grafana/dashboards/machines.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-07-04 10:18:37.000000 gordo-5.1.3/run_workflow_and_argo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-04 10:18:37.000000 gordo-5.1.3/scripts/download_argo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-04 10:18:37.000000 gordo-5.1.3/scripts/github_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-04 10:18:37.000000 gordo-5.1.3/scripts/tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 10:18:37.000000 gordo-5.1.3/scripts/trivy_scan.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:20:56.060648 gordo-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 10:18:37.000000 gordo-5.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/config-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/builder/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/builder/test_local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/builder/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/cli/test_exception_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/client/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/metadata/test_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_factories_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_raw_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/model/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.056648 gordo-5.1.3/tests/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/reporters/test_mlflow_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/reporters/test_postgres_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.060648 gordo-5.1.3/tests/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/serializer/definition_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/serializer/test_serializer_from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/serializer/test_serializer_into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/serializer/test_serializer_load_dump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.060648 gordo-5.1.3/tests/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/server/test_anomaly_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/server/test_base_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/server/test_gordo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/server/test_model_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/server/test_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/server/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.060648 gordo-5.1.3/tests/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/util/test_disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/util/test_sensor_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/util/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.060648 gordo-5.1.3/tests/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_config_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_normalized_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.060648 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:20:56.060648 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
--rw-r--r--   0 runner    (1001) docker     (123)    28554 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/mocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-04 10:18:37.000000 gordo-5.1.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.651140 gordo-5.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 13:43:05.000000 gordo-5.1.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 13:43:05.000000 gordo-5.1.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 13:43:05.000000 gordo-5.1.4/.github/dependabot.yml 
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-18 13:43:05.000000 gordo-5.1.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-18 13:43:05.000000 gordo-5.1.4/.github/workflows/master-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-18 13:43:05.000000 gordo-5.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 13:43:05.000000 gordo-5.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-18 13:43:05.000000 gordo-5.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/.trivyignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-18 13:43:05.000000 gordo-5.1.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-18 13:43:05.000000 gordo-5.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-18 13:43:05.000000 gordo-5.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-18 13:45:08.651140 gordo-5.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-18 13:43:05.000000 gordo-5.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-18 13:43:05.000000 gordo-5.1.4/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/benchmarks/load_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-18 13:43:05.000000 gordo-5.1.4/benchmarks/load_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-18 13:43:05.000000 gordo-5.1.4/benchmarks/load_test/load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-18 13:43:05.000000 gordo-5.1.4/benchmarks/load_test/task_set.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-18 13:43:05.000000 gordo-5.1.4/benchmarks/test_ml_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-18 13:43:05.000000 gordo-5.1.4/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/_static/Gordo_C4.README
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/_static/Gordo_C4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/_static/_placeholder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   113230 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/_static/architecture_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/_static/architecture_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/_static/argo_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/_static/endpoint-metadata.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.631139 gordo-5.1.4/docs/api/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/loader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/docs/api/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/model-factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/register.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/transformer-funcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/model/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/machine/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/reporters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/serializer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/docs/api/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/server/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/server/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/server/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/server/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/server/properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/server/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/server/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/api/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/docs/general/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/general/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/general/cluster_deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/general/endpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/general/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/docs/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/ml/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/ml/model_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/ml/model_output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-18 13:43:05.000000 gordo-5.1.4/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    42032 2023-07-18 13:43:05.000000 gordo-5.1.4/examples/Gordo-Workflow-High-Level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-07-18 13:43:05.000000 gordo-5.1.4/examples/Pipelines-with-Gordo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-18 13:43:05.000000 gordo-5.1.4/examples/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-18 13:43:05.000000 gordo-5.1.4/examples/model-configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 13:43:05.000000 gordo-5.1.4/examples/test-project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-18 13:43:05.000000 gordo-5.1.4/functions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26331 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/builder/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/builder/local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/cli/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/cli/exceptions_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/cli/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/anomaly/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/anomaly/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/machine/model/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/factories/feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/factories/lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/factories/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/machine/model/transformer_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/transformer_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/transformer_funcs/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/machine/model/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/transformers/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/machine/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/reporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/reporters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/reporters/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/reporters/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/serializer/from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/serializer/into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/serializer/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/serializer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/server/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/blueprints/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/blueprints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/model_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.639140 gordo-5.1.4/gordo/server/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/prometheus/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/prometheus/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/prometheus/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/util/disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/util/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/gordo/workflow/config_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/config_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/config_elements/normalized_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/config_elements/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/gordo/workflow/workflow_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/workflow_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/workflow_generator/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/gordo/workflow/workflow_generator/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/workflow_generator/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70808 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-18 13:43:05.000000 gordo-5.1.4/gordo/workflow/workflow_generator/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.635139 gordo-5.1.4/gordo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:45:08.000000 gordo-5.1.4/gordo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 13:43:05.000000 gordo-5.1.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-18 13:43:05.000000 gordo-5.1.4/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-18 13:43:05.000000 gordo-5.1.4/requirements/docs_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-18 13:43:05.000000 gordo-5.1.4/requirements/full_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 13:43:05.000000 gordo-5.1.4/requirements/mlflow_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 13:43:05.000000 gordo-5.1.4/requirements/postgres_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-18 13:43:05.000000 gordo-5.1.4/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 13:43:05.000000 gordo-5.1.4/requirements/test_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-18 13:43:05.000000 gordo-5.1.4/requirements/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.627139 gordo-5.1.4/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.627139 gordo-5.1.4/resources/grafana/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/resources/grafana/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-07-18 13:43:05.000000 gordo-5.1.4/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 13:43:05.000000 gordo-5.1.4/resources/grafana/dashboards/how_to_modify_dashboard.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-07-18 13:43:05.000000 gordo-5.1.4/resources/grafana/dashboards/machines.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-07-18 13:43:05.000000 gordo-5.1.4/run_workflow_and_argo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-18 13:43:05.000000 gordo-5.1.4/scripts/download_argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-18 13:43:05.000000 gordo-5.1.4/scripts/github_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-18 13:43:05.000000 gordo-5.1.4/scripts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-18 13:43:05.000000 gordo-5.1.4/scripts/trivy_scan.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:45:08.651140 gordo-5.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-18 13:43:05.000000 gordo-5.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/config-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/tests/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/tests/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/builder/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/builder/test_local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/builder/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/tests/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/cli/test_exception_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.643139 gordo-5.1.4/tests/gordo/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/client/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.647140 gordo-5.1.4/tests/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.647140 gordo-5.1.4/tests/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/metadata/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.647140 gordo-5.1.4/tests/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.647140 gordo-5.1.4/tests/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_factories_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_raw_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/model/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.647140 gordo-5.1.4/tests/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/reporters/test_mlflow_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/reporters/test_postgres_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.647140 gordo-5.1.4/tests/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/serializer/definition_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/serializer/test_serializer_from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/serializer/test_serializer_into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/serializer/test_serializer_load_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.651140 gordo-5.1.4/tests/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/server/test_anomaly_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/server/test_base_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/server/test_gordo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/server/test_model_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/server/test_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/server/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.651140 gordo-5.1.4/tests/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/util/test_disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/util/test_sensor_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.651140 gordo-5.1.4/tests/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_config_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_normalized_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.651140 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:45:08.651140 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    28554 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/mocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-18 13:43:05.000000 gordo-5.1.4/tests/utils.py
```

### Comparing `gordo-5.1.3/.github/workflows/main.yml` & `gordo-5.1.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/.github/workflows/master-ci.yml` & `gordo-5.1.4/.github/workflows/master-ci.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/.github/workflows/release.yml` & `gordo-5.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/.gitignore` & `gordo-5.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/Dockerfile` & `gordo-5.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/LICENSE` & `gordo-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/Makefile` & `gordo-5.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/PKG-INFO` & `gordo-5.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.1.3
+Version: 5.1.4
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.1.3 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.1.4 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
 Extra: mlflow Provides-Extra: postgres Provides-Extra: tests Provides-Extra:
```

### Comparing `gordo-5.1.3/README.md` & `gordo-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/benchmarks/load_test/README.md` & `gordo-5.1.4/benchmarks/load_test/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/benchmarks/load_test/load_test.py` & `gordo-5.1.4/benchmarks/load_test/load_test.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/benchmarks/test_ml_server.py` & `gordo-5.1.4/benchmarks/test_ml_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/Makefile` & `gordo-5.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/_static/Gordo_C4.svg` & `gordo-5.1.4/docs/_static/Gordo_C4.svg`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/_static/architecture_diagram.png` & `gordo-5.1.4/docs/_static/architecture_diagram.png`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/_static/architecture_diagram.py` & `gordo-5.1.4/docs/_static/architecture_diagram.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/_static/argo_logo.png` & `gordo-5.1.4/docs/_static/argo_logo.png`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/_static/endpoint-metadata.png` & `gordo-5.1.4/docs/_static/endpoint-metadata.png`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/builder.rst` & `gordo-5.1.4/docs/api/builder.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/cli.rst` & `gordo-5.1.4/docs/api/cli.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/machine/metadata.rst` & `gordo-5.1.4/docs/api/machine/metadata.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/machine/model/anomaly.rst` & `gordo-5.1.4/docs/api/machine/model/anomaly.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/machine/model/model-factories.rst` & `gordo-5.1.4/docs/api/machine/model/model-factories.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/serializer.rst` & `gordo-5.1.4/docs/api/serializer.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/util.rst` & `gordo-5.1.4/docs/api/util.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/api/workflow.rst` & `gordo-5.1.4/docs/api/workflow.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/conf.py` & `gordo-5.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/general/cluster_deployment.rst` & `gordo-5.1.4/docs/general/cluster_deployment.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/general/endpoints.rst` & `gordo-5.1.4/docs/general/endpoints.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/ml/model_configuration.rst` & `gordo-5.1.4/docs/ml/model_configuration.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/ml/model_output.rst` & `gordo-5.1.4/docs/ml/model_output.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/docs/overview.rst` & `gordo-5.1.4/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/examples/Gordo-Workflow-High-Level.ipynb` & `gordo-5.1.4/examples/Gordo-Workflow-High-Level.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/examples/Pipelines-with-Gordo.ipynb` & `gordo-5.1.4/examples/Pipelines-with-Gordo.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/examples/config.yaml` & `gordo-5.1.4/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/examples/model-configuration.yaml` & `gordo-5.1.4/examples/model-configuration.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/examples/test-project.yaml` & `gordo-5.1.4/examples/test-project.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/functions.sh` & `gordo-5.1.4/functions.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/__init__.py` & `gordo-5.1.4/gordo/__init__.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/builder/build_model.py` & `gordo-5.1.4/gordo/builder/build_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/builder/local_build.py` & `gordo-5.1.4/gordo/builder/local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/builder/utils.py` & `gordo-5.1.4/gordo/builder/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/cli/cli.py` & `gordo-5.1.4/gordo/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/cli/custom_types.py` & `gordo-5.1.4/gordo/cli/custom_types.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/cli/exceptions_reporter.py` & `gordo-5.1.4/gordo/cli/exceptions_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/cli/workflow_generator.py` & `gordo-5.1.4/gordo/cli/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/encoders.py` & `gordo-5.1.4/gordo/machine/encoders.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/loader.py` & `gordo-5.1.4/gordo/machine/loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/machine.py` & `gordo-5.1.4/gordo/machine/machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/metadata/metadata.py` & `gordo-5.1.4/gordo/machine/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/anomaly/base.py` & `gordo-5.1.4/gordo/machine/model/anomaly/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/anomaly/diff.py` & `gordo-5.1.4/gordo/machine/model/anomaly/diff.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/base.py` & `gordo-5.1.4/gordo/machine/model/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/factories/feedforward_autoencoder.py` & `gordo-5.1.4/gordo/machine/model/factories/feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/factories/lstm_autoencoder.py` & `gordo-5.1.4/gordo/machine/model/factories/lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/factories/utils.py` & `gordo-5.1.4/gordo/machine/model/factories/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/models.py` & `gordo-5.1.4/gordo/machine/model/models.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/register.py` & `gordo-5.1.4/gordo/machine/model/register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/transformer_funcs/general.py` & `gordo-5.1.4/gordo/machine/model/transformer_funcs/general.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/transformers/imputer.py` & `gordo-5.1.4/gordo/machine/model/transformers/imputer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/model/utils.py` & `gordo-5.1.4/gordo/machine/model/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/machine/validators.py` & `gordo-5.1.4/gordo/machine/validators.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/reporters/base.py` & `gordo-5.1.4/gordo/reporters/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/reporters/mlflow.py` & `gordo-5.1.4/gordo/reporters/mlflow.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/reporters/postgres.py` & `gordo-5.1.4/gordo/reporters/postgres.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/serializer/from_definition.py` & `gordo-5.1.4/gordo/serializer/from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/serializer/into_definition.py` & `gordo-5.1.4/gordo/serializer/into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/serializer/serializer.py` & `gordo-5.1.4/gordo/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/serializer/utils.py` & `gordo-5.1.4/gordo/serializer/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/blueprints/anomaly.py` & `gordo-5.1.4/gordo/server/blueprints/anomaly.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/blueprints/base.py` & `gordo-5.1.4/gordo/server/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/model_io.py` & `gordo-5.1.4/gordo/server/model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/prometheus/metrics.py` & `gordo-5.1.4/gordo/server/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/prometheus/server.py` & `gordo-5.1.4/gordo/server/prometheus/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/properties.py` & `gordo-5.1.4/gordo/server/properties.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/server.py` & `gordo-5.1.4/gordo/server/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/server/utils.py` & `gordo-5.1.4/gordo/server/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/util/disk_registry.py` & `gordo-5.1.4/gordo/util/disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/util/utils.py` & `gordo-5.1.4/gordo/util/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/util/version.py` & `gordo-5.1.4/gordo/util/version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/utils.py` & `gordo-5.1.4/gordo/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/workflow/config_elements/normalized_config.py` & `gordo-5.1.4/gordo/workflow/config_elements/normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/workflow/config_elements/schemas.py` & `gordo-5.1.4/gordo/workflow/config_elements/schemas.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/workflow/workflow_generator/helpers.py` & `gordo-5.1.4/gordo/workflow/workflow_generator/helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template` & `gordo-5.1.4/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo/workflow/workflow_generator/workflow_generator.py` & `gordo-5.1.4/gordo/workflow/workflow_generator/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo.egg-info/PKG-INFO` & `gordo-5.1.4/gordo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.1.3
+Version: 5.1.4
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.1.3 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.1.4 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
 Extra: mlflow Provides-Extra: postgres Provides-Extra: tests Provides-Extra:
```

### Comparing `gordo-5.1.3/gordo.egg-info/SOURCES.txt` & `gordo-5.1.4/gordo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/gordo.egg-info/requires.txt` & `gordo-5.1.4/gordo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/pytest.ini` & `gordo-5.1.4/pytest.ini`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/requirements/full_requirements.txt` & `gordo-5.1.4/requirements/full_requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=full_requirements.txt --resolver=backtracking mlflow_requirements.in postgres_requirements.in requirements.in
+#    pip-compile --output-file=full_requirements.txt mlflow_requirements.in postgres_requirements.in requirements.in
 #
 absl-py==1.4.0
     # via
     #   tensorboard
     #   tensorflow
 adal==1.2.7
     # via
@@ -25,15 +25,15 @@
     #   azure-graphrbac
     #   azure-mgmt-authorization
     #   azure-mgmt-containerregistry
     #   azure-mgmt-keyvault
     #   azure-mgmt-resource
     #   azure-mgmt-storage
     #   azureml-core
-azure-core==1.27.1
+azure-core==1.28.0
     # via
     #   azure-mgmt-core
     #   azureml-core
     #   msrest
 azure-graphrbac==0.61.1
     # via azureml-core
 azure-mgmt-authorization==3.0.0
@@ -73,42 +73,42 @@
     # via
     #   msrest
     #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.5
     # via
     #   databricks-cli
     #   flask
     #   gordo-client
     #   mlflow
 cloudpickle==2.2.1
     # via mlflow
 contextlib2==21.6.0
     # via azureml-core
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.1
+cryptography==41.0.2
     # via
     #   adal
     #   azureml-core
     #   msal
     #   paramiko
     #   pyjwt
     #   pyopenssl
     #   secretstorage
 cycler==0.11.0
     # via matplotlib
 databricks-cli==0.17.7
     # via mlflow
-dataclasses-json==0.5.8
+dataclasses-json==0.5.12
     # via -r requirements.in
 dictdiffer==0.9.0
     # via -r requirements.in
 docker==6.1.3
     # via
     #   azureml-core
     #   mlflow
@@ -116,31 +116,31 @@
     # via mlflow
 flask==2.3.2
     # via
     #   -r requirements.in
     #   mlflow
 flatbuffers==23.5.26
     # via tensorflow
-fonttools==4.40.0
+fonttools==4.41.0
     # via matplotlib
 gast==0.4.0
     # via tensorflow
 gitdb==4.0.10
     # via gitpython
-gitpython==3.1.31
+gitpython==3.1.32
     # via mlflow
-google-auth==2.21.0
+google-auth==2.22.0
     # via
     #   google-auth-oauthlib
     #   tensorboard
 google-auth-oauthlib==1.0.0
     # via tensorboard
 google-pasta==0.2.0
     # via tensorflow
-gordo-client==6.2.2
+gordo-client==6.2.3
     # via -r requirements.in
 gordo-core==0.3.2
     # via gordo-client
 graphviz==0.20.1
     # via catboost
 greenlet==2.0.2
     # via sqlalchemy
@@ -156,15 +156,15 @@
     # via
     #   -r requirements.in
     #   tensorflow
 humanfriendly==10.0
     # via azureml-core
 idna==3.4
     # via requests
-importlib-metadata==6.7.0
+importlib-metadata==6.8.0
     # via mlflow
 influxdb==5.3.1
     # via gordo-core
 isodate==0.6.1
     # via
     #   azure-mgmt-keyvault
     #   msrest
@@ -179,50 +179,46 @@
     #   -r requirements.in
     #   flask
     #   mlflow
 jmespath==1.0.1
     # via
     #   azureml-core
     #   knack
-joblib==1.2.0
+joblib==1.3.1
     # via scikit-learn
 jsonpickle==3.0.1
     # via azureml-core
 keras==2.12.0
     # via tensorflow
 kiwisolver==1.4.4
     # via matplotlib
 knack==0.10.1
     # via azureml-core
-libclang==16.0.0
+libclang==16.0.6
     # via tensorflow
 mako==1.2.4
     # via alembic
 markdown==3.4.3
     # via
     #   mlflow
     #   tensorboard
 markupsafe==2.1.3
     # via
     #   jinja2
     #   mako
     #   werkzeug
 marshmallow==3.19.0
-    # via
-    #   dataclasses-json
-    #   marshmallow-enum
-marshmallow-enum==1.5.1
     # via dataclasses-json
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via
     #   catboost
     #   mlflow
 ml-dtypes==0.2.0
     # via jax
-mlflow==2.4.1
+mlflow==2.5.0
     # via -r mlflow_requirements.in
 msal==1.22.0
     # via
     #   azureml-core
     #   msal-extensions
 msal-extensions==1.0.0
     # via azureml-core
@@ -243,15 +239,15 @@
     #   azureml-core
 mypy-extensions==1.0.0
     # via typing-inspect
 ndg-httpsclient==0.5.1
     # via azureml-core
 numexpr==2.8.4
     # via gordo-core
-numpy==1.23.5
+numpy==1.24.3
     # via
     #   catboost
     #   contourpy
     #   gordo-core
     #   h5py
     #   jax
     #   matplotlib
@@ -293,25 +289,25 @@
     #   xarray
 paramiko==3.2.0
     # via azureml-core
 pathspec==0.11.1
     # via azureml-core
 peewee==3.16.2
     # via -r postgres_requirements.in
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pkginfo==1.9.6
     # via azureml-core
 plotly==5.15.0
     # via catboost
 portalocker==2.7.0
     # via msal-extensions
-prometheus-client==0.17.0
+prometheus-client==0.17.1
     # via -r requirements.in
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   mlflow
     #   tensorboard
     #   tensorflow
 psycopg2-binary==2.9.6
     # via -r postgres_requirements.in
 pyarrow==10.0.1
@@ -323,15 +319,15 @@
     #   ndg-httpsclient
     #   pyasn1-modules
     #   rsa
 pyasn1-modules==0.3.0
     # via google-auth
 pycparser==2.21
     # via cffi
-pydantic==1.10.9
+pydantic==1.10.11
     # via gordo-client
 pygments==2.15.1
     # via knack
 pyjwt[crypto]==2.7.0
     # via
     #   adal
     #   azureml-core
@@ -339,15 +335,15 @@
     #   msal
 pynacl==1.5.0
     # via paramiko
 pyopenssl==23.2.0
     # via
     #   azureml-core
     #   ndg-httpsclient
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via
     #   matplotlib
     #   packaging
 pysocks==1.7.1
     # via requests
 python-dateutil==2.8.2
     # via
@@ -359,15 +355,15 @@
     #   pandas
 pytz==2023.3
     # via
     #   azureml-core
     #   influxdb
     #   mlflow
     #   pandas
-pyyaml==5.4.1
+pyyaml==6.0.1
     # via
     #   gordo-client
     #   knack
     #   mlflow
 querystring-parser==1.2.4
     # via mlflow
 requests[socks]==2.31.0
@@ -386,19 +382,19 @@
     #   tensorboard
 requests-oauthlib==1.3.1
     # via
     #   google-auth-oauthlib
     #   msrest
 rsa==4.9
     # via google-auth
-scikit-learn==1.2.2
+scikit-learn==1.3.0
     # via
     #   gordo-core
     #   mlflow
-scipy==1.11.0
+scipy==1.11.1
     # via
     #   catboost
     #   jax
     #   mlflow
     #   scikit-learn
 secretstorage==3.3.3
     # via azureml-core
@@ -418,15 +414,15 @@
     #   isodate
     #   msrestazure
     #   python-dateutil
     #   querystring-parser
     #   tensorflow
 smmap==5.0.0
     # via gitdb
-sqlalchemy==2.0.17
+sqlalchemy==2.0.19
     # via
     #   alembic
     #   mlflow
 sqlparse==0.4.4
     # via mlflow
 tabulate==0.9.0
     # via
@@ -434,25 +430,25 @@
     #   knack
 tenacity==8.2.2
     # via plotly
 tensorboard==2.12.3
     # via tensorflow
 tensorboard-data-server==0.7.1
     # via tensorboard
-tensorflow==2.12.0
+tensorflow==2.12.1
     # via -r requirements.in
 tensorflow-estimator==2.12.0
     # via tensorflow
 tensorflow-io-gcs-filesystem==0.32.0
     # via tensorflow
 termcolor==2.3.0
     # via tensorflow
-threadpoolctl==3.1.0
+threadpoolctl==3.2.0
     # via scikit-learn
-typing-extensions==4.6.3
+typing-extensions==4.5.0
     # via
     #   alembic
     #   azure-core
     #   pydantic
     #   sqlalchemy
     #   tensorflow
     #   typing-inspect
@@ -475,14 +471,14 @@
     # via
     #   astunparse
     #   tensorboard
 wrapt==1.14.1
     # via
     #   gordo-client
     #   tensorflow
-xarray==2023.6.0
+xarray==2023.7.0
     # via gordo-core
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `gordo-5.1.3/requirements/test_requirements.txt` & `gordo-5.1.4/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json` & `gordo-5.1.4/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/resources/grafana/dashboards/machines.json` & `gordo-5.1.4/resources/grafana/dashboards/machines.json`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/run_workflow_and_argo.sh` & `gordo-5.1.4/run_workflow_and_argo.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/scripts/download_argo.py` & `gordo-5.1.4/scripts/download_argo.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/scripts/github_docker.py` & `gordo-5.1.4/scripts/github_docker.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/scripts/tests.sh` & `gordo-5.1.4/scripts/tests.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/scripts/trivy_scan.sh` & `gordo-5.1.4/scripts/trivy_scan.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/setup.py` & `gordo-5.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/config-test.yaml` & `gordo-5.1.4/tests/config-test.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/conftest.py` & `gordo-5.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/builder/test_builder.py` & `gordo-5.1.4/tests/gordo/builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/builder/test_local_build.py` & `gordo-5.1.4/tests/gordo/builder/test_local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/builder/test_utils.py` & `gordo-5.1.4/tests/gordo/builder/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/cli/test_cli.py` & `gordo-5.1.4/tests/gordo/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/cli/test_exception_reporter.py` & `gordo-5.1.4/tests/gordo/cli/test_exception_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/client/test_client.py` & `gordo-5.1.4/tests/gordo/client/test_client.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/metadata/test_metadata.py` & `gordo-5.1.4/tests/gordo/machine/metadata/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py` & `gordo-5.1.4/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_factories_utils.py` & `gordo-5.1.4/tests/gordo/machine/model/test_factories_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_feedforward_autoencoder.py` & `gordo-5.1.4/tests/gordo/machine/model/test_feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_lstm_autoencoder.py` & `gordo-5.1.4/tests/gordo/machine/model/test_lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_model.py` & `gordo-5.1.4/tests/gordo/machine/model/test_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_raw_keras.py` & `gordo-5.1.4/tests/gordo/machine/model/test_raw_keras.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_register.py` & `gordo-5.1.4/tests/gordo/machine/model/test_register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_transformers.py` & `gordo-5.1.4/tests/gordo/machine/model/test_transformers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/model/test_utils.py` & `gordo-5.1.4/tests/gordo/machine/model/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/test_descriptors.py` & `gordo-5.1.4/tests/gordo/machine/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/test_loader.py` & `gordo-5.1.4/tests/gordo/machine/test_loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/machine/test_machine.py` & `gordo-5.1.4/tests/gordo/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/reporters/test_mlflow_reporter.py` & `gordo-5.1.4/tests/gordo/reporters/test_mlflow_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/reporters/test_postgres_reporter.py` & `gordo-5.1.4/tests/gordo/reporters/test_postgres_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/serializer/test_serializer_from_definition.py` & `gordo-5.1.4/tests/gordo/serializer/test_serializer_from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/serializer/test_serializer_into_definition.py` & `gordo-5.1.4/tests/gordo/serializer/test_serializer_into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/serializer/test_serializer_load_dump.py` & `gordo-5.1.4/tests/gordo/serializer/test_serializer_load_dump.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/server/test_anomaly_blueprint.py` & `gordo-5.1.4/tests/gordo/server/test_anomaly_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/server/test_base_blueprint.py` & `gordo-5.1.4/tests/gordo/server/test_base_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/server/test_gordo_server.py` & `gordo-5.1.4/tests/gordo/server/test_gordo_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/server/test_model_io.py` & `gordo-5.1.4/tests/gordo/server/test_model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/server/test_prometheus.py` & `gordo-5.1.4/tests/gordo/server/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/server/test_utils.py` & `gordo-5.1.4/tests/gordo/server/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/test_version.py` & `gordo-5.1.4/tests/gordo/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/util/test_disk_registry.py` & `gordo-5.1.4/tests/gordo/util/test_disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/util/test_version.py` & `gordo-5.1.4/tests/gordo/util/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_config_elements.py` & `gordo-5.1.4/tests/gordo/workflow/test_config_elements.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_helpers.py` & `gordo-5.1.4/tests/gordo/workflow/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_normalized_config.py` & `gordo-5.1.4/tests/gordo/workflow/test_normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py` & `gordo-5.1.4/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/test_examples.py` & `gordo-5.1.4/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gordo-5.1.3/tests/utils.py` & `gordo-5.1.4/tests/utils.py`

 * *Files identical despite different names*

