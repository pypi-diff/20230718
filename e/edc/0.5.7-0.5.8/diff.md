# Comparing `tmp/edc-0.5.7.tar.gz` & `tmp/edc-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.5.7.tar", last modified: Wed Jul 12 23:55:50 2023, max compression
+gzip compressed data, was "edc-0.5.8.tar", last modified: Tue Jul 18 02:12:34 2023, max compression
```

## Comparing `edc-0.5.7.tar` & `edc-0.5.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.245848 edc-0.5.7/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    42694 2023-07-12 23:55:42.000000 edc-0.5.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-12 23:55:50.245972 edc-0.5.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37646 2023-07-12 23:55:42.000000 edc-0.5.7/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.231897 edc-0.5.7/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.235007 edc-0.5.7/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.7/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.7/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.7/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.235732 edc-0.5.7/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.7/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.7/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.7/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.7/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.237049 edc-0.5.7/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.241351 edc-0.5.7/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.7/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.7/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.7/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.7/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.7/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.7/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.7/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.7/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.7/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.7/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.7/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.7/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.7/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.7/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.7/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.7/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.7/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.7/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.7/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.242277 edc-0.5.7/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.7/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.242378 edc-0.5.7/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.7/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.7/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.245319 edc-0.5.7/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.7/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.7/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.7/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.7/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.7/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.7/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.7/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.7/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.7/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.7/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.7/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2959 2023-07-12 23:55:50.246368 edc-0.5.7/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.245622 edc-0.5.7/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.7/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.7/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.871976 edc-0.5.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    42968 2023-07-18 02:12:25.000000 edc-0.5.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-18 02:12:34.872106 edc-0.5.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37646 2023-07-12 23:55:42.000000 edc-0.5.8/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.858391 edc-0.5.8/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.860989 edc-0.5.8/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.8/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.8/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.8/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.861816 edc-0.5.8/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.8/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.8/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.8/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.8/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.863085 edc-0.5.8/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.867430 edc-0.5.8/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.8/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.8/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.8/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.8/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.8/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.8/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.8/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.8/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.8/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.8/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.8/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.8/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.8/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.8/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.8/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.8/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.8/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.8/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.8/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.868381 edc-0.5.8/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.8/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.868514 edc-0.5.8/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.8/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.8/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.871418 edc-0.5.8/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.8/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.8/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.8/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.8/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.8/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.8/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.8/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.8/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.8/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.8/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.8/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2959 2023-07-18 02:12:34.872485 edc-0.5.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.871742 edc-0.5.8/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.8/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.8/utils/get_edc_requirements.py
```

### Comparing `edc-0.5.7/.gitignore` & `edc-0.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/.pre-commit-config.yaml` & `edc-0.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/CHANGES` & `edc-0.5.8/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 -------
 
+0.5.8
+-----
+- use SQLAlchemy to prepare sql text for pandas, upgrade pandas
+  to latest, require SQLAlchemy (edc-pdutils)
+- typing hints (edc-pdutils, edc-export)
+- check settings before loading load_data (edc-list-data)
+- add func to get all sites for country (edc-sites)
+
 0.5.7
 -----
 - change field `return_in_days` to `rx_days` (edc-rx)
 
 0.5.6
 -----
 - major refactor; eliminated use of TargetHandler classes; removed
```

### Comparing `edc-0.5.7/LICENSE` & `edc-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/PKG-INFO` & `edc-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.7
+Version: 0.5.8
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.7/README.rst` & `edc-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/bin/nginx/edc-uat.conf` & `edc-0.5.8/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/bin/nginx/edc.conf` & `edc-0.5.8/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/bin/scripts/dev_repos.sh` & `edc-0.5.8/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/bin/scripts/update_edc.sh` & `edc-0.5.8/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/bin/systemd/celery-uat.service` & `edc-0.5.8/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/bin/systemd/celery.service` & `edc-0.5.8/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/Makefile` & `edc-0.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/README.rst` & `edc-0.5.8/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/backup.rst` & `edc-0.5.8/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/celery.rst` & `edc-0.5.8/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/conda.rst` & `edc-0.5.8/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/conf.py` & `edc-0.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/configure_web_services.rst` & `edc-0.5.8/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/deploy_new_droplet.rst` & `edc-0.5.8/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/exporting_encrypted_data.rst` & `edc-0.5.8/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/forms_reference.md` & `edc-0.5.8/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/landing_page.rst` & `edc-0.5.8/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/make.bat` & `edc-0.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/prepare_database.rst` & `edc-0.5.8/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/printing.rst` & `edc-0.5.8/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/docs/update_deployment.rst` & `edc-0.5.8/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/edc.egg-info/PKG-INFO` & `edc-0.5.8/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.7
+Version: 0.5.8
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.7/edc.egg-info/SOURCES.txt` & `edc-0.5.8/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/edc.egg-info/requires.txt` & `edc-0.5.8/edc.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,44 +33,44 @@
 edc-dashboard==0.3.45
 edc-data-manager==0.3.56
 edc-device==0.3.11
 edc-document-status==0.1.4
 edc-dx==0.1.20
 edc-dx-review==0.1.39
 edc-egfr==0.1.11
-edc-export==0.3.27
+edc-export==0.3.28
 edc-facility==0.3.15
 edc-fieldsets==0.3.13
 edc-form-describer==0.3.16
 edc-form-label==0.3.9
 edc-form-validators==0.3.34
 edc-glucose==0.1.30
 edc-he==0.1.8
 edc-identifier==0.3.24
 edc-lab==0.3.44
 edc-lab-dashboard==0.3.11
 edc-lab-panel==0.1.15
 edc-lab-results==0.1.38
 edc-label==0.3.13
-edc-list-data==0.3.18
+edc-list-data==0.3.19
 edc-listboard==0.1.11
 edc-locator==0.3.24
 edc-ltfu==0.3.24
 edc-metadata==0.3.54
 edc-mnsi==0.1.17
 edc-model==0.3.32
 edc-model-admin==0.3.47
 edc-model-fields==0.3.7
 edc-model-form==0.1.12
 edc-model-wrapper==0.3.10
 edc-navbar==0.3.16
 edc-notification==0.3.18
 edc-offstudy==0.3.33
-edc-pdf-reports==0.3.13
-edc-pdutils==0.3.22
+edc-pdf-reports==0.3.14
+edc-pdutils==0.3.23
 edc-pharmacy==0.1.39
 edc-pharmacy-dashboard==0.1.3
 edc-prn==0.3.13
 edc-protocol==0.3.9
 edc-protocol-incident==0.1.26
 edc-qol==0.1.15
 edc-randomization==0.3.47
@@ -78,15 +78,15 @@
 edc-refusal==0.1.13
 edc-registration==0.3.30
 edc-reportable==0.3.31
 edc-review-dashboard==0.3.19
 edc-rx==0.1.7
 edc-screening==0.3.35
 edc-search==0.3.7
-edc-sites==0.3.25
+edc-sites==0.3.26
 edc-subject-dashboard==0.3.38
 edc-subject-model-wrappers==0.3.15
 edc-timepoint==0.3.11
 edc-transfer==0.3.14
 edc-unblinding==0.1.15
 edc-utils==0.3.20
 edc-visit-schedule==0.3.62
```

### Comparing `edc-0.5.7/image/icon-pycharm.png` & `edc-0.5.8/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/requirements.tests/edc.txt` & `edc-0.5.8/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/requirements.tests/edc_dev.txt` & `edc-0.5.8/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.7/setup.cfg` & `edc-0.5.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -61,44 +61,44 @@
 	edc-dashboard==0.3.45
 	edc-data-manager==0.3.56
 	edc-device==0.3.11
 	edc-document-status==0.1.4
 	edc-dx==0.1.20
 	edc-dx-review==0.1.39
 	edc-egfr==0.1.11
-	edc-export==0.3.27
+	edc-export==0.3.28
 	edc-facility==0.3.15
 	edc-fieldsets==0.3.13
 	edc-form-describer==0.3.16
 	edc-form-label==0.3.9
 	edc-form-validators==0.3.34
 	edc-glucose==0.1.30
 	edc-he==0.1.8
 	edc-identifier==0.3.24
 	edc-lab==0.3.44
 	edc-lab-dashboard==0.3.11
 	edc-lab-panel==0.1.15
 	edc-lab-results==0.1.38
 	edc-label==0.3.13
-	edc-list-data==0.3.18
+	edc-list-data==0.3.19
 	edc-listboard==0.1.11
 	edc-locator==0.3.24
 	edc-ltfu==0.3.24
 	edc-metadata==0.3.54
 	edc-mnsi==0.1.17
 	edc-model==0.3.32
 	edc-model-admin==0.3.47
 	edc-model-fields==0.3.7
 	edc-model-form==0.1.12
 	edc-model-wrapper==0.3.10
 	edc-navbar==0.3.16
 	edc-notification==0.3.18
 	edc-offstudy==0.3.33
-	edc-pdf-reports==0.3.13
-	edc-pdutils==0.3.22
+	edc-pdf-reports==0.3.14
+	edc-pdutils==0.3.23
 	edc-pharmacy==0.1.39
 	edc-pharmacy-dashboard==0.1.3
 	edc-prn==0.3.13
 	edc-protocol==0.3.9
 	edc-protocol-incident==0.1.26
 	edc-qol==0.1.15
 	edc-randomization==0.3.47
@@ -106,15 +106,15 @@
 	edc-refusal==0.1.13
 	edc-registration==0.3.30
 	edc-reportable==0.3.31
 	edc-review-dashboard==0.3.19
 	edc-rx==0.1.7
 	edc-screening==0.3.35
 	edc-search==0.3.7
-	edc-sites==0.3.25
+	edc-sites==0.3.26
 	edc-subject-dashboard==0.3.38
 	edc-subject-model-wrappers==0.3.15
 	edc-timepoint==0.3.11
 	edc-transfer==0.3.14
 	edc-unblinding==0.1.15
 	edc-utils==0.3.20
 	edc-visit-schedule==0.3.62
```

### Comparing `edc-0.5.7/utils/get_edc_requirements.py` & `edc-0.5.8/utils/get_edc_requirements.py`

 * *Files identical despite different names*

