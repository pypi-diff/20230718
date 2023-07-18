# Comparing `tmp/oenv2config-1.2.1.tar.gz` & `tmp/oenv2config-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oenv2config-1.2.1.tar", last modified: Thu Jul  6 14:48:07 2023, max compression
+gzip compressed data, was "oenv2config-1.3.0.tar", last modified: Tue Jul 18 09:04:14 2023, max compression
```

## Comparing `oenv2config-1.2.1.tar` & `oenv2config-1.3.0.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.605159 oenv2config-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1885 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.577159 oenv2config-1.2.1/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.idea/oenv2config.iml
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-06 13:22:33.000000 oenv2config-1.2.1/.idea/ruff.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.577159 oenv2config-1.2.1/.idea/runConfigurations/
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.idea/runConfigurations/Python_tests__no_Odoo_.xml
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-07-06 13:22:33.000000 oenv2config-1.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/.ruff
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-06 14:48:07.605159 oenv2config-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-26 12:10:44.000000 oenv2config-1.2.1/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.581159 oenv2config-1.2.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.581159 oenv2config-1.2.1/docs/mkdocs/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/cli.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/db_options.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/entry.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/index.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/mappers.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/options.md
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/reference.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/mkdocs/utils.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.569159 oenv2config-1.2.1/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.581159 oenv2config-1.2.1/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.581159 oenv2config-1.2.1/docs/modules/ROOT/images/
--rw-rw-rw-   0 root         (0) root         (0)    44111 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/images/run_odoo_test.png
--rw-rw-rw-   0 root         (0) root         (0)    35877 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/images/run_test.png
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.585159 oenv2config-1.2.1/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/pages/antora.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/pages/contribute.adoc
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/pages/mkdocs.adoc
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/pages/tests.adoc
--rw-rw-rw-   0 root         (0) root         (0)     1878 2023-06-26 12:10:44.000000 oenv2config-1.2.1/docs/modules/ROOT/pages/tests_odoo.adoc
--rwxrwxrwx   0 root         (0) root         (0)      320 2023-06-26 12:10:44.000000 oenv2config-1.2.1/in_docker_test.sh
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-26 12:10:44.000000 oenv2config-1.2.1/mkdocs-plugins.txt
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-06-26 12:10:44.000000 oenv2config-1.2.1/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-07-06 13:22:33.000000 oenv2config-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:48:07.605159 oenv2config-1.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-06-26 12:10:44.000000 oenv2config-1.2.1/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.573159 oenv2config-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.589159 oenv2config-1.2.1/src/odoo_env_config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-07-06 14:48:07.000000 oenv2config-1.2.1/src/odoo_env_config/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4656 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/api.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-07-06 14:37:27.000000 oenv2config-1.2.1/src/odoo_env_config/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3782 2023-07-06 13:22:33.000000 oenv2config-1.2.1/src/odoo_env_config/entry.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4853 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/mappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.569159 oenv2config-1.2.1/src/odoo_env_config/odoo_modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.589159 oenv2config-1.2.1/src/odoo_env_config/odoo_modules/env2config/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/odoo_modules/env2config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.589159 oenv2config-1.2.1/src/odoo_env_config/odoo_modules/env2config/cli/
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-06 13:22:33.000000 oenv2config-1.2.1/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.593159 oenv2config-1.2.1/src/odoo_env_config/section/
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-06 13:22:33.000000 oenv2config-1.2.1/src/odoo_env_config/section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/db_section.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2155 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/log_section.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/s3_section.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/test_section.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/section/worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)    10125 2023-06-26 12:10:44.000000 oenv2config-1.2.1/src/odoo_env_config/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.593159 oenv2config-1.2.1/src/oenv2config.egg-info/
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-06 14:48:07.000000 oenv2config-1.2.1/src/oenv2config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3300 2023-07-06 14:48:07.000000 oenv2config-1.2.1/src/oenv2config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:48:07.000000 oenv2config-1.2.1/src/oenv2config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-06 14:48:07.000000 oenv2config-1.2.1/src/oenv2config.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-06 14:48:07.000000 oenv2config-1.2.1/src/oenv2config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 14:48:07.000000 oenv2config-1.2.1/src/oenv2config.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.597159 oenv2config-1.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-07-06 13:22:33.000000 oenv2config-1.2.1/tests/_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5458 2023-07-06 13:22:33.000000 oenv2config-1.2.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_doctests.py
--rw-rw-rw-   0 root         (0) root         (0)     4524 2023-07-06 13:22:33.000000 oenv2config-1.2.1/tests/test_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_libs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.597159 oenv2config-1.2.1/tests/test_mapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_mapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9833 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_mapper/test_mapper_clever_cloud_cellar.py
--rw-rw-rw-   0 root         (0) root         (0)    10835 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_mapper/test_mapper_clever_cloud_postgres.py
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_mapper/test_mapper_odoo_compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_mapper/test_mapper_queue_job.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_mapper/test_mapper_redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.601159 oenv2config-1.2.1/tests/test_section/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     7581 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_db_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     5567 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_log_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_s3_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_test_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     6727 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_section/test_worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.601159 oenv2config-1.2.1/tests/tests_odoo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/tests_odoo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-07-06 13:22:33.000000 oenv2config-1.2.1/tests/tests_odoo/_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:48:07.605159 oenv2config-1.2.1/tests/tests_odoo/profiles/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/tests_odoo/profiles/filestore_s3.env
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/tests_odoo/profiles/filestore_s3_cellar.env
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/tests_odoo/profiles/test_db_clever.env
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-26 12:10:44.000000 oenv2config-1.2.1/tests/tests_odoo/profiles/test_db_clever_direct.env
--rw-rw-rw-   0 root         (0) root         (0)     4117 2023-07-06 13:22:33.000000 oenv2config-1.2.1/tests/tests_odoo/test_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.655676 oenv2config-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.635676 oenv2config-1.3.0/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/oenv2config.iml
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/ruff.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.635676 oenv2config-1.3.0/.idea/runConfigurations/
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/.ruff
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-18 09:04:14.655676 oenv2config-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-07-18 06:34:40.000000 oenv2config-1.3.0/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.635676 oenv2config-1.3.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.639676 oenv2config-1.3.0/docs/mkdocs/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/cli.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/db_options.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/entry.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/mappers.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/options.md
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/reference.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/mkdocs/utils.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.631676 oenv2config-1.3.0/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.639676 oenv2config-1.3.0/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.639676 oenv2config-1.3.0/docs/modules/ROOT/images/
+-rw-rw-rw-   0 root         (0) root         (0)    44111 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/images/run_odoo_test.png
+-rw-rw-rw-   0 root         (0) root         (0)    35877 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/images/run_test.png
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.639676 oenv2config-1.3.0/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/pages/antora.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/pages/contribute.adoc
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/pages/mkdocs.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/pages/tests.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-18 06:34:40.000000 oenv2config-1.3.0/docs/modules/ROOT/pages/tests_odoo.adoc
+-rwxrwxrwx   0 root         (0) root         (0)      313 2023-07-18 08:48:02.000000 oenv2config-1.3.0/in_docker_test.sh
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-18 06:34:40.000000 oenv2config-1.3.0/mkdocs-plugins.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-18 06:34:40.000000 oenv2config-1.3.0/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-07-18 06:34:40.000000 oenv2config-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 09:04:14.655676 oenv2config-1.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-07-18 06:34:40.000000 oenv2config-1.3.0/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.631676 oenv2config-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.643676 oenv2config-1.3.0/src/odoo_env_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-18 09:04:14.000000 oenv2config-1.3.0/src/odoo_env_config/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4940 2023-07-18 08:48:02.000000 oenv2config-1.3.0/src/odoo_env_config/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3782 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4853 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/mappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.631676 oenv2config-1.3.0/src/odoo_env_config/odoo_modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.643676 oenv2config-1.3.0/src/odoo_env_config/odoo_modules/env2config/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/odoo_modules/env2config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.643676 oenv2config-1.3.0/src/odoo_env_config/odoo_modules/env2config/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.647676 oenv2config-1.3.0/src/odoo_env_config/section/
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2155 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-07-18 08:50:10.000000 oenv2config-1.3.0/src/odoo_env_config/section/misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/s3_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/section/worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)    11802 2023-07-18 06:34:40.000000 oenv2config-1.3.0/src/odoo_env_config/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.647676 oenv2config-1.3.0/src/oenv2config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-18 09:04:14.000000 oenv2config-1.3.0/src/oenv2config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-07-18 09:04:14.000000 oenv2config-1.3.0/src/oenv2config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 09:04:14.000000 oenv2config-1.3.0/src/oenv2config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-18 09:04:14.000000 oenv2config-1.3.0/src/oenv2config.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-18 09:04:14.000000 oenv2config-1.3.0/src/oenv2config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 09:04:14.000000 oenv2config-1.3.0/src/oenv2config.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.647676 oenv2config-1.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_doctests.py
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_libs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.651676 oenv2config-1.3.0/tests/test_mapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_mapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9833 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py
+-rw-rw-rw-   0 root         (0) root         (0)    10835 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py
+-rw-rw-rw-   0 root         (0) root         (0)     6535 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_mapper/test_mapper_odoo_compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_mapper/test_mapper_queue_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_mapper/test_mapper_redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.651676 oenv2config-1.3.0/tests/test_section/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     7581 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     5567 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_s3_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     6727 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_section/test_worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.655676 oenv2config-1.3.0/tests/tests_odoo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/tests_odoo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/tests_odoo/_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:04:14.655676 oenv2config-1.3.0/tests/tests_odoo/profiles/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/tests_odoo/profiles/filestore_s3.env
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/tests_odoo/profiles/filestore_s3_cellar.env
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/tests_odoo/profiles/runbot_classic_before.env
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/tests_odoo/profiles/test_db_clever.env
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-18 06:34:40.000000 oenv2config-1.3.0/tests/tests_odoo/profiles/test_db_clever_direct.env
+-rw-rw-rw-   0 root         (0) root         (0)     4999 2023-07-18 08:48:02.000000 oenv2config-1.3.0/tests/tests_odoo/test_base.py
```

### Comparing `oenv2config-1.2.1/.gitignore` & `oenv2config-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/.gitlab-ci.yml` & `oenv2config-1.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/.idea/oenv2config.iml` & `oenv2config-1.3.0/.idea/oenv2config.iml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/.idea/runConfigurations/Python_tests__no_Odoo_.xml` & `oenv2config-1.3.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/.idea/runConfigurations/Python_tests_in_tests_odoo.xml` & `oenv2config-1.3.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/README.adoc` & `oenv2config-1.3.0/README.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/docs/modules/ROOT/images/run_odoo_test.png` & `oenv2config-1.3.0/docs/modules/ROOT/images/run_odoo_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/docs/modules/ROOT/images/run_test.png` & `oenv2config-1.3.0/docs/modules/ROOT/images/run_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/docs/modules/ROOT/pages/tests.adoc` & `oenv2config-1.3.0/docs/modules/ROOT/pages/tests.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/docs/modules/ROOT/pages/tests_odoo.adoc` & `oenv2config-1.3.0/docs/modules/ROOT/pages/tests_odoo.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/mkdocs.yml` & `oenv2config-1.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/pyproject.toml` & `oenv2config-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/api.py` & `oenv2config-1.3.0/src/odoo_env_config/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,16 +95,21 @@
 
     def get_enum(self, key: str, enum_type: Type[ET], *, default: ET) -> ET:
         value = self.get(key)
         if not value or value not in enum_type.__members__:
             return default
         return enum_type[value]
 
+    def is_boolean(self, *keys: str) -> bool:
+        return utils.is_boolean(self.gets(*keys))
+
     def get_list(self, key: str, separator=",", allow_duplicate: bool = False) -> List[str]:
         value = self.get(key)
+        if self.is_boolean(key) and not self.get_bool(key):
+            return []
         if not value:
             return []
         if allow_duplicate:
             return [u.strip() for u in value.strip().split(separator)]
         res = OrderedDict()
         for value in value.strip().split(separator):
             res[value.strip()] = None
```

### Comparing `oenv2config-1.2.1/src/odoo_env_config/cli.py` & `oenv2config-1.3.0/src/odoo_env_config/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,17 @@
         sub_args = [s for s in sub_args if s.split()]
         odoo_config = self.odoo_module.tools.config
         odoo_config.config_file = ns.config_dest
         extra_env = _load_profiles(ns.profiles)
         env_args = entry.env_to_odoo_args(extra_env)
         odoo_config._parse_config(env_args)
         odoo_config._parse_config(sub_args)
+        admin_passwd = entry.env_to_section(entry.MiscSection, extra_env).admin_password
+        if admin_passwd:
+            odoo_config.set_admin_password(admin_passwd)
         odoo_config.save()
 
 
 def _load_profiles(profiles: List[str]) -> api.Env:
     extra_env = api.Env()
     for profile in profiles:
         path_profile = os.path.abspath(os.path.expanduser(profile))
```

### Comparing `oenv2config-1.2.1/src/odoo_env_config/entry.py` & `oenv2config-1.3.0/src/odoo_env_config/entry.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/mappers.py` & `oenv2config-1.3.0/src/odoo_env_config/mappers.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/odoo_modules/env2config/__manifest__.py` & `oenv2config-1.3.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/__init__.py` & `oenv2config-1.3.0/src/odoo_env_config/section/__init__.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/addons_path_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/addons_path_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/db_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/db_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/http_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/http_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/limit_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/limit_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/log_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/log_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/s3_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/s3_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/test_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/test_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/update_init_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/update_init_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/widemodule_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/widemodule_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/section/worker_section.py` & `oenv2config-1.3.0/src/odoo_env_config/section/worker_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/src/odoo_env_config/utils.py` & `oenv2config-1.3.0/src/odoo_env_config/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import warnings
 from collections import OrderedDict
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Set, Union
+
+BOOL_ACCEPTED_VALUE: Set[str] = {str(1), str(0), str(True), str(False), "Yes", "No"}
+BOOL_ACCEPTED_VALUE |= {a[0] for a in BOOL_ACCEPTED_VALUE}
+BOOL_ACCEPTED_VALUE |= {a.lower() for a in BOOL_ACCEPTED_VALUE}
 
 
 def to_bool(anything: Union[Any, None]) -> bool:
     """
     Convert `anything` to a [bool][bool] according to [os.environ][os.environ] most found _True_ value.
     Args:
         anything: The value to convert
@@ -41,14 +45,50 @@
         bool(anything)
         and (str(anything).isdigit() and bool(int(anything)))
         or (str(anything).capitalize() == str(True))
         or False
     )
 
 
+def is_boolean(anything: Union[Any, None]) -> bool:
+    """
+    Return `True` if the value is a boolean value.
+    Args:
+        anything: The value to test
+    Returns:
+        `True` if `anything` can be considered as a boolean value
+    Notes:
+        If the value is a string, then this is case **insensitive**
+    Examples:
+        >>> is_boolean("") or is_boolean(" ") is_boolean(None)
+        False
+        >>> is_boolean("True") and is_boolean("true") and is_boolean("TrUe") and is_boolean("TRUE")
+        True
+        >>> is_boolean("False") and is_boolean("false") and is_boolean("FalSe") and is_boolean("FALSE")
+        True
+        >>> is_boolean("Yes") and is_boolean("Y") and is_boolean("y") and is_boolean("yes") and is_boolean("yES")
+        True
+        >>> is_boolean("No") and is_boolean("NO") and is_boolean("no") and is_boolean("n") and is_boolean("N")
+        True
+        >>> is_boolean("T") and is_boolean("t") and is_boolean("F") and is_boolean("F")
+        True
+        >>> is_boolean(1) and is_boolean(1) and is_boolean(0) and is_boolean("1") and is_boolean("0")
+        True
+        >>> is_boolean(2) or is_boolean(-1)
+        False
+        >>> is_boolean("Vrai") or is_boolean("Faux") or is_boolean("FauX") or is_boolean("VRai")
+        False
+        >>> is_boolean("V") or is_boolean("v")
+        False
+        >>> is_boolean(True) and is_boolean(False)
+        True
+    """
+    return str(anything).lower() in BOOL_ACCEPTED_VALUE
+
+
 def is_true(anything: Union[Any, None]) -> bool:
     """
     Deprecated, the name is confusing, with the new function `is_bool`
      Args:
         anything: The value to convert
     Returns:
         `True` if `anything` in `True`, `"True"` `"1"`  otherwise `False`
```

### Comparing `oenv2config-1.2.1/src/oenv2config.egg-info/SOURCES.txt` & `oenv2config-1.3.0/src/oenv2config.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -91,9 +91,10 @@
 tests/test_section/test_widemodule_section.py
 tests/test_section/test_worker_section.py
 tests/tests_odoo/__init__.py
 tests/tests_odoo/_helpers.py
 tests/tests_odoo/test_base.py
 tests/tests_odoo/profiles/filestore_s3.env
 tests/tests_odoo/profiles/filestore_s3_cellar.env
+tests/tests_odoo/profiles/runbot_classic_before.env
 tests/tests_odoo/profiles/test_db_clever.env
 tests/tests_odoo/profiles/test_db_clever_direct.env
```

### Comparing `oenv2config-1.2.1/tests/_decorators.py` & `oenv2config-1.3.0/tests/_decorators.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_cli.py` & `oenv2config-1.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_entry.py` & `oenv2config-1.3.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_libs.py` & `oenv2config-1.3.0/tests/test_libs.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_mapper/test_mapper_clever_cloud_cellar.py` & `oenv2config-1.3.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_mapper/test_mapper_clever_cloud_postgres.py` & `oenv2config-1.3.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_mapper/test_mapper_odoo_compatibility.py` & `oenv2config-1.3.0/tests/test_mapper/test_mapper_odoo_compatibility.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_mapper/test_mapper_queue_job.py` & `oenv2config-1.3.0/tests/test_mapper/test_mapper_queue_job.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_mapper/test_mapper_redis.py` & `oenv2config-1.3.0/tests/test_mapper/test_mapper_redis.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_addons_path_section.py` & `oenv2config-1.3.0/tests/test_section/test_addons_path_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_db_section.py` & `oenv2config-1.3.0/tests/test_section/test_db_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_http_section.py` & `oenv2config-1.3.0/tests/test_section/test_http_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_limit_section.py` & `oenv2config-1.3.0/tests/test_section/test_limit_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_log_section.py` & `oenv2config-1.3.0/tests/test_section/test_log_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_misc_section.py` & `oenv2config-1.3.0/tests/test_section/test_s3_section.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 import unittest
 
 from odoo_env_config.api import Env
-from odoo_env_config.section import MiscSection
+from odoo_env_config.section import S3Section
 
 
-class TestMiscSection(unittest.TestCase):
+class TestLogSection(unittest.TestCase):
     def test_default(self):
-        conf = MiscSection()
-        self.assertFalse(conf.unaccent)
-        self.assertEqual([], conf.without_demo)
-        self.assertFalse(conf.stop_after_init)
-        self.assertFalse(conf.save_config_file)
+        conf = S3Section()
+        self.assertFalse(conf.access_key)
+        self.assertFalse(conf.secret)
+        self.assertFalse(conf.region)
+        self.assertFalse(conf.host)
+        self.assertFalse(conf.bucket_name)
+
+    def test_values(self):
+        conf = S3Section().init(
+            Env(
+                {
+                    "S3_FILESTORE_ACCESS_KEY": "s3_access_value",
+                    "S3_FILESTORE_SECRET_KEY": "s3_secret_value",
+                    "S3_FILESTORE_BUCKET": "s3_bucket_value",
+                    "S3_FILESTORE_HOST": "s3_host_value",
+                    "S3_FILESTORE_REGION": "s3_region_value",
+                }
+            )
+        )
+        self.assertEqual("s3_access_value", conf.access_key)
+        self.assertEqual("s3_secret_value", conf.secret)
+        self.assertEqual("s3_bucket_value", conf.bucket_name)
+        self.assertEqual("s3_host_value", conf.host)
+        self.assertEqual("s3_region_value", conf.region)
 
         flags = conf.to_values()
         self.assertFalse(flags)
 
-    def test_global(self):
-        conf = MiscSection().init(
+    def test_subdir(self):
+        conf = S3Section().init(
             Env(
                 {
-                    "UNACCENT": str(True),
-                    "WITHOUT_DEMO": "all,account",
-                    "STOP_AFTER_INIT": str(True),
-                    "SAVE_CONFIG_FILE": str(True),
+                    "S3_FILESTORE_ACCESS_KEY": "s3_access_value",
+                    "S3_FILESTORE_SECRET_KEY": "s3_secret_value",
+                    "S3_FILESTORE_BUCKET": "s3_bucket_value",
+                    "S3_FILESTORE_HOST": "s3_host_value",
+                    "S3_FILESTORE_SUB_DIR": "S3_db_name",
                 }
             )
         )
-        self.assertTrue(conf.unaccent)
-        self.assertListEqual(["all", "account"], conf.without_demo)
-        self.assertTrue(conf.stop_after_init)
-        self.assertTrue(conf.save_config_file)
+        self.assertEqual("s3_access_value", conf.access_key)
+        self.assertEqual("s3_secret_value", conf.secret)
+        self.assertEqual("s3_bucket_value", conf.bucket_name)
+        self.assertEqual("s3_host_value", conf.host)
+        self.assertFalse(conf.region)
+        self.assertEqual("S3_db_name", conf.sub_dir)
 
         flags = conf.to_values()
-        self.assertIn("unaccent", flags)
-        self.assertTrue(flags["unaccent"])
-
-        self.assertIn("without-demo", flags)
-        self.assertEqual("all,account", flags["without-demo"])
-
-        self.assertIn("save", flags)
-        self.assertTrue(flags["save"])
-
-        self.assertIn("stop-after-init", flags)
-        self.assertTrue(flags["stop-after-init"])
+        self.assertFalse(flags)
```

### Comparing `oenv2config-1.2.1/tests/test_section/test_test_section.py` & `oenv2config-1.3.0/tests/test_section/test_test_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_update_init_section.py` & `oenv2config-1.3.0/tests/test_section/test_update_init_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_widemodule_section.py` & `oenv2config-1.3.0/tests/test_section/test_widemodule_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_section/test_worker_section.py` & `oenv2config-1.3.0/tests/test_section/test_worker_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/test_utils.py` & `oenv2config-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/tests_odoo/_helpers.py` & `oenv2config-1.3.0/tests/tests_odoo/_helpers.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.2.1/tests/tests_odoo/test_base.py` & `oenv2config-1.3.0/tests/tests_odoo/test_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,14 +105,37 @@
                 "db_sslmode": "prefer",
                 "db_template": "template0",
                 "db_user": "my_db_user_direct",
                 "dbfilter": "",
             },
         )
 
+    def test_runbot_classic_config(self):
+        parser = create_config(["runbot_classic_before"])
+        assertParser(
+            self,
+            parser,
+            {
+                "db_host": "database",
+                "db_maxconn": 64,
+                "db_name": "databasehbkw",
+                "db_password": "ltniqmdrwo",
+                "db_port": 5432,
+                "db_sslmode": "prefer",
+                "db_template": "template0",
+                "db_user": "ddjwl",
+                "log_level": "debug",
+                "without_demo": "False",
+                "test_enable": "False",
+            },
+        )
+        self.assertNotEqual("admin", parser.get("options", "admin_passwd"))
+        self.assertTrue(parser.get("options", "admin_passwd").startswith("$pbkdf2-sha512$25000$"))
+        self.assertEqual(len(parser.get("options", "admin_passwd")), 130)
+
     def test_filestore(self):
         """
         Assert module `odoo_filestore_s3` is enable.
         Returns:
 
         """
         parser = create_config(["filestore_s3"])
```

