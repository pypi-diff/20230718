# Comparing `tmp/educommon-2.19.3.tar.gz` & `tmp/educommon-2.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educommon-2.19.3.tar", last modified: Tue Nov 15 11:33:40 2022, max compression
+gzip compressed data, was "educommon-2.20.0.tar", last modified: Tue Jul 18 06:09:32 2023, max compression
```

## Comparing `educommon-2.19.3.tar` & `educommon-2.20.0.tar`

### file list

```diff
@@ -1,401 +1,427 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.574709 educommon-2.19.3/
--rw-r--r--   0 root         (0) root         (0)   109351 2022-11-15 11:33:28.000000 educommon-2.19.3/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)      102 2022-07-05 14:23:59.000000 educommon-2.19.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1058 2022-11-15 11:33:40.574709 educommon-2.19.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2022-07-05 14:23:59.000000 educommon-2.19.3/README.rst
--rw-r--r--   0 root         (0) root         (0)     1981 2022-07-05 14:23:59.000000 educommon-2.19.3/UPGRADE.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-15 11:33:40.574709 educommon-2.19.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2466 2022-07-05 14:23:59.000000 educommon-2.19.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.350709 educommon-2.19.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.362709 educommon-2.19.3/src/educommon/
--rw-r--r--   0 root         (0) root         (0)      475 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.368709 educommon-2.19.3/src/educommon/about/
--rw-r--r--   0 root         (0) root         (0)     2685 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/README.rst
--rw-r--r--   0 root         (0) root         (0)      149 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.350709 educommon-2.19.3/src/educommon/about/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.369709 educommon-2.19.3/src/educommon/about/static/edu_about/
--rw-r--r--   0 root         (0) root         (0)     8382 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/static/edu_about/barsgroup.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.372709 educommon-2.19.3/src/educommon/about/ui/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/ui/about-window.js
--rw-r--r--   0 root         (0) root         (0)     6090 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/ui/actions.py
--rw-r--r--   0 root         (0) root         (0)      700 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/ui/common-tab.html
--rw-r--r--   0 root         (0) root         (0)    11192 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/ui/packages-tab.js
--rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/ui/postgresql-extensions-tab.js
--rw-r--r--   0 root         (0) root         (0)     5381 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/ui/ui.py
--rw-r--r--   0 root         (0) root         (0)      718 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/about/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.377709 educommon-2.19.3/src/educommon/async_tasks/
--rw-r--r--   0 root         (0) root         (0)      166 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      146 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/apps.py
--rw-r--r--   0 root         (0) root         (0)      267 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.377709 educommon-2.19.3/src/educommon/async_tasks/fixtures/
--rw-r--r--   0 root         (0) root         (0)      303 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/fixtures/initial_data.json
--rw-r--r--   0 root         (0) root         (0)     3468 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/locks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.380709 educommon-2.19.3/src/educommon/async_tasks/migrations/
--rw-r--r--   0 root         (0) root         (0)     4309 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/migrations/0002_load_initial_data.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3618 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/models.py
--rw-r--r--   0 root         (0) root         (0)     1487 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/statuses.py
--rw-r--r--   0 root         (0) root         (0)    11236 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/async_tasks/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.385709 educommon-2.19.3/src/educommon/audit_log/
--rw-r--r--   0 root         (0) root         (0)     2829 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5924 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/actions.py
--rw-r--r--   0 root         (0) root         (0)      302 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     4994 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/apps.py
--rw-r--r--   0 root         (0) root         (0)      936 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.386709 educommon-2.19.3/src/educommon/audit_log/error_log/
--rw-r--r--   0 root         (0) root         (0)      153 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/error_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2310 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/error_log/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.387709 educommon-2.19.3/src/educommon/audit_log/management/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.387709 educommon-2.19.3/src/educommon/audit_log/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1813 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/management/commands/reinstall_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1187 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.395709 educommon-2.19.3/src/educommon/audit_log/migrations/
--rw-r--r--   0 root         (0) root         (0)     4547 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     2907 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/migrations/0002_install_audit_log.py
--rw-r--r--   0 root         (0) root         (0)      492 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/migrations/0003_logproxy.py
--rw-r--r--   0 root         (0) root         (0)      342 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
--rw-r--r--   0 root         (0) root         (0)      769 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/migrations/0005_postgresql_error.py
--rw-r--r--   0 root         (0) root         (0)      669 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
--rw-r--r--   0 root         (0) root         (0)     1472 2022-07-08 03:53:12.000000 educommon-2.19.3/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8272 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/models.py
--rw-r--r--   0 root         (0) root         (0)     1307 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/permissions.py
--rw-r--r--   0 root         (0) root         (0)     8820 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/proxies.py
--rw-r--r--   0 root         (0) root         (0)      251 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/routers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.397709 educommon-2.19.3/src/educommon/audit_log/sql/
--rw-r--r--   0 root         (0) root         (0)     1395 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/sql/configure_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)      431 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/sql/configure_selective_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)     1841 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/sql/create_selective_tables_function.sql
--rw-r--r--   0 root         (0) root         (0)    14310 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/sql/install_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)     2137 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.399709 educommon-2.19.3/src/educommon/audit_log/utils/
--rw-r--r--   0 root         (0) root         (0)    12583 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/audit_log/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/audit_log/utils/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.399709 educommon-2.19.3/src/educommon/auth/
--rw-r--r--   0 root         (0) root         (0)      135 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.406709 educommon-2.19.3/src/educommon/auth/rbac/
--rw-r--r--   0 root         (0) root         (0)      378 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27149 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/actions.py
--rw-r--r--   0 root         (0) root         (0)      473 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/app_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.409709 educommon-2.19.3/src/educommon/auth/rbac/backends/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3082 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/backends/base.py
--rw-r--r--   0 root         (0) root         (0)    10328 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/backends/caching.py
--rw-r--r--   0 root         (0) root         (0)     5066 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/backends/simple.py
--rw-r--r--   0 root         (0) root         (0)     3016 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/checker.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/config.py
--rw-r--r--   0 root         (0) root         (0)      562 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.410709 educommon-2.19.3/src/educommon/auth/rbac/management/
--rw-r--r--   0 root         (0) root         (0)      127 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.411709 educommon-2.19.3/src/educommon/auth/rbac/management/commands/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5551 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/management/commands/rbac.py
--rw-r--r--   0 root         (0) root         (0)    16332 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.413709 educommon-2.19.3/src/educommon/auth/rbac/migrations/
--rw-r--r--   0 root         (0) root         (0)     5578 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      681 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
--rw-r--r--   0 root         (0) root         (0)      574 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
--rw-r--r--   0 root         (0) root         (0)     2181 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15466 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/models.py
--rw-r--r--   0 root         (0) root         (0)      927 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.352709 educommon-2.19.3/src/educommon/auth/rbac/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.416709 educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/
--rw-r--r--   0 root         (0) root         (0)      335 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/role-add-window.js
--rw-r--r--   0 root         (0) root         (0)     7914 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
--rw-r--r--   0 root         (0) root         (0)     3768 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
--rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
--rw-r--r--   0 root         (0) root         (0)    15794 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/ui.py
--rw-r--r--   0 root         (0) root         (0)     7929 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/utils.py
--rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/rbac/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.421709 educommon-2.19.3/src/educommon/auth/simple_auth/
--rw-r--r--   0 root         (0) root         (0)      289 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11903 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/actions.py
--rw-r--r--   0 root         (0) root         (0)     1112 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     2587 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/checkers.py
--rw-r--r--   0 root         (0) root         (0)      453 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.421709 educommon-2.19.3/src/educommon/auth/simple_auth/migrations/
--rw-r--r--   0 root         (0) root         (0)     1491 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      745 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.352709 educommon-2.19.3/src/educommon/auth/simple_auth/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.422709 educommon-2.19.3/src/educommon/auth/simple_auth/static/simple_auth/
--rw-r--r--   0 root         (0) root         (0)      123 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.352709 educommon-2.19.3/src/educommon/auth/simple_auth/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.423709 educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/
--rw-r--r--   0 root         (0) root         (0)     1577 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.423709 educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/email/
--rw-r--r--   0 root         (0) root         (0)      635 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
--rw-r--r--   0 root         (0) root         (0)     1444 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
--rw-r--r--   0 root         (0) root         (0)     1340 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
--rw-r--r--   0 root         (0) root         (0)     4676 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/ui.py
--rw-r--r--   0 root         (0) root         (0)      270 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/auth/simple_auth/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.425709 educommon-2.19.3/src/educommon/contingent/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3074 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/actions.py
--rw-r--r--   0 root         (0) root         (0)      309 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     6968 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/base.py
--rw-r--r--   0 root         (0) root         (0)    60706 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/catalogs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.432709 educommon-2.19.3/src/educommon/contingent/contingent_plugin/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      721 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/actions.py
--rw-r--r--   0 root         (0) root         (0)      711 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.433709 educommon-2.19.3/src/educommon/contingent/contingent_plugin/migrations/
--rw-r--r--   0 root         (0) root         (0)     1680 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1241 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      893 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/model_views.py
--rw-r--r--   0 root         (0) root         (0)     2495 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/models.py
--rw-r--r--   0 root         (0) root         (0)     5296 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/observer.py
--rw-r--r--   0 root         (0) root         (0)      205 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/plugin_meta.py
--rw-r--r--   0 root         (0) root         (0)     3311 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/storage.py
--rw-r--r--   0 root         (0) root         (0)     7094 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/contingent_plugin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.435709 educommon-2.19.3/src/educommon/contingent/json_data/
--rw-r--r--   0 root         (0) root         (0)    53540 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/json_data/okogu.json
--rw-r--r--   0 root         (0) root         (0)    30723 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/contingent/json_data/oksm.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.437709 educommon-2.19.3/src/educommon/django/
--rw-r--r--   0 root         (0) root         (0)      125 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.443709 educommon-2.19.3/src/educommon/django/db/
--rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7092 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.444709 educommon-2.19.3/src/educommon/django/db/migration/
--rw-r--r--   0 root         (0) root         (0)     1882 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9734 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/migration/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.447709 educommon-2.19.3/src/educommon/django/db/mixins/
--rw-r--r--   0 root         (0) root         (0)    10390 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24890 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/mixins/date_interval.py
--rw-r--r--   0 root         (0) root         (0)    12510 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/mixins/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.448709 educommon-2.19.3/src/educommon/django/db/model_view/
--rw-r--r--   0 root         (0) root         (0)    12516 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/model_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/model_view/table-view.html
--rw-r--r--   0 root         (0) root         (0)     2059 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/models.py
--rw-r--r--   0 root         (0) root         (0)    11197 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/observer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.450709 educommon-2.19.3/src/educommon/django/db/partitioning/
--rw-r--r--   0 root         (0) root         (0)     4455 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/README.md
--rw-r--r--   0 root         (0) root         (0)    22512 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.451709 educommon-2.19.3/src/educommon/django/db/partitioning/management/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.453709 educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
--rw-r--r--   0 root         (0) root         (0)     2280 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/clear_table.py
--rw-r--r--   0 root         (0) root         (0)     2127 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/split_table.py
--rw-r--r--   0 root         (0) root         (0)    20345 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/partitioning.sql
--rw-r--r--   0 root         (0) root         (0)     3401 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/partitioning/triggers.sql
--rw-r--r--   0 root         (0) root         (0)     3274 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/routers.py
--rw-r--r--   0 root         (0) root         (0)     9489 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.454709 educommon-2.19.3/src/educommon/django/db/validators/
--rw-r--r--   0 root         (0) root         (0)     2084 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38870 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/db/validators/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.455709 educommon-2.19.3/src/educommon/django/storages/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.460709 educommon-2.19.3/src/educommon/django/storages/atcfs/
--rw-r--r--   0 root         (0) root         (0)     2656 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/README.rst
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6079 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/api.py
--rw-r--r--   0 root         (0) root         (0)      435 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      172 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.461709 educommon-2.19.3/src/educommon/django/storages/atcfs/management/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.463709 educommon-2.19.3/src/educommon/django/storages/atcfs/management/commands/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7567 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
--rw-r--r--   0 root         (0) root         (0)      207 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/models.py
--rw-r--r--   0 root         (0) root         (0)     3108 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/monkey_patching.py
--rw-r--r--   0 root         (0) root         (0)      847 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/settings.py
--rw-r--r--   0 root         (0) root         (0)     4135 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.463709 educommon-2.19.3/src/educommon/django/storages/atcfs/templates/
--rw-r--r--   0 root         (0) root         (0)      196 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.463709 educommon-2.19.3/src/educommon/extjs/
--rw-r--r--   0 root         (0) root         (0)      143 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/extjs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.464709 educommon-2.19.3/src/educommon/extjs/fields/
--rw-r--r--   0 root         (0) root         (0)      166 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/extjs/fields/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/extjs/fields/input_params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.470709 educommon-2.19.3/src/educommon/importer/
--rw-r--r--   0 root         (0) root         (0)    37974 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/XLSReader.py
--rw-r--r--   0 root         (0) root         (0)      140 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13456 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/api.py
--rw-r--r--   0 root         (0) root         (0)      798 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/constants.py
--rw-r--r--   0 root         (0) root         (0)    10392 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/loggers.py
--rw-r--r--   0 root         (0) root         (0)    37557 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/proxy.py
--rw-r--r--   0 root         (0) root         (0)     6315 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/proxy_import.py
--rw-r--r--   0 root         (0) root         (0)     2087 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/refactoring-notes.txt
--rw-r--r--   0 root         (0) root         (0)     1585 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/report.py
--rw-r--r--   0 root         (0) root         (0)     8704 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/test_file.xls
--rw-r--r--   0 root         (0) root         (0)     3983 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/ui.py
--rw-r--r--   0 root         (0) root         (0)     1306 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/importer/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.471709 educommon-2.19.3/src/educommon/ioc/
--rw-r--r--   0 root         (0) root         (0)     4098 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ioc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.472709 educommon-2.19.3/src/educommon/m3/
--rw-r--r--   0 root         (0) root         (0)    17732 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.477709 educommon-2.19.3/src/educommon/m3/extensions/
--rw-r--r--   0 root         (0) root         (0)      269 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.479709 educommon-2.19.3/src/educommon/m3/extensions/listeners/
--rw-r--r--   0 root         (0) root         (0)     9021 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.483709 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/__init__.py
--rw-r--r--   0 root         (0) root         (0)      916 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
--rw-r--r--   0 root         (0) root         (0)     6145 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/listeners.py
--rw-r--r--   0 root         (0) root         (0)     7648 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/mixins.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
--rw-r--r--   0 root         (0) root         (0)      474 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/signals.py
--rw-r--r--   0 root         (0) root         (0)     3529 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/ui.py
--rw-r--r--   0 root         (0) root         (0)     3026 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/utils.py
--rw-r--r--   0 root         (0) root         (0)     6971 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/extensions/ui.py
--rw-r--r--   0 root         (0) root         (0)     5187 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/m3/transaction_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.485709 educommon-2.19.3/src/educommon/objectpack/
--rw-r--r--   0 root         (0) root         (0)      126 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14370 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/actions.py
--rw-r--r--   0 root         (0) root         (0)      268 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.491709 educommon-2.19.3/src/educommon/objectpack/templates/
--rw-r--r--   0 root         (0) root         (0)      437 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/templates/base-grid-window.js
--rw-r--r--   0 root         (0) root         (0)     1408 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/templates/filter-panel.js
--rw-r--r--   0 root         (0) root         (0)     1544 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/templates/grid-panel.js
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/templates/multiSelectWindow.js
--rw-r--r--   0 root         (0) root         (0)     6741 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/templates/multiselect-page-fix.js
--rw-r--r--   0 root         (0) root         (0)     1838 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/templates/relations-check-mixin-template.html
--rw-r--r--   0 root         (0) root         (0)    15059 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/objectpack/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.494709 educommon-2.19.3/src/educommon/report/
--rw-r--r--   0 root         (0) root         (0)    18050 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8846 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.504709 educommon-2.19.3/src/educommon/report/constructor/
--rw-r--r--   0 root         (0) root         (0)     1138 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/README.rst
--rw-r--r--   0 root         (0) root         (0)     1300 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      211 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      424 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/apps.py
--rw-r--r--   0 root         (0) root         (0)    26060 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.504709 educommon-2.19.3/src/educommon/report/constructor/builders/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/builders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.510709 educommon-2.19.3/src/educommon/report/constructor/builders/excel/
--rw-r--r--   0 root         (0) root         (0)      160 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/builders/excel/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56385 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/builders/excel/_base.py
--rw-r--r--   0 root         (0) root         (0)     4843 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/builders/excel/_header.py
--rw-r--r--   0 root         (0) root         (0)       85 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/builders/excel/constants.py
--rw-r--r--   0 root         (0) root         (0)     6273 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/builders/excel/product.py
--rw-r--r--   0 root         (0) root         (0)     5182 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/builders/excel/with_merged_cells.py
--rw-r--r--   0 root         (0) root         (0)     1095 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/config.py
--rw-r--r--   0 root         (0) root         (0)     3540 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.514709 educommon-2.19.3/src/educommon/report/constructor/editor/
--rw-r--r--   0 root         (0) root         (0)       97 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/editor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39015 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/editor/actions.py
--rw-r--r--   0 root         (0) root         (0)    39225 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/editor/edit-window.js
--rw-r--r--   0 root         (0) root         (0)     3247 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/editor/list-window.js
--rw-r--r--   0 root         (0) root         (0)    24876 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/editor/ui.py
--rw-r--r--   0 root         (0) root         (0)     1353 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.525709 educommon-2.19.3/src/educommon/report/constructor/migrations/
--rw-r--r--   0 root         (0) root         (0)     3497 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     5113 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0002_report_filters.py
--rw-r--r--   0 root         (0) root         (0)      576 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
--rw-r--r--   0 root         (0) root         (0)     1473 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
--rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
--rw-r--r--   0 root         (0) root         (0)     1388 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0006_reportsorting.py
--rw-r--r--   0 root         (0) root         (0)     1645 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0007_include_available_units.py
--rw-r--r--   0 root         (0) root         (0)      647 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
--rw-r--r--   0 root         (0) root         (0)      623 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
--rw-r--r--   0 root         (0) root         (0)      973 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2421 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/mixins.py
--rw-r--r--   0 root         (0) root         (0)    18818 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/models.py
--rw-r--r--   0 root         (0) root         (0)      171 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/plugin_meta.py
--rw-r--r--   0 root         (0) root         (0)     1948 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/registries.py
--rw-r--r--   0 root         (0) root         (0)     6918 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/utils.py
--rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/constructor/validators.py
--rw-r--r--   0 root         (0) root         (0)    10100 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/reporter.py
--rw-r--r--   0 root         (0) root         (0)    10124 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/report/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.528709 educommon-2.19.3/src/educommon/rest/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1264 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/rest/actions.py
--rw-r--r--   0 root         (0) root         (0)     3887 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/rest/context.py
--rw-r--r--   0 root         (0) root         (0)     2525 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/rest/controllers.py
--rw-r--r--   0 root         (0) root         (0)      493 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/rest/misc.py
--rw-r--r--   0 root         (0) root         (0)     4888 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/rest/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.530709 educommon-2.19.3/src/educommon/secure_media/
--rw-r--r--   0 root         (0) root         (0)     4001 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/secure_media/README.rst
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/secure_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1318 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/secure_media/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      108 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/thread_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.537709 educommon-2.19.3/src/educommon/utils/
--rw-r--r--   0 root         (0) root         (0)     2508 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      546 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/caching.py
--rw-r--r--   0 root         (0) root         (0)     5513 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/date.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.540709 educommon-2.19.3/src/educommon/utils/db/
--rw-r--r--   0 root         (0) root         (0)     7729 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2886 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/utils/db/postgresql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.553709 educommon-2.19.3/src/educommon/utils/fonts/
--rw-r--r--   0 root         (0) root         (0)   275572 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/fonts/Arial.ttf
--rw-r--r--   0 root         (0) root         (0)   811820 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/fonts/Calibri.ttf
--rw-r--r--   0 root         (0) root         (0)   265528 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/fonts/Tahoma.ttf
--rw-r--r--   0 root         (0) root         (0)     4875 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.554709 educommon-2.19.3/src/educommon/utils/licence/
--rw-r--r--   0 root         (0) root         (0)     5217 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/licence/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1230 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/licence/converters.py
--rw-r--r--   0 root         (0) root         (0)     3445 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     1238 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/patches.py
--rw-r--r--   0 root         (0) root         (0)     9547 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/plugins.py
--rw-r--r--   0 root         (0) root         (0)     2021 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/registry.py
--rw-r--r--   0 root         (0) root         (0)     8848 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/serializer.py
--rw-r--r--   0 root         (0) root         (0)     2907 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/storage.py
--rw-r--r--   0 root         (0) root         (0)     2863 2022-11-15 11:33:28.000000 educommon-2.19.3/src/educommon/utils/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.555709 educommon-2.19.3/src/educommon/utils/system_app/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/system_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.556709 educommon-2.19.3/src/educommon/utils/system_app/management/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/system_app/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.557709 educommon-2.19.3/src/educommon/utils/system_app/management/commands/
--rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/system_app/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9513 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/system_app/management/commands/delete_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.558709 educommon-2.19.3/src/educommon/utils/system_app/templatetags/
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/system_app/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      312 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/system_app/templatetags/educommon.py
--rw-r--r--   0 root         (0) root         (0)    14374 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.561709 educommon-2.19.3/src/educommon/utils/xml/
--rw-r--r--   0 root         (0) root         (0)     2243 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/xml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/xml/catalog.json
--rw-r--r--   0 root         (0) root         (0)     1760 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/xml/resolver.py
--rw-r--r--   0 root         (0) root         (0)    13160 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
--rw-r--r--   0 root         (0) root         (0)    13465 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
--rw-r--r--   0 root         (0) root         (0)     5234 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/xml/xenc-schema.xsd
--rw-r--r--   0 root         (0) root         (0)    10293 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/utils/xml/xmldsig-core-schema.xsd
--rw-r--r--   0 root         (0) root         (0)      452 2022-11-15 11:33:40.000000 educommon-2.19.3/src/educommon/version.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.565709 educommon-2.19.3/src/educommon/ws_log/
--rw-r--r--   0 root         (0) root         (0)     5467 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/README.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9269 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/actions.py
--rw-r--r--   0 root         (0) root         (0)      150 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     7369 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.569709 educommon-2.19.3/src/educommon/ws_log/migrations/
--rw-r--r--   0 root         (0) root         (0)     2810 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1014 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
--rw-r--r--   0 root         (0) root         (0)     1786 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
--rw-r--r--   0 root         (0) root         (0)     1036 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
--rw-r--r--   0 root         (0) root         (0)     1690 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
--rw-r--r--   0 root         (0) root         (0)      583 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
--rw-r--r--   0 root         (0) root         (0)     1376 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
--rw-r--r--   0 root         (0) root         (0)      581 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5781 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/models.py
--rw-r--r--   0 root         (0) root         (0)      925 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/provider.py
--rw-r--r--   0 root         (0) root         (0)     3483 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.571709 educommon-2.19.3/src/educommon/ws_log/smev/
--rw-r--r--   0 root         (0) root         (0)      140 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5871 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/smev/applications.py
--rw-r--r--   0 root         (0) root         (0)      673 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/smev/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.357709 educommon-2.19.3/src/educommon/ws_log/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.572709 educommon-2.19.3/src/educommon/ws_log/templates/report/
--rw-r--r--   0 root         (0) root         (0)    10439 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/templates/report/smev_logs.xlsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.573709 educommon-2.19.3/src/educommon/ws_log/templates/ui-js/
--rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
--rw-r--r--   0 root         (0) root         (0)     1103 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
--rw-r--r--   0 root         (0) root         (0)     4147 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/ui.py
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-05 14:23:59.000000 educommon-2.19.3/src/educommon/ws_log/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 11:33:40.363709 educommon-2.19.3/src/educommon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1058 2022-11-15 11:33:40.000000 educommon-2.19.3/src/educommon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14466 2022-11-15 11:33:40.000000 educommon-2.19.3/src/educommon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-15 11:33:40.000000 educommon-2.19.3/src/educommon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      324 2022-11-15 11:33:40.000000 educommon-2.19.3/src/educommon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-11-15 11:33:40.000000 educommon-2.19.3/src/educommon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.708430 educommon-2.20.0/
+-rw-r--r--   0 root         (0) root         (0)   110498 2023-07-18 06:09:18.000000 educommon-2.20.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)      102 2022-07-05 14:23:59.000000 educommon-2.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-18 06:09:32.707430 educommon-2.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2022-07-05 14:23:59.000000 educommon-2.20.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1981 2022-07-05 14:23:59.000000 educommon-2.20.0/UPGRADE.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 06:09:32.708430 educommon-2.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2466 2022-07-05 14:23:59.000000 educommon-2.20.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.345430 educommon-2.20.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.361430 educommon-2.20.0/src/educommon/
+-rw-r--r--   0 root         (0) root         (0)      475 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.366430 educommon-2.20.0/src/educommon/about/
+-rw-r--r--   0 root         (0) root         (0)     2685 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/README.rst
+-rw-r--r--   0 root         (0) root         (0)      149 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.345430 educommon-2.20.0/src/educommon/about/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.367430 educommon-2.20.0/src/educommon/about/static/edu_about/
+-rw-r--r--   0 root         (0) root         (0)     8382 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/static/edu_about/barsgroup.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.375430 educommon-2.20.0/src/educommon/about/ui/
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/about-window.js
+-rw-r--r--   0 root         (0) root         (0)     6090 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/actions.py
+-rw-r--r--   0 root         (0) root         (0)      700 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/common-tab.html
+-rw-r--r--   0 root         (0) root         (0)    11192 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/packages-tab.js
+-rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/postgresql-extensions-tab.js
+-rw-r--r--   0 root         (0) root         (0)     5381 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/ui/ui.py
+-rw-r--r--   0 root         (0) root         (0)      718 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/about/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.380430 educommon-2.20.0/src/educommon/async_tasks/
+-rw-r--r--   0 root         (0) root         (0)      166 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      146 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/apps.py
+-rw-r--r--   0 root         (0) root         (0)      267 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.382430 educommon-2.20.0/src/educommon/async_tasks/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      303 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/fixtures/initial_data.json
+-rw-r--r--   0 root         (0) root         (0)     3468 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/locks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.385430 educommon-2.20.0/src/educommon/async_tasks/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4309 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      603 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/migrations/0002_load_initial_data.py
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3618 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/models.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/statuses.py
+-rw-r--r--   0 root         (0) root         (0)    11236 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/async_tasks/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.394430 educommon-2.20.0/src/educommon/audit_log/
+-rw-r--r--   0 root         (0) root         (0)     2829 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)      302 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/apps.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.395430 educommon-2.20.0/src/educommon/audit_log/error_log/
+-rw-r--r--   0 root         (0) root         (0)      153 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/error_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/error_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.396430 educommon-2.20.0/src/educommon/audit_log/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.396430 educommon-2.20.0/src/educommon/audit_log/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.405430 educommon-2.20.0/src/educommon/audit_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4547 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0002_install_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)      492 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0003_logproxy.py
+-rw-r--r--   0 root         (0) root         (0)      342 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)      769 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0005_postgresql_error.py
+-rw-r--r--   0 root         (0) root         (0)      669 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2022-07-08 03:53:12.000000 educommon-2.20.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/models.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     8820 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/proxies.py
+-rw-r--r--   0 root         (0) root         (0)      251 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/routers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.409430 educommon-2.20.0/src/educommon/audit_log/sql/
+-rw-r--r--   0 root         (0) root         (0)     1395 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/sql/configure_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/sql/configure_selective_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/sql/create_selective_tables_function.sql
+-rw-r--r--   0 root         (0) root         (0)    14310 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/sql/install_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)     2137 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.410430 educommon-2.20.0/src/educommon/audit_log/utils/
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/audit_log/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/audit_log/utils/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.411430 educommon-2.20.0/src/educommon/auth/
+-rw-r--r--   0 root         (0) root         (0)      135 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.425430 educommon-2.20.0/src/educommon/auth/rbac/
+-rw-r--r--   0 root         (0) root         (0)      378 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27149 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/actions.py
+-rw-r--r--   0 root         (0) root         (0)      473 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/app_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.429430 educommon-2.20.0/src/educommon/auth/rbac/backends/
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/base.py
+-rw-r--r--   0 root         (0) root         (0)    10328 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/caching.py
+-rw-r--r--   0 root         (0) root         (0)     5066 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/backends/simple.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/checker.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/config.py
+-rw-r--r--   0 root         (0) root         (0)      562 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.432430 educommon-2.20.0/src/educommon/auth/rbac/management/
+-rw-r--r--   0 root         (0) root         (0)      127 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.433430 educommon-2.20.0/src/educommon/auth/rbac/management/commands/
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/management/commands/rbac.py
+-rw-r--r--   0 root         (0) root         (0)    16332 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.435430 educommon-2.20.0/src/educommon/auth/rbac/migrations/
+-rw-r--r--   0 root         (0) root         (0)     5578 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      681 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
+-rw-r--r--   0 root         (0) root         (0)      574 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15466 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/models.py
+-rw-r--r--   0 root         (0) root         (0)      927 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.348430 educommon-2.20.0/src/educommon/auth/rbac/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.439430 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/
+-rw-r--r--   0 root         (0) root         (0)      335 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/role-add-window.js
+-rw-r--r--   0 root         (0) root         (0)     7914 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
+-rw-r--r--   0 root         (0) root         (0)     3768 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
+-rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
+-rw-r--r--   0 root         (0) root         (0)    15794 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/ui.py
+-rw-r--r--   0 root         (0) root         (0)     7929 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/utils.py
+-rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/rbac/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.446430 educommon-2.20.0/src/educommon/auth/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)      289 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11903 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/actions.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/checkers.py
+-rw-r--r--   0 root         (0) root         (0)      453 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.447430 educommon-2.20.0/src/educommon/auth/simple_auth/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1491 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      745 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.348430 educommon-2.20.0/src/educommon/auth/simple_auth/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.448430 educommon-2.20.0/src/educommon/auth/simple_auth/static/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)      123 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.349430 educommon-2.20.0/src/educommon/auth/simple_auth/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.450430 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)     1577 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.451430 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/email/
+-rw-r--r--   0 root         (0) root         (0)      635 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
+-rw-r--r--   0 root         (0) root         (0)     1444 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
+-rw-r--r--   0 root         (0) root         (0)     4676 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/ui.py
+-rw-r--r--   0 root         (0) root         (0)      270 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/auth/simple_auth/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.456430 educommon-2.20.0/src/educommon/contingent/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/actions.py
+-rw-r--r--   0 root         (0) root         (0)      309 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/base.py
+-rw-r--r--   0 root         (0) root         (0)    60706 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/catalogs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.465430 educommon-2.20.0/src/educommon/contingent/contingent_plugin/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      721 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/actions.py
+-rw-r--r--   0 root         (0) root         (0)      711 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.467430 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1680 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      893 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/model_views.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/models.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/observer.py
+-rw-r--r--   0 root         (0) root         (0)      205 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/plugin_meta.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/storage.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/contingent_plugin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.471430 educommon-2.20.0/src/educommon/contingent/json_data/
+-rw-r--r--   0 root         (0) root         (0)    53540 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/json_data/okogu.json
+-rw-r--r--   0 root         (0) root         (0)    30723 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/contingent/json_data/oksm.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.472430 educommon-2.20.0/src/educommon/django/
+-rw-r--r--   0 root         (0) root         (0)      125 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.479430 educommon-2.20.0/src/educommon/django/db/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7092 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.481430 educommon-2.20.0/src/educommon/django/db/migration/
+-rw-r--r--   0 root         (0) root         (0)     1882 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9734 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/migration/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.484430 educommon-2.20.0/src/educommon/django/db/mixins/
+-rw-r--r--   0 root         (0) root         (0)    14747 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/django/db/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24890 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/mixins/date_interval.py
+-rw-r--r--   0 root         (0) root         (0)    12510 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/mixins/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.487430 educommon-2.20.0/src/educommon/django/db/model_view/
+-rw-r--r--   0 root         (0) root         (0)    12516 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/model_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/model_view/table-view.html
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/django/db/models.py
+-rw-r--r--   0 root         (0) root         (0)    11197 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/observer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.491430 educommon-2.20.0/src/educommon/django/db/partitioning/
+-rw-r--r--   0 root         (0) root         (0)     4455 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/README.md
+-rw-r--r--   0 root         (0) root         (0)    22512 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.491430 educommon-2.20.0/src/educommon/django/db/partitioning/management/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.497430 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/clear_table.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/split_table.py
+-rw-r--r--   0 root         (0) root         (0)    20345 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/partitioning.sql
+-rw-r--r--   0 root         (0) root         (0)     3401 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/partitioning/triggers.sql
+-rw-r--r--   0 root         (0) root         (0)     3274 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/routers.py
+-rw-r--r--   0 root         (0) root         (0)     9489 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.499430 educommon-2.20.0/src/educommon/django/db/validators/
+-rw-r--r--   0 root         (0) root         (0)     2084 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/validators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38870 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/db/validators/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.502430 educommon-2.20.0/src/educommon/django/storages/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.513430 educommon-2.20.0/src/educommon/django/storages/atcfs/
+-rw-r--r--   0 root         (0) root         (0)     2656 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/api.py
+-rw-r--r--   0 root         (0) root         (0)      435 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)      172 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.515430 educommon-2.20.0/src/educommon/django/storages/atcfs/management/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.517430 educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7567 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
+-rw-r--r--   0 root         (0) root         (0)      207 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/models.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/monkey_patching.py
+-rw-r--r--   0 root         (0) root         (0)      847 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/settings.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.518430 educommon-2.20.0/src/educommon/django/storages/atcfs/templates/
+-rw-r--r--   0 root         (0) root         (0)      196 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.519430 educommon-2.20.0/src/educommon/extjs/
+-rw-r--r--   0 root         (0) root         (0)      143 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/extjs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.520430 educommon-2.20.0/src/educommon/extjs/fields/
+-rw-r--r--   0 root         (0) root         (0)      166 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/extjs/fields/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/extjs/fields/input_params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.538430 educommon-2.20.0/src/educommon/importer/
+-rw-r--r--   0 root         (0) root         (0)    37974 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/XLSReader.py
+-rw-r--r--   0 root         (0) root         (0)      140 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13456 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/api.py
+-rw-r--r--   0 root         (0) root         (0)      798 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10392 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/loggers.py
+-rw-r--r--   0 root         (0) root         (0)    37557 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6315 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/proxy_import.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/refactoring-notes.txt
+-rw-r--r--   0 root         (0) root         (0)     1585 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/report.py
+-rw-r--r--   0 root         (0) root         (0)     8704 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/test_file.xls
+-rw-r--r--   0 root         (0) root         (0)     3983 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/importer/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.541430 educommon-2.20.0/src/educommon/integration_entities/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/consts.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/entities.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/enums.py
+-rw-r--r--   0 root         (0) root         (0)     8675 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/integration_entities/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.541430 educommon-2.20.0/src/educommon/ioc/
+-rw-r--r--   0 root         (0) root         (0)     4098 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ioc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.544430 educommon-2.20.0/src/educommon/m3/
+-rw-r--r--   0 root         (0) root         (0)    17732 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.546430 educommon-2.20.0/src/educommon/m3/extensions/
+-rw-r--r--   0 root         (0) root         (0)      269 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.547430 educommon-2.20.0/src/educommon/m3/extensions/listeners/
+-rw-r--r--   0 root         (0) root         (0)     9021 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.553430 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      916 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
+-rw-r--r--   0 root         (0) root         (0)     6145 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py
+-rw-r--r--   0 root         (0) root         (0)     7648 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py
+-rw-r--r--   0 root         (0) root         (0)       94 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
+-rw-r--r--   0 root         (0) root         (0)      474 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/signals.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6971 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/extensions/ui.py
+-rw-r--r--   0 root         (0) root         (0)     5187 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/m3/transaction_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.556430 educommon-2.20.0/src/educommon/objectpack/
+-rw-r--r--   0 root         (0) root         (0)      126 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14370 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/actions.py
+-rw-r--r--   0 root         (0) root         (0)      268 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.562430 educommon-2.20.0/src/educommon/objectpack/templates/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/base-grid-window.js
+-rw-r--r--   0 root         (0) root         (0)     1408 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/filter-panel.js
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/grid-panel.js
+-rw-r--r--   0 root         (0) root         (0)     1842 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/multiSelectWindow.js
+-rw-r--r--   0 root         (0) root         (0)     6741 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/multiselect-page-fix.js
+-rw-r--r--   0 root         (0) root         (0)     1838 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/templates/relations-check-mixin-template.html
+-rw-r--r--   0 root         (0) root         (0)    15059 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/objectpack/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.566430 educommon-2.20.0/src/educommon/report/
+-rw-r--r--   0 root         (0) root         (0)    18050 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8846 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.580430 educommon-2.20.0/src/educommon/report/constructor/
+-rw-r--r--   0 root         (0) root         (0)     1138 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1300 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      211 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)      424 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/apps.py
+-rw-r--r--   0 root         (0) root         (0)    26060 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.581430 educommon-2.20.0/src/educommon/report/constructor/builders/
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.587430 educommon-2.20.0/src/educommon/report/constructor/builders/excel/
+-rw-r--r--   0 root         (0) root         (0)      160 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56385 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/_header.py
+-rw-r--r--   0 root         (0) root         (0)       85 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6273 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/product.py
+-rw-r--r--   0 root         (0) root         (0)     5182 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/config.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.594430 educommon-2.20.0/src/educommon/report/constructor/editor/
+-rw-r--r--   0 root         (0) root         (0)       97 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39015 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/actions.py
+-rw-r--r--   0 root         (0) root         (0)    39225 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/edit-window.js
+-rw-r--r--   0 root         (0) root         (0)     3247 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/list-window.js
+-rw-r--r--   0 root         (0) root         (0)    24876 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/editor/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.611430 educommon-2.20.0/src/educommon/report/constructor/migrations/
+-rw-r--r--   0 root         (0) root         (0)     3497 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0002_report_filters.py
+-rw-r--r--   0 root         (0) root         (0)      576 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
+-rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0006_reportsorting.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0007_include_available_units.py
+-rw-r--r--   0 root         (0) root         (0)      647 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
+-rw-r--r--   0 root         (0) root         (0)      623 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
+-rw-r--r--   0 root         (0) root         (0)      973 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    18818 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/models.py
+-rw-r--r--   0 root         (0) root         (0)      171 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/plugin_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/registries.py
+-rw-r--r--   0 root         (0) root         (0)     6918 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/utils.py
+-rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/constructor/validators.py
+-rw-r--r--   0 root         (0) root         (0)    10100 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/reporter.py
+-rw-r--r--   0 root         (0) root         (0)    10124 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/report/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.618430 educommon-2.20.0/src/educommon/rest/
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/actions.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/context.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/controllers.py
+-rw-r--r--   0 root         (0) root         (0)      493 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4888 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/rest/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.622430 educommon-2.20.0/src/educommon/secure_media/
+-rw-r--r--   0 root         (0) root         (0)     4001 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/secure_media/README.rst
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/secure_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/secure_media/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)      108 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/thread_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.632430 educommon-2.20.0/src/educommon/utils/
+-rw-r--r--   0 root         (0) root         (0)     2508 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4066 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/caching.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/conversion.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)     9133 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/date.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.634430 educommon-2.20.0/src/educommon/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     7729 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/db/postgresql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.657430 educommon-2.20.0/src/educommon/utils/fonts/
+-rw-r--r--   0 root         (0) root         (0)   275572 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/Arial.ttf
+-rw-r--r--   0 root         (0) root         (0)   811820 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/Calibri.ttf
+-rw-r--r--   0 root         (0) root         (0)   265528 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/Tahoma.ttf
+-rw-r--r--   0 root         (0) root         (0)     4875 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.659430 educommon-2.20.0/src/educommon/utils/licence/
+-rw-r--r--   0 root         (0) root         (0)     5217 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/licence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/licence/converters.py
+-rw-r--r--   0 root         (0) root         (0)     3445 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/patches.py
+-rw-r--r--   0 root         (0) root         (0)     9547 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/registry.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/seqtools.py
+-rw-r--r--   0 root         (0) root         (0)     8848 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/storage.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-07-18 06:09:18.000000 educommon-2.20.0/src/educommon/utils/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.660430 educommon-2.20.0/src/educommon/utils/system_app/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.662430 educommon-2.20.0/src/educommon/utils/system_app/management/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.663430 educommon-2.20.0/src/educommon/utils/system_app/management/commands/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9513 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/management/commands/delete_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.664430 educommon-2.20.0/src/educommon/utils/system_app/templatetags/
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      312 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/system_app/templatetags/educommon.py
+-rw-r--r--   0 root         (0) root         (0)    14374 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.670430 educommon-2.20.0/src/educommon/utils/xml/
+-rw-r--r--   0 root         (0) root         (0)     2243 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/catalog.json
+-rw-r--r--   0 root         (0) root         (0)     1760 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    13160 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0 root         (0) root         (0)    13465 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
+-rw-r--r--   0 root         (0) root         (0)     5234 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/xenc-schema.xsd
+-rw-r--r--   0 root         (0) root         (0)    10293 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/utils/xml/xmldsig-core-schema.xsd
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.676430 educommon-2.20.0/src/educommon/ws_log/
+-rw-r--r--   0 root         (0) root         (0)     5467 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1013 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9269 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)      150 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.681430 educommon-2.20.0/src/educommon/ws_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2810 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
+-rw-r--r--   0 root         (0) root         (0)     1786 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
+-rw-r--r--   0 root         (0) root         (0)      583 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
+-rw-r--r--   0 root         (0) root         (0)      581 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
+-rw-r--r--   0 root         (0) root         (0)       16 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5781 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/models.py
+-rw-r--r--   0 root         (0) root         (0)      925 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/provider.py
+-rw-r--r--   0 root         (0) root         (0)     3483 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.684430 educommon-2.20.0/src/educommon/ws_log/smev/
+-rw-r--r--   0 root         (0) root         (0)      140 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/smev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5871 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/smev/applications.py
+-rw-r--r--   0 root         (0) root         (0)      673 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/smev/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.356430 educommon-2.20.0/src/educommon/ws_log/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.685430 educommon-2.20.0/src/educommon/ws_log/templates/report/
+-rw-r--r--   0 root         (0) root         (0)    10439 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/templates/report/smev_logs.xlsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.687430 educommon-2.20.0/src/educommon/ws_log/templates/ui-js/
+-rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
+-rw-r--r--   0 root         (0) root         (0)     1103 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
+-rw-r--r--   0 root         (0) root         (0)     4147 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2022-07-05 14:23:59.000000 educommon-2.20.0/src/educommon/ws_log/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.362430 educommon-2.20.0/src/educommon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15274 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-18 06:09:32.000000 educommon-2.20.0/src/educommon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:09:32.707430 educommon-2.20.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     6381 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_contingent_plugin_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_delete_check.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_delete_objects.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_django_db_utils.py
+-rw-r--r--   0 root         (0) root         (0)    21913 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_interval_mixins.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_patches.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_personal_data_fields.py
+-rw-r--r--   0 root         (0) root         (0)    14782 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_report.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_service_db_router.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_utils_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8531 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/test_validators.py
+-rw-r--r--   0 root         (0) root         (0)     6443 2022-07-05 14:23:59.000000 educommon-2.20.0/tests/tests_rbac.py
```

### Comparing `educommon-2.19.3/CHANGELOG.rst` & `educommon-2.20.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 .. :changelog:
 
 История изменений
 -----------------
 
+2.20.0
+++++++
+- Перенос общих компонентов РВД из ЭШ
+    - get_models_table_ids возвращает перечень id таблиц из AuditLog соответствующих указанным моделям;
+    - сущности для реализации интеграций ГИС РУО, Сферум, РВД;
+    - cached_function кэширует результат функции на указанное время для указанного набора параметров функции;
+    - преобразователи str_or_empty, str_without_control_chars, uuid_or_none, int_or_none, decimal_or_none, float_or_none;
+    - HashData вспомогательный класс для хеширования данных;
+    - вспомогательные функции для работы с датами get_today_min_datetime, get_today_max_datetime,
+      get_date_range_intersection, is_date_range_intersection, date_to_str, класс Week для работы с неделей;
+    - make_chunks метод нарезки итерабельного объекта на части.
+
 2.19.3
 ++++++
 - Доработка audit_log
     - Исправлен подход к удалению логов для моделей, которые стали нелогируемыми.
 
 2.19.2
 ++++++
```

### Comparing `educommon-2.19.3/PKG-INFO` & `educommon-2.20.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 2.19.3
+Version: 2.20.0
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `educommon-2.19.3/README.rst` & `educommon-2.20.0/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/UPGRADE.rst` & `educommon-2.20.0/UPGRADE.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/setup.py` & `educommon-2.20.0/setup.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/README.rst` & `educommon-2.20.0/src/educommon/about/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/static/edu_about/barsgroup.png` & `educommon-2.20.0/src/educommon/about/static/edu_about/barsgroup.png`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/ui/about-window.js` & `educommon-2.20.0/src/educommon/about/ui/about-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/ui/actions.py` & `educommon-2.20.0/src/educommon/about/ui/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/ui/common-tab.html` & `educommon-2.20.0/src/educommon/about/ui/common-tab.html`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/ui/packages-tab.js` & `educommon-2.20.0/src/educommon/about/ui/packages-tab.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/ui/ui.py` & `educommon-2.20.0/src/educommon/about/ui/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/about/utils.py` & `educommon-2.20.0/src/educommon/about/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/async_tasks/locks.py` & `educommon-2.20.0/src/educommon/async_tasks/locks.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/async_tasks/migrations/0001_initial.py` & `educommon-2.20.0/src/educommon/async_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/async_tasks/migrations/0002_load_initial_data.py` & `educommon-2.20.0/src/educommon/async_tasks/migrations/0002_load_initial_data.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/async_tasks/models.py` & `educommon-2.20.0/src/educommon/async_tasks/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/async_tasks/statuses.py` & `educommon-2.20.0/src/educommon/async_tasks/statuses.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/async_tasks/tasks.py` & `educommon-2.20.0/src/educommon/async_tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/__init__.py` & `educommon-2.20.0/src/educommon/audit_log/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/actions.py` & `educommon-2.20.0/src/educommon/audit_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/apps.py` & `educommon-2.20.0/src/educommon/audit_log/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/constants.py` & `educommon-2.20.0/src/educommon/audit_log/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/error_log/actions.py` & `educommon-2.20.0/src/educommon/audit_log/error_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/management/commands/reinstall_audit_log.py` & `educommon-2.20.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/middleware.py` & `educommon-2.20.0/src/educommon/audit_log/middleware.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/migrations/0001_initial.py` & `educommon-2.20.0/src/educommon/audit_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/migrations/0002_install_audit_log.py` & `educommon-2.20.0/src/educommon/audit_log/migrations/0002_install_audit_log.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/migrations/0005_postgresql_error.py` & `educommon-2.20.0/src/educommon/audit_log/migrations/0005_postgresql_error.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py` & `educommon-2.20.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py` & `educommon-2.20.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/models.py` & `educommon-2.20.0/src/educommon/audit_log/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/permissions.py` & `educommon-2.20.0/src/educommon/audit_log/permissions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/proxies.py` & `educommon-2.20.0/src/educommon/audit_log/proxies.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/sql/configure_audit_log.sql` & `educommon-2.20.0/src/educommon/audit_log/sql/configure_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/sql/create_selective_tables_function.sql` & `educommon-2.20.0/src/educommon/audit_log/sql/create_selective_tables_function.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/sql/install_audit_log.sql` & `educommon-2.20.0/src/educommon/audit_log/sql/install_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/ui.py` & `educommon-2.20.0/src/educommon/audit_log/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/utils/__init__.py` & `educommon-2.20.0/src/educommon/audit_log/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/audit_log/utils/operations.py` & `educommon-2.20.0/src/educommon/audit_log/utils/operations.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/actions.py` & `educommon-2.20.0/src/educommon/auth/rbac/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/backends/base.py` & `educommon-2.20.0/src/educommon/auth/rbac/backends/base.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/backends/caching.py` & `educommon-2.20.0/src/educommon/auth/rbac/backends/caching.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/backends/simple.py` & `educommon-2.20.0/src/educommon/auth/rbac/backends/simple.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/checker.py` & `educommon-2.20.0/src/educommon/auth/rbac/checker.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/config.py` & `educommon-2.20.0/src/educommon/auth/rbac/config.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/constants.py` & `educommon-2.20.0/src/educommon/auth/rbac/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/management/commands/rbac.py` & `educommon-2.20.0/src/educommon/auth/rbac/management/commands/rbac.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/manager.py` & `educommon-2.20.0/src/educommon/auth/rbac/manager.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/migrations/0001_initial.py` & `educommon-2.20.0/src/educommon/auth/rbac/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py` & `educommon-2.20.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/migrations/0003_permission_hidden.py` & `educommon-2.20.0/src/educommon/auth/rbac/migrations/0003_permission_hidden.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py` & `educommon-2.20.0/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/models.py` & `educommon-2.20.0/src/educommon/auth/rbac/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/permissions.py` & `educommon-2.20.0/src/educommon/auth/rbac/permissions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/role-edit-window.js` & `educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/roles-list-window.js` & `educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js` & `educommon-2.20.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/ui.py` & `educommon-2.20.0/src/educommon/auth/rbac/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/utils.py` & `educommon-2.20.0/src/educommon/auth/rbac/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/rbac/validators.py` & `educommon-2.20.0/src/educommon/auth/rbac/validators.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/actions.py` & `educommon-2.20.0/src/educommon/auth/simple_auth/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/app_meta.py` & `educommon-2.20.0/src/educommon/auth/simple_auth/app_meta.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/checkers.py` & `educommon-2.20.0/src/educommon/auth/simple_auth/checkers.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/migrations/0001_initial.py` & `educommon-2.20.0/src/educommon/auth/simple_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/models.py` & `educommon-2.20.0/src/educommon/auth/simple_auth/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html` & `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html` & `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html` & `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html` & `educommon-2.20.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/auth/simple_auth/ui.py` & `educommon-2.20.0/src/educommon/auth/simple_auth/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/actions.py` & `educommon-2.20.0/src/educommon/contingent/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/base.py` & `educommon-2.20.0/src/educommon/contingent/base.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/catalogs.py` & `educommon-2.20.0/src/educommon/contingent/catalogs.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/actions.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/apps.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/model_views.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/model_views.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/models.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/observer.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/observer.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/storage.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/contingent_plugin/utils.py` & `educommon-2.20.0/src/educommon/contingent/contingent_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/json_data/okogu.json` & `educommon-2.20.0/src/educommon/contingent/json_data/okogu.json`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/contingent/json_data/oksm.json` & `educommon-2.20.0/src/educommon/contingent/json_data/oksm.json`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/fields.py` & `educommon-2.20.0/src/educommon/django/db/fields.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/migration/__init__.py` & `educommon-2.20.0/src/educommon/django/db/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/migration/operations.py` & `educommon-2.20.0/src/educommon/django/db/migration/operations.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/mixins/__init__.py` & `educommon-2.20.0/src/educommon/report/reporter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,224 +1,265 @@
 # coding: utf-8
-u"""Классы-примеси для моделей Django."""
+u"Модуль с построителями отчетов"
 from __future__ import absolute_import
 
-from django.db import models
-from m3_django_compat import atomic
-import six
+import os
+import sys
+import uuid
 
+from django.conf import settings
+from simple_report.converter.abstract import FileConverter
+from simple_report.report import DocumentReport
+from simple_report.report import SpreadsheetReport
+from simple_report.xls.document import DocumentXLS
 
-class DeferredActionsMixin(models.Model):
 
-    """Класс-примесь для выполнения отложенных действий в моделях.
+path_dir = settings.REPORTS_DIR
+if not os.path.exists(path_dir):
+    os.makedirs(path_dir)
 
-    Позволяет выполнять действия, оформленные в виде callable-объектов,
-    до/после сохранения/удаления объекта модели.
 
-    .. code-block:: python
+def get_path(filename):
+    u"""Путь до временного файла отчёта.
 
-       class TestModel(DeferredActionsMixin, BaseModel):
-           def simple_clean(self, errors):
-               super(TestModel, self).simple_clean()
-
-               if self.status_id != get_original_object(self).status_id:
-                   log = Log.objects.create(
-                       object_id=self.id,
-                   )
-                   log.full_clean()
-                   self.after_save(log.save)
+    :param str filename: имя файла (с раcширением, без пути до файла)
+    :rtype: str
     """
+    return os.path.abspath(os.path.join(path_dir, filename))
 
-    class Meta:  # noqa: D106
-        abstract = True
 
-    def __init__(self, *args, **kwargs):  # noqa: D107
-        super(DeferredActionsMixin, self).__init__(*args, **kwargs)
+def get_url(filename):
+    u"""URL до временного файла отчёта.
 
-        self.__pre_save_actions = []
-        self.__post_save_actions = []
-        self.__pre_delete_actions = []
-        self.__post_delete_actions = []
-
-    def before_save(self, action):
-        """Добавляет действие, которое будет выполнено ДО сохранения."""
-        self.__pre_save_actions.append(action)
-
-    def after_save(self, action):
-        """Добавляет действие, которое будет выполнено ПОСЛЕ сохранения."""
-        self.__post_save_actions.append(action)
-
-    def before_delete(self, action):
-        """Добавляет действие, которое будет выполнено ДО удаления."""
-        self.__pre_delete_actions.append(action)
-
-    def after_delete(self, action):
-        """Добавляет действие, которое будет выполнено ПОСЛЕ удаления."""
-        self.__post_delete_actions.append(action)
-
-    def __execute_actions(self, actions):
-        """Выполняет запланированные ранее действия."""
-        while actions:
-            action = actions.pop()
-            action()
-
-    @atomic
-    def save(self, *args, **kwargs):  # pylint: disable=arguments-differ
-        """Дополняет сохранение объекта выполнением запланированных действий.
-
-        Действия, выполняемые **до** и **после** сохранения добавляются с
-        помощью методов :meth:`before_save` и :meth:`after_save`
-        соответственно.
-        """
-        self.__execute_actions(self.__pre_save_actions)
-        super(DeferredActionsMixin, self).save(*args, **kwargs)
-        self.__execute_actions(self.__post_save_actions)
-
-    @atomic
-    def delete(self, *args, **kwargs):  # pylint: disable=arguments-differ
-        """Дополняет удаление объекта выполнением запланированных действий.
-
-        Действия, выполняемые **до** и **после** удаления добавляются с
-        помощью методов :meth:`before_delete` и :meth:`after_delete`
-        соответственно.
-        """
-        self.__execute_actions(self.__pre_delete_actions)
-        result = super(DeferredActionsMixin, self).delete(*args, **kwargs)
-        self.__execute_actions(self.__post_delete_actions)
-        return result
-
-    @atomic
-    def safe_delete(self, *args, **kwargs):  # pylint: disable=arguments-differ
-        """Дополняет удаление объекта выполнением запланированных действий.
-
-        Действия, выполняемые **до** и **после** удаления добавляются с
-        помощью методов :meth:`before_delete` и :meth:`after_delete`
-        соответственно.
-        """
-        self.__execute_actions(self.__pre_delete_actions)
-        result = super(DeferredActionsMixin, self).safe_delete(*args, **kwargs)
-        self.__execute_actions(self.__post_delete_actions)
-        return result
-
-
-class DeleteOnSaveMixin(models.Model):
-
-    u"""Примесь для удаления объектов до/после сохранения модели.
-
-    Функционал данной примеси актуален при валидации моделей. В некоторых
-    случаях во время валидации выясняется, что какой-либо зависимый объект
-    должен быть удален. Но т.к. во время валидации экземляра модели удалять
-    объект еще рано, то можно этот объект пометить для удаления до/после
-    сохранения экземпляра модели.
-
-    Рекомендуется указывать данную примесь первой в списке базовых классов
-    модели, тогда удаление объектов будет выполняться в первую/последнюю
-    очередь.
+    :param str filename: имя файла (с раcширением, без пути до файла)
+    :rtype: str
     """
+    return '/'.join((settings.REPORTS_URL, filename))
 
-    def __init__(self, *args, **kwargs):
-        super(DeleteOnSaveMixin, self).__init__(*args, **kwargs)
-
-        # Список объектов, подлежащих удалению после сохранения self
-        self.__objects_for_delete_before_save = set()
-        self.__objects_for_delete_after_save = set()
-
-    def delete_before_save(self, obj):
-        u"""Добавляет объект в список удаляемых **перед** сохранением.
-
-        Указанный в аргументе `obj` объект помещается в список объектов,
-        которые будут удалены **до** сохранения.
-
-        :param obj: Объект модели, подлежащий удалению **до** сохранения.
-        :type obj: django.db.models.Model
-        """
-        if obj is None:
-            return
-
-        assert isinstance(obj, models.Model), type(obj)
-
-        if obj not in self.__objects_for_delete_after_save:
-            self.__objects_for_delete_before_save.add(obj)
-
-    def delete_after_save(self, obj):
-        u"""Добавляет объект в список удаляемых **после** сохранения.
 
-        Указанный в аргументе `obj` объект помещается в список объектов,
-        которые будут удалены **после** сохранения.
+class SimpleReporter(object):
+    u"""
+    Объект занимающийся комплексным построением отчета на основе simple_report:
+    1) инстанцированием и загрузкой данных провайдера
+    2) инстанцированием билдера
+    3) построением отчета
 
-        :param obj: Объект модели, подлежащий удалению **после** сохранения.
-        :type obj: django.db.models.Model
-        """
-        if obj is None:
-            return
-
-        assert isinstance(obj, models.Model), type(obj)
+    Можно использовать вне паков и экшнов
 
-        if obj not in self.__objects_for_delete_before_save:
-            self.__objects_for_delete_after_save.add(obj)
+    ..code:
 
-    @atomic
-    def save(self, *args, **kwargs):
-        def delete_object(obj):
-            if hasattr(obj, 'safe_delete'):
-                obj.safe_delete()
-            else:
-                obj.delete()
+    reporter = MySimpleReporter(provider_params, builder_params)
+    report_url = reporter.make_report()
+    """
+    # доступные форматы
+    _available_extensions = ['.xls', '.xlsx', '.docx']
 
-        def delete_objects(objects):
-            while objects:
-                obj = objects.pop()
-                if obj.pk is not None and obj != self:
-                    delete_object(obj)
+    # формат по-умолчанию
+    extension = '.xls'
 
-        delete_objects(self.__objects_for_delete_before_save)
+    # путь где лежит файл шаблона отчета
+    template_file_path = None
+    u"""
+    будет искать шаблон report.{extension} в директори отчета
+    template_file_path = None
+    custom_report.{extension} по абсолютному пути
+    template_file_path = '/tmp/some/custom_report.{extension}'
+    по относительному ./templates в директории отчета
+    template_file_path = './templates/custom_report.{extension}'
+    report.{extension} в ./templates/somedir/
+    template_file_path = './templates/somedir/'
+    """
 
-        super(DeleteOnSaveMixin, self).save(*args, **kwargs)
+    # класс провайдера для случая простого провайдера
+    data_provider_class = None
 
-        delete_objects(self.__objects_for_delete_after_save)
+    # класс билдера
+    builder_class = None
 
-    class Meta:
-        abstract = True
+    # класс адаптера
+    adapter_class = None
 
+    def __init__(self, provider_params, builder_params):
+        assert self.builder_class, u''
+        self.provider_params = provider_params
+        self.builder_params = builder_params
+
+    def get_template(self, default_base_name='report'):
+        u"""Возвращает путь к шаблону отчета.
+
+        :param default_base_name: базовое имя шаблона,
+            если определить не удалось
+        :type default_base_name: str
+        :returns: str - полный путь к шаблону
+        """
+        if (self.template_file_path is not None and
+                os.path.isabs(self.template_file_path)):
+            return self.template_file_path
+
+        report_file_path = sys.modules[self.__module__].__file__
+
+        report_dir = os.path.dirname(report_file_path)
+
+        rel_sub_path = ''
+        if (self.template_file_path is not None and
+                self.template_file_path.startswith('./')):
+            rel_sub_path = os.path.relpath(
+                os.path.dirname(self.template_file_path))
+
+        if self.template_file_path is None:
+            base_name, _ = os.path.splitext(os.path.basename(report_dir))
+        else:
+            base_name, _ = os.path.splitext(
+                os.path.basename(self.template_file_path))
+            if not base_name:
+                base_name = default_base_name
+
+        auto_report_name = '{0}{1}{2}'.format(
+            base_name, os.path.extsep, self.extension.strip('.'))
+        auto_report_path = os.path.join(
+            report_dir, rel_sub_path, auto_report_name)
+
+        assert os.path.isfile(auto_report_path), (
+            u"Report template '{0}' not found at {1}".format(
+                auto_report_name, auto_report_path))
+        return auto_report_path
+
+    def set_up_report(self):
+        u"""Настройка формата отчёта."""
+        template_path = self.get_template()
+
+        if self.extension == '.xls':
+            report = SpreadsheetReport(
+                template_path, wrapper=DocumentXLS, type=FileConverter.XLS)
+        elif self.extension == '.xlsx':
+            report = SpreadsheetReport(template_path)
+        elif self.extension == '.docx':
+            report = DocumentReport(template_path)
+        else:
+            raise Exception('Unknown template extension')
+
+        return report
+
+    def set_file_and_url(self):
+        u"""
+        Возвращает кортеж из абс. пути отчёта и url для скачивания.
+        Не требует переопределения.
+        """
+        title = self.builder_params.get('title')
+        title = title + '_' if title else ''
+        base_name = title + str(uuid.uuid4())[0:16] + self.extension
+        out_file_path = get_path(base_name)
+        out_file_url = get_url(base_name)
+
+        return (out_file_path, out_file_url)
+
+    def create_provider(self):
+        u"""
+        Кастомный метод для создания экземпляра класса провайдера.
+
+        Используется в случае необходимости явного вызова конструктора
+        провайдера, например, для композитного провайдера.
+        :returns: инстанс дата-провайдера
+        """
 
-class StringFieldsCleanerMixin(models.Model):
+    def init_provider(self, data_provider):
+        u"""
+        Инициализирует дата-провайдер с параметрами self.provider_params
+        """
+        data_provider.init(**self.provider_params)
 
-    u"""Примесь для удаления из строковых полей модели лишних пробелов.
+    def create_builder(self, data_provider, report):
+        u"""
+        Создание билдера.
+        Если требуется, можно использовать адаптер self.adapter_class
 
-    Во всех текстовых полях модели удаляет пробельные символы в начале и конце
-    строки, несколько идущих подряд пробелов заменяет на один.
+        :returns: билдер с параметрами self.builder_params
+        """
+        return self.builder_class(
+            data_provider,
+            adapter=self.adapter_class,
+            report=report,
+            params=self.builder_params
+        )
+
+    def get_data_provider(self):
+        u"""
+        Создание провайдера и взятие данных.
 
-    Для полей с разрешенными пустыми значениями (null=True) пустые строки
-    заменяет на None.
+        :return: Provider с уже сформированным результатом
+        """
+        # создание провайдера
+        # для случая композитного провайдера
+        data_provider = self.create_provider()
+        if data_provider is None:
+            # если простой провайдер, достаточно описать его класс
+            data_provider = self.data_provider_class()
+
+        self.init_provider(data_provider)
+        data_provider.load_data()
+
+        return data_provider
+
+    def _get_report_builder(self, data_provider, report):
+        u"""
+        Создание билдера и построение отчета.
+
+        :param data_provider: Provider с уже сформированным результатом.
+        :param report: Отчет форматов .xls, .xlsx или .docx
+        :returns: Результат выполнения метода build
+        """
+        # создание билдера, который будет строить кастомный отчёт
+        report_builder = self.create_builder(data_provider, report=report)
+        return report_builder.build()
+
+    def create_dir(self, out_file):
+        u"""
+        Создание директории для сохранения файла
+
+        :param out_file:  str, путь к файлу.
+        :raise: OsError
+        :return: None
+        """
+        # Если пытаемся сохранить файл в несуществующую директорию,
+        # то попробуем её предварительно создать
+        cat = os.path.dirname(out_file)
+        if not os.path.exists(cat):
+            # здесь может быть OsError
+            os.makedirs(cat)
+
+    def build_report(self, report, out_file, params):
+        u"""
+        Построение отчета.
+
+        :param report: Отчет форматов .xls, .xlsx или .docx
+        :param out_file: str, путь к файлу.
+        :param params: Результат выполение работы билдера.
+        :return: None
+        """
+        # построение отчёта
+        if isinstance(report, DocumentReport):
+            report.build(out_file, params)
+        else:
+            report.build(out_file)
+
+    def make_report(self):
+        u"""
+        Основной метод, выполняющий построение отчета
+        """
+        # получение абс. пути отчёта
+        out_file, out_url = self.set_file_and_url()
+        # настройка формата отчета
+        report = self.set_up_report()
 
-    .. note::
-       В документации Django текстовых полей не рекомендуется использовать
-       значение *None*, т.к. в этом случае возникает неоднозначность - пустым
-       значением будет являться не только None, но и пустая строка. Подробнее
-       см. http://djbook.ru/rel1.4/ref/models/fields.html#null. Но
-       использование пустой строки совместно с ограничением уникальности
-       приводит к невозможности сохранения более одной записи с пустым
-       значением, поэтому для однозначности в текстовых полях будем
-       использовать значение None, если указано null=True, и пустую строку в
-       остальных случаях.
-    """
+        # создает провайдер и формирует данные
+        data_provider = self.get_data_provider()
 
-    def clean_fields(self, exclude=None):
-        for field in self._meta.fields:
-            if isinstance(field, (models.TextField, models.CharField)):
-                field_value = getattr(self, field.attname)
-
-                if field_value is not None:
-                    field_value = six.text_type(field_value).strip()
-                    # Удаление лишних пробелов
-                    while field_value.find(u'  ') != -1:
-                        field_value = field_value.replace(u'  ', u' ')
-
-                if not field_value:
-                    field_value = None if field.null else u''
+        # создание билдера и построение отчета
+        params = self._get_report_builder(data_provider, report)
 
-                setattr(self, field.attname, field_value)
+        # создание директории для сохранения файла
+        self.create_dir(out_file)
 
-        return super(StringFieldsCleanerMixin, self).clean_fields(exclude)
+        # построение отчета.
+        self.build_report(report, out_file, params)
 
-    class Meta:
-        abstract = True
+        return out_url
```

### Comparing `educommon-2.19.3/src/educommon/django/db/mixins/date_interval.py` & `educommon-2.20.0/src/educommon/django/db/mixins/date_interval.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/mixins/validation.py` & `educommon-2.20.0/src/educommon/django/db/mixins/validation.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/model_view/__init__.py` & `educommon-2.20.0/src/educommon/django/db/model_view/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/model_view/table-view.html` & `educommon-2.20.0/src/educommon/django/db/model_view/table-view.html`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/models.py` & `educommon-2.20.0/src/educommon/django/db/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-# coding: utf-8
-from __future__ import absolute_import
+from django.db import (
+    models,
+)
+from m3.actions.exceptions import (
+    ApplicationLogicException,
+)
+from m3.db import (
+    BaseObjectModel,
+)
 
-from django.db import models
-from m3.actions.exceptions import ApplicationLogicException
-from m3.db import BaseObjectModel
-
-from .mixins import DeferredActionsMixin
-from .mixins import DeleteOnSaveMixin
-from .mixins import StringFieldsCleanerMixin
-from .mixins.validation import ModelValidationMixin
+from educommon.django.db.mixins import (
+    DeferredActionsMixin,
+    DeleteOnSaveMixin,
+    ReprStrPreModelMixin,
+    StringFieldsCleanerMixin,
+)
+from educommon.django.db.mixins.validation import (
+    ModelValidationMixin,
+)
 
 
 class BaseModel(
     DeferredActionsMixin,
     DeleteOnSaveMixin,
     StringFieldsCleanerMixin,
     ModelValidationMixin,
-    BaseObjectModel
+    ReprStrPreModelMixin,
+    BaseObjectModel,
 ):
 
-    u"""Базовый класс для всех моделей системы."""
+    """Базовый класс для всех моделей системы."""
 
     class Meta:
         abstract = True
 
 
 class ReadOnlyMixin(models.Model):
 
-    u"""Класс-примесь для моделей с записями только для чтения.
+    """Класс-примесь для моделей с записями только для чтения.
 
     В основной модели должны быть реализованы два метода:
         - is_read_only()
         - get_read_only_error_message(delete)
 
     is_read_only(obj) должен возаращать True, если объект модели obj не
     подлежит изменению/удалению.
```

### Comparing `educommon-2.19.3/src/educommon/django/db/observer.py` & `educommon-2.20.0/src/educommon/django/db/observer.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/partitioning/README.md` & `educommon-2.20.0/src/educommon/django/db/partitioning/README.md`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/partitioning/__init__.py` & `educommon-2.20.0/src/educommon/django/db/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py` & `educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/clear_table.py` & `educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/clear_table.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/partitioning/management/commands/split_table.py` & `educommon-2.20.0/src/educommon/django/db/partitioning/management/commands/split_table.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/partitioning/partitioning.sql` & `educommon-2.20.0/src/educommon/django/db/partitioning/partitioning.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/partitioning/triggers.sql` & `educommon-2.20.0/src/educommon/django/db/partitioning/triggers.sql`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/routers.py` & `educommon-2.20.0/src/educommon/django/db/routers.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/utils.py` & `educommon-2.20.0/src/educommon/django/db/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/validators/__init__.py` & `educommon-2.20.0/src/educommon/django/db/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/db/validators/simple.py` & `educommon-2.20.0/src/educommon/django/db/validators/simple.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/storages/atcfs/README.rst` & `educommon-2.20.0/src/educommon/django/storages/atcfs/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/storages/atcfs/api.py` & `educommon-2.20.0/src/educommon/django/storages/atcfs/api.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py` & `educommon-2.20.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/storages/atcfs/monkey_patching.py` & `educommon-2.20.0/src/educommon/django/storages/atcfs/monkey_patching.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/storages/atcfs/settings.py` & `educommon-2.20.0/src/educommon/django/storages/atcfs/settings.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/django/storages/atcfs/storage.py` & `educommon-2.20.0/src/educommon/django/storages/atcfs/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/extjs/fields/input_params.py` & `educommon-2.20.0/src/educommon/extjs/fields/input_params.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/XLSReader.py` & `educommon-2.20.0/src/educommon/importer/XLSReader.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/api.py` & `educommon-2.20.0/src/educommon/importer/api.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/constants.py` & `educommon-2.20.0/src/educommon/importer/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/loggers.py` & `educommon-2.20.0/src/educommon/importer/loggers.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/proxy.py` & `educommon-2.20.0/src/educommon/importer/proxy.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/proxy_import.py` & `educommon-2.20.0/src/educommon/importer/proxy_import.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/refactoring-notes.txt` & `educommon-2.20.0/src/educommon/importer/refactoring-notes.txt`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/report.py` & `educommon-2.20.0/src/educommon/importer/report.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/test_file.xls` & `educommon-2.20.0/src/educommon/importer/test_file.xls`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/ui.py` & `educommon-2.20.0/src/educommon/importer/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/importer/validators.py` & `educommon-2.20.0/src/educommon/importer/validators.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ioc/__init__.py` & `educommon-2.20.0/src/educommon/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/__init__.py` & `educommon-2.20.0/src/educommon/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/extensions/listeners/__init__.py` & `educommon-2.20.0/src/educommon/m3/extensions/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js` & `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/listeners.py` & `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/mixins.py` & `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/ui.py` & `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/extensions/listeners/delete_check/utils.py` & `educommon-2.20.0/src/educommon/m3/extensions/listeners/delete_check/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/extensions/ui.py` & `educommon-2.20.0/src/educommon/m3/extensions/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/m3/transaction_context.py` & `educommon-2.20.0/src/educommon/m3/transaction_context.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/objectpack/actions.py` & `educommon-2.20.0/src/educommon/objectpack/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/objectpack/templates/filter-panel.js` & `educommon-2.20.0/src/educommon/objectpack/templates/filter-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/objectpack/templates/grid-panel.js` & `educommon-2.20.0/src/educommon/objectpack/templates/grid-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/objectpack/templates/multiSelectWindow.js` & `educommon-2.20.0/src/educommon/objectpack/templates/multiSelectWindow.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/objectpack/templates/multiselect-page-fix.js` & `educommon-2.20.0/src/educommon/objectpack/templates/multiselect-page-fix.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/objectpack/templates/relations-check-mixin-template.html` & `educommon-2.20.0/src/educommon/objectpack/templates/relations-check-mixin-template.html`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/objectpack/ui.py` & `educommon-2.20.0/src/educommon/objectpack/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/__init__.py` & `educommon-2.20.0/src/educommon/report/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/actions.py` & `educommon-2.20.0/src/educommon/report/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/README.rst` & `educommon-2.20.0/src/educommon/report/constructor/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/__init__.py` & `educommon-2.20.0/src/educommon/report/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/base.py` & `educommon-2.20.0/src/educommon/report/constructor/base.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/builders/excel/_base.py` & `educommon-2.20.0/src/educommon/report/constructor/builders/excel/_base.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/builders/excel/_header.py` & `educommon-2.20.0/src/educommon/report/constructor/builders/excel/_header.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/builders/excel/product.py` & `educommon-2.20.0/src/educommon/report/constructor/builders/excel/product.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/builders/excel/with_merged_cells.py` & `educommon-2.20.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/config.py` & `educommon-2.20.0/src/educommon/report/constructor/config.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/constants.py` & `educommon-2.20.0/src/educommon/report/constructor/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/editor/actions.py` & `educommon-2.20.0/src/educommon/report/constructor/editor/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/editor/edit-window.js` & `educommon-2.20.0/src/educommon/report/constructor/editor/edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/editor/list-window.js` & `educommon-2.20.0/src/educommon/report/constructor/editor/list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/editor/ui.py` & `educommon-2.20.0/src/educommon/report/constructor/editor/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/exceptions.py` & `educommon-2.20.0/src/educommon/report/constructor/exceptions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0001_initial.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0002_report_filters.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0002_report_filters.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0006_reportsorting.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0006_reportsorting.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0007_include_available_units.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0007_include_available_units.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py` & `educommon-2.20.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/mixins.py` & `educommon-2.20.0/src/educommon/report/constructor/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/models.py` & `educommon-2.20.0/src/educommon/report/constructor/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/registries.py` & `educommon-2.20.0/src/educommon/report/constructor/registries.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/utils.py` & `educommon-2.20.0/src/educommon/report/constructor/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/constructor/validators.py` & `educommon-2.20.0/src/educommon/report/constructor/validators.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/report/reporter.py` & `educommon-2.20.0/src/educommon/report/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,265 +1,234 @@
 # coding: utf-8
-u"Модуль с построителями отчетов"
 from __future__ import absolute_import
 
-import os
-import sys
-import uuid
+from six.moves import range
 
-from django.conf import settings
-from simple_report.converter.abstract import FileConverter
-from simple_report.report import DocumentReport
-from simple_report.report import SpreadsheetReport
-from simple_report.xls.document import DocumentXLS
+from educommon.utils.fonts import ARIAL
+from educommon.utils.fonts import get_font
+from educommon.utils.fonts import split_text
 
 
-path_dir = settings.REPORTS_DIR
-if not os.path.exists(path_dir):
-    os.makedirs(path_dir)
+# Высота и ширина символа "0" шрифта по умолчанию в xlwt.
+DEFAULT_CHAR_SIZE = 256
 
 
-def get_path(filename):
-    u"""Путь до временного файла отчёта.
+def cm_to_inch(value):
+    u"""Переводит значение из сантиметров в дюймы."""
+    return value / 2.54
 
-    :param str filename: имя файла (с раcширением, без пути до файла)
-    :rtype: str
-    """
-    return os.path.abspath(os.path.join(path_dir, filename))
 
+def inch_to_cm(value):
+    u"""Переводит значение из дюймов в сантиметры."""
+    return value * 2.54
+
+
+def get_cell_bounds(section, row_index, column_index):
+    u"""Возвращает границы ячейки, находящейся на пересечении строки и столбца.
+
+    .. note::
+
+       Индексы строк и колонок начинаются с нуля.
 
-def get_url(filename):
-    u"""URL до временного файла отчёта.
+    :param section: Секция, в которой находится строка.
+    :type section: :class:`simple_report.xls.section.Section`
 
-    :param str filename: имя файла (с раcширением, без пути до файла)
-    :rtype: str
+    :param int row_index: Индекс строки в таблице excel.
+
+    :param int column_index: Индекс столбца в таблице excel.
+
+    :returns: Кортеж из четырех целых чисел: верхней строки, нижней строки,
+        левой колонки и правой колонки.
+    :rtype: tuple
     """
-    return '/'.join((settings.REPORTS_URL, filename))
+    merged_ranges = section.writer.wtsheet.merged_ranges
+    for first_row, last_row, first_column, last_column in merged_ranges:
+        if (
+            first_row <= row_index <= last_row and
+            first_column <= column_index <= last_column
+        ):
+            return first_row, last_row, first_column, last_column
+
+    return row_index, row_index, column_index, column_index
+
 
+def get_cell_width(section, row_index, column_index):
+    u"""Возвращает ширину ячейки с учётом объединения.
 
-class SimpleReporter(object):
-    u"""
-    Объект занимающийся комплексным построением отчета на основе simple_report:
-    1) инстанцированием и загрузкой данных провайдера
-    2) инстанцированием билдера
-    3) построением отчета
+    .. note ::
 
-    Можно использовать вне паков и экшнов
+       Ширина ячейки определяется, как 1/256 от ширины символа "0" первого
+       попавшегося шрифта в файле, т.е. единицы изменения достаточно условны.
 
-    ..code:
+    .. note::
 
-    reporter = MySimpleReporter(provider_params, builder_params)
-    report_url = reporter.make_report()
+       Индексы строк и колонок начинаются с нуля.
+
+    :param section: Секция, в которой находится строка.
+    :type section: :class:`simple_report.xls.section.Section`
+
+    :param int row_index: Индекс строки в таблице excel.
+
+    :param int column_index: Индекс столбца в таблице excel.
+
+    :rtype: int
     """
-    # доступные форматы
-    _available_extensions = ['.xls', '.xlsx', '.docx']
+    _, _, first_column, last_column = get_cell_bounds(
+        section, row_index, column_index
+    )
+    return sum(
+        section.writer.wtsheet.col(i).width
+        for i in range(first_column, last_column + 1)
+    )
+
+
+def get_cell_height(section, row_index, column_index):
+    u"""Возвращает высоту ячейки с учётом объединения.
+
+    .. note::
+
+       Индексы строк и колонок начинаются с нуля.
 
-    # формат по-умолчанию
-    extension = '.xls'
+    :param section: Секция, в которой находится строка.
+    :type section: :class:`simple_report.xls.section.Section`
 
-    # путь где лежит файл шаблона отчета
-    template_file_path = None
-    u"""
-    будет искать шаблон report.{extension} в директори отчета
-    template_file_path = None
-    custom_report.{extension} по абсолютному пути
-    template_file_path = '/tmp/some/custom_report.{extension}'
-    по относительному ./templates в директории отчета
-    template_file_path = './templates/custom_report.{extension}'
-    report.{extension} в ./templates/somedir/
-    template_file_path = './templates/somedir/'
+    :param int row_index: Индекс строки в таблице excel.
+
+    :param int column_index: Индекс столбца в таблице excel.
+
+    :returns: Высоту ячейки в `твипах <https://goo.gl/hfUW7x>`_.
+    :rtype: int
     """
+    first_row, last_row, _, _ = get_cell_bounds(
+        section, row_index, column_index
+    )
+    return sum(
+        section.writer.wtsheet.row(i).height
+        for i in range(first_row, last_row + 1)
+    )
 
-    # класс провайдера для случая простого провайдера
-    data_provider_class = None
 
-    # класс билдера
-    builder_class = None
+def adjust_row_height(section, row_idx, col_idx, text, font,
+                      adjusted_row_index=None):
+    u"""Увеличивает высоту строки, если необходимо.
 
-    # класс адаптера
-    adapter_class = None
+    Высота строки устанавливается такая, чтобы текст `text`
+    поместился в ячейку с индексами `row_idx`, `col_idx`.
 
-    def __init__(self, provider_params, builder_params):
-        assert self.builder_class, u''
-        self.provider_params = provider_params
-        self.builder_params = builder_params
-
-    def get_template(self, default_base_name='report'):
-        u"""Возвращает путь к шаблону отчета.
-
-        :param default_base_name: базовое имя шаблона,
-            если определить не удалось
-        :type default_base_name: str
-        :returns: str - полный путь к шаблону
-        """
-        if (self.template_file_path is not None and
-                os.path.isabs(self.template_file_path)):
-            return self.template_file_path
-
-        report_file_path = sys.modules[self.__module__].__file__
-
-        report_dir = os.path.dirname(report_file_path)
-
-        rel_sub_path = ''
-        if (self.template_file_path is not None and
-                self.template_file_path.startswith('./')):
-            rel_sub_path = os.path.relpath(
-                os.path.dirname(self.template_file_path))
+    Можно применять для нескольких ячеек одной строки. Тогда строке будет
+    установлена максимальная высота.
 
-        if self.template_file_path is None:
-            base_name, _ = os.path.splitext(os.path.basename(report_dir))
-        else:
-            base_name, _ = os.path.splitext(
-                os.path.basename(self.template_file_path))
-            if not base_name:
-                base_name = default_base_name
-
-        auto_report_name = '{0}{1}{2}'.format(
-            base_name, os.path.extsep, self.extension.strip('.'))
-        auto_report_path = os.path.join(
-            report_dir, rel_sub_path, auto_report_name)
-
-        assert os.path.isfile(auto_report_path), (
-            u"Report template '{0}' not found at {1}".format(
-                auto_report_name, auto_report_path))
-        return auto_report_path
-
-    def set_up_report(self):
-        u"""Настройка формата отчёта."""
-        template_path = self.get_template()
-
-        if self.extension == '.xls':
-            report = SpreadsheetReport(
-                template_path, wrapper=DocumentXLS, type=FileConverter.XLS)
-        elif self.extension == '.xlsx':
-            report = SpreadsheetReport(template_path)
-        elif self.extension == '.docx':
-            report = DocumentReport(template_path)
-        else:
-            raise Exception('Unknown template extension')
+    .. note::
+
+       Индексы строк и колонок начинаются с нуля.
+
+    :param section: Секция, в которой находится строка.
+    :type section: :class:`simple_report.xls.section.Section`
+
+    :param int row_idx: Индекс строки в таблице excel.
+
+    :param int col_idx: Индекс столбца в таблице excel.
+
+    :param unicode text: Строка, которая будет записана в ячейку.
 
-        return report
+    :param font: Шрифт.
+    :type font: :class:`PIL.ImageFont.FreeTypeFont`
 
-    def set_file_and_url(self):
-        u"""
-        Возвращает кортеж из абс. пути отчёта и url для скачивания.
-        Не требует переопределения.
-        """
-        title = self.builder_params.get('title')
-        title = title + '_' if title else ''
-        base_name = title + str(uuid.uuid4())[0:16] + self.extension
-        out_file_path = get_path(base_name)
-        out_file_url = get_url(base_name)
-
-        return (out_file_path, out_file_url)
-
-    def create_provider(self):
-        u"""
-        Кастомный метод для создания экземпляра класса провайдера.
-
-        Используется в случае необходимости явного вызова конструктора
-        провайдера, например, для композитного провайдера.
-        :returns: инстанс дата-провайдера
-        """
-
-    def init_provider(self, data_provider):
-        u"""
-        Инициализирует дата-провайдер с параметрами self.provider_params
-        """
-        data_provider.init(**self.provider_params)
-
-    def create_builder(self, data_provider, report):
-        u"""
-        Создание билдера.
-        Если требуется, можно использовать адаптер self.adapter_class
-
-        :returns: билдер с параметрами self.builder_params
-        """
-        return self.builder_class(
-            data_provider,
-            adapter=self.adapter_class,
-            report=report,
-            params=self.builder_params
+    :param int adjusted_row_index: Номер строки, размер которой будет увеличен.
+        Если не указывается (``None``), то высота всех строк объединенной
+        ячейки будет увеличена равномерно. Номер указывается относительно
+        ячейки, нумерация начинается с нуля.
+    """
+    def get_text_height(column_width):
+        u"""Вычисляет высоту строки отчета в зависимости от текста."""
+        # Т.к. высота и ширина ячейки измеряется в единицах относительно
+        # дефолтного шрифта, берем его параметры.
+        normal_font = get_font(ARIAL, 10)
+
+        # Количество символов "0", которое входит в одну ячейку без переносов.
+        # DEFAULT_CHAR_SIZE * 0.8 определяет ширину отступов слева и справа (в
+        # сумме, а не каждого отступа по отдельности). Источник точной
+        # информации об отступах в ячейке найти не удалось.
+        width_in_chars = (
+            int(column_width - DEFAULT_CHAR_SIZE * 0.8) // DEFAULT_CHAR_SIZE
         )
 
-    def get_data_provider(self):
-        u"""
-        Создание провайдера и взятие данных.
-
-        :return: Provider с уже сформированным результатом
-        """
-        # создание провайдера
-        # для случая композитного провайдера
-        data_provider = self.create_provider()
-        if data_provider is None:
-            # если простой провайдер, достаточно описать его класс
-            data_provider = self.data_provider_class()
-
-        self.init_provider(data_provider)
-        data_provider.load_data()
-
-        return data_provider
-
-    def _get_report_builder(self, data_provider, report):
-        u"""
-        Создание билдера и построение отчета.
-
-        :param data_provider: Provider с уже сформированным результатом.
-        :param report: Отчет форматов .xls, .xlsx или .docx
-        :returns: Результат выполнения метода build
-        """
-        # создание билдера, который будет строить кастомный отчёт
-        report_builder = self.create_builder(data_provider, report=report)
-        return report_builder.build()
-
-    def create_dir(self, out_file):
-        u"""
-        Создание директории для сохранения файла
-
-        :param out_file:  str, путь к файлу.
-        :raise: OsError
-        :return: None
-        """
-        # Если пытаемся сохранить файл в несуществующую директорию,
-        # то попробуем её предварительно создать
-        cat = os.path.dirname(out_file)
-        if not os.path.exists(cat):
-            # здесь может быть OsError
-            os.makedirs(cat)
-
-    def build_report(self, report, out_file, params):
-        u"""
-        Построение отчета.
-
-        :param report: Отчет форматов .xls, .xlsx или .docx
-        :param out_file: str, путь к файлу.
-        :param params: Результат выполение работы билдера.
-        :return: None
-        """
-        # построение отчёта
-        if isinstance(report, DocumentReport):
-            report.build(out_file, params)
-        else:
-            report.build(out_file)
+        str_width_px, str_height_px = normal_font.getsize('0' * width_in_chars)
+
+        # Определяем коэффициент масштабирования высоты шрифта к дефолтному.
+        _, choosen_font_height_px = font.getsize('0')
+        height_scale = (choosen_font_height_px * 1.0) / str_height_px
+
+        rows_count = len(
+            split_text(text, font, str_width_px)
+        )
+
+        height = int(rows_count * height_scale * DEFAULT_CHAR_SIZE)
 
-    def make_report(self):
-        u"""
-        Основной метод, выполняющий построение отчета
-        """
-        # получение абс. пути отчёта
-        out_file, out_url = self.set_file_and_url()
-        # настройка формата отчета
-        report = self.set_up_report()
-
-        # создает провайдер и формирует данные
-        data_provider = self.get_data_provider()
-
-        # создание билдера и построение отчета
-        params = self._get_report_builder(data_provider, report)
+        return height
 
-        # создание директории для сохранения файла
-        self.create_dir(out_file)
+    first_row, last_row, first_column, last_column = get_cell_bounds(
+        section, row_idx, col_idx
+    )
+
+    merged = first_row != last_row or first_column != last_column
+
+    cell_width = get_cell_width(section, row_idx, col_idx)
+    cell_height = get_cell_height(section, row_idx, col_idx)
+
+    # Высотя ячейки, в которой поместится указанный текст.
+    text_height = get_text_height(cell_width)
+
+    # Разница между текущей высотой ячейки и необходимой для размещения текста
+    # высотой.
+    height_delta = max(0, text_height - cell_height)
+
+    def add_row_height(row, height):
+        row.height_mismatch = True
+        row.height += height
+
+    if height_delta > 0:
+        if merged:
+            row_count = last_row - first_row + 1
+            if adjusted_row_index is None:
+                # Равномерное увеличение высоты строк
+                for r in range(first_row, last_row + 1):
+                    row = section.writer.wtsheet.row(r)
+                    add_row_height(row, height_delta // row_count)
+            else:
+                assert adjusted_row_index > row_count, (
+                    adjusted_row_index, row_count
+                )
+                row = section.writer.wtsheet.row(
+                    first_row + adjusted_row_index
+                )
+                add_row_height(row, height_delta)
+        else:
+            row = section.writer.wtsheet.row(row_idx)
+            add_row_height(row, height_delta)
 
-        # построение отчета.
-        self.build_report(report, out_file, params)
 
-        return out_url
+def adjust_row_height_arial(section, row_idx, col_idx, text, font_size=10,
+                            adjusted_row_index=None):
+    u"""Устанавливает высоту строки автоматически.
+
+    Высота строки устанавливается такая, чтобы текст text
+    поместился в ячейку с индексами row_idx, col_idx.
+
+    Расчет ведется для шрифта Arial, и соответствует отображению ячеек в
+    MS Excel.
+
+    :param section: Секция, в которой находится строка
+    :type section: :class:`simple_report.xls.section.Section`
+    :param int row_idx: Индекс строки в таблице excel
+    :param int col_idx: Индекс столбца в таблице excel
+    :param unicode text: Строка, которая будет записана в ячейку
+    :param int font_size: Размер шрифта в пунктах
+    :param int adjusted_row_index: Номер строки, размер которой будет увеличен.
+        Если не указывается (``None``), то высота всех строк объединенной
+        ячейки будет увеличена равномерно. Номер указывается относительно
+        ячейки, нумерация начинается с нуля.
+    """
+    font = get_font(ARIAL, font_size)
+    adjust_row_height(
+        section, row_idx, col_idx, text, font, adjusted_row_index
+    )
```

### Comparing `educommon-2.19.3/src/educommon/report/utils.py` & `educommon-2.20.0/src/educommon/utils/plugins.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,255 @@
 # coding: utf-8
-from __future__ import absolute_import
+from collections import defaultdict
+from functools import wraps
+from inspect import isclass
+from types import FunctionType
+from types import MethodType
 
-from six.moves import range
+from django.apps import apps
+from django.core.exceptions import ImproperlyConfigured
+from six import PY3
+from six import with_metaclass
 
-from educommon.utils.fonts import ARIAL
-from educommon.utils.fonts import get_font
-from educommon.utils.fonts import split_text
+from educommon.utils import SingletonMeta
 
 
-# Высота и ширина символа "0" шрифта по умолчанию в xlwt.
-DEFAULT_CHAR_SIZE = 256
+__all__ = ['extender_for']
 
 
-def cm_to_inch(value):
-    u"""Переводит значение из сантиметров в дюймы."""
-    return value / 2.54
+class _ExtenderRegistry(object, with_metaclass(SingletonMeta)):
 
+    """Реестр расширителей классов.
 
-def inch_to_cm(value):
-    u"""Переводит значение из дюймов в сантиметры."""
-    return value * 2.54
+    Обеспечивает работу декораторов
+    :func:`~educommon.utils.plugins.extender_for` и
+    :func:`~educommon.utils.plugins.extendable`.
 
+    .. warning::
 
-def get_cell_bounds(section, row_index, column_index):
-    u"""Возвращает границы ячейки, находящейся на пересечении строки и столбца.
+       Не предназначен для использования напрямую.
+    """
 
-    .. note::
+    def __init__(self):
+        self._extenders = defaultdict(list)
 
-       Индексы строк и колонок начинаются с нуля.
+    def _get_extender_priority(self, extender):
+        result = getattr(extender, 'priority', 0)
+        if not isinstance(result, int):
+            result = 0
+        return result
+
+    def add_extender(self, extendable_class, extender_class):
+        """Добавление расширителя для класса.
+
+        :param type extendable_class: Расширяемый класс.
+        :param type extender_class: Расширяющий класс.
+        """
+        assert isclass(extendable_class), extendable_class
+        assert isclass(extender_class), extender_class
+
+        extenders = self._extenders[extendable_class]
+        priority = self._get_extender_priority(extender_class)
+        for i, ext in enumerate(extenders):
+            if priority > self._get_extender_priority(ext):
+                extenders.insert(i, extender_class)
+                break
+        else:
+            extenders.append(extender_class)
 
-    :param section: Секция, в которой находится строка.
-    :type section: :class:`simple_report.xls.section.Section`
+    def get_extenders(self, extendable_class):
+        """Возвращает генератор классов-расширителей для указанного класса.
 
-    :param int row_index: Индекс строки в таблице excel.
+        :param type extendable_class: Расширяемый класс.
 
-    :param int column_index: Индекс столбца в таблице excel.
+        :rtype: generator
+        """
+        for extender_class in self._extenders[extendable_class]:
+            yield extender_class
 
-    :returns: Кортеж из четырех целых чисел: верхней строки, нижней строки,
-        левой колонки и правой колонки.
-    :rtype: tuple
-    """
-    merged_ranges = section.writer.wtsheet.merged_ranges
-    for first_row, last_row, first_column, last_column in merged_ranges:
-        if (
-            first_row <= row_index <= last_row and
-            first_column <= column_index <= last_column
-        ):
-            return first_row, last_row, first_column, last_column
 
-    return row_index, row_index, column_index, column_index
+_extender_registry = _ExtenderRegistry()
 
 
-def get_cell_width(section, row_index, column_index):
-    u"""Возвращает ширину ячейки с учётом объединения.
+def _function_types():
+    """Возвращает типы функций и методов, доступных для расширения."""
+    from m3_django_compat import WrapperDescriptorType
+    from m3_django_compat import MethodWrapperType
+    from m3_django_compat import MethodDescriptorType
 
-    .. note ::
+    return (
+        FunctionType,
+        MethodType,
+        WrapperDescriptorType,
+        MethodWrapperType,
+        MethodDescriptorType
+    )
 
-       Ширина ячейки определяется, как 1/256 от ширины символа "0" первого
-       попавшегося шрифта в файле, т.е. единицы изменения достаточно условны.
 
-    .. note::
+if PY3:
+    from functools import lru_cache
+    _function_types = lru_cache(maxsize=1)(_function_types)
 
-       Индексы строк и колонок начинаются с нуля.
 
-    :param section: Секция, в которой находится строка.
-    :type section: :class:`simple_report.xls.section.Section`
+def extender_for(*extendables):
+    """Помечает класс, как расширитель для указанных классов.
 
-    :param int row_index: Индекс строки в таблице excel.
+    Имена расширяемых методов должны быть указаны в ``extends_methods``. Эти
+    методы будут обернуты декоратором. Расширение staticmethod и classmethod
+    не поддерживается.
+    :func:`~educommon.utils.plugins.extendable`.
 
-    :param int column_index: Индекс столбца в таблице excel.
+    Расширение функциональности классов работает следующим образом:
 
-    :rtype: int
-    """
-    _, _, first_column, last_column = get_cell_bounds(
-        section, row_index, column_index
-    )
-    return sum(
-        section.writer.wtsheet.col(i).width
-        for i in range(first_column, last_column + 1)
-    )
+        1. Сначала вызывается метод расширяемого класса.
+        2. Затем в порядке приоритета вызываются одноименные методы у
+           классов-расширителей (если они есть в классе-расширителе). В первом
+           аргументе передаётся экземпляр расширяемого класса (``self``),
+           результат работы расширяемого метода или предыдущего расширителя, а
+           также аргументы расширяемого метода.
+        3. Результат работы последнего расширителя класса возвращается в
+           качестве результата расширяемого метода.
 
+    .. code-block:: python
+       :caption: Пример использования
 
-def get_cell_height(section, row_index, column_index):
-    u"""Возвращает высоту ячейки с учётом объединения.
+       @extender_for(ListWindow, AddWindow, EditWindow):
+       class WindowExtender(object):
 
-    .. note::
+           extends_methods = ('set_params',)
 
-       Индексы строк и колонок начинаются с нуля.
+           @staticmethod
+           def set_params(window, result, params):
+               window.width, window.height = 1000, 1000
+               return result
+    """
+    assert all(isclass(extendable) for extendable in extendables)
 
-    :param section: Секция, в которой находится строка.
-    :type section: :class:`simple_report.xls.section.Section`
+    def decorator(extender):
+        assert isclass(extender), extender
+        assert extender.extends_methods
+        assert all(
+            isinstance(getattr(extendable, method_name), _function_types())
+            for extendable in extendables
+            for method_name in extender.extends_methods
+        )
 
-    :param int row_index: Индекс строки в таблице excel.
+        for extendable_class in extendables:
+            _extender_registry.add_extender(extendable_class, extender)
 
-    :param int column_index: Индекс столбца в таблице excel.
+            for method_name in extender.extends_methods:
+                method = getattr(extendable_class, method_name)
+                if not getattr(method, '__extended__', None):
+                    method = _extendable(method)
+                    setattr(extendable_class, method_name, method)
 
-    :returns: Высоту ячейки в `твипах <https://goo.gl/hfUW7x>`_.
-    :rtype: int
-    """
-    first_row, last_row, _, _ = get_cell_bounds(
-        section, row_index, column_index
-    )
-    return sum(
-        section.writer.wtsheet.row(i).height
-        for i in range(first_row, last_row + 1)
-    )
+        return extender
+
+    return decorator
 
 
-def adjust_row_height(section, row_idx, col_idx, text, font,
-                      adjusted_row_index=None):
-    u"""Увеличивает высоту строки, если необходимо.
+def _extendable(func):
+    """Помечает метод класса как расширяемый.
 
-    Высота строки устанавливается такая, чтобы текст `text`
-    поместился в ячейку с индексами `row_idx`, `col_idx`.
+    Методы, помеченные этим декоратором могут быть расширены в классах,
+    помеченных декоратором :func:`~educommon.utils.plugins.extender_for`.
 
-    Можно применять для нескольких ячеек одной строки. Тогда строке будет
-    установлена максимальная высота.
+    О том, как работает расширение классов, написано в описании
+    :func:`~educommon.utils.plugins.extender_for`.
 
-    .. note::
+    .. code-block:: python
+       :caption: Пример использования
 
-       Индексы строк и колонок начинаются с нуля.
+       class EditWindow(BaseEditWindow):
 
-    :param section: Секция, в которой находится строка.
-    :type section: :class:`simple_report.xls.section.Section`
+           @extendable
+           def set_params(self, params):
+               ...
+    """
+    assert isinstance(func, _function_types()), func
 
-    :param int row_idx: Индекс строки в таблице excel.
+    @wraps(func)
+    def wrapper(self, *args, **kwargs):
+        from m3_django_compat import WrapperDescriptorType
+        unbound_types = (FunctionType, WrapperDescriptorType,)
+
+        assert all((
+            isinstance(func, unbound_types),
+            not isclass(self))
+        ), 'Нельзя расширить staticmethod и classmethod'
 
-    :param int col_idx: Индекс столбца в таблице excel.
+        result = func(self, *args, **kwargs)
 
-    :param unicode text: Строка, которая будет записана в ячейку.
+        if isinstance(func, MethodType):
+            method_name = func.__func__.__name__
+        else:
+            method_name = func.__name__
 
-    :param font: Шрифт.
-    :type font: :class:`PIL.ImageFont.FreeTypeFont`
+        extendable_class = self if isclass(self) else self.__class__
 
-    :param int adjusted_row_index: Номер строки, размер которой будет увеличен.
-        Если не указывается (``None``), то высота всех строк объединенной
-        ячейки будет увеличена равномерно. Номер указывается относительно
-        ячейки, нумерация начинается с нуля.
-    """
-    def get_text_height(column_width):
-        u"""Вычисляет высоту строки отчета в зависимости от текста."""
-        # Т.к. высота и ширина ячейки измеряется в единицах относительно
-        # дефолтного шрифта, берем его параметры.
-        normal_font = get_font(ARIAL, 10)
-
-        # Количество символов "0", которое входит в одну ячейку без переносов.
-        # DEFAULT_CHAR_SIZE * 0.8 определяет ширину отступов слева и справа (в
-        # сумме, а не каждого отступа по отдельности). Источник точной
-        # информации об отступах в ячейке найти не удалось.
-        width_in_chars = (
-            int(column_width - DEFAULT_CHAR_SIZE * 0.8) // DEFAULT_CHAR_SIZE
-        )
+        for extender in _extender_registry.get_extenders(extendable_class):
+            if method_name in extender.extends_methods:
+                extender_method = getattr(extender, method_name, None)
+                if callable(extender_method):
+                    result = extender_method(self, result, *args, **kwargs)
 
-        str_width_px, str_height_px = normal_font.getsize('0' * width_in_chars)
+        return result
 
-        # Определяем коэффициент масштабирования высоты шрифта к дефолтному.
-        _, choosen_font_height_px = font.getsize('0')
-        height_scale = (choosen_font_height_px * 1.0) / str_height_px
+    wrapper.__extended__ = True
 
-        rows_count = len(
-            split_text(text, font, str_width_px)
-        )
+    return wrapper
 
-        height = int(rows_count * height_scale * DEFAULT_CHAR_SIZE)
 
-        return height
+def get_plugin_apps():
+    """Возвращает подключенные плагины.
 
-    first_row, last_row, first_column, last_column = get_cell_bounds(
-        section, row_idx, col_idx
+    :rtype: generator of django.apps.config.AppConfig
+    """
+    return (
+        app_config
+        for app_config in apps.get_app_configs()
+        if (
+            hasattr(app_config.module, 'plugin_meta') and
+            hasattr(app_config.module.plugin_meta, 'connect_plugin') and
+            callable(app_config.module.plugin_meta.connect_plugin)
+        )
     )
 
-    merged = first_row != last_row or first_column != last_column
-
-    cell_width = get_cell_width(section, row_idx, col_idx)
-    cell_height = get_cell_height(section, row_idx, col_idx)
 
-    # Высотя ячейки, в которой поместится указанный текст.
-    text_height = get_text_height(cell_width)
+def init_plugin(package, settings=None, config=None):
+    """Инициализация плагина.
 
-    # Разница между текущей высотой ячейки и необходимой для размещения текста
-    # высотой.
-    height_delta = max(0, text_height - cell_height)
-
-    def add_row_height(row, height):
-        row.height_mismatch = True
-        row.height += height
-
-    if height_delta > 0:
-        if merged:
-            row_count = last_row - first_row + 1
-            if adjusted_row_index is None:
-                # Равномерное увеличение высоты строк
-                for r in range(first_row, last_row + 1):
-                    row = section.writer.wtsheet.row(r)
-                    add_row_height(row, height_delta // row_count)
-            else:
-                assert adjusted_row_index > row_count, (
-                    adjusted_row_index, row_count
-                )
-                row = section.writer.wtsheet.row(
-                    first_row + adjusted_row_index
-                )
-                add_row_height(row, height_delta)
-        else:
-            row = section.writer.wtsheet.row(row_idx)
-            add_row_height(row, height_delta)
+    Для инициализации плагина импортируется модуль ``plugin_meta`` из пакета,
+    указанного в :arg:`package`. Затем из этого пакета вызывается функция
+    ``plugin_connect``.
+
+    :param str package: имя пакета с плагином.
+    :param dict settings: переменные модуля settings системы.
+    :param dict config: параметры плагина, указанные в файле конфигурации.
+
+    :raises django.core.exceptions.ImproperlyConfigured: если указанный пакет
+        не является плагином (не импортируется, либо не содержит модуля
+        plugin_meta``, либо в этом модуле нет функции ``connect_plugin``).
+    """
+    try:
+        meta_module = __import__(
+            '.'.join((package, 'plugin_meta')),  # module name
+            {},  # globals
+            {},  # locals
+            ['connect_plugin'],  # from list
+            0  # absolute import
+        )
+    except ImportError:
+        raise ImproperlyConfigured(
+            '{} is not plugin application.'.format(package)
+        )
 
+    meta_module.__package__ = package
 
-def adjust_row_height_arial(section, row_idx, col_idx, text, font_size=10,
-                            adjusted_row_index=None):
-    u"""Устанавливает высоту строки автоматически.
-
-    Высота строки устанавливается такая, чтобы текст text
-    поместился в ячейку с индексами row_idx, col_idx.
-
-    Расчет ведется для шрифта Arial, и соответствует отображению ячеек в
-    MS Excel.
-
-    :param section: Секция, в которой находится строка
-    :type section: :class:`simple_report.xls.section.Section`
-    :param int row_idx: Индекс строки в таблице excel
-    :param int col_idx: Индекс столбца в таблице excel
-    :param unicode text: Строка, которая будет записана в ячейку
-    :param int font_size: Размер шрифта в пунктах
-    :param int adjusted_row_index: Номер строки, размер которой будет увеличен.
-        Если не указывается (``None``), то высота всех строк объединенной
-        ячейки будет увеличена равномерно. Номер указывается относительно
-        ячейки, нумерация начинается с нуля.
-    """
-    font = get_font(ARIAL, font_size)
-    adjust_row_height(
-        section, row_idx, col_idx, text, font, adjusted_row_index
-    )
+    if (not hasattr(meta_module, 'connect_plugin') or
+            not callable(meta_module.connect_plugin)):
+        raise ImproperlyConfigured(
+            '{} is not a plugin application '
+            '(module {} has not connect_plugin function)'
+            .format(package, meta_module)
+        )
+    meta_module.connect_plugin(settings, config or {})
```

### Comparing `educommon-2.19.3/src/educommon/rest/actions.py` & `educommon-2.20.0/src/educommon/rest/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/rest/context.py` & `educommon-2.20.0/src/educommon/rest/context.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/rest/controllers.py` & `educommon-2.20.0/src/educommon/rest/controllers.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/rest/mixins.py` & `educommon-2.20.0/src/educommon/rest/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/secure_media/README.rst` & `educommon-2.20.0/src/educommon/secure_media/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/secure_media/app_meta.py` & `educommon-2.20.0/src/educommon/secure_media/app_meta.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/__init__.py` & `educommon-2.20.0/src/educommon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/db/__init__.py` & `educommon-2.20.0/src/educommon/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/db/postgresql.py` & `educommon-2.20.0/src/educommon/utils/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/fonts/Arial.ttf` & `educommon-2.20.0/src/educommon/utils/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/fonts/Calibri.ttf` & `educommon-2.20.0/src/educommon/utils/fonts/Calibri.ttf`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/fonts/Tahoma.ttf` & `educommon-2.20.0/src/educommon/utils/fonts/Tahoma.ttf`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/fonts/__init__.py` & `educommon-2.20.0/src/educommon/utils/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/licence/__init__.py` & `educommon-2.20.0/src/educommon/utils/licence/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/licence/converters.py` & `educommon-2.20.0/src/educommon/utils/licence/converters.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/misc.py` & `educommon-2.20.0/src/educommon/utils/misc.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/patches.py` & `educommon-2.20.0/src/educommon/utils/patches.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/registry.py` & `educommon-2.20.0/src/educommon/utils/registry.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/serializer.py` & `educommon-2.20.0/src/educommon/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/storage.py` & `educommon-2.20.0/src/educommon/utils/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/system.py` & `educommon-2.20.0/src/educommon/utils/system.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/system_app/management/commands/delete_objects.py` & `educommon-2.20.0/src/educommon/utils/system_app/management/commands/delete_objects.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/ui.py` & `educommon-2.20.0/src/educommon/utils/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/xml/__init__.py` & `educommon-2.20.0/src/educommon/utils/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/xml/catalog.json` & `educommon-2.20.0/src/educommon/utils/xml/catalog.json`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/xml/resolver.py` & `educommon-2.20.0/src/educommon/utils/xml/resolver.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd` & `educommon-2.20.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd` & `educommon-2.20.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/xml/xenc-schema.xsd` & `educommon-2.20.0/src/educommon/utils/xml/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/utils/xml/xmldsig-core-schema.xsd` & `educommon-2.20.0/src/educommon/utils/xml/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/README.rst` & `educommon-2.20.0/src/educommon/ws_log/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/__init__.py` & `educommon-2.20.0/src/educommon/ws_log/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/actions.py` & `educommon-2.20.0/src/educommon/ws_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/base.py` & `educommon-2.20.0/src/educommon/ws_log/base.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0001_initial.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py` & `educommon-2.20.0/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/models.py` & `educommon-2.20.0/src/educommon/ws_log/models.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/provider.py` & `educommon-2.20.0/src/educommon/ws_log/provider.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/report.py` & `educommon-2.20.0/src/educommon/ws_log/report.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/smev/applications.py` & `educommon-2.20.0/src/educommon/ws_log/smev/applications.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/smev/exceptions.py` & `educommon-2.20.0/src/educommon/ws_log/smev/exceptions.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/templates/report/smev_logs.xlsx` & `educommon-2.20.0/src/educommon/ws_log/templates/report/smev_logs.xlsx`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js` & `educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js` & `educommon-2.20.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/ui.py` & `educommon-2.20.0/src/educommon/ws_log/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon/ws_log/utils.py` & `educommon-2.20.0/src/educommon/ws_log/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-2.19.3/src/educommon.egg-info/PKG-INFO` & `educommon-2.20.0/src/educommon.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 2.19.3
+Version: 2.20.0
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `educommon-2.19.3/src/educommon.egg-info/SOURCES.txt` & `educommon-2.20.0/src/educommon.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 src/educommon/async_tasks/migrations/0002_load_initial_data.py
 src/educommon/async_tasks/migrations/__init__.py
 src/educommon/audit_log/__init__.py
 src/educommon/audit_log/actions.py
 src/educommon/audit_log/app_meta.py
 src/educommon/audit_log/apps.py
 src/educommon/audit_log/constants.py
+src/educommon/audit_log/helpers.py
 src/educommon/audit_log/middleware.py
 src/educommon/audit_log/models.py
 src/educommon/audit_log/permissions.py
 src/educommon/audit_log/proxies.py
 src/educommon/audit_log/routers.py
 src/educommon/audit_log/ui.py
 src/educommon/audit_log/error_log/__init__.py
@@ -177,14 +178,21 @@
 src/educommon/importer/proxy.py
 src/educommon/importer/proxy_import.py
 src/educommon/importer/refactoring-notes.txt
 src/educommon/importer/report.py
 src/educommon/importer/test_file.xls
 src/educommon/importer/ui.py
 src/educommon/importer/validators.py
+src/educommon/integration_entities/README.rst
+src/educommon/integration_entities/__init__.py
+src/educommon/integration_entities/consts.py
+src/educommon/integration_entities/entities.py
+src/educommon/integration_entities/enums.py
+src/educommon/integration_entities/helpers.py
+src/educommon/integration_entities/mixins.py
 src/educommon/ioc/__init__.py
 src/educommon/m3/__init__.py
 src/educommon/m3/transaction_context.py
 src/educommon/m3/extensions/__init__.py
 src/educommon/m3/extensions/ui.py
 src/educommon/m3/extensions/listeners/__init__.py
 src/educommon/m3/extensions/listeners/delete_check/__init__.py
@@ -253,19 +261,22 @@
 src/educommon/rest/misc.py
 src/educommon/rest/mixins.py
 src/educommon/secure_media/README.rst
 src/educommon/secure_media/__init__.py
 src/educommon/secure_media/app_meta.py
 src/educommon/utils/__init__.py
 src/educommon/utils/caching.py
+src/educommon/utils/conversion.py
+src/educommon/utils/crypto.py
 src/educommon/utils/date.py
 src/educommon/utils/misc.py
 src/educommon/utils/patches.py
 src/educommon/utils/plugins.py
 src/educommon/utils/registry.py
+src/educommon/utils/seqtools.py
 src/educommon/utils/serializer.py
 src/educommon/utils/storage.py
 src/educommon/utils/system.py
 src/educommon/utils/ui.py
 src/educommon/utils/db/__init__.py
 src/educommon/utils/db/postgresql.py
 src/educommon/utils/fonts/Arial.ttf
@@ -308,8 +319,21 @@
 src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
 src/educommon/ws_log/migrations/__init__.py
 src/educommon/ws_log/smev/__init__.py
 src/educommon/ws_log/smev/applications.py
 src/educommon/ws_log/smev/exceptions.py
 src/educommon/ws_log/templates/report/smev_logs.xlsx
 src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
-src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
+src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
+tests/test_contingent_plugin_utils.py
+tests/test_delete_check.py
+tests/test_delete_objects.py
+tests/test_django_db_utils.py
+tests/test_interval_mixins.py
+tests/test_patches.py
+tests/test_personal_data_fields.py
+tests/test_report.py
+tests/test_service_db_router.py
+tests/test_utils.py
+tests/test_utils_plugins.py
+tests/test_validators.py
+tests/tests_rbac.py
```

