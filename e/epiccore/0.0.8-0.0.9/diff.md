# Comparing `tmp/epiccore-0.0.8.tar.gz` & `tmp/epiccore-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/epiccore-0.0.8.tar", last modified: Thu Nov 12 16:16:09 2020, max compression
+gzip compressed data, was "dist/epiccore-0.0.9.tar", last modified: Fri Nov 13 11:34:10 2020, max compression
```

## Comparing `epiccore-0.0.8.tar` & `epiccore-0.0.9.tar`

### file list

```diff
@@ -1,128 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-12 16:16:09.314977 epiccore-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     9251 2020-11-12 16:16:09.314977 epiccore-0.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (116)     7372 2020-11-12 16:16:01.000000 epiccore-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-12 16:16:09.302977 epiccore-0.0.8/epiccore/
--rwxr-xr-x   0 runner    (1001) docker     (116)     3842 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-12 16:16:09.302977 epiccore-0.0.8/epiccore/api/
--rwxr-xr-x   0 runner    (1001) docker     (116)      503 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    12126 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/billing_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    25446 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/catalog_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    12516 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/data_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    48710 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/job_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    19059 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/jobauth_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    31297 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/jobstep_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6179 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/profile_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    12527 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/projects_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    24370 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api/teams_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    27526 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/api_client.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    17018 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4622 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-12 16:16:09.306977 epiccore-0.0.8/epiccore/models/
--rwxr-xr-x   0 runner    (1001) docker     (116)     2982 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5090 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/batch_application_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5162 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/batch_application_list.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5905 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/batch_application_version_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    13982 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/batch_queue_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3903 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/budget.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3993 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/data_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     7536 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/folder.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8551 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/folder_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5810 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response200.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5821 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2001.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5788 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2002.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5779 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2003.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5809 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2004.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5791 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2005.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5791 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2006.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5812 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2007.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5782 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/inline_response2008.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    16470 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3932 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_app_options.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6336 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_array_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     7002 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6762 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_auth_status.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4050 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_cluster_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6594 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     7472 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_data_binding.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6152 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_log.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3752 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_quote.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6398 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    17499 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_step.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    19444 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_step_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8202 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_summary.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     9366 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/job_task_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6324 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/limit.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8425 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/limits.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6802 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/product_name.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5670 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/profile_summary.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6040 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/project.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4697 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/sla.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     9925 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/task_quote.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6830 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/team.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6998 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/team_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5224 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/team_membership.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4222 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/models/user_name.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    12535 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-12 16:16:09.314977 epiccore-0.0.8/epiccore/test/
--rwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2176 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_batch_application_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2442 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_batch_application_list.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1928 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_batch_application_version_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2206 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_batch_queue_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1171 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_billing_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1567 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_budget.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1407 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_catalog_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1121 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_data_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1573 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_data_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1901 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_folder.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2016 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_folder_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3375 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response200.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3126 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2001.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2866 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2002.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6706 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2003.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3160 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2004.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3366 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2005.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2278 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2006.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2208 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2007.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2354 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_inline_response2008.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3482 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1677 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1720 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_app_options.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4389 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_array_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1651 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2065 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_auth_status.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1639 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_cluster_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1771 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3225 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_data_binding.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1620 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_log.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1963 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_quote.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2290 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2138 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_step.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2480 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_step_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1724 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_summary.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1871 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_job_task_spec.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1225 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_jobauth_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1445 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_jobstep_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2303 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_limit.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3727 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_limits.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1778 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_product_name.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1043 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_profile_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1699 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_profile_summary.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1666 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_project.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1133 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_projects_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1552 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_sla.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1795 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_task_quote.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1635 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_team.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1714 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_team_details.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1669 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_team_membership.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1379 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_teams_api.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1553 2020-11-12 16:16:01.000000 epiccore-0.0.8/epiccore/test/test_user_name.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-12 16:16:09.302977 epiccore-0.0.8/epiccore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9251 2020-11-12 16:16:09.000000 epiccore-0.0.8/epiccore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3938 2020-11-12 16:16:09.000000 epiccore-0.0.8/epiccore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-12 16:16:09.000000 epiccore-0.0.8/epiccore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       36 2020-11-12 16:16:09.000000 epiccore-0.0.8/epiccore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-11-12 16:16:09.000000 epiccore-0.0.8/epiccore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       97 2020-11-12 16:16:01.000000 epiccore-0.0.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (116)      822 2020-11-12 16:16:09.314977 epiccore-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      170 2020-11-12 16:16:01.000000 epiccore-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-13 11:34:10.298578 epiccore-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     9236 2020-11-13 11:34:10.298578 epiccore-0.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (116)     7365 2020-11-13 11:33:56.000000 epiccore-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-13 11:34:10.290578 epiccore-0.0.9/epiccore/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3842 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-13 11:34:10.294578 epiccore-0.0.9/epiccore/api/
+-rwxr-xr-x   0 runner    (1001) docker     (116)      503 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    12126 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/billing_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    25446 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/catalog_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    12516 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/data_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    48710 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/job_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19059 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/jobauth_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    31297 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/jobstep_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6179 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/profile_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    12527 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/projects_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    24370 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api/teams_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    27526 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/api_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    17012 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4622 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-13 11:34:10.298578 epiccore-0.0.9/epiccore/models/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2982 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5090 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/batch_application_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5162 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/batch_application_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5905 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/batch_application_version_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    13982 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/batch_queue_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3903 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/budget.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3993 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/data_spec.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     7536 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/folder.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8551 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/folder_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5810 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response200.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5821 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2001.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5788 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2002.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5779 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2003.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5809 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2004.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5791 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2005.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5791 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2006.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5812 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2007.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5782 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/inline_response2008.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    16610 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3932 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_app_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6336 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_array_spec.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     7002 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6762 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_auth_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4050 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_cluster_spec.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6594 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     7472 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_data_binding.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6152 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3752 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_quote.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6398 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_spec.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    17499 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_step.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    19444 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_step_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8202 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     9366 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/job_task_spec.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6324 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/limit.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8425 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/limits.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6802 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/product_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5670 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/profile_summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6040 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/project.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4697 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/sla.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     9925 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/task_quote.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6830 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/team.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6998 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/team_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5224 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/team_membership.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4222 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/models/user_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    12535 2020-11-13 11:33:56.000000 epiccore-0.0.9/epiccore/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-13 11:34:10.294578 epiccore-0.0.9/epiccore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     9236 2020-11-13 11:34:09.000000 epiccore-0.0.9/epiccore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2047 2020-11-13 11:34:10.000000 epiccore-0.0.9/epiccore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-13 11:34:09.000000 epiccore-0.0.9/epiccore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       36 2020-11-13 11:34:09.000000 epiccore-0.0.9/epiccore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2020-11-13 11:34:09.000000 epiccore-0.0.9/epiccore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       97 2020-11-13 11:33:56.000000 epiccore-0.0.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (116)      822 2020-11-13 11:34:10.298578 epiccore-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      170 2020-11-13 11:33:56.000000 epiccore-0.0.9/setup.py
```

### Comparing `epiccore-0.0.8/PKG-INFO` & `epiccore-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epiccore
-Version: 0.0.8
+Version: 0.0.9
 Summary: "EPIC Core API"
 Home-page: UNKNOWN
 Author: "Zenotech"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Description: # epiccore
         REST API for interacting with EPIC (https://epic.zenotech.com) services. <br /> 
@@ -40,15 +40,15 @@
         from __future__ import print_function
         
         import time
         import epiccore
         from epiccore.rest import ApiException
         from pprint import pprint
         
-        # Defining the host is optional and defaults to https://epic-qa.zenotech.com/api/v2
+        # Defining the host is optional and defaults to https://epic.zenotech.com/api/v2
         # See configuration.py for a list of all supported configuration parameters.
         configuration = epiccore.Configuration(
             host = "https://epic.zenotech.com/api/v2"
         )
         
         # The client must configure the authentication and authorization parameters
         # in accordance with the API server security policy.
@@ -77,15 +77,15 @@
             except ApiException as e:
                 print("Exception when calling BillingApi->billing_limits_list: %s\n" % e)
             
         ```
         
         ## Documentation for API Endpoints
         
-        All URIs are relative to *https://epic-qa.zenotech.com/api/v2*
+        All URIs are relative to *https://epic.zenotech.com/api/v2*
         
         Class | Method | HTTP request | Description
         ------------ | ------------- | ------------- | -------------
         *BillingApi* | [**billing_limits_list**](docs/BillingApi.md#billing_limits_list) | **GET** /billing/limits/ | 
         *BillingApi* | [**billing_limits_partial_update**](docs/BillingApi.md#billing_limits_partial_update) | **PATCH** /billing/limits/ | 
         *CatalogApi* | [**catalog_applications_list**](docs/CatalogApi.md#catalog_applications_list) | **GET** /catalog/applications/ | 
         *CatalogApi* | [**catalog_applications_read**](docs/CatalogApi.md#catalog_applications_read) | **GET** /catalog/applications/{id}/ | 
@@ -174,15 +174,14 @@
         - **API key parameter name**: Authorization
         - **Location**: HTTP header
         
         
         ## Author
         
         support@zenotech.com
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `epiccore-0.0.8/README.md` & `epiccore-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from __future__ import print_function
 
 import time
 import epiccore
 from epiccore.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to https://epic-qa.zenotech.com/api/v2
+# Defining the host is optional and defaults to https://epic.zenotech.com/api/v2
 # See configuration.py for a list of all supported configuration parameters.
 configuration = epiccore.Configuration(
     host = "https://epic.zenotech.com/api/v2"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
@@ -69,15 +69,15 @@
     except ApiException as e:
         print("Exception when calling BillingApi->billing_limits_list: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://epic-qa.zenotech.com/api/v2*
+All URIs are relative to *https://epic.zenotech.com/api/v2*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *BillingApi* | [**billing_limits_list**](docs/BillingApi.md#billing_limits_list) | **GET** /billing/limits/ | 
 *BillingApi* | [**billing_limits_partial_update**](docs/BillingApi.md#billing_limits_partial_update) | **PATCH** /billing/limits/ | 
 *CatalogApi* | [**catalog_applications_list**](docs/CatalogApi.md#catalog_applications_list) | **GET** /catalog/applications/ | 
 *CatalogApi* | [**catalog_applications_read**](docs/CatalogApi.md#catalog_applications_read) | **GET** /catalog/applications/{id}/ | 
@@ -165,8 +165,8 @@
 - **Type**: API key
 - **API key parameter name**: Authorization
 - **Location**: HTTP header
 
 
 ## Author
 
-support@zenotech.com
+support@zenotech.com
```

### Comparing `epiccore-0.0.8/epiccore/__init__.py` & `epiccore-0.0.9/epiccore/__init__.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/billing_api.py` & `epiccore-0.0.9/epiccore/api/billing_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/catalog_api.py` & `epiccore-0.0.9/epiccore/api/catalog_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/data_api.py` & `epiccore-0.0.9/epiccore/api/data_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/job_api.py` & `epiccore-0.0.9/epiccore/api/job_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/jobauth_api.py` & `epiccore-0.0.9/epiccore/api/jobauth_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/jobstep_api.py` & `epiccore-0.0.9/epiccore/api/jobstep_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/profile_api.py` & `epiccore-0.0.9/epiccore/api/profile_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/projects_api.py` & `epiccore-0.0.9/epiccore/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api/teams_api.py` & `epiccore-0.0.9/epiccore/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/api_client.py` & `epiccore-0.0.9/epiccore/api_client.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/configuration.py` & `epiccore-0.0.9/epiccore/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                  discard_unknown_keys=False,
                  disabled_client_side_validations="",
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ):
         """Constructor
         """
-        self._base_path = "https://epic-qa.zenotech.com/api/v2" if host is None else host
+        self._base_path = "https://epic.zenotech.com/api/v2" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -410,15 +410,15 @@
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://epic-qa.zenotech.com/api/v2",
+                'url': "https://epic.zenotech.com/api/v2",
                 'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `epiccore-0.0.8/epiccore/exceptions.py` & `epiccore-0.0.9/epiccore/exceptions.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/__init__.py` & `epiccore-0.0.9/epiccore/models/__init__.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/batch_application_details.py` & `epiccore-0.0.9/epiccore/models/batch_application_details.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/batch_application_list.py` & `epiccore-0.0.9/epiccore/models/batch_application_list.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/batch_application_version_details.py` & `epiccore-0.0.9/epiccore/models/batch_application_version_details.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/batch_queue_details.py` & `epiccore-0.0.9/epiccore/models/batch_queue_details.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/budget.py` & `epiccore-0.0.9/epiccore/models/budget.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/data_spec.py` & `epiccore-0.0.9/epiccore/models/data_spec.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/folder.py` & `epiccore-0.0.9/epiccore/models/folder.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/folder_details.py` & `epiccore-0.0.9/epiccore/models/folder_details.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response200.py` & `epiccore-0.0.9/epiccore/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2001.py` & `epiccore-0.0.9/epiccore/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2002.py` & `epiccore-0.0.9/epiccore/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2003.py` & `epiccore-0.0.9/epiccore/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2004.py` & `epiccore-0.0.9/epiccore/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2005.py` & `epiccore-0.0.9/epiccore/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2006.py` & `epiccore-0.0.9/epiccore/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2007.py` & `epiccore-0.0.9/epiccore/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/inline_response2008.py` & `epiccore-0.0.9/epiccore/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job.py` & `epiccore-0.0.9/epiccore/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'submitted_by': 'str',
         'submitted_at': 'str',
         'finished': 'bool',
         'resource': 'BatchQueueDetails',
         'project': 'int',
         'invoice_reference': 'str',
         'config': 'JobConfiguration',
-        'job_steps': 'JobStep'
+        'job_steps': 'list[JobStep]'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'app': 'app',
         'app_options': 'app_options',
@@ -471,27 +471,29 @@
 
         self._config = config
 
     @property
     def job_steps(self):
         """Gets the job_steps of this Job.  # noqa: E501
 
+        The job steps associated with this Job  # noqa: E501
 
         :return: The job_steps of this Job.  # noqa: E501
-        :rtype: JobStep
+        :rtype: list[JobStep]
         """
         return self._job_steps
 
     @job_steps.setter
     def job_steps(self, job_steps):
         """Sets the job_steps of this Job.
 
+        The job steps associated with this Job  # noqa: E501
 
         :param job_steps: The job_steps of this Job.  # noqa: E501
-        :type job_steps: JobStep
+        :type job_steps: list[JobStep]
         """
 
         self._job_steps = job_steps
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `epiccore-0.0.8/epiccore/models/job_app_options.py` & `epiccore-0.0.9/epiccore/models/job_app_options.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_array_spec.py` & `epiccore-0.0.9/epiccore/models/job_array_spec.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_auth.py` & `epiccore-0.0.9/epiccore/models/job_auth.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_auth_status.py` & `epiccore-0.0.9/epiccore/models/job_auth_status.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_cluster_spec.py` & `epiccore-0.0.9/epiccore/models/job_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_configuration.py` & `epiccore-0.0.9/epiccore/models/job_configuration.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_data_binding.py` & `epiccore-0.0.9/epiccore/models/job_data_binding.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_log.py` & `epiccore-0.0.9/epiccore/models/job_log.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_quote.py` & `epiccore-0.0.9/epiccore/models/job_quote.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_spec.py` & `epiccore-0.0.9/epiccore/models/job_spec.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_step.py` & `epiccore-0.0.9/epiccore/models/job_step.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_step_details.py` & `epiccore-0.0.9/epiccore/models/job_step_details.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_summary.py` & `epiccore-0.0.9/epiccore/models/job_summary.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/job_task_spec.py` & `epiccore-0.0.9/epiccore/models/job_task_spec.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/limit.py` & `epiccore-0.0.9/epiccore/models/limit.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/limits.py` & `epiccore-0.0.9/epiccore/models/limits.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/product_name.py` & `epiccore-0.0.9/epiccore/models/product_name.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/profile_summary.py` & `epiccore-0.0.9/epiccore/models/profile_summary.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/project.py` & `epiccore-0.0.9/epiccore/models/project.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/sla.py` & `epiccore-0.0.9/epiccore/models/sla.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/task_quote.py` & `epiccore-0.0.9/epiccore/models/task_quote.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/team.py` & `epiccore-0.0.9/epiccore/models/team.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/team_details.py` & `epiccore-0.0.9/epiccore/models/team_details.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/team_membership.py` & `epiccore-0.0.9/epiccore/models/team_membership.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/models/user_name.py` & `epiccore-0.0.9/epiccore/models/user_name.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore/rest.py` & `epiccore-0.0.9/epiccore/rest.py`

 * *Files identical despite different names*

### Comparing `epiccore-0.0.8/epiccore.egg-info/PKG-INFO` & `epiccore-0.0.9/epiccore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epiccore
-Version: 0.0.8
+Version: 0.0.9
 Summary: "EPIC Core API"
 Home-page: UNKNOWN
 Author: "Zenotech"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Description: # epiccore
         REST API for interacting with EPIC (https://epic.zenotech.com) services. <br /> 
@@ -40,15 +40,15 @@
         from __future__ import print_function
         
         import time
         import epiccore
         from epiccore.rest import ApiException
         from pprint import pprint
         
-        # Defining the host is optional and defaults to https://epic-qa.zenotech.com/api/v2
+        # Defining the host is optional and defaults to https://epic.zenotech.com/api/v2
         # See configuration.py for a list of all supported configuration parameters.
         configuration = epiccore.Configuration(
             host = "https://epic.zenotech.com/api/v2"
         )
         
         # The client must configure the authentication and authorization parameters
         # in accordance with the API server security policy.
@@ -77,15 +77,15 @@
             except ApiException as e:
                 print("Exception when calling BillingApi->billing_limits_list: %s\n" % e)
             
         ```
         
         ## Documentation for API Endpoints
         
-        All URIs are relative to *https://epic-qa.zenotech.com/api/v2*
+        All URIs are relative to *https://epic.zenotech.com/api/v2*
         
         Class | Method | HTTP request | Description
         ------------ | ------------- | ------------- | -------------
         *BillingApi* | [**billing_limits_list**](docs/BillingApi.md#billing_limits_list) | **GET** /billing/limits/ | 
         *BillingApi* | [**billing_limits_partial_update**](docs/BillingApi.md#billing_limits_partial_update) | **PATCH** /billing/limits/ | 
         *CatalogApi* | [**catalog_applications_list**](docs/CatalogApi.md#catalog_applications_list) | **GET** /catalog/applications/ | 
         *CatalogApi* | [**catalog_applications_read**](docs/CatalogApi.md#catalog_applications_read) | **GET** /catalog/applications/{id}/ | 
@@ -174,15 +174,14 @@
         - **API key parameter name**: Authorization
         - **Location**: HTTP header
         
         
         ## Author
         
         support@zenotech.com
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `epiccore-0.0.8/setup.cfg` & `epiccore-0.0.9/setup.cfg`

 * *Files identical despite different names*

