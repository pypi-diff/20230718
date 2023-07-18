# Comparing `tmp/repod-0.2.2.tar.gz` & `tmp/repod-0.3.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repod-0.2.2.tar", max compression
+gzip compressed data, was "repod-0.3.0.post0.tar", last modified: Tue Jul 18 07:14:35 2023, max compression
```

## Comparing `repod-0.2.2.tar` & `repod-0.3.0.post0.tar`

### file list

```diff
@@ -1,78 +1,96 @@
--rw-r--r--   0        0        0    35149 2022-08-29 20:41:00.315138 repod-0.2.2/LICENSE
--rw-r--r--   0        0        0     2234 2022-08-29 20:41:00.315138 repod-0.2.2/README.md
--rw-r--r--   0        0        0    22964 2022-08-29 20:41:00.315138 repod-0.2.2/docs/LICENSE
--rw-r--r--   0        0        0      634 2022-08-29 20:41:00.315138 repod-0.2.2/docs/Makefile
--rw-r--r--   0        0        0     2546 2022-08-29 20:41:00.318472 repod-0.2.2/docs/conf.py
--rw-r--r--   0        0        0     1241 2022-08-29 20:41:00.318472 repod-0.2.2/docs/index.rst
--rw-r--r--   0        0        0     4107 2022-08-29 20:41:00.318472 repod-0.2.2/docs/packages/contents.rst
--rw-r--r--   0        0        0     1164 2022-08-29 20:41:00.318472 repod-0.2.2/docs/packages/signatures.rst
--rw-r--r--   0        0        0     6126 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repod/changelog.rst
--rw-r--r--   0        0        0     2112 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repod/installation.rst
--rw-r--r--   0        0        0       84 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repod/man/index.rst
--rw-r--r--   0        0        0    12041 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repod/man/repod_conf.rst
--rw-r--r--   0        0        0     2421 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repod/man/repod_file.rst
--rw-r--r--   0        0        0     2119 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repositories/binary_repository.rst
--rw-r--r--   0        0        0     5101 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repositories/management_repository.rst
--rw-r--r--   0        0        0     1437 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repositories/source_repository.rst
--rw-r--r--   0        0        0     1077 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repositories/source_tarball_repository.rst
--rw-r--r--   0        0        0     8834 2022-08-29 20:41:00.318472 repod-0.2.2/docs/repositories/sync_database.rst
--rw-r--r--   0        0        0        0 2022-08-29 20:41:00.345139 repod-0.2.2/docs/schema/.gitkeep
--rw-r--r--   0        0        0     1016 2022-08-29 20:41:00.318472 repod-0.2.2/justfile
--rw-r--r--   0        0        0     3945 2022-08-29 20:41:00.318472 repod-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      471 2022-08-29 20:41:00.318472 repod-0.2.2/repod/__init__.py
--rw-r--r--   0        0        0       51 2022-08-29 20:41:00.318472 repod-0.2.2/repod/cli/__init__.py
--rw-r--r--   0        0        0    11339 2022-08-29 20:41:00.318472 repod-0.2.2/repod/cli/argparse.py
--rw-r--r--   0        0        0    13738 2022-08-29 20:41:00.318472 repod-0.2.2/repod/cli/cli.py
--rw-r--r--   0        0        0     2321 2022-08-29 20:41:00.318472 repod-0.2.2/repod/commands.py
--rw-r--r--   0        0        0     7741 2022-08-29 20:41:00.318472 repod-0.2.2/repod/common/enums.py
--rw-r--r--   0        0        0    16719 2022-08-29 20:41:00.318472 repod-0.2.2/repod/common/models.py
--rw-r--r--   0        0        0     1289 2022-08-29 20:41:00.318472 repod-0.2.2/repod/common/regex.py
--rw-r--r--   0        0        0       77 2022-08-29 20:41:00.318472 repod-0.2.2/repod/config/__init__.py
--rw-r--r--   0        0        0     1477 2022-08-29 20:41:00.318472 repod-0.2.2/repod/config/defaults.py
--rw-r--r--   0        0        0    72384 2022-08-29 20:41:00.318472 repod-0.2.2/repod/config/settings.py
--rw-r--r--   0        0        0      571 2022-08-29 20:41:00.318472 repod-0.2.2/repod/errors.py
--rw-r--r--   0        0        0     1069 2022-08-29 20:41:00.318472 repod-0.2.2/repod/files/__init__.py
--rw-r--r--   0        0        0    13555 2022-08-29 20:41:00.318472 repod-0.2.2/repod/files/buildinfo.py
--rw-r--r--   0        0        0     8071 2022-08-29 20:41:00.318472 repod-0.2.2/repod/files/common.py
--rw-r--r--   0        0        0    13454 2022-08-29 20:41:00.321805 repod-0.2.2/repod/files/mtree.py
--rw-r--r--   0        0        0     6953 2022-08-29 20:41:00.321805 repod-0.2.2/repod/files/package.py
--rw-r--r--   0        0        0    15701 2022-08-29 20:41:00.321805 repod-0.2.2/repod/files/pkginfo.py
--rw-r--r--   0        0        0      975 2022-08-29 20:41:00.321805 repod-0.2.2/repod/repo/__init__.py
--rw-r--r--   0        0        0      177 2022-08-29 20:41:00.321805 repod-0.2.2/repod/repo/management/__init__.py
--rw-r--r--   0        0        0    35031 2022-08-29 20:41:00.321805 repod-0.2.2/repod/repo/management/outputpackage.py
--rw-r--r--   0        0        0      390 2022-08-29 20:41:00.321805 repod-0.2.2/repod/repo/package/__init__.py
--rw-r--r--   0        0        0    11234 2022-08-29 20:41:00.321805 repod-0.2.2/repod/repo/package/repofile.py
--rw-r--r--   0        0        0    48569 2022-08-29 20:41:00.321805 repod-0.2.2/repod/repo/package/syncdb.py
--rw-r--r--   0        0        0     1271 2022-08-29 20:41:00.321805 repod-0.2.2/repod/templates/desc_v1.j2
--rw-r--r--   0        0        0     1232 2022-08-29 20:41:00.321805 repod-0.2.2/repod/templates/desc_v2.j2
--rw-r--r--   0        0        0       84 2022-08-29 20:41:00.321805 repod-0.2.2/repod/templates/files_v1.j2
--rw-r--r--   0        0        0       67 2022-08-29 20:41:00.321805 repod-0.2.2/repod/verification/__init__.py
--rw-r--r--   0        0        0     1614 2022-08-29 20:41:00.321805 repod-0.2.2/repod/verification/pgp.py
--rw-r--r--   0        0        0        0 2022-08-29 20:41:00.345139 repod-0.2.2/repod/version/__init__.py
--rw-r--r--   0        0        0     5403 2022-08-29 20:41:00.321805 repod-0.2.2/repod/version/alpm.py
--rw-r--r--   0        0        0      584 2022-08-29 20:41:00.321805 repod-0.2.2/repod/version/util.py
--rw-r--r--   0        0        0        0 2022-08-29 20:41:00.345139 repod-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     2695 2022-08-29 20:41:00.321805 repod-0.2.2/tests/cli/test_argparse.py
--rw-r--r--   0        0        0    20722 2022-08-29 20:41:00.321805 repod-0.2.2/tests/cli/test_cli.py
--rw-r--r--   0        0        0     1459 2022-08-29 20:41:00.321805 repod-0.2.2/tests/common/test_enums.py
--rw-r--r--   0        0        0    10278 2022-08-29 20:41:00.321805 repod-0.2.2/tests/common/test_models.py
--rw-r--r--   0        0        0     4006 2022-08-29 20:41:00.321805 repod-0.2.2/tests/common/test_regex.py
--rw-r--r--   0        0        0    60879 2022-08-29 20:41:00.321805 repod-0.2.2/tests/config/test_settings.py
--rw-r--r--   0        0        0    46352 2022-08-29 20:41:00.321805 repod-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     7386 2022-08-29 20:41:00.321805 repod-0.2.2/tests/files/test_buildinfo.py
--rw-r--r--   0        0        0     5821 2022-08-29 20:41:00.321805 repod-0.2.2/tests/files/test_common.py
--rw-r--r--   0        0        0      143 2022-08-29 20:41:00.321805 repod-0.2.2/tests/files/test_files_init.py
--rw-r--r--   0        0        0    14282 2022-08-29 20:41:00.321805 repod-0.2.2/tests/files/test_mtree.py
--rw-r--r--   0        0        0     2178 2022-08-29 20:41:00.321805 repod-0.2.2/tests/files/test_package.py
--rw-r--r--   0        0        0     6097 2022-08-29 20:41:00.321805 repod-0.2.2/tests/files/test_pkginfo.py
--rw-r--r--   0        0        0    11176 2022-08-29 20:41:00.321805 repod-0.2.2/tests/repo/management/test_outputpackage.py
--rw-r--r--   0        0        0    10215 2022-08-29 20:41:00.321805 repod-0.2.2/tests/repo/package/test_repofile.py
--rw-r--r--   0        0        0    30932 2022-08-29 20:41:00.321805 repod-0.2.2/tests/repo/package/test_syncdb.py
--rw-r--r--   0        0        0      141 2022-08-29 20:41:00.321805 repod-0.2.2/tests/repo/test_repo_init.py
--rw-r--r--   0        0        0     1166 2022-08-29 20:41:00.321805 repod-0.2.2/tests/test_commands.py
--rw-r--r--   0        0        0      132 2022-08-29 20:41:00.321805 repod-0.2.2/tests/test_repod_init.py
--rw-r--r--   0        0        0     1982 2022-08-29 20:41:00.321805 repod-0.2.2/tests/verification/test_pgp.py
--rw-r--r--   0        0        0     2250 2022-08-29 20:41:00.321805 repod-0.2.2/tests/version/test_alpm.py
--rw-r--r--   0        0        0      561 2022-08-29 20:41:00.321805 repod-0.2.2/tests/version/test_util.py
--rw-r--r--   0        0        0     3693 2022-08-29 20:41:10.510909 repod-0.2.2/setup.py
--rw-r--r--   0        0        0     4248 2022-08-29 20:41:10.511187 repod-0.2.2/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-07-18 07:14:23.251012 repod-0.3.0.post0/AUTHORS.rst -> docs/authors.rst
+-rw-r--r--   0        0        0    35149 2023-07-18 07:14:23.251012 repod-0.3.0.post0/LICENSE
+-rw-r--r--   0        0        0    35149 2023-07-18 07:14:23.251012 repod-0.3.0.post0/LICENSE
+-rw-r--r--   0        0        0     1741 2023-07-18 07:14:23.251012 repod-0.3.0.post0/Makefile
+-rw-r--r--   0        0        0     1551 2023-07-18 07:14:23.251012 repod-0.3.0.post0/README.md
+-rw-r--r--   0        0        0    22964 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/LICENSE
+-rw-r--r--   0        0        0      634 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/Makefile
+-rw-r--r--   0        0        0    20138 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/LICENSE
+-rw-r--r--   0        0        0     4286 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/logo.ico
+-rw-r--r--   0        0        0    15160 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/logo.png
+-rw-r--r--   0        0        0     1509 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/repod.svg
+-rw-r--r--   0        0        0      484 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/authors.rst
+-rw-r--r--   0        0        0     2610 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/conf.py
+-rw-r--r--   0        0        0     4011 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/contributing.rst
+-rw-r--r--   0        0        0     1295 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/index.rst
+-rw-r--r--   0        0        0     4107 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/packages/contents.rst
+-rw-r--r--   0        0        0     1164 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/packages/signatures.rst
+-rw-r--r--   0        0        0    12784 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/changelog.rst
+-rw-r--r--   0        0        0     2000 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/installation.rst
+-rw-r--r--   0        0        0       84 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/man/index.rst
+-rw-r--r--   0        0        0    23153 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/man/repod_conf.rst
+-rw-r--r--   0        0        0     2421 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/man/repod_file.rst
+-rw-r--r--   0        0        0     5846 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/usage.rst
+-rw-r--r--   0        0        0     2119 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/binary_repository.rst
+-rw-r--r--   0        0        0     5101 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/management_repository.rst
+-rw-r--r--   0        0        0     3177 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/source_repository.rst
+-rw-r--r--   0        0        0     1077 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/source_tarball_repository.rst
+-rw-r--r--   0        0        0     8834 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/sync_database.rst
+-rw-r--r--   0        0        0     5027 2023-07-18 07:14:35.304535 repod-0.3.0.post0/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/__init__.py
+-rw-r--r--   0        0        0    31984 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/action/check.py
+-rw-r--r--   0        0        0    97335 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/action/task.py
+-rw-r--r--   0        0        0    12824 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/action/workflow.py
+-rw-r--r--   0        0        0     3154 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/archive/archive.py
+-rw-r--r--   0        0        0       81 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/cli/__init__.py
+-rw-r--r--   0        0        0    13334 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/cli/argparse.py
+-rw-r--r--   0        0        0     8472 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/cli/cli.py
+-rw-r--r--   0        0        0     2295 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/commands.py
+-rw-r--r--   0        0        0    11902 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/common/enums.py
+-rw-r--r--   0        0        0    18711 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/common/models.py
+-rw-r--r--   0        0        0     1397 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/common/regex.py
+-rw-r--r--   0        0        0      147 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/config/__init__.py
+-rw-r--r--   0        0        0     2213 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/config/defaults.py
+-rw-r--r--   0        0        0   105128 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/config/settings.py
+-rw-r--r--   0        0        0      845 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/errors.py
+-rw-r--r--   0        0        0     1269 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/__init__.py
+-rw-r--r--   0        0        0    14590 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/buildinfo.py
+-rw-r--r--   0        0        0     8789 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/common.py
+-rw-r--r--   0        0        0    14183 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/mtree.py
+-rw-r--r--   0        0        0     7319 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/package.py
+-rw-r--r--   0        0        0    15956 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/files/pkginfo.py
+-rw-r--r--   0        0        0    20922 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/files/srcinfo.py
+-rw-r--r--   0        0        0        0 2023-07-18 07:14:23.294346 repod-0.3.0.post0/repod/py.typed
+-rw-r--r--   0        0        0     1003 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/__init__.py
+-rw-r--r--   0        0        0      226 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/management/__init__.py
+-rw-r--r--   0        0        0    35361 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/management/outputpackage.py
+-rw-r--r--   0        0        0      943 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/package/__init__.py
+-rw-r--r--   0        0        0    13103 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/package/repofile.py
+-rw-r--r--   0        0        0    48850 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/package/syncdb.py
+-rw-r--r--   0        0        0     1271 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/templates/desc_v1.j2
+-rw-r--r--   0        0        0     1232 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/templates/desc_v2.j2
+-rw-r--r--   0        0        0       84 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/templates/files_v1.j2
+-rw-r--r--   0        0        0      113 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/verification/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/verification/pgp.py
+-rw-r--r--   0        0        0       47 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/version/__init__.py
+-rw-r--r--   0        0        0     5461 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/version/alpm.py
+-rw-r--r--   0        0        0      626 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/version/util.py
+-rw-r--r--   0        0        0       23 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/__init__.py
+-rw-r--r--   0        0        0    12495 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/action/test_check.py
+-rw-r--r--   0        0        0    85867 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/action/test_task.py
+-rw-r--r--   0        0        0     8604 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/action/test_workflow.py
+-rw-r--r--   0        0        0     3195 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/archive/test_archive.py
+-rw-r--r--   0        0        0     4414 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/cli/test_argparse.py
+-rw-r--r--   0        0        0    20655 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/cli/test_cli.py
+-rw-r--r--   0        0        0     3489 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/common/test_enums.py
+-rw-r--r--   0        0        0    11693 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/common/test_models.py
+-rw-r--r--   0        0        0     5473 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/common/test_regex.py
+-rw-r--r--   0        0        0   101383 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/config/test_settings.py
+-rw-r--r--   0        0        0    59495 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/conftest.py
+-rw-r--r--   0        0        0     8991 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_buildinfo.py
+-rw-r--r--   0        0        0     7166 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_common.py
+-rw-r--r--   0        0        0      220 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_files_init.py
+-rw-r--r--   0        0        0    16214 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_mtree.py
+-rw-r--r--   0        0        0     2480 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_package.py
+-rw-r--r--   0        0        0     6711 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_pkginfo.py
+-rw-r--r--   0        0        0     5094 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_srcinfo.py
+-rw-r--r--   0        0        0    11279 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/repo/management/test_outputpackage.py
+-rw-r--r--   0        0        0    13599 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/repo/package/test_repofile.py
+-rw-r--r--   0        0        0    33240 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/repo/package/test_syncdb.py
+-rw-r--r--   0        0        0      216 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/repo/test_repo_init.py
+-rw-r--r--   0        0        0     1248 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/test_commands.py
+-rw-r--r--   0        0        0      197 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/test_repod_init.py
+-rw-r--r--   0        0        0     2202 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/verification/test_pgp.py
+-rw-r--r--   0        0        0     2414 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/version/test_alpm.py
+-rw-r--r--   0        0        0      613 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/version/test_util.py
+-rw-r--r--   0        0        0     3630 1970-01-01 00:00:00.000000 repod-0.3.0.post0/PKG-INFO
```

### Comparing `repod-0.2.2/LICENSE` & `repod-0.3.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/LICENSE` & `repod-0.3.0.post0/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/Makefile` & `repod-0.3.0.post0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/conf.py` & `repod-0.3.0.post0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# This file only contains a selection of the most common options. For a full
-# list see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
+"""Configuration file for the Sphinx documentation builder.
+
+This file only contains a selection of the most common options. For a full
+list see the documentation:
+https://www.sphinx-doc.org/en/master/usage/configuration.html
+"""
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
@@ -18,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "repod"
 copyright = "2022, David Runge"
 author = "David Runge"
 
 # The full version, including alpha/beta/rc tags
-release = "0.1.0"
+release = "latest"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -52,14 +53,16 @@
 #
 html_theme = "sphinx_rtd_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
+html_logo = "artwork/logo.png"
+html_favicon = "artwork/logo.ico"
 
 html_context = {
     "display_gitlab": True,
     "gitlab_host": "gitlab.archlinux.org",
     "gitlab_user": "archlinux",
     "gitlab_repo": "repod",
     "gitlab_version": "main",
```

### Comparing `repod-0.2.2/docs/index.rst` & `repod-0.3.0.post0/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 
    Repod is still considered |alpha|. Aside from test and development setups it
    is strongly recommended to not use it in a production environment at this
    point!
 
 .. toctree::
    :maxdepth: 2
+   :caption: Using Repod
+
+   repod/installation.rst
+   repod/usage.rst
+   repod/man/index.rst
+   repod/changelog.rst
+   contributing.rst
+   authors.rst
+
+.. toctree::
+   :maxdepth: 2
    :caption: Repositories
 
    repositories/source_repository.rst
    repositories/source_tarball_repository.rst
    repositories/binary_repository.rst
    repositories/sync_database.rst
    repositories/management_repository.rst
@@ -26,22 +37,14 @@
 .. toctree::
    :maxdepth: 2
    :caption: Packages
 
    packages/contents.rst
    packages/signatures.rst
 
-.. toctree::
-   :maxdepth: 2
-   :caption: Using Repod
-
-   repod/installation.rst
-   repod/man/index.rst
-   repod/changelog.rst
-
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `repod-0.2.2/docs/packages/contents.rst` & `repod-0.3.0.post0/docs/packages/contents.rst`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/packages/signatures.rst` & `repod-0.3.0.post0/docs/packages/signatures.rst`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/repod/installation.rst` & `repod-0.3.0.post0/docs/repod/installation.rst`

 * *Files 25% similar despite different names*

```diff
@@ -15,16 +15,21 @@
 
 .. note::
 
   Installing a wheel distributable (e.g. via ``pip install``) does not create
   required directories for system-mode (see :ref:`repod.conf`), nor does it
   provide the man pages.
   Users requiring system-mode and downstream packagers should therefore use the
-  provided |justfile| for installation on a system level. Refer to ``just -l``
-  to learn more about the provided targets.
+  provided ``Makefile`` for installation on a system level.
+
+.. code:: sh
+
+  make build
+  make system-docs
+  make install
 
 Requirements
 ------------
 
 Installing repod automatically installs its dependencies as well.
 
 A few optional dependencies offer different functionality over the defaults.
@@ -41,28 +46,24 @@
 By default repod makes use of |python-magic| for file type detection. If
 ``file-magic`` (provided by |file|) is detected, it is used instead.
 
 Development environment
 -----------------------
 
 The repod project can be used from a git clone of the project, with the help of
-|poetry|.
+|pdm|.
 
 .. code:: sh
 
   git clone https://gitlab.archlinux.org/archlinux/repod/
   cd repod
-  poetry install
-
-Afterwards it is possible to make use of existing :ref:`tooling <manuals>` with the help
-of ``poetry run`` (e.g. ``poetry run repod-file --help``).
-
-.. |justfile| raw:: html
+  pdm install
 
-  <a target="blank" href="https://just.systems/man/en/">justfile</a>
+Afterwards it is possible to make use of existing :ref:`tooling <manuals>` with
+the help of ``pdm run`` (e.g. ``pdm run repod-file --help``).
 
 .. |vercmp| raw:: html
 
   <a target="blank" href="https://man.archlinux.org/man/vercmp.8">vercmp</a>
 
 .. |pyalpm| raw:: html
 
@@ -72,10 +73,10 @@
 
   <a target="blank" href="https://pypi.org/project/python-magic/">python-magic</a>
 
 .. |file| raw:: html
 
   <a target="blank" href="https://darwinsys.com/file/">file</a>
 
-.. |poetry| raw:: html
+.. |pdm| raw:: html
 
-  <a target="blank" href="https://python-poetry.org/">poetry</a>
+  <a target="blank" href="https://pdm.fming.dev/latest/">pdm</a>
```

### Comparing `repod-0.2.2/docs/repod/man/repod_file.rst` & `repod-0.3.0.post0/docs/repod/man/repod_file.rst`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/repositories/binary_repository.rst` & `repod-0.3.0.post0/docs/repositories/binary_repository.rst`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/repositories/management_repository.rst` & `repod-0.3.0.post0/docs/repositories/management_repository.rst`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/repositories/source_tarball_repository.rst` & `repod-0.3.0.post0/docs/repositories/source_tarball_repository.rst`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/docs/repositories/sync_database.rst` & `repod-0.3.0.post0/docs/repositories/sync_database.rst`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/repod/cli/argparse.py` & `repod-0.3.0.post0/repod/cli/argparse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,37 @@
+"""Argparser factory for repod's CLI."""
+from __future__ import annotations
+
 import os
 from argparse import ArgumentParser, ArgumentTypeError
 from pathlib import Path
 
+from pydantic import AnyUrl, TypeAdapter, ValidationError
+
 from repod.common.enums import ArchitectureEnum
 
 
 class ArgParseFactory:
-    """A factory class to create different types of ArgumentParser instances
+    """A factory class to create different types of ArgumentParser instances.
 
     Attributes
     ----------
     parser: ArgumentParser
         The instance's ArgumentParser instance, which is created with a default verbose argument
 
     """
 
     def __init__(self, description: str = "default") -> None:
+        """Initialize an instance of ArgParseFactory.
+
+        Parameters
+        ----------
+        description: str
+            The description string of the resulting self.parser (an ArgumentParser)
+        """
         self.parser = ArgumentParser(description=description)
         self.parser.add_argument(
             "-c",
             "--config",
             type=self.string_to_file_path,
             help="configuration file",
         )
@@ -42,22 +54,21 @@
             action="store_true",
             dest="verbose_mode",
             help="verbose output",
         )
 
     @classmethod
     def repod_file(cls) -> ArgumentParser:
-        """A class method to create an ArgumentParser for the repod-file script
+        """Create an ArgumentParser for the repod-file script.
 
         Returns
         -------
         ArgumentParser
             An ArgumentParser instance specific for the repod-file script
         """
-
         instance = cls(description="File actions for packages, management repository and sync databases.")
         subcommands = instance.parser.add_subparsers(dest="subcommand")
 
         package = subcommands.add_parser(name="package", help="interact with package files")
         package_subcommands = package.add_subparsers(dest="package")
 
         package_inspect_parser = package_subcommands.add_parser(name="inspect", help="inspect package files")
@@ -123,15 +134,15 @@
             "--testing",
             action="store_true",
             help="import to testing repository",
         )
 
         repo_importpkg_parser = repo_subcommands.add_parser(
             name="importpkg",
-            help="import packages of the same pkgbase to a repo",
+            help="import packages to a repo",
         )
         repo_importpkg_parser.add_argument(
             "file",
             nargs="+",
             type=cls.string_to_file_path,
             help="package files",
         )
@@ -160,14 +171,22 @@
         )
         repo_importpkg_parser.add_argument(
             "-s",
             "--with-signature",
             action="store_true",
             help="locate and use a signature file for each provided package file",
         )
+        repo_importpkg_parser.add_argument(
+            "-u",
+            "--source-url",
+            default=[],
+            nargs="+",
+            help="list of source URLs for added pkgbases (provided as one or more pkgbase=url strings)",
+            type=cls.string_to_tuple,
+        )
         mutual_exclusive_repo_importpkg = repo_importpkg_parser.add_mutually_exclusive_group()
         mutual_exclusive_repo_importpkg.add_argument(
             "-D",
             "--debug",
             action="store_true",
             help="import to debug repository",
         )
@@ -235,15 +254,15 @@
             help=("directory to which to write JSON files to"),
         )
 
         return instance.parser
 
     @classmethod
     def string_to_writable_file_path(cls, input_: str) -> Path:
-        """Convert an input string into a Path to a file
+        """Convert an input string into a Path to a file.
 
         This method checks whether an (existing) file is writable. If the file does not exist the parent directory is
         checked for existence and whether it is writable.
 
         Parameters
         ----------
         input_: str
@@ -255,15 +274,14 @@
             If a Path created from input_ does not exist or is not a file
 
         Returns
         -------
         Path
             A Path instance created from input_
         """
-
         path = Path(input_)
         if path.exists():
             if not path.is_file():
                 raise ArgumentTypeError(f"not a file: '{input_}'")
             if not os.access(path, os.W_OK):
                 raise ArgumentTypeError(f"the file '{input_}' is not writable")
         else:
@@ -273,15 +291,15 @@
                 raise ArgumentTypeError(f"parent is not a directory: '{input_}'")
             if not os.access(path.parent, os.W_OK):
                 raise ArgumentTypeError(f"the parent directory of '{input_}' is not writable")
         return path
 
     @classmethod
     def string_to_file_path(cls, input_: str) -> Path:
-        """Convert an input string into a Path to a file
+        """Convert an input string into a Path to a file.
 
         Parameters
         ----------
         input_: str
             A string that is used to create a Path
 
         Raises
@@ -290,25 +308,24 @@
             If a Path created from input_ does not exist or is not a file
 
         Returns
         -------
         Path
             A Path instance created from input_
         """
-
         path = Path(input_)
         if not path.exists():
             raise ArgumentTypeError(f"the file '{input_}' does not exist")
         if not path.is_file():
             raise ArgumentTypeError(f"not a file: {input_}")
         return path
 
     @classmethod
     def string_to_dir_path(cls, input_: str) -> Path:
-        """Convert an input string into a Path to a directory
+        """Convert an input string into a Path to a directory.
 
         Parameters
         ----------
         input_: str
             A string that is used to create a Path
 
         Raises
@@ -317,19 +334,56 @@
             If a Path created from input_ does not exist or is not a directory
 
         Returns
         -------
         Path
             A Path instance created from input_
         """
-
         path = Path(input_)
         if not path.exists():
             raise ArgumentTypeError(f"the directory '{input_}' does not exist")
         if not path.is_dir():
             raise ArgumentTypeError(f"not a directory: {input_}")
         return path
 
+    @classmethod
+    def string_to_tuple(cls, input_: str) -> tuple[str, AnyUrl]:
+        """Convert an input string into a tuple of string and AnyUrl.
+
+        The input string is expected to be delimited by at least one "=" character to split on.
+
+        Parameters
+        ----------
+        input_: str
+            A string that is used to create a tuple
+
+        Raises
+        ------
+        ArgumentTypeError:
+            If input_ does not have at least one "=" to split on,
+            or if the resulting left-hand string contains a whitespace character after stripping,
+            or if the resulting right-hand string can not be validated as a URL.
+
+        Returns
+        -------
+        tuple[str, AnyUrl]
+            A tuple denoting a word and an instance of AnyUrl
+        """
+        try:
+            pkgbase, url_str = [str_.strip() for str_ in input_.split(sep="=", maxsplit=1)]
+        except ValueError:
+            raise ArgumentTypeError(f"There is no '=' in '{input_}'!") from None
+
+        if " " in pkgbase:
+            raise ArgumentTypeError(f"The string left of the '=' in '{input_}' must be a single word!")
+
+        try:
+            url = TypeAdapter(AnyUrl).validate_python(url_str)
+        except ValidationError:
+            raise ArgumentTypeError(f"The URL string '{url_str}' found in '{input_}' is invalid!") from None
+
+        return (pkgbase, url)
+
 
 def sphinx_repod_file() -> ArgumentParser:
     """Return ArgParseFactory.repod_file() for sphinx."""
     return ArgParseFactory.repod_file()
```

### Comparing `repod-0.2.2/repod/commands.py` & `repod-0.3.0.post0/repod/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,65 @@
+"""Utility functions for running external commands."""
 from pathlib import Path
-from subprocess import PIPE, STDOUT, CalledProcessError
-from typing import Dict, List, Optional, Union
+from subprocess import PIPE, STDOUT, CalledProcessError  # nosec: B404
 
-from subprocess_tee import CompletedProcess, run
+from subprocess_tee import CompletedProcess, run  # nosec: B404
 
 
-def _print_env(env: Optional[Dict[str, str]]) -> None:
-    """Print the environment variables from a dict
+def _print_env(env: dict[str, str] | None) -> None:
+    """Print the environment variables from a dict.
 
     Parameters
     ----------
-    env: Optional[Dict[str, str]]
+    env: dict[str, str] | None
         An optional dict with environment variables and their values
     """
-
     if env:
-        for (key, value) in sorted(env.items()):
+        for key, value in sorted(env.items()):
             print(f"{key}: {value}")
 
 
 def run_command(
-    cmd: Union[str, List[str]],
-    env: Optional[Dict[str, str]] = None,
+    cmd: str | list[str],
+    env: dict[str, str] | None = None,
     debug: bool = False,
     echo: bool = False,
     quiet: bool = False,
     check: bool = False,
-    cwd: Union[Optional[str], Optional[Path]] = None,
+    cwd: str | Path | None = None,
 ) -> CompletedProcess:
-    """Run a command
+    """Run a command.
 
     Parameters
     ----------
-    cmd: Union[str, List[str]]
+    cmd: str | list[str]
         A string or list of strings that will be passed to subprocess.run()
-    env: Optional[Dict[str, str]]
+    env: dict[str, str] | None
         A dict of environment variables and their respective values (defaults to None)
     debug: bool
         Whether to run in debug mode, which prints environment variables and command output (defaults to False)
     echo: bool
         Whether to print the command before running it (defaults to False)
     quiet: bool
         Whether to print the output of command while running it (defaults to False)
     check: bool
         Whether to check the return code of the command, which implies raising CallecProcessError (defaults to False)
-    cwd: Union[Optional[str], Optional[Path]]
+    cwd: str | Path | None
         In which directory to run the command (defaults to None, which means current working directory)
 
     Raises
     ------
     CalledProcessError
         If check is True and the commands return code is not 0
 
     Returns
     -------
     CompletedProcess
         The result of the command
     """
-
     if debug:
         _print_env(env)
 
     result = run(
         cmd,
         env=env,
         stdout=PIPE,
```

### Comparing `repod-0.2.2/repod/common/models.py` & `repod-0.3.0.post0/repod/common/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,598 +1,653 @@
+"""Pydantic models shared throughout the codebase."""
 from __future__ import annotations
 
-import re
-from typing import List, Optional
+from pathlib import Path
 
 from email_validator import EmailNotValidError, validate_email
 from pydantic import (
     BaseModel,
     HttpUrl,
     NonNegativeInt,
     PositiveInt,
     conint,
     constr,
-    validator,
+    field_validator,
 )
 
 from repod.common.regex import (
     ARCHITECTURE,
     BASE64,
     EPOCH,
-    FILENAME,
     MD5,
+    OPTIONS,
+    PACKAGE_FILENAME,
     PACKAGE_NAME,
     PACKAGER_NAME,
     PKGREL,
-    RELATIVE_PATH,
     SHA256,
     VERSION,
 )
 from repod.version import alpm
-from repod.version.util import cmp
 
 
 class Arch(BaseModel):
-    """A model describing a single 'arch' attribute
+    """A model describing a single 'arch' attribute.
 
     Attributes
     ----------
     arch: str
         The attribute can be used to describe the (required) data below an %ARCH% identifier in a 'desc' file, which
         identifies a package's architecture
     """
 
-    arch: constr(regex=f"^{ARCHITECTURE}$")  # type: ignore[valid-type]  # noqa: F722
+    arch: constr(pattern=f"^{ARCHITECTURE}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class Backup(BaseModel):
-    """A model describing a single 'backup' attribute
+    """A model describing a single 'backup' attribute.
 
     Attributes
     ----------
-    backup: Optional[List[str]]
+    backup: list[str] | None
         The attribute can be used to describe the (optional) data below a %BACKUP% identifier in a 'desc' file, which
         identifies which file(s) of a package pacman will create backups for
     """
 
-    backup: Optional[List[constr(regex=f"^{RELATIVE_PATH}$")]]  # type: ignore[valid-type]  # noqa: F722
+    backup: list[str] | None = None
+
+    @field_validator("backup")
+    @classmethod
+    def validate_backup(cls, backup: list[str] | None) -> list[str] | None:  # noqa: N805
+        """Validate the backup attribute.
+
+        The backup attribute may not contain strings that represent absolute Paths or Paths in the home directory
+
+        Parameters
+        ----------
+        backup: list[str] | None
+            An optional list of strings, representing paths to validate
+
+        Returns
+        -------
+        list[str] | None
+            None if backup is None, empty list if backup is empty list, or a validated list of strings
+        """
+        if backup:
+            for file in backup:
+                path = Path(file)
+                if path.is_absolute():
+                    raise ValueError(f"Absolute paths in a list of files are not valid: {path}")
+                parts = path.parts
+                if parts[0] == "home" and len(parts) > 1:
+                    raise ValueError(
+                        f"Files or directories in the home directory is not valid in a list of files: {path}"
+                    )
+
+        return backup
 
 
 class Base(BaseModel):
-    """A model describing a single 'base' attribute
+    """A model describing a single 'base' attribute.
 
     Attributes
     ----------
     base: str
         The attribute can be used to describe the (required) data below a %BASE% identifier in a 'desc' file, which
         identifies a package's pkgbase
     """
 
-    base: constr(regex=f"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
+    base: constr(pattern=f"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class BuildDate(BaseModel):
-    """A model describing a single 'builddate' attribute
+    """A model describing a single 'builddate' attribute.
 
     Attributes
     ----------
     builddate: int
         The attribute can be used to describe the (required) data below a %BUILDDATE% identifier in a 'desc' file,
         which identifies a package's build date (represented in seconds since the epoch)
     """
 
     builddate: NonNegativeInt
 
 
 class CheckDepends(BaseModel):
-    """A model describing a single 'checkdepends' attribute
+    """A model describing a single 'checkdepends' attribute.
 
     Attributes
     ----------
-    checkdepends: Optional[List[str]]
+    checkdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %CHECKDEPENDS% identifier in a 'desc' file,
         which identifies a package's checkdepends
     """
 
-    checkdepends: Optional[List[str]]
+    checkdepends: list[str] | None = None
 
 
 class Conflicts(BaseModel):
-    """A model describing a single 'conflicts' attribute
+    """A model describing a single 'conflicts' attribute.
 
     Attributes
     ----------
-    conflicts: Optional[List[str]]
+    conflicts: list[str] | None
         The attribute can be used to describe the (optional) data below a %CONFLICTS% identifier in a 'desc' file, which
         identifies what other package(s) a package conflicts with
     """
 
-    conflicts: Optional[List[str]]
+    conflicts: list[str] | None = None
 
 
 class CSize(BaseModel):
-    """A model describing a single 'csize' attribute
+    """A model describing a single 'csize' attribute.
 
     Attributes
     ----------
     csize: int
         The attribute can be used to describe the (required) data below a %CSIZE% identifier in a 'desc' file, which
         identifies a package's size
     """
 
     csize: NonNegativeInt
 
 
 class Depends(BaseModel):
-    """A model describing a single 'depends' attribute
+    """A model describing a single 'depends' attribute.
 
     Attributes
     ----------
-    depends: Optional[List[str]]
+    depends: list[str] | None
         The attribute can be used to describe the (optional) data below a %DEPENDS% identifier in a 'desc' file, which
         identifies what other package(s) a package depends on
     """
 
-    depends: Optional[List[str]]
+    depends: list[str] | None = None
 
 
 class Desc(BaseModel):
-    """A model describing a single 'desc' attribute
+    """A model describing a single 'desc' attribute.
 
     Attributes
     ----------
     desc: str
         The attribute can be used to describe the (required) data below a %DESC% identifier in a 'desc' file, which
         identifies a package's description
     """
 
     desc: str
 
 
 class FileName(BaseModel):
-    """A model describing a single 'filename' attribute
+    """A model describing a single 'filename' attribute.
 
     Attributes
     ----------
     filename: str
         The attribute can be used to describe the (required) data below a %FILENAME% identifier in a 'desc' file, which
         identifies a package's file name
     """
 
-    filename: constr(regex=f"^{FILENAME}$")  # type: ignore[valid-type]  # noqa: F722
+    filename: constr(pattern=f"^{PACKAGE_FILENAME}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class FileList(BaseModel):
-    """A model describing an optional list of files
+    """A model describing an optional list of files.
 
     Attributes
     ----------
-    files: Optional[List[str]]
+    files: list[str] | None
         The attribute can be used to describe the (optional) data below a %FILES% identifier in a 'files' file, which
         identifies which file(s) belong to a package
     """
 
-    files: Optional[List[constr(regex=f"^{RELATIVE_PATH}$")]]  # type: ignore[valid-type]  # noqa: F722
+    files: list[str] | None = None
+
+    @field_validator("files")
+    @classmethod
+    def validate_files(cls, files: list[str] | None) -> list[str] | None:  # noqa: N805
+        """Validate the files attribute.
+
+        The files attribute may not contain strings that represent absolute Paths or Paths in the home directory
+
+        Parameters
+        ----------
+        files: list[str] | None
+            An optional list of strings, representing paths to validate
 
-    @validator("files")
-    def validate_no_file_in_home(cls, files: List[str]) -> Optional[List[str]]:
+        Returns
+        -------
+        list[str] | None
+            None if files is None, empty list if files is empty list, or a validated list of strings
+        """
         if files:
             for file in files:
-                if re.search("^(home/).+$", file):
-                    raise ValueError("A package must not provide files in /home")
+                path = Path(file)
+                if path.is_absolute():
+                    raise ValueError(f"Absolute paths in a list of files are not valid: {path}")
+                parts = path.parts
+                if parts[0] == "home" and len(parts) > 1:
+                    raise ValueError(
+                        f"Files or directories in the home directory is not valid in a list of files: {path}"
+                    )
 
         return files
 
 
 class Groups(BaseModel):
-    """A model describing a single 'groups' attribute
+    """A model describing a single 'groups' attribute.
 
     Attributes
     ----------
-    groups: Optional[List[str]]
+    groups: list[str] | None
         The attribute can be used to describe the (optional) data below a %GROUPS% identifier in a 'desc' file, which
         identifies a package's groups
     """
 
-    groups: Optional[List[constr(regex=f"^{PACKAGE_NAME}$")]]  # type: ignore[valid-type]  # noqa: F722
+    groups: list[constr(pattern=f"^{PACKAGE_NAME}$")] | None = None  # type: ignore[valid-type]  # noqa: F722
 
 
 class ISize(BaseModel):
-    """A model describing a single 'isize' attribute
+    """A model describing a single 'isize' attribute.
 
     Attributes
     ----------
     isize: int
         The attribute can be used to describe the (required) data below an %ISIZE% identifier in a 'desc' file, which
         identifies a package's installed size
     """
 
     isize: NonNegativeInt
 
 
 class License(BaseModel):
-    """A model describing a single 'license' attribute
+    """A model describing a single 'license' attribute.
 
     Attributes
     ----------
-    license: List[str]
+    license: list[str]
         The attribute can be used to describe the (required) data below a %LICENSE% identifier in a 'desc' file, which
         identifies a package's license(s)
     """
 
-    license: List[str]
+    license: list[str]  # noqa: A003
 
 
 class MakeDepends(BaseModel):
-    """A model describing a single 'makedepends' attribute
+    """A model describing a single 'makedepends' attribute.
 
     Attributes
     ----------
-    makedepends: Optional[List[str]]
+    makedepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %MAKEDEPENDS% identifier in a 'desc' file,
         which identifies a package's makedepends
     """
 
-    makedepends: Optional[List[str]]
+    makedepends: list[str] | None = None
 
 
 class Md5Sum(BaseModel):
-    """A model describing a single 'md5sum' attribute
+    """A model describing a single 'md5sum' attribute.
 
     Attributes
     ----------
     md5sum: str
         The attribute can be used to describe the (required) data below an %MD5SUM% identifier in a 'desc' file, which
         identifies a package's md5 checksum
     """
 
-    md5sum: constr(regex=MD5)  # type: ignore[valid-type]
+    md5sum: constr(pattern=MD5)  # type: ignore[valid-type]
 
 
 class Name(BaseModel):
-    """A model describing a single 'name' attribute
+    """A model describing a single 'name' attribute.
 
     Attributes
     ----------
     name: str
         The attribute can be used to describe the (required) data below a %NAME% identifier in a 'desc' file, which
         identifies a package's name
     """
 
-    name: constr(regex=f"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
+    name: constr(pattern=f"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
+
+
+class Options(BaseModel):
+    """A list of makepkg.conf OPTIONS used during the creation of a package.
+
+    For valid values refer to the OPTIONS subsection in https://man.archlinux.org/man/makepkg.conf.5#OPTIONS
+
+    Attributes
+    ----------
+    options: list[str] | None
+        An optional list of strings representing makepkg.conf OPTIONS used during the creation of a package
+    """
+
+    options: list[constr(pattern=rf"^{OPTIONS}$")] | None = None  # type: ignore[valid-type]  # noqa: F722
 
 
 class Packager(BaseModel):
-    """A model describing a single 'packager' attribute
+    """A model describing a single 'packager' attribute.
 
     Attributes
     ----------
     packager: str
         The attribute can be used to describe the (required) data below a %PACKAGER% identifier in a 'desc' file, which
         identifies a package's packager
     """
 
-    packager: constr(regex=(rf"^{PACKAGER_NAME}\s<(.*)>$"))  # type: ignore[valid-type]  # noqa: F722
+    packager: constr(pattern=(rf"^{PACKAGER_NAME}\s<(.*)>$"))  # type: ignore[valid-type]  # noqa: F722
 
-    @validator("packager")
-    def validate_packager_has_valid_email(cls, packager: str) -> str:
+    @field_validator("packager")
+    @classmethod
+    def validate_packager_has_valid_email(cls, packager: str) -> str:  # noqa: N805
+        """Validate that Packager has an email in the UID.
 
+        Parameters
+        ----------
+        packager: str
+            The packager UID string
+
+        Raises
+        ------
+        ValuError
+            If no valid mail is found in packager
+
+        Returns
+        -------
+        str
+            A validated Packager UID string
+        """
         email = packager.replace(">", "").split("<")[1]
         try:
             validate_email(email, check_deliverability=False)
         except EmailNotValidError as e:
-            raise ValueError(f"The packager email is not valid: {email}\n{e}")
+            raise ValueError(f"The packager email is not valid: {email}\n{e}") from e
 
         return packager
 
 
 class PgpSig(BaseModel):
-    """A model describing a single 'pgpsig' attribute
+    """A model describing a single 'pgpsig' attribute.
 
     Attributes
     ----------
     pgpsig: str
         The attribute can be used to describe the (optional) data below a %PGPSIG% identifier in a 'desc' file, which
         identifies a package's PGP signature
     """
 
-    pgpsig: Optional[constr(regex=f"^{BASE64}$")]  # type: ignore[valid-type]  # noqa: F722
+    pgpsig: constr(pattern=f"^{BASE64}$") | None = None  # type: ignore[valid-type]  # noqa: F722
+
+
+class PkgBase(BaseModel):
+    """A pkgbase for a package.
+
+    Refer to https://man.archlinux.org/man/PKGBUILD.5.en#PACKAGE_SPLITTING for details on pkgbase
+
+    Attributes
+    ----------
+    pkgbase: str
+        A string representing the pkgbase of a package
+    """
+
+    pkgbase: constr(pattern=rf"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
+
+
+class PkgDesc(BaseModel):
+    """A model describing a single pkgdesc attribute.
+
+    Attributes
+    ----------
+    pkgdesc: str
+        A string used as package description
+    """
+
+    pkgdesc: str
+
+
+class PkgName(BaseModel):
+    """A pkgname of a package.
+
+    Refer to the pkgname section in https://man.archlinux.org/man/PKGBUILD.5.en#OPTIONS_AND_DIRECTIVES for details
+
+    Attributes
+    ----------
+    pkgname: str
+        A string representing the pkgname of a package
+    """
+
+    pkgname: constr(pattern=rf"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class Provides(BaseModel):
-    """A model describing a single 'provides' attribute
+    """A model describing a single 'provides' attribute.
 
     Attributes
     ----------
-    provides: Optional[List[str]]
+    provides: list[str] | None
         The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
         identifies what other package(s) a package provides
     """
 
-    provides: Optional[List[str]]
+    provides: list[str] | None = None
 
 
 class Replaces(BaseModel):
-    """A model describing a single 'replaces' attribute
+    """A model describing a single 'replaces' attribute.
 
     Attributes
     ----------
-    replaces: Optional[List[str]]
+    replaces: list[str] | None
         The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
         identifies what other package(s) a package replaces
     """
 
-    replaces: Optional[List[str]]
+    replaces: list[str] | None = None
 
 
 class SchemaVersionV1(BaseModel):
-    """A model describing a schema version 1
+    """A model describing a schema version 1.
 
     Attributes
     ----------
     schema_version: PositiveInt
         A schema version - 1 - for a model
     """
 
     schema_version: conint(ge=1, le=1) = 1  # type: ignore[valid-type]
 
 
 class SchemaVersionV2(BaseModel):
-    """A model describing a schema version 2
+    """A model describing a schema version 2.
 
     Attributes
     ----------
     schema_version: PositiveInt
         A schema version - 2 - for a model
     """
 
     schema_version: conint(ge=2, le=2) = 2  # type: ignore[valid-type]
 
 
 class Sha256Sum(BaseModel):
-    """A model describing a single 'sha256sum' attribute
+    """A model describing a single 'sha256sum' attribute.
 
     Attributes
     ----------
     sha256sum: str
         The attribute can be used to describe the (required) data below an %SHA256SUM% identifier in a 'desc' file,
         which identifies a package's sha256 checksum
     """
 
-    sha256sum: constr(regex=SHA256)  # type: ignore[valid-type]
+    sha256sum: constr(pattern=SHA256)  # type: ignore[valid-type]
 
 
 class OptDepends(BaseModel):
-    """A model describing a single 'optdepends' attribute
+    """A model describing a single 'optdepends' attribute.
 
     Attributes
     ----------
-    optdepends: Optional[List[str]]
+    optdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
         which identifies what other package(s) a package optionally depends on
     """
 
-    optdepends: Optional[List[str]]
+    optdepends: list[str] | None = None
 
 
 class Url(BaseModel):
-    """A model describing a single 'url' attribute
+    """A model describing a single 'url' attribute.
 
     Attributes
     ----------
     url: str
         The attribute can be used to describe the (required) data below a %URL% identifier in a 'desc' file, which
         identifies a package's URL
     """
 
     url: HttpUrl
 
 
-class Epoch(BaseModel):
-    """A model dscribing a single 'epoch' attribute
-
-    The epoch denotes a downgrade in version of a given package (a version with an epoch trumps one without)
+class SourceUrl(BaseModel):
+    """A URL pointing at sources.
 
     Attributes
     ----------
-    epoch: PositiveInt
-        A string representing a valid epoch of a package
+    source_url: HttpUrl | None
+        An optional url that points at sources (defaults to None)
     """
 
-    epoch: PositiveInt
+    source_url: HttpUrl | None = None
 
-    def vercmp(self, epoch: Epoch) -> int:
-        """Compare the epoch with another
 
-        The comparison algorithm is based on pyalpm's/ pacman's vercmp behavior.
+class Epoch(BaseModel):
+    """A model dscribing a single 'epoch' attribute.
 
-        Returns
-        -------
-        int
-            -1 if self.epoch is older than epoch
-            0 if self.epoch is equal to epoch
-            1 if self.epoch is newer than epoch
-        """
+    The epoch denotes a downgrade in version of a given package (a version with an epoch trumps one without)
+
+    Attributes
+    ----------
+    epoch: PositiveInt | None
+        An optional positive integer representing the epoch of a package
+    """
 
-        return cmp(self.epoch, epoch.epoch)
+    epoch: PositiveInt | None = None
 
 
 class PkgRel(BaseModel):
-    """A model dscribing a single 'pkgrel' attribute
+    """A model dscribing a single 'pkgrel' attribute.
 
     The pkgrel denotes the build version of a given package
 
     Attributes
     ----------
     pkgrel: str
-        A string representing a valid pkgrel of a package
+        A string representing the pkgrel (package release version) of a package
     """
 
-    pkgrel: constr(regex=rf"^{PKGREL}$")  # type: ignore[valid-type]  # noqa: F722
-
-    def as_list(self) -> List[str]:
-        """Return the pkgrel components as list
-
-        The version string is split by "."
-
-        Returns
-        -------
-        List[str]
-            A list of strings representing the components of the pkgrel
-        """
-
-        return [str(part) for part in self.pkgrel.split(".")]
-
-    def vercmp(self, pkgrel: PkgRel) -> int:
-        """Compare the pkgrel with another
-
-        The comparison algorithm is based on pyalpm's/ pacman's vercmp behavior.
-
-        Returns
-        -------
-        int
-            -1 if self.pkgrel is older than pkgrel
-            0 if self.pkgrel is equal to pkgrel
-            1 if self.pkgrel is newer than pkgrel
-        """
-
-        return alpm.vercmp(self.pkgrel, pkgrel.pkgrel)
+    pkgrel: constr(pattern=rf"^{PKGREL}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class PkgVer(BaseModel):
-    """A model dscribing a single 'pkgver' attribute
+    """A model dscribing a single 'pkgver' attribute.
 
     The pkgver denotes the upstream version of a given package
 
     Attributes
     ----------
     pkgver: str
-        A string representing a valid pkgver of a package
+        A string representing the pkgver (upstream package version) of a package
     """
 
-    pkgver: constr(regex=rf"^({VERSION})$")  # type: ignore[valid-type]  # noqa: F722
-
-    def as_list(self) -> List[str]:
-        """Return the pkgver components as list
-
-        The version string is split on none alpanum characters
-
-        Returns
-        -------
-        List[str]
-            A list of strings representing the components of the pkgver
-        """
-
-        return [part for part in re.split(r"[^a-zA-Z\d]", self.pkgver) if part]
-
-    def vercmp(self, pkgver: PkgVer) -> int:
-        """Compare the pkgver with another
-
-        The comparison algorithm is based on pyalpm's/ pacman's vercmp behavior.
-        If PYALPM_VERCMP is True, pyalpm has been imported and its implementation of vercmp() is used.
-
-        Returns
-        -------
-        int
-            -1 if self.pkgver is older than pkgver
-            0 if self.pkgver is equal to pkgver
-            1 if self.pkgver is newer than pkgver
-        """
-
-        return alpm.vercmp(self.pkgver, pkgver.pkgver)
+    pkgver: constr(pattern=rf"^({VERSION})$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class Version(BaseModel):
-    """A model describing a single 'version' attribute
+    """A model describing a single 'version' attribute.
 
     Attributes
     ----------
     version: str
         The attribute can be used to describe the (required) data below a %VERSION% identifier in a 'desc' file, which
         identifies a package's version (this is the accumulation of epoch, pkgver and pkgrel)
     """
 
-    version: constr(regex=rf"^({EPOCH}|){VERSION}-{PKGREL}$")  # type: ignore[valid-type]  # noqa: F722
+    version: constr(pattern=rf"^({EPOCH}|){VERSION}-{PKGREL}$")  # type: ignore[valid-type]  # noqa: F722
 
-    def get_epoch(self) -> Optional[Epoch]:
-        """Return the epoch of the version
+    def get_epoch(self: Version) -> Epoch | None:
+        """Return the epoch of the version.
 
         Returns
         -------
-        Optional[int]
+        int | None
             An optional string representing the epoch of the version
         """
-
         if ":" in self.version:
             return Epoch(epoch=self.version.split(":")[0])
-        else:
-            return None
 
-    def get_pkgver(self) -> PkgVer:
-        """Return the pkgver of the version
+        return None
+
+    def get_pkgver(self: Version) -> PkgVer:
+        """Return the pkgver of the version.
 
         Returns
         -------
         PkgVer
             A PkgVer representing the pkgver of the version
         """
-
         pkgver_pkgrel = self.version.split(":")[1] if ":" in self.version else self.version
         return PkgVer(pkgver=str(pkgver_pkgrel.split("-")[0]))
 
-    def get_pkgrel(self) -> PkgRel:
-        """Return the pkgrel of the version
+    def get_pkgrel(self: Version) -> PkgRel:
+        """Return the pkgrel of the version.
 
         Returns
         -------
         PkgRel
             A PkgRel representing the pkgrel of the version
         """
-
         pkgver_pkgrel = self.version.split(":")[1] if ":" in self.version else self.version
         return PkgRel(pkgrel=str(pkgver_pkgrel.split("-")[1]))
 
-    def vercmp(self, version: Version) -> int:
-        """Compare the version with another
+    def vercmp(self: Version, version: Version) -> int:
+        """Compare the version with another.
 
         The comparison algorithm is based on pyalpm's/ pacman's vercmp behavior.
         If PYALPM_VERCMP is True, pyalpm has been imported and its implementation of vercmp() is used.
 
         Returns
         -------
         int
             -1 if self.version is older than version
             0 if self.version is equal to version
             1 if self.version is newer than version
         """
-
         return alpm.pkg_vercmp(self.version, version.version)
 
-    def is_older_than(self, version: Version) -> bool:
-        """Check whether the version is older than a provided version
+    def is_older_than(self: Version, version: Version) -> bool:
+        """Check whether the version is older than a provided version.
 
         Parameters
         ----------
         version: Version
             Another version to compare that of self to
 
         Returns
         -------
         True if self.version is older than the provided version, False otherwise.
         """
-
         return True if self.vercmp(version=version) < 0 else False
 
-    def is_newer_than(self, version: Version) -> bool:
-        """Check whether the version is newer than a provided version
+    def is_newer_than(self: Version, version: Version) -> bool:
+        """Check whether the version is newer than a provided version.
 
         Parameters
         ----------
         version: Version
             Another version to compare that of self to
 
         Returns
         -------
         True if self.version is newer than the provided version, False otherwise.
         """
-
         return True if self.vercmp(version=version) > 0 else False
```

### Comparing `repod-0.2.2/repod/common/regex.py` & `repod-0.3.0.post0/repod/common/regex.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+"""Regular expressions used for matching strings in packages and sync databases."""
 from repod.common.enums import (
     ArchitectureEnum,
     tar_compression_types_for_filename_regex,
 )
 
 RELATIVE_MTREE_PATH = r"[A-Za-z0-9.,:;/_()@\\&$?!+%~{}<>*\-\"\'\[\]\`^|]+"
 """
 RELATIVE_MTREE_PATH may include printable ASCII characters other than space, #, =. The backslash is included as it's a
 result of encoding special characters. See the mtree implementation in libarchive:
 https://github.com/libarchive/libarchive/blob/v3.6.1/libarchive/archive_write_set_format_mtree.c#L307
 """
 ABSOLUTE_MTREE_PATH = rf"/{RELATIVE_MTREE_PATH}"
 ARCHITECTURE = rf"({ArchitectureEnum.as_or_regex()})"
+B2 = r"^[a-f0-9]{128}$"
 BASE64 = r"[0-9A-Za-z/+]+={0,2}"
 BUILDENVS = r"(!|)[\w\-.]+"
+CK = r"^[0-9]{10}$"
 EPOCH = r"[1-9]+[0-9]*:"
 MD5 = r"^[a-f0-9]{32}$"
 OPTIONS = r"(!|)[\w\-.]+"
+PGP_KEY_ID = r"^[A-F0-9]{40}$"
 PKGREL = r"[1-9]+[0-9]*(|[.]{1}[1-9]+[0-9]*)"
 PACKAGE_NAME = r"[a-z\d_@+]+[a-z\d\-._@+]*"
 PACKAGER_NAME = r"[\w\s\-().]+"
-RELATIVE_PATH = r"[^/][\w\d\s.,:;/_=#()@\\&$?!+%~{}<>*\-\"\'\[\]\`^]+"
-ABSOLUTE_PATH = rf"/{RELATIVE_PATH}"
+SHA1 = r"^[a-f0-9]{40}$"
+SHA224 = r"^[a-f0-9]{56}$"
 SHA256 = r"^[a-f0-9]{64}$"
+SHA384 = r"^[a-f0-9]{96}$"
+SHA512 = r"^[a-f0-9]{128}$"
 VERSION = r"([A-Za-z\d]+)[_+.]?[A-Za-z\d_+.]*"
-FILENAME = (
+PACKAGE_FILENAME = (
     rf"{PACKAGE_NAME}-({EPOCH}|){VERSION}-{PKGREL}-{ARCHITECTURE}"
     rf"(.pkg.tar)({tar_compression_types_for_filename_regex()})"
 )
-PACKAGE_PATH = rf"{ABSOLUTE_PATH}/{FILENAME}"
-PACKAGE_SIGNATURE_PATH = rf"{ABSOLUTE_PATH}/{FILENAME}(.sig)"
+SIGNATURE_FILENAME = rf"{PACKAGE_FILENAME}(.sig)"
```

### Comparing `repod-0.2.2/repod/config/defaults.py` & `repod-0.3.0.post0/repod/config/defaults.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+"""Module with configuration defaults for settings.
+
+The defaults for locations and directories are provided as dicts which use SettingsTypeEnum as keys to distinguish
+between different ways of running repod.
+"""
 from pathlib import Path
 
+from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS
 from xdg.BaseDirectory import xdg_config_home, xdg_state_home
 
 from repod.common.enums import ArchitectureEnum, CompressionTypeEnum, SettingsTypeEnum
 
 DEFAULT_ARCHITECTURE = ArchitectureEnum.ANY
+DEFAULT_BUILD_REQUIREMENTS_EXIST: bool = True
 DEFAULT_DATABASE_COMPRESSION = CompressionTypeEnum.GZIP
 DEFAULT_NAME = "default"
 
+ORJSON_OPTION = OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS
+
 SETTINGS_LOCATION = {
     SettingsTypeEnum.SYSTEM: Path("/etc/repod.conf"),
     SettingsTypeEnum.USER: Path(xdg_config_home + "/repod/repod.conf"),
 }
 SETTINGS_OVERRIDE_LOCATION = {
     SettingsTypeEnum.SYSTEM: Path("/etc/repod.conf.d/"),
     SettingsTypeEnum.USER: Path(xdg_config_home + "/repod/repod.conf.d/"),
@@ -33,7 +42,15 @@
     SettingsTypeEnum.SYSTEM: Path("/var/lib/repod/data/pool/source/"),
     SettingsTypeEnum.USER: Path(xdg_state_home + "/repod/data/pool/source/"),
 }
 SOURCE_REPO_BASE = {
     SettingsTypeEnum.SYSTEM: Path("/var/lib/repod/data/repo/source/"),
     SettingsTypeEnum.USER: Path(xdg_state_home + "/repod/data/repo/source/"),
 }
+PACKAGE_ARCHIVE_DIR = {
+    SettingsTypeEnum.SYSTEM: Path("/var/lib/repod/archive/package/"),
+    SettingsTypeEnum.USER: Path(xdg_state_home + "/repod/archive/package/"),
+}
+SOURCE_ARCHIVE_DIR = {
+    SettingsTypeEnum.SYSTEM: Path("/var/lib/repod/archive/source/"),
+    SettingsTypeEnum.USER: Path(xdg_state_home + "/repod/archive/source/"),
+}
```

### Comparing `repod-0.2.2/repod/errors.py` & `repod-0.3.0.post0/repod/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,25 @@
+"""Custom Exceptions for repod."""
+
+
 class RepoManagementError(Exception):
-    """A class of Errors that is raised on issues with handling a repository database"""
+    """A class of Errors that is raised on issues with handling a repository database."""
 
 
 class RepoManagementFileError(RepoManagementError):
-    """An Error that is raised on issues with reading or writing files using repo_managment"""
+    """An Error that is raised on issues with reading or writing files using repo_managment."""
 
 
 class RepoManagementValidationError(RepoManagementError):
-    """An Error that is raised on issues with validating files using repo_managment"""
+    """An Error that is raised on issues with validating files using repo_managment."""
 
 
 class RepoManagementFileNotFoundError(RepoManagementFileError, FileNotFoundError):
-    """An Error that is raised when a file can not be found"""
+    """An Error that is raised when a file can not be found."""
+
+
+class TaskError(RepoManagementError):
+    """An Error that is raised when an error occurs in a Task."""
+
+
+class FileParserError(RepoManagementError):
+    """An Error that is raised when an error occurs during parsing of a file."""
```

### Comparing `repod-0.2.2/repod/files/buildinfo.py` & `repod-0.3.0.post0/repod/files/buildinfo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,270 +1,284 @@
+"""Handling of .BUILDINFO files."""
 from __future__ import annotations
 
 from io import StringIO
 from pathlib import Path
 from re import fullmatch
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any
 
-from pydantic import BaseModel, NonNegativeInt, conint, constr, root_validator
+from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS, dumps
+from pydantic import BaseModel, NonNegativeInt, constr, field_validator, model_validator
 
-from repod.common.enums import FieldTypeEnum
-from repod.common.models import Packager
+from repod.common.enums import ArchitectureEnum, FieldTypeEnum
+from repod.common.models import (
+    Options,
+    Packager,
+    PkgBase,
+    PkgName,
+    SchemaVersionV1,
+    SchemaVersionV2,
+)
 from repod.common.regex import (
-    ABSOLUTE_PATH,
     ARCHITECTURE,
     BUILDENVS,
     EPOCH,
-    OPTIONS,
     PACKAGE_NAME,
     PKGREL,
     SHA256,
     VERSION,
 )
 from repod.errors import RepoManagementError
 
-BUILDINFO_ASSIGNMENTS: Dict[str, Tuple[str, FieldTypeEnum]] = {
+BUILDINFO_ASSIGNMENTS: dict[str, tuple[str, FieldTypeEnum]] = {
     "builddate": ("builddate", FieldTypeEnum.INT),
     "builddir": ("builddir", FieldTypeEnum.STRING),
     "buildenv": ("buildenv", FieldTypeEnum.STRING_LIST),
     "buildtool": ("buildtool", FieldTypeEnum.STRING),
     "buildtoolver": ("buildtoolver", FieldTypeEnum.STRING),
-    "format": ("format_", FieldTypeEnum.INT),
+    "format": ("schema_version", FieldTypeEnum.INT),
     "installed": ("installed", FieldTypeEnum.STRING_LIST),
     "options": ("options", FieldTypeEnum.STRING_LIST),
     "packager": ("packager", FieldTypeEnum.STRING),
     "pkgarch": ("pkgarch", FieldTypeEnum.STRING),
     "pkgbase": ("pkgbase", FieldTypeEnum.STRING),
     "pkgbuild_sha256sum": ("pkgbuild_sha256sum", FieldTypeEnum.STRING),
     "pkgname": ("pkgname", FieldTypeEnum.STRING),
     "pkgver": ("pkgver", FieldTypeEnum.STRING),
     "startdir": ("startdir", FieldTypeEnum.STRING),
 }
 
 
 class BuildDate(BaseModel):
-    """A build date in seconds since the epoch
+    """A build date in seconds since the epoch.
 
     Attributes
     ----------
     builddate: NonNegativeInt
         A number >= 0
     """
 
     builddate: NonNegativeInt
 
 
 class BuildDir(BaseModel):
-    """An absolute build directory
+    """An absolute build directory.
 
     Attributes
     ----------
     builddir: str
         A string representing an absolute directory
     """
 
-    builddir: constr(regex=rf"^{ABSOLUTE_PATH}$")  # type: ignore[valid-type]  # noqa: F722
+    builddir: str
+
+    @field_validator("builddir")
+    @classmethod
+    def validate_builddir(cls, builddir: str) -> str:
+        """Validate the builddir attribute.
+
+        The builddir attribute may not contain strings that represent absolute Paths or Paths in the home directory
+
+        Parameters
+        ----------
+        builddir: str
+            A string, representing a path
+
+        Returns
+        -------
+        str
+            A validated string, representing an absolute Path
+        """
+        path = Path(builddir)
+        if not path.is_absolute():
+            raise ValueError(f"A relative path as builddir is not valid: {path}")
+
+        return builddir
 
 
 class BuildEnv(BaseModel):
-    """A list of build environment options
+    """A list of build environment options.
 
     For valid values refer to BUILDENV in https://man.archlinux.org/man/makepkg.conf.5#OPTIONS
 
     Attributes
     ----------
-    buildenv: List[str]
+    buildenv: list[str]
         A list of strings as described by makepkg.conf's BUILDENV option
     """
 
-    buildenv: List[constr(regex=rf"^{BUILDENVS}$")]  # type: ignore[valid-type]  # noqa: F722
+    buildenv: list[constr(pattern=rf"^{BUILDENVS}$")]  # type: ignore[valid-type]  # noqa: F722
 
 
 class BuildTool(BaseModel):
-    """The build tool used to create a package
+    """The build tool used to create a package.
 
     Attributes
     ----------
     buildtool: str
         The package name of the build tool used to create a package
     """
 
-    buildtool: constr(regex=rf"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
+    buildtool: constr(pattern=rf"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class BuildToolVer(BaseModel):
-    """The package version of the build tool used to create a package
+    """The package version of the build tool used to create a package.
 
     Attributes
     ----------
     buildtoolver: str
         The version of the build tool used to create a package
     """
 
     buildtoolver: str
 
 
-class FormatV1(BaseModel):
-    """The format version of a .BUILDINFO file (version 1)
-
-    Attributes
-    ----------
-    format_: int
-        1 - representing version 1
-    """
-
-    format_: conint(ge=1, le=1) = 1  # type: ignore[valid-type]
-
-
-class FormatV2(BaseModel):
-    """The format version of a .BUILDINFO file (version 2)
-
-    Attributes
-    ----------
-    format_: int
-        2 - representing version 2
-    """
-
-    format_: conint(ge=2, le=2) = 2  # type: ignore[valid-type]
-
-
 class Installed(BaseModel):
-    """A list of package names and versions installed during the creation of a package
+    """A list of package names and versions installed during the creation of a package.
 
     Attributes
     ----------
-    installed: List[str]
+    installed: list[str]
         A list of strings representing <package_name>-<epoch><version>-<pkgrel>-<architecture> of packages installed
         during the creation of a package
     """
 
-    installed: List[  # type: ignore[valid-type]
-        constr(regex=rf"^({PACKAGE_NAME})-({EPOCH}|){VERSION}-{PKGREL}-{ARCHITECTURE}$")  # noqa: F722
+    installed: list[  # type: ignore[valid-type]
+        constr(pattern=rf"^({PACKAGE_NAME})-({EPOCH}|){VERSION}-{PKGREL}-{ARCHITECTURE}$")  # noqa: F722
     ]
 
+    @classmethod
+    def as_models(cls, installed: list[str]) -> list[tuple[PkgName, PkgVer, ArchitectureEnum]]:
+        """Return a list of installed dependencies as models.
 
-class Options(BaseModel):
-    """A list of makepkg.conf OPTIONS used during the creation of a package
-
-    For valid values refer to the OPTIONS subsection in https://man.archlinux.org/man/makepkg.conf.5#OPTIONS
+        Parameters
+        ----------
+        installed: list[str]
+            A list of strings, each describing pkgname-version-architecture
 
-    Attributes
-    ----------
-    options: List[str]
-        A list of strings representing makepkg.conf OPTIONS used during the creation of a package
-    """
+        Raises
+        ------
+        ValidationError
+            If any of the entries in installed can not be validated using PkgName, PkgVer, Architecture
 
-    options: List[constr(regex=rf"^{OPTIONS}$")]  # type: ignore[valid-type]  # noqa: F722
+        Returns
+        -------
+        list[tuple[PkgName, PkgVer, ArchitectureEnum]]
+            A list of PkgName, PkgVer and ArchitectureEnum tuples, which describe each entry in installed
+        """
+        return [
+            (
+                PkgName(pkgname="-".join(dep.split("-")[0:-3])),
+                PkgVer(pkgver="-".join(dep.split("-")[-3:-1])),
+                ArchitectureEnum(dep.split("-")[-1]),
+            )
+            for dep in installed
+        ]
 
 
 class PkgArch(BaseModel):
-    """A CPU architecture for a package
+    """A CPU architecture for a package.
 
     Refer to the arch subsection in https://man.archlinux.org/man/PKGBUILD.5.en#OPTIONS_AND_DIRECTIVES for details
 
     Attributes
     ----------
     pkgarch: str
         A valid CPU architecture for a package
     """
 
-    pkgarch: constr(regex=rf"^{ARCHITECTURE}$")  # type: ignore[valid-type]  # noqa: F722
-
-
-class PkgBase(BaseModel):
-    """A pkgbase for a package
-
-    Refer to https://man.archlinux.org/man/PKGBUILD.5.en#PACKAGE_SPLITTING for details on pkgbase
-
-    Attributes
-    ----------
-    pkgbase: str
-        A string representing a valid pkgbase for a package
-    """
-
-    pkgbase: constr(regex=rf"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
+    pkgarch: constr(pattern=rf"^{ARCHITECTURE}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class PkgBuildSha256Sum(BaseModel):
-    """A SHA-256 checksum for a PKGBUILD file of a package
+    """A SHA-256 checksum for a PKGBUILD file of a package.
 
     Attributes
     ----------
     pkgbuild_sha256sum: str
         A string representing a SHA-256 checksum for a PKGBUILD of a package
     """
 
-    pkgbuild_sha256sum: constr(regex=rf"{SHA256}")  # type: ignore[valid-type]  # noqa: F722
-
-
-class PkgName(BaseModel):
-    """A pkgname of a package
-
-    Refer to the pkgname section in https://man.archlinux.org/man/PKGBUILD.5.en#OPTIONS_AND_DIRECTIVES for details
-
-    Attributes
-    ----------
-    pkgname: str
-        A string representing a valid pkgname of a package
-    """
-
-    pkgname: constr(regex=rf"^{PACKAGE_NAME}$")  # type: ignore[valid-type]  # noqa: F722
+    pkgbuild_sha256sum: constr(pattern=rf"{SHA256}")  # type: ignore[valid-type]
 
 
 class PkgVer(BaseModel):
-    """A version string for a package, consisting of epoch, pkgver and pkgrel
+    """A version string for a package, consisting of epoch, pkgver and pkgrel.
 
     Refer to the epoch, pkgrel and pkgver sections in https://man.archlinux.org/man/PKGBUILD.5.en#OPTIONS_AND_DIRECTIVES
     for details
 
     Attributes
     ----------
     pkgver: str
         A valid package version string which includes epoch, version and pkgrel
     """
 
-    pkgver: constr(regex=rf"^({EPOCH}|){VERSION}-{PKGREL}$")  # type: ignore[valid-type]  # noqa: F722
+    pkgver: constr(pattern=rf"^({EPOCH}|){VERSION}-{PKGREL}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class StartDir(BaseModel):
-    """An absolute directory used as startdir for a package
+    """An absolute directory used as startdir for a package.
 
     Refer to the startdir subsection in https://man.archlinux.org/man/PKGBUILD.5.en#PACKAGING_FUNCTIONS
 
     Attributes
     ----------
     startdir: str
         A string representing the absolute startdir directory of a package
     """
 
-    startdir: constr(regex=rf"^{ABSOLUTE_PATH}$")  # type: ignore[valid-type]  # noqa: F722
+    startdir: str
+
+    @field_validator("startdir")
+    @classmethod
+    def validate_startdir(cls, startdir: str) -> str:
+        """Validate the startdir attribute.
+
+        The startdir attribute may not contain strings that represent absolute Paths or Paths in the home directory
+
+        Parameters
+        ----------
+        startdir: str
+            A string, representing a path
+
+        Returns
+        -------
+        str
+            A validated string, representing an absolute Path
+        """
+        path = Path(startdir)
+        if not path.is_absolute():
+            raise ValueError(f"A relative path as startdir is not valid: {path}")
+
+        return startdir
 
 
 class BuildInfo(BaseModel):
-    """The representation of a .BUILDINFO file
+    """The representation of a .BUILDINFO file.
 
     This is a template class and should not be used directly. Instead instantiate one of the classes derived from it.
     """
 
     @classmethod
     def from_file(cls, data: StringIO) -> BuildInfo:
-        """Create an instance of BuildInfo from an io.StringIO representing the contents of a BUILDINFO file
+        """Create an instance of BuildInfo from an io.StringIO representing the contents of a BUILDINFO file.
 
         Parameters
         ----------
         data: io.StringIO
             A text stream representing the contents of a .BUILDINFO file
 
         Returns
         -------
         BuildInfo
             An instance of BuildInfo
         """
-
-        entries: Dict[str, Union[int, str, List[str]]] = {}
+        entries: dict[str, int | str | list[str]] = {}
 
         for line in data:
             [key, value] = [x.strip() for x in line.strip().split("=")]
 
             assignment_key = BUILDINFO_ASSIGNMENTS.get(key)
             if isinstance(assignment_key, tuple):
                 match assignment_key[1]:
@@ -278,175 +292,181 @@
                             entry.append(str(value))
                         else:
                             entries[assignment_key[0]] = [str(value)]
                     # NOTE: the catch all can never be reached but is here to satisfy our tooling
                     case _:  # pragma: no cover
                         continue
 
-        match entries.get("format_"):
+        match entries.get("schema_version"):
             case 1:
-                return BuildInfoV1(**entries)
+                return BuildInfoV1.model_validate(entries)
             case 2:
-                return BuildInfoV2(**entries)
+                return BuildInfoV2.model_validate(entries)
             case _:
-                raise RepoManagementError(f"Encountered unhandled .BUILDINFO format {entries.get('format')}!")
+                raise RepoManagementError(
+                    f"Encountered unhandled .BUILDINFO schema_version {entries.get('schema_version')}!"
+                )
 
 
 class BuildInfoV1(
     BuildDate,
     BuildDir,
     BuildEnv,
     BuildInfo,
-    FormatV1,
     Installed,
     Options,
     Packager,
     PkgArch,
     PkgBase,
     PkgBuildSha256Sum,
     PkgName,
     PkgVer,
+    SchemaVersionV1,
 ):
-    """The representation of a .BUILDINFO file (version 1)
+    """The representation of a .BUILDINFO file (version 1).
 
     Attributes
     ----------
     builddate: NonNegativeInt
         A number >= 0
     builddir: str
         A string representing an absolute directory
-    buildenv: List[str]
+    buildenv: list[str]
         A list of strings as described by makepkg.conf's BUILDENV option
-    format_: int
-        1 - representing version 1
-    installed: List[str]
+    installed: list[str]
         A list of strings representing <package_name>-<epoch><version>-<pkgrel>-<architecture> of packages installed
         during the creation of a package
-    options: List[str]
+    options: list[str]
         A list of strings representing makepkg.conf OPTIONS used during the creation of a package
     packager: str
         A string representing a packager UID (e.g. "First Last <mail@example.tld>")
     pkgarch: str
         A valid CPU architecture for a package
     pkgbase: str
         A string representing a valid pkgbase for a package
     pkgbuild_sha256sum: str
         A string representing a SHA-256 checksum for a PKGBUILD of a package
     pkgname: str
         A string representing a valid pkgname of a package
     pkgver: str
         A valid package version string which includes epoch, version and pkgrel
+    schema_version: int
+        1 - representing `format = 1` in the .BUILDINFO file; schema_version is chosen for uniformity
     """
 
     pass
 
 
 class BuildInfoV2(
     BuildDate,
     BuildDir,
     BuildEnv,
     BuildInfo,
     BuildTool,
     BuildToolVer,
-    FormatV2,
     Installed,
     Options,
     Packager,
     PkgArch,
     PkgBase,
     PkgBuildSha256Sum,
     PkgName,
     PkgVer,
+    SchemaVersionV2,
     StartDir,
 ):
-    """The representation of a .BUILDINFO file (version 2)
+    """The representation of a .BUILDINFO file (version 2).
 
     Attributes
     ----------
     builddate: NonNegativeInt
         A number >= 0
     builddir: str
         A string representing an absolute directory
-    buildenv: List[str]
+    buildenv: list[str]
         A list of strings as described by makepkg.conf's BUILDENV option
     buildtool: str
         The package name of the build tool used to create a package
     buildtoolver: str
         The version of the build tool used to create a package
-    format_: int
-        2 - representing version 2
-    installed: List[str]
+    installed: list[str]
         A list of strings representing <package_name>-<epoch><version>-<pkgrel>-<architecture> of packages installed
         during the creation of a package
-    options: List[str]
+    options: list[str]
         A list of strings representing makepkg.conf OPTIONS used during the creation of a package
     packager: str
         A string representing a packager UID (e.g. "First Last <mail@example.tld>")
     pkgarch: str
         A valid CPU architecture for a package
     pkgbase: str
         A string representing a valid pkgbase for a package
     pkgbuild_sha256sum: str
         A string representing a SHA-256 checksum for a PKGBUILD of a package
     pkgname: str
         A string representing a valid pkgname of a package
     pkgver: str
         A valid package version string which includes epoch, version and pkgrel
+    schema_version: int
+        2 - representing `format = 2` in the .BUILDINFO file; schema_version is chosen for uniformity
     startdir: str
         A string representing the absolute startdir directory of a package
     """
 
-    @root_validator
-    def validate_devtools_version(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """A root validator that ensures the use of a valid version string when devtools is the buildtool
+    @model_validator(mode="before")
+    def validate_devtools_version(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Validate the use of a valid version string when devtools is the buildtool.
 
         Parameters
         ----------
-        values: Dict[str, Any]
+        values: dict[str, Any]
             A dict with all values of a BuildInfoV2 object
 
         Raises
         ------
         ValueError
             If buildtool is "devtools" and buildtoolver does not follow the format
             <optional_epoch><pkgver>-<pkgrel>-<arch>
 
         Returns
-        ------- values: Dict[str, Any]
+        -------
+        values: dict[str, Any]
             The unmodified dict with all values of a BuildInfoV2 instance
         """
-
         buildtool, buildtoolver = str(values.get("buildtool")), str(values.get("buildtoolver"))
         if buildtool == "devtools" and not fullmatch(rf"^({EPOCH}|){VERSION}-{PKGREL}-{ARCHITECTURE}$", buildtoolver):
             raise ValueError(
                 "When building with devtools the buildtoolver must be of the format "
                 f"<optional_epoch><pkgver>-<pkgrel>-<arch>, but it is {buildtoolver}!"
             )
 
         return values
 
 
-def export_schemas(output: Union[Path, str]) -> None:
-    """Export the JSON schema of selected pydantic models to an output directory
+def export_schemas(output: Path | str) -> None:
+    """Export the JSON schema of selected pydantic models to an output directory.
 
     Parameters
     ----------
     output: Path
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-
     classes = [BuildInfoV1, BuildInfoV2]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
 
     for class_ in classes:
-        with open(output / f"{class_.__name__}.json", "w") as f:
-            print(class_.schema_json(indent=2), file=f)
+        with open(output / f"{class_.__name__}.json", "wb") as f:
+            f.write(
+                dumps(
+                    class_.model_json_schema(),  # type: ignore[attr-defined]
+                    option=OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS,
+                )
+            )
```

### Comparing `repod-0.2.2/repod/files/common.py` & `repod-0.3.0.post0/repod/files/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,59 @@
+"""Common function and tools to work with files."""
 from gzip import BadGzipFile
 from gzip import open as gzip_open
 from io import BytesIO, StringIO
 from logging import debug
 from pathlib import Path
 from tarfile import ReadError, TarFile
 from tarfile import open as tarfile_open
-from typing import IO, Dict, List, Literal, Optional, Set, Union
+from typing import IO, Literal
 
 import magic
 from pyzstd import CParameter, ZstdDict, ZstdFile
 
 from repod.common.enums import CompressionTypeEnum
 from repod.errors import RepoManagementFileError, RepoManagementFileNotFoundError
 
 
 class ZstdTarFile(TarFile):
-    """A class to provide reading and writing of zstandard files using TarFile functionality"""
+    """A class to provide reading and writing of zstandard files using TarFile functionality."""
 
     def __init__(  # type: ignore[no-untyped-def]
         self,
-        name: Union[str, Path],
+        name: str | Path,
         mode: Literal["r", "a", "w", "x"] = "r",
-        level_or_option: Union[None, int, Dict[CParameter, int]] = None,
-        zstd_dict: Optional[ZstdDict] = None,
+        level_or_option: None | int | dict[CParameter, int] = None,
+        zstd_dict: ZstdDict | None = None,
         **kwargs,
     ) -> None:
+        """Initialize an instance of ZstdTarFile."""
         self.zstd_file = ZstdFile(
             filename=name,
             mode=mode,
             level_or_option=level_or_option,
             zstd_dict=zstd_dict,
         )
 
         try:
             super().__init__(fileobj=self.zstd_file, mode=mode, **kwargs)
         except Exception as e:
             self.zstd_file.close()
             raise RepoManagementFileError(f"An error occured while trying to open the file {name}!\n{e}")
 
     def close(self) -> None:
+        """Close the file."""
         try:
             super().close()
         finally:
             self.zstd_file.close()
 
 
 def compression_type_of_tarfile(path: Path) -> CompressionTypeEnum:
-    """Retrieve the compression type of a tar file
+    """Retrieve the compression type of a tar file.
 
     Parameters
     ----------
     path: Path
         The path to a tar file
 
     Raises
@@ -59,60 +62,59 @@
         If an unknown compression type is encountered
 
     Returns
     -------
     CompressionTypeEnum
         A member of CompressionTypeEnum, that reflects the compression type of tar file at path
     """
-
     with open(path, "rb") as f:
         file_start_bytes: bytes = f.read(2048)
 
     # Try and detect the instance of the libmagic shared library (loaded via
     # ctypes) used by the magic.py shipped with file.
     if hasattr(magic, "_libraries"):  # pragma: no cover
-        file = magic.detect_from_content(file_start_bytes).name  # type: ignore[attr-defined]
+        types = magic.detect_from_content(file_start_bytes).name  # type: ignore[attr-defined]
     else:
-        file = magic.from_buffer(file_start_bytes)
-    file = " ".join(file.split()[0:3]).lower().strip(",")
-    debug(f"Type of file {path} detected as: {file}")
-
-    match file:
-        case "posix tar archive":
-            return CompressionTypeEnum.NONE
-        case "bzip2 compressed data":
-            return CompressionTypeEnum.BZIP2
-        case "gzip compressed data":
-            return CompressionTypeEnum.GZIP
-        case "xz compressed data":
-            return CompressionTypeEnum.LZMA
-        case "zstandard compressed data":
-            return CompressionTypeEnum.ZSTANDARD
-        case _:
-            raise RepoManagementFileError(
-                f"An error occured while attempting to retrieve the compression type of tar file: {path}!\n"
-                "Unknown compression type encountered."
-            )
+        m = magic.Magic(keep_going=True)
+        types = m.from_buffer(file_start_bytes)
+    types = types.lower().strip(",")
+    debug(f"Types of file {path} detected as: {types}")
+
+    if "posix tar archive" in types:
+        return CompressionTypeEnum.NONE
+    elif "bzip2 compressed data" in types:
+        return CompressionTypeEnum.BZIP2
+    elif "gzip compressed data" in types:
+        return CompressionTypeEnum.GZIP
+    elif "xz compressed data" in types:
+        return CompressionTypeEnum.LZMA
+    elif "zstandard compressed data" in types:
+        return CompressionTypeEnum.ZSTANDARD
+    else:
+        raise RepoManagementFileError(
+            f"An error occured while attempting to retrieve the compression type of tar file: {path}!\n"
+            "Unknown compression type encountered."
+        )
 
 
 def open_tarfile(
     path: Path,
-    compression: Optional[CompressionTypeEnum] = None,
+    compression: CompressionTypeEnum | None = None,
     mode: Literal["r", "w", "x"] = "r",
 ) -> TarFile:
-    """Open a file as a TarFile
+    """Open a file as a TarFile.
 
     This function distinguishes between bzip2, gzip, lzma and zstandard compression depending on file suffix.
     The detection can be overridden by providing either a file suffix or compression type.
 
     Parameters
     ----------
     path: Path
         A Path to a file
-    compression: Optional[CompressionTypeEnum]
+    compression: CompressionTypeEnum | None
         An optional compression type to override the detection based on mime type.
     mode: Literal["r", "w", "x"]
         A mode to open the file with (defaults to "r").
         "r" - open file for reading
         "w" - open file for writing
         "x" - create file
 
@@ -126,15 +128,14 @@
         If the compression type is unknown
 
     Returns
     -------
     tarfile.Tarfile
         An instance of Tarfile
     """
-
     debug(f"Opening file {path}...")
 
     if not path.is_absolute():
         raise RepoManagementFileError(f"An error occured while attempting to resolve a file path: {path} is relative!")
     if path.is_symlink():
         path = path.resolve()
 
@@ -158,16 +159,16 @@
 
 
 async def extract_file_from_tarfile(
     tarfile: TarFile,
     file: str,
     as_stringio: bool = False,
     gzip_compressed: bool = False,
-) -> Union[IO[bytes], StringIO]:
-    """Extract a file from a TarFile and return it as a bytes stream or text I/O buffer
+) -> IO[bytes] | StringIO:
+    """Extract a file from a TarFile and return it as a bytes stream or text I/O buffer.
 
     Parameters
     ----------
     tarfile: TarFile
         An instance of TarFile
     file: str
         A string representing the name of a file contained in tarfile
@@ -181,18 +182,17 @@
     RepoManagementFileNotFoundError
         If the requested file does not exist in the tarfile or if the requested file is neither a file nor a symlink
     RepoManagementFileError
         If gzip_compressed is True and file is not a gzip compressed file or the gzip compressed file is corrupted
 
     Returns
     -------
-    IO[bytes]
-        A bytes stream that represents the file to extract
+    IO[bytes] | StringIO
+        A bytes stream or StringIO that represents the file to extract
     """
-
     debug(f"Extracting file {file} from {str(tarfile.name)}...")
 
     try:
         extracted = tarfile.extractfile(file)
         if extracted is None:
             raise RepoManagementFileNotFoundError(
                 f"File {file} in {str(tarfile.name)} is not a file or a symbolic link!"
@@ -212,30 +212,56 @@
     else:
         if as_stringio:
             return StringIO(initial_value=extracted.read().decode("utf-8"))
         else:
             return extracted
 
 
-def names_in_tarfile(tarfile: TarFile, names: Union[List[str], Set[str]]) -> bool:
-    """Check whether a list of names is found in the list of names of a TarFile
+def names_in_tarfile(tarfile: TarFile, names: list[str] | set[str]) -> bool:
+    """Check whether a list of names is found in the list of names of a TarFile.
 
     Parameters
     ----------
     tarfile: TarFile
         A TarFile to lookup names in
-    names: Union[List[str], Set[str]]
+    names: list[str] | set[str]
         A list or set of names to lookup
 
     Returns
     -------
     bool
         True if all names can be found in the list of TarFile names, else False
     """
-
     if isinstance(names, list):
         names = set(names)
 
     if names == set([name for name in tarfile.getnames() if name in names]):
         return True
     else:
         return False
+
+
+def read_text_from_file(path: str | Path) -> StringIO:
+    """Read text from a file and return it in a StringIO.
+
+    Parameters
+    ----------
+    path: str | Path
+        A Path or str representing a file to read
+
+    Raises
+    ------
+    RepoManagementFileNotFoundError
+        If the file identifed by path does not exist
+
+    Returns
+    -------
+    StringIO
+        A string IO stream representing the contents of the file
+    """
+    if isinstance(path, str):
+        path = Path(path)
+
+    try:
+        return StringIO(initial_value=path.read_text())
+    except FileNotFoundError as e:
+        raise RepoManagementFileNotFoundError(e)
```

### Comparing `repod-0.2.2/repod/files/mtree.py` & `repod-0.3.0.post0/repod/files/mtree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+"""Handling of .MTREE files."""
 from __future__ import annotations
 
 import io
 import re
 from logging import debug
 from pathlib import Path
-from typing import Dict, List, Optional, Union
 
+from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS, dumps
 from pydantic import (
     BaseModel,
     NonNegativeFloat,
     NonNegativeInt,
     ValidationError,
     conint,
     constr,
@@ -17,146 +18,146 @@
 
 from repod.common.models import SchemaVersionV1
 from repod.common.regex import ABSOLUTE_MTREE_PATH, MD5, RELATIVE_MTREE_PATH, SHA256
 from repod.errors import RepoManagementValidationError
 
 
 class SystemGID(BaseModel):
-    """The group ID of a system group
+    """The group ID of a system group.
 
     Attributes
     ----------
     gid: int
         A group ID >0, <1000
     """
 
     gid: conint(ge=0, lt=1000)  # type: ignore[valid-type]
 
 
 class LinkTarget(BaseModel):
-    """The target location of a symlink
+    """The target location of a symlink.
 
     Attributes
     ----------
-    link: Optional[str]
+    link: str | None
         An optional string representing a relative or absolute file
     """
 
-    link: Optional[  # type: ignore[valid-type]
-        constr(regex=rf"^({RELATIVE_MTREE_PATH}|{ABSOLUTE_MTREE_PATH})$")  # noqa: F722
-    ]
+    link: constr(  # type: ignore[valid-type]
+        pattern=rf"^({RELATIVE_MTREE_PATH}|{ABSOLUTE_MTREE_PATH})$"  # noqa: F722
+    ) | None = None
 
 
 class Md5(BaseModel):
-    """An MD5 checksum
+    """An MD5 checksum.
 
     Attributes
     ----------
-    md5: Optional[str]
+    md5: str | None
         An optional string representing an MD5 checksum
     """
 
-    md5: Optional[constr(regex=rf"^{MD5}$")]  # type: ignore[valid-type]  # noqa: F722
+    md5: constr(pattern=rf"^{MD5}$") | None = None  # type: ignore[valid-type]  # noqa: F722
 
 
 class FileMode(BaseModel):
-    """A numeric unix file mode
+    """A numeric unix file mode.
 
     Attributes
     ----------
     mode: str
         A three or four digit long string, consisting only of valid file modes
     """
 
-    mode: constr(regex=r"^[01234567]{3,4}$")  # type: ignore[valid-type]  # noqa: F722
+    mode: constr(pattern=r"^[01234567]{3,4}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class MTreeEntryName(BaseModel):
-    """A file name in mtree representation
+    """A file name in mtree representation.
 
     The mtree format allows for encoding characters using a block of backslash and three octal digits (see
     https://man.archlinux.org/man/mtree.5#General_Format).
 
     Attributes
     ----------
     name: str
         A string representing an absolute file location in mtree format
     """
 
-    name: constr(regex=rf"^{ABSOLUTE_MTREE_PATH}$")  # type: ignore[valid-type]  # noqa: F722
+    name: constr(pattern=rf"^{ABSOLUTE_MTREE_PATH}$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class Sha256(BaseModel):
-    """A SHA-256 checksum
+    """A SHA-256 checksum.
 
     Attributes
     ----------
     sha256:
         An optional string representing a SHA-256 checksum
     """
 
-    sha256: Optional[constr(regex=rf"^{SHA256}$")]  # type: ignore[valid-type]  # noqa: F722
+    sha256: constr(pattern=rf"^{SHA256}$") | None = None  # type: ignore[valid-type]  # noqa: F722
 
 
 class FileSize(BaseModel):
-    """A file size in bytes
+    """A file size in bytes.
 
     Attributes
     ----------
     size: int
         A non-negative integer describing a file size in bytes
     """
 
-    size: Optional[NonNegativeInt]
+    size: NonNegativeInt | None = None
 
 
 class UnixTime(BaseModel):
-    """A timestamp in seconds since the epoch
+    """A timestamp in seconds since the epoch.
 
     Attributes
     ----------
     time: float
         A float > 0 representing a unix timestamp (seconds since the epoch)
     """
 
     time: NonNegativeFloat
 
 
 class MTreeEntryType(BaseModel):
-    """A file type for mtree entries (see https://man.archlinux.org/man/mtree.5#Keywords)
+    """A file type for mtree entries (see https://man.archlinux.org/man/mtree.5#Keywords).
 
     Attributes
     ----------
     type_: str
         A string representing a valid mtree type (one of block, char, dir, fifo, file, link or socket)
     """
 
-    type_: constr(regex=r"^(block|char|dir|fifo|file|link|socket)$")  # type: ignore[valid-type]  # noqa: F722
+    type_: constr(pattern=r"^(block|char|dir|fifo|file|link|socket)$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class SystemUID(BaseModel):
-    """The user ID of a system user
+    """The user ID of a system user.
 
     Attributes
     ----------
     uid: int
         A user ID >0, <1000
     """
 
     uid: conint(ge=0, lt=1000)  # type: ignore[valid-type]
 
 
 class MTreeEntry(BaseModel):
-    """An entry in an MTree
+    """An entry in an MTree.
 
     This is a template class and should not be used directly. Instead instantiate one of the classes derived from it.
     """
 
     def get_file_path(self) -> Path:
-        """Return the file name as a Path
+        """Return the file name as a Path.
 
         The mtree format allows for encoding characters using a block of backslash and three octal digits (see
         https://man.archlinux.org/man/mtree.5#General_Format).
         This method finds and replaces occurences of these encoded characters.
 
         Raises
         ------
@@ -164,28 +165,27 @@
             If called on the template class MTreeEntry
 
         Returns
         -------
         Path
             The Path representation of name
         """
-
         if not hasattr(self, "name"):
             raise RuntimeError("It is not possible to retrieve a file path from the template class MTreeEntry!")
 
-        output_name = self.name  # type: ignore[attr-defined]
+        output_name = self.name
 
         if len(re.findall(r"\\[0-9A-F]{3}", output_name)) > 0:
             output_name = output_name.encode("latin1").decode("unicode-escape").encode("latin1").decode("utf8")
-            debug(f"Converted MTree path {self.name} to {output_name}.")  # type: ignore[attr-defined]
+            debug(f"Converted MTree path {self.name} to {output_name}.")
 
         return Path(output_name)
 
-    def get_link_path(self, resolve: bool = False) -> Optional[Path]:
-        """Return the link as a Path
+    def get_link_path(self, resolve: bool = False) -> Path | None:
+        """Return the link as a Path.
 
         The mtree format allows for encoding characters using a block of backslash and three octal digits (see
         https://man.archlinux.org/man/mtree.5#General_Format).
         This method finds and replaces occurences of these encoded characters.
         Any relative paths are converted to absolute ones.
 
         Parameters
@@ -196,22 +196,21 @@
         Raises
         ------
         RuntimeError
             If called on the template class MTreeEntry
 
         Returns
         -------
-        Optional[Path]
+        Path | None
             The Path representation of link, or None if there is None
         """
-
         if not hasattr(self, "link"):
             raise RuntimeError("It is not possible to retrieve a file path from the template class MTreeEntry!")
 
-        output_name = self.link  # type: ignore[attr-defined]
+        output_name = self.link
         if output_name is None:
             return output_name
 
         if len(re.findall(r"\\[0-9A-F]{3}", output_name)) > 0:
             output_name = output_name.encode("latin1").decode("unicode-escape").encode("latin1").decode("utf8")
             debug(f"Converted MTree path {self.name} to {output_name}.")  # type: ignore[attr-defined]
 
@@ -222,31 +221,30 @@
         else:
             if output_name.startswith(".."):
                 return (self.get_file_path() / output_path).resolve()
             else:
                 return (self.get_file_path() / ".." / output_path).resolve()
 
     def get_type(self) -> str:
-        """Return the type as a string
+        """Return the type as a string.
 
         Raises
         ------
         RuntimeError
             If called on the template class MTreeEntry
 
         Returns
         -------
         str
             The type of the MTreeEntry
         """
-
         if not hasattr(self, "type_"):
             raise RuntimeError("It is not possible to retrieve a type from the template class MTreeEntry!")
 
-        return str(self.type_)  # type: ignore[attr-defined]
+        return str(self.type_)
 
 
 class MTreeEntryV1(
     MTreeEntry,
     SchemaVersionV1,
     FileMode,
     FileSize,
@@ -255,23 +253,23 @@
     MTreeEntryName,
     MTreeEntryType,
     Sha256,
     UnixTime,
     SystemGID,
     SystemUID,
 ):
-    """An entry in an MTree (version 1)
+    """An entry in an MTree (version 1).
 
     Attributes
     ----------
     gid: int
         A group ID >0, <1000
-    link: Optional[str]
+    link: str | None
         An optional string representing a relative or absolute file
-    md5: Optional[str]
+    md5: str | None
         A optional string representing an MD5 checksum
     mode: str
         A three or four digit long string, consisting only of valid file modes
     name: str
         A string representing an absolute file location in mtree format
     schema_version: int
         A schema version (defaults to 1)
@@ -287,27 +285,27 @@
         A user ID >0, <1000
     """
 
     pass
 
 
 class MTree(BaseModel):
-    """A class to describe an mtree file
+    """A class to describe an mtree file.
 
     Attributes
     ----------
-    files: List[File]
+    files: list[File]
         A list of File instances, representing the entries in an mtree file
     """
 
-    entries: List[MTreeEntry]
+    entries: list[MTreeEntry]
 
     @classmethod
     def from_file(cls, data: io.StringIO) -> MTree:
-        """Create an instance of MTree from an io.StringIO representing the contents of an mtree file
+        """Create an instance of MTree from an io.StringIO representing the contents of an mtree file.
 
         Parameters
         ----------
         data: io.StringIO
             A text stream representing the contents of an mtree file
 
         Raises
@@ -317,63 +315,74 @@
 
         Returns
         -------
         MTree
             An instance of MTree, derived from data
         """
 
-        base_settings: Dict[str, Union[int, str]] = {}
-        entries: List[MTreeEntry] = []
+        def sanitize_mtree_pairs(
+            settings_list: list[list[str]],
+            settings_dict: dict[str, float | int | str],
+        ) -> None:
+            """Sanitize mtree pairs in a list and add them to a dict.
+
+            Parameters
+            ----------
+            settings_list: list[list[str]]
+                A list of string lists, that represent mtree key-value pairs
+            settings_dict: dict[str, float | int | str]
+                A dict to which sanitized mtree key-value pairs are added
+            """
+            for setting in settings_list:
+                settings_key = setting[0]
+                setting_value = setting[1].strip("\n")
+                match settings_key:
+                    case "gid" | "uid" | "size":
+                        settings_dict[settings_key] = int(setting_value)
+                    case "time":
+                        settings_dict[settings_key] = float(setting_value)
+                    case "type":
+                        # NOTE: do not overload type()
+                        settings_dict["type_"] = setting_value
+                    case "mode":
+                        # NOTE: ensure that file modes are zero-filled and of length 4
+                        settings_dict[settings_key] = setting_value.zfill(4)
+                    case "md5digest" | "sha1digest" | "sha256digest" | "sha384digest" | "sha512digest":
+                        # NOTE: only use the name of the digest as key to be more flexible in reusing the model
+                        settings_dict[settings_key.replace("digest", "")] = setting_value
+                    case _:
+                        settings_dict[settings_key] = setting_value
+
+        base_settings: dict[str, float | int | str] = {}
+        entries: list[MTreeEntry] = []
 
         for line in data:
             if line.startswith("/set"):
-                settings = [assignment.split("=") for assignment in line.split(" ")[1:]]
-                for setting in settings:
-                    setting_value = setting[1].strip("\n")
-                    match setting[0]:
-                        case "gid" | "uid":
-                            base_settings[setting[0]] = int(setting_value)
-                        case "type":
-                            base_settings["type_"] = setting_value
-                        case _:
-                            base_settings[setting[0]] = setting_value
+                settings_list = [assignment.split("=") for assignment in line.split(" ")[1:]]
+                sanitize_mtree_pairs(settings_list=settings_list, settings_dict=base_settings)
 
             elif line.startswith("."):
-                file_settings: Dict[str, Union[float, int, str]] = {}
+                file_settings: dict[str, float | int | str] = {}
                 file_settings["name"] = line.split()[0][1:]
 
                 # provide a list of all settings in an entry line (skip empty assigments due to multiple whitespace)
                 settings_list = [assignment.split("=") for assignment in line.split()[1:] if assignment]
-                for setting in settings_list:
-                    setting_value = setting[1].strip("\n")
-                    match setting[0]:
-                        case "gid" | "uid" | "size":
-                            file_settings[setting[0]] = int(setting_value)
-                        case "time":
-                            file_settings[setting[0]] = float(setting_value)
-                        case "type":
-                            # NOTE: do not overload type()
-                            file_settings["type_"] = setting_value
-                        case "md5digest" | "sha1digest" | "sha256digest" | "sha384digest" | "sha512digest":
-                            # NOTE: only use the name of the digest as key to be more flexible in reusing the model
-                            file_settings[setting[0].replace("digest", "")] = setting_value
-                        case _:
-                            file_settings[setting[0]] = setting_value
+                sanitize_mtree_pairs(settings_list=settings_list, settings_dict=file_settings)
 
                 try:
                     entries.append(
                         MTreeEntryV1(
                             gid=file_settings.get("gid") or base_settings.get("gid"),
                             link=file_settings.get("link"),
-                            md5=file_settings.get("md5"),
+                            md5=file_settings.get("md5") or base_settings.get("md5"),
                             mode=file_settings.get("mode") or base_settings.get("mode"),
                             name=file_settings.get("name"),
-                            sha256=file_settings.get("sha256"),
-                            size=file_settings.get("size"),
-                            time=file_settings.get("time"),
+                            sha256=file_settings.get("sha256") or base_settings.get("sha256"),
+                            size=file_settings.get("size") or base_settings.get("size"),  # type: ignore[arg-type]
+                            time=file_settings.get("time") or base_settings.get("time"),  # type: ignore[arg-type]
                             type_=file_settings.get("type_") or base_settings.get("type_"),
                             uid=file_settings.get("uid") or base_settings.get("uid"),
                         )
                     )
                 except ValidationError as e:
                     raise RepoManagementValidationError(
                         f"An error occured when validating mtree data!\n"
@@ -382,58 +391,61 @@
                         f"{e}"
                     )
             else:
                 continue
 
         return MTree(entries=entries)
 
-    def get_paths(self, show_all: bool = False) -> List[Path]:
-        """Return the list of Paths described by the entries of the MTree
+    def get_paths(self, show_all: bool = False) -> list[Path]:
+        """Return the list of Paths described by the entries of the MTree.
 
         Parameters
         ----------
         show_all: bool
             Also show files that are not installed on target systems (defaults to False)
 
         Returns
         -------
-        List[Path]
+        list[Path]
             A list of Paths
         """
-
-        path_list: List[Path] = []
+        path_list: list[Path] = []
 
         for entry in self.entries:
             path = entry.get_file_path()
             if path in [Path("/.BUILDINFO"), Path("/.INSTALL"), Path("/.MTREE"), Path("/.PKGINFO")] and not show_all:
                 continue
 
             path_list.append(path)
 
         return path_list
 
 
-def export_schemas(output: Union[Path, str]) -> None:
-    """Export the JSON schema of selected pydantic models to an output directory
+def export_schemas(output: Path | str) -> None:
+    """Export the JSON schema of selected pydantic models to an output directory.
 
     Parameters
     ----------
     output: Path
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-
     classes = [MTreeEntryV1]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
 
     for class_ in classes:
-        with open(output / f"{class_.__name__}.json", "w") as f:
-            print(class_.schema_json(indent=2), file=f)
+        with open(output / f"{class_.__name__}.json", "wb") as f:
+            f.write(
+                dumps(
+                    class_.model_json_schema(),
+                    option=OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS,
+                )
+            )
```

### Comparing `repod-0.2.2/repod/files/package.py` & `repod-0.3.0.post0/repod/files/package.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,66 @@
+"""Handling of package files and their contents."""
 from __future__ import annotations
 
 from base64 import b64encode
 from hashlib import md5, sha256
 from logging import debug, info
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any
 
-from pydantic import BaseModel
+from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS, dumps
+from pydantic import BaseModel, SerializeAsAny
 
 from repod.common.models import CSize, FileName, Md5Sum, PgpSig, Sha256Sum
 from repod.errors import RepoManagementFileError
 from repod.files.buildinfo import BuildInfo
-from repod.files.common import (  # noqa: F401
-    extract_file_from_tarfile,
-    names_in_tarfile,
-    open_tarfile,
-)
+from repod.files.common import extract_file_from_tarfile, names_in_tarfile, open_tarfile
 from repod.files.mtree import MTree
 from repod.files.pkginfo import PkgInfo
 
 PACKAGE_VERSIONS = {
     1: {
         "required": {".BUILDINFO", ".MTREE", ".PKGINFO"},
     },
 }
 
 
 class Package(BaseModel):
-    """Package representation
+    """Package representation.
 
     This is a template class and (apart from its class methods) should not be used directly. Instead instatiate one of
     the classes derived from it.
     """
 
     @classmethod
-    async def from_file(cls, package: Path, signature: Optional[Path] = None) -> Package:
-        """Create a Package from a package file and an optional signature
+    async def from_file(cls, package: Path, signature: Path | None = None) -> Package:
+        """Create a Package from a package file and an optional signature.
 
         Parameters
         ----------
         package: Path
             The path to a package file
-        signature: Optional[Path]
+        signature: Path | None
             The optional path to a signature file for package
 
         Raises
         ------
         RepoManagementFileError
             If the signature file does not match the package file.
             If the signature file does not exist.
 
         Returns
         -------
         Package
             A Package representing the metadata contained in package and the optional signature file
         """
-
         package_version = 0
         package_md5sum = ""
         package_sha256sum = ""
-        pgpsig: Optional[str] = None
+        pgpsig: str | None = None
 
         if signature:
             debug(f"Opening signature file {signature} for reading...")
             if not Path(str(package) + ".sig") == signature:
                 raise RepoManagementFileError(
                     f"The signature file for {package} should be {str(package) + '.sig'}, but {signature} is provided!"
                 )
@@ -75,15 +72,16 @@
                 debug(f"Created pgpsig: {pgpsig}")
         else:
             info(f"No signature file for package {package} provided, commencing without...")
 
         debug(f"Creating checksums for package {package}...")
         with open(package, "rb") as package_file:
             package_bytes = package_file.read()
-            package_md5sum = md5(package_bytes).hexdigest()
+            # NOTE: MD5 sums are still part of the PackageV1 API
+            package_md5sum = md5(package_bytes).hexdigest()  # nosec: B324
             package_sha256sum = sha256(package_bytes).hexdigest()
 
         debug(f"Opening package file {package} for reading...")
         with open_tarfile(package) as tarfile:
             for version in range(len(PACKAGE_VERSIONS), 0, -1):
                 debug(f"Testing data against Package version {version}...")
                 if names_in_tarfile(tarfile=tarfile, names=PACKAGE_VERSIONS[version]["required"]):
@@ -123,81 +121,84 @@
                         sha256sum=package_sha256sum,
                     )
                 case _:
                     raise RepoManagementFileError(
                         f"The provided file {package} does not match any known package versions!"
                     )
 
-    def top_level_dict(self) -> Dict[str, Any]:
-        """Flatten the keys and values tracked by Package (one level deep) and return them in a dict
+    def top_level_dict(self) -> dict[str, Any]:
+        """Flatten the keys and values tracked by Package (one level deep) and return them in a dict.
 
         NOTE: Duplicate entries are merged!
 
         Returns
         -------
-        Dict[str, Any]
+        dict[str, Any]
             A flattened dict representation of Package
         """
-
-        top_level: Dict[str, Any] = {}
-        for key, value in self.dict().items():
+        top_level: dict[str, Any] = {}
+        for key, value in self.model_dump(mode="python").items():
             if isinstance(value, dict):
                 top_level.update(value)
             else:
                 top_level.update({key: value})
 
         return top_level
 
 
 class PackageV1(CSize, FileName, Md5Sum, Package, PgpSig, Sha256Sum):
-    """Package representation version 1
+    """Package representation version 1.
 
     Attributes
     ----------
     buildinfo: BuildInfo
         A .BUILDINFO file representation
     csize: CSize
         The file size of the Package
     filename: FileName
         The filename of the Package
     md5sum: str
         An MD5 checksum for the package
     mtree: MTree
         An .MTREE file representation
-    pgpsig: Optional[str]
+    pgpsig: str | None
         An optional PGP signature (in base64 representation) for the package
     pkginfo: PkgInfo
         A .PKGINFO file representation
     sha256sum: str
         A SHA256 checksum for the package
     """
 
-    buildinfo: BuildInfo
-    mtree: MTree
-    pkginfo: PkgInfo
+    buildinfo: SerializeAsAny[BuildInfo]
+    mtree: SerializeAsAny[MTree]
+    pkginfo: SerializeAsAny[PkgInfo]
 
 
-def export_schemas(output: Union[Path, str]) -> None:
-    """Export the JSON schema of selected pydantic models to an output directory
+def export_schemas(output: Path | str) -> None:
+    """Export the JSON schema of selected pydantic models to an output directory.
 
     Parameters
     ----------
     output: Path
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-
     classes = [PackageV1]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
 
     for class_ in classes:
-        with open(output / f"{class_.__name__}.json", "w") as f:
-            print(class_.schema_json(indent=2), file=f)
+        with open(output / f"{class_.__name__}.json", "wb") as f:
+            f.write(
+                dumps(
+                    class_.model_json_schema(),
+                    option=OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS,
+                )
+            )
```

### Comparing `repod-0.2.2/repod/files/pkginfo.py` & `repod-0.3.0.post0/repod/files/pkginfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+"""Handling of .PKGINFO files."""
 from __future__ import annotations
 
 from io import StringIO
 from logging import debug
 from pathlib import Path
-from typing import Any, Dict, List, Set, Tuple, Union
+from typing import Any
 
+from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS, dumps
 from pydantic import BaseModel, constr
 
 from repod.common.enums import FieldTypeEnum, PkgTypeEnum
 from repod.common.models import (
     Arch,
     Backup,
     Base,
@@ -30,15 +32,15 @@
     SchemaVersionV2,
     Url,
     Version,
 )
 from repod.common.regex import VERSION
 from repod.errors import RepoManagementError, RepoManagementFileError
 
-PKGINFO_ASSIGNMENTS: Dict[str, Tuple[str, FieldTypeEnum]] = {
+PKGINFO_ASSIGNMENTS: dict[str, tuple[str, FieldTypeEnum]] = {
     "pkgname": ("name", FieldTypeEnum.STRING),
     "pkgbase": ("base", FieldTypeEnum.STRING),
     "pkgtype": ("pkgtype", FieldTypeEnum.STRING),
     "pkgver": ("version", FieldTypeEnum.STRING),
     "pkgdesc": ("desc", FieldTypeEnum.STRING),
     "url": ("url", FieldTypeEnum.STRING),
     "builddate": ("builddate", FieldTypeEnum.INT),
@@ -53,19 +55,19 @@
     "backup": ("backup", FieldTypeEnum.STRING_LIST),
     "depend": ("depends", FieldTypeEnum.STRING_LIST),
     "optdepend": ("optdepends", FieldTypeEnum.STRING_LIST),
     "makedepend": ("makedepends", FieldTypeEnum.STRING_LIST),
     "checkdepend": ("checkdepends", FieldTypeEnum.STRING_LIST),
     "xdata": ("xdata", FieldTypeEnum.KEY_VALUE_LIST),
 }
-PKGINFO_COMMENT_ASSIGNMENTS: Dict[str, Tuple[str, FieldTypeEnum]] = {
+PKGINFO_COMMENT_ASSIGNMENTS: dict[str, tuple[str, FieldTypeEnum]] = {
     "makepkg": ("makepkg_version", FieldTypeEnum.STRING),
     "fakeroot": ("fakeroot_version", FieldTypeEnum.STRING),
 }
-PKGINFO_VERSIONS: Dict[int, Dict[str, Set[str]]] = {
+PKGINFO_VERSIONS: dict[int, dict[str, set[str]]] = {
     1: {
         "required": {
             "arch",
             "base",
             "builddate",
             "desc",
             "fakeroot_version",
@@ -116,16 +118,16 @@
             "replaces",
             "xdata",
         },
     },
 }
 
 
-def parse_pairs(line: str, separator: str = " = ") -> Tuple[str, str, FieldTypeEnum]:
-    """Parse key-value pairs from a line of text
+def parse_pairs(line: str, separator: str = " = ") -> tuple[str, str, FieldTypeEnum]:
+    """Parse key-value pairs from a line of text.
 
     The line of text represents the data contained in a .PKGINFO file.
     All known key-value pairs are understood and also identifiers added in comment sections are extracted.
     Keys are resolved based on PKGINFO_ASSIGMENTS or PKGINFO_COMMENT_ASSIGNMENTS.
 
     Parameters
     ----------
@@ -138,19 +140,18 @@
     ------
     RepoManagementFileError
         If the extracted key can not be found in PKGINFO_ASSIGMENTS,
         or if an invalid line of text is provided.
 
     Returns
     -------
-    Tuple[str, str, FieldTypeEnum]
+    tuple[str, str, FieldTypeEnum]
         A tuple of two strings and a member of FieldTypeEnum, which represent key, value and field type extracted from
         the line of text
     """
-
     debug(f"Parsing: {line}")
     if line.startswith("#"):
         for keyword in PKGINFO_COMMENT_ASSIGNMENTS.keys():
             if keyword in line:
                 debug(f"Detected valid keyword {keyword}")
                 key = PKGINFO_COMMENT_ASSIGNMENTS[keyword][0]
                 value = line.strip().split()[-1]
@@ -168,155 +169,153 @@
             field_type = assignment_key[1]
         except ValueError as e:
             raise RepoManagementFileError(f"An error occurred while trying to parse the .PKGINFO line {line}\n{e}")
 
     return key, value, field_type
 
 
-def pairs_to_entries(key: str, value: str, field_type: FieldTypeEnum, entries: Dict[str, Any]) -> None:
-    """Append key value-pairs to a dict
+def pairs_to_entries(key: str, value: str, field_type: FieldTypeEnum, entries: dict[str, Any]) -> None:
+    """Append key value-pairs to a dict.
 
     Values are cast based on their provided field types.
     Nested values for xdata are understood and are initialized as their target types (e.g. PkgType).
 
     Parameters
     ----------
     key: str
         The resolved key
     value: str
         The extracted value
     field_type: FieldTypeEnum
         A member of FieldTypeEnum based upon which value is cast to a specific type
-    entries: Dict[str, Any]
+    entries: dict[str, Any]
         The dict to which the key-value pairs are added
 
     Raises
     ------
     RuntimeError
         If an invalid key/ field type combination is encountered
     """
-
     debug(f"Attempting to add key {key} and value {value} of field type {field_type} to {entries}")
     match key, field_type:
-        case "pkgtype", FieldTypeEnum.STRING:
+        case ["pkgtype", FieldTypeEnum.STRING]:
             if entries.get("xdata") is None:
                 entries["xdata"] = []
 
-            entries["xdata"].append(PkgType(pkgtype=value))
-        case _, FieldTypeEnum.INT:
+            entries["xdata"].append(PkgType(pkgtype=value))  # type: ignore[arg-type]
+        case [_, FieldTypeEnum.INT]:
             entries[key] = int(value)
-        case _, FieldTypeEnum.STRING:
+        case [_, FieldTypeEnum.STRING]:
             entries[key] = str(value)
-        case _, FieldTypeEnum.STRING_LIST:
+        case [_, FieldTypeEnum.STRING_LIST]:
             entry = entries.get(key)
             if entry is not None and isinstance(entry, list):
                 entry.append(str(value))
             else:
                 entries[key] = [str(value)]
-        case _, FieldTypeEnum.KEY_VALUE_LIST:
+        case [_, FieldTypeEnum.KEY_VALUE_LIST]:
             key_, value_, field_type_ = parse_pairs(line=value, separator="=")
             pairs_to_entries(key=key_, value=value_, field_type=field_type_, entries=entries)
 
         # NOTE: the catch all can never be reached but is here to satisfy our tooling
-        case _, _:  # pragma: no cover
+        case [_, _]:  # pragma: no cover
             raise RuntimeError(
                 "An invalid field type has been encountered while attempting to read a .PKGINFO file.\n"
                 "This most likely means a new field type has been introduced, but the .PKGINFO parser has "
                 "not been extended to make use of it!"
             )
 
 
 class FakerootVersion(BaseModel):
-    """A version of fakeroot
+    """A version of fakeroot.
 
     Attributes
     ----------
     fakeroot_version: str
         A string representing a version of fakeroot
     """
 
-    fakeroot_version: constr(regex=rf"^({VERSION})$")  # type: ignore[valid-type]  # noqa: F722
+    fakeroot_version: constr(pattern=rf"^({VERSION})$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class MakepkgVersion(BaseModel):
-    """A version of makepkg
+    """A version of makepkg.
 
     Attributes
     ----------
     makepkg_version: str
         A string representing a version of makepkg
     """
 
-    makepkg_version: constr(regex=rf"^({VERSION})$")  # type: ignore[valid-type]  # noqa: F722
+    makepkg_version: constr(pattern=rf"^({VERSION})$")  # type: ignore[valid-type]  # noqa: F722
 
 
 class PkgType(BaseModel):
-    """A package type
+    """A package type.
 
     Attributes
     ----------
     pkgtype: PkgTypeEnum
         A member of PkgTypeEnum representing a valid package type
     """
 
     pkgtype: PkgTypeEnum
 
 
 class XData(BaseModel):
-    """An optional list of extra data
+    """An optional list of extra data.
 
     Attributes
     ----------
-    xdata: List[PkgType]
+    xdata: list[PkgType]
         An list of extra data
     """
 
-    xdata: List[PkgType] = []
+    xdata: list[PkgType] = []
 
 
 class PkgInfo(BaseModel):
-    """The representation of a .PKGINFO file
+    """The representation of a .PKGINFO file.
 
     This is a template class and should not be used directly. Instead instatiate one of the classes derived from it.
     """
 
     @classmethod
     def from_file(cls, data: StringIO) -> PkgInfo:
-        """Create an instance of PkgInfo from an io.StringIO representing the contents of a PKGINFO file
+        """Create an instance of PkgInfo from an io.StringIO representing the contents of a PKGINFO file.
 
         Parameters
         ----------
         data: io.StringIO
             A text stream representing the contents of a .PKGINFO file
 
         Returns
         -------
         PkgInfo
             An instance of PkgInfo
         """
-
         pkg_info_version = 0
-        entries: Dict[str, Union[int, str, List[Union[str, Dict[str, Any]]]]] = {}
+        entries: dict[str, int | str | list[str | dict[str, Any]]] = {}
 
         for line in data:
             key, value, field_type = parse_pairs(line=line)
             pairs_to_entries(key=key, value=value, field_type=field_type, entries=entries)
 
         for version in range(len(PKGINFO_VERSIONS), 0, -1):
             debug(f"Testing data against .PKGINFO version {version}.")
             if PKGINFO_VERSIONS[version]["required"].issubset(set(entries.keys())):
                 debug(f".PKGINFO version {version} matches provided data!")
                 pkg_info_version = version
                 break
 
         match pkg_info_version:
             case 1:
-                return PkgInfoV1(**entries)
+                return PkgInfoV1.model_validate(entries)
             case 2:
-                return PkgInfoV2(**entries)
+                return PkgInfoV2.model_validate(entries)
             case _:
                 raise RepoManagementError(
                     f"Encountered unhandled .PKGINFO version {pkg_info_version} when trying to match data {entries}!"
                 )
 
 
 class PkgInfoV1(
@@ -340,55 +339,55 @@
     PkgInfo,
     Provides,
     Replaces,
     SchemaVersionV1,
     Url,
     Version,
 ):
-    """A PkgInfo version 1
+    """A PkgInfo version 1.
 
     Attributes
     ----------
     arch: str
         A string representing a CPU architecture
-    backup: Optional[List[str]]
+    backup: list[str] | None
         An optional list of strings representing relative file paths
     base: str
         A string representing a pkgbase
     builddate: int
         A number representing a build date (in seconds since the epoch)
-    checkdepends: Optional[List[str]]
+    checkdepends: list[str] | None
         An optional list of strings representing package names a package requires for tests
-    conflicts: Optional[List[str]]
+    conflicts: list[str] | None
         An optional list of strings representing package names a package conflicts with
-    depends: Optional[List[str]]
+    depends: list[str] | None
         An optional list of strings representing package names a package depends on
     desc: str
         A string that serves as description for a package
     fakeroot_version: str
         A string representing a version of fakeroot
-    groups: Optional[List[str]]
+    groups: list[str] | None
         An optional list of strings representing group names a package belongs to
     isize: int
         A number representing the installed sized of a package in bytes
     packager: str
         A string describing the UID of a package's packager
-    license: List[str]
+    license: list[str]
         A list of strings describing the license identifiers that apply to a package
-    makedepends: Optional[List[str]]
+    makedepends: list[str] | None
         An optional list of strings representing package names a package requires for building
     makepkg_version: str
         A string representing a version of makepkg
     name: str
         A string representing the name of a package
-    optdepends: Optional[List[str]]
+    optdepends: list[str] | None
         An optional list of strings representing package names a package requires optionally
-    provides: Optional[List[str]]
+    provides: list[str] | None
         An optional list of strings representing package names a package provides
-    replaces: Optional[List[str]]
+    replaces: list[str] | None
         An optional list of strings representing package names a package replaces
     url: str
         A string representing the upstream URL of a package
     version: str
         A string representing the full version (optional epoch, version and pkgrel) of a package
     """
 
@@ -417,85 +416,89 @@
     Provides,
     Replaces,
     SchemaVersionV2,
     Url,
     Version,
     XData,
 ):
-    """A PkgInfo version 2
+    """A PkgInfo version 2.
 
     Attributes
     ----------
     arch: str
         A string representing a CPU architecture
-    backup: Optional[List[str]]
+    backup: list[str] | None
         An optional list of strings representing relative file paths
     base: str
         A string representing a pkgbase
     builddate: int
         A number representing a build date (in seconds since the epoch)
-    checkdepends: Optional[List[str]]
+    checkdepends: list[str] | None
         An optional list of strings representing package names a package requires for tests
-    conflicts: Optional[List[str]]
+    conflicts: list[str] | None
         An optional list of strings representing package names a package conflicts with
-    depends: Optional[List[str]]
+    depends: list[str] | None
         An optional list of strings representing package names a package depends on
     desc: str
         A string that serves as description for a package
     fakeroot_version: str
         A string representing a version of fakeroot
-    groups: Optional[List[str]]
+    groups: list[str] | None
         An optional list of strings representing group names a package belongs to
     isize: int
         A number representing the installed sized of a package in bytes
     packager: str
         A string describing the UID of a package's packager
-    license: List[str]
+    license: list[str]
         A list of strings describing the license identifiers that apply to a package
-    makedepends: Optional[List[str]]
+    makedepends: list[str] | None
         An optional list of strings representing package names a package requires for building
     makepkg_version: str
         A string representing a version of makepkg
     name: str
         A string representing the name of a package
-    optdepends: Optional[List[str]]
+    optdepends: list[str] | None
         An optional list of strings representing package names a package requires optionally
-    provides: Optional[List[str]]
+    provides: list[str] | None
         An optional list of strings representing package names a package provides
-    replaces: Optional[List[str]]
+    replaces: list[str] | None
         An optional list of strings representing package names a package replaces
     url: str
         A string representing the upstream URL of a package
     version: str
         A string representing the full version (optional epoch, version and pkgrel) of a package
-    xdata: Optional[List[PkgType]]
+    xdata: list[PkgType] | None
         An optional list of extra data
     """
 
     pass
 
 
-def export_schemas(output: Union[Path, str]) -> None:
-    """Export the JSON schema of selected pydantic models to an output directory
+def export_schemas(output: Path | str) -> None:
+    """Export the JSON schema of selected pydantic models to an output directory.
 
     Parameters
     ----------
     output: Path
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-
     classes = [PkgInfoV1, PkgInfoV2]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
 
     for class_ in classes:
-        with open(output / f"{class_.__name__}.json", "w") as f:
-            print(class_.schema_json(indent=2), file=f)
+        with open(output / f"{class_.__name__}.json", "wb") as f:
+            f.write(
+                dumps(
+                    class_.model_json_schema(),  # type: ignore[attr-defined]
+                    option=OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS,
+                )
+            )
```

### Comparing `repod-0.2.2/repod/repo/__init__.py` & `repod-0.3.0.post0/repod/repo/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+"""Handling of management and package repository files."""
 from pathlib import Path
-from typing import Union
 
 from repod.repo.management import (  # noqa: F401
     Files,
     OutputPackage,
     OutputPackageBase,
     PackageDesc,
 )
@@ -20,18 +20,17 @@
     get_desc_json_name,
     get_files_json_field_type,
     get_files_json_keys,
     get_files_json_name,
 )
 
 
-def export_schemas(output: Union[Path, str]) -> None:
-    """Export the JSON schema files of the repod.repo package to a directory
+def export_schemas(output: Path | str) -> None:
+    """Export the JSON schema files of the repod.repo package to a directory.
 
     Parameters
     ----------
     output: Path
         A directory to write the JSON schema files to
     """
-
     management_export_schemas(output=output)
     package_export_schemas(output=output)
```

### Comparing `repod-0.2.2/repod/repo/management/outputpackage.py` & `repod-0.3.0.post0/repod/repo/management/outputpackage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+"""Reading and writing of OutputPackageBase and OutputPackage."""
 from __future__ import annotations
 
 from logging import debug
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple, Union
+from typing import Any
 
 from aiofiles import open as async_open
-from orjson import JSONDecodeError, loads
-from pydantic import BaseModel, ValidationError
+from orjson import (
+    OPT_APPEND_NEWLINE,
+    OPT_INDENT_2,
+    OPT_SORT_KEYS,
+    JSONDecodeError,
+    dumps,
+    loads,
+)
+from pydantic import BaseModel, SerializeAsAny, ValidationError
 
 from repod import errors
 from repod.common.enums import (
     FilesVersionEnum,
     OutputPackageVersionEnum,
     PackageDescVersionEnum,
 )
@@ -33,43 +41,43 @@
     Name,
     OptDepends,
     Packager,
     PgpSig,
     Provides,
     Replaces,
     SchemaVersionV1,
+    SchemaVersionV2,
     Sha256Sum,
+    SourceUrl,
     Url,
     Version,
 )
 from repod.files import package
 from repod.files.buildinfo import (
     BuildDir,
     BuildEnv,
     BuildInfo,
     BuildInfoV1,
     BuildInfoV2,
     BuildTool,
     BuildToolVer,
-    FormatV1,
-    FormatV2,
     Installed,
     Options,
     PkgBuildSha256Sum,
     StartDir,
 )
 from repod.repo.package.syncdb import (
     Files,
     FilesV1,
     PackageDesc,
     PackageDescV1,
     PackageDescV2,
 )
 
-OUTPUT_PACKAGE_VERSIONS: Dict[int, Dict[str, Set[str]]] = {
+OUTPUT_PACKAGE_VERSIONS: dict[int, dict[str, set[str]]] = {
     1: {
         "required": {
             "arch",
             "builddate",
             "csize",
             "desc",
             "filename",
@@ -90,38 +98,38 @@
             "optdepends",
             "pgpsig",
             "provides",
             "replaces",
         },
     },
 }
-OUTPUT_PACKAGE_BASE_VERSIONS: Dict[int, Dict[str, Union[int, Set[str]]]] = {
+OUTPUT_PACKAGE_BASE_VERSIONS: dict[int, dict[str, int | set[str]]] = {
     1: {
         "required": {
             "base",
             "makedepends",
             "packager",
             "packages",
             "version",
         },
     },
 }
 DEFAULT_OUTPUT_PACKAGE_BASE_VERSION = 1
 
 
 class OutputBuildInfo(BaseModel):
-    """A class tracking BuildInfo information of packages that are added to instances of OutputPackageBase
+    """A class tracking BuildInfo information of packages that are added to instances of OutputPackageBase.
 
     This class is a base template class and should not be used directly.
     Instead, instantiate one of its versioned child classes using the `from_buildinfo()` classmethod.
     """
 
     @classmethod
     def from_buildinfo(cls, buildinfo: BuildInfo) -> OutputBuildInfo:
-        """Create and return an instance of one of OutputBuildInfo's versioned child classes
+        """Create and return an instance of one of OutputBuildInfo's versioned child classes.
 
         Parameters
         ----------
         buildinfo: BuildInfo
             An instance of BuildInfo which will be used to create an instance of one of the versioned child classes of
             OutputBuildInfo
 
@@ -131,143 +139,141 @@
             If an unknown BuildInfo instance is encountered
 
         Returns
         -------
         OutputBuildInfo
             One of OutputBuildInfo's versioned child classes (e.g. OutputBuildInfoV1 or OutputBuildInfoV2)
         """
-
         if isinstance(buildinfo, BuildInfoV1):
             return OutputBuildInfoV1(
                 builddir=buildinfo.builddir,
                 buildenv=buildinfo.buildenv,
-                format_=buildinfo.format_,
                 installed=buildinfo.installed,
                 options=buildinfo.options,
                 pkgbuild_sha256sum=buildinfo.pkgbuild_sha256sum,
+                schema_version=buildinfo.schema_version,
             )
         elif isinstance(buildinfo, BuildInfoV2):
             return OutputBuildInfoV2(
                 builddir=buildinfo.builddir,
                 buildenv=buildinfo.buildenv,
                 buildtool=buildinfo.buildtool,
                 buildtoolver=buildinfo.buildtoolver,
-                format_=buildinfo.format_,
                 installed=buildinfo.installed,
                 options=buildinfo.options,
                 pkgbuild_sha256sum=buildinfo.pkgbuild_sha256sum,
+                schema_version=buildinfo.schema_version,
                 startdir=buildinfo.startdir,
             )
         else:
             raise RuntimeError(
                 "An unknown input format has been encountered while transforming a package's BuildInfo information "
                 "into the respective output format!"
             )
 
 
 class OutputBuildInfoV1(
     BuildDir,
     BuildEnv,
-    FormatV1,
     Installed,
     Options,
     OutputBuildInfo,
     PkgBuildSha256Sum,
+    SchemaVersionV1,
 ):
-    """OutputBuildInfo version 1
+    """OutputBuildInfo version 1.
 
     Attributes which are already covered by OutputPackageBase are ommitted.
     Instances of this class relate to OutputBuildInfo the same way as BuildinfoV1 relates to BuildInfo.
 
     Attributes
     ----------
     builddir: str
         A string representing an absolute directory
-    buildenv: List[str]
+    buildenv: list[str]
         A list of strings as described by makepkg.conf's BUILDENV option
-    format_: int
-        An integer describing a BuildInfo format version
-    installed: List[str]
+    installed: list[str]
         A list of strings representing <package_name>-<epoch><version>-<pkgrel>-<architecture> of packages installed
         during the creation of a package
-    options: List[str]
+    options: list[str]
         A list of strings representing makepkg.conf OPTIONS used during the creation of a package
     pkgbuild_sha256sum: str
         A string representing a SHA-256 checksum for a PKGBUILD of a package
+    schema_version: int
+        An integer describing a BuildInfo format version
     """
 
     pass
 
 
 class OutputBuildInfoV2(
     BuildDir,
     BuildEnv,
     BuildTool,
     BuildToolVer,
-    FormatV2,
     Installed,
     Options,
     OutputBuildInfo,
     PkgBuildSha256Sum,
+    SchemaVersionV2,
     StartDir,
 ):
-    """OutputBuildInfo version 2
+    """OutputBuildInfo version 2.
 
     Attributes which are already covered by OutputPackageBase are ommitted.
     Instances of this class relate to OutputBuildInfo the same way as BuildinfoV2 relates to BuildInfo.
 
     Attributes
     ----------
     builddir: str
         A string representing an absolute directory
-    buildenv: List[str]
+    buildenv: list[str]
         A list of strings as described by makepkg.conf's BUILDENV option
     buildtool: str
         The package name of the build tool used to create a package
     buildtoolver: str
         The version of the build tool used to create a package
-    format_: int
-        An integer describing a BuildInfo format version
-    installed: List[str]
+    installed: list[str]
         A list of strings representing <package_name>-<epoch><version>-<pkgrel>-<architecture> of packages installed
         during the creation of a package
-    options: List[str]
+    options: list[str]
         A list of strings representing makepkg.conf OPTIONS used during the creation of a package
     pkgbuild_sha256sum: str
         A string representing a SHA-256 checksum for a PKGBUILD of a package
+    schema_version: int
+        An integer describing a BuildInfo format version
     startdir: str
         A string representing the absolute startdir directory of a package
     """
 
     pass
 
 
 class OutputPackage(BaseModel):
-    """A template class to describe all required attributes that define a package in the context of an output file
+    """A template class to describe all required attributes that define a package in the context of an output file.
 
     This class should not be instantiated directly. Use one of its subclasses instead!
     """
 
     @classmethod
     def from_package(cls, package: package.Package) -> OutputPackage:
-        """Create an OutputPackage from a Package
+        """Create an OutputPackage from a Package.
 
         Parameters
         ----------
         package: Path
             The path to a package file
-        signature: Optional[Path]
+        signature: Path | None
             The optional path to a signature file for package
 
         Returns
         -------
         OutputPackage
             An instance of one of OutputPackage's child classes
         """
-
         outputpackage_version = 0
         data = package.top_level_dict()
         keys = set(data.keys())
 
         debug(f"Creating OutputPackage from Package {data.get('filename')}...")
 
         for version in range(len(OUTPUT_PACKAGE_VERSIONS), 0, -1):
@@ -280,15 +286,15 @@
         match outputpackage_version:
             case 1:
                 return OutputPackageV1(
                     arch=package.pkginfo.arch,  # type: ignore[attr-defined]
                     backup=package.pkginfo.backup,  # type: ignore[attr-defined]
                     builddate=package.pkginfo.builddate,  # type: ignore[attr-defined]
                     checkdepends=package.pkginfo.checkdepends,  # type: ignore[attr-defined]
-                    conflicts=package.pkginfo.checkdepends,  # type: ignore[attr-defined]
+                    conflicts=package.pkginfo.conflicts,  # type: ignore[attr-defined]
                     csize=package.csize,  # type: ignore[attr-defined]
                     depends=package.pkginfo.depends,  # type: ignore[attr-defined]
                     desc=package.pkginfo.desc,  # type: ignore[attr-defined]
                     filename=package.filename,  # type: ignore[attr-defined]
                     files=Files.from_dict(
                         {
                             "files": [
@@ -336,107 +342,107 @@
     PgpSig,
     Provides,
     Replaces,
     SchemaVersionV1,
     Sha256Sum,
     Url,
 ):
-    """A model describing all required attributes that define a package in the context of an output file (version 1)
+    """A model describing all required attributes that define a package in the context of an output file (version 1).
 
     Attributes
     ----------
     arch: str
         The attribute can be used to describe the (required) data below an %ARCH% identifier in a 'desc' file, which
         identifies a package's architecture
-    backup: Optional[List[str]]
+    backup: list[str] | None
         The attribute can be used to describe the (optional) data below a %BACKUP% identifier in a 'desc' file, which
         identifies which file(s) of a package pacman will create backups for
     builddate: int
         The attribute can be used to describe the (required) data below a %BUILDDATE% identifier in a 'desc' file,
         which identifies a package's build date (represented in seconds since the epoch)
-    checkdepends: Optional[List[str]]
+    checkdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %CHECKDEPENDS% identifier in a 'desc' file,
         which identifies a package's checkdepends
-    conflicts: Optional[List[str]]
+    conflicts: list[str] | None
         The attribute can be used to describe the (optional) data below a %CONFLICTS% identifier in a 'desc' file, which
         identifies what other package(s) a package conflicts with
     csize: int
         The attribute can be used to describe the (required) data below a %CSIZE% identifier in a 'desc' file, which
         identifies a package's size
-    depends: Optional[List[str]]
+    depends: list[str] | None
         The attribute can be used to describe the (optional) data below a %DEPENDS% identifier in a 'desc' file, which
         identifies what other package(s) a package depends on
     desc: str
         The attribute can be used to describe the (required) data below a %DESC% identifier in a 'desc' file, which
         identifies a package's description
     filename: str
         The attribute can be used to describe the (required) data below a %FILENAME% identifier in a 'desc' file, which
         identifies a package's file name
-    files: Optional[List[str]]
+    files: list[str] | None
         The attribute can be used to describe the (optional) data below a %FILES% identifier in a 'files' file, which
         identifies which file(s) belong to a package
-    groups: Optional[List[str]]
+    groups: list[str] | None
         The attribute can be used to describe the (optional) data below a %GROUPS% identifier in a 'desc' file, which
         identifies a package's groups
     isize: int
         The attribute can be used to describe the (required) data below an %ISIZE% identifier in a 'desc' file, which
         identifies a package's installed size
-    license: List[str]
+    license: list[str]
         The attribute can be used to describe the (required) data below a %LICENSE% identifier in a 'desc' file, which
         identifies a package's license(s)
     md5sum: str
         The attribute can be used to describe the (required) data below an %MD5SUM% identifier in a 'desc' file, which
         identifies a package's md5 checksum
     name: str
         The attribute can be used to describe the (required) data below a %NAME% identifier in a 'desc' file, which
         identifies a package's name
-    optdepends: Optional[List[str]]
+    optdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
         which identifies what other package(s) a package optionally depends on
     pgpsig: str
         The attribute can be used to describe the (required) data below a %PGPSIG% identifier in a 'desc' file, which
         identifies a package's PGP signature
-    provides: Optional[List[str]]
+    provides: list[str] | None
         The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
         identifies what other package(s) a package provides
-    replaces: Optional[List[str]]
+    replaces: list[str] | None
         The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
         identifies what other package(s) a package replaces
     schema_version: PositiveInt
         A positive integer - 1 - identifying the schema version of the object
     sha256sum: str
         The attribute can be used to describe the (required) data below an %SHA256SUM% identifier in a 'desc' file,
         which identifies a package's sha256 checksum
     url: str
         The attribute can be used to describe the (required) data below a %URL% identifier in a 'desc' file, which
         identifies a package's URL
     """
 
-    files: Optional[Files] = None
+    files: SerializeAsAny[Files | None] = None
 
 
 class OutputPackageBase(BaseModel):
-    """A template class with helper methods to create instances of one of its (versioned) subclasses
+    """A template class with helper methods to create instances of one of its (versioned) subclasses.
 
     This class should not be instantiated directly, as it only provides generic instance methods for its subclasses.
 
     NOTE: The `from_dict()` classmethod is used to create one of the versioned subclasses.
     """
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Union[Any, List[Any]]]) -> OutputPackageBase:
-        """Create an instance of one of OutputPackageBase's subclasses from a dict
+    def from_dict(cls, data: dict[str, Any | list[Any]]) -> OutputPackageBase:
+        """Create an instance of one of OutputPackageBase's subclasses from a dict.
 
         This method expects data derived from reading a pkgbase JSON file from the management repository.
         By default this method will prefer to create an instances of OutputPackageBase's subclasses as identified by
         DEFAULT_OUTPUT_PACKAGE_BASE_VERSION (if it is newer than the schema_version retrieved from the data).
 
         Parameters
         ----------
-        data: Dict[str, Union[Any, List[Any]]]
+        data: dict[str, Any | list[Any]]
             A dict containing data required to instantiate a subclass of OutputPackageBase
 
         Raises
         ------
         RepoManagementValidationError
             If an invalid schema_version is encountered when reading data
             If a ValidationError is encountered during instantiation of one of the OutputPackage subclasses
@@ -444,43 +450,42 @@
 
         Returns
         -------
         OutputPackageBase
             An instance of one of the subclasses of OutputPackageBase
         """
 
-        def default_output_package_from_dict(version: int, package: Dict[str, Any]) -> OutputPackage:
-            """Create the default OutputPackage subclass for a OutputPackageBase from a dict
+        def default_output_package_from_dict(version: int, package: dict[str, Any]) -> OutputPackage:
+            """Create the default OutputPackage subclass for a OutputPackageBase from a dict.
 
             Parameters
             ----------
             version: int
                 The schema_version of the OutputPackageBase subclass for which to create an instance of a subclass of
                 OutputPackage
-            package: Dict[str, Any]
+            package: dict[str, Any]
                 A dict describing the attributes of an OutputPackage instance
 
             Returns
             -------
             OutputPackage
                 A subclass of OutputPackage that is the default for the given OutputPackageBase schema_version
             """
-
             outputpackage_version = OutputPackageVersionEnum.DEFAULT.value
             files_version = FilesVersionEnum.DEFAULT.value
 
             match (outputpackage_version, files_version):
                 case (1, 1):
                     files = package.get("files")
                     if files:
                         if files.get("schema_version"):
                             del files["schema_version"]
-                        package["files"] = FilesV1(**files)
+                        package["files"] = FilesV1.model_validate(files)
 
-                    return OutputPackageV1(**package)
+                    return OutputPackageV1.model_validate(package)
                 # NOTE: the catch all can never be reached but is here to satisfy our tooling
                 case _:  # pragma: no cover
                     raise RuntimeError(
                         f"Invalid version provided for OutputPackage ({outputpackage_version} "
                         f"and/ or Files ({files_version})."
                     )
 
@@ -499,29 +504,29 @@
             case 1:
                 if isinstance(data.get("packages"), list):
                     data["packages"] = [
                         default_output_package_from_dict(version=used_schema_version, package=package)
                         for package in data.get("packages")  # type: ignore[union-attr]
                     ]
                 try:
-                    return OutputPackageBaseV1(**data)
+                    return OutputPackageBaseV1.model_validate(data)
                 except ValidationError as e:
                     raise errors.RepoManagementValidationError(
                         "A validation error occured while attempting to instantiate an OutputPackageBaseV1 using data:"
                         f"\n'{data}'\n{e}"
                     )
             case _:
                 raise errors.RepoManagementValidationError(
                     f"The unsupported schema version ({used_schema_version}) has been encountered, when "
                     f"attempting to read data:\n{data}"
                 )
 
     @classmethod
     async def from_file(cls, path: Path) -> OutputPackageBase:
-        """Initialize an OutputPackageBase from a JSON file
+        """Initialize an OutputPackageBase from a JSON file.
 
         Parameters
         ----------
         path: Path
             A Path to to a JSON file
 
         Raises
@@ -530,28 +535,27 @@
             If the JSON file can not be decoded
 
         Returns
         -------
         OutputPackageBase
             An instance of OutputPackageBase based on path
         """
-
         async with async_open(path, "r") as input_file:
             try:
                 return OutputPackageBase.from_dict(data=loads(await input_file.read()))
             except JSONDecodeError as e:
                 raise errors.RepoManagementFileError(f"The JSON file '{path}' could not be decoded!\n{e}")
 
     @classmethod
-    def from_package(cls, packages: List[package.Package]) -> OutputPackageBase:
-        """Create an OutputPackageBase from a list of Packages of the same pkgbase, pkgtype and version
+    def from_package(cls, packages: list[package.Package]) -> OutputPackageBase:
+        """Create an OutputPackageBase from a list of Packages of the same pkgbase, pkgtype and version.
 
         Parameters
         ----------
-        packages: List[Package]
+        packages: list[Package]
             A list of Packages to create an OutputPackageBase for
 
         Raises
         ------
         ValueError
             If packages is an empty list,
             if more than one pkgbase is used in the list of packages,
@@ -560,15 +564,14 @@
             or if mismatching pkgtypes are found in the list of packages
 
         Returns
         -------
         OutputPackageBase
             An OutputPackageBase that is based on packages
         """
-
         if len(packages) == 0:
             raise ValueError("At least one Package needs to be provided to create an OutputPackageBase.")
 
         pkgbases = set([str(pkg.top_level_dict().get("pkgbase")) for pkg in packages])
         if len(pkgbases) > 1:
             raise ValueError(
                 "Only one pkgbase can be used per OutputPackageBase, but Packages with the following pkgbases are "
@@ -587,24 +590,24 @@
         versions = set([str(pkg.top_level_dict().get("version")) for pkg in packages])
         if len(versions) != 1:
             raise ValueError(
                 "Only one version can be used per OutputPackageBase, but Packages with the following versions are "
                 f"provided: {', '.join(versions)}"
             )
 
-        all_xdata: List[List[Dict[str, Any]]] = [
+        all_xdata: list[list[dict[str, Any]]] = [
             pkg.top_level_dict().get("xdata")  # type: ignore[misc]
             for pkg in packages
             if pkg.top_level_dict().get("xdata")
         ]
         debug(f"all xdata: {all_xdata}")
-        xdata: List[Dict[str, str]] = []
+        xdata: list[dict[str, str]] = []
         xdata = [item for sublist in all_xdata for item in sublist]
         debug(f"collected xdata: {xdata}")
-        pkgtypes: List[str] = []
+        pkgtypes: list[str] = []
         pkgtypes = [data.get("pkgtype").value for data in xdata if data.get("pkgtype")]  # type: ignore[union-attr]
         debug(f"collected pkgtypes: {pkgtypes}")
 
         debug(f"pkgtypes: {pkgtypes}")
         if len(set(pkgtypes)) > 1:
             raise ValueError(
                 "An error occurred while trying to create an OutputPackageBase from Packages: "
@@ -644,68 +647,66 @@
                 )
             case _:
                 raise RuntimeError(
                     "An error occurred while attempting to create an OutputPackageBase!"
                     f"Unable to find matching version for Package keys: {keys}"
                 )
 
-    def add_packages(self, packages: List[OutputPackage]) -> None:
-        """Add packages to an instance of one of OutputPackageBase's subclasses
+    def add_packages(self, packages: list[OutputPackage]) -> None:
+        """Add packages to an instance of one of OutputPackageBase's subclasses.
 
         NOTE: This method only operates successfully if the instance of the class using it actually defines the
         `packages` field! The OutputPackageBase class does not do that!
 
         Parameters
         ----------
-        packages: List[OutputPackage]
+        packages: list[OutputPackage]
             A list of OutputPackage instances to add
 
         Raises
         ------
         RuntimeError
             If called on the OutputPackageBase template class
         """
-
         if hasattr(self, "packages"):
             # TODO: only add OutputPackage subclasses that are compatible with the OutputPackageBase version, else
             # attempt conversion
-            self.packages += packages  # type: ignore[attr-defined]
+            self.packages += packages
         else:
             raise RuntimeError("It is not possible to add packages to the template class OutputPackageBase!")
 
     def get_version(self) -> str:
-        """Get version of an instance of one of OutputPackage's subclasses
+        """Get version of an instance of one of OutputPackage's subclasses.
 
         NOTE: This method only successfully returns if the instance of the class using it defines the `get_version`
         field! The OutputPackageBase class does not do that!
 
         Raises
         ------
         RuntimeError
             If called on the OutputPackageBase template class
 
         Returns
         -------
         str
             The version string of the OutputPackageBase
         """
-
         if hasattr(self, "version"):
-            return str(self.version)  # type: ignore[attr-defined]
+            return str(self.version)
         else:
             raise RuntimeError(
                 "It is not possible to return the version attribute of the template class OutputPackageBase!"
             )
 
     async def get_packages_as_models(
         self,
         packagedesc_version: PackageDescVersionEnum = PackageDescVersionEnum.DEFAULT,
         files_version: FilesVersionEnum = FilesVersionEnum.DEFAULT,
-    ) -> List[Tuple[PackageDesc, Files]]:
-        """Return the list of packages as tuples of PackageDesc and Files models
+    ) -> list[tuple[PackageDesc, Files]]:
+        """Return the list of packages as tuples of PackageDesc and Files models.
 
         NOTE: This method only successfully returns if the instance of the class using it defines the required fields!
         The OutputPackageBase class does not do that!
 
         Parameters
         ----------
         packagedesc_version: int
@@ -718,27 +719,24 @@
         RuntimeError
             If this method is called on the template class OutputPackageBase (instead of on one of its subclasses)
             If an unknown schema_version is encountered in the OutputPackageBase instance.
             If unsupported packagedesc_version or files_version are encountered.
 
         Returns
         -------
-        List[Tuple[PackageDesc, Files]]
+        list[tuple[PackageDesc, Files]]
             A list of tuples with one PackageDesc and one Files each
         """
-
         if not hasattr(self, "schema_version"):
             raise RuntimeError(
                 "Packages and their files can not be retrieved from the templatae class OutputPackageBase!"
             )
 
-        if self.schema_version not in OUTPUT_PACKAGE_BASE_VERSIONS.keys():  # type: ignore[attr-defined]
-            raise RuntimeError(
-                f"OutputPackageBase has invalid schema_version {self.schema_version}!"  # type: ignore[attr-defined]
-            )
+        if self.schema_version not in OUTPUT_PACKAGE_BASE_VERSIONS.keys():
+            raise RuntimeError(f"OutputPackageBase has invalid schema_version {self.schema_version}!")
 
         match (packagedesc_version, files_version):
             case (PackageDescVersionEnum.ONE, FilesVersionEnum.DEFAULT):
                 return [
                     (
                         PackageDescV1(
                             arch=package.arch,
@@ -812,64 +810,70 @@
 
 class OutputPackageBaseV1(
     OutputPackageBase,
     Base,
     MakeDepends,
     Packager,
     SchemaVersionV1,
+    SourceUrl,
     Version,
 ):
-    """A model describing all required attributes for an output file, that describes a list of packages based upon a
-    pkgbase (version 1)
+    """A model for an output file format, that describes a list of packages based upon a pkgbase (version 1).
 
     Attributes
     ----------
     base: str
         The attribute can be used to describe the (required) data below a %BASE% identifier in a 'desc' file, which
         identifies a package's pkgbase
-    buildinfo: Optional[OutputBuildInfo]
+    buildinfo: OutputBuildInfo | None
         An optional OutputBuildInfo, which describes the build circumstances of the OutputPackageBase. The data is not
         covered in a repository sync database and therefore optional.
-    makedepends: Optional[List[str]]
+    makedepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %MAKEDEPENDS% identifier in a 'desc' file,
         which identifies a package's makedepends
     packager: str
         The attribute can be used to describe the (required) data below a %PACKAGER% identifier in a 'desc' file, which
         identifies a package's packager
-    packages: List[OutputPackage]
+    packages: list[OutputPackage]
         A list of OutputPackage instances that belong to the pkgbase identified by base
     schema_version: PositiveInt
         A positive integer - 1 - identifying the schema version of the object
+    source_url: HttpUrl | None
+        An optional url that points at sources (defaults to None)
     version: str
         The attribute can be used to describe the (required) data below a %VERSION% identifier in a 'desc' file, which
         identifies a package's version (this is the accumulation of epoch, pkgver and pkgrel)
     """
 
-    buildinfo: Optional[OutputBuildInfo]
-    packages: List[OutputPackage]
+    buildinfo: SerializeAsAny[OutputBuildInfo | None] = None
+    packages: SerializeAsAny[list[OutputPackage]]
 
 
-def export_schemas(output: Union[Path, str]) -> None:
-    """Export the JSON schema of selected pydantic models to an output directory
+def export_schemas(output: Path | str) -> None:
+    """Export the JSON schema of selected pydantic models to an output directory.
 
     Parameters
     ----------
     output: Path
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-
     classes = [OutputBuildInfoV1, OutputBuildInfoV2, OutputPackageV1, OutputPackageBaseV1]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
 
     for class_ in classes:
-        with open(output / f"{class_.__name__}.json", "w") as f:
-            print(class_.schema_json(indent=2), file=f)
+        with open(output / f"{class_.__name__}.json", "wb") as f:
+            f.write(
+                dumps(
+                    class_.model_json_schema(),  # type: ignore[attr-defined]
+                    option=OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS,
+                )
+            )
```

### Comparing `repod-0.2.2/repod/repo/package/repofile.py` & `repod-0.3.0.post0/repod/repo/package/repofile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,74 @@
+"""Functions and helpers to work with files in repod managed repositories."""
 from itertools import zip_longest
 from logging import debug, info
 from pathlib import Path
 from re import Match, fullmatch
 from shutil import copy2
-from typing import Any, Dict, List
+from typing import Any
 
-from pydantic import BaseModel, root_validator
+from pydantic import BaseModel, model_validator
 
 from repod.common.enums import RepoFileEnum
-from repod.common.regex import PACKAGE_PATH, PACKAGE_SIGNATURE_PATH
+from repod.common.regex import PACKAGE_FILENAME, SIGNATURE_FILENAME
 from repod.errors import RepoManagementFileError
 
 
+def filename_parts(file: Path) -> dict[str, str]:
+    """Split a package or signature name and return its specific metadata in a dict.
+
+    Parameters
+    ----------
+    file: Path
+        A package filename path
+
+    Raises
+    ------
+    ValueError
+        If file can not be split to derive architecture and suffix information.
+        If file can not be split to derive name and version information.
+
+    Returns
+    -------
+    dict[str, str]
+        A dict carrying data, derived from the package filename:
+        - arch: CPU architecture
+        - suffix: The package compression
+        - version: The full version
+        - pkgrel: The release version of the package
+        - pkgver: The version of the package
+        - epoch: The epoch of the package (if any)
+        - name: The name of the package
+    """
+    debug(f"Retrieving data from filename {file}")
+    name = file.name
+    output_dict: dict[str, str] = {}
+
+    arch_suffix_split = name.split("-")[-1].split(".")
+    if not (5 >= len(arch_suffix_split) >= 3):
+        raise ValueError(f"The provided file name {file} can not be split for architecture and suffix information!")
+
+    output_dict["arch"] = arch_suffix_split[0]
+    output_dict["suffix"] = ".".join(arch_suffix_split[1:])
+
+    name_version = name.split("-")[:-1]
+    if len(name_version) < 3:
+        raise ValueError(f"The provided file name {file} can not be split for name and version information!")
+
+    output_dict["version"] = "-".join([name_version[-2], name_version[-1]])
+    output_dict["pkgrel"] = name_version[-1]
+    output_dict["pkgver"] = name_version[-2].split(":")[-1]
+    output_dict["epoch"] = name_version[-2].split(":")[0] if len(name_version[-2].split(":")) > 1 else ""
+    output_dict["name"] = "-".join(name_version[0:-2])
+
+    return output_dict
+
+
 def shared_base_path(path_a: Path, path_b: Path) -> Path:
-    """Return the shared base path of two absolute paths
+    """Return the shared base path of two absolute paths.
 
     Parameters
     ----------
     path_a: Path
         An absolute path
     path_b: Path
         An absolute path
@@ -28,35 +79,34 @@
         If either path_a or path_b are not absolute paths
 
     Returns
     -------
     Path
         The shared base path of path_a and path_b
     """
-
     debug(f"Calculating the shared base path of {path_a} and {path_b}...")
     for path in (path_a, path_b):
         if not path.is_absolute():
             raise ValueError(f"The path {path} is not absolute!")
 
-    output_list: List[str] = []
+    output_list: list[str] = []
     # NOTE: we skip branch check here, because coveragepy does not detect that we can never have any of the Path objects
     # return an empty list of parts, as they are ensured to be absolute
     for part_a, part_b in zip_longest(path_a.parts, path_b.parts, fillvalue=None):  # pragma: no branch
         if part_a is not None and part_b is not None and part_a == part_b:
             output_list.append(part_a)
         else:
             break
 
     debug(f"Calculated shared base path: {Path(*output_list)}")
     return Path(*output_list)
 
 
 def relative_to_shared_base(path_a: Path, path_b: Path) -> Path:
-    """Return a Path to path_a, relative to the shared base path of path_a and path_b
+    """Return a Path to path_a, relative to the shared base path of path_a and path_b.
 
     This function calls shared_base_path() to determine the shared base path of path_a and path_b.
 
     Parameters
     ----------
     path_a: Path
         An absolute path
@@ -64,15 +114,14 @@
         An absolute path
 
     Returns
     -------
     Path
         The path to path_a, relative to the shared base path of path_a and path_b
     """
-
     debug(f"Calculating a path relative to the shared base path of {path_a} and {path_b}...")
     shared_base = shared_base_path(path_a=path_a, path_b=path_b)
     parent_distance = len(path_b.parent.parts) - len(shared_base.parts)
     debug(f"The parent distance of {path_a} to {shared_base} is {parent_distance}.")
 
     return_path: Path
     if parent_distance > 0:
@@ -81,15 +130,15 @@
         return_path = path_a.relative_to(shared_base)
 
     debug(f"Calculated path relative to the shared base path {shared_base}: {return_path}")
     return return_path
 
 
 class RepoFile(BaseModel):
-    """Class to interact with files in a repository
+    """Class to interact with files in a repository.
 
     Attributes
     ----------
     file_type: RepoFileEnum
         A RepoFileEnum member defining which type of file is targeted
     file_path: Path
         The path to the file
@@ -98,250 +147,231 @@
     """
 
     file_type: RepoFileEnum
     file_path: Path
     symlink_path: Path
 
     @classmethod
-    def validate_path(cls, path: Path, regex: str) -> None:
-        """Validate path to match regex
+    def validate_path(cls, path: Path, file_type: RepoFileEnum) -> None:
+        """Validate path to match regex.
 
         Parameters
         ----------
         path: Path
             A path to match
-        regex: str
-            A regular expression to match path against
+        file_type: RepoFileEnum
+            A member of RepoFileEnum identifying which type of RepoFile to validate
 
         Raises
         ------
         ValueError
-            If path does not match regex
-        """
-
-        if not isinstance(fullmatch(regex, str(path)), Match):
-            raise ValueError(f"The path {path} does not match the regular expression {regex}.")
-
-    @classmethod
-    def get_file_type_regex(cls, file_type: RepoFileEnum) -> str:
-        """Return the regular expression associated with a given RepodFileEnum member
-
-        Parameters
-        ----------
-        file_type: RepoFileEnum
-            A member of RepoFileEnum
-
-        Returns
-        -------
-        str
-            The regular expression string associated with file_type
+            If path can not be validated
         """
-
         match file_type:
             case RepoFileEnum.PACKAGE:
-                return rf"^{PACKAGE_PATH}$"
+                if not path.is_absolute():
+                    raise ValueError(f"The path {path} must be absolute!")
+                if not isinstance(fullmatch(PACKAGE_FILENAME, path.name), Match):
+                    raise ValueError(f"The path {path} does not match the regular expression {PACKAGE_FILENAME}.")
+                return
+
             case RepoFileEnum.PACKAGE_SIGNATURE:
-                return rf"^{PACKAGE_SIGNATURE_PATH}$"
+                if not path.is_absolute():
+                    raise ValueError(f"The path {path} must be absolute!")
+                if not isinstance(fullmatch(SIGNATURE_FILENAME, path.name), Match):
+                    raise ValueError(f"The path {path} does not match the regular expression {SIGNATURE_FILENAME}.")
+                return
             case _:
-                raise RuntimeError(f"Invalid RepoFile.file_type encountered: {file_type}")
+                raise RuntimeError(f"Unknown repository file type: {file_type}")
 
-    @root_validator
-    def validate_paths(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """Validator for absolute Paths
+    @model_validator(mode="before")
+    def validate_paths(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Validate absolute Paths.
 
         Parameters
         ----------
-        values: Dict[str, Any]
+        values: dict[str, Any]
             A dict with all values of the RepoFile instance
 
         Raises
         ------
         ValueError
             If file_path and symlink_path are equal.
-            If path does not match the PACKAGE_PATH regular expression
+            If the path can not be validated using RepoFile.validate_path()
 
         Returns
         -------
         Path
             The validated Path
         """
+        file_type: RepoFileEnum = values.get("file_type")  # type: ignore[assignment]
 
-        file_type = values.get("file_type")
-        regex = RepoFile.get_file_type_regex(file_type=file_type)
-
-        paths: List[Path] = []
+        paths: list[Path] = []
         paths.append(values.get("file_path"))  # type: ignore[arg-type]
         paths.append(values.get("symlink_path"))  # type: ignore[arg-type]
 
         if paths[0] == paths[1]:
             raise ValueError(
                 f"The file_path ({paths[0]}) and the symlink_path ({paths[1]}) attributes must not be equal!"
             )
 
         for path in paths:
-            RepoFile.validate_path(regex=regex, path=path)
+            RepoFile.validate_path(path=path, file_type=file_type)
 
         return values
 
     def check_file_path_exists(self, exists: bool = True) -> None:
-        """Ensure that file_path exists
+        """Ensure that file_path exists.
 
         Parameters
         ----------
         exists: bool
             Whether file_path should exist or not (defaults to True)
 
         Raises
         ------
         RepoManagementFileError
             If self.file_path does not exist
         """
-
         if exists:
             if not self.file_path.exists():
                 raise RepoManagementFileError(
                     f"An error occured checking for the existence of a file: {self.file_path} does not exist!"
                 )
         else:
             if self.file_path.exists():
                 raise RepoManagementFileError(
                     f"An error occured checking for the existence of a file: {self.file_path} exists already!"
                 )
 
     def check_symlink_path_exists(self, exists: bool = True) -> None:
-        """Ensure that symlink_path exists
+        """Ensure that symlink_path exists.
 
         Parameters
         ----------
         exists: bool
             Whether symlink_path should exist or not (defaults to True)
 
         Raises
         ------
         RepoManagementFileError
             If self.symlink_path does not exist
         """
-
         if exists:
             if not self.symlink_path.exists():
                 raise RepoManagementFileError(
                     "An error occured checking for the existence of a symlink: {self.symlink_path} does not exist!"
                 )
         else:
             if self.symlink_path.exists():
                 raise RepoManagementFileError(
                     "An error occured checking for the existence of a symlink: {self.symlink_path} exists already!"
                 )
 
     def copy_from(self, path: Path) -> None:
-        """Copy file from a provided Path to file_path
+        """Copy file from a provided Path to file_path.
 
         Before doing further checks, RepoFile.validate_path() is run on path.
 
         Parameters
         ----------
         path: Path
             Path to move from
 
         Raises
         ------
         RepoManagementFileError
             If path does not exist
         """
-
         info(f"Copy {self.file_path} from {path}...")
-        RepoFile.validate_path(path=path, regex=RepoFile.get_file_type_regex(file_type=self.file_type))
+        RepoFile.validate_path(path=path, file_type=self.file_type)
         if not path.exists():
             raise RepoManagementFileError(f"Error on trying to move file: The input file {path} does not exist!")
 
         self.check_file_path_exists(exists=False)
         copy2(src=path, dst=self.file_path)
 
     def move_from(self, path: Path) -> None:
-        """Move file from a provided Path to file_path
+        """Move file from a provided Path to file_path.
 
         Before doing further checks, RepoFile.validate_path() is run on path.
 
         Parameters
         ----------
         path: Path
             Path to move from
 
         Raises
         ------
         RepoManagementFileError
             If path does not exist
         """
-
         info(f"Move {self.file_path} from {path}...")
-        RepoFile.validate_path(path=path, regex=RepoFile.get_file_type_regex(file_type=self.file_type))
+        RepoFile.validate_path(path=path, file_type=self.file_type)
         if not path.exists():
             raise RepoManagementFileError(f"Error on trying to move file: The input file {path} does not exist!")
 
         self.check_file_path_exists(exists=False)
         path.rename(target=self.file_path)
 
     def link(self, check: bool = True) -> None:
-        """Link the symlink_path to file_path using a relative symlink
+        """Link the symlink_path to file_path using a relative symlink.
 
         Parameters
         ----------
         check: bool
             Whether to check if the symlink_path exists already prior to linking (defaults to True)
 
         Raises
         ------
         RepoManagementFileError
             If the file exists already
         """
-
         info(f"Link {self.symlink_path} to {self.file_path}...")
         if check:
             debug(f"Checking that {self.symlink_path} does not yet exist...")
             self.check_symlink_path_exists(exists=False)
 
         try:
             self.symlink_path.symlink_to(relative_to_shared_base(path_a=self.file_path, path_b=self.symlink_path))
         except FileExistsError:
             raise RepoManagementFileError(
                 f"An error occured attempting to symlink {self.symlink_path} to {self.file_path}."
                 f"{self.symlink_path} exists already!"
             )
 
     def unlink(self, check: bool = True) -> None:
-        """Unlink the symlink_path from file_path
+        """Unlink the symlink_path from file_path.
 
         Parameters
         ----------
         check: bool
             Whether to check that the symlink_path does not exist prior to removal (defaults to True)
 
         Raises
         ------
         RepoManagementFileError
             If the file does not exist and check = True
         """
-
         info(f"Unlink {self.symlink_path} from {self.file_path}...")
         if check:
             debug(f"Checking that {self.symlink_path} exists...")
             self.check_symlink_path_exists()
 
         self.symlink_path.unlink(missing_ok=not check)
 
     def remove(self, force: bool = False, unlink: bool = False) -> None:
-        """Remove file_path and optionally unlink symlink_path from file_path
+        """Remove file_path and optionally unlink symlink_path from file_path.
 
         Parameters
         ----------
         force: bool
             Whether to not check for path existence before unlinking and to ignore errors on removing non-existing files
             (defaults to False)
         """
-
         info(f"Removing {self.file_path}...")
         if not force:
             debug(f"Checking that {self.file_path} exists...")
             self.check_file_path_exists()
 
         self.file_path.unlink(missing_ok=force)
```

### Comparing `repod-0.2.2/repod/repo/package/syncdb.py` & `repod-0.3.0.post0/repod/repo/package/syncdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+"""Sync database handling."""
 from __future__ import annotations
 
 import io
 import re
 from enum import IntEnum
 from logging import debug, warning
 from pathlib import Path
 from tarfile import DIRTYPE, TarFile, TarInfo
 from time import time
-from typing import Dict, List, Optional, Set, Tuple, Union
 
 from jinja2 import Environment, PackageLoader, TemplateNotFound
+from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS, dumps
 from pydantic import BaseModel, ValidationError
 
 from repod.common.enums import (
     CompressionTypeEnum,
     FieldTypeEnum,
     FilesVersionEnum,
     PackageDescVersionEnum,
@@ -54,15 +55,15 @@
 from repod.files.common import open_tarfile
 from repod.repo.management import outputpackage
 
 DB_USER = "root"
 DB_GROUP = "root"
 DB_FILE_MODE = "0644"
 DB_DIR_MODE = "0755"
-DESC_JSON: Dict[str, Tuple[str, FieldTypeEnum]] = {
+DESC_JSON: dict[str, tuple[str, FieldTypeEnum]] = {
     "%BASE%": ("base", FieldTypeEnum.STRING),
     "%VERSION%": ("version", FieldTypeEnum.STRING),
     "%MAKEDEPENDS%": ("makedepends", FieldTypeEnum.STRING_LIST),
     "%CHECKDEPENDS%": ("checkdepends", FieldTypeEnum.STRING_LIST),
     "%FILENAME%": ("filename", FieldTypeEnum.STRING),
     "%NAME%": ("name", FieldTypeEnum.STRING),
     "%DESC%": ("desc", FieldTypeEnum.STRING),
@@ -80,26 +81,26 @@
     "%REPLACES%": ("replaces", FieldTypeEnum.STRING_LIST),
     "%CONFLICTS%": ("conflicts", FieldTypeEnum.STRING_LIST),
     "%PROVIDES%": ("provides", FieldTypeEnum.STRING_LIST),
     "%DEPENDS%": ("depends", FieldTypeEnum.STRING_LIST),
     "%OPTDEPENDS%": ("optdepends", FieldTypeEnum.STRING_LIST),
     "%BACKUP%": ("backup", FieldTypeEnum.STRING_LIST),
 }
-FILES_JSON: Dict[str, Tuple[str, FieldTypeEnum]] = {"%FILES%": ("files", FieldTypeEnum.STRING_LIST)}
-FILES_VERSIONS: Dict[int, Dict[str, Set[str]]] = {
+FILES_JSON: dict[str, tuple[str, FieldTypeEnum]] = {"%FILES%": ("files", FieldTypeEnum.STRING_LIST)}
+FILES_VERSIONS: dict[int, dict[str, set[str]]] = {
     1: {
         "required": {
             "files",
         },
         "optional": set(),
     },
 }
 DEFAULT_FILES_VERSION = 1
 DEFAULT_PACKAGE_DESC_VERSION = 1
-PACKAGE_DESC_VERSIONS: Dict[int, Dict[str, Union[Set[str], int]]] = {
+PACKAGE_DESC_VERSIONS: dict[int, dict[str, set[str] | int]] = {
     1: {
         "required": {
             "arch",
             "base",
             "builddate",
             "csize",
             "desc",
@@ -177,42 +178,41 @@
 
     UNKNOWN = 0
     DESC = 1
     FILES = 2
 
 
 class RepoDbTypeEnum(IntEnum):
-    """An IntEnum to distinguish types of binary repository database files
+    """An IntEnum to distinguish types of binary repository database files.
 
     Attributes
     ----------
     DEFAULT: int
         Use this to identify .db files
     FILES: int
         Use this to identify .files files
     """
 
     DEFAULT = 0
     FILES = 2
 
 
-def get_desc_json_keys() -> Set[str]:
-    """Get the keys of repod.models.repo.DESC_JSON
+def get_desc_json_keys() -> set[str]:
+    """Get the keys of repod.models.repo.DESC_JSON.
 
     Returns
     -------
-    Set[str]
+    set[str]
         A set of strings representing the keys of repod.models.repo.DESC_JSON
     """
-
     return set(DESC_JSON.keys())
 
 
 def get_desc_json_name(key: str) -> str:
-    """Get the JSON name of a given key from the definition in repod.models.repo.DESC_JSON
+    """Get the JSON name of a given key from the definition in repod.models.repo.DESC_JSON.
 
     Parameters
     ----------
     key: str
         A string corresponding with one of the keys in repod.models.repo.DESC_JSON
 
     Raises
@@ -221,23 +221,22 @@
         If an unknown key is encountered
 
     Returns
     -------
     str
         The JSON name of a given 'desc' file identifier provided by key
     """
-
     try:
         return DESC_JSON[key][0]
     except KeyError:
         raise RepoManagementFileError(f"The key {key} is not a known 'desc' file identifier.")
 
 
 def get_desc_json_field_type(key: str) -> FieldTypeEnum:
-    """Get the FieldTypeEnum of a given key from the definition in repod.models.repo.DESC_JSON
+    """Get the FieldTypeEnum of a given key from the definition in repod.models.repo.DESC_JSON.
 
     Parameters
     ----------
     key: str
         A string corresponding with one of the keys in repod.models.repo.DESC_JSON
 
     Raises
@@ -246,35 +245,33 @@
         If an unknown key is encountered
 
     Returns
     -------
     str
         The FieldTypeEnum of a given 'desc' file identifier provided by key
     """
-
     try:
         return DESC_JSON[key][1]
     except KeyError:
         raise RepoManagementFileError(f"The key {key} is not a known 'desc' file identifier.")
 
 
-def get_files_json_keys() -> Set[str]:
-    """Get the keys of repod.models.repo.FILES_JSON
+def get_files_json_keys() -> set[str]:
+    """Get the keys of repod.models.repo.FILES_JSON.
 
     Returns
     -------
-    Set[str]
+    set[str]
         A set of strings representing the keys of repod.models.repo.FILES_JSON
     """
-
     return set(FILES_JSON.keys())
 
 
 def get_files_json_name(key: str) -> str:
-    """Get the JSON name of a given key from the definition in repod.models.repo.FILES_JSON
+    """Get the JSON name of a given key from the definition in repod.models.repo.FILES_JSON.
 
     Parameters
     ----------
     key: str
         A string corresponding with one of the keys in repod.models.repo.FILES_JSON
 
     Raises
@@ -283,23 +280,22 @@
         If an unknown key is encountered
 
     Returns
     -------
     str
         The JSON name of a given 'files' file identifier provided by key
     """
-
     try:
         return FILES_JSON[key][0]
     except KeyError:
         raise RepoManagementFileError(f"The key {key} is not a known 'files' file identifier.")
 
 
 def get_files_json_field_type(key: str) -> FieldTypeEnum:
-    """Get the FieldTypeEnum of a given key from the definition in repod.models.repo.FILES_JSON
+    """Get the FieldTypeEnum of a given key from the definition in repod.models.repo.FILES_JSON.
 
     Parameters
     ----------
     key: str
         A string corresponding with one of the keys in repod.models.repo.FILES_JSON
 
     Raises
@@ -308,50 +304,49 @@
         If an unknown key is encountered
 
     Returns
     -------
     str
         The FieldTypeEnum of a given 'desc' file identifier provided by key
     """
-
     try:
         return FILES_JSON[key][1]
     except KeyError:
         raise RepoManagementFileError(f"The key {key} is not a known 'files' file identifier.")
 
 
 class SyncDatabase(BaseModel):
-    """A model describing a repository sync database
+    """A model describing a repository sync database.
 
     Attributes
     ----------
     database: Path
         The path to the database that the instance manages
     database_type: RepoDbTypeEnum
         The type of database that the instance manages
     compression_type: CompressionTypeEnum
         The compression type which is used for  the database
     """
 
     database: Path
-    database_type: Optional[RepoDbTypeEnum]
-    compression_type: Optional[CompressionTypeEnum]
+    database_type: RepoDbTypeEnum | None = None
+    compression_type: CompressionTypeEnum | None = None
     desc_version: PackageDescVersionEnum
     files_version: FilesVersionEnum
 
     @classmethod
     async def outputpackagebase_to_tarfile(
         cls,
         tarfile: TarFile,
-        database_type: Optional[RepoDbTypeEnum],
+        database_type: RepoDbTypeEnum | None,
         model: outputpackage.OutputPackageBase,
         packagedesc_version: PackageDescVersionEnum,
         files_version: FilesVersionEnum,
     ) -> None:
-        """Stream descriptor files derived from an OutputPackageBase to a TarFile
+        """Stream descriptor files derived from an OutputPackageBase to a TarFile.
 
         Allows streaming to a default repository database or a files database
 
         Parameters
         ----------
         tarfile: TarFile
             A TarFile to stream data to
@@ -360,16 +355,15 @@
         model: OutputPackageBase
             The OutputPackageBase instance to derive descriptor files from
         packagedesc_version: PackageDescVersionEnum
             The version of PackageDesc to use
         files_version: FilesVersionEnum
             The version of Files to use
         """
-
-        for (desc_model, files_model) in await model.get_packages_as_models(
+        for desc_model, files_model in await model.get_packages_as_models(
             packagedesc_version=packagedesc_version,
             files_version=files_version,
         ):
             dirname = f"{desc_model.get_name()}-{model.get_version()}"
             directory = TarInfo(dirname)
             directory.type = DIRTYPE
             directory.mtime = int(time())
@@ -396,22 +390,21 @@
                 files_file.mtime = int(time())
                 files_file.uname = DB_USER
                 files_file.gname = DB_GROUP
                 files_file.mode = int(DB_FILE_MODE, base=8)
                 tarfile.addfile(files_file, io.BytesIO(files_content.getvalue().encode()))
 
     async def add(self, model: outputpackage.OutputPackageBase) -> None:
-        """Write descriptor files for packages of a single pkgbase to the repository sync database
+        """Write descriptor files for packages of a single pkgbase to the repository sync database.
 
         Parameters
         ----------
         model: OutputPackageBase
             The model to use for streaming descriptor files to the repository database
         """
-
         debug(f"Opening file {self.database} for writing...")
 
         with open_tarfile(
             path=self.database,
             compression=self.compression_type,
             mode="w",
         ) as database_file:
@@ -419,27 +412,25 @@
                 tarfile=database_file,
                 database_type=self.database_type,
                 model=model,
                 packagedesc_version=self.desc_version,
                 files_version=self.files_version,
             )
 
-    async def outputpackagebases(self) -> List[Tuple[str, outputpackage.OutputPackageBase]]:
-        """Read a repository database and yield the name of each pkgbase and the respective data (represented as an
-        instance of OutputPackageBase) in a Tuple.
+    async def outputpackagebases(self) -> list[tuple[str, outputpackage.OutputPackageBase]]:
+        """Read a repo sync database and return the name of each pkgbase and respective data.
 
         Returns
         -------
-        Iterator[Tuple[str, OutputPackageBase]]:
-            A Tuple holding the name of a pkgbase and its accompanying data in an instance of OutputPackageBase
+        list[tuple[str, OutputPackageBase]]:
+            A tuple holding the name of a pkgbase and its accompanying data in an instance of OutputPackageBase
         """
-
-        packages: Dict[str, outputpackage.OutputPackageBase] = {}
-        package_descs: Dict[str, PackageDesc] = {}
-        package_files: Dict[str, Files] = {}
+        packages: dict[str, outputpackage.OutputPackageBase] = {}
+        package_descs: dict[str, PackageDesc] = {}
+        package_files: dict[str, Files] = {}
 
         with open_tarfile(path=self.database, compression=self.compression_type) as db_file:
             for file_name in [
                 file_name for file_name in db_file.getnames() if re.search(r"(/desc|/files)$", file_name)
             ]:
                 pkgname = "".join(re.split("(-)", re.sub(r"(/desc|/files)$", "", file_name))[:-4])
 
@@ -473,107 +464,99 @@
                     )
                 else:  # pragma: no cover
                     # NOTE: this branch can never be reached, but we add it to make tests happy
                     raise RuntimeError(
                         f"The database file {self.database} contains the member {file_name} of an unsupported type!"
                     )
 
-        for (name, package_desc) in package_descs.items():
+        for name, package_desc in package_descs.items():
             if packages.get(package_desc.get_base()):
                 packages[package_desc.get_base()].add_packages(
                     [package_desc.get_output_package(files=package_files.get(name))]
                 )
             else:
                 packages.update(
                     {
                         package_desc.get_base(): package_desc.get_output_package_base(files=package_files.get(name)),
                     }
                 )
 
         return list(packages.items())
 
     async def stream_management_repo(self, path: Path) -> None:
-        """Stream descriptor files read from the JSON files of a management repository to the repository sync database
+        """Stream descriptor files read from JSON files of a management repository to the repository sync database.
 
         Parameters
         ----------
         path: Path
             The directory containing the files of the management repository
-
-        Raises
-        ------
-        RepoManagementFileNotFoundError
-            If no JSON files are found in path
         """
-
         file_list = sorted(path.glob("*.json"))
         if not file_list:
-            raise RepoManagementFileNotFoundError(f"There are no JSON files in {path}!")
+            debug(f"There are no JSON files in {path}! Creating empty sync db.")
 
         with open_tarfile(self.database, compression=self.compression_type, mode="w") as database_file:
             for json_file in file_list:
                 await SyncDatabase.outputpackagebase_to_tarfile(
                     tarfile=database_file,
                     database_type=self.database_type,
                     model=await outputpackage.OutputPackageBase.from_file(path=json_file),
                     packagedesc_version=self.desc_version,
                     files_version=self.files_version,
                 )
 
 
 class PackageDesc(BaseModel):
-    """A template class with helper methods to create instances of one of its (versioned) subclasses
+    """A template class with helper methods to create instances of one of its (versioned) subclasses.
 
     This class should not be instantiated directly, as it only provides generic instance methods for its subclasses.
 
     NOTE: The `from_dict()` classmethod is used to create one of the versioned subclasses.
     """
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Union[int, str, List[str]]]) -> PackageDesc:
-        """Create an instance of one of PackageDesc's subclasses from a dict
+    def from_dict(cls, data: dict[str, int | str | list[str]]) -> PackageDesc:
+        """Create an instance of one of PackageDesc's subclasses from a dict.
 
         This method should be used with data derived from reading a 'desc' file from a repository sync database.
 
         Parameters
         ----------
-        data: Dict[str, Union[int, str, List[str]]]
+        data: dict[str, int | str | list[str]]
             A dict containing data required to instantiate a subclass of PackageDesc
 
         Raises
         ------
         RepoManagementValidationError
             If a ValidationError is encountered while instantiating one of PackageDesc's subclasses
             If no supported schema_version can be found
 
         Returns
         -------
         PackageDesc
             An instance of one of the subclasses of PackageDesc
         """
 
-        def derive_package_desc_version(data: Set[str]) -> Optional[int]:
-            """Derive which PackageDesc subclass to instantiate
+        def derive_package_desc_version(data: set[str]) -> int | None:
+            """Derive which PackageDesc subclass to instantiate.
 
             Parameters
             ----------
-            data: Set[str]
+            data: set[str]
                  A set of strings representing the keys of the data dict passed to PackageDesc.from_dict()
 
             Returns
             -------
-            Optional[int]
+            int | None
                 The integer representing the version of the PackageDesc subclass, else None
             """
-
             for version, config in sorted(PACKAGE_DESC_VERSIONS.items(), reverse=True):
-
                 debug(f"Comparing 'desc' data to schema version {version}")
-                config_required: Set[str] = config["required"]  # type: ignore[assignment]
-                config_optional: Set[str] = config["optional"]  # type: ignore[assignment]
+                config_required: set[str] = config["required"]  # type: ignore[assignment]
+                config_optional: set[str] = config["optional"]  # type: ignore[assignment]
                 if config_required.issubset(data):
                     optionals = data - config_required
 
                     if len(optionals) > len(config_optional):
                         continue
                     else:
                         unmatched_optional = 0
@@ -596,34 +579,34 @@
 
         if detected_version is not None and (detected_version < DEFAULT_PACKAGE_DESC_VERSION):
             warning(f"Detected 'desc' version {detected_version}, but {DEFAULT_PACKAGE_DESC_VERSION} is the default!")
 
         match detected_version:
             case 1:
                 try:
-                    return PackageDescV1(**data)
+                    return PackageDescV1.model_validate(data)
                 except ValidationError as e:
                     raise RepoManagementValidationError(
                         "A validation error occured while attempting to instantiate a PackageDescV1 using the data:\n"
                         f"{data}\n{e}"
                     )
             case 2:
                 try:
-                    return PackageDescV2(**data)
+                    return PackageDescV2.model_validate(data)
                 except ValidationError as e:
                     raise RepoManagementValidationError(
                         "A validation error occured while attempting to instantiate a PackageDescV2 using the data:\n"
                         f"{data}\n{e}"
                     )
             case _:
                 raise RepoManagementValidationError(f"The data format of the 'desc' file is unknown:\n{data}")
 
     @classmethod
     async def from_stream(cls, data: io.StringIO) -> PackageDesc:
-        """Initialize a PackageDesc from an input stream
+        """Initialize a PackageDesc from an input stream.
 
         Parameters
         ----------
         data: io.StringIO
             A buffered I/O that represents a 'desc' file
 
         Raises
@@ -633,32 +616,31 @@
             is raised when converting data
 
         Returns
         -------
         PackageDesc
             A PackageDesc instance based on data
         """
-
         current_header = ""
         current_type: FieldTypeEnum
-        int_types: Dict[str, int] = {}
-        string_types: Dict[str, str] = {}
-        string_list_types: Dict[str, List[str]] = {}
+        int_types: dict[str, int] = {}
+        string_types: dict[str, str] = {}
+        string_list_types: dict[str, list[str]] = {}
         keys = get_desc_json_keys()
 
         for line in data:
             line = line.strip()
             if not line:
                 continue
 
             if line in keys:
                 current_header = get_desc_json_name(key=line)
                 current_type = get_desc_json_field_type(line)
-                # FIXME: find better way to provide a default (None or empty list for STRING_LIST as they all are
-                # Optional[List[str]]
+                # FIXME: find better way to provide a default
+                # (None or empty list for STRING_LIST as they all are list[str] | None)
                 if current_header and current_type == FieldTypeEnum.STRING_LIST:
                     string_list_types[current_header] = []
 
                 continue
 
             if current_header:
                 try:
@@ -673,61 +655,63 @@
                             pass
                 except ValueError as e:
                     raise RepoManagementValidationError(
                         "An error occured while attempting to cast values for a 'desc' file!\n"
                         f"\n{data.getvalue()}\n{e}"
                     )
 
-        desc_dict: Dict[str, Union[int, str, List[str]]] = {**int_types, **string_types, **string_list_types}
+        desc_dict: dict[str, int | str | list[str]] = {**int_types, **string_types, **string_list_types}
         try:
             return PackageDesc.from_dict(desc_dict)
         except RepoManagementValidationError as e:
             raise RepoManagementValidationError(
                 "An error occured while validating a 'desc' file!\n" f"\n{data.getvalue()}\n{e}"
             )
 
     async def render(self, output: io.StringIO) -> None:
-        """Use a 'desc' jinja template to write the PackageDesc contents to an output stream
+        """Use a 'desc' jinja template to write the PackageDesc contents to an output stream.
 
         Parameters
         ----------
         output: io.StringIO
             An output stream to write to
 
         Raises
         ------
         RepoManagementFileNotFoundError
             If no matching template can be found
         """
-
-        env = Environment(
+        # NOTE: We are not rendering HTML and need special characters, hence we are not affected by XSS problems and set
+        # autoescape=False
+        env = Environment(  # nosec: B701
+            autoescape=False,
             loader=PackageLoader("repod", "templates"),
             trim_blocks=True,
             lstrip_blocks=True,
             enable_async=True,
         )
         template_file = f"desc_v{self.get_schema_version()}.j2"
 
         debug(f"Rendering PackageDesc data using template file {template_file}...")
 
         try:
             template = env.get_template(template_file)
         except TemplateNotFound:
             raise RepoManagementFileNotFoundError(f"The 'desc' template file {template_file} could not be found!")
-        output.write(await template.render_async(self.dict()))
+        output.write(await template.render_async(self.model_dump(mode="json")))
 
-    def get_output_package(self, files: Optional[Files]) -> outputpackage.OutputPackage:
-        """Transform the PackageDesc model and an optional Files model into an OutputPackage model
+    def get_output_package(self, files: Files | None) -> outputpackage.OutputPackage:
+        """Transform the PackageDesc model and an optional Files model into an OutputPackage model.
 
         NOTE: This method only successfully returns if the instance of the class using it defines the required fields!
         The PackageDesc class does not do that!
 
         Parameters
         ----------
-        files: Optional[Files]:
+        files: Files | None:
             A pydantic model, that represents the list of files, that belong to the package described by self
 
         Raises
         ------
         RuntimeError
             If called on the PackageDesc template class
             If there is no matching OutputPackage schema_version defined in the configuration for the given
@@ -736,45 +720,44 @@
             If no configuration is available for a given PackageDesc.schema_version
 
         Returns
         -------
         OutputPackage
             A pydantic model, that describes a package and its list of files
         """
-
         schema_version = self.get_schema_version()
         schema_config = PACKAGE_DESC_VERSIONS.get(schema_version)
-        desc_dict = self.dict()
+        desc_dict = self.model_dump(mode="json")
         if schema_config:
             output_package_version = schema_config.get("output_package_version")
             match output_package_version:
                 case 1:
                     if files:
                         desc_dict["files"] = files
 
-                    return outputpackage.OutputPackageV1(**desc_dict)
+                    return outputpackage.OutputPackageV1.model_validate(desc_dict)
                 case _:
                     raise RuntimeError(
                         f"The OutputPackage version '{output_package_version}' is not valid. This is a bug!"
                     )
         else:
             raise RepoManagementValidationError(
                 f"The schema version '{schema_version}' is not valid for creating a "
                 "OutputPackage from a PackageDesc!"
             )
 
-    def get_output_package_base(self, files: Optional[Files]) -> outputpackage.OutputPackageBase:
-        """Transform the PackageDesc model and an Files model into an OutputPackageBase model
+    def get_output_package_base(self, files: Files | None) -> outputpackage.OutputPackageBase:
+        """Transform the PackageDesc model and an Files model into an OutputPackageBase model.
 
         NOTE: This method only successfully returns if the instance of the class using it defines the required fields!
         The PackageDesc class does not do that!
 
         Parameters
         ----------
-        files: Optional[Files]:
+        files: Files | None:
             A pydantic model, that represents the list of files, that belong to the package described by self
 
         Raises
         ------
         RuntimeError
             If called on the PackageDesc template class
             If there is no matching OutputPackage schema_version defined in the configuration for the given
@@ -783,154 +766,148 @@
             If no configuration is available for a given PackageDesc.schema_version
 
         Returns
         -------
         OutputPackageBase
             A pydantic model, that describes a package base and one of it's split packages
         """
-
         schema_version = self.get_schema_version()
         schema_config = PACKAGE_DESC_VERSIONS.get(schema_version)
-        desc_dict = self.dict()
+        desc_dict = self.model_dump(mode="json")
         if schema_config:
             output_package_version = schema_config.get("output_package_base_version")
             match output_package_version:
                 case 1:
                     desc_dict.update({"packages": [self.get_output_package(files=files)]})
-                    return outputpackage.OutputPackageBaseV1(**desc_dict)
+                    return outputpackage.OutputPackageBaseV1.model_validate(desc_dict)
                 case _:
                     raise RuntimeError(
                         f"The OutputPackageBase version '{output_package_version}' is not valid. This is a bug!"
                     )
         else:
             raise RepoManagementValidationError(
                 f"The schema version '{schema_version}' is not valid for creating a "
                 "OutputPackageBase from a PackageDesc!"
             )
 
     def get_base(self) -> str:
-        """Get the base attribute of the PackageDesc instance
+        """Get the base attribute of the PackageDesc instance.
 
         NOTE: This method only successfully returns if the instance of the class using it defines the `base` field! The
         PackageDesc class does not do that!
 
         Raises
         ------
         RuntimeError
             If the method is called on an instance of the PackageDesc template class
 
         Returns
         -------
         str
             The base attribute of a PackageDesc subclass
         """
-
         if hasattr(self, "base"):
-            return str(self.base)  # type: ignore[attr-defined]
+            return str(self.base)
         else:
             raise RuntimeError(
                 "It is not possible to retrieve the 'base' attribute from the template class PackageDesc!"
             )
 
     def get_name(self) -> str:
-        """Get the name attribute of the PackageDesc instance
+        """Get the name attribute of the PackageDesc instance.
 
         NOTE: This method only successfully returns if the instance of the class using it defines the `name` field! The
         PackageDesc class does not do that!
 
         Raises
         ------
         RuntimeError
             If the method is called on an instance of the PackageDesc template class
 
         Returns
         -------
         str
             The name attribute of a PackageDesc subclass
         """
-
         if hasattr(self, "name"):
-            return str(self.name)  # type: ignore[attr-defined]
+            return str(self.name)
         else:
             raise RuntimeError(
                 "It is not possible to retrieve the 'name' attribute from the template class PackageDesc!"
             )
 
     def get_schema_version(self) -> int:
-        """Get the schema_version attribute of the PackageDesc instance
+        """Get the schema_version attribute of the PackageDesc instance.
 
         NOTE: This method only successfully returns if the instance of the class using it defines the `schema_version`
         field! The PackageDesc class does not do that!
 
         Raises
         ------
         RuntimeError
             If the method is called on an instance of the PackageDesc template class
 
         Returns
         -------
         int
             The schema_version attribute of a PackageDesc subclass
         """
-
         if hasattr(self, "schema_version"):
-            return int(self.schema_version)  # type: ignore[attr-defined]
+            return int(self.schema_version)
         else:
             raise RuntimeError(
                 "It is not possible to retrieve the 'schema_version' attribute from the templatet class PackageDesc!"
             )
 
 
 class Files(BaseModel):
-    """A template class to describe files in the context of 'files' files in a repository sync database
+    """A template class to describe files in the context of 'files' files in a repository sync database.
 
     This class should not be instantiated directly, as it only provides generic instance methods for its subclasses.
 
     NOTE: The `from_dict()` classmethod is used to create one of the versioned subclasses.
     """
 
     @classmethod
-    def from_dict(cls, data: Dict[str, List[str]]) -> Files:
-        """Class method to create one of Files' subclasses from a dict
+    def from_dict(cls, data: dict[str, list[str]]) -> Files:
+        """Class method to create one of Files' subclasses from a dict.
 
         This method is supposed to be called with data derived from a 'files' file.
 
         Parameters
         ----------
-        data: Dict[str, List[str]]
+        data: dict[str, list[str]]
             A dict with required data read from a 'files' file, which is used to instantiate one of Files' subclasses
 
         Raises
         ------
         RepoManagementValidationError
             If a ValidationError occurs when instatiating one of Files' subclasses or if no valid schema version for the
             data could be derived.
 
         Returns
         -------
         Files
             A Files instance (technically only one of its subclasses), instantiated from data
         """
 
-        def derive_files_version(data: Set[str]) -> Optional[int]:
-            """Derive which Files subclass to instantiate
+        def derive_files_version(data: set[str]) -> int | None:
+            """Derive which Files subclass to instantiate.
 
             Parameters
             ----------
-            data: Set[str]
+            data: set[str]
                  A set of strings representing the keys of the data dict passed to Files.from_dict()
 
             Returns
             -------
-            Optional[int]
+            int | None
                 The integer representing the schema version of the Files subclass, else None
             """
-
             for version, config in sorted(FILES_VERSIONS.items(), reverse=True):
-
                 debug(f"Comparing 'files' data to schema version {version}")
                 config_required = config["required"]
                 config_optional = config["optional"]
                 if config_required.issubset(data):
                     optionals = data - config_required
 
                     if len(optionals) > len(config_optional):
@@ -955,28 +932,28 @@
 
         if detected_version is not None and (detected_version < DEFAULT_FILES_VERSION):
             warning(f"Detected 'files' version {detected_version}, but {DEFAULT_FILES_VERSION} is the default!")
 
         match detected_version:
             case 1:
                 try:
-                    return FilesV1(**data)
+                    return FilesV1.model_validate(data)
                 except ValidationError as e:
                     raise RepoManagementValidationError(
                         "A validation error occured while attempting to instantiate a FilesV1 using the data:\n"
                         f"{data}\n{e}"
                     )
             case _:
                 raise RepoManagementValidationError(
                     f"The data format '{detected_version}' of the 'files' file is unknown:\n{data}"
                 )
 
     @classmethod
     async def from_stream(cls, data: io.StringIO) -> Files:
-        """Initialize a Files from an input stream
+        """Initialize a Files from an input stream.
 
         Parameters
         ----------
         data: io.StringIO
             A buffered I/O that represents the contents of a 'files' file
 
         Raises
@@ -985,18 +962,17 @@
             If a pydantic.error_wrappers.ValidationError is raised (e.g. due to a missing attribute)
 
         Returns
         -------
         Files
             A Files instance based on data
         """
-
         current_header = ""
         current_type: FieldTypeEnum
-        string_list_types: Dict[str, List[str]] = {}
+        string_list_types: dict[str, list[str]] = {}
         keys = get_files_json_keys()
 
         for line in data:
             line = line.strip()
             if not line:
                 continue
 
@@ -1015,74 +991,74 @@
             return Files.from_dict(data=string_list_types)
         except RepoManagementValidationError as e:
             raise RepoManagementValidationError(
                 f"An error occured while validating a 'files' file!\n" f"\n{data.getvalue()}\n{e}"
             )
 
     async def render(self, output: io.StringIO) -> None:
-        """Use a 'files' jinja template to write the Files contents to an output stream
+        """Use a 'files' jinja template to write the Files contents to an output stream.
 
         Parameters
         ----------
         output: io.StringIO
             An output stream to write to
 
         Raises
         ------
         RepoManagementFileNotFoundError
             If no matching template can be found
         """
-
-        env = Environment(
+        # NOTE: We are not rendering HTML and need special characters, hence we are not affected by XSS problems and set
+        # autoescape=False
+        env = Environment(  # nosec: B701
             loader=PackageLoader("repod", "templates"),
             trim_blocks=True,
             lstrip_blocks=True,
             enable_async=True,
         )
         template_file = f"files_v{self.get_schema_version()}.j2"
 
         debug(f"Rendering Files data using template file {template_file}...")
 
         try:
             template = env.get_template(template_file)
         except TemplateNotFound:
             raise RepoManagementFileNotFoundError(f"The 'files' template file {template_file} could not be found!")
-        output.write(await template.render_async(self.dict()))
+        output.write(await template.render_async(self.model_dump(mode="json")))
 
     def get_schema_version(self) -> int:
-        """Get the schema_version of the Files instance
+        """Get the schema_version of the Files instance.
 
         NOTE: This method only successfully returns if the instance of the class using it actually defines the
         `schema_version` field!
 
         Raises
         ------
         RuntimeError
             If the method is called on an instance of the Files template class
 
         Returns
         -------
         int
             The schema_version attribute of a Files subclass
         """
-
         if hasattr(self, "schema_version"):
-            return int(self.schema_version)  # type: ignore[attr-defined]
+            return int(self.schema_version)
         else:
             raise RuntimeError(
                 "It is not possible to retrieve the 'schema_version' attribute from the Files template class!"
             )
 
 
 class FilesV1(Files, FileList, SchemaVersionV1):
-    """A pydantic model to describe files in the context of 'files' files in a repository sync database (version 1)
+    """A pydantic model to describe files in the context of 'files' files in a repository sync database (version 1).
 
     Attributes
     ----------
-    files: Optional[List[str]]
+    files: list[str] | None
         An optional list of files. This is the data below a %FILES% identifier in a 'files' file, which identifies which
         file(s) belong to a package
     """
 
     pass
 
 
@@ -1110,79 +1086,79 @@
     Provides,
     Replaces,
     SchemaVersionV1,
     Sha256Sum,
     Url,
     Version,
 ):
-    """A model describing all identifiers in a 'desc' file (version 1)
+    """A model describing all identifiers in a 'desc' file (version 1).
 
     Attributes
     ----------
     arch: str
         The attribute can be used to describe the (required) data below an %ARCH% identifier in a 'desc' file, which
         identifies a package's architecture
-    backup: Optional[List[str]]
+    backup: list[str] | None
         The attribute can be used to describe the (optional) data below a %BACKUP% identifier in a 'desc' file, which
         identifies which file(s) of a package pacman will create backups for
     base: str
         The attribute can be used to describe the (required) data below a %BASE% identifier in a 'desc' file, which
         identifies a package's pkgbase
     builddate: int
         The attribute can be used to describe the (required) data below a %BUILDDATE% identifier in a 'desc' file,
         which identifies a package's build date (represented in seconds since the epoch)
-    checkdepends: Optional[List[str]]
+    checkdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %CHECKDEPENDS% identifier in a 'desc' file,
         which identifies a package's checkdepends
-    conflicts: Optional[List[str]]
+    conflicts: list[str] | None
         The attribute can be used to describe the (optional) data below a %CONFLICTS% identifier in a 'desc' file, which
         identifies what other package(s) a package conflicts with
     csize: int
         The attribute can be used to describe the (required) data below a %CSIZE% identifier in a 'desc' file, which
         identifies a package's size
-    depends: Optional[List[str]]
+    depends: list[str] | None
         The attribute can be used to describe the (optional) data below a %DEPENDS% identifier in a 'desc' file, which
         identifies what other package(s) a package depends on
     desc: str
         The attribute can be used to describe the (required) data below a %DESC% identifier in a 'desc' file, which
         identifies a package's description
     filename: str
         The attribute can be used to describe the (required) data below a %FILENAME% identifier in a 'desc' file, which
         identifies a package's file name
-    groups: Optional[List[str]]
+    groups: list[str] | None
         The attribute can be used to describe the (optional) data below a %GROUPS% identifier in a 'desc' file, which
         identifies a package's groups
     isize: int
         The attribute can be used to describe the (required) data below an %ISIZE% identifier in a 'desc' file, which
         identifies a package's installed size
-    license: List[str]
+    license: list[str]
         The attribute can be used to describe the (required) data below a %LICENSE% identifier in a 'desc' file, which
         identifies a package's license(s)
-    makedepends: Optional[List[str]]
+    makedepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %MAKEDEPENDS% identifier in a 'desc' file,
         which identifies a package's makedepends
     md5sum: str
         The attribute can be used to describe the (required) data below an %MD5SUM% identifier in a 'desc' file, which
         identifies a package's md5 checksum
     name: str
         The attribute can be used to describe the (required) data below a %NAME% identifier in a 'desc' file, which
         identifies a package's name
-    optdepends: Optional[List[str]]
+    optdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
         which identifies what other package(s) a package optionally depends on
     packager: str
         The attribute can be used to describe the (required) data below a %PACKAGER% identifier in a 'desc' file, which
         identifies a package's packager
     pgpsig: str
         The attribute can be used to describe the (optional) data below a %PGPSIG% identifier in a 'desc' file, which
         identifies a package's PGP signature
-    provides: Optional[List[str]]
+    provides: list[str] | None
         The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
         identifies what other package(s) a package provides
-    replaces: Optional[List[str]]
+    replaces: list[str] | None
         The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
         identifies what other package(s) a package replaces
     schema_version: PositiveInt
         A positive integer - 1 - identifying the schema version of the object
     sha256sum: str
         The attribute can be used to describe the (required) data below an %SHA256SUM% identifier in a 'desc' file,
         which identifies a package's sha256 checksum
@@ -1218,76 +1194,76 @@
     Provides,
     Replaces,
     SchemaVersionV1,
     Sha256Sum,
     Url,
     Version,
 ):
-    """A model describing all identifiers in a 'desc' file (version 1)
+    """A model describing all identifiers in a 'desc' file (version 1).
 
     Attributes
     ----------
     arch: str
         The attribute can be used to describe the (required) data below an %ARCH% identifier in a 'desc' file, which
         identifies a package's architecture
-    backup: Optional[List[str]]
+    backup: list[str] | None
         The attribute can be used to describe the (optional) data below a %BACKUP% identifier in a 'desc' file, which
         identifies which file(s) of a package pacman will create backups for
     base: str
         The attribute can be used to describe the (required) data below a %BASE% identifier in a 'desc' file, which
         identifies a package's pkgbase
     builddate: int
         The attribute can be used to describe the (required) data below a %BUILDDATE% identifier in a 'desc' file,
         which identifies a package's build date (represented in seconds since the epoch)
-    checkdepends: Optional[List[str]]
+    checkdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %CHECKDEPENDS% identifier in a 'desc' file,
         which identifies a package's checkdepends
-    conflicts: Optional[List[str]]
+    conflicts: list[str] | None
         The attribute can be used to describe the (optional) data below a %CONFLICTS% identifier in a 'desc' file, which
         identifies what other package(s) a package conflicts with
     csize: int
         The attribute can be used to describe the (required) data below a %CSIZE% identifier in a 'desc' file, which
         identifies a package's size
-    depends: Optional[List[str]]
+    depends: list[str] | None
         The attribute can be used to describe the (optional) data below a %DEPENDS% identifier in a 'desc' file, which
         identifies what other package(s) a package depends on
     desc: str
         The attribute can be used to describe the (required) data below a %DESC% identifier in a 'desc' file, which
         identifies a package's description
     filename: str
         The attribute can be used to describe the (required) data below a %FILENAME% identifier in a 'desc' file, which
         identifies a package's file name
-    groups: Optional[List[str]]
+    groups: list[str] | None
         The attribute can be used to describe the (optional) data below a %GROUPS% identifier in a 'desc' file, which
         identifies a package's groups
     isize: int
         The attribute can be used to describe the (required) data below an %ISIZE% identifier in a 'desc' file, which
         identifies a package's installed size
-    license: List[str]
+    license: list[str]
         The attribute can be used to describe the (required) data below a %LICENSE% identifier in a 'desc' file, which
         identifies a package's license(s)
-    makedepends: Optional[List[str]]
+    makedepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %MAKEDEPENDS% identifier in a 'desc' file,
         which identifies a package's makedepends
     md5sum: str
         The attribute can be used to describe the (required) data below an %MD5SUM% identifier in a 'desc' file, which
         identifies a package's md5 checksum
     name: str
         The attribute can be used to describe the (required) data below a %NAME% identifier in a 'desc' file, which
         identifies a package's name
-    optdepends: Optional[List[str]]
+    optdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
         which identifies what other package(s) a package optionally depends on
     packager: str
         The attribute can be used to describe the (required) data below a %PACKAGER% identifier in a 'desc' file, which
         identifies a package's packager
-    provides: Optional[List[str]]
+    provides: list[str] | None
         The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
         identifies what other package(s) a package provides
-    replaces: Optional[List[str]]
+    replaces: list[str] | None
         The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
         identifies what other package(s) a package replaces
     schema_version: PositiveInt
         A positive integer - 1 - identifying the schema version of the object
     sha256sum: str
         The attribute can be used to describe the (required) data below an %SHA256SUM% identifier in a 'desc' file,
         which identifies a package's sha256 checksum
@@ -1296,32 +1272,36 @@
         identifies a package's URL
     version: str
         The attribute can be used to describe the (required) data below a %VERSION% identifier in a 'desc' file, which
         identifies a package's version (this is the accumulation of epoch, pkgver and pkgrel)
     """
 
 
-def export_schemas(output: Union[Path, str]) -> None:
-    """Export the JSON schema of selected pydantic models to an output directory
+def export_schemas(output: Path | str) -> None:
+    """Export the JSON schema of selected pydantic models to an output directory.
 
     Parameters
     ----------
     output: Path
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-
     classes = [FilesV1, PackageDescV1, PackageDescV2]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
 
     for class_ in classes:
-        with open(output / f"{class_.__name__}.json", "w") as f:
-            print(class_.schema_json(indent=2), file=f)
+        with open(output / f"{class_.__name__}.json", "wb") as f:
+            f.write(
+                dumps(
+                    class_.model_json_schema(),  # type: ignore[attr-defined]
+                    option=OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS,
+                )
+            )
```

### Comparing `repod-0.2.2/repod/templates/desc_v1.j2` & `repod-0.3.0.post0/repod/templates/desc_v1.j2`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/repod/templates/desc_v2.j2` & `repod-0.3.0.post0/repod/templates/desc_v2.j2`

 * *Files identical despite different names*

### Comparing `repod-0.2.2/repod/verification/pgp.py` & `repod-0.3.0.post0/repod/verification/pgp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,60 @@
+"""Implementation of PGP based verification."""
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from logging import info
 from pathlib import Path
 
 from repod.commands import run_command
 
 
 class PGPVerifier(ABC):
-    """An abstract base class implementing PGP verification"""
+    """An abstract base class implementing PGP verification."""
 
     @abstractmethod
-    def verify(self, package: Path, signature: Path) -> bool:
-        """An abstractmethod to verify a package and its accompanying signature
+    def verify(self: PGPVerifier, package: Path, signature: Path) -> bool:
+        """Verify a package and its accompanying signature.
 
         Parameters
         ----------
         package: Path
             The path to a package file
         signature: Path
             The path to a PGP signature for package
 
         Returns
         -------
         bool
             True if the signature can be verified, False otherwise
         """
-
         pass  # pragma: nocover
 
 
 class PacmanKeyVerifier(PGPVerifier):
-    """A class implementing PGP verification using pacman-key"""
+    """A class implementing PGP verification using pacman-key."""
 
-    def verify(self, package: Path, signature: Path) -> bool:
-        """Verify the detached PGP signature of a package file using pacman-key --verify
+    def verify(self: PGPVerifier, package: Path, signature: Path) -> bool:
+        """Verify the detached PGP signature of a package file using pacman-key --verify.
 
         Parameters
         ----------
         package: Path
             The path to a package file
         signature: Path
             The path to a PGP signature for package
 
         Returns
         -------
         bool
             True if the signature can be verified, False otherwise
         """
-
         result = run_command(
             cmd=["pacman-key", "--verify", f"{signature}"],
             quiet=True,
         )
 
-        if result.returncode == 0:
-            return True
-        else:
+        if result.returncode != 0:
             info(f"The package file {package} could not be verified using the signature {signature}!\n{result.stderr}")
             return False
+
+        return True
```

### Comparing `repod-0.2.2/repod/version/alpm.py` & `repod-0.3.0.post0/repod/version/alpm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""An implementation of libalpm functionality for version comparison."""
 from itertools import takewhile
 
 from .util import cmp
 
 PYALPM_VERCMP = False
 try:
     from pyalpm import vercmp as pyalpm_vercmp  # pragma: no-cover-nonlinux
@@ -21,15 +22,14 @@
     Returns
     -------
     int
         -1 if a is newer than b
          0 if a and b are the same version
          1 if b is newer than a
     """
-
     if PYALPM_VERCMP:  # pragma: no-cover-nonlinux
         return int(pyalpm_vercmp(a, b))  # pragma: no-cover-nonlinux
 
     # easy comparison to see if versions are identical
     if a == b:
         return 0
 
@@ -132,29 +132,27 @@
     """
     if (not one and not two[0].isalpha()) or (one and one[0].isalpha()):
         return -1
     return 1
 
 
 def pkg_vercmp(a: str, b: str) -> int:
-    """Compare individual components of two versions by splitting them
-    based in alpm's version schema into epoch, pkgver, pkgrel.
+    """Compare individual components of versions by splitting based on alpm's version scheme into epoch, pkgver, pkgrel.
 
     The comparison algorithm is based on libalpm pacman's vercmp behavior.
 
     Calls pyalpm's interface in case it's available.
 
     Returns
     -------
     int
         -1 if a is newer than b
          0 if a and b are the same version
          1 if b is newer than a
     """
-
     if PYALPM_VERCMP:  # pragma: no-cover-nonlinux
         return int(pyalpm_vercmp(a, b))  # pragma: no-cover-nonlinux
 
     epoch1 = a.split(":")[0] if ":" in a else ""
     epoch2 = b.split(":")[0] if ":" in b else ""
 
     pkgver_pkgrel1 = a.split(":")[1] if ":" in a else a
```

### Comparing `repod-0.2.2/repod/version/util.py` & `repod-0.3.0.post0/repod/version/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Any
+"""A version utility module."""
 
 
-def cmp(a: Any, b: Any) -> int:
+def cmp(a: int | str, b: int | str) -> int:
     """
-    C style cmp function returning the compare result as int
+    C style cmp function returning the compare result as int.
 
     Compare the two objects a and b and return an integer according to
     the outcome. The return value is negative if x < b, zero if a == b
     and strictly positive if a > b.
 
     Parameters
     ----------
@@ -19,8 +19,8 @@
     Returns
     -------
     int
         -1 if 'b' is greater
          0 if both are equal
          1 if 'a' is greater
     """
-    return int(a > b) - int(a < b)
+    return int(str(a) > str(b)) - int(str(a) < str(b))
```

### Comparing `repod-0.2.2/tests/cli/test_cli.py` & `repod-0.3.0.post0/tests/cli/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,40 @@
+"""Tests for repod.cli.cli."""
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
-from contextlib import nullcontext as does_not_raise
 from logging import DEBUG
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
 from tempfile import TemporaryDirectory
-from typing import ContextManager, Optional, Tuple
 from unittest.mock import Mock, patch
 
 from pytest import LogCaptureFixture, mark, raises
 
 from repod import commands
 from repod.cli import cli
 from repod.common.enums import (
     ArchitectureEnum,
     FilesVersionEnum,
     PackageDescVersionEnum,
-    PkgVerificationTypeEnum,
     tar_compression_types_for_filename_regex,
 )
 from repod.config import UserSettings
 from repod.config.defaults import DEFAULT_DATABASE_COMPRESSION
 
 
 @mark.parametrize(
     "message, argparser",
     [
         ("foo", None),
         ("foo", ArgumentParser()),
     ],
 )
 @patch("repod.cli.cli.exit")
-def test_exit_on_error(exit_mock: Mock, message: str, argparser: Optional[ArgumentParser]) -> None:
+def test_exit_on_error(exit_mock: Mock, message: str, argparser: ArgumentParser | None) -> None:
+    """Tests for repod.cli.cli.exit_on_error."""
     cli.exit_on_error(message=message, argparser=argparser)
     exit_mock.assert_called_once_with(1)
 
 
 @mark.parametrize(
     "args, calls_exit_on_error",
     [
@@ -50,20 +49,20 @@
         (Namespace(package="foo"), True),
     ],
 )
 @patch("repod.cli.cli.exit_on_error")
 def test_repod_file_package(
     exit_on_error_mock: Mock,
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
-    debug_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     tmp_path: Path,
     args: Namespace,
     calls_exit_on_error: bool,
 ) -> None:
+    """Tests for repod.cli.cli.repod_file_package."""
     caplog.set_level(DEBUG)
 
     settings_mock = Mock()
     args.file = [default_package_file[0]]
 
     cli.repod_file_package(args=args, settings=settings_mock)
     if calls_exit_on_error:
@@ -99,27 +98,29 @@
             ),
             False,
         ),
         (Namespace(repo="foo"), True),
     ],
 )
 @patch("repod.cli.cli.repod_file_repo_importpkg")
+@patch("repod.cli.cli.write_sync_databases")
 @patch("repod.cli.cli.exit_on_error")
 def test_repod_file_repo(
     exit_on_error_mock: Mock,
+    write_sync_databases_mock: Mock,
     repod_file_repo_importpkg_mock: Mock,
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
-    debug_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     outputpackagebasev1_json_files_in_dir: Path,
-    default_sync_db_file: Tuple[Path, Path],
+    default_sync_db_file: tuple[Path, Path],
     tmp_path: Path,
     args: Namespace,
     calls_exit_on_error: bool,
 ) -> None:
+    """Tests for repod.cli.cli.repod_file_repo."""
     caplog.set_level(DEBUG)
 
     settings_mock = Mock()
     settings_mock.get_repo_path = Mock(return_value=tmp_path)
     settings_mock.get_repo_database_compression = Mock(return_value=DEFAULT_DATABASE_COMPRESSION)
     syncdb_settings_mock = Mock()
     syncdb_settings_mock.desc_version = PackageDescVersionEnum.DEFAULT
@@ -131,209 +132,89 @@
         args.name = tmp_path
     if args.repo == "writedb":
         args.name = "default"
 
     cli.repod_file_repo(args=args, settings=settings_mock)
     if args.repo == "importpkg":
         repod_file_repo_importpkg_mock.assert_called_once()
+    if args.repo == "writedb":
+        write_sync_databases_mock.assert_called_once()
     if calls_exit_on_error:
         exit_on_error_mock.assert_called_once()
 
 
-@mark.parametrize(
-    "package_verification, package_verifies, debug_pkg, args, expectation",
-    [
-        (
-            None,
-            True,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=True,
-                with_signature=False,
-                debug=False,
-                staging=False,
-                testing=False,
-            ),
-            does_not_raise(),
-        ),
-        (
-            None,
-            True,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=False,
-                with_signature=False,
-                debug=False,
-                staging=False,
-                testing=False,
-            ),
-            does_not_raise(),
-        ),
-        (
-            None,
-            True,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=True,
-                with_signature=False,
-                debug=True,
-                staging=False,
-                testing=False,
-            ),
-            raises(RuntimeError),
-        ),
-        (
-            None,
-            True,
-            True,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=True,
-                with_signature=False,
-                debug=False,
-                staging=False,
-                testing=False,
-            ),
-            raises(RuntimeError),
-        ),
-        (
-            None,
-            True,
-            True,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=True,
-                with_signature=False,
-                debug=True,
-                staging=False,
-                testing=False,
-            ),
-            does_not_raise(),
-        ),
-        (
-            None,
-            True,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=False,
-                with_signature=False,
-                debug=True,
-                staging=False,
-                testing=False,
-            ),
-            raises(RuntimeError),
-        ),
-        (
-            PkgVerificationTypeEnum.PACMANKEY,
-            True,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=True,
-                with_signature=True,
-                debug=False,
-                staging=False,
-                testing=False,
-            ),
-            does_not_raise(),
-        ),
-        (
-            PkgVerificationTypeEnum.PACMANKEY,
-            False,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=True,
-                with_signature=True,
-                debug=False,
-                staging=False,
-                testing=False,
-            ),
-            raises(RuntimeError),
-        ),
-        (
-            None,
-            True,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=False,
-                with_signature=True,
-                debug=False,
-                staging=False,
-                testing=False,
-            ),
-            does_not_raise(),
-        ),
-        (
-            None,
-            True,
-            False,
-            Namespace(
-                repo="importpkg",
-                architecture=ArchitectureEnum.ANY,
-                dry_run=True,
-                with_signature=True,
-                debug=True,
-                staging=False,
-                testing=False,
-            ),
-            raises(RuntimeError),
-        ),
-    ],
-)
+@mark.parametrize("dry_run", [(True), (False)])
+@patch("repod.cli.cli.add_packages_dryrun")
+@patch("repod.cli.cli.add_packages")
 def test_repod_file_repo_importpkg(
-    caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
-    debug_package_file: Tuple[Path, ...],
-    outputpackagebasev1_json_files_in_dir: Path,
-    default_sync_db_file: Tuple[Path, Path],
-    tmp_path: Path,
+    add_packages_mock: Mock,
+    add_packages_dryrun_mock: Mock,
+    dry_run: bool,
     usersettings: UserSettings,
-    package_verification: Optional[PkgVerificationTypeEnum],
-    package_verifies: bool,
-    debug_pkg: bool,
-    args: Namespace,
-    expectation: ContextManager[str],
+    caplog: LogCaptureFixture,
 ) -> None:
+    """Tests for repod.cli.cli.repod_file_importpkg."""
     caplog.set_level(DEBUG)
 
-    usersettings.package_verification = package_verification
-    args.file = [debug_package_file[0] if debug_pkg else default_package_file[0]]
-    args.name = Path("default")
-
-    with patch("repod.cli.cli.PacmanKeyVerifier", Mock(return_value=Mock(verify=Mock(return_value=package_verifies)))):
-        with expectation:
-            cli.repod_file_repo_importpkg(args=args, settings=usersettings)
+    file: list[Path] = []
+    name = Path("foo")
+    architecture = ArchitectureEnum.ANY
+    debug_bool = False
+    staging_bool = False
+    testing_bool = False
+    with_signature = True
+    namespace = Namespace(
+        file=file,
+        name=name,
+        architecture=architecture,
+        debug=debug_bool,
+        staging=staging_bool,
+        testing=testing_bool,
+        with_signature=with_signature,
+        dry_run=dry_run,
+        source_url=[],
+    )
+
+    cli.repod_file_repo_importpkg(args=namespace, settings=usersettings)
+    if dry_run:
+        add_packages_dryrun_mock.assert_called_once_with(
+            settings=usersettings,
+            files=file,
+            repo_name=name,
+            repo_architecture=architecture,
+            debug_repo=debug_bool,
+            with_signature=with_signature,
+            pkgbase_urls={},
+        )
+    else:
+        add_packages_mock.assert_called_once_with(
+            settings=usersettings,
+            files=file,
+            repo_name=name,
+            repo_architecture=architecture,
+            debug_repo=debug_bool,
+            staging_repo=staging_bool,
+            testing_repo=testing_bool,
+            with_signature=with_signature,
+            pkgbase_urls={},
+        )
 
 
 @mark.parametrize(
     "args, calls_exit_on_error",
     [(Namespace(schema="export"), False), (Namespace(schema="foo"), True)],
 )
 @patch("repod.cli.cli.exit_on_error")
 def test_repod_file_schema(
     exit_on_error_mock: Mock,
     tmp_path: Path,
     args: Namespace,
     calls_exit_on_error: bool,
 ) -> None:
+    """Tests for repod.cli.cli.repod_file_schema."""
     if args.schema == "export":
         args.dir = tmp_path
 
     cli.repod_file_schema(args=args)
     if calls_exit_on_error:
         exit_on_error_mock.assert_called_once()
 
@@ -419,14 +300,15 @@
     parse_args_mock: Mock,
     repod_file_package_mock: Mock,
     repod_file_repo_mock: Mock,
     repod_file_schema_mock: Mock,
     args: Namespace,
     calls_exit_on_error: bool,
 ) -> None:
+    """Tests for repod.cli.cli.repod_file."""
     user_settings = Mock()
     usersettings_mock.return_value = user_settings
     system_settings = Mock()
     systemsettings_mock.return_value = system_settings
 
     parse_args_mock.return_value = args
 
@@ -450,27 +332,43 @@
 
     if calls_exit_on_error:
         exit_on_error_mock.assert_called_once()
 
 
 @patch("repod.cli.argparse.ArgumentParser.parse_args")
 def test_repod_file_raise_on_argumenterror(parse_args_mock: Mock) -> None:
+    """Tests for repod.cli.cli.repod_file raising on ArgumentTypeError."""
     parse_args_mock.side_effect = ArgumentTypeError
     with raises(RuntimeError):
         cli.repod_file()
 
 
 def transform_databases(repo_name: str, base_path: Path) -> None:
+    """Transform a repository sync database to management repository and back.
+
+    Repository sync databases in default locations on pacman based distributions (i.e. /var/lib/pacman/sync/) are
+    considered by name.
+
+    Parameters
+    ----------
+    repo_name: str
+        Name of the repository (identifying a local repository sync database)
+    base_path: Path
+        The base directory below which repod specific data is stored
+    """
     custom_config = f"""
     [[repositories]]
 
+    architecture = "x86_64"
     name = "{base_path}/data/repo/package/{repo_name}"
     debug = "{base_path}/data/repo/package/{repo_name}-debug"
     staging = "{base_path}/data/repo/package/{repo_name}-staging"
+    staging_debug = "{base_path}/data/repo/package/{repo_name}-staging-debug"
     testing = "{base_path}/data/repo/package/{repo_name}-testing"
+    testing_debug = "{base_path}/data/repo/package/{repo_name}-testing-debug"
     package_pool = "{base_path}/data/pool/package/{repo_name}"
     source_pool = "{base_path}/data/pool/source/{repo_name}"
 
     [repositories.management_repo]
     directory = "{base_path}/management/{repo_name}"
     """
 
@@ -503,16 +401,29 @@
             f"{base_path}/data/repo/package/{repo_name}/",
         ],
         debug=True,
         check=True,
     )
 
 
-def list_database(repo_name: str, base_path: Path) -> None:
-    syncdb_path = Path(f"{base_path}/data/repo/package/{repo_name}/any/")
+def list_database(repo_name: str, base_path: Path, architecture: str) -> None:
+    """List contents (packages) of a repository sync database and files tracked in a files database of a repository.
+
+    First all package names of the repository are printed, afterwards all files.
+
+    Parameters
+    ----------
+    repo_name: str
+        Name of the repository (identifying a local repository sync database)
+    base_path: Path
+        The base directory below which repod specific data is stored
+    architecture: str
+        The architecture of the repository
+    """
+    syncdb_path = Path(f"{base_path}/data/repo/package/{repo_name}/{architecture}/")
     with TemporaryDirectory(prefix="pacman_", dir=base_path) as dbpath:
         (Path(dbpath) / "sync").symlink_to(syncdb_path)
         cache_path = base_path / "cache"
         cache_path.mkdir(parents=True)
         pacman_conf_path = cache_path / "pacman.conf"
         pacman_conf_contents = f"""[options]
         HoldPkg = pacman glibc
@@ -562,110 +473,146 @@
 
 
 @mark.integration
 @mark.skipif(
     not Path("/var/lib/pacman/sync/core.files").exists(),
     reason="/var/lib/pacman/sync/core.files does not exist",
 )
-def test_transform_core_databases(empty_dir: Path, tmp_path: Path) -> None:
+def test_transform_core_databases(tmp_path: Path) -> None:
+    """Integration tests for transforming the packages of a repository named core."""
     name = "core"
     transform_databases(repo_name=name, base_path=tmp_path)
-    list_database(repo_name=name, base_path=tmp_path)
+    list_database(repo_name=name, base_path=tmp_path, architecture="x86_64")
 
 
 @mark.integration
 @mark.skipif(
     not Path("/var/lib/pacman/sync/extra.files").exists(),
     reason="/var/lib/pacman/sync/extra.files does not exist",
 )
-def test_transform_extra_databases(empty_dir: Path, tmp_path: Path) -> None:
+def test_transform_extra_databases(tmp_path: Path) -> None:
+    """Integration tests for transforming the packages of a repository named extra."""
     name = "extra"
     transform_databases(repo_name=name, base_path=tmp_path)
-    list_database(repo_name=name, base_path=tmp_path)
+    list_database(repo_name=name, base_path=tmp_path, architecture="x86_64")
 
 
 @mark.integration
 @mark.skipif(
     not Path("/var/lib/pacman/sync/community.files").exists(),
     reason="/var/lib/pacman/sync/community.files does not exist",
 )
-def test_transform_community_databases(empty_dir: Path, tmp_path: Path) -> None:
+def test_transform_community_databases(tmp_path: Path) -> None:
+    """Integration tests for transforming the packages of a repository named community."""
     name = "community"
     transform_databases(repo_name="community", base_path=tmp_path)
-    list_database(repo_name=name, base_path=tmp_path)
+    list_database(repo_name=name, base_path=tmp_path, architecture="x86_64")
 
 
 @mark.integration
 @mark.skipif(
     not Path("/var/lib/pacman/sync/multilib.files").exists(),
     reason="/var/lib/pacman/sync/multilib.files does not exist",
 )
-def test_transform_multilib_databases(empty_dir: Path, tmp_path: Path) -> None:
+def test_transform_multilib_databases(tmp_path: Path) -> None:
+    """Integration tests for transforming the packages of a repository named multilib."""
     name = "multilib"
     transform_databases(repo_name=name, base_path=tmp_path)
-    list_database(repo_name=name, base_path=tmp_path)
+    list_database(repo_name=name, base_path=tmp_path, architecture="x86_64")
 
 
 @mark.integration
 @mark.skipif(
     not Path("/var/cache/pacman/pkg/").exists(),
     reason="Package cache in /var/cache/pacman/pkg/ does not exist",
 )
 def test_import_into_default_repo(tmp_path: Path) -> None:
+    """Integration tests for importing a set of packages into a repod managed repository."""
     packages = sorted(
         [
-            path
+            str(path)
             for path in list(Path("/var/cache/pacman/pkg/").iterdir())
             if isinstance(fullmatch(rf"^.*\.pkg\.tar({tar_compression_types_for_filename_regex()})$", str(path)), Match)
         ]
     )
-    if len(packages) > 50:
-        packages = sample(packages, 50)
+    if len(packages) > 5:
+        packages = sample(packages, 5)
 
     custom_config = f"""
-    [[repositories]]
+    archiving = {{ packages = "{tmp_path}/archive/package/", sources = "{tmp_path}/archive/sources/" }}
 
+    [[repositories]]
+    architecture = "x86_64"
+    build_requirements_exist = false
     name = "{tmp_path}/data/repo/package/default/"
     debug = "{tmp_path}/data/repo/package/default-debug/"
     staging = "{tmp_path}/data/repo/package/default-staging/"
+    staging_debug = "{tmp_path}/data/repo/package/default-staging-debug/"
     testing = "{tmp_path}/data/repo/package/default-testing/"
+    testing_debug = "{tmp_path}/data/repo/package/default-testing-debug/"
     package_pool = "{tmp_path}/data/pool/package/default/"
     source_pool = "{tmp_path}/data/pool/source/default/"
 
     [repositories.management_repo]
     directory = "{tmp_path}/management/default/"
     """
 
     config_path = tmp_path / "repod.conf"
     with open(config_path, "w") as file:
         file.write(custom_config)
 
-    for package in packages:
-        commands.run_command(
-            cmd=[
-                "repod-file",
-                "-d",
-                "-c",
-                f"{config_path}",
-                "repo",
-                "importpkg",
-                "-s",
-                f"{package}",
-                f"{tmp_path}/data/repo/package/default/",
-            ],
-            debug=True,
-            check=True,
-        )
+    commands.run_command(
+        cmd=[
+            "repod-file",
+            "-d",
+            "-c",
+            f"{config_path}",
+            "repo",
+            "importpkg",
+            "-s",
+        ]
+        + packages
+        + [f"{tmp_path}/data/repo/package/default/"],
+        debug=True,
+        check=True,
+    )
+    list_database(repo_name="default", base_path=tmp_path, architecture="x86_64")
+
+
+@mark.integration
+def test_write_empty_sync_db(tmp_path: Path) -> None:
+    """Integration tests for writing an empty repository sync database."""
+    custom_config = f"""
+    [[repositories]]
+
+    architecture = "x86_64"
+    name = "{tmp_path}/data/repo/package/default/"
+    debug = "{tmp_path}/data/repo/package/default-debug/"
+    staging = "{tmp_path}/data/repo/package/default-staging/"
+    staging_debug = "{tmp_path}/data/repo/package/default-staging-debug/"
+    testing = "{tmp_path}/data/repo/package/default-testing/"
+    testing_debug = "{tmp_path}/data/repo/package/default-testing-debug/"
+    package_pool = "{tmp_path}/data/pool/package/default/"
+    source_pool = "{tmp_path}/data/pool/source/default/"
+
+    [repositories.management_repo]
+    directory = "{tmp_path}/management/default/"
+    """
+
+    config_path = tmp_path / "repod.conf"
+    with open(config_path, "w") as file:
+        file.write(custom_config)
 
     commands.run_command(
         cmd=[
             "repod-file",
             "-d",
             "-c",
             f"{config_path}",
             "repo",
             "writedb",
             f"{tmp_path}/data/repo/package/default/",
         ],
         debug=True,
         check=True,
     )
+    list_database(repo_name="default", base_path=tmp_path, architecture="x86_64")
```

### Comparing `repod-0.2.2/tests/conftest.py` & `repod-0.3.0.post0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,264 +1,298 @@
+"""Pytest conftest."""
 import gzip
 import sys
 from copy import deepcopy
 from io import BytesIO, StringIO
+from logging import DEBUG, debug
 from os import chdir
 from pathlib import Path
 from random import choice
 from string import ascii_lowercase, ascii_uppercase, digits
 from tarfile import open as tarfile_open
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from textwrap import dedent
-from typing import IO, Any, AsyncGenerator, Generator, List, Tuple
-from unittest.mock import patch
+from typing import IO, Any, AsyncGenerator, Generator
+from unittest.mock import Mock, patch
 
 import orjson
 import pytest_asyncio
 from pydantic import BaseModel
-from pytest import fixture
+from pytest import LogCaptureFixture, fixture
 
 from repod.common.enums import (
     ArchitectureEnum,
     CompressionTypeEnum,
     FilesVersionEnum,
     PackageDescVersionEnum,
     PkgTypeEnum,
 )
 from repod.config.settings import (
     DEFAULT_ARCHITECTURE,
     DEFAULT_DATABASE_COMPRESSION,
     DEFAULT_NAME,
+    ArchiveSettings,
     ManagementRepo,
     PackageRepo,
     UserSettings,
 )
 from repod.files import open_tarfile
 from repod.files.buildinfo import BuildInfo, BuildInfoV1, BuildInfoV2
 from repod.files.common import ZstdTarFile
 from repod.files.mtree import MTree, MTreeEntryV1
 from repod.files.package import PackageV1
 from repod.files.pkginfo import PkgInfo, PkgInfoV1, PkgInfoV2, PkgType
 from repod.repo.management import OutputBuildInfo, OutputPackageBase
 from repod.repo.management.outputpackage import OutputPackageBaseV1, OutputPackageV1
 from repod.repo.package import Files, PackageDesc, RepoDbTypeEnum
+from repod.repo.package.repofile import relative_to_shared_base
 from repod.repo.package.syncdb import (
     FilesV1,
     PackageDescV1,
     PackageDescV2,
     SyncDatabase,
 )
 
 
 class SchemaVersion9999(BaseModel):
+    """An invalid SchemaVersion."""
+
     schema_version: int = 9999
 
 
 class BuildInfoV9999(BuildInfo, SchemaVersion9999):
+    """An invalid BuildInfo."""
+
     pass
 
 
 class FilesV9999(Files, SchemaVersion9999):
+    """An invalid Files."""
+
     pass
 
 
 class OutputPackageBaseV9999(OutputPackageBase, SchemaVersion9999):
+    """An invalid OutputPackageBase."""
+
     pass
 
 
 class PackageDescV9999(PackageDesc, SchemaVersion9999):
+    """An invalid PackageDesc."""
+
     pass
 
 
 def create_default_arch() -> str:
-    return str(choice([arch.value for arch in ArchitectureEnum]))
+    """Return a (pseudo-randomly selected) ArchitectureEnum as string."""
+    return str(choice([arch.value for arch in ArchitectureEnum]))  # nosec: B311
 
 
 @fixture(scope="session")
 def default_arch() -> str:
+    """Return a session-wide (pseudo-randomly selected) ArchitectureEnum as string."""
     return create_default_arch()
 
 
 def create_base64_pgpsig() -> str:
-    return "".join(choice(ascii_uppercase + ascii_lowercase + digits + "/+") for x in range(400)) + "=="
+    """Return a fake base64 encoded PGP signature string."""
+    return "".join(choice(ascii_uppercase + ascii_lowercase + digits + "/+") for x in range(400)) + "=="  # nosec: B311
 
 
 @fixture(scope="session")
 def base64_pgpsig() -> str:
+    """Return a session-wide fake base64 encoded PGP signature string."""
     return create_base64_pgpsig()
 
 
 def create_default_buildenv() -> str:
+    """Return a dummy repod.files.buildinfo.BuildEnv string."""
     return "foo"
 
 
 @fixture(scope="session")
 def default_buildenv() -> str:
+    """Return a session-wide dummy repod.files.buildinfo.BuildEnv string."""
     return create_default_buildenv()
 
 
 def create_default_invalid_buildenv() -> str:
+    """Return an invalid repod.files.buildinfo.BuildEnv string."""
     return "! foo"
 
 
 @fixture(scope="session")
 def default_invalid_buildenv() -> str:
+    """Return a session-wide invalid repod.files.buildinfo.BuildEnv string."""
     return create_default_invalid_buildenv()
 
 
 def create_default_description() -> str:
+    """Return a dummy description string."""
     return "description"
 
 
 @fixture(scope="session")
 def default_description() -> str:
+    """Return a session-wide dummy description string."""
     return create_default_description()
 
 
 def create_default_filename() -> str:
+    """Return a dummy package filename string."""
     return f"foo-{create_default_full_version()}-any.pkg.tar.zst"
 
 
 @fixture(scope="session")
 def default_filename() -> str:
+    """Return a session-wide dummy package filename string."""
     return create_default_filename()
 
 
 def create_default_license() -> str:
+    """Return a dummy license string."""
     return "GPL"
 
 
 @fixture(scope="session")
 def default_license() -> str:
+    """Return a session-wide dummy license string."""
     return create_default_license()
 
 
 def create_default_full_version() -> str:
+    """Return a version string (including epoch, pkgver and pkgrel)."""
     return "1:1.0.0-1"
 
 
 @fixture(scope="session")
 def default_full_version() -> str:
+    """Return a session-wide version string (including epoch, pkgver and pkgrel)."""
     return create_default_full_version()
 
 
 def create_default_invalid_full_version() -> str:
+    """Return an invalid version string."""
     return "0:1/0-0.1"
 
 
 @fixture(scope="function")
 def default_invalid_full_version() -> str:
+    """Return a session-wide invalid version string."""
     return create_default_invalid_full_version()
 
 
 def create_default_option() -> str:
+    """Return a dummy option string."""
     return "foo"
 
 
 @fixture(scope="session")
 def default_option() -> str:
+    """Return a session-wide dummy option string."""
     return create_default_option()
 
 
 def create_default_invalid_option() -> str:
+    """Return an invalid option string."""
     return "! foo"
 
 
 @fixture(scope="function")
 def default_invalid_option() -> str:
+    """Return a session-wide invalid option string."""
     return create_default_invalid_option()
 
 
 def create_default_package_name() -> str:
+    """Return a dummy package name string."""
     return "foo"
 
 
 @fixture(scope="session")
 def default_package_name() -> str:
+    """Return a session-wide dummy package name string."""
     return create_default_package_name()
 
 
 def create_default_invalid_package_name() -> str:
+    """Return an invalid package name string."""
     return ".foo"
 
 
 @fixture(scope="session")
 def default_invalid_package_name() -> str:
+    """Return a session-wide invalid package name string."""
     return create_default_invalid_package_name()
 
 
 def create_default_packager() -> str:
+    """Return a dummy packager string."""
     return "Foobar McFooface <foobar@archlinux.org>"
 
 
 @fixture(scope="session")
 def default_packager() -> str:
+    """Return a session-wide dummy packager string."""
     return create_default_packager()
 
 
 def create_default_invalid_packager() -> str:
+    """Return an invalid packager string."""
     return "Foobar McFooface <foo>"
 
 
 @fixture(scope="session")
 def default_invalid_packager() -> str:
+    """Return a session-wide invalid packager string."""
     return create_default_invalid_packager()
 
 
 @fixture(scope="session")
 def default_pkgtype() -> str:
+    """Return a session-wide pkgtype string."""
     return "pkg"
 
 
 @fixture(scope="session")
 def default_invalid_pkgtype() -> str:
+    """Return a session-wide invalid pkgtype string."""
     return "foo"
 
 
 def create_url() -> str:
+    """Return a dummy URL string."""
     return "https://foobar.tld"
 
 
 @fixture(scope="session")
 def url() -> str:
+    """Return a session-wide dummy URL string."""
     return create_url()
 
 
 @fixture(scope="session")
 def default_version() -> str:
+    """Return a session-wide version (pkgver) string."""
     return "1.0.0"
 
 
 @fixture(scope="session")
 def default_invalid_version() -> str:
+    """Return a session-wide invalid version (pkgver) string."""
     return "-1.0.0"
 
 
-@fixture(scope="session")
-def absolute_dir() -> str:
-    return "/foo"
-
-
-@fixture(
-    scope="session",
-    params=[
-        "/",
-        "foo",
-        "",
-    ],
-)
-def invalid_absolute_dir(request: Any) -> str:
-    return str(request.param)
-
-
 @fixture(
     scope="session",
     params=[arch.value for arch in ArchitectureEnum],
 )
 def arch(request: Any) -> str:
+    """Return all available ArchitectureEnum members session-wide as string."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "foo",
@@ -267,45 +301,49 @@
         "foo123",
         "foo-123",
         "foo.123",
         "foo_",
     ],
 )
 def buildenv(request: Any) -> str:
+    """Return a set of valid buildenv strings session-wide."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "",
         "!",
         "! foo",
     ],
 )
 def invalid_buildenv(request: Any) -> str:
+    """Return a set of invalid buildenv strings session-wide."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[name.value for name in CompressionTypeEnum],
 )
 def compression_type(request: Any) -> str:
+    """Return all members of CompressionTypeEnum session-wide as string."""
     return str("." + request.param if request.param else request.param)
 
 
 @fixture(
     scope="session",
     params=[
         ".foo",
         "_foo",
     ],
 )
 def invalid_compression_type(request: Any) -> str:
+    """Return a set of invalid compression types session-wide as string."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "foobar@mcfooface.tld",
@@ -314,14 +352,15 @@
         "foo_bar@mc-fooface.tld",
         "foo_bar@mc.fooface.tld",
         "foo-bar@mc.fooface.tld",
         "foobar@mcfooface.tld-foo",
     ],
 )
 def email(request: Any) -> str:
+    """Return a set of valid email address strings session-wide."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "foo",
@@ -329,47 +368,52 @@
         "foobar@.tld",
         "foobar@mcfooface.",
         "foobar@mcfooface",
         "foobar@@mcfooface.tld",
     ],
 )
 def invalid_email(request: Any) -> str:
+    """Return a set of invalid email address strings session-wide."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "1:",
         "10:",
         "100:",
     ],
 )
 def epoch(request: Any) -> str:
+    """Return a set of valid epoch strings session-wide."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "0:",
         "1",
         ":1",
     ],
 )
 def invalid_epoch(request: Any) -> str:
+    """Return a set of invalid epoch strings session-wide."""
     return str(request.param)
 
 
 def create_md5sum() -> str:
-    return "".join(choice("abcdef" + digits) for x in range(32))
+    """Return a dummy MD5 string."""
+    return "".join(choice("abcdef" + digits) for x in range(32))  # nosec: B311
 
 
 @fixture(scope="session")
 def md5sum() -> str:
+    """Return a session-wide dummy MD5 string."""
     return create_md5sum()
 
 
 @fixture(
     scope="session",
     params=[
         "foo",
@@ -378,40 +422,43 @@
         "foo123",
         "foo-123",
         "foo.123",
         "foo_",
     ],
 )
 def option(request: Any) -> str:
+    """Return string session-wide from a set of valid option strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "",
         "!",
         "! foo",
     ],
 )
 def invalid_option(request: Any) -> str:
+    """Return string session-wide from a set of invalid option strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "foo",
         "_foo",
         "@foo",
         "+foo",
         "foo.+_-123",
     ],
 )
 def package_name(request: Any) -> str:
+    """Return string session-wide from a set of valid package name strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "foo!",
@@ -419,54 +466,59 @@
         ".foo",
         "-foo",
         "fo,o",
         "fo*o",
     ],
 )
 def invalid_package_name(request: Any) -> str:
+    """Return string session-wide from a set of invalid package name strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "1",
         "10",
         "1.1",
         "1.10",
         "10.10",
     ],
 )
 def pkgrel(request: Any) -> str:
+    """Return string session-wide from a set of valid pkgrel strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "0",
         "1.0",
         "0.1",
         "",
     ],
 )
 def invalid_pkgrel(request: Any) -> str:
+    """Return string session-wide from a set of invalid pkgrel strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[pkgtype.value for pkgtype in PkgTypeEnum],
 )
 def pkgtype(request: Any) -> str:
+    """Return string session-wide from the set of PkgTypeEnum values."""
     return str(request.param)
 
 
 @fixture(scope="session")
 def invalid_pkgtype() -> str:
+    """Return invalid pkgtype string session-wide."""
     return "foo"
 
 
 @fixture(
     scope="session",
     params=[
         "Foobar",
@@ -475,38 +527,54 @@
         "Foobar McFooface (The great Bar)",
         "Foobar McFooface (The great Bar..)",
         "Foobar McFooface (The 1st)",
         "foo",
     ],
 )
 def packager_name(request: Any) -> str:
+    """Return string session-wide from a set of valid packager name strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "",
         "Foobar!",
         "Foobar, McFooface",
     ],
 )
 def invalid_packager_name(request: Any) -> str:
+    """Return string session-wide from a set of invalid packager name strings."""
     return str(request.param)
 
 
 def create_sha256sum() -> str:
-    return "".join(choice("abcdef" + digits) for x in range(64))
+    """Return dummy SHA-256 sum string."""
+    return "".join(choice("abcdef" + digits) for x in range(64))  # nosec: B311
 
 
 @fixture(scope="session")
 def sha256sum() -> str:
+    """Return session-wide dummy SHA-256 sum string."""
     return create_sha256sum()
 
 
+@fixture(scope="session")
+def signature() -> str:
+    """Return session-wide signature file suffix string."""
+    return ".sig"
+
+
+@fixture(scope="session")
+def invalid_signature() -> str:
+    """Return session-wide invalid signature file suffix string."""
+    return ".foo"
+
+
 @fixture(
     scope="session",
     params=[
         "0.0.1",
         "0_0_1",
         "0+0+1",
         "0.1.0",
@@ -517,55 +585,66 @@
         "0",
         "1.",
         "1..",
         "foo",
     ],
 )
 def version(request: Any) -> str:
+    """Return string session-wide from a set of valid version strings."""
     return str(request.param)
 
 
 @fixture(
     scope="session",
     params=[
         "-1",
         "1 0",
         "1-0",
         "1/0",
     ],
 )
 def invalid_version(request: Any) -> str:
+    """Return string session-wide from a set of invalid version strings."""
     return str(request.param)
 
 
 @fixture(scope="function")
 def mtreeentryv1_stringio() -> Generator[StringIO, None, None]:
+    """Yield MTreeEntryV1 in a StringIO function-wide."""
     mtree_contents = """
         #mtree
         /set type=file uid=0 gid=0 mode=644
         ./.BUILDINFO time=1651787473.0 size=5651 md5digest=f712adf35b8a74755b3a93997b05793c \
         sha256digest=ed4e5855da200753eaf00cd584f017bef6910c09f70d72e4a642515312919804
         ./.INSTALL time=1651787473.0 size=808 md5digest=d96cc20315471e332a06c4261590b505 \
         sha256digest=96fc0c8b3aa4011de41c9dd1ba95e63bf2e9767daa801c14bea1d57359baf307
         ./.PKGINFO time=1651787473.0 size=1689 md5digest=76ff63a0094096fabe790fb35daadf79 \
         sha256digest=e15a57a4ddb0fa9feddbe410f395524b25be345d17f75f5f2ccc273034d388bc
         /set mode=755
         ./etc time=1651787473.0 type=dir
         ./etc/foo time=1651787473.0 type=dir
         ./etc/foo/foo.conf time=1651787473.0 mode=644 size=2761 md5digest=c6e1c562468738e93335f2e2ce314e8b \
         sha256digest=87d2b2075fbb24eb1108fed7ef9f2971d7954ae0894b1405425a04ff9e1df49e
-        ./etc/foo.conf.d time=1651787473.0 type=dir
-        ./usr time=1651787473.0 type=dir
-        ./usr/share time=1651787473.0 type=dir
-        ./usr/share/foo time=1651787473.0 type=dir
-        ./usr/share/foo/conf time=1651787473.0 type=dir
-        ./usr/share/foo/conf/override.conf time=1651787473.0 mode=777 type=link link=/etc/foo.conf.d/override.conf
+        ./etc/foo/bar.conf time=1651787473.0 mode=44 size=2761 md5digest=c6e1c562468738e93335f2e2ce314e8b \
+        sha256digest=87d2b2075fbb24eb1108fed7ef9f2971d7954ae0894b1405425a04ff9e1df49e
+        /set time=1651787473.0
+        ./etc/foo.conf.d type=dir
+        ./usr type=dir
+        ./usr/share type=dir
+        ./usr/share/foo type=dir
+        ./usr/share/foo/conf type=dir
+        ./usr/share/foo/conf/override.conf time=1651787476.0 mode=777 type=link link=/etc/foo.conf.d/override.conf
+        /set mode=66
+        ./usr/share/foo/conf/foo.conf size=2761 md5digest=c6e1c562468738e93335f2e2ce314e8b \
+        sha256digest=87d2b2075fbb24eb1108fed7ef9f2971d7954ae0894b1405425a04ff9e1df49e
+        ./usr/share/foo/conf/bar.conf size=2761 md5digest=c6e1c562468738e93335f2e2ce314e8b \
+        sha256digest=87d2b2075fbb24eb1108fed7ef9f2971d7954ae0894b1405425a04ff9e1df49e
         """
 
-    yield StringIO(initial_value=mtree_contents.strip())
+    yield StringIO(initial_value=dedent(mtree_contents).strip())
 
 
 @fixture(
     scope="function",
     params=[
         (
             """
@@ -657,37 +736,43 @@
         "invalid_size",
         "invalid_time",
         "invalid_type",
         "invalid_uid",
     ],
 )
 def invalid_mtreeentryv1_stringio(request: Any) -> Generator[StringIO, None, None]:
+    """Yield invalid MTreeEntryV1 in a StringIO function-wide from a set of invalid string inputs."""
     entry = dedent(request.param).strip()
     print(entry)
     yield StringIO(initial_value=entry)
 
 
 @fixture(scope="function")
-def mtreeentryv1_internals() -> Generator[List[MTreeEntryV1], None, None]:
+def mtreeentryv1_internals() -> Generator[list[MTreeEntryV1], None, None]:
+    """Yield list of MTreeEntryV1 representing the required internal package files."""
     base = {
         "gid": 0,
         "link": None,
-        "md5": "".join(choice("abcdef" + digits) for x in range(32)),
+        "md5": "".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
         "mode": "0644",
-        "sha256": "".join(choice("abcdef" + digits) for x in range(64)),
+        "sha256": "".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
         "time": 1000,
         "type_": "file",
         "uid": 0,
     }
 
-    yield [MTreeEntryV1(name=name, **base) for name in ["/.BUILDINFO", "/.INSTALL", "/.MTREE", "/.PKGINFO"]]
+    yield [
+        MTreeEntryV1(name=name, **base)  # type: ignore[arg-type]
+        for name in ["/.BUILDINFO", "/.INSTALL", "/.MTREE", "/.PKGINFO"]
+    ]
 
 
 @fixture(scope="function")
 def mtreeentryv1_dir(md5sum: str, sha256sum: str) -> Generator[MTreeEntryV1, None, None]:
+    """Yield an MTreeEntryV1 function-wide representing a directory."""
     yield MTreeEntryV1(
         gid=0,
         link=None,
         md5=md5sum,
         mode="0755",
         name="/foo/dir",
         sha256=sha256sum,
@@ -695,14 +780,15 @@
         type_="dir",
         uid=0,
     )
 
 
 @fixture(scope="function")
 def mtreeentryv1_file(md5sum: str, sha256sum: str) -> Generator[MTreeEntryV1, None, None]:
+    """Yield an MTreeEntryV1 function-wide representing a file."""
     yield MTreeEntryV1(
         gid=0,
         link=None,
         md5=md5sum,
         mode="0644",
         name="/foo/file",
         sha256=sha256sum,
@@ -710,14 +796,15 @@
         type_="file",
         uid=0,
     )
 
 
 @fixture(scope="function")
 def mtreeentryv1_link(md5sum: str, sha256sum: str) -> Generator[MTreeEntryV1, None, None]:
+    """Yield an MTreeEntryV1 function-wide representing a symlink."""
     yield MTreeEntryV1(
         gid=0,
         link="/foo/target",
         md5=md5sum,
         mode="0777",
         name="/foo/link",
         sha256=sha256sum,
@@ -728,50 +815,54 @@
 
 
 @fixture(scope="function")
 def valid_mtree(
     mtreeentryv1_dir: MTreeEntryV1,
     mtreeentryv1_file: MTreeEntryV1,
     mtreeentryv1_link: MTreeEntryV1,
-    mtreeentryv1_internals: List[MTreeEntryV1],
+    mtreeentryv1_internals: list[MTreeEntryV1],
 ) -> Generator[MTree, None, None]:
+    """Yield an MTree function-wide representing a set of files and directories."""
     yield MTree(
-        entries=[
+        entries=[  # type: ignore[arg-type]
             mtreeentryv1_dir,
             mtreeentryv1_file,
             mtreeentryv1_link,
         ]
         + mtreeentryv1_internals,
     )
 
 
 @fixture(scope="function")
 def valid_mtree_file(mtreeentryv1_stringio: StringIO, tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield the Path to an mtree file function-wide."""
     with NamedTemporaryFile(prefix="mtree_", dir=tmp_path, delete=False) as mtree_file:
         with gzip.open(filename=mtree_file.name, mode="wt") as gzip_mtree:
             gzip_mtree.write(mtreeentryv1_stringio.getvalue())
 
     yield Path(mtree_file.name)
 
 
 @fixture(scope="function")
 def valid_mtree_bytesio(valid_mtree_file: Path) -> Generator[IO[bytes], None, None]:
+    """Yield a bytes stream function-wide representing MTree data."""
     with open(valid_mtree_file, mode="rb") as gzip_mtree:
         yield BytesIO(gzip_mtree.read())
 
 
 @fixture(scope="function")
 def packagev1(
     default_filename: str,
     md5sum: str,
     sha256sum: str,
     valid_buildinfov1: BuildInfo,
     valid_mtree: MTree,
     valid_pkginfov1: PkgInfo,
 ) -> PackageV1:
+    """Return a PackageV1 using BuildInfoV1 and PkgInfoV1."""
     return PackageV1(
         buildinfo=valid_buildinfov1,
         csize=1,
         filename=default_filename,
         md5sum=md5sum,
         mtree=valid_mtree,
         pkginfo=valid_pkginfov1,
@@ -784,110 +875,114 @@
     default_filename: str,
     md5sum: str,
     sha256sum: str,
     valid_buildinfov1: BuildInfo,
     valid_mtree: MTree,
     valid_pkginfov2: PkgInfo,
 ) -> PackageV1:
+    """Return a PackageV1 using BuildInfoV1 and PkgInfoV2."""
     return PackageV1(
         buildinfo=valid_buildinfov1,
         csize=1,
         filename=default_filename,
         md5sum=md5sum,
         mtree=valid_mtree,
         pkginfo=valid_pkginfov2,
         sha256sum=sha256sum,
     )
 
 
 @fixture(scope="function")
-def temp_dir() -> Generator[Path, None, None]:
-    with TemporaryDirectory() as temp_dir:
-        yield Path(temp_dir)
-
-
-@fixture(scope="function")
-def text_file(temp_dir: Path) -> Generator[Path, None, None]:
-    with NamedTemporaryFile(prefix="pkg_content_", dir=temp_dir, suffix=".txt", delete=False) as temp_file:
+def text_file(tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield the Path to a dummy text file function-wide."""
+    with NamedTemporaryFile(prefix="pkg_content_", dir=tmp_path, suffix=".txt", delete=False) as temp_file:
         with open(temp_file.name, "w") as f:
             print("foo", file=f)
 
     yield Path(temp_file.name)
 
 
 @fixture(scope="function")
 def bz2_file(text_file: Path) -> Generator[Path, None, None]:
-    with TemporaryDirectory() as temp_dir:
-        with NamedTemporaryFile(dir=temp_dir, suffix=".bz2", delete=False) as tarfile:
+    """Yield the Path to a bzip2 compressed file containing a dummy text file function-wide."""
+    with TemporaryDirectory() as tmp_path:
+        with NamedTemporaryFile(dir=tmp_path, suffix=".bz2", delete=False) as tarfile:
             with tarfile_open(tarfile.name, mode="w:bz2") as compressed_tarfile:
                 compressed_tarfile.add(text_file.parent)
                 compressed_tarfile.add(text_file)
 
         yield Path(tarfile.name)
 
 
 @fixture(scope="function")
 def gz_file(text_file: Path) -> Generator[Path, None, None]:
-    with TemporaryDirectory() as temp_dir:
-        with NamedTemporaryFile(dir=temp_dir, suffix=".gz", delete=False) as tarfile:
+    """Yield the Path to a gzip compressed file containing a dummy text file function-wide."""
+    with TemporaryDirectory() as tmp_path:
+        with NamedTemporaryFile(dir=tmp_path, suffix=".gz", delete=False) as tarfile:
             with tarfile_open(tarfile.name, mode="w:gz") as compressed_tarfile:
                 compressed_tarfile.add(text_file.parent)
                 compressed_tarfile.add(text_file)
 
         yield Path(tarfile.name)
 
 
 @fixture(scope="function")
 def tar_file(text_file: Path) -> Generator[Path, None, None]:
-    with TemporaryDirectory() as temp_dir:
-        with NamedTemporaryFile(dir=temp_dir, suffix=".tar", delete=False) as tarfile:
+    """Yield the Path to a tar bundled file containing a dummy text file function-wide."""
+    with TemporaryDirectory() as tmp_path:
+        with NamedTemporaryFile(dir=tmp_path, suffix=".tar", delete=False) as tarfile:
             with tarfile_open(tarfile.name, mode="w:") as uncompressed_tarfile:
                 uncompressed_tarfile.add(text_file.parent)
                 uncompressed_tarfile.add(text_file)
 
         yield Path(tarfile.name)
 
 
 @fixture(scope="function")
 def xz_file(text_file: Path) -> Generator[Path, None, None]:
-    with TemporaryDirectory() as temp_dir:
-        with NamedTemporaryFile(dir=temp_dir, suffix=".xz", delete=False) as tarfile:
+    """Yield the Path to a xz compressed file containing a dummy text file function-wide."""
+    with TemporaryDirectory() as tmp_path:
+        with NamedTemporaryFile(dir=tmp_path, suffix=".xz", delete=False) as tarfile:
             with tarfile_open(tarfile.name, mode="w:xz") as compressed_tarfile:
                 compressed_tarfile.add(text_file.parent)
                 compressed_tarfile.add(text_file)
 
         yield Path(tarfile.name)
 
 
 @fixture(scope="function")
 def zst_file(text_file: Path) -> Generator[Path, None, None]:
-    with TemporaryDirectory() as temp_dir:
-        with NamedTemporaryFile(dir=temp_dir, suffix=".zst", delete=False) as tarfile:
+    """Yield the Path to a zstd compressed file containing a dummy text file function-wide."""
+    with TemporaryDirectory() as tmp_path:
+        with NamedTemporaryFile(dir=tmp_path, suffix=".zst", delete=False) as tarfile:
             with ZstdTarFile(tarfile.name, mode="w") as compressed_tarfile:
                 compressed_tarfile.add(text_file.parent)
                 compressed_tarfile.add(text_file)
 
         yield Path(tarfile.name)
 
 
 @fixture(scope="session")
 def epoch_version_pkgrel(epoch: str, version: str, pkgrel: str) -> str:
+    """Return a version string session-wide, representing all valid permutations of epoch, pkgver and pkgrel."""
     return f"{epoch}{version}-{pkgrel}"
 
 
 @fixture(scope="session")
 def invalid_epoch_version_pkgrel(invalid_epoch: str, invalid_version: str, invalid_pkgrel: str) -> str:
+    """Return a version string session-wide, representing all invalid permutations of epoch, pkgver and pkgrel."""
     return f"{invalid_epoch}{invalid_version}-{invalid_pkgrel}"
 
 
 @fixture(scope="function")
 def buildinfov1_stringio(
     default_packager: str,
     sha256sum: str,
 ) -> Generator[StringIO, None, None]:
+    """Yield a StringIO function-wide representing valid BuildInfoV1 data."""
     buildinfov1_contents = f"""format = 1
         pkgname = foo
         pkgbase = bar
         pkgver = 1:1.0.0-1
         pkgarch = any
         pkgbuild_sha256sum = {sha256sum}
         packager = {default_packager}
@@ -905,14 +1000,15 @@
 
 
 @fixture(scope="function")
 def buildinfov2_stringio(
     default_packager: str,
     sha256sum: str,
 ) -> Generator[StringIO, None, None]:
+    """Yield a StringIO function-wide representing valid BuildInfoV2 data."""
     buildinfov1_contents = f"""format = 2
         pkgname = foo
         pkgbase = bar
         pkgver = 1:1.0.0-1
         pkgarch = any
         pkgbuild_sha256sum = {sha256sum}
         packager = {default_packager}
@@ -930,81 +1026,93 @@
         """
 
     yield StringIO(initial_value=dedent(buildinfov1_contents).strip())
 
 
 @fixture(scope="function")
 def valid_buildinfov1_file(buildinfov1_stringio: StringIO) -> Generator[Path, None, None]:
+    """Yield the Path to a file function-wide representing valid BuildInfoV1 data."""
     with NamedTemporaryFile() as buildinfo_file:
         with open(buildinfo_file.name, mode="wt") as f:
             print(buildinfov1_stringio.getvalue(), file=f)
 
         yield Path(buildinfo_file.name)
 
 
 @fixture(scope="function")
 def valid_buildinfov2_file(buildinfov2_stringio: StringIO, tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield the Path to a file function-wide representing valid BuildInfoV2 data."""
     with NamedTemporaryFile(prefix="buildinfov2_", dir=tmp_path, delete=False) as buildinfo_file:
         with open(buildinfo_file.name, mode="wt") as f:
             print(buildinfov2_stringio.getvalue(), file=f)
 
     yield Path(buildinfo_file.name)
 
 
 @fixture(scope="session")
+def default_installed() -> list[str]:
+    """Return a list of strings session-wide, representing repod.files.buildinfo.Installed entries."""
+    return ["build_foo-1:1.0.1-1-any", "build_bar-1:1.0.1-1-any"]
+
+
+@fixture(scope="session")
 def valid_buildinfov1(
     default_arch: str,
     default_buildenv: str,
     default_full_version: str,
+    default_installed: list[str],
     default_option: str,
     default_packager: str,
     sha256sum: str,
     url: str,
 ) -> BuildInfo:
+    """Return a BuildInfoV1 session-wide."""
     return BuildInfoV1(
         builddate=1,
         builddir="/build",
         buildenv=[default_buildenv],
-        format_=1,
-        installed=["bar-1:1.0.1-1-any", "baz-1:1.0.1-1-any"],
+        installed=default_installed,
         options=[default_option],
         packager=default_packager,
         pkgarch=default_arch,
         pkgbase="foo",
         pkgbuild_sha256sum=sha256sum,
         pkgname="foo",
         pkgver=default_full_version,
+        schema_version=1,
     )
 
 
 @fixture(scope="session")
 def valid_buildinfov2(
     default_arch: str,
     default_buildenv: str,
     default_full_version: str,
+    default_installed: list[str],
     default_option: str,
     default_packager: str,
     sha256sum: str,
     url: str,
 ) -> BuildInfo:
+    """Return a BuildInfoV2 session-wide."""
     return BuildInfoV2(
         builddate=1,
         builddir="/build",
         buildenv=[default_buildenv],
         buildtool="buildtool",
         buildtoolver=default_full_version,
-        format_=2,
-        installed=["bar-1:1.0.1-1-any", "baz-1:1.0.1-1-any"],
+        installed=default_installed,
         options=[default_option],
         packager=default_packager,
         pkgarch=default_arch,
         pkgbase="foo",
         pkgbuild_sha256sum=sha256sum,
         pkgname="foo",
         pkgver=default_full_version,
+        schema_version=2,
         startdir="/startdir",
     )
 
 
 @fixture(scope="function")
 def pkginfov1_stringio(
     default_arch: str,
@@ -1012,14 +1120,15 @@
     default_full_version: str,
     default_license: str,
     default_package_name: str,
     default_packager: str,
     default_version: str,
     url: str,
 ) -> Generator[StringIO, None, None]:
+    """Yield a StringIO function-wide representing PkgInfoV1 data."""
     file_data = f"""# Generated by makepkg {default_version}
         # using fakeroot version {default_version}
         pkgname = {default_package_name}
         pkgbase = {default_package_name}
         pkgver = {default_full_version}
         pkgdesc = {default_description}
         url = {url}
@@ -1044,14 +1153,15 @@
     default_license: str,
     default_package_name: str,
     default_packager: str,
     default_pkgtype: str,
     default_version: str,
     url: str,
 ) -> Generator[StringIO, None, None]:
+    """Yield a StringIO function-wide representing PkgInfoV2 data."""
     file_data = f"""# Generated by makepkg {default_version}
         # using fakeroot version {default_version}
         pkgname = {default_package_name}
         pkgbase = {default_package_name}
         xdata = pkgtype={default_pkgtype}
         xdata = url=bar
         pkgver = {default_full_version}
@@ -1077,14 +1187,15 @@
     default_full_version: str,
     default_license: str,
     default_package_name: str,
     default_packager: str,
     default_version: str,
     url: str,
 ) -> Generator[StringIO, None, None]:
+    """Yield a StringIO function-wide representing PkgInfoV2 data of a debug package."""
     file_data = f"""# Generated by makepkg {default_version}
         # using fakeroot version {default_version}
         pkgname = {default_package_name}-debug
         pkgbase = {default_package_name}
         xdata = pkgtype=debug
         xdata = url=bar
         pkgver = {default_full_version}
@@ -1100,32 +1211,35 @@
         """
 
     yield StringIO(initial_value="\n".join([line.strip() for line in dedent(file_data).split("\n") if line]))
 
 
 @fixture(scope="function")
 def valid_pkginfov1_file(pkginfov1_stringio: StringIO) -> Generator[Path, None, None]:
+    """Yield a Path function-wide representing a PkgInfoV1 file."""
     with NamedTemporaryFile() as file:
         with open(file.name, mode="wt") as f:
             print(pkginfov1_stringio.getvalue(), file=f)
 
         yield Path(file.name)
 
 
 @fixture(scope="function")
 def valid_pkginfov2_file(pkginfov2_stringio: StringIO, tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield a Path function-wide representing a PkgInfoV2 file."""
     with NamedTemporaryFile(prefix="pkginfov2_", dir=tmp_path, delete=False) as file:
         with open(file.name, mode="wt") as f:
             print(pkginfov2_stringio.getvalue(), file=f)
 
     yield Path(file.name)
 
 
 @fixture(scope="function")
 def debug_pkginfov2_file(debug_pkginfov2_stringio: StringIO, tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield a Path function-wide representing a PkgInfoV2 file of a debug package."""
     with NamedTemporaryFile(prefix="pkginfov2_debug_", dir=tmp_path, delete=False) as file:
         with open(file.name, mode="wt") as f:
             print(debug_pkginfov2_stringio.getvalue(), file=f)
 
     yield Path(file.name)
 
 
@@ -1135,14 +1249,15 @@
     default_description: str,
     default_full_version: str,
     default_license: str,
     default_packager: str,
     default_version: str,
     url: str,
 ) -> PkgInfo:
+    """Return a PkgInfoV1 session-wide."""
     return PkgInfoV1(
         arch=default_arch,
         backup=None,
         base="foo",
         builddate=1,
         checkdepends=None,
         conflicts=None,
@@ -1155,15 +1270,15 @@
         license=[default_license],
         makedepends=None,
         makepkg_version=default_version,
         name="foo",
         optdepends=None,
         provides=None,
         replaces=None,
-        url=url,
+        url=url,  # type: ignore[arg-type]
         version=default_full_version,
     )
 
 
 @fixture(scope="session")
 def valid_pkginfov2(
     default_arch: str,
@@ -1171,14 +1286,15 @@
     default_full_version: str,
     default_license: str,
     default_packager: str,
     default_pkgtype: str,
     default_version: str,
     url: str,
 ) -> PkgInfo:
+    """Return a PkgInfoV2 session-wide."""
     return PkgInfoV2(
         arch=default_arch,
         backup=None,
         base="foo",
         builddate=1,
         checkdepends=None,
         conflicts=None,
@@ -1191,50 +1307,52 @@
         license=[default_license],
         makedepends=None,
         makepkg_version=default_version,
         name="foo",
         optdepends=None,
         provides=None,
         replaces=None,
-        url=url,
+        url=url,  # type: ignore[arg-type]
         version=default_full_version,
-        xdata=[PkgType(pkgtype=default_pkgtype)],
+        xdata=[PkgType(pkgtype=default_pkgtype)],  # type: ignore[arg-type]
     )
 
 
 @fixture(scope="function")
 def filesv1() -> FilesV1:
+    """Return a FilesV1 function-wide."""
     return FilesV1(files=["foo", "bar"])
 
 
 @fixture(scope="function")
 def outputpackagev1(
     base64_pgpsig: str,
     default_description: str,
     default_filename: str,
     default_license: str,
     filesv1: FilesV1,
     md5sum: str,
     sha256sum: str,
     url: str,
 ) -> OutputPackageV1:
+    """Return an OutputPackageV1 function-wide."""
     return OutputPackageV1(
         arch="any",
         builddate=1,
         csize=1,
         desc=default_description,
         filename=default_filename,
         files=filesv1,
         isize=1,
         license=[default_license],
         md5sum=md5sum,
         name="foo",
         pgpsig=base64_pgpsig,
         sha256sum=sha256sum,
-        url=url,
+        url=url,  # type: ignore[arg-type]
     )
 
 
 @fixture(scope="function")
 def outputpackagebasev1(
     base64_pgpsig: str,
     default_description: str,
@@ -1245,14 +1363,15 @@
     filesv1: FilesV1,
     md5sum: str,
     outputpackagev1: OutputPackageV1,
     sha256sum: str,
     url: str,
     valid_buildinfov1: BuildInfo,
 ) -> OutputPackageBaseV1:
+    """Return an OutputPackageBaseV1 function-wide."""
     outputpackage2 = deepcopy(outputpackagev1)
     outputpackage2.filename = outputpackage2.filename.replace("foo", "bar")
     outputpackage2.name = "bar"
     outputpackage2.files = FilesV1(files=["bar"])
 
     return OutputPackageBaseV1(
         base="foo",
@@ -1274,29 +1393,30 @@
     default_full_version: str,
     default_license: str,
     default_packager: str,
     md5sum: str,
     sha256sum: str,
     url: str,
 ) -> PackageDescV1:
+    """Return a PackageDescV1 function-wide."""
     return PackageDescV1(
         arch="any",
         base="foo",
         builddate=1,
         csize=1,
         desc=default_description,
         filename=default_filename,
         isize=1,
         license=[default_license],
         md5sum=md5sum,
         name="foo",
         packager=default_packager,
         pgpsig=base64_pgpsig,
         sha256sum=sha256sum,
-        url=url,
+        url=url,  # type: ignore[arg-type]
         version=default_full_version,
     )
 
 
 @fixture(scope="function")
 def packagedescv2(
     default_description: str,
@@ -1304,28 +1424,29 @@
     default_full_version: str,
     default_license: str,
     default_packager: str,
     md5sum: str,
     sha256sum: str,
     url: str,
 ) -> PackageDescV2:
+    """Return a PackageDescV2 function-wide."""
     return PackageDescV2(
         arch="any",
         base="foo",
         builddate=1,
         csize=1,
         desc=default_description,
         filename=default_filename,
         isize=1,
         license=[default_license],
         md5sum=md5sum,
         name="foo",
         packager=default_packager,
         sha256sum=sha256sum,
-        url=url,
+        url=url,  # type: ignore[arg-type]
         version=default_full_version,
     )
 
 
 @pytest_asyncio.fixture(
     scope="function",
     params=[
@@ -1343,15 +1464,16 @@
 )
 async def default_sync_db_file(
     md5sum: str,
     outputpackagebasev1: OutputPackageBaseV1,
     request: Any,
     sha256sum: str,
     tmp_path: Path,
-) -> AsyncGenerator[Tuple[Path, Path], None]:
+) -> AsyncGenerator[tuple[Path, Path], None]:
+    """Yield a tuple of two Paths function-wide, representing a default repo sync db and its symlink."""
     compression = request.param
     suffix = ""
     match compression:
         case CompressionTypeEnum.BZIP2:
             suffix = ".bz2"
         case CompressionTypeEnum.GZIP:
             suffix = ".gz"
@@ -1396,15 +1518,16 @@
     ],
 )
 async def files_sync_db_file(
     md5sum: str,
     outputpackagebasev1: OutputPackageBaseV1,
     request: Any,
     sha256sum: str,
-) -> AsyncGenerator[Tuple[Path, Path], None]:
+) -> AsyncGenerator[tuple[Path, Path], None]:
+    """Yield a tuple of two Paths function-wide, representing a files repo sync db and its symlink."""
     compression = request.param
     suffix = ""
     match compression:
         case CompressionTypeEnum.BZIP2:
             suffix = ".bz2"
         case CompressionTypeEnum.GZIP:
             suffix = ".gz"
@@ -1412,16 +1535,16 @@
             suffix = ".xz"
         case CompressionTypeEnum.ZSTANDARD:
             suffix = ".zst"
 
     tar_db_name = Path(f"test.files.tar{suffix}")
     symlink_db_name = Path("test.files")
 
-    with TemporaryDirectory() as temp_dir:
-        temp_path = Path(temp_dir)
+    with TemporaryDirectory() as tmp_path:
+        temp_path = Path(tmp_path)
         sync_db_tarfile = temp_path / tar_db_name
         sync_db_symlink = temp_path / symlink_db_name
         sync_db = SyncDatabase(
             database=sync_db_tarfile,
             database_type=RepoDbTypeEnum.FILES,
             compression_type=compression,
             desc_version=PackageDescVersionEnum.DEFAULT,
@@ -1445,15 +1568,16 @@
     default_full_version: str,
     text_file: Path,
     tmp_path: Path,
     valid_mtree_file: Path,
     valid_buildinfov2_file: Path,
     debug_pkginfov2_file: Path,
     request: Any,
-) -> Tuple[Path, ...]:
+) -> tuple[Path, ...]:
+    """Return a tuple of two Paths function-wide, representing a debug package file and its dummy signature."""
     compression = request.param
     suffix = "." + str(request.param.value) if request.param.value else ""
     pkg_name = Path(f"{default_package_name}-debug-{default_full_version}-{default_arch}.pkg.tar{suffix}")
     sig_name = Path(f"{default_package_name}-debug-{default_full_version}-{default_arch}.pkg.tar{suffix}.sig")
     pkg_path = tmp_path / pkg_name
     sig_path = tmp_path / sig_name
     text_file_symlink = text_file.parent / "debug_symlink_to_text_file"
@@ -1466,15 +1590,15 @@
         tarfile.add(text_file, "text_file")
         tarfile.add(text_file_symlink, "text_file_symlink")
         tarfile.add(tmp_path, "empty_dir", recursive=False)
 
     with open(sig_path, "wb") as sig_file:
         sig_file.write(b"THIS IS NOT A VALID SIGNATURE")
 
-    return tuple([pkg_path, sig_path])
+    return (pkg_path, sig_path)
 
 
 @fixture(
     scope="function",
     params=[name for name in CompressionTypeEnum],
     ids=[name.value for name in CompressionTypeEnum],
 )
@@ -1484,15 +1608,16 @@
     default_full_version: str,
     text_file: Path,
     tmp_path: Path,
     valid_mtree_file: Path,
     valid_buildinfov2_file: Path,
     valid_pkginfov2_file: Path,
     request: Any,
-) -> Tuple[Path, ...]:
+) -> tuple[Path, ...]:
+    """Return a tuple of two Paths function-wide, representing a default package file and its dummy signature."""
     compression = request.param
     suffix = "." + str(request.param.value) if request.param.value else ""
     pkg_name = Path(f"{default_package_name}-{default_full_version}-{default_arch}.pkg.tar{suffix}")
     sig_name = Path(f"{default_package_name}-{default_full_version}-{default_arch}.pkg.tar{suffix}.sig")
     pkg_path = tmp_path / pkg_name
     sig_path = tmp_path / sig_name
     text_file_symlink = text_file.parent / "symlink_to_text_file"
@@ -1505,184 +1630,306 @@
         tarfile.add(text_file, "text_file")
         tarfile.add(text_file_symlink, "text_file_symlink")
         tarfile.add(tmp_path, "empty_dir", recursive=False)
 
     with open(sig_path, "wb") as sig_file:
         sig_file.write(b"THIS IS NOT A VALID SIGNATURE")
 
-    return tuple([pkg_path, sig_path])
+    return (pkg_path, sig_path)
 
 
 @fixture(scope="function")
 def outputpackagebasev1_json_files_in_dir(
-    base64_pgpsig: str,
-    default_description: str,
-    default_filename: str,
-    default_license: str,
-    default_packager: str,
-    default_full_version: str,
-    filesv1: Files,
-    md5sum: str,
-    sha256sum: str,
     tmp_path: Path,
-    url: str,
+    outputpackagebasev1: OutputPackageBase,
 ) -> Path:
-    for name, files in [
-        ("foo", filesv1),
-        ("bar", filesv1),
-        ("baz", None),
-    ]:
-        model = OutputPackageBaseV1(
-            base=name,
-            packager=default_packager,
-            version=default_full_version,
-            packages=[
-                OutputPackageV1(
-                    arch="any",
-                    builddate=1,
-                    csize=0,
-                    desc=default_description.replace("foo", name),
-                    filename=default_filename,
-                    files=files,
-                    isize=1,
-                    license=[default_license],
-                    md5sum=md5sum,
-                    name=name,
-                    pgpsig=base64_pgpsig,
-                    sha256sum=sha256sum,
-                    url=url,
-                )
-            ],
-        )
+    """Return a dir Path function-wide, representing a management repository layout with JSON files."""
+    outputpackagebasev1.packages[0].files = None  # type: ignore[attr-defined]
 
-        with open(tmp_path / f"{name}.json", "wb") as output_file:
-            output_file.write(
-                orjson.dumps(
-                    model.dict(), option=orjson.OPT_INDENT_2 | orjson.OPT_APPEND_NEWLINE | orjson.OPT_SORT_KEYS
-                )
+    management_dir = tmp_path / "management"
+    pkgnames_dir = management_dir / "pkgnames"
+    pkgnames_dir.mkdir(parents=True)
+
+    pkgbase_file = management_dir / f"{outputpackagebasev1.base}.json"  # type: ignore[attr-defined]
+    with open(pkgbase_file, "wb") as output_file:
+        output_file.write(
+            orjson.dumps(
+                outputpackagebasev1.model_dump(mode="json"),
+                option=orjson.OPT_INDENT_2 | orjson.OPT_APPEND_NEWLINE | orjson.OPT_SORT_KEYS,
             )
+        )
 
-    return tmp_path
+    for package in outputpackagebasev1.packages:  # type: ignore[attr-defined]
+        symlink_path = pkgnames_dir / f"{package.name}.json"
+        symlink_path.symlink_to(relative_to_shared_base(path_b=symlink_path, path_a=pkgbase_file))
+
+    return management_dir
 
 
 @fixture(scope="function")
 def empty_dir(tmp_path: Path) -> Path:
+    """Return a Path function-wide, representing an empty directory."""
     directory = tmp_path / "empty"
     directory.mkdir()
     return directory
 
 
 @fixture(scope="function")
 def empty_file(tmp_path: Path) -> Path:
+    """Return a Path function-wide, representing an empty file."""
     file = NamedTemporaryFile(prefix="empty_", dir=tmp_path, delete=False)
     return Path(file.name)
 
 
 @fixture(scope="function")
-def empty_syncdbs(tmp_path: Path) -> List[Path]:
+def empty_syncdbs(tmp_path: Path) -> list[Path]:
+    """Return a list of Paths function-wide, representing empty default and files repo sync databases."""
     directory = tmp_path / "pacman/sync"
-    files: List[Path] = [directory / "tmp.db", directory / "tmp.files"]
+    files: list[Path] = [directory / "tmp.db", directory / "tmp.files"]
 
     directory.mkdir(parents=True)
     for file in files:
         file.touch()
 
     return files
 
 
 @fixture(scope="function")
 def broken_json_file(tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield a Path function-wide, representing a broken JSON file."""
     with NamedTemporaryFile(prefix="broken_", suffix=".json", dir=tmp_path, delete=False) as json_file:
         json_file.write(b"garbage")
         path = Path(json_file.name)
     yield path
 
 
 @fixture(scope="function")
 def invalid_json_file(tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield a Path function-wide, representing an invalid JSON file."""
     with NamedTemporaryFile(prefix="invalid_", suffix=".json", dir=tmp_path, delete=False) as json_file:
         json_file.write(b'{"foo": "bar"}')
         path = Path(json_file.name)
     yield path
 
 
 @fixture(scope="function")
 def empty_toml_file(tmp_path: Path) -> Path:
+    """Yield a Path function-wide, representing an empty TOML file (with .conf suffix)."""
     return Path(NamedTemporaryFile(suffix=".conf", dir=tmp_path, delete=False).name)
 
 
 @fixture(scope="function")
 def empty_toml_files_in_dir(tmp_path: Path) -> Path:
+    """Yield a Path function-wide, representing a directory containing empty TOML files (with .conf suffix)."""
     for i in range(5):
         NamedTemporaryFile(suffix=".conf", dir=tmp_path, delete=False)
     return tmp_path
 
 
-def params_for_vercmp() -> Any:
+def params_for_vercmp() -> list[bool]:
+    """Create params for pyalpm_vercmp_fun."""
     if "linux" not in sys.platform:
         return [False]
     else:
         return [True, False]
 
 
 @fixture(scope="session", params=params_for_vercmp())
-def pyalpm_vercmp_fun(request: Any) -> Any:
-    return request.param
+def pyalpm_vercmp_fun(request: Any) -> bool:
+    """Return a boolean value based on params_for_vercmp."""
+    return bool(request.param)
 
 
 @fixture(scope="function")
-def packagerepo_in_tmp_path(tmp_path: Path) -> PackageRepo:
+def packagerepo_in_tmp_path(tmp_path: Path, caplog: LogCaptureFixture) -> PackageRepo:
+    """Return a PackageRepo function-wide."""
+    caplog.set_level(DEBUG)
+
     management_repo_base = tmp_path / "management_repo_base"
     source_repo_base = tmp_path / "source_repo_base"
     source_pool_base = tmp_path / "source_pool_base"
     package_repo_base = tmp_path / "package_repo_base"
     package_pool_base = tmp_path / "package_pool_base"
 
     package_repo = PackageRepo(
-        name=DEFAULT_NAME,
+        name=DEFAULT_NAME,  # type: ignore[arg-type]
         architecture=DEFAULT_ARCHITECTURE,
+        archiving=None,
         database_compression=DEFAULT_DATABASE_COMPRESSION,
         management_repo=ManagementRepo(directory=(management_repo_base / DEFAULT_NAME)),
         package_pool=(package_pool_base / DEFAULT_NAME),
         source_pool=(source_pool_base / DEFAULT_NAME),
         debug=Path(f"{DEFAULT_NAME}-debug"),
         staging=Path(f"{DEFAULT_NAME}-staging"),
+        staging_debug=Path(f"{DEFAULT_NAME}-staging-debug"),
         testing=Path(f"{DEFAULT_NAME}-testing"),
+        testing_debug=Path(f"{DEFAULT_NAME}-testing-debug"),
+    )
+
+    package_repo._stable_management_repo_dir = management_repo_base / f"{DEFAULT_ARCHITECTURE.value}/{DEFAULT_NAME}"
+    package_repo._stable_repo_dir = package_repo_base / f"{DEFAULT_NAME}/{DEFAULT_ARCHITECTURE.value}"
+    package_repo._stable_source_repo_dir = source_repo_base / f"{DEFAULT_NAME}/{DEFAULT_ARCHITECTURE.value}"
+
+    package_repo._debug_management_repo_dir = (
+        management_repo_base / f"{DEFAULT_ARCHITECTURE.value}/{DEFAULT_NAME}-debug"
+    )
+    package_repo._debug_repo_dir = package_repo_base / Path(f"{DEFAULT_NAME}-debug/{DEFAULT_ARCHITECTURE.value}")
+    package_repo._debug_source_repo_dir = source_repo_base / Path(f"{DEFAULT_NAME}-debug/{DEFAULT_ARCHITECTURE.value}")
+
+    package_repo._staging_management_repo_dir = (
+        management_repo_base / f"{DEFAULT_ARCHITECTURE.value}/{DEFAULT_NAME}-staging"
+    )
+    package_repo._staging_repo_dir = package_repo_base / Path(f"{DEFAULT_NAME}-staging/{DEFAULT_ARCHITECTURE.value}")
+    package_repo._staging_source_repo_dir = source_repo_base / Path(
+        f"{DEFAULT_NAME}-staging/{DEFAULT_ARCHITECTURE.value}"
+    )
+
+    package_repo._staging_debug_management_repo_dir = (
+        management_repo_base / f"{DEFAULT_ARCHITECTURE.value}/{DEFAULT_NAME}-staging-debug"
+    )
+    package_repo._staging_debug_repo_dir = package_repo_base / Path(
+        f"{DEFAULT_NAME}-staging-debug/{DEFAULT_ARCHITECTURE.value}"
+    )
+    package_repo._staging_debug_source_repo_dir = source_repo_base / Path(
+        f"{DEFAULT_NAME}-staging-debug/{DEFAULT_ARCHITECTURE.value}"
+    )
+
+    package_repo._testing_management_repo_dir = (
+        management_repo_base / f"{DEFAULT_ARCHITECTURE.value}/{DEFAULT_NAME}-testing"
+    )
+    package_repo._testing_repo_dir = package_repo_base / Path(f"{DEFAULT_NAME}-testing/{DEFAULT_ARCHITECTURE.value}")
+    package_repo._testing_source_repo_dir = source_repo_base / Path(
+        f"{DEFAULT_NAME}-testing/{DEFAULT_ARCHITECTURE.value}"
     )
 
-    package_repo._stable_management_repo_dir = management_repo_base / f"{DEFAULT_ARCHITECTURE}/{DEFAULT_NAME}"
-    package_repo._stable_repo_dir = package_repo_base / f"{DEFAULT_NAME}/{DEFAULT_ARCHITECTURE}"
-    package_repo._stable_source_repo_dir = source_repo_base / f"{DEFAULT_NAME}/{DEFAULT_ARCHITECTURE}"
-
-    package_repo._debug_management_repo_dir = management_repo_base / f"{DEFAULT_ARCHITECTURE}/{DEFAULT_NAME}-debug"
-    package_repo._debug_repo_dir = package_repo_base / Path(f"{DEFAULT_NAME}-debug/{DEFAULT_ARCHITECTURE}")
-    package_repo._debug_source_repo_dir = source_repo_base / Path(f"{DEFAULT_NAME}-debug/{DEFAULT_ARCHITECTURE}")
-
-    package_repo._staging_management_repo_dir = management_repo_base / f"{DEFAULT_ARCHITECTURE}/{DEFAULT_NAME}-staging"
-    package_repo._staging_repo_dir = package_repo_base / Path(f"{DEFAULT_NAME}-staging/{DEFAULT_ARCHITECTURE}")
-    package_repo._staging_source_repo_dir = source_repo_base / Path(f"{DEFAULT_NAME}-staging/{DEFAULT_ARCHITECTURE}")
-
-    package_repo._testing_management_repo_dir = management_repo_base / f"{DEFAULT_ARCHITECTURE}/{DEFAULT_NAME}-testing"
-    package_repo._testing_repo_dir = package_repo_base / Path(f"{DEFAULT_NAME}-testing/{DEFAULT_ARCHITECTURE}")
-    package_repo._testing_source_repo_dir = source_repo_base / Path(f"{DEFAULT_NAME}-testing/{DEFAULT_ARCHITECTURE}")
+    package_repo._testing_debug_management_repo_dir = (
+        management_repo_base / f"{DEFAULT_ARCHITECTURE.value}/{DEFAULT_NAME}-testing-debug"
+    )
+    package_repo._testing_debug_repo_dir = package_repo_base / Path(
+        f"{DEFAULT_NAME}-testing-debug/{DEFAULT_ARCHITECTURE.value}"
+    )
+    package_repo._testing_debug_source_repo_dir = source_repo_base / Path(
+        f"{DEFAULT_NAME}-testing-debug/{DEFAULT_ARCHITECTURE.value}"
+    )
 
     package_repo._package_pool_dir = package_pool_base / DEFAULT_NAME
     package_repo._source_pool_dir = source_pool_base / DEFAULT_NAME
 
+    debug("Creating package repo fixture")
+    debug(package_repo)
     return package_repo
 
 
 @fixture(scope="function")
-def usersettings(packagerepo_in_tmp_path: PackageRepo, empty_file: Path, tmp_path: Path) -> UserSettings:
+@patch("repod.config.settings.get_default_archive_settings")
+def usersettings(
+    get_default_archive_settings_mock: Mock,
+    packagerepo_in_tmp_path: PackageRepo,
+    empty_file: Path,
+    tmp_path: Path,
+    caplog: LogCaptureFixture,
+) -> UserSettings:
+    """Return a UserSettings function-wide."""
+    caplog.set_level(DEBUG)
     tmp_dir_path = tmp_path / "usersettings"
+
+    get_default_archive_settings_mock.return_value = ArchiveSettings(
+        packages=tmp_dir_path / "archive/package",
+        sources=tmp_dir_path / "archive/sources",
+    )
     with patch("repod.config.settings.CUSTOM_CONFIG", empty_file):
         with patch("repod.config.settings.UserSettings._management_repo_base", tmp_dir_path / "management"):
             with patch("repod.config.settings.UserSettings._package_pool_base", tmp_dir_path / "data/pool/package"):
                 with patch("repod.config.settings.UserSettings._package_repo_base", tmp_dir_path / "data/repo/package"):
                     with patch(
                         "repod.config.settings.UserSettings._source_pool_base", tmp_dir_path / "data/pool/source"
                     ):
                         with patch(
                             "repod.config.settings.UserSettings._source_repo_base",
                             tmp_dir_path / "data/repo/source",
                         ):
-                            return UserSettings(repositories=[packagerepo_in_tmp_path])
+                            return UserSettings(
+                                repositories=[packagerepo_in_tmp_path],
+                            )
+
+
+@fixture(scope="function")
+def srcinfov1_single_stringio(
+    default_arch: str,
+    url: str,
+    default_license: str,
+    default_package_name: str,
+    default_version: str,
+    default_packager: str,
+    sha256sum: str,
+) -> Generator[StringIO, None, None]:
+    """Yield a StringIO function-wide, representing SrcInfoV1 data of a single package."""
+    buildinfov1_contents = f"""
+        # foo
+        pkgbase = {default_package_name}
+        \tpkgdesc = description
+        \tepoch = 1
+        \tpkgver = {default_version}
+        \tpkgrel = 1
+        \turl = {url}
+        \tarch = {default_arch}
+        \tlicense = {default_license}
+        \toptions = debug
+        \toptions = strip
+
+        pkgname = {default_package_name}
+        """
+
+    yield StringIO(initial_value=dedent(buildinfov1_contents).strip())
+
+
+@fixture(scope="function")
+def srcinfov1_split_stringio(
+    default_arch: str,
+    url: str,
+    default_license: str,
+    default_package_name: str,
+    default_version: str,
+    default_packager: str,
+    sha256sum: str,
+) -> Generator[StringIO, None, None]:
+    """Yield a StringIO function-wide, representing SrcInfoV1 data of a split package."""
+    buildinfov1_contents = f"""
+        # foo
+        pkgbase = {default_package_name}
+        \tpkgdesc = description
+        \tpkgver = {default_version}
+        \tpkgrel = 1
+        \turl = {url}
+        \tarch = {default_arch}
+        \tlicense = {default_license}
+        \toptions = debug
+        \toptions = strip
+
+        pkgname = {default_package_name}
+        \tpkgdesc = other description
+
+        pkgname = {default_package_name}-b
+        \tpkgdesc = other description
+        """
+
+    yield StringIO(initial_value=dedent(buildinfov1_contents).strip())
+
+
+@fixture(scope="function")
+def srcinfov1_single_file(srcinfov1_single_stringio: StringIO) -> Generator[Path, None, None]:
+    """Yield a Path function-wide, representing a SrcInfoV1 file of a single package."""
+    with NamedTemporaryFile(prefix="srcinfov1_single_") as buildinfo_file:
+        with open(buildinfo_file.name, mode="wt") as f:
+            print(srcinfov1_single_stringio.getvalue(), file=f)
+
+        yield Path(buildinfo_file.name)
+
+
+@fixture(scope="function")
+def srcinfov1_split_file(srcinfov1_split_stringio: StringIO, tmp_path: Path) -> Generator[Path, None, None]:
+    """Yield a Path function-wide, representing a SrcInfoV1 file of a split package."""
+    with NamedTemporaryFile(prefix="srcinfov1_split_", dir=tmp_path, delete=False) as buildinfo_file:
+        with open(buildinfo_file.name, mode="wt") as f:
+            print(srcinfov1_split_stringio.getvalue(), file=f)
+
+    yield Path(buildinfo_file.name)
```

### Comparing `repod-0.2.2/tests/files/test_buildinfo.py` & `repod-0.3.0.post0/tests/files/test_buildinfo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,178 +1,221 @@
+"""Tests for repod.files.buildinfo."""
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
 from tempfile import TemporaryDirectory
 from typing import ContextManager
 
 from pydantic import ValidationError
 from pytest import mark, raises
 
-from repod.common.enums import tar_compression_types_for_filename_regex
+from repod.common.enums import (
+    ArchitectureEnum,
+    tar_compression_types_for_filename_regex,
+)
 from repod.errors import RepoManagementError
 from repod.files import buildinfo
 from repod.files.common import extract_file_from_tarfile, open_tarfile
+from tests.conftest import (
+    create_default_arch,
+    create_default_full_version,
+    create_default_invalid_full_version,
+    create_default_invalid_package_name,
+    create_default_package_name,
+)
 
 
 @mark.parametrize(
     "number, expectation",
     [
         (0, does_not_raise()),
         (1, does_not_raise()),
         (-1, raises(ValidationError)),
     ],
 )
 def test_builddate(number: int, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.buildinfo.BuildDate."""
     with expectation:
         buildinfo.BuildDate(builddate=number)
 
 
-def test_builddir(absolute_dir: str, invalid_absolute_dir: str) -> None:
-    with does_not_raise():
-        buildinfo.BuildDir(builddir=absolute_dir)
-    with raises(ValidationError):
-        buildinfo.BuildDir(builddir=invalid_absolute_dir)
+@mark.parametrize(
+    "path, expectation",
+    [
+        ("/", does_not_raise()),
+        ("/foo", does_not_raise()),
+        ("foo", raises(ValidationError)),
+        ("", raises(ValidationError)),
+    ],
+)
+def test_builddir(
+    path: str,
+    expectation: ContextManager[str],
+) -> None:
+    """Tests for repod.files.buildinfo.BuildDir."""
+    with expectation:
+        buildinfo.BuildDir(builddir=path)
 
 
 def test_buildenv(default_buildenv: str, default_invalid_buildenv: str) -> None:
+    """Tests for repod.files.buildinfo.BuildEnv."""
     with does_not_raise():
         buildinfo.BuildEnv(buildenv=[default_buildenv])
     with raises(ValidationError):
         buildinfo.BuildEnv(buildenv=[default_invalid_buildenv])
 
 
 def test_buildtool(default_package_name: str, default_invalid_package_name: str) -> None:
+    """Tests for repod.files.buildinfo.BuildTool."""
     with does_not_raise():
         buildinfo.BuildTool(buildtool=default_package_name)
     with raises(ValidationError):
         buildinfo.BuildTool(buildtool=default_invalid_package_name)
 
 
 def test_buildtoolver() -> None:
-    assert buildinfo.BuildToolVer(buildtoolver="foo")
-
-
-@mark.parametrize(
-    "format_, expectation",
-    [
-        (1, does_not_raise()),
-        (0, raises(ValidationError)),
-        (2, raises(ValidationError)),
-    ],
-)
-def test_formatv1(format_: int, expectation: ContextManager[str]) -> None:
-    with expectation:
-        buildinfo.FormatV1(format_=format_)
+    """Tests for repod.files.buildinfo.BuildToolVer."""
+    assert buildinfo.BuildToolVer(buildtoolver="foo")  # nosec: B101
 
 
 @mark.parametrize(
-    "format_, expectation",
+    "installed, expectation",
     [
-        (2, does_not_raise()),
-        (1, raises(ValidationError)),
-        (3, raises(ValidationError)),
+        (
+            [f"{create_default_package_name()}-{create_default_full_version()}-{create_default_arch()}"],
+            does_not_raise(),
+        ),
+        (
+            [f"{create_default_invalid_package_name()}-{create_default_invalid_full_version()}-foo"],
+            raises(ValidationError),
+        ),
     ],
 )
-def test_formatv2(format_: int, expectation: ContextManager[str]) -> None:
+def test_installed(installed: list[str], expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.buildinfo.Installed."""
     with expectation:
-        buildinfo.FormatV2(format_=format_)
-
+        buildinfo.Installed(installed=installed)
 
-def test_installed(default_package_name: str, default_full_version: str, default_arch: str) -> None:
-    with does_not_raise():
-        buildinfo.Installed(installed=[f"{default_package_name}-{default_full_version}-{default_arch}"])
 
-
-def test_invalid_installed(
-    default_invalid_package_name: str,
-    default_invalid_full_version: str,
+def test_installed_as_models(
+    default_arch: str,
+    default_full_version: str,
+    default_package_name: str,
 ) -> None:
-    with raises(ValidationError):
-        buildinfo.Installed(installed=[f"{default_invalid_package_name}-{default_invalid_full_version}-foo"])
+    """Tests for repod.files.buildinfo.Installed.as_models."""
+    assert [  # nosec: B101
+        (
+            buildinfo.PkgName(pkgname=default_package_name),
+            buildinfo.PkgVer(pkgver=default_full_version),
+            ArchitectureEnum(default_arch),
+        )
+    ] == buildinfo.Installed.as_models(installed=[f"{default_package_name}-{default_full_version}-{default_arch}"])
 
 
 def test_options(default_option: str, default_invalid_option: str) -> None:
+    """Tests for repod.files.buildinfo.Options."""
     with does_not_raise():
         buildinfo.Options(options=[default_option])
     with raises(ValidationError):
         buildinfo.Options(options=[default_invalid_option])
 
 
 def test_packager(default_packager: str) -> None:
+    """Tests for repod.files.buildinfo.Packager."""
     with does_not_raise():
         buildinfo.Packager(packager=default_packager)
 
 
 def test_invalid_packager(default_invalid_packager: str) -> None:
+    """Tests for repod.files.buildinfo.Packager."""
     with raises(ValidationError):
         buildinfo.Packager(packager=default_invalid_packager)
 
 
 def test_pkgarch(default_arch: str) -> None:
+    """Tests for repod.files.buildinfo.PkgArch."""
     with does_not_raise():
         buildinfo.PkgArch(pkgarch=default_arch)
     with raises(ValidationError):
         buildinfo.PkgArch(pkgarch="foo")
 
 
 def test_pkgbase(default_package_name: str, default_invalid_package_name: str) -> None:
+    """Tests for repod.files.buildinfo.PkgBase."""
     with does_not_raise():
         buildinfo.PkgBase(pkgbase=default_package_name)
     with raises(ValidationError):
         buildinfo.PkgBase(pkgbase=default_invalid_package_name)
 
 
 def test_pkgbuildsha256sum(sha256sum: str) -> None:
+    """Tests for repod.files.buildinfo.PkgBuildSha256Sum."""
     with does_not_raise():
         buildinfo.PkgBuildSha256Sum(pkgbuild_sha256sum=sha256sum)
     with raises(ValidationError):
         buildinfo.PkgBuildSha256Sum(pkgbuild_sha256sum="f00")
 
 
 def test_pkgname(default_package_name: str, default_invalid_package_name: str) -> None:
+    """Tests for repod.files.buildinfo.PkgName."""
     with does_not_raise():
         buildinfo.PkgName(pkgname=default_package_name)
     with raises(ValidationError):
         buildinfo.PkgName(pkgname=default_invalid_package_name)
 
 
 def test_pkgver(default_full_version: str, default_invalid_full_version: str) -> None:
+    """Tests for repod.files.buildinfo.PkgVer."""
     with does_not_raise():
         buildinfo.PkgVer(pkgver=default_full_version)
     with raises(ValidationError):
         buildinfo.PkgVer(pkgver=default_invalid_full_version)
 
 
-def test_startdir(absolute_dir: str, invalid_absolute_dir: str) -> None:
-    with does_not_raise():
-        buildinfo.StartDir(startdir=absolute_dir)
-    with raises(ValidationError):
-        buildinfo.StartDir(startdir=invalid_absolute_dir)
+@mark.parametrize(
+    "path, expectation",
+    [
+        ("/", does_not_raise()),
+        ("/foo", does_not_raise()),
+        ("foo", raises(ValidationError)),
+        ("", raises(ValidationError)),
+    ],
+)
+def test_startdir(path: str, expectation: ContextManager[str]) -> None:
+    """Tests for invalid repod.files.buildinfo.StartDir."""
+    with expectation:
+        buildinfo.StartDir(startdir=path)
 
 
 def test_buildinfo_from_file(
     buildinfov1_stringio: StringIO,
     buildinfov2_stringio: StringIO,
 ) -> None:
+    """Tests for repod.files.buildinfo.BuildInfo.from_file."""
     with does_not_raise():
-        assert isinstance(buildinfo.BuildInfo.from_file(data=buildinfov1_stringio), buildinfo.BuildInfoV1)
-        assert isinstance(buildinfo.BuildInfo.from_file(data=buildinfov2_stringio), buildinfo.BuildInfoV2)
+        assert isinstance(  # nosec: B101
+            buildinfo.BuildInfo.from_file(data=buildinfov1_stringio), buildinfo.BuildInfoV1
+        )
+        assert isinstance(  # nosec: B101
+            buildinfo.BuildInfo.from_file(data=buildinfov2_stringio), buildinfo.BuildInfoV2
+        )
 
     with raises(RepoManagementError):
         buildinfo.BuildInfo.from_file(data=StringIO(initial_value="foo = bar\n"))
 
 
 def test_buildinfov2_validate_devtools_version(
     default_full_version: str,
     default_invalid_full_version: str,
     default_packager: str,
     sha256sum: str,
 ) -> None:
+    """Tests for repod.files.buildinfo.BuildInfoV2.validate_devtools_version."""
     with raises(ValidationError):
         buildinfo.BuildInfoV2(
             builddate=1,
             builddir="/foo",
             buildenv=[],
             buildtool="devtools",
             buildtoolver=f"{default_invalid_full_version}-any",
@@ -185,14 +228,15 @@
             pkgname="foo",
             pkgver=default_full_version,
             startdir="/bar",
         )
 
 
 def test_export_schemas() -> None:
+    """Tests for repod.files.buildinfo.export_schemas."""
     with TemporaryDirectory() as tmp:
         buildinfo.export_schemas(output=str(tmp))
         buildinfo.export_schemas(output=tmp)
 
     with raises(RuntimeError):
         buildinfo.export_schemas(output="/foobar")
 
@@ -202,26 +246,27 @@
 
 @mark.integration
 @mark.skipif(
     not Path("/var/cache/pacman/pkg/").exists(),
     reason="Package cache in /var/cache/pacman/pkg/ does not exist",
 )
 async def test_read_buildinfo_files() -> None:
+    """Integration tests for repod.files.buildinfo.BuildInfo.from_file."""
     packages = sorted(
         [
             path
             for path in list(Path("/var/cache/pacman/pkg/").iterdir())
             if isinstance(fullmatch(rf"^.*\.pkg\.tar({tar_compression_types_for_filename_regex()})$", str(path)), Match)
         ]
     )
     if len(packages) > 50:
         packages = sample(packages, 50)
     for package in packages:
         print(f"DEBUG::: Reading .BUILDINFO file from package {package}...")
-        assert isinstance(
+        assert isinstance(  # nosec: B101
             buildinfo.BuildInfo.from_file(
                 await extract_file_from_tarfile(  # type: ignore[arg-type]
                     tarfile=open_tarfile(package),
                     file=".BUILDINFO",
                     as_stringio=True,
                 )
             ),
```

### Comparing `repod-0.2.2/tests/files/test_common.py` & `repod-0.3.0.post0/tests/files/test_common.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+"""Tests for repod.files.common."""
 from contextlib import nullcontext as does_not_raise
+from io import StringIO
 from pathlib import Path
 from tarfile import TarFile
-from typing import ContextManager, List, Optional, Set, Tuple, Union
+from typing import ContextManager
 from unittest.mock import patch
 
 from pytest import mark, raises
 
 from repod.common.enums import CompressionTypeEnum
 from repod.errors import RepoManagementFileError, RepoManagementFileNotFoundError
 from repod.files import common
@@ -26,23 +28,24 @@
         (".zst", CompressionTypeEnum.LZMA, raises(RepoManagementFileError)),
         (".txt", CompressionTypeEnum.NONE, raises(RepoManagementFileError)),
         (".txt", "foo", raises(RepoManagementFileError)),
     ],
 )
 def test_open_tarfile(
     file_type: str,
-    compression_override: Optional[str],
+    compression_override: CompressionTypeEnum | None,
     expectation: ContextManager[str],
     bz2_file: Path,
     gz_file: Path,
     tar_file: Path,
     text_file: Path,
     xz_file: Path,
     zst_file: Path,
 ) -> None:
+    """Tests for repod.files.common.open_tarfile."""
     match file_type:
         case ".bz2":
             path = bz2_file
         case ".gz":
             path = gz_file
         case ".tar":
             path = tar_file
@@ -53,34 +56,36 @@
         case ".txt":
             path = text_file
     with expectation:
         with common.open_tarfile(
             path=path,
             compression=compression_override,
         ) as tarfile_file:
-            assert isinstance(tarfile_file, TarFile)
+            assert isinstance(tarfile_file, TarFile)  # nosec: B101
 
 
 def test_open_tarfile_sync_db_file(
-    default_sync_db_file: Tuple[Path, Path],
-    files_sync_db_file: Tuple[Path, Path],
+    default_sync_db_file: tuple[Path, Path],
+    files_sync_db_file: tuple[Path, Path],
 ) -> None:
+    """Tests for opening sync database files using repod.files.common.open_tarfile."""
     for path in default_sync_db_file + files_sync_db_file:
         with common.open_tarfile(
             path=path,
         ) as tarfile_file:
-            assert isinstance(tarfile_file, TarFile)
+            assert isinstance(tarfile_file, TarFile)  # nosec: B101
 
 
 def test_open_tarfile_relative_path() -> None:
+    """Tests for opening relative paths using repod.files.common.open_tarfile."""
     with raises(RepoManagementFileError):
         with common.open_tarfile(
             path=Path("foo"),
         ) as tarfile_file:
-            assert isinstance(tarfile_file, TarFile)
+            assert isinstance(tarfile_file, TarFile)  # nosec: B101
 
 
 @mark.parametrize(
     "file, as_stringio, gzip_compressed, expectation",
     [
         (".BUILDINFO", True, False, does_not_raise()),
         (".MTREE", True, True, does_not_raise()),
@@ -94,27 +99,29 @@
     ],
 )
 async def test_extract_file_from_tarfile(
     file: str,
     as_stringio: bool,
     gzip_compressed: bool,
     expectation: ContextManager[str],
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
 ) -> None:
+    """Tests for repod.files.common.extract_file_from_tarfile."""
     with common.open_tarfile(path=default_package_file[0], compression=None, mode="r") as tarfile:
         with expectation:
             await common.extract_file_from_tarfile(
                 tarfile=tarfile,
                 file=file,
                 as_stringio=as_stringio,
                 gzip_compressed=gzip_compressed,
             )
 
 
 def test_zstdtarfile_raises(zst_file: Path) -> None:
+    """Tests for failing repod.files.common.ZstdTarFile."""
     with patch.object(common.TarFile, "__init__") as tarfile_mock:
         tarfile_mock.side_effect = Exception("FAIL")
         with raises(RepoManagementFileError):
             common.ZstdTarFile(name=zst_file, mode="r")
 
 
 @mark.parametrize(
@@ -134,48 +141,77 @@
     bz2_file: Path,
     gz_file: Path,
     tar_file: Path,
     text_file: Path,
     xz_file: Path,
     zst_file: Path,
 ) -> None:
+    """Tests for repod.files.common.compression_type_of_tarfile."""
     match file_type:
         case ".bz2":
             path = bz2_file
             result = CompressionTypeEnum.BZIP2
         case ".gz":
             path = gz_file
             result = CompressionTypeEnum.GZIP
         case ".tar":
             path = tar_file
             result = CompressionTypeEnum.NONE
         case ".txt":
             path = text_file
-            result = None
+            result = None  # type: ignore[assignment]
         case ".xz":
             path = xz_file
             result = CompressionTypeEnum.LZMA
         case ".zst":
             path = zst_file
             result = CompressionTypeEnum.ZSTANDARD
         case ".foo":
             path = Path("foo.foo")
     with expectation:
-        assert common.compression_type_of_tarfile(path=path) == result
+        assert common.compression_type_of_tarfile(path=path) == result  # nosec: B101
 
 
 @mark.parametrize(
     "names, expectation",
     [
         ([".BUILDINFO", ".MTREE", ".PKGINFO", "text_file"], True),
         ({".BUILDINFO", ".MTREE", ".PKGINFO", "text_file"}, True),
         (["foo", "bar"], False),
         ({"foo", "bar"}, False),
     ],
 )
 def test_names_in_tarfile(
-    names: Union[List[str], Set[str]],
+    names: list[str] | set[str],
     expectation: bool,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
 ) -> None:
+    """Tests for repod.files.common.names_in_tarfile."""
     with common.open_tarfile(path=default_package_file[0], compression=None, mode="r") as tarfile:
-        assert common.names_in_tarfile(tarfile=tarfile, names=names) is expectation
+        assert common.names_in_tarfile(tarfile=tarfile, names=names) is expectation  # nosec: B101
+
+
+@mark.parametrize(
+    "as_string, exists, expectation",
+    [
+        (True, True, does_not_raise()),
+        (False, True, does_not_raise()),
+        (False, False, raises(RepoManagementFileNotFoundError)),
+        (True, False, raises(RepoManagementFileNotFoundError)),
+    ],
+)
+def test_read_text_from_file(
+    as_string: bool,
+    exists: bool,
+    expectation: ContextManager[str],
+    text_file: Path,
+) -> None:
+    """Tests for repod.files.common.read_text_from_file."""
+    path: str | Path = text_file
+    if as_string:
+        path = str(text_file)
+
+    if not exists:
+        path = text_file.parent / "foo"
+
+    with expectation:
+        assert isinstance(common.read_text_from_file(path=path), StringIO)  # nosec: B101
```

### Comparing `repod-0.2.2/tests/files/test_mtree.py` & `repod-0.3.0.post0/tests/files/test_mtree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,129 @@
+"""Tests for repod.files.mtree."""
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from logging import DEBUG
 from pathlib import Path
 from random import choice, randrange, sample
 from re import Match, fullmatch
 from string import ascii_lowercase, digits
 from tempfile import TemporaryDirectory
-from typing import ContextManager, Optional
+from typing import ContextManager
 
 from pydantic import ValidationError
 from pytest import LogCaptureFixture, mark, raises
 
 from repod.common.enums import tar_compression_types_for_filename_regex
 from repod.errors import RepoManagementValidationError
 from repod.files import mtree
 from repod.files.common import extract_file_from_tarfile, open_tarfile
 
 
 @mark.parametrize(
     "gid, expectation",
     [
-        (randrange(0, 1000, 1), does_not_raise()),
-        (randrange(1000, 65535, 1), raises(ValidationError)),
-        (randrange(-65535, 0, 1), raises(ValidationError)),
+        (randrange(0, 1000, 1), does_not_raise()),  # nosec: B311
+        (randrange(1000, 65535, 1), raises(ValidationError)),  # nosec: B311
+        (randrange(-65535, 0, 1), raises(ValidationError)),  # nosec: B311
     ],
 )
 def test_systemgid(gid: int, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.SystemGID."""
     with expectation:
         mtree.SystemGID(gid=gid)
 
 
 @mark.parametrize(
     "link, expectation",
     [
         (None, does_not_raise()),
         ("../foo/bar", does_not_raise()),
         ("/foo/bar", does_not_raise()),
         ("/foo/bar", does_not_raise()),
         ("äüö", raises(ValidationError)),
     ],
 )
-def test_linktarget(link: Optional[str], expectation: ContextManager[str]) -> None:
+def test_linktarget(link: str | None, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.LinkTarget."""
     with expectation:
         mtree.LinkTarget(link=link)
 
 
 @mark.parametrize(
     "md5, expectation",
     [
         (None, does_not_raise()),
-        ("".join(choice("abcdef" + digits) for x in range(32)), does_not_raise()),
-        ("".join(choice("abcdef" + digits) for x in range(33)), raises(ValidationError)),
-        ("".join(choice("abcdef" + digits) for x in range(31)), raises(ValidationError)),
-        ("".join(choice(ascii_lowercase + digits) for x in range(32)), raises(ValidationError)),
+        ("".join(choice("abcdef" + digits) for x in range(32)), does_not_raise()),  # nosec: B311
+        ("".join(choice("abcdef" + digits) for x in range(33)), raises(ValidationError)),  # nosec: B311
+        ("".join(choice("abcdef" + digits) for x in range(31)), raises(ValidationError)),  # nosec: B311
+        ("".join(choice(ascii_lowercase + digits) for x in range(32)), raises(ValidationError)),  # nosec: B311
     ],
 )
-def test_md5(md5: Optional[str], expectation: ContextManager[str]) -> None:
+def test_md5(md5: str | None, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.Md5."""
     with expectation:
         mtree.Md5(md5=md5)
 
 
 @mark.parametrize(
     "mode, expectation",
     [
-        ("".join(choice("01234567") for x in range(3)), does_not_raise()),
-        ("".join(choice("01234567") for x in range(4)), does_not_raise()),
-        ("".join(choice("01234567") for x in range(2)), raises(ValidationError)),
-        ("".join(choice("01234567") for x in range(5)), raises(ValidationError)),
-        ("".join(choice("89") for x in range(3)), raises(ValidationError)),
-        ("".join(choice("89") for x in range(4)), raises(ValidationError)),
+        ("".join(choice("01234567") for x in range(3)), does_not_raise()),  # nosec: B311
+        ("".join(choice("01234567") for x in range(4)), does_not_raise()),  # nosec: B311
+        ("".join(choice("01234567") for x in range(2)), raises(ValidationError)),  # nosec: B311
+        ("".join(choice("01234567") for x in range(5)), raises(ValidationError)),  # nosec: B311
+        ("".join(choice("89") for x in range(3)), raises(ValidationError)),  # nosec: B311
+        ("".join(choice("89") for x in range(4)), raises(ValidationError)),  # nosec: B311
     ],
 )
 def test_filemode(mode: str, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.FileMode."""
     with expectation:
         mtree.FileMode(mode=mode)
 
 
 @mark.parametrize(
     "sha256, expectation",
     [
         (None, does_not_raise()),
-        ("".join(choice("abcdef" + digits) for x in range(64)), does_not_raise()),
-        ("".join(choice("abcdef" + digits) for x in range(65)), raises(ValidationError)),
-        ("".join(choice("abcdef" + digits) for x in range(63)), raises(ValidationError)),
-        ("".join(choice(ascii_lowercase + digits) for x in range(64)), raises(ValidationError)),
+        ("".join(choice("abcdef" + digits) for x in range(64)), does_not_raise()),  # nosec: B311
+        ("".join(choice("abcdef" + digits) for x in range(65)), raises(ValidationError)),  # nosec: B311
+        ("".join(choice("abcdef" + digits) for x in range(63)), raises(ValidationError)),  # nosec: B311
+        ("".join(choice(ascii_lowercase + digits) for x in range(64)), raises(ValidationError)),  # nosec: B311
     ],
 )
-def test_sha256(sha256: Optional[str], expectation: ContextManager[str]) -> None:
+def test_sha256(sha256: str | None, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.Sha256."""
     with expectation:
         mtree.Sha256(sha256=sha256)
 
 
 @mark.parametrize(
     "size, expectation",
     [
         (None, does_not_raise()),
-        (randrange(0, 1000, 1), does_not_raise()),
-        (randrange(-1000, 0, 1), raises(ValidationError)),
+        (randrange(0, 1000, 1), does_not_raise()),  # nosec: B311
+        (randrange(-1000, 0, 1), raises(ValidationError)),  # nosec: B311
     ],
 )
-def test_filesize(size: Optional[int], expectation: ContextManager[str]) -> None:
+def test_filesize(size: int | None, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.FileSize."""
     with expectation:
         mtree.FileSize(size=size)
 
 
 @mark.parametrize(
     "time, expectation",
     [
         (1000.0, does_not_raise()),
         (-1000.0, raises(ValidationError)),
     ],
 )
-def test_unixtime(time: Optional[float], expectation: ContextManager[str]) -> None:
+def test_unixtime(time: float, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.UnixTime."""
     with expectation:
         mtree.UnixTime(time=time)
 
 
 @mark.parametrize(
     "type_, expectation",
     [
@@ -126,298 +134,312 @@
         ("file", does_not_raise()),
         ("link", does_not_raise()),
         ("socket", does_not_raise()),
         ("foo", raises(ValidationError)),
     ],
 )
 def test_mtreefiletype(type_: str, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.MTreeEntryType."""
     with expectation:
         mtree.MTreeEntryType(type_=type_)
 
 
 @mark.parametrize(
     "uid, expectation",
     [
-        (randrange(0, 1000, 1), does_not_raise()),
-        (randrange(1000, 65535, 1), raises(ValidationError)),
-        (randrange(-65535, 0, 1), raises(ValidationError)),
+        (randrange(0, 1000, 1), does_not_raise()),  # nosec: B311
+        (randrange(1000, 65535, 1), raises(ValidationError)),  # nosec: B311
+        (randrange(-65535, 0, 1), raises(ValidationError)),  # nosec: B311
     ],
 )
 def test_systemuid(uid: int, expectation: ContextManager[str]) -> None:
+    """Tests for repod.files.mtree.SystemUID."""
     with expectation:
         mtree.SystemUID(uid=uid)
 
 
 def test_mtreefile_get_file_path() -> None:
+    """Tests for repod.files.mtree.MTreeEntry.get_file_path."""
     mtreefile = mtree.MTreeEntry()
     with raises(RuntimeError):
         mtreefile.get_file_path()
 
 
 def test_mtreefile_get_link_path() -> None:
+    """Tests for repod.files.mtree.MTreeEntry.get_link_path."""
     mtreefile = mtree.MTreeEntry()
     with raises(RuntimeError):
         mtreefile.get_link_path()
 
 
 @mark.parametrize(
     "mtreefilev1, return_value",
     [
         (
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link=None,
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo\\040bar",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("/foo bar"),
         ),
         (
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link=None,
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/" + "".join(map(str, set(range(0x20, 0x7E)) - {ord("#"), ord(" "), ord("="), ord("\\")})),
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("/" + "".join(map(str, set(range(0x20, 0x7E)) - {ord("#"), ord(" "), ord("="), ord("\\")}))),
         ),
         (
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link=None,
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/\\320\\220\\321\\202\\320\\273\\320\\260\\321\\201\\320\\275\\321\\213\\320\\265.svgz",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
-            Path("/Атласные.svgz"),
+            Path("/Атласные.svgz"),  # noqa: RUF001
         ),
     ],
 )
 def test_mtreefilev1_get_file_path(
     mtreefilev1: mtree.MTreeEntryV1, return_value: Path, caplog: LogCaptureFixture
 ) -> None:
+    """Tests for repod.files.mtree.MTreeEntryV1.get_file_path."""
     caplog.set_level(DEBUG)
-    assert mtreefilev1.get_file_path() == return_value
+    assert mtreefilev1.get_file_path() == return_value  # nosec: B101
 
 
 @mark.parametrize(
     "resolve, mtreefilev1, return_value",
     [
         (
             False,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="/bar\\040baz",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo\\040bar",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("/bar baz"),
         ),
         (
             False,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="bar\\040baz",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo\\040bar",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("bar baz"),
         ),
         (
             False,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="../bar\\040baz",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo/bar/baz",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("../bar baz"),
         ),
         (
             True,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="/bar\\040baz",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo\\040bar",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("/bar baz"),
         ),
         (
             True,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="bar\\040baz",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo\\040bar",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("/bar baz"),
         ),
         (
             True,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="../bar\\040baz",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo/bar/baz",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("/foo/bar/bar baz"),
         ),
         (
             True,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="../\\320\\220\\321\\202\\320\\273\\320\\260\\321\\201\\320\\275\\321\\213\\320\\265.svgz",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo/bar/baz",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
-            Path("/foo/bar/Атласные.svgz"),
+            Path("/foo/bar/Атласные.svgz"),  # noqa: RUF001
         ),
         (
             False,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link="/foo",
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo/bar/baz",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             Path("/foo"),
         ),
         (
             False,
             mtree.MTreeEntryV1(
                 mode="0644",
-                size="1000",
+                size=1000,
                 link=None,
-                md5="".join(choice("abcdef" + digits) for x in range(32)),
+                md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
                 name="/foo\\040bar",
                 type_="file",
-                sha256="".join(choice("abcdef" + digits) for x in range(64)),
+                sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
                 time=200,
                 gid=0,
                 uid=0,
             ),
             None,
         ),
     ],
 )
 def test_mtreefilev1_get_link_path(resolve: bool, mtreefilev1: mtree.MTreeEntryV1, return_value: Path) -> None:
-    assert mtreefilev1.get_link_path(resolve=resolve) == return_value
+    """Tests for repod.files.mtree.MTreeEntryV1.get_link_path."""
+    assert mtreefilev1.get_link_path(resolve=resolve) == return_value  # nosec: B101
 
 
 def test_mtreefile_get_type() -> None:
+    """Tests for repod.files.mtree.MTreeEntry.get_type."""
     mtreefile = mtree.MTreeEntry()
     with raises(RuntimeError):
         mtreefile.get_type()
 
 
 def test_mtreefilev1_get_type() -> None:
-    assert (
+    """Tests for repod.files.mtree.MTreeEntryV1.get_type."""
+    assert (  # nosec: B101
         mtree.MTreeEntryV1(
             mode="0644",
-            size="1000",
+            size=1000,
             link=None,
-            md5="".join(choice("abcdef" + digits) for x in range(32)),
+            md5="".join(choice("abcdef" + digits) for x in range(32)),  # nosec: B311
             name="/foo\\040bar",
             type_="file",
-            sha256="".join(choice("abcdef" + digits) for x in range(64)),
+            sha256="".join(choice("abcdef" + digits) for x in range(64)),  # nosec: B311
             time=200,
             gid=0,
             uid=0,
         ).get_type()
         == "file"
     )
 
 
 def test_mtree_get_paths(valid_mtree: mtree.MTree) -> None:
-    assert valid_mtree.get_paths()
+    """Tests for repod.files.mtree.MTreeEntryV1.get_paths."""
+    assert valid_mtree.get_paths()  # nosec: B101
 
 
 @mark.parametrize("valid, expectation", [(True, does_not_raise()), (False, raises(RepoManagementValidationError))])
 def test_mtree_from_file(
     valid: bool,
     expectation: ContextManager[str],
     mtreeentryv1_stringio: StringIO,
     invalid_mtreeentryv1_stringio: StringIO,
+    caplog: LogCaptureFixture,
 ) -> None:
+    """Tests for repod.files.mtree.MTree.from_file."""
+    caplog.set_level(DEBUG)
+
     if valid:
         data = mtreeentryv1_stringio
     else:
         data = invalid_mtreeentryv1_stringio
 
     with expectation:
-        assert isinstance(mtree.MTree.from_file(data=data), mtree.MTree)
+        assert isinstance(mtree.MTree.from_file(data=data), mtree.MTree)  # nosec: B101
 
 
 def test_export_schemas() -> None:
+    """Tests for repod.files.mtree.export_schemas."""
     with TemporaryDirectory() as tmp:
         mtree.export_schemas(output=str(tmp))
         mtree.export_schemas(output=tmp)
 
     with raises(RuntimeError):
         mtree.export_schemas(output="/foobar")
 
@@ -427,25 +449,26 @@
 
 @mark.integration
 @mark.skipif(
     not Path("/var/cache/pacman/pkg/").exists(),
     reason="Package cache in /var/cache/pacman/pkg/ does not exist",
 )
 async def test_read_mtree_files() -> None:
+    """Integration tests for repod.files.mtree.MTree.from_file."""
     packages = sorted(
         [
             path
             for path in list(Path("/var/cache/pacman/pkg/").iterdir())
             if isinstance(fullmatch(rf"^.*\.pkg\.tar({tar_compression_types_for_filename_regex()})$", str(path)), Match)
         ]
     )
     if len(packages) > 50:
         packages = sample(packages, 50)
     for package in packages:
-        assert isinstance(
+        assert isinstance(  # nosec: B101
             mtree.MTree.from_file(
                 await extract_file_from_tarfile(  # type: ignore[arg-type]
                     tarfile=open_tarfile(package),
                     file=".MTREE",
                     as_stringio=True,
                     gzip_compressed=True,
                 )
```

### Comparing `repod-0.2.2/tests/files/test_package.py` & `repod-0.3.0.post0/tests/files/test_package.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+"""Tests for repod.files.package."""
 from contextlib import nullcontext as does_not_raise
 from logging import DEBUG
 from pathlib import Path
-from typing import ContextManager, Tuple
+from typing import ContextManager
 
 from pytest import LogCaptureFixture, mark, raises
 
 from repod.errors import RepoManagementFileError
 from repod.files import package
 
 
@@ -20,29 +21,30 @@
 )
 async def test_package_from_file(
     add_sig: bool,
     valid_sig_name: bool,
     sig_exists: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
-    default_sync_db_file: Tuple[Path],
+    default_package_file: tuple[Path, ...],
+    default_sync_db_file: tuple[Path],
 ) -> None:
+    """Tests for repod.files.package.Package.from_file."""
     caplog.set_level(DEBUG)
 
     signature = default_package_file[1]
 
     if not sig_exists:
         signature.unlink()
 
     if not valid_sig_name:
         signature = Path("foo")
 
     with expectation:
-        assert isinstance(
+        assert isinstance(  # nosec: B101
             await package.Package.from_file(
                 package=default_package_file[0],
                 signature=signature if add_sig else None,
             ),
             package.PackageV1,
         )
 
@@ -50,23 +52,25 @@
         await package.Package.from_file(package=default_sync_db_file[0])
 
 
 async def test_packagev1_top_level_dict(
     caplog: LogCaptureFixture,
     packagev1: package.PackageV1,
 ) -> None:
+    """Tests for repod.files.package.Package.top_level_dict."""
     caplog.set_level(DEBUG)
     keys = set(packagev1.top_level_dict().keys())
-    assert len(packagev1.buildinfo.dict().keys() - keys) == 0
-    assert len(packagev1.mtree.dict().keys() - keys) == 0
-    assert len(packagev1.pkginfo.dict().keys() - keys) == 0
-    assert len({"csize", "filename", "md5sum", "pgpsig", "sha256sum"} - keys) == 0
+    assert len(packagev1.buildinfo.model_dump().keys() - keys) == 0  # nosec: B101
+    assert len(packagev1.mtree.model_dump().keys() - keys) == 0  # nosec: B101
+    assert len(packagev1.pkginfo.model_dump().keys() - keys) == 0  # nosec: B101
+    assert len({"csize", "filename", "md5sum", "pgpsig", "sha256sum"} - keys) == 0  # nosec: B101
 
 
 def test_export_schemas(tmp_path: Path) -> None:
+    """Tests for repod.files.package.export_schemas."""
     package.export_schemas(output=str(tmp_path))
     package.export_schemas(output=tmp_path)
 
     with raises(RuntimeError):
         package.export_schemas(output="/foobar")
 
     with raises(RuntimeError):
```

### Comparing `repod-0.2.2/tests/files/test_pkginfo.py` & `repod-0.3.0.post0/tests/files/test_pkginfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+"""Tests for repod.files.pkginfo."""
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from logging import DEBUG
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
-from typing import Any, ContextManager, Dict, List, Union
+from typing import Any, ContextManager
 from unittest.mock import patch
 
 from pydantic import ValidationError
 from pytest import LogCaptureFixture, mark, raises
 
 from repod.common.enums import FieldTypeEnum, tar_compression_types_for_filename_regex
 from repod.errors import RepoManagementError, RepoManagementFileError
@@ -26,23 +27,24 @@
         ("foobar", " = ", None, None, None, raises(RepoManagementFileError)),
     ],
 )
 def test_parse_pairs(
     line: str,
     separator: str,
     key: str,
-    value: Union[int, str, List[str]],
+    value: int | str | list[str],
     field_type: FieldTypeEnum,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
 ) -> None:
+    """Tests for repod.files.pkginfo.parse_pairs."""
     caplog.set_level(DEBUG)
 
     with expectation:
-        assert (key, value, field_type) == pkginfo.parse_pairs(line=line, separator=separator)
+        assert (key, value, field_type) == pkginfo.parse_pairs(line=line, separator=separator)  # nosec: B101
 
 
 @mark.parametrize(
     "key, value, field_type, input_entries, output_entries, expectation",
     [
         (
             "pkgtype",
@@ -73,53 +75,58 @@
         ),
     ],
 )
 def test_pairs_to_entries(
     key: str,
     value: str,
     field_type: FieldTypeEnum,
-    input_entries: Dict[str, Any],
-    output_entries: Dict[str, Any],
+    input_entries: dict[str, Any],
+    output_entries: dict[str, Any],
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
 ) -> None:
+    """Tests for repod.files.pkginfo.pairs_to_entries."""
     caplog.set_level(DEBUG)
 
     with expectation:
         pkginfo.pairs_to_entries(
             key=key,
             value=value,
             field_type=field_type,
             entries=input_entries,
         )
-        assert input_entries == output_entries
+        assert input_entries == output_entries  # nosec: B101
 
 
 def test_fakerootversion(default_version: str, default_invalid_version: str) -> None:
+    """Tests for repod.files.pkginfo.FakerootVersion."""
     with does_not_raise():
         pkginfo.FakerootVersion(fakeroot_version=default_version)
     with raises(ValidationError):
         pkginfo.FakerootVersion(fakeroot_version=default_invalid_version)
 
 
 def test_makepkgversion(default_version: str, default_invalid_version: str) -> None:
+    """Tests for repod.files.pkginfo.MakepkgVersion."""
     with does_not_raise():
         pkginfo.MakepkgVersion(makepkg_version=default_version)
     with raises(ValidationError):
         pkginfo.MakepkgVersion(makepkg_version=default_invalid_version)
 
 
 def test_pkgtype(default_pkgtype: str, default_invalid_pkgtype: str) -> None:
+    """Tests for repod.files.pkginfo.PkgType."""
     with does_not_raise():
-        pkginfo.PkgType(pkgtype=default_pkgtype)
+        pkginfo.PkgType(pkgtype=default_pkgtype)  # type: ignore[arg-type]
     with raises(ValidationError):
-        pkginfo.PkgType(pkgtype=default_invalid_pkgtype)
+        pkginfo.PkgType(pkgtype=default_invalid_pkgtype)  # type: ignore[arg-type]
 
 
 def test_export_schemas(tmp_path: Path) -> None:
+    """Tests for repod.files.pkginfo.export_schemas."""
     pkginfo.export_schemas(output=str(tmp_path))
     pkginfo.export_schemas(output=tmp_path)
 
     with raises(RuntimeError):
         pkginfo.export_schemas(output="/foobar")
 
     with raises(RuntimeError):
@@ -127,51 +134,53 @@
 
 
 def test_pkginfo_from_file(
     caplog: LogCaptureFixture,
     pkginfov1_stringio: StringIO,
     pkginfov2_stringio: StringIO,
 ) -> None:
+    """Tests for repod.files.pkginfo.PkgInfo.from_file."""
     caplog.set_level(DEBUG)
     with does_not_raise():
-        assert isinstance(pkginfo.PkgInfo.from_file(data=pkginfov2_stringio), pkginfo.PkgInfoV2)
+        assert isinstance(pkginfo.PkgInfo.from_file(data=pkginfov2_stringio), pkginfo.PkgInfoV2)  # nosec: B101
 
     with patch(
         "repod.files.pkginfo.PKGINFO_VERSIONS",
         pkginfo.PKGINFO_VERSIONS | {len(pkginfo.PKGINFO_VERSIONS) + 1: {"required": {"foo"}}},
     ):
         with raises(RepoManagementError):
-            assert isinstance(pkginfo.PkgInfo.from_file(data=pkginfov2_stringio), pkginfo.PkgInfoV2)
+            assert isinstance(pkginfo.PkgInfo.from_file(data=pkginfov2_stringio), pkginfo.PkgInfoV2)  # nosec: B101
 
     with patch("repod.files.pkginfo.PKGINFO_VERSIONS", {1: pkginfo.PKGINFO_VERSIONS[1]}):
         with does_not_raise():
-            assert isinstance(pkginfo.PkgInfo.from_file(data=pkginfov1_stringio), pkginfo.PkgInfoV1)
+            assert isinstance(pkginfo.PkgInfo.from_file(data=pkginfov1_stringio), pkginfo.PkgInfoV1)  # nosec: B101
 
     with raises(RepoManagementError):
         pkginfo.PkgInfo.from_file(data=StringIO(initial_value="base = foo\n"))
 
 
 @mark.integration
 @mark.skipif(
     not Path("/var/cache/pacman/pkg/").exists(),
     reason="Package cache in /var/cache/pacman/pkg/ does not exist",
 )
 async def test_read_pkginfo_files() -> None:
+    """Integration tests for repod.files.pkginfo.PkgInfo.from_file."""
     packages = sorted(
         [
             path
             for path in list(Path("/var/cache/pacman/pkg/").iterdir())
             if isinstance(fullmatch(rf"^.*\.pkg\.tar({tar_compression_types_for_filename_regex()})$", str(path)), Match)
         ]
     )
     if len(packages) > 50:
         packages = sample(packages, 50)
     for package in packages:
         print(f"DEBUG::: Reading .PKGINFO file from package {package}...")
-        assert isinstance(
+        assert isinstance(  # nosec: B101
             pkginfo.PkgInfo.from_file(
                 await extract_file_from_tarfile(  # type: ignore[arg-type]
                     tarfile=open_tarfile(package),
                     file=".PKGINFO",
                     as_stringio=True,
                 )
             ),
```

### Comparing `repod-0.2.2/tests/repo/management/test_outputpackage.py` & `repod-0.3.0.post0/tests/repo/management/test_outputpackage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from contextlib import nullcontext as does_not_raise
 from copy import deepcopy
 from logging import DEBUG
 from pathlib import Path
-from typing import Any, ContextManager, Dict, List, Optional, Union
+from typing import Any, ContextManager
 
 from pytest import LogCaptureFixture, mark, raises
 
-from repod.common.enums import FilesVersionEnum, PackageDescVersionEnum
+from repod.common.enums import FilesVersionEnum, PackageDescVersionEnum, PkgTypeEnum
 from repod.errors import RepoManagementFileError, RepoManagementValidationError
 from repod.files.buildinfo import BuildInfo
 from repod.files.package import Package
 from repod.files.pkginfo import PkgType
 from repod.repo.management import outputpackage
 from repod.repo.package import syncdb
 from tests.conftest import (
@@ -46,15 +46,15 @@
 )
 @mark.asyncio
 async def test_output_package_base_v1_get_packages_as_models(
     packagedescv1: outputpackage.PackageDescV1,
     packagedescv2: outputpackage.PackageDescV2,
     filesv1: syncdb.FilesV1,
     outputpackagebasev1: outputpackage.OutputPackageBase,
-    outputpackagebase_version: Optional[int],
+    outputpackagebase_version: int | None,
     packagedesc_version: PackageDescVersionEnum,
     files_version: FilesVersionEnum,
     expectation: ContextManager[str],
 ) -> None:
     packagedesc: syncdb.PackageDesc
     match packagedesc_version:
         case PackageDescVersionEnum.ONE:
@@ -63,27 +63,26 @@
             packagedesc = packagedescv2
 
     files: syncdb.Files
     match files_version:
         case FilesVersionEnum.ONE:
             files = filesv1
 
-    outputpackagebase: outputpackage.OutputPackageBase
     match outputpackagebase_version:
         case None:
             output_package_base = outputpackage.OutputPackageBase()
         case 1:
             output_package_base = outputpackagebasev1
             # remove all but the first package
             output_package_base.packages = output_package_base.packages[0:1]  # type: ignore[attr-defined]
         case 9999:
             output_package_base = OutputPackageBaseV9999()
 
     with expectation:
-        assert [(packagedesc, files)] == await output_package_base.get_packages_as_models(
+        assert [(packagedesc, files)] == await output_package_base.get_packages_as_models(  # nosec: B101
             packagedesc_version=packagedesc_version,
             files_version=files_version,
         )
 
 
 @mark.parametrize(
     "data, expectation",
@@ -184,17 +183,19 @@
         "schema version 1, no packages",
         "schema version 0, no packages",
         "schema version 9999, no packages",
         "schema version 1, 1 package",
         "schema version 1, package is string",
     ],
 )
-def test_outputpackagebase_from_dict(data: Dict[str, Union[Any, List[Any]]], expectation: ContextManager[str]) -> None:
+def test_outputpackagebase_from_dict(data: dict[str, Any | list[Any]], expectation: ContextManager[str]) -> None:
     with expectation:
-        assert isinstance(outputpackage.OutputPackageBase.from_dict(data=data), outputpackage.OutputPackageBase)
+        assert isinstance(  # nosec: B101
+            outputpackage.OutputPackageBase.from_dict(data=data), outputpackage.OutputPackageBase
+        )
 
 
 @mark.asyncio
 async def test_outputpackagebase_from_file(broken_json_file: Path, invalid_json_file: Path) -> None:
     with raises(RepoManagementFileError):
         await outputpackage.OutputPackageBase.from_file(path=broken_json_file)
     with raises(RepoManagementValidationError):
@@ -203,20 +204,20 @@
 
 def test_outputpackagebase_from_package() -> None:
     with raises(RuntimeError):
         outputpackage.OutputPackageBase.from_package(packages=[Package()])
 
 
 def test_outputpackagebase_from_packagev1(packagev1: Package) -> None:
-    assert outputpackage.OutputPackageBase.from_package(packages=[packagev1])
+    assert outputpackage.OutputPackageBase.from_package(packages=[packagev1])  # nosec: B101
 
 
 def test_outputpackagebase_from_package_raise_on_no_package() -> None:
     with raises(ValueError):
-        assert outputpackage.OutputPackageBase.from_package(packages=[])
+        assert outputpackage.OutputPackageBase.from_package(packages=[])  # nosec: B101
 
 
 def test_outputpackagebase_from_packagev1_raise_on_multiple_pkgbases(packagev1: Package) -> None:
     package_b = deepcopy(packagev1)
     package_b.buildinfo.pkgbase = "wrong"  # type: ignore[attr-defined]
     with raises(ValueError):
         outputpackage.OutputPackageBase.from_package(packages=[packagev1, package_b])
@@ -224,15 +225,18 @@
 
 def test_outputpackagebase_from_packagev1_raise_on_duplicate_names(packagev1: Package) -> None:
     package_b = deepcopy(packagev1)
     with raises(ValueError):
         outputpackage.OutputPackageBase.from_package(packages=[packagev1, package_b])
 
 
-def test_outputpackagebase_from_packagev1_raise_on_version_mismatch(packagev1: Package) -> None:
+def test_outputpackagebase_from_packagev1_raise_on_version_mismatch(
+    packagev1: Package, caplog: LogCaptureFixture
+) -> None:
+    caplog.set_level(DEBUG)
     package_b = deepcopy(packagev1)
     package_b.pkginfo.name = "different"  # type: ignore[attr-defined]
     package_b.pkginfo.version = "wrong"  # type: ignore[attr-defined]
     with raises(ValueError):
         outputpackage.OutputPackageBase.from_package(packages=[packagev1, package_b])
 
 
@@ -240,15 +244,15 @@
     packagev1_pkginfov2: Package,
     caplog: LogCaptureFixture,
 ) -> None:
     caplog.set_level(DEBUG)
 
     package_b = deepcopy(packagev1_pkginfov2)
     package_b.pkginfo.name = "different"  # type: ignore[attr-defined]
-    package_b.pkginfo.xdata = [PkgType(pkgtype="debug")]  # type: ignore[attr-defined]
+    package_b.pkginfo.xdata = [PkgType(pkgtype=PkgTypeEnum.DEBUG)]  # type: ignore[attr-defined]
     with raises(ValueError):
         outputpackage.OutputPackageBase.from_package(packages=[packagev1_pkginfov2, package_b])
 
 
 @mark.parametrize(
     "output_package_base_type, expectation",
     [
@@ -314,10 +318,10 @@
             buildinfo = BuildInfoV9999()
 
     with expectation:
         outputbuildinfo = outputpackage.OutputBuildInfo.from_buildinfo(buildinfo=buildinfo)
 
         match buildinfo_version:
             case 1:
-                assert isinstance(outputbuildinfo, outputpackage.OutputBuildInfoV1)
+                assert isinstance(outputbuildinfo, outputpackage.OutputBuildInfoV1)  # nosec: B101
             case 2:
-                assert isinstance(outputbuildinfo, outputpackage.OutputBuildInfoV2)
+                assert isinstance(outputbuildinfo, outputpackage.OutputBuildInfoV2)  # nosec: B101
```

### Comparing `repod-0.2.2/tests/repo/package/test_repofile.py` & `repod-0.3.0.post0/tests/repo/package/test_repofile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,97 @@
 from contextlib import nullcontext as does_not_raise
 from logging import DEBUG
 from pathlib import Path
-from typing import ContextManager, Tuple
+from typing import ContextManager
 
 from pytest import LogCaptureFixture, mark, raises
 
 from repod.common.enums import RepoFileEnum
 from repod.errors import RepoManagementFileError
 from repod.repo.package import repofile
 
 
 @mark.parametrize(
+    "file, output, expectation",
+    [
+        (
+            Path("foo-1.0.0-1-any.pkg.tar.gz"),
+            {
+                "arch": "any",
+                "name": "foo",
+                "version": "1.0.0-1",
+                "suffix": "pkg.tar.gz",
+                "pkgrel": "1",
+                "pkgver": "1.0.0",
+                "epoch": "",
+            },
+            does_not_raise(),
+        ),
+        (
+            Path("foo-1.0.0-1-any.pkg.tar.gz.sig"),
+            {
+                "arch": "any",
+                "name": "foo",
+                "version": "1.0.0-1",
+                "suffix": "pkg.tar.gz.sig",
+                "pkgrel": "1",
+                "pkgver": "1.0.0",
+                "epoch": "",
+            },
+            does_not_raise(),
+        ),
+        (
+            Path("foo-1:1.0.0-1-any.pkg.tar.gz"),
+            {
+                "arch": "any",
+                "name": "foo",
+                "version": "1:1.0.0-1",
+                "suffix": "pkg.tar.gz",
+                "pkgrel": "1",
+                "pkgver": "1.0.0",
+                "epoch": "1",
+            },
+            does_not_raise(),
+        ),
+        (
+            Path("foo-bar-1:1.0.0-1-any.pkg.tar.gz"),
+            {
+                "arch": "any",
+                "name": "foo-bar",
+                "version": "1:1.0.0-1",
+                "suffix": "pkg.tar.gz",
+                "pkgrel": "1",
+                "pkgver": "1.0.0",
+                "epoch": "1",
+            },
+            does_not_raise(),
+        ),
+        (
+            Path("foo-bar-any.pkg.tar.gz"),
+            None,
+            raises(ValueError),
+        ),
+        (
+            Path("foo-bar-1.0.0-1-any.pkg"),
+            None,
+            raises(ValueError),
+        ),
+        (
+            Path("foo-bar-1.0.0-1-any.pkg.tar.gz.sig.foo"),
+            None,
+            raises(ValueError),
+        ),
+    ],
+)
+def test_filename_parts(file: Path, output: dict[str, str], expectation: ContextManager[str]) -> None:
+    with expectation:
+        assert repofile.filename_parts(file=file) == output  # nosec: B101
+
+
+@mark.parametrize(
     "path_a, path_b, return_value, expectation",
     [
         (Path("/foo/bar/baz"), Path("/foo/bar/beh"), Path("/foo/bar"), does_not_raise()),
         (Path("/foo/bar/baz"), Path("/foo/bar/baz"), Path("/foo/bar/baz"), does_not_raise()),
         (Path("/foo/bar/baz/buh/bah"), Path("/foo/bar/beh"), Path("/foo/bar"), does_not_raise()),
         (Path("/foo/bar/baz"), Path("/foo/bar/beh/buh/bah"), Path("/foo/bar"), does_not_raise()),
         (Path("/baz"), Path("/beh"), Path("/"), does_not_raise()),
@@ -25,15 +102,15 @@
     ],
 )
 def test_shared_base_path(
     path_a: Path, path_b: Path, return_value: Path, expectation: ContextManager[str], caplog: LogCaptureFixture
 ) -> None:
     caplog.set_level(DEBUG)
     with expectation:
-        assert repofile.shared_base_path(path_a=path_a, path_b=path_b) == return_value
+        assert repofile.shared_base_path(path_a=path_a, path_b=path_b) == return_value  # nosec: B101
 
 
 @mark.parametrize(
     "path_a, path_b, return_value, expectation",
     [
         (Path("/foo/bar/baz/file"), Path("/foo/bar/beh/file"), Path("../baz/file"), does_not_raise()),
         (Path("/foo/bar/baz/file_a"), Path("/foo/bar/baz/file_b"), Path("file_a"), does_not_raise()),
@@ -42,15 +119,15 @@
     ],
 )
 def test_relative_to_shared_base(
     path_a: Path, path_b: Path, return_value: Path, expectation: ContextManager[str], caplog: LogCaptureFixture
 ) -> None:
     caplog.set_level(DEBUG)
     with expectation:
-        assert repofile.relative_to_shared_base(path_a=path_a, path_b=path_b) == return_value
+        assert repofile.relative_to_shared_base(path_a=path_a, path_b=path_b) == return_value  # nosec: B101
 
 
 @mark.parametrize(
     "file_symlink_equal, wrong_file_type, expectation",
     [
         (False, False, does_not_raise()),
         (True, False, raises(ValueError)),
@@ -58,15 +135,15 @@
     ],
 )
 def test_repofile(
     file_symlink_equal: bool,
     wrong_file_type: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     for file in default_package_file:
         if wrong_file_type:
             file_type = RepoFileEnum.PACKAGE if file.name.endswith(".sig") else RepoFileEnum.PACKAGE_SIGNATURE
@@ -76,20 +153,52 @@
         file_path = file
         symlink_path = empty_dir / file.name
 
         if file_symlink_equal:
             symlink_path = file_path
 
         with expectation:
-            assert repofile.RepoFile(file_type=file_type, file_path=file_path, symlink_path=symlink_path)
+            assert repofile.RepoFile(file_type=file_type, file_path=file_path, symlink_path=symlink_path)  # nosec: B101
+
+
+@mark.parametrize(
+    "path_absolute, filename_matches, file_type, expectation",
+    [
+        (True, True, RepoFileEnum.PACKAGE, does_not_raise()),
+        (True, True, RepoFileEnum.PACKAGE_SIGNATURE, does_not_raise()),
+        (False, True, RepoFileEnum.PACKAGE, raises(ValueError)),
+        (False, True, RepoFileEnum.PACKAGE_SIGNATURE, raises(ValueError)),
+        (True, False, RepoFileEnum.PACKAGE, raises(ValueError)),
+        (True, False, RepoFileEnum.PACKAGE_SIGNATURE, raises(ValueError)),
+    ],
+)
+def test_repofile_validate_path(
+    path_absolute: bool,
+    filename_matches: bool,
+    file_type: RepoFileEnum,
+    expectation: ContextManager[str],
+    default_filename: str,
+    tmp_path: Path,
+) -> None:
+    if path_absolute:
+        base_path = tmp_path
+    else:
+        base_path = Path("foo")
 
+    if filename_matches:
+        match file_type:
+            case RepoFileEnum.PACKAGE:
+                path = base_path / Path(default_filename)
+            case RepoFileEnum.PACKAGE_SIGNATURE:
+                path = base_path / Path(f"{default_filename}.sig")
+    else:
+        path = base_path / "foo"
 
-def test_repofile_get_file_type_regex_raises_on_invalid() -> None:
-    with raises(RuntimeError):
-        repofile.RepoFile.get_file_type_regex(file_type=None)
+    with expectation:
+        repofile.RepoFile.validate_path(path=path, file_type=file_type)
 
 
 @mark.parametrize(
     "file_exists, exists, expectation",
     [
         (True, True, does_not_raise()),
         (False, True, raises(RepoManagementFileError)),
@@ -98,15 +207,15 @@
     ],
 )
 def test_repofile_check_file_path_exists(
     file_exists: bool,
     exists: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     if file_exists:
         file_path = default_package_file[0]
     else:
@@ -130,15 +239,15 @@
     ],
 )
 def test_repofile_check_symlink_path_exists(
     symlink_exists: bool,
     exists: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     symlink_path = empty_dir / default_package_file[0].name
     if symlink_exists:
         symlink_path.touch()
@@ -153,65 +262,65 @@
 
 
 @mark.parametrize("source_exists, expectation", [(True, does_not_raise()), (False, raises(RepoManagementFileError))])
 def test_repofile_copy_from(
     source_exists: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     source_path = default_package_file[0]
     destination_path = empty_dir / default_package_file[0].name
     if not source_exists:
         source_path = empty_dir / "bar" / default_package_file[0].name
 
-    assert not destination_path.exists()
+    assert not destination_path.exists()  # nosec: B101
 
     file = repofile.RepoFile(
         file_type=RepoFileEnum.PACKAGE,
         file_path=destination_path,
         symlink_path=empty_dir / "foo" / default_package_file[0].name,
     )
 
     with expectation:
         file.copy_from(path=source_path)
-        assert source_path.exists()
-        assert destination_path.exists()
+        assert source_path.exists()  # nosec: B101
+        assert destination_path.exists()  # nosec: B101
 
 
 @mark.parametrize("source_exists, expectation", [(True, does_not_raise()), (False, raises(RepoManagementFileError))])
 def test_repofile_move_from(
     source_exists: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     source_path = default_package_file[0]
     destination_path = empty_dir / default_package_file[0].name
     if not source_exists:
         source_path = empty_dir / "bar" / default_package_file[0].name
 
-    assert not destination_path.exists()
+    assert not destination_path.exists()  # nosec: B101
 
     file = repofile.RepoFile(
         file_type=RepoFileEnum.PACKAGE,
         file_path=destination_path,
         symlink_path=empty_dir / "foo" / default_package_file[0].name,
     )
 
     with expectation:
         file.move_from(path=source_path)
-        assert not source_path.exists()
-        assert destination_path.exists()
+        assert not source_path.exists()  # nosec: B101
+        assert destination_path.exists()  # nosec: B101
 
 
 @mark.parametrize(
     "link_exists, check, expectation",
     [
         (True, True, raises(RepoManagementFileError)),
         (True, False, raises(RepoManagementFileError)),
@@ -220,34 +329,34 @@
     ],
 )
 def test_repofile_link(
     link_exists: bool,
     check: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     symlink_path = empty_dir / default_package_file[0].name
     if link_exists:
         symlink_path.touch()
     else:
-        assert not symlink_path.exists()
+        assert not symlink_path.exists()  # nosec: B101
 
     file = repofile.RepoFile(
         file_type=RepoFileEnum.PACKAGE,
         file_path=default_package_file[0],
         symlink_path=symlink_path,
     )
 
     with expectation:
         file.link(check=check)
-        assert symlink_path.exists()
+        assert symlink_path.exists()  # nosec: B101
 
 
 @mark.parametrize(
     "link_exists, check, expectation",
     [
         (False, True, raises(RepoManagementFileError)),
         (False, False, does_not_raise()),
@@ -256,34 +365,34 @@
     ],
 )
 def test_repofile_unlink(
     link_exists: bool,
     check: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     symlink_path = empty_dir / default_package_file[0].name
     if link_exists:
         symlink_path.touch()
     else:
-        assert not symlink_path.exists()
+        assert not symlink_path.exists()  # nosec: B101
 
     file = repofile.RepoFile(
         file_type=RepoFileEnum.PACKAGE,
         file_path=default_package_file[0],
         symlink_path=symlink_path,
     )
 
     with expectation:
         file.unlink(check=check)
-        assert not symlink_path.exists()
+        assert not symlink_path.exists()  # nosec: B101
 
 
 @mark.parametrize(
     "file_exists, symlink_exists, force, unlink, expectation",
     [
         (True, True, True, True, does_not_raise()),
         (True, True, False, True, does_not_raise()),
@@ -297,15 +406,15 @@
 def test_repofile_remove(
     file_exists: bool,
     symlink_exists: bool,
     force: bool,
     unlink: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
-    default_package_file: Tuple[Path, ...],
+    default_package_file: tuple[Path, ...],
     empty_dir: Path,
 ) -> None:
     caplog.set_level(DEBUG)
 
     file_path = default_package_file[0]
     symlink_path = empty_dir / default_package_file[0].name
 
@@ -319,11 +428,11 @@
         file_type=RepoFileEnum.PACKAGE,
         file_path=file_path,
         symlink_path=symlink_path,
     )
 
     with expectation:
         file.remove(force=force, unlink=unlink)
-        assert not file_path.exists()
+        assert not file_path.exists()  # nosec: B101
 
         if (unlink and symlink_exists) or not symlink_exists:
-            assert not symlink_path.exists()
+            assert not symlink_path.exists()  # nosec: B101
```

### Comparing `repod-0.2.2/tests/repo/package/test_syncdb.py` & `repod-0.3.0.post0/tests/repo/package/test_syncdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+"""Tests for repod.repo.package.syncdb."""
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from logging import DEBUG
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, ContextManager, Dict, List, Optional, Set, Tuple, Union
+from typing import Any, ContextManager
 from unittest.mock import patch
 
 from pytest import LogCaptureFixture, mark, raises
 
 from repod.common.enums import (
     CompressionTypeEnum,
     FilesVersionEnum,
@@ -31,68 +32,71 @@
     create_md5sum,
     create_sha256sum,
     create_url,
 )
 
 
 def test_get_desc_json_name() -> None:
-
-    for identifier in syncdb.DESC_JSON.keys():
+    """Tests for repod.repo.package.syncdb.get_desc_json_name."""
+    for identifier in syncdb.DESC_JSON:
         with does_not_raise():
-            assert syncdb.get_desc_json_name(key=identifier) == syncdb.DESC_JSON[identifier][0]
+            assert syncdb.get_desc_json_name(key=identifier) == syncdb.DESC_JSON[identifier][0]  # nosec: B101
 
     with raises(RepoManagementFileError):
         syncdb.get_desc_json_name(key="%FOO%")
 
 
 def test_get_desc_json_field_type() -> None:
-
-    for identifier in syncdb.DESC_JSON.keys():
+    """Tests for repod.repo.package.syncdb.get_desc_json_field_type."""
+    for identifier in syncdb.DESC_JSON:
         with does_not_raise():
-            assert syncdb.get_desc_json_field_type(key=identifier) == syncdb.DESC_JSON[identifier][1]
+            assert syncdb.get_desc_json_field_type(key=identifier) == syncdb.DESC_JSON[identifier][1]  # nosec: B101
 
     with raises(RepoManagementFileError):
         syncdb.get_desc_json_field_type(key="%FOO%")
 
 
 def test_get_files_json_name() -> None:
-
-    for identifier in syncdb.FILES_JSON.keys():
+    """Tests for repod.repo.package.syncdb.get_files_json_name."""
+    for identifier in syncdb.FILES_JSON:
         with does_not_raise():
-            assert syncdb.get_files_json_name(key=identifier) == syncdb.FILES_JSON[identifier][0]
+            assert syncdb.get_files_json_name(key=identifier) == syncdb.FILES_JSON[identifier][0]  # nosec: B101
 
     with raises(RepoManagementFileError):
         syncdb.get_files_json_name(key="%FOO%")
 
 
 def test_get_files_json_field_type() -> None:
-
-    for identifier in syncdb.FILES_JSON.keys():
+    """Tests for repod.repo.package.syncdb.get_files_json_field_type."""
+    for identifier in syncdb.FILES_JSON:
         with does_not_raise():
-            assert syncdb.get_files_json_field_type(key=identifier) == syncdb.FILES_JSON[identifier][1]
+            assert syncdb.get_files_json_field_type(key=identifier) == syncdb.FILES_JSON[identifier][1]  # nosec: B101
 
     with raises(RepoManagementFileError):
         syncdb.get_files_json_field_type(key="%FOO%")
 
 
 @mark.asyncio
 async def test_files_render(filesv1: syncdb.Files) -> None:
+    """Tests for repod.repo.package.syncdb.FilesV1.render."""
     output = StringIO()
     await filesv1.render(output=output)
-    assert output.getvalue()
+    assert output.getvalue()  # nosec: B101
 
 
 @mark.asyncio
 async def test_files_render_raise_on_missing_template() -> None:
+    """Tests for repod.repo.package.syncdb.FilesV1.render."""
     output = StringIO()
     with raises(RepoManagementFileNotFoundError):
         await FilesV9999().render(output=output)
 
 
 def test_files_get_schema_version() -> None:
+    """Tests for repod.repo.package.syncdb.Files.get_schema_version."""
     model = syncdb.Files()
     with raises(RuntimeError):
         model.get_schema_version()
 
 
 @mark.parametrize(
     "data, expectation",
@@ -111,15 +115,16 @@
         ),
         (
             {"foo": "bar"},
             raises(RepoManagementValidationError),
         ),
     ],
 )
-def test_files_from_dict(data: Dict[str, Any], expectation: ContextManager[str]) -> None:
+def test_files_from_dict(data: dict[str, Any], expectation: ContextManager[str]) -> None:
+    """Tests for repod.repo.package.syncdb.Files.from_dict."""
     with expectation:
         syncdb.Files.from_dict(data=data)
 
 
 @mark.parametrize(
     "data, expectation",
     [
@@ -160,17 +165,20 @@
         "files_v1, unknown keyword",
         "only values",
         "empty",
     ],
 )
 @mark.asyncio
 async def test_files_from_stream(data: str, expectation: ContextManager[str], caplog: LogCaptureFixture) -> None:
+    """Tests for repod.repo.package.syncdb.Files.from_stream."""
     caplog.set_level(DEBUG)
     with expectation:
-        assert await syncdb.Files.from_stream(data=StringIO("\n".join([m.strip() for m in dedent(data).split("\n")])))
+        assert await syncdb.Files.from_stream(  # nosec: B101
+            data=StringIO("\n".join([m.strip() for m in dedent(data).split("\n")]))
+        )
 
 
 @mark.parametrize(
     "files_versions, default_files_version, files_dict, emit_warning, expectation",
     [
         (
             {1: {"required": {"files"}, "optional": {"foo"}}, 2: {"required": {"files"}, "optional": set()}},
@@ -192,21 +200,22 @@
             {"files": ["foo", "bar"], "foo": ["bar"]},
             False,
             does_not_raise(),
         ),
     ],
 )
 def test_files_from_dict_derive_file_version(
-    files_versions: Dict[int, Dict[str, Set[str]]],
+    files_versions: dict[int, dict[str, set[str]]],
     default_files_version: int,
-    files_dict: Dict[str, List[str]],
+    files_dict: dict[str, list[str]],
     emit_warning: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
 ) -> None:
+    """Tests for repod.repo.package.syncdb.Files.from_dict deriving file version."""
     caplog.set_level(DEBUG)
     with expectation:
         with patch("repod.repo.package.syncdb.warning") as logging_warning_mock:
             with patch("repod.repo.package.syncdb.FILES_VERSIONS", files_versions):
                 with patch("repod.repo.package.syncdb.DEFAULT_FILES_VERSION", default_files_version):
                     syncdb.Files.from_dict(data=files_dict)
                     if emit_warning:
@@ -398,21 +407,22 @@
         "default version 2 does not match",
         "default version 1 matches, no pgpsig",
         "default version 2 matches",
         "default version 2 matches, raises ValidationError",
     ],
 )
 def test_package_desc_from_dict_derive_file_version(
-    files_versions: Dict[int, Dict[str, Set[str]]],
+    files_versions: dict[int, dict[str, set[str]]],
     default_version: int,
-    input_dict: Dict[str, Union[int, str, List[str]]],
+    input_dict: dict[str, int | str | list[str]],
     emit_warning: bool,
     expectation: ContextManager[str],
     caplog: LogCaptureFixture,
 ) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.from_dict deriving file version."""
     caplog.set_level(DEBUG)
     with expectation:
         with patch("repod.repo.package.syncdb.warning") as logging_warning_mock:
             with patch("repod.repo.package.syncdb.PACKAGE_DESC_VERSIONS", files_versions):
                 with patch("repod.repo.package.syncdb.DEFAULT_PACKAGE_DESC_VERSION", default_version):
                     syncdb.PackageDesc.from_dict(data=input_dict)
                     if emit_warning:
@@ -893,17 +903,18 @@
         "desc_v1, single invalid field",
         "desc_v1, minimum fields populated, missing %ARCH% field",
         "empty",
     ],
 )
 @mark.asyncio
 async def test_packagedesc_from_stream(data: str, expectation: ContextManager[str], caplog: LogCaptureFixture) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.from_stream."""
     caplog.set_level(DEBUG)
     with expectation:
-        assert await syncdb.PackageDesc.from_stream(
+        assert await syncdb.PackageDesc.from_stream(  # nosec: B101
             data=StringIO("\n".join([m.strip() for m in dedent(data).split("\n")]))
         )
 
 
 @mark.parametrize(
     "no_files, invalid_packagedesc_version, expectation",
     [
@@ -911,33 +922,35 @@
         (True, False, does_not_raise()),
         (True, True, raises(RepoManagementValidationError)),
     ],
 )
 def test_package_desc_v1_get_output_package_v1(
     outputpackagev1: OutputPackage,
     packagedescv1: syncdb.PackageDesc,
-    filesv1: Optional[syncdb.FilesV1],
+    filesv1: syncdb.FilesV1 | None,
     no_files: bool,
     invalid_packagedesc_version: bool,
     expectation: ContextManager[str],
 ) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.get_output_package."""
     output_package = outputpackagev1
     package_desc = packagedescv1
     files = filesv1
     if no_files:
-        output_package.files = None  # type: ignore[attr-defined]
+        output_package.files = None
         files = None
     if invalid_packagedesc_version:
         package_desc = PackageDescV9999()
 
     with expectation:
-        assert output_package == package_desc.get_output_package(files)
+        assert output_package == package_desc.get_output_package(files)  # nosec: B101
 
 
 def test_package_desc_get_output_package_inconsistent_schema_config(packagedescv1: syncdb.PackageDesc) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDescV1.get_output_package with inconsistent schema config."""
     with patch("repod.repo.package.syncdb.PACKAGE_DESC_VERSIONS", {1: {"output_package_version": 9999}}):
         with raises(RuntimeError):
             packagedescv1.get_output_package(files=None)
 
 
 @mark.parametrize(
     "no_files, invalid_package_desc, expectation",
@@ -947,85 +960,94 @@
         (False, True, raises(RepoManagementValidationError)),
         (True, True, raises(RepoManagementValidationError)),
     ],
 )
 def test_package_desc_v1_get_output_package_base_v1(
     outputpackagebasev1: OutputPackageBase,
     packagedescv1: syncdb.PackageDesc,
-    filesv1: Optional[syncdb.Files],
+    filesv1: syncdb.Files | None,
     no_files: bool,
     invalid_package_desc: bool,
     expectation: ContextManager[str],
 ) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDescV1.get_output_package_base."""
     output_package_base = outputpackagebasev1
     package_desc = packagedescv1
     files = filesv1
     # remove all but the first package
     output_package_base.packages = output_package_base.packages[0:1]  # type: ignore[attr-defined]
     # remove buildinfo data (when converting from sync databases we do not have the data available)
-    output_package_base.buildinfo = None  # type: ignore[attr-defined]
+    output_package_base.buildinfo = None
 
     if no_files:
         files = None
         output_package_base.packages[0].files = None  # type: ignore[attr-defined]
     if invalid_package_desc:
         package_desc = PackageDescV9999()
 
     with expectation:
-        assert output_package_base == package_desc.get_output_package_base(files)
+        assert output_package_base == package_desc.get_output_package_base(files)  # nosec: B101
 
 
 def test_package_desc_get_output_package_base_inconsistent_schema_config(
     packagedescv1: syncdb.PackageDesc,
 ) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDescV1.get_output_package_base with inconsistent schema config."""
     with patch("repod.repo.package.syncdb.PACKAGE_DESC_VERSIONS", {1: {"output_package_base_version": 9999}}):
         with raises(RuntimeError):
             packagedescv1.get_output_package_base(files=None)
 
 
 @mark.asyncio
 async def test_packagedesc_render(packagedescv1: syncdb.PackageDesc) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDescV1.render."""
     output = StringIO()
     await packagedescv1.render(output=output)
-    assert output.getvalue()
+    assert output.getvalue()  # nosec: B101
 
 
 @mark.asyncio
 async def test_packagedesc_render_raise_on_missing_template() -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.render raising Exception."""
     output = StringIO()
     with raises(RepoManagementFileNotFoundError):
         await PackageDescV9999().render(output=output)
 
 
 def test_packagedesc_get_base() -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.get_base."""
     model = syncdb.PackageDesc()
     with raises(RuntimeError):
         model.get_base()
 
 
 def test_packagedesc_get_name() -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.get_name."""
     model = syncdb.PackageDesc()
     with raises(RuntimeError):
         model.get_name()
 
 
 def test_packagedesc_get_schema_version() -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.get_schema_version."""
     model = syncdb.PackageDesc()
     with raises(RuntimeError):
         model.get_schema_version()
 
 
 def test_packagedesc_get_output_package() -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.get_output_package."""
     files = syncdb.FilesV1(files=["foo", "bar", "baz"])
     model = syncdb.PackageDesc()
     with raises(RuntimeError):
         model.get_output_package(files=files)
 
 
 def test_packagedesc_get_output_package_base() -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.get_output_package_base."""
     files = syncdb.FilesV1(files=["foo", "bar", "baz"])
     model = syncdb.PackageDesc()
     with raises(RuntimeError):
         model.get_output_package_base(files=files)
 
 
 @mark.parametrize(
@@ -1094,20 +1116,22 @@
     ],
     ids=[
         "default",
         "version missing",
         "invalid key-value pair",
     ],
 )
-def test_packagedesc_from_dict(data: Dict[str, Union[int, str, List[str]]], expectation: ContextManager[str]) -> None:
+def test_packagedesc_from_dict(data: dict[str, int | str | list[str]], expectation: ContextManager[str]) -> None:
+    """Tests for repod.repo.package.syncdb.PackageDesc.from_dict."""
     with expectation:
         syncdb.PackageDesc.from_dict(data=data)
 
 
 def test_export_schemas(tmp_path: Path) -> None:
+    """Tests for repod.repo.package.syncdb.export_schemas."""
     syncdb.export_schemas(output=str(tmp_path))
     syncdb.export_schemas(output=tmp_path)
 
     with raises(RuntimeError):
         syncdb.export_schemas(output="/foobar")
 
     with raises(RuntimeError):
@@ -1118,34 +1142,36 @@
 @mark.asyncio
 async def test_syncdatabase_outputpackagebase_to_tarfile(
     caplog: LogCaptureFixture,
     database_type: syncdb.RepoDbTypeEnum,
     tmp_path: Path,
     outputpackagebasev1: OutputPackageBase,
 ) -> None:
+    """Tests for repod.repo.package.syncdb.SyncDatabase.outputpackagebase_to_tarfile."""
     caplog.set_level(DEBUG)
     database = tmp_path / "tarfile"
     with open_tarfile(path=database, mode="w", compression=CompressionTypeEnum.GZIP) as tar_file:
         await syncdb.SyncDatabase.outputpackagebase_to_tarfile(
             tarfile=tar_file,
-            database_type=syncdb.RepoDbTypeEnum.DEFAULT,
+            database_type=database_type,
             model=outputpackagebasev1,
             packagedesc_version=PackageDescVersionEnum.DEFAULT,
             files_version=FilesVersionEnum.DEFAULT,
         )
 
 
 @mark.parametrize("database_type", [(syncdb.RepoDbTypeEnum.DEFAULT), (syncdb.RepoDbTypeEnum.FILES)])
 @mark.asyncio
 async def test_syncdatabase_add(
     caplog: LogCaptureFixture,
     database_type: syncdb.RepoDbTypeEnum,
-    default_sync_db_file: Tuple[Path, Path],
+    default_sync_db_file: tuple[Path, Path],
     outputpackagebasev1: OutputPackageBase,
 ) -> None:
+    """Tests for repod.repo.package.syncdb.SyncDatabase.add."""
     caplog.set_level(DEBUG)
     await syncdb.SyncDatabase(
         database=default_sync_db_file[0],
         database_type=database_type,
         compression_type=compression_type_of_tarfile(default_sync_db_file[0]),
         desc_version=PackageDescVersionEnum.DEFAULT,
         files_version=FilesVersionEnum.DEFAULT,
@@ -1153,48 +1179,50 @@
 
 
 @mark.parametrize("database_type", [(syncdb.RepoDbTypeEnum.DEFAULT), (syncdb.RepoDbTypeEnum.FILES)])
 @mark.asyncio
 async def test_syncdatabase_stream_management_repo(
     caplog: LogCaptureFixture,
     database_type: syncdb.RepoDbTypeEnum,
-    default_sync_db_file: Tuple[Path, Path],
+    default_sync_db_file: tuple[Path, Path],
     outputpackagebasev1_json_files_in_dir: Path,
 ) -> None:
+    """Tests for repod.repo.package.syncdb.SyncDatabase.stream_management_repo."""
     caplog.set_level(DEBUG)
     await syncdb.SyncDatabase(
         database=default_sync_db_file[0],
         database_type=database_type,
         compression_type=compression_type_of_tarfile(default_sync_db_file[0]),
         desc_version=PackageDescVersionEnum.DEFAULT,
         files_version=FilesVersionEnum.DEFAULT,
     ).stream_management_repo(path=outputpackagebasev1_json_files_in_dir)
 
 
 @mark.parametrize("database_type", [(syncdb.RepoDbTypeEnum.DEFAULT), (syncdb.RepoDbTypeEnum.FILES)])
 @mark.asyncio
-async def test_syncdatabase_stream_management_repo_raises_on_empty_dir(
+async def test_syncdatabase_stream_management_repo_empty_dir(
     caplog: LogCaptureFixture,
     database_type: syncdb.RepoDbTypeEnum,
-    default_sync_db_file: Tuple[Path, Path],
+    default_sync_db_file: tuple[Path, Path],
     tmp_path: Path,
 ) -> None:
+    """Tests for repod.repo.package.syncdb.SyncDatabase.stream_management_repo from empty directory."""
     caplog.set_level(DEBUG)
-    with raises(RepoManagementFileNotFoundError):
-        await syncdb.SyncDatabase(
-            database=default_sync_db_file[0],
-            database_type=database_type,
-            compression_type=compression_type_of_tarfile(default_sync_db_file[0]),
-            desc_version=PackageDescVersionEnum.DEFAULT,
-            files_version=FilesVersionEnum.DEFAULT,
-        ).stream_management_repo(path=tmp_path)
+    await syncdb.SyncDatabase(
+        database=default_sync_db_file[0],
+        database_type=database_type,
+        compression_type=compression_type_of_tarfile(default_sync_db_file[0]),
+        desc_version=PackageDescVersionEnum.DEFAULT,
+        files_version=FilesVersionEnum.DEFAULT,
+    ).stream_management_repo(path=tmp_path)
 
 
 @mark.asyncio
-async def test_syncdatabase_outputpackagebases(files_sync_db_file: Tuple[Path, Path]) -> None:
-    for (name, model) in await syncdb.SyncDatabase(
+async def test_syncdatabase_outputpackagebases(files_sync_db_file: tuple[Path, Path]) -> None:
+    """Tests for repod.repo.package.syncdb.SyncDatabase.outputpackagebases."""
+    for name, model in await syncdb.SyncDatabase(
         database=files_sync_db_file[0],
         desc_version=PackageDescVersionEnum.DEFAULT,
         files_version=FilesVersionEnum.DEFAULT,
     ).outputpackagebases():
-        assert isinstance(name, str)
-        assert isinstance(model, OutputPackageBase)
+        assert isinstance(name, str)  # nosec: B101
+        assert isinstance(model, OutputPackageBase)  # nosec: B101
```

### Comparing `repod-0.2.2/tests/test_commands.py` & `repod-0.3.0.post0/tests/test_commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+"""Tests for repod.commands."""
 from contextlib import nullcontext as does_not_raise
 from pathlib import Path
-from subprocess import CalledProcessError
-from typing import ContextManager, Dict, List, Optional, Union
+from subprocess import CalledProcessError  # nosec: B404
+from typing import ContextManager
 
 from pytest import mark, raises
 
 from repod import commands
 
 
 @mark.parametrize("env", [(None), ({"FOO": "BAR"})])
-def test__print_env(env: Optional[Dict[str, str]]) -> None:
+def test__print_env(env: dict[str, str] | None) -> None:
+    """Tests for repod.commands._print_env."""
     commands._print_env(env)
 
 
 @mark.parametrize(
     "cmd, env, debug, echo, quiet, check, cwd, expectation",
     [
         (["ls", "-lah"], {"FOO": "BAR"}, False, False, False, False, None, does_not_raise()),
         (["ls", "-lah"], {"FOO": "BAR"}, True, False, False, False, None, does_not_raise()),
         (["cd", "-f"], {"FOO": "BAR"}, True, False, False, True, None, raises(CalledProcessError)),
     ],
 )
 @mark.asyncio
 def test_run_command(
-    cmd: Union[str, List[str]],
-    env: Optional[Dict[str, str]],
+    cmd: str | list[str],
+    env: dict[str, str] | None,
     debug: bool,
     echo: bool,
     quiet: bool,
     check: bool,
-    cwd: Union[Optional[str], Optional[Path]],
+    cwd: str | Path | None,
     expectation: ContextManager[str],
 ) -> None:
+    """Tests for repod.commands.run_command."""
     with expectation:
         commands.run_command(cmd=cmd, env=env, debug=debug, echo=echo, quiet=quiet, check=check, cwd=cwd)
```

### Comparing `repod-0.2.2/tests/verification/test_pgp.py` & `repod-0.3.0.post0/tests/verification/test_pgp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Tests for repod.verification.pgp."""
 from logging import DEBUG
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
 from unittest.mock import Mock, patch
 
 from pytest import LogCaptureFixture, mark
@@ -11,35 +12,37 @@
 
 
 @mark.parametrize("verifies, result", [(True, True), (False, False)])
 @patch("repod.verification.pgp.run_command")
 def test_pacmankeyverifier_verify(
     run_command_mock: Mock, caplog: LogCaptureFixture, verifies: bool, result: bool
 ) -> None:
+    """Tests for repod.verification.pgp.Pacmankeyverifier.verify."""
     caplog.set_level(DEBUG)
     package = Path("package")
     signature = Path("signature")
     error_message = "error_message"
     result_mock = Mock()
     result_mock.returncode = 0 if verifies else 1
     result_mock.stderr = error_message
     run_command_mock.return_value = result_mock
     print(result_mock)
 
     verifier = pgp.PacmanKeyVerifier()
-    assert verifier.verify(package=package, signature=signature) is result
+    assert verifier.verify(package=package, signature=signature) is result  # nosec: B101
 
 
 @mark.integration
 @mark.xfail(reason="May fail on packages with old signatures in a system's pacman cache.")
 @mark.skipif(
     not Path("/var/cache/pacman/pkg/").exists(),
     reason="Package cache in /var/cache/pacman/pkg/ does not exist",
 )
 def test_pacmankeyverifier_verify_with_packages(caplog: LogCaptureFixture) -> None:
+    """Integration tests for repod.verification.pgp.Pacmankeyverifier.verify."""
     caplog.set_level(DEBUG)
     verifier = pgp.PacmanKeyVerifier()
 
     signatures = sorted(
         [
             path
             for path in list(Path("/var/cache/pacman/pkg/").iterdir())
@@ -48,14 +51,14 @@
                 Match,
             )
         ]
     )
     if len(signatures) > 50:
         signatures = sample(signatures, 50)
     for signature in signatures:
-        assert (
+        assert (  # nosec: B101
             verifier.verify(
                 package=Path(str(signature).replace(".sig", "")),
                 signature=signature,
             )
             is True
         )
```

### Comparing `repod-0.2.2/tests/version/test_alpm.py` & `repod-0.3.0.post0/tests/version/test_alpm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Tests for repod.version.alpm."""
 from unittest.mock import patch
 
 from pytest import mark
 from pytest_lazyfixture import lazy_fixture
 
 from repod.version.alpm import pkg_vercmp, vercmp
 
@@ -55,23 +56,25 @@
         ("", "", 0),
         ("", "1", -1),
         ("", "a", 1),
     ],
 )
 @mark.parametrize("pyalpm_vercmp", [lazy_fixture("pyalpm_vercmp_fun")])
 def test_vercmp(first: str, second: str, expectation: int, pyalpm_vercmp: bool) -> None:
+    """Tests for repod.version.alpm.vercmp."""
     with patch("repod.version.alpm.PYALPM_VERCMP", pyalpm_vercmp):
-        assert vercmp(a=first, b=second) == expectation
+        assert vercmp(a=first, b=second) == expectation  # nosec: B101
 
 
 @mark.parametrize(
     "first, second, expectation",
     [
         ("1-2", "1-2", 0),
         ("1:2-3", "2-3", 1),
         ("1:2-3", "1:2-4", -1),
     ],
 )
 @mark.parametrize("pyalpm_vercmp", [lazy_fixture("pyalpm_vercmp_fun")])
 def test_pkgver_vercmp(first: str, second: str, expectation: int, pyalpm_vercmp: bool) -> None:
+    """Tests for repod.version.alpm.pkg_vercmp."""
     with patch("repod.version.alpm.PYALPM_VERCMP", pyalpm_vercmp):
-        assert pkg_vercmp(a=first, b=second) == expectation
+        assert pkg_vercmp(a=first, b=second) == expectation  # nosec: B101
```

### Comparing `repod-0.2.2/PKG-INFO` & `repod-0.3.0.post0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,91 @@
 Metadata-Version: 2.1
 Name: repod
-Version: 0.2.2
+Version: 0.3.0.post0
 Summary: Tooling to maintain binary package repositories for Linux distributions using the pacman package manager
+Keywords: arch linux repository pacman packages
 Home-page: https://gitlab.archlinux.org/archlinux/repod
+Author-Email: Arch Linux <arch-projects@lists.archlinux.org>
 License: GPL-3.0-or-later
-Keywords: arch linux,repository,pacman,packages
-Author: Arch Linux
-Author-email: arch-projects@lists.archlinux.org
-Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Internet
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Provides-Extra: vercmp
-Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
-Requires-Dist: aiofiles (>=0.8.0,<0.9.0)
-Requires-Dist: email-validator (>=1.2.1,<2.0.0)
-Requires-Dist: orjson (>=3.6.6,<4.0.0)
-Requires-Dist: pyalpm[vercmp] (>=0.10.6,<0.11.0); extra == "vercmp"
-Requires-Dist: pydantic (>=1.8.1,<2.0.0)
-Requires-Dist: python-magic (>=0.4.26,<0.5.0)
-Requires-Dist: pyxdg (>=0.28,<0.29)
-Requires-Dist: pyzstd (>=0.15.2,<0.16.0)
-Requires-Dist: subprocess-tee (>=0.3.5,<0.4.0)
-Requires-Dist: tomli (>=2.0.0,<3.0.0)
-Project-URL: Bug Tracker, https://gitlab.archlinux.org/archlinux/repod/-/issues/
-Project-URL: Documentation, https://repod.archlinux.page
+Project-URL: Bug tracker, https://gitlab.archlinux.org/archlinux/repod/-/issues/
+Project-URL: Homepage, https://gitlab.archlinux.org/archlinux/repod
 Project-URL: Repository, https://gitlab.archlinux.org/archlinux/repod
+Project-URL: Documentation, https://repod.archlinux.page
+Requires-Python: <4.0,>=3.10
+Requires-Dist: aiofiles>=23.1.0
+Requires-Dist: email-validator>=2.0.0
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: orjson>=3.9.2
+Requires-Dist: pydantic>=2.0
+Requires-Dist: pydantic-settings>=2.0.2
+Requires-Dist: python-magic>=0.4.27
+Requires-Dist: pyxdg>=0.28
+Requires-Dist: pyzstd>=0.15.7
+Requires-Dist: subprocess-tee>=0.4.1
+Requires-Dist: tomli>=2.0.1; python_version < "3.11"
+Requires-Dist: pyalpm<1.0.0,>=0.10.6; extra == "alt-vercmp"
+Requires-Dist: file-magic<1.0.0,>=0.4.0; extra == "alt-file"
+Provides-Extra: alt_vercmp
+Provides-Extra: alt_file
 Description-Content-Type: text/markdown
 
 # repod
 This project contains tooling to maintain binary package repositories for Linux
 distributions using the [pacman](https://archlinux.org/pacman/) package manager.
 
 The latest documentation can be found at
 [repod.archlinux.page](https://repod.archlinux.page).
 
 **NOTE**: *Repod is still alpha grade software and as such has not yet reached
-its targetted feature set and has not been thoroughly tested in the field. It
-should not be used in a production environment!*
+its targeted feature set. It has not been thoroughly tested in the field and
+therefore should not be used in a production environment!*
 
 ## Installation
 
-You can install the latest released version of repod by executing
+You can install repod using your distribution's package manager or
+alternatively by executing
 
 ```
 pip install repod
 ```
 
-## Requirements
-
-When installing repod, its dependencies are automatically installed.
-
-However, the project has a few special dependencies which can be replaced by
-other packages, depending on availability.
-
-### Pyalpm
-
-The Python package [pyalpm](https://pypi.org/project/pyalpm/) is not
-installable on all operating systems as it depends on the availability of
-[libalpm](https://man.archlinux.org/man/libalpm.3) (a C library), which is
-usually provided via [pacman](https://man.archlinux.org/man/pacman.8).
-
-However, if `pyalpm` is detected, repod will make use of it for version
-comparison instead of a builtin implementation of this functionality, which is
-based on [vercmp](https://man.archlinux.org/man/vercmp.8).
-
-### Python-magic
-
-By default the [python-magic](https://pypi.org/project/python-magic/) Python
-package is used by repod to detect file types. The detection is based on
-`libmagic` (a C library), usually provided via
-[file](https://darwinsys.com/file/).
-
-Confusingly, the file project also offers a Python module called `file-magic`,
-but it is not available on pypi.org and mostly only found on e.g. Linux
-distributions.
-
-If file's `file-magic` Python module is detected, repod will make use of it for
-file type detection instead of using `python-magic`.
+Further information on optional requirements and setting up a development
+environment can be found in the official [installation
+instructions](https://repod.archlinux.page/repod/installation.html).
+
+## Usage
+
+Please refer to the [usage
+information](https://repod.archlinux.page/repod/usage.html) in the official
+documentation to learn how to use repod.
 
 ## Contributing
 
-Read our [contributing guide](CONTRIBUTING.md) to learn more about how to
-provide fixes or improvements for the code and documentation.
+Read our [contributing guide](https://repod.archlinux.page/contributing.html)
+to learn more about how to provide fixes or improvements for the code and
+documentation.
 
 ## License
 
-Repod's code is licensed under the terms of the **GPL-3.0-or-later** (see
-[LICENSE](LICENSE)) and its documentation is licensed under the terms of the
-**GFDL-1.3-or-later** (see [docs/LICENSE](docs/LICENSE)).
-
+Repod's code is licensed under the terms of the **GPL-3.0-or-later** (see the
+top-level *LICENSE* file), its documentation is licensed under the terms of the
+**GFDL-1.3-or-later** (see the *docs/LICENSE* file) and its artwork (created by
+Safi @ [betriebsbuero](http://betriebsbuero.com)) is licensed under the terms
+of the **CC-BY-SA-4.0** (see the *docs/artwork/LICENSE* file).
```

