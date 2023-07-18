# Comparing `tmp/kafkit-0.3.0b1.tar.gz` & `tmp/kafkit-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkit-0.3.0b1.tar", last modified: Tue Jan 10 16:56:26 2023, max compression
+gzip compressed data, was "kafkit-1.0.0a1.tar", last modified: Tue Jul 18 16:14:29 2023, max compression
```

## Comparing `kafkit-0.3.0b1.tar` & `kafkit-1.0.0a1.tar`

### file list

```diff
@@ -1,74 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.590450 kafkit-0.3.0b1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.590450 kafkit-0.3.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/.github/workflows/periodic-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.594451 kafkit-0.3.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.594451 kafkit-0.3.0b1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.594451 kafkit-0.3.0b1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/guide/recordnameschemamanager-howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/guide/strimzi-ssl-howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.594451 kafkit-0.3.0b1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/licenses/gidgethub.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.590450 kafkit-0.3.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.594451 kafkit-0.3.0b1/src/kafkit/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/src/kafkit/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/registry/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/registry/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/registry/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/registry/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/registry/sansio.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/registry/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/src/kafkit/ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/src/kafkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-01-10 16:56:26.000000 kafkit-0.3.0b1/src/kafkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-01-10 16:56:26.000000 kafkit-0.3.0b1/src/kafkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 16:56:26.000000 kafkit-0.3.0b1/src/kafkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-10 16:56:26.000000 kafkit-0.3.0b1/src/kafkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-10 16:56:26.000000 kafkit-0.3.0b1/src/kafkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.590450 kafkit-0.3.0b1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/tests/data/record_name_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/data/record_name_schemas/kafkit.a.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/data/record_name_schemas/kafkit.b.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 16:56:26.598451 kafkit-0.3.0b1/tests/data/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/data/ssl/client.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/data/ssl/client.key
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/data/ssl/cluster.ca.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/httputils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/registry_httpx_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/registry_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/registry_sansio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/registry_serializer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tests/ssl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-10 16:56:13.000000 kafkit-0.3.0b1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.489451 kafkit-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.github/workflows/dependencies.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.github/workflows/periodic-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/changelog.d/20230613_123447_jsick_DM_39648.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/changelog.d/20230717_125707_jsick_DM_39646.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/changelog.d/_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/guide/recordnameschemamanager-howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/guide/strimzi-ssl-howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/licenses/gidgethub.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:14:29.489451 kafkit-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.477451 kafkit-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.481451 kafkit-1.0.0a1/src/kafkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/src/kafkit/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/src/kafkit/fastapi/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/fastapi/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/fastapi/dependencies/aiokafkaproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/fastapi/dependencies/pydanticschemamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/fastapi/dependencies/registryapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/src/kafkit/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/src/kafkit/registry/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/manager/_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/manager/_recordname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/sansio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/registry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/src/kafkit/ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/src/kafkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-18 16:14:29.000000 kafkit-1.0.0a1/src/kafkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-18 16:14:29.000000 kafkit-1.0.0a1/src/kafkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:14:29.000000 kafkit-1.0.0a1/src/kafkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-18 16:14:29.000000 kafkit-1.0.0a1/src/kafkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 16:14:29.000000 kafkit-1.0.0a1/src/kafkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.477451 kafkit-1.0.0a1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/tests/data/record_name_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/data/record_name_schemas/kafkit.a.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/data/record_name_schemas/kafkit.b.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:14:29.485451 kafkit-1.0.0a1/tests/data/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/data/ssl/client.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/data/ssl/client.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/data/ssl/cluster.ca.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/httputils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/pydantic_schema_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/registry_httpx_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/registry_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/registry_sansio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/registry_serializer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tests/ssl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-18 16:14:17.000000 kafkit-1.0.0a1/tox.ini
```

### Comparing `kafkit-0.3.0b1/.github/workflows/periodic-ci.yaml` & `kafkit-1.0.0a1/.github/workflows/periodic-ci.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 jobs:
   test:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python:
-          - "3.8"
-          - "3.9"
           - "3.10"
           - "3.11"
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Run tests in tox
@@ -35,25 +33,25 @@
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Build docs in tox
         uses: lsst-sqre/run-tox@v1
         with:
-          python-version: "3.10"
+          python-version: "3.11"
           tox-envs: "docs,docs-linkcheck"
           use-cache: false
 
-  pypi:
+  test-packaging:
     runs-on: ubuntu-latest
+    timeout-minutes: 10
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
       - name: Build and publish
-        uses: lsst-sqre/build-and-publish-to-pypi@v1
+        uses: lsst-sqre/build-and-publish-to-pypi@v2
         with:
-          pypi-token: ""
-          python-version: "3.10"
+          python-version: "3.11"
           upload: false
```

### Comparing `kafkit-0.3.0b1/.gitignore` & `kafkit-1.0.0a1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.vscode
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `kafkit-0.3.0b1/.pre-commit-config.yaml` & `kafkit-1.0.0a1/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -3,33 +3,33 @@
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: check-yaml
       - id: check-toml
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies: [toml]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.1.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==22.6.0]
+        additional_dependencies: [black==23.1.0]
         args: [-l, '79', -t, py38]
 
   - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.2.2
+    rev: 6.3.0
     hooks:
     - id: pydocstyle
       additional_dependencies: [tomli]
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
```

### Comparing `kafkit-0.3.0b1/LICENSE` & `kafkit-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/PKG-INFO` & `kafkit-1.0.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: kafkit
-Version: 0.3.0b1
+Version: 1.0.0a1
 Summary: Kafkit helps you write Kafka producers and consumers in Python with asyncio.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT
 Project-URL: Homepage, https://kafkit.lsst.io
 Project-URL: Source, https://github.com/lsst-sqre/kafkit
 Keywords: rubin,lsst
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: aiohttp
 Provides-Extra: httpx
+Provides-Extra: pydantic
+Provides-Extra: aiokafka
 Provides-Extra: dev
 License-File: LICENSE
 
 # Kafkit
 
 Kafkit helps you write Kafka producers and consumers in Python with asyncio:
```

### Comparing `kafkit-0.3.0b1/README.md` & `kafkit-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/docker-compose.yaml` & `kafkit-1.0.0a1/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/docs/Makefile` & `kafkit-1.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/docs/_rst_epilog.rst` & `kafkit-1.0.0a1/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/docs/dev/development.rst` & `kafkit-1.0.0a1/docs/dev/development.rst`

 * *Files 8% similar despite different names*

```diff
@@ -39,17 +39,14 @@
 
 Pre-commit hooks
 ================
 
 The pre-commit hooks, which are automatically installed by running the :command:`make init` command on :ref:`set up <dev-environment>`, ensure that files are valid and properly formatted.
 Some pre-commit hooks automatically reformat code:
 
-``seed-isort-config``
-    Adds configuration for isort to the :file:`pyproject.toml` file.
-
 ``isort``
     Automatically sorts imports in Python modules.
 
 ``black``
     Automatically formats Python code.
 
 ``blacken-docs``
@@ -69,67 +66,64 @@
 
    pytest
 
 You can also run tox_, which tests the library the same way that the CI workflow does:
 
 .. code-block:: sh
 
-   tox
+   tox run
 
 To see a listing of test environments, run:
 
 .. code-block:: sh
 
-   tox -av
+   tox list
 
 .. _dev-build-docs:
 
 Building documentation
 ======================
 
 Documentation is built with Sphinx_:
 
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 
 .. code-block:: sh
 
-   tox -e docs
+   tox run -e docs
 
 The build documentation is located in the :file:`docs/_build/html` directory.
 
 .. _dev-change-log:
 
 Updating the change log
 =======================
 
-Each pull request should update the change log (:file:`CHANGELOG.rst`).
+Each pull request should update the change log (:file:`CHANGELOG.md`).
 Add a description of new features and fixes as list items under a section at the top of the change log called "Unreleased:"
 
-.. code-block:: rst
+.. code-block:: md
 
-   Unreleased
-   ----------
+   ## Unreleased
 
    - Description of the feature or fix.
 
-If the next version is known (because Kafkit's master branch is being prepared for a new major or minor version), the section may contain that version information:
+If the next version is known (because Kafkit's main branch is being prepared for a new major or minor version), the section may contain that version information:
 
-.. code-block:: rst
+.. code-block:: md
 
-   X.Y.0 (unreleased)
-   ------------------
+   ## X.Y.0 (unreleased)
 
    - Description of the feature or fix.
 
 If the exact version and release date is known (:doc:`because a release is being prepared <release>`), the section header is formatted as:
 
 .. code-block:: rst
 
-   X.Y.0 (YYYY-MM-DD)
-   ------------------
+   ## X.Y.0 (YYYY-MM-DD)
 
    - Description of the feature or fix.
 
 .. _style-guide:
 
 Style guide
 ===========
```

### Comparing `kafkit-0.3.0b1/docs/dev/release.rst` & `kafkit-1.0.0a1/docs/dev/release.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,40 +6,40 @@
 This information is only useful for maintainers.
 
 Kafkit's releases are largely automated through GitHub Actions (see the `ci.yaml`_ workflow file for details).
 When a semantic version tag is pushed to GitHub, `Kafkit is released to PyPI`_ with that version.
 Similarly, documentation is built and pushed for each version (see https://kafkit.lsst.io/v).
 
 .. _`Kafkit is released to PyPI`: https://pypi.org/project/kafkit/
-.. _`ci.yaml`: https://github.com/lsst-sqre/kafkit/blob/master/.github/workflows/ci.yaml
+.. _`ci.yaml`: https://github.com/lsst-sqre/kafkit/blob/main/.github/workflows/ci.yaml
 
 .. _regular-release:
 
 Regular releases
 ================
 
-Regular releases happen from the ``master`` branch after changes have been merged.
-From the ``master`` branch you can release a new major version (``X.0.0``), a new minor version of the current major version (``X.Y.0``), or a new patch of the current major-minor version (``X.Y.Z``).
+Regular releases happen from the ``main`` branch after changes have been merged.
+From the ``main`` branch you can release a new major version (``X.0.0``), a new minor version of the current major version (``X.Y.0``), or a new patch of the current major-minor version (``X.Y.Z``).
 See :ref:`backport-release` to patch an earlier major-minor version.
 
 Release tags are semantic version identifiers following the :pep:`440` specification.
 
 1. Change log and documentation
 -------------------------------
 
 Each PR should include updates to the change log.
-If the change log or documentation needs additional updates, now is the time to make those changes through the regular branch-and-PR development method against the ``master`` branch.
+If the change log or documentation needs additional updates, now is the time to make those changes through the regular branch-and-PR development method against the ``main`` branch.
 
 In particular, replace the "Unreleased" section headline with the semantic version and date.
 See :ref:`dev-change-log` in the *Developer guide* for details.
 
 2. Tag the release
 ------------------
 
-At the HEAD of the ``master`` branch, create and push a tag with the semantic version:
+At the HEAD of the ``main`` branch, create and push a tag with the semantic version:
 
 .. code-block:: sh
 
    git tag -s X.Y.Z -m "X.Y.Z"
    git push --tags
 
 The tag **must** follow the :pep:`440` specification since Kafkit uses setuptools_scm_ to set version metadata based on Git tags.
@@ -50,15 +50,15 @@
 The `ci.yaml`_ GitHub Actions workflow uploads the new release to PyPI and documentation to https://kafkit.lsst.io.
 
 .. _backport-release:
 
 Backport releases
 =================
 
-The regular release procedure works from the main line of development on the ``master`` Git branch.
+The regular release procedure works from the main line of development on the ``main`` Git branch.
 To create a release that patches an earlier major or minor version, you need to release from a **release branch.**
 
 Creating a release branch
 -------------------------
 
 Release branches are named after the major and minor components of the version string: ``X.Y``.
 If the release branch doesn't already exist, check out the latest patch for that major-minor version:
@@ -68,16 +68,16 @@
    git checkout X.Y.Z
    git checkout -b X.Y
    git push -u
 
 Developing on a release branch
 ------------------------------
 
-Once a release branch exists, it becomes the "master" branch for patches of that major-minor version.
+Once a release branch exists, it becomes the "main" branch for patches of that major-minor version.
 Pull requests should be based on, and merged into, the release branch.
 
-If the development on the release branch is a backport of commits on the ``master`` branch, use ``git cherry-pick`` to copy those commits into a new pull request against the release branch.
+If the development on the release branch is a backport of commits on the ``main`` branch, use ``git cherry-pick`` to copy those commits into a new pull request against the release branch.
 
 Releasing from a release branch
 -------------------------------
 
-Releases from a release branch are equivalent to :ref:`regular releases <regular-release>`, except that the release branch takes the role of the ``master`` branch.
+Releases from a release branch are equivalent to :ref:`regular releases <regular-release>`, except that the release branch takes the role of the ``main`` branch.
```

### Comparing `kafkit-0.3.0b1/docs/guide/recordnameschemamanager-howto.rst` & `kafkit-1.0.0a1/docs/guide/recordnameschemamanager-howto.rst`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/docs/guide/strimzi-ssl-howto.rst` & `kafkit-1.0.0a1/docs/guide/strimzi-ssl-howto.rst`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/docs/index.rst` & `kafkit-1.0.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/licenses/gidgethub.txt` & `kafkit-1.0.0a1/licenses/gidgethub.txt`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/pyproject.toml` & `kafkit-1.0.0a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 keywords = ["rubin", "lsst"]
 # https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: POSIX",
     "Typing :: Typed",
 ]
-requires-python = ">=3.8"
-dependencies = ["uritemplate", "fastavro"]
+requires-python = ">=3.10"
+dependencies = ["fastavro", "uritemplate"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 aiohttp = ["aiohttp"]
 httpx = ["httpx"]
+pydantic = ["pydantic", "dataclasses-avroschema[pydantic]"]
+aiokafka = ["aiokafka"]
 dev = [
     # Testing
     "coverage[toml]",
     "pytest",
     "pytest-asyncio",
     "pre-commit",
     "mypy",
@@ -76,15 +77,15 @@
     "if 0:",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
 ]
 
 [tool.black]
 line-length = 79
-target-version = ['py38']
+target-version = ['py310']
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.mypy_cache
   | \.tox
   | \.venv
@@ -134,7 +135,20 @@
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 ignore_missing_imports = true
 strict_equality = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_ignores = true
+
+[tool.scriv]
+categories = [
+    "Backwards-incompatible changes",
+    "New features",
+    "Bug fixes",
+    "Other changes",
+]
+entry_title_template = "{{ version }} ({{ date.strftime('%Y-%m-%d') }})"
+format = "md"
+md_header_level = "2"
+new_fragment_template = "file:changelog.d/_template.md"
+skip_fragments = "_template.md"
```

### Comparing `kafkit-0.3.0b1/src/kafkit/__init__.py` & `kafkit-1.0.0a1/src/kafkit/__init__.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/src/kafkit/httputils.py` & `kafkit-1.0.0a1/src/kafkit/httputils.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/src/kafkit/registry/__init__.py` & `kafkit-1.0.0a1/src/kafkit/registry/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,20 +4,28 @@
 
 from kafkit.registry.errors import (
     RegistryBadRequestError,
     RegistryBrokenError,
     RegistryError,
     RegistryHttpError,
     RegistryRedirectionError,
+    UnmanagedSchemaError,
+)
+from kafkit.registry.serializer import (
+    Deserializer,
+    MessageInfo,
+    PolySerializer,
+    Serializer,
 )
-from kafkit.registry.serializer import Deserializer, PolySerializer, Serializer
 
 __all__ = [
     "Deserializer",
+    "MessageInfo",
     "Serializer",
     "PolySerializer",
     "RegistryBadRequestError",
     "RegistryBrokenError",
     "RegistryError",
     "RegistryHttpError",
     "RegistryRedirectionError",
+    "UnmanagedSchemaError",
 ]
```

### Comparing `kafkit-0.3.0b1/src/kafkit/registry/aiohttp.py` & `kafkit-1.0.0a1/src/kafkit/registry/aiohttp.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/src/kafkit/registry/errors.py` & `kafkit-1.0.0a1/src/kafkit/registry/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 __all__ = [
     "RegistryError",
     "RegistryHttpError",
     "RegistryRedirectionError",
     "RegistryBadRequestError",
     "RegistryBrokenError",
+    "UnmanagedSchemaError",
 ]
 
 from typing import Any, Optional
 
 
 class RegistryError(Exception):
     """Base exception for Registry errors."""
@@ -57,7 +58,13 @@
 
 class RegistryBadRequestError(RegistryHttpError):
     """An exception if the request is invalid (4XX errors)."""
 
 
 class RegistryBrokenError(RegistryHttpError):
     """An excpetion if the server is down (5XX errors)."""
+
+
+class UnmanagedSchemaError(Exception):
+    """An exception for when a schema is not managed by the Registry, and
+    therefore cannot be deserialized into a native Python object.
+    """
```

### Comparing `kafkit-0.3.0b1/src/kafkit/registry/httpx.py` & `kafkit-1.0.0a1/src/kafkit/registry/httpx.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/src/kafkit/registry/sansio.py` & `kafkit-1.0.0a1/src/kafkit/registry/sansio.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import json
 import logging
 from enum import Enum
 from typing import Any, Dict, Mapping, Optional, Tuple, Union, overload
 
 import fastavro
 
-from kafkit.httputils import format_url, parse_content_type
-from kafkit.registry.errors import (
+from ..httputils import format_url, parse_content_type
+from .errors import (
     RegistryBadRequestError,
     RegistryBrokenError,
     RegistryHttpError,
     RegistryRedirectionError,
 )
 
 __all__ = [
@@ -124,14 +124,15 @@
 class RegistryApi(metaclass=abc.ABCMeta):
     """A baseclass for Confluent Schema Registry clients."""
 
     def __init__(self, *, url: str) -> None:
         self.url = url
         self._schema_cache = SchemaCache()
         self._subject_cache = SubjectCache(self._schema_cache)
+        self._logger = logging.getLogger(__name__)
 
     @property
     def schema_cache(self) -> SchemaCache:
         """The schema cache (`~kafkit.registry.sansio.SchemaCache`)."""
         return self._schema_cache
 
     @property
@@ -390,36 +391,44 @@
 
     @staticmethod
     def _prep_schema(schema: Mapping[str, Any]) -> str:
         """Prep a schema for submission through an API request by
         removing any fastavro hints and dumping to a string.
         """
         schema = dict(copy.deepcopy(schema))
-        try:
+        if "__fastavro_parsed" in schema:
             del schema["__fastavro_parsed"]
-        except KeyError:
-            pass
+        if "__named_schemas" in schema:
+            del schema["__named_schemas"]
         # sort keys for repeatable tests
         return json.dumps(schema, sort_keys=True)
 
     async def register_schema(
-        self, schema: Mapping[str, Any], subject: Optional[str] = None
+        self,
+        schema: Mapping[str, Any],
+        subject: Optional[str] = None,
+        compatibility: Optional[str] = None,
     ) -> int:
         """Register a schema or get the ID of an existing schema.
 
         Wraps ``POST /subjects/(string: subject)/versions``.
 
         Parameters
         ----------
         schema : `dict`
             An `Avro schema <http://avro.apache.org/docs/current/spec.html>`__
             as a Python dictionary.
         subject : `str`, optional
             The subject to register the schema under. If not provided, the
             fully-qualified name of the schema is adopted as the subject name.
+        compatibility : `str`, optional
+            The compatibility level to use for the subject. If not provided,
+            the existing compatibility level is used (or the server's default
+            compatibility level if subject does not have a specific
+            compatibility level).
 
         Returns
         -------
         schema_id : `int`
             The ID of the schema in the registry.
 
         Notes
@@ -453,16 +462,66 @@
             url_vars={"subject": subject},
             data={"schema": self._prep_schema(schema)},
         )
 
         # add to cache
         self.schema_cache.insert(schema, result["id"])
 
+        if compatibility is not None:
+            await self.set_subject_compatibility(subject, compatibility)
+
         return result["id"]
 
+    async def set_subject_compatibility(
+        self, subject: str, compatibility: str
+    ) -> None:
+        # Validate compatibility setting
+        try:
+            CompatibilityType[compatibility]
+        except KeyError:
+            raise ValueError(
+                f"Compatibility setting {compatibility!r} is not in the "
+                f"allowed set: {[v.value for v in CompatibilityType]}"
+            )
+
+        try:
+            subject_config = await self.get(
+                "/config{/subject}", url_vars={"subject": subject}
+            )
+        except RegistryBadRequestError:
+            self._logger.info(
+                "No existing configuration for this subject: %s", subject
+            )
+            # Create a mock config that forces a reset
+            subject_config = {"compatibilityLevel": None}
+
+        self._logger.debug(
+            "Current config subject=%s config=%s", subject, subject_config
+        )
+
+        if subject_config["compatibilityLevel"] != compatibility:
+            await self.put(
+                "/config{/subject}",
+                url_vars={"subject": subject},
+                data={"compatibility": compatibility},
+            )
+            self._logger.info(
+                "Reset subject compatibility level. "
+                "subject=%s compatibility=%s",
+                subject,
+                compatibility,
+            )
+        else:
+            self._logger.debug(
+                "Existing subject compatibility level is good. "
+                "subject=%s compatibility=%s",
+                subject,
+                compatibility,
+            )
+
     async def get_schema_by_id(self, schema_id: int) -> Dict[str, Any]:
         """Get a schema from the registry given its ID.
 
         Wraps ``GET /schemas/ids/{int: id}``.
 
         Parameters
         ----------
@@ -828,41 +887,39 @@
         subject: str,
         version: int,
         schema_id: Optional[int] = None,
         schema: Optional[Mapping[str, Any]] = None,
     ) -> None:
         """Insert a subject version into the cache.
 
+        If the subject version being cached is already in the schema cache,
+        then only one of ``schema_id`` or ``schema`` need to be passed to this
+        method. However, if the schema isn't cached, then both ``schema_id``
+        and ``schema`` need to be set. The ``schema_id`` and ``schema`` are
+        added to the underlying schema cache.
+
         Parameters
         ----------
         subject : `str`
             The name of the subject.
         version : `int`
             The version number of the schema in the subject.
         schema_id : `int`, optional
-            ID of the schema in a Schema Registry. See Notes.
+            ID of the schema in a Schema Registry.
         schema : `dict`, optional
-            The Avro schema itself. See Notes.
+            The Avro schema itself.
 
         Raises
         ------
         TypeError
             Raised if the ``version`` parameter is a string. String-based
             versions, like "latest," cannot be cached.
         ValueError
             Raised if the ``schema_id`` or ``schema`` parameters are needed
-            but aren't set. See Notes.
-
-        Notes
-        -----
-        If the subject version being cached is already in the schema cache,
-        then only one of ``schema_id`` or ``schema`` need to be passed to this
-        method. However, if the schema isn't cached, then both ``schema_id``
-        and ``schema`` need to be set. The ``schema_id`` and ``schema`` are
-        added to the underlying schema cache.
+            but aren't set.
         """
         if not isinstance(version, int):
             raise TypeError(
                 "Cannot cache a non-integer version of a subject "
                 '(such as "latest").'
             )
```

### Comparing `kafkit-0.3.0b1/src/kafkit/registry/serializer.py` & `kafkit-1.0.0a1/src/kafkit/registry/serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Avro serialization and deserialization helpers that integrate with the
 Confluent Schema Registry.
 """
 
 from __future__ import annotations
 
 import struct
+from dataclasses import dataclass
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
 
 import fastavro
 
 if TYPE_CHECKING:
     from kafkit.registry.sansio import RegistryApi
 
 __all__ = [
     "Serializer",
     "PolySerializer",
     "Deserializer",
+    "MessageInfo",
 ]
 
 
 class Serializer:
     """An Avro message serializer that writes in the Confluent Wire Format.
 
     Use the `Serializer.register` class method to create a Serializer instance.
@@ -200,14 +202,67 @@
     message_fh.write(pack_wire_format_prefix(schema_id))
     # Write the Avro-encoded message
     fastavro.schemaless_writer(message_fh, schema, data)
     message_fh.seek(0)
     return message_fh.read()
 
 
+@dataclass
+class MessageInfo:
+    """A message, along with schema information.
+
+    Parameters
+    ----------
+    id
+        The ID of the schema (an `int`) in the Schema Registry. This uniquely
+        identifies the message's schema.
+    schema
+        The schema, as a Python object.
+    message
+        The message itself, as a decoded Python object.
+
+    Attributes
+    ----------
+    id
+        The ID of the schema (an `int`) in the Schema Registry. This uniquely
+        identifies the message's schema.
+    schema
+        The schema, as a Python object.
+    message
+        The message itself, as a decoded Python object.
+    """
+
+    id: int
+    """The ID of the schema (an `int`) in the Schema Registry. This uniquely
+    identifies the message's schema.
+    """
+
+    schema: dict[str, Any]
+    """The schema, as a Python object."""
+
+    message: Any
+    """The message itself, as a decoded Python object."""
+
+    def __getitem__(self, key: str) -> Any:
+        """Get info by key (for backwards compatibility).
+
+        This method is for backwards-compatibility when
+        `Deserializer.deserialize` returned a dict. Attribute-based access is
+        recommended, e.g. ``message_info.id``, to enable type checking.
+        """
+        if key == "id":
+            return self.id
+        elif key == "message":
+            return self.message
+        elif key == "schema":
+            return self.schema
+
+        raise KeyError(f"Unknown key: {key}")
+
+
 class Deserializer:
     """An Avro message deserializer that understands the Confluent Wire Format
     and obtains schemas on-demand from a Confluent Schema Registry.
 
     Parameters
     ----------
     registry : `kafkit.registry.sansio.RegistryApi`
@@ -242,55 +297,35 @@
     coroutines. It's not the end of the world, though, just call
     `~Deserializer.deserialize` manually on by bytes obtained by the consumer.
     """
 
     def __init__(self, *, registry: RegistryApi) -> None:
         self._registry = registry
 
-    async def deserialize(
-        self, data: bytes, include_schema: bool = False
-    ) -> Dict[str, Any]:
+    async def deserialize(self, data: bytes) -> MessageInfo:
         """Deserialize a message.
 
         Parameters
         ----------
         data : `bytes`
             The encoded message, usually obtained directly from a Kafka
             consumer. The message must be in the Confluent Wire Format.
-        include_schema : `bool`, optional
-            If `True`, the schema itself is included in the returned value.
-            This is useful if your application operates on many different
-            types of messages, and needs a convenient way to introspect
-            a message's type.
 
         Returns
         -------
-        message_info : `dict`
-            The deserialized message is wrapped in a dictionary to include
-            metadata. The keys are:
-
-            ``'id'``
-                The ID of the schema (an `int`) in the Schema Registry. This
-                uniquely identifies the message's schema.
-            ``'message'``
-                The message itself, as a decoded Python object.
-            ``'schema'``
-                The schema, as a Python object. This key is only included
-                when ``include_schema`` is `True`.
+        MessageInfo
+            The deserialized message and schema information.
         """
         schema_id, message_data = unpack_wire_format_data(data)
         schema = await self._registry.get_schema_by_id(schema_id)
 
         message_fh = BytesIO(message_data)
         message_fh.seek(0)
         message = fastavro.schemaless_reader(message_fh, schema)
-        result = {"id": schema_id, "message": message}
-        if include_schema:
-            result["schema"] = schema
-        return result
+        return MessageInfo(schema_id, schema, message)
 
 
 def pack_wire_format_prefix(schema_id: int) -> bytes:
     """Create the bytes prefix for a Confluent Wire Format message.
 
     Parameters
     ----------
```

### Comparing `kafkit-0.3.0b1/src/kafkit/ssl.py` & `kafkit-1.0.0a1/src/kafkit/ssl.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/src/kafkit.egg-info/PKG-INFO` & `kafkit-1.0.0a1/src/kafkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: kafkit
-Version: 0.3.0b1
+Version: 1.0.0a1
 Summary: Kafkit helps you write Kafka producers and consumers in Python with asyncio.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT
 Project-URL: Homepage, https://kafkit.lsst.io
 Project-URL: Source, https://github.com/lsst-sqre/kafkit
 Keywords: rubin,lsst
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: aiohttp
 Provides-Extra: httpx
+Provides-Extra: pydantic
+Provides-Extra: aiokafka
 Provides-Extra: dev
 License-File: LICENSE
 
 # Kafkit
 
 Kafkit helps you write Kafka producers and consumers in Python with asyncio:
```

### Comparing `kafkit-0.3.0b1/src/kafkit.egg-info/SOURCES.txt` & `kafkit-1.0.0a1/src/kafkit.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
+.prettierignore
 CHANGELOG.md
 LICENSE
 Makefile
 README.md
 docker-compose.yaml
 pyproject.toml
-setup.py
 tox.ini
 .github/dependabot.yml
 .github/workflows/ci.yaml
+.github/workflows/dependencies.yaml
 .github/workflows/periodic-ci.yaml
+changelog.d/20230613_123447_jsick_DM_39648.md
+changelog.d/20230717_125707_jsick_DM_39646.md
+changelog.d/_template.md
 docs/.gitignore
 docs/Makefile
 docs/_rst_epilog.rst
 docs/api.rst
 docs/changelog.md
 docs/conf.py
 docs/documenteer.toml
@@ -26,29 +30,39 @@
 docs/guide/index.rst
 docs/guide/recordnameschemamanager-howto.rst
 docs/guide/strimzi-ssl-howto.rst
 licenses/gidgethub.txt
 src/kafkit/__init__.py
 src/kafkit/httputils.py
 src/kafkit/py.typed
+src/kafkit/settings.py
 src/kafkit/ssl.py
 src/kafkit.egg-info/PKG-INFO
 src/kafkit.egg-info/SOURCES.txt
 src/kafkit.egg-info/dependency_links.txt
 src/kafkit.egg-info/requires.txt
 src/kafkit.egg-info/top_level.txt
+src/kafkit/fastapi/__init__.py
+src/kafkit/fastapi/dependencies/__init__.py
+src/kafkit/fastapi/dependencies/aiokafkaproducer.py
+src/kafkit/fastapi/dependencies/pydanticschemamanager.py
+src/kafkit/fastapi/dependencies/registryapi.py
 src/kafkit/registry/__init__.py
 src/kafkit/registry/aiohttp.py
 src/kafkit/registry/errors.py
 src/kafkit/registry/httpx.py
-src/kafkit/registry/manager.py
 src/kafkit/registry/sansio.py
 src/kafkit/registry/serializer.py
+src/kafkit/registry/utils.py
+src/kafkit/registry/manager/__init__.py
+src/kafkit/registry/manager/_pydantic.py
+src/kafkit/registry/manager/_recordname.py
 tests/__init__.py
 tests/httputils_test.py
+tests/pydantic_schema_manager_test.py
 tests/registry_httpx_test.py
 tests/registry_manager_test.py
 tests/registry_sansio_test.py
 tests/registry_serializer_test.py
 tests/ssl_test.py
 tests/data/record_name_schemas/kafkit.a.json
 tests/data/record_name_schemas/kafkit.b.json
```

### Comparing `kafkit-0.3.0b1/tests/data/ssl/client.crt` & `kafkit-1.0.0a1/tests/data/ssl/client.crt`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/tests/data/ssl/client.key` & `kafkit-1.0.0a1/tests/data/ssl/client.key`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/tests/data/ssl/cluster.ca.crt` & `kafkit-1.0.0a1/tests/data/ssl/cluster.ca.crt`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/tests/httputils_test.py` & `kafkit-1.0.0a1/tests/httputils_test.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/tests/registry_httpx_test.py` & `kafkit-1.0.0a1/tests/registry_httpx_test.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/tests/registry_manager_test.py` & `kafkit-1.0.0a1/tests/registry_manager_test.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/tests/registry_sansio_test.py` & `kafkit-1.0.0a1/tests/registry_sansio_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,15 @@
         client.url
         == "http://registry:8081/subjects/test-schemas.schema1/versions"
     )
     sent_json = json.loads(client.body)
     assert "schema" in sent_json
     sent_schema = json.loads(sent_json["schema"])
     assert "__fastavro_parsed" not in sent_schema
+    assert "__named_schemas" not in sent_schema
     assert sent_schema["name"] == "test-schemas.schema1"
 
     # Check that the schema is in the cache and is parsed
     # Value of type "Union[int, Dict[str, Any]]" is not indexable
     cached_schema = client.schema_cache[1]
     assert cached_schema["name"] == "test-schemas.schema1"
     assert "__fastavro_parsed" in cached_schema
```

### Comparing `kafkit-0.3.0b1/tests/registry_serializer_test.py` & `kafkit-1.0.0a1/tests/registry_serializer_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,22 +109,23 @@
     message_2 = {"c": 13, "d": "bonjour"}
     data_2 = serializer2(message_2)
 
     # Deserialization
     deserializer = Deserializer(registry=client)
 
     response_1 = await deserializer.deserialize(data_1)
+    # Test attribute and key-based access to message info
     assert response_1["id"] == schema1_id
     assert response_1["message"] == message_1
-    assert "schema" not in response_1
+    assert response_1.id == schema1_id
+    assert response_1.message == message_1
 
-    response_2 = await deserializer.deserialize(data_2, include_schema=True)
+    response_2 = await deserializer.deserialize(data_2)
     assert response_2["id"] == schema2_id
     assert response_2["message"] == message_2
-    assert "schema" in response_2
     assert response_2["schema"]["name"] == "test-schemas.schema2"
 
 
 @pytest.mark.asyncio
 async def test_polyserializer_given_id() -> None:
     """Test the PolySerializer class, given schema IDs."""
     # First schema
```

### Comparing `kafkit-0.3.0b1/tests/ssl_test.py` & `kafkit-1.0.0a1/tests/ssl_test.py`

 * *Files identical despite different names*

### Comparing `kafkit-0.3.0b1/tox.ini` & `kafkit-1.0.0a1/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 description = Run pytest against {envname}.
 deps =
     holdup < 3
 extras =
     dev
     aiohttp
     httpx
+    pydantic
+    aiokafka
 allowlist_externals =
     docker-compose
 setenv =
     KAFKA_BROKER_URL=localhost:9092
     SCHEMA_REGISTRY_URL=http://localhost:8081
 commands =
     docker-compose up -d
@@ -30,15 +32,15 @@
 commands =
     coverage combine
     coverage report
 
 [testenv:typing]
 description = Run mypy.
 commands =
-    mypy src/kafkit tests setup.py
+    mypy src/kafkit tests
 
 [testenv:lint]
 description = Lint codebase by running pre-commit (Black, isort, Flake8).
 skip_install = true
 deps = pre-commit
 commands = pre-commit run --all-files
```

