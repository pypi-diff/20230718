# Comparing `tmp/netbox_config_backup-1.4.7.tar.gz` & `tmp/netbox_config_backup-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_config_backup-1.4.7.tar", last modified: Thu Jun 22 17:59:28 2023, max compression
+gzip compressed data, was "netbox_config_backup-1.4.8.tar", last modified: Tue Jul 18 16:25:48 2023, max compression
```

## Comparing `netbox_config_backup-1.4.7.tar` & `netbox_config_backup-1.4.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.301155 netbox_config_backup-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-22 17:59:28.301155 netbox_config_backup-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.293155 netbox_config_backup-1.4.7/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.297155 netbox_config_backup-1.4.7/netbox_config_backup/api/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.297155 netbox_config_backup-1.4.7/netbox_config_backup/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.297155 netbox_config_backup-1.4.7/netbox_config_backup/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/management/commands/enqueue_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/management/commands/fix_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/management/commands/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/management/commands/runbackup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.297155 netbox_config_backup-1.4.7/netbox_config_backup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0002_git_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0004_custom_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0005_commit_add_time_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0010_backup_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0011_alter_backup_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0012_backup_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.297155 netbox_config_backup-1.4.7/netbox_config_backup/models/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/models/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.293155 netbox_config_backup-1.4.7/netbox_config_backup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.301155 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/backup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/backups.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/diff.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.301155 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/repository.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.301155 netbox_config_backup-1.4.7/netbox_config_backup/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/templatetags/ncb_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.301155 netbox_config_backup-1.4.7/netbox_config_backup/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/utils/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/utils/rq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/netbox_config_backup/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:59:28.293155 netbox_config_backup-1.4.7/netbox_config_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-22 17:59:28.000000 netbox_config_backup-1.4.7/netbox_config_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-22 17:59:28.000000 netbox_config_backup-1.4.7/netbox_config_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:59:28.000000 netbox_config_backup-1.4.7/netbox_config_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:59:28.000000 netbox_config_backup-1.4.7/netbox_config_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-22 17:59:28.000000 netbox_config_backup-1.4.7/netbox_config_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 17:59:28.000000 netbox_config_backup-1.4.7/netbox_config_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 17:59:28.301155 netbox_config_backup-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-22 17:59:19.000000 netbox_config_backup-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.810246 netbox_config_backup-1.4.8/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.810246 netbox_config_backup-1.4.8/netbox_config_backup/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.810246 netbox_config_backup-1.4.8/netbox_config_backup/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.810246 netbox_config_backup-1.4.8/netbox_config_backup/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/management/commands/enqueue_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/management/commands/fix_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/management/commands/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/management/commands/runbackup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/netbox_config_backup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0002_git_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0004_custom_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0005_commit_add_time_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0010_backup_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0011_alter_backup_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0012_backup_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/netbox_config_backup/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/models/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.806246 netbox_config_backup-1.4.8/netbox_config_backup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/backup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/backups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/diff.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/repository.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/netbox_config_backup/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/templatetags/ncb_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/netbox_config_backup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/utils/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/utils/rq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/netbox_config_backup/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:25:48.810246 netbox_config_backup-1.4.8/netbox_config_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-18 16:25:48.000000 netbox_config_backup-1.4.8/netbox_config_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-18 16:25:48.000000 netbox_config_backup-1.4.8/netbox_config_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:25:48.000000 netbox_config_backup-1.4.8/netbox_config_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:25:48.000000 netbox_config_backup-1.4.8/netbox_config_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 16:25:48.000000 netbox_config_backup-1.4.8/netbox_config_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 16:25:48.000000 netbox_config_backup-1.4.8/netbox_config_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:25:48.814246 netbox_config_backup-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-18 16:25:41.000000 netbox_config_backup-1.4.8/setup.py
```

### Comparing `netbox_config_backup-1.4.7/LICENSE` & `netbox_config_backup-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/PKG-INFO` & `netbox_config_backup-1.4.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_config_backup
-Version: 1.4.7
+Version: 1.4.8
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.7/README.md` & `netbox_config_backup-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/__init__.py` & `netbox_config_backup-1.4.8/netbox_config_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/api/serializers.py` & `netbox_config_backup-1.4.8/netbox_config_backup/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/choices.py` & `netbox_config_backup-1.4.8/netbox_config_backup/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/filtersets.py` & `netbox_config_backup-1.4.8/netbox_config_backup/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/forms.py` & `netbox_config_backup-1.4.8/netbox_config_backup/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/git.py` & `netbox_config_backup-1.4.8/netbox_config_backup/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def __init__(self):
         self.location = get_repository_dir()
 
         if os.path.exists(self.location):
             self.repository = repo.Repo(self.location)
 
         if self.repository is None:
-            self.repository = repo.Repo.init(self.location, True)
+            self.repository = repo.Repo.init(path=self.location, mkdir=True)
 
         if self.repository is not None:
             try:
                 self.driller = Git(self.location)
             except OSError:
                 pass
```

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/management/commands/fix_missing.py` & `netbox_config_backup-1.4.8/netbox_config_backup/management/commands/fix_missing.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/management/commands/rebuild.py` & `netbox_config_backup-1.4.8/netbox_config_backup/management/commands/rebuild.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/management/commands/runbackup.py` & `netbox_config_backup-1.4.8/netbox_config_backup/management/commands/runbackup.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0001_initial.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0002_git_models.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0002_git_models.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0003_primary_model_to_bigid.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0003_primary_model_to_bigid.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0010_backup_ip.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0010_backup_ip.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py` & `netbox_config_backup-1.4.8/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/models/backups.py` & `netbox_config_backup-1.4.8/netbox_config_backup/models/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/models/jobs.py` & `netbox_config_backup-1.4.8/netbox_config_backup/models/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/navigation.py` & `netbox_config_backup-1.4.8/netbox_config_backup/navigation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from extras.plugins import PluginMenuItem, PluginMenuButton, PluginMenu
 from utilities.choices import ButtonColorChoices
 
-item = PluginMenuItem(
+assigned = PluginMenuItem(
     link='plugins:netbox_config_backup:backup_list',
     link_text='Devices',
     permissions=['netbox_config_backup.view_backups'],
     buttons=[
         PluginMenuButton(
             link="plugins:netbox_config_backup:backup_add",
             title="Add",
             icon_class="mdi mdi-plus",
             color=ButtonColorChoices.GREEN,
         ),
     ]
 )
 
+unassigned = PluginMenuItem(
+    link='plugins:netbox_config_backup:unassignedbackup_list',
+    link_text='Unassigned Backups',
+    permissions=['netbox_config_backup.view_backups'],
+    buttons=[]
+)
+
 menu = PluginMenu(
     label="Configuration Backup",
     groups=(
-        ('Backup Jobs', (item,)),
+        ('Backup Jobs', (assigned, unassigned)),
     )
 )
```

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/tables.py` & `netbox_config_backup-1.4.8/netbox_config_backup/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/tasks.py` & `netbox_config_backup-1.4.8/netbox_config_backup/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import sys
 import traceback
 from datetime import timedelta
 
 from django.utils import timezone
 from django_rq import job
+from netmiko import NetmikoAuthenticationException, NetmikoTimeoutException
 
 from extras.choices import JobResultStatusChoices
 from netbox import settings
 from netbox.api.exceptions import ServiceUnavailable
 from netbox.config import get_config
 from netbox_config_backup.models import Backup, BackupJob, BackupCommit
 
@@ -26,15 +27,15 @@
 
 def napalm_init(device, ip=None, extra_args={}):
     config = get_config()
     username = config.NAPALM_USERNAME
     password = config.NAPALM_PASSWORD
     timeout = config.NAPALM_TIMEOUT
     optional_args = config.NAPALM_ARGS.copy()
-    if device.platform.napalm_args is not None:
+    if device and device.platform and device.platform.napalm_args is not None:
         optional_args.update(device.platform.napalm_args)
     if extra_args != {}:
         optional_args.update(extra_args)
 
     # Check for primary IP address from NetBox object
     if ip is not None:
         host = str(ip.address.ip)
@@ -69,14 +70,18 @@
         password=password,
         timeout=timeout,
         optional_args=optional_args
     )
     try:
         d.open()
     except Exception as e:
+        if isinstance(e, NetmikoAuthenticationException):
+            logger.info('Authentication error')
+        elif isinstance(e, NetmikoTimeoutException):
+            logger.info('Connection error')
         raise ServiceUnavailable("Error connecting to the device at {}: {}".format(host, e))
 
     return d
 
 
 def backup_config(backup, pk=None):
     commit = None
@@ -135,18 +140,19 @@
         except Exception as e:
             logger.error(f'Job Enqueue after completion failed for job: {backup}')
             logger.error(f'\tException: {e}')
     except netmiko.exceptions.ReadTimeout as e:
         BackupJob.enqueue_if_needed(backup, delay=delay, job_id=job_result.job_id)
         logger.error(f'Netmiko read timeout on job: {backup}')
     except ServiceUnavailable as e:
-        logger.error(f'Napalm service read failure on job: {backup}')
+        logger.info(f'Napalm service read failure on job: {backup}')
         BackupJob.enqueue_if_needed(backup, delay=delay, job_id=job_result.job_id)
     except Exception as e:
         logger.error(f'Exception at line 148 on job: {backup}')
+        logger.error(e.with_traceback())
         job_result.set_status(JobResultStatusChoices.STATUS_FAILED)
         BackupJob.enqueue_if_needed(backup, delay=delay, job_id=job_result.job_id)
 
     #logger.debug(f'[{pk}] Saving result')
     job_result.save()
 
     # Clear queue of old jobs
```

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/template_content.py` & `netbox_config_backup-1.4.8/netbox_config_backup/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/backup.html` & `netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/backup.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/backups.html` & `netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/backups.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/templates/netbox_config_backup/diff.html` & `netbox_config_backup-1.4.8/netbox_config_backup/templates/netbox_config_backup/diff.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/urls.py` & `netbox_config_backup-1.4.8/netbox_config_backup/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.urls import path
 from . import views
 
 urlpatterns = [
+    path('unassigned/', views.UnassignedBackupListView.as_view(), name='unassignedbackup_list'),
     path('devices/', views.BackupListView.as_view(), name='backup_list'),
     path('devices/add/', views.BackupEditView.as_view(), name='backup_add'),
     path('devices/<int:pk>/', views.BackupView.as_view(), name='backup'),
     path('devices/<int:pk>/edit/', views.BackupEditView.as_view(), name='backup_edit'),
     path('devices/<int:pk>/delete/', views.BackupDeleteView.as_view(), name='backup_delete'),
     path('devices/<int:pk>/backups/', views.BackupBackupsView.as_view(), name='backup_backups'),
     path('devices/<int:pk>/config/', views.ConfigView.as_view(), name='backup_config'),
```

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/utils/backups.py` & `netbox_config_backup-1.4.8/netbox_config_backup/utils/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/utils/git.py` & `netbox_config_backup-1.4.8/netbox_config_backup/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/utils/rq.py` & `netbox_config_backup-1.4.8/netbox_config_backup/utils/rq.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup/views.py` & `netbox_config_backup-1.4.8/netbox_config_backup/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,27 @@
 from netbox_config_backup.utils import get_backup_tables, Differ
 from utilities.views import register_model_view, ViewTab
 
 logger = logging.getLogger(f"netbox_config_backup")
 
 
 class BackupListView(ObjectListView):
-    queryset = Backup.objects.all()
+    queryset = Backup.objects.filter(device__isnull=False)
+    filterset = BackupFilterSet
+    filterset_form = BackupFilterSetForm
+    table = BackupTable
+    action_buttons = ('add', )
+
+
+class UnassignedBackupListView(ObjectListView):
+    queryset = Backup.objects.filter(device__isnull=True)
     filterset = BackupFilterSet
     filterset_form = BackupFilterSetForm
     table = BackupTable
-    action_buttons = ('add',)
+    action_buttons = ()
 
 
 @register_model_view(Backup)
 class BackupView(ObjectView):
     queryset = Backup.objects.all()
     template_name = 'netbox_config_backup/backup.html'
```

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup.egg-info/PKG-INFO` & `netbox_config_backup-1.4.8/netbox_config_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-backup
-Version: 1.4.7
+Version: 1.4.8
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.7/netbox_config_backup.egg-info/SOURCES.txt` & `netbox_config_backup-1.4.8/netbox_config_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.7/setup.py` & `netbox_config_backup-1.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox_config_backup',
-    version='1.4.7',
+    version='1.4.8',
     description='NetBox Configuration Backup',
     long_description='Plugin to backup device configuration',
     url='https://github.com/dansheps/netbox-config-backup/',
     download_url='https://github.com/dansheps/netbox-config-backup/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

