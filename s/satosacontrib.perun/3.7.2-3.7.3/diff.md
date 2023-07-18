# Comparing `tmp/satosacontrib.perun-3.7.2.tar.gz` & `tmp/satosacontrib.perun-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosacontrib.perun-3.7.2.tar", last modified: Sat Jul 15 12:10:47 2023, max compression
+gzip compressed data, was "satosacontrib.perun-3.7.3.tar", last modified: Tue Jul 18 09:20:57 2023, max compression
```

## Comparing `satosacontrib.perun-3.7.2.tar` & `satosacontrib.perun-3.7.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.089826 satosacontrib.perun-3.7.2/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4897 2023-07-15 12:10:47.089826 satosacontrib.perun-3.7.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3902 2023-07-11 10:25:54.000000 satosacontrib.perun-3.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.077826 satosacontrib.perun-3.7.2/satosacontrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.077826 satosacontrib.perun-3.7.2/satosacontrib/perun/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.081826 satosacontrib.perun-3.7.2/satosacontrib/perun/addons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 20:25:20.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/addons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1528 2023-07-15 11:55:34.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/addons/extended_introspection_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.081826 satosacontrib.perun-3.7.2/satosacontrib/perun/backends/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-11 10:25:55.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/backends/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10129 2023-07-14 20:28:21.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/backends/seznam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.085826 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/attribute_typing_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-11 10:25:55.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/auth_switcher_lite.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/cardinality_single_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/compute_eligibility.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-07 14:33:28.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/context_attributes_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.085826 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8313 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/additional_identifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    11822 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/perun_user.py
--rw-rw-rw-   0 root         (0) root         (0)    24791 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/sp_authorization.py
--rw-rw-rw-   0 root         (0) root         (0)    11491 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/is_banned_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/multi_idphint_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-04 07:23:14.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/proxystatistics_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2023-07-04 08:38:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/session_started_with_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.089826 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/CurlConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/CurlConnectorInterface.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/PerunConstants.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/satosacontrib/perun/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.077826 satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4897 2023-07-15 12:10:46.000000 satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2591 2023-07-15 12:10:47.000000 satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 12:10:46.000000 satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-15 12:10:46.000000 satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-15 12:10:46.000000 satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-15 12:10:47.093826 satosacontrib.perun-3.7.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-15 11:55:34.000000 satosacontrib.perun-3.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 12:10:47.089826 satosacontrib.perun-3.7.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10917 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_additional_indentifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_auth_event_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2023-07-07 14:33:28.000000 satosacontrib.perun-3.7.2/tests/test_context_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_is_banned.py
--rw-rw-rw-   0 root         (0) root         (0)     7500 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_microservice_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_perun_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    14517 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    36568 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-06-15 11:29:51.000000 satosacontrib.perun-3.7.2/tests/test_update_ues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:57.268122 satosacontrib.perun-3.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4897 2023-07-18 09:20:57.268122 satosacontrib.perun-3.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3902 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.320099 satosacontrib.perun-3.7.3/satosacontrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.320099 satosacontrib.perun-3.7.3/satosacontrib/perun/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.320099 satosacontrib.perun-3.7.3/satosacontrib/perun/addons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/addons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/addons/extended_introspection_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.548104 satosacontrib.perun-3.7.3/satosacontrib/perun/backends/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/backends/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10129 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/backends/seznam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.708108 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/attribute_typing_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/auth_switcher_lite.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/cardinality_single_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/compute_eligibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/context_attributes_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.904113 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/additional_identifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11822 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    11268 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/perun_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    24791 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/sp_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/is_banned_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/multi_idphint_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/proxystatistics_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/session_started_with_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.988115 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/CurlConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/CurlConnectorInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/PerunConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/satosacontrib/perun/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:56.320099 satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4897 2023-07-18 09:20:56.000000 satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-18 09:20:56.000000 satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 09:20:56.000000 satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-18 09:20:56.000000 satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-18 09:20:56.000000 satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-18 09:20:57.268122 satosacontrib.perun-3.7.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:20:57.256121 satosacontrib.perun-3.7.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10917 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_additional_indentifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_auth_event_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_context_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_is_banned.py
+-rw-rw-rw-   0 root         (0) root         (0)     7500 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_microservice_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_perun_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_perun_ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)     7106 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_perun_entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_perun_user_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)    36568 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_sp_authorization_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-07-18 09:10:38.000000 satosacontrib.perun-3.7.3/tests/test_update_ues.py
```

### Comparing `satosacontrib.perun-3.7.2/LICENSE` & `satosacontrib.perun-3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/PKG-INFO` & `satosacontrib.perun-3.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosacontrib.perun
-Version: 3.7.2
+Version: 3.7.3
 Summary: Microservices for SATOSA authentication proxy, made by the Perun team
 Home-page: https://github.com/CESNET/satosacontrib.perun.git
 License: UNKNOWN
 Description: # satosacontrib.perun
         
         Microservices for [SATOSA](https://github.com/IdentityPython/SATOSA) authentication
         proxy, made by the Perun team.
```

### Comparing `satosacontrib.perun-3.7.2/README.md` & `satosacontrib.perun-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/addons/extended_introspection_response.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/addons/extended_introspection_response.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/backends/seznam.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/backends/seznam.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/__init__.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/__init__.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/attribute_typing_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/attribute_typing_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/auth_event_logging_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/auth_event_logging_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/auth_switcher_lite.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/auth_switcher_lite.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/cardinality_single_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/cardinality_single_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/compute_eligibility.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/compute_eligibility.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/context_attributes_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/context_attributes_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/additional_identifiers.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/additional_identifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/attributes.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/ensure_member.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/entitlement.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/entitlement.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,51 +25,52 @@
     resource capabilities and facility capabilities"""
 
     def __init__(self, config, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.__logger = Logger.get_logger(self.__class__.__name__)
 
-        self.OUTPUT_ATTR_NAME = "eduperson_entitlement"
+        self.OUTPUT_ATTR_NAME = "output_attr_name"
         self.RELEASE_FORWARDED_ENTITLEMENT = "release_forwarded_entitlement"
-        self.FORWARDED_EDU_PERSON_ENTITLEMENT = (
-            "forwarded_eduperson_entitlement"  # noqa
-        )
+        self.FORWARDED_EDUPERSON_ENTITLEMENT = "forwarded_eduperson_entitlement"
         self.ENTITLEMENT_PREFIX_ATTR = "entitlement_prefix"
         self.ENTITLEMENT_AUTHORITY_ATTR = "entitlement_authority"
         self.GROUP_NAME_AARC_ATTR = "group_name_AARC"
 
         self.__config = config
 
         self.__group_mapping = self.__config["group_mapping"]
-        self.__extended = False
-        if self.__config["entitlement_extended"] == "true":
-            self.__extended = True
+        self.__extended = self.__config.get("entitlement_extended", False) in [
+            True,
+            "True",
+            "true",
+            "1",
+            1,
+        ]
 
         self.__global_cfg = ConfigStore.get_global_cfg(config["global_cfg_path"])
 
         self.__attr_map_cfg = ConfigStore.get_attributes_map(
             self.__global_cfg["attrs_cfg_path"]
         )
         self.__allowed_requesters = self.__global_cfg.get("allowed_requesters", {})
         self.__adapters_manager = AdaptersManager(
             self.__global_cfg["adapters_manager"], self.__attr_map_cfg
         )
-        if not self.__extended:
-            self.__edu_person_entitlement = self.__global_cfg[self.OUTPUT_ATTR_NAME]
-        else:
-            self.__output_attr_name = self.__global_cfg[self.OUTPUT_ATTR_NAME]
+        self.__output_attr_name = self.__config.get(
+            self.OUTPUT_ATTR_NAME, "eduperson_entitlement"
+        )
 
-        self.__release_forwarded_entitlement = self.__global_cfg.get(
+        self.__release_forwarded_entitlement = self.__config.get(
             self.RELEASE_FORWARDED_ENTITLEMENT, True
         )
 
-        self.__forwarded_edu_person_entitlement = self.__global_cfg[
-            self.FORWARDED_EDU_PERSON_ENTITLEMENT
-        ]
+        self.__forwarded_eduperson_entitlement = self.__config.get(
+            self.FORWARDED_EDUPERSON_ENTITLEMENT
+        )
 
         self.__group_name_aarc = self.__config[self.GROUP_NAME_AARC_ATTR]
 
         self.__entitlement_prefix = self.__config[self.ENTITLEMENT_PREFIX_ATTR]
 
         self.__entitlement_authority = self.__config[self.ENTITLEMENT_AUTHORITY_ATTR]
 
@@ -80,70 +81,62 @@
         next callable is called).
 
         @param context: The current context
         @param data: Data to be modified
         """
         if not Utils.allow_by_requester(context, data, self.__allowed_requesters):
             return super().process(context, data)
-        edu_person_entitlement = []
-        edu_person_entitlement_extended = []
+        eduperson_entitlement = []
+        eduperson_entitlement_extended = []
         capabilities = []
-        forwarded_edu_person_entitlement = []
+        forwarded_eduperson_entitlement = []
         if data.data["perun"]["groups"]:
             if not self.__extended:
-                edu_person_entitlement = self.__get_edu_person_entitlement(data)
+                eduperson_entitlement = self.__get_eduperson_entitlement(data)
             else:
-                edu_person_entitlement_extended = (
-                    self.__get_edu_person_entitlement_extended(data)
+                eduperson_entitlement_extended = (
+                    self.__get_eduperson_entitlement_extended(data)
                 )
 
             capabilities = self.__get_capabilities(data)
 
         else:
             self.__logger.debug(
                 "perun:Entitlement: There are no user "
                 "groups assigned to facility. => Skipping "
                 "getEduPersonEntitlement and getCapabilities"
             )
 
         if self.__release_forwarded_entitlement:
-            forwarded_edu_person_entitlement = (
-                self.__get_forwarded_edu_person_entitlement(
+            forwarded_eduperson_entitlement = (
+                self.__get_forwarded_eduperson_entitlement(
                     data,
                 )
             )
 
-        if not self.__extended:
-            data.attributes[self.__edu_person_entitlement] = list(
-                set(
-                    edu_person_entitlement
-                    + forwarded_edu_person_entitlement
-                    + capabilities
-                )
-            )
-        else:
-            data.attributes[self.__edu_person_entitlement] = list(
-                set(
-                    edu_person_entitlement_extended
-                    + forwarded_edu_person_entitlement
-                    + capabilities
-                )
-            )
+        values = data.attributes.get(self.__output_attr_name, [])
+        values = values + (
+            eduperson_entitlement_extended if self.__extended else eduperson_entitlement
+        )
+        values = values + forwarded_eduperson_entitlement
+        values = values + capabilities
+        values = list(set(values))
+        data.attributes[self.__output_attr_name] = values
 
         return super().process(context, data)
 
-    def __get_edu_person_entitlement(self, data):
+    def __get_eduperson_entitlement(self, data):
         """
         This method gets entitlements of groups stored in `data`
 
         @param data: Data (from process) to be modified
         @return: list of entitlements
         """
 
-        edu_person_entitlement = []
+        eduperson_entitlement = []
 
         groups = data.data["perun"]["groups"]
         for group in groups:
             group_name = group.unique_name
             group_name = sub(r"^(\w*):members$", r"\1", group_name)
 
             if self.__config["group_name_AARC"] or self.__group_name_aarc:
@@ -155,93 +148,91 @@
                         "or 'groupNamePrefix'."
                     )
 
                 group_name = self.__group_name_wrapper(group_name)
             else:
                 group_name = self.__map_group_name(group_name, data.requester)
 
-            edu_person_entitlement.append(group_name)
+            eduperson_entitlement.append(group_name)
 
-        natsorted(edu_person_entitlement)
+        natsorted(eduperson_entitlement)
 
-        return edu_person_entitlement
+        return eduperson_entitlement
 
-    def __get_edu_person_entitlement_extended(self, data):
+    def __get_eduperson_entitlement_extended(self, data):
         """
         This method gets entitlements of groups stored in `data`
         in extended mode
 
         @param data: Data (from process) to be modified
         @return: list of entitlements
         """
 
-        edu_person_entitlement_extended = []
+        eduperson_entitlement_extended = []
 
         groups = data.data["perun"]["groups"]
         for group in groups:
             entitlement = self.__group_entitlement_wrapper(group.uuid)
 
-            edu_person_entitlement_extended.append(entitlement)
+            eduperson_entitlement_extended.append(entitlement)
 
             group_name = group.unique_name
             group_name = sub(r"^(\w*):members$", r"\1", group_name)
 
             entitlement_with_attributes = (
                 self.__group_entitlement_with_attributes_wrapper(group.uuid, group_name)
             )
-            edu_person_entitlement_extended.append(entitlement_with_attributes)
+            eduperson_entitlement_extended.append(entitlement_with_attributes)
 
-        natsorted(edu_person_entitlement_extended)
-        return edu_person_entitlement_extended
+        natsorted(eduperson_entitlement_extended)
+        return eduperson_entitlement_extended
 
-    def __get_forwarded_edu_person_entitlement(self, data):
+    def __get_forwarded_eduperson_entitlement(self, data):
         """
-        This method gets forwarded_edu_person_entitlement
+        This method gets forwarded_eduperson_entitlement
         based on the user in `data`
 
         @param data: Data (from process) to be modified
         @return: list of forwarded edu person entitlements
         """
 
         result = []
 
-        user_id = data.attributes.get(
-            self.__global_cfg["perun_user_id_attribute"]
-        )  # noqa
+        user_id = data.attributes.get(self.__global_cfg["perun_user_id_attribute"])
         if not user_id:
             self.__logger.debug(
                 "perun:Entitlement: Perun User Id is not "
                 "specified. => Skipping getting forwardedEntitlement."
             )
 
             return result
 
-        forwarded_edu_person_entitlement_map = dict()
+        forwarded_eduperson_entitlement_map = dict()
 
         try:
-            forwarded_edu_person_entitlement_map = (
+            forwarded_eduperson_entitlement_map = (
                 self.__adapters_manager.get_user_attributes(
-                    user_id, [self.__forwarded_edu_person_entitlement]
+                    user_id, [self.__forwarded_eduperson_entitlement]
                 )
             )
         except Exception as e:
             self.__logger.debug(
                 "perun:Entitlement: Exception "
                 + str(e)
                 + " was thrown in method 'getForwardedEduPersonEntitlement'."
             )
 
-        if forwarded_edu_person_entitlement_map:
-            result = [list(forwarded_edu_person_entitlement_map.values())[0]]
+        if forwarded_eduperson_entitlement_map:
+            result = [list(forwarded_eduperson_entitlement_map.values())[0]]
 
         return result
 
     def __get_capabilities(self, data):
         """
-        This method gets forwarded_edu_person_entitlement
+        This method gets forwarded_eduperson_entitlement
         based on the user in `data`
 
         @param data: Data (from process) to be modified
         @return: list of forwarded edu person entitlements
         """
 
         resource_capabilities = []
```

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/perun_user.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/perun_user.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/sp_authorization.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/sp_authorization.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/idm/update_user_ext_source.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/idm/update_user_ext_source.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/is_banned_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/is_banned_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/is_eligible_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/multi_idphint_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/multi_idphint_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/nameid_attribute_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/nameid_attribute_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/persist_authorization_params_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/proxystatistics_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/proxystatistics_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/micro_services/session_started_with_microservice.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/micro_services/session_started_with_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/utils/AuthEventLoggingDbModels.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/utils/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/utils/ConfigStore.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/utils/CurlConnector.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/utils/CurlConnector.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/utils/CurlConnectorInterface.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/utils/CurlConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib/perun/utils/Utils.py` & `satosacontrib.perun-3.7.3/satosacontrib/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/PKG-INFO` & `satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosacontrib.perun
-Version: 3.7.2
+Version: 3.7.3
 Summary: Microservices for SATOSA authentication proxy, made by the Perun team
 Home-page: https://github.com/CESNET/satosacontrib.perun.git
 License: UNKNOWN
 Description: # satosacontrib.perun
         
         Microservices for [SATOSA](https://github.com/IdentityPython/SATOSA) authentication
         proxy, made by the Perun team.
```

### Comparing `satosacontrib.perun-3.7.2/satosacontrib.perun.egg-info/SOURCES.txt` & `satosacontrib.perun-3.7.3/satosacontrib.perun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/setup.py` & `satosacontrib.perun-3.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
         "SATOSA~=8.1",
         "pysaml2~=7.1",
         "requests~=2.28",
         "perun.connector~=3.7",
         "PyYAML~=6.0",
         "SQLAlchemy~=1.4",
         "jwcrypto~=1.3",
-        "natsort~=8.3.1",
+        "natsort~=8.4.0",
         "python-dateutil~=2.8",
         "geoip2~=4.6",
         "user_agents~=2.2",
         "pymongo~=4.3",
     ],
 )
```

### Comparing `satosacontrib.perun-3.7.2/tests/test_additional_indentifiers.py` & `satosacontrib.perun-3.7.3/tests/test_additional_indentifiers.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_auth_event_logging.py` & `satosacontrib.perun-3.7.3/tests/test_auth_event_logging.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_context_attributes.py` & `satosacontrib.perun-3.7.3/tests/test_context_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_is_banned.py` & `satosacontrib.perun-3.7.3/tests/test_is_banned.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_is_eligible_microservice.py` & `satosacontrib.perun-3.7.3/tests/test_is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_microservice_loader.py` & `satosacontrib.perun-3.7.3/tests/test_microservice_loader.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_perun_attributes.py` & `satosacontrib.perun-3.7.3/tests/test_perun_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_perun_ensure_member.py` & `satosacontrib.perun-3.7.3/tests/test_perun_ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_perun_entitlement.py` & `satosacontrib.perun-3.7.3/tests/test_perun_entitlement.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,79 +151,79 @@
     AdaptersManager.get_resource_capabilities_by_rp_id = MagicMock(
         side_effect=[Exception("sth went wrong")]
     )
 
     assert TEST_INSTANCE._Entitlement__get_capabilities(TestData(DATA, None)) == []
 
 
-def test_get_forwarded_edu_person_entitlement_user_missing():
+def test_get_forwarded_eduperson_entitlement_user_missing():
     attrs = {"example_user_id": "example_user_id"}
 
     test_data = TestData(data=DATA_WITHOUT_USER, attributes=attrs)
-    assert not TEST_INSTANCE._Entitlement__get_forwarded_edu_person_entitlement(
+    assert not TEST_INSTANCE._Entitlement__get_forwarded_eduperson_entitlement(
         test_data
     )
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_user_attributes")
-def test_get_forwarded_edu_person_entitlement(mock_request):
+def test_get_forwarded_eduperson_entitlement(mock_request):
     ext_src_attrs = {"attr1": "this_is_entitlement", "attr2": "attr2", "attr3": "attr3"}
 
     attrs = {"example_user_id": "example_user_id"}
 
     test_data = TestData(data=DATA, attributes=attrs)
 
     result = ["this_is_entitlement"]
     AdaptersManager.get_user_attributes = MagicMock(return_value=ext_src_attrs)
 
     assert (
-        TEST_INSTANCE._Entitlement__get_forwarded_edu_person_entitlement(test_data)
+        TEST_INSTANCE._Entitlement__get_forwarded_eduperson_entitlement(test_data)
         == result
     )
 
 
-def test_get_edu_person_entitlement_extended():
+def test_get_eduperson_entitlement_extended():
     expected_result = [
         "prefix:groupuuid#authority",
         "prefix:groupAttributes:uuid?=displayName=group1#authority",  # noqa
         "prefix:groupuuid#authority",
         "prefix:groupAttributes:uuid?=displayName=group2#authority",
     ]  # noqa
 
-    result = TEST_INSTANCE._Entitlement__get_edu_person_entitlement_extended(
+    result = TEST_INSTANCE._Entitlement__get_eduperson_entitlement_extended(
         TestData(DATA, None)
     )  # noqa
 
     assert expected_result == result
 
 
-def test_get_edu_person_entitlement():
+def test_get_eduperson_entitlement():
     expected_result = ["prefix:group:group1#authority", "prefix:group:group2#authority"]
 
-    result = TEST_INSTANCE._Entitlement__get_edu_person_entitlement(
+    result = TEST_INSTANCE._Entitlement__get_eduperson_entitlement(
         TestData(DATA, None)
     )  # noqa
 
     assert expected_result == result
 
 
-def test_get_edu_person_entitlement_exception():
+def test_get_eduperson_entitlement_exception():
     expected_error_message = (
         "perun:Entitlement: missing "
         "mandatory configuration options "
         "'groupNameAuthority' "
         "or 'groupNamePrefix'."
     )
 
     with pytest.raises(Exception) as error:
-        _ = TEST_INSTANCE_WITHOUT_PREFIX._Entitlement__get_edu_person_entitlement(
+        _ = TEST_INSTANCE_WITHOUT_PREFIX._Entitlement__get_eduperson_entitlement(
             TestData(DATA, None)
         )
 
     assert str(error.value.args[0]) == expected_error_message
 
     with pytest.raises(Exception) as error:
-        _ = TEST_INSTANCE_WITHOUT_AUTHORITY._Entitlement__get_edu_person_entitlement(
+        _ = TEST_INSTANCE_WITHOUT_AUTHORITY._Entitlement__get_eduperson_entitlement(
             TestData(DATA, None)
         )
 
     assert str(error.value.args[0]) == expected_error_message
```

### Comparing `satosacontrib.perun-3.7.2/tests/test_perun_user_microservice.py` & `satosacontrib.perun-3.7.3/tests/test_perun_user_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_sp_authorization_microservice.py` & `satosacontrib.perun-3.7.3/tests/test_sp_authorization_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.7.2/tests/test_update_ues.py` & `satosacontrib.perun-3.7.3/tests/test_update_ues.py`

 * *Files identical despite different names*

