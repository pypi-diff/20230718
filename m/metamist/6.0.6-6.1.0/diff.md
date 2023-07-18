# Comparing `tmp/metamist-6.0.6.tar.gz` & `tmp/metamist-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-6.0.6.tar", last modified: Thu Jun 22 11:50:42 2023, max compression
+gzip compressed data, was "metamist-6.1.0.tar", last modified: Tue Jul 18 03:00:55 2023, max compression
```

## Comparing `metamist-6.0.6.tar` & `metamist-6.1.0.tar`

### file list

```diff
@@ -1,116 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.040164 metamist-6.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 11:44:49.000000 metamist-6.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 11:44:49.000000 metamist-6.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-22 11:50:42.040164 metamist-6.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-06-22 11:44:49.000000 metamist-6.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.000163 metamist-6.0.6/metamist/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.004163 metamist-6.0.6/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23776 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47368 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46972 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.008164 metamist-6.0.6/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.012163 metamist-6.0.6/metamist/audit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/audit_upload_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/audithelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/delete_sequence_files_from_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)    27845 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.012163 metamist-6.0.6/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-22 11:47:48.000000 metamist-6.0.6/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.020164 metamist-6.0.6/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/assay.py
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_assays_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/family_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/project_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sequencing_group_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.020164 metamist-6.0.6/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.024164 metamist-6.0.6/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31027 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50852 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.000163 metamist-6.0.6/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 11:44:49.000000 metamist-6.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 11:50:42.040164 metamist-6.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-22 11:44:49.000000 metamist-6.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.040164 metamist-6.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_metamist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_update_participant_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-22 11:44:49.000000 metamist-6.0.6/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:00:55.569671 metamist-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-18 02:56:06.000000 metamist-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 02:56:06.000000 metamist-6.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-18 03:00:55.569671 metamist-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-07-18 02:56:06.000000 metamist-6.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:00:55.553671 metamist-6.1.0/metamist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:00:55.557671 metamist-6.1.0/metamist/audit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/audit/audit_upload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/audit/audithelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/audit/delete_assay_files_from_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24194 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/audit/generic_auditor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:00:55.557671 metamist-6.1.0/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-18 02:58:38.000000 metamist-6.1.0/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:00:55.561671 metamist-6.1.0/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31027 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50886 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-18 02:56:06.000000 metamist-6.1.0/metamist/parser/sample_file_map_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:00:55.557671 metamist-6.1.0/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-18 03:00:55.000000 metamist-6.1.0/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-18 03:00:55.000000 metamist-6.1.0/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:00:55.000000 metamist-6.1.0/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:00:55.000000 metamist-6.1.0/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 03:00:55.000000 metamist-6.1.0/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 03:00:55.000000 metamist-6.1.0/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 02:56:06.000000 metamist-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:00:55.569671 metamist-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-18 02:56:06.000000 metamist-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:00:55.569671 metamist-6.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_update_participant_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-07-18 02:56:06.000000 metamist-6.1.0/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-18 02:56:06.000000 metamist-6.1.0/test/testbase.py
```

### Comparing `metamist-6.0.6/LICENSE` & `metamist-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/PKG-INFO` & `metamist-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.6
+Version: 6.1.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.6/README.md` & `metamist-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/metamist/audit/audit_upload_bucket.py` & `metamist-6.1.0/metamist/audit/audit_upload_bucket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 """
 This auditor looks for sequence files in the main upload bucket that can be deleted or ingested,
 as well as samples that have no completed cram.
 
 Procedure:
 1. Input a Metamist dataset, sequence types to audit, and file types to search for in the bucket
-2. Get all the participants, samples, and sequences for this dataset from Metamist
-3. Search the upload bucket for all sequence files, and compare to the files in the metamist sequences
+2. Get all the participants, samples, sequencing groups, and assays for this dataset
+3. Search the upload bucket for all assay files, and compare to the files in the metamist assay reads
     - If there are discrepencies, check if the file name and size is the same in the bucket as it is in metamist
       - If the name and file size are the same, assume this file has just been moved around in the bucket
-4. Check if a sample has a completed cram - if so, its sequence data can be removed
-5. Any remaining sequence data in the bucket might require ingestion
-6. Create reports in the audit_results folder of the upload bucket, containing sequence files to delete,
-   ingest, and any samples without completed crams.
+4. Check if a sequencing group has a completed cram - if so, its assay read files can be removed
+5. Any remaining assay data in the bucket might require ingestion
+6. Create reports in the audit_results folder of the upload bucket, containing assay read files to delete,
+   ingest, and any sequencing groups without completed crams.
 """
 
 
 from datetime import datetime
 import sys
 import logging
 import os
@@ -47,15 +47,15 @@
     'cram': CRAM_EXTENSIONS,
     'all_reads': READ_EXTENSIONS,
     'gvcf': GVCF_EXTENSIONS,
     'vcf': VCF_EXTENSIONS,
     'all': ALL_EXTENSIONS,
 }
 
-SEQUENCE_TYPES_MAP = {
+SEQUENCING_TYPES_MAP = {
     'genome': [
         'genome',
     ],
     'exome': [
         'exome',
     ],
     'all': [
@@ -85,67 +85,74 @@
         )
 
     def write_upload_bucket_audit_reports(
         self,
         bucket_name: str,
         sequencing_type_str: str,
         file_types_str: str,
-        sequence_files_to_delete: list[tuple[str, int, str, list[int]]],
-        sequence_files_to_ingest: list[tuple[str, str, str, int, str]],
-        incomplete_samples: list[tuple[str, str]],
+        assay_files_to_delete: list[tuple[str, int, str, list[int]]],
+        assay_files_to_ingest: list[tuple[str, str, str, int, str]],
+        unaligned_sgs: list[tuple[str, str]],
     ):
-        """Write the sequences to delete and ingest to csv files and upload them to the bucket"""
-        # Writing the output to files with the file type, sequence type, and date specified
+        """
+        Writes the 'sequence files to delete/ingest' csv reports and upload them to the bucket.
+        Also writes a report for any sequence files found that match existing samples and may
+        require ingestion.
+
+        The reports name includes the file types, sequencing types, and date of the audit.
+        """
         today = datetime.today().strftime('%Y-%m-%d')
 
         report_path = f'{bucket_name}/audit_results/{today}/'
 
-        # Sequences to delete report has several data points for validation
-        if not sequence_files_to_delete:
-            logging.info('No sequence read files to delete found. Skipping report...')
+        if not assay_files_to_delete:
+            logging.info('No assay read files to delete found. Skipping report...')
         else:
-            sequences_to_delete_file = f'{self.dataset}_{file_types_str}_{sequencing_type_str}_sequences_to_delete_{today}.csv'
+            assays_to_delete_file = f'{self.dataset}_{file_types_str}_{sequencing_type_str}_assay_files_to_delete_{today}.csv'
             self.write_csv_report_to_cloud(
-                data_to_write=sequence_files_to_delete,
-                report_path=os.path.join(report_path, sequences_to_delete_file),
+                data_to_write=assay_files_to_delete,
+                report_path=os.path.join(report_path, assays_to_delete_file),
                 header_row=[
-                    'Sample_ID',
-                    'Sequence_ID',
-                    'Sequence_Path',
+                    'SG_ID',
+                    'Assay_ID',
+                    'Assay_Read_File_Path',
                     'Analysis_IDs',
                     'Filesize',
                 ],
             )
 
-        # Sequences to ingest file only contains paths to the (possibly) uningested files
-        if not sequence_files_to_ingest:
-            logging.info('No sequence reads to ingest found. Skipping report...')
+        # 'Sequences to ingest' report contains paths to the (possibly) uningested files - and any samples/SGs that might be related
+        if not assay_files_to_ingest:
+            logging.info('No assay reads to ingest found. Skipping report...')
         else:
-            sequences_to_ingest_file = f'{self.dataset}_{file_types_str}_{sequencing_type_str}_sequences_to_ingest_{today}.csv'
+            assays_to_ingest_file = f'{self.dataset}_{file_types_str}_{sequencing_type_str}_assay_files_to_ingest_{today}.csv'
             self.write_csv_report_to_cloud(
-                data_to_write=sequence_files_to_ingest,
-                report_path=os.path.join(report_path, sequences_to_ingest_file),
+                data_to_write=assay_files_to_ingest,
+                report_path=os.path.join(report_path, assays_to_ingest_file),
                 header_row=[
-                    'Sequence_Path',
-                    'Extenal_Sample_ID',
-                    'Internal_Sample_ID',
+                    'Assay_File_Path',
+                    'SG_ID',
+                    'Sample_ID',
+                    'Sample_External_ID',
                     'CRAM_Analysis_ID',
                     'CRAM_Path',
                 ],
             )
 
-        # Write the samples without any completed cram to a csv
-        if not incomplete_samples:
-            logging.info(f'No samples without crams found. Skipping report...')
+        # Write the sequencing groups without any completed cram to a csv
+        if not unaligned_sgs:
+            logging.info(
+                f'No sequencing groups without crams found. Skipping report...'
+            )
         else:
-            incomplete_samples_file = f'{self.dataset}_{file_types_str}_{sequencing_type_str}_samples_without_crams_{today}.csv'
+            unaligned_sgs_file = f'{self.dataset}_{file_types_str}_{sequencing_type_str}_unaligned_sgs_{today}.csv'
             self.write_csv_report_to_cloud(
-                data_to_write=incomplete_samples,
-                report_path=os.path.join(report_path, incomplete_samples_file),
-                header_row=['Internal_Sample_ID', 'External_Sample_ID'],
+                data_to_write=unaligned_sgs,
+                report_path=os.path.join(report_path, unaligned_sgs_file),
+                header_row=['SG_ID', 'Sample_ID', 'Sample_External_ID'],
             )
 
 
 async def audit_upload_bucket_files(
     dataset, sequencing_type, file_types, default_analysis_type, default_analysis_status
 ):
     """
@@ -154,18 +161,19 @@
     Reports any files to delete, files to ingest, and samples without completed crams in output files
     """
     config = get_config()
     if not dataset:
         dataset = config['workflow']['dataset']
 
     bucket_name = config['storage']['default']['upload']
+    bucket_name = f'gs://cpg-{dataset}-main-upload'
 
     auditor = UploadBucketAuditor(
         dataset=dataset,
-        sequencing_type=SEQUENCE_TYPES_MAP.get(sequencing_type),
+        sequencing_type=SEQUENCING_TYPES_MAP.get(sequencing_type),
         file_types=FILE_TYPES_MAP.get(file_types),
         default_analysis_type=default_analysis_type,
         default_analysis_status=default_analysis_status,
     )
 
     # Get all the participants and all the samples mapped to participants
     participant_data = auditor.get_participant_data_for_dataset()
@@ -173,65 +181,70 @@
     # Get all the samples
     sample_internal_external_id_map = auditor.map_internal_to_external_sample_ids(
         participant_data
     )
 
     # Get all the sequences for the samples in the dataset and map them to their samples and reads
     (
-        seq_id_sample_id_map,
-        sequence_filepaths_filesizes,
-    ) = auditor.get_sequence_map_from_participants(participant_data)
+        sg_sample_id_map,
+        assay_sg_id_map,
+        assay_filepaths_filesizes,
+    ) = auditor.get_assay_map_from_participants(participant_data)
 
     # Get all completed cram output paths for the samples in the dataset and validate them
-    sample_cram_paths = auditor.get_analysis_cram_paths_for_dataset_samples(
-        sample_internal_external_id_map
-    )
+    sg_cram_paths = auditor.get_analysis_cram_paths_for_dataset_sgs(assay_sg_id_map)
 
-    # Identify samples with and without completed crams
-    sample_completion = auditor.get_complete_and_incomplete_samples(
-        sample_internal_external_id_map, sample_cram_paths
-    )
-    incomplete_samples = [
-        (sample_id, sample_internal_external_id_map.get(sample_id))
-        for sample_id in sample_completion.get('incomplete')
+    # Identify sgs with and without completed crams
+    sg_completion = auditor.get_complete_and_incomplete_sgs(
+        assay_sg_id_map, sg_cram_paths
+    )
+    unaligned_sgs = [
+        (
+            sg_id,
+            sg_sample_id_map[sg_id],
+            sample_internal_external_id_map.get(sg_sample_id_map[sg_id]),
+        )
+        for sg_id in sg_completion.get('incomplete')
     ]
 
     # Samples with completed crams can have their sequences deleted - these are the obvious ones
     (
-        sequence_reads_to_delete,
-        sequence_files_to_ingest,
+        reads_to_delete,
+        reads_to_ingest,
     ) = await auditor.get_reads_to_delete_or_ingest(
         bucket_name,
-        sample_completion.get('complete'),
-        sequence_filepaths_filesizes,
-        seq_id_sample_id_map,
+        sg_completion.get('complete'),
+        assay_filepaths_filesizes,
+        sg_sample_id_map,
+        assay_sg_id_map,
         sample_internal_external_id_map,
     )
 
-    possible_sequence_ingests = auditor.find_crams_for_reads_to_ingest(
-        sequence_files_to_ingest, sample_cram_paths
+    possible_assay_ingests = auditor.find_crams_for_reads_to_ingest(
+        reads_to_ingest, sg_cram_paths
     )
 
     auditor.write_upload_bucket_audit_reports(
         bucket_name,
         sequencing_type_str=sequencing_type,
         file_types_str=file_types,
-        sequence_files_to_delete=sequence_reads_to_delete,
-        sequence_files_to_ingest=possible_sequence_ingests,
-        incomplete_samples=incomplete_samples,
+        assay_files_to_delete=reads_to_delete,
+        assay_files_to_ingest=possible_assay_ingests,
+        unaligned_sgs=unaligned_sgs,
     )
 
 
 @click.command()
 @click.option(
     '--dataset',
+    '-d',
     help='Metamist dataset, used to filter samples',
 )
 @click.option(
-    '--sequence-type',
+    '--sequencing-type',
     '-s',
     type=click.Choice(['genome', 'exome', 'all']),
     required='True',
     help='genome, exome, or all',
 )
 @click.option(
     '--file-types',
```

### Comparing `metamist-6.0.6/metamist/audit/delete_sequence_files_from_audit.py` & `metamist-6.1.0/metamist/audit/delete_assay_files_from_audit.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 This script will take a path to a csv file, containing a column with rows populated
 by paths to delete. The --delete-field-name option allows you to specify which field
 of the csv contains the paths to delete.
 Creates a log file of all the deletes, in the same directory as the input csv.
 
 The typical upload-bucket audit results will be found in a file such as:
- > gs://cpg-dataset-main-upload/audit_results/2023-xx-xx/dataset_seqtype_readstype_sequences_to_delete_2023-xx-xx.csv
+ > gs://cpg-dataset-main-upload/audit_results/2023-xx-xx/dataset_seqtype_readstype_assay_files_to_delete_20xx-xx-xx.csv
 And the field name containing the delete paths will be
- > "Sequence_Path"
+ > "Assay_Read_File_Path"
 """
 
 import csv
 from datetime import datetime
 import logging
 import os
 import sys
@@ -40,15 +40,15 @@
         # Many possible http exceptions could occur so use a broad exception
         except Exception:  # pylint: disable=W0718
             logging.warning(f'{location.name} threw an exception - file not deleted.')
 
     return deleted_files
 
 
-@click.command('Delete the sequence paths found by the audit')
+@click.command('Delete the assay files found by the audit')
 @click.option(
     '--delete-field-name',
     '-d',
     help='The field in the input csv corresponding to the files to delete',
     required=True,
 )
 @click.argument('delete-file-path')
@@ -76,15 +76,14 @@
     logging.info(f'{len(deleted_files)} sequence files deleted.')
 
     # Write a log of the deleted files to the same location
     log_path = f'{delete_file_path.removesuffix(os.path.basename(delete_file_path))}deleted_{TODAY}.csv'
     AuditHelper.write_csv_report_to_cloud(
         deleted_files, log_path, header_row=['Deleted_file_path']
     )
-    logging.info(f'Wrote deletion log to {log_path}.')
 
 
 if __name__ == '__main__':
     logging.basicConfig(
         level=logging.INFO,
         format='%(asctime)s %(levelname)s %(module)s:%(lineno)d - %(message)s',
         datefmt='%Y-%M-%d %H:%M:%S',
```

### Comparing `metamist-6.0.6/metamist/audit/generic_auditor.py` & `metamist-6.1.0/metamist/audit/generic_auditor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,78 @@
 from collections import defaultdict, namedtuple
 import logging
 import os
 from typing import Any
 
+from gql.transport.requests import log as requests_logger
 from metamist.audit.audithelper import AuditHelper
-from metamist.graphql import query
+from metamist.graphql import query, gql
 
 
 ANALYSIS_TYPES = [
     'QC',
-    'JOINT_CALLING',
+    'JOINT-CALLING',
     'GVCF',
     'CRAM',
     'CUSTOM',
-    'ES_INDEX',
+    'ES-INDEX',
     'SV',
-    'WEB_REPORT',
-    'ANALYSIS_RUNNER',
+    'WEB',
+    'ANALYSIS-RUNNER',
 ]
 
-EXCLUDED_SAMPLES = [
-    'CPG11783',  # acute-care, no FASTQ data
-    'CPG13409',  # perth-neuro, coverage ~0x
-    'CPG243717',  # validation, NA12878_KCCG low coverage https://main-web.populationgenomics.org.au/validation/qc/cram/multiqc.html,
-    'CPG246645',  # ag-hidden, eof issue  https://batch.hail.populationgenomics.org.au/batches/97645/jobs/440
-    'CPG246678',  # ag-hidden, diff fastq size  https://batch.hail.populationgenomics.org.au/batches/97645/jobs/446
-    'CPG261792',  # rdp-kidney misformated fastq - https://batch.hail.populationgenomics.org.au/batches/378736/jobs/43
-    # acute care fasq parsing errors https://batch.hail.populationgenomics.org.au/batches/379303/jobs/24
-    'CPG259150',
-    'CPG258814',
-    'CPG258137',
-    'CPG258111',
-    'CPG258012',
-    # ohmr4 cram parsing in align issues
-    'CPG261339',
-    'CPG261347',
-    # IBMDX truncated sample? https://batch.hail.populationgenomics.org.au/batches/422181/jobs/99
-    'CPG265876',
-]
-
-PARTICIPANTS_SAMPLES_SEQUENCES_QUERY = """
+QUERY_PARTICIPANTS_SAMPLES_SGS_ASSAYS = gql(
+    """
         query DatasetData($datasetName: String!) {
             project(name: $datasetName) {
                 participants {
                     externalId
                     id
                     samples {
                         id
                         externalId
-                        sequences {
+                        sequencingGroups {
                             id
-                            meta
                             type
+                            assays {
+                                id
+                                meta
+                            }
                         }
                     }
                 }
             }
         }
         """
+)
 
-SAMPLE_ANALYSIS_QUERY = """
-        query sampleCrams($sampleId: String!, $analysisType: AnalysisType!) {
-          sample(id: $sampleId) {
-            analyses(status: COMPLETED, type: $analysisType) {
+QUERY_SG_ANALYSES = gql(
+    """
+        query sgAnalyses($sgId: String!, $analysisType: String!) {
+          sequencingGroups(id: {eq: $sgId}) {
+            analyses(status: {eq: COMPLETED}, type: {eq: $analysisType}) {
               id
               meta
               output
               timestampCompleted
             }
           }
         }
 """
+)
 
 # Variable type definitions
-SequenceId = int
+AssayId = int
 SampleId = str
 SampleExternalId = str
 ParticipantExternalId = str
 
-SequenceReportEntry = namedtuple(
-    'SequenceReportEntry',
-    'sample_id sequence_id sequence_file_path analysis_ids filesize',
+AssayReportEntry = namedtuple(
+    'AssayReportEntry',
+    'sg_id assay_id assay_file_path analysis_ids filesize',
 )
 
 
 class GenericAuditor(AuditHelper):
     """Auditor for cloud storage buckets"""
 
     # pylint: disable=too-many-instance-attributes
@@ -103,547 +91,514 @@
 
         self.dataset = dataset
         self.sequencing_type = sequencing_type
         self.file_types = file_types
         self.default_analysis_type: str = default_analysis_type
         self.default_analysis_status: str = default_analysis_status
 
+        requests_logger.setLevel(logging.WARNING)
+
     def get_participant_data_for_dataset(self) -> list[dict]:
         """
         Uses a graphQL query to return all participants in a Metamist dataset.
         Nested in the return are all samples associated with the participants,
-        and then all the sequences associated with those samples.
+        and then all the assays associated with those samples.
         """
 
-        participant_data = query(   # pylint: disable=unsubscriptable-object
-            PARTICIPANTS_SAMPLES_SEQUENCES_QUERY, {'datasetName': self.dataset}
+        participant_data = query(  # pylint: disable=unsubscriptable-object
+            QUERY_PARTICIPANTS_SAMPLES_SGS_ASSAYS, {'datasetName': self.dataset}
         )['project']['participants']
 
-        # Filter out any participants with no samples and log any found
+        filtered_participants = []
         for participant in participant_data:
-            if not participant.get('samples'):
+            if not participant['samples']:
                 logging.info(
-                    f'{self.dataset} :: Filtering participant {participant.get("id")} ({participant.get("externalId")}) it has no samples.'
+                    f'{self.dataset} :: Filtering participant {participant["id"]} ({participant["externalId"]}) as it has no samples.'
                 )
-        participant_data = [
-            participant
-            for participant in participant_data
-            if participant.get('samples')
-        ]
+                continue
+            filtered_participants.append(participant)
 
-        return participant_data
+        return filtered_participants
 
+    # TODO
+    # Remove this method?
     @staticmethod
     def map_participants_to_samples(
         participants: list[dict],
     ) -> dict[ParticipantExternalId, list[SampleId]]:
         """
         Returns the {external_participant_id : sample_internal_id}
             mapping for a Metamist dataset
         - Also reports if any participants have more than one sample
         """
 
-        # Create mapping of participant external ID to sample ID
+        # Create mapping of participant external id to sample id
         participant_eid_sample_id_map = {
-            participant.get('externalId'): [
-                sample.get('id') for sample in participant.get('samples')
+            participant['externalId']: [
+                sample['id'] for sample in participant['samples']
             ]
             for participant in participants
         }
 
-        # Create mapping of participant external ID to internal ID
+        # Create mapping of participant external id to internal id
         participant_eid_to_iid = {
-            participant.get('externalId'): participant.get('id')
-            for participant in participants
+            participant['externalId']: participant['id'] for participant in participants
         }
 
-        # Report if any participants have more than one sample ID
+        # Report if any participants have more than one sample id
         for participant_eid, sample_ids in participant_eid_sample_id_map.items():
             if len(sample_ids) > 1:
                 logging.info(
                     f'Participant {participant_eid_to_iid[participant_eid]} '
-                    f'(external ID: {participant_eid}) associated with more than '
+                    f'(external id: {participant_eid}) associated with more than '
                     f'one sample id: {sample_ids}'
                 )
 
         return participant_eid_sample_id_map
 
     @staticmethod
     def map_internal_to_external_sample_ids(
         participants: list[dict],
     ) -> dict[SampleId, SampleExternalId]:
         """
-        Returns the {internal sample ID : external sample ID} mapping for all
-            participants in a Metamist dataset
-        Also removes any samples that are part of the exclusions list
-        """
-        # Create a list of dictionaries, each mapping a sample ID to its external ID
-        samples_all = [
-            {
-                sample.get('id'): sample.get('externalId')
-                for sample in participant['samples']
-            }
+        Returns the {internal sample id : external sample id} mapping for all participants in a Metamist dataset
+        """
+        return {
+            sample['id']: sample['externalId']
             for participant in participants
-        ]
-
-        # Squish them into a single dictionary not a list of dictionaries
-        sample_internal_external_id_map = {
-            sample_id: sample_external_id
-            for sample_map in samples_all
-            for sample_id, sample_external_id in sample_map.items()
-            if sample_id not in EXCLUDED_SAMPLES
+            for sample in participant['samples']
         }
 
-        return sample_internal_external_id_map
-
-    def get_sequence_map_from_participants(
+    def get_assay_map_from_participants(
         self, participants: list[dict]
-    ) -> tuple[dict[Any, Any], dict[Any, list[tuple[Any, Any]]]]:
+    ) -> tuple[dict[str, str], dict[int, str], dict[Any, list[tuple[Any, Any]]]]:
         """
-        Input the list of Metamist participant dictionaries from the master graphql Query
+        Input the list of Metamist participant dictionaries from the 'QUERY_PARTICIPANTS_SAMPLES_SGS_ASSAYS' query
 
-        Returns dictionary mappings:
-        {sequence_id : sample_internal_id}, and {sequence_id : (sequence_filepath, sequence_filesize)}
+        Returns the mappings:
+        1. { sg_id       : sample_id }
+        2. { assay_id       : sg_id }
+        3. { assay_id    : (read_filepath, read_filesize,) }
         """
-        all_sequences = [
-            {
-                sample.get('id'): sample.get('sequences')
-                for sample in participant.get('samples')
-            }
+
+        sg_sample_id_map = {}
+        assay_sg_id_map = {}
+        assay_filepaths_filesizes = defaultdict(list)
+
+        sample_sgs = {
+            sample['id']: sample['sequencingGroups']
             for participant in participants
-        ]
+            for sample in participant['samples']
+        }
+        for sample_id, sgs in sample_sgs.items():
+            for sg in sgs:
+                if not sg['type'].lower() in self.sequencing_type:
+                    continue
 
-        seq_id_sample_id_map = {}
-        # multiple reads per sequence is possible so use defaultdict(list)
-        sequence_filepaths_filesizes = defaultdict(list)
-        for sample_sequence in all_sequences:  # pylint: disable=R1702
-            sample_internal_id = list(sample_sequence.keys())[
-                0
-            ]  # Extract the sample ID
-            for sequences in sample_sequence.values():
-                for sequence in sequences:
-                    if not sequence.get('type').lower() in self.sequencing_type:
-                        continue
-                    meta = sequence.get('meta')
-                    reads = meta.get('reads')
-                    seq_id_sample_id_map[sequence.get('id')] = sample_internal_id
+                sg_sample_id_map[sg['id']] = sample_id
+                for assay in sg['assays']:
+                    reads = assay['meta'].get('reads')
                     if not reads:
-                        logging.info(
-                            f'Sample {sample_internal_id} has no sequence reads'
-                        )
-                        continue
-                    # support up to three levels of nesting, because:
-                    #
-                    #   - reads is typically an array
-                    #       - handle the case where it's not an array
-                    #   - fastqs exist in pairs.
-                    # eg:
-                    #   - reads: cram   # this shouldn't happen, but handle it anyway
-                    #   - reads: [cram1, cram2]
-                    #   - reads: [[fq1_forward, fq1_back], [fq2_forward, fq2_back]]
-                    if isinstance(reads, dict):
-                        sequence_filepaths_filesizes[sequence.get('id')].append(
-                            (reads.get('location'), reads.get('size'))
+                        logging.warning(
+                            f'{self.dataset} :: SG {sg["id"]} assay {assay["id"]} has no reads field'
                         )
                         continue
-                    if not isinstance(reads, list):
-                        logging.error(f'Invalid read type: {type(reads)}: {reads}')
-                        continue
+
+                    assay_sg_id_map[assay['id']] = sg['id']
                     for read in reads:
-                        if isinstance(read, list):
-                            for inner_read in read:
-                                if not isinstance(inner_read, dict):
-                                    logging.error(
-                                        f'Got {type(inner_read)} read, expected dict: {inner_read}'
-                                    )
-                                    continue
-                                sequence_filepaths_filesizes[sequence.get('id')].append(
-                                    (inner_read.get('location'), inner_read.get('size'))
-                                )
-                        else:
-                            if not isinstance(read, dict):
-                                logging.error(
-                                    f'Got {type(read)} read, expected dict: {read}'
-                                )
-                                continue
-                            sequence_filepaths_filesizes[sequence.get('id')].append(
-                                (read.get('location'), read.get('size'))
+                        if not isinstance(read, dict):
+                            logging.error(
+                                f'{self.dataset} :: Got {type(read)} read for SG {sg["id"]}, expected dict: {read}'
                             )
+                            continue
 
-        return seq_id_sample_id_map, sequence_filepaths_filesizes
+                        assay_filepaths_filesizes[assay['id']].append(
+                            (
+                                read.get('location'),
+                                read.get('size'),
+                            )
+                        )
+
+        return sg_sample_id_map, assay_sg_id_map, assay_filepaths_filesizes
 
-    def get_analysis_cram_paths_for_dataset_samples(
+    def get_analysis_cram_paths_for_dataset_sgs(
         self,
-        sample_internal_to_external_id_map: dict[str, str],
+        assay_sg_id_map: dict[int, str],
     ) -> dict[str, dict[int, str]]:
         """
-        Queries all analyses for the list of samples in the given dataset AND the seqr dataset.
-        Returns a dict mapping {sample_id : (analysis_id, cram_path) }
+        Fetches all CRAMs for the list of sgs in the given dataset AND the seqr dataset.
+        Returns a dict mapping {sg_id : (analysis_id, cram_path) }
         """
-        sample_ids = list(sample_internal_to_external_id_map.keys())
+        sg_ids = list(assay_sg_id_map.values())
 
         analyses = []
-        for sample in sample_ids:
+        for sg_id in sg_ids:
             analyses.extend(
-                query(   # pylint: disable=unsubscriptable-object
-                    SAMPLE_ANALYSIS_QUERY, {'sampleId': sample, 'analysisType': 'CRAM'}
-                )['sample']['analyses']
+                [
+                    sg['analyses']
+                    for sg in query(  # pylint: disable=unsubscriptable-object
+                        QUERY_SG_ANALYSES, {'sgId': sg_id, 'analysisType': 'CRAM'}
+                    )['sequencingGroups']
+                ]
             )
-        # Report any crams missing the sequence type
+        analyses = [
+            analysis for analyses_list in analyses for analysis in analyses_list
+        ]
+        # Report any crams missing the sequencing type
         crams_with_missing_seq_type = [
-            analysis.get('id')
+            analysis['id']
             for analysis in analyses
             if 'sequencing_type' not in analysis['meta']
         ]
         if crams_with_missing_seq_type:
             raise ValueError(
-                f'CRAMs from dataset {self.dataset} did not have sequencing_type: {crams_with_missing_seq_type}'
+                f'{self.dataset} :: CRAM analyses are missing sequencing_type field: {crams_with_missing_seq_type}'
             )
 
-        # Filter the analyses based on input sequence type
+        # Filter the analyses based on input sequencing type
         analyses = [
             analysis
             for analysis in analyses
-            if analysis.get('meta')['sequencing_type'] in self.sequencing_type
+            if analysis['meta'].get('sequencing_type') in self.sequencing_type
         ]
 
-        # For each sample ID, collect the analysis IDs and cram paths
-        sample_cram_paths: dict[str, dict[int, str]] = defaultdict(dict)
+        # For each sg id, collect the analysis ids and cram paths
+        sg_cram_paths: dict[str, dict[int, str]] = defaultdict(dict)
         for analysis in analyses:
             # Check the analysis output path is a valid gs path to a .cram file
             if not analysis['output'].startswith('gs://') and analysis[
                 'output'
             ].endswith('cram'):
-                logging.info(
+                logging.warning(
                     f'Analysis {analysis["id"]} invalid output path: {analysis["output"]}'
                 )
                 continue
+
             try:
-                # Try getting the sample ID from the 'sample_ids' field
-                sample_id = analysis['sample_ids'][0]
-            except KeyError:
-                # Try getting the sample ID from the 'sample' meta field
-                sample_id = analysis.get('meta')['sample']
+                sg_id = self.get_sequencing_group_ids_from_analysis(analysis)[0]
+                sg_cram_paths[sg_id].update(
+                    [(analysis.get('id'), analysis.get('output'))]
+                )
+            except ValueError:
                 logging.warning(
-                    f'Analysis: {analysis.get("id")} missing "sample_ids" field. Using analysis["meta"].get("sample") instead.'
+                    f'Analysis {analysis["id"]} missing sample or sequencing group field.'
                 )
+                continue
 
-            sample_cram_paths[sample_id].update(
-                [(analysis.get('id'), analysis.get('output'))]
-            )
-
-        return sample_cram_paths
+        return sg_cram_paths
 
-    def analyses_for_samples_without_crams(self, samples_without_crams: list[str]):
+    def analyses_for_sgs_without_crams(self, sgs_without_crams: list[str]):
         """Checks if other completed analyses exist for samples without completed crams"""
 
-        all_sample_analyses: dict[str, list[dict[str, int | str]]] = defaultdict(
-            list
-        )
+        all_sg_analyses: dict[str, list[dict[str, int | str]]] = defaultdict(list)
 
         analyses = []
         for analysis_type in ANALYSIS_TYPES:
             if analysis_type == 'CRAM':
                 continue
-            for sample in samples_without_crams:
+            for sg in sgs_without_crams:
                 analyses.extend(
-                    query(  # pylint: disable=unsubscriptable-object
-                        SAMPLE_ANALYSIS_QUERY,
-                        {'sampleId': sample, 'analysisType': analysis_type},
-                    )['sample']['analyses']
+                    [
+                        sg['analyses']
+                        for sg in query(  # pylint: disable=unsubscriptable-object
+                            QUERY_SG_ANALYSES,
+                            {'sgId': sg, 'analysisType': analysis_type},
+                        )['sequencingGroups']
+                    ]
                 )
-
+        analyses = [
+            analysis for analyses_list in analyses for analysis in analyses_list
+        ]
         for analysis in analyses:
             try:
-                # Try getting the sample IDs from the 'sample_ids' field
-                samples = analysis['sample_ids']
-            except KeyError:
-                # Try getting the sample IDs from the 'sample' meta field
-                try:
-                    samples = analysis['meta']['sample']
-                # Try getting the sample ID from the 'samples' meta field
-                except KeyError:
-                    samples = analysis['meta']['samples']
-
-            if not isinstance(samples, list):
-                samples = [
-                    samples,
-                ]
+                sg_ids = self.get_sequencing_group_ids_from_analysis(analysis)
+            except ValueError:
+                logging.warning(
+                    f'Analysis {analysis["id"]} missing sample or sequencing group field.'
+                )
+                continue
 
-            for sample_id in samples:
-                if sample_id not in samples_without_crams:
+            for sg_id in sg_ids:
+                if sg_id not in sgs_without_crams:
                     continue
                 analysis_entry = {
-                    'analysis_id': analysis.get('id'),
-                    'analysis_type': analysis.get('type'),
-                    'analysis_output': analysis.get('output'),
-                    'timestamp_completed': analysis.get('timestampCompleted'),
+                    'analysis_id': analysis['id'],
+                    'analysis_type': analysis['type'],
+                    'analysis_output': analysis['output'],
+                    'timestamp_completed': analysis['timestampCompleted'],
                 }
-                all_sample_analyses[sample_id].append(analysis_entry)
+                all_sg_analyses[sg_id].append(analysis_entry)
 
-        if all_sample_analyses:
-            for sample_without_cram, completed_analyses in all_sample_analyses.items():
+        if all_sg_analyses:
+            for sg_without_cram, completed_analyses in all_sg_analyses.items():
                 for completed_analysis in completed_analyses:
                     logging.warning(
-                        f'{sample_without_cram} missing CRAM but has analysis {completed_analysis}'
+                        f'{self.dataset} :: SG {sg_without_cram} missing CRAM but has analysis {completed_analysis}'
                     )
 
-    def get_complete_and_incomplete_samples(
+    def get_complete_and_incomplete_sgs(
         self,
-        sample_internal_to_external_id_map: dict[str, str],
-        sample_cram_paths: dict[str, dict[int, str]],
+        assay_sg_id_map: dict[int, str],
+        sg_cram_paths: dict[str, dict[int, str]],
     ) -> dict[str, Any]:
         """
-        Returns a dictionary containing two categories of samples:
-         - the completed samples which have finished aligning and have a cram, as a dict mapping
-            the sample_id to the analysis IDs
-         - the incomplete samples where the alignment hasn't completed and no cram exists, as a list
+        Returns a dictionary containing two categories of sequencing groups:
+         - the completed sgs which have finished aligning and have a cram, as a dict mapping
+            the sg_id to the analysis_ids
+         - the incomplete sgs where the alignment hasn't completed and no cram exists, as a list
         """
         # Get all the unique cram paths to check
         cram_paths = set()
-        for analyses in sample_cram_paths.values():
+        for analyses in sg_cram_paths.values():
             cram_paths.update(list(analyses.values()))
 
         # Check the analysis paths actually point to crams that exist in the bucket
         buckets_subdirs = self.get_gcs_bucket_subdirs_to_search(list(cram_paths))
         crams_in_bucket = self.find_files_in_gcs_buckets_subdirs(
             buckets_subdirs,
             ('cram',),
         )
 
         # Incomplete samples initialised as the list of samples without a valid analysis cram output path
-        incomplete_samples = set(sample_internal_to_external_id_map.keys()).difference(
-            set(sample_cram_paths.keys())
+        incomplete_sgs = set(assay_sg_id_map.values()).difference(
+            set(sg_cram_paths.keys())
         )
 
-        # Completed samples are those whose completed cram output path exists in the bucket at the same path
-        completed_samples = defaultdict(list)
-        for sample_internal_id, analyses in sample_cram_paths.items():
+        # Completed sgs are those whose completed cram output path exists in the bucket at the same path
+        completed_sgs = defaultdict(list)
+        for sg_id, analyses in sg_cram_paths.items():
             for analysis_id, cram_path in analyses.items():
                 if cram_path in crams_in_bucket:
-                    completed_samples[sample_internal_id].append(analysis_id)
+                    completed_sgs[sg_id].append(analysis_id)
                     continue
-                incomplete_samples.update(sample_internal_id)
+                incomplete_sgs.update(sg_id)
 
-        if (
-            incomplete_samples
-        ):  # Report on samples without CRAMs especially if other analysis types have been created
-            logging.info(f'Samples without CRAMs found: {list(incomplete_samples)}')
-            self.analyses_for_samples_without_crams(list(incomplete_samples))
+        if incomplete_sgs:
+            logging.warning(
+                f'{self.dataset} :: {len(incomplete_sgs)} SGs without CRAMs found: {list(incomplete_sgs)}'
+            )
+            self.analyses_for_sgs_without_crams(list(incomplete_sgs))
 
-        return {'complete': completed_samples, 'incomplete': list(incomplete_samples)}
+        return {'complete': completed_sgs, 'incomplete': list(incomplete_sgs)}
 
-    async def check_for_uningested_or_moved_sequences(  # pylint: disable=R0914
+    async def check_for_uningested_or_moved_assays(  # pylint: disable=R0914
         self,
         bucket_name: str,
-        sequence_filepaths_filesizes: dict[int, list[tuple[str, int]]],
-        completed_samples: dict[str, list[int]],
-        seq_id_sample_id_map: dict[int, str],
-        sample_id_internal_external_map: dict[str, str],
+        assay_filepaths_filesizes: dict[int, list[tuple[str, int]]],
+        completed_sgs: dict[str, list[int]],
+        sg_sample_id_map: dict[str, str],
+        assay_sg_id_map: dict[int, str],
+        sample_internal_external_id_map: dict[str, str],
     ):
         """
-        Compares the sequences in a Metamist dataset to the sequences in the main-upload bucket
+        Compares the assays in a Metamist dataset to the assays in the main-upload bucket
 
-        Input: The dataset name, the {sequence_id : read_paths} mapping, the sequence file types,
-               and the sample internal -> external ID mapping.
-        Returns: 1. Paths to sequences that have not yet been ingested - checks if any completed
+        Input: The dataset name, the {assay_id : read_paths} mapping, the assay file types,
+               and the sample internal -> external id mapping.
+        Returns: 1. Paths to assays that have not yet been ingested - checks if any completed
                     sample external IDs are in the filename and includes this in output.
-                 2. A dict mapping sequence IDs to GS filepaths that have been ingested,
+                 2. A dict mapping assay IDs to GS filepaths that have been ingested,
                     but where the path in the bucket is different to the path for this
-                    sequence in Metamist. If the filenames and file sizes match,
-                    these are identified as sequence files that have been moved from
+                    assay in Metamist. If the filenames and file sizes match,
+                    these are identified as assay files that have been moved from
                     their original location to a new location.
                  3. The paths saved in metamist for the read data that has been moved. These paths go nowhere.
         """
-        # Get all the paths to sequence data anywhere in the main-upload bucket
-        sequence_paths_in_bucket = self.find_sequence_files_in_gcs_bucket(
+        # Get all the paths to assay data anywhere in the main-upload bucket
+        assay_paths_in_bucket = self.find_assay_files_in_gcs_bucket(
             bucket_name, self.file_types
         )
 
-        # Flatten all the Metamist sequence file paths and sizes into a single list
-        sequence_paths_sizes_in_metamist: list[tuple[str, int]] = []
-        for sequence in sequence_filepaths_filesizes.values():
-            sequence_paths_sizes_in_metamist.extend(sequence)
+        # Flatten all the Metamist assay file paths and sizes into a single list
+        assay_paths_sizes_in_metamist: list[tuple[str, int]] = []
+        for assay in assay_filepaths_filesizes.values():
+            assay_paths_sizes_in_metamist.extend(assay)
 
         # Find the paths that exist in the bucket and not in metamist
-        sequence_paths_in_metamist = [
-            path_size[0] for path_size in sequence_paths_sizes_in_metamist
+        assay_paths_in_metamist = [
+            path_size[0] for path_size in assay_paths_sizes_in_metamist
         ]
-        uningested_sequence_paths = set(sequence_paths_in_bucket).difference(
-            set(sequence_paths_in_metamist)
+        uningested_assay_paths = set(assay_paths_in_bucket).difference(
+            set(assay_paths_in_metamist)
         )
-        # These metamist paths lead nowhere so we can go ahead and ignore them
-        metamist_paths_to_nowhere = set(sequence_paths_in_metamist).difference(
-            set(sequence_paths_in_bucket)
+        # Find the paths that exist in metamist and not in the bucket
+        metamist_paths_to_nowhere = set(assay_paths_in_metamist).difference(
+            set(assay_paths_in_bucket)
         )
 
         # Strip the metamist paths into just filenames
         # Map each file name to its file size and path
-        metamist_sequence_file_size_map = {
+        metamist_assay_file_size_map = {
             os.path.basename(path_size[0]): path_size[1]
-            for path_size in sequence_paths_sizes_in_metamist
+            for path_size in assay_paths_sizes_in_metamist
         }
-        metamist_sequence_file_path_map = {
+        metamist_assay_file_path_map = {
             os.path.basename(path_size[0]): path_size[0]
-            for path_size in sequence_paths_sizes_in_metamist
+            for path_size in assay_paths_sizes_in_metamist
         }
 
-        # Identify if any paths are to files that have actually just been moved by checking if they are in the bucket but not metamist
+        # Identify if any paths are to files that have actually just been moved
+        # by checking if they are in the bucket but not metamist
         ingested_and_moved_filepaths = []
-        new_sequence_path_sizes = {}
-        for path in uningested_sequence_paths:
+        new_assay_path_sizes = {}
+        for path in uningested_assay_paths:
             filename = os.path.basename(path)
             # If the file in the bucket has the exact same name and size as one in metamist, assume its the same
-            if filename in metamist_sequence_file_size_map.keys():
+            if filename in metamist_assay_file_size_map.keys():
                 filesize = await self.file_size(path)
-                if filesize == metamist_sequence_file_size_map.get(filename):
+                if filesize == metamist_assay_file_size_map.get(filename):
                     ingested_and_moved_filepaths.append(
-                        (path, metamist_sequence_file_path_map.get(filename))
+                        (path, metamist_assay_file_path_map.get(filename))
                     )
-                    new_sequence_path_sizes[path] = filesize
+                    new_assay_path_sizes[path] = filesize
         logging.info(
             f'Found {len(ingested_and_moved_filepaths)} ingested files that have been moved'
         )
 
         # If the file has just been moved, we consider it ingested
-        uningested_sequence_paths -= {
+        uningested_assay_paths -= {
             bucket_path for bucket_path, _ in ingested_and_moved_filepaths
         }
 
-        # Check the list of uningested paths to see if any of them contain sample IDs for ingested samples
+        # Check the list of uningested paths to see if any of them contain sample ids for ingested samples
         # This could happen when we ingest a fastq read pair for a sample, and additional read files were provided
         # but not ingested, such as bams and vcfs.
-        uningested_reads: dict[str, list[tuple[str, str]]] = defaultdict(
-            list, {k: [] for k in uningested_sequence_paths}
+        uningested_reads: dict[str, list[tuple[str, str, str]]] = defaultdict(
+            list, {k: [] for k in uningested_assay_paths}
         )
-        for sample_id, analysis_ids in completed_samples.items():
+        for sg_id, analysis_ids in completed_sgs.items():
             try:
-                sample_ext_id = sample_id_internal_external_map[sample_id]
-                for uningested_sequence in uningested_sequence_paths:
-                    if sample_ext_id not in uningested_sequence:
+                sample_id = sg_sample_id_map[sg_id]
+                sample_ext_id = sample_internal_external_id_map[sample_id]
+                for uningested_assay in uningested_assay_paths:
+                    if sample_ext_id not in uningested_assay:
                         continue
-                    uningested_reads[uningested_sequence].append(
-                        (sample_id, sample_ext_id))
+                    uningested_reads[uningested_assay].append(
+                        (sg_id, sample_id, sample_ext_id)
+                    )
             except KeyError:
                 logging.warning(
-                    f'{sample_id} from analyses: {analysis_ids} not found in sample map.'
+                    f'{sg_id} from analyses: {analysis_ids} not found in SG-sample map.'
                 )
 
-        # flip the sequence id : reads mapping to identify sequence IDs by their read paths
-        reads_sequences = {}
-        for sequence_id, reads_sizes in sequence_filepaths_filesizes.items():
+        # flip the assay id : reads mapping to identify assays by their reads
+        reads_assays = {}
+        for assay_id, reads_sizes in assay_filepaths_filesizes.items():
             for read_size in reads_sizes:
-                reads_sequences[read_size[0]] = sequence_id
+                reads_assays[read_size[0]] = assay_id
 
-        # Collect the sequences for files that have been ingested and moved to a different bucket location
-        sequences_moved_paths = []
+        # Collect the assays for files that have been ingested and moved to a different bucket location
+        assays_moved_paths = []
         for bucket_path, metamist_path in ingested_and_moved_filepaths:
-            seq_id = reads_sequences.get(metamist_path)
-            sample_id = seq_id_sample_id_map.get(seq_id)
-            analysis_ids = completed_samples.get(sample_id)
-            if sample_id not in EXCLUDED_SAMPLES:
-                filesize = new_sequence_path_sizes[bucket_path]
-                sequences_moved_paths.append(
-                    SequenceReportEntry(
-                        sample_id=sample_id,
-                        sequence_id=seq_id,
-                        sequence_file_path=bucket_path,
+            assay_id = reads_assays.get(metamist_path)
+            sg_id = assay_sg_id_map.get(assay_id)
+            analysis_ids = completed_sgs.get(sg_id)
+            if sg_id not in AuditHelper.EXCLUDED_SGS and analysis_ids:
+                filesize = new_assay_path_sizes[bucket_path]
+                assays_moved_paths.append(
+                    AssayReportEntry(
+                        sg_id=sg_id,
+                        assay_id=assay_id,
+                        assay_file_path=bucket_path,
                         analysis_ids=analysis_ids,
                         filesize=filesize,
                     )
                 )
 
-        return uningested_reads, sequences_moved_paths, metamist_paths_to_nowhere
+        return uningested_reads, assays_moved_paths, metamist_paths_to_nowhere
 
     async def get_reads_to_delete_or_ingest(
         self,
         bucket_name: str,
-        completed_samples: dict[str, list[int]],
-        sequence_filepaths_filesizes: dict[int, list[tuple[str, int]]],
-        seq_id_sample_id_map: dict[int, str],
-        sample_id_internal_external_map: dict[str, str],
+        completed_sgs: dict[str, list[int]],
+        assay_filepaths_filesizes: dict[int, list[tuple[str, int]]],
+        sg_sample_id_map: dict[str, str],
+        assay_sg_id_map: dict[int, str],
+        sample_internal_external_id_map: dict[str, str],
     ) -> tuple[list, list]:
         """
         Inputs: 1. List of samples which have completed CRAMs
-                2. Dictionary mapping of sequence IDs to sequence file paths and file sizes
-                3. Dictionary mapping sample IDs to sequence IDs
-                4. Dictionary mapping sequence IDs to sample IDs
-        Returns a tuple of two lists, each containing sequences IDs and sequence file paths.
+                2. Dictionary mapping of assay IDs to assay file paths and file sizes
+                3. Dictionary mapping sample IDs to assay IDs
+                4. Dictionary mapping assay IDs to sample IDs
+        Returns a tuple of two lists, each containing assays IDs and assay file paths.
         The first containins reads which can be deleted, the second containing reads to ingest.
-        The sample ID, sequence ID, and analysis ID (of completed cram) are included in the delete list.
+        The sample id, assay id, and analysis id (of completed cram) are included in the delete list.
         """
-        # Check for uningested sequence data that may be hiding or sequence data that has been moved
+        # Check for uningested assay data that may be hiding or assay data that has been moved
         (
             reads_to_ingest,
-            moved_sequences_to_delete,
+            moved_assays_to_delete,
             metamist_paths_to_nowhere,
-        ) = await self.check_for_uningested_or_moved_sequences(
+        ) = await self.check_for_uningested_or_moved_assays(
             bucket_name,
-            sequence_filepaths_filesizes,
-            completed_samples,
-            seq_id_sample_id_map,
-            sample_id_internal_external_map,
+            assay_filepaths_filesizes,
+            completed_sgs,
+            sg_sample_id_map,
+            assay_sg_id_map,
+            sample_internal_external_id_map,
         )
 
-        # Create a mapping of sample ID: sequence ID - use defaultdict in case a sample has several sequences
-        sample_id_seq_id_map: dict[str, list[int]] = defaultdict(list)
-        for sequence, sample in seq_id_sample_id_map.items():
-            sample_id_seq_id_map[sample].append(sequence)
-
-        sequence_reads_to_delete = []
-        for sample_id, analysis_ids in completed_samples.items():
-            if sample_id in EXCLUDED_SAMPLES:
+        # Create a mapping of sg id: assay id - use defaultdict in case a sg has several assays
+        sg_assays_id_map: dict[str, list[int]] = defaultdict(list)
+        for assay_id, sg_id in assay_sg_id_map.items():
+            sg_assays_id_map[sg_id].append(assay_id)
+
+        assay_reads_to_delete = []
+        for sg_id, analysis_ids in completed_sgs.items():
+            if sg_id in AuditHelper.EXCLUDED_SGS:
                 continue
-            seq_ids = sample_id_seq_id_map[sample_id]
-            for seq_id in seq_ids:
-                seq_read_paths = sequence_filepaths_filesizes[seq_id]
-                for path, size in seq_read_paths:
+            assay_ids = sg_assays_id_map[sg_id]
+            for assay_id in assay_ids:
+                assay_read_paths = assay_filepaths_filesizes[assay_id]
+                for path, size in assay_read_paths:
                     if path in metamist_paths_to_nowhere:
                         continue
                     filesize = size
-                    sequence_reads_to_delete.append(
-                        SequenceReportEntry(
-                            sample_id=sample_id,
-                            sequence_id=seq_id,
-                            sequence_file_path=path,
+                    assay_reads_to_delete.append(
+                        AssayReportEntry(
+                            sg_id=sg_id,
+                            assay_id=assay_id,
+                            assay_file_path=path,
                             analysis_ids=analysis_ids,
                             filesize=filesize,
                         )
                     )
 
-        reads_to_delete = sequence_reads_to_delete + moved_sequences_to_delete
+        reads_to_delete = assay_reads_to_delete + moved_assays_to_delete
 
         return reads_to_delete, reads_to_ingest
 
     @staticmethod
     def find_crams_for_reads_to_ingest(
         reads_to_ingest: dict[str, list],
-        sample_cram_paths: dict[str, dict[int, str]],
-    ) -> list[tuple[str, str, str, int, str]]:
+        sg_cram_paths: dict[str, dict[int, str]],
+    ) -> list[tuple[str, str, str, str, int, str]]:
         """
         Compares the external sample IDs for samples with completed CRAMs against the
         uningested read files. This may turn up results for cases where multiple read types
         have been provided for a sample, but only one type was ingested and used for alignment.
         """
-        possible_sequence_ingests = []
-        for sequence_path, samples in reads_to_ingest.items():
-            if not samples:
+        possible_assay_ingests = []
+        for assay_path, sample_tuples in reads_to_ingest.items():
+            if not sample_tuples:
                 # If no samples detected in filename, add the path in an empty tuple
-                possible_sequence_ingests.append((sequence_path, '', '', 0, ''))
+                possible_assay_ingests.append((assay_path, '', '', '', 0, ''))
                 continue
-            for sample in samples:
-                # Else get the completed CRAM analysis ID and path for the sample
-                sample_internal_id, sample_ext_id = sample
-                sample_cram = sample_cram_paths[sample_internal_id]
-                analysis_id = int(list(sample_cram.keys())[0])
-                cram_path = sample_cram[analysis_id]
-                possible_sequence_ingests.append(
+            for sample_tuple in sample_tuples:
+                # Else get the completed CRAM analysis id and path for the sample
+                sg_id, sample_id, sample_external_id = sample_tuple
+                sg_cram = sg_cram_paths[sg_id]
+                analysis_id = int(list(sg_cram.keys())[0])
+                cram_path = sg_cram[analysis_id]
+                possible_assay_ingests.append(
                     (
-                        sequence_path,
-                        sample_ext_id,
-                        sample_internal_id,
+                        assay_path,
+                        sg_id,
+                        sample_id,
+                        sample_external_id,
                         analysis_id,
                         cram_path,
                     )
                 )
 
-        return possible_sequence_ingests
+        return possible_assay_ingests
```

### Comparing `metamist-6.0.6/metamist/graphql/__init__.py` & `metamist-6.1.0/metamist/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/metamist/graphql/schema.graphql` & `metamist-6.1.0/metamist/graphql/schema.graphql`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   dataset: String!
   meta: JSON!
   readGroupName: String
   writeGroupName: String
   pedigree(internalFamilyIds: [Int!] = null, replaceWithParticipantExternalIds: Boolean! = true, replaceWithFamilyExternalIds: Boolean! = true, includeParticipantsNotInFamilies: Boolean! = false, emptyParticipantValue: String = null): [JSON!]!
   families: [GraphQLFamily!]!
   participants: [GraphQLParticipant!]!
-  samples(type: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, meta: JSON = null): [GraphQLSample!]!
+  samples(type: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, id: StrGraphQLFilter = null, meta: JSON = null): [GraphQLSample!]!
   sequencingGroups(id: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
   analyses(type: StrGraphQLFilter = null, status: AnalysisStatusGraphQLFilter = null, active: BoolGraphQLFilter = null, meta: JSON = null): [GraphQLAnalysis!]!
 }
 
 type GraphQLSample {
   id: String!
   externalId: String!
```

### Comparing `metamist-6.0.6/metamist/parser/cloudhelper.py` & `metamist-6.1.0/metamist/parser/cloudhelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,18 @@
 
         blob = storage.Blob.from_string(filename, client=self.gcs_client)
 
         if not blob.exists():
             # maintain existing behaviour
             return None
 
+        if not blob.time_created:
+            # GCP blobs sometimes need a reload
+            blob.reload()
+
         return blob
 
     def _list_gcs_directory(self, gcs_path) -> list[str]:
         path = GSPath(gcs_path)
         if path.parts[2:]:
             remaining_path = '/'.join(path.parts[2:]) + '/'  # has to end with "/"
         else:
```

### Comparing `metamist-6.0.6/metamist/parser/generic_metadata_parser.py` & `metamist-6.1.0/metamist/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/metamist/parser/generic_parser.py` & `metamist-6.1.0/metamist/parser/generic_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 
         self.samples: list[ParsedSample] = []
 
     def to_sm(self) -> ParticipantUpsert:
         """Convert to SM upsert model"""
         samples = [s.to_sm() for s in self.samples]
         return ParticipantUpsert(
+            id=self.internal_pid,
             external_id=self.external_pid,
             reported_sex=self.reported_sex,
             reported_gender=self.reported_gender,
             karyotype=self.karyotype,
             meta=self.meta,
             samples=samples,
         )
```

### Comparing `metamist-6.0.6/metamist/parser/sample_file_map_parser.py` & `metamist-6.1.0/metamist/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/metamist.egg-info/PKG-INFO` & `metamist-6.1.0/metamist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.6
+Version: 6.1.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.6/setup.py` & `metamist-6.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='6.0.6',
+    version='6.1.0',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `metamist-6.0.6/test/test_analysis.py` & `metamist-6.1.0/test/test_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,36 +74,55 @@
                 ],
             )
         )
         self.sample_id = sample.id
         self.genome_sequencing_group_id = sample.sequencing_groups[0].id
         self.exome_sequencing_group_id = sample.sequencing_groups[self.project_id].id
 
-        await self.al.create_analysis(
+    @run_as_sync
+    async def test_get_analysis_by_id(self):
+        """
+        Test getting an analysis by id
+        """
+        analysis_id = await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[self.genome_sequencing_group_id],
                 meta={'sequencing_type': 'genome', 'size': 1024},
             )
         )
 
+        analysis = await self.al.get_analysis_by_id(analysis_id)
+        self.assertEqual(analysis_id, analysis.id)
+        self.assertEqual('cram', analysis.type)
+        self.assertEqual(AnalysisStatus.COMPLETED, analysis.status)
+
     @run_as_sync
     async def test_add_cram(self):
         """
         Test adding an analysis of type CRAM
         """
 
+        analysis_id = await self.al.create_analysis(
+            AnalysisInternal(
+                type='cram',
+                status=AnalysisStatus.COMPLETED,
+                sequencing_group_ids=[self.genome_sequencing_group_id],
+                meta={'sequencing_type': 'genome', 'size': 1024},
+            )
+        )
+
         analyses = await self.connection.connection.fetch_all('SELECT * FROM analysis')
         analysis_sgs = await self.connection.connection.fetch_all(
             'SELECT * FROM analysis_sequencing_group'
         )
 
         self.assertEqual(1, len(analyses))
-
+        self.assertEqual(analysis_id, analyses[0]['id'])
         self.assertEqual(1, analysis_sgs[0]['sequencing_group_id'])
         self.assertEqual(analyses[0]['id'], analysis_sgs[0]['analysis_id'])
 
     @run_as_sync
     async def test_get_analysis(self):
         """
         Test adding an analysis of type ANALYSIS_RUNNER
@@ -145,15 +164,27 @@
     async def test_get_sequencing_group_file_sizes_single(self):
         """
         Test retrieval of sample file sizes over time
         """
 
         today = datetime.utcnow().date()
 
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
+        # insert analysis
+        await self.al.create_analysis(
+            AnalysisInternal(
+                type='cram',
+                status=AnalysisStatus.COMPLETED,
+                sequencing_group_ids=[self.genome_sequencing_group_id],
+                meta={'sequencing_type': 'genome', 'size': 1024},
+            )
+        )
+
+        result = await self.al.get_sequencing_group_file_sizes(
+            project_ids=[self.project_id]
+        )
         expected = {
             'project': self.project_id,
             'sequencing_groups': {
                 self.genome_sequencing_group_id: [
                     {
                         'start': today,
                         'end': None,
@@ -171,14 +202,24 @@
     async def test_get_sequencing_group_file_sizes_single_sample_double_sg(self):
         """
         Test getting file sizes for sequencing groups
             1 sample, w/ 2 sequencing groups
         """
         today = datetime.utcnow().date()
 
+        # Add genome cram
+        await self.al.create_analysis(
+            AnalysisInternal(
+                type='cram',
+                status=AnalysisStatus.COMPLETED,
+                sequencing_group_ids=[self.genome_sequencing_group_id],
+                meta={'sequencing_type': 'genome', 'size': 1024},
+            )
+        )
+
         # Add exome cram
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[self.exome_sequencing_group_id],
                 meta={'sequencing_type': 'exome', 'size': 3141},
@@ -201,15 +242,17 @@
                         'size': 3141,
                     }
                 ],
             },
         }
 
         # Assert that the exome size was added correctly
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
+        result = await self.al.get_sequencing_group_file_sizes(
+            project_ids=[self.project_id]
+        )
         self.assertDictEqual(expected, result[0])
 
     @run_as_sync
     async def test_get_sequencing_group_file_sizes_exclusive_date_range(self):
         """
         Exclusive date range returning no data
         """
@@ -227,14 +270,24 @@
     @run_as_sync
     async def test_get_sequencing_group_file_sizes_newer_sample(self):
         """
         Update analysis for sequencing group, making sure we only return the later one
         """
         today = datetime.utcnow().date()
 
+        # Add genome cram that's older
+        await self.al.create_analysis(
+            AnalysisInternal(
+                type='cram',
+                status=AnalysisStatus.COMPLETED,
+                sequencing_group_ids=[self.genome_sequencing_group_id],
+                meta={'sequencing_type': 'genome', 'size': 1024},
+            )
+        )
+
         # Add another genome cram that's newer
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[self.genome_sequencing_group_id],
                 meta={'sequencing_type': 'genome', 'size': 11111},
@@ -249,15 +302,17 @@
                         'end': None,
                         'size': 11111,
                     }
                 ]
             },
         }
 
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
+        result = await self.al.get_sequencing_group_file_sizes(
+            project_ids=[self.project_id]
+        )
         self.assertDictEqual(expected, result[0])
 
     @run_as_sync
     async def test_get_sequencing_group_file_sizes_two_samples(self):
         """Test that it works for two samples"""
         today = datetime.utcnow().date()
 
@@ -285,14 +340,24 @@
                                 },
                             )
                         ],
                     )
                 ],
             )
         )
+        # add for sg 1
+        await self.al.create_analysis(
+            AnalysisInternal(
+                type='cram',
+                status=AnalysisStatus.COMPLETED,
+                sequencing_group_ids=[self.genome_sequencing_group_id],
+                meta={'sequencing_type': 'genome', 'size': 1024},
+            )
+        )
+
         sequencing_group_2_id = sample_2.sequencing_groups[0].id
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[sequencing_group_2_id],
                 meta={'sequencing_type': 'genome', 'size': 987654321},
@@ -315,9 +380,11 @@
                         'end': None,
                         'size': 987654321,
                     }
                 ],
             },
         }
 
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
+        result = await self.al.get_sequencing_group_file_sizes(
+            project_ids=[self.project_id]
+        )
         self.assertDictEqual(expected, result[0])
```

### Comparing `metamist-6.0.6/test/test_assay.py` & `metamist-6.1.0/test/test_assay.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_generate_data.py` & `metamist-6.1.0/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_generic_auditor.py` & `metamist-6.1.0/test/test_generic_auditor.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,483 +18,619 @@
         )
         mock_query.return_value = {
             'project': {
                 'dataset': 'test',
                 'participants': [
                     {
                         'id': 1,
-                        'samples': [{'id': 'CPG123', 'sequences': [{'id': 1}]}],
+                        'externalId': 'P01',
+                        'samples': [
+                            {
+                                'id': 'XPG123',
+                                'sequencingGroups': [
+                                    {'id': 'CPG123', 'assays': [{'id': 1}]}
+                                ],
+                            }
+                        ],
                     },
                     {
                         'id': 2,
+                        'externalId': 'P02',
                         'samples': [
-                            {'id': 'CPG456', 'sequences': [{'id': 2}, {'id': 3}]}
+                            {
+                                'id': 'XPG456',
+                                'sequencingGroups': [
+                                    {'id': 'CPG456', 'assays': [{'id': 2}, {'id': 3}]}
+                                ],
+                            }
                         ],
                     },
-                    {'id': 3, 'samples': []},
+                    {'id': 3, 'externalId': 'P01', 'samples': []},
                 ],
             }
         }
 
         expected_participants = [
             {
                 'id': 1,
-                'samples': [{'id': 'CPG123', 'sequences': [{'id': 1}]}],
+                'externalId': 'P01',
+                'samples': [
+                    {
+                        'id': 'XPG123',
+                        'sequencingGroups': [{'id': 'CPG123', 'assays': [{'id': 1}]}],
+                    }
+                ],
             },
             {
                 'id': 2,
-                'samples': [{'id': 'CPG456', 'sequences': [{'id': 2}, {'id': 3}]}],
+                'externalId': 'P02',
+                'samples': [
+                    {
+                        'id': 'XPG456',
+                        'sequencingGroups': [
+                            {'id': 'CPG456', 'assays': [{'id': 2}, {'id': 3}]}
+                        ],
+                    }
+                ],
             },
         ]
 
         participant_data = auditor.get_participant_data_for_dataset()
 
         self.assertListEqual(expected_participants, participant_data)
 
-    def test_get_genome_sequence_mapping(self):
+    def test_get_assay_map_from_participants_genome(self):
         """Only genome sequences should be mapped to the sample ID"""
         auditor = GenericAuditor(
             dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
         )
         participants = [
             {
                 'externalId': 'EX01',
                 'id': 1,
                 'samples': [
                     {
-                        'id': 'CPG123',
+                        'id': 'XPG123',
                         'externalId': 'EX01',
-                        'sequences': [
+                        'sequencingGroups': [
                             {
-                                'id': 1,
+                                'id': 'CPG123',
                                 'type': 'genome',
-                                'meta': {
-                                    'reads': {
-                                        'location': 'gs://cpg-dataset-main-upload/read.fq',
-                                        'size': 12,
+                                'assays': [
+                                    {
+                                        'id': 1,
+                                        'meta': {
+                                            'reads': [
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/read.fq',
+                                                    'size': 11,
+                                                }
+                                            ]
+                                        },
+                                    },
+                                    {
+                                        'id': 2,
+                                        'meta': {
+                                            'reads': [
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/R1.fq',
+                                                    'size': 12,
+                                                },
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/R2.fq',
+                                                    'size': 13,
+                                                },
+                                            ]
+                                        },
+                                    },
+                                    {
+                                        'id': 3,
+                                        'meta': {
+                                            'reads': [{'location': 'test', 'size': 0}]
+                                        },
+                                    },
+                                ],
+                            },
+                            {
+                                'id': 'CPG456',
+                                'type': 'exome',
+                                'assays': [
+                                    {
+                                        'id': 4,
+                                        'meta': {
+                                            'reads': [
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/exome/read.fq',
+                                                    'size': 14,
+                                                }
+                                            ]
+                                        },
                                     }
-                                },
+                                ],
                             },
+                        ],
+                    },
+                ],
+            }
+        ]
+
+        (
+            sg_sample_id_map,
+            assay_sg_id_map,
+            assay_paths_sizes,
+        ) = auditor.get_assay_map_from_participants(participants)
+
+        expected_sg_sample_mapping = {'CPG123': 'XPG123'}
+        expected_assay_sg_mapping = {1: 'CPG123', 2: 'CPG123', 3: 'CPG123'}
+        expected_read_sizes = {
+            1: [
+                ('gs://cpg-dataset-main-upload/read.fq', 11),
+            ],
+            2: [
+                ('gs://cpg-dataset-main-upload/R1.fq', 12),
+                ('gs://cpg-dataset-main-upload/R2.fq', 13),
+            ],
+            3: [
+                ('test', 0),
+            ],
+        }
+
+        self.assertDictEqual(sg_sample_id_map, expected_sg_sample_mapping)
+        self.assertDictEqual(assay_sg_id_map, expected_assay_sg_mapping)
+        self.assertDictEqual(assay_paths_sizes, expected_read_sizes)
+
+    def test_get_assay_map_from_participants_all(self):
+        """Both genome and exome sequences should be mapped to the sample IDs"""
+        auditor = GenericAuditor(
+            dataset='dev', sequencing_type=['genome', 'exome'], file_types=('fastq',)
+        )
+        participants = [
+            {
+                'externalId': 'EX01',
+                'id': 1,
+                'samples': [
+                    {
+                        'id': 'XPG123',
+                        'externalId': 'EX01',
+                        'sequencingGroups': [
                             {
-                                'id': 2,
+                                'id': 'CPG123',
                                 'type': 'genome',
-                                'meta': {
-                                    'reads': [
-                                        {
-                                            'location': 'gs://cpg-dataset-main-upload/R1.fq',
-                                            'size': 12,
+                                'assays': [
+                                    {
+                                        'id': 1,
+                                        'meta': {
+                                            'reads': [
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/read.fq',
+                                                    'size': 11,
+                                                }
+                                            ]
                                         },
-                                        {
-                                            'location': 'gs://cpg-dataset-main-upload/R2.fq',
-                                            'size': 13,
+                                    },
+                                    {
+                                        'id': 2,
+                                        'meta': {
+                                            'reads': [
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/R1.fq',
+                                                    'size': 12,
+                                                },
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/R2.fq',
+                                                    'size': 13,
+                                                },
+                                            ]
                                         },
-                                    ]
-                                },
+                                    },
+                                    {
+                                        'id': 3,
+                                        'meta': {
+                                            'reads': [{'location': 'test', 'size': 0}]
+                                        },
+                                    },
+                                ],
                             },
                             {
-                                'id': 3,
+                                'id': 'CPG456',
                                 'type': 'exome',
-                                'meta': {'reads': {'location': 'test', 'size': 0}},
+                                'assays': [
+                                    {
+                                        'id': 4,
+                                        'meta': {
+                                            'reads': [
+                                                {
+                                                    'location': 'gs://cpg-dataset-main-upload/exome/read.fq',
+                                                    'size': 14,
+                                                }
+                                            ]
+                                        },
+                                    }
+                                ],
                             },
                         ],
                     },
                 ],
-            },
+            }
         ]
-        seq_sample_id_map, seq_reads_sizes = auditor.get_sequence_map_from_participants(
-            participants
-        )
+        (
+            sg_sample_id_map,
+            assay_sg_id_map,
+            assay_paths_sizes,
+        ) = auditor.get_assay_map_from_participants(participants)
 
-        expected_mapping = {1: 'CPG123', 2: 'CPG123'}
+        expected_sg_sample_mapping = {'CPG123': 'XPG123', 'CPG456': 'XPG123'}
+        expected_assay_sg_mapping = {1: 'CPG123', 2: 'CPG123', 3: 'CPG123', 4: 'CPG456'}
         expected_read_sizes = {
             1: [
-                ('gs://cpg-dataset-main-upload/read.fq', 12),
+                ('gs://cpg-dataset-main-upload/read.fq', 11),
             ],
             2: [
                 ('gs://cpg-dataset-main-upload/R1.fq', 12),
                 ('gs://cpg-dataset-main-upload/R2.fq', 13),
             ],
+            3: [
+                ('test', 0),
+            ],
+            4: [
+                ('gs://cpg-dataset-main-upload/exome/read.fq', 14),
+            ],
         }
 
-        self.assertDictEqual(seq_sample_id_map, expected_mapping)
-        self.assertDictEqual(seq_reads_sizes, expected_read_sizes)
-
-    # def test_get_all_sequence_mapping_list_reads(self):
-    #     """Both genome and exome sequences should be mapped to the sample IDs"""
-    #     auditor = GenericAuditor(
-    #         dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
-    #     )
-    #     participants = [
-    #         {
-    #             'externalId': 'EX01',
-    #             'id': 1,
-    #             'samples': [
-    #                 {
-    #                     'id': 'CPG123',
-    #                     'externalId': 'EX01',
-    #                     'sequences': [
-    #                         {
-    #                             'id': 1,
-    #                             'type': 'genome',
-    #                             'meta': {
-    #                                 'reads': [
-    #                                     {
-    #                                         'location': 'gs://cpg-dataset-main-upload/R1.fq',
-    #                                         'size': 12,
-    #                                     },
-    #                                     {
-    #                                         'location': 'gs://cpg-dataset-main-upload/R2.fq',
-    #                                         'size': 13,
-    #                                     },
-    #                                 ]
-    #                             },
-    #                         },
-    #                     ],
-    #                 },
-    #             ],
-    #         },
-    #         {
-    #             'externalId': 'EX02',
-    #             'id': 2,
-    #             'samples': [
-    #                 {
-    #                     'id': 'CPG456',
-    #                     'externalId': 'EX02',
-    #                     'sequences': [
-    #                         {
-    #                             'id': 2,
-    #                             'type': 'exome',
-    #                             'meta': {
-    #                                 'reads': [
-    #                                     {
-    #                                         'location': 'gs://cpg-dataset-main-upload/exomes/R1.fq',
-    #                                         'size': 14,
-    #                                     },
-    #                                     {
-    #                                         'location': 'gs://cpg-dataset-main-upload/exomes/R2.fq',
-    #                                         'size': 15,
-    #                                     },
-    #                                 ]
-    #                             },
-    #                         },
-    #                     ],
-    #                 },
-    #             ],
-    #         },
-    #     ]
-    #     seq_sample_id_map, seq_reads_sizes = auditor.get_sequence_map_from_participants(
-    #         participants
-    #     )
-    #     expected_mapping = {1: 'CPG123', 2: 'CPG456'}
-    #     expected_read_sizes = {
-    #         1: [
-    #             ('gs://cpg-dataset-main-upload/R1.fq', 12),
-    #             ('gs://cpg-dataset-main-upload/R2.fq', 13),
-    #         ],
-    #         2: [
-    #             ('gs://cpg-dataset-main-upload/exomes/R1.fq', 14),
-    #             ('gs://cpg-dataset-main-upload/exomes/R2.fq', 15),
-    #         ],
-    #     }
-    #
-    #     self.assertDictEqual(seq_sample_id_map, expected_mapping)
-    #     self.assertDictEqual(seq_reads_sizes, expected_read_sizes)
+        self.assertDictEqual(sg_sample_id_map, expected_sg_sample_mapping)
+        self.assertDictEqual(assay_sg_id_map, expected_assay_sg_mapping)
+        self.assertDictEqual(assay_paths_sizes, expected_read_sizes)
 
-    def test_get_sequence_mapping_logging(self):
+    def test_get_sequence_mapping_error_logging(self):
         """If the sequence reads meta field maps to a raw string, logging.error triggers"""
         auditor = GenericAuditor(
             dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
         )
         participants = [
             {
                 'externalId': 'EX01',
                 'id': 1,
                 'samples': [
                     {
-                        'id': 'CPG123',
+                        'id': 'XPG123',
                         'externalId': 'EX01',
-                        'sequences': [
+                        'sequencingGroups': [
                             {
-                                'id': 1,
+                                'id': 'CPG123',
                                 'type': 'genome',
-                                'meta': {
-                                    'reads': 'gs://cpg-dataset-main-upload/read.cram'
-                                },
+                                'assays': [
+                                    {
+                                        'id': 1,
+                                        'meta': {
+                                            'reads': [
+                                                'gs://cpg-dataset-main-upload/read.fq',
+                                            ]
+                                        },
+                                    },
+                                ],
                             },
                         ],
                     },
                 ],
             },
         ]
         with self.assertLogs(level='ERROR') as log:
-            _, _ = auditor.get_sequence_map_from_participants(participants)
+            _, _, _ = auditor.get_assay_map_from_participants(participants)
             self.assertEqual(len(log.output), 1)
             self.assertEqual(len(log.records), 1)
             self.assertIn(
-                "Invalid read type: <class 'str'>: gs://cpg-dataset-main-upload/read.cram",
+                "ERROR:root:dev :: Got <class 'str'> read for SG CPG123, expected dict: gs://cpg-dataset-main-upload/read.fq",
+                log.output[0],
+            )
+
+    def test_get_sequence_mapping_warning_logging(self):
+        """If the sequence reads meta field is missing, logging.warning triggers"""
+        auditor = GenericAuditor(
+            dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
+        )
+        participants = [
+            {
+                'externalId': 'EX01',
+                'id': 1,
+                'samples': [
+                    {
+                        'id': 'XPG123',
+                        'externalId': 'EX01',
+                        'sequencingGroups': [
+                            {
+                                'id': 'CPG123',
+                                'type': 'genome',
+                                'assays': [
+                                    {
+                                        'id': 1,
+                                        'meta': {},
+                                    },
+                                ],
+                            },
+                        ],
+                    },
+                ],
+            },
+        ]
+        with self.assertLogs(level='WARNING') as log:
+            _, _, _ = auditor.get_assay_map_from_participants(participants)
+            self.assertEqual(len(log.output), 1)
+            self.assertEqual(len(log.records), 1)
+            self.assertIn(
+                'WARNING:root:dev :: SG CPG123 assay 1 has no reads field',
                 log.output[0],
             )
 
     @patch('metamist.audit.generic_auditor.query')
     def test_query_genome_analyses_crams(self, mock_query):
         """Test that only the genome analysis crams for a sample map dictionary are returned"""
         auditor = GenericAuditor(
             dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
         )
         mock_query.side_effect = [
             {
-                'sample': {
-                    'id': 'CPG123',
-                    'analyses': [
-                        {
-                            'id': 1,
-                            'meta': {
-                                'sequencing_type': 'genome',
+                'sequencingGroups': [
+                    {
+                        'id': 'CPG123',
+                        'type': 'genome',
+                        'analyses': [
+                            {
+                                'id': 1,
+                                'meta': {
+                                    'sequencing_type': 'genome',
+                                    'sample_ids': [
+                                        'CPG123',
+                                    ],
+                                },
+                                'output': 'gs://cpg-dataset-main/cram/CPG123.cram',
                             },
-                            'sample_ids': [
-                                'CPG123',
-                            ],
-                            'output': 'gs://cpg-dataset-main/cram/CPG123.cram',
-                        },
-                    ],
-                },
+                        ],
+                    },
+                    {
+                        'id': 'CPG456',
+                        'type': 'exome',
+                        'analyses': [
+                            {
+                                'id': 2,
+                                'meta': {
+                                    'sequencing_type': 'exome',
+                                    'sample_ids': [
+                                        'CPG456',
+                                    ],
+                                },
+                                'output': 'gs://cpg-dataset-main/exome/cram/CPG123.cram',
+                            },
+                        ],
+                    },
+                ]
+            }
+        ]
+
+        test_result = auditor.get_analysis_cram_paths_for_dataset_sgs(
+            assay_sg_id_map={1: 'CPG123'}
+        )
+        expected_result = {'CPG123': {1: 'gs://cpg-dataset-main/cram/CPG123.cram'}}
+
+        self.assertDictEqual(test_result, expected_result)
+
+    @patch('metamist.audit.generic_auditor.query')
+    def test_query_genome_and_exome_analyses_crams(self, mock_query):
+        """Test that both the genome and exome analysis crams for a sample map dictionary are returned"""
+        auditor = GenericAuditor(
+            dataset='dev', sequencing_type=['genome', 'exome'], file_types=('fastq',)
+        )
+        mock_query.side_effect = [
+            {
+                'sequencingGroups': [
+                    {
+                        'id': 'CPG123',
+                        'type': 'genome',
+                        'analyses': [
+                            {
+                                'id': 1,
+                                'meta': {
+                                    'sequencing_type': 'genome',
+                                    'sample_ids': [
+                                        'CPG123',
+                                    ],
+                                },
+                                'output': 'gs://cpg-dataset-main/cram/CPG123.cram',
+                            },
+                        ],
+                    }
+                ]
             },
             {
-                'sample': {
-                    'id': 'CPG456',
-                    'analyses': [
-                        {
-                            'id': 2,
-                            'meta': {
-                                'sequencing_type': 'exome',
+                'sequencingGroups': [
+                    {
+                        'id': 'CPG456',
+                        'type': 'exome',
+                        'analyses': [
+                            {
+                                'id': 2,
+                                'meta': {
+                                    'sequencing_type': 'exome',
+                                    'sample_ids': [
+                                        'CPG456',
+                                    ],
+                                },
+                                'output': 'gs://cpg-dataset-main/exome/cram/CPG123.cram',
                             },
-                            'sample_ids': [
-                                'CPG456',
-                            ],
-                            'output': 'gs://cpg-dataset-main/exome/cram/CPG123.cram',
-                        },
-                    ],
-                },
+                        ],
+                    },
+                ]
             },
         ]
 
-        test_result = auditor.get_analysis_cram_paths_for_dataset_samples(
-            sample_internal_to_external_id_map={'CPG123': 'EXT123'}
+        test_result = auditor.get_analysis_cram_paths_for_dataset_sgs(
+            assay_sg_id_map={1: 'CPG123', 2: 'CPG456'}
         )
 
-        expected_result = {'CPG123': {1: 'gs://cpg-dataset-main/cram/CPG123.cram'}}
+        expected_result = {
+            'CPG123': {1: 'gs://cpg-dataset-main/cram/CPG123.cram'},
+            'CPG456': {2: 'gs://cpg-dataset-main/exome/cram/CPG123.cram'},
+        }
 
         self.assertDictEqual(test_result, expected_result)
 
-    # @patch('metamist.audit.generic_auditor.query')
-    # def test_query_genome_and_exome_analyses_crams(self, mock_query):
-    #     """Test that both the genome and exome analysis crams for a sample map dictionary are returned"""
-    #     auditor = GenericAuditor(
-    #         dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
-    #     )
-    #     mock_query.side_effect = [
-    #         {
-    #             'sample': {
-    #                 'id': 'CPG123',
-    #                 'analyses': [
-    #                     {
-    #                         'id': 1,
-    #                         'meta': {
-    #                             'sequencing_type': 'genome',
-    #                         },
-    #                         'sample_ids': [
-    #                             'CPG123',
-    #                         ],
-    #                         'output': 'gs://cpg-dataset-main/cram/CPG123.cram',
-    #                     },
-    #                 ],
-    #             },
-    #         },
-    #         {
-    #             'sample': {
-    #                 'id': 'CPG456',
-    #                 'analyses': [
-    #                     {
-    #                         'id': 2,
-    #                         'meta': {
-    #                             'sequencing_type': 'exome',
-    #                         },
-    #                         'sample_ids': [
-    #                             'CPG456',
-    #                         ],
-    #                         'output': 'gs://cpg-dataset-main/exome/cram/CPG123.cram',
-    #                     },
-    #                 ],
-    #             },
-    #         },
-    #     ]
-    #
-    #     test_result = auditor.get_analysis_cram_paths_for_dataset_samples(
-    #         sample_internal_to_external_id_map={'CPG123': 'EXT123', 'CPG456': 'EXT456'}
-    #     )
-    #
-    #     expected_result = {
-    #         'CPG123': {1: 'gs://cpg-dataset-main/cram/CPG123.cram'},
-    #         'CPG456': {2: 'gs://cpg-dataset-main/exome/cram/CPG123.cram'},
-    #     }
-    #
-    #     self.assertDictEqual(test_result, expected_result)
-
     @patch('metamist.audit.generic_auditor.query')
     def test_query_broken_analyses_crams(self, mock_query):
         """
         All analysis crams must have 'sequencing_type' meta field,
         ValueError raised if not
         """
         auditor = GenericAuditor(
             dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
         )
         mock_query.return_value = {
-            'sample': {
-                'id': 'CPG123',
-                'analyses': [
-                    {
-                        'id': 1,
-                        'meta': {
-                            'sequence_type': 'genome',
+            'sequencingGroups': [
+                {
+                    'id': 'CPG123',
+                    'analyses': [
+                        {
+                            'id': 1,
+                            'meta': {
+                                'sequence_type': 'genome',
+                            },
+                            'sample_ids': [
+                                'CPG123',
+                            ],
+                            'output': '',
                         },
-                        'sample_ids': [
-                            'CPG123',
-                        ],
-                        'output': '',
-                    },
-                ],
-            },
+                    ],
+                },
+            ]
         }
 
         with self.assertRaises(ValueError):
-            auditor.get_analysis_cram_paths_for_dataset_samples(
-                sample_internal_to_external_id_map={'CPG123': 'EXT123'}
+            auditor.get_analysis_cram_paths_for_dataset_sgs(
+                assay_sg_id_map={1: 'CPG123'}
             )
 
     @patch('metamist.audit.generic_auditor.query')
     def test_query_analyses_crams_warning(self, mock_query):
         """Warn if the sample_ids field is absent and the sample meta field is used instead"""
         auditor = GenericAuditor(
             dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
         )
         mock_query.return_value = {
-            'sample': {
-                'id': 'CPG123',
-                'analyses': [
-                    {
-                        'id': 1,
-                        'meta': {
-                            'sequencing_type': 'genome',
-                            'sample': 'CPG123',
+            'sequencingGroups': [
+                {
+                    'id': 'CPG123',
+                    'analyses': [
+                        {
+                            'id': 1,
+                            'meta': {
+                                'sequencing_type': 'genome',
+                                'sampling_id': 'CPG123',
+                            },
+                            'output': 'gs://cpg-dataset-main/cram/CPG123.cram',
                         },
-                        'output': 'gs://cpg-dataset-main/cram/CPG123.cram',
-                    },
-                ],
-            }
+                    ],
+                }
+            ]
         }
 
         with self.assertLogs(level='WARNING') as log:
-            test_result = auditor.get_analysis_cram_paths_for_dataset_samples(
-                sample_internal_to_external_id_map={'CPG123': 'EXT123'}
+            _ = auditor.get_analysis_cram_paths_for_dataset_sgs(
+                assay_sg_id_map={1: 'CPG123'}
             )
             self.assertEqual(len(log.output), 1)
             self.assertEqual(len(log.records), 1)
             self.assertIn(
-                'Analysis: 1 missing "sample_ids" field. Using analysis["meta"].get("sample") instead.',
+                'WARNING:root:Analysis 1 missing sample or sequencing group field.',
                 log.output[0],
             )
 
-        expected_result = {'CPG123': {1: 'gs://cpg-dataset-main/cram/CPG123.cram'}}
-
-        self.assertDictEqual(test_result, expected_result)
-
     @patch('metamist.audit.generic_auditor.query')
-    def test_analyses_for_samples_without_crams(self, mock_query):
+    def test_analyses_for_sgs_without_crams(self, mock_query):
         """Log any analyses found for samples without completed CRAMs"""
         auditor = GenericAuditor(
             dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
         )
-        samples_without_crams = [  # noqa: B006
+        sgs_without_crams = [  # noqa: B006
             'CPG123',
         ]
 
         mock_query.return_value = {
-            'sample': {
-                'id': 'CPG123',
-                'analyses': [
-                    {
-                        'id': 1,
-                        'meta': {'sequencing_type': 'genome', 'sample': 'CPG123'},
-                        'output': 'gs://cpg-dataset-main/gvcf/CPG123.g.vcf.gz',
-                        'type': 'gvcf',
-                        'timestampCompleted': '2023-05-11T16:33:00',
-                    }
-                ],
-            }
+            'sequencingGroups': [
+                {
+                    'id': 'CPG123',
+                    'analyses': [
+                        {
+                            'id': 1,
+                            'meta': {'sequencing_type': 'genome', 'sample': 'CPG123'},
+                            'output': 'gs://cpg-dataset-main/gvcf/CPG123.g.vcf.gz',
+                            'type': 'gvcf',
+                            'timestampCompleted': '2023-05-11T16:33:00',
+                        }
+                    ],
+                }
+            ]
         }
 
         with self.assertLogs(level='WARNING') as log:
-            _ = auditor.analyses_for_samples_without_crams(samples_without_crams)
+            _ = auditor.analyses_for_sgs_without_crams(sgs_without_crams)
             self.assertEqual(len(log.output), 8)  # 8 analysis types checked
             self.assertEqual(len(log.records), 8)
             self.assertIn(
-                "WARNING:root:CPG123 missing CRAM but has analysis {'analysis_id': 1, 'analysis_type': 'gvcf', 'analysis_output': 'gs://cpg-dataset-main/gvcf/CPG123.g.vcf.gz', 'timestamp_completed': '2023-05-11T16:33:00'}",
-                log.output[6],
+                "WARNING:root:dev :: SG CPG123 missing CRAM but has analysis {'analysis_id': 1, 'analysis_type': 'gvcf', 'analysis_output': 'gs://cpg-dataset-main/gvcf/CPG123.g.vcf.gz', 'timestamp_completed': '2023-05-11T16:33:00'}",
+                log.output[0],
             )
 
-    def test_get_complete_and_incomplete_samples(self):
+    def test_get_complete_and_incomplete_sgs(self):
         """Report on samples that have completed CRAMs and those that dont"""
-        sample_map = {  # noqa: B006
-            'CPG123': 'EXT123',
-            'CPG456': 'EXT456',
-            'CPG789': 'EXT789',
+        assay_sg_id_map = {  # noqa: B006
+            1: 'CPG123',
+            2: 'CPG456',
+            3: 'CPG789',
         }
-        sample_cram_paths = {  # noqa: B006
+        sg_cram_paths = {  # noqa: B006
             'CPG123': {1: 'gs://cpg-dataset-main/cram/CPG123.cram'},
             'CPG456': {2: 'gs://cpg-dataset-main/exome/cram/CPG456.cram'},
         }
         auditor = GenericAuditor(
-            dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
+            dataset='dev', sequencing_type=['genome', 'exome'], file_types=('fastq',)
         )
         auditor.get_gcs_bucket_subdirs_to_search = MagicMock()
         auditor.find_files_in_gcs_buckets_subdirs = MagicMock()
-        auditor.analyses_for_samples_without_crams = MagicMock()
+        auditor.analyses_for_sgs_without_crams = MagicMock()
 
         auditor.get_gcs_bucket_subdirs_to_search.return_value = {
             'cpg-dataset-main': ['cram', 'exome/cram']
         }
         auditor.find_files_in_gcs_buckets_subdirs.return_value = [
             'gs://cpg-dataset-main/cram/CPG123.cram',
             'gs://cpg-dataset-main/exome/cram/CPG456.cram',
         ]
 
-        result = auditor.get_complete_and_incomplete_samples(
-            sample_internal_to_external_id_map=sample_map,
-            sample_cram_paths=sample_cram_paths,
+        result = auditor.get_complete_and_incomplete_sgs(
+            assay_sg_id_map=assay_sg_id_map,
+            sg_cram_paths=sg_cram_paths,
         )
 
         expected_result = {
             'complete': {'CPG123': [1], 'CPG456': [2]},
             'incomplete': ['CPG789'],
         }
 
         self.assertDictEqual(result, expected_result)
 
-    async def test_check_for_uningested_or_moved_sequences(self):
+    async def test_check_for_uningested_or_moved_assays(self):
         """Test 2 ingested reads, one ingested and moved read, and one uningested read"""
         auditor = GenericAuditor(
             dataset='dev', sequencing_type=['genome'], file_types=('fastq',)
         )
-        seq_reads_sizes = {  # noqa: B006
+        assay_reads_sizes = {  # noqa: B006
             1: [('read1.fq', 10), ('read2.fq', 11), ('dir1/read3.fq', 12)]
         }
-        completed_samples = {'CPG123': [1]}
-        seq_sample_map = {1: 'CPG123'}
-        sample_id_internal_external_map = {'CPG123': 'EXT123'}
+        completed_sgs = {'CPG123': [1]}
+        sg_sample_id_map = {'CPG123': 'EXT123'}
+        assay_sg_id_map = {1: 'CPG123'}
+        sample_internal_external_id_map = {'CPG123': 'EXT123'}
         auditor.find_sequence_files_in_gcs_bucket = MagicMock()
         auditor.find_sequence_files_in_gcs_bucket.return_value = [
             'read1.fq',
             'read2.fq',
             'dir2/read3.fq',
             'read4.fq',
         ]
@@ -502,35 +638,37 @@
         auditor.file_size = MagicMock()
         auditor.file_size.return_value = 12
 
         (
             uningested_sequence_paths,
             sequences_moved_paths,
             _,
-        ) = await auditor.check_for_uningested_or_moved_sequences(
+        ) = await auditor.check_for_uningested_or_moved_assays(
             bucket_name='gs://cpg-test-upload',
-            sequence_filepaths_filesizes=seq_reads_sizes,
-            completed_samples=completed_samples,
-            seq_id_sample_id_map=seq_sample_map,
-            sample_id_internal_external_map=sample_id_internal_external_map,
+            assay_filepaths_filesizes=assay_reads_sizes,
+            completed_sgs=completed_sgs,
+            sg_sample_id_map=sg_sample_id_map,
+            assay_sg_id_map=assay_sg_id_map,
+            sample_internal_external_id_map=sample_internal_external_id_map,
         )
 
-        SequenceReportEntry = namedtuple(
-            'sequence_report_entry',
-            'sample_id sequence_id sequence_file_path analysis_ids',
+        AssayReportEntry = namedtuple(
+            'AssayReportEntry',
+            'sg_id assay_id assay_file_path analysis_ids filesize',
         )
         self.assertEqual(uningested_sequence_paths, {'read4.fq'})
         self.assertEqual(
             sequences_moved_paths,
             [
-                SequenceReportEntry(
-                    sample_id='CPG123',
-                    sequence_id=1,
-                    sequence_file_path='dir2/read3.fq',
+                AssayReportEntry(
+                    sg_id='CPG123',
+                    assay_id=1,
+                    assay_file_path='dir2/read3.fq',
                     analysis_ids=[1],
+                    filesize=12,
                 ),
             ],
         )
 
     def test_get_gcs_bucket_subdirs_to_search(self):
         """
         Takes a list of paths and extracts the bucket name and subdirectory, returning all unique pairs
```

### Comparing `metamist-6.0.6/test/test_generic_filters.py` & `metamist-6.1.0/test/test_generic_filters.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_get_participants.py` & `metamist-6.1.0/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_graphql.py` & `metamist-6.1.0/test/test_graphql.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_import_individual_metadata.py` & `metamist-6.1.0/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_metamist.py` & `metamist-6.1.0/test/test_metamist.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_models.py` & `metamist-6.1.0/test/test_models.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_parse_existing_cohort.py` & `metamist-6.1.0/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_parse_file_map.py` & `metamist-6.1.0/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_parse_generic_metadata.py` & `metamist-6.1.0/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_parse_ont_processor.py` & `metamist-6.1.0/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_parse_ont_sheet.py` & `metamist-6.1.0/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_pedigree.py` & `metamist-6.1.0/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_sample.py` & `metamist-6.1.0/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_search.py` & `metamist-6.1.0/test/test_search.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_sequencing_groups.py` & `metamist-6.1.0/test/test_sequencing_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_update_participant_family.py` & `metamist-6.1.0/test/test_update_participant_family.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_upsert.py` & `metamist-6.1.0/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/test_web.py` & `metamist-6.1.0/test/test_web.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.6/test/testbase.py` & `metamist-6.1.0/test/testbase.py`

 * *Files identical despite different names*

