# Comparing `tmp/antsibull-0.8.0.tar.gz` & `tmp/antsibull-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antsibull-0.8.0.tar", last modified: Mon Jun  8 18:40:53 2020, max compression
+gzip compressed data, was "antsibull-0.9.0.tar", last modified: Thu Jun 18 07:19:57 2020, max compression
```

## Comparing `antsibull-0.8.0.tar` & `antsibull-0.9.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
--rw-r--r--   0        0        0    35149 2020-06-02 09:03:07.101192 antsibull-0.8.0/LICENSE
--rw-r--r--   0        0        0     1373 2020-06-02 09:03:07.101192 antsibull-0.8.0/README.md
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.101192 antsibull-0.8.0/antsibull/__init__.py
--rw-r--r--   0        0        0     9093 2020-06-03 07:47:45.322618 antsibull-0.8.0/antsibull/ansible_base.py
--rw-r--r--   0        0        0     2706 2020-06-08 18:40:43.760447 antsibull-0.8.0/antsibull/augment_docs.py
--rw-r--r--   0        0        0    10127 2020-06-08 18:40:43.760447 antsibull-0.8.0/antsibull/build_acd_commands.py
--rw-r--r--   0        0        0     1486 2020-06-02 09:03:07.102192 antsibull-0.8.0/antsibull/build_collection.py
--rw-r--r--   0        0        0       29 2020-06-02 09:03:07.102192 antsibull-0.8.0/antsibull/cli/__init__.py
--rw-r--r--   0        0        0     8671 2020-06-02 09:03:07.102192 antsibull-0.8.0/antsibull/cli/antsibull_build.py
--rw-r--r--   0        0        0    11130 2020-06-08 18:40:43.760447 antsibull-0.8.0/antsibull/cli/antsibull_docs.py
--rw-r--r--   0        0        0     3288 2020-06-02 09:03:07.103192 antsibull-0.8.0/antsibull/cli/antsibull_lint.py
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.103192 antsibull-0.8.0/antsibull/cli/doc_commands/__init__.py
--rw-r--r--   0        0        0      290 2020-06-02 09:03:07.103192 antsibull-0.8.0/antsibull/cli/doc_commands/collection.py
--rw-r--r--   0        0        0     2976 2020-06-03 07:47:45.323618 antsibull-0.8.0/antsibull/cli/doc_commands/current.py
--rw-r--r--   0        0        0      290 2020-06-02 09:03:07.103192 antsibull-0.8.0/antsibull/cli/doc_commands/devel.py
--rw-r--r--   0        0        0      290 2020-06-02 09:03:07.103192 antsibull-0.8.0/antsibull/cli/doc_commands/plugin.py
--rw-r--r--   0        0        0    14082 2020-06-08 18:40:43.760447 antsibull-0.8.0/antsibull/cli/doc_commands/stable.py
--rw-r--r--   0        0        0     3314 2020-06-08 18:40:43.761447 antsibull-0.8.0/antsibull/collections.py
--rw-r--r--   0        0        0     1181 2020-06-02 09:03:07.104192 antsibull-0.8.0/antsibull/compat.py
--rw-r--r--   0        0        0      634 2020-06-02 09:03:07.104192 antsibull-0.8.0/antsibull/config.py
--rw-r--r--   0        0        0     1149 2020-06-03 07:47:45.323618 antsibull-0.8.0/antsibull/constants.py
--rw-r--r--   0        0        0      179 2020-06-02 09:03:07.105192 antsibull-0.8.0/antsibull/data/README_md.txt
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.105192 antsibull-0.8.0/antsibull/data/__init__.py
--rw-r--r--   0        0        0      198 2020-06-02 09:03:07.105192 antsibull-0.8.0/antsibull/data/acd-readme.txt
--rw-r--r--   0        0        0     2132 2020-06-02 09:03:07.105192 antsibull-0.8.0/antsibull/data/acd-setup_py.j2
--rw-r--r--   0        0        0      431 2020-06-02 09:03:07.105192 antsibull-0.8.0/antsibull/data/collection-readme.j2
--rw-r--r--   0        0        0      772 2020-06-02 09:03:07.105192 antsibull-0.8.0/antsibull/data/collection-setup_py.j2
--rw-r--r--   0        0        0      136 2020-06-02 09:03:07.105192 antsibull-0.8.0/antsibull/data/debian/changelog.j2
--rw-r--r--   0        0        0      835 2020-06-02 09:03:07.106192 antsibull-0.8.0/antsibull/data/debian/control
--rw-r--r--   0        0        0     1075 2020-06-02 09:03:07.106192 antsibull-0.8.0/antsibull/data/debian/copyright
--rwxr-xr-x   0        0        0      566 2020-06-02 09:03:07.106192 antsibull-0.8.0/antsibull/data/debian/rules
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.106192 antsibull-0.8.0/antsibull/data/docsite/__init__.py
--rw-r--r--   0        0        0      261 2020-06-03 07:47:45.323618 antsibull-0.8.0/antsibull/data/docsite/list_of_collections.rst.j2
--rw-r--r--   0        0        0      521 2020-06-02 09:03:07.106192 antsibull-0.8.0/antsibull/data/docsite/plugin-deprecation.rst.j2
--rw-r--r--   0        0        0      407 2020-06-04 06:29:27.914657 antsibull-0.8.0/antsibull/data/docsite/plugin-error.rst.j2
--rw-r--r--   0        0        0    18264 2020-06-08 18:40:43.761447 antsibull-0.8.0/antsibull/data/docsite/plugin.rst.j2
--rw-r--r--   0        0        0      768 2020-06-02 09:03:07.107192 antsibull-0.8.0/antsibull/data/docsite/plugins_by_collection.rst.j2
--rw-r--r--   0        0        0     2382 2020-06-02 09:03:07.107192 antsibull-0.8.0/antsibull/data/galaxy_yml.j2
--rw-r--r--   0        0        0    35148 2020-06-02 09:03:07.108192 antsibull-0.8.0/antsibull/data/gplv3.txt
--rw-r--r--   0        0        0     6027 2020-06-02 09:03:07.108192 antsibull-0.8.0/antsibull/dependency_files.py
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.108192 antsibull-0.8.0/antsibull/docs_parsing/__init__.py
--rw-r--r--   0        0        0     9959 2020-06-08 18:40:43.761447 antsibull-0.8.0/antsibull/docs_parsing/ansible_doc.py
--rw-r--r--   0        0        0     1387 2020-06-02 09:03:07.109192 antsibull-0.8.0/antsibull/docs_parsing/fqcn.py
--rw-r--r--   0        0        0     2720 2020-06-02 09:03:07.109192 antsibull-0.8.0/antsibull/filesystem.py
--rw-r--r--   0        0        0    10704 2020-06-02 09:03:07.109192 antsibull-0.8.0/antsibull/galaxy.py
--rw-r--r--   0        0        0     1028 2020-06-02 09:03:07.109192 antsibull-0.8.0/antsibull/hashing.py
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.110192 antsibull-0.8.0/antsibull/jinja2/__init__.py
--rw-r--r--   0        0        0     2308 2020-06-02 09:03:07.110192 antsibull-0.8.0/antsibull/jinja2/environment.py
--rw-r--r--   0        0        0     2411 2020-06-02 09:03:07.110192 antsibull-0.8.0/antsibull/jinja2/filters.py
--rw-r--r--   0        0        0     1733 2020-06-02 09:03:07.110192 antsibull-0.8.0/antsibull/jinja2/tests.py
--rw-r--r--   0        0        0      742 2020-06-02 09:03:07.110192 antsibull-0.8.0/antsibull/logging.py
--rw-r--r--   0        0        0     2877 2020-06-08 18:40:43.761447 antsibull-0.8.0/antsibull/new_acd.py
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.110192 antsibull-0.8.0/antsibull/schemas/__init__.py
--rw-r--r--   0        0        0     4417 2020-06-02 09:03:07.111192 antsibull-0.8.0/antsibull/schemas/ansible_doc.py
--rw-r--r--   0        0        0    15398 2020-06-08 18:40:43.762447 antsibull-0.8.0/antsibull/schemas/base.py
--rw-r--r--   0        0        0     1098 2020-06-02 09:03:07.111192 antsibull-0.8.0/antsibull/schemas/callback.py
--rw-r--r--   0        0        0     1264 2020-06-02 09:03:07.111192 antsibull-0.8.0/antsibull/schemas/config.py
--rw-r--r--   0        0        0     2379 2020-06-02 09:03:07.111192 antsibull-0.8.0/antsibull/schemas/docs.py
--rw-r--r--   0        0        0     1367 2020-06-02 09:03:07.112192 antsibull-0.8.0/antsibull/schemas/module.py
--rw-r--r--   0        0        0     3926 2020-06-02 09:03:07.112192 antsibull-0.8.0/antsibull/schemas/plugin.py
--rw-r--r--   0        0        0     1425 2020-06-02 09:03:07.115192 antsibull-0.8.0/antsibull/tarball.py
--rw-r--r--   0        0        0        0 2020-06-08 18:40:43.762447 antsibull-0.8.0/antsibull/utils/__init__.py
--rw-r--r--   0        0        0     1092 2020-06-08 18:40:43.762447 antsibull-0.8.0/antsibull/utils/collections.py
--rw-r--r--   0        0        0        0 2020-06-02 09:03:07.115192 antsibull-0.8.0/antsibull/vendored/__init__.py
--rw-r--r--   0        0        0     3608 2020-06-02 09:03:07.115192 antsibull-0.8.0/antsibull/vendored/collections.py
--rw-r--r--   0        0        0     3311 2020-06-02 09:03:07.116192 antsibull-0.8.0/antsibull/vendored/json_utils.py
--rw-r--r--   0        0        0     3355 2020-06-03 07:47:45.324618 antsibull-0.8.0/antsibull/venv.py
--rw-r--r--   0        0        0     7214 2020-06-08 18:40:43.763447 antsibull-0.8.0/antsibull/write_docs.py
--rw-r--r--   0        0        0     1253 2020-06-08 18:40:43.763447 antsibull-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3932 2020-06-02 09:03:07.119192 antsibull-0.8.0/tests/aiohttp_utils.py
--rw-r--r--   0        0        0     3895 2020-06-02 09:03:07.119192 antsibull-0.8.0/tests/certificate_utils.py
--rw-r--r--   0        0        0     1987 2020-06-02 09:03:07.120192 antsibull-0.8.0/tests/functional/schema/good_data/one_become.json
--rw-r--r--   0        0        0     3436 2020-06-02 09:03:07.120192 antsibull-0.8.0/tests/functional/schema/good_data/one_become_results.json
--rw-r--r--   0        0        0     2467 2020-06-02 09:03:07.120192 antsibull-0.8.0/tests/functional/schema/good_data/one_cache.json
--rw-r--r--   0        0        0     4859 2020-06-02 09:03:07.120192 antsibull-0.8.0/tests/functional/schema/good_data/one_cache_results.json
--rw-r--r--   0        0        0     1818 2020-06-02 09:03:07.120192 antsibull-0.8.0/tests/functional/schema/good_data/one_callback.json
--rw-r--r--   0        0        0     2240 2020-06-02 09:03:07.120192 antsibull-0.8.0/tests/functional/schema/good_data/one_callback_results.json
--rw-r--r--   0        0        0     1418 2020-06-02 09:03:07.120192 antsibull-0.8.0/tests/functional/schema/good_data/one_cliconf.json
--rw-r--r--   0        0        0     2367 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_cliconf_results.json
--rw-r--r--   0        0        0    10708 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_connection.json
--rw-r--r--   0        0        0    18935 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_connection_results.json
--rw-r--r--   0        0        0     1163 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_httpapi.json
--rw-r--r--   0        0        0     2079 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_httpapi_results.json
--rw-r--r--   0        0        0    15025 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_inventory.json
--rw-r--r--   0        0        0    28033 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_inventory_results.json
--rw-r--r--   0        0        0     5093 2020-06-02 09:03:07.121192 antsibull-0.8.0/tests/functional/schema/good_data/one_lookup.json
--rw-r--r--   0        0        0    11281 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_lookup_results.json
--rw-r--r--   0        0        0     3548 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_module.json
--rw-r--r--   0        0        0     4598 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_module_results.json
--rw-r--r--   0        0        0     1166 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_netconf.json
--rw-r--r--   0        0        0     2035 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_netconf_results.json
--rw-r--r--   0        0        0     4711 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_shell.json
--rw-r--r--   0        0        0     8245 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_shell_results.json
--rw-r--r--   0        0        0     1115 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_strategy.json
--rw-r--r--   0        0        0     1530 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_strategy_results.json
--rw-r--r--   0        0        0     3489 2020-06-02 09:03:07.122192 antsibull-0.8.0/tests/functional/schema/good_data/one_vars.json
--rw-r--r--   0        0        0     5036 2020-06-02 09:03:07.123192 antsibull-0.8.0/tests/functional/schema/good_data/one_vars_results.json
--rw-r--r--   0        0        0     1540 2020-06-02 09:03:07.123192 antsibull-0.8.0/tests/functional/schema/test_schema.py
--rw-r--r--   0        0        0     1261 2020-06-02 09:03:07.123192 antsibull-0.8.0/tests/test_galaxy.py
--rw-r--r--   0        0        0      563 2020-06-02 09:03:07.123192 antsibull-0.8.0/tests/units/test_parse_pieces.py
--rw-r--r--   0        0        0     2879 2020-06-08 18:40:53.835327 antsibull-0.8.0/setup.py
--rw-r--r--   0        0        0     2414 2020-06-08 18:40:53.835705 antsibull-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-05-26 22:56:26.130291 antsibull-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1373 2020-06-01 15:41:41.108995 antsibull-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2020-05-26 22:56:26.130291 antsibull-0.9.0/antsibull/__init__.py
+-rw-r--r--   0        0        0     9034 2020-06-12 04:00:29.706593 antsibull-0.9.0/antsibull/ansible_base.py
+-rw-r--r--   0        0        0     2626 2020-06-12 04:00:29.713593 antsibull-0.9.0/antsibull/augment_docs.py
+-rw-r--r--   0        0        0    11514 2020-06-18 06:49:07.093979 antsibull-0.9.0/antsibull/build_acd_commands.py
+-rw-r--r--   0        0        0     1486 2020-05-26 22:56:26.130291 antsibull-0.9.0/antsibull/build_collection.py
+-rw-r--r--   0        0        0       29 2020-06-01 01:22:42.760824 antsibull-0.9.0/antsibull/cli/__init__.py
+-rw-r--r--   0        0        0     8676 2020-06-12 04:00:29.714593 antsibull-0.9.0/antsibull/cli/antsibull_build.py
+-rw-r--r--   0        0        0    11130 2020-06-08 18:42:01.374297 antsibull-0.9.0/antsibull/cli/antsibull_docs.py
+-rw-r--r--   0        0        0     3288 2020-06-01 01:22:42.762824 antsibull-0.9.0/antsibull/cli/antsibull_lint.py
+-rw-r--r--   0        0        0        0 2020-06-01 01:22:42.762824 antsibull-0.9.0/antsibull/cli/doc_commands/__init__.py
+-rw-r--r--   0        0        0      290 2020-06-01 01:22:42.763824 antsibull-0.9.0/antsibull/cli/doc_commands/collection.py
+-rw-r--r--   0        0        0     2976 2020-06-05 17:11:58.930576 antsibull-0.9.0/antsibull/cli/doc_commands/current.py
+-rw-r--r--   0        0        0      290 2020-06-01 01:22:42.763824 antsibull-0.9.0/antsibull/cli/doc_commands/devel.py
+-rw-r--r--   0        0        0      290 2020-06-01 01:22:42.763824 antsibull-0.9.0/antsibull/cli/doc_commands/plugin.py
+-rw-r--r--   0        0        0    14396 2020-06-12 04:00:29.714593 antsibull-0.9.0/antsibull/cli/doc_commands/stable.py
+-rw-r--r--   0        0        0     3314 2020-06-08 18:42:01.375297 antsibull-0.9.0/antsibull/collections.py
+-rw-r--r--   0        0        0     1181 2020-06-01 01:22:42.765824 antsibull-0.9.0/antsibull/compat.py
+-rw-r--r--   0        0        0      634 2020-06-01 01:22:42.765824 antsibull-0.9.0/antsibull/config.py
+-rw-r--r--   0        0        0     1149 2020-06-05 17:11:58.931576 antsibull-0.9.0/antsibull/constants.py
+-rw-r--r--   0        0        0      179 2020-05-26 22:56:26.134291 antsibull-0.9.0/antsibull/data/README_md.txt
+-rw-r--r--   0        0        0        0 2020-05-26 22:56:26.134291 antsibull-0.9.0/antsibull/data/__init__.py
+-rw-r--r--   0        0        0      198 2020-05-26 22:56:26.134291 antsibull-0.9.0/antsibull/data/acd-readme.txt
+-rw-r--r--   0        0        0     2171 2020-06-12 04:00:29.715593 antsibull-0.9.0/antsibull/data/acd-setup_py.j2
+-rw-r--r--   0        0        0      370 2020-06-17 07:54:08.926499 antsibull-0.9.0/antsibull/data/build-ansible.sh.j2
+-rw-r--r--   0        0        0      431 2020-05-26 22:56:26.134291 antsibull-0.9.0/antsibull/data/collection-readme.j2
+-rw-r--r--   0        0        0      772 2020-05-26 22:56:26.134291 antsibull-0.9.0/antsibull/data/collection-setup_py.j2
+-rw-r--r--   0        0        0      136 2020-05-29 22:20:34.073768 antsibull-0.9.0/antsibull/data/debian/changelog.j2
+-rw-r--r--   0        0        0      835 2020-05-29 22:20:34.073768 antsibull-0.9.0/antsibull/data/debian/control
+-rw-r--r--   0        0        0     1075 2020-05-29 22:20:34.073768 antsibull-0.9.0/antsibull/data/debian/copyright
+-rwxr-xr-x   0        0        0      566 2020-05-29 22:20:34.073768 antsibull-0.9.0/antsibull/data/debian/rules
+-rw-r--r--   0        0        0        0 2020-06-01 01:22:42.766824 antsibull-0.9.0/antsibull/data/docsite/__init__.py
+-rw-r--r--   0        0        0      261 2020-06-05 17:11:58.931576 antsibull-0.9.0/antsibull/data/docsite/list_of_collections.rst.j2
+-rw-r--r--   0        0        0      521 2020-06-01 01:23:44.011812 antsibull-0.9.0/antsibull/data/docsite/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0      407 2020-06-05 17:11:58.931576 antsibull-0.9.0/antsibull/data/docsite/plugin-error.rst.j2
+-rw-r--r--   0        0        0    18264 2020-06-08 18:42:01.375297 antsibull-0.9.0/antsibull/data/docsite/plugin.rst.j2
+-rw-r--r--   0        0        0      768 2020-06-01 01:22:42.767824 antsibull-0.9.0/antsibull/data/docsite/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     2382 2020-05-26 22:56:26.135290 antsibull-0.9.0/antsibull/data/galaxy_yml.j2
+-rw-r--r--   0        0        0    35148 2020-05-26 22:56:26.135290 antsibull-0.9.0/antsibull/data/gplv3.txt
+-rw-r--r--   0        0        0     6011 2020-06-12 04:00:29.715593 antsibull-0.9.0/antsibull/dependency_files.py
+-rw-r--r--   0        0        0        0 2020-06-01 01:22:42.768824 antsibull-0.9.0/antsibull/docs_parsing/__init__.py
+-rw-r--r--   0        0        0    10253 2020-06-12 04:00:29.716593 antsibull-0.9.0/antsibull/docs_parsing/ansible_doc.py
+-rw-r--r--   0        0        0     1387 2020-06-01 01:22:42.768824 antsibull-0.9.0/antsibull/docs_parsing/fqcn.py
+-rw-r--r--   0        0        0     2720 2020-06-01 01:22:42.769824 antsibull-0.9.0/antsibull/filesystem.py
+-rw-r--r--   0        0        0    10704 2020-06-05 17:11:58.932576 antsibull-0.9.0/antsibull/galaxy.py
+-rw-r--r--   0        0        0     1028 2020-06-05 17:11:58.932576 antsibull-0.9.0/antsibull/hashing.py
+-rw-r--r--   0        0        0        0 2020-06-01 01:22:42.769824 antsibull-0.9.0/antsibull/jinja2/__init__.py
+-rw-r--r--   0        0        0     2308 2020-06-01 01:22:42.769824 antsibull-0.9.0/antsibull/jinja2/environment.py
+-rw-r--r--   0        0        0     2411 2020-06-01 01:22:42.770824 antsibull-0.9.0/antsibull/jinja2/filters.py
+-rw-r--r--   0        0        0     1733 2020-06-01 01:22:42.770824 antsibull-0.9.0/antsibull/jinja2/tests.py
+-rw-r--r--   0        0        0      742 2020-06-01 01:22:42.771824 antsibull-0.9.0/antsibull/logging.py
+-rw-r--r--   0        0        0     2870 2020-06-12 04:00:29.716593 antsibull-0.9.0/antsibull/new_acd.py
+-rw-r--r--   0        0        0        0 2020-05-26 22:56:26.136291 antsibull-0.9.0/antsibull/schemas/__init__.py
+-rw-r--r--   0        0        0     4417 2020-05-26 22:56:26.136291 antsibull-0.9.0/antsibull/schemas/ansible_doc.py
+-rw-r--r--   0        0        0    15398 2020-06-08 18:42:01.376297 antsibull-0.9.0/antsibull/schemas/base.py
+-rw-r--r--   0        0        0     1098 2020-05-26 22:56:26.137291 antsibull-0.9.0/antsibull/schemas/callback.py
+-rw-r--r--   0        0        0     1264 2020-06-01 01:22:42.773824 antsibull-0.9.0/antsibull/schemas/config.py
+-rw-r--r--   0        0        0     2379 2020-05-26 22:56:26.137291 antsibull-0.9.0/antsibull/schemas/docs.py
+-rw-r--r--   0        0        0     1367 2020-05-26 22:56:26.137291 antsibull-0.9.0/antsibull/schemas/module.py
+-rw-r--r--   0        0        0     3926 2020-05-26 22:56:26.137291 antsibull-0.9.0/antsibull/schemas/plugin.py
+-rw-r--r--   0        0        0     1425 2020-06-01 01:22:42.773824 antsibull-0.9.0/antsibull/tarball.py
+-rw-r--r--   0        0        0        0 2020-06-08 18:42:01.376297 antsibull-0.9.0/antsibull/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2020-06-08 18:42:01.377297 antsibull-0.9.0/antsibull/utils/collections.py
+-rw-r--r--   0        0        0        0 2020-06-01 01:22:42.774824 antsibull-0.9.0/antsibull/vendored/__init__.py
+-rw-r--r--   0        0        0     3608 2020-06-01 01:22:42.774824 antsibull-0.9.0/antsibull/vendored/collections.py
+-rw-r--r--   0        0        0     3311 2020-06-01 01:22:42.775824 antsibull-0.9.0/antsibull/vendored/json_utils.py
+-rw-r--r--   0        0        0     3355 2020-06-05 17:11:58.932576 antsibull-0.9.0/antsibull/venv.py
+-rw-r--r--   0        0        0     7214 2020-06-08 18:42:01.377297 antsibull-0.9.0/antsibull/write_docs.py
+-rw-r--r--   0        0        0     1253 2020-06-12 04:00:29.717593 antsibull-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3932 2020-05-26 22:56:26.139291 antsibull-0.9.0/tests/aiohttp_utils.py
+-rw-r--r--   0        0        0     3895 2020-05-26 22:56:26.139291 antsibull-0.9.0/tests/certificate_utils.py
+-rw-r--r--   0        0        0     1987 2020-05-26 22:56:26.142290 antsibull-0.9.0/tests/functional/schema/good_data/one_become.json
+-rw-r--r--   0        0        0     3436 2020-06-01 01:22:42.778824 antsibull-0.9.0/tests/functional/schema/good_data/one_become_results.json
+-rw-r--r--   0        0        0     2467 2020-05-26 22:56:26.142290 antsibull-0.9.0/tests/functional/schema/good_data/one_cache.json
+-rw-r--r--   0        0        0     4859 2020-06-01 01:22:42.778824 antsibull-0.9.0/tests/functional/schema/good_data/one_cache_results.json
+-rw-r--r--   0        0        0     1818 2020-05-26 22:56:26.143291 antsibull-0.9.0/tests/functional/schema/good_data/one_callback.json
+-rw-r--r--   0        0        0     2240 2020-06-01 01:22:42.779824 antsibull-0.9.0/tests/functional/schema/good_data/one_callback_results.json
+-rw-r--r--   0        0        0     1418 2020-05-26 22:56:26.143291 antsibull-0.9.0/tests/functional/schema/good_data/one_cliconf.json
+-rw-r--r--   0        0        0     2367 2020-06-01 01:22:42.780824 antsibull-0.9.0/tests/functional/schema/good_data/one_cliconf_results.json
+-rw-r--r--   0        0        0    10708 2020-05-26 22:56:26.143291 antsibull-0.9.0/tests/functional/schema/good_data/one_connection.json
+-rw-r--r--   0        0        0    18935 2020-06-01 01:22:42.781824 antsibull-0.9.0/tests/functional/schema/good_data/one_connection_results.json
+-rw-r--r--   0        0        0     1163 2020-05-26 22:56:26.143291 antsibull-0.9.0/tests/functional/schema/good_data/one_httpapi.json
+-rw-r--r--   0        0        0     2079 2020-06-01 01:22:42.781824 antsibull-0.9.0/tests/functional/schema/good_data/one_httpapi_results.json
+-rw-r--r--   0        0        0    15025 2020-05-26 22:56:26.143291 antsibull-0.9.0/tests/functional/schema/good_data/one_inventory.json
+-rw-r--r--   0        0        0    28033 2020-06-01 01:22:42.782824 antsibull-0.9.0/tests/functional/schema/good_data/one_inventory_results.json
+-rw-r--r--   0        0        0     5093 2020-05-26 22:56:26.144291 antsibull-0.9.0/tests/functional/schema/good_data/one_lookup.json
+-rw-r--r--   0        0        0    11281 2020-06-01 01:22:42.783824 antsibull-0.9.0/tests/functional/schema/good_data/one_lookup_results.json
+-rw-r--r--   0        0        0     3548 2020-05-26 22:56:26.144291 antsibull-0.9.0/tests/functional/schema/good_data/one_module.json
+-rw-r--r--   0        0        0     4598 2020-06-01 01:22:42.783824 antsibull-0.9.0/tests/functional/schema/good_data/one_module_results.json
+-rw-r--r--   0        0        0     1166 2020-06-01 01:22:42.784824 antsibull-0.9.0/tests/functional/schema/good_data/one_netconf.json
+-rw-r--r--   0        0        0     2035 2020-06-01 01:22:42.785824 antsibull-0.9.0/tests/functional/schema/good_data/one_netconf_results.json
+-rw-r--r--   0        0        0     4711 2020-05-26 22:56:26.144291 antsibull-0.9.0/tests/functional/schema/good_data/one_shell.json
+-rw-r--r--   0        0        0     8245 2020-06-01 01:22:42.786824 antsibull-0.9.0/tests/functional/schema/good_data/one_shell_results.json
+-rw-r--r--   0        0        0     1115 2020-05-26 22:56:26.144291 antsibull-0.9.0/tests/functional/schema/good_data/one_strategy.json
+-rw-r--r--   0        0        0     1530 2020-06-01 01:22:42.787824 antsibull-0.9.0/tests/functional/schema/good_data/one_strategy_results.json
+-rw-r--r--   0        0        0     3489 2020-05-26 22:56:26.145290 antsibull-0.9.0/tests/functional/schema/good_data/one_vars.json
+-rw-r--r--   0        0        0     5036 2020-06-01 01:22:42.787824 antsibull-0.9.0/tests/functional/schema/good_data/one_vars_results.json
+-rw-r--r--   0        0        0     1540 2020-05-26 22:56:26.145290 antsibull-0.9.0/tests/functional/schema/test_schema.py
+-rw-r--r--   0        0        0     1261 2020-05-26 22:56:26.145290 antsibull-0.9.0/tests/test_galaxy.py
+-rw-r--r--   0        0        0      563 2020-05-26 22:56:26.145290 antsibull-0.9.0/tests/units/test_parse_pieces.py
+-rw-r--r--   0        0        0     2879 2020-06-18 07:19:57.550319 antsibull-0.9.0/setup.py
+-rw-r--r--   0        0        0     2414 2020-06-18 07:19:57.550732 antsibull-0.9.0/PKG-INFO
```

### Comparing `antsibull-0.8.0/LICENSE` & `antsibull-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/README.md` & `antsibull-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/ansible_base.py` & `antsibull-0.9.0/antsibull/ansible_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import os
 import re
 import typing as t
 from functools import lru_cache
 from urllib.parse import urljoin
 
 import aiofiles
-import packaging.version as pypiver
 import sh
+from packaging.version import Version as PypiVer
 
 from .compat import best_get_loop
 from .constants import CHUNKSIZE
 
 if t.TYPE_CHECKING:
     import aiohttp.client
 
@@ -57,27 +57,27 @@
         """
         # Retrieve the ansible-base package info from pypi
         query_url = urljoin(self.pypi_server_url, 'pypi/ansible-base/json')
         async with self.aio_session.get(query_url) as response:
             pkg_info = await response.json()
         return pkg_info
 
-    async def get_versions(self) -> t.List[pypiver.Version]:
+    async def get_versions(self) -> t.List[PypiVer]:
         """
         Get the versions of the ansible-base package on pypi.
 
         :returns: A list of :pypkg:obj:`packaging.versioning.Version`s
             for all the versions on pypi, including prereleases.
         """
         pkg_info = await self.get_info()
-        versions = [pypiver.Version(r) for r in pkg_info['releases']]
+        versions = [PypiVer(r) for r in pkg_info['releases']]
         versions.sort(reverse=True)
         return versions
 
-    async def get_latest_version(self) -> pypiver.Version:
+    async def get_latest_version(self) -> PypiVer:
         """
         Get the latest version of ansible-base uploaded to pypi.
 
         :return: A :pypkg:obj:`packaging.versioning.Version` object representing the latest version
             of the package on pypi.  This may be a pre-release.
         """
         versions = await self.get_versions()
@@ -111,15 +111,15 @@
                 while chunk:
                     await f.write(chunk)
                     chunk = await response.content.read(CHUNKSIZE)
 
         return tar_filename
 
 
-def _get_cache_version(ansible_base_cache: str) -> pypiver.Version:
+def _get_cache_version(ansible_base_cache: str) -> PypiVer:
     with open(os.path.join(ansible_base_cache, 'lib', 'ansible', 'release.py')) as f:
         root = ast.parse(f.read())
 
     # Find the version of the cache
     cache_version = None
     # Iterate backwards in case __version__ is assigned to multiple times
     for node in reversed(root.body):
@@ -132,15 +132,15 @@
 
         if cache_version:
             break
 
     if not cache_version:
         raise ValueError('Version was not found')
 
-    return pypiver.Version(cache_version)
+    return PypiVer(cache_version)
 
 
 def cache_is_devel(ansible_base_cache: t.Optional[str]) -> bool:
     """
     :arg ansible_base_cache: A path to an Ansible-base checkout or expanded sdist or None.
         This will be used instead of downloading an ansible-base package if the version matches
         with ``ansible_base_version``.
@@ -158,15 +158,15 @@
     if dev_version.match(cache_version.public):
         return True
 
     return False
 
 
 def cache_is_correct_version(ansible_base_cache: t.Optional[str],
-                             ansible_base_version: pypiver.Version) -> bool:
+                             ansible_base_version: PypiVer) -> bool:
     """
     :arg ansible_base_cache: A path to an Ansible-base checkout or expanded sdist or None.
         This will be used instead of downloading an ansible-base package if the version matches
         with ``ansible_base_version``.
     :arg ansible_base_version: Version of ansible-base to retrieve.
     :returns: True if the cache is for a compatible version at or newer than the requested version
     """
@@ -225,17 +225,17 @@
             assert ansible_base_cache is not None
             return ansible_base_cache
 
         install_file = await checkout_from_git(tmpdir)
     else:
         pypi_client = AnsibleBasePyPiClient(aio_session)
         if ansible_base_version == '@latest':
-            ansible_base_version: pypiver.Version = await pypi_client.get_latest_version()
+            ansible_base_version: PypiVer = await pypi_client.get_latest_version()
         else:
-            ansible_base_version: pypiver.Version = pypiver.Version(ansible_base_version)
+            ansible_base_version: PypiVer = PypiVer(ansible_base_version)
 
         # is the cache the asked for version?
         if cache_is_correct_version(ansible_base_cache, ansible_base_version):
             assert ansible_base_cache is not None
             return ansible_base_cache
 
         install_file = await pypi_client.retrieve(ansible_base_version.public, tmpdir)
```

### Comparing `antsibull-0.8.0/antsibull/augment_docs.py` & `antsibull-0.9.0/antsibull/augment_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # Author: Toshio Kuratomi <tkuratom@redhat.com>
 # License: GPLv3+
 # Copyright: Ansible Project, 2020
 """Augment data from plugin documenation with additional values."""
 
 import typing as t
-from collections.abc import Mapping
-
-from .utils.collections import is_sequence
 
 
 def add_full_key(options_data: t.Mapping[str, t.Any], suboption_entry: str,
                  _full_key: t.Optional[list] = None) -> None:
     """
     Add information on the strucfture of a dict value in options or returns.
```

### Comparing `antsibull-0.8.0/antsibull/build_acd_commands.py` & `antsibull-0.9.0/antsibull/build_acd_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from functools import partial
 
 import aiofiles
 import aiohttp
 import asyncio_pool
 import sh
 from jinja2 import Template
+from packaging.version import Version as PypiVer
 
 from .collections import install_separately, install_together
 from .constants import THREAD_MAX
 from .dependency_files import BuildFile, DepsFile
 from .galaxy import CollectionDownloader
 
 
@@ -65,33 +66,37 @@
 
 
 def write_manifest(package_dir, debian=False):
     manifest_file = os.path.join(package_dir, 'MANIFEST.in')
     with open(manifest_file, 'w') as f:
         f.write('include COPYING\n')
         f.write('include README\n')
+        f.write('include build-ansible.sh\n')
         if debian:
             f.write('include debian/*\n')
         f.write('recursive-include ansible_collections/ **\n')
 
 
-def write_setup(acd_version, collection_deps, package_dir):
+def write_setup(acd_version, ansible_base_version, collection_deps, package_dir):
     setup_filename = os.path.join(package_dir, 'setup.py')
 
     setup_tmpl = Template(pkgutil.get_data('antsibull.data', 'acd-setup_py.j2').decode('utf-8'))
-    setup_contents = setup_tmpl.render(version=acd_version, collection_deps=collection_deps)
+    setup_contents = setup_tmpl.render(version=acd_version,
+                                       ansible_base_version=ansible_base_version,
+                                       collection_deps=collection_deps)
 
     with open(setup_filename, 'w') as f:
         f.write(setup_contents)
 
 
-def write_python_build_files(acd_version, collection_deps, package_dir, debian=False):
+def write_python_build_files(acd_version, ansible_base_version, collection_deps, package_dir,
+                             debian=False):
     copy_boilerplate_files(package_dir)
     write_manifest(package_dir, debian)
-    write_setup(acd_version, collection_deps, package_dir)
+    write_setup(acd_version, ansible_base_version, collection_deps, package_dir)
 
 
 def write_debian_directory(acd_version, package_dir):
     debian_dir = os.path.join(package_dir, 'debian')
     os.mkdir(debian_dir, mode=0o700)
     debian_files = ('changelog.j2', 'control', 'copyright', 'rules')
     for filename in debian_files:
@@ -120,17 +125,32 @@
     files = os.listdir(dist_dir)
     if len(files) != 1:
         raise Exception('python setup.py sdist should only have created one file')
 
     shutil.move(os.path.join(dist_dir, files[0]), dest_dir)
 
 
+def write_build_script(acd_version, ansible_base_version, package_dir):
+    """Write a build-script that tells how to build this tarball."""
+    build_ansible_filename = os.path.join(package_dir, 'build-ansible.sh')
+
+    build_ansible_tmpl = Template(pkgutil.get_data('antsibull.data',
+                                                   'build-ansible.sh.j2').decode('utf-8'))
+    build_ansible_contents = build_ansible_tmpl.render(version=acd_version,
+                                                       ansible_base_version=ansible_base_version)
+
+    with open(build_ansible_filename, 'w') as f:
+        f.write(build_ansible_contents)
+    os.chmod(build_ansible_filename, mode=0o755)
+
+
 def build_single_command(args):
     build_file = BuildFile(args.build_file)
     build_acd_version, ansible_base_version, deps = build_file.parse()
+    ansible_base_version = PypiVer(ansible_base_version)
 
     if not str(args.acd_version).startswith(build_acd_version):
         print(f'{args.build_file} is for version {build_acd_version} but we need'
               ' {args.acd_version.major}.{arg.acd_version.minor}')
         return 1
 
     with tempfile.TemporaryDirectory() as tmp_dir:
@@ -143,15 +163,17 @@
         os.mkdir(package_dir, mode=0o700)
         ansible_collections_dir = os.path.join(package_dir, 'ansible_collections')
         os.mkdir(ansible_collections_dir, mode=0o700)
 
         collections_to_install = [p for f in os.listdir(download_dir)
                                   if os.path.isfile(p := os.path.join(download_dir, f))]
         asyncio.run(install_together(collections_to_install, ansible_collections_dir))
-        write_python_build_files(args.acd_version, '', package_dir, args.debian)
+        write_build_script(args.acd_version, ansible_base_version, package_dir)
+        write_python_build_files(args.acd_version, ansible_base_version, '',
+                                 package_dir, args.debian)
         if args.debian:
             write_debian_directory(args.acd_version, package_dir)
         make_dist(package_dir, args.dest_dir)
 
     deps_filename = os.path.join(args.dest_dir, args.deps_file)
     deps_file = DepsFile(deps_filename)
     deps_file.write(args.acd_version, ansible_base_version, included_versions)
@@ -222,14 +244,15 @@
 
         await asyncio.gather(*dist_creators)
 
 
 def build_multiple_command(args):
     build_file = BuildFile(args.build_file)
     build_acd_version, ansible_base_version, deps = build_file.parse()
+    ansible_base_version = PypiVer(ansible_base_version)
 
     if not str(args.acd_version).startswith(build_acd_version):
         print(f'{args.build_file} is for version {build_acd_version} but we need'
               f' {args.acd_version.major}.{args.acd_version.minor}')
         return 1
 
     with tempfile.TemporaryDirectory() as tmp_dir:
@@ -249,15 +272,17 @@
         os.mkdir(ansible_collections_dir, mode=0o700)
 
         # Construct the list of dependent collection packages
         collection_deps = []
         for collection, version in sorted(included_versions.items()):
             collection_deps.append(f"        '{collection}>={version},<{version.next_major()}'")
         collection_deps = '\n' + ',\n'.join(collection_deps)
-        write_python_build_files(args.acd_version, collection_deps, package_dir)
+        write_build_script(args.acd_version, ansible_base_version, package_dir)
+        write_python_build_files(args.acd_version, ansible_base_version,
+                                 collection_deps, package_dir)
 
         make_dist(package_dir, args.dest_dir)
 
     # Write the deps file
     deps_filename = os.path.join(args.dest_dir, args.deps_file)
     deps_file = DepsFile(deps_filename)
     deps_file.write(args.acd_version, ansible_base_version, included_versions)
```

### Comparing `antsibull-0.8.0/antsibull/build_collection.py` & `antsibull-0.9.0/antsibull/build_collection.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/cli/antsibull_build.py` & `antsibull-0.9.0/antsibull/cli/antsibull_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Entrypoint to the antsibull-build tool."""
 
 import argparse
 import os.path
 import sys
 from typing import List
 
-import packaging.version as pypiver
+from packaging.version import Version as PypiVer
 
 from ..new_acd import new_acd_command
 from ..build_collection import build_collection_command
 from ..build_acd_commands import build_single_command, build_multiple_command
 
 
 DEFAULT_FILE_BASE = 'acd'
@@ -92,15 +92,15 @@
 
     :arg program_name: The name of the program
     :arg args: A list of the command line arguments
     :returns: A :python:`argparse.Namespace`
     :raises InvalidArgumentError: Whenever there's something wrong with the arguments.
     """
     common_parser = argparse.ArgumentParser(add_help=False)
-    common_parser.add_argument('acd_version', type=pypiver.Version,
+    common_parser.add_argument('acd_version', type=PypiVer,
                                help='The X.Y.Z version of ACD that this will be for')
     common_parser.add_argument('--dest-dir', default='.',
                                help='Directory to write the output to')
 
     build_parser = argparse.ArgumentParser(add_help=False)
     build_parser.add_argument('--build-file', default=None,
                               help='File containing the list of collections with version ranges.'
```

### Comparing `antsibull-0.8.0/antsibull/cli/antsibull_docs.py` & `antsibull-0.9.0/antsibull/cli/antsibull_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/cli/antsibull_lint.py` & `antsibull-0.9.0/antsibull/cli/antsibull_lint.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/cli/doc_commands/current.py` & `antsibull-0.9.0/antsibull/cli/doc_commands/current.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/cli/doc_commands/stable.py` & `antsibull-0.9.0/antsibull/cli/doc_commands/stable.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,20 +103,24 @@
     # Note: loop through "doc" before any other keys.
     for field in ('doc', 'examples', 'return'):
         try:
             field_model = DOCS_SCHEMAS[plugin_type][field].parse_obj({field: plugin_info[field]})
         except ValidationError as e:
             if field == 'doc':
                 # We can't recover if there's not a doc field
-                raise
+                # pydantic exceptions are not picklable (probably due to bugs in the pickle module)
+                # so convert it to an exception type which is picklable
+                raise ValueError(str(e))
+
             # But we can use the default value (some variant of "empty") for everything else
-            # Note: We looped through doc first and raised an exception if doc did not normalize
+            # Note: We looped through doc first and returned an exception if doc did not normalize
             # so we're able to use it in the error message here.
             errors.append(f'Unable to normalize {new_info["doc"]["name"]}: {field}'
                           f' due to: {str(e)}')
+
             field_model = DOCS_SCHEMAS[plugin_type][field].parse_obj({})
 
         new_info.update(field_model.dict(by_alias=True))
 
     return (new_info, errors)
 
 
@@ -173,15 +177,15 @@
     return new_plugin_info, nonfatal_errors
 
 
 def get_collection_contents(plugin_info: t.Mapping[str, t.Mapping[str, t.Any]],
                             nonfatal_errors: PluginErrorsRT
                             ) -> t.DefaultDict[str, t.DefaultDict[str, t.Dict[str, str]]]:
     """
-    Return the contents plugins which are in each collection.
+    Return the plugins which are in each collection.
 
     :arg plugin_info: Mapping of plugin type to a mapping of plugin name to plugin record.
         The plugin_type, plugin_name, and short_description from plugin_records are used.
     :arg nonfatal_errors: mapping of plugin type to plugin name to list of error messages.
         The plugin_type and plugin_name are used.
     :returns: A Mapping of collection name to a mapping of plugin type to a mapping of plugin names
         to short_descriptions.
@@ -269,14 +273,18 @@
         """
         # Turn these into some sort of decorator that will load choose to dump or load the values
         # if a command line arg is specified.
         with open('dump_raw_plugin_info.json', 'w') as f:
             import json
             json.dump(plugin_info, f)
         flog.debug('Finished dumping raw plugin_info')
+
+        with open('dump_formatted_plugin_info.json', 'r') as f:
+            import json
+            plugin_info = json.load(f)
         """
 
         plugin_info, nonfatal_errors = asyncio_run(normalize_all_plugin_info(plugin_info))
         flog.debug('Finished normalizing data')
         augment_docs(plugin_info)
 
         """
```

### Comparing `antsibull-0.8.0/antsibull/collections.py` & `antsibull-0.9.0/antsibull/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/compat.py` & `antsibull-0.9.0/antsibull/compat.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/config.py` & `antsibull-0.9.0/antsibull/config.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/constants.py` & `antsibull-0.9.0/antsibull/constants.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/acd-setup_py.j2` & `antsibull-0.9.0/antsibull/data/acd-setup_py.j2`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         'Source Code': 'https://github.com/ansible/ansible',
     },
     license='GPLv3+',
     python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
     packages=['ansible_collections'],
     include_package_data=True,
     install_requires=[
-        'ansible-base>={{ version }},<{{ version.major }}.{{ version.minor + 1 }}',{{ collection_deps }}
+        'ansible-base>={{ ansible_base_version }},<{{ ansible_base_version.major }}.{{ ansible_base_version.minor + 1 }}',{{ collection_deps }}
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
```

### Comparing `antsibull-0.8.0/antsibull/data/collection-setup_py.j2` & `antsibull-0.9.0/antsibull/data/collection-setup_py.j2`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/debian/control` & `antsibull-0.9.0/antsibull/data/debian/control`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/debian/copyright` & `antsibull-0.9.0/antsibull/data/debian/copyright`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/debian/rules` & `antsibull-0.9.0/antsibull/data/debian/rules`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/docsite/plugin-deprecation.rst.j2` & `antsibull-0.9.0/antsibull/data/docsite/plugin-deprecation.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/docsite/plugin.rst.j2` & `antsibull-0.9.0/antsibull/data/docsite/plugin.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/docsite/plugins_by_collection.rst.j2` & `antsibull-0.9.0/antsibull/data/docsite/plugins_by_collection.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/galaxy_yml.j2` & `antsibull-0.9.0/antsibull/data/galaxy_yml.j2`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/data/gplv3.txt` & `antsibull-0.9.0/antsibull/data/gplv3.txt`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/dependency_files.py` & `antsibull-0.9.0/antsibull/dependency_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 When we initially build an ACD major release, we'll use certain versions of collections.
 We don't want to install backwards incompatible collections until the next major ACD release.
 """
 
 from typing import TYPE_CHECKING, Dict, List, Mapping, NamedTuple, Optional
 
 if TYPE_CHECKING:
-    from packaging.version import Version as PyPiVersion
-    from semantic_version import Version as SemVersion
+    from packaging.version import Version as PypiVer
+    from semantic_version import Version as SemVer
 
 
 class DependencyFileData(NamedTuple):
     ansible_version: str
     ansible_base_version: str
     deps: Dict[str, str]
 
@@ -132,16 +132,16 @@
     def __init__(self, build_file: str) -> None:
         self.filename: str = build_file
 
     def parse(self) -> DependencyFileData:
         """Parse the build from a dependency file."""
         return _parse_name_version_spec_file(self.filename)
 
-    def write(self, acd_version: 'PyPiVersion', ansible_base_version: str,
-              dependencies: Mapping[str, 'SemVersion']) -> None:
+    def write(self, acd_version: 'PypiVer', ansible_base_version: str,
+              dependencies: Mapping[str, 'SemVer']) -> None:
         """
         Write a build dependency file.
 
         A build dependency file records the collections that went into a given Ansible release along
         with the exact version of the collection that was included.
 
         :arg acd_version: The version of Ansible that is being recorded.
```

### Comparing `antsibull-0.8.0/antsibull/docs_parsing/ansible_doc.py` & `antsibull-0.9.0/antsibull/docs_parsing/ansible_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,20 +158,27 @@
     # We invoke _get_plugin_info once for each documentable plugin type.  Within _get_plugin_info,
     # new threads are spawned to handle waiting for ansible-doc to parse files and give us results.
     # To keep ourselves under THREAD_MAX, we need to divide the number of threads we're allowed over
     # each call of _get_plugin_info.
     # Why use THREAD_MAX instead of process max?  Even though this ultimately invokes separate
     # ansible-doc processes, the limiting factor is IO as ansible-doc reads from disk.  So it makes
     # sense to scale up to THREAD_MAX instead of PROCESS_MAX.
-    max_workers = int(THREAD_MAX / len(DOCUMENTABLE_PLUGINS))
-    if max_workers < 1:
-        max_workers = 1
+
+    # Allocate more for modules because the vast majority of plugins are modules
+    module_workers = max(int(.7 * THREAD_MAX), 1)
+    other_workers = int((THREAD_MAX - module_workers) / (len(DOCUMENTABLE_PLUGINS) - 1))
+    if other_workers < 1:
+        other_workers = 1
 
     extractors = {}
     for plugin_type in DOCUMENTABLE_PLUGINS:
+        if plugin_type == 'module':
+            max_workers = module_workers
+        else:
+            max_workers = other_workers
         extractors[plugin_type] = asyncio.create_task(
             _get_plugin_info(plugin_type, venv_ansible_doc, max_workers))
 
     results = await asyncio.gather(*extractors.values(), return_exceptions=True)
 
     plugin_map = {}
     err_msg = []
```

### Comparing `antsibull-0.8.0/antsibull/docs_parsing/fqcn.py` & `antsibull-0.9.0/antsibull/docs_parsing/fqcn.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/filesystem.py` & `antsibull-0.9.0/antsibull/filesystem.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/galaxy.py` & `antsibull-0.9.0/antsibull/galaxy.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/hashing.py` & `antsibull-0.9.0/antsibull/hashing.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/jinja2/environment.py` & `antsibull-0.9.0/antsibull/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/jinja2/filters.py` & `antsibull-0.9.0/antsibull/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/jinja2/tests.py` & `antsibull-0.9.0/antsibull/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/logging.py` & `antsibull-0.9.0/antsibull/logging.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/new_acd.py` & `antsibull-0.9.0/antsibull/new_acd.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 async def get_version_info(collections):
     loop = asyncio.get_running_loop()
     loop.set_exception_handler(display_exception)
 
     requestors = {}
     async with aiohttp.ClientSession() as aio_session:
-        async with asyncio_pool.AioPool(max_workers=THREAD_MAX) as pool:
+        async with asyncio_pool.AioPool(size=THREAD_MAX) as pool:
             pypi_client = AnsibleBasePyPiClient(aio_session)
             requestors['_ansible_base'] = await pool.spawn(pypi_client.get_versions())
             galaxy_client = GalaxyClient(aio_session)
 
             for collection in collections:
                 requestors[collection] = await pool.spawn(
                     galaxy_client.get_versions(collection))
```

### Comparing `antsibull-0.8.0/antsibull/schemas/ansible_doc.py` & `antsibull-0.9.0/antsibull/schemas/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/schemas/base.py` & `antsibull-0.9.0/antsibull/schemas/base.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/schemas/callback.py` & `antsibull-0.9.0/antsibull/schemas/callback.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/schemas/config.py` & `antsibull-0.9.0/antsibull/schemas/config.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/schemas/docs.py` & `antsibull-0.9.0/antsibull/schemas/docs.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/schemas/module.py` & `antsibull-0.9.0/antsibull/schemas/module.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/schemas/plugin.py` & `antsibull-0.9.0/antsibull/schemas/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/tarball.py` & `antsibull-0.9.0/antsibull/tarball.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/utils/collections.py` & `antsibull-0.9.0/antsibull/utils/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/vendored/collections.py` & `antsibull-0.9.0/antsibull/vendored/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/vendored/json_utils.py` & `antsibull-0.9.0/antsibull/vendored/json_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/venv.py` & `antsibull-0.9.0/antsibull/venv.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/antsibull/write_docs.py` & `antsibull-0.9.0/antsibull/write_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/pyproject.toml` & `antsibull-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "antsibull"
-version = "0.8.0"
+version = "0.9.0"
 description = "Tools for building the Ansible Distribution"
 authors = ["Toshio Kuratomi <a.badger@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/ansible-community/antsibull"
 packages = [
     { include = "antsibull" },
```

### Comparing `antsibull-0.8.0/tests/aiohttp_utils.py` & `antsibull-0.9.0/tests/aiohttp_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/certificate_utils.py` & `antsibull-0.9.0/tests/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_become.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_become.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_become_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_become_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_cache.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_cache.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_cache_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_cache_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_callback.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_callback.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_callback_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_callback_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_cliconf.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_cliconf.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_cliconf_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_cliconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_connection.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_connection_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_httpapi.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_httpapi.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_httpapi_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_httpapi_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_inventory.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_inventory.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_inventory_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_inventory_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_lookup.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_lookup.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_lookup_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_lookup_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_module.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_module.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_module_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_module_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_netconf.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_netconf.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_netconf_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_netconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_shell.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_shell.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_shell_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_shell_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_strategy.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_strategy.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_strategy_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_strategy_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_vars.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_vars.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/good_data/one_vars_results.json` & `antsibull-0.9.0/tests/functional/schema/good_data/one_vars_results.json`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/functional/schema/test_schema.py` & `antsibull-0.9.0/tests/functional/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/test_galaxy.py` & `antsibull-0.9.0/tests/test_galaxy.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/tests/units/test_parse_pieces.py` & `antsibull-0.9.0/tests/units/test_parse_pieces.py`

 * *Files identical despite different names*

### Comparing `antsibull-0.8.0/setup.py` & `antsibull-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 entry_points = \
 {'console_scripts': ['antsibull-build = antsibull.cli.antsibull_build:main',
                      'antsibull-docs = antsibull.cli.antsibull_docs:main',
                      'antsibull-lint = antsibull.cli.antsibull_lint:main']}
 
 setup_kwargs = {
     'name': 'antsibull',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Tools for building the Ansible Distribution',
     'long_description': "# antsibull -- Ansible Build Scripts\nTooling for building various things related to Ansible\n\nScripts that are here:\n\n* antsibull-build - Builds Ansible-2.10+ from component collections ([docs](docs/build-ansible.rst))\n* antsibull-docs - Extracts documentation from ansible plugins\n* antsibull-lint - Right now only validates ``changelogs/changelog.yaml`` files ([docs](docs/changelog.yaml-format.md))\n\nA related project is [antsibull-changelog](https://pypi.org/project/antsibull-changelog/), which is in its [own repository](https://github.com/ansible-community/antsibull-changelog/).\n\nScripts are created by poetry at build time.  So if you want to run from\na checkout, you'll have to run them under poetry::\n\n    python3 -m pip install poetry\n    poetry install  # Installs dependencies into a virtualenv\n    poetry run antsibull-build --help\n\nIf you want to create a new release::\n\n    poetry build\n    poetry publish  # Uploads to pypi.  Be sure you really want to do this\n\n.. note:: When installing a package published by poetry, it is best to use\n    pip >= 19.0.  Installing with pip-18.1 and below could create scripts which\n    use pkg_resources which can slow down startup time (in some environments by\n    quite a large amount).\n\nUnless otherwise noted in the code, it is licensed under the terms of the GNU\nGeneral Public License v3 or, at your option, later.\n",
     'author': 'Toshio Kuratomi',
     'author_email': 'a.badger@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ansible-community/antsibull',
```

### Comparing `antsibull-0.8.0/PKG-INFO` & `antsibull-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antsibull
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools for building the Ansible Distribution
 Home-page: https://github.com/ansible-community/antsibull
 License: GPL-3.0-or-later
 Author: Toshio Kuratomi
 Author-email: a.badger@gmail.com
 Requires-Python: >=3.6.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

