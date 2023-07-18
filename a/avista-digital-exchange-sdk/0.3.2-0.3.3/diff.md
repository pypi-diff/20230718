# Comparing `tmp/avista_digital_exchange_sdk-0.3.2.tar.gz` & `tmp/avista_digital_exchange_sdk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avista_digital_exchange_sdk-0.3.2.tar", last modified: Mon Jul 17 20:01:00 2023, max compression
+gzip compressed data, was "avista_digital_exchange_sdk-0.3.3.tar", last modified: Tue Jul 18 15:22:05 2023, max compression
```

## Comparing `avista_digital_exchange_sdk-0.3.2.tar` & `avista_digital_exchange_sdk-0.3.3.tar`

### file list

```diff
@@ -1,265 +1,300 @@
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.960546 avista_digital_exchange_sdk-0.3.2/
--rw-r--r--   0 Justin     (502) staff       (20)    35148 2022-09-13 20:02:44.000000 avista_digital_exchange_sdk-0.3.2/LICENSE
--rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-07-17 20:01:00.960034 avista_digital_exchange_sdk-0.3.2/PKG-INFO
--rw-r--r--   0 Justin     (502) staff       (20)    33555 2023-06-15 18:40:21.000000 avista_digital_exchange_sdk-0.3.2/README.md
--rw-r--r--   0 Justin     (502) staff       (20)     1002 2023-07-17 20:00:47.000000 avista_digital_exchange_sdk-0.3.2/pyproject.toml
--rw-r--r--   0 Justin     (502) staff       (20)       38 2023-07-17 20:01:00.960703 avista_digital_exchange_sdk-0.3.2/setup.cfg
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.708151 avista_digital_exchange_sdk-0.3.2/src/
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.724532 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/
--rw-r--r--   0 Justin     (502) staff       (20)     4950 2023-07-17 17:55:00.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/DxTypes.py
--rw-r--r--   0 Justin     (502) staff       (20)      213 2023-06-14 18:10:08.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/__init__.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.877905 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/
--rw-r--r--   0 Justin     (502) staff       (20)    94776 2023-07-17 18:23:29.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1951 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/base_model.py
--rw-r--r--   0 Justin     (502) staff       (20)   200668 2023-07-17 18:23:29.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/client.py
--rw-r--r--   0 Justin     (502) staff       (20)    10104 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_add_service_to_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     5545 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_get_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     7026 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_member_organization_requests.py
--rw-r--r--   0 Justin     (502) staff       (20)    10171 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_services.py
--rw-r--r--   0 Justin     (502) staff       (20)     5665 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)     6610 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives_service_shared_with.py
--rw-r--r--   0 Justin     (502) staff       (20)    10544 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_remove_service_from_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     5568 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_update_collaborative_member_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      675 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_attach_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_create_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     1088 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_attachment.py
--rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     1238 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_active_capture_data_export_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)     3976 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     1229 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     1100 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_export_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)     1906 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model.py
--rw-r--r--   0 Justin     (502) staff       (20)      738 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model_export.py
--rw-r--r--   0 Justin     (502) staff       (20)      864 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_file_attachment_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)      413 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_python_s_d_k_sample.py
--rw-r--r--   0 Justin     (502) staff       (20)     4288 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_handle_completion.py
--rw-r--r--   0 Justin     (502) staff       (20)     1100 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_attachments.py
--rw-r--r--   0 Justin     (502) staff       (20)     4568 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_captures.py
--rw-r--r--   0 Justin     (502) staff       (20)     4535 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_notify_capture_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1840 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_publish_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1228 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_regenerate_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     4070 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_start_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     4016 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_stop_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     2024 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_data_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     4137 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/enums.py
--rw-r--r--   0 Justin     (502) staff       (20)     2418 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/exceptions.py
--rw-r--r--   0 Justin     (502) staff       (20)     5844 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/input_types.py
--rw-r--r--   0 Justin     (502) staff       (20)     2523 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_add_endpoints_to_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      606 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_cancel_query.py
--rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     1873 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_new_model_version.py
--rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_model.py
--rw-r--r--   0 Justin     (502) staff       (20)      768 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_generate_query_result_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1011 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     2135 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      554 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1543 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model.py
--rw-r--r--   0 Justin     (502) staff       (20)      390 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model_in_d_t_d_l_format.py
--rw-r--r--   0 Justin     (502) staff       (20)     2334 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoint_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)     1903 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoints_in_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     2235 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups.py
--rw-r--r--   0 Justin     (502) staff       (20)     2551 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups_endpoints_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)      610 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs.py
--rw-r--r--   0 Justin     (502) staff       (20)     2495 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs_endpoints_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)     1617 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_models.py
--rw-r--r--   0 Justin     (502) staff       (20)      837 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_notify_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     2282 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)      954 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_query_by_time_range.py
--rw-r--r--   0 Justin     (502) staff       (20)     1081 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_regenerate_endpoint_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     2779 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_remove_endpoints_from_group.py
--rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     2062 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint_properties.py
--rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     2146 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model_used_by_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     8790 2023-07-17 19:05:03.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/modified_async_base_client.py
--rw-r--r--   0 Justin     (502) staff       (20)      842 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/notifications_notify_upload_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1783 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_capture_publish_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     2417 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_iot_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)     4069 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_capture_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)      857 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_iot_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)      956 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_time_series_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)      731 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_upload_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     3642 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_start_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     3602 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_stop_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     1414 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_time_series_db_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)     5859 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_add_collaborative_member.py
--rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     6089 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_collaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)     9608 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_services.py
--rw-r--r--   0 Justin     (502) staff       (20)     5546 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      759 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1388 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     5666 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_collaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)      801 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_organizations.py
--rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_users.py
--rw-r--r--   0 Justin     (502) staff       (20)     6610 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_collaboratives_ownership.py
--rw-r--r--   0 Justin     (502) staff       (20)    10525 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_services_ownership.py
--rw-r--r--   0 Justin     (502) staff       (20)     6021 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_remove_collaborative_member.py
--rw-r--r--   0 Justin     (502) staff       (20)     1617 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_resend_user_invitation.py
--rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     6021 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative_member.py
--rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_user.py
--rw-r--r--   0 Justin     (502) staff       (20)      220 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/scalars.py
--rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)      726 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     1410 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file_data_view.py
--rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1328 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     1410 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file_data_view.py
--rw-r--r--   0 Justin     (502) staff       (20)      755 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3782 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1298 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)      808 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)      798 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_zip_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)      797 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_list_data_stores.py
--rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1328 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)      779 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_cancel_database_query.py
--rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_create_database.py
--rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_delete_database.py
--rw-r--r--   0 Justin     (502) staff       (20)      992 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_generate_query_result_export_file.py
--rw-r--r--   0 Justin     (502) staff       (20)      843 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_get_database.py
--rw-r--r--   0 Justin     (502) staff       (20)     2470 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_all_asset_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)      885 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_databases.py
--rw-r--r--   0 Justin     (502) staff       (20)     1059 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_notify_time_series_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1702 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_publish_to_database.py
--rw-r--r--   0 Justin     (502) staff       (20)     1022 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database.py
--rw-r--r--   0 Justin     (502) staff       (20)      912 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database_with_timestream_query.py
--rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_update_database.py
--rw-r--r--   0 Justin     (502) staff       (20)     1111 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_create_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     1111 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_delete_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     1555 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_get_user_session.py
--rw-r--r--   0 Justin     (502) staff       (20)     1117 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_list_authentication_tokens.py
--rw-r--r--   0 Justin     (502) staff       (20)     1629 2023-07-10 20:54:52.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/avista_digital_exchange.py
--rw-r--r--   0 Justin     (502) staff       (20)     4712 2023-07-17 17:54:14.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/client.py
--rw-r--r--   0 Justin     (502) staff       (20)     3384 2022-12-02 17:38:29.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/collaborativeUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     7112 2023-07-17 17:55:03.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/dataCaptureUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     2784 2022-12-02 17:57:07.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/dataStoreUtil.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.920927 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/
--rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1989 2022-09-29 18:39:50.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1630 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      852 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     6818 2022-10-10 19:11:23.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     6384 2022-12-19 18:46:23.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     6657 2022-12-19 18:45:32.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     2124 2022-10-05 17:07:09.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store_object.py
--rw-r--r--   0 Justin     (502) staff       (20)     1751 2023-01-24 17:50:55.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     1414 2022-12-05 17:33:37.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)     1214 2022-11-28 17:35:44.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_property.py
--rw-r--r--   0 Justin     (502) staff       (20)      990 2022-11-29 01:10:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      681 2022-11-29 19:31:15.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1020 2022-12-02 19:07:37.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py
--rw-r--r--   0 Justin     (502) staff       (20)     1340 2022-12-03 00:58:02.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      924 2022-12-01 19:36:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py
--rw-r--r--   0 Justin     (502) staff       (20)      403 2022-12-09 00:20:12.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_attribute_value_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1175 2022-11-22 17:09:32.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      860 2022-11-22 17:17:39.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py
--rw-r--r--   0 Justin     (502) staff       (20)     1816 2022-12-19 19:40:35.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1479 2022-11-28 18:00:38.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py
--rw-r--r--   0 Justin     (502) staff       (20)     1834 2022-12-03 00:56:11.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1396 2022-11-30 19:33:37.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1807 2022-12-05 17:37:27.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)      726 2022-12-01 19:24:03.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1889 2022-12-13 17:12:23.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     2008 2022-12-13 17:11:14.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_query_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1161 2023-01-24 17:48:06.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_property.py
--rw-r--r--   0 Justin     (502) staff       (20)     1795 2023-01-25 00:41:35.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_property_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-01-24 17:48:35.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_telemetry.py
--rw-r--r--   0 Justin     (502) staff       (20)      984 2023-01-25 00:48:12.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      785 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/presigned_url.py
--rw-r--r--   0 Justin     (502) staff       (20)     1521 2022-12-08 19:15:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py
--rw-r--r--   0 Justin     (502) staff       (20)      727 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/server_response.py
--rw-r--r--   0 Justin     (502) staff       (20)     2594 2022-10-05 21:52:25.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/service.py
--rw-r--r--   0 Justin     (502) staff       (20)     1423 2022-09-29 19:12:44.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py
--rw-r--r--   0 Justin     (502) staff       (20)      811 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1408 2022-09-30 17:03:56.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1902 2022-09-29 19:12:59.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1384 2022-10-05 16:49:01.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_db.py
--rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 19:13:54.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py
--rw-r--r--   0 Justin     (502) staff       (20)      809 2022-09-29 19:11:31.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     3466 2022-09-30 16:48:18.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      640 2022-09-29 19:17:22.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py
--rw-r--r--   0 Justin     (502) staff       (20)      911 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      837 2022-09-29 19:18:29.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py
--rw-r--r--   0 Justin     (502) staff       (20)     1925 2022-09-30 00:39:31.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1334 2022-09-29 19:45:45.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:30:48.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1579 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/user.py
--rw-r--r--   0 Justin     (502) staff       (20)      176 2022-11-21 23:52:33.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/endpointUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     2597 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/exceptions.py
--rw-r--r--   0 Justin     (502) staff       (20)      460 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/globals.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.931805 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/
--rw-r--r--   0 Justin     (502) staff       (20)     1489 2022-09-29 19:23:24.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1469 2022-09-29 19:24:19.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      329 2023-05-17 16:29:16.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/dataCapture_publishData.py
--rw-r--r--   0 Justin     (502) staff       (20)     1055 2022-12-02 17:40:14.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1401 2023-02-15 19:36:31.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-02-14 23:10:32.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py
--rw-r--r--   0 Justin     (502) staff       (20)     1333 2022-12-01 20:55:30.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py
--rw-r--r--   0 Justin     (502) staff       (20)     1374 2022-11-23 17:59:59.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)     1375 2022-11-29 01:46:34.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py
--rw-r--r--   0 Justin     (502) staff       (20)     1410 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py
--rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:24:48.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1199 2022-09-29 19:25:14.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1204 2022-09-29 19:25:37.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1503 2022-09-29 19:25:41.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1825 2022-09-29 19:22:38.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.954533 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/
--rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1273 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1470 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py
--rw-r--r--   0 Justin     (502) staff       (20)     1247 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)     1776 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py
--rw-r--r--   0 Justin     (502) staff       (20)     1205 2022-12-03 00:56:58.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1779 2022-11-28 19:19:16.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py
--rw-r--r--   0 Justin     (502) staff       (20)     2454 2022-12-01 19:24:44.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py
--rw-r--r--   0 Justin     (502) staff       (20)     1394 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/query.py
--rw-r--r--   0 Justin     (502) staff       (20)     1189 2022-10-05 16:34:47.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py
--rw-r--r--   0 Justin     (502) staff       (20)     1327 2022-10-05 21:54:09.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1264 2022-10-05 21:53:38.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1417 2022-12-20 17:42:57.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py
--rw-r--r--   0 Justin     (502) staff       (20)     1195 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py
--rw-r--r--   0 Justin     (502) staff       (20)     1277 2022-09-29 18:46:04.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py
--rw-r--r--   0 Justin     (502) staff       (20)     1839 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py
--rw-r--r--   0 Justin     (502) staff       (20)     1216 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py
--rw-r--r--   0 Justin     (502) staff       (20)     3214 2022-09-30 00:23:31.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py
--rw-r--r--   0 Justin     (502) staff       (20)     2085 2022-09-29 19:12:18.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1021 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.956489 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_subscriptions/
--rw-r--r--   0 Justin     (502) staff       (20)     3353 2022-12-13 17:40:26.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py
--rw-r--r--   0 Justin     (502) staff       (20)     3526 2022-09-29 19:46:08.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1486 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py
--rw-r--r--   0 Justin     (502) staff       (20)     8418 2023-07-17 17:09:02.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/iotUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     1000 2023-06-13 20:20:28.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/logger.py
--rw-r--r--   0 Justin     (502) staff       (20)     6848 2023-07-14 23:41:31.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/subscriptionClient.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.729383 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/
--rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-07-17 20:01:00.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Justin     (502) staff       (20)    19552 2023-07-17 20:01:00.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Justin     (502) staff       (20)        1 2023-07-17 20:01:00.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Justin     (502) staff       (20)       53 2023-07-17 20:01:00.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/requires.txt
--rw-r--r--   0 Justin     (502) staff       (20)       28 2023-07-17 20:01:00.000000 avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 20:01:00.959062 avista_digital_exchange_sdk-0.3.2/tests/
--rw-r--r--   0 Justin     (502) staff       (20)      711 2023-07-17 18:43:02.000000 avista_digital_exchange_sdk-0.3.2/tests/test.py
--rw-r--r--   0 Justin     (502) staff       (20)      162 2023-06-15 16:15:35.000000 avista_digital_exchange_sdk-0.3.2/tests/test_dataCapture_publishData.py
--rw-r--r--   0 Justin     (502) staff       (20)     1541 2023-06-27 21:36:07.000000 avista_digital_exchange_sdk-0.3.2/tests/test_iot_publishData.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.673212 avista_digital_exchange_sdk-0.3.3/
+-rw-r--r--   0 Justin     (502) staff       (20)    35148 2022-09-13 20:02:44.000000 avista_digital_exchange_sdk-0.3.3/LICENSE
+-rw-r--r--   0 Justin     (502) staff       (20)    75213 2023-07-18 15:22:05.672715 avista_digital_exchange_sdk-0.3.3/PKG-INFO
+-rw-r--r--   0 Justin     (502) staff       (20)    33970 2023-07-17 23:33:05.000000 avista_digital_exchange_sdk-0.3.3/README.md
+-rw-r--r--   0 Justin     (502) staff       (20)     1021 2023-07-18 15:21:02.000000 avista_digital_exchange_sdk-0.3.3/pyproject.toml
+-rw-r--r--   0 Justin     (502) staff       (20)       38 2023-07-18 15:22:05.673338 avista_digital_exchange_sdk-0.3.3/setup.cfg
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.534119 avista_digital_exchange_sdk-0.3.3/src/
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.545502 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/
+-rw-r--r--   0 Justin     (502) staff       (20)     4950 2023-07-17 22:33:36.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/DxTypes.py
+-rw-r--r--   0 Justin     (502) staff       (20)      213 2023-06-14 18:10:08.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/__init__.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.619180 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/
+-rw-r--r--   0 Justin     (502) staff       (20)    94776 2023-07-17 22:57:17.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1951 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/base_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)   200668 2023-07-17 22:57:17.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/client.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10104 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_add_service_to_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5545 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_get_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     7026 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_member_organization_requests.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10171 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_services.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5665 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6610 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives_service_shared_with.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10544 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_remove_service_from_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5568 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_update_collaborative_member_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      675 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_attach_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_create_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1088 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_attachment.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1238 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_active_capture_data_export_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3976 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1229 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1100 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_export_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1906 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      738 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)      864 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_file_attachment_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      413 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_python_s_d_k_sample.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4288 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_handle_completion.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1100 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_attachments.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4568 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_captures.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4535 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_notify_capture_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1840 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_publish_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1228 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_regenerate_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4070 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_start_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4016 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_stop_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2024 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_data_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4137 2023-07-17 22:57:12.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/enums.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2483 2023-07-17 23:04:19.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/exceptions.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5844 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/input_types.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2523 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_add_endpoints_to_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      606 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_cancel_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1873 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_new_model_version.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      768 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_generate_query_result_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1011 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2135 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      554 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1543 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      390 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model_in_d_t_d_l_format.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2334 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoint_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1903 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoints_in_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2235 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2551 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups_endpoints_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)      610 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2495 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs_endpoints_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1617 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_models.py
+-rw-r--r--   0 Justin     (502) staff       (20)      837 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_notify_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2282 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)      954 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_query_by_time_range.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1081 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_regenerate_endpoint_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2779 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_remove_endpoints_from_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2062 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint_properties.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2146 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model_used_by_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     8310 2023-07-17 22:58:52.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/modified_async_base_client.py
+-rw-r--r--   0 Justin     (502) staff       (20)      842 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/notifications_notify_upload_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1783 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_capture_publish_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2417 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4069 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_capture_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      857 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_iot_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      956 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_time_series_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      731 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_upload_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3642 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_start_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3602 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_stop_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1414 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_time_series_db_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5859 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_add_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6089 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     9608 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_services.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5546 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      759 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1388 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5666 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)      801 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_organizations.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_users.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6610 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_collaboratives_ownership.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10525 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_services_ownership.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6021 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_remove_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1617 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_resend_user_invitation.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6021 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)      220 2023-07-17 22:57:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/scalars.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)      726 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1410 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file_data_view.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1328 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1410 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file_data_view.py
+-rw-r--r--   0 Justin     (502) staff       (20)      755 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3782 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1298 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      808 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      798 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_zip_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      797 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_list_data_stores.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1328 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      779 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_cancel_database_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_create_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_delete_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      992 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_generate_query_result_export_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      843 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_get_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2470 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_all_asset_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)      885 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_databases.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1059 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_notify_time_series_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1702 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_publish_to_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1022 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      912 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database_with_timestream_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_update_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1111 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_create_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1111 2023-07-17 22:57:13.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_delete_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1555 2023-07-17 22:57:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_get_user_session.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1117 2023-07-17 22:57:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_list_authentication_tokens.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1628 2023-07-18 15:20:11.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/avista_digital_exchange.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4712 2023-07-17 17:54:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/client.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3384 2022-12-02 17:38:29.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/collaborativeUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     7356 2023-07-17 22:42:18.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/dataCaptureUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2784 2022-12-02 17:57:07.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/dataStoreUtil.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.639098 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/
+-rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1989 2022-09-29 18:39:50.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1630 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      852 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6818 2022-10-10 19:11:23.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6384 2022-12-19 18:46:23.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6657 2022-12-19 18:45:32.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2124 2022-10-05 17:07:09.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store_object.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1751 2023-01-24 17:50:55.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1414 2022-12-05 17:33:37.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1214 2022-11-28 17:35:44.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_property.py
+-rw-r--r--   0 Justin     (502) staff       (20)      990 2022-11-29 01:10:28.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      681 2022-11-29 19:31:15.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1020 2022-12-02 19:07:37.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1340 2022-12-03 00:58:02.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      924 2022-12-01 19:36:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py
+-rw-r--r--   0 Justin     (502) staff       (20)      403 2022-12-09 00:20:12.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_attribute_value_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1175 2022-11-22 17:09:32.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      860 2022-11-22 17:17:39.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1816 2022-12-19 19:40:35.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1479 2022-11-28 18:00:38.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1834 2022-12-03 00:56:11.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1396 2022-11-30 19:33:37.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1807 2022-12-05 17:37:27.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)      726 2022-12-01 19:24:03.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1889 2022-12-13 17:12:23.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2008 2022-12-13 17:11:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_query_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1161 2023-01-24 17:48:06.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_property.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1795 2023-01-25 00:41:35.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_property_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-01-24 17:48:35.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_telemetry.py
+-rw-r--r--   0 Justin     (502) staff       (20)      984 2023-01-25 00:48:12.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/presigned_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1521 2022-12-08 19:15:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)      727 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/server_response.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2594 2022-10-05 21:52:25.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/service.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1423 2022-09-29 19:12:44.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py
+-rw-r--r--   0 Justin     (502) staff       (20)      811 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1408 2022-09-30 17:03:56.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1902 2022-09-29 19:12:59.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1384 2022-10-05 16:49:01.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_db.py
+-rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 19:13:54.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py
+-rw-r--r--   0 Justin     (502) staff       (20)      809 2022-09-29 19:11:31.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3466 2022-09-30 16:48:18.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      640 2022-09-29 19:17:22.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py
+-rw-r--r--   0 Justin     (502) staff       (20)      911 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      837 2022-09-29 19:18:29.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1925 2022-09-30 00:39:31.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1334 2022-09-29 19:45:45.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:30:48.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1579 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/user.py
+-rw-r--r--   0 Justin     (502) staff       (20)      176 2022-11-21 23:52:33.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/endpointUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2597 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/exceptions.py
+-rw-r--r--   0 Justin     (502) staff       (20)      460 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/globals.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.645858 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/
+-rw-r--r--   0 Justin     (502) staff       (20)     1489 2022-09-29 19:23:24.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1469 2022-09-29 19:24:19.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      329 2023-05-17 16:29:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/dataCapture_publishData.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1055 2022-12-02 17:40:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1401 2023-02-15 19:36:31.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-02-14 23:10:32.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1333 2022-12-01 20:55:30.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1374 2022-11-23 17:59:59.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1375 2022-11-29 01:46:34.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1410 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:24:48.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1199 2022-09-29 19:25:14.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1204 2022-09-29 19:25:37.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1503 2022-09-29 19:25:41.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1825 2022-09-29 19:22:38.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.655854 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/
+-rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1273 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1470 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1247 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1776 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1205 2022-12-03 00:56:58.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1779 2022-11-28 19:19:16.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2454 2022-12-01 19:24:44.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1394 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/query.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1189 2022-10-05 16:34:47.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1327 2022-10-05 21:54:09.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1264 2022-10-05 21:53:38.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1417 2022-12-20 17:42:57.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1195 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1277 2022-09-29 18:46:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1839 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1216 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3214 2022-09-30 00:23:31.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2085 2022-09-29 19:12:18.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1021 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.657363 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_subscriptions/
+-rw-r--r--   0 Justin     (502) staff       (20)     3353 2022-12-13 17:40:26.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3526 2022-09-29 19:46:08.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1486 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py
+-rw-r--r--   0 Justin     (502) staff       (20)     8418 2023-07-17 17:09:02.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/iotUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1000 2023-06-13 20:20:28.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/logger.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6847 2023-07-17 23:31:32.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/subscriptionClient.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.657855 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.658359 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/compliance/
+-rw-r--r--   0 Justin     (502) staff       (20)     1926 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/compliance/test_fuzzingclient.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.536954 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/docs/
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.658833 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/docs/source/
+-rw-r--r--   0 Justin     (502) staff       (20)     2337 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/docs/source/conf.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.660048 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/examples/
+-rw-r--r--   0 Justin     (502) staff       (20)      344 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/examples/echo_client.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1009 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/examples/echoapp_client.py
+-rw-r--r--   0 Justin     (502) staff       (20)      351 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/examples/rel_client.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2592 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/setup.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.666426 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/
+-rw-r--r--   0 Justin     (502) staff       (20)      801 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)    13656 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_abnf.py
+-rw-r--r--   0 Justin     (502) staff       (20)    21207 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_app.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2164 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_cookiejar.py
+-rw-r--r--   0 Justin     (502) staff       (20)    20110 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_core.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2116 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_exceptions.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6709 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_handshake.py
+-rw-r--r--   0 Justin     (502) staff       (20)    11816 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_http.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2220 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_logging.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5000 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_socket.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1122 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_ssl_compat.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4917 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3667 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_utils.py
+-rwxr-xr-x   0 Justin     (502) staff       (20)     7106 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/_wsdump.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.670137 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/
+-rw-r--r--   0 Justin     (502) staff       (20)        0 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)      486 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/echo-server.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4175 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_abnf.py
+-rw-r--r--   0 Justin     (502) staff       (20)    12681 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_app.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4325 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_cookiejar.py
+-rw-r--r--   0 Justin     (502) staff       (20)     9623 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_http.py
+-rw-r--r--   0 Justin     (502) staff       (20)    14589 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)    18072 2023-07-17 23:24:04.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_websocket.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.547395 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/
+-rw-r--r--   0 Justin     (502) staff       (20)    75213 2023-07-18 15:22:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Justin     (502) staff       (20)    21570 2023-07-18 15:22:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Justin     (502) staff       (20)        1 2023-07-18 15:22:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Justin     (502) staff       (20)       68 2023-07-18 15:22:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/requires.txt
+-rw-r--r--   0 Justin     (502) staff       (20)       28 2023-07-18 15:22:05.000000 avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-18 15:22:05.671786 avista_digital_exchange_sdk-0.3.3/tests/
+-rw-r--r--   0 Justin     (502) staff       (20)      711 2023-07-17 18:43:02.000000 avista_digital_exchange_sdk-0.3.3/tests/test.py
+-rw-r--r--   0 Justin     (502) staff       (20)      162 2023-06-15 16:15:35.000000 avista_digital_exchange_sdk-0.3.3/tests/test_dataCapture_publishData.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1541 2023-06-27 21:36:07.000000 avista_digital_exchange_sdk-0.3.3/tests/test_iot_publishData.py
```

### Comparing `avista_digital_exchange_sdk-0.3.2/LICENSE` & `avista_digital_exchange_sdk-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/PKG-INFO` & `avista_digital_exchange_sdk-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avista_digital_exchange_sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: SDK to programmatically access the Avista Digital Exchange
 Author-email: Justin Whicker <jwhicker@urbanova.org>, Jon Thompson <jon.thompson@avistacorp.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -753,14 +753,15 @@
     - [DxTypes.PublishCaptureDataFailedRecord](#dxtypespublishcapturedatafailedrecord)
     - [DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
     - [DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
   - [Development](#development)
   - [Deployment](#deployment)
   - [Generating Python types and GraphQL Client from GraphQL Schema](#generating-python-types-and-graphql-client-from-graphql-schema)
   - [Fix for py-graphql-mapper module](#fix-for-py-graphql-mapper-module)
+  - [websocketclient / websocket-client submodule](#websocketclient--websocket-client-submodule)
   - [Resources](#resources)
 
 ## Getting Started<a id="getting-started"></a>
 
 1. Install the python package.
 
 ```
@@ -1938,14 +1939,18 @@
     elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list):
 '''
 to
 '''
     elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list) or "gql_types.list_" in str(fieldType):
 '''
 
+## websocketclient / websocket-client submodule
+
+To mitigate an issue when using ```import websocket``` when both websocket and websocket-client packages are installed, we added a git submodule to reference websocket-client directly. Once the SDK moves away from the subscriptionClient.py usage, this can be removed.
+
 ## Resources<a id="resources"></a>
 
 1. [Avista Digital Exchange](https://energy.collaboratives.io/)
 2. [PyPi SDK project listing](https://pypi.org/project/avista-digital-exchange-sdk/)
 3. [GitHub project repository](https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk)
 4. [Python package deployment tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 5. [PyPi API Token](https://pypi.org/help/#apitoken)
```

### Comparing `avista_digital_exchange_sdk-0.3.2/README.md` & `avista_digital_exchange_sdk-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     - [DxTypes.PublishCaptureDataFailedRecord](#dxtypespublishcapturedatafailedrecord)
     - [DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
     - [DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
   - [Development](#development)
   - [Deployment](#deployment)
   - [Generating Python types and GraphQL Client from GraphQL Schema](#generating-python-types-and-graphql-client-from-graphql-schema)
   - [Fix for py-graphql-mapper module](#fix-for-py-graphql-mapper-module)
+  - [websocketclient / websocket-client submodule](#websocketclient--websocket-client-submodule)
   - [Resources](#resources)
 
 ## Getting Started<a id="getting-started"></a>
 
 1. Install the python package.
 
 ```
@@ -1249,14 +1250,18 @@
     elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list):
 '''
 to
 '''
     elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list) or "gql_types.list_" in str(fieldType):
 '''
 
+## websocketclient / websocket-client submodule
+
+To mitigate an issue when using ```import websocket``` when both websocket and websocket-client packages are installed, we added a git submodule to reference websocket-client directly. Once the SDK moves away from the subscriptionClient.py usage, this can be removed.
+
 ## Resources<a id="resources"></a>
 
 1. [Avista Digital Exchange](https://energy.collaboratives.io/)
 2. [PyPi SDK project listing](https://pypi.org/project/avista-digital-exchange-sdk/)
 3. [GitHub project repository](https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk)
 4. [Python package deployment tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 5. [PyPi API Token](https://pypi.org/help/#apitoken)
```

### Comparing `avista_digital_exchange_sdk-0.3.2/pyproject.toml` & `avista_digital_exchange_sdk-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0","requests", "httpx", "pydantic==1.10.8", "certifi", "websockets"] #  "py-graphql-mapper", "pip-system-certs"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avista_digital_exchange_sdk"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Justin Whicker", email="jwhicker@urbanova.org"},
   {  name="Jon Thompson", email="jon.thompson@avistacorp.com" }
 ]
 description = "SDK to programmatically access the Avista Digital Exchange"
 readme = "README.md"
-dependencies=["requests","pydantic==1.10.8","httpx","websocket","websockets"]
+dependencies=["requests","pydantic==1.10.8","httpx","websockets", "certifi", "pip-system-certs"]
 
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/DxTypes.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/DxTypes.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/__init__.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 
 from .base_model import BaseModel
 from .client import Client
 from .collaborative_add_service_to_collaborative import (
     CollaborativeAddServiceToCollaborative,
     CollaborativeAddServiceToCollaborativeCollaborativeAddServiceToCollaborative,
     CollaborativeAddServiceToCollaborativeCollaborativeAddServiceToCollaborativeDataCapture,
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/base_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/client.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import AsyncIterator, List, Optional, Union
 
 from .base_model import UNSET, UnsetType
 from .collaborative_add_service_to_collaborative import (
     CollaborativeAddServiceToCollaborative,
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_add_service_to_collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_add_service_to_collaborative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_get_collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_get_collaborative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_member_organization_requests.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_member_organization_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_services.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives_service_shared_with.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives_service_shared_with.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_remove_service_from_collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_remove_service_from_collaborative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_update_collaborative_member_organization.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_update_collaborative_member_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_attach_file.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_attach_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_create_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_create_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_attachment.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_active_capture_data_export_download_url.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_active_capture_data_export_download_url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture_authentication_token.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture_authentication_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_export_download_url.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_export_download_url.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model_export.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model_export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_file_attachment_download_url.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_file_attachment_download_url.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_handle_completion.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_handle_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_attachments.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_attachments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_captures.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_captures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_notify_capture_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_notify_capture_complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_publish_data.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_publish_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_regenerate_authentication_token.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_regenerate_authentication_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_start_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_start_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_stop_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_stop_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_data_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/enums.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../input/schema.graphql
 
 from enum import Enum
 
 
 class AuthenticationTokenType(str, Enum):
     DATA_CAPTURE_READ_WRITE = "DATA_CAPTURE_READ_WRITE"
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/exceptions.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 
 # Generated by ariadne-codegen on 2023-07-17 11:03
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
@@ -44,14 +44,16 @@
         self.orginal = orginal
 
     def __str__(self) -> str:
         return self.message
 
     @classmethod
     def from_dict(cls, error: dict[str, Any]) -> "GraphQLClientGraphQLError":
+        print("from_dict")
+        print(error)
         return cls(
             message=error["message"],
             locations=error.get("locations"),
             path=error.get("path"),
             extensions=error.get("extensions"),
             orginal=error,
         )
@@ -66,15 +68,16 @@
         return "; ".join(str(e) for e in self.errors)
 
     @classmethod
     def from_errors_dicts(
         cls, errors_dicts: List[dict[str, Any]], data: dict[str, Any]
     ) -> "GraphQLClientGraphQLMultiError":
         return cls(
-            errors=[GraphQLClientGraphQLError.from_dict(e) for e in errors_dicts],
+            errors=[GraphQLClientGraphQLError.from_dict(
+                e) for e in errors_dicts],
             data=data,
         )
 
 
 class GraphQLClientInvalidMessageFormat(GraphQLClientError):
     def __init__(self, message: Union[str, bytes]) -> None:
         self.message = message
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/input_types.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../input/schema.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_add_endpoints_to_group.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_add_endpoints_to_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_endpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_group.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_hub.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_new_model_version.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_new_model_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_endpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_group.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_hub.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_hub.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_generate_query_result_export.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_generate_query_result_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint_token.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_group.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_hub.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoint_last_values.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoint_last_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoints_in_hub.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoints_in_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups_endpoints_last_values.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups_endpoints_last_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs_endpoints_last_values.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs_endpoints_last_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_models.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_notify_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_notify_query_export_complete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_publish.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_query_by_time_range.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_query_by_time_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_regenerate_endpoint_token.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_regenerate_endpoint_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_remove_endpoints_from_group.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_remove_endpoints_from_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint_properties.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_group.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_hub.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_hub.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model_used_by_endpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model_used_by_endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/modified_async_base_client.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/modified_async_base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 
 # Generated by ariadne-codegen on 2023-06-08 15:03
 
 from typing import Any, Dict, List, Optional, Union
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
@@ -44,18 +44,16 @@
 
 GRAPHQL_TRANSPORT_WS = "graphql-ws"
 
 
 class GraphQLTransportWSMessageType(str, enum.Enum):
     CONNECTION_INIT = "connection_init"
     CONNECTION_ACK = "connection_ack"
-    PING = "ping"
-    PONG = "pong"
+    CONNECTION_ERROR = "connection_error"
     SUBSCRIBE = "subscribe"
-    NEXT = "next"
     ERROR = "error"
     COMPLETE = "complete"
     KA = "ka"
     START = "start"
     START_ACK = "start_ack"
     DATA = "data"
     STOP = "stop"
@@ -135,38 +133,35 @@
     async def execute_ws(
         self, query: str, variables: Optional[Dict[str, Any]] = None
     ) -> AsyncIterator[Dict[str, Any]]:
         operation_id = str(uuid4())
 
         async with ws_connect(
             self.ws_url,
-            subprotocols=["graphql-ws"],
+            subprotocols=[Subprotocol(GRAPHQL_TRANSPORT_WS)],
             origin=self.ws_origin,
             extra_headers=self.ws_headers,
         ) as websocket:
             def quitHandler(signum, frame):
                 # Stop subscription on terminate
-                print("Cancelling data subscription....")
                 self._send_stop(websocket=websocket, operation_id=operation_id)
-                exit()
 
             signal.signal(signal.SIGINT, quitHandler)
 
             await self._send_connection_init(websocket)
 
             await self._send_subscribe(
                 websocket,
                 operation_id=operation_id,
                 query=query,
                 variables=variables,
             )
 
             async for message in websocket:
                 data = await self._handle_ws_message(message, websocket)
-                print(data)
                 if data:
                     yield data
 
     def _convert_dict_to_json_serializable(
         self, dict_: Dict[str, Any]
     ) -> Dict[str, Any]:
         return {
@@ -229,35 +224,25 @@
         try:
             message_dict = json.loads(message)
         except json.JSONDecodeError as exc:
             raise GraphQLClientInvalidMessageFormat(message=message) from exc
 
         type_ = message_dict.get("type")
         payload = message_dict.get("payload", {})
-
+        print(type_)
+        print(payload)
         if not type_ or type_ not in {t.value for t in GraphQLTransportWSMessageType}:
             raise GraphQLClientInvalidMessageFormat(message=message)
 
         if type_ == GraphQLTransportWSMessageType.KA:
-            print("ka message received")
+            return None
         elif type_ == GraphQLTransportWSMessageType.DATA:
-            print("data message received")
             return cast(Dict[str, Any], payload["data"])
         elif type_ == GraphQLTransportWSMessageType.ERROR:
-            print("error message received")
             raise GraphQLClientGraphQLMultiError.from_errors_dicts(
                 errors_dicts=payload, data=message_dict
             )
-        return None
-        if type_ == GraphQLTransportWSMessageType.NEXT:
-            if "data" not in payload:
-                raise GraphQLClientInvalidMessageFormat(message=message)
-            return cast(Dict[str, Any], payload["data"])
-
-        if type_ == GraphQLTransportWSMessageType.COMPLETE:
-            await websocket.close()
-        elif type_ == GraphQLTransportWSMessageType.PING:
-            await websocket.send(
-                json.dumps({"type": GraphQLTransportWSMessageType.PONG.value})
+        elif type_ == GraphQLTransportWSMessageType.CONNECTION_ERROR:
+            raise GraphQLClientGraphQLMultiError.from_errors_dicts(
+                errors_dicts=payload, data=message_dict
             )
-
         return None
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/notifications_notify_upload_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/notifications_notify_upload_complete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_capture_publish_data.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_capture_publish_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_iot_publish.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_iot_publish.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_capture_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_capture_complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_iot_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_iot_query_export_complete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_time_series_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_time_series_query_export_complete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_upload_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_upload_complete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_start_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_start_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_stop_capture.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_stop_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/on_time_series_db_publish.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/on_time_series_db_publish.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_add_collaborative_member.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_add_collaborative_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_collaborative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_organization.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_organization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_user.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_collaborative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_organization.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_organization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_user.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_collaboratives.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_collaboratives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_services.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_collaborative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_organization.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_user.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_collaboratives.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_collaboratives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_organizations.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_users.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_collaboratives_ownership.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_collaboratives_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_services_ownership.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_services_ownership.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_remove_collaborative_member.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_remove_collaborative_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_resend_user_invitation.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_resend_user_invitation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative_member.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative_member.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_organization.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_user.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file_data_view.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file_data_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file_data_view.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file_data_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file_download_url.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file_download_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_zip_download_url.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_zip_download_url.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_list_data_stores.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_list_data_stores.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_file.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_cancel_database_query.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_cancel_database_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_create_database.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_create_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_delete_database.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_delete_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_generate_query_result_export_file.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_generate_query_result_export_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_get_database.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_get_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_all_asset_last_values.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_all_asset_last_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_databases.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_databases.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_notify_time_series_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_notify_time_series_query_export_complete.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_publish_to_database.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_publish_to_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database_with_timestream_query.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database_with_timestream_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_update_database.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_update_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_create_authentication_token.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_create_authentication_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_delete_authentication_token.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_delete_authentication_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_get_user_session.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_get_user_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/async_graphql_client/user_list_authentication_tokens.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/async_graphql_client/user_list_authentication_tokens.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 11:23
+# Generated by ariadne-codegen on 2023-07-17 15:57
 # Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/avista_digital_exchange.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/avista_digital_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class AvistaDigitalExchange(object):
 
     def __init__(self, token, debug=False):
         if type(debug) is not bool:
             raise InvalidParameterException(
                 "AvistaDigitalExchange debug parameter must be a bool")
-        self._stage: str = "DEVELOPMENT"
+        self._stage: str = "PRODUCTION"
         self._debug: bool = debug
         self._token: str = token
         self._client: Client = Client(self._token, self._stage, self._debug)
         self._logger: Logger = logging.getLogger(name="dx-logger")
         self._logger.setLevel(20)
         self.iot: IoTUtil = IoTUtil(self._debug, self._client)
         # self.collaboratives = CollaborativeUtil(self._debug, self._client)
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/client.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/client.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/collaborativeUtil.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/collaborativeUtil.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/dataCaptureUtil.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/dataCaptureUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from logging import Logger
-from typing import List
+from typing import AsyncIterator, List
 from .async_graphql_client import exceptions, input_types
 from .client import Client as DxClient
 from . import DxTypes
 
 
 class DataCaptureUtil(object):
     _debug: bool
@@ -12,21 +12,24 @@
     _logger: Logger
 
     def __init__(self, debug: bool, client: DxClient, logger: Logger):
         self._debug = debug
         self._client = client
         self._logger = logger
 
-    async def listenForCaptureData(self, captureId: str):
-        print("Subscribing to capture data....")
+    async def listenForCaptureData(self, captureId: str) -> AsyncIterator[DxTypes.PublishCaptureDataResult]:
+        if self._debug:
+            print("Subscribing to capture data....")
         async for item in self._client.updatedGqlClient.on_capture_publish_data(
                 capture_id=captureId):
-            print("In for loop...")
-            print("Subscription item....")
-            print(item)
+            if self._debug:
+                print("DataCapture.listenForCaptureData: Data received.")
+            result = DxTypes.PublishCaptureDataResult.fromCapturePublishResult(
+                item.on_capture_publish_data)
+            yield result
 
     async def publishData(self, captureId: str, data: List[DxTypes.CaptureDataRecordInput]) -> DxTypes.PublishCaptureDataResult:
         if self._debug:
             print("DataCapture.publishData: - processing data input")
 
         # Format data records argument
         dataRecords: List[input_types.DataCaptureDataRecordInput] = []
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/dataStoreUtil.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/dataStoreUtil.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/collaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/collaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store_directory.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store_directory.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store_file.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store_file.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/data_store_object.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/data_store_object.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_property.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_property.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/iot_query_export.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/iot_query_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_property.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_property.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_property_input.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_property_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_telemetry.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_telemetry.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/organization.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/organization.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/presigned_url.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/presigned_url.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/server_response.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/server_response.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/service.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/service.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_db.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_db.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/data_types/user.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/data_types/user.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/exceptions.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/query.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/query.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/iotUtil.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/iotUtil.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/logger.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk/subscriptionClient.py` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk/subscriptionClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # subscription_client.py
 
 from base64 import b64encode, decode
 from datetime import datetime
 # from lib2to3.pgen2 import token
 from uuid import uuid4
 
-import websocket
+from .websocketclient.websocket import WebSocketApp
 import threading
 
 import json
 import ssl
 
 global globToken
 global SUB_ID
@@ -77,25 +77,26 @@
         #  also defines callback functions for websocket events
         #  NOTE: The connection requires a subprotocol 'graphql-ws'
 
         # Uncomment to see socket bytestreams
         # websocket.enableTrace(True)
         if self._debug:
             print('Connecting to: ' + self.connectionUrl)
-        self.ws = websocket.WebSocketApp(self.connectionUrl,
-                                         subprotocols=['graphql-ws'],
-                                         on_open=self.onOpen,
-                                         on_message=self.onMessage,
-                                         on_error=self.onError,
-                                         on_close=self.onClose)
+        self.ws = WebSocketApp(self.connectionUrl,
+                               subprotocols=['graphql-ws'],
+                               on_open=self.onOpen,
+                               on_message=self.onMessage,
+                               on_error=self.onError,
+                               on_close=self.onClose)
         # ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
         self.ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
 
     def stop(self):
-        self.ws.close()
+        if self.ws:
+            self.ws.close()
 
     def onMessage(self, ws, message):
         """Socket Event Callbacks, used in WebSocketApp Constructor"""
 
         global globToken
         global SUB_ID
         global timeoutTimer
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/PKG-INFO` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avista-digital-exchange-sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: SDK to programmatically access the Avista Digital Exchange
 Author-email: Justin Whicker <jwhicker@urbanova.org>, Jon Thompson <jon.thompson@avistacorp.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -753,14 +753,15 @@
     - [DxTypes.PublishCaptureDataFailedRecord](#dxtypespublishcapturedatafailedrecord)
     - [DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
     - [DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
   - [Development](#development)
   - [Deployment](#deployment)
   - [Generating Python types and GraphQL Client from GraphQL Schema](#generating-python-types-and-graphql-client-from-graphql-schema)
   - [Fix for py-graphql-mapper module](#fix-for-py-graphql-mapper-module)
+  - [websocketclient / websocket-client submodule](#websocketclient--websocket-client-submodule)
   - [Resources](#resources)
 
 ## Getting Started<a id="getting-started"></a>
 
 1. Install the python package.
 
 ```
@@ -1938,14 +1939,18 @@
     elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list):
 '''
 to
 '''
     elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list) or "gql_types.list_" in str(fieldType):
 '''
 
+## websocketclient / websocket-client submodule
+
+To mitigate an issue when using ```import websocket``` when both websocket and websocket-client packages are installed, we added a git submodule to reference websocket-client directly. Once the SDK moves away from the subscriptionClient.py usage, this can be removed.
+
 ## Resources<a id="resources"></a>
 
 1. [Avista Digital Exchange](https://energy.collaboratives.io/)
 2. [PyPi SDK project listing](https://pypi.org/project/avista-digital-exchange-sdk/)
 3. [GitHub project repository](https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk)
 4. [Python package deployment tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 5. [PyPi API Token](https://pypi.org/help/#apitoken)
```

### Comparing `avista_digital_exchange_sdk-0.3.2/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt` & `avista_digital_exchange_sdk-0.3.3/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -244,10 +244,38 @@
 src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py
 src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py
 src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py
 src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py
 src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py
 src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py
 src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py
+src/avista_digital_exchange_sdk/websocketclient/setup.py
+src/avista_digital_exchange_sdk/websocketclient/compliance/test_fuzzingclient.py
+src/avista_digital_exchange_sdk/websocketclient/docs/source/conf.py
+src/avista_digital_exchange_sdk/websocketclient/examples/echo_client.py
+src/avista_digital_exchange_sdk/websocketclient/examples/echoapp_client.py
+src/avista_digital_exchange_sdk/websocketclient/examples/rel_client.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/__init__.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_abnf.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_app.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_cookiejar.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_core.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_exceptions.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_handshake.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_http.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_logging.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_socket.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_ssl_compat.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_url.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_utils.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/_wsdump.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/__init__.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/echo-server.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_abnf.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_app.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_cookiejar.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_http.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_url.py
+src/avista_digital_exchange_sdk/websocketclient/websocket/tests/test_websocket.py
 tests/test.py
 tests/test_dataCapture_publishData.py
 tests/test_iot_publishData.py
```

### Comparing `avista_digital_exchange_sdk-0.3.2/tests/test.py` & `avista_digital_exchange_sdk-0.3.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.2/tests/test_iot_publishData.py` & `avista_digital_exchange_sdk-0.3.3/tests/test_iot_publishData.py`

 * *Files identical despite different names*

