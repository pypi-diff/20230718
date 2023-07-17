# Comparing `tmp/zhmcclient-1.9.0.tar.gz` & `tmp/zhmcclient-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmcclient-1.9.0.tar", last modified: Fri Jul 14 08:44:31 2023, max compression
+gzip compressed data, was "zhmcclient-1.9.1.tar", last modified: Mon Jul 17 22:27:46 2023, max compression
```

## Comparing `zhmcclient-1.9.0.tar` & `zhmcclient-1.9.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-14 08:44:27.000000 zhmcclient-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/extra-testutils-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.546871 zhmcclient-1.9.0/zhmcclient/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_activation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_auto_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_capacity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32810 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    95566 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    47315 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_ldap_server_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    79949 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    43902 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    36278 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_nic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18861 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    53547 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    25001 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    69514 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_group_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_storage_volume_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_timestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_unmanaged_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_user_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_virtual_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_virtual_storage_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/_virtual_switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/zhmcclient/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_cpc_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_inventory_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient/testutils/_hmc_vault_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.546871 zhmcclient-1.9.0/zhmcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 08:44:31.000000 zhmcclient-1.9.0/zhmcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:43:41.000000 zhmcclient-1.9.0/zhmcclient.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:44:31.550871 zhmcclient-1.9.0/zhmcclient_mock/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_idpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    42583 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-07-14 08:43:30.000000 zhmcclient-1.9.0/zhmcclient_mock/_urihandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:27:46.868782 zhmcclient-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-17 22:27:43.000000 zhmcclient-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-17 22:27:46.868782 zhmcclient-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/extra-testutils-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:27:46.868782 zhmcclient-1.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:27:46.856781 zhmcclient-1.9.1/zhmcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_activation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_auto_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_capacity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32810 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95566 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47315 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79949 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43902 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36278 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_nic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18861 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53547 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25001 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69514 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_storage_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_storage_group_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_storage_volume_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_timestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_user_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19074 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_virtual_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_virtual_storage_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/_virtual_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:27:46.860781 zhmcclient-1.9.1/zhmcclient/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/testutils/_cpc_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/testutils/_hmc_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/testutils/_hmc_definition_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/testutils/_hmc_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/testutils/_hmc_inventory_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient/testutils/_hmc_vault_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:27:46.856781 zhmcclient-1.9.1/zhmcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-17 22:27:46.000000 zhmcclient-1.9.1/zhmcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-17 22:27:46.000000 zhmcclient-1.9.1/zhmcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:27:46.000000 zhmcclient-1.9.1/zhmcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 22:27:46.000000 zhmcclient-1.9.1/zhmcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 22:27:46.000000 zhmcclient-1.9.1/zhmcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:27:07.000000 zhmcclient-1.9.1/zhmcclient.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:27:46.868782 zhmcclient-1.9.1/zhmcclient_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient_mock/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient_mock/_idpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42583 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient_mock/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-07-17 22:26:56.000000 zhmcclient-1.9.1/zhmcclient_mock/_urihandler.py
```

### Comparing `zhmcclient-1.9.0/LICENSE` & `zhmcclient-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/MANIFEST.in` & `zhmcclient-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/PKG-INFO` & `zhmcclient-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.9.0
+Version: 1.9.1
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.9.0/README.rst` & `zhmcclient-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/extra-testutils-requirements.txt` & `zhmcclient-1.9.1/extra-testutils-requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/requirements.txt` & `zhmcclient-1.9.1/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -39,16 +39,22 @@
 
 # PyYAML pulled in by zhmcclient_mock (and zhmcclient examples, and python-coveralls)
 # PyYAML 5.3 fixes narrow build error
 # PyYAML 5.4 removed support for py35
 # PyYAML 6.0 removed support for py27
 # PyYAML 5.3.1 fixes safety issue 38100
 # PyYAML 5.4 fixes safety issue 39611
+# PyYAML 5.3 has wheel archives for Python 2.7, 3.5 - 3.9
+# PyYAML 5.4 has wheel archives for Python 2.7, 3.6 - 3.9
+# PyYAML 6.0 has wheel archives for Python 3.6 - 3.11
+# PyYAML 5.4 and 6.0.0 fails install since Cython 3 was released, see issue
+#   https://github.com/yaml/pyyaml/issues/724.
 PyYAML>=5.3.1; python_version <= '3.5'
-PyYAML>=5.4; python_version >= '3.6'
+PyYAML>=5.3.1,!=5.4.0,!=5.4.1; python_version >= '3.6' and python_version <= '3.11'
+PyYAML>=5.3.1,!=5.4.0,!=5.4.1,!=6.0.0; python_version >= '3.12'
 
 # yamlloader pulled in by zhmcclient_mock and zhmcclient.testutils
 # yamlloader 1.0 removed support for py27,35
 yamlloader>=0.5.5
 
 # jsonschema pulled in by zhmcclient_mock and zhmcclient.testutils
 # jsonschema 4.0 removed support for py27,35,36
```

### Comparing `zhmcclient-1.9.0/setup.py` & `zhmcclient-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/__init__.py` & `zhmcclient-1.9.1/zhmcclient/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_activation_profile.py` & `zhmcclient-1.9.1/zhmcclient/_activation_profile.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_adapter.py` & `zhmcclient-1.9.1/zhmcclient/_adapter.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_auto_updater.py` & `zhmcclient-1.9.1/zhmcclient/_auto_updater.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_capacity_group.py` & `zhmcclient-1.9.1/zhmcclient/_capacity_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_certificates.py` & `zhmcclient-1.9.1/zhmcclient/_certificates.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_client.py` & `zhmcclient-1.9.1/zhmcclient/_client.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_console.py` & `zhmcclient-1.9.1/zhmcclient/_console.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_constants.py` & `zhmcclient-1.9.1/zhmcclient/_constants.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_cpc.py` & `zhmcclient-1.9.1/zhmcclient/_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_debug_info.py` & `zhmcclient-1.9.1/zhmcclient/_debug_info.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_exceptions.py` & `zhmcclient-1.9.1/zhmcclient/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_group.py` & `zhmcclient-1.9.1/zhmcclient/_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_hba.py` & `zhmcclient-1.9.1/zhmcclient/_hba.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_ldap_server_definition.py` & `zhmcclient-1.9.1/zhmcclient/_ldap_server_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_logging.py` & `zhmcclient-1.9.1/zhmcclient/_logging.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_lpar.py` & `zhmcclient-1.9.1/zhmcclient/_lpar.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_manager.py` & `zhmcclient-1.9.1/zhmcclient/_manager.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_metrics.py` & `zhmcclient-1.9.1/zhmcclient/_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_nic.py` & `zhmcclient-1.9.1/zhmcclient/_nic.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_notification.py` & `zhmcclient-1.9.1/zhmcclient/_notification.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_partition.py` & `zhmcclient-1.9.1/zhmcclient/_partition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_password_rule.py` & `zhmcclient-1.9.1/zhmcclient/_password_rule.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_port.py` & `zhmcclient-1.9.1/zhmcclient/_port.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_resource.py` & `zhmcclient-1.9.1/zhmcclient/_resource.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_session.py` & `zhmcclient-1.9.1/zhmcclient/_session.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_storage_group.py` & `zhmcclient-1.9.1/zhmcclient/_storage_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_storage_group_template.py` & `zhmcclient-1.9.1/zhmcclient/_storage_group_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_storage_volume.py` & `zhmcclient-1.9.1/zhmcclient/_storage_volume.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_storage_volume_template.py` & `zhmcclient-1.9.1/zhmcclient/_storage_volume_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_task.py` & `zhmcclient-1.9.1/zhmcclient/_task.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_timestats.py` & `zhmcclient-1.9.1/zhmcclient/_timestats.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_unmanaged_cpc.py` & `zhmcclient-1.9.1/zhmcclient/_unmanaged_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_user.py` & `zhmcclient-1.9.1/zhmcclient/_user.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_user_pattern.py` & `zhmcclient-1.9.1/zhmcclient/_user_pattern.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_user_role.py` & `zhmcclient-1.9.1/zhmcclient/_user_role.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_utils.py` & `zhmcclient-1.9.1/zhmcclient/_utils.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_version.py` & `zhmcclient-1.9.1/zhmcclient/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 
 # Check supported Python versions
 # Keep these Python versions in sync with:
 # - python_requires and classifiers in setup.py
 # - Section "Supported environments" in docs/intro.rst
 _PYTHON_M = sys.version_info[0]
 _PYTHON_N = sys.version_info[1]
```

### Comparing `zhmcclient-1.9.0/zhmcclient/_virtual_function.py` & `zhmcclient-1.9.1/zhmcclient/_virtual_function.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_virtual_storage_resource.py` & `zhmcclient-1.9.1/zhmcclient/_virtual_storage_resource.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/_virtual_switch.py` & `zhmcclient-1.9.1/zhmcclient/_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/testutils/__init__.py` & `zhmcclient-1.9.1/zhmcclient/testutils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/testutils/_cpc_fixtures.py` & `zhmcclient-1.9.1/zhmcclient/testutils/_cpc_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition.py` & `zhmcclient-1.9.1/zhmcclient/testutils/_hmc_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definition_fixtures.py` & `zhmcclient-1.9.1/zhmcclient/testutils/_hmc_definition_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_definitions.py` & `zhmcclient-1.9.1/zhmcclient/testutils/_hmc_definitions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_inventory_file.py` & `zhmcclient-1.9.1/zhmcclient/testutils/_hmc_inventory_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient/testutils/_hmc_vault_file.py` & `zhmcclient-1.9.1/zhmcclient/testutils/_hmc_vault_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient.egg-info/PKG-INFO` & `zhmcclient-1.9.1/zhmcclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.9.0
+Version: 1.9.1
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.9.0/zhmcclient.egg-info/SOURCES.txt` & `zhmcclient-1.9.1/zhmcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient.egg-info/requires.txt` & `zhmcclient-1.9.1/zhmcclient.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,20 +20,25 @@
 [:python_version == "2.7"]
 decorator<5.0,>=4.0.11
 
 [:python_version >= "3.10"]
 pytz>=2019.1
 six>=1.16.0
 
+[:python_version >= "3.12"]
+PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1
+
 [:python_version >= "3.5"]
 decorator>=4.0.11
 
 [:python_version >= "3.6"]
 stomp.py!=6.1.0,!=6.1.1,<7.0.0,>=4.1.23
-PyYAML>=5.4
+
+[:python_version >= "3.6" and python_version <= "3.11"]
+PyYAML!=5.4.0,!=5.4.1,>=5.3.1
 
 [:python_version >= "3.7"]
 requests>=2.31.0
 
 [testutils]
 
 [testutils:python_version == "2.7"]
```

### Comparing `zhmcclient-1.9.0/zhmcclient_mock/__init__.py` & `zhmcclient-1.9.1/zhmcclient_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient_mock/_hmc.py` & `zhmcclient-1.9.1/zhmcclient_mock/_hmc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient_mock/_idpool.py` & `zhmcclient-1.9.1/zhmcclient_mock/_idpool.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient_mock/_session.py` & `zhmcclient-1.9.1/zhmcclient_mock/_session.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.9.0/zhmcclient_mock/_urihandler.py` & `zhmcclient-1.9.1/zhmcclient_mock/_urihandler.py`

 * *Files identical despite different names*

