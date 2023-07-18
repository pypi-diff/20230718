# Comparing `tmp/Pokie-0.4.4.tar.gz` & `tmp/Pokie-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pokie-0.4.4.tar", last modified: Mon Jul 17 17:11:27 2023, max compression
+gzip compressed data, was "Pokie-0.4.5.tar", last modified: Tue Jul 18 00:07:15 2023, max compression
```

## Comparing `Pokie-0.4.4.tar` & `Pokie-0.4.5.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 17:10:55.000000 Pokie-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 17:10:55.000000 Pokie-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 17:11:27.965400 Pokie-0.4.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/Pokie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 17:11:27.000000 Pokie-0.4.4/Pokie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-17 17:10:55.000000 Pokie-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/codegen/pg/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/pg/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/codegen/textfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/config/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/cli/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/dto/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/dto/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/plugin/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.957400 Pokie-0.4.4/pokie/contrib/auth/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/repository/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/repository/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/auth/service/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/service/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/auth/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/sql/001-auth-schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/auth/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/auth/view/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/db_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/cli/tpl_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/dto/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/job/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/job/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/repository/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/service/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/autorest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/service/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/sql/001-settings.sql
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/sql/002-fixtures.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/base/validators/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/base/validators/pk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.961400 Pokie-0.4.4/pokie/contrib/mail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/cli/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/dto/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/job/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/job/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/repository/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/service/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/service/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/service/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/contrib/mail/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/contrib/mail/sql/001-mail.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/core/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/core/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/pgsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/factories/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/core/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/http/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/http/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/plugins/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/rest/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/rest/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/pokie/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 17:10:55.000000 Pokie-0.4.4/pokie/util/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-17 17:11:27.965400 Pokie-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 17:10:55.000000 Pokie-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:11:27.965400 Pokie-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:10:55.000000 Pokie-0.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.371698 Pokie-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-18 00:06:34.000000 Pokie-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-18 00:06:34.000000 Pokie-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-18 00:07:15.371698 Pokie-0.4.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.355697 Pokie-0.4.5/Pokie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-18 00:07:15.000000 Pokie-0.4.5/Pokie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-18 00:07:15.000000 Pokie-0.4.5/Pokie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:07:15.000000 Pokie-0.4.5/Pokie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:07:15.000000 Pokie-0.4.5/Pokie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-18 00:07:15.000000 Pokie-0.4.5/Pokie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 00:07:15.000000 Pokie-0.4.5/Pokie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-18 00:06:34.000000 Pokie-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.355697 Pokie-0.4.5/pokie/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.355697 Pokie-0.4.5/pokie/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/codegen/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/pg/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/pg/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/pg/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/codegen/textfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/config/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/cli/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/dto/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/dto/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/plugin/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/repository/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/repository/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/service/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/service/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/service/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/sql/001-auth-schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/auth/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/auth/view/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.359697 Pokie-0.4.5/pokie/contrib/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.363698 Pokie-0.4.5/pokie/contrib/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/db_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/cli/tpl_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.363698 Pokie-0.4.5/pokie/contrib/base/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/dto/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.363698 Pokie-0.4.5/pokie/contrib/base/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/job/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.363698 Pokie-0.4.5/pokie/contrib/base/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/repository/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/repository/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/repository/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.363698 Pokie-0.4.5/pokie/contrib/base/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/service/autorest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/service/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/service/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/service/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.363698 Pokie-0.4.5/pokie/contrib/base/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/sql/001-settings.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/sql/002-fixtures.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/base/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/base/validators/pk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/mail/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/cli/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/mail/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/dto/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/mail/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/job/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/mail/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/repository/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/mail/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/service/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/service/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/contrib/mail/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/contrib/mail/sql/001-mail.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.367698 Pokie-0.4.5/pokie/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.371698 Pokie-0.4.5/pokie/core/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/factories/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/factories/pgsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/factories/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/core/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.371698 Pokie-0.4.5/pokie/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/http/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/http/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/http/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/http/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/http/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.371698 Pokie-0.4.5/pokie/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/plugins/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.371698 Pokie-0.4.5/pokie/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/rest/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/rest/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.371698 Pokie-0.4.5/pokie/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 00:06:34.000000 Pokie-0.4.5/pokie/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-18 00:07:15.371698 Pokie-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 00:06:34.000000 Pokie-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:07:15.371698 Pokie-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:06:34.000000 Pokie-0.4.5/tests/__init__.py
```

### Comparing `Pokie-0.4.4/LICENSE` & `Pokie-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/PKG-INFO` & `Pokie-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.4
+Version: 0.4.5
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.4/Pokie.egg-info/PKG-INFO` & `Pokie-0.4.5/Pokie.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.4
+Version: 0.4.5
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.4/Pokie.egg-info/SOURCES.txt` & `Pokie-0.4.5/Pokie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/README.md` & `Pokie-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/codegen/pg/record.py` & `Pokie-0.4.5/pokie/codegen/pg/record.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/codegen/pg/request.py` & `Pokie-0.4.5/pokie/codegen/pg/request.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/codegen/pg/spec.py` & `Pokie-0.4.5/pokie/codegen/pg/spec.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/codegen/template.py` & `Pokie-0.4.5/pokie/codegen/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/codegen/textfile.py` & `Pokie-0.4.5/pokie/codegen/textfile.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/config/template.py` & `Pokie-0.4.5/pokie/config/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/constants.py` & `Pokie-0.4.5/pokie/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version
-POKIE_VERSION = ["0", "4", "4"]
+POKIE_VERSION = ["0", "4", "5"]
 
 
 def get_version():
     return ".".join(POKIE_VERSION)
 
 
 # Http Codes
```

### Comparing `Pokie-0.4.4/pokie/contrib/auth/cli/acl.py` & `Pokie-0.4.5/pokie/contrib/auth/cli/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/cli/user.py` & `Pokie-0.4.5/pokie/contrib/auth/cli/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/dto/acl.py` & `Pokie-0.4.5/pokie/contrib/auth/dto/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/module.py` & `Pokie-0.4.5/pokie/contrib/auth/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/plugin/db.py` & `Pokie-0.4.5/pokie/contrib/auth/plugin/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/repository/acl.py` & `Pokie-0.4.5/pokie/contrib/auth/repository/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/repository/user.py` & `Pokie-0.4.5/pokie/contrib/auth/repository/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/service/acl.py` & `Pokie-0.4.5/pokie/contrib/auth/service/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/service/auth.py` & `Pokie-0.4.5/pokie/contrib/auth/service/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/service/user.py` & `Pokie-0.4.5/pokie/contrib/auth/service/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/sql/001-auth-schema.sql` & `Pokie-0.4.5/pokie/contrib/auth/sql/001-auth-schema.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/auth/view/account.py` & `Pokie-0.4.5/pokie/contrib/auth/view/account.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/cli/base.py` & `Pokie-0.4.5/pokie/contrib/base/cli/base.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/cli/db.py` & `Pokie-0.4.5/pokie/contrib/base/cli/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/cli/db_codegen.py` & `Pokie-0.4.5/pokie/contrib/base/cli/db_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/cli/fixture.py` & `Pokie-0.4.5/pokie/contrib/base/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/cli/job.py` & `Pokie-0.4.5/pokie/contrib/base/cli/job.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/cli/tpl_codegen.py` & `Pokie-0.4.5/pokie/contrib/base/cli/tpl_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/module.py` & `Pokie-0.4.5/pokie/contrib/base/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/repository/settings.py` & `Pokie-0.4.5/pokie/contrib/base/repository/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/repository/validator.py` & `Pokie-0.4.5/pokie/contrib/base/repository/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/service/autorest.py` & `Pokie-0.4.5/pokie/contrib/base/service/autorest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/service/fixture.py` & `Pokie-0.4.5/pokie/contrib/base/service/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/service/settings.py` & `Pokie-0.4.5/pokie/contrib/base/service/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/service/validator.py` & `Pokie-0.4.5/pokie/contrib/base/service/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/base/validators/pk.py` & `Pokie-0.4.5/pokie/contrib/base/validators/pk.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/cli/queue.py` & `Pokie-0.4.5/pokie/contrib/mail/cli/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/dto/records.py` & `Pokie-0.4.5/pokie/contrib/mail/dto/records.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/helpers.py` & `Pokie-0.4.5/pokie/contrib/mail/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/job/queue.py` & `Pokie-0.4.5/pokie/contrib/mail/job/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/module.py` & `Pokie-0.4.5/pokie/contrib/mail/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/repository/repositories.py` & `Pokie-0.4.5/pokie/contrib/mail/repository/repositories.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/service/queue.py` & `Pokie-0.4.5/pokie/contrib/mail/service/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/service/template.py` & `Pokie-0.4.5/pokie/contrib/mail/service/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/contrib/mail/sql/001-mail.sql` & `Pokie-0.4.5/pokie/contrib/mail/sql/001-mail.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/core/application.py` & `Pokie-0.4.5/pokie/core/application.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/core/command.py` & `Pokie-0.4.5/pokie/core/command.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/core/factories/login.py` & `Pokie-0.4.5/pokie/core/factories/login.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/core/factories/pgsql.py` & `Pokie-0.4.5/pokie/core/factories/pgsql.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/core/factories/redis.py` & `Pokie-0.4.5/pokie/core/factories/redis.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/core/signal.py` & `Pokie-0.4.5/pokie/core/signal.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/http/helpers.py` & `Pokie-0.4.5/pokie/http/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/http/http_error.py` & `Pokie-0.4.5/pokie/http/http_error.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/http/response.py` & `Pokie-0.4.5/pokie/http/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ):
         pass
 
     def assemble(self, _app, **kwargs):
         pass
 
 
-class JsonResponse(ResponseRenderer):
+class JsonResponse(ResponseRendererInterface):
     """
     Default JSON response formatter
 
     The usual JSON response has the following format:
 
     success is True:
     {
```

### Comparing `Pokie-0.4.4/pokie/http/rest.py` & `Pokie-0.4.5/pokie/http/rest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/http/routes.py` & `Pokie-0.4.5/pokie/http/routes.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/http/view.py` & `Pokie-0.4.5/pokie/http/view.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/plugins/auth.py` & `Pokie-0.4.5/pokie/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/rest/mixin.py` & `Pokie-0.4.5/pokie/rest/mixin.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/rest/service.py` & `Pokie-0.4.5/pokie/rest/service.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/pokie/util/cli_args.py` & `Pokie-0.4.5/pokie/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.4/setup.cfg` & `Pokie-0.4.5/setup.cfg`

 * *Files identical despite different names*

