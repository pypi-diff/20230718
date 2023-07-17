# Comparing `tmp/fern_merge-0.0.33.tar.gz` & `tmp/fern_merge-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_merge-0.0.33.tar", max compression
+gzip compressed data, was "fern_merge-0.0.34.tar", max compression
```

## Comparing `fern_merge-0.0.33.tar` & `fern_merge-0.0.34.tar`

### file list

```diff
@@ -1,456 +1,456 @@
--rw-r--r--   0        0        0     2139 2023-07-17 19:24:43.761405 fern_merge-0.0.33/README.md
--rw-r--r--   0        0        0      389 2023-07-17 19:24:43.761405 fern_merge-0.0.33/pyproject.toml
--rw-r--r--   0        0        0      187 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/__init__.py
--rw-r--r--   0        0        0     1627 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/client.py
--rw-r--r--   0        0        0      519 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/core/api_error.py
--rw-r--r--   0        0        0     1101 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      201 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/environment.py
--rw-r--r--   0        0        0        0 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/py.typed
--rw-r--r--   0        0        0      116 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/__init__.py
--rw-r--r--   0        0        0     9656 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/__init__.py
--rw-r--r--   0        0        0    10018 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/client.py
--rw-r--r--   0        0        0     1144 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2284 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2334 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/activities/__init__.py
--rw-r--r--   0        0        0    12564 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/activities/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/applications/__init__.py
--rw-r--r--   0        0        0    15247 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/applications/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/attachments/__init__.py
--rw-r--r--   0        0        0    12326 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2304 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/candidates/__init__.py
--rw-r--r--   0        0        0    17208 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/candidates/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2045 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/departments/__init__.py
--rw-r--r--   0        0        0     6270 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/departments/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/eeocs/__init__.py
--rw-r--r--   0        0        0     8547 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/eeocs/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2362 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2537 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/interviews/__init__.py
--rw-r--r--   0        0        0    13032 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/interviews/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/issues/__init__.py
--rw-r--r--   0        0        0     7052 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/job_interview_stages/__init__.py
--rw-r--r--   0        0        0     7085 2023-07-17 19:24:43.761405 fern_merge-0.0.33/src/merge/resources/ats/resources/job_interview_stages/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/jobs/__init__.py
--rw-r--r--   0        0        0     8673 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4924 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5589 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/offers/__init__.py
--rw-r--r--   0        0        0     8533 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/offers/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/offices/__init__.py
--rw-r--r--   0        0        0     6198 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/offices/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4900 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2545 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/reject_reasons/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/reject_reasons/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/scorecards/__init__.py
--rw-r--r--   0        0        0     8991 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/scorecards/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     7004 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2756 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/tags/__init__.py
--rw-r--r--   0        0        0     4453 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/users/__init__.py
--rw-r--r--   0        0        0     7813 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4455 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13447 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/__init__.py
--rw-r--r--   0        0        0     1240 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/access_role_enum.py
--rw-r--r--   0        0        0     1483 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/account_token.py
--rw-r--r--   0        0        0      857 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activities_list_request_remote_fields.py
--rw-r--r--   0        0        0      869 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      873 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      885 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     2705 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity.py
--rw-r--r--   0        0        0      189 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity_activity_type.py
--rw-r--r--   0        0        0     2155 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity_request.py
--rw-r--r--   0        0        0      196 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity_request_activity_type.py
--rw-r--r--   0        0        0      187 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity_request_visibility.py
--rw-r--r--   0        0        0     1109 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity_response.py
--rw-r--r--   0        0        0      705 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/activity_visibility.py
--rw-r--r--   0        0        0     2473 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/application.py
--rw-r--r--   0        0        0     2269 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/application_request.py
--rw-r--r--   0        0        0     1121 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/application_response.py
--rw-r--r--   0        0        0     8243 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/applications_list_request_expand.py
--rw-r--r--   0        0        0     8371 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/applications_retrieve_request_expand.py
--rw-r--r--   0        0        0     2146 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/attachment.py
--rw-r--r--   0        0        0      199 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/attachment_attachment_type.py
--rw-r--r--   0        0        0     1820 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/attachment_request.py
--rw-r--r--   0        0        0      206 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/attachment_request_attachment_type.py
--rw-r--r--   0        0        0     1117 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/attachment_response.py
--rw-r--r--   0        0        0      985 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/attachment_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/available_actions.py
--rw-r--r--   0        0        0     3471 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/candidate.py
--rw-r--r--   0        0        0     3061 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/candidate_request.py
--rw-r--r--   0        0        0     1113 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/candidate_response.py
--rw-r--r--   0        0        0      833 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/candidates_list_request_expand.py
--rw-r--r--   0        0        0      849 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
--rw-r--r--   0        0        0     1391 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-17 19:24:43.765405 fern_merge-0.0.33/src/merge/resources/ats/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1698 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/department.py
--rw-r--r--   0        0        0     1337 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/disability_status_enum.py
--rw-r--r--   0        0        0     4088 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeoc.py
--rw-r--r--   0        0        0      201 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeoc_disability_status.py
--rw-r--r--   0        0        0      160 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeoc_gender.py
--rw-r--r--   0        0        0      152 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeoc_race.py
--rw-r--r--   0        0        0      189 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeoc_veteran_status.py
--rw-r--r--   0        0        0     3803 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
--rw-r--r--   0        0        0     3851 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     3867 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     3915 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1529 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/email_address.py
--rw-r--r--   0        0        0      210 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/email_address_email_address_type.py
--rw-r--r--   0        0        0     1553 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/email_address_request.py
--rw-r--r--   0        0        0      217 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/email_address_request_email_address_type.py
--rw-r--r--   0        0        0      742 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/email_address_type_enum.py
--rw-r--r--   0        0        0      522 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/error_validation_problem.py
--rw-r--r--   0        0        0     1160 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/gender_enum.py
--rw-r--r--   0        0        0     4187 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/interviews_list_request_expand.py
--rw-r--r--   0        0        0     4251 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/issues_list_request_status.py
--rw-r--r--   0        0        0     3428 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/job.py
--rw-r--r--   0        0        0     2387 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/job_interview_stage.py
--rw-r--r--   0        0        0      169 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/job_status.py
--rw-r--r--   0        0        0     1045 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/job_status_enum.py
--rw-r--r--   0        0        0     3771 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/jobs_list_request_expand.py
--rw-r--r--   0        0        0      956 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/jobs_list_request_status.py
--rw-r--r--   0        0        0     3835 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2786 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/offer.py
--rw-r--r--   0        0        0      177 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/offer_status.py
--rw-r--r--   0        0        0     1832 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/offer_status_enum.py
--rw-r--r--   0        0        0      767 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/offers_list_request_expand.py
--rw-r--r--   0        0        0      783 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/offers_retrieve_request_expand.py
--rw-r--r--   0        0        0     1817 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/office.py
--rw-r--r--   0        0        0      993 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/operator_schema.py
--rw-r--r--   0        0        0     1180 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/overall_recommendation_enum.py
--rw-r--r--   0        0        0      959 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      892 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_activity_list.py
--rw-r--r--   0        0        0      904 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_application_list.py
--rw-r--r--   0        0        0      900 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      896 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_candidate_list.py
--rw-r--r--   0        0        0      921 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      900 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_department_list.py
--rw-r--r--   0        0        0      876 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_eeoc_list.py
--rw-r--r--   0        0        0      880 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_issue_list.py
--rw-r--r--   0        0        0      930 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
--rw-r--r--   0        0        0      872 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_job_list.py
--rw-r--r--   0        0        0      880 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_offer_list.py
--rw-r--r--   0        0        0      884 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_office_list.py
--rw-r--r--   0        0        0      909 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_reject_reason_list.py
--rw-r--r--   0        0        0      901 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_remote_user_list.py
--rw-r--r--   0        0        0      933 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
--rw-r--r--   0        0        0      896 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_scorecard_list.py
--rw-r--r--   0        0        0      901 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/paginated_tag_list.py
--rw-r--r--   0        0        0     3068 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/patched_candidate_request.py
--rw-r--r--   0        0        0     1624 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/phone_number.py
--rw-r--r--   0        0        0      205 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/phone_number_phone_number_type.py
--rw-r--r--   0        0        0     1648 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/phone_number_request.py
--rw-r--r--   0        0        0      212 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
--rw-r--r--   0        0        0     1039 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/phone_number_type_enum.py
--rw-r--r--   0        0        0     2326 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/race_enum.py
--rw-r--r--   0        0        0      814 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/reason_enum.py
--rw-r--r--   0        0        0     1775 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/reject_reason.py
--rw-r--r--   0        0        0      802 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/remote_response_response_type.py
--rw-r--r--   0        0        0     2562 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/remote_user.py
--rw-r--r--   0        0        0      183 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/remote_user_access_role.py
--rw-r--r--   0        0        0      723 2023-07-17 19:24:43.769405 fern_merge-0.0.33/src/merge/resources/ats/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/response_type_enum.py
--rw-r--r--   0        0        0     3187 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview.py
--rw-r--r--   0        0        0     2464 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_request.py
--rw-r--r--   0        0        0      237 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_request_status.py
--rw-r--r--   0        0        0     1150 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_response.py
--rw-r--r--   0        0        0      230 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_status.py
--rw-r--r--   0        0        0      893 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_status_enum.py
--rw-r--r--   0        0        0     2692 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scorecard.py
--rw-r--r--   0        0        0      226 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scorecard_overall_recommendation.py
--rw-r--r--   0        0        0     1731 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scorecards_list_request_expand.py
--rw-r--r--   0        0        0     1763 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
--rw-r--r--   0        0        0      695 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1623 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/tag.py
--rw-r--r--   0        0        0     1659 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/url.py
--rw-r--r--   0        0        0     1683 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/url_request.py
--rw-r--r--   0        0        0      171 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/url_request_url_type.py
--rw-r--r--   0        0        0     1451 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/url_type_enum.py
--rw-r--r--   0        0        0      164 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/url_url_type.py
--rw-r--r--   0        0        0      762 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/validation_problem_source.py
--rw-r--r--   0        0        0     1467 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/veteran_status_enum.py
--rw-r--r--   0        0        0      760 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/visibility_enum.py
--rw-r--r--   0        0        0      915 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/ats/types/webhook_receiver.py
--rw-r--r--   0        0        0    10290 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/__init__.py
--rw-r--r--   0        0        0     9511 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/client.py
--rw-r--r--   0        0        0     1106 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2286 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2336 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2306 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/bank_info/__init__.py
--rw-r--r--   0        0        0     9159 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/bank_info/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/benefits/__init__.py
--rw-r--r--   0        0        0     6947 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/benefits/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/companies/__init__.py
--rw-r--r--   0        0        0     6226 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/companies/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2047 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
--rw-r--r--   0        0        0     8378 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/employee_payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/employees/__init__.py
--rw-r--r--   0        0        0    18323 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/employees/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/employments/__init__.py
--rw-r--r--   0        0        0     9179 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/employments/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2364 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/groups/__init__.py
--rw-r--r--   0        0        0     7705 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/issues/__init__.py
--rw-r--r--   0        0        0     7056 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4926 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5591 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/locations/__init__.py
--rw-r--r--   0        0        0     7671 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/locations/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4902 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/pay_groups/__init__.py
--rw-r--r--   0        0        0     6244 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/pay_groups/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/payroll_runs/__init__.py
--rw-r--r--   0        0        0     9202 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2547 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     7010 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2758 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.773405 fern_merge-0.0.33/src/merge/resources/hris/resources/teams/__init__.py
--rw-r--r--   0        0        0     6923 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/resources/time_off/__init__.py
--rw-r--r--   0        0        0    13310 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/resources/time_off/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/resources/time_off_balances/__init__.py
--rw-r--r--   0        0        0     8802 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/resources/time_off_balances/client.py
--rw-r--r--   0        0        0       65 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4459 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    14549 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/account_token.py
--rw-r--r--   0        0        0      555 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/account_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/available_actions.py
--rw-r--r--   0        0        0     2399 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/bank_info.py
--rw-r--r--   0        0        0      185 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/bank_info_account_type.py
--rw-r--r--   0        0        0      529 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/bank_info_list_request_account_type.py
--rw-r--r--   0        0        0      728 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/bank_info_list_request_order_by.py
--rw-r--r--   0        0        0     2342 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/benefit.py
--rw-r--r--   0        0        0     1391 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     1962 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/company.py
--rw-r--r--   0        0        0     2324 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/condition_type_enum.py
--rw-r--r--   0        0        0    35178 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/country_enum.py
--rw-r--r--   0        0        0      870 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     2140 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/deduction.py
--rw-r--r--   0        0        0     2143 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/earning.py
--rw-r--r--   0        0        0      177 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/earning_type.py
--rw-r--r--   0        0        0      949 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/earning_type_enum.py
--rw-r--r--   0        0        0     6788 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee.py
--rw-r--r--   0        0        0      205 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_employment_status.py
--rw-r--r--   0        0        0      176 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_ethnicity.py
--rw-r--r--   0        0        0      164 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_gender.py
--rw-r--r--   0        0        0      193 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_marital_status.py
--rw-r--r--   0        0        0     2796 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_payroll_run.py
--rw-r--r--   0        0        0      829 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
--rw-r--r--   0        0        0      845 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
--rw-r--r--   0        0        0     6252 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_request.py
--rw-r--r--   0        0        0      212 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_request_employment_status.py
--rw-r--r--   0        0        0      183 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_request_ethnicity.py
--rw-r--r--   0        0        0      171 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_request_gender.py
--rw-r--r--   0        0        0      200 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_request_marital_status.py
--rw-r--r--   0        0        0     1109 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employee_response.py
--rw-r--r--   0        0        0      739 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_employment_status.py
--rw-r--r--   0        0        0    80247 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_expand.py
--rw-r--r--   0        0        0     4067 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_remote_fields.py
--rw-r--r--   0        0        0     4115 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
--rw-r--r--   0        0        0    81343 2023-07-17 19:24:43.777405 fern_merge-0.0.33/src/merge/resources/hris/types/employees_retrieve_request_expand.py
--rw-r--r--   0        0        0     4131 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4179 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    18682 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment.py
--rw-r--r--   0        0        0      199 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment_employment_type.py
--rw-r--r--   0        0        0      183 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment_flsa_status.py
--rw-r--r--   0        0        0      187 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment_pay_currency.py
--rw-r--r--   0        0        0      191 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment_pay_frequency.py
--rw-r--r--   0        0        0      179 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment_pay_period.py
--rw-r--r--   0        0        0      770 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment_status_enum.py
--rw-r--r--   0        0        0     1166 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employment_type_enum.py
--rw-r--r--   0        0        0      777 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_expand.py
--rw-r--r--   0        0        0      707 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_order_by.py
--rw-r--r--   0        0        0     4219 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_remote_fields.py
--rw-r--r--   0        0        0     4267 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      793 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employments_retrieve_request_expand.py
--rw-r--r--   0        0        0     4283 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4331 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      522 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/error_validation_problem.py
--rw-r--r--   0        0        0     2511 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/ethnicity_enum.py
--rw-r--r--   0        0        0      986 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/flsa_status_enum.py
--rw-r--r--   0        0        0     1146 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/gender_enum.py
--rw-r--r--   0        0        0     2225 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/group.py
--rw-r--r--   0        0        0      169 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/group_type.py
--rw-r--r--   0        0        0     1136 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/group_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/ignore_common_model_request_reason.py
--rw-r--r--   0        0        0     1323 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0    11870 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/location.py
--rw-r--r--   0        0        0      168 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/location_country.py
--rw-r--r--   0        0        0      189 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/location_location_type.py
--rw-r--r--   0        0        0      509 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/location_type_enum.py
--rw-r--r--   0        0        0     1685 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/marital_status_enum.py
--rw-r--r--   0        0        0     1037 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      893 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_bank_info_list.py
--rw-r--r--   0        0        0      888 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_benefit_list.py
--rw-r--r--   0        0        0      888 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_company_list.py
--rw-r--r--   0        0        0      921 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      892 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_employee_list.py
--rw-r--r--   0        0        0      934 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
--rw-r--r--   0        0        0      900 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_employment_list.py
--rw-r--r--   0        0        0      880 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_issue_list.py
--rw-r--r--   0        0        0      892 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_location_list.py
--rw-r--r--   0        0        0      893 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_pay_group_list.py
--rw-r--r--   0        0        0      901 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_payroll_run_list.py
--rw-r--r--   0        0        0      901 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_team_list.py
--rw-r--r--   0        0        0      918 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_time_off_balance_list.py
--rw-r--r--   0        0        0      889 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/paginated_time_off_list.py
--rw-r--r--   0        0        0    48882 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/pay_currency_enum.py
--rw-r--r--   0        0        0     1940 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/pay_frequency_enum.py
--rw-r--r--   0        0        0     1754 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/pay_group.py
--rw-r--r--   0        0        0     1798 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/pay_period_enum.py
--rw-r--r--   0        0        0     2811 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_run.py
--rw-r--r--   0        0        0      175 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_run_run_state.py
--rw-r--r--   0        0        0      171 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_run_run_type.py
--rw-r--r--   0        0        0      801 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
--rw-r--r--   0        0        0     1104 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
--rw-r--r--   0        0        0      813 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      817 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      829 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1305 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/policy_type_enum.py
--rw-r--r--   0        0        0      814 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/remote_response_response_type.py
--rw-r--r--   0        0        0      723 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/request_format_enum.py
--rw-r--r--   0        0        0     1312 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/request_type_enum.py
--rw-r--r--   0        0        0      562 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/response_type_enum.py
--rw-r--r--   0        0        0     1032 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/run_state_enum.py
--rw-r--r--   0        0        0     1173 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/run_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1975 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/tax.py
--rw-r--r--   0        0        0     1953 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/team.py
--rw-r--r--   0        0        0     3481 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off.py
--rw-r--r--   0        0        0     2517 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_balance.py
--rw-r--r--   0        0        0      187 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_balance_policy_type.py
--rw-r--r--   0        0        0     1272 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
--rw-r--r--   0        0        0      751 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_expand.py
--rw-r--r--   0        0        0     1595 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
--rw-r--r--   0        0        0     1223 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_request_type.py
--rw-r--r--   0        0        0     1619 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1029 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_status.py
--rw-r--r--   0        0        0     3199 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_request.py
--rw-r--r--   0        0        0      191 2023-07-17 19:24:43.781405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_request_request_type.py
--rw-r--r--   0        0        0      193 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_request_status.py
--rw-r--r--   0        0        0      184 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_request_type.py
--rw-r--r--   0        0        0      166 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_request_units.py
--rw-r--r--   0        0        0     1106 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_response.py
--rw-r--r--   0        0        0      767 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
--rw-r--r--   0        0        0     1627 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1651 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      186 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_status.py
--rw-r--r--   0        0        0     1146 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_status_enum.py
--rw-r--r--   0        0        0      159 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/time_off_units.py
--rw-r--r--   0        0        0      495 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/units_enum.py
--rw-r--r--   0        0        0      762 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-17 19:24:43.785405 fern_merge-0.0.33/src/merge/resources/hris/types/webhook_receiver.py
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0     2139 2023-07-17 22:56:29.494258 fern_merge-0.0.34/README.md
+-rw-r--r--   0        0        0      389 2023-07-17 22:56:29.494258 fern_merge-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/__init__.py
+-rw-r--r--   0        0        0     1627 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/client.py
+-rw-r--r--   0        0        0      519 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/core/api_error.py
+-rw-r--r--   0        0        0     1101 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      201 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/environment.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/py.typed
+-rw-r--r--   0        0        0      116 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/__init__.py
+-rw-r--r--   0        0        0     9656 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/__init__.py
+-rw-r--r--   0        0        0    10018 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/client.py
+-rw-r--r--   0        0        0     1144 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2284 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/activities/__init__.py
+-rw-r--r--   0        0        0    12564 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/activities/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/applications/__init__.py
+-rw-r--r--   0        0        0    15247 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/applications/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    12326 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2304 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/candidates/__init__.py
+-rw-r--r--   0        0        0    17208 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/candidates/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2045 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/departments/__init__.py
+-rw-r--r--   0        0        0     6270 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/departments/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/eeocs/__init__.py
+-rw-r--r--   0        0        0     8547 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/eeocs/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2362 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2537 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/interviews/__init__.py
+-rw-r--r--   0        0        0    13032 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/interviews/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/issues/__init__.py
+-rw-r--r--   0        0        0     7052 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/job_interview_stages/__init__.py
+-rw-r--r--   0        0        0     7085 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/job_interview_stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     8673 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4924 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5589 2023-07-17 22:56:29.494258 fern_merge-0.0.34/src/merge/resources/ats/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/offers/__init__.py
+-rw-r--r--   0        0        0     8533 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/offers/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/offices/__init__.py
+-rw-r--r--   0        0        0     6198 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/offices/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4900 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2545 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/reject_reasons/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/reject_reasons/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/scorecards/__init__.py
+-rw-r--r--   0        0        0     8991 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/scorecards/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     7004 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2756 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/tags/__init__.py
+-rw-r--r--   0        0        0     4453 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/users/__init__.py
+-rw-r--r--   0        0        0     7813 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13447 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/access_role_enum.py
+-rw-r--r--   0        0        0     1483 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/account_token.py
+-rw-r--r--   0        0        0      857 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activities_list_request_remote_fields.py
+-rw-r--r--   0        0        0      869 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      873 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      885 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     2705 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity.py
+-rw-r--r--   0        0        0      189 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity_activity_type.py
+-rw-r--r--   0        0        0     2155 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity_request.py
+-rw-r--r--   0        0        0      196 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity_request_activity_type.py
+-rw-r--r--   0        0        0      187 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity_request_visibility.py
+-rw-r--r--   0        0        0     1109 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity_response.py
+-rw-r--r--   0        0        0      705 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/activity_visibility.py
+-rw-r--r--   0        0        0     2473 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/application.py
+-rw-r--r--   0        0        0     2269 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/application_request.py
+-rw-r--r--   0        0        0     1121 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/application_response.py
+-rw-r--r--   0        0        0     8243 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/applications_list_request_expand.py
+-rw-r--r--   0        0        0     8371 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/applications_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2146 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/attachment.py
+-rw-r--r--   0        0        0      199 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/attachment_attachment_type.py
+-rw-r--r--   0        0        0     1820 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/attachment_request.py
+-rw-r--r--   0        0        0      206 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/attachment_request_attachment_type.py
+-rw-r--r--   0        0        0     1117 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/attachment_response.py
+-rw-r--r--   0        0        0      985 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/attachment_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/available_actions.py
+-rw-r--r--   0        0        0     3471 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/candidate.py
+-rw-r--r--   0        0        0     3061 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/candidate_request.py
+-rw-r--r--   0        0        0     1113 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/candidate_response.py
+-rw-r--r--   0        0        0      833 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/candidates_list_request_expand.py
+-rw-r--r--   0        0        0      849 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1391 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1698 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/department.py
+-rw-r--r--   0        0        0     1337 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/disability_status_enum.py
+-rw-r--r--   0        0        0     4088 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeoc.py
+-rw-r--r--   0        0        0      201 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeoc_disability_status.py
+-rw-r--r--   0        0        0      160 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeoc_gender.py
+-rw-r--r--   0        0        0      152 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeoc_race.py
+-rw-r--r--   0        0        0      189 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeoc_veteran_status.py
+-rw-r--r--   0        0        0     3803 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     3851 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     3867 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     3915 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1529 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/email_address.py
+-rw-r--r--   0        0        0      210 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/email_address_email_address_type.py
+-rw-r--r--   0        0        0     1553 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/email_address_request.py
+-rw-r--r--   0        0        0      217 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/email_address_request_email_address_type.py
+-rw-r--r--   0        0        0      742 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/email_address_type_enum.py
+-rw-r--r--   0        0        0      522 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1160 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/gender_enum.py
+-rw-r--r--   0        0        0     4187 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/interviews_list_request_expand.py
+-rw-r--r--   0        0        0     4251 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     3428 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/job.py
+-rw-r--r--   0        0        0     2387 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/job_interview_stage.py
+-rw-r--r--   0        0        0      169 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/job_status.py
+-rw-r--r--   0        0        0     1045 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/job_status_enum.py
+-rw-r--r--   0        0        0     3771 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/jobs_list_request_expand.py
+-rw-r--r--   0        0        0      956 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/jobs_list_request_status.py
+-rw-r--r--   0        0        0     3835 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2786 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/offer.py
+-rw-r--r--   0        0        0      177 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/offer_status.py
+-rw-r--r--   0        0        0     1832 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/offer_status_enum.py
+-rw-r--r--   0        0        0      767 2023-07-17 22:56:29.498258 fern_merge-0.0.34/src/merge/resources/ats/types/offers_list_request_expand.py
+-rw-r--r--   0        0        0      783 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/offers_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1817 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/office.py
+-rw-r--r--   0        0        0      993 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/operator_schema.py
+-rw-r--r--   0        0        0     1180 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/overall_recommendation_enum.py
+-rw-r--r--   0        0        0      959 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      892 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_activity_list.py
+-rw-r--r--   0        0        0      904 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_application_list.py
+-rw-r--r--   0        0        0      900 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      896 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_candidate_list.py
+-rw-r--r--   0        0        0      921 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      900 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_department_list.py
+-rw-r--r--   0        0        0      876 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_eeoc_list.py
+-rw-r--r--   0        0        0      880 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      930 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
+-rw-r--r--   0        0        0      872 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_job_list.py
+-rw-r--r--   0        0        0      880 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_offer_list.py
+-rw-r--r--   0        0        0      884 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_office_list.py
+-rw-r--r--   0        0        0      909 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_reject_reason_list.py
+-rw-r--r--   0        0        0      901 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_remote_user_list.py
+-rw-r--r--   0        0        0      933 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
+-rw-r--r--   0        0        0      896 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_scorecard_list.py
+-rw-r--r--   0        0        0      901 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/paginated_tag_list.py
+-rw-r--r--   0        0        0     3068 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/patched_candidate_request.py
+-rw-r--r--   0        0        0     1624 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/phone_number.py
+-rw-r--r--   0        0        0      205 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/phone_number_phone_number_type.py
+-rw-r--r--   0        0        0     1648 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/phone_number_request.py
+-rw-r--r--   0        0        0      212 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
+-rw-r--r--   0        0        0     1039 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/phone_number_type_enum.py
+-rw-r--r--   0        0        0     2326 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/race_enum.py
+-rw-r--r--   0        0        0      814 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/reason_enum.py
+-rw-r--r--   0        0        0     1775 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/reject_reason.py
+-rw-r--r--   0        0        0      802 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/remote_response_response_type.py
+-rw-r--r--   0        0        0     2562 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/remote_user.py
+-rw-r--r--   0        0        0      183 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/remote_user_access_role.py
+-rw-r--r--   0        0        0      723 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/response_type_enum.py
+-rw-r--r--   0        0        0     3187 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview.py
+-rw-r--r--   0        0        0     2464 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_request.py
+-rw-r--r--   0        0        0      237 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_request_status.py
+-rw-r--r--   0        0        0     1150 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_response.py
+-rw-r--r--   0        0        0      230 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_status.py
+-rw-r--r--   0        0        0      893 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_status_enum.py
+-rw-r--r--   0        0        0     2692 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scorecard.py
+-rw-r--r--   0        0        0      226 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scorecard_overall_recommendation.py
+-rw-r--r--   0        0        0     1731 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scorecards_list_request_expand.py
+-rw-r--r--   0        0        0     1763 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
+-rw-r--r--   0        0        0      695 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1623 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/tag.py
+-rw-r--r--   0        0        0     1659 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/url.py
+-rw-r--r--   0        0        0     1683 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/url_request.py
+-rw-r--r--   0        0        0      171 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/url_request_url_type.py
+-rw-r--r--   0        0        0     1451 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/url_type_enum.py
+-rw-r--r--   0        0        0      164 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/url_url_type.py
+-rw-r--r--   0        0        0      762 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/validation_problem_source.py
+-rw-r--r--   0        0        0     1467 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/veteran_status_enum.py
+-rw-r--r--   0        0        0      760 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/visibility_enum.py
+-rw-r--r--   0        0        0      915 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/ats/types/webhook_receiver.py
+-rw-r--r--   0        0        0    10290 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/__init__.py
+-rw-r--r--   0        0        0     9511 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/client.py
+-rw-r--r--   0        0        0     1106 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2286 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2336 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2306 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/bank_info/__init__.py
+-rw-r--r--   0        0        0     9159 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/bank_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/benefits/__init__.py
+-rw-r--r--   0        0        0     6947 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/benefits/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/companies/__init__.py
+-rw-r--r--   0        0        0     6226 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/companies/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2047 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
+-rw-r--r--   0        0        0     8378 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/employee_payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/employees/__init__.py
+-rw-r--r--   0        0        0    18323 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/employees/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/employments/__init__.py
+-rw-r--r--   0        0        0     9179 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/employments/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2364 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/groups/__init__.py
+-rw-r--r--   0        0        0     7705 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/issues/__init__.py
+-rw-r--r--   0        0        0     7056 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4926 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5591 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/locations/__init__.py
+-rw-r--r--   0        0        0     7671 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/locations/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4902 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/pay_groups/__init__.py
+-rw-r--r--   0        0        0     6244 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/pay_groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/payroll_runs/__init__.py
+-rw-r--r--   0        0        0     9202 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2547 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     7010 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2758 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/teams/__init__.py
+-rw-r--r--   0        0        0     6923 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/time_off/__init__.py
+-rw-r--r--   0        0        0    13310 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/time_off/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/time_off_balances/__init__.py
+-rw-r--r--   0        0        0     8802 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/time_off_balances/client.py
+-rw-r--r--   0        0        0       65 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4459 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    14549 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-17 22:56:29.502258 fern_merge-0.0.34/src/merge/resources/hris/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/account_token.py
+-rw-r--r--   0        0        0      555 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/account_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/available_actions.py
+-rw-r--r--   0        0        0     2399 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/bank_info.py
+-rw-r--r--   0        0        0      185 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/bank_info_account_type.py
+-rw-r--r--   0        0        0      529 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/bank_info_list_request_account_type.py
+-rw-r--r--   0        0        0      728 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/bank_info_list_request_order_by.py
+-rw-r--r--   0        0        0     2342 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/benefit.py
+-rw-r--r--   0        0        0     1391 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     1962 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/company.py
+-rw-r--r--   0        0        0     2324 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/condition_type_enum.py
+-rw-r--r--   0        0        0    35178 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/country_enum.py
+-rw-r--r--   0        0        0      870 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     2140 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/deduction.py
+-rw-r--r--   0        0        0     2143 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/earning.py
+-rw-r--r--   0        0        0      177 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/earning_type.py
+-rw-r--r--   0        0        0      949 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/earning_type_enum.py
+-rw-r--r--   0        0        0     6788 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee.py
+-rw-r--r--   0        0        0      205 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_employment_status.py
+-rw-r--r--   0        0        0      176 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_ethnicity.py
+-rw-r--r--   0        0        0      164 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_gender.py
+-rw-r--r--   0        0        0      193 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_marital_status.py
+-rw-r--r--   0        0        0     2796 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_payroll_run.py
+-rw-r--r--   0        0        0      829 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
+-rw-r--r--   0        0        0      845 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
+-rw-r--r--   0        0        0     6252 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_request.py
+-rw-r--r--   0        0        0      212 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_request_employment_status.py
+-rw-r--r--   0        0        0      183 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_request_ethnicity.py
+-rw-r--r--   0        0        0      171 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_request_gender.py
+-rw-r--r--   0        0        0      200 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_request_marital_status.py
+-rw-r--r--   0        0        0     1109 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employee_response.py
+-rw-r--r--   0        0        0      739 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_employment_status.py
+-rw-r--r--   0        0        0    80247 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_expand.py
+-rw-r--r--   0        0        0     4067 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4115 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0    81343 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employees_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4131 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4179 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    18682 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment.py
+-rw-r--r--   0        0        0      199 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment_employment_type.py
+-rw-r--r--   0        0        0      183 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment_flsa_status.py
+-rw-r--r--   0        0        0      187 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment_pay_currency.py
+-rw-r--r--   0        0        0      191 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment_pay_frequency.py
+-rw-r--r--   0        0        0      179 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment_pay_period.py
+-rw-r--r--   0        0        0      770 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment_status_enum.py
+-rw-r--r--   0        0        0     1166 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employment_type_enum.py
+-rw-r--r--   0        0        0      777 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_expand.py
+-rw-r--r--   0        0        0      707 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_order_by.py
+-rw-r--r--   0        0        0     4219 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4267 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      793 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employments_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4283 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4331 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      522 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2511 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/ethnicity_enum.py
+-rw-r--r--   0        0        0      986 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/flsa_status_enum.py
+-rw-r--r--   0        0        0     1146 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/gender_enum.py
+-rw-r--r--   0        0        0     2225 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/group.py
+-rw-r--r--   0        0        0      169 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/group_type.py
+-rw-r--r--   0        0        0     1136 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/group_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/ignore_common_model_request_reason.py
+-rw-r--r--   0        0        0     1323 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0    11870 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/location.py
+-rw-r--r--   0        0        0      168 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/location_country.py
+-rw-r--r--   0        0        0      189 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/location_location_type.py
+-rw-r--r--   0        0        0      509 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/location_type_enum.py
+-rw-r--r--   0        0        0     1685 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/marital_status_enum.py
+-rw-r--r--   0        0        0     1037 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      893 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_bank_info_list.py
+-rw-r--r--   0        0        0      888 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_benefit_list.py
+-rw-r--r--   0        0        0      888 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_company_list.py
+-rw-r--r--   0        0        0      921 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      892 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_employee_list.py
+-rw-r--r--   0        0        0      934 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
+-rw-r--r--   0        0        0      900 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_employment_list.py
+-rw-r--r--   0        0        0      880 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      892 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_location_list.py
+-rw-r--r--   0        0        0      893 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_pay_group_list.py
+-rw-r--r--   0        0        0      901 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_payroll_run_list.py
+-rw-r--r--   0        0        0      901 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_team_list.py
+-rw-r--r--   0        0        0      918 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_time_off_balance_list.py
+-rw-r--r--   0        0        0      889 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/paginated_time_off_list.py
+-rw-r--r--   0        0        0    48882 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/pay_currency_enum.py
+-rw-r--r--   0        0        0     1940 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/pay_frequency_enum.py
+-rw-r--r--   0        0        0     1754 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/pay_group.py
+-rw-r--r--   0        0        0     1798 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/pay_period_enum.py
+-rw-r--r--   0        0        0     2811 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_run.py
+-rw-r--r--   0        0        0      175 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_run_run_state.py
+-rw-r--r--   0        0        0      171 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_run_run_type.py
+-rw-r--r--   0        0        0      801 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1104 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
+-rw-r--r--   0        0        0      813 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      817 2023-07-17 22:56:29.506258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      829 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1305 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/policy_type_enum.py
+-rw-r--r--   0        0        0      814 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/remote_response_response_type.py
+-rw-r--r--   0        0        0      723 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/request_format_enum.py
+-rw-r--r--   0        0        0     1312 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/request_type_enum.py
+-rw-r--r--   0        0        0      562 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/response_type_enum.py
+-rw-r--r--   0        0        0     1032 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/run_state_enum.py
+-rw-r--r--   0        0        0     1173 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/run_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1975 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/tax.py
+-rw-r--r--   0        0        0     1953 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/team.py
+-rw-r--r--   0        0        0     3481 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off.py
+-rw-r--r--   0        0        0     2517 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_balance.py
+-rw-r--r--   0        0        0      187 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_balance_policy_type.py
+-rw-r--r--   0        0        0     1272 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
+-rw-r--r--   0        0        0      751 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_expand.py
+-rw-r--r--   0        0        0     1595 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1223 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_request_type.py
+-rw-r--r--   0        0        0     1619 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1029 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_status.py
+-rw-r--r--   0        0        0     3199 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_request.py
+-rw-r--r--   0        0        0      191 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_request_request_type.py
+-rw-r--r--   0        0        0      193 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_request_status.py
+-rw-r--r--   0        0        0      184 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_request_type.py
+-rw-r--r--   0        0        0      166 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_request_units.py
+-rw-r--r--   0        0        0     1106 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_response.py
+-rw-r--r--   0        0        0      767 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1627 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1651 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      186 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_status.py
+-rw-r--r--   0        0        0     1146 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_status_enum.py
+-rw-r--r--   0        0        0      159 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/time_off_units.py
+-rw-r--r--   0        0        0      495 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/units_enum.py
+-rw-r--r--   0        0        0      762 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-17 22:56:29.510258 fern_merge-0.0.34/src/merge/resources/hris/types/webhook_receiver.py
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.34/PKG-INFO
```

### Comparing `fern_merge-0.0.33/README.md` & `fern_merge-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/client.py` & `fern_merge-0.0.34/src/merge/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/core/__init__.py` & `fern_merge-0.0.34/src/merge/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/core/client_wrapper.py` & `fern_merge-0.0.34/src/merge/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/core/datetime_utils.py` & `fern_merge-0.0.34/src/merge/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/core/jsonable_encoder.py` & `fern_merge-0.0.34/src/merge/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/__init__.py` & `fern_merge-0.0.34/src/merge/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/__init__.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/account_details/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/account_token/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/activities/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/activities/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/applications/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/applications/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/attachments/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/available_actions/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/candidates/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/candidates/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/delete_account/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/departments/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/departments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/eeocs/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/eeocs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/force_resync/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/generate_key/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/interviews/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/interviews/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/issues/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/job_interview_stages/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/job_interview_stages/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/jobs/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/link_token/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/linked_accounts/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/offers/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/offers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/offices/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/offices/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/passthrough/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/regenerate_key/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/reject_reasons/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/reject_reasons/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/scorecards/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/scorecards/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/selective_sync/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/sync_status/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/tags/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/users/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/resources/webhook_receivers/client.py` & `fern_merge-0.0.34/src/merge/resources/ats/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/__init__.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/access_role_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/access_role_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/account_details.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/account_details_and_actions.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/account_details_and_actions_integration.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/account_integration.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/account_token.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activities_list_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activities_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activity.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activity.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activity_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activity_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activity_response.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activity_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/activity_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/application.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/application.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/application_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/application_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/application_response.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/application_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/applications_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/applications_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/applications_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/applications_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/attachment.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/attachment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/attachment_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/attachment_response.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/attachment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/attachment_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/attachment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/available_actions.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/candidate.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/candidate.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/candidate_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/candidate_response.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/candidate_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/candidates_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/candidates_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/candidates_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/candidates_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/categories_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/category_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/common_model_scopes_body_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/condition_schema.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/condition_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/debug_mode_log.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/debug_model_log_summary.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/department.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/department.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/disability_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/disability_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/eeoc.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/eeoc.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/email_address.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/email_address.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/email_address_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/email_address_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/email_address_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/enabled_actions_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/encoding_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/error_validation_problem.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/gender_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/interviews_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/interviews_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/interviews_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/interviews_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/issue.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/issue_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/job.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/job.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/job_interview_stage.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/job_interview_stage.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/job_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/job_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/jobs_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/jobs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/jobs_list_request_status.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/jobs_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/jobs_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/jobs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/link_token.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_condition.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_condition_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/linked_account_status.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/meta_response.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/method_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/model_operation.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/multipart_form_field_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/offer.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/offer.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/offer_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/offer_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/offers_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/offers_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/offers_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/offers_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/office.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/office.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/operator_schema.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/overall_recommendation_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/overall_recommendation_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_activity_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_activity_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_application_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_attachment_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_candidate_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_candidate_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_condition_schema_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_department_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_department_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_eeoc_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_eeoc_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_issue_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_job_interview_stage_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_job_interview_stage_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_job_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_job_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_offer_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_offer_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_office_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_office_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_reject_reason_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_reject_reason_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_remote_user_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_remote_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_scheduled_interview_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_scheduled_interview_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_scorecard_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_scorecard_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_sync_status_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/paginated_tag_list.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/patched_candidate_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/patched_candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/phone_number.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/phone_number_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/phone_number_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/phone_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/race_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/race_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/reason_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/reject_reason.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/reject_reason.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/remote_data.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/remote_key.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/remote_response.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/remote_user.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/remote_user.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/request_format_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/response_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_response.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/scheduled_interview_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/scheduled_interview_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/scorecard.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/scorecard.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/scorecards_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/scorecards_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/sync_status.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/sync_status_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/tag.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/tag.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/url.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/url.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/url_request.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/url_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/url_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/url_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/validation_problem_source.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/veteran_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/veteran_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/visibility_enum.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/visibility_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/warning_validation_problem.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/ats/types/webhook_receiver.py` & `fern_merge-0.0.34/src/merge/resources/ats/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/__init__.py` & `fern_merge-0.0.34/src/merge/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/__init__.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/account_details/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/account_token/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/available_actions/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/bank_info/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/bank_info/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/benefits/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/benefits/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/companies/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/companies/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/delete_account/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/employee_payroll_runs/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/employee_payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/employees/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/employees/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/employments/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/employments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/force_resync/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/generate_key/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/groups/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/issues/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/link_token/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/linked_accounts/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/locations/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/locations/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/passthrough/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/pay_groups/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/pay_groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/payroll_runs/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/regenerate_key/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/selective_sync/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/sync_status/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/teams/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/time_off/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/time_off/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/time_off_balances/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/time_off_balances/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/resources/webhook_receivers/client.py` & `fern_merge-0.0.34/src/merge/resources/hris/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/__init__.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/account_details.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/account_details_and_actions.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/account_details_and_actions_integration.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/account_integration.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/account_token.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/account_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/account_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/available_actions.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/bank_info.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/bank_info.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/bank_info_list_request_account_type.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/bank_info_list_request_account_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/bank_info_list_request_order_by.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/bank_info_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/benefit.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/benefit.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/categories_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/category_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/common_model_scopes_body_request.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/company.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/company.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/condition_schema.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/condition_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/country_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/debug_mode_log.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/debug_model_log_summary.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/deduction.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/deduction.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/earning.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/earning.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/earning_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/earning_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employee.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employee.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employee_payroll_run.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employee_payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employee_request.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employee_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employee_response.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employee_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_employment_status.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_employment_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employees_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employees_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employment.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employment_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employment_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employment_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_order_by.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employments_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/enabled_actions_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/encoding_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/error_validation_problem.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/ethnicity_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/ethnicity_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/flsa_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/flsa_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/gender_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/group.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/group_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/group_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/issue.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/issue_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/link_token.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_condition.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_condition_request.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/linked_account_status.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/location.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/location.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/marital_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/meta_response.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/method_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/model_operation.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/multipart_form_field_request.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/operator_schema.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_bank_info_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_bank_info_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_benefit_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_benefit_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_company_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_condition_schema_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_employee_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_employee_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_employment_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_employment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_group_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_issue_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_location_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_location_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_pay_group_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_pay_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_payroll_run_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_sync_status_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_team_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_time_off_balance_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_time_off_balance_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/paginated_time_off_list.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/paginated_time_off_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/pay_currency_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/pay_currency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/pay_frequency_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/pay_frequency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/pay_group.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/pay_group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/pay_period_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/pay_period_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/payroll_run.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/policy_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/policy_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/reason_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/remote_data.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/remote_key.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/remote_response.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/request_format_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/request_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/request_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/response_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/run_state_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/run_state_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/run_type_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/run_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/sync_status.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/sync_status_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/tax.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/tax.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/team.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/team.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_balance.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_balance.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_request_type.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_request_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_list_request_status.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_request.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_response.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_retrieve_request_expand.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/time_off_status_enum.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/time_off_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/validation_problem_source.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/warning_validation_problem.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/src/merge/resources/hris/types/webhook_receiver.py` & `fern_merge-0.0.34/src/merge/resources/hris/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.33/PKG-INFO` & `fern_merge-0.0.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-merge
-Version: 0.0.33
+Version: 0.0.34
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

