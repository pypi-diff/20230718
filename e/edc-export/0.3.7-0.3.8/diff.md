# Comparing `tmp/edc-export-0.3.7.tar.gz` & `tmp/edc-export-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-export-0.3.7.tar", last modified: Wed Feb 16 00:23:14 2022, max compression
+gzip compressed data, was "edc-export-0.3.8.tar", last modified: Wed May 25 11:30:13 2022, max compression
```

## Comparing `edc-export-0.3.7.tar` & `edc-export-0.3.8.tar`

### file list

```diff
@@ -1,111 +1,133 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.999383 edc-export-0.3.7/
--rw-r--r--   0 erikvw     (501) staff       (20)      222 2020-03-04 22:53:05.000000 edc-export-0.3.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1363 2022-02-16 00:23:13.999464 edc-export-0.3.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      623 2021-02-08 23:37:32.000000 edc-export-0.3.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-02-16 00:23:01.000000 edc-export-0.3.7/VERSION
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.988908 edc-export-0.3.7/edc_export/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.990833 edc-export-0.3.7/edc_export/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1417 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/data_request_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1320 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/data_request_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      454 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/export_receipt_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/file_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      715 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/object_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/plan_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      520 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/admin/upload_export_receipt_file_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-05-16 19:56:00.000000 edc-export-0.3.7/edc_export/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1251 2021-04-23 11:28:44.000000 edc-export-0.3.7/edc_export/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2573 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/archive_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1454 2021-09-14 02:02:53.000000 edc-export-0.3.7/edc_export/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      222 2021-09-14 02:02:53.000000 edc-export-0.3.7/edc_export/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-02-16 00:23:01.000000 edc-export-0.3.7/edc_export/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2021-01-25 02:18:04.000000 edc-export-0.3.7/edc_export/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4921 2021-09-14 02:02:53.000000 edc-export-0.3.7/edc_export/exportables.py
--rw-r--r--   0 erikvw     (501) staff       (20)      694 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/files_archiver.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3157 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/files_emailer.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.991106 edc-export-0.3.7/edc_export/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)       47 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      925 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/forms/data_request_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.991318 edc-export-0.3.7/edc_export/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.991688 edc-export-0.3.7/edc_export/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      837 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/management/commands/export_object_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4642 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/management/commands/import_receipts.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1203 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/managers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.993650 edc-export-0.3.7/edc_export/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    59335 2021-04-23 11:28:44.000000 edc-export-0.3.7/edc_export/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      496 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/migrations/0002_auto_20180922_1843.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1521 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/migrations/0003_auto_20181108_0353.py
--rw-r--r--   0 erikvw     (501) staff       (20)    19594 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/migrations/0004_auto_20190305_0123.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1294 2021-09-11 18:17:23.000000 edc-export-0.3.7/edc_export/migrations/0005_exportdata_importdata.py
--rw-r--r--   0 erikvw     (501) staff       (20)      870 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/migrations/0006_auto_20200512_0208.py
--rw-r--r--   0 erikvw     (501) staff       (20)      674 2020-05-12 20:38:52.000000 edc-export-0.3.7/edc_export/migrations/0007_auto_20200512_0452.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1300 2021-01-25 02:18:04.000000 edc-export-0.3.7/edc_export/migrations/0008_auto_20201002_0403.py
--rw-r--r--   0 erikvw     (501) staff       (20)      722 2021-05-16 19:56:00.000000 edc-export-0.3.7/edc_export/migrations/0009_auto_20210510_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)      582 2021-09-11 18:17:23.000000 edc-export-0.3.7/edc_export/migrations/0010_auto_20210910_1636.py
--rw-r--r--   0 erikvw     (501) staff       (20)      938 2022-02-16 00:23:01.000000 edc-export-0.3.7/edc_export/migrations/0011_auto_20220215_2308.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.994625 edc-export-0.3.7/edc_export/model_exporter/
--rw-r--r--   0 erikvw     (501) staff       (20)      235 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/model_exporter/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1290 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/model_exporter/file_history_updater.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6291 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/model_exporter/model_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3762 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/model_exporter/object_history_helpers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1143 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/model_exporter/plan_exporter.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.995362 edc-export-0.3.7/edc_export/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      205 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1181 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/model_mixins/export_tracking_fields_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      717 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/model_mixins/notification_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      379 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/model_mixins/notification_plan_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1429 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/model_options.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.996703 edc-export-0.3.7/edc_export/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      511 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1188 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/models/data_request.py
--rw-r--r--   0 erikvw     (501) staff       (20)      742 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/models/data_request_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)      889 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/models/export_receipt.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2353 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/models/file_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)      369 2021-09-11 18:17:23.000000 edc-export-0.3.7/edc_export/models/import_export.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2276 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/models/object_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1721 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/models/plan.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2530 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/models/upload_export_receipt_file.py
--rw-r--r--   0 erikvw     (501) staff       (20)      565 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)      384 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/offline_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1282 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/signals.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.983970 edc-export-0.3.7/edc_export/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.996957 edc-export-0.3.7/edc_export/static/edc_export/
--rw-r--r--   0 erikvw     (501) staff       (20)      995 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/static/edc_export/edc.css
--rw-r--r--   0 erikvw     (501) staff       (20)      553 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/static/edc_export/edc.js
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.984060 edc-export-0.3.7/edc_export/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.984099 edc-export-0.3.7/edc_export/templates/edc_export/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.997237 edc-export-0.3.7/edc_export/templates/edc_export/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)     5341 2021-01-25 02:18:04.000000 edc-export-0.3.7/edc_export/templates/edc_export/bootstrap3/export_models.html
--rw-r--r--   0 erikvw     (501) staff       (20)      871 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/templates/edc_export/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.997892 edc-export-0.3.7/edc_export/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4569 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/tests/helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4380 2021-09-11 18:17:23.000000 edc-export-0.3.7/edc_export/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.998770 edc-export-0.3.7/edc_export/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-28 03:09:28.000000 edc-export-0.3.7/edc_export/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1821 2021-07-28 03:09:28.000000 edc-export-0.3.7/edc_export/tests/tests/test_archive_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14337 2021-07-28 03:09:28.000000 edc-export-0.3.7/edc_export/tests/tests/test_export_model.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3331 2021-07-28 03:09:28.000000 edc-export-0.3.7/edc_export/tests/tests/test_exportable.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4464 2021-07-28 03:09:28.000000 edc-export-0.3.7/edc_export/tests/tests/test_model_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1106 2021-07-28 03:09:28.000000 edc-export-0.3.7/edc_export/tests/tests/test_plan.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3365 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-07-17 20:05:24.000000 edc-export-0.3.7/edc_export/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.999259 edc-export-0.3.7/edc_export/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      147 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1048 2020-06-15 03:07:39.000000 edc-export-0.3.7/edc_export/views/export_models_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6905 2021-02-08 23:37:32.000000 edc-export-0.3.7/edc_export/views/export_selected_models_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      497 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export/views/home_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-02-16 00:23:13.989664 edc-export-0.3.7/edc_export.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1363 2022-02-16 00:23:13.000000 edc-export-0.3.7/edc_export.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     3260 2022-02-16 00:23:13.000000 edc-export-0.3.7/edc_export.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-02-16 00:23:13.000000 edc-export-0.3.7/edc_export.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:53:05.000000 edc-export-0.3.7/edc_export.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-02-16 00:23:13.000000 edc-export-0.3.7/edc_export.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      344 2021-02-08 23:37:32.000000 edc-export-0.3.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:51:04.000000 edc-export-0.3.7/requirements.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-02-16 00:23:13.999723 edc-export-0.3.7/setup.cfg
--rw-r--r--   0 erikvw     (501) staff       (20)     1325 2022-02-16 00:23:01.000000 edc-export-0.3.7/setup.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.239953 edc-export-0.3.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       90 2021-02-08 23:37:32.000000 edc-export-0.3.8/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 23:37:32.000000 edc-export-0.3.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.221037 edc-export-0.3.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.224876 edc-export-0.3.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-export-0.3.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      932 2022-05-25 11:26:35.000000 edc-export-0.3.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-05-25 11:26:35.000000 edc-export-0.3.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)      913 2022-05-25 11:26:35.000000 edc-export-0.3.8/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)     1343 2022-05-25 11:30:13.240025 edc-export-0.3.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      623 2021-02-08 23:37:32.000000 edc-export-0.3.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-05-25 11:30:05.000000 edc-export-0.3.8/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      200 2022-05-25 11:30:04.000000 edc-export-0.3.8/_version.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-08 23:37:32.000000 edc-export-0.3.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.227599 edc-export-0.3.8/edc_export/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.229357 edc-export-0.3.8/edc_export/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1417 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/data_request_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1320 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/data_request_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      454 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/export_receipt_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/file_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      715 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/object_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/plan_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      520 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/admin/upload_export_receipt_file_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-05-16 19:56:00.000000 edc-export-0.3.8/edc_export/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1251 2022-05-25 11:26:35.000000 edc-export-0.3.8/edc_export/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2573 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/archive_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1454 2021-09-14 02:02:53.000000 edc-export-0.3.8/edc_export/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2021-09-14 02:02:53.000000 edc-export-0.3.8/edc_export/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2022-02-16 00:23:01.000000 edc-export-0.3.8/edc_export/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2021-01-25 02:18:04.000000 edc-export-0.3.8/edc_export/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4921 2021-09-14 02:02:53.000000 edc-export-0.3.8/edc_export/exportables.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      694 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/files_archiver.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3157 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/files_emailer.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.229614 edc-export-0.3.8/edc_export/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)       47 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      925 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/forms/data_request_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.229770 edc-export-0.3.8/edc_export/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.230128 edc-export-0.3.8/edc_export/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      837 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/management/commands/export_object_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4642 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/management/commands/import_receipts.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1203 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/managers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.232712 edc-export-0.3.8/edc_export/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    59335 2022-05-25 11:27:43.000000 edc-export-0.3.8/edc_export/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      496 2022-05-25 11:27:45.000000 edc-export-0.3.8/edc_export/migrations/0002_auto_20180922_1843.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1521 2022-05-25 11:27:48.000000 edc-export-0.3.8/edc_export/migrations/0003_auto_20181108_0353.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    19594 2022-05-25 11:27:51.000000 edc-export-0.3.8/edc_export/migrations/0004_auto_20190305_0123.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1294 2022-05-25 11:27:53.000000 edc-export-0.3.8/edc_export/migrations/0005_exportdata_importdata.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      870 2022-05-25 11:27:57.000000 edc-export-0.3.8/edc_export/migrations/0006_auto_20200512_0208.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      674 2022-05-25 11:28:00.000000 edc-export-0.3.8/edc_export/migrations/0007_auto_20200512_0452.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1300 2022-05-25 11:28:04.000000 edc-export-0.3.8/edc_export/migrations/0008_auto_20201002_0403.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      722 2022-05-25 11:28:06.000000 edc-export-0.3.8/edc_export/migrations/0009_auto_20210510_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      642 2022-05-25 11:30:04.000000 edc-export-0.3.8/edc_export/migrations/0010_auto_20210910_1636.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1302 2022-05-25 11:30:04.000000 edc-export-0.3.8/edc_export/migrations/0011_auto_20220215_2308.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.233556 edc-export-0.3.8/edc_export/model_exporter/
+-rw-r--r--   0 erikvw     (501) staff       (20)      235 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/model_exporter/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1290 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/model_exporter/file_history_updater.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6291 2022-05-25 11:26:35.000000 edc-export-0.3.8/edc_export/model_exporter/model_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3762 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/model_exporter/object_history_helpers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1143 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/model_exporter/plan_exporter.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.234317 edc-export-0.3.8/edc_export/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      205 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1181 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/model_mixins/export_tracking_fields_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      717 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/model_mixins/notification_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/model_mixins/notification_plan_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1429 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/model_options.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.235869 edc-export-0.3.8/edc_export/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      511 2022-05-25 11:26:35.000000 edc-export-0.3.8/edc_export/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1188 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/models/data_request.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      742 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/models/data_request_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      889 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/models/export_receipt.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2353 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/models/file_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      369 2021-09-11 18:17:23.000000 edc-export-0.3.8/edc_export/models/import_export.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2276 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/models/object_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1721 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/models/plan.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2530 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/models/upload_export_receipt_file.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      565 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      384 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/offline_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-05-25 11:26:35.000000 edc-export-0.3.8/edc_export/signals.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.221700 edc-export-0.3.8/edc_export/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.236205 edc-export-0.3.8/edc_export/static/edc_export/
+-rw-r--r--   0 erikvw     (501) staff       (20)      995 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/static/edc_export/edc.css
+-rw-r--r--   0 erikvw     (501) staff       (20)      553 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/static/edc_export/edc.js
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.221811 edc-export-0.3.8/edc_export/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.221849 edc-export-0.3.8/edc_export/templates/edc_export/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.236512 edc-export-0.3.8/edc_export/templates/edc_export/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5341 2021-01-25 02:18:04.000000 edc-export-0.3.8/edc_export/templates/edc_export/bootstrap3/export_models.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      871 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/templates/edc_export/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.237313 edc-export-0.3.8/edc_export/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.238425 edc-export-0.3.8/edc_export/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     4569 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/tests/helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     4380 2021-09-11 18:17:23.000000 edc-export-0.3.8/edc_export/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.239257 edc-export-0.3.8/edc_export/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-28 03:09:28.000000 edc-export-0.3.8/edc_export/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1821 2022-05-25 11:26:35.000000 edc-export-0.3.8/edc_export/tests/tests/test_archive_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14337 2022-05-25 11:26:35.000000 edc-export-0.3.8/edc_export/tests/tests/test_export_model.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3331 2021-07-28 03:09:28.000000 edc-export-0.3.8/edc_export/tests/tests/test_exportable.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4464 2021-07-28 03:09:28.000000 edc-export-0.3.8/edc_export/tests/tests/test_model_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1106 2022-05-25 11:26:35.000000 edc-export-0.3.8/edc_export/tests/tests/test_plan.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3365 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-07-17 20:05:24.000000 edc-export-0.3.8/edc_export/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.239833 edc-export-0.3.8/edc_export/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      147 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1048 2020-06-15 03:07:39.000000 edc-export-0.3.8/edc_export/views/export_models_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6905 2021-02-08 23:37:32.000000 edc-export-0.3.8/edc_export/views/export_selected_models_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      497 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export/views/home_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 11:30:13.228311 edc-export-0.3.8/edc_export.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1343 2022-05-25 11:30:13.000000 edc-export-0.3.8/edc_export.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     3790 2022-05-25 11:30:13.000000 edc-export-0.3.8/edc_export.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-25 11:30:13.000000 edc-export-0.3.8/edc_export.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:53:05.000000 edc-export-0.3.8/edc_export.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-05-25 11:30:13.000000 edc-export-0.3.8/edc_export.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      808 2022-05-25 11:26:35.000000 edc-export-0.3.8/manage.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      344 2022-05-25 11:26:35.000000 edc-export-0.3.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 11:26:35.000000 edc-export-0.3.8/requirements.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2086 2021-05-16 19:56:01.000000 edc-export-0.3.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-05-25 11:30:13.240272 edc-export-0.3.8/setup.cfg
+-rw-r--r--   0 erikvw     (501) staff       (20)     1325 2022-05-25 11:26:35.000000 edc-export-0.3.8/setup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1368 2022-05-25 11:26:35.000000 edc-export-0.3.8/tox.ini
```

### Comparing `edc-export-0.3.7/PKG-INFO` & `edc-export-0.3.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edc-export
-Version: 0.3.7
+Version: 0.3.8
 Summary: Export from in the clinicedc/edc.
 Home-page: https://github.com/clinicedc/edc-export
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc export
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -34,9 +33,7 @@
 
 .. |codecov| image:: https://codecov.io/gh/clinicedc/edc-export/branch/develop/graph/badge.svg
   :target: https://codecov.io/gh/clinicedc/edc-export
 
 .. |downloads| image:: https://pepy.tech/badge/edc-export
    :target: https://pepy.tech/project/edc-export
 
-
-
```

### Comparing `edc-export-0.3.7/README.rst` & `edc-export-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/admin/data_request_admin.py` & `edc-export-0.3.8/edc_export/admin/data_request_admin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/admin/data_request_history_admin.py` & `edc-export-0.3.8/edc_export/admin/data_request_history_admin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/admin/file_history_admin.py` & `edc-export-0.3.8/edc_export/admin/file_history_admin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/admin/object_history_admin.py` & `edc-export-0.3.8/edc_export/admin/object_history_admin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/admin/plan_admin.py` & `edc-export-0.3.8/edc_export/admin/plan_admin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/admin/upload_export_receipt_file_admin.py` & `edc-export-0.3.8/edc_export/admin/upload_export_receipt_file_admin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/apps.py` & `edc-export-0.3.8/edc_export/apps.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/archive_exporter.py` & `edc-export-0.3.8/edc_export/archive_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/auth_objects.py` & `edc-export-0.3.8/edc_export/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/exportables.py` & `edc-export-0.3.8/edc_export/exportables.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/files_archiver.py` & `edc-export-0.3.8/edc_export/files_archiver.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/files_emailer.py` & `edc-export-0.3.8/edc_export/files_emailer.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/forms/data_request_form.py` & `edc-export-0.3.8/edc_export/forms/data_request_form.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/management/commands/export_object_history.py` & `edc-export-0.3.8/edc_export/management/commands/export_object_history.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/management/commands/import_receipts.py` & `edc-export-0.3.8/edc_export/management/commands/import_receipts.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/managers.py` & `edc-export-0.3.8/edc_export/managers.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0001_initial.py` & `edc-export-0.3.8/edc_export/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0003_auto_20181108_0353.py` & `edc-export-0.3.8/edc_export/migrations/0003_auto_20181108_0353.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0004_auto_20190305_0123.py` & `edc-export-0.3.8/edc_export/migrations/0004_auto_20190305_0123.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0005_exportdata_importdata.py` & `edc-export-0.3.8/edc_export/migrations/0005_exportdata_importdata.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0006_auto_20200512_0208.py` & `edc-export-0.3.8/edc_export/migrations/0006_auto_20200512_0208.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0007_auto_20200512_0452.py` & `edc-export-0.3.8/edc_export/migrations/0007_auto_20200512_0452.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0008_auto_20201002_0403.py` & `edc-export-0.3.8/edc_export/migrations/0008_auto_20201002_0403.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0009_auto_20210510_2036.py` & `edc-export-0.3.8/edc_export/migrations/0009_auto_20210510_2036.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/migrations/0010_auto_20210910_1636.py` & `edc-export-0.3.8/edc_export/migrations/0010_auto_20210910_1636.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('edc_export', '0009_auto_20210510_2036'),
+        ("edc_export", "0009_auto_20210510_2036"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
-            name='exportdata',
-            options={'permissions': [('display_export_admin_action', 'Display export action')]},
+            name="exportdata",
+            options={
+                "permissions": [("display_export_admin_action", "Display export action")]
+            },
         ),
         migrations.AlterModelOptions(
-            name='importdata',
-            options={'permissions': [('display_import_admin_action', 'Display import action')]},
+            name="importdata",
+            options={
+                "permissions": [("display_import_admin_action", "Display import action")]
+            },
         ),
     ]
```

### Comparing `edc-export-0.3.7/edc_export/model_exporter/file_history_updater.py` & `edc-export-0.3.8/edc_export/model_exporter/file_history_updater.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/model_exporter/model_exporter.py` & `edc-export-0.3.8/edc_export/model_exporter/model_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/model_exporter/object_history_helpers.py` & `edc-export-0.3.8/edc_export/model_exporter/object_history_helpers.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/model_exporter/plan_exporter.py` & `edc-export-0.3.8/edc_export/model_exporter/plan_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/model_mixins/export_tracking_fields_model_mixin.py` & `edc-export-0.3.8/edc_export/model_mixins/export_tracking_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/model_mixins/notification_model_mixin.py` & `edc-export-0.3.8/edc_export/model_mixins/notification_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/model_options.py` & `edc-export-0.3.8/edc_export/model_options.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/models/data_request.py` & `edc-export-0.3.8/edc_export/models/data_request.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/models/data_request_history.py` & `edc-export-0.3.8/edc_export/models/data_request_history.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/models/export_receipt.py` & `edc-export-0.3.8/edc_export/models/export_receipt.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/models/file_history.py` & `edc-export-0.3.8/edc_export/models/file_history.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/models/object_history.py` & `edc-export-0.3.8/edc_export/models/object_history.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/models/plan.py` & `edc-export-0.3.8/edc_export/models/plan.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/models/upload_export_receipt_file.py` & `edc-export-0.3.8/edc_export/models/upload_export_receipt_file.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/navbars.py` & `edc-export-0.3.8/edc_export/navbars.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/signals.py` & `edc-export-0.3.8/edc_export/signals.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/static/edc_export/edc.css` & `edc-export-0.3.8/edc_export/static/edc_export/edc.css`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/static/edc_export/edc.js` & `edc-export-0.3.8/edc_export/static/edc_export/edc.js`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/templates/edc_export/bootstrap3/export_models.html` & `edc-export-0.3.8/edc_export/templates/edc_export/bootstrap3/export_models.html`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/templates/edc_export/bootstrap3/home.html` & `edc-export-0.3.8/edc_export/templates/edc_export/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/helper.py` & `edc-export-0.3.8/edc_export/tests/helper.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/models.py` & `edc-export-0.3.8/edc_export/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/tests/test_archive_exporter.py` & `edc-export-0.3.8/edc_export/tests/tests/test_archive_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/tests/test_export_model.py` & `edc-export-0.3.8/edc_export/tests/tests/test_export_model.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/tests/test_exportable.py` & `edc-export-0.3.8/edc_export/tests/tests/test_exportable.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/tests/test_model_exporter.py` & `edc-export-0.3.8/edc_export/tests/tests/test_model_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/tests/test_plan.py` & `edc-export-0.3.8/edc_export/tests/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/tests/visit_schedule.py` & `edc-export-0.3.8/edc_export/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/urls.py` & `edc-export-0.3.8/edc_export/urls.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/views/export_models_view.py` & `edc-export-0.3.8/edc_export/views/export_models_view.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export/views/export_selected_models_view.py` & `edc-export-0.3.8/edc_export/views/export_selected_models_view.py`

 * *Files identical despite different names*

### Comparing `edc-export-0.3.7/edc_export.egg-info/PKG-INFO` & `edc-export-0.3.8/edc_export.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edc-export
-Version: 0.3.7
+Version: 0.3.8
 Summary: Export from in the clinicedc/edc.
 Home-page: https://github.com/clinicedc/edc-export
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc export
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -34,9 +33,7 @@
 
 .. |codecov| image:: https://codecov.io/gh/clinicedc/edc-export/branch/develop/graph/badge.svg
   :target: https://codecov.io/gh/clinicedc/edc-export
 
 .. |downloads| image:: https://pepy.tech/badge/edc-export
    :target: https://pepy.tech/project/edc-export
 
-
-
```

### Comparing `edc-export-0.3.7/edc_export.egg-info/SOURCES.txt` & `edc-export-0.3.8/edc_export.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,24 @@
+.coveragerc
+.editorconfig
+.gitignore
 MANIFEST.in
+Makefile
 README.rst
 VERSION
+_version.py
+codecov.yml
+manage.py
 pyproject.toml
 requirements.txt
+runtests.py
 setup.cfg
 setup.py
+tox.ini
+.github/workflows/build.yml
 edc_export/__init__.py
 edc_export/admin_site.py
 edc_export/apps.py
 edc_export/archive_exporter.py
 edc_export/auth_objects.py
 edc_export/auths.py
 edc_export/choices.py
@@ -73,16 +83,25 @@
 edc_export/models/upload_export_receipt_file.py
 edc_export/static/edc_export/edc.css
 edc_export/static/edc_export/edc.js
 edc_export/templates/edc_export/bootstrap3/export_models.html
 edc_export/templates/edc_export/bootstrap3/home.html
 edc_export/tests/__init__.py
 edc_export/tests/helper.py
+edc_export/tests/holidays.csv
 edc_export/tests/models.py
 edc_export/tests/visit_schedule.py
+edc_export/tests/etc/user-aes-local.key
+edc_export/tests/etc/user-aes-restricted.key
+edc_export/tests/etc/user-rsa-local-private.pem
+edc_export/tests/etc/user-rsa-local-public.pem
+edc_export/tests/etc/user-rsa-restricted-private.pem
+edc_export/tests/etc/user-rsa-restricted-public.pem
+edc_export/tests/etc/user-salt-local.key
+edc_export/tests/etc/user-salt-restricted.key
 edc_export/tests/tests/__init__.py
 edc_export/tests/tests/test_archive_exporter.py
 edc_export/tests/tests/test_export_model.py
 edc_export/tests/tests/test_exportable.py
 edc_export/tests/tests/test_model_exporter.py
 edc_export/tests/tests/test_plan.py
 edc_export/views/__init__.py
```

### Comparing `edc-export-0.3.7/setup.py` & `edc-export-0.3.8/setup.py`

 * *Files identical despite different names*

