# Comparing `tmp/enrichsdk-4.8.4.tar.gz` & `tmp/enrichsdk-4.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrichsdk-4.8.4.tar", last modified: Sun Jul  2 11:16:31 2023, max compression
+gzip compressed data, was "enrichsdk-4.8.8.tar", last modified: Tue Jul 18 14:05:49 2023, max compression
```

## Comparing `enrichsdk-4.8.4.tar` & `enrichsdk-4.8.8.tar`

### file list

```diff
@@ -1,335 +1,336 @@
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.996049 enrichsdk-4.8.4/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/LICENSE
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/MANIFEST.in
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3562 2023-07-02 11:16:30.996049 enrichsdk-4.8.4/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2342 2023-05-23 17:29:05.000000 enrichsdk-4.8.4/README.rst
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.928039 enrichsdk-4.8.4/enrichsdk/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2023-06-30 11:08:26.000000 enrichsdk-4.8.4/enrichsdk/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.932040 enrichsdk-4.8.4/enrichsdk/api/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6446 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/api/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/api/draw.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.932040 enrichsdk-4.8.4/enrichsdk/app/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/app/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.932040 enrichsdk-4.8.4/enrichsdk/app/bases/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2023-01-10 11:58:12.000000 enrichsdk-4.8.4/enrichsdk/app/bases/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.932040 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.924039 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.924039 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.936040 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9434 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17331 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    19424 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14149 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3125 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14039 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    16381 2023-06-01 04:13:26.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    31961 2023-05-24 11:09:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.924039 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.924039 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.936040 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.936040 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      272 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       21 2023-05-12 09:38:40.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_donothing.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      571 2023-06-14 07:55:26.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1091 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      694 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2372 2023-06-09 07:01:47.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      657 2023-06-30 11:07:22.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7278 2023-06-30 11:00:46.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.940041 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3740 2023-05-14 15:19:15.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4963 2023-05-15 10:25:46.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1397 2023-05-14 15:19:41.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1601 2023-05-14 15:02:24.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4443 2023-05-14 15:19:54.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7244 2023-05-14 15:10:44.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8024 2023-05-14 15:20:08.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7261 2023-05-14 15:11:01.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3164 2023-06-16 10:58:53.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2985 2023-05-14 15:20:20.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3423 2023-05-14 15:20:27.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.940041 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.924039 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.924039 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.944042 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2320 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2220 2023-05-01 12:58:05.000000 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10025 2023-06-06 08:51:04.000000 enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/views.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3352 2023-05-02 10:46:19.000000 enrichsdk-4.8.4/enrichsdk/app/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.944042 enrichsdk-4.8.4/enrichsdk/app/widget/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/app/widget/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/app/widget/basewidget.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/app/widget/customcomponent.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/app/widget/customwidget.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.944042 enrichsdk-4.8.4/enrichsdk/commands/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/commands/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11171 2023-05-30 15:32:53.000000 enrichsdk-4.8.4/enrichsdk/commands/config.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/commands/decorators.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/commands/helper.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/commands/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/commands/run.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.944042 enrichsdk-4.8.4/enrichsdk/contrib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.948042 enrichsdk-4.8.4/enrichsdk/contrib/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.948042 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2023-03-08 02:41:34.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2023-02-14 06:43:41.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/anonymizer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7017 2023-02-07 10:54:16.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/changepoints.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2023-01-10 09:26:26.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/llmtextgen.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-16 05:19:04.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/syndata.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2023-03-08 02:41:34.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2023-01-03 13:19:44.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/logprocessor.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.948042 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      880 2023-05-30 13:50:35.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.948042 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/anomalies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.948042 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/changepoints/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2023-05-23 11:51:26.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.948042 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/classifier/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/classifier/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.952043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/data_quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.952043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/data_sanitizer/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    21225 2023-05-24 03:24:06.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.952043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.952043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/filebased_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.952043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2023-04-04 16:04:30.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.952043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23726 2023-04-04 16:04:30.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.952043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17300 2023-05-29 12:15:00.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/metrics/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/notebook_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/observability/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33359 2023-06-14 05:54:17.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/observability/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2023-04-05 10:51:48.000000 enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      469 2023-05-30 13:50:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/transforms/pqexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/pqexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/pqexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.956043 enrichsdk-4.8.4/enrichsdk/contrib/transforms/sqlexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/sqlexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14007 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/sqlexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.960044 enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.960044 enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.964045 enrichsdk-4.8.4/enrichsdk/core/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/core/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/core/frames.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    41276 2023-03-08 02:41:34.000000 enrichsdk-4.8.4/enrichsdk/core/mixins.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2023-03-08 02:41:34.000000 enrichsdk-4.8.4/enrichsdk/core/node.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/core/patch.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/core/render.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1292 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/core/res.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2023-04-05 10:39:21.000000 enrichsdk-4.8.4/enrichsdk/core/run.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/core/sdk.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6898 2023-03-09 06:57:39.000000 enrichsdk-4.8.4/enrichsdk/core/state.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/core/widgets.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.964045 enrichsdk-4.8.4/enrichsdk/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/datasets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    37013 2023-05-06 11:02:09.000000 enrichsdk-4.8.4/enrichsdk/datasets/discover.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18153 2023-05-29 06:02:24.000000 enrichsdk-4.8.4/enrichsdk/datasets/doodle.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/datasets/generators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.964045 enrichsdk-4.8.4/enrichsdk/extractors/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/extractors/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.964045 enrichsdk-4.8.4/enrichsdk/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.964045 enrichsdk-4.8.4/enrichsdk/featurestore/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/featurestore/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/featurestore/schema.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.964045 enrichsdk-4.8.4/enrichsdk/hedwig/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10907 2023-05-05 12:48:49.000000 enrichsdk-4.8.4/enrichsdk/hedwig/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.968045 enrichsdk-4.8.4/enrichsdk/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23696 2023-04-13 03:39:51.000000 enrichsdk-4.8.4/enrichsdk/lib/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4945 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/lib/context.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2023-02-26 08:39:33.000000 enrichsdk-4.8.4/enrichsdk/lib/customer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2023-03-09 06:57:39.000000 enrichsdk-4.8.4/enrichsdk/lib/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2903 2023-03-08 02:41:34.000000 enrichsdk-4.8.4/enrichsdk/lib/integration.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2023-01-10 09:26:26.000000 enrichsdk-4.8.4/enrichsdk/lib/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/lib/permissions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/lib/renderlib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1357 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/lib/resources.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.968045 enrichsdk-4.8.4/enrichsdk/notebook/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8611 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/notebook/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/notebook/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.972046 enrichsdk-4.8.4/enrichsdk/package/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    86268 2023-05-29 05:29:42.000000 enrichsdk-4.8.4/enrichsdk/package/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2023-02-01 09:43:30.000000 enrichsdk-4.8.4/enrichsdk/package/lib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/package/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2023-01-03 13:19:44.000000 enrichsdk-4.8.4/enrichsdk/package/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23793 2023-06-14 13:39:27.000000 enrichsdk-4.8.4/enrichsdk/package/mock.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/package/validators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.972046 enrichsdk-4.8.4/enrichsdk/policy/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/policy/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/policy/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.972046 enrichsdk-4.8.4/enrichsdk/quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/quality/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/quality/base.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/quality/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/quality/expectations.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/quality/reconciliation.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/quality/transforms.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.976046 enrichsdk-4.8.4/enrichsdk/realtime/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/realtime/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/realtime/db.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/realtime/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/realtime/messaging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/realtime/spark.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/realtime/transforms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/realtime/workflow.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.976046 enrichsdk-4.8.4/enrichsdk/render/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/render/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.976046 enrichsdk-4.8.4/enrichsdk/scripts/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/scripts/__init__.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/scripts/enrichcmd.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)    44415 2023-05-29 05:29:42.000000 enrichsdk-4.8.4/enrichsdk/scripts/enrichpkg.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.976046 enrichsdk-4.8.4/enrichsdk/services/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/services/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.980047 enrichsdk-4.8.4/enrichsdk/tasks/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/tasks/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.980047 enrichsdk-4.8.4/enrichsdk/tasks/dummy_task/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/tasks/dummy_task/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/tasks/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.984048 enrichsdk-4.8.4/enrichsdk/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/LICENSE.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/MANIFEST.in.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/README.md.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2023-01-02 14:59:19.000000 enrichsdk-4.8.4/enrichsdk/templates/README_PIPELINE.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/README_TASK.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.984048 enrichsdk-4.8.4/enrichsdk/templates/airflow/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/airflow/contrib-pipeline-v1.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.984048 enrichsdk-4.8.4/enrichsdk/templates/appstore2.0/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2023-01-17 08:20:08.000000 enrichsdk-4.8.4/enrichsdk/templates/appstore2.0/index.html.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.988048 enrichsdk-4.8.4/enrichsdk/templates/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/assets/datasets.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/config.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.988048 enrichsdk-4.8.4/enrichsdk/templates/dashboard/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/apps.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      220 2023-06-01 11:53:29.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      269 2023-06-01 09:52:08.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/custom.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/persona.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/tasks.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.988048 enrichsdk-4.8.4/enrichsdk/templates/dashboard/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/templates/complex_result.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/templates/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/urls.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6066 2023-06-01 11:53:11.000000 enrichsdk-4.8.4/enrichsdk/templates/dashboard/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.988048 enrichsdk-4.8.4/enrichsdk/templates/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/datasets/manifest.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2022-08-02 10:38:39.000000 enrichsdk-4.8.4/enrichsdk/templates/datasets.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/enrich.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.928039 enrichsdk-4.8.4/enrichsdk/templates/fixtures/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.988048 enrichsdk-4.8.4/enrichsdk/templates/fixtures/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/fixtures/configs/1.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/fixtures/configs/2.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-4.8.4/enrichsdk/templates/helloworld.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-4.8.4/enrichsdk/templates/iris.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/manifest.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.992049 enrichsdk-4.8.4/enrichsdk/templates/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/metrics/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/metrics/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1248 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/pipelineconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/pipelinepyconf.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.992049 enrichsdk-4.8.4/enrichsdk/templates/prefect/
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/prefect/default.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/pyscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-4.8.4/enrichsdk/templates/query.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/repo.init.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/root.README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/root.enrich.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/rscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/setup.cfg.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/setup.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-4.8.4/enrichsdk/templates/simpletransform.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2023-02-07 03:49:08.000000 enrichsdk-4.8.4/enrichsdk/templates/singlepageapp.py.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.992049 enrichsdk-4.8.4/enrichsdk/templates/spark/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/README.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.992049 enrichsdk-4.8.4/enrichsdk/templates/spark/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/configs/etl_config.json
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.992049 enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/enrich.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/logging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/spark.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.992049 enrichsdk-4.8.4/enrichsdk/templates/spark/jobs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/jobs/run_spark.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/spark/run.sh
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/taskconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/tasklib.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/test_module.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-4.8.4/enrichsdk/templates/transform.node.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.996049 enrichsdk-4.8.4/enrichsdk/templates/widgets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/barchart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/chart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/footer.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/fullpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/gridelement.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/header.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/heatmap.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/hero.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/mediumpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/multicolumn_list.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/nextrow.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/sectionfooter.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/sectionheader.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/shortpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-4.8.4/enrichsdk/templates/widgets/trophy.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.996049 enrichsdk-4.8.4/enrichsdk/utils/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4507 2023-06-02 07:59:52.000000 enrichsdk-4.8.4/enrichsdk/utils/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/utils/excel.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/utils/redis.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-4.8.4/enrichsdk/utils/sample.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-02 11:16:30.928039 enrichsdk-4.8.4/enrichsdk.egg-info/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3562 2023-07-02 11:16:30.000000 enrichsdk-4.8.4/enrichsdk.egg-info/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11143 2023-07-02 11:16:30.000000 enrichsdk-4.8.4/enrichsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2023-07-02 11:16:30.000000 enrichsdk-4.8.4/enrichsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       64 2023-07-02 11:16:30.000000 enrichsdk-4.8.4/enrichsdk.egg-info/entry_points.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-4.8.4/enrichsdk.egg-info/not-zip-safe
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      960 2023-07-02 11:16:30.000000 enrichsdk-4.8.4/enrichsdk.egg-info/requires.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       10 2023-07-02 11:16:30.000000 enrichsdk-4.8.4/enrichsdk.egg-info/top_level.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1391 2023-06-11 09:08:13.000000 enrichsdk-4.8.4/requirements.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2023-07-02 11:16:30.996049 enrichsdk-4.8.4/setup.cfg
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3092 2023-06-30 11:08:26.000000 enrichsdk-4.8.4/setup.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.045604 enrichsdk-4.8.8/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/LICENSE
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/MANIFEST.in
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3562 2023-07-18 14:05:49.045604 enrichsdk-4.8.8/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2342 2023-05-23 17:29:05.000000 enrichsdk-4.8.8/README.rst
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.001605 enrichsdk-4.8.8/enrichsdk/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2023-07-18 14:04:32.000000 enrichsdk-4.8.8/enrichsdk/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.001605 enrichsdk-4.8.8/enrichsdk/api/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6657 2023-07-18 13:56:43.000000 enrichsdk-4.8.8/enrichsdk/api/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/api/draw.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.005605 enrichsdk-4.8.8/enrichsdk/app/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/app/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.005605 enrichsdk-4.8.8/enrichsdk/app/bases/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2023-01-10 11:58:12.000000 enrichsdk-4.8.8/enrichsdk/app/bases/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.005605 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:48.997605 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:48.997605 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.005605 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9434 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17331 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    19424 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14149 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3125 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14039 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    16381 2023-06-01 04:13:26.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    31961 2023-05-24 11:09:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:48.997605 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:48.997605 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.005605 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.009605 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      272 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       21 2023-05-12 09:38:40.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_donothing.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      571 2023-06-14 07:55:26.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1091 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      260 2023-07-04 09:52:12.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/noaction_icon.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      694 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2372 2023-06-09 07:01:47.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1146 2023-07-07 05:49:30.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7278 2023-06-30 11:00:46.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3740 2023-05-14 15:19:15.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4963 2023-05-15 10:25:46.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1397 2023-05-14 15:19:41.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1601 2023-05-14 15:02:24.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4443 2023-05-14 15:19:54.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7244 2023-05-14 15:10:44.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8024 2023-05-14 15:20:08.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7261 2023-05-14 15:11:01.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3164 2023-06-16 10:58:53.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2985 2023-05-14 15:20:20.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3423 2023-05-14 15:20:27.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:48.997605 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:48.997605 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2320 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2220 2023-05-01 12:58:05.000000 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10025 2023-06-06 08:51:04.000000 enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/views.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3352 2023-05-02 10:46:19.000000 enrichsdk-4.8.8/enrichsdk/app/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/app/widget/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/app/widget/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/app/widget/basewidget.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/app/widget/customcomponent.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/app/widget/customwidget.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/commands/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/commands/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11171 2023-05-30 15:32:53.000000 enrichsdk-4.8.8/enrichsdk/commands/config.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/commands/decorators.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/commands/helper.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/commands/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/commands/run.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/contrib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/contrib/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2023-03-08 02:41:34.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2023-02-14 06:43:41.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/anonymizer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7017 2023-02-07 10:54:16.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/changepoints.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2023-01-10 09:26:26.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/llmtextgen.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-16 05:19:04.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/syndata.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2023-03-08 02:41:34.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2023-01-03 13:19:44.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/logprocessor.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      880 2023-05-30 13:50:35.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.013605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/anomalies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/changepoints/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2023-05-23 11:51:26.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/classifier/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/classifier/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/data_quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/data_sanitizer/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    21225 2023-05-24 03:24:06.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/filebased_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2023-04-04 16:04:30.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23726 2023-04-04 16:04:30.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17300 2023-05-29 12:15:00.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/metrics/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/notebook_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/observability/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33359 2023-06-14 05:54:17.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/observability/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2023-04-05 10:51:48.000000 enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      469 2023-05-30 13:50:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/pqexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/pqexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/pqexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/sqlexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/sqlexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14007 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/sqlexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.017605 enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/core/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/core/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/core/frames.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    41276 2023-03-08 02:41:34.000000 enrichsdk-4.8.8/enrichsdk/core/mixins.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2023-03-08 02:41:34.000000 enrichsdk-4.8.8/enrichsdk/core/node.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/core/patch.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/core/render.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1292 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/core/res.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2023-04-05 10:39:21.000000 enrichsdk-4.8.8/enrichsdk/core/run.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2023-07-17 17:19:15.000000 enrichsdk-4.8.8/enrichsdk/core/sdk.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6898 2023-03-09 06:57:39.000000 enrichsdk-4.8.8/enrichsdk/core/state.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/core/widgets.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/datasets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    37013 2023-05-06 11:02:09.000000 enrichsdk-4.8.8/enrichsdk/datasets/discover.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18153 2023-05-29 06:02:24.000000 enrichsdk-4.8.8/enrichsdk/datasets/doodle.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/datasets/generators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/extractors/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/extractors/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/featurestore/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/featurestore/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/featurestore/schema.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/hedwig/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10907 2023-05-05 12:48:49.000000 enrichsdk-4.8.8/enrichsdk/hedwig/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23696 2023-04-13 03:39:51.000000 enrichsdk-4.8.8/enrichsdk/lib/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4945 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/lib/context.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2023-02-26 08:39:33.000000 enrichsdk-4.8.8/enrichsdk/lib/customer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2023-03-09 06:57:39.000000 enrichsdk-4.8.8/enrichsdk/lib/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2903 2023-03-08 02:41:34.000000 enrichsdk-4.8.8/enrichsdk/lib/integration.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2023-01-10 09:26:26.000000 enrichsdk-4.8.8/enrichsdk/lib/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/lib/permissions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/lib/renderlib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1357 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/lib/resources.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/notebook/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8611 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/notebook/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/notebook/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/package/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    86800 2023-07-07 14:49:38.000000 enrichsdk-4.8.8/enrichsdk/package/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2023-02-01 09:43:30.000000 enrichsdk-4.8.8/enrichsdk/package/lib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/package/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2023-01-03 13:19:44.000000 enrichsdk-4.8.8/enrichsdk/package/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23793 2023-06-14 13:39:27.000000 enrichsdk-4.8.8/enrichsdk/package/mock.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/package/validators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/policy/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/policy/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/policy/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/quality/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/quality/base.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/quality/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/quality/expectations.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/quality/reconciliation.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/quality/transforms.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/realtime/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/realtime/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/realtime/db.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/realtime/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/realtime/messaging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/realtime/spark.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/realtime/transforms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/realtime/workflow.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/render/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/render/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/scripts/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/scripts/__init__.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/scripts/enrichcmd.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)    44415 2023-05-29 05:29:42.000000 enrichsdk-4.8.8/enrichsdk/scripts/enrichpkg.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/services/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/services/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/tasks/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/tasks/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.021605 enrichsdk-4.8.8/enrichsdk/tasks/dummy_task/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/tasks/dummy_task/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/tasks/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/LICENSE.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/MANIFEST.in.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/README.md.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2023-01-02 14:59:19.000000 enrichsdk-4.8.8/enrichsdk/templates/README_PIPELINE.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/README_TASK.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/airflow/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/airflow/contrib-pipeline-v1.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/appstore2.0/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2023-01-17 08:20:08.000000 enrichsdk-4.8.8/enrichsdk/templates/appstore2.0/index.html.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/assets/datasets.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/config.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/dashboard/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/apps.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      220 2023-06-01 11:53:29.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      269 2023-06-01 09:52:08.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/custom.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/persona.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/tasks.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/dashboard/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/templates/complex_result.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/templates/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/urls.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6066 2023-06-01 11:53:11.000000 enrichsdk-4.8.8/enrichsdk/templates/dashboard/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/datasets/manifest.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2022-08-02 10:38:39.000000 enrichsdk-4.8.8/enrichsdk/templates/datasets.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/enrich.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.001605 enrichsdk-4.8.8/enrichsdk/templates/fixtures/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/fixtures/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/fixtures/configs/1.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/fixtures/configs/2.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-4.8.8/enrichsdk/templates/helloworld.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-4.8.8/enrichsdk/templates/iris.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/manifest.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/metrics/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/metrics/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1248 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/pipelineconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/pipelinepyconf.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/prefect/
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/prefect/default.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/pyscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-4.8.8/enrichsdk/templates/query.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/repo.init.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/root.README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/root.enrich.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/rscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/setup.cfg.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/setup.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-4.8.8/enrichsdk/templates/simpletransform.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2023-02-07 03:49:08.000000 enrichsdk-4.8.8/enrichsdk/templates/singlepageapp.py.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/spark/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/README.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.037604 enrichsdk-4.8.8/enrichsdk/templates/spark/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/configs/etl_config.json
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.041604 enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/enrich.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/logging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/spark.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.041604 enrichsdk-4.8.8/enrichsdk/templates/spark/jobs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/jobs/run_spark.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/spark/run.sh
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/taskconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/tasklib.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/test_module.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-4.8.8/enrichsdk/templates/transform.node.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.045604 enrichsdk-4.8.8/enrichsdk/templates/widgets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/barchart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/chart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/footer.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/fullpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/gridelement.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/header.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/heatmap.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/hero.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/mediumpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/multicolumn_list.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/nextrow.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/sectionfooter.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/sectionheader.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/shortpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-4.8.8/enrichsdk/templates/widgets/trophy.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.045604 enrichsdk-4.8.8/enrichsdk/utils/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4788 2023-07-18 13:29:18.000000 enrichsdk-4.8.8/enrichsdk/utils/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/utils/excel.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/utils/redis.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-4.8.8/enrichsdk/utils/sample.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-07-18 14:05:49.001605 enrichsdk-4.8.8/enrichsdk.egg-info/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3562 2023-07-18 14:05:48.000000 enrichsdk-4.8.8/enrichsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11223 2023-07-18 14:05:48.000000 enrichsdk-4.8.8/enrichsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2023-07-18 14:05:48.000000 enrichsdk-4.8.8/enrichsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       64 2023-07-18 14:05:48.000000 enrichsdk-4.8.8/enrichsdk.egg-info/entry_points.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-4.8.8/enrichsdk.egg-info/not-zip-safe
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      960 2023-07-18 14:05:48.000000 enrichsdk-4.8.8/enrichsdk.egg-info/requires.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       10 2023-07-18 14:05:48.000000 enrichsdk-4.8.8/enrichsdk.egg-info/top_level.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1391 2023-06-11 09:08:13.000000 enrichsdk-4.8.8/requirements.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2023-07-18 14:05:49.045604 enrichsdk-4.8.8/setup.cfg
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3092 2023-07-18 14:04:32.000000 enrichsdk-4.8.8/setup.py
```

### Comparing `enrichsdk-4.8.4/LICENSE` & `enrichsdk-4.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/PKG-INFO` & `enrichsdk-4.8.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: enrichsdk
-Version: 4.8.4
+Version: 4.8.8
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Description: ==========
         Enrich SDK
```

### Comparing `enrichsdk-4.8.4/README.rst` & `enrichsdk-4.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/__init__.py` & `enrichsdk-4.8.8/enrichsdk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 |_____|_| |_|_|  |_|\___|_| |_| |____/|____/|_|\_\
 
 </pre>
 
 """
 import os
 
-VERSION = "4.8.4"
+VERSION = "4.8.8"
 
 
 def _get_git_revision(path):
     revision_file = os.path.join(path, "refs", "heads", "master")
     if os.path.exists(revision_file):
         with open(revision_file) as fh:
             return fh.read().strip()[:7]
```

### Comparing `enrichsdk-4.8.4/enrichsdk/api/__init__.py` & `enrichsdk-4.8.8/enrichsdk/api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,31 +27,30 @@
 
         Args:
 
            config (dict): Should have 'server' and 'key'.
         """
 
         self.config = config
-        assert "server" in config
-        assert "key" in config
-        assert "htpasswd_user" in config
-        assert "htpasswd_pwd" in config
+        assert (("server" in config) or ("url" in config))
+        assert (("key" in config) or ("apikey" in config))
 
     def get_api_url(self, path, use_prefix=True):
 
         path = path.replace("//", "/")
-        server = self.config["server"]
+        server = self.config.get("server",
+                                 self.config.get("url"))
 
         # Avoid double lines...
         if server[-1] == "/":
             server = server[:-1]
         if ((len(path) > 0) and (path[0] == "/")):
             path = path[1:]
 
-        if use_prefix:
+        if use_prefix and ("/api/v2" not in server):
             apiversion = self.config.get("version", "v2")
             url = "{}/api/{}/{}".format(server, apiversion, path)
         else:
             url = "{}/{}".format(server, path)
 
         return url
 
@@ -63,24 +62,26 @@
 
            path (str): API path suffix (after api/v1.0/)
            params (dict): Query parameters
         """
 
         method = str(method).lower()
 
-        key = self.config["key"]
-        user = self.config['htpasswd_user']
-        pwd = self.config['htpasswd_pwd']
-        auth = b64encode(f"{user}:{pwd}".encode('utf-8')).decode('utf-8')
+        key = self.config.get("key", self.config.get("apikey"))
 
         headers = {
             "X-API-Key": key,
-            "Authorization": f"Basic {auth}",
             "Accept": "application/json",
         }
+        if (('htpasswd_user' in self.config) and
+            ('htpasswd_pwsd' in self.config)):
+            user = self.config['htpasswd_user']
+            pwd = self.config['htpasswd_pwd']
+            auth = b64encode(f"{user}:{pwd}".encode('utf-8')).decode('utf-8')
+            headers["Authorization"] = f"Basic {auth}"
 
         try:
             if method == "get":
                 response = requests.get(
                     url,
                     verify=False,  # ignore SSL checks
                     headers=headers,
```

### Comparing `enrichsdk-4.8.4/enrichsdk/api/draw.py` & `enrichsdk-4.8.8/enrichsdk/api/draw.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/models.py` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/models.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/policyapp/views.py` & `enrichsdk-4.8.8/enrichsdk/app/bases/policyapp/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html` & `enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/bases/singlepageapp/views.py` & `enrichsdk-4.8.8/enrichsdk/app/bases/singlepageapp/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/utils.py` & `enrichsdk-4.8.8/enrichsdk/app/utils.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/widget/basewidget.py` & `enrichsdk-4.8.8/enrichsdk/app/widget/basewidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/widget/customcomponent.py` & `enrichsdk-4.8.8/enrichsdk/app/widget/customcomponent.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/app/widget/customwidget.py` & `enrichsdk-4.8.8/enrichsdk/app/widget/customwidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/commands/config.py` & `enrichsdk-4.8.8/enrichsdk/commands/config.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/commands/decorators.py` & `enrichsdk-4.8.8/enrichsdk/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/commands/helper.py` & `enrichsdk-4.8.8/enrichsdk/commands/helper.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/commands/log.py` & `enrichsdk-4.8.8/enrichsdk/commands/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/commands/run.py` & `enrichsdk-4.8.8/enrichsdk/commands/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/anonymizer.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/anonymizer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/changepoints.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/changepoints.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/llmtextgen.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/llmtextgen.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/profilespec.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/assets/timeseries_forecasting.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/assets/timeseries_forecasting.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/catalog.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/catalog.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/logprocessor.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/logprocessor.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/anomalies/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/anomalies/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/changepoints/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/changepoints/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/classifier/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/classifier/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/data_quality/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/data_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/fileops/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/metrics/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/notebook_executor/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/notebook_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/observability/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/observability/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/fileops/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/fileops/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/fileops/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsink/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsource/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/jsonsource/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/jsonsource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/pqexport/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/pqexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/pqexport/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/pqexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/sqlexport/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/sqlexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/sqlexport/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/sqlexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesink/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesink/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesink/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesource/README.md` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/contrib/transforms/tablesource/__init__.py` & `enrichsdk-4.8.8/enrichsdk/contrib/transforms/tablesource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/__init__.py` & `enrichsdk-4.8.8/enrichsdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/frames.py` & `enrichsdk-4.8.8/enrichsdk/core/frames.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/mixins.py` & `enrichsdk-4.8.8/enrichsdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/node.py` & `enrichsdk-4.8.8/enrichsdk/core/node.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/patch.py` & `enrichsdk-4.8.8/enrichsdk/core/patch.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/render.py` & `enrichsdk-4.8.8/enrichsdk/core/render.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/res.py` & `enrichsdk-4.8.8/enrichsdk/core/res.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/run.py` & `enrichsdk-4.8.8/enrichsdk/core/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/sdk.py` & `enrichsdk-4.8.8/enrichsdk/core/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/state.py` & `enrichsdk-4.8.8/enrichsdk/core/state.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/core/widgets.py` & `enrichsdk-4.8.8/enrichsdk/core/widgets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/datasets/__init__.py` & `enrichsdk-4.8.8/enrichsdk/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/datasets/discover.py` & `enrichsdk-4.8.8/enrichsdk/datasets/discover.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/datasets/doodle.py` & `enrichsdk-4.8.8/enrichsdk/datasets/doodle.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/datasets/generators.py` & `enrichsdk-4.8.8/enrichsdk/datasets/generators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/extractors/__init__.py` & `enrichsdk-4.8.8/enrichsdk/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/feature_compute/__init__.py` & `enrichsdk-4.8.8/enrichsdk/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/featurestore/__init__.py` & `enrichsdk-4.8.8/enrichsdk/featurestore/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/featurestore/schema.py` & `enrichsdk-4.8.8/enrichsdk/featurestore/schema.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/hedwig/__init__.py` & `enrichsdk-4.8.8/enrichsdk/hedwig/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/__init__.py` & `enrichsdk-4.8.8/enrichsdk/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/context.py` & `enrichsdk-4.8.8/enrichsdk/lib/context.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/customer.py` & `enrichsdk-4.8.8/enrichsdk/lib/customer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/exceptions.py` & `enrichsdk-4.8.8/enrichsdk/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/integration.py` & `enrichsdk-4.8.8/enrichsdk/lib/integration.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/misc.py` & `enrichsdk-4.8.8/enrichsdk/lib/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/permissions.py` & `enrichsdk-4.8.8/enrichsdk/lib/permissions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/renderlib.py` & `enrichsdk-4.8.8/enrichsdk/lib/renderlib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/lib/resources.py` & `enrichsdk-4.8.8/enrichsdk/lib/resources.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/notebook/__init__.py` & `enrichsdk-4.8.8/enrichsdk/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/package/__init__.py` & `enrichsdk-4.8.8/enrichsdk/package/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,26 +458,39 @@
         content = content.replace("APPNAME", appname)
         basename = os.path.basename(f)
         targetfile = os.path.join(templatedir, basename)
         with open(targetfile, "w") as fd:
             fd.write(content)
         print(basename, "=>", targetfile)
 
-    print("Add the following to the enrich.json")
+    print("Adding the following to the enrich.json")
     print(
         json.dumps(
             {
                 "installed_apps": [
                     f"{appname}.apps.{appname}Config"
                 ]
             },
             indent=4,
         )
     )
 
+    if os.path.exists('enrich.json'):
+        enrichdata = json.load(open('enrich.json'))
+        if 'installed_apps' not in enrichdata:
+            entry = f"{appname}.apps.{appname}Config"
+            enrichdata['installed_apps'] = [entry]
+        else:
+            enrichdata['installed_apps'].append(entry)
+        with open('enrich.json', 'w') as fd:
+            fd.write(json.dumps(enrichdata,indent=4))
+        print("Added successfully!")
+    else:
+        print("Failed to add. Please do it manually!")        
+        
 
 def prepare_module_generic(target, templatepath, what):
     """
     Bootstrap a generic module template..
     """
 
     if templatepath is None:
```

### Comparing `enrichsdk-4.8.4/enrichsdk/package/lib.py` & `enrichsdk-4.8.8/enrichsdk/package/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/package/log.py` & `enrichsdk-4.8.8/enrichsdk/package/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/package/misc.py` & `enrichsdk-4.8.8/enrichsdk/package/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/package/mock.py` & `enrichsdk-4.8.8/enrichsdk/package/mock.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/package/validators.py` & `enrichsdk-4.8.8/enrichsdk/package/validators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/policy/__init__.py` & `enrichsdk-4.8.8/enrichsdk/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/policy/sdk.py` & `enrichsdk-4.8.8/enrichsdk/policy/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/quality/__init__.py` & `enrichsdk-4.8.8/enrichsdk/quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/quality/base.py` & `enrichsdk-4.8.8/enrichsdk/quality/base.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/quality/exceptions.py` & `enrichsdk-4.8.8/enrichsdk/quality/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/quality/expectations.py` & `enrichsdk-4.8.8/enrichsdk/quality/expectations.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/quality/reconciliation.py` & `enrichsdk-4.8.8/enrichsdk/quality/reconciliation.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/quality/transforms.py` & `enrichsdk-4.8.8/enrichsdk/quality/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/realtime/db.py` & `enrichsdk-4.8.8/enrichsdk/realtime/db.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/realtime/log.py` & `enrichsdk-4.8.8/enrichsdk/realtime/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/realtime/messaging.py` & `enrichsdk-4.8.8/enrichsdk/realtime/messaging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/realtime/spark.py` & `enrichsdk-4.8.8/enrichsdk/realtime/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/realtime/transforms.py` & `enrichsdk-4.8.8/enrichsdk/realtime/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/realtime/workflow.py` & `enrichsdk-4.8.8/enrichsdk/realtime/workflow.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/render/__init__.py` & `enrichsdk-4.8.8/enrichsdk/render/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/scripts/enrichcmd.py` & `enrichsdk-4.8.8/enrichsdk/scripts/enrichcmd.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/scripts/enrichpkg.py` & `enrichsdk-4.8.8/enrichsdk/scripts/enrichpkg.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/services/__init__.py` & `enrichsdk-4.8.8/enrichsdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/tasks/__init__.py` & `enrichsdk-4.8.8/enrichsdk/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/tasks/dummy_task/__init__.py` & `enrichsdk-4.8.8/enrichsdk/tasks/dummy_task/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/tasks/sdk.py` & `enrichsdk-4.8.8/enrichsdk/tasks/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/airflow/contrib-pipeline-v1.py` & `enrichsdk-4.8.8/enrichsdk/templates/airflow/contrib-pipeline-v1.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/appstore2.0/index.html.template` & `enrichsdk-4.8.8/enrichsdk/templates/appstore2.0/index.html.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/assets/datasets.py` & `enrichsdk-4.8.8/enrichsdk/templates/assets/datasets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/config.json.template` & `enrichsdk-4.8.8/enrichsdk/templates/config.json.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/dashboard/persona.py` & `enrichsdk-4.8.8/enrichsdk/templates/dashboard/persona.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/dashboard/tasks.py` & `enrichsdk-4.8.8/enrichsdk/templates/dashboard/tasks.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/dashboard/templates/complex_result.html` & `enrichsdk-4.8.8/enrichsdk/templates/dashboard/templates/complex_result.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/dashboard/templates/index.html` & `enrichsdk-4.8.8/enrichsdk/templates/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/dashboard/urls.py` & `enrichsdk-4.8.8/enrichsdk/templates/dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/dashboard/views.py` & `enrichsdk-4.8.8/enrichsdk/templates/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/datasets.py.template` & `enrichsdk-4.8.8/enrichsdk/templates/datasets.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/helloworld.node.template` & `enrichsdk-4.8.8/enrichsdk/templates/helloworld.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/iris.node.template` & `enrichsdk-4.8.8/enrichsdk/templates/iris.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/metrics/__init__.py` & `enrichsdk-4.8.8/enrichsdk/templates/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/metrics/profilespec.py` & `enrichsdk-4.8.8/enrichsdk/templates/metrics/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/pipelineconf.template` & `enrichsdk-4.8.8/enrichsdk/templates/pipelineconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/pipelinepyconf.template` & `enrichsdk-4.8.8/enrichsdk/templates/pipelinepyconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/prefect/default.py` & `enrichsdk-4.8.8/enrichsdk/templates/prefect/default.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/pyscript.template` & `enrichsdk-4.8.8/enrichsdk/templates/pyscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/query.node.template` & `enrichsdk-4.8.8/enrichsdk/templates/query.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/rscript.template` & `enrichsdk-4.8.8/enrichsdk/templates/rscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/setup.py.template` & `enrichsdk-4.8.8/enrichsdk/templates/setup.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/simpletransform.node.template` & `enrichsdk-4.8.8/enrichsdk/templates/simpletransform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/singlepageapp.py.template` & `enrichsdk-4.8.8/enrichsdk/templates/singlepageapp.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/spark/README.md` & `enrichsdk-4.8.8/enrichsdk/templates/spark/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/enrich.py` & `enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/enrich.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/logging.py` & `enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/logging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/spark/dependencies/spark.py` & `enrichsdk-4.8.8/enrichsdk/templates/spark/dependencies/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/spark/jobs/run_spark.py` & `enrichsdk-4.8.8/enrichsdk/templates/spark/jobs/run_spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/spark/run.sh` & `enrichsdk-4.8.8/enrichsdk/templates/spark/run.sh`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/taskconf.template` & `enrichsdk-4.8.8/enrichsdk/templates/taskconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/tasklib.template` & `enrichsdk-4.8.8/enrichsdk/templates/tasklib.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/test_module.py.template` & `enrichsdk-4.8.8/enrichsdk/templates/test_module.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/transform.node.template` & `enrichsdk-4.8.8/enrichsdk/templates/transform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/widgets/barchart.html` & `enrichsdk-4.8.8/enrichsdk/templates/widgets/barchart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/widgets/chart.html` & `enrichsdk-4.8.8/enrichsdk/templates/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/widgets/heatmap.html` & `enrichsdk-4.8.8/enrichsdk/templates/widgets/heatmap.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/widgets/hero.html` & `enrichsdk-4.8.8/enrichsdk/templates/widgets/hero.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/templates/widgets/linechart.html` & `enrichsdk-4.8.8/enrichsdk/templates/widgets/linechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/utils/__init__.py` & `enrichsdk-4.8.8/enrichsdk/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+
+import os
+import sys
 import json
+import re
 import numpy as np
 from sqllineage.runner import LineageRunner
 from datetime import date, datetime
 
 from .sample import *
 from .excel import *
 def get_lineage_of_query(engine, sql):
@@ -158,7 +162,16 @@
 def get_today():
     return date.today().isoformat()
 
 def get_daybefore():
     daybefore = date.today() + timedelta(days=-2)
     return daybefore.isoformat()
 
+########################################
+# Text cleaner...
+########################################
+def slugify(s):
+  s = s.lower().strip()
+  s = re.sub(r'[^\w\s-]', '', s)
+  s = re.sub(r'[\s_-]+', '_', s)
+  s = re.sub(r'^-+|-+$', '', s)
+  return s
```

### Comparing `enrichsdk-4.8.4/enrichsdk/utils/excel.py` & `enrichsdk-4.8.8/enrichsdk/utils/excel.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/utils/redis.py` & `enrichsdk-4.8.8/enrichsdk/utils/redis.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk/utils/sample.py` & `enrichsdk-4.8.8/enrichsdk/utils/sample.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/enrichsdk.egg-info/PKG-INFO` & `enrichsdk-4.8.8/enrichsdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: enrichsdk
-Version: 4.8.4
+Version: 4.8.8
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Description: ==========
         Enrich SDK
```

### Comparing `enrichsdk-4.8.4/enrichsdk.egg-info/SOURCES.txt` & `enrichsdk-4.8.8/enrichsdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_donothing.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
+enrichsdk/app/bases/sharedapp/templates/sharedapp/components/noaction_icon.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
```

### Comparing `enrichsdk-4.8.4/enrichsdk.egg-info/requires.txt` & `enrichsdk-4.8.8/enrichsdk.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 pyarrow>=0.9.0
 pyfiglet
 pyhive
 pykafka
 pykafka==2.8.0
 pymongo
 pytest-cov
-pytest>=4.8.4
+pytest>=4.8.8
 python-dateutil>=2.8.1
 python-json-logger==2.0.4
 pytz>=2020.1
 raven==6.6.0
 redis
 requests-oauthlib==0.8.0
 requests==2.26.0
```

### Comparing `enrichsdk-4.8.4/requirements.txt` & `enrichsdk-4.8.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.8.4/setup.py` & `enrichsdk-4.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("enrichsdk/__init__.py", "rb") as f:
     version = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 setup(
     name="enrichsdk",
-    version="4.8.4",
+    version="4.8.8",
     description="Enrich Developer Kit",
     long_description=readme,
     url="http://github.com/pingali/scribble-enrichsdk",
     author="Venkata Pingali",
     author_email="pingali@scribbledata.io",
     license="All rights reserved",
     scripts=[],
@@ -34,15 +34,15 @@
         "click>=7.1.2",
         "aioitertools==0.8.0",
 
         "glob2==0.7",
         "httpx",
         "requests==2.26.0",
         "requests-oauthlib==0.8.0",
-        "pytest>=4.8.4",
+        "pytest>=4.8.8",
         "pandas>=1.3.5,<1.5",
         "distributed==2.30.1",
         "idna==2.8",
         "coverage==5.5",
         "flake8",
         "raven==6.6.0",
         "python-json-logger==2.0.4",
```

