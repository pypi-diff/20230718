# Comparing `tmp/mite-1.1.7.tar.gz` & `tmp/mite-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mite-1.1.7.tar", last modified: Fri Apr 21 11:15:36 2023, max compression
+gzip compressed data, was "mite-1.1.8.tar", last modified: Tue Jul 18 14:32:46 2023, max compression
```

## Comparing `mite-1.1.7.tar` & `mite-1.1.8.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/.circleci/
--rw-r--r--   0 root         (0) root         (0)     5548 2023-04-21 11:15:24.000000 mite-1.1.7/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      233 2023-04-21 11:15:24.000000 mite-1.1.7/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-21 11:15:24.000000 mite-1.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      604 2023-04-21 11:15:24.000000 mite-1.1.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 root         (0) root         (0)      115 2023-04-21 11:15:24.000000 mite-1.1.7/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1212 2023-04-21 11:15:24.000000 mite-1.1.7/.gitignore
--rw-r--r--   0 root         (0) root         (0)      138 2023-04-21 11:15:24.000000 mite-1.1.7/.isort.cfg
--rw-r--r--   0 root         (0) root         (0)      332 2023-04-21 11:15:24.000000 mite-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      696 2023-04-21 11:15:24.000000 mite-1.1.7/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     3230 2023-04-21 11:15:24.000000 mite-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     3929 2023-04-21 11:15:24.000000 mite-1.1.7/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     3082 2023-04-21 11:15:24.000000 mite-1.1.7/DEV.md
--rw-r--r--   0 root         (0) root         (0)     1444 2023-04-21 11:15:24.000000 mite-1.1.7/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      307 2023-04-21 11:15:24.000000 mite-1.1.7/Dockerfile.perftest
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-21 11:15:24.000000 mite-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-21 11:15:24.000000 mite-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9319 2023-04-21 11:15:36.870287 mite-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8676 2023-04-21 11:15:24.000000 mite-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/cd-scripts/
--rwxr-xr-x   0 root         (0) root         (0)      526 2023-04-21 11:15:24.000000 mite-1.1.7/cd-scripts/cdBuild-1.sh
--rw-r--r--   0 root         (0) root         (0)     4138 2023-04-21 11:15:24.000000 mite-1.1.7/cd-scripts/cdRelease.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-21 11:15:24.000000 mite-1.1.7/cd.yml
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 11:15:24.000000 mite-1.1.7/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1624 2023-04-21 11:15:24.000000 mite-1.1.7/docker_compose.yml
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-21 11:15:24.000000 mite-1.1.7/docker_compose_monitoring.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-21 11:15:24.000000 mite-1.1.7/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     6220 2023-04-21 11:15:24.000000 mite-1.1.7/docs/components.rst
--rw-r--r--   0 root         (0) root         (0)     2165 2023-04-21 11:15:24.000000 mite-1.1.7/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-04-21 11:15:24.000000 mite-1.1.7/docs/config.rst
--rw-r--r--   0 root         (0) root         (0)     7835 2023-04-21 11:15:24.000000 mite-1.1.7/docs/design-deployment.rst
--rw-r--r--   0 root         (0) root         (0)      945 2023-04-21 11:15:24.000000 mite-1.1.7/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     3908 2023-04-21 11:15:24.000000 mite-1.1.7/docs/journeys.rst
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-21 11:15:24.000000 mite-1.1.7/docs/notes.txt
--rw-r--r--   0 root         (0) root         (0)     2324 2023-04-21 11:15:24.000000 mite-1.1.7/docs/prometheus.rst
--rw-r--r--   0 root         (0) root         (0)     6507 2023-04-21 11:15:24.000000 mite-1.1.7/docs/stats.rst
--rw-r--r--   0 root         (0) root         (0)     1717 2023-04-21 11:15:24.000000 mite-1.1.7/docs/volume-model.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/grafana/
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/Dockerfile
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.842288 mite-1.1.7/grafana/provisioning/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/grafana/provisioning/dashboards/
--rw-r--r--   0 root         (0) root         (0)      145 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/dashboards/dashboards.yml
--rw-r--r--   0 root         (0) root         (0)    27978 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/dashboards/grafana_dashboard_template.json
--rw-r--r--   0 root         (0) root         (0)    28427 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/dashboards/mite_docker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/grafana/provisioning/datasources/
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/datasources/datasources.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/local/
--rw-r--r--   0 root         (0) root         (0)      628 2023-04-21 11:15:24.000000 mite-1.1.7/local/Makefile
--rw-r--r--   0 root         (0) root         (0)     1349 2023-04-21 11:15:24.000000 mite-1.1.7/local/README.md
--rw-r--r--   0 root         (0) root         (0)      678 2023-04-21 11:15:24.000000 mite-1.1.7/local/demo.py
--rwxr-xr-x   0 root         (0) root         (0)     1024 2023-04-21 11:15:24.000000 mite-1.1.7/local/run_mite.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite/
--rwxr-xr-x   0 root         (0) root         (0)     2353 2023-04-21 11:15:24.000000 mite-1.1.7/mite/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    15198 2023-04-21 11:15:24.000000 mite-1.1.7/mite/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/cat.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/collector.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/common.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/duplicator.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/receiver.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/stats.py
--rw-r--r--   0 root         (0) root         (0)     6560 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/test.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-21 11:15:24.000000 mite-1.1.7/mite/collector.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-04-21 11:15:24.000000 mite-1.1.7/mite/config.py
--rwxr-xr-x   0 root         (0) root         (0)     4815 2023-04-21 11:15:24.000000 mite-1.1.7/mite/context.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-04-21 11:15:24.000000 mite-1.1.7/mite/controller.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-04-21 11:15:24.000000 mite-1.1.7/mite/datapools.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-04-21 11:15:24.000000 mite-1.1.7/mite/example.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-04-21 11:15:24.000000 mite-1.1.7/mite/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-04-21 11:15:24.000000 mite-1.1.7/mite/har_to_mite.py
--rw-r--r--   0 root         (0) root         (0)     4804 2023-04-21 11:15:24.000000 mite-1.1.7/mite/logoutput.py
--rwxr-xr-x   0 root         (0) root         (0)     4591 2023-04-21 11:15:24.000000 mite-1.1.7/mite/nanomsg.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-21 11:15:24.000000 mite-1.1.7/mite/recorder.py
--rwxr-xr-x   0 root         (0) root         (0)     6986 2023-04-21 11:15:24.000000 mite-1.1.7/mite/runner.py
--rw-r--r--   0 root         (0) root         (0)     6226 2023-04-21 11:15:24.000000 mite-1.1.7/mite/scenario.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-21 11:15:24.000000 mite-1.1.7/mite/stats.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-04-21 11:15:24.000000 mite-1.1.7/mite/test.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-21 11:15:24.000000 mite-1.1.7/mite/utils.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-04-21 11:15:24.000000 mite-1.1.7/mite/volume_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite/web/
--rw-r--r--   0 root         (0) root         (0)      469 2023-04-21 11:15:24.000000 mite-1.1.7/mite/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3559 2023-04-21 11:15:24.000000 mite-1.1.7/mite/web/prometheus.py
--rwxr-xr-x   0 root         (0) root         (0)     6247 2023-04-21 11:15:24.000000 mite-1.1.7/mite/zmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9319 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3460 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_amqp/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-04-21 11:15:24.000000 mite-1.1.7/mite_amqp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_browser/
--rwxr-xr-x   0 root         (0) root         (0)    17442 2023-04-21 11:15:24.000000 mite-1.1.7/mite_browser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_finagle/
--rw-r--r--   0 root         (0) root         (0)     8329 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/README.md
--rw-r--r--   0 root         (0) root         (0)     6504 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11258 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/mux.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_finagle/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_finagle/tests/foo_service/
--rwxr-xr-x   0 root         (0) root         (0)     2698 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/Foo-remote
--rw-r--r--   0 root         (0) root         (0)     7560 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/Foo.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/__init__.py
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/constants.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/ttypes.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service.thrift
--rw-r--r--   0 root         (0) root         (0)     3503 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     4738 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/test_mux.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/test_thrift.py
--rw-r--r--   0 root         (0) root         (0)     9650 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/thrift.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_http/
--rw-r--r--   0 root         (0) root         (0)     2964 2023-04-21 11:15:24.000000 mite-1.1.7/mite_http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-21 11:15:24.000000 mite-1.1.7/mite_http/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_selenium/
--rw-r--r--   0 root         (0) root         (0)    11427 2023-04-21 11:15:24.000000 mite-1.1.7/mite_selenium/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-04-21 11:15:24.000000 mite-1.1.7/mite_selenium/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_websocket/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-04-21 11:15:24.000000 mite-1.1.7/mite_websocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/prometheus/
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-21 11:15:24.000000 mite-1.1.7/prometheus/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      206 2023-04-21 11:15:24.000000 mite-1.1.7/prometheus/prometheus_config_docker.yml
--rw-r--r--   0 root         (0) root         (0)      136 2023-04-21 11:15:24.000000 mite-1.1.7/prometheus/prometheus_config_template.yml
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-21 11:15:24.000000 mite-1.1.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-21 11:15:24.000000 mite-1.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-04-21 11:15:36.870287 mite-1.1.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      114 2023-04-21 11:15:24.000000 mite-1.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/test/
--rw-r--r--   0 root         (0) root         (0)      124 2023-04-21 11:15:24.000000 mite-1.1.7/test/legacy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/test/mocks/
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_collector.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_context.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_direct_receiver.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_direct_runner_transport.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_recorder_msg_http.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_selenium.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/test/perf/
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1677 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/http_server.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/http_server_aiohttp.py
--rw-r--r--   0 root         (0) root         (0)      817 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/mite_perftest.py
--rwxr-xr-x   0 root         (0) root         (0)     4625 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/perftest.py
--rwxr-xr-x   0 root         (0) root         (0)     1330 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/run-perftest.sh
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0) 10236043 2023-04-21 11:15:24.000000 mite-1.1.7/test/test.har
--rw-r--r--   0 root         (0) root         (0)     5240 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_collector.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_context.py
--rw-r--r--   0 root         (0) root         (0)     3700 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_controller.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_datapools.py
--rw-r--r--   0 root         (0) root         (0)     7712 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_har_to_mite.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_amqp.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_browser.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_http.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_utils.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_websockets.py
--rw-r--r--   0 root         (0) root         (0)     4015 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_prometheus_mite.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_recorder.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_runner_tracker.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_scenario.py
--rw-r--r--   0 root         (0) root         (0)     5867 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_stats.py
--rw-r--r--   0 root         (0) root         (0)     3375 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_volume_model.py
--rw-r--r--   0 root         (0) root         (0)     8670 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_webdriver.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_work_tracker.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-21 11:15:24.000000 mite-1.1.7/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0) 10236043 2023-04-21 11:15:24.000000 mite-1.1.7/test.har
--rw-r--r--   0 root         (0) root         (0)     1860 2023-04-21 11:15:24.000000 mite-1.1.7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.185753 mite-1.1.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.165753 mite-1.1.8/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-07-18 14:32:33.000000 mite-1.1.8/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-18 14:32:33.000000 mite-1.1.8/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.165753 mite-1.1.8/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.165753 mite-1.1.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-18 14:32:33.000000 mite-1.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-18 14:32:33.000000 mite-1.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 root         (0) root         (0)      115 2023-07-18 14:32:33.000000 mite-1.1.8/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-07-18 14:32:33.000000 mite-1.1.8/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-18 14:32:33.000000 mite-1.1.8/.isort.cfg
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-18 14:32:33.000000 mite-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      696 2023-07-18 14:32:33.000000 mite-1.1.8/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)     3230 2023-07-18 14:32:33.000000 mite-1.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     3929 2023-07-18 14:32:33.000000 mite-1.1.8/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-07-18 14:32:33.000000 mite-1.1.8/DEV.md
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-07-18 14:32:33.000000 mite-1.1.8/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      307 2023-07-18 14:32:33.000000 mite-1.1.8/Dockerfile.perftest
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-07-18 14:32:33.000000 mite-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 14:32:33.000000 mite-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9413 2023-07-18 14:32:46.185753 mite-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8770 2023-07-18 14:32:33.000000 mite-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.165753 mite-1.1.8/cd-scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      526 2023-07-18 14:32:33.000000 mite-1.1.8/cd-scripts/cdBuild-1.sh
+-rw-r--r--   0 root         (0) root         (0)     4138 2023-07-18 14:32:33.000000 mite-1.1.8/cd-scripts/cdRelease.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-07-18 14:32:33.000000 mite-1.1.8/cd.yml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-18 14:32:33.000000 mite-1.1.8/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-07-18 14:32:33.000000 mite-1.1.8/docker_compose.yml
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-18 14:32:33.000000 mite-1.1.8/docker_compose_monitoring.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.165753 mite-1.1.8/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-18 14:32:33.000000 mite-1.1.8/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6220 2023-07-18 14:32:33.000000 mite-1.1.8/docs/components.rst
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-07-18 14:32:33.000000 mite-1.1.8/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-18 14:32:33.000000 mite-1.1.8/docs/config.rst
+-rw-r--r--   0 root         (0) root         (0)     7835 2023-07-18 14:32:33.000000 mite-1.1.8/docs/design-deployment.rst
+-rw-r--r--   0 root         (0) root         (0)      945 2023-07-18 14:32:33.000000 mite-1.1.8/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-07-18 14:32:33.000000 mite-1.1.8/docs/journeys.rst
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-18 14:32:33.000000 mite-1.1.8/docs/notes.txt
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-07-18 14:32:33.000000 mite-1.1.8/docs/prometheus.rst
+-rw-r--r--   0 root         (0) root         (0)     6507 2023-07-18 14:32:33.000000 mite-1.1.8/docs/stats.rst
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-07-18 14:32:33.000000 mite-1.1.8/docs/volume-model.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.165753 mite-1.1.8/grafana/
+-rw-r--r--   0 root         (0) root         (0)      129 2023-07-18 14:32:33.000000 mite-1.1.8/grafana/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-18 14:32:33.000000 mite-1.1.8/grafana/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.153754 mite-1.1.8/grafana/provisioning/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.169753 mite-1.1.8/grafana/provisioning/dashboards/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-18 14:32:33.000000 mite-1.1.8/grafana/provisioning/dashboards/dashboards.yml
+-rw-r--r--   0 root         (0) root         (0)    27978 2023-07-18 14:32:33.000000 mite-1.1.8/grafana/provisioning/dashboards/grafana_dashboard_template.json
+-rw-r--r--   0 root         (0) root         (0)    28427 2023-07-18 14:32:33.000000 mite-1.1.8/grafana/provisioning/dashboards/mite_docker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.169753 mite-1.1.8/grafana/provisioning/datasources/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-18 14:32:33.000000 mite-1.1.8/grafana/provisioning/datasources/datasources.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.169753 mite-1.1.8/local/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-18 14:32:33.000000 mite-1.1.8/local/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-07-18 14:32:33.000000 mite-1.1.8/local/README.md
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-18 14:32:33.000000 mite-1.1.8/local/demo.py
+-rwxr-xr-x   0 root         (0) root         (0)     1024 2023-07-18 14:32:33.000000 mite-1.1.8/local/run_mite.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.169753 mite-1.1.8/mite/
+-rwxr-xr-x   0 root         (0) root         (0)     2353 2023-07-18 14:32:33.000000 mite-1.1.8/mite/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15198 2023-07-18 14:32:33.000000 mite-1.1.8/mite/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/cat.py
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/collector.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/duplicator.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/receiver.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/stats.py
+-rw-r--r--   0 root         (0) root         (0)     6560 2023-07-18 14:32:33.000000 mite-1.1.8/mite/cli/test.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-07-18 14:32:33.000000 mite-1.1.8/mite/collector.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-07-18 14:32:33.000000 mite-1.1.8/mite/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     4815 2023-07-18 14:32:33.000000 mite-1.1.8/mite/context.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-07-18 14:32:33.000000 mite-1.1.8/mite/controller.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-18 14:32:33.000000 mite-1.1.8/mite/datapools.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-18 14:32:33.000000 mite-1.1.8/mite/example.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-18 14:32:33.000000 mite-1.1.8/mite/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-07-18 14:32:33.000000 mite-1.1.8/mite/har_to_mite.py
+-rw-r--r--   0 root         (0) root         (0)     4804 2023-07-18 14:32:33.000000 mite-1.1.8/mite/logoutput.py
+-rwxr-xr-x   0 root         (0) root         (0)     4591 2023-07-18 14:32:33.000000 mite-1.1.8/mite/nanomsg.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-07-18 14:32:33.000000 mite-1.1.8/mite/recorder.py
+-rwxr-xr-x   0 root         (0) root         (0)     6986 2023-07-18 14:32:33.000000 mite-1.1.8/mite/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-07-18 14:32:33.000000 mite-1.1.8/mite/scenario.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-18 14:32:33.000000 mite-1.1.8/mite/stats.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-07-18 14:32:33.000000 mite-1.1.8/mite/test.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-18 14:32:33.000000 mite-1.1.8/mite/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-07-18 14:32:33.000000 mite-1.1.8/mite/volume_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite/web/
+-rw-r--r--   0 root         (0) root         (0)      469 2023-07-18 14:32:33.000000 mite-1.1.8/mite/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3559 2023-07-18 14:32:33.000000 mite-1.1.8/mite/web/prometheus.py
+-rwxr-xr-x   0 root         (0) root         (0)     6247 2023-07-18 14:32:33.000000 mite-1.1.8/mite/zmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.169753 mite-1.1.8/mite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9413 2023-07-18 14:32:46.000000 mite-1.1.8/mite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-07-18 14:32:46.000000 mite-1.1.8/mite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 14:32:46.000000 mite-1.1.8/mite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-18 14:32:46.000000 mite-1.1.8/mite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-18 14:32:46.000000 mite-1.1.8/mite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-18 14:32:46.000000 mite-1.1.8/mite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_amqp/
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-07-18 14:32:33.000000 mite-1.1.8/mite_amqp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_browser/
+-rwxr-xr-x   0 root         (0) root         (0)    17442 2023-07-18 14:32:33.000000 mite-1.1.8/mite_browser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_finagle/
+-rw-r--r--   0 root         (0) root         (0)     8329 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/README.md
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11258 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/mux.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_finagle/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_finagle/tests/foo_service/
+-rwxr-xr-x   0 root         (0) root         (0)     2698 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/foo_service/Foo-remote
+-rw-r--r--   0 root         (0) root         (0)     7560 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/foo_service/Foo.py
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/foo_service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      366 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/foo_service/constants.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/foo_service/ttypes.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/foo_service.thrift
+-rw-r--r--   0 root         (0) root         (0)     3503 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/test_mux.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/tests/test_thrift.py
+-rw-r--r--   0 root         (0) root         (0)     9650 2023-07-18 14:32:33.000000 mite-1.1.8/mite_finagle/thrift.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_http/
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-07-18 14:32:33.000000 mite-1.1.8/mite_http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-07-18 14:32:33.000000 mite-1.1.8/mite_http/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_selenium/
+-rw-r--r--   0 root         (0) root         (0)    11427 2023-07-18 14:32:33.000000 mite-1.1.8/mite_selenium/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-07-18 14:32:33.000000 mite-1.1.8/mite_selenium/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/mite_websocket/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-07-18 14:32:33.000000 mite-1.1.8/mite_websocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.173753 mite-1.1.8/prometheus/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-18 14:32:33.000000 mite-1.1.8/prometheus/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      206 2023-07-18 14:32:33.000000 mite-1.1.8/prometheus/prometheus_config_docker.yml
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-18 14:32:33.000000 mite-1.1.8/prometheus/prometheus_config_template.yml
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-18 14:32:33.000000 mite-1.1.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-18 14:32:33.000000 mite-1.1.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-18 14:32:46.185753 mite-1.1.8/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      114 2023-07-18 14:32:33.000000 mite-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.181753 mite-1.1.8/test/
+-rw-r--r--   0 root         (0) root         (0)      124 2023-07-18 14:32:33.000000 mite-1.1.8/test/legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.185753 mite-1.1.8/test/mocks/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-18 14:32:33.000000 mite-1.1.8/test/mocks/mock_collector.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-18 14:32:33.000000 mite-1.1.8/test/mocks/mock_context.py
+-rw-r--r--   0 root         (0) root         (0)      584 2023-07-18 14:32:33.000000 mite-1.1.8/test/mocks/mock_direct_receiver.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-07-18 14:32:33.000000 mite-1.1.8/test/mocks/mock_direct_runner_transport.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-18 14:32:33.000000 mite-1.1.8/test/mocks/mock_recorder_msg_http.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-07-18 14:32:33.000000 mite-1.1.8/test/mocks/mock_selenium.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-07-18 14:32:33.000000 mite-1.1.8/test/mocks/mock_sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:46.185753 mite-1.1.8/test/perf/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-18 14:32:33.000000 mite-1.1.8/test/perf/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-07-18 14:32:33.000000 mite-1.1.8/test/perf/http_server.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-07-18 14:32:33.000000 mite-1.1.8/test/perf/http_server_aiohttp.py
+-rw-r--r--   0 root         (0) root         (0)      817 2023-07-18 14:32:33.000000 mite-1.1.8/test/perf/mite_perftest.py
+-rwxr-xr-x   0 root         (0) root         (0)     4625 2023-07-18 14:32:33.000000 mite-1.1.8/test/perf/perftest.py
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2023-07-18 14:32:33.000000 mite-1.1.8/test/perf/run-perftest.sh
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-18 14:32:33.000000 mite-1.1.8/test/perf/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0) 10236043 2023-07-18 14:32:33.000000 mite-1.1.8/test/test.har
+-rw-r--r--   0 root         (0) root         (0)     5240 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_collector.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_context.py
+-rw-r--r--   0 root         (0) root         (0)     3700 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_datapools.py
+-rw-r--r--   0 root         (0) root         (0)     7712 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_har_to_mite.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_mite_amqp.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_mite_browser.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_mite_http.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_mite_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_mite_websockets.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_prometheus_mite.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_recorder.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_runner_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_scenario.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_stats.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_volume_model.py
+-rw-r--r--   0 root         (0) root         (0)     8670 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_webdriver.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-18 14:32:33.000000 mite-1.1.8/test/test_work_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-18 14:32:33.000000 mite-1.1.8/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0) 10236043 2023-07-18 14:32:33.000000 mite-1.1.8/test.har
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-07-18 14:32:33.000000 mite-1.1.8/tox.ini
```

### Comparing `mite-1.1.7/.circleci/config.yml` & `mite-1.1.8/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `mite-1.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/.gitignore` & `mite-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/.travis.yml` & `mite-1.1.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/CODE_OF_CONDUCT.md` & `mite-1.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/CONTRIBUTING.md` & `mite-1.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/DEV.md` & `mite-1.1.8/DEV.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/Dockerfile` & `mite-1.1.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/LICENSE` & `mite-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/PKG-INFO` & `mite-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mite
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python Performance Testing Framework
 Home-page: https://github.com/sky-uk/mite/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,28 +15,25 @@
 Provides-Extra: finagle
 Provides-Extra: selenium
 Provides-Extra: selenium_wire
 License-File: LICENSE
 
 # Mite
 
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sky-uk/mite/blob/master/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![Docs](https://img.shields.io/badge/docs-read-blue)](https://sky-uk.github.io/mite/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/) [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sky-uk/mite/blob/master/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![Docs](https://img.shields.io/badge/docs-read-blue)](https://sky-uk.github.io/mite/)
 
 ## Load Testing Framework
 
 Mite is a load testing framework with distributed components written in Python.
 Requests are executed asynchronously, allowing large throughput from relatively small infrastructure.
 
 ## Installation
 
 ```bash
-python3 -m venv ~/.virtualenvs/mite
-source ~/.virtualenvs/mite/bin/activate
-
-pip install -r requirements.txt
+pip install mite
 ```
 
 
 This requires that you have libcurl installed on your system (including C header files for development, which are often distributed separately from the shared libraries).  On Ubuntu, this can be accomplished with the command:
 
 ```
 sudo apt install libcurl4 libcurl4-openssl-dev
@@ -225,13 +222,13 @@
 
 ## Maintainers
 
 If you run into any trouble or need support getting to grips with Mite,
 reach out on [Slack](https://sky.slack.com/messages/mite) if you work at Sky,
  or contact one of the maintainers if you're an external contributer:
 
-| [<img src="https://avatars.githubusercontent.com/jb098" width=100 height=100 alt="Jordan Brennan" /><br />Jordan Brennan](https://github.com/jb098)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/aecay" width=100 height=100 alt="Aaron Ecay" /> <br />Aaron Ecay](https://github.com/aecay)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/DavAnnunz" width=100 height=100 alt="Davide Annunziata" /><br />Davide Annunziata](https://github.com/DavAnnunz)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/arroncanhamskyuk" width=100 height=100 alt="Arron Canham" /><br />Arron Canham](https://github.com/arroncanhamskyuk)<br /><sub>💻</sub> |
-| :---: | :---: | :---: | :---: |
+| [<img src="https://avatars.githubusercontent.com/jb098" width=100 height=100 alt="Jordan Brennan" /><br />Jordan Brennan](https://github.com/jb098)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/aecay" width=100 height=100 alt="Aaron Ecay" /> <br />Aaron Ecay](https://github.com/aecay)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/DavAnnunz" width=100 height=100 alt="Davide Annunziata" /><br />Davide Annunziata](https://github.com/DavAnnunz)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/ryanlinnit-sky" width=100 height=100 alt="Ryan Linnit" /><br />Ryan Linnit](https://github.com/ryanlinnit-sky)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/cosmaprc" width=100 height=100 alt="Cosmin Purcherea" /><br />Cosmin Purcherea](https://github.com/cosmaprc)<br /><sub>💻</sub> |
+| :---: | :---: | :---: | :---: | :---: |
 
 **Special thanks to the following contributors:**
 
 * [Tony Simpson](https://github.com/tonysimpson)
```

### Comparing `mite-1.1.7/README.md` & `mite-1.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # Mite
 
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sky-uk/mite/blob/master/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![Docs](https://img.shields.io/badge/docs-read-blue)](https://sky-uk.github.io/mite/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/) [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sky-uk/mite/blob/master/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![Docs](https://img.shields.io/badge/docs-read-blue)](https://sky-uk.github.io/mite/)
 
 ## Load Testing Framework
 
 Mite is a load testing framework with distributed components written in Python.
 Requests are executed asynchronously, allowing large throughput from relatively small infrastructure.
 
 ## Installation
 
 ```bash
-python3 -m venv ~/.virtualenvs/mite
-source ~/.virtualenvs/mite/bin/activate
-
-pip install -r requirements.txt
+pip install mite
 ```
 
 
 This requires that you have libcurl installed on your system (including C header files for development, which are often distributed separately from the shared libraries).  On Ubuntu, this can be accomplished with the command:
 
 ```
 sudo apt install libcurl4 libcurl4-openssl-dev
@@ -206,13 +203,13 @@
 
 ## Maintainers
 
 If you run into any trouble or need support getting to grips with Mite,
 reach out on [Slack](https://sky.slack.com/messages/mite) if you work at Sky,
  or contact one of the maintainers if you're an external contributer:
 
-| [<img src="https://avatars.githubusercontent.com/jb098" width=100 height=100 alt="Jordan Brennan" /><br />Jordan Brennan](https://github.com/jb098)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/aecay" width=100 height=100 alt="Aaron Ecay" /> <br />Aaron Ecay](https://github.com/aecay)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/DavAnnunz" width=100 height=100 alt="Davide Annunziata" /><br />Davide Annunziata](https://github.com/DavAnnunz)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/arroncanhamskyuk" width=100 height=100 alt="Arron Canham" /><br />Arron Canham](https://github.com/arroncanhamskyuk)<br /><sub>💻</sub> |
-| :---: | :---: | :---: | :---: |
+| [<img src="https://avatars.githubusercontent.com/jb098" width=100 height=100 alt="Jordan Brennan" /><br />Jordan Brennan](https://github.com/jb098)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/aecay" width=100 height=100 alt="Aaron Ecay" /> <br />Aaron Ecay](https://github.com/aecay)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/DavAnnunz" width=100 height=100 alt="Davide Annunziata" /><br />Davide Annunziata](https://github.com/DavAnnunz)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/ryanlinnit-sky" width=100 height=100 alt="Ryan Linnit" /><br />Ryan Linnit](https://github.com/ryanlinnit-sky)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/cosmaprc" width=100 height=100 alt="Cosmin Purcherea" /><br />Cosmin Purcherea](https://github.com/cosmaprc)<br /><sub>💻</sub> |
+| :---: | :---: | :---: | :---: | :---: |
 
 **Special thanks to the following contributors:**
 
 * [Tony Simpson](https://github.com/tonysimpson)
```

### Comparing `mite-1.1.7/cd-scripts/cdBuild-1.sh` & `mite-1.1.8/cd-scripts/cdBuild-1.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/cd-scripts/cdRelease.py` & `mite-1.1.8/cd-scripts/cdRelease.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/cd.yml` & `mite-1.1.8/cd.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docker_compose.yml` & `mite-1.1.8/docker_compose.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docker_compose_monitoring.yml` & `mite-1.1.8/docker_compose_monitoring.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/Makefile` & `mite-1.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/components.rst` & `mite-1.1.8/docs/components.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/conf.py` & `mite-1.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/config.rst` & `mite-1.1.8/docs/config.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/design-deployment.rst` & `mite-1.1.8/docs/design-deployment.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/index.rst` & `mite-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/journeys.rst` & `mite-1.1.8/docs/journeys.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/prometheus.rst` & `mite-1.1.8/docs/prometheus.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/stats.rst` & `mite-1.1.8/docs/stats.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/docs/volume-model.rst` & `mite-1.1.8/docs/volume-model.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/grafana/provisioning/dashboards/grafana_dashboard_template.json` & `mite-1.1.8/grafana/provisioning/dashboards/grafana_dashboard_template.json`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/grafana/provisioning/dashboards/mite_docker.json` & `mite-1.1.8/grafana/provisioning/dashboards/mite_docker.json`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/local/Makefile` & `mite-1.1.8/local/Makefile`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/local/README.md` & `mite-1.1.8/local/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/local/demo.py` & `mite-1.1.8/local/demo.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/local/run_mite.sh` & `mite-1.1.8/local/run_mite.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/__init__.py` & `mite-1.1.8/mite/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/__main__.py` & `mite-1.1.8/mite/__main__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/cli/cat.py` & `mite-1.1.8/mite/cli/cat.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/cli/collector.py` & `mite-1.1.8/mite/cli/collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/cli/common.py` & `mite-1.1.8/mite/cli/common.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/cli/duplicator.py` & `mite-1.1.8/mite/cli/duplicator.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/cli/receiver.py` & `mite-1.1.8/mite/cli/receiver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/cli/stats.py` & `mite-1.1.8/mite/cli/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/cli/test.py` & `mite-1.1.8/mite/cli/test.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/collector.py` & `mite-1.1.8/mite/collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/config.py` & `mite-1.1.8/mite/config.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/context.py` & `mite-1.1.8/mite/context.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/controller.py` & `mite-1.1.8/mite/controller.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/datapools.py` & `mite-1.1.8/mite/datapools.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/example.py` & `mite-1.1.8/mite/example.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/har_to_mite.py` & `mite-1.1.8/mite/har_to_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/logoutput.py` & `mite-1.1.8/mite/logoutput.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/nanomsg.py` & `mite-1.1.8/mite/nanomsg.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/recorder.py` & `mite-1.1.8/mite/recorder.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/runner.py` & `mite-1.1.8/mite/runner.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/scenario.py` & `mite-1.1.8/mite/scenario.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/stats.py` & `mite-1.1.8/mite/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/test.py` & `mite-1.1.8/mite/test.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/utils.py` & `mite-1.1.8/mite/utils.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/volume_model.py` & `mite-1.1.8/mite/volume_model.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/web/prometheus.py` & `mite-1.1.8/mite/web/prometheus.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite/zmq.py` & `mite-1.1.8/mite/zmq.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite.egg-info/PKG-INFO` & `mite-1.1.8/mite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mite
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python Performance Testing Framework
 Home-page: https://github.com/sky-uk/mite/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,28 +15,25 @@
 Provides-Extra: finagle
 Provides-Extra: selenium
 Provides-Extra: selenium_wire
 License-File: LICENSE
 
 # Mite
 
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sky-uk/mite/blob/master/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![Docs](https://img.shields.io/badge/docs-read-blue)](https://sky-uk.github.io/mite/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/) [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sky-uk/mite/blob/master/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![Docs](https://img.shields.io/badge/docs-read-blue)](https://sky-uk.github.io/mite/)
 
 ## Load Testing Framework
 
 Mite is a load testing framework with distributed components written in Python.
 Requests are executed asynchronously, allowing large throughput from relatively small infrastructure.
 
 ## Installation
 
 ```bash
-python3 -m venv ~/.virtualenvs/mite
-source ~/.virtualenvs/mite/bin/activate
-
-pip install -r requirements.txt
+pip install mite
 ```
 
 
 This requires that you have libcurl installed on your system (including C header files for development, which are often distributed separately from the shared libraries).  On Ubuntu, this can be accomplished with the command:
 
 ```
 sudo apt install libcurl4 libcurl4-openssl-dev
@@ -225,13 +222,13 @@
 
 ## Maintainers
 
 If you run into any trouble or need support getting to grips with Mite,
 reach out on [Slack](https://sky.slack.com/messages/mite) if you work at Sky,
  or contact one of the maintainers if you're an external contributer:
 
-| [<img src="https://avatars.githubusercontent.com/jb098" width=100 height=100 alt="Jordan Brennan" /><br />Jordan Brennan](https://github.com/jb098)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/aecay" width=100 height=100 alt="Aaron Ecay" /> <br />Aaron Ecay](https://github.com/aecay)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/DavAnnunz" width=100 height=100 alt="Davide Annunziata" /><br />Davide Annunziata](https://github.com/DavAnnunz)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/arroncanhamskyuk" width=100 height=100 alt="Arron Canham" /><br />Arron Canham](https://github.com/arroncanhamskyuk)<br /><sub>💻</sub> |
-| :---: | :---: | :---: | :---: |
+| [<img src="https://avatars.githubusercontent.com/jb098" width=100 height=100 alt="Jordan Brennan" /><br />Jordan Brennan](https://github.com/jb098)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/aecay" width=100 height=100 alt="Aaron Ecay" /> <br />Aaron Ecay](https://github.com/aecay)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/DavAnnunz" width=100 height=100 alt="Davide Annunziata" /><br />Davide Annunziata](https://github.com/DavAnnunz)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/ryanlinnit-sky" width=100 height=100 alt="Ryan Linnit" /><br />Ryan Linnit](https://github.com/ryanlinnit-sky)<br /><sub>💻</sub> | [<img src="https://avatars.githubusercontent.com/cosmaprc" width=100 height=100 alt="Cosmin Purcherea" /><br />Cosmin Purcherea](https://github.com/cosmaprc)<br /><sub>💻</sub> |
+| :---: | :---: | :---: | :---: | :---: |
 
 **Special thanks to the following contributors:**
 
 * [Tony Simpson](https://github.com/tonysimpson)
```

### Comparing `mite-1.1.7/mite.egg-info/SOURCES.txt` & `mite-1.1.8/mite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_amqp/__init__.py` & `mite-1.1.8/mite_amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_browser/__init__.py` & `mite-1.1.8/mite_browser/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/README.md` & `mite-1.1.8/mite_finagle/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/__init__.py` & `mite-1.1.8/mite_finagle/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/mux.py` & `mite-1.1.8/mite_finagle/mux.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/stats.py` & `mite-1.1.8/mite_finagle/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/tests/conftest.py` & `mite-1.1.8/mite_finagle/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/tests/foo_service/Foo-remote` & `mite-1.1.8/mite_finagle/tests/foo_service/Foo-remote`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/tests/foo_service/Foo.py` & `mite-1.1.8/mite_finagle/tests/foo_service/Foo.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/tests/foo_service/ttypes.py` & `mite-1.1.8/mite_finagle/tests/foo_service/ttypes.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/tests/test_integration.py` & `mite-1.1.8/mite_finagle/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/tests/test_mux.py` & `mite-1.1.8/mite_finagle/tests/test_mux.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/tests/test_thrift.py` & `mite-1.1.8/mite_finagle/tests/test_thrift.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_finagle/thrift.py` & `mite-1.1.8/mite_finagle/thrift.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_http/__init__.py` & `mite-1.1.8/mite_http/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_http/stats.py` & `mite-1.1.8/mite_http/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_selenium/__init__.py` & `mite-1.1.8/mite_selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_selenium/stats.py` & `mite-1.1.8/mite_selenium/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/mite_websocket/__init__.py` & `mite-1.1.8/mite_websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/setup.cfg` & `mite-1.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/mocks/mock_direct_receiver.py` & `mite-1.1.8/test/mocks/mock_direct_receiver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/mocks/mock_direct_runner_transport.py` & `mite-1.1.8/test/mocks/mock_direct_runner_transport.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/mocks/mock_recorder_msg_http.py` & `mite-1.1.8/test/mocks/mock_recorder_msg_http.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/mocks/mock_selenium.py` & `mite-1.1.8/test/mocks/mock_selenium.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/perf/http_server.py` & `mite-1.1.8/test/perf/http_server.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/perf/http_server_aiohttp.py` & `mite-1.1.8/test/perf/http_server_aiohttp.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/perf/mite_perftest.py` & `mite-1.1.8/test/perf/mite_perftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/perf/perftest.py` & `mite-1.1.8/test/perf/perftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/perf/run-perftest.sh` & `mite-1.1.8/test/perf/run-perftest.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test.har` & `mite-1.1.8/test/test.har`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_collector.py` & `mite-1.1.8/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_config.py` & `mite-1.1.8/test/test_config.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_context.py` & `mite-1.1.8/test/test_context.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_controller.py` & `mite-1.1.8/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_datapools.py` & `mite-1.1.8/test/test_datapools.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_har_to_mite.py` & `mite-1.1.8/test/test_har_to_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_mite_amqp.py` & `mite-1.1.8/test/test_mite_amqp.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_mite_browser.py` & `mite-1.1.8/test/test_mite_browser.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_mite_http.py` & `mite-1.1.8/test/test_mite_http.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_mite_utils.py` & `mite-1.1.8/test/test_mite_utils.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_mite_websockets.py` & `mite-1.1.8/test/test_mite_websockets.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_prometheus_mite.py` & `mite-1.1.8/test/test_prometheus_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_recorder.py` & `mite-1.1.8/test/test_recorder.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_runner.py` & `mite-1.1.8/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_runner_tracker.py` & `mite-1.1.8/test/test_runner_tracker.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_scenario.py` & `mite-1.1.8/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_stats.py` & `mite-1.1.8/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_volume_model.py` & `mite-1.1.8/test/test_volume_model.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_webdriver.py` & `mite-1.1.8/test/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test/test_work_tracker.py` & `mite-1.1.8/test/test_work_tracker.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/test.har` & `mite-1.1.8/test.har`

 * *Files identical despite different names*

### Comparing `mite-1.1.7/tox.ini` & `mite-1.1.8/tox.ini`

 * *Files identical despite different names*

