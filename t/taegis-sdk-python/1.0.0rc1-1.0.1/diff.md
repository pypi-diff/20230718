# Comparing `tmp/taegis-sdk-python-1.0.0rc1.tar.gz` & `tmp/taegis-sdk-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.0rc1.tar", last modified: Mon Jun 26 14:41:11 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.1.tar", last modified: Tue Jul 18 14:15:37 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.0rc1.tar` & `taegis-sdk-python-1.0.1.tar`

### file list

```diff
@@ -1,202 +1,208 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.840248 taegis-sdk-python-1.0.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6231 2023-06-26 14:41:11.840248 taegis-sdk-python-1.0.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5793 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:41:11.840248 taegis-sdk-python-1.0.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.808248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8618 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10895 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.810248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    13384 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.811248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.812248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.813248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78106 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.814248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6375 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14954 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.815248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12807 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25755 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.816248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.817248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.818248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15823 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    22760 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    30929 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.819248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.820248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.821248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7325 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8546 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.822248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7674 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.823248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.824248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.825248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9191 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.826248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12999 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10457 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24248 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.827248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    28008 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37546 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.828248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12204 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7214 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    41182 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.829248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9291 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.830248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.831248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6858 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.832248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5923 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5961 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12949 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.833248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6660 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13046 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.834248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14207 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16097 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.835248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.836248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11617 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5913 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31658 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.837248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3443 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13781 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.838248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7993 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.839248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11558 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7075 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25732 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     6493 2023-06-26 14:38:42.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:41:11.810248 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6231 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7969 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 14:41:11.000000 taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.667305 taegis-sdk-python-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-07-18 14:15:37.666305 taegis-sdk-python-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5793 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 14:15:37.667305 taegis-sdk-python-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.637305 taegis-sdk-python-1.0.1/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.638305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    13731 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.639305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.640305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4740 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.641305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-07-18 14:14:36.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78106 2023-07-18 14:14:36.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.642305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6375 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14954 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.643305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12807 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25755 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.644305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10314 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.645305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.646305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15823 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    24262 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31817 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.647305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.648305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.649305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8546 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.650305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7782 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.651305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.651305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.652305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10577 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.653305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12999 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10457 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24248 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.654305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    28008 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.655305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7214 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    41182 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.656305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.657305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.658305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6858 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.659305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5923 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12949 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.660305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13046 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.661305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14207 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16097 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.662305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.662305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17210 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9170 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    19048 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenant_profiles/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.663305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    34203 2023-07-17 14:50:15.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.664305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13781 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.665305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.666305 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11558 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7075 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25732 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     6493 2023-07-17 08:10:16.000000 taegis-sdk-python-1.0.1/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:15:37.638305 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8246 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-18 14:15:37.000000 taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.0rc1/LICENSE` & `taegis-sdk-python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/PKG-INFO` & `taegis-sdk-python-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0rc1/README.md` & `taegis-sdk-python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/setup.py` & `taegis-sdk-python-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/service_core.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 from taegis_sdk_python.services.notebooks import NotebooksService
 from taegis_sdk_python.services.notifications import NotificationsService
 from taegis_sdk_python.services.preferences import PreferencesService
 from taegis_sdk_python.services.roadrunner import RoadrunnerService
 from taegis_sdk_python.services.rules import RulesService
 from taegis_sdk_python.services.sharelinks import SharelinksService
+from taegis_sdk_python.services.tenant_profiles import TenantProfilesService
 from taegis_sdk_python.services.tenants import TenantsService
 from taegis_sdk_python.services.threat import ThreatService
 from taegis_sdk_python.services.trip import TripService
 from taegis_sdk_python.services.users import UsersService
 
 __all__ = ["GraphQLService"]
 
@@ -114,14 +115,15 @@
         self._notebooks = None
         self._notifications = None
         self._preferences = None
         self._roadrunner = None
         self._rules = None
         self._core = None
         self._sharelinks = None
+        self._tenant_profiles = None
         self._tenants = None
         self._threat = None
         self._trip = None
         self._users = None
 
     def __call__(self, **kwargs):
         self._context_manager.update(kwargs)
@@ -380,14 +382,21 @@
     def sharelinks(self):
         """Sharelinks Service Endpoint."""
         if not self._sharelinks:
             self._sharelinks = SharelinksService(self)
         return self._sharelinks
 
     @property
+    def tenant_profiles(self):
+        """Tenant Profiles Service Endpoint."""
+        if not self._tenant_profiles:
+            self._tenant_profiles = TenantProfilesService(self)
+        return self._tenant_profiles
+
+    @property
     def tenants(self):
         """Tenants Service Endpoint."""
         if not self._tenants:
             self._tenants = TenantsService(self)
         return self._tenants
 
     @property
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/agent/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     BETA = "BETA"
     PREVIEW = "PREVIEW"
     STABLE = "STABLE"
     DEV = "DEV"
     CANARY = "CANARY"
     QE_PREV = "QE_PREV"
     QE_NEXT = "QE_NEXT"
+    WEEKLY = "WEEKLY"
+    WEEKLY_NEXT = "WEEKLY_NEXT"
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class MetaData:
     """MetaData."""
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/assets2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/clients/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,20 @@
     )
     updated_by: Optional[str] = field(
         default=None, metadata=config(field_name="updated_by")
     )
     environment: Optional[str] = field(
         default=None, metadata=config(field_name="environment")
     )
+    token_request_time: Optional[str] = field(
+        default=None, metadata=config(field_name="token_request_time")
+    )
+    token_request_count: Optional[int] = field(
+        default=None, metadata=config(field_name="token_request_count")
+    )
     role_assignments: Optional[List[ClientRoleAssignment]] = field(
         default=None, metadata=config(field_name="role_assignments")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,54 @@
             },
             output=build_output_string(Cluster),
         )
         if result.get(endpoint) is not None:
             return Cluster.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query getCluster")
 
+    def get_cluster_backlog_count(
+        self, cluster_id: str, time_range: TimeRange
+    ) -> List[ClusterNodeTimeSeries]:
+        """None."""
+        endpoint = "getClusterBacklogCount"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "clusterID": prepare_input(cluster_id),
+                "timeRange": prepare_input(time_range),
+            },
+            output=build_output_string(ClusterNodeTimeSeries),
+        )
+        if result.get(endpoint) is not None:
+            return ClusterNodeTimeSeries.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query getClusterBacklogCount")
+
+    def get_cluster_backlog_age(
+        self, cluster_id: str, time_range: TimeRange
+    ) -> List[ClusterNodeTimeSeries]:
+        """None."""
+        endpoint = "getClusterBacklogAge"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "clusterID": prepare_input(cluster_id),
+                "timeRange": prepare_input(time_range),
+            },
+            output=build_output_string(ClusterNodeTimeSeries),
+        )
+        if result.get(endpoint) is not None:
+            return ClusterNodeTimeSeries.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query getClusterBacklogAge")
+
     def get_clusters_by_ids(self, cluster_ids: List[str]) -> List[Cluster]:
         """Get clusters by IDs."""
         endpoint = "getClustersByIDs"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/collector/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,14 +334,23 @@
     aggregate_rate: Optional[Any] = field(
         default=None, metadata=config(field_name="aggregateRate")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class TimeSeries:
+    """TimeSeries."""
+
+    time: Optional[str] = field(default=None, metadata=config(field_name="time"))
+    value: Optional[str] = field(default=None, metadata=config(field_name="value"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class FlowRate:
     """FlowRate."""
 
     per_flow_max: Optional[Any] = field(
         default=None, metadata=config(field_name="perFlowMax")
     )
     per_flow_average: Optional[Any] = field(
@@ -617,14 +626,32 @@
     hosts: Optional[List[HostsInput]] = field(
         default=None, metadata=config(field_name="hosts")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class ClusterNodeTimeSeries:
+    """ClusterNodeTimeSeries."""
+
+    cluster_id: Optional[str] = field(
+        default=None, metadata=config(field_name="clusterID")
+    )
+    tenant: Optional[str] = field(default=None, metadata=config(field_name="tenant"))
+    node_id: Optional[str] = field(default=None, metadata=config(field_name="nodeId"))
+    node_name: Optional[str] = field(
+        default=None, metadata=config(field_name="nodeName")
+    )
+    val: Optional[List[TimeSeries]] = field(
+        default=None, metadata=config(field_name="val")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class LogLastSeenMetrics:
     """LogLastSeenMetrics."""
 
     log_metrics: Optional[List[LogLastSeenMetric]] = field(
         default=None, metadata=config(field_name="logMetrics")
     )
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/detector_registry/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/detector_registry/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
     )
     policy_name: Optional[str] = field(
         default=None, metadata=config(field_name="policyName")
     )
     is_system_generated: Optional[bool] = field(
         default=None, metadata=config(field_name="isSystemGenerated")
     )
+    is_default: Optional[bool] = field(
+        default=None, metadata=config(field_name="isDefault")
+    )
     desired_agent_version: Optional[str] = field(
         default=None, metadata=config(field_name="desiredAgentVersion")
     )
     channel: Optional[str] = field(default=None, metadata=config(field_name="channel"))
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="createdAt")
     )
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/entity_profile/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/entity_profile/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/event_search/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/events/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,19 +76,33 @@
     UUID = "UUID"
     SENSOR_ID = "SensorId"
     TIMESTAMP = "Timestamp"
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class BackendTargetingStrategy:
+    """BackendTargetingStrategy."""
+
+    primary: Optional[int] = field(default=None, metadata=config(field_name="primary"))
+    exclude: Optional[List[int]] = field(
+        default=None, metadata=config(field_name="exclude")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class Event:
     """Event."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     values: Optional[dict] = field(default=None, metadata=config(field_name="values"))
+    backends: Optional[List[int]] = field(
+        default=None, metadata=config(field_name="backends")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class EventUser:
     """EventUser."""
 
@@ -140,14 +154,35 @@
     )
     include_mitre_attack_info_data: Optional[bool] = field(
         default=None, metadata=config(field_name="includeMitreAttackInfoData")
     )
     normalize_event_keys: Optional[bool] = field(
         default=None, metadata=config(field_name="normalizeEventKeys")
     )
+    backend_strategy: Optional[BackendTargetingStrategy] = field(
+        default=None, metadata=config(field_name="backendStrategy")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class Field:
+    """Field."""
+
+    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    searchable: Optional[bool] = field(
+        default=None, metadata=config(field_name="searchable")
+    )
+    debug: Optional[bool] = field(default=None, metadata=config(field_name="debug"))
+    base_type: Optional[BaseType] = field(
+        default=None, metadata=config(field_name="baseType")
+    )
+    logical_type: Optional[LogicalType] = field(
+        default=None, metadata=config(field_name="logicalType")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class EventQueryOptions:
     """EventQueryOptions."""
 
@@ -167,36 +202,35 @@
     include_alerts_data: Optional[bool] = field(
         default=None, metadata=config(field_name="includeAlertsData")
     )
     include_mitre_attack_info_data: Optional[bool] = field(
         default=None, metadata=config(field_name="includeMitreAttackInfoData")
     )
     save_to_cache: Optional[bool] = field(
-        default=None, metadata=config(field_name="saveToCache")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "Moving to backendStrategy as an exclusion option",
+            },
+            field_name="saveToCache",
+        ),
     )
     search_target: Optional[SearchTarget] = field(
-        default=None, metadata=config(field_name="searchTarget")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class Field:
-    """Field."""
-
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    searchable: Optional[bool] = field(
-        default=None, metadata=config(field_name="searchable")
-    )
-    debug: Optional[bool] = field(default=None, metadata=config(field_name="debug"))
-    base_type: Optional[BaseType] = field(
-        default=None, metadata=config(field_name="baseType")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "Moving to backendStrategy",
+            },
+            field_name="searchTarget",
+        ),
     )
-    logical_type: Optional[LogicalType] = field(
-        default=None, metadata=config(field_name="logicalType")
+    backend_strategy: Optional[BackendTargetingStrategy] = field(
+        default=None, metadata=config(field_name="backendStrategy")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class EventQueryResult:
     """EventQueryResult."""
@@ -208,15 +242,27 @@
     submitted: Optional[str] = field(
         default=None, metadata=config(field_name="submitted")
     )
     completed: Optional[str] = field(
         default=None, metadata=config(field_name="completed")
     )
     expires: Optional[str] = field(default=None, metadata=config(field_name="expires"))
-    backend: Optional[str] = field(default=None, metadata=config(field_name="backend"))
+    backend: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "Moved to backendTarget",
+            },
+            field_name="backend",
+        ),
+    )
+    backend_target: Optional[int] = field(
+        default=None, metadata=config(field_name="backendTarget")
+    )
     facets: Optional[dict] = field(default=None, metadata=config(field_name="facets"))
     rows: Optional[List[dict]] = field(default=None, metadata=config(field_name="rows"))
     progress: Optional[EventQueryProgress] = field(
         default=None, metadata=config(field_name="progress")
     )
     fields: Optional[List[Field]] = field(
         default=None, metadata=config(field_name="fields")
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/investigations2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/preferences/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/preferences/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/roadrunner/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/roadrunner/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,7 +299,24 @@
                 "newPartnerTenantID": prepare_input(new_partner_tenant_id),
             },
             output=build_output_string(Tenant),
         )
         if result.get(endpoint) is not None:
             return Tenant.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation changeTenantHierarchy")
+
+    def request_service(
+        self, tenant_service_input: TenantServiceInput
+    ) -> TenantService:
+        """Requests a service for the tenant, the subject should have tenant.update on TenantServiceInput.tenantID, only internal services can be requested."""
+        endpoint = "requestService"
+
+        result = self.service.execute_mutation(
+            endpoint=endpoint,
+            variables={
+                "tenantServiceInput": prepare_input(tenant_service_input),
+            },
+            output=build_output_string(TenantService),
+        )
+        if result.get(endpoint) is not None:
+            return TenantService.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation requestService")
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/tenants/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 
     UPDATE = "Update"
     READ = "Read"
     CREATE = "Create"
     DELETE = "Delete"
 
 
+class TenantType(str, Enum):
+    """TenantType."""
+
+    INTERNAL_TENANT = "InternalTenant"
+    CONNECTION_OWNER = "ConnectionOwner"
+    SERVICE_OWNER = "ServiceOwner"
+
+
 class TenantOrderField(str, Enum):
     """TenantOrderField."""
 
     ID = "Id"
     NAME = "Name"
     CREATED_AT = "CreatedAt"
     UPDATED_AT = "UpdatedAt"
@@ -167,14 +175,53 @@
     owner_tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="owner_tenant_id")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class TenantService:
+    """TenantService."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+    service_id: Optional[str] = field(
+        default=None, metadata=config(field_name="service_id")
+    )
+    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    description: Optional[str] = field(
+        default=None, metadata=config(field_name="description")
+    )
+    service_owner_id: Optional[str] = field(
+        default=None, metadata=config(field_name="service_owner_id")
+    )
+    owned_by_partner: Optional[bool] = field(
+        default=None, metadata=config(field_name="owned_by_partner")
+    )
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="created_at")
+    )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updated_at")
+    )
+    requested_at: Optional[str] = field(
+        default=None, metadata=config(field_name="requested_at")
+    )
+    granted_at: Optional[str] = field(
+        default=None, metadata=config(field_name="granted_at")
+    )
+    revoked_at: Optional[str] = field(
+        default=None, metadata=config(field_name="revoked_at")
+    )
+    requested_by: Optional[str] = field(
+        default=None, metadata=config(field_name="requested_by")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class ServiceEvents:
     """ServiceEvents."""
 
     tenant_id: Optional[str] = field(
         default=None, metadata=config(field_name="tenantID")
     )
     service_name: Optional[str] = field(
@@ -455,14 +502,27 @@
         default=None, metadata=config(field_name="clientSecret")
     )
     domain: Optional[str] = field(default=None, metadata=config(field_name="domain"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class TenantServiceInput:
+    """TenantServiceInput."""
+
+    service_id: Optional[str] = field(
+        default=None, metadata=config(field_name="serviceID")
+    )
+    tenant_id: Optional[str] = field(
+        default=None, metadata=config(field_name="tenantID")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class AuditResults:
     """AuditResults."""
 
     cursor_pos: Optional[str] = field(
         default=None, metadata=config(field_name="cursorPos")
     )
     count: Optional[int] = field(default=None, metadata=config(field_name="count"))
@@ -687,14 +747,70 @@
     exclude_status: Optional[List[SSOConnectionStatus]] = field(
         default=None, metadata=config(field_name="excludeStatus")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class SSOConnection:
+    """SSOConnection."""
+
+    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    external_name: Optional[str] = field(
+        default=None, metadata=config(field_name="externalName")
+    )
+    external_id: Optional[str] = field(
+        default=None, metadata=config(field_name="externalID")
+    )
+    tenant_id: Optional[str] = field(
+        default=None, metadata=config(field_name="tenantID")
+    )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt")
+    )
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt")
+    )
+    cert_name: Optional[str] = field(
+        default=None, metadata=config(field_name="certName")
+    )
+    expires_at: Optional[str] = field(
+        default=None, metadata=config(field_name="expiresAt")
+    )
+    not_before: Optional[str] = field(
+        default=None, metadata=config(field_name="notBefore")
+    )
+    issuer: Optional[str] = field(default=None, metadata=config(field_name="issuer"))
+    subject: Optional[str] = field(default=None, metadata=config(field_name="subject"))
+    domains: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="domains")
+    )
+    testers: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="testers")
+    )
+    type: Optional[SSOConnectionType] = field(
+        default=None, metadata=config(field_name="type")
+    )
+    status: Optional[SSOConnectionStatus] = field(
+        default=None, metadata=config(field_name="status")
+    )
+    environment: Optional[SSOEnvironment] = field(
+        default=None, metadata=config(field_name="environment")
+    )
+    sso_connection_parameters: Optional[SSOConnectionParameters] = field(
+        default=None, metadata=config(field_name="ssoConnectionParameters")
+    )
+    sso_connection_idp_config: Optional[SSOConnectionConfiguration] = field(
+        default=None, metadata=config(field_name="ssoConnectionIDPConfig")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class Tenant:
     """Tenant."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="created_at")
     )
@@ -737,74 +853,31 @@
     labels: Optional[List[TenantLabel]] = field(
         default=None, metadata=config(field_name="labels")
     )
     environments: Optional[List[Environment]] = field(
         default=None, metadata=config(field_name="environments")
     )
     services: Optional[List[Service]] = field(
-        default=None, metadata=config(field_name="services")
-    )
-    partnership: Optional[Partnership] = field(
-        default=None, metadata=config(field_name="partnership")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class SSOConnection:
-    """SSOConnection."""
-
-    id: Optional[str] = field(default=None, metadata=config(field_name="id"))
-    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
-    external_name: Optional[str] = field(
-        default=None, metadata=config(field_name="externalName")
-    )
-    external_id: Optional[str] = field(
-        default=None, metadata=config(field_name="externalID")
-    )
-    tenant_id: Optional[str] = field(
-        default=None, metadata=config(field_name="tenantID")
-    )
-    updated_at: Optional[str] = field(
-        default=None, metadata=config(field_name="updatedAt")
-    )
-    created_at: Optional[str] = field(
-        default=None, metadata=config(field_name="createdAt")
-    )
-    cert_name: Optional[str] = field(
-        default=None, metadata=config(field_name="certName")
-    )
-    expires_at: Optional[str] = field(
-        default=None, metadata=config(field_name="expiresAt")
-    )
-    not_before: Optional[str] = field(
-        default=None, metadata=config(field_name="notBefore")
-    )
-    issuer: Optional[str] = field(default=None, metadata=config(field_name="issuer"))
-    subject: Optional[str] = field(default=None, metadata=config(field_name="subject"))
-    domains: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="domains")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "use all services"},
+            field_name="services",
+        ),
     )
-    testers: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="testers")
+    granted_services: Optional[List[TenantService]] = field(
+        default=None, metadata=config(field_name="granted_services")
     )
-    type: Optional[SSOConnectionType] = field(
-        default=None, metadata=config(field_name="type")
+    requested_services: Optional[List[TenantService]] = field(
+        default=None, metadata=config(field_name="requested_services")
     )
-    status: Optional[SSOConnectionStatus] = field(
-        default=None, metadata=config(field_name="status")
+    all_services: Optional[List[TenantService]] = field(
+        default=None, metadata=config(field_name="all_services")
     )
-    environment: Optional[SSOEnvironment] = field(
-        default=None, metadata=config(field_name="environment")
-    )
-    sso_connection_parameters: Optional[SSOConnectionParameters] = field(
-        default=None, metadata=config(field_name="ssoConnectionParameters")
-    )
-    sso_connection_idp_config: Optional[SSOConnectionConfiguration] = field(
-        default=None, metadata=config(field_name="ssoConnectionIDPConfig")
+    partnership: Optional[Partnership] = field(
+        default=None, metadata=config(field_name="partnership")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class TenantsQuery:
     """TenantsQuery."""
@@ -823,14 +896,17 @@
     )
     with_service: Optional[str] = field(
         default=None, metadata=config(field_name="withService")
     )
     with_services: Optional[List[str]] = field(
         default=None, metadata=config(field_name="withServices")
     )
+    with_requested_services: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="withRequestedServices")
+    )
     with_partner_subscription: Optional[str] = field(
         default=None, metadata=config(field_name="withPartnerSubscription")
     )
     with_partner_subscriptions: Optional[List[str]] = field(
         default=None, metadata=config(field_name="withPartnerSubscriptions")
     )
     is_partner: Optional[bool] = field(
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/services/users/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.1/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0rc1/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.1/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,19 @@
 taegis_sdk_python/services/rules/subscriptions.py
 taegis_sdk_python/services/rules/types.py
 taegis_sdk_python/services/sharelinks/__init__.py
 taegis_sdk_python/services/sharelinks/mutations.py
 taegis_sdk_python/services/sharelinks/queries.py
 taegis_sdk_python/services/sharelinks/subscriptions.py
 taegis_sdk_python/services/sharelinks/types.py
+taegis_sdk_python/services/tenant_profiles/__init__.py
+taegis_sdk_python/services/tenant_profiles/mutations.py
+taegis_sdk_python/services/tenant_profiles/queries.py
+taegis_sdk_python/services/tenant_profiles/subscriptions.py
+taegis_sdk_python/services/tenant_profiles/types.py
 taegis_sdk_python/services/tenants/__init__.py
 taegis_sdk_python/services/tenants/mutations.py
 taegis_sdk_python/services/tenants/queries.py
 taegis_sdk_python/services/tenants/subscriptions.py
 taegis_sdk_python/services/tenants/types.py
 taegis_sdk_python/services/threat/__init__.py
 taegis_sdk_python/services/threat/mutations.py
```

