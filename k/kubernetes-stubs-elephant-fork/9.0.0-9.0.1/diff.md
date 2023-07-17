# Comparing `tmp/kubernetes-stubs-elephant-fork-9.0.0.tar.gz` & `tmp/kubernetes-stubs-elephant-fork-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernetes-stubs-elephant-fork-9.0.0.tar", max compression
+gzip compressed data, was "kubernetes-stubs-elephant-fork-9.0.1.tar", max compression
```

## Comparing `kubernetes-stubs-elephant-fork-9.0.0.tar` & `kubernetes-stubs-elephant-fork-9.0.1.tar`

### file list

```diff
@@ -1,652 +1,652 @@
--rw-r--r--   0        0        0      517 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 06:21:59.619735 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/__init__.pyi
--rw-r--r--   0        0        0   146454 2023-06-02 06:22:01.303762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/__init__.pyi
--rw-r--r--   0        0        0     5701 2023-06-02 06:22:01.787770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/__init__.pyi
--rw-r--r--   0        0        0      254 2023-06-02 06:22:01.783770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/admissionregistration_api.pyi
--rw-r--r--   0        0        0     2650 2023-06-02 06:22:01.771770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/admissionregistration_v1alpha1_api.pyi
--rw-r--r--   0        0        0     5166 2023-06-02 06:22:01.755769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/admissionregistration_v1beta1_api.pyi
--rw-r--r--   0        0        0      246 2023-06-02 06:22:01.751769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiextensions_api.pyi
--rw-r--r--   0        0        0     3301 2023-06-02 06:22:01.783770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiextensions_v1beta1_api.pyi
--rw-r--r--   0        0        0      248 2023-06-02 06:22:01.771770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiregistration_api.pyi
--rw-r--r--   0        0        0     2939 2023-06-02 06:22:01.763769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiregistration_v1_api.pyi
--rw-r--r--   0        0        0     2999 2023-06-02 06:22:01.775770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiregistration_v1beta1_api.pyi
--rw-r--r--   0        0        0      244 2023-06-02 06:22:01.755769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apis_api.pyi
--rw-r--r--   0        0        0      237 2023-06-02 06:22:01.767770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apps_api.pyi
--rw-r--r--   0        0        0    18683 2023-06-02 06:22:01.771770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apps_v1_api.pyi
--rw-r--r--   0        0        0    11841 2023-06-02 06:22:01.747769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apps_v1beta1_api.pyi
--rw-r--r--   0        0        0    19028 2023-06-02 06:22:01.747769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apps_v1beta2_api.pyi
--rw-r--r--   0        0        0      250 2023-06-02 06:22:01.743769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/auditregistration_api.pyi
--rw-r--r--   0        0        0     2436 2023-06-02 06:22:01.751769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/auditregistration_v1alpha1_api.pyi
--rw-r--r--   0        0        0      247 2023-06-02 06:22:01.751769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authentication_api.pyi
--rw-r--r--   0        0        0      509 2023-06-02 06:22:01.755769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authentication_v1_api.pyi
--rw-r--r--   0        0        0      524 2023-06-02 06:22:01.775770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authentication_v1beta1_api.pyi
--rw-r--r--   0        0        0      246 2023-06-02 06:22:01.751769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authorization_api.pyi
--rw-r--r--   0        0        0     1421 2023-06-02 06:22:01.759770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authorization_v1_api.pyi
--rw-r--r--   0        0        0     1466 2023-06-02 06:22:01.771770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authorization_v1beta1_api.pyi
--rw-r--r--   0        0        0      244 2023-06-02 06:22:01.759770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/autoscaling_api.pyi
--rw-r--r--   0        0        0     3996 2023-06-02 06:22:01.767770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/autoscaling_v1_api.pyi
--rw-r--r--   0        0        0     4061 2023-06-02 06:22:01.759770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/autoscaling_v2beta1_api.pyi
--rw-r--r--   0        0        0     4061 2023-06-02 06:22:01.779770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/autoscaling_v2beta2_api.pyi
--rw-r--r--   0        0        0      238 2023-06-02 06:22:01.787770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/batch_api.pyi
--rw-r--r--   0        0        0     3508 2023-06-02 06:22:01.767770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/batch_v1_api.pyi
--rw-r--r--   0        0        0     3676 2023-06-02 06:22:01.747769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/batch_v1beta1_api.pyi
--rw-r--r--   0        0        0     3689 2023-06-02 06:22:01.755769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/batch_v2alpha1_api.pyi
--rw-r--r--   0        0        0      245 2023-06-02 06:22:01.775770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/certificates_api.pyi
--rw-r--r--   0        0        0     3592 2023-06-02 06:22:01.779770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/certificates_v1beta1_api.pyi
--rw-r--r--   0        0        0      245 2023-06-02 06:22:01.763769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/coordination_api.pyi
--rw-r--r--   0        0        0     3024 2023-06-02 06:22:01.771770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/coordination_v1beta1_api.pyi
--rw-r--r--   0        0        0      243 2023-06-02 06:22:01.755769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/core_api.pyi
--rw-r--r--   0        0        0    54192 2023-06-02 06:22:01.763769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/core_v1_api.pyi
--rw-r--r--   0        0        0     4499 2023-06-02 06:22:01.767770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/custom_objects_api.pyi
--rw-r--r--   0        0        0      239 2023-06-02 06:22:01.767770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/events_api.pyi
--rw-r--r--   0        0        0     3018 2023-06-02 06:22:01.783770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/events_v1beta1_api.pyi
--rw-r--r--   0        0        0      243 2023-06-02 06:22:01.779770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/extensions_api.pyi
--rw-r--r--   0        0        0    21799 2023-06-02 06:22:01.751769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/extensions_v1beta1_api.pyi
--rw-r--r--   0        0        0      287 2023-06-02 06:22:01.759770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/logs_api.pyi
--rw-r--r--   0        0        0      243 2023-06-02 06:22:01.775770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/networking_api.pyi
--rw-r--r--   0        0        0     3113 2023-06-02 06:22:01.779770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/networking_v1_api.pyi
--rw-r--r--   0        0        0      239 2023-06-02 06:22:01.779770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/policy_api.pyi
--rw-r--r--   0        0        0     6285 2023-06-02 06:22:01.775770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/policy_v1beta1_api.pyi
--rw-r--r--   0        0        0      250 2023-06-02 06:22:01.747769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/rbacAuthorization_api.pyi
--rw-r--r--   0        0        0     9912 2023-06-02 06:22:01.775770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/rbacAuthorization_v1_api.pyi
--rw-r--r--   0        0        0    10098 2023-06-02 06:22:01.759770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/rbacAuthorization_v1alpha1_api.pyi
--rw-r--r--   0        0        0    10067 2023-06-02 06:22:01.787770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/rbacAuthorization_v1beta1_api.pyi
--rw-r--r--   0        0        0      243 2023-06-02 06:22:01.771770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/scheduling_api.pyi
--rw-r--r--   0        0        0     2485 2023-06-02 06:22:01.755769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/scheduling_v1alpha1_api.pyi
--rw-r--r--   0        0        0     2477 2023-06-02 06:22:01.763769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/scheduling_v1beta1_api.pyi
--rw-r--r--   0        0        0      241 2023-06-02 06:22:01.783770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/settings_api.pyi
--rw-r--r--   0        0        0     3101 2023-06-02 06:22:01.751769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/settings_v1alpha1_api.pyi
--rw-r--r--   0        0        0      240 2023-06-02 06:22:01.767770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/storage_api.pyi
--rw-r--r--   0        0        0     5224 2023-06-02 06:22:01.759770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/storage_v1_api.pyi
--rw-r--r--   0        0        0     2524 2023-06-02 06:22:01.747769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/storage_v1alpha1_api.pyi
--rw-r--r--   0        0        0     4718 2023-06-02 06:22:01.779770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/storage_v1beta1_api.pyi
--rw-r--r--   0        0        0      236 2023-06-02 06:22:01.743769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/version_api.pyi
--rw-r--r--   0        0        0      420 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api_client.pyi
--rw-r--r--   0        0        0      496 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/configuration.pyi
--rw-r--r--   0        0        0     1165 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/exceptions.pyi
--rw-r--r--   0        0        0   140444 2023-06-02 06:22:01.715769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/__init__.pyi
--rw-r--r--   0        0        0      524 2023-06-02 06:22:01.427764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/admissionregistration_v1beta1_service_reference.pyi
--rw-r--r--   0        0        0      833 2023-06-02 06:22:01.339763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/admissionregistration_v1beta1_webhook_client_config.pyi
--rw-r--r--   0        0        0      500 2023-06-02 06:22:01.351763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apiextensions_v1beta1_service_reference.pyi
--rw-r--r--   0        0        0      785 2023-06-02 06:22:01.431764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apiextensions_v1beta1_webhook_client_config.pyi
--rw-r--r--   0        0        0      524 2023-06-02 06:22:01.583767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apiregistration_v1beta1_service_reference.pyi
--rw-r--r--   0        0        0     1123 2023-06-02 06:22:01.371763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment.pyi
--rw-r--r--   0        0        0      940 2023-06-02 06:22:01.651768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_condition.pyi
--rw-r--r--   0        0        0      849 2023-06-02 06:22:01.627767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_list.pyi
--rw-r--r--   0        0        0      897 2023-06-02 06:22:01.375764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_rollback.pyi
--rw-r--r--   0        0        0     1766 2023-06-02 06:22:01.371763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_spec.pyi
--rw-r--r--   0        0        0     1467 2023-06-02 06:22:01.431764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_status.pyi
--rw-r--r--   0        0        0      662 2023-06-02 06:22:01.467765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_strategy.pyi
--rw-r--r--   0        0        0      386 2023-06-02 06:22:01.359763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_rollback_config.pyi
--rw-r--r--   0        0        0      585 2023-06-02 06:22:01.323763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_rolling_update_deployment.pyi
--rw-r--r--   0        0        0     1078 2023-06-02 06:22:01.483765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_scale.pyi
--rw-r--r--   0        0        0      371 2023-06-02 06:22:01.311762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_scale_spec.pyi
--rw-r--r--   0        0        0      589 2023-06-02 06:22:01.511766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_scale_status.pyi
--rw-r--r--   0        0        0      350 2023-06-02 06:22:01.515766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_allowed_flex_volume.pyi
--rw-r--r--   0        0        0      528 2023-06-02 06:22:01.511766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_allowed_host_path.pyi
--rw-r--r--   0        0        0     1177 2023-06-02 06:22:01.575767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment.pyi
--rw-r--r--   0        0        0      958 2023-06-02 06:22:01.343763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_condition.pyi
--rw-r--r--   0        0        0      885 2023-06-02 06:22:01.663768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_list.pyi
--rw-r--r--   0        0        0      933 2023-06-02 06:22:01.439765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_rollback.pyi
--rw-r--r--   0        0        0     1820 2023-06-02 06:22:01.419764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_spec.pyi
--rw-r--r--   0        0        0     1503 2023-06-02 06:22:01.583767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_status.pyi
--rw-r--r--   0        0        0      698 2023-06-02 06:22:01.659768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_strategy.pyi
--rw-r--r--   0        0        0      657 2023-06-02 06:22:01.367763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_fs_group_strategy_options.pyi
--rw-r--r--   0        0        0      365 2023-06-02 06:22:01.583767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_host_port_range.pyi
--rw-r--r--   0        0        0      347 2023-06-02 06:22:01.403764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_id_range.pyi
--rw-r--r--   0        0        0      969 2023-06-02 06:22:01.651768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy.pyi
--rw-r--r--   0        0        0      927 2023-06-02 06:22:01.735769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_list.pyi
--rw-r--r--   0        0        0     4524 2023-06-02 06:22:01.723769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_spec.pyi
--rw-r--r--   0        0        0      404 2023-06-02 06:22:01.743769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_rollback_config.pyi
--rw-r--r--   0        0        0      603 2023-06-02 06:22:01.387764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_rolling_update_deployment.pyi
--rw-r--r--   0        0        0      609 2023-06-02 06:22:01.347763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_run_as_group_strategy_options.pyi
--rw-r--r--   0        0        0      606 2023-06-02 06:22:01.655768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_run_as_user_strategy_options.pyi
--rw-r--r--   0        0        0     1132 2023-06-02 06:22:01.343763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_scale.pyi
--rw-r--r--   0        0        0      389 2023-06-02 06:22:01.411764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_scale_spec.pyi
--rw-r--r--   0        0        0      607 2023-06-02 06:22:01.559766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_scale_status.pyi
--rw-r--r--   0        0        0      586 2023-06-02 06:22:01.539766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_se_linux_strategy_options.pyi
--rw-r--r--   0        0        0      690 2023-06-02 06:22:01.499765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_supplemental_groups_strategy_options.pyi
--rw-r--r--   0        0        0      338 2023-06-02 06:22:01.331763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_allowed_flex_volume.pyi
--rw-r--r--   0        0        0      516 2023-06-02 06:22:01.487765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_allowed_host_path.pyi
--rw-r--r--   0        0        0      633 2023-06-02 06:22:01.439765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_fs_group_strategy_options.pyi
--rw-r--r--   0        0        0      353 2023-06-02 06:22:01.503766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_host_port_range.pyi
--rw-r--r--   0        0        0      335 2023-06-02 06:22:01.415764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_id_range.pyi
--rw-r--r--   0        0        0      945 2023-06-02 06:22:01.383764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy.pyi
--rw-r--r--   0        0        0      903 2023-06-02 06:22:01.387764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_list.pyi
--rw-r--r--   0        0        0     4416 2023-06-02 06:22:01.443765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_spec.pyi
--rw-r--r--   0        0        0      585 2023-06-02 06:22:01.663768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_run_as_group_strategy_options.pyi
--rw-r--r--   0        0        0      582 2023-06-02 06:22:01.475765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_run_as_user_strategy_options.pyi
--rw-r--r--   0        0        0      574 2023-06-02 06:22:01.471765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_se_linux_strategy_options.pyi
--rw-r--r--   0        0        0      666 2023-06-02 06:22:01.455765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_supplemental_groups_strategy_options.pyi
--rw-r--r--   0        0        0      296 2023-06-02 06:22:01.423764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/runtime_raw_extension.pyi
--rw-r--r--   0        0        0      886 2023-06-02 06:22:01.647768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_affinity.pyi
--rw-r--r--   0        0        0      514 2023-06-02 06:22:01.451765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_aggregation_rule.pyi
--rw-r--r--   0        0        0     1261 2023-06-02 06:22:01.543766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_group.pyi
--rw-r--r--   0        0        0      599 2023-06-02 06:22:01.603767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_group_list.pyi
--rw-r--r--   0        0        0      975 2023-06-02 06:22:01.531766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_resource.pyi
--rw-r--r--   0        0        0      691 2023-06-02 06:22:01.563767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_resource_list.pyi
--rw-r--r--   0        0        0     1042 2023-06-02 06:22:01.307762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service.pyi
--rw-r--r--   0        0        0      741 2023-06-02 06:22:01.371763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service_condition.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.403764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service_list.pyi
--rw-r--r--   0        0        0     1037 2023-06-02 06:22:01.735769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service_spec.pyi
--rw-r--r--   0        0        0      501 2023-06-02 06:22:01.575767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service_status.pyi
--rw-r--r--   0        0        0      786 2023-06-02 06:22:01.619767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_versions.pyi
--rw-r--r--   0        0        0      349 2023-06-02 06:22:01.547766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_attached_volume.pyi
--rw-r--r--   0        0        0      686 2023-06-02 06:22:01.479765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_aws_elastic_block_store_volume_source.pyi
--rw-r--r--   0        0        0      807 2023-06-02 06:22:01.371763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_azure_disk_volume_source.pyi
--rw-r--r--   0        0        0      661 2023-06-02 06:22:01.515766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_azure_file_persistent_volume_source.pyi
--rw-r--r--   0        0        0      500 2023-06-02 06:22:01.487765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_azure_file_volume_source.pyi
--rw-r--r--   0        0        0      780 2023-06-02 06:22:01.567767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_binding.pyi
--rw-r--r--   0        0        0      470 2023-06-02 06:22:01.327763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_capabilities.pyi
--rw-r--r--   0        0        0      996 2023-06-02 06:22:01.515766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_ceph_fs_persistent_volume_source.pyi
--rw-r--r--   0        0        0      981 2023-06-02 06:22:01.607767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_ceph_fs_volume_source.pyi
--rw-r--r--   0        0        0      776 2023-06-02 06:22:01.519766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cinder_persistent_volume_source.pyi
--rw-r--r--   0        0        0      761 2023-06-02 06:22:01.435764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cinder_volume_source.pyi
--rw-r--r--   0        0        0      379 2023-06-02 06:22:01.491765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_client_ip_config.pyi
--rw-r--r--   0        0        0     1023 2023-06-02 06:22:01.487765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role.pyi
--rw-r--r--   0        0        0      996 2023-06-02 06:22:01.727769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role_binding.pyi
--rw-r--r--   0        0        0      843 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role_binding_list.pyi
--rw-r--r--   0        0        0      801 2023-06-02 06:22:01.739769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role_list.pyi
--rw-r--r--   0        0        0      551 2023-06-02 06:22:01.655768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_component_condition.pyi
--rw-r--r--   0        0        0      900 2023-06-02 06:22:01.391764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_component_status.pyi
--rw-r--r--   0        0        0      825 2023-06-02 06:22:01.511766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_component_status_list.pyi
--rw-r--r--   0        0        0      919 2023-06-02 06:22:01.635768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map.pyi
--rw-r--r--   0        0        0      470 2023-06-02 06:22:01.615767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_env_source.pyi
--rw-r--r--   0        0        0      512 2023-06-02 06:22:01.643768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_key_selector.pyi
--rw-r--r--   0        0        0      789 2023-06-02 06:22:01.335763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_list.pyi
--rw-r--r--   0        0        0      680 2023-06-02 06:22:01.531766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_node_config_source.pyi
--rw-r--r--   0        0        0      672 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_projection.pyi
--rw-r--r--   0        0        0      797 2023-06-02 06:22:01.399764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_volume_source.pyi
--rw-r--r--   0        0        0     3607 2023-06-02 06:22:01.627767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container.pyi
--rw-r--r--   0        0        0      424 2023-06-02 06:22:01.619767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_image.pyi
--rw-r--r--   0        0        0      734 2023-06-02 06:22:01.483765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_port.pyi
--rw-r--r--   0        0        0      938 2023-06-02 06:22:01.723769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_state.pyi
--rw-r--r--   0        0        0      427 2023-06-02 06:22:01.631768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_state_running.pyi
--rw-r--r--   0        0        0     1075 2023-06-02 06:22:01.403764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_state_terminated.pyi
--rw-r--r--   0        0        0      479 2023-06-02 06:22:01.347763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_state_waiting.pyi
--rw-r--r--   0        0        0     1020 2023-06-02 06:22:01.655768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_status.pyi
--rw-r--r--   0        0        0      921 2023-06-02 06:22:01.391764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_controller_revision.pyi
--rw-r--r--   0        0        0      843 2023-06-02 06:22:01.399764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_controller_revision_list.pyi
--rw-r--r--   0        0        0      484 2023-06-02 06:22:01.455765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cross_version_object_reference.pyi
--rw-r--r--   0        0        0     1540 2023-06-02 06:22:01.743769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_csi_persistent_volume_source.pyi
--rw-r--r--   0        0        0      290 2023-06-02 06:22:01.439765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_endpoint.pyi
--rw-r--r--   0        0        0     1033 2023-06-02 06:22:01.591767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set.pyi
--rw-r--r--   0        0        0      738 2023-06-02 06:22:01.407764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_condition.pyi
--rw-r--r--   0        0        0      789 2023-06-02 06:22:01.543766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_list.pyi
--rw-r--r--   0        0        0     1077 2023-06-02 06:22:01.563767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_spec.pyi
--rw-r--r--   0        0        0     1524 2023-06-02 06:22:01.595767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_status.pyi
--rw-r--r--   0        0        0      620 2023-06-02 06:22:01.375764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_update_strategy.pyi
--rw-r--r--   0        0        0     1215 2023-06-02 06:22:01.611767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_delete_options.pyi
--rw-r--r--   0        0        0     1042 2023-06-02 06:22:01.539766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment.pyi
--rw-r--r--   0        0        0      913 2023-06-02 06:22:01.727769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_condition.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.395764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_list.pyi
--rw-r--r--   0        0        0     1415 2023-06-02 06:22:01.571767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_spec.pyi
--rw-r--r--   0        0        0     1413 2023-06-02 06:22:01.639768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_status.pyi
--rw-r--r--   0        0        0      608 2023-06-02 06:22:01.427764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_strategy.pyi
--rw-r--r--   0        0        0      507 2023-06-02 06:22:01.615767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_downward_api_projection.pyi
--rw-r--r--   0        0        0      883 2023-06-02 06:22:01.555766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_downward_api_volume_file.pyi
--rw-r--r--   0        0        0      632 2023-06-02 06:22:01.403764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_downward_api_volume_source.pyi
--rw-r--r--   0        0        0      484 2023-06-02 06:22:01.347763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_empty_dir_volume_source.pyi
--rw-r--r--   0        0        0      718 2023-06-02 06:22:01.323763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoint_address.pyi
--rw-r--r--   0        0        0      488 2023-06-02 06:22:01.591767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoint_port.pyi
--rw-r--r--   0        0        0      945 2023-06-02 06:22:01.579767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoint_subset.pyi
--rw-r--r--   0        0        0      861 2023-06-02 06:22:01.383764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoints.pyi
--rw-r--r--   0        0        0      789 2023-06-02 06:22:01.455765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoints_list.pyi
--rw-r--r--   0        0        0      796 2023-06-02 06:22:01.611767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_env_from_source.pyi
--rw-r--r--   0        0        0      569 2023-06-02 06:22:01.451765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_env_var.pyi
--rw-r--r--   0        0        0     1201 2023-06-02 06:22:01.451765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_env_var_source.pyi
--rw-r--r--   0        0        0     2601 2023-06-02 06:22:01.367763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_event.pyi
--rw-r--r--   0        0        0      765 2023-06-02 06:22:01.319763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_event_list.pyi
--rw-r--r--   0        0        0      618 2023-06-02 06:22:01.599767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_event_series.pyi
--rw-r--r--   0        0        0      449 2023-06-02 06:22:01.723769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_event_source.pyi
--rw-r--r--   0        0        0      362 2023-06-02 06:22:01.615767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_exec_action.pyi
--rw-r--r--   0        0        0      814 2023-06-02 06:22:01.367763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_fc_volume_source.pyi
--rw-r--r--   0        0        0      900 2023-06-02 06:22:01.471765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_flex_persistent_volume_source.pyi
--rw-r--r--   0        0        0      885 2023-06-02 06:22:01.311762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_flex_volume_source.pyi
--rw-r--r--   0        0        0      504 2023-06-02 06:22:01.459765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_flocker_volume_source.pyi
--rw-r--r--   0        0        0      671 2023-06-02 06:22:01.363763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_gce_persistent_disk_volume_source.pyi
--rw-r--r--   0        0        0      542 2023-06-02 06:22:01.331763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_git_repo_volume_source.pyi
--rw-r--r--   0        0        0      648 2023-06-02 06:22:01.539766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_glusterfs_persistent_volume_source.pyi
--rw-r--r--   0        0        0      478 2023-06-02 06:22:01.411764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_glusterfs_volume_source.pyi
--rw-r--r--   0        0        0      394 2023-06-02 06:22:01.611767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_group_version_for_discovery.pyi
--rw-r--r--   0        0        0      828 2023-06-02 06:22:01.315763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_handler.pyi
--rw-r--r--   0        0        0     1159 2023-06-02 06:22:01.439765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler.pyi
--rw-r--r--   0        0        0      873 2023-06-02 06:22:01.467765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_list.pyi
--rw-r--r--   0        0        0      860 2023-06-02 06:22:01.367763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_spec.pyi
--rw-r--r--   0        0        0      936 2023-06-02 06:22:01.423764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_status.pyi
--rw-r--r--   0        0        0      455 2023-06-02 06:22:01.387764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_host_alias.pyi
--rw-r--r--   0        0        0      404 2023-06-02 06:22:01.511766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_host_path_volume_source.pyi
--rw-r--r--   0        0        0      824 2023-06-02 06:22:01.555766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_http_get_action.pyi
--rw-r--r--   0        0        0      320 2023-06-02 06:22:01.511766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_http_header.pyi
--rw-r--r--   0        0        0      281 2023-06-02 06:22:01.659768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_initializer.pyi
--rw-r--r--   0        0        0      574 2023-06-02 06:22:01.315763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_initializers.pyi
--rw-r--r--   0        0        0      392 2023-06-02 06:22:01.627767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_ip_block.pyi
--rw-r--r--   0        0        0     1511 2023-06-02 06:22:01.395764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_iscsi_persistent_volume_source.pyi
--rw-r--r--   0        0        0     1496 2023-06-02 06:22:01.451765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_iscsi_volume_source.pyi
--rw-r--r--   0        0        0      979 2023-06-02 06:22:01.727769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job.pyi
--rw-r--r--   0        0        0      889 2023-06-02 06:22:01.351763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_condition.pyi
--rw-r--r--   0        0        0      753 2023-06-02 06:22:01.603767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_list.pyi
--rw-r--r--   0        0        0     1380 2023-06-02 06:22:01.547766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_spec.pyi
--rw-r--r--   0        0        0     1099 2023-06-02 06:22:01.399764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_status.pyi
--rw-r--r--   0        0        0      407 2023-06-02 06:22:01.419764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_key_to_path.pyi
--rw-r--r--   0        0        0      679 2023-06-02 06:22:01.659768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_label_selector.pyi
--rw-r--r--   0        0        0      488 2023-06-02 06:22:01.475765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_label_selector_requirement.pyi
--rw-r--r--   0        0        0      608 2023-06-02 06:22:01.651768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_lifecycle.pyi
--rw-r--r--   0        0        0      837 2023-06-02 06:22:01.731769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_limit_range.pyi
--rw-r--r--   0        0        0     1081 2023-06-02 06:22:01.339763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_limit_range_item.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.547766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_limit_range_list.pyi
--rw-r--r--   0        0        0      411 2023-06-02 06:22:01.359763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_limit_range_spec.pyi
--rw-r--r--   0        0        0      585 2023-06-02 06:22:01.507766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_list_meta.pyi
--rw-r--r--   0        0        0      464 2023-06-02 06:22:01.551766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_load_balancer_ingress.pyi
--rw-r--r--   0        0        0      498 2023-06-02 06:22:01.379763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_load_balancer_status.pyi
--rw-r--r--   0        0        0      365 2023-06-02 06:22:01.351763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_local_object_reference.pyi
--rw-r--r--   0        0        0     1081 2023-06-02 06:22:01.355763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_local_subject_access_review.pyi
--rw-r--r--   0        0        0      403 2023-06-02 06:22:01.415764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_local_volume_source.pyi
--rw-r--r--   0        0        0     1033 2023-06-02 06:22:01.355763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_namespace.pyi
--rw-r--r--   0        0        0      789 2023-06-02 06:22:01.423764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_namespace_list.pyi
--rw-r--r--   0        0        0      380 2023-06-02 06:22:01.343763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_namespace_spec.pyi
--rw-r--r--   0        0        0      353 2023-06-02 06:22:01.411764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_namespace_status.pyi
--rw-r--r--   0        0        0      855 2023-06-02 06:22:01.495766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy.pyi
--rw-r--r--   0        0        0      715 2023-06-02 06:22:01.739769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_egress_rule.pyi
--rw-r--r--   0        0        0      727 2023-06-02 06:22:01.467765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_ingress_rule.pyi
--rw-r--r--   0        0        0      813 2023-06-02 06:22:01.475765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_list.pyi
--rw-r--r--   0        0        0      887 2023-06-02 06:22:01.363763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_peer.pyi
--rw-r--r--   0        0        0      485 2023-06-02 06:22:01.371763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_port.pyi
--rw-r--r--   0        0        0     1047 2023-06-02 06:22:01.411764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_spec.pyi
--rw-r--r--   0        0        0      451 2023-06-02 06:22:01.647768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_nfs_volume_source.pyi
--rw-r--r--   0        0        0      988 2023-06-02 06:22:01.451765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node.pyi
--rw-r--r--   0        0        0      329 2023-06-02 06:22:01.507766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_address.pyi
--rw-r--r--   0        0        0      945 2023-06-02 06:22:01.555766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_affinity.pyi
--rw-r--r--   0        0        0      904 2023-06-02 06:22:01.427764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_condition.pyi
--rw-r--r--   0        0        0      500 2023-06-02 06:22:01.447765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_config_source.pyi
--rw-r--r--   0        0        0     1002 2023-06-02 06:22:01.603767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_config_status.pyi
--rw-r--r--   0        0        0      494 2023-06-02 06:22:01.463765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_daemon_endpoints.pyi
--rw-r--r--   0        0        0      759 2023-06-02 06:22:01.423764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_list.pyi
--rw-r--r--   0        0        0      448 2023-06-02 06:22:01.495766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_selector.pyi
--rw-r--r--   0        0        0      485 2023-06-02 06:22:01.543766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_selector_requirement.pyi
--rw-r--r--   0        0        0      794 2023-06-02 06:22:01.735769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_selector_term.pyi
--rw-r--r--   0        0        0     1113 2023-06-02 06:22:01.631768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_spec.pyi
--rw-r--r--   0        0        0     2332 2023-06-02 06:22:01.507766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_status.pyi
--rw-r--r--   0        0        0      918 2023-06-02 06:22:01.491765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_system_info.pyi
--rw-r--r--   0        0        0      464 2023-06-02 06:22:01.323763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_non_resource_attributes.pyi
--rw-r--r--   0        0        0      467 2023-06-02 06:22:01.431764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_non_resource_rule.pyi
--rw-r--r--   0        0        0      438 2023-06-02 06:22:01.623767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_object_field_selector.pyi
--rw-r--r--   0        0        0     2535 2023-06-02 06:22:01.423764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_object_meta.pyi
--rw-r--r--   0        0        0     1010 2023-06-02 06:22:01.327763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_object_reference.pyi
--rw-r--r--   0        0        0      686 2023-06-02 06:22:01.523766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_owner_reference.pyi
--rw-r--r--   0        0        0     1096 2023-06-02 06:22:01.607767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume.pyi
--rw-r--r--   0        0        0     1141 2023-06-02 06:22:01.327763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim.pyi
--rw-r--r--   0        0        0      943 2023-06-02 06:22:01.735769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_condition.pyi
--rw-r--r--   0        0        0      861 2023-06-02 06:22:01.519766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_list.pyi
--rw-r--r--   0        0        0     1463 2023-06-02 06:22:01.639768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_spec.pyi
--rw-r--r--   0        0        0      944 2023-06-02 06:22:01.543766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_status.pyi
--rw-r--r--   0        0        0      477 2023-06-02 06:22:01.731769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_volume_source.pyi
--rw-r--r--   0        0        0      831 2023-06-02 06:22:01.471765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_list.pyi
--rw-r--r--   0        0        0     6866 2023-06-02 06:22:01.391764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_spec.pyi
--rw-r--r--   0        0        0      581 2023-06-02 06:22:01.315763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_status.pyi
--rw-r--r--   0        0        0      450 2023-06-02 06:22:01.435764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_photon_persistent_disk_volume_source.pyi
--rw-r--r--   0        0        0      979 2023-06-02 06:22:01.311762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod.pyi
--rw-r--r--   0        0        0      969 2023-06-02 06:22:01.467765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_affinity.pyi
--rw-r--r--   0        0        0      667 2023-06-02 06:22:01.567767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_affinity_term.pyi
--rw-r--r--   0        0        0      981 2023-06-02 06:22:01.535766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_anti_affinity.pyi
--rw-r--r--   0        0        0      889 2023-06-02 06:22:01.331763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_condition.pyi
--rw-r--r--   0        0        0      738 2023-06-02 06:22:01.639768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_dns_config.pyi
--rw-r--r--   0        0        0      458 2023-06-02 06:22:01.359763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_dns_config_option.pyi
--rw-r--r--   0        0        0      753 2023-06-02 06:22:01.415764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_list.pyi
--rw-r--r--   0        0        0      325 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_readiness_gate.pyi
--rw-r--r--   0        0        0     1313 2023-06-02 06:22:01.607767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_security_context.pyi
--rw-r--r--   0        0        0     5045 2023-06-02 06:22:01.447765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_spec.pyi
--rw-r--r--   0        0        0     1898 2023-06-02 06:22:01.459765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_status.pyi
--rw-r--r--   0        0        0      855 2023-06-02 06:22:01.531766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_template.pyi
--rw-r--r--   0        0        0      801 2023-06-02 06:22:01.463765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_template_list.pyi
--rw-r--r--   0        0        0      619 2023-06-02 06:22:01.559766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_template_spec.pyi
--rw-r--r--   0        0        0      855 2023-06-02 06:22:01.523766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_policy_rule.pyi
--rw-r--r--   0        0        0      539 2023-06-02 06:22:01.739769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_portworx_volume_source.pyi
--rw-r--r--   0        0        0      341 2023-06-02 06:22:01.339763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_preconditions.pyi
--rw-r--r--   0        0        0      483 2023-06-02 06:22:01.415764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_preferred_scheduling_term.pyi
--rw-r--r--   0        0        0     1488 2023-06-02 06:22:01.487765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_probe.pyi
--rw-r--r--   0        0        0      560 2023-06-02 06:22:01.379763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_projected_volume_source.pyi
--rw-r--r--   0        0        0      670 2023-06-02 06:22:01.547766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_quobyte_volume_source.pyi
--rw-r--r--   0        0        0     1122 2023-06-02 06:22:01.427764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rbd_persistent_volume_source.pyi
--rw-r--r--   0        0        0     1107 2023-06-02 06:22:01.579767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rbd_volume_source.pyi
--rw-r--r--   0        0        0     1042 2023-06-02 06:22:01.479765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set.pyi
--rw-r--r--   0        0        0      741 2023-06-02 06:22:01.359763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_condition.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.399764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_list.pyi
--rw-r--r--   0        0        0      845 2023-06-02 06:22:01.575767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_spec.pyi
--rw-r--r--   0        0        0     1102 2023-06-02 06:22:01.455765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_status.pyi
--rw-r--r--   0        0        0     1141 2023-06-02 06:22:01.435764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller.pyi
--rw-r--r--   0        0        0      774 2023-06-02 06:22:01.371763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_condition.pyi
--rw-r--r--   0        0        0      861 2023-06-02 06:22:01.495766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_list.pyi
--rw-r--r--   0        0        0      874 2023-06-02 06:22:01.599767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_spec.pyi
--rw-r--r--   0        0        0     1168 2023-06-02 06:22:01.351763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_status.pyi
--rw-r--r--   0        0        0      995 2023-06-02 06:22:01.431764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_attributes.pyi
--rw-r--r--   0        0        0      553 2023-06-02 06:22:01.635768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_field_selector.pyi
--rw-r--r--   0        0        0     1069 2023-06-02 06:22:01.455765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota.pyi
--rw-r--r--   0        0        0      813 2023-06-02 06:22:01.719769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota_list.pyi
--rw-r--r--   0        0        0      728 2023-06-02 06:22:01.311762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota_spec.pyi
--rw-r--r--   0        0        0      524 2023-06-02 06:22:01.323763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota_status.pyi
--rw-r--r--   0        0        0      545 2023-06-02 06:22:01.615767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_requirements.pyi
--rw-r--r--   0        0        0      708 2023-06-02 06:22:01.415764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_rule.pyi
--rw-r--r--   0        0        0      771 2023-06-02 06:22:01.479765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role.pyi
--rw-r--r--   0        0        0      975 2023-06-02 06:22:01.399764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role_binding.pyi
--rw-r--r--   0        0        0      801 2023-06-02 06:22:01.471765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role_binding_list.pyi
--rw-r--r--   0        0        0      759 2023-06-02 06:22:01.623767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role_list.pyi
--rw-r--r--   0        0        0      361 2023-06-02 06:22:01.479765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role_ref.pyi
--rw-r--r--   0        0        0      424 2023-06-02 06:22:01.395764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rolling_update_daemon_set.pyi
--rw-r--r--   0        0        0      558 2023-06-02 06:22:01.383764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rolling_update_deployment.pyi
--rw-r--r--   0        0        0      416 2023-06-02 06:22:01.739769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rolling_update_stateful_set_strategy.pyi
--rw-r--r--   0        0        0      997 2023-06-02 06:22:01.559766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale.pyi
--rw-r--r--   0        0        0     1369 2023-06-02 06:22:01.735769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale_io_persistent_volume_source.pyi
--rw-r--r--   0        0        0     1354 2023-06-02 06:22:01.563767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale_io_volume_source.pyi
--rw-r--r--   0        0        0      344 2023-06-02 06:22:01.451765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale_spec.pyi
--rw-r--r--   0        0        0      401 2023-06-02 06:22:01.323763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale_status.pyi
--rw-r--r--   0        0        0      554 2023-06-02 06:22:01.567767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scope_selector.pyi
--rw-r--r--   0        0        0      535 2023-06-02 06:22:01.491765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scoped_resource_selector_requirement.pyi
--rw-r--r--   0        0        0      638 2023-06-02 06:22:01.663768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_se_linux_options.pyi
--rw-r--r--   0        0        0     1006 2023-06-02 06:22:01.403764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret.pyi
--rw-r--r--   0        0        0      461 2023-06-02 06:22:01.347763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_env_source.pyi
--rw-r--r--   0        0        0      503 2023-06-02 06:22:01.443765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_key_selector.pyi
--rw-r--r--   0        0        0      771 2023-06-02 06:22:01.583767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_list.pyi
--rw-r--r--   0        0        0      663 2023-06-02 06:22:01.583767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_projection.pyi
--rw-r--r--   0        0        0      461 2023-06-02 06:22:01.595767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_reference.pyi
--rw-r--r--   0        0        0      808 2023-06-02 06:22:01.599767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_volume_source.pyi
--rw-r--r--   0        0        0     1606 2023-06-02 06:22:01.435764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_security_context.pyi
--rw-r--r--   0        0        0     1090 2023-06-02 06:22:01.635768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_self_subject_access_review.pyi
--rw-r--r--   0        0        0      808 2023-06-02 06:22:01.363763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_self_subject_access_review_spec.pyi
--rw-r--r--   0        0        0     1081 2023-06-02 06:22:01.511766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_self_subject_rules_review.pyi
--rw-r--r--   0        0        0      398 2023-06-02 06:22:01.507766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_self_subject_rules_review_spec.pyi
--rw-r--r--   0        0        0      411 2023-06-02 06:22:01.559766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_server_address_by_client_cidr.pyi
--rw-r--r--   0        0        0     1015 2023-06-02 06:22:01.595767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service.pyi
--rw-r--r--   0        0        0     1325 2023-06-02 06:22:01.499765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_account.pyi
--rw-r--r--   0        0        0      819 2023-06-02 06:22:01.551766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_account_list.pyi
--rw-r--r--   0        0        0      580 2023-06-02 06:22:01.615767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_account_token_projection.pyi
--rw-r--r--   0        0        0      777 2023-06-02 06:22:01.719769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_list.pyi
--rw-r--r--   0        0        0      732 2023-06-02 06:22:01.415764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_port.pyi
--rw-r--r--   0        0        0      464 2023-06-02 06:22:01.407764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_reference.pyi
--rw-r--r--   0        0        0     2231 2023-06-02 06:22:01.315763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_spec.pyi
--rw-r--r--   0        0        0      479 2023-06-02 06:22:01.531766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_status.pyi
--rw-r--r--   0        0        0      479 2023-06-02 06:22:01.335763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_session_affinity_config.pyi
--rw-r--r--   0        0        0     1051 2023-06-02 06:22:01.647768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set.pyi
--rw-r--r--   0        0        0      744 2023-06-02 06:22:01.443765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_condition.pyi
--rw-r--r--   0        0        0      801 2023-06-02 06:22:01.419764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_list.pyi
--rw-r--r--   0        0        0     1555 2023-06-02 06:22:01.483765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_spec.pyi
--rw-r--r--   0        0        0     1472 2023-06-02 06:22:01.351763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_status.pyi
--rw-r--r--   0        0        0      656 2023-06-02 06:22:01.495766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_update_strategy.pyi
--rw-r--r--   0        0        0     1230 2023-06-02 06:22:01.543766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_status.pyi
--rw-r--r--   0        0        0      548 2023-06-02 06:22:01.379763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_status_cause.pyi
--rw-r--r--   0        0        0      979 2023-06-02 06:22:01.655768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_status_details.pyi
--rw-r--r--   0        0        0     1682 2023-06-02 06:22:01.587767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_class.pyi
--rw-r--r--   0        0        0      807 2023-06-02 06:22:01.607767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_class_list.pyi
--rw-r--r--   0        0        0      979 2023-06-02 06:22:01.399764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_os_persistent_volume_source.pyi
--rw-r--r--   0        0        0      964 2023-06-02 06:22:01.363763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_os_volume_source.pyi
--rw-r--r--   0        0        0      529 2023-06-02 06:22:01.619767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject.pyi
--rw-r--r--   0        0        0     1066 2023-06-02 06:22:01.579767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_access_review.pyi
--rw-r--r--   0        0        0     1255 2023-06-02 06:22:01.591767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_access_review_spec.pyi
--rw-r--r--   0        0        0      673 2023-06-02 06:22:01.579767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_access_review_status.pyi
--rw-r--r--   0        0        0      846 2023-06-02 06:22:01.599767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_rules_review_status.pyi
--rw-r--r--   0        0        0      308 2023-06-02 06:22:01.575767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_sysctl.pyi
--rw-r--r--   0        0        0      559 2023-06-02 06:22:01.419764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_taint.pyi
--rw-r--r--   0        0        0      410 2023-06-02 06:22:01.395764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_tcp_socket_action.pyi
--rw-r--r--   0        0        0      994 2023-06-02 06:22:01.407764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_token_review.pyi
--rw-r--r--   0        0        0      482 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_token_review_spec.pyi
--rw-r--r--   0        0        0      789 2023-06-02 06:22:01.563767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_token_review_status.pyi
--rw-r--r--   0        0        0      778 2023-06-02 06:22:01.647768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_toleration.pyi
--rw-r--r--   0        0        0      404 2023-06-02 06:22:01.611767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_topology_selector_label_requirement.pyi
--rw-r--r--   0        0        0      589 2023-06-02 06:22:01.647768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_topology_selector_term.pyi
--rw-r--r--   0        0        0      472 2023-06-02 06:22:01.403764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_typed_local_object_reference.pyi
--rw-r--r--   0        0        0      704 2023-06-02 06:22:01.723769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_user_info.pyi
--rw-r--r--   0        0        0     6540 2023-06-02 06:22:01.383764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume.pyi
--rw-r--r--   0        0        0     1039 2023-06-02 06:22:01.319763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment.pyi
--rw-r--r--   0        0        0      831 2023-06-02 06:22:01.551766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment_list.pyi
--rw-r--r--   0        0        0      423 2023-06-02 06:22:01.387764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment_source.pyi
--rw-r--r--   0        0        0      539 2023-06-02 06:22:01.319763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment_spec.pyi
--rw-r--r--   0        0        0      916 2023-06-02 06:22:01.355763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment_status.pyi
--rw-r--r--   0        0        0      343 2023-06-02 06:22:01.483765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_device.pyi
--rw-r--r--   0        0        0      485 2023-06-02 06:22:01.627767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_error.pyi
--rw-r--r--   0        0        0      691 2023-06-02 06:22:01.743769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_mount.pyi
--rw-r--r--   0        0        0      462 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_node_affinity.pyi
--rw-r--r--   0        0        0     1211 2023-06-02 06:22:01.495766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_projection.pyi
--rw-r--r--   0        0        0      734 2023-06-02 06:22:01.571767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_vsphere_virtual_disk_volume_source.pyi
--rw-r--r--   0        0        0      429 2023-06-02 06:22:01.615767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_watch_event.pyi
--rw-r--r--   0        0        0      499 2023-06-02 06:22:01.555766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_weighted_pod_affinity_term.pyi
--rw-r--r--   0        0        0      532 2023-06-02 06:22:01.619767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_aggregation_rule.pyi
--rw-r--r--   0        0        0      867 2023-06-02 06:22:01.307762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_audit_sink.pyi
--rw-r--r--   0        0        0      825 2023-06-02 06:22:01.543766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_audit_sink_list.pyi
--rw-r--r--   0        0        0      544 2023-06-02 06:22:01.575767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_audit_sink_spec.pyi
--rw-r--r--   0        0        0     1077 2023-06-02 06:22:01.603767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role.pyi
--rw-r--r--   0        0        0     1050 2023-06-02 06:22:01.443765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding.pyi
--rw-r--r--   0        0        0      879 2023-06-02 06:22:01.359763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding_list.pyi
--rw-r--r--   0        0        0      837 2023-06-02 06:22:01.379763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role_list.pyi
--rw-r--r--   0        0        0      501 2023-06-02 06:22:01.535766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_initializer.pyi
--rw-r--r--   0        0        0      948 2023-06-02 06:22:01.319763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_initializer_configuration.pyi
--rw-r--r--   0        0        0      915 2023-06-02 06:22:01.591767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_initializer_configuration_list.pyi
--rw-r--r--   0        0        0      867 2023-06-02 06:22:01.491765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_pod_preset.pyi
--rw-r--r--   0        0        0      825 2023-06-02 06:22:01.375764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_pod_preset_list.pyi
--rw-r--r--   0        0        0     1295 2023-06-02 06:22:01.387764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_pod_preset_spec.pyi
--rw-r--r--   0        0        0      407 2023-06-02 06:22:01.555766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_policy.pyi
--rw-r--r--   0        0        0      873 2023-06-02 06:22:01.511766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_policy_rule.pyi
--rw-r--r--   0        0        0      958 2023-06-02 06:22:01.431764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_priority_class.pyi
--rw-r--r--   0        0        0      849 2023-06-02 06:22:01.623767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_priority_class_list.pyi
--rw-r--r--   0        0        0      807 2023-06-02 06:22:01.635768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role.pyi
--rw-r--r--   0        0        0     1029 2023-06-02 06:22:01.375764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role_binding.pyi
--rw-r--r--   0        0        0      837 2023-06-02 06:22:01.439765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role_binding_list.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.439765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role_list.pyi
--rw-r--r--   0        0        0      379 2023-06-02 06:22:01.423764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role_ref.pyi
--rw-r--r--   0        0        0      636 2023-06-02 06:22:01.375764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_rule.pyi
--rw-r--r--   0        0        0      464 2023-06-02 06:22:01.655768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_service_reference.pyi
--rw-r--r--   0        0        0      553 2023-06-02 06:22:01.539766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_subject.pyi
--rw-r--r--   0        0        0     1093 2023-06-02 06:22:01.503766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment.pyi
--rw-r--r--   0        0        0      867 2023-06-02 06:22:01.499765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment_list.pyi
--rw-r--r--   0        0        0      441 2023-06-02 06:22:01.311762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment_source.pyi
--rw-r--r--   0        0        0      575 2023-06-02 06:22:01.331763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment_spec.pyi
--rw-r--r--   0        0        0      970 2023-06-02 06:22:01.339763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment_status.pyi
--rw-r--r--   0        0        0      503 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_error.pyi
--rw-r--r--   0        0        0      687 2023-06-02 06:22:01.607767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_webhook.pyi
--rw-r--r--   0        0        0      713 2023-06-02 06:22:01.639768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_webhook_client_config.pyi
--rw-r--r--   0        0        0      482 2023-06-02 06:22:01.723769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_webhook_throttle_config.pyi
--rw-r--r--   0        0        0      529 2023-06-02 06:22:01.623767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_aggregation_rule.pyi
--rw-r--r--   0        0        0     1087 2023-06-02 06:22:01.379763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service.pyi
--rw-r--r--   0        0        0      756 2023-06-02 06:22:01.735769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_condition.pyi
--rw-r--r--   0        0        0      825 2023-06-02 06:22:01.651768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_list.pyi
--rw-r--r--   0        0        0     1112 2023-06-02 06:22:01.519766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_spec.pyi
--rw-r--r--   0        0        0      531 2023-06-02 06:22:01.439765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_status.pyi
--rw-r--r--   0        0        0     1222 2023-06-02 06:22:01.743769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request.pyi
--rw-r--r--   0        0        0      744 2023-06-02 06:22:01.727769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_condition.pyi
--rw-r--r--   0        0        0      915 2023-06-02 06:22:01.435764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_list.pyi
--rw-r--r--   0        0        0      950 2023-06-02 06:22:01.587767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_spec.pyi
--rw-r--r--   0        0        0      738 2023-06-02 06:22:01.459765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_status.pyi
--rw-r--r--   0        0        0     1068 2023-06-02 06:22:01.419764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role.pyi
--rw-r--r--   0        0        0     1041 2023-06-02 06:22:01.611767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role_binding.pyi
--rw-r--r--   0        0        0      873 2023-06-02 06:22:01.635768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role_binding_list.pyi
--rw-r--r--   0        0        0      831 2023-06-02 06:22:01.431764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role_list.pyi
--rw-r--r--   0        0        0      936 2023-06-02 06:22:01.499765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_controller_revision.pyi
--rw-r--r--   0        0        0      873 2023-06-02 06:22:01.571767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_controller_revision_list.pyi
--rw-r--r--   0        0        0     1060 2023-06-02 06:22:01.347763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job.pyi
--rw-r--r--   0        0        0      807 2023-06-02 06:22:01.367763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job_list.pyi
--rw-r--r--   0        0        0     1211 2023-06-02 06:22:01.567767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job_spec.pyi
--rw-r--r--   0        0        0      661 2023-06-02 06:22:01.363763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job_status.pyi
--rw-r--r--   0        0        0      772 2023-06-02 06:22:01.347763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_column_definition.pyi
--rw-r--r--   0        0        0      658 2023-06-02 06:22:01.523766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_conversion.pyi
--rw-r--r--   0        0        0     1156 2023-06-02 06:22:01.535766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition.pyi
--rw-r--r--   0        0        0      798 2023-06-02 06:22:01.631768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_condition.pyi
--rw-r--r--   0        0        0      909 2023-06-02 06:22:01.367763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_list.pyi
--rw-r--r--   0        0        0      879 2023-06-02 06:22:01.579767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_names.pyi
--rw-r--r--   0        0        0     2103 2023-06-02 06:22:01.659768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_spec.pyi
--rw-r--r--   0        0        0      872 2023-06-02 06:22:01.391764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_status.pyi
--rw-r--r--   0        0        0     1305 2023-06-02 06:22:01.619767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_version.pyi
--rw-r--r--   0        0        0      617 2023-06-02 06:22:01.447765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_subresource_scale.pyi
--rw-r--r--   0        0        0      684 2023-06-02 06:22:01.515766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_subresources.pyi
--rw-r--r--   0        0        0      544 2023-06-02 06:22:01.731769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_validation.pyi
--rw-r--r--   0        0        0     1078 2023-06-02 06:22:01.631768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set.pyi
--rw-r--r--   0        0        0      753 2023-06-02 06:22:01.487765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_condition.pyi
--rw-r--r--   0        0        0      819 2023-06-02 06:22:01.567767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_list.pyi
--rw-r--r--   0        0        0     1304 2023-06-02 06:22:01.571767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_spec.pyi
--rw-r--r--   0        0        0     1554 2023-06-02 06:22:01.523766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_status.pyi
--rw-r--r--   0        0        0      650 2023-06-02 06:22:01.351763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_update_strategy.pyi
--rw-r--r--   0        0        0     2793 2023-06-02 06:22:01.535766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_event.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.379763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_event_list.pyi
--rw-r--r--   0        0        0      462 2023-06-02 06:22:01.591767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_event_series.pyi
--rw-r--r--   0        0        0      872 2023-06-02 06:22:01.407764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_eviction.pyi
--rw-r--r--   0        0        0      497 2023-06-02 06:22:01.343763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_external_documentation.pyi
--rw-r--r--   0        0        0      525 2023-06-02 06:22:01.587767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_http_ingress_path.pyi
--rw-r--r--   0        0        0      459 2023-06-02 06:22:01.355763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_http_ingress_rule_value.pyi
--rw-r--r--   0        0        0     1060 2023-06-02 06:22:01.727769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress.pyi
--rw-r--r--   0        0        0      411 2023-06-02 06:22:01.643768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_backend.pyi
--rw-r--r--   0        0        0      807 2023-06-02 06:22:01.719769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_list.pyi
--rw-r--r--   0        0        0      579 2023-06-02 06:22:01.631768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_rule.pyi
--rw-r--r--   0        0        0      905 2023-06-02 06:22:01.539766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_spec.pyi
--rw-r--r--   0        0        0      494 2023-06-02 06:22:01.483765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_status.pyi
--rw-r--r--   0        0        0      487 2023-06-02 06:22:01.571767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_tls.pyi
--rw-r--r--   0        0        0      407 2023-06-02 06:22:01.627767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ip_block.pyi
--rw-r--r--   0        0        0      634 2023-06-02 06:22:01.463765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_job_template_spec.pyi
--rw-r--r--   0        0        0     5615 2023-06-02 06:22:01.427764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_json_schema_props.pyi
--rw-r--r--   0        0        0      837 2023-06-02 06:22:01.651768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_lease.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.595767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_lease_list.pyi
--rw-r--r--   0        0        0      977 2023-06-02 06:22:01.603767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_lease_spec.pyi
--rw-r--r--   0        0        0     1126 2023-06-02 06:22:01.467765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_local_subject_access_review.pyi
--rw-r--r--   0        0        0      930 2023-06-02 06:22:01.411764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration.pyi
--rw-r--r--   0        0        0      933 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration_list.pyi
--rw-r--r--   0        0        0      885 2023-06-02 06:22:01.463765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy.pyi
--rw-r--r--   0        0        0      760 2023-06-02 06:22:01.395764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_egress_rule.pyi
--rw-r--r--   0        0        0      772 2023-06-02 06:22:01.563767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_ingress_rule.pyi
--rw-r--r--   0        0        0      843 2023-06-02 06:22:01.539766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_list.pyi
--rw-r--r--   0        0        0      917 2023-06-02 06:22:01.535766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_peer.pyi
--rw-r--r--   0        0        0      500 2023-06-02 06:22:01.471765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_port.pyi
--rw-r--r--   0        0        0     1092 2023-06-02 06:22:01.531766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_spec.pyi
--rw-r--r--   0        0        0      479 2023-06-02 06:22:01.467765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_non_resource_attributes.pyi
--rw-r--r--   0        0        0      482 2023-06-02 06:22:01.503766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_non_resource_rule.pyi
--rw-r--r--   0        0        0     1168 2023-06-02 06:22:01.327763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget.pyi
--rw-r--r--   0        0        0      879 2023-06-02 06:22:01.447765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_list.pyi
--rw-r--r--   0        0        0      787 2023-06-02 06:22:01.359763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_spec.pyi
--rw-r--r--   0        0        0      929 2023-06-02 06:22:01.567767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_status.pyi
--rw-r--r--   0        0        0      870 2023-06-02 06:22:01.651768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_policy_rule.pyi
--rw-r--r--   0        0        0      955 2023-06-02 06:22:01.731769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_priority_class.pyi
--rw-r--r--   0        0        0      843 2023-06-02 06:22:01.559766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_priority_class_list.pyi
--rw-r--r--   0        0        0     1087 2023-06-02 06:22:01.479765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set.pyi
--rw-r--r--   0        0        0      756 2023-06-02 06:22:01.503766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_condition.pyi
--rw-r--r--   0        0        0      825 2023-06-02 06:22:01.327763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_list.pyi
--rw-r--r--   0        0        0      917 2023-06-02 06:22:01.659768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_spec.pyi
--rw-r--r--   0        0        0     1132 2023-06-02 06:22:01.599767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_status.pyi
--rw-r--r--   0        0        0     1010 2023-06-02 06:22:01.571767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_resource_attributes.pyi
--rw-r--r--   0        0        0      723 2023-06-02 06:22:01.483765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_resource_rule.pyi
--rw-r--r--   0        0        0      801 2023-06-02 06:22:01.479765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role.pyi
--rw-r--r--   0        0        0     1020 2023-06-02 06:22:01.723769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role_binding.pyi
--rw-r--r--   0        0        0      831 2023-06-02 06:22:01.595767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role_binding_list.pyi
--rw-r--r--   0        0        0      789 2023-06-02 06:22:01.587767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role_list.pyi
--rw-r--r--   0        0        0      376 2023-06-02 06:22:01.731769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role_ref.pyi
--rw-r--r--   0        0        0      439 2023-06-02 06:22:01.475765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_rolling_update_daemon_set.pyi
--rw-r--r--   0        0        0      431 2023-06-02 06:22:01.447765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_rolling_update_stateful_set_strategy.pyi
--rw-r--r--   0        0        0      807 2023-06-02 06:22:01.643768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_rule_with_operations.pyi
--rw-r--r--   0        0        0     1135 2023-06-02 06:22:01.611767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_self_subject_access_review.pyi
--rw-r--r--   0        0        0      853 2023-06-02 06:22:01.655768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_self_subject_access_review_spec.pyi
--rw-r--r--   0        0        0     1126 2023-06-02 06:22:01.339763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_self_subject_rules_review.pyi
--rw-r--r--   0        0        0      413 2023-06-02 06:22:01.575767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_self_subject_rules_review_spec.pyi
--rw-r--r--   0        0        0     1096 2023-06-02 06:22:01.463765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set.pyi
--rw-r--r--   0        0        0      759 2023-06-02 06:22:01.591767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_condition.pyi
--rw-r--r--   0        0        0      831 2023-06-02 06:22:01.643768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_list.pyi
--rw-r--r--   0        0        0     1642 2023-06-02 06:22:01.587767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_spec.pyi
--rw-r--r--   0        0        0     1502 2023-06-02 06:22:01.659768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_status.pyi
--rw-r--r--   0        0        0      686 2023-06-02 06:22:01.535766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_update_strategy.pyi
--rw-r--r--   0        0        0     1697 2023-06-02 06:22:01.499765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_storage_class.pyi
--rw-r--r--   0        0        0      837 2023-06-02 06:22:01.427764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_storage_class_list.pyi
--rw-r--r--   0        0        0      544 2023-06-02 06:22:01.639768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject.pyi
--rw-r--r--   0        0        0     1111 2023-06-02 06:22:01.459765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_access_review.pyi
--rw-r--r--   0        0        0     1297 2023-06-02 06:22:01.595767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_access_review_spec.pyi
--rw-r--r--   0        0        0      688 2023-06-02 06:22:01.419764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_access_review_status.pyi
--rw-r--r--   0        0        0      891 2023-06-02 06:22:01.623767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_rules_review_status.pyi
--rw-r--r--   0        0        0     1039 2023-06-02 06:22:01.383764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_token_review.pyi
--rw-r--r--   0        0        0      497 2023-06-02 06:22:01.459765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_token_review_spec.pyi
--rw-r--r--   0        0        0      819 2023-06-02 06:22:01.631768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_token_review_status.pyi
--rw-r--r--   0        0        0      719 2023-06-02 06:22:01.387764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_user_info.pyi
--rw-r--r--   0        0        0      936 2023-06-02 06:22:01.491765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration.pyi
--rw-r--r--   0        0        0      945 2023-06-02 06:22:01.447765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration_list.pyi
--rw-r--r--   0        0        0     1084 2023-06-02 06:22:01.375764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment.pyi
--rw-r--r--   0        0        0      861 2023-06-02 06:22:01.603767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment_list.pyi
--rw-r--r--   0        0        0      438 2023-06-02 06:22:01.363763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment_source.pyi
--rw-r--r--   0        0        0      569 2023-06-02 06:22:01.307762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment_spec.pyi
--rw-r--r--   0        0        0      961 2023-06-02 06:22:01.587767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment_status.pyi
--rw-r--r--   0        0        0      500 2023-06-02 06:22:01.547766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_error.pyi
--rw-r--r--   0        0        0     1255 2023-06-02 06:22:01.335763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_webhook.pyi
--rw-r--r--   0        0        0      936 2023-06-02 06:22:01.547766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_controller_revision.pyi
--rw-r--r--   0        0        0      873 2023-06-02 06:22:01.311762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_controller_revision_list.pyi
--rw-r--r--   0        0        0     1078 2023-06-02 06:22:01.643768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set.pyi
--rw-r--r--   0        0        0      753 2023-06-02 06:22:01.463765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_condition.pyi
--rw-r--r--   0        0        0      819 2023-06-02 06:22:01.335763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_list.pyi
--rw-r--r--   0        0        0     1107 2023-06-02 06:22:01.459765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_spec.pyi
--rw-r--r--   0        0        0     1554 2023-06-02 06:22:01.335763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_status.pyi
--rw-r--r--   0        0        0      650 2023-06-02 06:22:01.739769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_update_strategy.pyi
--rw-r--r--   0        0        0     1087 2023-06-02 06:22:01.719769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment.pyi
--rw-r--r--   0        0        0      928 2023-06-02 06:22:01.471765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_condition.pyi
--rw-r--r--   0        0        0      825 2023-06-02 06:22:01.499765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_list.pyi
--rw-r--r--   0        0        0     1445 2023-06-02 06:22:01.551766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_spec.pyi
--rw-r--r--   0        0        0     1443 2023-06-02 06:22:01.719769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_status.pyi
--rw-r--r--   0        0        0      638 2023-06-02 06:22:01.307762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_strategy.pyi
--rw-r--r--   0        0        0     1087 2023-06-02 06:22:01.335763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set.pyi
--rw-r--r--   0        0        0      756 2023-06-02 06:22:01.475765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_condition.pyi
--rw-r--r--   0        0        0      825 2023-06-02 06:22:01.519766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_list.pyi
--rw-r--r--   0        0        0      860 2023-06-02 06:22:01.719769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_spec.pyi
--rw-r--r--   0        0        0     1132 2023-06-02 06:22:01.623767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_status.pyi
--rw-r--r--   0        0        0      439 2023-06-02 06:22:01.487765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_rolling_update_daemon_set.pyi
--rw-r--r--   0        0        0      573 2023-06-02 06:22:01.559766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_rolling_update_deployment.pyi
--rw-r--r--   0        0        0      431 2023-06-02 06:22:01.319763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_rolling_update_stateful_set_strategy.pyi
--rw-r--r--   0        0        0     1042 2023-06-02 06:22:01.315763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_scale.pyi
--rw-r--r--   0        0        0      359 2023-06-02 06:22:01.607767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_scale_spec.pyi
--rw-r--r--   0        0        0      577 2023-06-02 06:22:01.319763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_scale_status.pyi
--rw-r--r--   0        0        0     1096 2023-06-02 06:22:01.395764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set.pyi
--rw-r--r--   0        0        0      759 2023-06-02 06:22:01.455765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_condition.pyi
--rw-r--r--   0        0        0      831 2023-06-02 06:22:01.507766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_list.pyi
--rw-r--r--   0        0        0     1585 2023-06-02 06:22:01.323763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_spec.pyi
--rw-r--r--   0        0        0     1502 2023-06-02 06:22:01.599767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_status.pyi
--rw-r--r--   0        0        0      686 2023-06-02 06:22:01.579767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_update_strategy.pyi
--rw-r--r--   0        0        0     1069 2023-06-02 06:22:01.315763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job.pyi
--rw-r--r--   0        0        0      813 2023-06-02 06:22:01.355763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job_list.pyi
--rw-r--r--   0        0        0     1217 2023-06-02 06:22:01.407764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job_spec.pyi
--rw-r--r--   0        0        0      664 2023-06-02 06:22:01.407764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job_status.pyi
--rw-r--r--   0        0        0      637 2023-06-02 06:22:01.583767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_job_template_spec.pyi
--rw-r--r--   0        0        0      499 2023-06-02 06:22:01.327763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_cross_version_object_reference.pyi
--rw-r--r--   0        0        0      826 2023-06-02 06:22:01.491765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_external_metric_source.pyi
--rw-r--r--   0        0        0      775 2023-06-02 06:22:01.355763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_external_metric_status.pyi
--rw-r--r--   0        0        0     1204 2023-06-02 06:22:01.411764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.519766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_condition.pyi
--rw-r--r--   0        0        0      903 2023-06-02 06:22:01.555766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_list.pyi
--rw-r--r--   0        0        0      933 2023-06-02 06:22:01.331763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_spec.pyi
--rw-r--r--   0        0        0     1261 2023-06-02 06:22:01.639768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_status.pyi
--rw-r--r--   0        0        0     1209 2023-06-02 06:22:01.531766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_metric_spec.pyi
--rw-r--r--   0        0        0     1215 2023-06-02 06:22:01.563767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_metric_status.pyi
--rw-r--r--   0        0        0      919 2023-06-02 06:22:01.619767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_object_metric_source.pyi
--rw-r--r--   0        0        0      922 2023-06-02 06:22:01.443765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_object_metric_status.pyi
--rw-r--r--   0        0        0      618 2023-06-02 06:22:01.627767 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_pods_metric_source.pyi
--rw-r--r--   0        0        0      621 2023-06-02 06:22:01.731769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_pods_metric_status.pyi
--rw-r--r--   0        0        0      625 2023-06-02 06:22:01.515766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_resource_metric_source.pyi
--rw-r--r--   0        0        0      574 2023-06-02 06:22:01.495766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_resource_metric_status.pyi
--rw-r--r--   0        0        0      499 2023-06-02 06:22:01.551766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_cross_version_object_reference.pyi
--rw-r--r--   0        0        0      598 2023-06-02 06:22:01.343763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_external_metric_source.pyi
--rw-r--r--   0        0        0      616 2023-06-02 06:22:01.339763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_external_metric_status.pyi
--rw-r--r--   0        0        0     1204 2023-06-02 06:22:01.503766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler.pyi
--rw-r--r--   0        0        0      795 2023-06-02 06:22:01.739769 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_condition.pyi
--rw-r--r--   0        0        0      903 2023-06-02 06:22:01.647768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_list.pyi
--rw-r--r--   0        0        0      933 2023-06-02 06:22:01.391764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_spec.pyi
--rw-r--r--   0        0        0     1261 2023-06-02 06:22:01.551766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_status.pyi
--rw-r--r--   0        0        0      513 2023-06-02 06:22:01.307762 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_identifier.pyi
--rw-r--r--   0        0        0     1209 2023-06-02 06:22:01.383764 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_spec.pyi
--rw-r--r--   0        0        0     1215 2023-06-02 06:22:01.519766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_status.pyi
--rw-r--r--   0        0        0      660 2023-06-02 06:22:01.507766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_target.pyi
--rw-r--r--   0        0        0      636 2023-06-02 06:22:01.643768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_value_status.pyi
--rw-r--r--   0        0        0      817 2023-06-02 06:22:01.515766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_object_metric_source.pyi
--rw-r--r--   0        0        0      835 2023-06-02 06:22:01.475765 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_object_metric_status.pyi
--rw-r--r--   0        0        0      586 2023-06-02 06:22:01.343763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_pods_metric_source.pyi
--rw-r--r--   0        0        0      604 2023-06-02 06:22:01.635768 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_pods_metric_status.pyi
--rw-r--r--   0        0        0      474 2023-06-02 06:22:01.503766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_resource_metric_source.pyi
--rw-r--r--   0        0        0      492 2023-06-02 06:22:01.527766 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_resource_metric_status.pyi
--rw-r--r--   0        0        0      716 2023-06-02 06:22:01.331763 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/version_info.pyi
--rw-r--r--   0        0        0       74 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/rest.pyi
--rw-r--r--   0        0        0      474 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/config/__init__.pyi
--rw-r--r--   0        0        0       38 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/config/config_exception.pyi
--rw-r--r--   0        0        0      203 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/config/incluster_config.pyi
--rw-r--r--   0        0        0      920 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/config/kube_config.pyi
--rw-r--r--   0        0        0      206 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/stream.pyi
--rw-r--r--   0        0        0   395180 2023-06-02 06:22:01.795770 kubernetes-stubs-elephant-fork-9.0.0/kubernetes_ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:21:43.663532 kubernetes-stubs-elephant-fork-9.0.0/kubernetes_ext/py.typed
--rw-r--r--   0        0        0      760 2023-06-02 06:22:01.887771 kubernetes-stubs-elephant-fork-9.0.0/pyproject.toml
--rw-r--r--   0        0        0     1281 2023-06-02 06:22:03.167053 kubernetes-stubs-elephant-fork-9.0.0/setup.py
--rw-r--r--   0        0        0     1387 2023-06-02 06:22:03.167386 kubernetes-stubs-elephant-fork-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0      517 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 07:15:29.342148 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/__init__.pyi
+-rw-r--r--   0        0        0   146454 2023-06-02 07:15:31.050134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/__init__.pyi
+-rw-r--r--   0        0        0     5701 2023-06-02 07:15:31.534129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/__init__.pyi
+-rw-r--r--   0        0        0      254 2023-06-02 07:15:31.506130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/admissionregistration_api.pyi
+-rw-r--r--   0        0        0     2650 2023-06-02 07:15:31.510130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/admissionregistration_v1alpha1_api.pyi
+-rw-r--r--   0        0        0     5166 2023-06-02 07:15:31.522129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/admissionregistration_v1beta1_api.pyi
+-rw-r--r--   0        0        0      246 2023-06-02 07:15:31.538129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiextensions_api.pyi
+-rw-r--r--   0        0        0     3301 2023-06-02 07:15:31.526129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiextensions_v1beta1_api.pyi
+-rw-r--r--   0        0        0      248 2023-06-02 07:15:31.522129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiregistration_api.pyi
+-rw-r--r--   0        0        0     2939 2023-06-02 07:15:31.502130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiregistration_v1_api.pyi
+-rw-r--r--   0        0        0     2999 2023-06-02 07:15:31.530129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiregistration_v1beta1_api.pyi
+-rw-r--r--   0        0        0      244 2023-06-02 07:15:31.502130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apis_api.pyi
+-rw-r--r--   0        0        0      237 2023-06-02 07:15:31.538129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apps_api.pyi
+-rw-r--r--   0        0        0    18683 2023-06-02 07:15:31.518129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apps_v1_api.pyi
+-rw-r--r--   0        0        0    11841 2023-06-02 07:15:31.510130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apps_v1beta1_api.pyi
+-rw-r--r--   0        0        0    19028 2023-06-02 07:15:31.530129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apps_v1beta2_api.pyi
+-rw-r--r--   0        0        0      250 2023-06-02 07:15:31.526129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/auditregistration_api.pyi
+-rw-r--r--   0        0        0     2436 2023-06-02 07:15:31.526129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/auditregistration_v1alpha1_api.pyi
+-rw-r--r--   0        0        0      247 2023-06-02 07:15:31.526129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authentication_api.pyi
+-rw-r--r--   0        0        0      509 2023-06-02 07:15:31.498130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authentication_v1_api.pyi
+-rw-r--r--   0        0        0      524 2023-06-02 07:15:31.534129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authentication_v1beta1_api.pyi
+-rw-r--r--   0        0        0      246 2023-06-02 07:15:31.518129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authorization_api.pyi
+-rw-r--r--   0        0        0     1421 2023-06-02 07:15:31.538129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authorization_v1_api.pyi
+-rw-r--r--   0        0        0     1466 2023-06-02 07:15:31.526129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authorization_v1beta1_api.pyi
+-rw-r--r--   0        0        0      244 2023-06-02 07:15:31.506130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/autoscaling_api.pyi
+-rw-r--r--   0        0        0     3996 2023-06-02 07:15:31.522129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/autoscaling_v1_api.pyi
+-rw-r--r--   0        0        0     4061 2023-06-02 07:15:31.538129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/autoscaling_v2beta1_api.pyi
+-rw-r--r--   0        0        0     4061 2023-06-02 07:15:31.506130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/autoscaling_v2beta2_api.pyi
+-rw-r--r--   0        0        0      238 2023-06-02 07:15:31.498130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/batch_api.pyi
+-rw-r--r--   0        0        0     3508 2023-06-02 07:15:31.514129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/batch_v1_api.pyi
+-rw-r--r--   0        0        0     3676 2023-06-02 07:15:31.522129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/batch_v1beta1_api.pyi
+-rw-r--r--   0        0        0     3689 2023-06-02 07:15:31.526129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/batch_v2alpha1_api.pyi
+-rw-r--r--   0        0        0      245 2023-06-02 07:15:31.502130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/certificates_api.pyi
+-rw-r--r--   0        0        0     3592 2023-06-02 07:15:31.498130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/certificates_v1beta1_api.pyi
+-rw-r--r--   0        0        0      245 2023-06-02 07:15:31.510130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/coordination_api.pyi
+-rw-r--r--   0        0        0     3024 2023-06-02 07:15:31.542129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/coordination_v1beta1_api.pyi
+-rw-r--r--   0        0        0      243 2023-06-02 07:15:31.518129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/core_api.pyi
+-rw-r--r--   0        0        0    54192 2023-06-02 07:15:31.530129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/core_v1_api.pyi
+-rw-r--r--   0        0        0     4499 2023-06-02 07:15:31.502130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/custom_objects_api.pyi
+-rw-r--r--   0        0        0      239 2023-06-02 07:15:31.514129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/events_api.pyi
+-rw-r--r--   0        0        0     3018 2023-06-02 07:15:31.514129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/events_v1beta1_api.pyi
+-rw-r--r--   0        0        0      243 2023-06-02 07:15:31.502130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/extensions_api.pyi
+-rw-r--r--   0        0        0    21799 2023-06-02 07:15:31.506130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/extensions_v1beta1_api.pyi
+-rw-r--r--   0        0        0      287 2023-06-02 07:15:31.522129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/logs_api.pyi
+-rw-r--r--   0        0        0      243 2023-06-02 07:15:31.498130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/networking_api.pyi
+-rw-r--r--   0        0        0     3113 2023-06-02 07:15:31.506130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/networking_v1_api.pyi
+-rw-r--r--   0        0        0      239 2023-06-02 07:15:31.510130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/policy_api.pyi
+-rw-r--r--   0        0        0     6285 2023-06-02 07:15:31.530129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/policy_v1beta1_api.pyi
+-rw-r--r--   0        0        0      250 2023-06-02 07:15:31.518129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/rbacAuthorization_api.pyi
+-rw-r--r--   0        0        0     9912 2023-06-02 07:15:31.514129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/rbacAuthorization_v1_api.pyi
+-rw-r--r--   0        0        0    10098 2023-06-02 07:15:31.542129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/rbacAuthorization_v1alpha1_api.pyi
+-rw-r--r--   0        0        0    10067 2023-06-02 07:15:31.498130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/rbacAuthorization_v1beta1_api.pyi
+-rw-r--r--   0        0        0      243 2023-06-02 07:15:31.502130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/scheduling_api.pyi
+-rw-r--r--   0        0        0     2485 2023-06-02 07:15:31.518129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/scheduling_v1alpha1_api.pyi
+-rw-r--r--   0        0        0     2477 2023-06-02 07:15:31.522129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/scheduling_v1beta1_api.pyi
+-rw-r--r--   0        0        0      241 2023-06-02 07:15:31.518129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/settings_api.pyi
+-rw-r--r--   0        0        0     3101 2023-06-02 07:15:31.506130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/settings_v1alpha1_api.pyi
+-rw-r--r--   0        0        0      240 2023-06-02 07:15:31.510130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/storage_api.pyi
+-rw-r--r--   0        0        0     5224 2023-06-02 07:15:31.514129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/storage_v1_api.pyi
+-rw-r--r--   0        0        0     2524 2023-06-02 07:15:31.510130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/storage_v1alpha1_api.pyi
+-rw-r--r--   0        0        0     4718 2023-06-02 07:15:31.538129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/storage_v1beta1_api.pyi
+-rw-r--r--   0        0        0      236 2023-06-02 07:15:31.538129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/version_api.pyi
+-rw-r--r--   0        0        0      420 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api_client.pyi
+-rw-r--r--   0        0        0      496 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/configuration.pyi
+-rw-r--r--   0        0        0     1165 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/exceptions.pyi
+-rw-r--r--   0        0        0   140444 2023-06-02 07:15:31.418130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/__init__.pyi
+-rw-r--r--   0        0        0      524 2023-06-02 07:15:31.350131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/admissionregistration_v1beta1_service_reference.pyi
+-rw-r--r--   0        0        0      833 2023-06-02 07:15:31.182133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/admissionregistration_v1beta1_webhook_client_config.pyi
+-rw-r--r--   0        0        0      500 2023-06-02 07:15:31.174132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apiextensions_v1beta1_service_reference.pyi
+-rw-r--r--   0        0        0      785 2023-06-02 07:15:31.246132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apiextensions_v1beta1_webhook_client_config.pyi
+-rw-r--r--   0        0        0      524 2023-06-02 07:15:31.214132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apiregistration_v1beta1_service_reference.pyi
+-rw-r--r--   0        0        0     1123 2023-06-02 07:15:31.458130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment.pyi
+-rw-r--r--   0        0        0      940 2023-06-02 07:15:31.098133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_condition.pyi
+-rw-r--r--   0        0        0      849 2023-06-02 07:15:31.258132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_list.pyi
+-rw-r--r--   0        0        0      897 2023-06-02 07:15:31.126133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_rollback.pyi
+-rw-r--r--   0        0        0     1766 2023-06-02 07:15:31.454130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_spec.pyi
+-rw-r--r--   0        0        0     1467 2023-06-02 07:15:31.490130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_status.pyi
+-rw-r--r--   0        0        0      662 2023-06-02 07:15:31.470130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_strategy.pyi
+-rw-r--r--   0        0        0      386 2023-06-02 07:15:31.074133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_rollback_config.pyi
+-rw-r--r--   0        0        0      585 2023-06-02 07:15:31.170132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_rolling_update_deployment.pyi
+-rw-r--r--   0        0        0     1078 2023-06-02 07:15:31.350131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_scale.pyi
+-rw-r--r--   0        0        0      371 2023-06-02 07:15:31.222132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_scale_spec.pyi
+-rw-r--r--   0        0        0      589 2023-06-02 07:15:31.214132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_scale_status.pyi
+-rw-r--r--   0        0        0      350 2023-06-02 07:15:31.490130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_allowed_flex_volume.pyi
+-rw-r--r--   0        0        0      528 2023-06-02 07:15:31.282132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_allowed_host_path.pyi
+-rw-r--r--   0        0        0     1177 2023-06-02 07:15:31.426130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment.pyi
+-rw-r--r--   0        0        0      958 2023-06-02 07:15:31.310131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_condition.pyi
+-rw-r--r--   0        0        0      885 2023-06-02 07:15:31.078133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_list.pyi
+-rw-r--r--   0        0        0      933 2023-06-02 07:15:31.230132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_rollback.pyi
+-rw-r--r--   0        0        0     1820 2023-06-02 07:15:31.154133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_spec.pyi
+-rw-r--r--   0        0        0     1503 2023-06-02 07:15:31.190132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_status.pyi
+-rw-r--r--   0        0        0      698 2023-06-02 07:15:31.186133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_strategy.pyi
+-rw-r--r--   0        0        0      657 2023-06-02 07:15:31.334131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_fs_group_strategy_options.pyi
+-rw-r--r--   0        0        0      365 2023-06-02 07:15:31.354131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_host_port_range.pyi
+-rw-r--r--   0        0        0      347 2023-06-02 07:15:31.178133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_id_range.pyi
+-rw-r--r--   0        0        0      969 2023-06-02 07:15:31.130133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy.pyi
+-rw-r--r--   0        0        0      927 2023-06-02 07:15:31.194132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_list.pyi
+-rw-r--r--   0        0        0     4524 2023-06-02 07:15:31.110133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_spec.pyi
+-rw-r--r--   0        0        0      404 2023-06-02 07:15:31.438130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_rollback_config.pyi
+-rw-r--r--   0        0        0      603 2023-06-02 07:15:31.474130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_rolling_update_deployment.pyi
+-rw-r--r--   0        0        0      609 2023-06-02 07:15:31.226132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_run_as_group_strategy_options.pyi
+-rw-r--r--   0        0        0      606 2023-06-02 07:15:31.302132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_run_as_user_strategy_options.pyi
+-rw-r--r--   0        0        0     1132 2023-06-02 07:15:31.162133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_scale.pyi
+-rw-r--r--   0        0        0      389 2023-06-02 07:15:31.078133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_scale_spec.pyi
+-rw-r--r--   0        0        0      607 2023-06-02 07:15:31.054134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_scale_status.pyi
+-rw-r--r--   0        0        0      586 2023-06-02 07:15:31.194132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_se_linux_strategy_options.pyi
+-rw-r--r--   0        0        0      690 2023-06-02 07:15:31.202132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_supplemental_groups_strategy_options.pyi
+-rw-r--r--   0        0        0      338 2023-06-02 07:15:31.462130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_allowed_flex_volume.pyi
+-rw-r--r--   0        0        0      516 2023-06-02 07:15:31.426130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_allowed_host_path.pyi
+-rw-r--r--   0        0        0      633 2023-06-02 07:15:31.154133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_fs_group_strategy_options.pyi
+-rw-r--r--   0        0        0      353 2023-06-02 07:15:31.094133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_host_port_range.pyi
+-rw-r--r--   0        0        0      335 2023-06-02 07:15:31.202132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_id_range.pyi
+-rw-r--r--   0        0        0      945 2023-06-02 07:15:31.070134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy.pyi
+-rw-r--r--   0        0        0      903 2023-06-02 07:15:31.186133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_list.pyi
+-rw-r--r--   0        0        0     4416 2023-06-02 07:15:31.162133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_spec.pyi
+-rw-r--r--   0        0        0      585 2023-06-02 07:15:31.122133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_run_as_group_strategy_options.pyi
+-rw-r--r--   0        0        0      582 2023-06-02 07:15:31.158133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_run_as_user_strategy_options.pyi
+-rw-r--r--   0        0        0      574 2023-06-02 07:15:31.126133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_se_linux_strategy_options.pyi
+-rw-r--r--   0        0        0      666 2023-06-02 07:15:31.262132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_supplemental_groups_strategy_options.pyi
+-rw-r--r--   0        0        0      296 2023-06-02 07:15:31.062134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/runtime_raw_extension.pyi
+-rw-r--r--   0        0        0      886 2023-06-02 07:15:31.486130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_affinity.pyi
+-rw-r--r--   0        0        0      514 2023-06-02 07:15:31.230132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_aggregation_rule.pyi
+-rw-r--r--   0        0        0     1261 2023-06-02 07:15:31.338131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_group.pyi
+-rw-r--r--   0        0        0      599 2023-06-02 07:15:31.426130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_group_list.pyi
+-rw-r--r--   0        0        0      975 2023-06-02 07:15:31.442130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_resource.pyi
+-rw-r--r--   0        0        0      691 2023-06-02 07:15:31.314131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_resource_list.pyi
+-rw-r--r--   0        0        0     1042 2023-06-02 07:15:31.438130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service.pyi
+-rw-r--r--   0        0        0      741 2023-06-02 07:15:31.146133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service_condition.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.270132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service_list.pyi
+-rw-r--r--   0        0        0     1037 2023-06-02 07:15:31.426130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service_spec.pyi
+-rw-r--r--   0        0        0      501 2023-06-02 07:15:31.326131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service_status.pyi
+-rw-r--r--   0        0        0      786 2023-06-02 07:15:31.122133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_versions.pyi
+-rw-r--r--   0        0        0      349 2023-06-02 07:15:31.066134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_attached_volume.pyi
+-rw-r--r--   0        0        0      686 2023-06-02 07:15:31.442130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_aws_elastic_block_store_volume_source.pyi
+-rw-r--r--   0        0        0      807 2023-06-02 07:15:31.346131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_azure_disk_volume_source.pyi
+-rw-r--r--   0        0        0      661 2023-06-02 07:15:31.250132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_azure_file_persistent_volume_source.pyi
+-rw-r--r--   0        0        0      500 2023-06-02 07:15:31.330131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_azure_file_volume_source.pyi
+-rw-r--r--   0        0        0      780 2023-06-02 07:15:31.186133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_binding.pyi
+-rw-r--r--   0        0        0      470 2023-06-02 07:15:31.058134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_capabilities.pyi
+-rw-r--r--   0        0        0      996 2023-06-02 07:15:31.466130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_ceph_fs_persistent_volume_source.pyi
+-rw-r--r--   0        0        0      981 2023-06-02 07:15:31.270132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_ceph_fs_volume_source.pyi
+-rw-r--r--   0        0        0      776 2023-06-02 07:15:31.462130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cinder_persistent_volume_source.pyi
+-rw-r--r--   0        0        0      761 2023-06-02 07:15:31.482130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cinder_volume_source.pyi
+-rw-r--r--   0        0        0      379 2023-06-02 07:15:31.234132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_client_ip_config.pyi
+-rw-r--r--   0        0        0     1023 2023-06-02 07:15:31.094133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role.pyi
+-rw-r--r--   0        0        0      996 2023-06-02 07:15:31.262132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role_binding.pyi
+-rw-r--r--   0        0        0      843 2023-06-02 07:15:31.182133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role_binding_list.pyi
+-rw-r--r--   0        0        0      801 2023-06-02 07:15:31.318131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role_list.pyi
+-rw-r--r--   0        0        0      551 2023-06-02 07:15:31.118133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_component_condition.pyi
+-rw-r--r--   0        0        0      900 2023-06-02 07:15:31.170132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_component_status.pyi
+-rw-r--r--   0        0        0      825 2023-06-02 07:15:31.190132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_component_status_list.pyi
+-rw-r--r--   0        0        0      919 2023-06-02 07:15:31.330131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map.pyi
+-rw-r--r--   0        0        0      470 2023-06-02 07:15:31.418130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_env_source.pyi
+-rw-r--r--   0        0        0      512 2023-06-02 07:15:31.258132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_key_selector.pyi
+-rw-r--r--   0        0        0      789 2023-06-02 07:15:31.262132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_list.pyi
+-rw-r--r--   0        0        0      680 2023-06-02 07:15:31.286131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_node_config_source.pyi
+-rw-r--r--   0        0        0      672 2023-06-02 07:15:31.214132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_projection.pyi
+-rw-r--r--   0        0        0      797 2023-06-02 07:15:31.358131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_volume_source.pyi
+-rw-r--r--   0        0        0     3607 2023-06-02 07:15:31.302132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container.pyi
+-rw-r--r--   0        0        0      424 2023-06-02 07:15:31.486130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_image.pyi
+-rw-r--r--   0        0        0      734 2023-06-02 07:15:31.262132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_port.pyi
+-rw-r--r--   0        0        0      938 2023-06-02 07:15:31.290131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_state.pyi
+-rw-r--r--   0        0        0      427 2023-06-02 07:15:31.190132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_state_running.pyi
+-rw-r--r--   0        0        0     1075 2023-06-02 07:15:31.122133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_state_terminated.pyi
+-rw-r--r--   0        0        0      479 2023-06-02 07:15:31.242132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_state_waiting.pyi
+-rw-r--r--   0        0        0     1020 2023-06-02 07:15:31.082133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_status.pyi
+-rw-r--r--   0        0        0      921 2023-06-02 07:15:31.490130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_controller_revision.pyi
+-rw-r--r--   0        0        0      843 2023-06-02 07:15:31.442130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_controller_revision_list.pyi
+-rw-r--r--   0        0        0      484 2023-06-02 07:15:31.170132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cross_version_object_reference.pyi
+-rw-r--r--   0        0        0     1540 2023-06-02 07:15:31.478130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_csi_persistent_volume_source.pyi
+-rw-r--r--   0        0        0      290 2023-06-02 07:15:31.282132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_endpoint.pyi
+-rw-r--r--   0        0        0     1033 2023-06-02 07:15:31.166133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set.pyi
+-rw-r--r--   0        0        0      738 2023-06-02 07:15:31.178133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_condition.pyi
+-rw-r--r--   0        0        0      789 2023-06-02 07:15:31.474130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_list.pyi
+-rw-r--r--   0        0        0     1077 2023-06-02 07:15:31.106133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_spec.pyi
+-rw-r--r--   0        0        0     1524 2023-06-02 07:15:31.058134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_status.pyi
+-rw-r--r--   0        0        0      620 2023-06-02 07:15:31.162133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_update_strategy.pyi
+-rw-r--r--   0        0        0     1215 2023-06-02 07:15:31.302132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_delete_options.pyi
+-rw-r--r--   0        0        0     1042 2023-06-02 07:15:31.146133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment.pyi
+-rw-r--r--   0        0        0      913 2023-06-02 07:15:31.206132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_condition.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.062134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_list.pyi
+-rw-r--r--   0        0        0     1415 2023-06-02 07:15:31.282132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_spec.pyi
+-rw-r--r--   0        0        0     1413 2023-06-02 07:15:31.434130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_status.pyi
+-rw-r--r--   0        0        0      608 2023-06-02 07:15:31.314131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_strategy.pyi
+-rw-r--r--   0        0        0      507 2023-06-02 07:15:31.458130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_downward_api_projection.pyi
+-rw-r--r--   0        0        0      883 2023-06-02 07:15:31.266132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_downward_api_volume_file.pyi
+-rw-r--r--   0        0        0      632 2023-06-02 07:15:31.230132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_downward_api_volume_source.pyi
+-rw-r--r--   0        0        0      484 2023-06-02 07:15:31.318131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_empty_dir_volume_source.pyi
+-rw-r--r--   0        0        0      718 2023-06-02 07:15:31.066134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoint_address.pyi
+-rw-r--r--   0        0        0      488 2023-06-02 07:15:31.066134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoint_port.pyi
+-rw-r--r--   0        0        0      945 2023-06-02 07:15:31.290131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoint_subset.pyi
+-rw-r--r--   0        0        0      861 2023-06-02 07:15:31.330131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoints.pyi
+-rw-r--r--   0        0        0      789 2023-06-02 07:15:31.110133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoints_list.pyi
+-rw-r--r--   0        0        0      796 2023-06-02 07:15:31.474130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_env_from_source.pyi
+-rw-r--r--   0        0        0      569 2023-06-02 07:15:31.094133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_env_var.pyi
+-rw-r--r--   0        0        0     1201 2023-06-02 07:15:31.310131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_env_var_source.pyi
+-rw-r--r--   0        0        0     2601 2023-06-02 07:15:31.330131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_event.pyi
+-rw-r--r--   0        0        0      765 2023-06-02 07:15:31.114133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_event_list.pyi
+-rw-r--r--   0        0        0      618 2023-06-02 07:15:31.358131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_event_series.pyi
+-rw-r--r--   0        0        0      449 2023-06-02 07:15:31.294131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_event_source.pyi
+-rw-r--r--   0        0        0      362 2023-06-02 07:15:31.426130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_exec_action.pyi
+-rw-r--r--   0        0        0      814 2023-06-02 07:15:31.334131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_fc_volume_source.pyi
+-rw-r--r--   0        0        0      900 2023-06-02 07:15:31.138133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_flex_persistent_volume_source.pyi
+-rw-r--r--   0        0        0      885 2023-06-02 07:15:31.258132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_flex_volume_source.pyi
+-rw-r--r--   0        0        0      504 2023-06-02 07:15:31.218132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_flocker_volume_source.pyi
+-rw-r--r--   0        0        0      671 2023-06-02 07:15:31.106133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_gce_persistent_disk_volume_source.pyi
+-rw-r--r--   0        0        0      542 2023-06-02 07:15:31.490130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_git_repo_volume_source.pyi
+-rw-r--r--   0        0        0      648 2023-06-02 07:15:31.206132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_glusterfs_persistent_volume_source.pyi
+-rw-r--r--   0        0        0      478 2023-06-02 07:15:31.290131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_glusterfs_volume_source.pyi
+-rw-r--r--   0        0        0      394 2023-06-02 07:15:31.078133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_group_version_for_discovery.pyi
+-rw-r--r--   0        0        0      828 2023-06-02 07:15:31.102133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_handler.pyi
+-rw-r--r--   0        0        0     1159 2023-06-02 07:15:31.270132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler.pyi
+-rw-r--r--   0        0        0      873 2023-06-02 07:15:31.450130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_list.pyi
+-rw-r--r--   0        0        0      860 2023-06-02 07:15:31.058134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_spec.pyi
+-rw-r--r--   0        0        0      936 2023-06-02 07:15:31.070134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_status.pyi
+-rw-r--r--   0        0        0      455 2023-06-02 07:15:31.350131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_host_alias.pyi
+-rw-r--r--   0        0        0      404 2023-06-02 07:15:31.274132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_host_path_volume_source.pyi
+-rw-r--r--   0        0        0      824 2023-06-02 07:15:31.478130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_http_get_action.pyi
+-rw-r--r--   0        0        0      320 2023-06-02 07:15:31.274132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_http_header.pyi
+-rw-r--r--   0        0        0      281 2023-06-02 07:15:31.226132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_initializer.pyi
+-rw-r--r--   0        0        0      574 2023-06-02 07:15:31.334131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_initializers.pyi
+-rw-r--r--   0        0        0      392 2023-06-02 07:15:31.234132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_ip_block.pyi
+-rw-r--r--   0        0        0     1511 2023-06-02 07:15:31.098133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_iscsi_persistent_volume_source.pyi
+-rw-r--r--   0        0        0     1496 2023-06-02 07:15:31.238132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_iscsi_volume_source.pyi
+-rw-r--r--   0        0        0      979 2023-06-02 07:15:31.482130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job.pyi
+-rw-r--r--   0        0        0      889 2023-06-02 07:15:31.470130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_condition.pyi
+-rw-r--r--   0        0        0      753 2023-06-02 07:15:31.090133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_list.pyi
+-rw-r--r--   0        0        0     1380 2023-06-02 07:15:31.246132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_spec.pyi
+-rw-r--r--   0        0        0     1099 2023-06-02 07:15:31.322131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_status.pyi
+-rw-r--r--   0        0        0      407 2023-06-02 07:15:31.246132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_key_to_path.pyi
+-rw-r--r--   0        0        0      679 2023-06-02 07:15:31.214132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_label_selector.pyi
+-rw-r--r--   0        0        0      488 2023-06-02 07:15:31.154133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_label_selector_requirement.pyi
+-rw-r--r--   0        0        0      608 2023-06-02 07:15:31.350131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_lifecycle.pyi
+-rw-r--r--   0        0        0      837 2023-06-02 07:15:31.230132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_limit_range.pyi
+-rw-r--r--   0        0        0     1081 2023-06-02 07:15:31.490130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_limit_range_item.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.350131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_limit_range_list.pyi
+-rw-r--r--   0        0        0      411 2023-06-02 07:15:31.326131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_limit_range_spec.pyi
+-rw-r--r--   0        0        0      585 2023-06-02 07:15:31.150133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_list_meta.pyi
+-rw-r--r--   0        0        0      464 2023-06-02 07:15:31.470130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_load_balancer_ingress.pyi
+-rw-r--r--   0        0        0      498 2023-06-02 07:15:31.190132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_load_balancer_status.pyi
+-rw-r--r--   0        0        0      365 2023-06-02 07:15:31.426130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_local_object_reference.pyi
+-rw-r--r--   0        0        0     1081 2023-06-02 07:15:31.278132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_local_subject_access_review.pyi
+-rw-r--r--   0        0        0      403 2023-06-02 07:15:31.450130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_local_volume_source.pyi
+-rw-r--r--   0        0        0     1033 2023-06-02 07:15:31.258132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_namespace.pyi
+-rw-r--r--   0        0        0      789 2023-06-02 07:15:31.238132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_namespace_list.pyi
+-rw-r--r--   0        0        0      380 2023-06-02 07:15:31.134133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_namespace_spec.pyi
+-rw-r--r--   0        0        0      353 2023-06-02 07:15:31.230132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_namespace_status.pyi
+-rw-r--r--   0        0        0      855 2023-06-02 07:15:31.310131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy.pyi
+-rw-r--r--   0        0        0      715 2023-06-02 07:15:31.082133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_egress_rule.pyi
+-rw-r--r--   0        0        0      727 2023-06-02 07:15:31.234132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_ingress_rule.pyi
+-rw-r--r--   0        0        0      813 2023-06-02 07:15:31.210132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_list.pyi
+-rw-r--r--   0        0        0      887 2023-06-02 07:15:31.362131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_peer.pyi
+-rw-r--r--   0        0        0      485 2023-06-02 07:15:31.082133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_port.pyi
+-rw-r--r--   0        0        0     1047 2023-06-02 07:15:31.238132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_spec.pyi
+-rw-r--r--   0        0        0      451 2023-06-02 07:15:31.494130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_nfs_volume_source.pyi
+-rw-r--r--   0        0        0      988 2023-06-02 07:15:31.250132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node.pyi
+-rw-r--r--   0        0        0      329 2023-06-02 07:15:31.106133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_address.pyi
+-rw-r--r--   0        0        0      945 2023-06-02 07:15:31.234132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_affinity.pyi
+-rw-r--r--   0        0        0      904 2023-06-02 07:15:31.242132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_condition.pyi
+-rw-r--r--   0        0        0      500 2023-06-02 07:15:31.102133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_config_source.pyi
+-rw-r--r--   0        0        0     1002 2023-06-02 07:15:31.486130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_config_status.pyi
+-rw-r--r--   0        0        0      494 2023-06-02 07:15:31.118133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_daemon_endpoints.pyi
+-rw-r--r--   0        0        0      759 2023-06-02 07:15:31.150133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_list.pyi
+-rw-r--r--   0        0        0      448 2023-06-02 07:15:31.118133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_selector.pyi
+-rw-r--r--   0        0        0      485 2023-06-02 07:15:31.078133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_selector_requirement.pyi
+-rw-r--r--   0        0        0      794 2023-06-02 07:15:31.298131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_selector_term.pyi
+-rw-r--r--   0        0        0     1113 2023-06-02 07:15:31.294131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_spec.pyi
+-rw-r--r--   0        0        0     2332 2023-06-02 07:15:31.090133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_status.pyi
+-rw-r--r--   0        0        0      918 2023-06-02 07:15:31.066134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_system_info.pyi
+-rw-r--r--   0        0        0      464 2023-06-02 07:15:31.194132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_non_resource_attributes.pyi
+-rw-r--r--   0        0        0      467 2023-06-02 07:15:31.318131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_non_resource_rule.pyi
+-rw-r--r--   0        0        0      438 2023-06-02 07:15:31.338131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_object_field_selector.pyi
+-rw-r--r--   0        0        0     2535 2023-06-02 07:15:31.338131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_object_meta.pyi
+-rw-r--r--   0        0        0     1010 2023-06-02 07:15:31.494130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_object_reference.pyi
+-rw-r--r--   0        0        0      686 2023-06-02 07:15:31.346131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_owner_reference.pyi
+-rw-r--r--   0        0        0     1096 2023-06-02 07:15:31.258132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume.pyi
+-rw-r--r--   0        0        0     1141 2023-06-02 07:15:31.210132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim.pyi
+-rw-r--r--   0        0        0      943 2023-06-02 07:15:31.170132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_condition.pyi
+-rw-r--r--   0        0        0      861 2023-06-02 07:15:31.146133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_list.pyi
+-rw-r--r--   0        0        0     1463 2023-06-02 07:15:31.474130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_spec.pyi
+-rw-r--r--   0        0        0      944 2023-06-02 07:15:31.098133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_status.pyi
+-rw-r--r--   0        0        0      477 2023-06-02 07:15:31.062134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_volume_source.pyi
+-rw-r--r--   0        0        0      831 2023-06-02 07:15:31.326131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_list.pyi
+-rw-r--r--   0        0        0     6866 2023-06-02 07:15:31.054134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_spec.pyi
+-rw-r--r--   0        0        0      581 2023-06-02 07:15:31.306131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_status.pyi
+-rw-r--r--   0        0        0      450 2023-06-02 07:15:31.454130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_photon_persistent_disk_volume_source.pyi
+-rw-r--r--   0        0        0      979 2023-06-02 07:15:31.358131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod.pyi
+-rw-r--r--   0        0        0      969 2023-06-02 07:15:31.170132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_affinity.pyi
+-rw-r--r--   0        0        0      667 2023-06-02 07:15:31.102133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_affinity_term.pyi
+-rw-r--r--   0        0        0      981 2023-06-02 07:15:31.334131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_anti_affinity.pyi
+-rw-r--r--   0        0        0      889 2023-06-02 07:15:31.122133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_condition.pyi
+-rw-r--r--   0        0        0      738 2023-06-02 07:15:31.142133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_dns_config.pyi
+-rw-r--r--   0        0        0      458 2023-06-02 07:15:31.130133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_dns_config_option.pyi
+-rw-r--r--   0        0        0      753 2023-06-02 07:15:31.274132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_list.pyi
+-rw-r--r--   0        0        0      325 2023-06-02 07:15:31.338131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_readiness_gate.pyi
+-rw-r--r--   0        0        0     1313 2023-06-02 07:15:31.482130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_security_context.pyi
+-rw-r--r--   0        0        0     5045 2023-06-02 07:15:31.098133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_spec.pyi
+-rw-r--r--   0        0        0     1898 2023-06-02 07:15:31.178133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_status.pyi
+-rw-r--r--   0        0        0      855 2023-06-02 07:15:31.322131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_template.pyi
+-rw-r--r--   0        0        0      801 2023-06-02 07:15:31.238132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_template_list.pyi
+-rw-r--r--   0        0        0      619 2023-06-02 07:15:31.110133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_template_spec.pyi
+-rw-r--r--   0        0        0      855 2023-06-02 07:15:31.250132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_policy_rule.pyi
+-rw-r--r--   0        0        0      539 2023-06-02 07:15:31.462130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_portworx_volume_source.pyi
+-rw-r--r--   0        0        0      341 2023-06-02 07:15:31.074133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_preconditions.pyi
+-rw-r--r--   0        0        0      483 2023-06-02 07:15:31.470130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_preferred_scheduling_term.pyi
+-rw-r--r--   0        0        0     1488 2023-06-02 07:15:31.334131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_probe.pyi
+-rw-r--r--   0        0        0      560 2023-06-02 07:15:31.322131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_projected_volume_source.pyi
+-rw-r--r--   0        0        0      670 2023-06-02 07:15:31.054134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_quobyte_volume_source.pyi
+-rw-r--r--   0        0        0     1122 2023-06-02 07:15:31.486130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rbd_persistent_volume_source.pyi
+-rw-r--r--   0        0        0     1107 2023-06-02 07:15:31.478130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rbd_volume_source.pyi
+-rw-r--r--   0        0        0     1042 2023-06-02 07:15:31.270132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set.pyi
+-rw-r--r--   0        0        0      741 2023-06-02 07:15:31.222132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_condition.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.438130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_list.pyi
+-rw-r--r--   0        0        0      845 2023-06-02 07:15:31.058134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_spec.pyi
+-rw-r--r--   0        0        0     1102 2023-06-02 07:15:31.478130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_status.pyi
+-rw-r--r--   0        0        0     1141 2023-06-02 07:15:31.238132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller.pyi
+-rw-r--r--   0        0        0      774 2023-06-02 07:15:31.086133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_condition.pyi
+-rw-r--r--   0        0        0      861 2023-06-02 07:15:31.278132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_list.pyi
+-rw-r--r--   0        0        0      874 2023-06-02 07:15:31.466130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_spec.pyi
+-rw-r--r--   0        0        0     1168 2023-06-02 07:15:31.142133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_status.pyi
+-rw-r--r--   0        0        0      995 2023-06-02 07:15:31.266132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_attributes.pyi
+-rw-r--r--   0        0        0      553 2023-06-02 07:15:31.422130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_field_selector.pyi
+-rw-r--r--   0        0        0     1069 2023-06-02 07:15:31.158133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota.pyi
+-rw-r--r--   0        0        0      813 2023-06-02 07:15:31.166133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota_list.pyi
+-rw-r--r--   0        0        0      728 2023-06-02 07:15:31.318131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota_spec.pyi
+-rw-r--r--   0        0        0      524 2023-06-02 07:15:31.194132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota_status.pyi
+-rw-r--r--   0        0        0      545 2023-06-02 07:15:31.110133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_requirements.pyi
+-rw-r--r--   0        0        0      708 2023-06-02 07:15:31.066134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_rule.pyi
+-rw-r--r--   0        0        0      771 2023-06-02 07:15:31.322131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role.pyi
+-rw-r--r--   0        0        0      975 2023-06-02 07:15:31.310131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role_binding.pyi
+-rw-r--r--   0        0        0      801 2023-06-02 07:15:31.302132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role_binding_list.pyi
+-rw-r--r--   0        0        0      759 2023-06-02 07:15:31.178133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role_list.pyi
+-rw-r--r--   0        0        0      361 2023-06-02 07:15:31.306131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role_ref.pyi
+-rw-r--r--   0        0        0      424 2023-06-02 07:15:31.330131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rolling_update_daemon_set.pyi
+-rw-r--r--   0        0        0      558 2023-06-02 07:15:31.110133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rolling_update_deployment.pyi
+-rw-r--r--   0        0        0      416 2023-06-02 07:15:31.066134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rolling_update_stateful_set_strategy.pyi
+-rw-r--r--   0        0        0      997 2023-06-02 07:15:31.446130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale.pyi
+-rw-r--r--   0        0        0     1369 2023-06-02 07:15:31.294131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale_io_persistent_volume_source.pyi
+-rw-r--r--   0        0        0     1354 2023-06-02 07:15:31.306131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale_io_volume_source.pyi
+-rw-r--r--   0        0        0      344 2023-06-02 07:15:31.450130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale_spec.pyi
+-rw-r--r--   0        0        0      401 2023-06-02 07:15:31.114133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale_status.pyi
+-rw-r--r--   0        0        0      554 2023-06-02 07:15:31.266132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scope_selector.pyi
+-rw-r--r--   0        0        0      535 2023-06-02 07:15:31.218132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scoped_resource_selector_requirement.pyi
+-rw-r--r--   0        0        0      638 2023-06-02 07:15:31.098133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_se_linux_options.pyi
+-rw-r--r--   0        0        0     1006 2023-06-02 07:15:31.130133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret.pyi
+-rw-r--r--   0        0        0      461 2023-06-02 07:15:31.222132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_env_source.pyi
+-rw-r--r--   0        0        0      503 2023-06-02 07:15:31.054134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_key_selector.pyi
+-rw-r--r--   0        0        0      771 2023-06-02 07:15:31.290131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_list.pyi
+-rw-r--r--   0        0        0      663 2023-06-02 07:15:31.122133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_projection.pyi
+-rw-r--r--   0        0        0      461 2023-06-02 07:15:31.362131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_reference.pyi
+-rw-r--r--   0        0        0      808 2023-06-02 07:15:31.286131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_volume_source.pyi
+-rw-r--r--   0        0        0     1606 2023-06-02 07:15:31.342131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_security_context.pyi
+-rw-r--r--   0        0        0     1090 2023-06-02 07:15:31.154133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_self_subject_access_review.pyi
+-rw-r--r--   0        0        0      808 2023-06-02 07:15:31.218132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_self_subject_access_review_spec.pyi
+-rw-r--r--   0        0        0     1081 2023-06-02 07:15:31.134133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_self_subject_rules_review.pyi
+-rw-r--r--   0        0        0      398 2023-06-02 07:15:31.198132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_self_subject_rules_review_spec.pyi
+-rw-r--r--   0        0        0      411 2023-06-02 07:15:31.150133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_server_address_by_client_cidr.pyi
+-rw-r--r--   0        0        0     1015 2023-06-02 07:15:31.258132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service.pyi
+-rw-r--r--   0        0        0     1325 2023-06-02 07:15:31.154133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_account.pyi
+-rw-r--r--   0        0        0      819 2023-06-02 07:15:31.202132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_account_list.pyi
+-rw-r--r--   0        0        0      580 2023-06-02 07:15:31.202132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_account_token_projection.pyi
+-rw-r--r--   0        0        0      777 2023-06-02 07:15:31.158133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_list.pyi
+-rw-r--r--   0        0        0      732 2023-06-02 07:15:31.182133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_port.pyi
+-rw-r--r--   0        0        0      464 2023-06-02 07:15:31.218132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_reference.pyi
+-rw-r--r--   0        0        0     2231 2023-06-02 07:15:31.366131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_spec.pyi
+-rw-r--r--   0        0        0      479 2023-06-02 07:15:31.478130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_status.pyi
+-rw-r--r--   0        0        0      479 2023-06-02 07:15:31.070134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_session_affinity_config.pyi
+-rw-r--r--   0        0        0     1051 2023-06-02 07:15:31.146133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set.pyi
+-rw-r--r--   0        0        0      744 2023-06-02 07:15:31.434130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_condition.pyi
+-rw-r--r--   0        0        0      801 2023-06-02 07:15:31.086133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_list.pyi
+-rw-r--r--   0        0        0     1555 2023-06-02 07:15:31.346131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_spec.pyi
+-rw-r--r--   0        0        0     1472 2023-06-02 07:15:31.266132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_status.pyi
+-rw-r--r--   0        0        0      656 2023-06-02 07:15:31.438130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_update_strategy.pyi
+-rw-r--r--   0        0        0     1230 2023-06-02 07:15:31.126133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_status.pyi
+-rw-r--r--   0        0        0      548 2023-06-02 07:15:31.206132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_status_cause.pyi
+-rw-r--r--   0        0        0      979 2023-06-02 07:15:31.286131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_status_details.pyi
+-rw-r--r--   0        0        0     1682 2023-06-02 07:15:31.230132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_class.pyi
+-rw-r--r--   0        0        0      807 2023-06-02 07:15:31.354131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_class_list.pyi
+-rw-r--r--   0        0        0      979 2023-06-02 07:15:31.298131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_os_persistent_volume_source.pyi
+-rw-r--r--   0        0        0      964 2023-06-02 07:15:31.346131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_os_volume_source.pyi
+-rw-r--r--   0        0        0      529 2023-06-02 07:15:31.366131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject.pyi
+-rw-r--r--   0        0        0     1066 2023-06-02 07:15:31.134133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_access_review.pyi
+-rw-r--r--   0        0        0     1255 2023-06-02 07:15:31.074133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_access_review_spec.pyi
+-rw-r--r--   0        0        0      673 2023-06-02 07:15:31.102133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_access_review_status.pyi
+-rw-r--r--   0        0        0      846 2023-06-02 07:15:31.306131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_rules_review_status.pyi
+-rw-r--r--   0        0        0      308 2023-06-02 07:15:31.186133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_sysctl.pyi
+-rw-r--r--   0        0        0      559 2023-06-02 07:15:31.106133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_taint.pyi
+-rw-r--r--   0        0        0      410 2023-06-02 07:15:31.150133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_tcp_socket_action.pyi
+-rw-r--r--   0        0        0      994 2023-06-02 07:15:31.494130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_token_review.pyi
+-rw-r--r--   0        0        0      482 2023-06-02 07:15:31.286131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_token_review_spec.pyi
+-rw-r--r--   0        0        0      789 2023-06-02 07:15:31.090133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_token_review_status.pyi
+-rw-r--r--   0        0        0      778 2023-06-02 07:15:31.466130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_toleration.pyi
+-rw-r--r--   0        0        0      404 2023-06-02 07:15:31.234132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_topology_selector_label_requirement.pyi
+-rw-r--r--   0        0        0      589 2023-06-02 07:15:31.458130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_topology_selector_term.pyi
+-rw-r--r--   0        0        0      472 2023-06-02 07:15:31.110133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_typed_local_object_reference.pyi
+-rw-r--r--   0        0        0      704 2023-06-02 07:15:31.266132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_user_info.pyi
+-rw-r--r--   0        0        0     6540 2023-06-02 07:15:31.274132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume.pyi
+-rw-r--r--   0        0        0     1039 2023-06-02 07:15:31.422130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment.pyi
+-rw-r--r--   0        0        0      831 2023-06-02 07:15:31.282132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment_list.pyi
+-rw-r--r--   0        0        0      423 2023-06-02 07:15:31.062134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment_source.pyi
+-rw-r--r--   0        0        0      539 2023-06-02 07:15:31.454130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment_spec.pyi
+-rw-r--r--   0        0        0      916 2023-06-02 07:15:31.454130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment_status.pyi
+-rw-r--r--   0        0        0      343 2023-06-02 07:15:31.418130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_device.pyi
+-rw-r--r--   0        0        0      485 2023-06-02 07:15:31.226132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_error.pyi
+-rw-r--r--   0        0        0      691 2023-06-02 07:15:31.330131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_mount.pyi
+-rw-r--r--   0        0        0      462 2023-06-02 07:15:31.098133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_node_affinity.pyi
+-rw-r--r--   0        0        0     1211 2023-06-02 07:15:31.326131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_projection.pyi
+-rw-r--r--   0        0        0      734 2023-06-02 07:15:31.442130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_vsphere_virtual_disk_volume_source.pyi
+-rw-r--r--   0        0        0      429 2023-06-02 07:15:31.322131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_watch_event.pyi
+-rw-r--r--   0        0        0      499 2023-06-02 07:15:31.482130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_weighted_pod_affinity_term.pyi
+-rw-r--r--   0        0        0      532 2023-06-02 07:15:31.090133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_aggregation_rule.pyi
+-rw-r--r--   0        0        0      867 2023-06-02 07:15:31.346131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_audit_sink.pyi
+-rw-r--r--   0        0        0      825 2023-06-02 07:15:31.354131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_audit_sink_list.pyi
+-rw-r--r--   0        0        0      544 2023-06-02 07:15:31.242132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_audit_sink_spec.pyi
+-rw-r--r--   0        0        0     1077 2023-06-02 07:15:31.174132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role.pyi
+-rw-r--r--   0        0        0     1050 2023-06-02 07:15:31.278132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding.pyi
+-rw-r--r--   0        0        0      879 2023-06-02 07:15:31.494130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding_list.pyi
+-rw-r--r--   0        0        0      837 2023-06-02 07:15:31.082133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role_list.pyi
+-rw-r--r--   0        0        0      501 2023-06-02 07:15:31.474130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_initializer.pyi
+-rw-r--r--   0        0        0      948 2023-06-02 07:15:31.302132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_initializer_configuration.pyi
+-rw-r--r--   0        0        0      915 2023-06-02 07:15:31.142133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_initializer_configuration_list.pyi
+-rw-r--r--   0        0        0      867 2023-06-02 07:15:31.278132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_pod_preset.pyi
+-rw-r--r--   0        0        0      825 2023-06-02 07:15:31.106133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_pod_preset_list.pyi
+-rw-r--r--   0        0        0     1295 2023-06-02 07:15:31.178133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_pod_preset_spec.pyi
+-rw-r--r--   0        0        0      407 2023-06-02 07:15:31.462130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_policy.pyi
+-rw-r--r--   0        0        0      873 2023-06-02 07:15:31.210132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_policy_rule.pyi
+-rw-r--r--   0        0        0      958 2023-06-02 07:15:31.450130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_priority_class.pyi
+-rw-r--r--   0        0        0      849 2023-06-02 07:15:31.362131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_priority_class_list.pyi
+-rw-r--r--   0        0        0      807 2023-06-02 07:15:31.210132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role.pyi
+-rw-r--r--   0        0        0     1029 2023-06-02 07:15:31.430130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role_binding.pyi
+-rw-r--r--   0        0        0      837 2023-06-02 07:15:31.190132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role_binding_list.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.434130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role_list.pyi
+-rw-r--r--   0        0        0      379 2023-06-02 07:15:31.134133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role_ref.pyi
+-rw-r--r--   0        0        0      636 2023-06-02 07:15:31.162133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_rule.pyi
+-rw-r--r--   0        0        0      464 2023-06-02 07:15:31.174132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_service_reference.pyi
+-rw-r--r--   0        0        0      553 2023-06-02 07:15:31.138133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_subject.pyi
+-rw-r--r--   0        0        0     1093 2023-06-02 07:15:31.446130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment.pyi
+-rw-r--r--   0        0        0      867 2023-06-02 07:15:31.086133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment_list.pyi
+-rw-r--r--   0        0        0      441 2023-06-02 07:15:31.430130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment_source.pyi
+-rw-r--r--   0        0        0      575 2023-06-02 07:15:31.218132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment_spec.pyi
+-rw-r--r--   0        0        0      970 2023-06-02 07:15:31.102133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment_status.pyi
+-rw-r--r--   0        0        0      503 2023-06-02 07:15:31.294131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_error.pyi
+-rw-r--r--   0        0        0      687 2023-06-02 07:15:31.142133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_webhook.pyi
+-rw-r--r--   0        0        0      713 2023-06-02 07:15:31.454130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_webhook_client_config.pyi
+-rw-r--r--   0        0        0      482 2023-06-02 07:15:31.158133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_webhook_throttle_config.pyi
+-rw-r--r--   0        0        0      529 2023-06-02 07:15:31.270132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_aggregation_rule.pyi
+-rw-r--r--   0        0        0     1087 2023-06-02 07:15:31.058134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service.pyi
+-rw-r--r--   0        0        0      756 2023-06-02 07:15:31.070134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_condition.pyi
+-rw-r--r--   0        0        0      825 2023-06-02 07:15:31.158133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_list.pyi
+-rw-r--r--   0        0        0     1112 2023-06-02 07:15:31.198132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_spec.pyi
+-rw-r--r--   0        0        0      531 2023-06-02 07:15:31.122133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_status.pyi
+-rw-r--r--   0        0        0     1222 2023-06-02 07:15:31.322131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request.pyi
+-rw-r--r--   0        0        0      744 2023-06-02 07:15:31.182133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_condition.pyi
+-rw-r--r--   0        0        0      915 2023-06-02 07:15:31.198132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_list.pyi
+-rw-r--r--   0        0        0      950 2023-06-02 07:15:31.446130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_spec.pyi
+-rw-r--r--   0        0        0      738 2023-06-02 07:15:31.150133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_status.pyi
+-rw-r--r--   0        0        0     1068 2023-06-02 07:15:31.194132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role.pyi
+-rw-r--r--   0        0        0     1041 2023-06-02 07:15:31.342131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role_binding.pyi
+-rw-r--r--   0        0        0      873 2023-06-02 07:15:31.210132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role_binding_list.pyi
+-rw-r--r--   0        0        0      831 2023-06-02 07:15:31.218132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role_list.pyi
+-rw-r--r--   0        0        0      936 2023-06-02 07:15:31.118133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_controller_revision.pyi
+-rw-r--r--   0        0        0      873 2023-06-02 07:15:31.354131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_controller_revision_list.pyi
+-rw-r--r--   0        0        0     1060 2023-06-02 07:15:31.254132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job.pyi
+-rw-r--r--   0        0        0      807 2023-06-02 07:15:31.090133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job_list.pyi
+-rw-r--r--   0        0        0     1211 2023-06-02 07:15:31.130133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job_spec.pyi
+-rw-r--r--   0        0        0      661 2023-06-02 07:15:31.242132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job_status.pyi
+-rw-r--r--   0        0        0      772 2023-06-02 07:15:31.482130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_column_definition.pyi
+-rw-r--r--   0        0        0      658 2023-06-02 07:15:31.198132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_conversion.pyi
+-rw-r--r--   0        0        0     1156 2023-06-02 07:15:31.234132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition.pyi
+-rw-r--r--   0        0        0      798 2023-06-02 07:15:31.458130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_condition.pyi
+-rw-r--r--   0        0        0      909 2023-06-02 07:15:31.274132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_list.pyi
+-rw-r--r--   0        0        0      879 2023-06-02 07:15:31.422130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_names.pyi
+-rw-r--r--   0        0        0     2103 2023-06-02 07:15:31.166133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_spec.pyi
+-rw-r--r--   0        0        0      872 2023-06-02 07:15:31.314131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_status.pyi
+-rw-r--r--   0        0        0     1305 2023-06-02 07:15:31.446130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_version.pyi
+-rw-r--r--   0        0        0      617 2023-06-02 07:15:31.298131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_subresource_scale.pyi
+-rw-r--r--   0        0        0      684 2023-06-02 07:15:31.182133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_subresources.pyi
+-rw-r--r--   0        0        0      544 2023-06-02 07:15:31.334131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_validation.pyi
+-rw-r--r--   0        0        0     1078 2023-06-02 07:15:31.274132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set.pyi
+-rw-r--r--   0        0        0      753 2023-06-02 07:15:31.262132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_condition.pyi
+-rw-r--r--   0        0        0      819 2023-06-02 07:15:31.250132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_list.pyi
+-rw-r--r--   0        0        0     1304 2023-06-02 07:15:31.210132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_spec.pyi
+-rw-r--r--   0        0        0     1554 2023-06-02 07:15:31.338131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_status.pyi
+-rw-r--r--   0        0        0      650 2023-06-02 07:15:31.430130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_update_strategy.pyi
+-rw-r--r--   0        0        0     2793 2023-06-02 07:15:31.298131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_event.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.226132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_event_list.pyi
+-rw-r--r--   0        0        0      462 2023-06-02 07:15:31.058134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_event_series.pyi
+-rw-r--r--   0        0        0      872 2023-06-02 07:15:31.250132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_eviction.pyi
+-rw-r--r--   0        0        0      497 2023-06-02 07:15:31.102133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_external_documentation.pyi
+-rw-r--r--   0        0        0      525 2023-06-02 07:15:31.482130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_http_ingress_path.pyi
+-rw-r--r--   0        0        0      459 2023-06-02 07:15:31.202132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_http_ingress_rule_value.pyi
+-rw-r--r--   0        0        0     1060 2023-06-02 07:15:31.498130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress.pyi
+-rw-r--r--   0        0        0      411 2023-06-02 07:15:31.062134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_backend.pyi
+-rw-r--r--   0        0        0      807 2023-06-02 07:15:31.342131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_list.pyi
+-rw-r--r--   0        0        0      579 2023-06-02 07:15:31.166133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_rule.pyi
+-rw-r--r--   0        0        0      905 2023-06-02 07:15:31.246132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_spec.pyi
+-rw-r--r--   0        0        0      494 2023-06-02 07:15:31.466130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_status.pyi
+-rw-r--r--   0        0        0      487 2023-06-02 07:15:31.078133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_tls.pyi
+-rw-r--r--   0        0        0      407 2023-06-02 07:15:31.294131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ip_block.pyi
+-rw-r--r--   0        0        0      634 2023-06-02 07:15:31.466130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_job_template_spec.pyi
+-rw-r--r--   0        0        0     5615 2023-06-02 07:15:31.074133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_json_schema_props.pyi
+-rw-r--r--   0        0        0      837 2023-06-02 07:15:31.430130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_lease.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.150133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_lease_list.pyi
+-rw-r--r--   0        0        0      977 2023-06-02 07:15:31.074133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_lease_spec.pyi
+-rw-r--r--   0        0        0     1126 2023-06-02 07:15:31.470130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_local_subject_access_review.pyi
+-rw-r--r--   0        0        0      930 2023-06-02 07:15:31.226132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration.pyi
+-rw-r--r--   0        0        0      933 2023-06-02 07:15:31.306131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration_list.pyi
+-rw-r--r--   0        0        0      885 2023-06-02 07:15:31.438130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy.pyi
+-rw-r--r--   0        0        0      760 2023-06-02 07:15:31.090133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_egress_rule.pyi
+-rw-r--r--   0        0        0      772 2023-06-02 07:15:31.342131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_ingress_rule.pyi
+-rw-r--r--   0        0        0      843 2023-06-02 07:15:31.086133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_list.pyi
+-rw-r--r--   0        0        0      917 2023-06-02 07:15:31.238132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_peer.pyi
+-rw-r--r--   0        0        0      500 2023-06-02 07:15:31.298131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_port.pyi
+-rw-r--r--   0        0        0     1092 2023-06-02 07:15:31.342131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_spec.pyi
+-rw-r--r--   0        0        0      479 2023-06-02 07:15:31.082133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_non_resource_attributes.pyi
+-rw-r--r--   0        0        0      482 2023-06-02 07:15:31.206132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_non_resource_rule.pyi
+-rw-r--r--   0        0        0     1168 2023-06-02 07:15:31.214132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget.pyi
+-rw-r--r--   0        0        0      879 2023-06-02 07:15:31.178133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_list.pyi
+-rw-r--r--   0        0        0      787 2023-06-02 07:15:31.126133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_spec.pyi
+-rw-r--r--   0        0        0      929 2023-06-02 07:15:31.222132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_status.pyi
+-rw-r--r--   0        0        0      870 2023-06-02 07:15:31.086133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_policy_rule.pyi
+-rw-r--r--   0        0        0      955 2023-06-02 07:15:31.114133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_priority_class.pyi
+-rw-r--r--   0        0        0      843 2023-06-02 07:15:31.494130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_priority_class_list.pyi
+-rw-r--r--   0        0        0     1087 2023-06-02 07:15:31.302132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set.pyi
+-rw-r--r--   0        0        0      756 2023-06-02 07:15:31.362131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_condition.pyi
+-rw-r--r--   0        0        0      825 2023-06-02 07:15:31.082133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_list.pyi
+-rw-r--r--   0        0        0      917 2023-06-02 07:15:31.254132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_spec.pyi
+-rw-r--r--   0        0        0     1132 2023-06-02 07:15:31.294131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_status.pyi
+-rw-r--r--   0        0        0     1010 2023-06-02 07:15:31.350131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_resource_attributes.pyi
+-rw-r--r--   0        0        0      723 2023-06-02 07:15:31.450130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_resource_rule.pyi
+-rw-r--r--   0        0        0      801 2023-06-02 07:15:31.250132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role.pyi
+-rw-r--r--   0        0        0     1020 2023-06-02 07:15:31.134133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role_binding.pyi
+-rw-r--r--   0        0        0      831 2023-06-02 07:15:31.054134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role_binding_list.pyi
+-rw-r--r--   0        0        0      789 2023-06-02 07:15:31.222132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role_list.pyi
+-rw-r--r--   0        0        0      376 2023-06-02 07:15:31.206132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role_ref.pyi
+-rw-r--r--   0        0        0      439 2023-06-02 07:15:31.126133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_rolling_update_daemon_set.pyi
+-rw-r--r--   0        0        0      431 2023-06-02 07:15:31.494130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_rolling_update_stateful_set_strategy.pyi
+-rw-r--r--   0        0        0      807 2023-06-02 07:15:31.346131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_rule_with_operations.pyi
+-rw-r--r--   0        0        0     1135 2023-06-02 07:15:31.310131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_self_subject_access_review.pyi
+-rw-r--r--   0        0        0      853 2023-06-02 07:15:31.166133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_self_subject_access_review_spec.pyi
+-rw-r--r--   0        0        0     1126 2023-06-02 07:15:31.062134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_self_subject_rules_review.pyi
+-rw-r--r--   0        0        0      413 2023-06-02 07:15:31.174132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_self_subject_rules_review_spec.pyi
+-rw-r--r--   0        0        0     1096 2023-06-02 07:15:31.138133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set.pyi
+-rw-r--r--   0        0        0      759 2023-06-02 07:15:31.354131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_condition.pyi
+-rw-r--r--   0        0        0      831 2023-06-02 07:15:31.306131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_list.pyi
+-rw-r--r--   0        0        0     1642 2023-06-02 07:15:31.278132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_spec.pyi
+-rw-r--r--   0        0        0     1502 2023-06-02 07:15:31.254132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_status.pyi
+-rw-r--r--   0        0        0      686 2023-06-02 07:15:31.162133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_update_strategy.pyi
+-rw-r--r--   0        0        0     1697 2023-06-02 07:15:31.094133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_storage_class.pyi
+-rw-r--r--   0        0        0      837 2023-06-02 07:15:31.114133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_storage_class_list.pyi
+-rw-r--r--   0        0        0      544 2023-06-02 07:15:31.114133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject.pyi
+-rw-r--r--   0        0        0     1111 2023-06-02 07:15:31.470130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_access_review.pyi
+-rw-r--r--   0        0        0     1297 2023-06-02 07:15:31.270132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_access_review_spec.pyi
+-rw-r--r--   0        0        0      688 2023-06-02 07:15:31.190132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_access_review_status.pyi
+-rw-r--r--   0        0        0      891 2023-06-02 07:15:31.142133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_rules_review_status.pyi
+-rw-r--r--   0        0        0     1039 2023-06-02 07:15:31.458130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_token_review.pyi
+-rw-r--r--   0        0        0      497 2023-06-02 07:15:31.130133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_token_review_spec.pyi
+-rw-r--r--   0        0        0      819 2023-06-02 07:15:31.462130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_token_review_status.pyi
+-rw-r--r--   0        0        0      719 2023-06-02 07:15:31.354131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_user_info.pyi
+-rw-r--r--   0        0        0      936 2023-06-02 07:15:31.118133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration.pyi
+-rw-r--r--   0        0        0      945 2023-06-02 07:15:31.222132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration_list.pyi
+-rw-r--r--   0        0        0     1084 2023-06-02 07:15:31.438130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment.pyi
+-rw-r--r--   0        0        0      861 2023-06-02 07:15:31.194132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment_list.pyi
+-rw-r--r--   0        0        0      438 2023-06-02 07:15:31.314131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment_source.pyi
+-rw-r--r--   0        0        0      569 2023-06-02 07:15:31.290131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment_spec.pyi
+-rw-r--r--   0        0        0      961 2023-06-02 07:15:31.286131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment_status.pyi
+-rw-r--r--   0        0        0      500 2023-06-02 07:15:31.466130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_error.pyi
+-rw-r--r--   0        0        0     1255 2023-06-02 07:15:31.314131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_webhook.pyi
+-rw-r--r--   0        0        0      936 2023-06-02 07:15:31.242132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_controller_revision.pyi
+-rw-r--r--   0        0        0      873 2023-06-02 07:15:31.158133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_controller_revision_list.pyi
+-rw-r--r--   0        0        0     1078 2023-06-02 07:15:31.286131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set.pyi
+-rw-r--r--   0        0        0      753 2023-06-02 07:15:31.282132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_condition.pyi
+-rw-r--r--   0        0        0      819 2023-06-02 07:15:31.278132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_list.pyi
+-rw-r--r--   0        0        0     1107 2023-06-02 07:15:31.186133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_spec.pyi
+-rw-r--r--   0        0        0     1554 2023-06-02 07:15:31.358131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_status.pyi
+-rw-r--r--   0        0        0      650 2023-06-02 07:15:31.454130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_update_strategy.pyi
+-rw-r--r--   0        0        0     1087 2023-06-02 07:15:31.462130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment.pyi
+-rw-r--r--   0        0        0      928 2023-06-02 07:15:31.170132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_condition.pyi
+-rw-r--r--   0        0        0      825 2023-06-02 07:15:31.262132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_list.pyi
+-rw-r--r--   0        0        0     1445 2023-06-02 07:15:31.310131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_spec.pyi
+-rw-r--r--   0        0        0     1443 2023-06-02 07:15:31.338131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_status.pyi
+-rw-r--r--   0        0        0      638 2023-06-02 07:15:31.118133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_strategy.pyi
+-rw-r--r--   0        0        0     1087 2023-06-02 07:15:31.446130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set.pyi
+-rw-r--r--   0        0        0      756 2023-06-02 07:15:31.358131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_condition.pyi
+-rw-r--r--   0        0        0      825 2023-06-02 07:15:31.298131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_list.pyi
+-rw-r--r--   0        0        0      860 2023-06-02 07:15:31.342131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_spec.pyi
+-rw-r--r--   0        0        0     1132 2023-06-02 07:15:31.094133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_status.pyi
+-rw-r--r--   0        0        0      439 2023-06-02 07:15:31.314131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_rolling_update_daemon_set.pyi
+-rw-r--r--   0        0        0      573 2023-06-02 07:15:31.094133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_rolling_update_deployment.pyi
+-rw-r--r--   0        0        0      431 2023-06-02 07:15:31.478130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_rolling_update_stateful_set_strategy.pyi
+-rw-r--r--   0        0        0     1042 2023-06-02 07:15:31.318131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_scale.pyi
+-rw-r--r--   0        0        0      359 2023-06-02 07:15:31.138133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_scale_spec.pyi
+-rw-r--r--   0        0        0      577 2023-06-02 07:15:31.242132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_scale_status.pyi
+-rw-r--r--   0        0        0     1096 2023-06-02 07:15:31.126133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set.pyi
+-rw-r--r--   0        0        0      759 2023-06-02 07:15:31.146133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_condition.pyi
+-rw-r--r--   0        0        0      831 2023-06-02 07:15:31.226132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_list.pyi
+-rw-r--r--   0        0        0     1585 2023-06-02 07:15:31.430130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_spec.pyi
+-rw-r--r--   0        0        0     1502 2023-06-02 07:15:31.446130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_status.pyi
+-rw-r--r--   0        0        0      686 2023-06-02 07:15:31.198132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_update_strategy.pyi
+-rw-r--r--   0        0        0     1069 2023-06-02 07:15:31.290131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job.pyi
+-rw-r--r--   0        0        0      813 2023-06-02 07:15:31.182133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job_list.pyi
+-rw-r--r--   0        0        0     1217 2023-06-02 07:15:31.214132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job_spec.pyi
+-rw-r--r--   0        0        0      664 2023-06-02 07:15:31.142133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job_status.pyi
+-rw-r--r--   0        0        0      637 2023-06-02 07:15:31.486130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_job_template_spec.pyi
+-rw-r--r--   0        0        0      499 2023-06-02 07:15:31.458130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_cross_version_object_reference.pyi
+-rw-r--r--   0        0        0      826 2023-06-02 07:15:31.422130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_external_metric_source.pyi
+-rw-r--r--   0        0        0      775 2023-06-02 07:15:31.318131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_external_metric_status.pyi
+-rw-r--r--   0        0        0     1204 2023-06-02 07:15:31.054134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.442130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_condition.pyi
+-rw-r--r--   0        0        0      903 2023-06-02 07:15:31.486130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_list.pyi
+-rw-r--r--   0        0        0      933 2023-06-02 07:15:31.362131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_spec.pyi
+-rw-r--r--   0        0        0     1261 2023-06-02 07:15:31.254132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_status.pyi
+-rw-r--r--   0        0        0     1209 2023-06-02 07:15:31.202132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_metric_spec.pyi
+-rw-r--r--   0        0        0     1215 2023-06-02 07:15:31.198132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_metric_status.pyi
+-rw-r--r--   0        0        0      919 2023-06-02 07:15:31.174132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_object_metric_source.pyi
+-rw-r--r--   0        0        0      922 2023-06-02 07:15:31.134133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_object_metric_status.pyi
+-rw-r--r--   0        0        0      618 2023-06-02 07:15:31.326131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_pods_metric_source.pyi
+-rw-r--r--   0        0        0      621 2023-06-02 07:15:31.138133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_pods_metric_status.pyi
+-rw-r--r--   0        0        0      625 2023-06-02 07:15:31.422130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_resource_metric_source.pyi
+-rw-r--r--   0        0        0      574 2023-06-02 07:15:31.266132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_resource_metric_status.pyi
+-rw-r--r--   0        0        0      499 2023-06-02 07:15:31.186133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_cross_version_object_reference.pyi
+-rw-r--r--   0        0        0      598 2023-06-02 07:15:31.250132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_external_metric_source.pyi
+-rw-r--r--   0        0        0      616 2023-06-02 07:15:31.450130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_external_metric_status.pyi
+-rw-r--r--   0        0        0     1204 2023-06-02 07:15:31.206132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler.pyi
+-rw-r--r--   0        0        0      795 2023-06-02 07:15:31.174132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_condition.pyi
+-rw-r--r--   0        0        0      903 2023-06-02 07:15:31.254132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_list.pyi
+-rw-r--r--   0        0        0      933 2023-06-02 07:15:31.086133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_spec.pyi
+-rw-r--r--   0        0        0     1261 2023-06-02 07:15:31.138133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_status.pyi
+-rw-r--r--   0        0        0      513 2023-06-02 07:15:31.154133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_identifier.pyi
+-rw-r--r--   0        0        0     1209 2023-06-02 07:15:31.246132 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_spec.pyi
+-rw-r--r--   0        0        0     1215 2023-06-02 07:15:31.166133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_status.pyi
+-rw-r--r--   0        0        0      660 2023-06-02 07:15:31.074133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_target.pyi
+-rw-r--r--   0        0        0      636 2023-06-02 07:15:31.070134 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_value_status.pyi
+-rw-r--r--   0        0        0      817 2023-06-02 07:15:31.130133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_object_metric_source.pyi
+-rw-r--r--   0        0        0      835 2023-06-02 07:15:31.146133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_object_metric_status.pyi
+-rw-r--r--   0        0        0      586 2023-06-02 07:15:31.358131 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_pods_metric_source.pyi
+-rw-r--r--   0        0        0      604 2023-06-02 07:15:31.474130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_pods_metric_status.pyi
+-rw-r--r--   0        0        0      474 2023-06-02 07:15:31.114133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_resource_metric_source.pyi
+-rw-r--r--   0        0        0      492 2023-06-02 07:15:31.078133 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_resource_metric_status.pyi
+-rw-r--r--   0        0        0      716 2023-06-02 07:15:31.422130 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/version_info.pyi
+-rw-r--r--   0        0        0       74 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/rest.pyi
+-rw-r--r--   0        0        0      474 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/config/__init__.pyi
+-rw-r--r--   0        0        0       38 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/config/config_exception.pyi
+-rw-r--r--   0        0        0      203 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/config/incluster_config.pyi
+-rw-r--r--   0        0        0      920 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/config/kube_config.pyi
+-rw-r--r--   0        0        0      206 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/stream.pyi
+-rw-r--r--   0        0        0   395180 2023-06-02 07:15:31.550129 kubernetes-stubs-elephant-fork-9.0.1/kubernetes_ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 07:15:13.586287 kubernetes-stubs-elephant-fork-9.0.1/kubernetes_ext/py.typed
+-rw-r--r--   0        0        0      760 2023-06-02 07:15:31.638128 kubernetes-stubs-elephant-fork-9.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1281 2023-06-02 07:15:32.915864 kubernetes-stubs-elephant-fork-9.0.1/setup.py
+-rw-r--r--   0        0        0     1387 2023-06-02 07:15:32.916169 kubernetes-stubs-elephant-fork-9.0.1/PKG-INFO
```

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/README.md` & `kubernetes-stubs-elephant-fork-9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/__init__.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/__init__.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/admissionregistration_v1alpha1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/admissionregistration_v1alpha1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/admissionregistration_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/admissionregistration_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiextensions_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiextensions_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiregistration_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiregistration_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apiregistration_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apiregistration_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apps_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apps_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apps_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apps_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/apps_v1beta2_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/apps_v1beta2_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/auditregistration_v1alpha1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/auditregistration_v1alpha1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authentication_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authentication_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authorization_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authorization_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/authorization_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/authorization_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/autoscaling_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/autoscaling_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/autoscaling_v2beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/autoscaling_v2beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/autoscaling_v2beta2_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/autoscaling_v2beta2_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/batch_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/batch_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/batch_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/batch_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/batch_v2alpha1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/batch_v2alpha1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/certificates_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/certificates_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/coordination_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/coordination_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/core_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/core_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/custom_objects_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/custom_objects_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/events_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/events_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/extensions_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/extensions_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/networking_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/networking_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/policy_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/policy_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/rbacAuthorization_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/rbacAuthorization_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/rbacAuthorization_v1alpha1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/rbacAuthorization_v1alpha1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/rbacAuthorization_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/rbacAuthorization_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/scheduling_v1alpha1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/scheduling_v1alpha1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/scheduling_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/scheduling_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/settings_v1alpha1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/settings_v1alpha1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/storage_v1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/storage_v1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/storage_v1alpha1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/storage_v1alpha1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/api/storage_v1beta1_api.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/api/storage_v1beta1_api.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/exceptions.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/__init__.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/admissionregistration_v1beta1_service_reference.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/admissionregistration_v1beta1_service_reference.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/admissionregistration_v1beta1_webhook_client_config.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/admissionregistration_v1beta1_webhook_client_config.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apiextensions_v1beta1_webhook_client_config.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apiextensions_v1beta1_webhook_client_config.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apiregistration_v1beta1_service_reference.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apiregistration_v1beta1_service_reference.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_rollback.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_rollback.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_deployment_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_deployment_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_rolling_update_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_rolling_update_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_scale.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_scale.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/apps_v1beta1_scale_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/apps_v1beta1_scale_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_allowed_host_path.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_allowed_host_path.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_rollback.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_rollback.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_deployment_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_deployment_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_fs_group_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_fs_group_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_pod_security_policy_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_rolling_update_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_rolling_update_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_run_as_group_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_run_as_group_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_run_as_user_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_run_as_user_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_scale.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_scale.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_scale_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_scale_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_se_linux_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_se_linux_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/extensions_v1beta1_supplemental_groups_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/extensions_v1beta1_supplemental_groups_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_allowed_host_path.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_allowed_host_path.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_fs_group_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_fs_group_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_pod_security_policy_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_run_as_group_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_run_as_group_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_run_as_user_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_run_as_user_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_se_linux_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_se_linux_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/policy_v1beta1_supplemental_groups_strategy_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/policy_v1beta1_supplemental_groups_strategy_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_affinity.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_affinity.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_aggregation_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_aggregation_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_group.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_group.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_group_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_group_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_resource.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_resource.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_resource_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_resource_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_service_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_service_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_api_versions.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_api_versions.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_aws_elastic_block_store_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_aws_elastic_block_store_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_azure_disk_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_azure_disk_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_azure_file_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_azure_file_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_binding.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_binding.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_ceph_fs_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_ceph_fs_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_ceph_fs_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_ceph_fs_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cinder_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cinder_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cinder_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cinder_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role_binding.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role_binding.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role_binding_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role_binding_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_cluster_role_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_cluster_role_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_component_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_component_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_component_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_component_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_component_status_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_component_status_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_key_selector.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_key_selector.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_node_config_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_node_config_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_projection.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_projection.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_config_map_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_config_map_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_port.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_port.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_state.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_state.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_state_terminated.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_state_terminated.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_container_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_container_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_controller_revision.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_controller_revision.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_controller_revision_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_controller_revision_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_csi_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_csi_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_daemon_set_update_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_daemon_set_update_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_delete_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_delete_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_deployment_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_deployment_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_downward_api_volume_file.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_downward_api_volume_file.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_downward_api_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_downward_api_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoint_address.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoint_address.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoint_subset.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoint_subset.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoints.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_endpoints_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_endpoints_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_env_from_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_env_from_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_env_var.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_env_var.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_env_var_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_env_var_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_event.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_event.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_event_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_event_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_event_series.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_event_series.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_fc_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_fc_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_flex_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_flex_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_flex_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_flex_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_gce_persistent_disk_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_gce_persistent_disk_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_git_repo_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_git_repo_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_glusterfs_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_glusterfs_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_handler.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_handler.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_horizontal_pod_autoscaler_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_http_get_action.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_http_get_action.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_initializers.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_initializers.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_iscsi_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_iscsi_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_iscsi_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_iscsi_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_job_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_job_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_label_selector.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_label_selector.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_lifecycle.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_lifecycle.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_limit_range.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_limit_range.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_limit_range_item.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_limit_range_item.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_limit_range_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_limit_range_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_list_meta.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_list_meta.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_local_subject_access_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_local_subject_access_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_namespace.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_namespace.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_namespace_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_namespace_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_egress_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_egress_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_ingress_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_ingress_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_peer.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_peer.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_network_policy_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_network_policy_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_affinity.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_affinity.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_config_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_config_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_selector_term.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_selector_term.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_node_system_info.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_node_system_info.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_object_meta.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_object_meta.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_object_reference.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_object_reference.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_owner_reference.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_owner_reference.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_claim_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_claim_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_persistent_volume_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_persistent_volume_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_affinity.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_affinity.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_affinity_term.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_affinity_term.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_anti_affinity.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_anti_affinity.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_dns_config.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_dns_config.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_security_context.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_security_context.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_template.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_template.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_template_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_template_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_pod_template_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_pod_template_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_policy_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_policy_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_portworx_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_portworx_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_probe.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_probe.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_projected_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_projected_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_quobyte_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_quobyte_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rbd_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rbd_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rbd_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rbd_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replica_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replica_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_replication_controller_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_replication_controller_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_attributes.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_attributes.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_field_selector.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_field_selector.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_quota_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_quota_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_requirements.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_requirements.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_resource_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_resource_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role_binding.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role_binding.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role_binding_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role_binding_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_role_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_role_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_rolling_update_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_rolling_update_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale_io_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale_io_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scale_io_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scale_io_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scope_selector.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scope_selector.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_scoped_resource_selector_requirement.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_scoped_resource_selector_requirement.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_se_linux_options.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_se_linux_options.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_projection.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_projection.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_secret_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_secret_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_security_context.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_security_context.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_self_subject_access_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_self_subject_access_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_self_subject_access_review_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_self_subject_access_review_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_self_subject_rules_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_self_subject_rules_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_account.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_account.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_account_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_account_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_account_token_projection.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_account_token_projection.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_port.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_port.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_service_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_service_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_stateful_set_update_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_stateful_set_update_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_status_cause.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_status_cause.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_status_details.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_status_details.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_class.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_class.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_class_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_class_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_os_persistent_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_os_persistent_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_storage_os_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_storage_os_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_access_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_access_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_access_review_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_access_review_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_access_review_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_access_review_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_subject_rules_review_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_subject_rules_review_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_taint.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_taint.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_token_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_token_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_token_review_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_token_review_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_toleration.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_toleration.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_topology_selector_term.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_topology_selector_term.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_user_info.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_user_info.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_attachment_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_attachment_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_mount.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_mount.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_volume_projection.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_volume_projection.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1_vsphere_virtual_disk_volume_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1_vsphere_virtual_disk_volume_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_aggregation_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_aggregation_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_audit_sink.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_audit_sink.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_audit_sink_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_audit_sink_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_audit_sink_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_audit_sink_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role_binding_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_cluster_role_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_cluster_role_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_initializer_configuration.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_initializer_configuration.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_initializer_configuration_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_initializer_configuration_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_pod_preset.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_pod_preset.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_pod_preset_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_pod_preset_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_pod_preset_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_pod_preset_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_policy_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_policy_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_priority_class.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_priority_class.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_priority_class_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_priority_class_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role_binding.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role_binding.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role_binding_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role_binding_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_role_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_role_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_subject.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_subject.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_volume_attachment_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_volume_attachment_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_webhook.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_webhook.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1alpha1_webhook_client_config.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1alpha1_webhook_client_config.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_aggregation_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_aggregation_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_api_service_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_api_service_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_certificate_signing_request_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role_binding.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role_binding.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role_binding_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role_binding_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cluster_role_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cluster_role_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_controller_revision.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_controller_revision.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_controller_revision_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_controller_revision_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_cron_job_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_cron_job_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_column_definition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_column_definition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_conversion.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_conversion.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_names.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_names.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_version.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_definition_version.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_subresource_scale.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_subresource_scale.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_subresources.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_subresources.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_custom_resource_validation.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_custom_resource_validation.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_daemon_set_update_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_daemon_set_update_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_event.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_event.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_event_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_event_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_eviction.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_eviction.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_http_ingress_path.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_http_ingress_path.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_ingress_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_ingress_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_job_template_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_job_template_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_json_schema_props.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_json_schema_props.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_lease.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_lease.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_lease_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_lease_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_lease_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_lease_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_local_subject_access_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_local_subject_access_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_mutating_webhook_configuration_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_egress_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_egress_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_ingress_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_ingress_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_peer.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_peer.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_network_policy_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_network_policy_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_pod_disruption_budget_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_policy_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_policy_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_priority_class.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_priority_class.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_priority_class_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_priority_class_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_replica_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_replica_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_resource_attributes.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_resource_attributes.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_resource_rule.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_resource_rule.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role_binding.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role_binding.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role_binding_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role_binding_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_role_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_role_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_rule_with_operations.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_rule_with_operations.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_self_subject_access_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_self_subject_access_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_self_subject_access_review_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_self_subject_access_review_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_self_subject_rules_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_self_subject_rules_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_stateful_set_update_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_stateful_set_update_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_storage_class.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_storage_class.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_storage_class_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_storage_class_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_access_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_access_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_access_review_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_access_review_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_access_review_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_access_review_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_subject_rules_review_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_subject_rules_review_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_token_review.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_token_review.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_token_review_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_token_review_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_user_info.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_user_info.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_validating_webhook_configuration_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_volume_attachment_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_volume_attachment_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta1_webhook.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta1_webhook.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_controller_revision.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_controller_revision.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_controller_revision_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_controller_revision_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_daemon_set_update_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_daemon_set_update_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_deployment_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_deployment_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_replica_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_replica_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_rolling_update_deployment.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_rolling_update_deployment.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_scale.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_scale.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_scale_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_scale_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v1beta2_stateful_set_update_strategy.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v1beta2_stateful_set_update_strategy.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_cron_job_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_cron_job_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2alpha1_job_template_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2alpha1_job_template_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_external_metric_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_external_metric_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_external_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_external_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_horizontal_pod_autoscaler_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_metric_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_metric_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_object_metric_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_object_metric_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_object_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_object_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_pods_metric_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_pods_metric_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_pods_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_pods_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_resource_metric_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_resource_metric_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta1_resource_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta1_resource_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_external_metric_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_external_metric_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_external_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_external_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_condition.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_condition.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_list.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_list.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_horizontal_pod_autoscaler_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_identifier.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_identifier.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_spec.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_spec.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_target.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_target.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_metric_value_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_metric_value_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_object_metric_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_object_metric_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_object_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_object_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_pods_metric_source.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_pods_metric_source.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/v2beta2_pods_metric_status.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/v2beta2_pods_metric_status.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/client/models/version_info.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/client/models/version_info.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes-stubs/config/kube_config.pyi` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes-stubs/config/kube_config.pyi`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/kubernetes_ext/__init__.py` & `kubernetes-stubs-elephant-fork-9.0.1/kubernetes_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/pyproject.toml` & `kubernetes-stubs-elephant-fork-9.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 homepage = "https://github.com/lexdene/kubernetes-stubs"
 description = "Type stubs for the Kubernetes Python API client"
 authors = ["Nikhil Benesch <nikhil.benesch@gmail.com>", "Rami Chowdhury <rami.chowdhury@gmail.com>", "Elephant Liu"]
 license = "Apache-2.0"
 readme = "README.md"
 
 # version will be updated by build script
-version = "9.0.0"
+version = "9.0.1"
 
 packages = [
     { include = "kubernetes_ext" },
     { include = "kubernetes-stubs" },
 ]
 include = [
     { path = "kubernetes_ext/**/*" },
```

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/setup.py` & `kubernetes-stubs-elephant-fork-9.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  'kubernetes-stubs': ['client/*',
                       'client/api/*',
                       'client/models/*',
                       'config/*']}
 
 setup_kwargs = {
     'name': 'kubernetes-stubs-elephant-fork',
-    'version': '9.0.0',
+    'version': '9.0.1',
     'description': 'Type stubs for the Kubernetes Python API client',
     'long_description': '# kubernetes-stubs-elephant-fork\n\nfork of [kubernetes-stubs][1]\n\n## why fork?\n\n[kubernetes-stubs][1] has not provided stubs for [kubernetes][2] >= 23.0 yet (2023-05-30).\n\n`kubernetes-stubs-elephant-fork` provides stubs for all releases after 7.0 of [kubernetes][2],\neven includes any release in the future automatically.\n\nI run a crontab by github actions which looks for new releases of [kubernetes][2]\nand build stubs for it.\n\n[1]: https://pypi.org/project/kubernetes-stubs\n[2]: https://pypi.org/project/kubernetes\n',
     'author': 'Nikhil Benesch',
     'author_email': 'nikhil.benesch@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/lexdene/kubernetes-stubs',
```

### Comparing `kubernetes-stubs-elephant-fork-9.0.0/PKG-INFO` & `kubernetes-stubs-elephant-fork-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubernetes-stubs-elephant-fork
-Version: 9.0.0
+Version: 9.0.1
 Summary: Type stubs for the Kubernetes Python API client
 Home-page: https://github.com/lexdene/kubernetes-stubs
 License: Apache-2.0
 Author: Nikhil Benesch
 Author-email: nikhil.benesch@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
```

