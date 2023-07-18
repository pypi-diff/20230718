# Comparing `tmp/stytch-7.0.0.tar.gz` & `tmp/stytch-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-7.0.0.tar", last modified: Mon Jul 17 17:51:51 2023, max compression
+gzip compressed data, was "stytch-7.0.1.tar", last modified: Tue Jul 18 15:37:49 2023, max compression
```

## Comparing `stytch-7.0.0.tar` & `stytch-7.0.1.tar`

### file list

```diff
@@ -1,67 +1,107 @@
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.610122 stytch-7.0.0/
--rw-r--r--   0 gorel      (501) staff       (20)     1059 2022-12-06 17:10:39.000000 stytch-7.0.0/LICENSE.txt
--rw-r--r--   0 gorel      (501) staff       (20)     5142 2023-07-17 17:51:51.610184 stytch-7.0.0/PKG-INFO
--rw-r--r--   0 gorel      (501) staff       (20)     4367 2023-04-20 19:06:08.000000 stytch-7.0.0/README.md
--rw-r--r--   0 gorel      (501) staff       (20)      110 2023-07-17 17:51:51.610404 stytch-7.0.0/setup.cfg
--rw-r--r--   0 gorel      (501) staff       (20)     1739 2022-12-16 21:16:07.000000 stytch-7.0.0/setup.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.601994 stytch-7.0.0/stytch/
--rw-r--r--   0 gorel      (501) staff       (20)      181 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/__init__.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.602757 stytch-7.0.0/stytch/b2b/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.605898 stytch-7.0.0/stytch/b2b/api/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)      892 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)     7036 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)    21373 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)     8980 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 gorel      (501) staff       (20)     2833 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)    16783 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     5807 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)    31415 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)    22509 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 gorel      (501) staff       (20)    22270 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 gorel      (501) staff       (20)    18614 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     8525 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 gorel      (501) staff       (20)     3439 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 gorel      (501) staff       (20)    19582 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)    11114 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sso.py
--rw-r--r--   0 gorel      (501) staff       (20)    10786 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 gorel      (501) staff       (20)    10369 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 gorel      (501) staff       (20)     1423 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/client.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.608427 stytch-7.0.0/stytch/b2b/models/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)     1452 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)     1159 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)     2325 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)     1712 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 gorel      (501) staff       (20)     1674 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)     1536 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 gorel      (501) staff       (20)      431 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)    11086 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)     2938 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 gorel      (501) staff       (20)     5719 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 gorel      (501) staff       (20)     1883 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     1149 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 gorel      (501) staff       (20)      957 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 gorel      (501) staff       (20)     3802 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)     3314 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sso.py
--rw-r--r--   0 gorel      (501) staff       (20)     1400 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 gorel      (501) staff       (20)     1307 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/b2b/models/sso_saml.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.609203 stytch-7.0.0/stytch/core/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2022-12-16 21:16:07.000000 stytch-7.0.0/stytch/core/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)      586 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/core/api_base.py
--rw-r--r--   0 gorel      (501) staff       (20)     1210 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/core/client_base.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.609454 stytch-7.0.0/stytch/core/http/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2022-12-20 16:48:17.000000 stytch-7.0.0/stytch/core/http/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)     3605 2023-06-05 21:01:43.000000 stytch-7.0.0/stytch/core/http/client.py
--rw-r--r--   0 gorel      (501) staff       (20)     2106 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/core/response_base.py
--rw-r--r--   0 gorel      (501) staff       (20)       22 2023-07-17 16:16:44.000000 stytch-7.0.0/stytch/version.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.602556 stytch-7.0.0/stytch.egg-info/
--rw-r--r--   0 gorel      (501) staff       (20)     5142 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 gorel      (501) staff       (20)     1776 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 gorel      (501) staff       (20)        1 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 gorel      (501) staff       (20)       69 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/requires.txt
--rw-r--r--   0 gorel      (501) staff       (20)        7 2023-07-17 17:51:51.000000 stytch-7.0.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-17 17:51:51.609961 stytch-7.0.0/test/
--rw-r--r--   0 gorel      (501) staff       (20)     9527 2023-07-17 16:16:44.000000 stytch-7.0.0/test/test_integration.py
--rw-r--r--   0 gorel      (501) staff       (20)    12747 2023-07-17 16:16:44.000000 stytch-7.0.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.457611 stytch-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-18 15:37:32.000000 stytch-7.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-18 15:37:49.457611 stytch-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-18 15:37:32.000000 stytch-7.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 15:37:49.457611 stytch-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-18 15:37:32.000000 stytch-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.441612 stytch-7.0.1/stytch/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.441612 stytch-7.0.1/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.449612 stytch-7.0.1/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31415 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22509 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.453611 stytch-7.0.1/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/b2b/models/sso_saml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.453611 stytch-7.0.1/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.453611 stytch-7.0.1/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32410 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28091 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.457611 stytch-7.0.1/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.457611 stytch-7.0.1/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.457611 stytch-7.0.1/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:37:32.000000 stytch-7.0.1/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.441612 stytch-7.0.1/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-18 15:37:49.000000 stytch-7.0.1/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-18 15:37:49.000000 stytch-7.0.1/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:37:49.000000 stytch-7.0.1/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 15:37:49.000000 stytch-7.0.1/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 15:37:49.000000 stytch-7.0.1/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:37:49.457611 stytch-7.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-18 15:37:32.000000 stytch-7.0.1/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-07-18 15:37:32.000000 stytch-7.0.1/test/test_integration_async.py
```

### Comparing `stytch-7.0.0/LICENSE.txt` & `stytch-7.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/PKG-INFO` & `stytch-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.0.0
+Version: 7.0.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-7.0.0/README.md` & `stytch-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/setup.py` & `stytch-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/discovery.py` & `stytch-7.0.1/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-7.0.1/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/discovery_organizations.py` & `stytch-7.0.1/stytch/b2b/api/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/magic_links.py` & `stytch-7.0.1/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-7.0.1/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/magic_links_email.py` & `stytch-7.0.1/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-7.0.1/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/organizations.py` & `stytch-7.0.1/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/organizations_members.py` & `stytch-7.0.1/stytch/b2b/api/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/passwords.py` & `stytch-7.0.1/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/passwords_email.py` & `stytch-7.0.1/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-7.0.1/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/passwords_session.py` & `stytch-7.0.1/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/sessions.py` & `stytch-7.0.1/stytch/b2b/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/sso.py` & `stytch-7.0.1/stytch/b2b/api/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/sso_oidc.py` & `stytch-7.0.1/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/api/sso_saml.py` & `stytch-7.0.1/stytch/b2b/api/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/client.py` & `stytch-7.0.1/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/discovery.py` & `stytch-7.0.1/stytch/b2b/models/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-7.0.1/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/discovery_organizations.py` & `stytch-7.0.1/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/magic_links.py` & `stytch-7.0.1/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-7.0.1/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/magic_links_email.py` & `stytch-7.0.1/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/organizations.py` & `stytch-7.0.1/stytch/b2b/models/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/organizations_members.py` & `stytch-7.0.1/stytch/b2b/models/organizations_members.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/passwords.py` & `stytch-7.0.1/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/passwords_email.py` & `stytch-7.0.1/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-7.0.1/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/passwords_session.py` & `stytch-7.0.1/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/sessions.py` & `stytch-7.0.1/stytch/b2b/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/sso.py` & `stytch-7.0.1/stytch/b2b/models/sso.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/sso_oidc.py` & `stytch-7.0.1/stytch/b2b/models/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/b2b/models/sso_saml.py` & `stytch-7.0.1/stytch/b2b/models/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/core/api_base.py` & `stytch-7.0.1/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/core/client_base.py` & `stytch-7.0.1/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/core/http/client.py` & `stytch-7.0.1/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch/core/response_base.py` & `stytch-7.0.1/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/stytch.egg-info/PKG-INFO` & `stytch-7.0.1/stytch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.0.0
+Version: 7.0.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-7.0.0/test/test_integration.py` & `stytch-7.0.1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.0/test/test_integration_async.py` & `stytch-7.0.1/test/test_integration_async.py`

 * *Files identical despite different names*

