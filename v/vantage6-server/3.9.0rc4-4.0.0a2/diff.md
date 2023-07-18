# Comparing `tmp/vantage6-server-3.9.0rc4.tar.gz` & `tmp/vantage6-server-4.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-3.9.0rc4.tar", last modified: Wed May 24 09:34:10 2023, max compression
+gzip compressed data, was "vantage6-server-4.0.0a2.tar", last modified: Tue Jul 18 13:32:09 2023, max compression
```

## Comparing `vantage6-server-3.9.0rc4.tar` & `vantage6-server-4.0.0a2.tar`

### file list

```diff
@@ -1,89 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/tests_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   100933 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    25405 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/node_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/server_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/testnodeconfiguration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.433729 vantage6-server-3.9.0rc4/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.433729 vantage6-server-3.9.0rc4/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.433729 vantage6-server-3.9.0rc4/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/common/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    26260 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    26410 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.496687 vantage6-server-4.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-18 13:32:09.496687 vantage6-server-4.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:32:09.496687 vantage6-server-4.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.488687 vantage6-server-4.0.0a2/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139499 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.488687 vantage6-server-4.0.0a2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.488687 vantage6-server-4.0.0a2/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    24701 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.488687 vantage6-server-4.0.0a2/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.492687 vantage6-server-4.0.0a2/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.492687 vantage6-server-4.0.0a2/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.492687 vantage6-server-4.0.0a2/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.492687 vantage6-server-4.0.0a2/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.492687 vantage6-server-4.0.0a2/vantage6/server/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/task_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.496687 vantage6-server-4.0.0a2/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.496687 vantage6-server-4.0.0a2/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/common/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/common/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/common/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18896 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28270 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22580 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32644 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-18 13:31:55.000000 vantage6-server-4.0.0a2/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:09.496687 vantage6-server-4.0.0a2/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-18 13:32:09.000000 vantage6-server-4.0.0a2/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-18 13:32:09.000000 vantage6-server-4.0.0a2/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:32:09.000000 vantage6-server-4.0.0a2/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 13:32:09.000000 vantage6-server-4.0.0a2/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 13:32:09.000000 vantage6-server-4.0.0a2/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 13:32:09.000000 vantage6-server-4.0.0a2/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-3.9.0rc4/PKG-INFO` & `vantage6-server-4.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a2 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.9.0rc4/setup.py` & `vantage6-server-4.0.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,17 @@
         'Flask-RESTful==0.3.9',
         'flask-marshmallow==0.14.0',
         'Flask-SocketIO==5.3.2',
         'gevent==22.10.2',
         'ipython==8.10.0',
         'jinja2==3.1.2',
         'kombu==5.2.4',
-        'marshmallow==2.16.3',
-        'marshmallow-sqlalchemy==0.15.0',
+        'marshmallow==3.19.0',
+        'marshmallow-sqlalchemy==0.29.0',
+        'PyJWT==2.6.0',
         'pyotp==2.8.0',
         'questionary==1.10.0',
         'requests==2.31.0',
         'requests-oauthlib==1.3.1',
         'schema==0.7.5',
         'SQLAlchemy==1.4.46',
         'werkzeug==2.3.4',
```

### Comparing `vantage6-server-3.9.0rc4/tests_server/test_models.py` & `vantage6-server-4.0.0a2/tests_server/test_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from vantage6.server import session
 from vantage6.server.model import (
     User,
     Organization,
     Collaboration,
     Task,
-    Result,
+    Run,
     Node,
     Rule,
     Role
 )
 from vantage6.server.model.rule import Scope, Operation
 
 
@@ -221,71 +221,71 @@
         for organization in Organization.get():
             for node in organization.nodes:
                 self.assertIsInstance(node, Node)
             for collaboration in organization.collaborations:
                 self.assertIsInstance(collaboration, Collaboration)
             for user in organization.users:
                 self.assertIsInstance(user, User)
-            for result in organization.results:
-                self.assertIsInstance(result, Result)
+            for run in organization.runs:
+                self.assertIsInstance(run, Run)
 
 
-class TestResultModel(TestBaseModel):
+class TestRunModel(TestBaseModel):
 
     def test_read(self):
-        for result in Result.get():
-            self.assertIsInstance(result, Result)
-            self.assertIsNone(result.result)
-            self.assertIsInstance(result.assigned_at, datetime.datetime)
-            self.assertIsNone(result.started_at)
-            self.assertIsNone(result.finished_at)
+        for run in Run.get():
+            self.assertIsInstance(run, Run)
+            self.assertIsNone(run.result)
+            self.assertIsInstance(run.assigned_at, datetime.datetime)
+            self.assertIsNone(run.started_at)
+            self.assertIsNone(run.finished_at)
 
     def test_insert(self):
         task = Task(name="unit_task")
-        result = Result(
+        run = Run(
             task=task,
             organization=Organization.get()[0],
             input="something"
         )
-        result.save()
-        self.assertEqual(result, result)
+        run.save()
+        self.assertEqual(run, run)
 
-    def test_methods(self):
-        for result in Result.get():
-            self.assertFalse(result.complete)
+    # def test_methods(self):
+    #     for result in Result.get():
+    #         self.assertFalse(result.complete)
 
     def test_relations(self):
-        result = Result.get()[0]
-        self.assertIsInstance(result.organization, Organization)
-        for user in result.organization.users:
+        run = Run.get()[0]
+        self.assertIsInstance(run.organization, Organization)
+        for user in run.organization.users:
             self.assertIsInstance(user, User)
-        self.assertIsInstance(result.task, Task)
+        self.assertIsInstance(run.task, Task)
 
 
 class TestTaskModel(TestBaseModel):
 
     def test_read(self):
         db_tasks = Task.get()
         for task in db_tasks:
             self.assertIsInstance(task, Task)
             self.assertIsInstance(task.name, str)
             # self.assertIsInstance(task.description, str)
             self.assertIsInstance(task.image, str)
             self.assertIsInstance(task.collaboration, Collaboration)
-            self.assertIsInstance(task.run_id, int)
+            self.assertIsInstance(task.job_id, int)
             # self.assertIsInstance(task.database, str)
-            for result in task.results:
-                self.assertIsInstance(result, Result)
+            for run in task.runs:
+                self.assertIsInstance(run, Run)
 
     def test_insert(self):
         task = Task(
             name="unit_task",
             image="some-image",
             collaboration=Collaboration.get()[0],
-            run_id=1
+            job_id=1
         )
         task.save()
         db_task = None
         for task in Task.get():
             if task.name == "unit_task":
                 db_task = task
                 break
@@ -298,18 +298,16 @@
                 highest_id = task.id
 
     def test_relations(self):
         db_task = Task.get()
         for task in db_task:
             self.assertIsInstance(task, Task)
             self.assertIsInstance(task.collaboration, Collaboration)
-            for result in task.results:
-                self.assertIsInstance(result, Result)
-            for result in task.results:
-                self.assertIsInstance(result, Result)
+            for run in task.runs:
+                self.assertIsInstance(run, Run)
             for user in task.collaboration.organizations[0].users:
                 self.assertIsInstance(user, User)
 
 
 class TestRuleModel(TestBaseModel):
 
     def test_read(self):
```

### Comparing `vantage6-server-3.9.0rc4/tests_server/test_resources.py` & `vantage6-server-4.0.0a2/tests_server/test_resources.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-import datetime
 from uuid import uuid1
 import yaml
 import unittest
 import logging
 import json
 import uuid
 
@@ -12,18 +11,19 @@
 from flask import Response as BaseResponse
 from flask.testing import FlaskClient
 from flask_socketio import SocketIO
 from werkzeug.utils import cached_property
 
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
+from vantage6.common.task_status import TaskStatus
 from vantage6.server.globals import PACKAGE_FOLDER
 from vantage6.server import ServerApp, session
 from vantage6.server.model import (Rule, Role, Organization, User, Node,
-                                   Collaboration, Task, Result)
+                                   Collaboration, Task, Run)
 from vantage6.server.model.rule import Scope, Operation
 from vantage6.server import context
 from vantage6.server._version import __version__
 from vantage6.server.model.base import Database, DatabaseSessionManager
 from vantage6.server.controller.fixture import load
 
 
@@ -118,15 +118,15 @@
             print('something wrong, during login:')
             print(tokens)
             return None
 
     def create_user(self, organization=None, rules=[], password="password"):
 
         if not organization:
-            organization = Organization(name="some-organization")
+            organization = Organization(name=str(uuid.uuid1()))
             organization.save()
 
         # user details
         username = str(uuid.uuid1())
 
         # create a temporary organization
         user = User(username=username, password=password,
@@ -139,18 +139,18 @@
             "password": password
         }
 
         return user
 
     def create_node(self, organization=None, collaboration=None):
         if not organization:
-            organization = Organization()
+            organization = Organization(name=str(uuid.uuid1()))
 
         if not collaboration:
-            collaboration = Collaboration()
+            collaboration = Collaboration(name=str(uuid.uuid1()))
 
         api_key = str(uuid1())
         node = Node(
             name=str(uuid1()),
             api_key=api_key,
             organization=organization,
             collaboration=collaboration
@@ -173,28 +173,28 @@
 
         return headers
 
     def login_container(self, collaboration=None, organization=None,
                         node=None, task=None, api_key=None):
         if not node:
             if not collaboration:
-                collaboration = Collaboration()
+                collaboration = Collaboration(name=str(uuid.uuid1()))
             if not organization:
-                organization = Organization()
+                organization = Organization(name=str(uuid.uuid1()))
             api_key = str(uuid1())
             node = Node(organization=organization, collaboration=collaboration,
                         api_key=api_key)
             node.save()
         else:
             collaboration = node.collaboration
             organization = node.organization
 
         if not task:
             task = Task(image="some-image", collaboration=collaboration,
-                        results=[Result()])
+                        runs=[Run(status=TaskStatus.PENDING)])
             task.save()
 
         headers = self.login_node(api_key)
         tokens = self.app.post('/api/token/container', headers=headers, json={
             "image": "some-image",
             "task_id": task.id
         }
@@ -204,14 +204,56 @@
             print(tokens['msg'])
 
         headers = {
             'Authorization': 'Bearer {}'.format(tokens['container_token'])
         }
         return headers
 
+    def paginated_list(
+        self, url: str, headers: dict = None
+    ) -> tuple[Response, list]:
+        """
+        Get all resources of a list endpoint by browsing through all pages
+
+        Parameters
+        ----------
+        url: str
+            The url of the list endpoint
+        headers: dict
+            The headers to use for the request
+        kwargs: dict
+            Additional arguments to pass to the request
+
+        Returns
+        -------
+        tuple[flask.Response, list]
+            The response and the list of all resources
+        """
+        result = self.app.get(url, headers=headers)
+
+        # check if response is OK
+        if result.status_code != HTTPStatus.OK:
+            return result, []
+
+        # get data
+        links = result.json.get('links')
+        page = 1
+        json_data = result.json.get('data')
+        if json_data is None:
+            json_data = []
+        while links and links.get('next'):
+            page += 1
+            new_response = self.app.get(
+                links.get('next'), headers=headers
+            )
+            json_data += new_response.json.get('data') \
+                if new_response.json.get('data') else []
+            links = new_response.json.get('links')
+        return result, json_data
+
     def create_node_and_login(self, *args, **kwargs):
         node, api_key = self.create_node(*args, **kwargs)
         return self.login_node(api_key)
 
     def create_user_and_login(self, organization=None, rules=[]):
         user = self.create_user(organization, rules)
         return self.login(user.username)
@@ -234,15 +276,15 @@
     def test_organization(self):
 
         rule = Rule.get_by_("organization", Scope.GLOBAL,
                             Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
 
         # First retrieve a list of all organizations
-        orgs = self.app.get('/api/organization', headers=headers).json
+        _response, orgs = self.paginated_list('/api/organization', headers)
         self.assertEqual(len(orgs), len(Organization.get()))
 
         attrs = [
             'id',
             'name',
             'domain',
             'name',
@@ -288,22 +330,22 @@
         headers = self.create_user_and_login(organization=org, rules=[rule])
 
         collaborations = self.app.get(
             '/api/collaboration', headers=headers
         )
         self.assertEqual(collaborations.status_code, HTTPStatus.OK)
         db_cols = Collaboration.get()
-        self.assertEqual(len(collaborations.json), len(db_cols))
+        self.assertEqual(len(collaborations.json['data']), len(db_cols))
 
     def test_node_without_id(self):
 
         # GET
         rule = Rule.get_by_("node", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        nodes = self.app.get("/api/node", headers=headers).json
+        nodes = self.app.get("/api/node", headers=headers).json['data']
         expected_fields = [
             'name',
             'collaboration',
             'organization',
             'status',
             'id',
             'type',
@@ -325,15 +367,15 @@
             "collaboration_id": 99999
         })
         response_json = response.json
         self.assertIn("msg", response_json)
         self.assertEqual(response.status_code, HTTPStatus.NOT_FOUND)
 
         # succesfully create a node
-        org = Organization()
+        org = Organization(name=str(uuid.uuid1()))
         col = Collaboration(organizations=[org])
         col.save()
 
         headers = self.create_user_and_login(org, rules=[rule])
         response = self.app.post("/api/node", headers=headers, json={
             "collaboration_id": col.id
         })
@@ -365,54 +407,50 @@
 
         # some nodes just don't exist
         node = self.app.get("/api/node/9999", headers=headers)
         self.assertEqual(node.status_code, 404)
 
     def test_result_with_id(self):
         headers = self.login("root")
-        result = self.app.get("/api/result/1", headers=headers)
-        self.assertEqual(result.status_code, 200)
+        run = self.app.get("/api/run/1", headers=headers)
+        self.assertEqual(run.status_code, 200)
 
-        result = self.app.get("/api/result/1?include=task", headers=headers)
-        self.assertEqual(result.status_code, 200)
+        run = self.app.get("/api/run/1?include=task", headers=headers)
+        self.assertEqual(run.status_code, 200)
 
-    def test_result_without_id(self):
+    def test_run_without_id(self):
         headers = self.login("root")
-        result1 = self.app.get("/api/result", headers=headers)
+        result1 = self.app.get("/api/run", headers=headers)
         self.assertEqual(result1.status_code, 200)
 
-        result2 = self.app.get("/api/result?state=open&&node_id=1",
+        result2 = self.app.get("/api/run?state=open",
                                headers=headers)
         self.assertEqual(result2.status_code, 200)
 
-        result3 = self.app.get("/api/result?task_id=1", headers=headers)
+        result3 = self.app.get("/api/run?task_id=1", headers=headers)
         self.assertEqual(result3.status_code, 200)
 
-        result4 = self.app.get("/api/result?task_id=1&&node_id=1",
-                               headers=headers)
-        self.assertEqual(result4.status_code, 200)
-
     def test_stats(self):
         headers = self.login("root")
-        result = self.app.get("/api/result", headers=headers)
+        result = self.app.get("/api/run", headers=headers)
         self.assertEqual(result.status_code, 200)
 
     def test_task_with_id(self):
         headers = self.login("root")
         result = self.app.get("/api/task/1", headers=headers)
         self.assertEqual(result.status_code, 200)
 
     def test_task_witout_id(self):
         headers = self.login("root")
         result = self.app.get("/api/task", headers=headers)
         self.assertEqual(result.status_code, 200)
 
-    def test_task_including_results(self):
+    def test_task_including_runs(self):
         headers = self.login("root")
-        result = self.app.get("/api/task?include=results", headers=headers)
+        result = self.app.get("/api/task?include=runs", headers=headers)
         self.assertEqual(result.status_code, 200)
 
     def test_task_unknown(self):
         headers = self.login("root")
         result = self.app.get("/api/task/9999", headers=headers)
         self.assertEqual(result.status_code, 404)
 
@@ -549,16 +587,16 @@
         result = self.app.patch("/api/password/change", headers=headers, json={
             "new_password": "a_new_password"
         })
         self.assertEqual(result.status_code, 400)
 
         # test if fails when wrong password is provided
         result = self.app.patch("/api/password/change", headers=headers, json={
-            "current_password": "wrong_password1!",
-            "new_password": "a_new_password"
+            "current_password": "Wrong_password1!",
+            "new_password": "A_new_password1!"
         })
         self.assertEqual(result.status_code, 401)
 
         # test if fails when new password is the same
         result = self.app.patch("/api/password/change", headers=headers, json={
             "current_password": "Password1!",
             "new_password": "Password1!"
@@ -580,24 +618,119 @@
         self.assertEqual(result.status_code, 200)
 
     def test_view_roles(self):
         headers = self.login("root")
         result = self.app.get("/api/role", headers=headers)
         self.assertEqual(result.status_code, 200)
 
-        body = result.json
+        body = result.json['data']
         expected_fields = ['organization', 'name', 'description', 'users']
         for field in expected_fields:
             self.assertIn(field, body[0])
 
+    def test_view_role_permissions(self):
+        org = Organization()
+        org.save()
+        other_org = Organization()
+        other_org.save()
+        col = Collaboration(organizations=[org, other_org])
+        col.save()
+        org_outside_collab = Organization()
+        org_outside_collab.save()
+
+        # non-existing role
+        headers = self.login('root')
+        result = self.app.get("/api/role/9999", headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
+
+        # root user can view all roles
+        result, json_data = self.paginated_list('/api/role', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+        self.assertEqual(len(json_data), len(Role.get()))
+
+        role = Role(organization=org)
+        role.save()
+
+        # without permissions should allow you to view your own roles, which
+        # in this case is an empty list
+        headers = self.create_user_and_login()
+        result, json_data = self.paginated_list('/api/role', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+        self.assertEqual(len(json_data), 0)
+
+        # view roles of your organization
+        rule = Rule.get_by_("role", Scope.ORGANIZATION, Operation.VIEW)
+        headers = self.create_user_and_login(org, rules=[rule])
+        result, json_data = self.paginated_list('/api/role', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # +3 for the root, container and node roles (other default roles are
+        # not generated for unit tests)
+        self.assertEqual(len(json_data), len(org.roles) + 3)
+
+        # view a single role of your organization
+        result = self.app.get(f'/api/role/{role.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # check that user of other organization cannot view roles with
+        # organization scope
+        headers = self.create_user_and_login(other_org, rules=[rule])
+        result = self.app.get(
+            '/api/role', headers=headers,
+            query_string={'organization_id': org.id}
+        )
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # user can view their own roles. This should always be possible
+        user = self.create_user(rules=[])
+        headers = self.login(user.username)
+        result = self.app.get('/api/role', headers=headers, query_string={
+            'user_id': user.id
+        })
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # collaboration permission - in same collaboration with id
+        rule = Rule.get_by_("role", Scope.COLLABORATION, Operation.VIEW)
+        headers = self.create_user_and_login(other_org, rules=[rule])
+        result = self.app.get(f"/api/role/{role.id}", headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # collaboration permission - in same collaboration without id
+        result, json_data = self.paginated_list('/api/role', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+        # +3 for the root, container and node roles (other default roles are
+        # not generated for unit tests)
+        self.assertEqual(len(json_data), len([
+            role_ for org in col.organizations for role_ in org.roles
+        ]) + 3)
+
+        # collaboration permission - in different collaboration with id
+        headers = self.create_user_and_login(org_outside_collab, rules=[rule])
+        result = self.app.get(f"/api/role/{role.id}", headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # collaboration permission - in different collaboration without id
+        result = self.app.get('/api/role', headers=headers,
+                              query_string={'collaboration_id': col.id})
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
+        org.delete()
+        other_org.delete()
+        org_outside_collab.delete()
+        col.delete()
+        role.delete()
+        user.delete()
+
     def test_create_role_as_root(self):
         headers = self.login("root")
 
         # obtain available rules
-        rules = self.app.get("/api/rule", headers=headers).json
+        rules = self.app.get("/api/rule", headers=headers,
+                             query_string={'no_pagination': 1}).json['data']
         rule_ids = [rule.get("id") for rule in rules]
 
         # assign first two rules to role
         body = {
             "name": "some-role-name",
             "description": "Testing if we can create a role",
             "rules": rule_ids[:2]
@@ -608,22 +741,26 @@
 
         # check that server responded ok
         self.assertEqual(result.status_code, HTTPStatus.CREATED)
 
         # verify the values
         self.assertEqual(result.json.get("name"), body["name"])
         self.assertEqual(result.json.get("description"), body["description"])
-        self.assertEqual(len(result.json.get("rules")), 2)
+        result = self.app.get(
+            "/api/rule", headers=headers,
+            query_string={'role_id': result.json.get("id")}
+        )
+        self.assertEqual(len(result.json.get('data')), 2)
 
     def test_create_role_as_root_for_different_organization(self):
         headers = self.login("root")
 
         # obtain available rules
-        rules = self.app.get("/api/rule", headers=headers).json
-
+        rules = self.app.get("/api/rule", headers=headers,
+                             query_string={'no_pagination': 1}).json['data']
         # create new organization, so we're sure that the current user
         # is not assigned to the same organization
         org = Organization(name="Some-random-organization")
         org.save()
 
         body = {
             "name": "some-role-name",
@@ -645,20 +782,19 @@
         all_rules = Rule.get()
 
         # check user without any permissions
         headers = self.create_user_and_login()
 
         body = {
             "name": "some-role-name",
-            "description": "Testing if we can create a rol for another org",
+            "description": "Testing if we can create a role for another org",
             "rules": [rule.id for rule in all_rules],
         }
         result = self.app.post("/api/role", headers=headers, json=body)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
-
         # check that user with a missing rule cannot create a role with that
         # missing rule
         headers = self.create_user_and_login(rules=(all_rules[:-2]))
         result = self.app.post("/api/role", headers=headers, json=body)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # check that user can create role within his organization
@@ -679,14 +815,36 @@
 
         # check that assigning an unexisting rule is not possible
         headers = self.create_user_and_login()
         body["rules"] = [9999]
         result = self.app.post("/api/role", headers=headers, json=body)
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
 
+        # check creating role inside the collaboration
+        org1 = Organization()
+        org1.save()
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org1, org2])
+        col.save()
+        rule = Rule.get_by_("role", scope=Scope.COLLABORATION,
+                            operation=Operation.CREATE)
+        headers = self.create_user_and_login(organization=org1, rules=[rule])
+        body["rules"] = [rule.id]
+        body["organization_id"] = org2.id
+        result = self.app.post("/api/role", headers=headers, json=body)
+        self.assertEqual(result.status_code, HTTPStatus.CREATED)
+
+        # check creating role outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        body["organization_id"] = org3.id
+        result = self.app.post("/api/role", headers=headers, json=body)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
     def test_edit_role(self):
         headers = self.login('root')
 
         # create testing entities
         org = Organization(name="some-organization-name")
         org.save()
         role = Role(name="some-role-name", organization=org)
@@ -733,14 +891,37 @@
         rule = Rule.get_by_("role", Scope.GLOBAL, Operation.EDIT)
         headers = self.create_user_and_login(org2, [rule])
         result = self.app.patch(f'/api/role/{role.id}', headers=headers, json={
             "name": "this-will-not-be-updated"
         })
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
+        # test editing role inside the collaboration
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        rule = Rule.get_by_("role", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        result = self.app.patch(f"/api/role/{role.id}", headers=headers, json={
+            "name": "new-role-name",
+        })
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # check editing role outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        role = Role(name="some-role-name", organization=org3)
+        role.save()
+        result = self.app.patch(f"/api/role/{role.id}", headers=headers, json={
+            "name": "this-will-not-be-updated"
+        })
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
     def test_remove_role(self):
 
         org = Organization()
         org.save()
         role = Role(organization=org)
         role.save()
 
@@ -765,36 +946,52 @@
 
         # test removal with global permissions
         rule = Rule.get_by_("role", Scope.GLOBAL, Operation.DELETE)
         headers = self.create_user_and_login(rules=[rule])
         result = self.app.delete(f'/api/role/{role.id}', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
-    def test_rules_from_role(self):
-        headers = self.login('root')
-        role = Role.get()[0]
+        # check removing role outside the collaboration fails
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        role = Role(organization=org)  # because we removed it...
+        role.save()
+
+        org3 = Organization()
+        org3.save()
+        rule = Rule.get_by_("role", Scope.COLLABORATION, Operation.DELETE)
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        result = self.app.delete(f"/api/role/{role.id}", headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
-        result = self.app.get(f'/api/role/{role.id}/rule', headers=headers)
+        # test removing role inside the collaboration
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        result = self.app.delete(f"/api/role/{role.id}", headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertEqual(len(role.rules), len(result.json))
 
-        result = self.app.get('/api/role/9999/rule', headers=headers)
-        self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
+        # cleanup
+        org3.delete()
+        org2.delete()
+        org.delete()
+        col.delete()
 
     def test_add_single_rule_to_role(self):
         headers = self.login('root')
 
         role = Role(name="empty", organization=Organization())
         role.save()
 
         # role without rules
-        result = self.app.get(f'/api/role/{role.id}/rule', headers=headers)
-
+        result, json_data = self.paginated_list(
+            f'/api/rule?role_id={role.id}', headers=headers
+        )
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertEqual(len(result.json), 0)
+        self.assertEqual(len(json_data), 0)
 
         rule = Rule.get()[0]
 
         # try to add rule to non existing role
         result = self.app.post(f'/api/role/9999/rule/{rule.id}',
                                headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
@@ -806,17 +1003,19 @@
 
         # add a rule to a role
         result = self.app.post(f'/api/role/{role.id}/rule/{rule.id}',
                                headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.CREATED)
 
         # check that the role now has one rule
-        result = self.app.get(f'/api/role/{role.id}/rule', headers=headers)
+        result, json_data = self.paginated_list(
+            f'/api/rule?role_id={role.id}', headers=headers
+        )
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertEqual(len(result.json), 1)
+        self.assertEqual(len(json_data), 1)
 
     def test_remove_single_rule_from_role(self):
         headers = self.login('root')
 
         rule = Rule.get()[0]
         role = Role(name="unit", organization=Organization(), rules=[rule])
         role.save()
@@ -827,51 +1026,29 @@
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
 
         # try to add non existent rule
         result = self.app.delete(f'/api/role/{role.id}/rule/9999',
                                  headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
 
-        result = self.app.get(f'/api/role/{role.id}/rule', headers=headers)
+        result, json_data = self.paginated_list(
+            f'/api/rule?role_id={role.id}', headers=headers
+        )
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertEqual(len(result.json), 1)
+        self.assertEqual(len(json_data), 1)
 
         result = self.app.delete(f'/api/role/{role.id}/rule/{rule.id}',
                                  headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
         self.assertEqual(len(result.json), 0)
 
-    def test_view_permission_rules(self):
-        rule = Rule.get_by_("role", Scope.ORGANIZATION, Operation.VIEW)
-
-        role = Role(name="some-role", organization=Organization())
-        role.save()
-
-        # user does not belong to organization
-        headers = self.create_user_and_login(rules=[rule])
-        result = self.app.get(f'/api/role/{role.id}/rule', headers=headers)
-        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
-
-        # user does belong to the organization
-        headers = self.create_user_and_login(organization=role.organization,
-                                             rules=[rule])
-        result = self.app.get(f'/api/role/{role.id}/rule', headers=headers)
-        self.assertEqual(result.status_code, HTTPStatus.OK)
-
-        # user has global permissions
-        rule = Rule.get_by_("role", Scope.GLOBAL, Operation.VIEW)
-        headers = self.create_user_and_login(rules=[rule])
-        result = self.app.get(f'/api/role/{role.id}/rule', headers=headers)
-        self.assertEqual(result.status_code, HTTPStatus.OK)
-
-        role.delete()
-
     def test_add_rule_to_role_permission(self):
-
-        role = Role(name="new-role", organization=Organization())
+        org = Organization()
+        org.save()
+        role = Role(name="new-role", organization=org)
         role.save()
 
         rule = Rule.get_by_("role", Scope.ORGANIZATION, Operation.EDIT)
 
         # try adding a rule without any permission
         headers = self.create_user_and_login()
         result = self.app.post(f'/api/role/{role.id}/rule/{rule.id}',
@@ -893,22 +1070,50 @@
 
         # however you can only assign rules that you own
         rule = Rule.get_by_("role", Scope.ORGANIZATION, Operation.EDIT)
         result = self.app.post(f'/api/role/{role.id}/rule/{rule.id}',
                                headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
+        # test inside the collaboration
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        rule = Rule.get_by_("role", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        result = self.app.post(f'/api/role/{role.id}/rule/{rule.id}',
+                               headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.CREATED)
+
+        # check outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        role2 = Role(name="some-role-name", organization=org3)
+        role2.save()
+        result = self.app.post(f'/api/role/{role2.id}/rule/{rule.id}',
+                               headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
         role.delete()
+        role2.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
 
     def test_remove_rule_from_role_permissions(self):
-
-        role = Role(name="new-role", organization=Organization())
+        org = Organization()
+        org.save()
+        role = Role(name="new-role", organization=org)
         role.save()
         rule = Rule.get_by_("role", Scope.ORGANIZATION,
-                            Operation.DELETE)
+                            Operation.EDIT)
 
         # try removing without any permissions
         headers = self.create_user_and_login()
         result = self.app.delete(f'/api/role/{role.id}/rule/{rule.id}',
                                  headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
@@ -916,16 +1121,15 @@
         headers = self.create_user_and_login(organization=Organization(),
                                              rules=[rule])
         result = self.app.delete(f'/api/role/{role.id}/rule/{rule.id}',
                                  headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # try removing rule which is not in the role
-        headers = self.create_user_and_login(organization=role.organization,
-                                             rules=[rule])
+        headers = self.create_user_and_login(organization=org, rules=[rule])
         result = self.app.delete(f'/api/role/{role.id}/rule/{rule.id}',
                                  headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
 
         role.rules.append(rule)
         role.save()
 
@@ -937,21 +1141,51 @@
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
         role.rules.append(rule)
         role.save()
 
         # power users can edit other organization rules
         power_rule = Rule.get_by_("role", Scope.GLOBAL,
-                                  Operation.DELETE)
+                                  Operation.EDIT)
         headers = self.create_user_and_login(rules=[power_rule, rule])
         result = self.app.delete(f'/api/role/{role.id}/rule/{rule.id}',
                                  headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
+        # test inside the collaboration
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        rule = Rule.get_by_("role", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        role.rules.append(rule)
+        role.save()
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        result = self.app.delete(f'/api/role/{role.id}/rule/{rule.id}',
+                                 headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # check outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        role2 = Role(name="some-role-name", organization=org3)
+        role2.rules.append(rule)
+        role2.save()
+        result = self.app.delete(f'/api/role/{role2.id}/rule/{rule.id}',
+                                 headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
         role.delete()
+        role2.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
 
     def test_view_permission_user(self):
 
         # user not found
         headers = self.create_user_and_login()
         result = self.app.get('/api/user/9999', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
@@ -959,35 +1193,79 @@
         # try to view users without any permissions
         headers = self.create_user_and_login()
         result = self.app.get('/api/user', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # root user can view all users
         headers = self.login('root')
-        result = self.app.get('/api/user', headers=headers)
+        result, json_data = self.paginated_list('/api/user', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertEqual(len(result.json), len(User.get()))
+        self.assertEqual(len(json_data), len(User.get()))
 
         # view users of your organization
         rule = Rule.get_by_("user", Scope.ORGANIZATION, Operation.VIEW)
-        org = Organization.get(1)
+        org = Organization()
+        org.save()
         headers = self.create_user_and_login(org, rules=[rule])
-        result = self.app.get('/api/user', headers=headers)
+        result, json_data = self.paginated_list('/api/user', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertEqual(len(result.json), len(org.users))
+        self.assertEqual(len(json_data), len(org.users))
 
         # view a single user of your organization
         user_id = org.users[0].id
         result = self.app.get(f'/api/user/{user_id}', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
         # user can view their own data. This should always be possible
         user = self.create_user(rules=[])
         headers = self.login(user.username)
         result = self.app.get(f'/api/user/{user.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # collaboration permission - view single user
+        org2 = Organization()
+        org2.save()
+        org3 = Organization()
+        org3.save()
+        col = Collaboration(organizations=[org2, org3])
+        col.save()
+        user = self.create_user(organization=org2, rules=[])
+        rule = Rule.get_by_("user", scope=Scope.COLLABORATION,
+                            operation=Operation.VIEW)
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        result = self.app.get(f'/api/user/{user.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # collaboration permission - view list of users
+        result = self.app.get('/api/user', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+        # expecting 2 users: 1 in org2 and the 1 in org3 which is logged in now
+        self.assertEqual(len(result.json['data']), 2)
+
+        # collaboration permission - viewing outside collaboration should fail
+        org_outside_col = Organization()
+        org_outside_col.save()
+        headers = self.create_user_and_login(organization=org_outside_col,
+                                             rules=[rule])
+        result = self.app.get(f'/api/user/{user.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # collaboration permission - viewing other collaborations should fail
+        result = self.app.get('/api/user', headers=headers, query_string={
+            'collaboration_id': col.id
+        })
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        org3.delete()
+        org_outside_col.delete()
+        col.delete()
+        user.delete()
 
     def test_bounce_existing_username_and_email(self):
         headers = self.create_user_and_login()
         User(username="something", email="mail@me.org").save()
         userdata = {
             "username": "not-important",
             "firstname": "name",
@@ -1030,26 +1308,63 @@
         # you need to own all rules in order to assign them
         headers = self.create_user_and_login(org, rules=[rule])
         userdata['username'] = 'smarty2'
         userdata['email'] = 'mail2@me.org'
         result = self.app.post('/api/user', headers=headers, json=userdata)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # you can only assign roles in which you have all rules
-        headers = self.create_user_and_login(org, rules=[rule])
+        # test inside the collaboration
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        rule = Rule.get_by_("user", scope=Scope.COLLABORATION,
+                            operation=Operation.CREATE)
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        userdata['username'] = 'smarty4'
+        userdata['email'] = 'mail4@me.org'
+        userdata['organization_id'] = org2.id
+        userdata['rules'] = [rule.id]
+        result = self.app.post('/api/user', headers=headers, json=userdata)
+        self.assertEqual(result.status_code, HTTPStatus.CREATED)
+
+        # check outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        userdata['username'] = 'smarty5'
+        userdata['email'] = 'mail5@me.org'
+        userdata['organization_id'] = org3.id
+        result = self.app.post('/api/user', headers=headers, json=userdata)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # you can only create users for in which you have all rules
+        rule_view_roles = Rule.get_by_(
+            "role", Scope.ORGANIZATION, Operation.VIEW)
+        headers = self.create_user_and_login(
+            org, rules=[rule, rule_view_roles])
         role = Role(rules=[rule], organization=org)
         role.save()
         userdata['username'] = 'smarty3'
         userdata['email'] = 'mail3@me.org'
         userdata['roles'] = [role.id]
         del userdata['organization_id']
         del userdata['rules']
         result = self.app.post('/api/user', headers=headers, json=userdata)
         self.assertEqual(result.status_code, HTTPStatus.CREATED)
-        self.assertEqual(len(result.json['roles']), 1)
+        # verify that user has the role
+        result = self.app.get('/api/role', headers=headers,
+                              query_string={'user_id': result.json['id']})
+        self.assertEqual(len(result.json['data']), 1)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
+        role.delete()
 
     def test_patch_user_permissions(self):
 
         org = Organization()
         user = User(firstname="Firstname", lastname="Lastname",
                     username="Username", password="Password", email="a@b.c",
                     organization=org)
@@ -1125,14 +1440,37 @@
             'lastname': 'and again',
         })
         session.session.refresh(user)
         self.assertEqual(result.status_code, HTTPStatus.OK)
         self.assertEqual("again", user.firstname)
         self.assertEqual("and again", user.lastname)
 
+        # test editing user inside the collaboration
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        rule2 = Rule.get_by_("user", scope=Scope.COLLABORATION,
+                             operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org2, rules=[rule2])
+        result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
+            'firstname': 'something',
+            'lastname': 'everything',
+        })
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # check editing outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        headers = self.create_user_and_login(organization=org3, rules=[rule2])
+        result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
+            'firstname': 'will-not-work',
+        })
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
         # test that you cannot assign rules that you not own
         not_owning_rule = Rule.get_by_("user", Scope.OWN,
                                        Operation.DELETE)
         headers = self.create_user_and_login(rules=[rule])
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
             'rules': [not_owning_rule.id]
         })
@@ -1156,41 +1494,54 @@
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test that you CAN change the rules. To do so, a user is generated
         # that has same rules as current user, but also rule to edit other
         # users and another one current user does not possess
         assigning_user_rules = user.rules
         assigning_user_rules.append(
-            Rule.get_by_("user", Scope.GLOBAL, Operation.EDIT)
+            Rule.get_by_("user", Scope.GLOBAL, Operation.EDIT),
         )
         assigning_user_rules.append(not_owning_rule)
         headers = self.create_user_and_login(rules=assigning_user_rules)
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
             'rules': [not_owning_rule.id, rule.id]
         })
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        user_rule_ids = [rule['id'] for rule in result.json['rules']]
+
+        result = self.app.get('/api/rule', headers=headers,
+                              query_string={'user_id': user.id})
+        user_rule_ids = [
+            rule['id'] for rule in result.json.get('data')
+        ]
         self.assertIn(not_owning_rule.id, user_rule_ids)
 
         # test that you cannot assign roles if you don't have all the
         # permissions for that role yourself (even though you have permission
         # to assign roles)
         headers = self.create_user_and_login(rules=[rule])
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
             'roles': [role.id]
         })
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test that you CAN assign roles
-        headers = self.create_user_and_login(rules=[rule, not_owning_rule])
+        rule_global_view = Rule.get_by_("role", Scope.GLOBAL, Operation.VIEW)
+        headers = self.create_user_and_login(
+            rules=[rule, not_owning_rule, rule_global_view]
+        )
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
             'roles': [role.id]
         })
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        user_role_ids = [role['id'] for role in result.json['roles']]
+
+        result = self.app.get('/api/role', headers=headers,
+                              query_string={'user_id': user.id})
+        user_role_ids = [
+            role['id'] for role in result.json.get('data')
+        ]
         self.assertIn(role.id, user_role_ids)
 
         # test that you CANNOT assign roles from different organization
         other_org_role = Role(name="somename", rules=[not_owning_rule],
                               organization=Organization())
         headers = self.create_user_and_login(rules=[rule, not_owning_rule])
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
@@ -1208,20 +1559,24 @@
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
             'rules': [9999]
         })
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
 
         user.delete()
         role.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
 
     def test_delete_user_permissions(self):
-
+        org = Organization()
         user = User(firstname="Firstname", lastname="Lastname",
                     username="Username", password="Password", email="a@b.c",
-                    organization=Organization())
+                    organization=org)
         user.save()
         self.credentials[user.username] = {'username': user.username,
                                            'password': "Password"}
 
         # check non-exsitsing user
         headers = self.create_user_and_login()
         result = self.app.delete('/api/user/9999', headers=headers)
@@ -1276,14 +1631,42 @@
         user.save()
         rule = Rule.get_by_("user", Scope.GLOBAL, Operation.DELETE)
         headers = self.create_user_and_login(rules=[rule])
         result = self.app.delete(f'/api/user/{user.id}', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
         # user is deleted by endpoint! user.delete()
 
+        # check delete outside the collaboration fails
+        user = User(firstname="Firstname", lastname="Lastname",
+                    username="Username", password="Password", email="a@b.c",
+                    organization=org)
+        user.save()
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        org3 = Organization()
+        org3.save()
+        rule = Rule.get_by_("user", Scope.COLLABORATION,
+                            Operation.DELETE)
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        result = self.app.delete(f'/api/user/{user.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test delete inside the collaboration
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        result = self.app.delete(f'/api/user/{user.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
+
     def test_view_organization_as_user_permissions(self):
 
         # view without any permissions
         headers = self.create_user_and_login()
         result = self.app.get('/api/organization', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
@@ -1300,34 +1683,56 @@
         org = Organization()
         org.save()
         result = self.app.get(f'/api/organization/{org.id}',
                               headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # Missing organization with global view
-        rule = Rule.get_by_("organization", Scope.GLOBAL,
-                            Operation.VIEW)
+        rule = Rule.get_by_("organization", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
         result = self.app.get('/api/organization/9999',
                               headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
 
         # test global view
-        result = self.app.get(f'/api/organization/{org.id}',
-                              headers=headers)
+        result = self.app.get(f'/api/organization/{org.id}', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
+        # test view inside the collaboration
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        rule = Rule.get_by_("organization", scope=Scope.COLLABORATION,
+                            operation=Operation.VIEW)
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        result = self.app.get(f'/api/organization/{org.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # check view outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        result = self.app.get(f'/api/organization/{org.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
+
     def test_view_organization_as_node_permission(self):
         node, api_key = self.create_node()
         headers = self.login_node(api_key)
 
         # test list organization with only your organization
         result = self.app.get('/api/organization', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertEqual(result.json[0]['id'], node.organization.id)
+        self.assertEqual(result.json['data'][0]['id'], node.organization.id)
 
         # test list organization
         result = self.app.get(
             f'/api/organization/{node.organization.id}',
             headers=headers
         )
         self.assertEqual(result.status_code, HTTPStatus.OK)
@@ -1348,15 +1753,15 @@
 
         # get all organizations in the collaboration
         result = self.app.get(
             '/api/organization',
             headers=headers
         )
         self.assertEqual(result.status_code, HTTPStatus.OK)
-        self.assertIsInstance(result.json, list)
+        self.assertIsInstance(result.json['data'], list)
 
         # cleanup
         node.delete()
 
     def test_create_organization_permissions(self):
 
         # try creating an organization without permissions
@@ -1376,22 +1781,23 @@
         self.assertEqual(result.status_code, HTTPStatus.CREATED)
         self.assertIsNotNone(Organization.get_by_name("this-is-gonna-happen"))
 
     def test_patch_organization_permissions(self):
 
         # unknown organization
         headers = self.create_user_and_login()
-        results = self.app.patch('/api/organization/9999', headers=headers)
+        results = self.app.patch('/api/organization/9999', headers=headers,
+                                 json={})
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
 
         # try to change anything without permissions
         org = Organization(name="first-name")
         org.save()
         results = self.app.patch(f'/api/organization/{org.id}',
-                                 headers=headers)
+                                 headers=headers, json={})
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # change as super user
         rule = Rule.get_by_("organization", Scope.GLOBAL,
                             Operation.EDIT)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.patch(f'/api/organization/{org.id}',
@@ -1401,128 +1807,163 @@
         self.assertEqual(results.status_code, HTTPStatus.OK)
         self.assertEqual(results.json['name'], "second-name")
 
         # change as organization editor
         rule = Rule.get_by_("organization", Scope.ORGANIZATION,
                             Operation.EDIT)
         headers = self.create_user_and_login(organization=org, rules=[rule])
-        results = self.app.patch(f'/api/organization/{org.id}',
-                                 headers=headers, json={
-                                     "name": "third-name"
-                                 })
+        results = self.app.patch(
+            f'/api/organization/{org.id}', headers=headers,
+            json={"name": "third-name"})
         self.assertEqual(results.status_code, HTTPStatus.OK)
         self.assertEqual(results.json['name'], "third-name")
 
         # change other organization as organization editor
         rule = Rule.get_by_("organization", Scope.ORGANIZATION,
                             Operation.EDIT)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.patch(f'/api/organization/{org.id}',
                                  headers=headers, json={
                                      "name": "third-name"
                                  })
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
+        # test editing organization inside the collaboration
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        rule2 = Rule.get_by_("organization", scope=Scope.COLLABORATION,
+                             operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org2, rules=[rule2])
+        results = self.app.patch(
+            f'/api/organization/{org.id}', headers=headers,
+            json={"name": "fourth-name"})
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # check editing outside the collaboration fails
+        org3 = Organization()
+        org3.save()
+        headers = self.create_user_and_login(organization=org3, rules=[rule2])
+        results = self.app.patch(
+            f'/api/organization/{org.id}', headers=headers,
+            json={"name": "not-going-to-happen"})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
     def test_organization_view_nodes(self):
 
         # create organization, collaboration and node
-        org = Organization()
+        org = Organization(name=str(uuid.uuid1()))
         org.save()
-        col = Collaboration(organizations=[org])
+        col = Collaboration(name=str(uuid.uuid1()), organizations=[org])
         col.save()
         node = Node(organization=org, collaboration=col)
         node.save()
 
         # try to view without permissions
         headers = self.create_user_and_login(org)
-        results = self.app.get(f"/api/organization/{org.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?organization_id={org.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # try to view with organization permissions
         rule = Rule.get_by_("node", Scope.ORGANIZATION, Operation.VIEW)
         headers = self.create_user_and_login(org, rules=[rule])
-        results = self.app.get(f"/api/organization/{org.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?organization_id={org.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # try to view other organization
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f"/api/organization/{org.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?organization_id={org.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # try to view with global permissions
         rule = Rule.get_by_("node", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f"/api/organization/{org.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?organization_id={org.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # try to view as node
         headers = self.create_node_and_login(organization=org)
-        results = self.app.get(f"/api/organization/{org.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?organization_id={org.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # try to view as node from another organization
         headers = self.create_node_and_login()
-        results = self.app.get(f"/api/organization/{org.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?organization_id={org.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # cleanup
         node.delete()
 
     def test_organization_view_collaboration_permissions(self):
 
         # test unknown organization
         org = Organization()
         org.save()
         col = Collaboration(organizations=[org])
         col.save()
 
         headers = self.create_user_and_login()
-        results = self.app.get('/api/organization/9999/collaboration',
-                               headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
 
-        # test view without any permission
-        results = self.app.get(f'/api/organization/{org.id}/collaboration',
-                               headers=headers)
+        # test that we can't view without permissions
+        results, json_data = self.paginated_list(
+            f'/api/collaboration?organization_id={org.id}', headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test view with organization scope
         rule = Rule.get_by_("collaboration", Scope.ORGANIZATION,
                             Operation.VIEW)
         headers = self.create_user_and_login(organization=org, rules=[rule])
-        results = self.app.get(f'/api/organization/{org.id}/collaboration',
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f'/api/collaboration?organization_id={org.id}', headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # test view with organization scope other organiation
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f'/api/organization/{org.id}/collaboration',
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f'/api/collaboration?organization_id={org.id}', headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test view with global scope
         rule = Rule.get_by_("collaboration", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f'/api/organization/{org.id}/collaboration',
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f'/api/collaboration?organization_id={org.id}', headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # test as node
         headers = self.create_node_and_login(organization=org,
                                              collaboration=col)
-        results = self.app.get(f'/api/organization/{org.id}/collaboration',
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f'/api/collaboration?organization_id={org.id}', headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
+        # test as node other organization - should not be permitted
+        results, json_data = self.paginated_list(
+            f'/api/collaboration?organization_id={org.id + 1}', headers=headers
+        )
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
     def test_view_collaboration_permissions(self):
 
         # setup organization and collaboration
         org = Organization()
         col = Collaboration(organizations=[org])
         col.save()
 
@@ -1587,14 +2028,43 @@
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.patch(f"/api/collaboration/{col.id}",
                                  headers=headers, json={
                                      "name": "this-is-gonna-fly"
                                  })
         self.assertEqual(results.status_code, HTTPStatus.OK)
         self.assertEqual(results.json["name"], "this-is-gonna-fly")
+        col.delete()
+
+        # test editing collaboration from within the collaboration
+        org = Organization()
+        org.save()
+        col = Collaboration(organizations=[org])
+        col.save()
+        rule = Rule.get_by_("collaboration", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        results = self.app.patch(
+            f'/api/collaboration/{col.id}', headers=headers,
+            json={"name": "some-name"})
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # check editing collaboration outside the collaboration fails without
+        # root access
+        org2 = Organization()
+        org2.save()
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        results = self.app.patch(
+            f'/api/collaboration/{col.id}', headers=headers,
+            json={"name": "not-going-to-happen"})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        col.delete()
 
     def test_delete_collaboration_permissions(self):
 
         col = Collaboration()
         col.save()
 
         # test deleting unknown collaboration
@@ -1611,93 +2081,136 @@
         # test deleting with permission
         rule = Rule.get_by_("collaboration", Scope.GLOBAL, Operation.DELETE)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.delete(f"/api/collaboration/{col.id}",
                                   headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
+        # check deleting with collaboration permission outside the
+        # collaboration fails
+        org = Organization()
+        org.save()
+        col = Collaboration(organizations=[org])
+        col.save()
+        org_not_member = Organization()
+        org_not_member.save()
+        rule = Rule.get_by_("collaboration", Scope.COLLABORATION,
+                            Operation.DELETE)
+        headers = self.create_user_and_login(organization=org_not_member,
+                                             rules=[rule])
+        result = self.app.delete(f"/api/collaboration/{col.id}",
+                                 headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # check deleting with collaboration permission inside the collaboration
+        # succeeds
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        result = self.app.delete(f"/api/collaboration/{col.id}",
+                                 headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # cleanup
+        org.delete()
+        org_not_member.delete()
+
     def test_view_collaboration_organization_permissions_as_user(self):
         headers = self.create_user_and_login()
 
-        # non-existing collaboration
-        results = self.app.get("/api/collaboration/9999/organization",
-                               headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
-
         org = Organization()
         org.save()
         col = Collaboration(organizations=[org])
         col.save()
 
         # access without the proper permissions
         headers = self.create_user_and_login(organization=org)
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # global permissions
-        rule = Rule.get_by_("collaboration", Scope.GLOBAL, Operation.VIEW)
+        rule = Rule.get_by_("organization", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(organization=org, rules=[rule])
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # organization permissions of another organization
-        rule = Rule.get_by_("collaboration", Scope.ORGANIZATION,
+        rule = Rule.get_by_("organization", Scope.ORGANIZATION,
                             Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # now with the correct organization
-        rule = Rule.get_by_("collaboration", Scope.ORGANIZATION,
+        # now with the correct organization but without the correct permissions
+        rule = Rule.get_by_("organization", Scope.ORGANIZATION,
                             Operation.VIEW)
         headers = self.create_user_and_login(organization=org, rules=[rule])
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # now with the correct organization and the correct permissions
+        rule = Rule.get_by_("organization", Scope.COLLABORATION,
+                            Operation.VIEW)
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(json_data), len(col.organizations))
 
     def test_view_collaboration_organization_permissions_as_node(self):
 
         org = Organization()
         org.save()
         col = Collaboration(organizations=[org])
         col.save()
 
         # node of a different organization
         headers = self.create_node_and_login()
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # node of the correct organization
         headers = self.create_node_and_login(organization=org,
                                              collaboration=col)
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(json_data), len(col.organizations))
 
     def test_view_collaboration_organization_permissions_as_container(self):
 
         org = Organization()
         org.save()
         col = Collaboration(organizations=[org])
         col.save()
 
-        # node of a different organization
+        # container of a different organization
         headers = self.login_container()
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
+        # container of the correct organization
         headers = self.login_container(organization=org, collaboration=col)
-        results = self.app.get(f"/api/collaboration/{col.id}/organization",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/organization?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(json_data), len(col.organizations))
 
     def test_edit_collaboration_organization_permissions(self):
 
         org = Organization()
         org.save()
         col = Collaboration(organizations=[org])
         col.save()
@@ -1715,88 +2228,160 @@
         rule = Rule.get_by_("collaboration", Scope.GLOBAL, Operation.EDIT)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.post(f"/api/collaboration/{col.id}/organization",
                                 headers=headers, json={'id': org2.id})
         self.assertEqual(results.status_code, HTTPStatus.OK)
         self.assertEqual(len(results.json), 2)
 
-    def test_delete_collaboration_organization_pesmissions(self):
+        # test adding new organization to collaboration from within the
+        # collaboration
+        org3 = Organization()
+        org3.save()
+        rule = Rule.get_by_("collaboration", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        results = self.app.post(f"/api/collaboration/{col.id}/organization",
+                                headers=headers, json={'id': org3.id})
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # adding new organization to collaboration from outside the
+        # collaboration should fail with collaboration permission
+        org4 = Organization()
+        org4.save()
+        headers = self.create_user_and_login(organization=org4, rules=[rule])
+        results = self.app.post(f"/api/collaboration/{col.id}/organization",
+                                headers=headers, json={'id': org4.id})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        org3.delete()
+        org4.delete()
+        col.delete()
+
+    def test_delete_collaboration_organization_permissions(self):
 
         org = Organization()
         org.save()
-        col = Collaboration(organizations=[org])
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
         col.save()
 
         # try to do it without permission
         headers = self.create_user_and_login()
         results = self.app.delete(f"/api/collaboration/{col.id}/organization",
                                   headers=headers, json={'id': org.id})
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # delete it!
-        rule = Rule.get_by_("collaboration", Scope.GLOBAL, Operation.DELETE)
+        # delete first organization
+        rule = Rule.get_by_("collaboration", Scope.GLOBAL, Operation.EDIT)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.delete(f"/api/collaboration/{col.id}/organization",
                                   headers=headers, json={'id': org.id})
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(results.json, [])
+        self.assertEqual(len(results.json), 1)  # one organization left
+
+        # add back first organization
+        col.organizations.append(org)
+        col.save()
+
+        # removing organization from collaboration from outside the
+        # collaboration should fail with collaboration permission
+        org3 = Organization()
+        org3.save()
+        rule = Rule.get_by_("collaboration", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        results = self.app.delete(f"/api/collaboration/{col.id}/organization",
+                                  headers=headers, json={'id': org2.id})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test removing organization from collaboration from within the
+        # collaboration
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        results = self.app.delete(f"/api/collaboration/{col.id}/organization",
+                                  headers=headers, json={'id': org2.id})
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
 
     def test_view_collaboration_node_permissions(self):
 
-        org = Organization()
-        col = Collaboration(organizations=[org])
+        org = Organization(name=str(uuid.uuid1()))
+        col = Collaboration(name=str(uuid.uuid1()), organizations=[org])
         node = Node(collaboration=col, organization=org)
         node.save()
 
-        # try to view an non-existant collaboration
-        headers = self.create_user_and_login()
-        results = self.app.get("/api/collaboration/9999/node", headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
-
         # try to view without any permissions
-        results = self.app.get(f"/api/collaboration/{col.id}/node",
-                               headers=headers)
+        headers = self.create_user_and_login()
+        results, json_data = self.paginated_list(
+            "/api/node?collaboration_id=9999", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # try to view from another organzization
-        rule = Rule.get_by_("collaboration", Scope.ORGANIZATION,
-                            Operation.VIEW)
+        rule = Rule.get_by_("node", Scope.ORGANIZATION, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f"/api/collaboration/{col.id}/node",
-                               headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+        results, json_data = self.paginated_list(
+            f"/api/node?collaboration_id={col.id}", headers=headers
+        )
+        self.assertEqual(len(json_data), 0)
 
         # try to view from another organization with global permissions
-        rule = Rule.get_by_("collaboration", Scope.GLOBAL,
-                            Operation.VIEW)
+        rule = Rule.get_by_("node", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f"/api/collaboration/{col.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json), len(col.nodes))
+        self.assertEqual(len(json_data), len(col.nodes))
 
-        # try to view from your organization
-        rule = Rule.get_by_("collaboration", Scope.ORGANIZATION,
-                            Operation.VIEW)
+        # try to view your collaboration's nodes with organization permissions
+        rule = Rule.get_by_("node", Scope.ORGANIZATION, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule], organization=org)
-        results = self.app.get(f"/api/collaboration/{col.id}/node",
-                               headers=headers)
+        results, json_data = self.paginated_list(
+            f"/api/node?collaboration_id={col.id}", headers=headers
+        )
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # and now with collaboration permissions
+        rule = Rule.get_by_("node", Scope.COLLABORATION, Operation.VIEW)
+        headers = self.create_user_and_login(rules=[rule], organization=org)
+        results, json_data = self.paginated_list(
+            f"/api/node?collaboration_id={col.id}", headers=headers
+        )
         self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(json_data), len(col.nodes))
 
         # cleanup
         node.delete()
 
     def test_add_collaboration_node_permissions(self):
 
         org = Organization()
         org.save()
-        col = Collaboration(organizations=[org])
+        org2 = Organization()
+        org2.save()
+        col = Collaboration(organizations=[org, org2])
         col.save()
         node = Node(organization=org)
         node.save()
+        node2 = Node(organization=org2)
+        node2.save()
+
+        org3 = Organization()
+        org3.save()
+        node3 = Node(organization=org3)
+        node3.save()
 
         # try non-existant collaboration
         headers = self.create_user_and_login()
 
         results = self.app.post('/api/collaboration/9999/node',
                                 headers=headers, json={'id': node.id})
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
@@ -1820,21 +2405,49 @@
         self.assertEqual(len(results.json), len(col.nodes))
 
         # try to add a node thats already in there
         results = self.app.post(f'/api/collaboration/{col.id}/node',
                                 headers=headers, json={'id': node.id})
         self.assertEqual(results.status_code, HTTPStatus.BAD_REQUEST)
 
+        # adding new node to collaboration from an organization that is not
+        # part of the collaboration should fail
+        results = self.app.post(f'/api/collaboration/{col.id}/node',
+                                headers=headers, json={'id': node3.id})
+        self.assertEqual(results.status_code, HTTPStatus.BAD_REQUEST)
+
+        # test new node to collaboration from within the collaboration
+        rule = Rule.get_by_("collaboration", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        results = self.app.post(f'/api/collaboration/{col.id}/node',
+                                headers=headers, json={'id': node2.id})
+        self.assertEqual(results.status_code, HTTPStatus.CREATED)
+
+        # adding new node to collaboration from outside collaboration should
+        # fail with collaboration-scope permission
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        results = self.app.post(f'/api/collaboration/{col.id}/node',
+                                headers=headers, json={'id': node3.id})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
         # cleanup
         node.delete()
+        node2.delete()
+        node3.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
 
     def test_delete_collaboration_node_permissions(self):
 
         org = Organization()
-        col = Collaboration(organizations=[org])
+        org2 = Organization()
+        col = Collaboration(organizations=[org, org2])
         node = Node(organization=org, collaboration=col)
         node.save()
 
         # try non-existant collaboration
         headers = self.create_user_and_login()
         results = self.app.delete('/api/collaboration/9999/node',
                                   headers=headers, json={'id': node.id})
@@ -1854,87 +2467,58 @@
 
         # try to add a node thats not in there
         node2 = Node()
         node2.save()
         results = self.app.delete(f'/api/collaboration/{col.id}/node',
                                   headers=headers, json={'id': node2.id})
         self.assertEqual(results.status_code, HTTPStatus.BAD_REQUEST)
+        node2.delete()
 
-        # delete a node!
+        # delete node from collaboration!
         results = self.app.delete(f'/api/collaboration/{col.id}/node',
                                   headers=headers, json={'id': node.id})
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
-        # cleanup
-        node.delete()
-        node2.delete()
-
-    def test_view_collaboration_task_permissions_as_user(self):
-
-        org = Organization()
-        col = Collaboration(organizations=[org])
-        task = Task(collaboration=col)
-        task.save()
-
-        # view non existing collaboration
-        headers = self.create_user_and_login()
-        results = self.app.get('/api/collaboration/9999/task',
-                               headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
-
-        # view without any permission
-        results = self.app.get(f'/api/collaboration/{col.id}/task',
-                               headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
-
-        # view from another organization
-        rule = Rule.get_by_("task", Scope.ORGANIZATION,
-                            Operation.VIEW)
-        headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f'/api/collaboration/{col.id}/task',
-                               headers=headers)
+        # removing node from collaboration from outside the
+        # collaboration should fail with collaboration permission
+        node2 = Node(organization=org2, collaboration=col)
+        node2.save()
+        org3 = Organization()
+        org3.save()
+        rule = Rule.get_by_("collaboration", scope=Scope.COLLABORATION,
+                            operation=Operation.EDIT)
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        results = self.app.delete(f"/api/collaboration/{col.id}/node",
+                                  headers=headers, json={'id': node2.id})
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # view from your own organization
-        headers = self.create_user_and_login(rules=[rule], organization=org)
-        results = self.app.get(f'/api/collaboration/{col.id}/task',
-                               headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json), len(col.tasks))
-
-        # view with global permissions
-        rule = Rule.get_by_("task", Scope.GLOBAL, Operation.VIEW)
-        headers = self.create_user_and_login(rules=[rule])
-        results = self.app.get(f'/api/collaboration/{col.id}/task',
-                               headers=headers)
-        self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json), len(col.tasks))
-
-    def test_view_collaboration_task_permissions_as_node(self):
-
-        org = Organization()
-        col = Collaboration(organizations=[org])
-        node, api_key = self.create_node(org, col)
-        task = Task(collaboration=col)
-        task.save()
-
-        headers = self.login_node(api_key)
-        results = self.app.get(f'/api/collaboration/{col.id}/task',
-                               headers=headers)
+        # test removing organization from collaboration from within the
+        # collaboration
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        results = self.app.delete(f"/api/collaboration/{col.id}/node",
+                                  headers=headers, json={'id': node2.id})
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # cleanup
         node.delete()
+        node2.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
 
     def test_view_node_permissions_as_user(self):
 
         org = Organization()
-        col = Collaboration(organizations=[org])
+        org2 = Organization()
+        col = Collaboration(organizations=[org, org2])
         node = Node(organization=org, collaboration=col)
         node.save()
+        node2 = Node(organization=org2, collaboration=col)
+        node2.save()
 
         # view non existing node
         headers = self.create_user_and_login()
         results = self.app.get('/api/node/9999', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
 
         # missing permissions
@@ -1958,24 +2542,53 @@
         results = self.app.get(f'/api/node/{node.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # list organization permissions
         headers = self.create_user_and_login(organization=org, rules=[rule1])
         results = self.app.get('/api/node', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json), len(col.nodes))
+        self.assertEqual(len(results.json['data']), 1)  # collab has 1 node
 
         # list global permissions
         headers = self.create_user_and_login(rules=[rule2])
+        results, json_data = self.paginated_list('/api/node', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(json_data), len(Node.get()))
+
+        # collaboration permission inside the collaboration
+        rule = Rule.get_by_("node", scope=Scope.COLLABORATION,
+                            operation=Operation.VIEW)
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        results = self.app.get(f'/api/node/{node.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # list collaboration permissions - in collaboration
         results = self.app.get('/api/node', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json), len(Node.get()))
+        self.assertEqual(len(results.json['data']), len(col.nodes))
+
+        # collaboration permission outside the collaboration should fail
+        org3 = Organization()
+        org3.save()
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        results = self.app.get(f'/api/node/{node.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # list collaboration permissions - other collaboration
+        results = self.app.get('/api/node', headers=headers,
+                               query_string={'collaboration_id': col.id})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # cleanup
         node.delete()
+        node2.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
 
     def test_view_node_permissions_as_node(self):
 
         org = Organization()
         col = Collaboration(organizations=[org])
         node, api_key = self.create_node(org, col)
 
@@ -1984,24 +2597,25 @@
         # global permissions
         results = self.app.get(f'/api/node/{node.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # list organization permissions
         results = self.app.get('/api/node', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertEqual(len(results.json), len(org.nodes))
+        self.assertEqual(len(results.json['data']), len(org.nodes))
 
         # cleanup
         node.delete()
 
     def test_create_node_permissions(self):
 
-        org = Organization()
+        org = Organization(name=str(uuid.uuid1()))
         col = Collaboration(organizations=[org])
-        org2 = Organization()
+        col.save()
+        org2 = Organization(name=str(uuid.uuid1()))
         org2.save()
 
         # test non existing collaboration
         headers = self.create_user_and_login()
         results = self.app.post('/api/node', headers=headers,
                                 json={'collaboration_id': 9999})
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
@@ -2025,17 +2639,18 @@
         node_id = results.json.get('id')
         results = self.app.post('/api/node', headers=headers, json={
             'collaboration_id': col.id,
             'organization_id': org2.id  # <-------
         })
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # test adding a node to an collaboration from an organization witch
+        # test adding a node to an collaboration from an organization which
         # does not belong to the collaboration
-        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        rule2 = Rule.get_by_("node", Scope.GLOBAL, Operation.CREATE)
+        headers = self.create_user_and_login(organization=org2, rules=[rule2])
         results = self.app.post('/api/node', headers=headers, json={
             'collaboration_id': col.id
         })
         self.assertEqual(results.status_code, HTTPStatus.BAD_REQUEST)
 
         # check an creating an already existing node
         headers = self.create_user_and_login(organization=org, rules=[rule])
@@ -2059,18 +2674,53 @@
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.post('/api/node', headers=headers, json={
             'collaboration_id': col.id,
             'organization_id': org2.id
         })
         self.assertEqual(results.status_code, HTTPStatus.CREATED)
 
+        # test collaboration permissions
+        org3 = Organization()
+        org3.save()
+        col.organizations.append(org3)
+        col.save()
+        rule = Rule.get_by_("node", scope=Scope.COLLABORATION,
+                            operation=Operation.CREATE)
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        result = self.app.post('/api/node', headers=headers, json={
+            'collaboration_id': col.id,
+            'organization_id': org3.id
+        })
+        self.assertEqual(result.status_code, HTTPStatus.CREATED)
+
+        # test collaboration permissions - outside of collaboration should fail
+        org4 = Organization()
+        org4.save()
+        col.organizations.append(org4)
+        col.save()
+        headers = self.create_user_and_login(organization=Organization(),
+                                             rules=[rule])
+        result = self.app.post('/api/node', headers=headers, json={
+            'collaboration_id': col.id,
+            'organization_id': org4.id
+        })
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
+        node.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        org4.delete()
+        col.delete()
+
     def test_delete_node_permissions(self):
 
-        org = Organization()
-        col = Collaboration(organizations=[org])
+        org = Organization(name=str(uuid.uuid1()))
+        col = Collaboration(name=str(uuid.uuid1()), organizations=[org])
         node = Node(organization=org, collaboration=col)
         node.save()
 
         # unexisting node
         headers = self.create_user_and_login()
         results = self.app.delete('/api/node/9999', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
@@ -2084,34 +2734,65 @@
         # organization permission
         rule = Rule.get_by_('node', Scope.ORGANIZATION, Operation.DELETE)
         headers = self.create_user_and_login(organization=org, rules=[rule])
         results = self.app.delete(f'/api/node/{node.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # global permission
-        node2 = Node(organization=org, collaboration=col)
+        org2 = Organization(name=str(uuid.uuid1()))
+        node2 = Node(organization=org2, collaboration=col)
         node2.save()
         rule = Rule.get_by_('node', Scope.GLOBAL, Operation.DELETE)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.delete(f'/api/node/{node2.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
+        # collaboration permission - removing node from outside collaboration
+        # should fail
+        org3 = Organization()
+        node3 = Node(organization=org3, collaboration=col)
+        node3.save()
+        col.organizations.append(org3)
+        col.save()
+        org_not_in_collab = Organization()
+        org_not_in_collab.save()
+        rule = Rule.get_by_("node", scope=Scope.COLLABORATION,
+                            operation=Operation.DELETE)
+        headers = self.create_user_and_login(organization=org_not_in_collab,
+                                             rules=[rule])
+        results = self.app.delete(f'/api/node/{node3.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # collaboration permission - now within collaboration
+        headers = self.create_user_and_login(organization=org, rules=[rule])
+        results = self.app.delete(f'/api/node/{node3.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # cleanup
+        org.delete()
+        org2.delete()
+        org3.delete()
+        org_not_in_collab.delete()
+        col.delete()
+
     def test_patch_node_permissions_as_user(self):
         # test patching non-existant node
         headers = self.create_user_and_login()
-        results = self.app.patch("/api/node/9999", headers=headers)
+        results = self.app.patch("/api/node/9999", headers=headers, json={})
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
 
         # test user without any permissions
         org = Organization()
-        col = Collaboration(organizations=[org])
+        org2 = Organization()
+        col = Collaboration(organizations=[org, org2])
         node = Node(organization=org, collaboration=col)
         node.save()
 
-        results = self.app.patch(f"/api/node/{node.id}", headers=headers)
+        results = self.app.patch(f"/api/node/{node.id}", headers=headers,
+                                 json={})
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test user with global permissions
         rule = Rule.get_by_("node", Scope.GLOBAL, Operation.EDIT)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.patch(f"/api/node/{node.id}", headers=headers,
                                  json={"name": "A"})
@@ -2164,68 +2845,185 @@
         self.assertEqual(results.json['ip'], '0.0.0.0')
 
         # assign unknow organization
         results = self.app.patch(f'/api/node/{node.id}', headers=headers,
                                  json={'organization_id': 9999})
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
 
+        # collaboration permission - inside the collaboration
+        rule = Rule.get_by_("node", Scope.COLLABORATION, Operation.EDIT)
+        headers = self.create_user_and_login(organization=org2, rules=[rule])
+        results = self.app.patch(f"/api/node/{node.id}", headers=headers,
+                                 json={"name": "A"})
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # collaboration permission - outside the collaboration
+        org3 = Organization()
+        org3.save()
+        headers = self.create_user_and_login(organization=org3, rules=[rule])
+        results = self.app.patch(f"/api/node/{node.id}", headers=headers,
+                                 json={"name": "A"})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
         # cleanup
         node.delete()
+        org.delete()
+        org2.delete()
+        org3.delete()
+        col.delete()
+        col2.delete()
 
     def test_view_task_permissions_as_user(self):
         # non existing task
         headers = self.create_user_and_login()
         results = self.app.get('/api/task/9999', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
 
         # test user without any permissions and id
         org = Organization()
-        col = Collaboration(organizations=[org])
-        task = Task(name="unit", collaboration=col)
+        org2 = Organization()
+        col = Collaboration(organizations=[org, org2])
+        task = Task(name="unit", collaboration=col, init_org=org)
         task.save()
 
         results = self.app.get(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # test user with org permissions with id
-        rule = Rule.get_by_("task", Scope.ORGANIZATION, Operation.VIEW)
+        # test user with col permissions with id
+        rule = Rule.get_by_("task", Scope.COLLABORATION, Operation.VIEW)
         headers = self.create_user_and_login(org, rules=[rule])
         results = self.app.get(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
         self.assertEqual(results.json['name'], 'unit')
 
+        # collaboration permission outside the collaboration should fail
+        org_not_in_collab = Organization()
+        org_not_in_collab.save()
+        headers = self.create_user_and_login(organization=org_not_in_collab,
+                                             rules=[rule])
+        results = self.app.get(f'/api/task/{task.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
         # test user with org permissions with id from another org
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.get(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test user with org permissions without id
         headers = self.create_user_and_login(org, rules=[rule])
         results = self.app.get('/api/task', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
+        # test that user is not allowed to view task results without id
+        results = self.app.get('/api/task', headers=headers,
+                               query_string={'include': 'results'})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test that user is allowed to view task results if they have the rule
+        # to view results
+        rule_view_results = Rule.get_by_("run", Scope.GLOBAL, Operation.VIEW)
+        headers = self.create_user_and_login(org,
+                                             rules=[rule, rule_view_results])
+        results = self.app.get('/api/task', headers=headers,
+                               query_string={'include': 'results'})
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
         # test user with global permissions and id
         rule = Rule.get_by_("task", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.get(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
+        # test that user is not allowed to view task results with id
+        results = self.app.get(f'/api/task/{task.id}', headers=headers,
+                               query_string={'include': 'results'})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test that user is allowed to view task results if they have the rule
+        # to view results
+        headers = self.create_user_and_login(org,
+                                             rules=[rule, rule_view_results])
+        results = self.app.get(f'/api/task/{task.id}', headers=headers,
+                               query_string={'include': 'results'})
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
         # test user with global permissions without id
         results = self.app.get('/api/task', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
+        # list collaboration permissions - in collaboration
+        rule = Rule.get_by_("task", Scope.COLLABORATION, Operation.VIEW)
+        headers = self.create_user_and_login(org, rules=[rule])
+        results = self.app.get('/api/task', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(results.json['data']), len(col.tasks))
+
+        # list collaboration permissions - other collaboration
+        headers = self.create_user_and_login(org_not_in_collab, rules=[rule])
+        results = self.app.get('/api/task', headers=headers,
+                               query_string={'collaboration_id': col.id})
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # list own organization permissions - same organization
+        rule = Rule.get_by_("task", Scope.ORGANIZATION, Operation.VIEW)
+        headers = self.create_user_and_login(org, rules=[rule])
+        results = self.app.get('/api/task', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(results.json['data']), len(col.tasks))
+
+        # list own organization permissions - other organization
+        headers = self.create_user_and_login(org2, rules=[rule])
+        results = self.app.get('/api/task', headers=headers, query_string={
+            'init_org_id': org.id
+        })
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # list own user's task permissions - same user without id
+        rule = Rule.get_by_("task", Scope.OWN, Operation.VIEW)
+        user = self.create_user(rules=[rule], organization=org)
+        headers = self.login(user.username)
+        task2 = Task(name="unit", collaboration=col, init_org=org,
+                     init_user=user)
+        task2.save()
+        results = self.app.get('/api/task', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertEqual(len(results.json['data']), 1)
+
+        # list own user's task permissions - same user with id
+        results = self.app.get(f'/api/task/{task2.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # list own user's task permissions - other user without id
+        headers = self.create_user_and_login(org, rules=[rule])
+        results = self.app.get('/api/task', headers=headers, query_string={
+            'init_user_id': user.id
+        })
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # list own user's task permissions - other user with id
+        results = self.app.get(f'/api/task/{task2.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # cleanup
+        task.delete()
+        task2.delete()
+        user.delete()
+        org.delete()
+        org2.delete()
+        col.delete()
+
     def test_view_task_permissions_as_node_and_container(self):
         # test node with id
         org = Organization()
         org.save()
         col = Collaboration(organizations=[org])
         col.save()
-        task = Task(collaboration=col, image="some-image")
+        task = Task(collaboration=col, image="some-image", init_org=org)
         task.save()
-        res = Result(task=task)
+        res = Run(task=task, status=TaskStatus.PENDING)
         res.save()
 
         headers = self.create_node_and_login(organization=org)
         results = self.app.get(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # test node without id
@@ -2241,135 +3039,131 @@
         # test container without id
         results = self.app.get('/api/task', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
     def test_create_task_permission_as_user(self):
         # non existant collaboration
         headers = self.create_user_and_login()
-        results = self.app.post('/api/task', headers=headers, json={
-            "collaboration_id": 9999
-        })
+        input_ = {'method': 'dummy'}
+        task_json = {
+            "collaboration_id": 9999,
+            "organizations": [{'id': 9999, 'input': input_}],
+            "image": "some-image"
+        }
+        results = self.app.post('/api/task', headers=headers, json=task_json)
         self.assertEqual(results.status_code, HTTPStatus.NOT_FOUND)
 
         # organizations outside of collaboration
         org = Organization()
         org.save()
         col = Collaboration(organizations=[org])
         col.save()
 
         # task without any node created
-        results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}],
-            "collaboration_id": col.id
-        })
+        task_json["organizations"] = [{'id': org.id, 'input': input_}]
+        task_json["collaboration_id"] = col.id
+        results = self.app.post('/api/task', headers=headers, json=task_json)
         self.assertEqual(results.status_code, HTTPStatus.BAD_REQUEST)
 
         # node is used implicitly as in further checks, can only create task
         # if node has been created
         node = Node(organization=org, collaboration=col)
 
         org2 = Organization()
         org2.save()
 
-        results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org2.id}], 'collaboration_id': col.id
-        })
+        task_json["organizations"] = [{'id': org2.id, 'input': input_}]
+        results = self.app.post('/api/task', headers=headers, json=task_json)
         self.assertEqual(results.status_code, HTTPStatus.BAD_REQUEST)
 
         # user without any permissions
-        results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}],
-            "collaboration_id": col.id
-        })
+        task_json["organizations"] = [{'id': org.id, 'input': input_}]
+        results = self.app.post('/api/task', headers=headers, json=task_json)
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # user with organization permissions for other organization
-        rule = Rule.get_by_("task", Scope.ORGANIZATION, Operation.CREATE)
+        rule = Rule.get_by_("task", Scope.COLLABORATION, Operation.CREATE)
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}], 'collaboration_id': col.id
-        })
+        results = self.app.post('/api/task', headers=headers, json=task_json)
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # user with organization permissions
         headers = self.create_user_and_login(org, rules=[rule])
-        results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}], 'collaboration_id': col.id
-        })
+        results = self.app.post('/api/task', headers=headers, json=task_json)
         self.assertEqual(results.status_code, HTTPStatus.CREATED)
 
         # user with global permissions but outside of the collaboration. They
         # should *not* be allowed to create a task in a collaboration that
         # they're not a part of
         # TODO add test for user with global permission that creates a task for
         # another organization than their own in the same collaboration
         rule = Rule.get_by_("task", Scope.GLOBAL, Operation.CREATE)
         headers = self.create_user_and_login(rules=[rule])
-        results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}], 'collaboration_id': col.id
-        })
+        results = self.app.post('/api/task', headers=headers, json=task_json)
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # test master task
-        rule = Rule.get_by_("task", Scope.ORGANIZATION, Operation.CREATE)
-        headers = self.create_user_and_login(org, rules=[rule])
-        results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}],
-            'collaboration_id': col.id,
-            'master': True
-        })
-        self.assertEqual(results.status_code, HTTPStatus.CREATED)
-
         # cleanup
         node.delete()
 
     def test_create_task_permissions_as_container(self):
         org = Organization()
         col = Collaboration(organizations=[org])
         parent_task = Task(collaboration=col, image="some-image")
         parent_task.save()
-        parent_res = Result(organization=org, task=parent_task)
+        parent_res = Run(organization=org, task=parent_task,
+                         status=TaskStatus.PENDING)
         parent_res.save()
 
         # test wrong image name
+        input_ = {'method': 'dummy'}
         headers = self.login_container(collaboration=col, organization=org,
                                        task=parent_task)
         results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}],
+            "organizations": [{'id': org.id, 'input': input_}],
             'collaboration_id': col.id,
             'image': 'other-image'
         })
 
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test other collaboration_id
         col2 = Collaboration(organizations=[org])
         col2.save()
         node2 = Node(organization=org, collaboration=col2)
         node2.save()
         results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}],
+            "organizations": [{'id': org.id, 'input': input_}],
             'collaboration_id': col2.id,
             'image': 'some-image'
         })
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test with correct parameters
         results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}],
+            "organizations": [{'id': org.id, 'input': input_}],
             'collaboration_id': col.id,
             'image': 'some-image'
         })
         self.assertEqual(results.status_code, HTTPStatus.CREATED)
 
         # test already completed task
-        parent_res.finished_at = datetime.date(2020, 1, 1)
+        parent_res.status = TaskStatus.COMPLETED
+        parent_res.save()
+        results = self.app.post('/api/task', headers=headers, json={
+            "organizations": [{'id': org.id, 'input': input_}],
+            'collaboration_id': col.id,
+            'image': 'some-image'
+        })
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test a failed task
+        parent_res.status = TaskStatus.FAILED
         parent_res.save()
         results = self.app.post('/api/task', headers=headers, json={
-            "organizations": [{'id': org.id}],
+            "organizations": [{'id': org.id, 'input': input_}],
             'collaboration_id': col.id,
             'image': 'some-image'
         })
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
         # cleanup
         node2.delete()
@@ -2378,86 +3172,189 @@
 
         # test non-existing task
         headers = self.create_user_and_login()
         self.app.delete('/api/task/9999', headers=headers)
 
         # test with organization permissions from other organization
         org = Organization()
-        col = Collaboration(organizations=[org])
-        task = Task(collaboration=col)
+        org2 = Organization()
+        col = Collaboration(organizations=[org, org2])
+        task = Task(collaboration=col, init_org=org)
         task.save()
 
-        rule = Rule.get_by_("task", Scope.ORGANIZATION, Operation.DELETE)
+        # test with user who is not member of collaboration
+        rule = Rule.get_by_("task", Scope.COLLABORATION, Operation.DELETE)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.delete(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # test with organization permissions
+        # test with collaboration permissions
         headers = self.create_user_and_login(org, [rule])
         results = self.app.delete(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # test with global permissions
         task = Task(collaboration=col)
         task.save()
         rule = Rule.get_by_("task", Scope.GLOBAL, Operation.DELETE)
         headers = self.create_user_and_login(rules=[rule])
         results = self.app.delete(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
         # test that all results are also deleted
         task = Task(collaboration=col)
-        res = Result(task=task)
-        res.save()
-        result_id = res.id  # cannot access this after deletion
+        run = Run(task=task)
+        run.save()
+        run_id = run.id  # cannot access this after deletion
+        results = self.app.delete(f'/api/task/{task.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+        self.assertIsNone(Task.get(run_id))
+
+        # test permission to delete tasks of own organization - other
+        # organization should fail
+        task = Task(collaboration=col, init_org=org)
+        task.save()
+        rule = Rule.get_by_("task", Scope.ORGANIZATION, Operation.DELETE)
+        headers = self.create_user_and_login(rules=[rule], organization=org2)
+        results = self.app.delete(f'/api/task/{task.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test permission to delete tasks of own organization - should work
+        headers = self.create_user_and_login(rules=[rule], organization=org)
         results = self.app.delete(f'/api/task/{task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
-        self.assertIsNone(Task.get(result_id))
+
+        # test permission to delete own tasks - other user of organization
+        # should fail
+        rule = Rule.get_by_("task", Scope.OWN, Operation.DELETE)
+        user = self.create_user(rules=[rule], organization=org)
+        task = Task(collaboration=col, init_org=org, init_user=user)
+        task.save()
+        headers = self.create_user_and_login(rules=[rule], organization=org)
+        results = self.app.delete(f'/api/task/{task.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test permission to delete own tasks with same user
+        headers = self.login(user.username)
+        results = self.app.delete(f'/api/task/{task.id}', headers=headers)
+        self.assertEqual(results.status_code, HTTPStatus.OK)
+
+        # cleanup
+        user.delete()
+        org.delete()
+        org2.delete()
+        col.delete()
 
     def test_view_task_result_permissions_as_user(self):
 
         # non-existing task
         headers = self.create_user_and_login()
-        result = self.app.get('/api/task/9999/result', headers=headers)
+        result = self.app.get('/api/task/9999/run', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.NOT_FOUND)
 
         # test with organization permissions from other organization
         org = Organization()
-        col = Collaboration(organizations=[org])
-        task = Task(collaboration=col)
+        org2 = Organization()
+        col = Collaboration(organizations=[org, org2])
+        col.save()
+        task = Task(collaboration=col, init_org=org)
         # NB: node is used implicitly in task/{id}/result schema
         node = Node(organization=org, collaboration=col)
-        res = Result(task=task, organization=org)
+        res = Run(task=task, organization=org)
         res.save()
 
-        rule = Rule.get_by_("result", Scope.ORGANIZATION, Operation.VIEW)
+        # Test with permissions of someone who is not in the collaboration
+        rule = Rule.get_by_("run", Scope.COLLABORATION, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        result = self.app.get(f'/api/task/{task.id}/result', headers=headers)
+        result = self.app.get(f'/api/run?task_id={task.id}', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # test with organization permission
+        # test with collaboration permission
         headers = self.create_user_and_login(org, [rule])
-        result = self.app.get(f'/api/task/{task.id}/result', headers=headers)
+        result = self.app.get(f'/api/run?task_id={task.id}', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
         # test with global permission
-        rule = Rule.get_by_("result", Scope.GLOBAL, Operation.VIEW)
+        rule = Rule.get_by_("run", Scope.GLOBAL, Operation.VIEW)
         headers = self.create_user_and_login(rules=[rule])
-        result = self.app.get(f'/api/task/{task.id}/result', headers=headers)
+        result = self.app.get(f'/api/run?task_id={task.id}', headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.OK)
 
+        # test also result endpoint
+        rule = Rule.get_by_("run", Scope.COLLABORATION, Operation.VIEW)
+        headers = self.create_user_and_login(rules=[rule])
+        result = self.app.get(
+            f'/api/result?task_id={task.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test result endpoint with organization permission
+        headers = self.create_user_and_login(org, [rule])
+        result = self.app.get(
+            f'/api/result?task_id={task.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # test result endpoint with global permission
+        rule = Rule.get_by_("run", Scope.GLOBAL, Operation.VIEW)
+        headers = self.create_user_and_login(rules=[rule])
+        result = self.app.get(
+            f'/api/result?task_id={task.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # test with organization permission
+        rule = Rule.get_by_("run", Scope.ORGANIZATION, Operation.VIEW)
+        headers = self.create_user_and_login(org, [rule])
+        result = self.app.get(f'/api/run?task_id={task.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+        result = self.app.get(f'/api/run/{res.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # test with organization permission - other organization should fail
+        headers = self.create_user_and_login(org2, [rule])
+        result = self.app.get(
+            f'/api/run?task_id={task.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+        result = self.app.get(f'/api/run/{res.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
+        # test with permission to view own runs
+        rule = Rule.get_by_("run", Scope.OWN, Operation.VIEW)
+        user = self.create_user(rules=[rule], organization=org)
+        headers = self.login(user.username)
+        task2 = Task(collaboration=col, init_org=org, init_user=user)
+        task2.save()
+        res2 = Run(task=task2, organization=org)
+        res2.save()
+        result = self.app.get(f'/api/run?task_id={task2.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+        result = self.app.get(f'/api/run/{res2.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # test with permission to view own runs - other user should fail
+        headers = self.create_user_and_login(rules=[rule], organization=org)
+        result = self.app.get(f'/api/run?task_id={task2.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+        result = self.app.get(f'/api/run/{res2.id}', headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
+
         # cleanup
         node.delete()
+        task.delete()
+        task2.delete()
+        res.delete()
+        res2.delete()
+        org.delete()
+        org2.delete()
+        col.delete()
 
-    def test_view_task_result_permissions_as_container(self):
+    def test_view_task_run_permissions_as_container(self):
         # test if container can
         org = Organization()
         col = Collaboration(organizations=[org])
-        task = Task(collaboration=col, image="some-image")
+        task = Task(collaboration=col, image="some-image", init_org=org)
         task.save()
-        res = Result(task=task, organization=org)
+        res = Run(task=task, organization=org, status=TaskStatus.PENDING)
         res.save()
 
         headers = self.login_container(collaboration=col, organization=org,
                                        task=task)
-        results = self.app.get(f'/api/task/{task.id}/result', headers=headers)
+        results = self.app.get(f'/api/run?task_id={task.id}', headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/__init__.py` & `vantage6-server-4.0.0a2/vantage6/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 from gevent import monkey
 
 # flake8: noqa: E402 (ignore import error)
 monkey.patch_all()
 
 import importlib
 import logging
-import os
 import uuid
 import json
 import time
 import datetime as dt
 import traceback
 
-from typing import Any
 from http import HTTPStatus
 from werkzeug.exceptions import HTTPException
 from flasgger import Swagger
 from flask import (
     Flask, make_response, current_app, request, send_from_directory, Request,
     Response
 )
@@ -38,22 +36,20 @@
 from threading import Thread
 from pathlib import Path
 
 from vantage6.common import logger_name
 from vantage6.common.globals import PING_INTERVAL_SECONDS
 from vantage6.server import db
 from vantage6.cli.context import ServerContext
-from vantage6.cli.globals import DEFAULT_SERVER_ENVIRONMENT
 from vantage6.server.model.base import DatabaseSessionManager, Database
-from vantage6.server.resource.common._schema import HATEOASModelSchema
+from vantage6.server.resource.common.output_schema import HATEOASModelSchema
 from vantage6.server.permission import RuleNeed, PermissionManager
 from vantage6.server.globals import (
     APPNAME,
     ACCESS_TOKEN_EXPIRES_HOURS,
-    JWT_TEST_ACCESS_TOKEN_EXPIRES,
     RESOURCES,
     SUPER_USER_INFO,
     REFRESH_TOKENS_EXPIRE_HOURS,
     DEFAULT_SUPPORT_EMAIL_ADDRESS,
     MIN_TOKEN_VALIDITY_SECONDS,
     MIN_REFRESH_TOKEN_EXPIRY_DELTA,
     SERVER_MODULE_NAME
@@ -211,23 +207,14 @@
                 self._get_jwt_expiration_seconds(
             config_key='refresh_token_expires_hours',
             default_hours=REFRESH_TOKENS_EXPIRE_HOURS,
             longer_than=token_expiry_seconds + MIN_REFRESH_TOKEN_EXPIRY_DELTA,
             is_refresh=True
         )
 
-        # Set an extra long expiration time on access tokens for testing
-        # TODO: this does not seem needed...
-        environment = self.ctx.config.get('type')
-        self.app.config['environment'] = environment
-        if environment == 'test':
-            log.warning("Setting 'JWT_ACCESS_TOKEN_EXPIRES' to one day!")
-            self.app.config['JWT_ACCESS_TOKEN_EXPIRES'] = \
-                JWT_TEST_ACCESS_TOKEN_EXPIRES
-
         # Open Api Specification (f.k.a. swagger)
         self.app.config['SWAGGER'] = {
             'title': APPNAME,
             'uiversion': "3",
             'openapi': '3.0.0',
             'version': __version__
         }
@@ -659,36 +646,32 @@
                         node.status = 'offline'
                         node.save()
             except Exception:
                 log.exception('Node-status thread had an exception')
                 time.sleep(PING_INTERVAL_SECONDS)
 
 
-def run_server(config: str, environment: str = DEFAULT_SERVER_ENVIRONMENT,
-               system_folders: bool = True) -> ServerApp:
+def run_server(config: str, system_folders: bool = True) -> ServerApp:
     """
     Run a vantage6 server.
 
     Parameters
     ----------
     config: str
         Configuration file path
-    environment: str
-        Configuration environment to use.
     system_folders: bool
         Whether to use system or user folders. Default is True.
 
     Returns
     -------
     ServerApp
         A running instance of the vantage6 server
     """
     ctx = ServerContext.from_external_config_file(
         config,
-        environment,
         system_folders
     )
     allow_drop_all = ctx.config["allow_drop_all"]
     Database().connect(uri=ctx.get_database_uri(),
                        allow_drop_all=allow_drop_all)
     return ServerApp(ctx).start()
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-4.0.0a2/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-4.0.0a2/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-4.0.0a2/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-4.0.0a2/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-4.0.0a2/vantage6/server/_data/dev/server.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-application:
-    api_path: '/api'
-    logging:
-        level:        CRITICAL                   # Can be on of 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'; 'NONE' disables logging.
-        file:         unittest.log           # Filename of logfile
-        use_console:  False                  # Log output to the console?
-        backup_count: 5                      # Number of logs to keep
-        max_size:     1024                   # Specified in kB (i.e. 1024 means a maximum file size of 1MB)
-        format:       "%(asctime)s - %(name)-14s - %(levelname)-8s - %(message)s"
-        datefmt:      "%Y-%m-%d %H:%M:%S"
-
+description: Dev
+type: dev
+ip: '127.0.0.1'
+port: 5000
+api_path: /api
+uri: sqlite:///develop.sqlite
+allow_drop_all: True
+logging:
+  level:        DEBUG                  # Can be on of 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'
+  file:         develop-server.log     # Filename of logfile
+  use_console:  True                   # Log output to the console?
+  backup_count: 5                      # Number of logs to keep
+  max_size:     1024                   # Specified in kB (i.e. 1024 means a maximum file size of 1MB)
+  format:       "%(asctime)s - %(name)-14s - %(levelname)-8s - %(message)s"
+  datefmt:      "%Y-%m-%d %H:%M:%S"
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-4.0.0a2/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/_version.py` & `vantage6-server-4.0.0a2/vantage6/server/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (3, 9, 0, 'candidate', __build__, 0)
+version_info = (4, 0, 0, 'alpha', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/context.py` & `vantage6-server-4.0.0a2/vantage6/server/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
         Returns
         -------
         TestContext
             Context object
         """
         return super().from_external_config_file(
-            cls.test_config_location(),
-            "unittest", "application", True
+            cls.test_config_location(), "unittest", True
         )
 
     @staticmethod
     def test_config_location() -> str:
         """
         Location of the unittest configuration file.
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/controller/fixture.py` & `vantage6-server-4.0.0a2/vantage6/server/controller/fixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,21 +113,21 @@
         log.debug("Processing Task Assignments")
         for image in col.get("tasks", {}):
             init_org = collaboration.organizations[0]
             task = db.Task(
                 name="Example task",
                 image=image,
                 collaboration=collaboration,
-                run_id=db.Task.next_run_id(),
-                initiator=init_org
+                job_id=db.Task.next_job_id(),
+                init_org=init_org
             )
 
             for organization in collaboration.organizations:
-                result = db.Result(
+                run = db.Run(
                     task=task,
                     input="something",
                     organization=organization
                 )
-                result.save()
+                run.save()
 
             task.save()
             log.debug(f"Processed task {task.name}")
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/db.py` & `vantage6-server-4.0.0a2/vantage6/server/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 import logging
 import datetime
 
 import enum
-import json
 import sqlalchemy as sql
 
 # TODO this file is akward...
 from vantage6.server.model import (
     Base,
     Task,
-    Result,
+    Run,
     Organization,
     User,
     Node,
     Authenticatable,
     Collaboration,
     Member,
     Permission,
     Role,
     Rule,
     UserPermission,
     role_rule_association,
     AlgorithmPort,
-    NodeConfig
+    NodeConfig,
+    TaskDatabase,
 )
 from vantage6.common import logger_name
 from vantage6.common.globals import STRING_ENCODING
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/default_roles.py` & `vantage6-server-4.0.0a2/vantage6/server/default_roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,28 +54,28 @@
         db.Rule.get_by_('user', Scope.OWN, Operation.DELETE),
         db.Rule.get_by_('user', Scope.ORGANIZATION, Operation.VIEW),
         db.Rule.get_by_('organization', Scope.ORGANIZATION, Operation.VIEW),
         db.Rule.get_by_('organization', Scope.COLLABORATION, Operation.VIEW),
         db.Rule.get_by_('collaboration', Scope.ORGANIZATION, Operation.VIEW),
         db.Rule.get_by_('role', Scope.ORGANIZATION, Operation.VIEW),
         db.Rule.get_by_('node', Scope.ORGANIZATION, Operation.VIEW),
-        db.Rule.get_by_('task', Scope.ORGANIZATION, Operation.VIEW),
-        db.Rule.get_by_('result', Scope.ORGANIZATION, Operation.VIEW),
+        db.Rule.get_by_('task', Scope.COLLABORATION, Operation.VIEW),
+        db.Rule.get_by_('run', Scope.COLLABORATION, Operation.VIEW),
         db.Rule.get_by_('port', Scope.ORGANIZATION, Operation.VIEW),
-        db.Rule.get_by_('event', Scope.ORGANIZATION, Operation.VIEW),
+        db.Rule.get_by_('event', Scope.ORGANIZATION, Operation.RECEIVE),
     ]
     VIEWER_ROLE = {
         'name': DefaultRole.VIEWER,
         'description': "Can manage their own account and view resources "
                        "related to their organization",
         'rules': VIEWER_RULES
     }
     # 3. Researcher role
     RESEARCHER_RULES = VIEWER_RULES + [
-        db.Rule.get_by_('task', Scope.ORGANIZATION, Operation.CREATE),
+        db.Rule.get_by_('task', Scope.COLLABORATION, Operation.CREATE),
         db.Rule.get_by_('task', Scope.ORGANIZATION, Operation.DELETE),
     ]
     RESEARCHER_ROLE = {
         'name': DefaultRole.RESEARCHER,
         'description': "Can perform tasks, manage their own account, and "
                        "view resources related to their organization",
         'rules': RESEARCHER_RULES
@@ -87,38 +87,43 @@
         db.Rule.get_by_('user', Scope.ORGANIZATION, Operation.DELETE),
         db.Rule.get_by_('organization', Scope.ORGANIZATION, Operation.EDIT),
         db.Rule.get_by_('role', Scope.ORGANIZATION, Operation.CREATE),
         db.Rule.get_by_('role', Scope.ORGANIZATION, Operation.EDIT),
         db.Rule.get_by_('role', Scope.ORGANIZATION, Operation.DELETE),
         db.Rule.get_by_('node', Scope.ORGANIZATION, Operation.CREATE),
         db.Rule.get_by_('node', Scope.ORGANIZATION, Operation.EDIT),
-        db.Rule.get_by_('event', Scope.ORGANIZATION, Operation.CREATE),
+        db.Rule.get_by_('event', Scope.ORGANIZATION, Operation.SEND),
     ]
     ORG_ADMIN_ROLE = {
         'name': DefaultRole.ORG_ADMIN,
         'description':
             "Can manage an organization including its users, roles, and nodes."
             " Also has all permissions of a researcher.",
         'rules': ORG_ADMIN_RULES
     }
     # 4. Collaboration administrator role
     COLLAB_ADMIN_RULES = ORG_ADMIN_RULES + [
-        db.Rule.get_by_('user', Scope.GLOBAL, Operation.VIEW),
-        db.Rule.get_by_('user', Scope.GLOBAL, Operation.CREATE),
-        db.Rule.get_by_('user', Scope.GLOBAL, Operation.EDIT),
+        db.Rule.get_by_('user', Scope.COLLABORATION, Operation.VIEW),
+        db.Rule.get_by_('user', Scope.COLLABORATION, Operation.CREATE),
+        db.Rule.get_by_('user', Scope.COLLABORATION, Operation.EDIT),
+        # The following rule is given so that a collaboration admin can
+        # view which organizations they may add to their collaboration
         db.Rule.get_by_('organization', Scope.GLOBAL, Operation.VIEW),
-        db.Rule.get_by_('organization', Scope.GLOBAL, Operation.EDIT),
-        db.Rule.get_by_('collaboration', Scope.GLOBAL, Operation.VIEW),
-        db.Rule.get_by_('collaboration', Scope.GLOBAL, Operation.EDIT),
-        db.Rule.get_by_('role', Scope.GLOBAL, Operation.VIEW),
-        db.Rule.get_by_('node', Scope.GLOBAL, Operation.CREATE),
-        db.Rule.get_by_('node', Scope.GLOBAL, Operation.VIEW),
-        db.Rule.get_by_('node', Scope.GLOBAL, Operation.DELETE),
-        db.Rule.get_by_('event', Scope.COLLABORATION, Operation.VIEW),
-        db.Rule.get_by_('event', Scope.COLLABORATION, Operation.CREATE),
+        db.Rule.get_by_('organization', Scope.COLLABORATION, Operation.EDIT),
+        db.Rule.get_by_('collaboration', Scope.COLLABORATION, Operation.VIEW),
+        db.Rule.get_by_('collaboration', Scope.COLLABORATION, Operation.EDIT),
+        # The following rule is given so that a collaboration admin can
+        # create a new collaboration
+        db.Rule.get_by_('collaboration', Scope.GLOBAL, Operation.CREATE),
+        db.Rule.get_by_('role', Scope.COLLABORATION, Operation.VIEW),
+        db.Rule.get_by_('node', Scope.COLLABORATION, Operation.CREATE),
+        db.Rule.get_by_('node', Scope.COLLABORATION, Operation.VIEW),
+        db.Rule.get_by_('node', Scope.COLLABORATION, Operation.DELETE),
+        db.Rule.get_by_('event', Scope.COLLABORATION, Operation.RECEIVE),
+        db.Rule.get_by_('event', Scope.COLLABORATION, Operation.SEND),
     ]
     COLLAB_ADMIN_ROLE = {
         'name': DefaultRole.COL_ADMIN,
         'description':
             "Can manage an collaboration including its organization and users."
             " Also has permissions of an organization admin.",
         'rules': COLLAB_ADMIN_RULES
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/globals.py` & `vantage6-server-4.0.0a2/vantage6/server/globals.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,20 +27,17 @@
 REFRESH_TOKENS_EXPIRE_HOURS = 48
 
 # Minimum time in seconds that a refresh token must be valid *longer than* the
 # access token. This is to prevent the access token from expiring before the
 # refresh token.
 MIN_REFRESH_TOKEN_EXPIRY_DELTA = 1
 
-# Expiretime of JWT token in a test environment
-JWT_TEST_ACCESS_TOKEN_EXPIRES = datetime.timedelta(days=1)
-
 # Which resources should be initialized. These names correspond to the
 # file-names in the resource directory
-RESOURCES = ['node', 'collaboration', 'organization', 'task', 'result',
+RESOURCES = ['node', 'collaboration', 'organization', 'task', 'run',
              'token', 'user', 'version', 'recover', 'role',
              'rule', 'health', 'vpn', 'port', 'event']
 
 # Super user information. This user is only created if it is not in the
 # database yet at startup time.
 SUPER_USER_INFO = {
     "username": "root",
@@ -48,7 +45,11 @@
 }
 
 # default support email address
 DEFAULT_SUPPORT_EMAIL_ADDRESS = 'support@vantage6.ai'
 
 # default time that token is valid in minutes
 DEFAULT_EMAILED_TOKEN_VALIDITY_MINUTES = 60
+
+# pagination settings
+DEFAULT_PAGE = 1
+DEFAULT_PAGE_SIZE = 10
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/mail_service.py` & `vantage6-server-4.0.0a2/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/__init__.py` & `vantage6-server-4.0.0a2/vantage6/server/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 from vantage6.server.model.organization import Organization
 from vantage6.server.model.collaboration import Collaboration
 from vantage6.server.model.base import Base
 from vantage6.server.model.member import Member
 from vantage6.server.model.node_config import NodeConfig
 from vantage6.server.model.node import Node
 from vantage6.server.model.task import Task
-from vantage6.server.model.result import Result
+from vantage6.server.model.run import Run
 from vantage6.server.model.permission import Permission, UserPermission
 from vantage6.server.model.role import Role
 from vantage6.server.model.rule import Rule
 from vantage6.server.model.role_rule_association import role_rule_association
 from vantage6.server.model.algorithm_port import AlgorithmPort
+from vantage6.server.model.task_database import TaskDatabase
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/algorithm_port.py` & `vantage6-server-4.0.0a2/vantage6/server/model/algorithm_port.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,11 +25,11 @@
     result: :class:`~vantage6.server.model.result.Result`
         The :class:`~vantage6.server.model.result.Result` that this port
         belongs to
     """
 
     # fields
     port = Column(Integer)
-    result_id = Column(Integer, ForeignKey("result.id"))
+    run_id = Column(Integer, ForeignKey("run.id"))
     label = Column(String)
 
-    result = relationship("Result", back_populates="ports")
+    run = relationship("Run", back_populates="ports")
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/authenticatable.py` & `vantage6-server-4.0.0a2/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/base.py` & `vantage6-server-4.0.0a2/vantage6/server/model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 import inspect as class_inspect
+from typing import Any
 from flask.globals import g
 
-from sqlalchemy import Column, Integer, inspect, Table
+from sqlalchemy import Column, Integer, inspect, Table, exists
 from sqlalchemy.orm.session import Session
 from sqlalchemy.ext.declarative import declarative_base, declared_attr
 from sqlalchemy.orm.clsregistry import _ModuleMarker
 from sqlalchemy import create_engine
 from sqlalchemy.engine.url import make_url
 from sqlalchemy.orm import scoped_session, sessionmaker, RelationshipProperty
 from sqlalchemy.orm.exc import NoResultFound
@@ -378,14 +379,37 @@
         """
         session = DatabaseSessionManager.get_session()
 
         session.delete(self)
         session.commit()
 
     @classmethod
+    def exists(cls, field: str, value: Any) -> bool:
+        """
+        Check if a value exists for a given field in the database model.
+
+        Parameters
+        ----------
+        field: str
+            The field to check
+        value: Any
+            The value to check
+
+        Returns
+        -------
+        bool
+            True if the value exists, False otherwise
+        """
+        session = DatabaseSessionManager.get_session()
+        result = session.query(exists().where(getattr(cls, field) == value))\
+            .scalar()
+        session.commit()
+        return result
+
+    @classmethod
     def help(cls) -> None:
         """
         Print a help message for the class.
         """
         i = inspect(cls)
         properties = ''.join([f' ->{a.key}\n' for a in i.mapper.column_attrs])
         relations = ''.join([f' ->{a[0]}\n' for a in i.relationships.items()])
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/collaboration.py` & `vantage6-server-4.0.0a2/vantage6/server/model/collaboration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
-from sqlalchemy import Column, String, Boolean, exists
+from sqlalchemy import Column, String, Boolean
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound
 
 from vantage6.server.model.base import Base, DatabaseSessionManager
 from vantage6.server.model.node import Node
 from vantage6.server.model.organization import Organization
 
 
 class Collaboration(Base):
     """
     Table that describes which collaborations are available.
 
     Collaborations are combinations of one or more organizations
-    that do studies together. Each :class:`.Organization` has a
+    that do studies together. Each
+    :class:`~vantage6.server.model.organization.Organization` has a
     :class:`~vantage6.server.model.node.Node` for
     each collaboration that it is part of. Within a collaboration multiple
-    :class:`.Task` can be executed.
+    :class:`~vantage6.server.model.task.Task` can be executed.
 
     Attributes
     ----------
     name : str
         Name of the collaboration
     encrypted : bool
         Whether the collaboration is encrypted or not
-    organizations : list[:class:`.Organization`]
+    organizations :
+            list[:class:`~vantage6.server.model.organization.Organization`]
         List of organizations that are part of this collaboration
     nodes : list[:class:`~vantage6.server.model.node.Node`]
         List of nodes that are part of this collaboration
-    tasks : list[:class:`.Task`]
+    tasks : list[:class:`~vantage6.server.model.task.Task`]
         List of tasks that are part of this collaboration
     """
 
     # fields
     name = Column(String, unique=True)
     encrypted = Column(Boolean, default=1)
 
@@ -79,84 +81,58 @@
             List of nodes that are part of the given organizations
         """
         return [n for n in self.nodes if n.organization.id in ids]
 
     def get_node_from_organization(
             self, organization: Organization) -> Node | None:
         """
-        Returns the node that is part of the given :class:`.Organization`.
+        Returns the node that is part of the given
+        :class:`~vantage6.server.model.organization.Organization`.
 
         Parameters
         ----------
-        organization: Organization
-            Organization
+        organization: :class:`~vantage6.server.model.organization.Organization`
+            Organization to get node from
 
         Returns
         -------
-        Union[:class:`~vantage6.server.model.node.Node`, None]
+        :class:`~vantage6.server.model.node.Node` | None
             Node for the given organization for this collaboration, or None if
             there is no node for the given organization.
         """
         for node in self.nodes:
             if node.organization.id == organization.id:
                 return node
         return None
 
     @classmethod
     def find_by_name(cls, name: str) -> Collaboration | None:
         """
         Find :class:`.Collaboration` by its name.
 
-        Note
-        ----
-        If multiple collaborations share the same name, the first
-        collaboration found is returned.
-
         Parameters
         ----------
         name: str
             Name of the collaboration
 
         Returns
         -------
         Union[Collaboration, None]
             Collaboration with the given name, or None if no collaboration
             with the given name exists.
         """
-        # FIXME BvB 2022-01-18. From v4+ there shouldn't be any collisions
-        # in collab names anymore, so correct docstring above
         session = DatabaseSessionManager.get_session()
         try:
             result = session.query(cls).filter_by(name=name).first()
             session.commit()
             return result
         except NoResultFound:
             return None
 
-    @classmethod
-    def name_exists(cls, name: str) -> bool:
-        """
-        Check if a collaboration with the given name exists.
-
-        Parameters
-        ----------
-        name: str
-            Name of the collaboration
-
-        Returns
-        -------
-        bool
-            True if a collaboration with the given name exists, else False
-        """
-        session = DatabaseSessionManager.get_session()
-        result = session.query(exists().where(cls.name == name)).scalar()
-        session.commit()
-        return result
-
-    def __repr__(self) -> str:
+    def __repr__(self):
         """
         Returns a string representation of the collaboration.
 
         Returns
         -------
         str
             String representation of the collaboration
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/member.py` & `vantage6-server-4.0.0a2/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/node.py` & `vantage6-server-4.0.0a2/vantage6/server/model/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Organization that the node belongs to
     """
     _hidden_attributes = ['api_key']
 
     id = Column(Integer, ForeignKey('authenticatable.id'), primary_key=True)
 
     # fields
-    name = Column(String)
+    name = Column(String, unique=True)
     api_key = Column(String)
     collaboration_id = Column(Integer, ForeignKey("collaboration.id"))
     organization_id = Column(Integer, ForeignKey("organization.id"))
 
     # relationships
     collaboration = relationship("Collaboration", back_populates='nodes')
     organization = relationship("Organization", back_populates='nodes')
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/node_config.py` & `vantage6-server-4.0.0a2/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/organization.py` & `vantage6-server-4.0.0a2/vantage6/server/model/organization.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,64 +30,46 @@
         Address of the organization
     zipcode : str
         Zipcode of the organization
     country : str
         Country of the organization
     _public_key : bytes
         Public key of the organization
-    collaborations : list[Collaboration]
+    collaborations :
+            list[:class:`~vantage6.server.model.collaboration.Collaboration`]
         List of collaborations that this organization is part of
-    results : list[:class:`~vantage6.server.model.result.Result`]
+    results : list[:class:`~vantage6.server.model.run.Run`]
         List of results that are part of this organization
     nodes : list[:class:`~vantage6.server.model.node.Node`]
         List of nodes that are part of this organization
-    users : list[User]
+    users : list[:class:`~vantage6.server.model.user.User`]
         List of users that are part of this organization
-    created_tasks : list[Task]
+    tasks : list[:class:`~vantage6.server.model.task.Task`]
         List of tasks that are created by this organization
-    roles : list[Role]
+    roles : list[:class:`~vantage6.server.model.role.Role`]
 
     """
     # fields
-    name = Column(String)
+    name = Column(String, unique=True)
     domain = Column(String)
     address1 = Column(String)
     address2 = Column(String)
     zipcode = Column(String)
     country = Column(String)
     _public_key = Column(LargeBinary)
 
     # relations
     collaborations = relationship("Collaboration", secondary="Member",
                                   back_populates="organizations")
-    results = relationship("Result", back_populates="organization")
+    runs = relationship("Run", back_populates="organization")
     nodes = relationship("Node", back_populates="organization")
     users = relationship("User", back_populates="organization")
-    created_tasks = relationship("Task", back_populates="initiator")
+    tasks = relationship("Task", back_populates="init_org")
     roles = relationship("Role", back_populates="organization")
 
-    def get_result_ids(self) -> list[int]:
-        """
-        Returns a list of result ids that are part of this organization.
-
-        Returns
-        -------
-        list[int]
-            List of result ids
-        """
-        # FIXME this should be removed in version 4.0 and above
-        # note that the import below is required since this file (Organization)
-        # is already imported in model.Result
-        from vantage6.server.model.result import Result
-        session = DatabaseSessionManager.get_session()
-        result_ids = session.query(Result.id)\
-                            .filter(Result.organization_id == self.id).all()
-        session.commit()
-        return result_ids
-
     @classmethod
     def get_by_name(cls, name) -> Organization | None:
         """
         Returns the organization with the given name.
 
         Parameters
         ----------
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/permission.py` & `vantage6-server-4.0.0a2/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/result.py` & `vantage6-server-4.0.0a2/vantage6/server/model/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import datetime
 import logging
 
 from sqlalchemy import Column, Text, DateTime, Integer, ForeignKey
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound, MultipleResultsFound
-from sqlalchemy.ext.hybrid import hybrid_property
 
 from vantage6.common import logger_name
 from vantage6.server.model.base import Base
 from vantage6.server.model import (
     Node,
     Collaboration,
     Organization
 )
 from vantage6.server.model.task import Task
 from vantage6.server.model.base import DatabaseSessionManager
 
 log_ = logging.getLogger(logger_name(__name__))
 
 
-class Result(Base):
+class Run(Base):
     """
-    Table that describes which results are available. A Result is the
-    description of a Task as executed by a Node.
+    A Run is the description of a :class:`.~vantage6.server.model.task.Task` as
+    executed by a Node.
 
-    The result (and the input) is encrypted and can be only read by the
+    The input and result fields will be encrypted and can be only read by the
     intended receiver of the message.
 
     Attributes
     ----------
     input : str
         Input data of the task
     task_id : int
@@ -43,19 +42,19 @@
         Time when the task was started
     finished_at : datetime
         Time when the task was finished
     status : str
         Status of the task
     log : str
         Log of the task
-    task : Task
+    task : :class:`.~vantage6.server.model.task.Task`
         Task that was executed
-    organization : Organization
+    organization : :class:`.~vantage6.server.model.organization.Organization`
         Organization that executed the task
-    ports : list[AlgorithmPort]
+    ports : list[:class:`.~vantage6.server.model.algorithm_port.AlgorithmPort`]
         List of ports that are part of this result
     """
 
     # fields
     input = Column(Text)
     task_id = Column(Integer, ForeignKey("task.id"))
     organization_id = Column(Integer, ForeignKey("organization.id"))
@@ -63,17 +62,17 @@
     assigned_at = Column(DateTime, default=datetime.datetime.utcnow)
     started_at = Column(DateTime)
     finished_at = Column(DateTime)
     status = Column(Text)
     log = Column(Text)
 
     # relationships
-    task = relationship("Task", back_populates="results")
-    organization = relationship("Organization", back_populates="results")
-    ports = relationship("AlgorithmPort", back_populates="result")
+    task = relationship("Task", back_populates="runs")
+    organization = relationship("Organization", back_populates="runs")
+    ports = relationship("AlgorithmPort", back_populates="run")
 
     @property
     def node(self) -> Node:
         """
         Returns the node that is associated with this result.
 
         Returns
@@ -82,17 +81,17 @@
             The node that is associated with this result.
         """
         session = DatabaseSessionManager.get_session()
         try:
             node = session.query(Node)\
                 .join(Collaboration)\
                 .join(Organization)\
-                .join(Result)\
+                .join(Run)\
                 .join(Task)\
-                .filter(Result.id == self.id)\
+                .filter(Run.id == self.id)\
                 .filter(self.organization_id == Node.organization_id)\
                 .filter(Task.collaboration_id == Node.collaboration_id)\
                 .one()
             session.commit()
         # FIXME 2022-03-03 BvB: the following errors are not currently
         # forwarded to the user as request response. Make that happen.
         except NoResultFound:
@@ -102,36 +101,24 @@
         except MultipleResultsFound:
             log_.error("Multiple nodes are registered for organization_id "
                        f"{self.organization_id} in the current collaboration. "
                        "Please delete all nodes but one.")
             raise
         return node
 
-    @hybrid_property
-    def complete(self) -> bool:
-        """
-        Returns whether the algorithm run has completed or not.
-
-        Returns
-        -------
-        bool
-            True if the algorithm run has completed, False otherwise.
-        """
-        return self.finished_at is not None
-
     def __repr__(self) -> str:
         """
         Returns a string representation of the result.
 
         Returns
         -------
         str
             String representation of the result.
         """
         return (
-            "<Result "
+            "<Run "
             f"{self.id}: '{self.task.name}', "
             f"organization: {self.organization.name}, "
             f"collaboration: {self.task.collaboration.name}, "
-            f"is_complete: {self.complete}"
+            f"status: {self.status}"
             ">"
         )
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/role.py` & `vantage6-server-4.0.0a2/vantage6/server/model/role.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound
 
 from vantage6.server.model.base import Base, DatabaseSessionManager
 
 
 class Role(Base):
-    """Collection of Rules
+    """Collection of :class:`.~vantage6.server.model.rule.Rule`s
 
     Attributes
     ----------
     name : str
         Name of the role
     description : str
         Description of the role
     organization_id : int
         Id of the organization this role belongs to
-    rules : list[Rule]
+    rules : list[:class:`.~vantage6.server.model.rule.Rule`]
         List of rules that belong to this role
-    organization : Organization
+    organization : :class:`.~vantage6.server.model.organization.Organization`
         Organization this role belongs to
-    users : list[User]
+    users : list[:class:`.~vantage6.server.model.user.User`]
         List of users that belong to this role
     """
 
     # fields
     name = Column(Text)
     description = Column(Text)
     organization_id = Column(Integer, ForeignKey("organization.id"))
@@ -45,15 +45,15 @@
         Parameters
         ----------
         name : str
             Name of the role
 
         Returns
         -------
-        Role | None
+        :class:`.~vantage6.server.model.role.Role` | None
             Role with the given name or None if no role with the given name
             exists
         """
         session = DatabaseSessionManager.get_session()
         try:
             result = session.query(cls).filter_by(name=name).first()
             session.commit()
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/rule.py` & `vantage6-server-4.0.0a2/vantage6/server/model/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 
 from sqlalchemy import Column, Text, String, Enum
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound
 from vantage6.server.model.base import Base, DatabaseSessionManager
 
 
-class Operation(Enumerate):
+class Operation(str, Enumerate):
     """ Enumerator of all available operations """
     VIEW = "v"
     EDIT = "e"
     CREATE = "c"
     DELETE = "d"
+    SEND = "s"
+    RECEIVE = "r"
 
 
-class Scope(Enumerate):
+class Scope(str, Enumerate):
     """ Enumerator of all available scopes """
     OWN = "own"
     ORGANIZATION = "org"
     COLLABORATION = "col"
     GLOBAL = "glo"
 
 
@@ -37,17 +39,17 @@
         Name of the rule
     operation : Operation
         Operation of the rule
     scope : Scope
         Scope of the rule
     description : str
         Description of the rule
-    roles : list[Role]
+    roles : list[:class:`.~vantage6.server.model.role.Role`]
         Roles that have this rule
-    users : list[User]
+    users : list[:class:`.~vantage6.server.model.user.User`]
         Users that have this rule
     """
 
     # fields
     name = Column(Text)
     operation = Column(Enum(Operation))
     scope = Column(Enum(Scope))
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/task.py` & `vantage6-server-4.0.0a2/vantage6/server/model/task.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from sqlalchemy import Column, String, ForeignKey, Integer, sql
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.hybrid import hybrid_property
 
 from vantage6.common.task_status import TaskStatus, has_task_failed
-from vantage6.server.model.node import Node
 from vantage6.server.model.base import Base, DatabaseSessionManager
 
 
 class Task(Base):
     """
     Table that describes all tasks.
 
-    A task can contain multiple Results for multiple organizations. The input
+    A Task can create algorithm Runs for multiple organizations. The input
     of the task is different for each organization (due to the encryption).
     Therefore the input for the task is encrypted for each organization
-    separately. The task originates from an organization to which the results
+    separately. The task originates from an organization to which the Runs
     need to be encrypted, therefore the originating organization is also logged
 
     Attributes
     ----------
     name : str
         Name of the task
     description : str
@@ -29,15 +28,15 @@
         Id of the collaboration that this task belongs to
     run_id : int
         Run id of the task
     parent_id : int
         Id of the parent task (if any)
     database : str
         Name of the database that needs to be used for this task
-    initiator_id : int
+    init_org_id : int
         Id of the organization that created this task
     init_user_id : int
         Id of the user that created this task
 
     collaboration : :class:`~.model.collaboration.Collaboration`
         Collaboration that this task belongs to
     parent : :class:`~.model.task.Task`
@@ -51,106 +50,66 @@
 
     """
     # fields
     name = Column(String)
     description = Column(String)
     image = Column(String)
     collaboration_id = Column(Integer, ForeignKey("collaboration.id"))
-    run_id = Column(Integer)
+    job_id = Column(Integer)
     parent_id = Column(Integer, ForeignKey("task.id"))
-    database = Column(String)
-    initiator_id = Column(Integer, ForeignKey("organization.id"))
+    init_org_id = Column(Integer, ForeignKey("organization.id"))
     init_user_id = Column(Integer, ForeignKey("user.id"))
 
     # relationships
     collaboration = relationship("Collaboration", back_populates="tasks")
     parent = relationship("Task", remote_side="Task.id", backref="children")
-    results = relationship("Result", back_populates="task")
-    # TODO in v4, rename the 'initiator' column so that there is a clear
-    # distinction between initiating organization and user
-    initiator = relationship("Organization", back_populates="created_tasks")
+    runs = relationship("Run", back_populates="task")
+    init_org = relationship("Organization", back_populates="tasks")
     init_user = relationship("User", back_populates="created_tasks")
-
-    # TODO remove this property in v4. It is superseded by status but now left
-    # here for backwards compatibility with other v3 versions
-    @hybrid_property
-    def complete(self) -> bool:
-        """
-        Determine if a task is complete, i.e. whether all underlying results
-        are complete.
-
-        Returns
-        -------
-        bool
-            True if task is complete, False otherwise
-        """
-        return all([r.complete for r in self.results])
+    databases = relationship("TaskDatabase", back_populates="task")
 
     @hybrid_property
     def status(self) -> str:
         """
         Returns the status of a task, which is derived from the statuses of
         the underlying algorithm runs.
 
         Returns
         -------
         str
             Status of task
         """
         # TODO what if there are no result ids? -> currently returns unknown
-        result_statuses = [r.status for r in self.results]
-        if all([status is None for status in result_statuses]):
-            # TODO remove in v4 (this is for backwards compatibility because
-            # task statuses where not present in <3.6)
-            return 'unknown'
-        elif any([has_task_failed(status) for status in result_statuses]):
+        run_statuses = [r.status for r in self.runs]
+        if any([has_task_failed(status) for status in run_statuses]):
             return TaskStatus.FAILED.value
-        elif TaskStatus.ACTIVE in result_statuses:
+        elif TaskStatus.ACTIVE in run_statuses:
             return TaskStatus.ACTIVE.value
-        elif TaskStatus.INITIALIZING in result_statuses:
+        elif TaskStatus.INITIALIZING in run_statuses:
             return TaskStatus.INITIALIZING.value
-        elif TaskStatus.PENDING in result_statuses:
+        elif TaskStatus.PENDING in run_statuses:
             return TaskStatus.PENDING.value
         else:
             return TaskStatus.COMPLETED.value
 
-    def results_for_node(self, node: Node) -> list:
-        """
-        Get all results for a given node.
-
-        Parameters
-        ----------
-        node: model.node.Node
-            Node for which to get the results
-
-        Returns
-        -------
-        List[model.result.Result]
-            List of results for the given node
-        """
-        assert isinstance(node, Node), "Should be a node..."
-        return [result for result in self.results if
-                self.collaboration == node.collaboration and
-                self.organization == node.organization]
-
     @classmethod
-    def next_run_id(cls) -> int:
+    def next_job_id(cls) -> int:
         """
         Get the next available run id for a new task.
 
         Returns
         -------
         int
             Next available run id
         """
         session = DatabaseSessionManager.get_session()
-        max_run_id = session.query(sql.func.max(cls.run_id)).scalar()
+        max_job_id = session.query(sql.func.max(cls.job_id)).scalar()
         session.commit()
-        if max_run_id:
-            return max_run_id + 1
+        if max_job_id:
+            return max_job_id + 1
         else:
             return 1
 
     def __repr__(self) -> str:
         """
         String representation of the Task object
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/model/user.py` & `vantage6-server-4.0.0a2/vantage6/server/model/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 import bcrypt
-import re
 import datetime as dt
 
-from sqlalchemy import Column, String, Integer, ForeignKey, exists, DateTime
+from sqlalchemy import Column, String, Integer, ForeignKey, DateTime
 from sqlalchemy.orm import relationship, validates
 
 from vantage6.server.model.base import DatabaseSessionManager
 from vantage6.server.model.authenticatable import Authenticatable
 from vantage6.server.model.rule import Operation, Rule, Scope
+from vantage6.server.model.common.utils import validate_password
 
 
 class User(Authenticatable):
     """
     Table to keep track of Users (persons) that can access the system.
 
     Users always belong to an organization and can have certain
@@ -123,31 +123,18 @@
 
         Returns
         -------
         str | None
             If the new password fails to pass the checks, a message is
             returned. Else, none is returned
         """
-        if len(pw) < 8:
-            return (
-                "Password too short: use at least 8 characters with mixed "
-                "lowercase, uppercase, numbers and special characters"
-            )
-        elif len(pw) > 128:
-            # because long passwords can be used for DoS attacks (long pw
-            # hashing consumes a lot of resources)
-            return "Password too long: use at most 128 characters"
-        elif re.search('[0-9]', pw) is None:
-            return "Password should contain at least one number"
-        elif re.search('[A-Z]', pw) is None:
-            return "Password should contain at least one uppercase letter"
-        elif re.search('[a-z]', pw) is None:
-            return "Password should contain at least one lowercase letter"
-        elif pw.isalnum():
-            return "Password should contain at least one special character"
+        try:
+            validate_password(pw)
+        except ValueError as e:
+            return str(e)
 
         self.password = pw
         self.save()
 
     def check_password(self, pw: str) -> bool:
         """
         Check if the password is correct
@@ -248,56 +235,29 @@
         """
         session = DatabaseSessionManager.get_session()
         result = session.query(cls).filter_by(email=email).one()
         session.commit()
         return result
 
     @classmethod
-    def username_exists(cls, username: str) -> bool:
+    def username_exists(cls, username) -> bool:
         """
-        Checks if user with certain username exists
+        Check if a user with the given username exists
 
         Parameters
         ----------
         username: str
             Username to check
 
         Returns
         -------
         bool
-            Whether or not user with given username exists
+            Whether or not a user with the given username exists
         """
-        session = DatabaseSessionManager.get_session()
-        result = session.query(exists().where(cls.username == username))\
-            .scalar()
-        session.commit()
-        return result
-
-    @classmethod
-    def exists(cls, field: str, value: str) -> bool:
-        """
-        Checks if user with certain key-value exists
-
-        Parameters
-        ----------
-        field: str
-            Name of the attribute to check
-        value: str
-            Value of the attribute to check
-
-        Returns
-        -------
-        bool
-            Whether or not user with given key-value exists
-        """
-        session = DatabaseSessionManager.get_session()
-        result = session.query(exists().where(getattr(cls, field) == value))\
-            .scalar()
-        session.commit()
-        return result
+        return cls.exists(field='username', value=username)
 
     def can(self, resource: str, scope: Scope, operation: Operation) -> bool:
         """
         Check if user is allowed to execute a certain action
 
         Parameters
         ---------
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/permission.py` & `vantage6-server-4.0.0a2/vantage6/server/permission.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 import importlib
 
 from collections import namedtuple
 from flask_principal import Permission, PermissionDenied
 
 from vantage6.server.globals import RESOURCES
 from vantage6.server.default_roles import DefaultRole
+from vantage6.server.model.base import Base
 from vantage6.server.model.role import Role
 from vantage6.server.model.rule import Rule, Operation, Scope
 from vantage6.server.model.base import DatabaseSessionManager
+from vantage6.server.utils import (
+    obtain_auth_collaborations, obtain_auth_organization
+)
 from vantage6.common import logger_name
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 RuleNeed = namedtuple("RuleNeed", ["name", "scope", "operation"])
 
 
-class RuleCollection:
+class RuleCollection(dict):
     """
     Class that tracks a set of all rules for a certain resource name
 
     Parameters
     ----------
     name: str
         Name of the resource endpoint (e.g. node, organization, user)
@@ -38,15 +42,184 @@
         ----------
         scope: Scope
             Scope within which to apply the rule
         operation: Operation
             What operation the rule applies to
         """
         permission = Permission(RuleNeed(self.name, scope, operation))
-        self.__setattr__(f'{operation.value}_{scope.value}', permission)
+        self.__setattr__(f'{operation}_{scope}', permission)
+
+    def can_for_org(self, operation: Operation, subject_org_id: int) -> bool:
+        """
+        Check if an operation is allowed on a certain organization
+
+        Parameters
+        ----------
+        operation: Operation
+            Operation to check if allowed
+        subject_org_id: int
+            Organization id on which the operation should be allowed
+
+        Returns
+        -------
+        bool
+            True if the operation is allowed on the organization, False
+            otherwise
+        """
+        auth_org = obtain_auth_organization()
+
+        # check if the entity has global permission
+        global_perm = getattr(self, f'{operation}_{Scope.GLOBAL}')
+        if global_perm and global_perm.can():
+            return True
+
+        # check if the entity has organization permission and organization is
+        # the same as the subject organization
+        org_perm = getattr(self, f'{operation}_{Scope.ORGANIZATION}')
+        if auth_org.id == subject_org_id and org_perm and org_perm.can():
+            return True
+
+        # check if the entity has collaboration permission and the subject
+        # organization is in the collaboration of the own organization
+        col_perm = getattr(self, f'{operation}_{Scope.COLLABORATION}')
+        if col_perm and col_perm.can():
+            for col in auth_org.collaborations:
+                if subject_org_id in [org.id for org in col.organizations]:
+                    return True
+
+        # no permission found
+        return False
+
+    def can_for_col(self, operation: Operation, collaboration_id: int) -> bool:
+        """
+        Check if the user or node can perform the operation on a certain
+        collaboration
+
+        Parameters
+        ----------
+        operation: Operation
+            Operation to check if allowed
+        collaboration_id: int
+            Collaboration id on which the operation should be allowed
+        """
+        auth_collabs = obtain_auth_collaborations()
+
+        # check if the entity has global permission
+        global_perm = getattr(self, f'{operation}_{Scope.GLOBAL}')
+        if global_perm and global_perm.can():
+            return True
+
+        # check if the entity has collaboration permission and the subject
+        # collaboration is in the collaborations of the user/node
+        col_perm = getattr(self, f'{operation}_{Scope.COLLABORATION}')
+        if col_perm and col_perm.can() and \
+                self._id_in_list(collaboration_id, auth_collabs):
+            return True
+
+        # no permission found
+        return False
+
+    def get_max_scope(self, operation: Operation) -> Scope | None:
+        """
+        Get the highest scope that the entity has for a certain operation
+
+        Parameters
+        ----------
+        operation: Operation
+            Operation to check
+
+        Returns
+        -------
+        Scope | None
+            Highest scope that the entity has for the operation. None if the
+            entity has no permission for the operation
+        """
+        if getattr(self, f'{operation}_{Scope.GLOBAL}'):
+            return Scope.GLOBAL
+        elif getattr(self, f'{operation}_{Scope.COLLABORATION}'):
+            return Scope.COLLABORATION
+        elif getattr(self, f'{operation}_{Scope.ORGANIZATION}'):
+            return Scope.ORGANIZATION
+        elif getattr(self, f'{operation}_{Scope.OWN}'):
+            return Scope.OWN
+        else:
+            return None
+
+    def has_at_least_scope(self, scope: Scope, operation: Operation) -> bool:
+        """
+        Check if the entity has at least a certain scope for a certain
+        operation
+
+        Parameters
+        ----------
+        scope: Scope
+            Scope to check if the entity has at least
+        operation: Operation
+            Operation to check
+
+        Returns
+        -------
+        bool
+            True if the entity has at least the scope, False otherwise
+        """
+        scopes: list[Scope] = self._get_scopes_from(scope)
+        for s in scopes:
+            perm = getattr(self, f'{operation}_{s}')
+            if perm and perm.can():
+                return True
+        return False
+
+    def _id_in_list(self, id_: int, resource_list: list[Base]) -> bool:
+        """
+        Check if resource list contains a resource with a certain ID
+
+        Parameters
+        ----------
+        id_ : int
+            ID of the resource
+        resource_list : list[db.Base]
+            List of resources
+
+        Returns
+        -------
+        bool
+            True if resource is in list, False otherwise
+        """
+        return any(r.id == id_ for r in resource_list)
+
+    def _get_scopes_from(self, minimal_scope: Scope) -> list[Scope]:
+        """
+        Get scopes that are at least equal to a certain scope
+
+        Parameters
+        ----------
+        minimal_scope: Scope
+            Minimal scope
+
+        Returns
+        -------
+        list[Scope]
+            List of scopes that are at least equal to the minimal scope
+
+        Raises
+        ------
+        ValueError
+            If the minimal scope is not known
+        """
+        if minimal_scope == Scope.ORGANIZATION:
+            return [Scope.ORGANIZATION, Scope.COLLABORATION, Scope.GLOBAL]
+        elif minimal_scope == Scope.COLLABORATION:
+            return [Scope.COLLABORATION, Scope.GLOBAL]
+        elif minimal_scope == Scope.GLOBAL:
+            return [Scope.GLOBAL]
+        elif minimal_scope == Scope.OWN:
+            return [Scope.OWN, Scope.ORGANIZATION, Scope.COLLABORATION,
+                    Scope.GLOBAL]
+        else:
+            raise ValueError(f"Unknown scope '{minimal_scope}'")
 
 
 class PermissionManager:
     """
     Loads the permissions and syncs rules in database with rules defined in
     the code
     """
@@ -297,15 +470,15 @@
     @staticmethod
     def check_user_rules(rules: list[Rule]) -> dict | bool:
         """
         Check if a user, node or container has all the `rules` in a list
 
         Parameters
         ----------
-        rules: List[Rule]
+        rules: list[:class:`~vantage6.server.model.rule.Rule`]
             List of rules that user is checked to have
 
         Returns
         -------
         dict | bool
             Dict with a message which rule is missing, else None
         """
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/__init__.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 from flask import g, request
 from flask_restful import Resource, Api
 from flask_mail import Mail
 from flask_jwt_extended import (
     get_jwt, get_jwt_identity, jwt_required
 )
 from flask_socketio import SocketIO
-from marshmallow_sqlalchemy import ModelSchema
 
 
 from vantage6.common import logger_name
 from vantage6.server import db
+from vantage6.server.utils import (
+    obtain_auth_collaborations, obtain_auth_organization
+)
+from vantage6.server.model.authenticatable import Authenticatable
+from vantage6.server.resource.common.output_schema import HATEOASModelSchema
 from vantage6.server.permission import PermissionManager
-from vantage6.server.resource.pagination import Page
+from vantage6.server.resource.common.pagination import Page
 
 log = logging.getLogger(logger_name(__name__))
 
 
 class ServicesResources(Resource):
     """
     Flask resource base class.
@@ -64,44 +68,41 @@
         Returns
         -------
         bool
             True if the field is included, False otherwise
         """
         return field in request.args.getlist('include')
 
-    def dump(self, page: Page, schema: ModelSchema) -> dict:
+    def dump(self, page: Page, schema: HATEOASModelSchema) -> dict:
         """
         Dump based on the request context (to paginate or not)
 
         Parameters
         ----------
         page : Page
             Page object to dump
-        schema : ModelSchema
+        schema : HATEOASModelSchema
             Schema to use for dumping
 
         Returns
         -------
         dict
             Dumped page
         """
-        if self.is_included('metadata'):
-            return schema.meta_dump(page)
-        else:
-            return schema.default_dump(page)
+        return schema.meta_dump(page)
 
-    def response(self, page: Page, schema: ModelSchema):
+    def response(self, page: Page, schema: HATEOASModelSchema):
         """
         Prepare a valid HTTP OK response from a page object
 
         Parameters
         ----------
         page : Page
             Page object to dump
-        schema : ModelSchema
+        schema : HATEOASModelSchema
             Schema to use for dumping
 
         Returns
         -------
         tuple
             Tuple of (dumped page, HTTPStatus.OK, headers of the page)
         """
@@ -148,21 +149,33 @@
         Obtain the organization model from the auth that is logged in.
 
         Returns
         -------
         db.Organization
             Organization model
         """
-        return db.Organization.get(cls.obtain_organization_id())
+        return obtain_auth_organization()
+
+    @staticmethod
+    def obtain_auth_collaborations() -> list[db.Collaboration]:
+        """
+        Obtain the collaborations that the auth is part of.
+
+        Returns
+        -------
+        list[db.Collaboration]
+            List of collaborations
+        """
+        return obtain_auth_collaborations()
 
 
 # ------------------------------------------------------------------------------
 # Helper functions/decoraters ...
 # ------------------------------------------------------------------------------
-def only_for(types: tuple[str] = ('user', 'node', 'container')):
+def only_for(types: tuple[str] = ('user', 'node', 'container')) -> callable:
     """
     JWT endpoint protection decorator
 
     Parameters
     ----------
     types : list[str]
         List of types that are allowed to access the endpoint. Possible types
@@ -266,7 +279,41 @@
     -------
     datetime
         Datetime object
     """
     if dt:
         return datetime.datetime.strptime(dt, '%Y-%m-%dT%H:%M:%S.%f')
     return default
+
+
+def get_org_ids_from_collabs(auth: Authenticatable,
+                             collab_id: int = None) -> list[int]:
+    """
+    Get all organization ids from the collaborations the user or node is in.
+
+    Parameters
+    ----------
+    auth : Authenticatable
+        User or node
+    collab_id : int, optional
+        Collaboration id. If given, only return the organization ids of this
+        collaboration. If not given, return all organization ids of all
+        collaborations the user or node is in.
+
+    Returns
+    -------
+    list[int]
+        List of organization ids
+    """
+    if collab_id:
+        return [
+            org.id
+            for col in auth.organization.collaborations
+            for org in col.organizations
+            if col.id == collab_id
+        ]
+    else:
+        return [
+            org.id
+            for col in auth.organization.collaborations
+            for org in col.organizations
+        ]
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/collaboration.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/collaboration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # -*- coding: utf-8 -*-
 import logging
 
 from flask import request, g
-from flask_restful import reqparse, Api
+from flask_restful import Api
 from http import HTTPStatus
 
 from vantage6.server import db
-from vantage6.server.resource.pagination import Pagination
+from vantage6.server.resource.common.pagination import Pagination
+from vantage6.server.resource.common.input_schema import (
+    CollaborationAddNodeSchema,
+    CollaborationAddOrganizationSchema,
+    CollaborationInputSchema
+)
 from vantage6.server.permission import (
+    RuleCollection,
     Scope as S,
     Operation as P,
     PermissionManager
 )
-from vantage6.server.resource.common._schema import (
+from vantage6.server.resource.common.output_schema import (
     CollaborationSchema,
-    TaskSchema,
     OrganizationSchema,
     NodeSchemaSimple
 )
 from vantage6.server.resource import (
-    with_user_or_node,
     with_user,
     only_for,
     ServicesResources
 )
 
 
 module_name = __name__.split('.')[-1]
@@ -60,38 +64,33 @@
         methods=('GET', 'PATCH', 'DELETE'),
         resource_class_kwargs=services
     )
     api.add_resource(
         CollaborationOrganization,
         path+'/<int:id>/organization',
         endpoint='collaboration_with_id_organization',
-        methods=('GET', 'POST', 'DELETE'),
+        methods=('POST', 'DELETE'),
         resource_class_kwargs=services
     )
     api.add_resource(
         CollaborationNode,
         path+'/<int:id>/node',
         endpoint='collaboration_with_id_node',
-        methods=('GET', 'POST', 'DELETE'),
-        resource_class_kwargs=services
-    )
-    api.add_resource(
-        CollaborationTask,
-        path+'/<int:id>/task',
-        endpoint='collaboration_with_id_task',
-        methods=('GET',),
+        methods=('POST', 'DELETE'),
         resource_class_kwargs=services
     )
 
 
 # Schemas
 collaboration_schema = CollaborationSchema()
-tasks_schema = TaskSchema()
 org_schema = OrganizationSchema()
 node_schema = NodeSchemaSimple()
+collaboration_input_schema = CollaborationInputSchema()
+collaboration_add_organization_schema = CollaborationAddOrganizationSchema()
+collaboration_add_node_schema = CollaborationAddNodeSchema()
 
 
 # -----------------------------------------------------------------------------
 # Permissions
 # -----------------------------------------------------------------------------
 def permissions(permissions: PermissionManager) -> None:
     """
@@ -110,35 +109,41 @@
 
     add(scope=S.ORGANIZATION, operation=P.VIEW, assign_to_container=True,
         assign_to_node=True,
         description="view collaborations of your organization")
 
     add(scope=S.GLOBAL, operation=P.EDIT,
         description="edit any collaboration")
+    add(scope=S.COLLABORATION, operation=P.EDIT,
+        description="edit any collaboration that your organization "
+                    "participates in")
 
     add(scope=S.GLOBAL, operation=P.CREATE,
         description="create a new collaboration")
 
     add(scope=S.GLOBAL, operation=P.DELETE,
         description="delete a collaboration")
+    add(scope=S.COLLABORATION, operation=P.DELETE,
+        description="delete any collaboration that your organization "
+                    "participates in")
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 class CollaborationBase(ServicesResources):
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
 
 
 class Collaborations(CollaborationBase):
 
-    @with_user
+    @only_for(['user', 'node'])
     def get(self):
         """Returns a list of collaborations
         ---
         description: >-
           Returns a list of collaborations. Depending on your permission, all
           collaborations are shown or only collaborations in which your
           organization participates. See the table bellow.\n\n
@@ -170,35 +175,38 @@
             description: Whether or not collaboration is encrypted
           - in: query
             name: organization_id
             schema:
               type: integer
             description: Organization id
           - in: query
-            name: include
-            schema:
-              type: string
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
             name: page
             schema:
               type: integer
-            description: Page number for pagination
+            description: Page number for pagination (default=1)
           - in: query
             name: per_page
             schema:
               type: integer
-            description: Number of items per page
+            description: Number of items per page (default=10)
+          - in: query
+            name: sort
+            schema:
+              type: string
+            description: >-
+              Sort by one or more fields, separated by a comma. Use a minus
+              sign (-) in front of the field to sort in descending order.
 
         responses:
           200:
             description: Ok
           401:
             description: Unauthorized
+          400:
+            description: Improper values for pagination or sorting parameters
 
         security:
           - bearerAuth: []
 
         tags: ["Collaboration"]
         """
 
@@ -233,17 +241,20 @@
                 q = q.join(db.Organization, db.Collaboration.organizations)\
                     .filter(db.Collaboration.organizations.any(id=auth_org_id))
             else:
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
         # paginate the results
-        page = Pagination.from_query(query=q, request=request)
+        try:
+            page = Pagination.from_query(q, request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
-        # serialize models, include metadata if requested
+        # serialize models
         return self.response(page, collaboration_schema)
 
     @with_user
     def post(self):
         """ Create collaboration
         ---
         description: >-
@@ -285,24 +296,23 @@
             description: Unauthorized
 
         security:
           - bearerAuth: []
 
         tags: ["Collaboration"]
         """
-        parser = reqparse.RequestParser()
-        parser.add_argument('name', type=str, required=True,
-                            help="This field cannot be left blank!")
-        parser.add_argument('organization_ids', type=int, required=True,
-                            action='append')
-        parser.add_argument('encrypted', type=int, required=False)
-        data = parser.parse_args()
+        data = request.get_json()
+        # validate request body
+        errors = collaboration_input_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         name = data["name"]
-        if db.Collaboration.name_exists(name):
+        if db.Collaboration.exists("name", name):
             return {"msg": f"Collaboration name '{name}' already exists!"}, \
                 HTTPStatus.BAD_REQUEST
 
         if not self.r.c_glo.can():
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
@@ -315,15 +325,15 @@
                 for org_id in data['organization_ids']
                 if db.Organization.get(org_id)
             ],
             encrypted=encrypted
         )
 
         collaboration.save()
-        return collaboration_schema.dump(collaboration).data, HTTPStatus.OK
+        return collaboration_schema.dump(collaboration), HTTPStatus.OK
 
 
 class Collaboration(CollaborationBase):
 
     @only_for(('user', 'node', 'container'))
     def get(self, id):
         """ Get collaboration
@@ -377,28 +387,30 @@
         # collaboration
         ids = [org.id for org in collaboration.organizations]
         if not self.r.v_glo.can():
             if not (self.r.v_org.can() and auth_org_id in ids):
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
-        return collaboration_schema.dump(collaboration, many=False).data, \
+        return collaboration_schema.dump(collaboration, many=False), \
             HTTPStatus.OK  # 200
 
     @with_user
     def patch(self, id):
         """ Update collaboration
         ---
         description: >-
           Updates the collaboration with the specified id.\n\n
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Collaboration|Global|Edit|❌|❌|Update a collaboration|\n\n
+          |Collaboration|Collaboration|Edit|❌|❌|Update a collaboration that
+          you are already a member of|\n\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
@@ -426,72 +438,94 @@
         responses:
           200:
             description: Ok
           404:
             description: Collaboration with specified id is not found
           401:
             description: Unauthorized
+          400:
+            description: Collaboration name already exists
 
         security:
           - bearerAuth: []
 
         tags: ["Collaboration"]
         """
         collaboration = db.Collaboration.get(id)
 
         # check if collaboration exists
         if not collaboration:
             return {"msg": f"collaboration having collaboration_id={id} "
                     "can not be found"}, HTTPStatus.NOT_FOUND  # 404
 
         # verify permissions
-        if not self.r.e_glo.can():
+        if not self.r.can_for_col(P.EDIT, collaboration.id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
-        # only update fields that are provided
         data = request.get_json()
+        # validate request body
+        errors = collaboration_input_schema.validate(data, partial=True)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
+        # only update fields that are provided
         if "name" in data:
-            collaboration.name = data["name"]
+            name = data["name"]
+            if collaboration.name != name and \
+                    db.Collaboration.exists("name", name):
+                return {
+                    "msg": f"Collaboration name '{name}' already exists!"
+                }, HTTPStatus.BAD_REQUEST
+            collaboration.name = name
         if "organization_ids" in data:
             collaboration.organizations = [
                 db.Organization.get(org_id)
                 for org_id in data['organization_ids']
                 if db.Organization.get(org_id)
             ]
         if 'encrypted' in data:
             collaboration.encrypted = data['encrypted']
 
         collaboration.save()
 
-        return collaboration_schema.dump(collaboration, many=False).data, \
+        return collaboration_schema.dump(collaboration, many=False), \
             HTTPStatus.OK  # 200
 
     @with_user
     def delete(self, id):
         """ Delete collaboration
         ---
         description: >-
           Removes the collaboration from the database entirely.
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Collaboration|Global|Delete|❌|❌|Remove collaboration|\n\n
+          |Collaboration|Collaboration|Delete|❌|❌|Remove collaborations
+          that you are part of yourself|\n\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
               type: integer
             description: Collaboration id
             required: true
+          - in: query
+            name: delete_dependents
+            schema:
+              type: boolean
+            description: If set to true, the collaboratio will be deleted along
+              with all its tasks and nodes (default=False)
 
         responses:
           200:
             description: Ok
           404:
             description: Collaboration with specified id is not found
           401:
@@ -505,116 +539,63 @@
 
         collaboration = db.Collaboration.get(id)
         if not collaboration:
             return {"msg": f"collaboration id={id} is not found"}, \
                 HTTPStatus.NOT_FOUND
 
         # verify permissions
-        if not self.r.d_glo.can():
+        if not self.r.can_for_col(P.DELETE, collaboration.id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
+        if collaboration.tasks or collaboration.nodes:
+            delete_dependents = request.args.get('delete_dependents', False)
+            if not delete_dependents:
+                return {
+                    "msg": f"Collaboration id={id} has "
+                    f"{len(collaboration.tasks)} tasks and "
+                    f"{len(collaboration.nodes)} nodes. Please delete them "
+                    "separately or set delete_dependents=True"
+                }, HTTPStatus.BAD_REQUEST
+            else:
+                log.warn(f"Deleting collaboration id={id} along with "
+                         f"{len(collaboration.tasks)} tasks and "
+                         f"{len(collaboration.nodes)} nodes")
+                for task in collaboration.tasks:
+                    task.delete()
+                for node in collaboration.nodes:
+                    node.delete()
+
         collaboration.delete()
         return {"msg": f"Collaboration id={id} successfully deleted"}, \
             HTTPStatus.OK
 
 
 class CollaborationOrganization(ServicesResources):
     """Resource for /api/collaboration/<int:id>/organization."""
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
-
-    @only_for(("node", "user", "container"))
-    def get(self, id):
-        """ Returns organizations that participate in the collaboration
-        ---
-        description: >-
-          Returns a list of all organizations that belong to the specified
-          collaboration.
-
-          ### Permission Table\n
-          |Rulename|Scope|Operation|Assigned to Node|Assigned to Container|
-          Description|\n
-          |--|--|--|--|--|--|\n
-          |Collaboration|Global|View|❌|❌|All collaborations|\n
-          |Collaboration|Organization|View|✅|✅|Collaborations
-          in which your organization participates|\n\n
-
-          Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            description: Collaboration id
-            required: true
-          - in: query
-            name: include
-            schema:
-              type: string
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
-            name: page
-            schema:
-              type: integer
-            description: Page number for pagination
-          - in: query
-            name: per_page
-            schema:
-              type: integer
-            description: Number of items per page
-
-        responses:
-            200:
-                description: Ok
-            404:
-                description: Collaboration specified by id does not exists
-            401:
-                description: Unauthorized
-
-        security:
-            - bearerAuth: []
-
-        tags: ["Collaboration"]
-        """
-        col = db.Collaboration.get(id)
-        if not col:
-            return {'msg': f'collaboration (id={id}) can not be found'},\
-                HTTPStatus.NOT_FOUND
-
-        # check permission
-        if not self.r.v_glo.can():
-            auth_org = self.obtain_auth_organization()
-            if not (self.r.v_org.can() and auth_org in col.organizations):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        # paginate organizations
-        page = Pagination.from_list(col.organizations, request)
-
-        # model serialization
-        return self.response(page, org_schema)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
 
     @with_user
     def post(self, id):
         """ Add organization to collaboration
         ---
         description: >-
           Adds a single organization to an existing collaboration.\n\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Collaboration|Global|Edit|❌|❌|Add organization to a
           collaboration|\n\n
+          |Collaboration|Collaboration|Edit|❌|❌|Add organization to a
+          collaboration that your organization is already a member of|\n\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
@@ -647,29 +628,35 @@
         # get collaboration to which te organization should be added
         collaboration = db.Collaboration.get(id)
         if not collaboration:
             return {"msg": f"collaboration having collaboration_id={id} can "
                     "not be found"}, HTTPStatus.NOT_FOUND
 
         # verify permissions
-        if not self.r.e_glo.can():
+        if not self.r.can_for_col(P.EDIT, collaboration.id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
-        # get the organization
+        # validate request body
         data = request.get_json()
+        errors = collaboration_add_organization_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
+        # get the organization
         organization = db.Organization.get(data['id'])
         if not organization:
             return {"msg": f"organization with id={id} is not found"}, \
                 HTTPStatus.NOT_FOUND
 
         # append organization to the collaboration
         collaboration.organizations.append(organization)
         collaboration.save()
-        return org_schema.dump(collaboration.organizations, many=True).data, \
+        return org_schema.dump(collaboration.organizations, many=True), \
             HTTPStatus.OK
 
     @with_user
     def delete(self, id):
         """ Remove organization from collaboration
         ---
         description: >-
@@ -677,14 +664,16 @@
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Collaboration|Global|Edit|❌|❌|Remove an organization from an
           existing collaboration|\n\n
+          |Collaboration|Collaboration|Edit|❌|❌|Remove an organization from
+          an existing collaboration that your organization is a member of|\n\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
@@ -710,125 +699,56 @@
             description: Unauthorized
 
         tags: ["Collaboration"]
         """
         # get collaboration from which organization should be removed
         collaboration = db.Collaboration.get(id)
         if not collaboration:
-            return {"msg": f"collaboration having collaboration_id={id} can "
+            return {"msg": f"Collaboration with collaboration_id={id} can "
                     "not be found"}, HTTPStatus.NOT_FOUND
 
         # get organization which should be deleted
         data = request.get_json()
         organization = db.Organization.get(data['id'])
         if not organization:
-            return {"msg": f"organization with id={id} is not found"}, \
+            return {"msg": f"Organization with id={id} is not found"}, \
                 HTTPStatus.NOT_FOUND
 
-        if not self.r.d_glo.can():
+        if not self.r.can_for_col(P.EDIT, collaboration.id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
         # delete organization and update
         collaboration.organizations.remove(organization)
         collaboration.save()
-        return org_schema.dump(collaboration.organizations, many=True).data, \
+        return org_schema.dump(collaboration.organizations, many=True), \
             HTTPStatus.OK
 
 
 class CollaborationNode(ServicesResources):
     """Resource for /api/collaboration/<int:id>/node."""
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
-
-    @with_user
-    def get(self, id):
-        """ List nodes in collaboration.
-        ---
-        description: >-
-          Returns a list of node(s) which belong to the specified
-          collaboration.\n
-
-          ### Permission Table\n
-          |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-          Description|\n
-          |--|--|--|--|--|--|\n
-          |Collaboration|Global|View|❌|❌|List nodes in a specified
-          collaboration|\n
-          |Collaboration|Organization|View|✅|✅|List nodes in a specified
-          collaboration|\n
-
-          Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            description: Collaboration id
-            required: true
-          - in: query
-            name: include
-            schema:
-              type: string
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
-            name: page
-            schema:
-              type: integer
-            description: Page number for pagination
-          - in: query
-            name: per_page
-            schema:
-              type: integer
-            description: Number of items per page
-
-        responses:
-          200:
-            description: Ok
-          404:
-            description: Collaboration not found
-          401:
-            description: Unauthorized
-
-        tags: ["Collaboration"]
-        """
-        col = db.Collaboration.get(id)
-        if not col:
-            return {"msg": f"collaboration id={id} can not be found"},\
-                HTTPStatus.NOT_FOUND
-
-        # check permission
-        if not self.r.v_glo.can():
-            auth_org = self.obtain_auth_organization()
-            if not (self.r.v_org.can() and auth_org in col.organizations):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        # paginate nodes
-        page = Pagination.from_list(col.nodes, request)
-
-        # model serialization
-        return self.response(page, node_schema)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
 
     @with_user
     def post(self, id):
         """ Add node to collaboration
         ---
         description: >-
           Add node to an existing collaboration.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
-          |Collaboration|Global|Create|❌|❌|Add node to collaboration|\n
+          |Collaboration|Global|Edit|❌|❌|Add node to collaboration|\n
+          |Collaboration|Collaboration|Edit|❌|❌|Add node to collaboration
+          that your organization is a member of|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
@@ -861,44 +781,59 @@
         tags: ["Collaboration"]
         """
         collaboration = db.Collaboration.get(id)
         if not collaboration:
             return {"msg": f"collaboration having collaboration_id={id} can "
                     "not be found"}, HTTPStatus.NOT_FOUND
 
-        if not self.r.e_glo.can():
+        if not self.r.can_for_col(P.EDIT, collaboration.id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
+        # validate request body
         data = request.get_json()
+        errors = collaboration_add_node_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
         node = db.Node.get(data['id'])
         if not node:
             return {"msg": f"node id={data['id']} not found"}, \
                 HTTPStatus.NOT_FOUND
+
         if node in collaboration.nodes:
             return {"msg": f"node id={data['id']} is already in collaboration "
                     f"id={id}"}, HTTPStatus.BAD_REQUEST
+        elif node.organization not in collaboration.organizations:
+            return {
+                "msg": f"Node id={data['id']} belongs to an organization that "
+                f"is not part of collaboration id={id}. Please add the "
+                "organization to the collaboration first"
+            }, HTTPStatus.BAD_REQUEST
 
         collaboration.nodes.append(node)
         collaboration.save()
-        return node_schema.dump(collaboration.nodes, many=True).data,\
+        return node_schema.dump(collaboration.nodes, many=True),\
             HTTPStatus.CREATED
 
     @with_user
     def delete(self, id):
         """ Remove node from collaboration
         ---
         description: >-
           Removes a single node from an existing collaboration.
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Collaboration|Global|Edit|❌|❌|Remove node from collaboration|\n
+          |Collaboration|Collaboration|Edit|❌|❌|Remove node from
+          collaboration that your organization is a member of|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
@@ -928,105 +863,24 @@
         tags: ["Collaboration"]
         """
         collaboration = db.Collaboration.get(id)
         if not collaboration:
             return {"msg": f"collaboration having collaboration_id={id} can "
                     "not be found"}, HTTPStatus.NOT_FOUND
 
-        if not self.r.e_glo.can():
+        if not self.r.can_for_col(P.EDIT, collaboration.id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
         data = request.get_json()
         node = db.Node.get(data['id'])
         if not node:
             return {"msg": f"node id={id} not found"}, HTTPStatus.NOT_FOUND
+
         if node not in collaboration.nodes:
             return {"msg": f"node id={data['id']} is not part of "
                     f"collaboration id={id}"}, HTTPStatus.BAD_REQUEST
 
         collaboration.nodes.remove(node)
         collaboration.save()
         return {"msg": f"node id={data['id']} removed from collaboration "
                 f"id={id}"}, HTTPStatus.OK
-
-
-class CollaborationTask(ServicesResources):
-    """Resource for /api/collaboration/<int:id>/task."""
-
-    def __init__(self, socketio, mail, api, permissions, config):
-        super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, 'task')
-
-    @with_user_or_node
-    def get(self, id):
-        """List tasks from collaboration
-        ---
-        description: >-
-            Returns a list of all tasks that belong to the collaboration.\n
-
-            ### Permission Table\n
-            |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-            Description|\n
-            |--|--|--|--|--|--|\n
-            |Task|Global|View|❌|❌|View tasks of collaboration|\n
-            |Task|Organization|View|✅|✅|View tasks only when your
-            organization participates in the collaboration|\n
-
-            Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            description: Collaboration id
-            required: true
-          - in: query
-            name: include
-            schema:
-              type: string
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
-            name: page
-            schema:
-              type: integer
-            description: Page number for pagination
-          - in: query
-            name: per_page
-            schema:
-              type: integer
-            description: Number of items per page
-
-        responses:
-          200:
-            description: Ok
-          401:
-            description: Unauthorized
-          404:
-            description: Collaboration not found
-
-        security:
-            - bearerAuth: []
-
-        tags: ["Collaboration"]
-
-        """
-        col = db.Collaboration.get(id)
-        if not col:
-            return {"msg": f"Collaboration id={id} can not be found"},\
-                HTTPStatus.NOT_FOUND
-
-        # obtain auth's organization id
-        auth_org = self.obtain_auth_organization()
-
-        if not self.r.v_glo.can():
-            if not (self.r.v_org.can() and auth_org in col.organizations):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        # paginate tasks
-        page = Pagination.from_list(col.tasks, request)
-
-        # model serialization
-        return self.response(page, tasks_schema)
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/common/auth_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 import datetime as dt
 import pyotp
 
 from http import HTTPStatus
 from flask import request, render_template
 from flask_mail import Mail
 
-
 from vantage6.common.globals import APPNAME, MAIN_VERSION_NAME
 from vantage6.server.globals import DEFAULT_SUPPORT_EMAIL_ADDRESS
-from vantage6.server import db
 from vantage6.server.model.user import User
 
 module_name = __name__.split('.')[-1]
 log = logging.getLogger(module_name)
 
 
 def user_login(
     config: dict, username: str, password: str, mail: Mail
-) -> tuple[dict | db.User, HTTPStatus]:
+) -> tuple[dict | User, HTTPStatus]:
     """
     Returns user a message in case of failed login attempt.
 
     config: dict
         Dictionary with configuration settings
     username: str
         Username of user to be logged in
@@ -30,24 +28,24 @@
         Password of user to be logged in
     mail: flask_mail.Mail
         An instance of the Flask mail class. Used to send email to user in case
         of too many failed login attempts.
 
     Returns
     -------
-    User or Dict:
+    :class:`~vantage6.server.model.user.User` or dict:
         User SQLAlchemy model if user is logged in, otherwise dictionary with
         error message
     HTTPStatus:
         Status code that the current request should return
     """
     log.info(f"Trying to login '{username}'")
     failed_login_msg = "Failed to login"
-    if db.User.username_exists(username):
-        user = db.User.get_by_username(username)
+    if User.username_exists(username):
+        user = User.get_by_username(username)
         password_policy = config.get("password_policy", {})
         max_failed_attempts = password_policy.get('max_failed_attempts', 5)
         inactivation_time = password_policy.get('inactivation_minutes', 15)
 
         is_blocked, min_rem = user.is_blocked(max_failed_attempts,
                                               inactivation_time)
         if is_blocked:
@@ -68,23 +66,23 @@
             user.last_login_attempt = dt.datetime.now()
             user.save()
 
     return {"msg": failed_login_msg}, HTTPStatus.UNAUTHORIZED
 
 
 def notify_user_blocked(
-    user: db.User, max_n_attempts: int, min_rem: int, mail: Mail,
+    user: User, max_n_attempts: int, min_rem: int, mail: Mail,
     config: dict
 ) -> None:
     """
     Sends an email to the user when his or her account is locked
 
     Parameters
     ----------
-    user: User
+    user: :class:`~vantage6.server.model.user.User`
         User who is temporarily blocked
     max_n_attempts: int
         Maximum number of failed login attempts before the account is locked
     min_rem: int
         Number of minutes remaining before the account is unlocked
     mail: flask_mail.Mail
         An instance of the Flask mail class. Used to send email to user in case
@@ -122,15 +120,15 @@
 
 def create_qr_uri(user: User) -> dict:
     """
     Create the URI to generate a QR code for authenticator apps
 
     Parameters
     ----------
-    user: User
+    user: :class:`~vantage6.server.model.user.User`
         User for whom two-factor authentication is to be set up
 
     Returns
     -------
     dict
         Dictionary with information on the TOTP secret required to generate
         a QR code or to enter it manually in an authenticator app
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/common/swagger_templates.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,36 +29,37 @@
                     },
                     "collaboration_id": {
                         "type": "integer",
                         "description": "Collaboration id"
                     },
                     "organizations": {
                         "type": "array",
-                        "items": {"type": "integer"},
+                        "items": {"type": "dictionary"},
                         "description": (
-                            "Organization ids in collaboration to create task "
-                            "for"
+                            "List of organizations for who the task is "
+                            "intended. For each organization, the 'id' and "
+                            "'input' fields should be specified."
                         )
                     },
-                    "database": {
-                        "type": "string",
-                        "description": "Database to use for this task"
-                    },
-                    "master": {
-                        "type": "boolean",
-                        "description": (
-                            "Whether or not this is a master task. Default "
-                            "value is False"
-                        )
+                    "databases": {
+                        "type": "array",
+                        "items": {"type": "string"},
+                        "description": "Databases to use for this task"
                     }
                 },
                 "example": {
                     "name": "human-readable-name",
                     "image": "hello-world",
-                    "collaboration_id": 1
+                    "collaboration_id": 1,
+                    "description": "human-readable-description",
+                    "organizations": [{
+                        "id": 1,
+                        "input": "input-for-organization-1"
+                    }],
+                    "databases": ["database1", "database2"],
                 },
                 "required": ["image", "collaboration_id"]
             },
             "Organization": {
                 "properties": {
                     "name": {
                         "type": "string",
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/event.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 from vantage6.server.resource import ServicesResources, with_user
 from vantage6.server import db
 from vantage6.server.permission import (
     Scope,
     Operation,
     PermissionManager
 )
+from vantage6.server.resource.common.input_schema import (
+    KillNodeTasksInputSchema,
+    KillTaskInputSchema
+)
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
     """
@@ -62,32 +66,34 @@
     Define the permissions for this resource.
 
     Parameters
     ----------
     permissions : PermissionManager
         Permission manager instance to which permissions are added
     """
-    # TODO in v4, change the operations below to 'SEND' and 'RECEIVE' as these
-    # are permissions to do stuff via socket connections
     add = permissions.appender(module_name)
 
-    add(scope=Scope.ORGANIZATION, operation=Operation.VIEW,
+    add(scope=Scope.ORGANIZATION, operation=Operation.RECEIVE,
         description="view websocket events of your organization")
-    add(scope=Scope.COLLABORATION, operation=Operation.VIEW,
+    add(scope=Scope.COLLABORATION, operation=Operation.RECEIVE,
         description="view websocket events of your collaborations")
-    add(scope=Scope.GLOBAL, operation=Operation.VIEW,
+    add(scope=Scope.GLOBAL, operation=Operation.RECEIVE,
         description="view websocket events")
-    add(scope=Scope.ORGANIZATION, operation=Operation.CREATE,
+    add(scope=Scope.ORGANIZATION, operation=Operation.SEND,
         description="send websocket events for your organization")
-    add(scope=Scope.COLLABORATION, operation=Operation.CREATE,
+    add(scope=Scope.COLLABORATION, operation=Operation.SEND,
         description="send websocket events for your collaborations")
-    add(scope=Scope.GLOBAL, operation=Operation.CREATE,
+    add(scope=Scope.GLOBAL, operation=Operation.SEND,
         description="send websocket events to all collaborations")
 
 
+kill_task_schema = KillTaskInputSchema()
+kill_node_tasks_schema = KillNodeTasksInputSchema()
+
+
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 class KillTask(ServicesResources):
     """ Provide endpoint to kill all containers executing a certain task """
 
     def __init__(self, socketio, mail, api, permissions, config):
@@ -128,35 +134,38 @@
           401:
             description: Unauthorized
           400:
             description: No task id provided
 
         tags: ["Task"]
         """
-        # obtain task id or node id from request
         body = request.get_json()
-        id_ = body.get("id")
-        if not id_:
-            return {"msg": "No task id provided!"}, HTTPStatus.BAD_REQUEST
 
+        # validate request body
+        errors = kill_task_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
+        id_ = body.get("id")
         task = db.Task.get(id_)
         if not task:
             return {"msg": f"Task id={id_} not found"}, HTTPStatus.NOT_FOUND
 
         if has_task_finished(task.status):
             return {
                 "msg": f"Task {id_} already finished with status "
                        f"'{task.status}', so cannot kill it!"
             }, HTTPStatus.BAD_REQUEST
 
         # Check permissions. If someone doesn't have global permissions, we
         # check if their organization is part of the appropriate collaboration.
-        if not self.r.c_glo.can():
+        if not self.r.s_glo.can():
             orgs = task.collaboration.organizations
-            if not (self.r.c_org.can() and g.user.organization in orgs):
+            if not (self.r.s_col.can() and g.user.organization in orgs):
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
         # call function to kill the task. This function is outside of the
         # endpoint as it is also used in other endpoints
         kill_task(task, self.socketio)
 
@@ -209,36 +218,38 @@
           401:
             description: Unauthorized
           400:
             description: No task id provided or node is not online
 
         tags: ["Task"]
         """
-        # obtain task id or node id from request
         body = request.get_json()
-        id_ = body.get("id")
-        if not id_:
-            return {"msg": "No node id provided!"}, HTTPStatus.BAD_REQUEST
+        # validate request body
+        errors = kill_node_tasks_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
+        id_ = body.get("id")
         node = db.Node.get(id_)
         if not node:
             return {"msg": f"Node id={id_} not found"}, HTTPStatus.NOT_FOUND
 
         if node.status != 'online':
             return {
                 "msg": f"Node {id_} is not online so cannot kill its tasks!"
             }, HTTPStatus.BAD_REQUEST
 
         # Check permissions. If someone doesn't have global permissions, we
         # check if their organization is part of the appropriate collaboration.
-        if not self.r.c_glo.can():
+        if not self.r.s_glo.can():
             collab_orgs = node.collaboration.organizations
             if not (
-                (self.r.c_col.can() and g.user.organization in collab_orgs) or
-                (self.r.c_org.can() and
+                (self.r.s_col.can() and g.user.organization in collab_orgs) or
+                (self.r.s_org.can() and
                     node.organization_id == g.user.organization_id)
             ):
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
         self.socketio.emit(
             'kill_containers', {
@@ -262,39 +273,39 @@
     Parameters
     ----------
     task: Task
         Task that should be killed
     socket: SocketIO
         SocketIO connection object to communicate kill instructions to node
     """
-    # Gather results and task ids of current task and child tasks
-    child_results = [r for child in task.children for r in child.results]
-    all_results = task.results + child_results
+    # Gather runs and task ids of current task and child tasks
+    child_runs = [r for child in task.children for r in child.runs]
+    all_runs = task.runs + child_runs
     child_task_ids = [child.id for child in task.children]
     all_task_ids = [task.id] + child_task_ids
 
     kill_list = [{
         'task_id': task_id,
-        'result_id': result.id,
-        'organization_id': result.organization_id
-    } for result, task_id in zip(all_results, all_task_ids)]
+        'run_id': run.id,
+        'organization_id': run.organization_id
+    } for run, task_id in zip(all_runs, all_task_ids)]
 
     # emit socket event to the node to execute the container kills
     socket.emit(
         'kill_containers', {
             'kill_list': kill_list,
             'collaboration_id': task.collaboration.id
         },
         namespace='/tasks',
         room=f"collaboration_{task.collaboration_id}",
     )
 
     # set tasks and subtasks status to killed
     def set_killed(task: db.Task):
-        for result in task.results:
-            result.status = TaskStatus.KILLED
-            result.finished_at = dt.datetime.now()
-            result.save()
+        for run in task.runs:
+            run.status = TaskStatus.KILLED
+            run.finished_at = dt.datetime.now()
+            run.save()
 
     set_killed(task)
     for subtask in task.children:
         set_killed(subtask)
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/health.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/node.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 import logging
 import uuid
 
 from http import HTTPStatus
 from flask import g, request
-from flask_restful import reqparse, Api
-
+from flask_restful import Api
 
 from vantage6.server.resource import with_user_or_node, with_user
 from vantage6.server.resource import ServicesResources
-from vantage6.server.resource.pagination import Pagination
-from vantage6.server.permission import (Scope as S,
-                                        Operation as P, PermissionManager)
+from vantage6.server.resource.common.pagination import Pagination
+from vantage6.server.permission import (
+    RuleCollection, Scope as S, Operation as P, PermissionManager
+)
 from vantage6.server import db
-from vantage6.server.resource.common._schema import NodeSchema
+from vantage6.server.resource.common.output_schema import NodeSchema
+from vantage6.server.resource.common.input_schema import NodeInputSchema
 
 
 module_name = __name__.split('.')[-1]
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
@@ -63,43 +64,52 @@
     ----------
     permissions : PermissionManager
         Permission manager instance to which permissions are added
     """
     add = permissions.appender(module_name)
 
     add(scope=S.GLOBAL, operation=P.VIEW, description="view any node")
+    add(scope=S.COLLABORATION, operation=P.VIEW,
+        description="view any node in your collaborations")
     add(scope=S.ORGANIZATION, operation=P.VIEW, assign_to_container=True,
         description="view your own node info", assign_to_node=True)
 
     add(scope=S.GLOBAL, operation=P.EDIT, description="edit any node")
+    add(scope=S.COLLABORATION, operation=P.EDIT,
+        description="edit any node in your collaborations")
     add(scope=S.ORGANIZATION, operation=P.EDIT,
         description="edit node that is part of your organization",
         assign_to_node=True)
 
     add(scope=S.GLOBAL, operation=P.CREATE,
         description="create node for any organization")
+    add(scope=S.COLLABORATION, operation=P.CREATE,
+        description="create node for any organization in your collaborations")
     add(scope=S.ORGANIZATION, operation=P.CREATE,
         description="create new node for your organization")
 
     add(scope=S.GLOBAL, operation=P.DELETE, description="delete any node")
+    add(scope=S.COLLABORATION, operation=P.DELETE,
+        description="delete any node in your collaborations")
     add(scope=S.ORGANIZATION, operation=P.DELETE,
         description="delete node that is part of your organization")
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 node_schema = NodeSchema()
+node_input_schema = NodeInputSchema()
 
 
 class NodeBase(ServicesResources):
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
 
 
 class Nodes(NodeBase):
 
     @with_user_or_node
     def get(self):
         """Returns a list of nodes
@@ -110,14 +120,16 @@
             this request, all nodes from all organizations are returned.\n
 
             ### Permission Table\n
             |Rule name|Scope|Operation|Assigned to node|Assigned to container|
             Description|\n
             |--|--|--|--|--|--|\n
             |Node|Global|View|❌|❌|View any node information|\n
+            |Node|Collaboration|View|❌|❌|View any node information for nodes
+            in your collaborations|\n
             |Node|Organization|View|✅|✅|View node information for nodes that
             belong to your organization|\n
 
             Accessible to users.
 
         parameters:
           - in: query
@@ -156,180 +168,219 @@
             description: Show only nodes seen since this date
           - in: query
             name: last_seen_till
             schema:
               type: date (yyyy-mm-dd)
             description: Show only nodes last seen before this date
           - in: query
-            name: include
-            schema:
-              type: string
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
             name: page
             schema:
               type: integer
-            description: Page number for pagination
+            description: Page number for pagination (default=1)
           - in: query
             name: per_page
             schema:
               type: integer
-            description: Number of items per page
+            description: Number of items per page (default=10)
+          - in: query
+            name: sort
+            schema:
+              type: string
+            description: >-
+              Sort by one or more fields, separated by a comma. Use a minus
+              sign (-) in front of the field to sort in descending order.
 
         responses:
             200:
                 description: Ok
             401:
                 description: Unauthorized
+            400:
+                description: Improper values for pagination or sorting
+                  parameters
 
         security:
             - bearerAuth: []
 
         tags: ["Node"]
         """
         q = g.session.query(db.Node)
         auth_org_id = self.obtain_organization_id()
         args = request.args
 
-        for param in ['organization_id', 'collaboration_id', 'status', 'ip']:
+        if 'organization_id' in args:
+            if not self.r.can_for_org(P.VIEW, int(args['organization_id'])):
+                return {
+                    'msg': 'You lack the permission view nodes from the '
+                    f'organization with id {args["organization_id"]}!'
+                }, HTTPStatus.UNAUTHORIZED
+            q = q.filter(db.Node.organization_id == args['organization_id'])
+
+        if 'collaboration_id' in args:
+            if not self.r.can_for_col(P.VIEW, int(args['collaboration_id'])):
+                return {
+                    'msg': 'You lack the permission view nodes from the '
+                    f'collaboration with id {args["collaboration_id"]}!'
+                }, HTTPStatus.UNAUTHORIZED
+            q = q.filter(db.Node.collaboration_id == args['collaboration_id'])
+
+        for param in ['status', 'ip']:
             if param in args:
                 q = q.filter(getattr(db.Node, param) == args[param])
         if 'name' in args:
             q = q.filter(db.Node.name.like(args['name']))
 
         if 'last_seen_till' in args:
             q = q.filter(db.Node.last_seen <= args['last_seen_till'])
         if 'last_seen_from' in args:
             q = q.filter(db.Node.last_seen >= args['last_seen_from'])
 
         if not self.r.v_glo.can():
-            if self.r.v_org.can():
+            if self.r.v_col.can():
+                q = q.filter(db.Node.collaboration_id.in_(
+                    [col.id for col in self.obtain_auth_collaborations()]
+                ))
+            elif self.r.v_org.can():
                 # only the results of the user's organization are returned
                 q = q.filter(db.Node.organization_id == auth_org_id)
             else:
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
         # paginate results
-        page = Pagination.from_query(q, request)
+        try:
+            page = Pagination.from_query(q, request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         # model serialization
         return self.response(page, node_schema)
 
     # TODO the example in swagger docs for this doesn't include
     # organization_id. Find out why
     @with_user
     def post(self):
         """Create node
         ---
         description: >-
-          Creates a new node-account belonging to a specific collaboration
-          which is specified in the POST body.\n
+          Creates a new node-account belonging to a specific organization and
+          collaboration which is specified in the POST body.\n
           The organization of the user needs to be within the collaboration.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Node|Global|Create|❌|❌|Create a new node account belonging to a
-          specific collaboration|\n
+          specific organization in any collaboration|\n
+          |Node|Collaboration|Create|❌|❌|Create a new node account belonging
+          to a specific organization in your collaborations|\n
           |Node|Organization|Create|❌|❌|Create a new node account belonging
-          to a specific organization which is also part of the collaboration|\n
+          to your organization|\n
 
           Accessible to users.
 
         requestBody:
           content:
             application/json:
               schema:
                 properties:
                   collaboration_id:
                     type: integer
                     description: Collaboration id
                   organization_id:
                     type: integer
-                    description: Organization id
+                    description: Organization id. If not provided, this
+                      defaults to the organization of the user creating the
+                      node.
                   name:
-                    type: str
-                    description: Human-readable name, if not profided a name
-                      is generated
+                    type: string
+                    description: Human-readable name. If not provided a name
+                      is generated based on organization and collaboration
+                      name.
 
         responses:
           201:
             description: New node-account created
           404:
             description: Collaboration specified by id does not exists
           400:
-            description: Organization is not part of the collaboration or it
-              already has a node for this collaboration
+            description: Organization is not part of the collaboration, or it
+              already has a node for this collaboration, or the node name is
+              not unique.
           401:
             description: Unauthorized
 
         security:
           - bearerAuth: []
 
         tags: ["Node"]
         """
-        parser = reqparse.RequestParser()
-        parser.add_argument("collaboration_id", type=int, required=True,
-                            help="This field cannot be left blank!")
-        parser.add_argument("organization_id", type=int, required=False)
-        parser.add_argument("name", type=str, required=False)
-        data = parser.parse_args()
-
-        collaboration = db.Collaboration.get(data["collaboration_id"])
+        data = request.get_json()
+        # validate request body
+        errors = node_input_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         # check that the collaboration exists
+        collaboration = db.Collaboration.get(data["collaboration_id"])
         if not collaboration:
             return {"msg": f"collaboration id={data['collaboration_id']} "
                     "does not exist"}, HTTPStatus.NOT_FOUND  # 404
 
+        org_id = data["organization_id"] \
+            if data.get("organization_id") is not None \
+            else g.user.organization_id
+        organization = db.Organization.get(org_id)
+
+        # check that the organization exists
+        if not organization:
+            return {"msg": f"organization id={org_id} does not exist"}, \
+                HTTPStatus.NOT_FOUND
+
         # check permissions
-        org_id = data["organization_id"]
-        user_org_id = g.user.organization.id
-        if not self.r.c_glo.can():
-            own = not org_id or org_id == user_org_id
-            if not (self.r.c_org.can() and own):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-            else:
-                org_id = g.user.organization.id
-        organization = db.Organization.get(org_id or user_org_id)
+        if not self.r.can_for_org(P.CREATE, org_id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
 
         # we need to check that the organization belongs to the
         # collaboration
         if not (organization in collaboration.organizations):
             return {'msg': f'The organization id={org_id} is not part of '
                     f'collabotation id={collaboration.id}. Add it first!'}, \
                         HTTPStatus.BAD_REQUEST
 
         # verify that this node does not already exist
         if db.Node.exists(organization.id, collaboration.id):
             return {'msg': f'Organization id={organization.id} already has a '
                     f'node for collaboration id={collaboration.id}'}, \
                         HTTPStatus.BAD_REQUEST
 
-        # if no name is profided, generate one
-        name = data['name'] if data['name'] else \
+        # if no name is provided, generate one
+        name = data['name'] if 'name' in data else \
             f"{organization.name} - {collaboration.name} Node"
+        if db.Node.exists("name", name):
+            return {
+                "msg": f"Node name '{name}' already exists!"
+            }, HTTPStatus.BAD_REQUEST
 
         # Ok we're good to go!
         api_key = str(uuid.uuid4())
         node = db.Node(
             name=name,
             collaboration=collaboration,
             organization=organization,
             api_key=api_key
         )
         node.save()
 
         # Return the node information to the user. Manually return the api_key
         # to the user as the hashed key is not returned
-        node_json = node_schema.dump(node).data
+        node_json = node_schema.dump(node)
         node_json['api_key'] = api_key
         return node_json, HTTPStatus.CREATED  # 201
 
 
 class Node(NodeBase):
 
     @with_user_or_node
@@ -342,22 +393,24 @@
           permission.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Node|Global|View|❌|❌|View any node information|\n
+          |Node|Collaboration|View|❌|❌|View any node information for nodes
+          within your collaborations|\n
           |Node|Organization|View|✅|✅|View node information for nodes that
           belong to your organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
-            name: id
+            name: id_
             schema:
               type: integer
               minimum: 1
             description: Node id
             required: tr
 
         responses:
@@ -371,27 +424,23 @@
         security:
           - bearerAuth: []
 
         tags: ["Node"]
         """
         node = db.Node.get(id)
         if not node:
-            return {'msg': f'Node id={id} is not found!'}, HTTPStatus.NOT_FOUND
-
-        # obtain authenticated model
-        auth = self.obtain_auth()
+            return {'msg': f'Node id={id} is not found!'}, \
+                HTTPStatus.NOT_FOUND
 
         # check permissions
-        if not self.r.v_glo.can():
-            same_org = auth.organization.id == node.organization.id
-            if not (self.r.v_org.can() and same_org):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
+        if not self.r.can_for_org(P.VIEW, node.organization_id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
 
-        return node_schema.dump(node, many=False).data, HTTPStatus.OK
+        return node_schema.dump(node, many=False), HTTPStatus.OK
 
     @with_user
     def delete(self, id):
         """
         Delete node
         ---
         description: >-
@@ -399,22 +448,24 @@
           organization of the node can delete it.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Node|Global|Delete|❌|❌|Delete a node|\n
+          |Node|Collaboration|Delete|❌|❌|Delete a node that belongs to
+          one of the organizations in your collaborations|\n
           |Node|Organization|Delete|❌|❌|Delete a node that belongs to your
           organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
-            name: id
+            name: id_
             schema:
               type: integer
               minimum: 1
             description: Node id
             required: tr
 
         responses:
@@ -430,19 +481,17 @@
 
         tags: ["Node"]
         """
         node = db.Node.get(id)
         if not node:
             return {"msg": f"Node id={id} not found"}, HTTPStatus.NOT_FOUND
 
-        if not self.r.d_glo.can():
-            own = node.organization == g.user.organization
-            if not (self.r.d_org.can() and own):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
+        if not self.r.can_for_org(P.DELETE, node.organization_id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
 
         node.delete()
         return {"msg": f"Successfully deleted node id={id}"}, HTTPStatus.OK
 
     @with_user_or_node
     def patch(self, id):
         """Update node
@@ -453,22 +502,24 @@
           If the node does not exists it is created as a new node.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Node|Global|Edit|❌|❌|Update a node specified by id|\n
+          |Node|Collaboration|Edit|❌|❌|Update a node specified by id which
+          is part of one of your collaborations|\n
           |Node|Organization|Edit|❌|❌|Update a node specified by id which is
           part of your organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
-            name: id
+            name: id_
             schema:
               type: integer
             description: Node id
             required: tr
 
         requestBody:
           content:
@@ -483,62 +534,72 @@
                     description: Organization id
                   name:
                     type: string
                     description: Node name
                   ip:
                     type: string
                     description: The node's VPN IP address
+                  clear_ip:
+                    type: boolean
+                    description: Clear the node's VPN IP address
 
         responses:
           200:
             description: Ok, node is updated
           400:
             description: A node already exist for this organization in this
-              collaboration
+              collaboration, or a node already exists with this name
           401:
             description: Unauthorized
           404:
             description: Organization or collaboration not found
 
         security:
           - bearerAuth: []
 
         tags: ["Node"]
         """
+        data = request.get_json()
+        # validate request body
+        errors = node_input_schema.validate(data, partial=True)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
         node = db.Node.get(id)
         if not node:
             return {'msg': f'Node id={id} not found!'}, HTTPStatus.NOT_FOUND
 
-        auth = g.user or g.node
-
-        if not self.r.e_glo.can():
-            own = auth.organization.id == node.organization.id
-            if not (self.r.e_org.can() and own):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        data = request.get_json()
+        if not self.r.can_for_org(P.EDIT, node.organization_id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
 
         # update fields
         if 'name' in data:
-            node.name = data['name']
+            name = data['name']
+            if node.name != name and db.Node.exists("name", name):
+                return {
+                    "msg": f"Node name '{name}' already exists!"
+                }, HTTPStatus.BAD_REQUEST
+            node.name = name
 
         # organization goes before collaboration (!)
         org_id = data.get('organization_id')
         updated_org = org_id and org_id != node.organization.id
         if updated_org:
             if not self.r.e_glo.can():
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
             organization = db.Organization.get(data['organization_id'])
             if not organization:
                 return {'msg': f'Organization id={data["organization_id"]} '
                         'not found!'}, HTTPStatus.NOT_FOUND
             node.organization = organization
 
+        auth = self.obtain_auth()
         col_id = data.get('collaboration_id')
         updated_col = col_id and col_id != node.collaboration.id
         if updated_col:
             collaboration = db.Collaboration.get(data['collaboration_id'])
             if not collaboration:
                 return {'msg': f'collaboration id={data["collaboration_id"]}'
                         'not found!'}, HTTPStatus.NOT_FOUND
@@ -560,10 +621,12 @@
                         f'{node.collaboration.id} already exists!'}, \
                             HTTPStatus.BAD_REQUEST
 
         # update node IP address if it is given
         ip = data.get('ip')
         if ip:
             node.ip = ip
+        elif data.get('clear_ip'):
+            node.ip = None
 
         node.save()
-        return node_schema.dump(node).data, HTTPStatus.OK
+        return node_schema.dump(node), HTTPStatus.OK
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/organization.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 from flask import request, g
 from flask_restful import Api
 from http import HTTPStatus
 
 from vantage6.common import logger_name
 from vantage6.server import db
-from vantage6.server.resource.pagination import Pagination
+from vantage6.server.resource.common.pagination import Pagination
 from vantage6.server.permission import (
     Scope as S,
     Operation as P,
-    PermissionManager
+    PermissionManager,
+    RuleCollection
 )
-from vantage6.server.resource import (
-    with_user_or_node, only_for, with_user, ServicesResources
+from vantage6.server.resource.common.input_schema import (
+    OrganizationInputSchema
 )
-from vantage6.server.resource.common._schema import (
-    OrganizationSchema,
-    CollaborationSchema,
-    NodeSchema
+from vantage6.server.resource import (
+    only_for, with_user, ServicesResources
 )
+from vantage6.server.resource.common.output_schema import OrganizationSchema
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
@@ -53,28 +53,14 @@
     api.add_resource(
         Organization,
         path + '/<int:id>',
         endpoint='organization_with_id',
         methods=('GET', 'PATCH'),
         resource_class_kwargs=services
     )
-    api.add_resource(
-        OrganizationCollaboration,
-        path + '/<int:id>/collaboration',
-        endpoint='organization_collaboration',
-        methods=('GET',),
-        resource_class_kwargs=services
-    )
-    api.add_resource(
-        OrganizationNode,
-        path + '/<int:id>/node',
-        endpoint='organization_node',
-        methods=('GET',),
-        resource_class_kwargs=services
-    )
 
 
 # -----------------------------------------------------------------------------
 # Permissions
 # -----------------------------------------------------------------------------
 def permissions(permissions: PermissionManager) -> None:
     """
@@ -95,29 +81,32 @@
     add(scope=S.COLLABORATION, operation=P.VIEW,
         description='view collaborating organizations',
         assign_to_container=True, assign_to_node=True)
     add(scope=S.GLOBAL, operation=P.EDIT,
         description="edit any organization")
     add(scope=S.ORGANIZATION, operation=P.EDIT,
         description="edit your own organization info", assign_to_node=True)
+    add(scope=S.COLLABORATION, operation=P.EDIT,
+        description='edit collaborating organizations')
     add(scope=S.GLOBAL, operation=P.CREATE,
         description="create a new organization")
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 org_schema = OrganizationSchema()
+org_input_schema = OrganizationInputSchema()
 
 
 class OrganizationBase(ServicesResources):
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
 
 
 class Organizations(OrganizationBase):
 
     @only_for(("user", "node", "container"))
     def get(self):
         """ Returns a list organizations
@@ -154,35 +143,38 @@
             description: Country
           - in: query
             name: collaboration_id
             schema:
               type: integer
             description: Collaboration id
           - in: query
-            name: include
-            schema:
-              type: string (can be multiple)
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
             name: page
             schema:
               type: integer
-            description: Page number for pagination
+            description: Page number for pagination (default=1)
           - in: query
             name: per_page
             schema:
               type: integer
-            description: Number of items per page
+            description: Number of items per page (default=10)
+          - in: query
+            name: sort
+            schema:
+              type: string
+            description: >-
+              Sort by one or more fields, separated by a comma. Use a minus
+              sign (-) in front of the field to sort in descending order.
 
         responses:
           200:
             description: Ok
           401:
             description: Unauthorized
+          400:
+            description: Improper values for pagination or sorting parameters
 
         security:
           - bearerAuth: []
 
         tags: ["Organization"]
         """
 
@@ -196,43 +188,52 @@
 
         # filter by a field of this endpoint
         if 'name' in args:
             q = q.filter(db.Organization.name.like(args['name']))
         if 'country' in args:
             q = q.filter(db.Organization.country == args['country'])
         if 'collaboration_id' in args:
+            if not self.r.can_for_col(P.VIEW, int(args['collaboration_id'])):
+                return {
+                    'msg': 'You lack the permission to get all organizations '
+                    'in your collaboration!'
+                }, HTTPStatus.UNAUTHORIZED
             q = q.join(db.Member).join(db.Collaboration)\
                  .filter(db.Collaboration.id == args['collaboration_id'])
 
         # filter the list of organizations based on the scope
         if self.r.v_glo.can():
             pass  # don't apply filters
         elif self.r.v_col.can():
             # obtain collaborations your organization participates in
             collabs = g.session.query(db.Collaboration).filter(
                 db.Collaboration.organizations.any(id=auth_org.id)
             ).all()
             g.session.commit()
 
-            # list comprehension fetish, and add own organization in case
-            # this organization does not participate in any collaborations yet
+            # filter orgs in own collaborations, and add own organization in
+            # case this organization does not participate in any collaborations
+            # yet
             org_ids = [o.id for col in collabs for o in col.organizations]
             org_ids = list(set(org_ids + [auth_org.id]))
 
             # select only the organizations in the collaborations
             q = q.filter(db.Organization.id.in_(org_ids))
 
         elif self.r.v_org.can():
             q = q.filter(db.Organization.id == auth_org.id)
         else:
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
         # paginate the results
-        page = Pagination.from_query(query=q, request=request)
+        try:
+            page = Pagination.from_query(query=q, request=request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         # serialization of DB model
         return self.response(page, org_schema)
 
     @with_user
     def post(self):
         """Create new organization
@@ -255,38 +256,52 @@
                 $ref: '#/components/schemas/Organization'
 
         responses:
           201:
             description: Ok
           401:
             description: Unauthorized
+          400:
+            description: Organization with that name already exists
 
         security:
           - bearerAuth: []
 
         tags: ["Organization"]
         """
 
         if not self.r.c_glo.can():
             return {'msg': 'You lack the permissions to do that!'},\
                 HTTPStatus.UNAUTHORIZED
 
+        # validate request body
         data = request.get_json()
+        errors = org_input_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
+        name = data.get('name')
+        if db.Organization.exists("name", name):
+            return {
+                "msg": f"Organization with name '{name}' already exists!"
+            }, HTTPStatus.BAD_REQUEST
+
         organization = db.Organization(
-            name=data.get('name', ''),
+            name=name,
             address1=data.get('address1', ''),
             address2=data.get('address2' ''),
             zipcode=data.get('zipcode', ''),
             country=data.get('country', ''),
             public_key=data.get('public_key', ''),
             domain=data.get('domain', '')
         )
         organization.save()
 
-        return org_schema.dump(organization, many=False).data, \
+        return org_schema.dump(organization, many=False), \
             HTTPStatus.CREATED
 
 
 class Organization(OrganizationBase):
 
     @only_for(("user", "node", "container"))
     def get(self, id):
@@ -325,58 +340,42 @@
 
         security:
           - bearerAuth: []
 
         tags: ["Organization"]
         """
 
-        # obtain organization of authenticated
-        auth_org = self.obtain_auth_organization()
-
         # retrieve requested organization
         req_org = db.Organization.get(id)
         if not req_org:
             return {'msg': f'Organization id={id} not found!'}, \
                 HTTPStatus.NOT_FOUND
 
-        accepted = False
         # Check if auth has enough permissions
-        if self.r.v_glo.can():
-            accepted = True
-        elif self.r.v_col.can():
-            # check if the organization is whithin a collaboration
-            for col in auth_org.collaborations:
-                if req_org in col.organizations:
-                    accepted = True
-            # or that the organization is auths org
-            if req_org == auth_org:
-                accepted = True
-        elif self.r.v_org.can():
-            accepted = auth_org == req_org
-
-        if accepted:
-            return org_schema.dump(req_org, many=False).data, \
-                HTTPStatus.OK
-        else:
+        if not self.r.can_for_org(P.VIEW, id):
             return {'msg': 'You do not have permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
+        return org_schema.dump(req_org, many=False), HTTPStatus.OK
+
     @only_for(("user", "node"))
     def patch(self, id):
         """Update organization
         ---
         description: >-
           Updates the organization with the specified id.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Organization|Global|Edit|❌|❌|Update an organization with
           specified id|\n
+          |Organization|Collaboration|Edit|❌|❌|Update an organization within
+          the collaboration the user is part of|\n
           |Organization|Organization|Edit|❌|❌|Update the organization that
           the user is part of|\n
 
           Accessible to users.
 
         parameters:
           - in: path
@@ -395,165 +394,48 @@
         responses:
           200:
             description: Ok
           404:
             description: Organization with specified id is not found
           401:
             description: Unauthorized
+          400:
+            description: Organization with that name already exists
 
         security:
           - bearerAuth: []
 
         tags: ["Organization"]
         """
+        # validate request body
+        data = request.get_json()
+        errors = org_input_schema.validate(data, partial=True)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         organization = db.Organization.get(id)
         if not organization:
             return {"msg": f"Organization with id={id} not found"}, \
                 HTTPStatus.NOT_FOUND
 
-        if not (
-            self.r.e_glo.can() or
-            (self.r.e_org.can() and g.user and id == g.user.organization.id) or
-            (self.r.e_org.can() and g.node and id == g.node.organization.id)
-        ):
+        if not self.r.can_for_org(P.EDIT, id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
-        data = request.get_json()
-        fields = ["name", "address1", "address2", "zipcode", "country",
+        name = data.get('name', None)
+        if name:
+            if organization.name != name and \
+                    db.Organization.exists("name", name):
+                return {
+                    "msg": f"Organization with name '{name}' already exists!"
+                }, HTTPStatus.BAD_REQUEST
+            organization.name = name
+
+        fields = ["address1", "address2", "zipcode", "country",
                   "public_key", "domain"]
         for field in fields:
             if field in data and data[field] is not None:
                 setattr(organization, field, data[field])
 
         organization.save()
-        return org_schema.dump(organization, many=False).data, \
-            HTTPStatus.OK
-
-
-class OrganizationCollaboration(ServicesResources):
-    """Collaborations for a specific organization."""
-
-    col_schema = CollaborationSchema()
-
-    @only_for(("user", "node"))
-    def get(self, id):
-        """Get collaborations from organization
-        ---
-        description: >-
-          Returns a list of collaborations in which the organization is a
-          participant of.\n
-
-          ### Permission Table\n
-          |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-          Description|\n
-          |--|--|--|--|--|--|\n
-          |Collaboration|Global|View|❌|❌|View all collaborations|\n
-          |Collaboration|Organization|View|✅|✅|View a list of collaborations
-          that the organization is a part of|\n
-
-          Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            description: Organization id
-            required: true
-
-        responses:
-          200:
-            description: Ok
-          404:
-            description: Organization not found
-          401:
-            description: Unauthorized
-
-        security:
-          - bearerAuth: []
-
-        tags: ["Organization"]
-        """
-        organization = db.Organization.get(id)
-        if not organization:
-            return {"msg": f"organization id={id} not found"}, \
-                HTTPStatus.NOT_FOUND
-
-        if g.node:
-            auth_org_id = g.node.organization.id
-        else:  # g.user:
-            auth_org_id = g.user.organization.id
-
-        if not self.permissions.collaboration.v_glo.can():
-            if not (self.permissions.collaboration.v_org.can() and
-                    auth_org_id == id):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        return self.col_schema.dump(
-            organization.collaborations,
-            many=True
-        ).data, HTTPStatus.OK
-
-
-class OrganizationNode(ServicesResources):
-    """Resource for /api/organization/<int:id>/node."""
-
-    nod_schema = NodeSchema()
-
-    @with_user_or_node
-    def get(self, id):
-        """Return a list of nodes.
-        ---
-        description: >-
-          Returns a list of nodes which are from the organization.\n
-
-          ### Permission Table\n
-          |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-          Description|\n
-          |--|--|--|--|--|--|\n
-          |Organization|Global|View|❌|❌|View any node|\n
-          |Organization|Organization|View|✅|✅|View a list of nodes that
-          belong to your organization|\n
-
-          Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            description: Organization id
-            required: true
-
-        responses:
-          200:
-            description: Ok
-          404:
-            description: Organization not found
-          401:
-            description: Unauthorized
-
-        security:
-          - bearerAuth: []
-
-        tags: ["Organization"]
-        """
-        organization = db.Organization.get(id)
-        if not organization:
-            return {"msg": f"organization id={id} not found"}, \
-                HTTPStatus.NOT_FOUND
-
-        if g.user:
-            auth_org_id = g.user.organization.id
-        else:  # g.node
-            auth_org_id = g.node.organization.id
-
-        if not self.permissions.node.v_glo.can():
-            if not (self.permissions.node.v_org.can() and id == auth_org_id):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        return self.nod_schema.dump(organization.nodes, many=True).data, \
-            HTTPStatus.OK
+        return org_schema.dump(organization, many=False), HTTPStatus.OK
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/port.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/port.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # -*- coding: utf-8 -*-
 import logging
 
 from flask import g, request
 from flask_restful import Api
 from http import HTTPStatus
-from sqlalchemy import desc
 
 from vantage6.common import logger_name
 from vantage6.server.permission import (
     PermissionManager,
     Scope as S,
     Operation as P
 )
 from vantage6.server.resource import (
     with_node,
-    only_for,
     ServicesResources
 )
 from vantage6.server import db
-from vantage6.server.resource.pagination import Pagination
-from vantage6.server.resource.common._schema import PortSchema
+from vantage6.server.resource.common.output_schema import PortSchema
+from vantage6.server.resource.common.input_schema import PortInputSchema
 from vantage6.server.model import (
-    Result,
+    Run,
     AlgorithmPort,
-    Collaboration,
-    Task
 )
 from vantage6.server.resource import with_container
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
@@ -48,35 +44,29 @@
     path = "/".join([api_base, module_name])
     log.info(f'Setting up "{path}" and subdirectories')
 
     api.add_resource(
         Ports,
         path,
         endpoint='port_without_id',
-        methods=('GET', 'POST', 'DELETE'),
-        resource_class_kwargs=services
-    )
-    api.add_resource(
-        Port,
-        path + '/<int:id>',
-        endpoint='port_with_id',
-        methods=('GET',),
+        methods=('POST', 'DELETE'),
         resource_class_kwargs=services
     )
     api.add_resource(
         VPNAddress,
         api_base + '/vpn/algorithm/addresses',
         endpoint='vpn_address',
         methods=('GET',),
         resource_class_kwargs=services
     )
 
 
 # Schemas
 port_schema = PortSchema()
+port_input_schema = PortInputSchema()
 
 
 # -----------------------------------------------------------------------------
 # Permissions
 # -----------------------------------------------------------------------------
 def permissions(permissions: PermissionManager) -> None:
     """
@@ -101,111 +91,14 @@
 class PortBase(ServicesResources):
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
         self.r = getattr(self.permissions, module_name)
 
 
 class Ports(PortBase):
-
-    @only_for(('node', 'user', 'container'))
-    def get(self):
-        """ Returns a list of ports
-        ---
-
-        description: >-
-          Returns a list of all ports you are allowed to see.\n
-
-          ### Permission Table\n
-          |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-          Description|\n
-          |--|--|--|--|--|--|\n
-          |Port|Global|View|❌|❌|View any result|\n
-          |Port|Organization|View|✅|✅|View the ports of your
-          organizations collaborations|\n
-
-          Accessible to users.
-
-        parameters:
-          - in: query
-            name: task_id
-            schema:
-              type: integer
-            description: Task id
-          - in: query
-            name: result_id
-            schema:
-              type: integer
-            description: Result id
-          - in: query
-            name: run_id
-            schema:
-              type: integer
-            description: Run id
-          - in: query
-            name: include
-            schema:
-              type: string (can be multiple)
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
-            name: page
-            schema:
-              type: integer
-            description: Page number for pagination
-          - in: query
-            name: per_page
-            schema:
-              type: integer
-            description: Number of items per page
-
-        responses:
-          200:
-            description: Ok
-          401:
-            description: Unauthorized
-
-        security:
-        - bearerAuth: []
-
-        tags: ["VPN"]
-        """
-        auth_org = self.obtain_auth_organization()
-        args = request.args
-
-        q = g.session.query(AlgorithmPort)
-
-        # relation filters
-        if 'result_id' in args:
-            q = q.filter(AlgorithmPort.result_id == args['result_id'])
-        if 'task_id' in args:
-            q = q.join(Result).filter(Result.task_id == args['task_id'])
-        if 'run_id' in args:
-            # check if Result was already joined in 'task_id' arg
-            if Result not in [joined.class_ for joined in q._join_entities]:
-                q = q.join(Result)
-            q = q.join(Task).filter(Task.run_id == args['run_id'])
-
-        # filter based on permissions
-        if not self.r.v_glo.can():
-            if self.r.v_org.can():
-                col_ids = [col.id for col in auth_org.collaborations]
-                q = q.filter(Collaboration.id.in_(col_ids))
-            else:
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        # query the DB and paginate
-        q = q.order_by(desc(AlgorithmPort.id))
-        page = Pagination.from_query(query=q, request=request)
-
-        # serialization of the models
-        s = port_schema
-
-        return self.response(page, s)
-
     @with_node
     def post(self):
         """Create a list of port description
         ---
         description: >-
           Creates a description of a port that is available for VPN
           communication for a certain algorithm. Only the node on which the
@@ -219,17 +112,17 @@
             application/json:
               schema:
                 properties:
                   port:
                     type: integer
                     description: Port number that receives container's VPN
                       traffic
-                  result_id:
+                  run_id:
                     type: integer
-                    description: Algorithm's result_id
+                    description: Algorithm's run_id
                   label:
                     type: string
                     description: Label for port specified in algorithm
                       docker image
 
         responses:
           201:
@@ -239,155 +132,94 @@
 
         security:
             - bearerAuth: []
 
         tags: ["VPN"]
         """
         data = request.get_json()
+        # validate request body
+        errors = port_input_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         # The only entity that is allowed to algorithm ports is the node where
         # those algorithms are running.
-        result_id = data.get('result_id', '')
-        linked_result = g.session.query(Result)\
-                         .filter(Result.id == result_id)\
-                         .one()
-        if g.node.id != linked_result.node.id:
+        run_id = data['run_id']
+        linked_run = g.session.query.query(Run).filter(Run.id == run_id).one()
+        if g.node.id != linked_run.node.id:
             return {'msg': 'You lack the permissions to do that!'},\
                 HTTPStatus.UNAUTHORIZED
 
         port = AlgorithmPort(
-            port=data.get('port', ''),
-            result_id=result_id,
+            port=data['port'],
+            run_id=run_id,
             label=data.get('label' ''),
         )
         port.save()
 
-        return port_schema.dump(port, many=False).data, HTTPStatus.CREATED
+        return port_schema.dump(port, many=False), HTTPStatus.CREATED
 
     @with_node
     def delete(self):
-        # FIXME should we have swagger docs if only accessible for node? Also
-        # same case for post request
-        """ Delete ports by result_id
+        """ Delete ports by run_id
         ---
         description: >-
           Deletes descriptions of a port that is available for VPN
           communication for a certain algorithm. The ports are deleted based
-          on result_id. Only the node on which the algorithm is running is
+          on run_id. Only the node on which the algorithm is running is
           allowed to delete this. This happens on task completion.\n
 
           This endpoint is not accessible for users, but only for
           authenticated nodes.
 
         parameters:
           - in: path
-            name: result_id
+            name: run_id
             schema:
               type: integer
             minimum: 1
-            description: Result id for which ports must be deleted
+            description: Run id for which ports must be deleted
             required: true
 
         responses:
           200:
             description: Ok
           400:
-            description: Result id was not defined
+            description: Run id was not defined
           401:
             description: Unauthorized
 
         security:
           - bearerAuth: []
 
         tags: ["VPN"]
         """
         args = request.args
-        if 'result_id' not in args:
-            return {'msg': 'The result_id argument is required!'}, \
+        if 'run_id' not in args:
+            return {'msg': 'The run_id argument is required!'}, \
               HTTPStatus.BAD_REQUEST
 
         # The only entity that is allowed to delete algorithm ports is the node
         # where those algorithms are running.
-        result_id = args['result_id']
-        linked_result = g.session.query(Result)\
-                         .filter(Result.id == result_id)\
-                         .one()
-        if g.node.id != linked_result.node.id:
+        run_id = args['run_id']
+        linked_run = g.session.query(Run).filter(Run.id == run_id).one()
+        if g.node.id != linked_run.node.id:
             return {'msg': 'You lack the permissions to do that!'},\
                 HTTPStatus.UNAUTHORIZED
 
         # all checks passed: delete the port entries
         g.session.query(AlgorithmPort).filter(
-            AlgorithmPort.result_id == result_id
+            AlgorithmPort.run_id == run_id
         ).delete()
         g.session.commit()
 
         return {"msg": "Ports removed from the database."}, HTTPStatus.OK
 
 
-class Port(PortBase):
-    """Resource for /api/port"""
-
-    @only_for(('node', 'user', 'container'))
-    def get(self, id):
-        """ Get a single port
-        ---
-        description: >-
-            Returns a port specified by an id.\n
-
-            ### Permission Table\n
-            |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-            Description|\n
-            |--|--|--|--|--|--|\n
-            |Port|Global|View|❌|❌|View any port|\n
-            |Port|Organization|View|✅|✅|View the ports of your
-            organization's collaborations|\n
-
-            Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            minimum: 1
-            description: Port id
-            required: true
-
-        responses:
-          200:
-              description: Ok
-          401:
-              description: Unauthorized
-          404:
-              description: Port id not found
-
-        security:
-          - bearerAuth: []
-
-        tags: ["VPN"]
-        """
-        auth_org = self.obtain_auth_organization()
-
-        port = AlgorithmPort.get(id)
-        if not port:
-            return {'msg': f'Port id={id} not found!'}, HTTPStatus.NOT_FOUND
-
-        # check permissions
-        if not self.r.v_glo.can():
-            if not self.r.v_org.can() and auth_org == auth_org.id:
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        # serialize
-        s = port_schema
-
-        return s.dump(port, many=False).data, HTTPStatus.OK
-
-
 class VPNAddress(ServicesResources):
 
     @with_container
     def get(self):
         """
         Get a list of the addresses (IP + port) and labels of algorithm
         containers in the same task as the authenticating container.
@@ -496,16 +328,16 @@
                 if only_parent:
                     task_ids = [parent.id]
                 else:
                     task_ids.append(parent.id)
 
         # get all ports for the tasks requested
         q = g.session.query(AlgorithmPort)\
-                     .join(Result)\
-                     .filter(Result.task_id.in_(task_ids))\
+                     .join(Run)\
+                     .filter(Run.task_id.in_(task_ids))\
 
         # filter by label if requested
         filter_label = request.args.get('label')
         if filter_label:
             q = q.filter(AlgorithmPort.label == filter_label)
 
         ports = q.all()
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/recover.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/recover.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 from vantage6.server.globals import (
     DEFAULT_EMAILED_TOKEN_VALIDITY_MINUTES, DEFAULT_SUPPORT_EMAIL_ADDRESS
 )
 from vantage6.server.resource import ServicesResources, with_user
 from vantage6.server.resource.common.auth_helper import (
     create_qr_uri, user_login
 )
+from vantage6.server.resource.common.input_schema import (
+    ChangePasswordInputSchema,
+    RecoverPasswordInputSchema,
+    ResetPasswordInputSchema,
+    Recover2FAInputSchema,
+    Reset2FAInputSchema,
+    ResetAPIKeyInputSchema
+)
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
     """
@@ -89,14 +97,22 @@
         path+'/node',
         endpoint="reset_api_key",
         methods=('POST',),
         resource_class_kwargs=services
     )
 
 
+recover_pw_schema = RecoverPasswordInputSchema()
+reset_pw_schema = ResetPasswordInputSchema()
+recover_2fa_schema = Recover2FAInputSchema()
+reset_2fa_schema = Reset2FAInputSchema()
+reset_api_key_schema = ResetAPIKeyInputSchema()
+change_pw_schema = ChangePasswordInputSchema()
+
+
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 class ResetPassword(ServicesResources):
     """User can use recover token to reset their password."""
 
     def post(self):
@@ -121,23 +137,24 @@
           200:
             description: Ok
           400:
             description: Password or recovery token is missing or invalid
 
         tags: ["Account recovery"]
         """
-        # retrieve user based on email or username
         body = request.get_json()
+        # validate request body
+        errors = reset_pw_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
         reset_token = body.get("reset_token")
         password = body.get("password")
 
-        if not reset_token or not password:
-            return {"msg": "The reset token and/or password is missing!"}, \
-                HTTPStatus.BAD_REQUEST
-
         # obtain user
         try:
             user_id = decode_token(reset_token)['sub'].get('id')
         except DecodeError:
             return {"msg": "Invalid recovery token!"}, HTTPStatus.BAD_REQUEST
 
         user = db.User.get(user_id)
@@ -188,22 +205,25 @@
             description: No username or email provided
 
         tags: ["Account recovery"]
         """
         # default return string
         ret = {"msg": "If the username or email is in our database you "
                       "will soon receive an email."}
-
-        # obtain username/email from request'
         body = request.get_json()
+
+        # validate request body
+        errors = recover_pw_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
+        # obtain username/email from request
         username = body.get("username")
         email = body.get("email")
-        if not (email or username):
-            return {"msg": "No username or email provided!"}, \
-                HTTPStatus.BAD_REQUEST
 
         # find user in the database, if not here we stop!
         try:
             if username:
                 user = db.User.get_by_username(username)
             else:
                 user = db.User.get_by_email(email)
@@ -277,20 +297,23 @@
           400:
             description: Recovery token is missing or invalid
 
         tags: ["Account recovery"]
         """
         # retrieve user based on email or username
         body = request.get_json()
-        reset_token = body.get("reset_token")
-        if not reset_token:
-            return {"msg": "The reset token is missing!"}, \
+
+        # validate request body
+        errors = reset_2fa_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
                 HTTPStatus.BAD_REQUEST
 
         # obtain user
+        reset_token = body.get("reset_token")
         try:
             user_id = decode_token(reset_token)['sub'].get('id')
         except DecodeError:
             return {"msg": "Invalid recovery token!"}, HTTPStatus.BAD_REQUEST
 
         user = db.User.get(user_id)
 
@@ -332,24 +355,26 @@
 
         tags: ["Account recovery"]
         """
         # default return string
         ret = {"msg": "If you sent a correct combination of username/email and"
                       "password, you will soon receive an email."}
 
-        # obtain parameters from request'
+        # obtain parameters from request
         body = request.get_json()
+
+        # validate request body
+        errors = recover_2fa_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
         username = body.get("username")
         email = body.get("email")
-        if not (email or username):
-            return {"msg": "No username or email provided!"}, \
-                HTTPStatus.BAD_REQUEST
         password = body.get("password")
-        if not password:
-            return {"msg": "No password provided!"}, HTTPStatus.BAD_REQUEST
 
         # find user in the database, if not here we stop!
         try:
             if username:
                 user = db.User.get_by_username(username)
             else:
                 user = db.User.get_by_email(email)
@@ -444,24 +469,23 @@
               criteria
           401:
             description: Current password is incorrect
 
         tags: ["Account recovery"]
         """
         body = request.get_json()
+        # validate request body
+        errors = change_pw_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
         old_password = body.get("current_password")
         new_password = body.get("new_password")
 
-        if not old_password:
-            return {"msg": "Your current password is missing"},  \
-                HTTPStatus.BAD_REQUEST
-        elif not new_password:
-            return {"msg": "Your new password is missing!"}, \
-                HTTPStatus.BAD_REQUEST
-
         user = g.user
         log.debug(f"Changing password for user {user.id}")
 
         # check if the old password is correct
         pw_correct = user.check_password(old_password)
         if not pw_correct:
             return {"msg": "Your current password is not correct!"}, \
@@ -510,15 +534,15 @@
 
         requestBody:
           content:
             application/json:
               schema:
                 properties:
                   id:
-                    type: int
+                    type: integer
                     description: ID of node whose API key is to be reset
 
         responses:
             200:
                 description: Ok
             400:
                 description: ID missing from json body
@@ -528,30 +552,28 @@
                 description: Node not found
 
         security:
             - bearerAuth: []
 
         tags: ["Account recovery"]
         """
-        if not request.is_json:
-            log.warning('Authentication failed because no JSON body was '
-                        'provided!')
-            return {"msg": "Missing JSON in request"}, HTTPStatus.BAD_REQUEST
-
-        # check which node should have its API key modified
-        id = request.json.get('id', None)
-        if not id:
-            msg = "ID missing in JSON body"
-            log.error(msg)
-            return {"msg": msg}, HTTPStatus.BAD_REQUEST
+        body = request.get_json()
+
+        # validate request body
+        errors = reset_api_key_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
-        # find the node
-        node = db.Node.get(id)
+        id_ = body['id']
+        node = db.Node.get(id_)
         if not node:
-            return {'msg': f'Node id={id} is not found!'}, HTTPStatus.NOT_FOUND
+            return {
+                'msg': f'Node id={id_} is not found!'
+            }, HTTPStatus.NOT_FOUND
 
         # check if user is allowed to edit the node
         if not self.r.e_glo.can():
             own = g.user.organization.id == node.organization.id
             if not (self.r.e_org.can() and own):
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/result.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 )
 from vantage6.server.resource import (
     with_node,
     only_for,
     parse_datetime,
     ServicesResources
 )
-from vantage6.server.resource.pagination import Pagination
-from vantage6.server.resource.common._schema import (
+from vantage6.server.resource.common.pagination import Pagination
+from vantage6.server.resource.common.output_schema import (
     ResultSchema,
     ResultTaskIncludedSchema
 )
 from vantage6.server.model import (
     Result as db_Result,
     Node,
     Task,
@@ -180,33 +180,40 @@
               schema:
                 type: integer
               description: Port number
             - in: query
               name: include
               schema:
                 type: string (can be multiple)
-              description: Include 'task' to include task data. Include
-                'metadata' to get pagination metadata. Note that this will put
-                the actual data in an envelope.
+              description: Include 'task' to include task data.
             - in: query
               name: page
               schema:
                 type: integer
-              description: Page number for pagination
+              description: Page number for pagination (default=1)
             - in: query
               name: per_page
               schema:
                 type: integer
-              description: Number of items per page
+              description: Number of items per page (default=10)
+            - in: query
+              name: sort
+              schema:
+                type: string
+              description: >-
+                Sort by one or more fields, separated by a comma. Use a minus
+                sign (-) in front of the field to sort in descending order.
 
         responses:
-            200:
-                description: Ok
-            401:
-                description: Unauthorized
+          200:
+            description: Ok
+          401:
+            description: Unauthorized
+          400:
+            description: Improper values for pagination or sorting parameters
 
         security:
         - bearerAuth: []
 
         tags: ["Result"]
         """
         auth_org = self.obtain_auth_organization()
@@ -225,15 +232,15 @@
                 q = q.filter(getattr(db_Result, f'{param}_at')
                              <= args[f'{param}_till'])
             if f'{param}_from' in args:
                 q = q.filter(db_Result.assigned_at >= args[f'{param}_from'])
 
         # custom filters
         if args.get('state') == 'open':
-            q = q.filter(db_Result.finished_at == None)
+            q = q.filter(db_Result.finished_at.is_(None))
 
         q = q.join(Organization).join(Node).join(Task, db_Result.task)\
             .join(Collaboration)
 
         if args.get('node_id'):
             q = q.filter(db.Node.id == args.get('node_id'))\
                 .filter(db.Collaboration.id == db.Node.collaboration_id)
@@ -245,15 +252,18 @@
                 q = q.filter(Collaboration.id.in_(col_ids))
             else:
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
         # query the DB and paginate
         q = q.order_by(desc(db_Result.id))
-        page = Pagination.from_query(query=q, request=request)
+        try:
+            page = Pagination.from_query(query=q, request=request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         # serialization of the models
         s = result_inc_schema if self.is_included('task') else result_schema
 
         return self.response(page, s)
 
 
@@ -317,15 +327,15 @@
             if not (self.r.v_org.can() and auth_org in c_orgs):
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
         s = result_inc_schema if request.args.get('include') == 'task' \
             else result_schema
 
-        return s.dump(result, many=False).data, HTTPStatus.OK
+        return s.dump(result, many=False), HTTPStatus.OK
 
     @with_node
     def patch(self, id):
         """Update results
         ---
         description: >-
           Update results from the node. Only done if the request comes from the
@@ -404,8 +414,8 @@
                                            result.started_at)
         result.finished_at = parse_datetime(data.get("finished_at"))
         result.result = data.get("result")
         result.log = data.get("log")
         result.status = data.get("status", result.status)
         result.save()
 
-        return result_schema.dump(result, many=False).data, HTTPStatus.OK
+        return result_schema.dump(result, many=False), HTTPStatus.OK
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/role.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/role.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # -*- coding: utf-8 -*-
 import logging
 
 from http import HTTPStatus
 from flask.globals import request
 from flask import g
-from flask_restful import reqparse, Api
+from flask_restful import Api
 from sqlalchemy import or_
 
 from vantage6.server import db
 from vantage6.server.resource import (
+    get_org_ids_from_collabs,
     with_user,
     ServicesResources
 )
 from vantage6.common import logger_name
 from vantage6.server.permission import (
-    PermissionManager
+    PermissionManager,
+    RuleCollection,
+    Operation as P,
 )
 from vantage6.server.model.rule import Operation, Scope
-from vantage6.server.resource.common._schema import RoleSchema, RuleSchema
-from vantage6.server.resource.pagination import Pagination
+from vantage6.server.resource.common.output_schema import (
+    RoleSchema, RuleSchema
+)
+from vantage6.server.resource.common.input_schema import RoleInputSchema
+from vantage6.server.resource.common.pagination import Pagination
 from vantage6.server.default_roles import DefaultRole
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
@@ -53,21 +59,14 @@
         path + '/<int:id>',
         endpoint="role_with_id",
         methods=('GET', 'PATCH', 'DELETE'),
         resource_class_kwargs=services
     )
     api.add_resource(
         RoleRules,
-        path + '/<int:id>/rule',
-        endpoint='role_rule_without_id',
-        methods=('GET',),
-        resource_class_kwargs=services
-    )
-    api.add_resource(
-        RoleRules,
         path + '/<int:id>/rule/<int:rule_id>',
         endpoint='role_rule_with_id',
         methods=('DELETE', 'POST'),
         resource_class_kwargs=services
     )
 
 
@@ -82,42 +81,52 @@
     ----------
     permissions : PermissionManager
         Permission manager instance to which permissions are added
     """
     add = permissions.appender(module_name)
     add(scope=Scope.GLOBAL, operation=Operation.VIEW,
         description="View any role")
+    add(scope=Scope.COLLABORATION, operation=Operation.VIEW,
+        description="View any role in your collaborations")
     add(scope=Scope.ORGANIZATION, operation=Operation.VIEW,
         description="View the roles of your organization")
     add(scope=Scope.GLOBAL, operation=Operation.CREATE,
         description="Create role for any organization")
+    add(scope=Scope.COLLABORATION, operation=Operation.CREATE,
+        description="Create role for any organization in your collaborations")
     add(scope=Scope.ORGANIZATION, operation=Operation.CREATE,
         description="Create role for your organization")
     add(scope=Scope.GLOBAL, operation=Operation.EDIT,
         description="Edit any role")
+    add(scope=Scope.COLLABORATION, operation=Operation.EDIT,
+        description="Edit any role in your collaborations")
     add(scope=Scope.ORGANIZATION, operation=Operation.EDIT,
         description="Edit a role from your organization")
     add(scope=Scope.GLOBAL, operation=Operation.DELETE,
-        description="Delete any organization")
+        description="Delete a role from any organization")
+    add(scope=Scope.COLLABORATION, operation=Operation.DELETE,
+        description="Delete a role from any organization in your "
+                    "collaborations")
     add(scope=Scope.ORGANIZATION, operation=Operation.DELETE,
-        description="Delete your organization")
+        description="Delete a role from your organization")
 
 
 # -----------------------------------------------------------------------------
 # Resources / API's
 # -----------------------------------------------------------------------------
 role_schema = RoleSchema()
 rule_schema = RuleSchema()
+role_input_schema = RoleInputSchema()
 
 
 class RoleBase(ServicesResources):
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
 
 
 class Roles(RoleBase):
 
     @with_user
     def get(self):
         """Returns a list of roles
@@ -129,14 +138,16 @@
             organization.\n
 
             ### Permission Table\n
             |Rule name|Scope|Operation|Assigned to node|Assigned to container|
             Description|\n
             |--|--|--|--|--|--|\n
             |Role|Global|View|❌|❌|View all roles|\n
+            |Role|Collaboration|View|❌|❌|View all roles in your
+            collaborations|\n
             |Role|Organization|View|❌|❌|View roles that are part of your
             organization|\n
 
             Accesible to users.
 
         parameters:
             - in: query
@@ -161,105 +172,166 @@
               name: organization_id
               schema:
                 type: array
                 items:
                   type: integer
                   description: Organization id of which you want to get roles
             - in: query
+              name: collaboration_id
+              schema:
+              type: integer
+              description: Collaboration id
+            - in: query
               name: rule_id
               schema:
                 type: integer
-              description: Rule that is part of a role
+              description: Get roles that this role id is part of
             - in: query
               name: user_id
               schema:
                 type: integer
-              description: get roles for this user id
+              description: Get roles for this user id
             - in: query
               name: include_root
               schema:
                  type: boolean
-              description: Whether or not to include root role
-            - in: query
-              name: include
-              schema:
-                type: string (can be multiple)
-              description: Include 'metadata' to get pagination metadata. Note
-                that this will put the actual data in an envelope.
+              description: Whether or not to include root role (default=False)
             - in: query
               name: page
               schema:
                 type: integer
-              description: Page number for pagination
+              description: Page number for pagination (default=1)
             - in: query
               name: per_page
               schema:
                 type: integer
-              description: Number of items per page
+              description: Number of items per page (default=10)
+            - in: query
+              name: sort
+              schema:
+                type: string
+              description: >-
+                Sort by one or more fields, separated by a comma. Use a minus
+                sign (-) in front of the field to sort in descending order.
 
         responses:
-            200:
-                description: Ok
-            401:
-                description: Unauthorized
+          200:
+            description: Ok
+          401:
+            description: Unauthorized
+          400:
+            description: Improper values for pagination or sorting parameters
 
         security:
             - bearerAuth: []
 
         tags: ["Role"]
         """
         q = g.session.query(db.Role)
 
-        auth_org_id = self.obtain_organization_id()
+        auth_org = self.obtain_auth_organization()
         args = request.args
 
         # filter by organization ids (include root role if desired)
         org_filters = args.getlist('organization_id')
         if org_filters:
+            for org_id in org_filters:
+                if not self.r.can_for_org(P.VIEW, org_id):
+                    return {
+                        'msg': 'You lack the permission view all roles from '
+                        f'organization {org_id}!'
+                    }, HTTPStatus.UNAUTHORIZED
             if 'include_root' in args and args['include_root']:
                 q = q.filter(or_(
                     db.Role.organization_id.in_(org_filters),
-                    db.Role.organization_id == None
+                    db.Role.organization_id.is_(None)
                 ))
             else:
                 q = q.filter(db.Role.organization_id.in_(org_filters))
 
+        # filter by collaboration id
+        if 'collaboration_id' in args:
+            if not self.r.can_for_col(P.VIEW, args['collaboration_id']):
+                return {
+                    'msg': 'You lack the permission view all roles from '
+                    f'collaboration {args["collaboration_id"]}!'
+                }, HTTPStatus.UNAUTHORIZED
+            org_ids = get_org_ids_from_collabs(g.user,
+                                               args['collaboration_id'])
+            if 'include_root' in args and args['include_root']:
+                q = q.filter(or_(
+                    db.Role.organization_id.in_(org_ids),
+                    db.Role.organization_id.is_(None)
+                ))
+            else:
+                q = q.filter(db.Role.organization_id.in_(org_ids))
+
         # filter by one or more names or descriptions
         for param in ['name', 'description']:
             filters = args.getlist(param)
             if filters:
                 q = q.filter(or_(*[
                     getattr(db.Role, param).like(f) for f in filters
                 ]))
 
         # find roles containing a specific rule
         if 'rule_id' in args:
+            rule = db.Rule.get(args['rule_id'])
+            if not rule:
+                return {'msg': f'Rule with id={args["rule_id"]} does not '
+                        'exist!'}, HTTPStatus.BAD_REQUEST
             q = q.join(db.role_rule_association).join(db.Rule)\
                  .filter(db.Rule.id == args['rule_id'])
 
         if 'user_id' in args:
+            user = db.User.get(args['user_id'])
+            if not user:
+                return {'msg': f'User with id={args["user_id"]} does not '
+                        'exist!'}, HTTPStatus.BAD_REQUEST
+            elif not self.r.can_for_org(P.VIEW, user.organization_id) and not \
+                    g.user.id == user.id:
+                return {
+                    'msg': 'You lack the permission view roles from the '
+                    f'organization that user id={user.id} belongs to!'
+                }, HTTPStatus.UNAUTHORIZED
             q = q.join(db.Permission).join(db.User)\
                  .filter(db.User.id == args['user_id'])
 
         if not self.r.v_glo.can():
             own_role_ids = [role.id for role in g.user.roles]
-            if self.r.v_org.can():
+            if self.r.v_col.can():
+                q = q.filter(or_(
+                    db.Role.id.in_(own_role_ids),
+                    db.Role.organization_id.is_(None),
+                    db.Role.organization_id.in_(
+                        [
+                            org.id
+                            for col in self.obtain_auth_collaborations()
+                            for org in col.organizations
+                        ]
+                    )
+                ))
+            elif self.r.v_org.can():
                 # allow user to view all roles of their organization and any
                 # other roles they may have themselves, or default roles from
                 # the root organization
                 q = q.filter(or_(
-                        db.Role.organization_id == auth_org_id,
+                        db.Role.organization_id == auth_org.id,
                         db.Role.id.in_(own_role_ids),
-                        db.Role.organization_id == None
+                        db.Role.organization_id.is_(None)
                     ))
             else:
                 # allow users without permission to view only their own roles
                 q = q.filter(db.Role.id.in_(own_role_ids))
 
-        page = Pagination.from_query(query=q, request=request)
+        # paginate results
+        try:
+            page = Pagination.from_query(query=q, request=request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         return self.response(page, role_schema)
 
     @with_user
     def post(self):
         """Creates a new role.
         ---
@@ -269,14 +341,16 @@
           organizations if you have gobal permission.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Role|Global|Create|❌|❌|Create a role for any organization|\n
+          |Role|Collaboration|Create|❌|❌|Create a role for organization in
+          your collaborations|\n
           |Role|Organization|Create|❌|❌|Create a role for your organization|\n
 
           Accessible to users.
 
         requestBody:
           content:
             application/json:
@@ -310,27 +384,20 @@
             description: Organization or rule was not found
 
         security:
           - bearerAuth: []
 
         tags: ["Role"]
         """
-        parser = reqparse.RequestParser()
-        parser.add_argument("name", type=str, required=True)
-        parser.add_argument("description", type=str, required=True)
-        parser.add_argument("rules", type=int, action='append', required=False)
-        parser.add_argument("organization_id", type=int, required=False)
-        data = parser.parse_args()
-
-        # check if role name is allowed (i.e. not a default role name)
-        if 'name' in data and data['name'] in [role for role in DefaultRole]:
-            return {
-                "msg": f"Cannot create role '{data['name']}' as it is a "
-                       "reserved role name."
-            }, HTTPStatus.BAD_REQUEST
+        data = request.get_json()
+        # validate request body
+        errors = role_input_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         # obtain the requested rules from the DB.
         rules = []
         if data['rules']:
             for rule_id in data["rules"]:
                 rule = db.Rule.get(rule_id)
                 if not rule:
@@ -342,37 +409,34 @@
         denied = self.permissions.check_user_rules(rules)
         if denied:
             return denied, HTTPStatus.UNAUTHORIZED
 
         # set the organization id
         organization_id = (
             data['organization_id']
-            if data['organization_id'] else g.user.organization_id
+            if 'organization_id' in data else g.user.organization_id
         )
         # verify that the organization for which we create a role exists
         if not db.Organization.get(organization_id):
             return {'msg': f'organization "{organization_id}" does not '
                     'exist!'}, HTTPStatus.NOT_FOUND
 
         # check if user is allowed to create this role
-        if (not self.r.c_glo.can() and
-                organization_id != g.user.organization_id):
+        if not self.r.can_for_org(P.CREATE, organization_id):
             return {
-                'msg': 'You cannot create roles for other organizations!'
+                'msg': 'You cannot create a role for this organization!'
             }, HTTPStatus.UNAUTHORIZED
-        elif not self.r.c_glo.can() and not self.r.c_org.can():
-            return {'msg': 'You lack the permission to create roles!'}, \
-                HTTPStatus.UNAUTHORIZED
 
         # create the actual role
-        role = db.Role(name=data["name"], description=data["description"],
-                       rules=rules, organization_id=organization_id)
+        role = db.Role(name=data.get("name"),
+                       description=data.get("description"), rules=rules,
+                       organization_id=organization_id)
         role.save()
 
-        return role_schema.dump(role, many=False).data, HTTPStatus.CREATED
+        return role_schema.dump(role, many=False), HTTPStatus.CREATED
 
 
 class Role(RoleBase):
 
     @with_user
     def get(self, id):
         """Get roles
@@ -381,14 +445,16 @@
           Get role based on role identifier.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Role|Global|View|❌|❌|View all roles|\n
+          |Role|Collaboration|View|❌|❌|View all roles for your
+          collaborations|\n
           |Role|Organization|View|❌|❌|View roles that are part of your
           organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
@@ -413,34 +479,37 @@
         role = db.Role.get(id)
 
         if not role:
             return {"msg": f"Role with id={id} not found."}, \
                 HTTPStatus.NOT_FOUND
 
         # check permissions. A user can always view their own roles
-        if not (self.r.v_glo.can() or role in g.user.roles):
-            if not (self.r.v_org.can()
-                    and role.organization == g.user.organization):
-                return {"msg": "You do not have permission to view this."},\
-                     HTTPStatus.UNAUTHORIZED
+        if not (
+            self.r.can_for_org(P.VIEW, role.organization_id) or
+            role in g.user.roles
+        ):
+            return {"msg": "You do not have permission to view this."},\
+                    HTTPStatus.UNAUTHORIZED
 
-        return role_schema.dump(role, many=False).data, HTTPStatus.OK
+        return role_schema.dump(role, many=False), HTTPStatus.OK
 
     @with_user
     def patch(self, id):
         """Update role
         ---
         description: >-
           Updates roles if the user has permission to do so.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Role|Global|Edit|❌|❌|Update any role|\n
+          |Role|Collaboration|Edit|❌|❌|Update any role in your
+          collaborations|\n
           |Role|Organization|Edit|❌|❌|Update a role from your organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
@@ -480,39 +549,40 @@
         security:
           - bearerAuth: []
 
         tags: ["Role"]
         """
         data = request.get_json()
 
+        # validate request body
+        errors = role_input_schema.validate(data, partial=True)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+        # organization_id cannot be changed in PATCH, only defined in POST
+        if 'organization_id' in data:
+            return {'msg': 'Cannot change organization of a role.'}, \
+                HTTPStatus.BAD_REQUEST
+
         role = db.Role.get(id)
         if not role:
             return {"msg": f"Role with id={id} not found."}, \
                 HTTPStatus.NOT_FOUND
 
-        # check if role name is allowed (i.e. not a default role name)
-        if 'name' in data and data['name'] in [role for role in DefaultRole]:
-            return {
-                "msg": f"Cannot change role name into '{data['name']}' as that"
-                       " is a reserved role name."
-            }, HTTPStatus.BAD_REQUEST
-        elif role.name in [role for role in DefaultRole]:
+        # check if user tries to change name of a default role
+        if role.name in [role for role in DefaultRole]:
             return {
                 "msg": f"This role ('{role.name}') is a default role. Its name"
                        " cannot be changed."
             }, HTTPStatus.BAD_REQUEST
 
         # check permission of the user
-        if not self.r.e_glo.can():
-            if not self.r.e_org.can():
-                return {'msg': 'You do not have permission to edit roles!'}, \
-                    HTTPStatus.UNAUTHORIZED
-            elif g.user.organization_id != role.organization.id:
-                return {'msg': 'You can\'t edit roles from another '
-                        'organization'}, HTTPStatus.UNAUTHORIZED
+        if not self.r.can_for_org(P.EDIT, role.organization_id):
+            return {'msg': 'You do not have permission to edit this role!'}, \
+                HTTPStatus.UNAUTHORIZED
 
         # process patch
         if 'name' in data:
             role.name = data["name"]
         if 'description' in data:
             role.description = data["description"]
         if 'rules' in data:
@@ -525,45 +595,55 @@
                 rules.append(rule)
             denied = self.permissions.check_user_rules(rules)
             if denied:
                 return denied, HTTPStatus.UNAUTHORIZED
             role.rules = rules
         role.save()
 
-        return role_schema.dump(role, many=False).data, HTTPStatus.OK
+        return role_schema.dump(role, many=False), HTTPStatus.OK
 
     @with_user
     def delete(self, id):
         """Delete role
         ---
         description: >-
           Delete role from an organization if user is allowed to delete the
           role.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Role|Global|Delete|❌|❌|Delete any role|\n
+          |Role|Collaboration|Delete|❌|❌|Delete any role in your
+          collaborations|\n
           |Role|Organization|Delete|❌|❌|Delete a role in your organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
               type: integer
               minimum: 1
             description: Role id
             required: true
+          - in: query
+            name: delete_dependents
+            schema:
+              type: boolean
+            description: If set to true, the role is deleted even though users
+               with this role may lose permissions (default=False)
 
         responses:
           200:
             description: Ok
+          400:
+            description: Cannot delete default roles
           401:
             description: Unauthorized
           404:
             description: Role id not found
 
         security:
           - bearerAuth: []
@@ -571,116 +651,60 @@
         tags: ["Role"]
         """
         role = db.Role.get(id)
         if not role:
             return {"msg": f"Role with id={id} not found."}, \
                 HTTPStatus.NOT_FOUND
 
-        if not self.r.d_glo.can():
-            if not self.r.d_org.can():
-                return {'msg': 'You do not have permission to delete roles!'},\
-                    HTTPStatus.UNAUTHORIZED
-            elif role.organization.id != g.user.organization.id:
-                return {'msg': 'You can\'t delete a role from another '
-                        'organization'}, HTTPStatus.UNAUTHORIZED
+        if role.name in [role for role in DefaultRole]:
+            return {
+                "msg": f"This role ('{role.name}') is a default role. Default"
+                       " roles cannot be deleted."
+            }, HTTPStatus.BAD_REQUEST
+
+        if not self.r.can_for_org(P.DELETE, role.organization_id):
+            return {'msg': 'You do not have permission to delete this role!'},\
+                HTTPStatus.UNAUTHORIZED
+
+        # check if role is assigned to users
+        if role.users:
+            params = request.args
+            if not params.get('delete_dependents', False):
+                return {
+                    'msg': "Role is assigned to users. Please remove the role "
+                    "from the users first, or set the 'delete_dependents' "
+                    "parameter to delete the role anyway."
+                }, HTTPStatus.BAD_REQUEST
+            else:
+                log.warn(f"Role {id} deleted even though it was assigned to "
+                         "users. This may result in missing permissions.")
+                # Note that the role is removed from the users automatically
+                # due to the relationship between the role and the user.
 
         role.delete()
 
         return {"msg": "Role removed from the database."}, HTTPStatus.OK
 
 
 class RoleRules(RoleBase):
-
-    @with_user
-    def get(self, id):
-        """Returns the rules for a specific role
-        ---
-        description: >-
-            View the rules that belong to a specific role.\n
-
-            ### Permission Table\n
-            |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-            Description|\n
-            |--|--|--|--|--|--|\n
-            |Role|Global|View|❌|❌|View a role's rules|\n
-            |Role|Organization|View|❌|❌|View a role's rules for roles in
-            your organization|\n
-
-            Accessible to users.
-
-        parameters:
-            - in: path
-              name: id
-              schema:
-                type: integer
-              minimum: 1
-              description: Role id
-              required: true
-            - in: query
-              name: include
-              schema:
-                type: string (can be multiple)
-              description: Include 'metadata' to get pagination metadata. Note
-                that this will put the actual data in an envelope.
-            - in: query
-              name: page
-              schema:
-                type: integer
-              description: Page number for pagination
-            - in: query
-              name: per_page
-              schema:
-                type: integer
-              description: Number of items per page
-
-        responses:
-            200:
-                description: Ok
-            404:
-                description: Node with specified id is not found
-            401:
-                description: Unauthorized
-
-        security:
-            - bearerAuth: []
-
-        tags: ["Role"]
-        """
-        role = db.Role.get(id)
-
-        if not role:
-            return {'msg': f'Role id={id} not found!'}, HTTPStatus.NOT_FOUND
-
-        # obtain auth organization model
-        auth_org = self.obtain_auth_organization()
-
-        # check permission
-        if not self.r.v_glo.can():
-            if not (self.r.v_org.can() and auth_org == role.organization):
-                return {'msg': 'You lack permissions to do that'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        # paginate elements
-        page = Pagination.from_list(role.rules, request)
-
-        return self.response(page, rule_schema)
-
     @with_user
     def post(self, id, rule_id):
         """Add a rule to a role.
         ---
         description: >-
           Add a rule to a role given that the role exists already and that the
           user has the permission to do so.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Role|Global|Edit|❌|❌|Edit any role|\n
+          |Role|Collaboration|Edit|❌|❌|Edit any role in your collaborations
+          |\n
           |Role|Organization|Edit|❌|❌|Edit any role in your organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
@@ -713,46 +737,45 @@
             return {'msg': f'Role id={id} not found!'}, HTTPStatus.NOT_FOUND
         rule = db.Rule.get(rule_id)
         if not rule:
             return {'msg': f'Rule id={rule_id} not found!'}, \
                 HTTPStatus.NOT_FOUND
 
         # check that this user can edit rules
-        if not self.r.e_glo.can():
-            if not (self.r.e_org.can() and
-                    g.user.organization == role.organization):
-                return {'msg': 'You lack permissions to do that'}, \
-                    HTTPStatus.UNAUTHORIZED
+        if not self.r.can_for_org(P.EDIT, role.organization_id):
+            return {'msg': 'You lack permissions to do that'}, \
+                HTTPStatus.UNAUTHORIZED
 
         # user needs to role to assign it
         denied = self.permissions.check_user_rules([rule])
         if denied:
             return denied, HTTPStatus.UNAUTHORIZED
 
         # We're good, lets add the rule
         role.rules.append(rule)
         role.save()
 
-        return rule_schema.dump(role.rules, many=False).data, \
-            HTTPStatus.CREATED
+        return rule_schema.dump(role.rules, many=True), HTTPStatus.CREATED
 
     @with_user
     def delete(self, id, rule_id):
         """Removes rule from role.
         ---
         description: >-
           Removes a rule from a role given the user has permission and the rule
           id exists.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
-          |Role|Global|Delete|❌|❌|Delete any role rule|\n
-          |Role|Organization|Delete|❌|❌|Delete any role rule in your
+          |Role|Global|Edit|❌|❌|Delete any rule in a role|\n
+          |Role|Collaboration|Edit|❌|❌|Delete any rule in roles in your
+          collaborations|\n
+          |Role|Organization|Edit|❌|❌|Delete any rule in roles in your
           organization|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
@@ -780,27 +803,24 @@
         if not role:
             return {'msg': f'Role id={id} not found!'}, HTTPStatus.NOT_FOUND
         rule = db.Rule.get(rule_id)
         if not rule:
             return {'msg': f'Rule id={rule_id} not found!'}, \
                 HTTPStatus.NOT_FOUND
 
-        if not self.r.d_glo.can():
-            if not (self.r.d_org.can() and
-                    g.user.organization == role.organization):
-                return {'msg': 'You lack permissions to do that'}, \
-                    HTTPStatus.UNAUTHORIZED
+        if not self.r.can_for_org(P.EDIT, role.organization_id):
+            return {'msg': 'You lack permissions to do that'}, \
+                HTTPStatus.UNAUTHORIZED
 
         # user needs to role to remove it
         denied = self.permissions.check_user_rules([rule])
         if denied:
             return denied, HTTPStatus.UNAUTHORIZED
 
         if not (rule in role.rules):
             return {'msg': f'Rule id={rule_id} not found in Role={id}!'}, \
                 HTTPStatus.NOT_FOUND
 
         # Ok jumped all hoopes, remove it..
         role.rules.remove(rule)
 
-        return rule_schema.dump(role.rules, many=False).data, \
-            HTTPStatus.OK
+        return rule_schema.dump(role.rules, many=True), HTTPStatus.OK
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/rule.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 import logging
 
 from http import HTTPStatus
 from flask.globals import request
 from flask import g
 from flask_restful import Api
+from sqlalchemy import or_
 
 from vantage6.server.resource import (
     with_user,
     ServicesResources
 )
 from vantage6.common import logger_name
 from vantage6.server import db
-from vantage6.server.resource.common._schema import RuleSchema
-from vantage6.server.resource.pagination import Pagination
+from vantage6.server.resource.common.output_schema import RuleSchema
+from vantage6.server.resource.common.pagination import Pagination
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 rule_schema = RuleSchema()
 
 
@@ -87,33 +88,48 @@
               description: Get rules for a specific scope
             - in: query
               name: role_id
               schema:
                 type: integer
               description: Get rules for a specific role
             - in: query
-              name: include
+              name: user_id
               schema:
-                type: string (can be multiple)
-              description: Include 'metadata' to get pagination metadata. Note
-                that this will put the actual data in an envelope.
+                type: integer
+              description: Get rules for a specific user. This includes the
+                rules that are part of the user's roles.
             - in: query
               name: page
               schema:
                 type: integer
-              description: Page number for pagination
+              description: Page number for pagination (default=1)
             - in: query
               name: per_page
               schema:
                 type: integer
-              description: Number of items per page
+              description: Number of items per page (default=10)
+            - in: query
+              name: sort
+              schema:
+                type: string
+              description: >-
+                Sort by one or more fields, separated by a comma. Use a minus
+                sign (-) in front of the field to sort in descending order.
+            - in: query
+              name: no_pagination
+              schema:
+                type: int
+              description: >-
+                If set to 1, pagination is disabled and all items are returned.
 
         responses:
           200:
             description: Ok
+          400:
+            description: Improper values for pagination or sorting parameters
 
         security:
             - bearerAuth: []
 
         tags: ["Rule"]
         """
         q = g.session.query(db.Rule)
@@ -126,16 +142,38 @@
                 q = q.filter(getattr(db.Rule, param) == args[param])
 
         # find roles containing a specific rule
         if 'role_id' in args:
             q = q.join(db.role_rule_association).join(db.Role)\
                  .filter(db.Role.id == args['role_id'])
 
+        # find all rules of a specific user. This is done by first joining all
+        # tables to find all rules originating from a user's roles. Then, we
+        # do an outer join to find all rules that are directly assigned to the
+        # user.
+        if 'user_id' in args:
+            q = q.join(db.role_rule_association).join(db.Role)\
+                 .join(db.Permission).join(db.User)\
+                 .outerjoin(db.UserPermission,
+                            db.Rule.id == db.UserPermission.c.rule_id)\
+                 .filter(or_(
+                    db.User.id == args['user_id'],
+                    db.UserPermission.c.user_id == args['user_id']
+                 ))
+
+        # check if pagination is disabled
+        paginate = True
+        if 'no_pagination' in args and args['no_pagination'] == '1':
+            paginate = False
+
         # paginate results
-        page = Pagination.from_query(q, request)
+        try:
+            page = Pagination.from_query(q, request, paginate=paginate)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         # model serialization
         return self.response(page, rule_schema)
 
 
 class Rule(ServicesResources):
 
@@ -169,8 +207,8 @@
 
         tags: ["Rule"]
         """
         rule = db.Rule.get(id)
         if not rule:
             return {'msg': f'Rule id={id} not found!'}, HTTPStatus.NOT_FOUND
 
-        return rule_schema.dump(rule, many=False).data, HTTPStatus.OK
+        return rule_schema.dump(rule, many=False), HTTPStatus.OK
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/stats.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,9 +35,9 @@
 
 #     # stats_schema = StatsSchema()
 #     @only_for(("user", "node"))
 #     def get(self, id=None):
 #         schema = CollaborationSchemaSimple(many=True)
 
 #         return {
-#             'collaborations': schema.dump(db.Collaboration.get()).data
+#             'collaborations': schema.dump(db.Collaboration.get())
 #         }, HTTPStatus.OK
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/task.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 from http import HTTPStatus
 from sqlalchemy import desc
 
 from vantage6.common.globals import STRING_ENCODING
 from vantage6.common.task_status import TaskStatus, has_task_finished
 from vantage6.server import db
 from vantage6.server.permission import (
+    RuleCollection,
     Scope as S,
     PermissionManager,
     Operation as P
 )
 from vantage6.server.resource import only_for, ServicesResources, with_user
-from vantage6.server.resource.common._schema import (
+from vantage6.server.resource.common.output_schema import (
     TaskSchema,
     TaskIncludedSchema,
-    TaskResultSchema
 )
-from vantage6.server.resource.pagination import Pagination
+from vantage6.server.resource.common.input_schema import TaskInputSchema
+from vantage6.server.resource.common.pagination import Pagination
 from vantage6.server.resource.event import kill_task
 
 
 module_name = __name__.split('.')[-1]
 log = logging.getLogger(module_name)
 
 
@@ -55,21 +56,14 @@
     api.add_resource(
         Task,
         path + '/<int:id>',
         endpoint='task_with_id',
         methods=('GET', 'DELETE'),
         resource_class_kwargs=services
     )
-    api.add_resource(
-        TaskResult,
-        path + '/<int:id>/result',
-        endpoint='task_result',
-        methods=('GET',),
-        resource_class_kwargs=services
-    )
 
 
 # -----------------------------------------------------------------------------
 # Permissions
 # -----------------------------------------------------------------------------
 def permissions(permissions: PermissionManager) -> None:
     """
@@ -78,48 +72,58 @@
     Parameters
     ----------
     permissions : PermissionManager
         Permission manager instance to which permissions are added
     """
     add = permissions.appender(module_name)
 
-    add(scope=S.GLOBAL, operation=P.VIEW,
-        description="view any task")
-    add(scope=S.ORGANIZATION, operation=P.VIEW, assign_to_container=True,
-        assign_to_node=True, description="view tasks of your organization")
+    add(scope=S.GLOBAL, operation=P.VIEW, description="view any task")
+    add(scope=S.COLLABORATION, operation=P.VIEW, assign_to_container=True,
+        assign_to_node=True, description="view tasks of your collaborations")
+    add(scope=S.ORGANIZATION, operation=P.VIEW,
+        description="view tasks that your organization initiated")
+    add(scope=S.OWN, operation=P.VIEW,
+        description="view tasks that you initiated")
 
     add(scope=S.GLOBAL, operation=P.CREATE, description="create a new task")
-    add(scope=S.ORGANIZATION, operation=P.CREATE,
+    add(scope=S.COLLABORATION, operation=P.CREATE,
         description=(
             "create a new task for collaborations in which your organization "
             "participates with"
         ))
 
     add(scope=S.GLOBAL, operation=P.DELETE,
         description="delete a task")
+    add(scope=S.COLLABORATION, operation=P.DELETE,
+        description="delete a task from your collaborations")
     add(scope=S.ORGANIZATION, operation=P.DELETE,
         description=(
             "delete a task from a collaboration in which your organization "
             "participates with"
         ))
+    add(scope=S.OWN, operation=P.DELETE,
+        description="delete tasks that you created")
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 task_schema = TaskSchema()
 task_result_schema = TaskIncludedSchema()
-task_result_schema2 = TaskResultSchema()
+task_input_schema = TaskInputSchema()
 
 
 class TaskBase(ServicesResources):
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
+        # permissions for the run resource are also relevant for the task
+        # resource as they are sometimes included
+        self.r_run: RuleCollection = getattr(self.permissions, 'run')
 
 
 class Tasks(TaskBase):
 
     @only_for(("user", "node", "container"))
     def get(self):
         """List tasks
@@ -128,36 +132,47 @@
           Returns a list of tasks.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Task|Global|View|❌|❌|View any task|\n
-          |Task|Organization|View|✅|✅|View any task in your organization|
+          |Task|Collaboration|View|✅|✅|View any task in your collaborations|
           \n
+          |Task|Organization|View|❌|❌|View any task that your organization
+          created|\n
+          |Task|Own|View|❌|❌|View any task that you created|\n
 
           Accessible to users.
 
         parameters:
           - in: query
-            name: initiator_id
+            name: init_org_id
             schema:
               type: int
             description: The organization id of the origin of the request
           - in: query
             name: init_user_id
             schema:
               type: int
             description: The user id of the user that started the task
           - in: query
             name: collaboration_id
             schema:
               type: int
             description: The collaboration id to which the task belongs
           - in: query
+            name: is_user_created
+            schema:
+              type: int
+            description: >-
+              If larger than 0, returns tasks created by a user (top-level
+              tasks). If equal to 0, returns subtask created by an algorithm.
+              If not specified, both are returned.
+          - in: query
             name: image
             schema:
               type: str
             description: >-
               (Docker) image name which is used in the task. Name to match
               with a LIKE operator. \n
               * The percent sign (%) represents zero, one, or multiple
@@ -165,15 +180,15 @@
               * underscore sign (_) represents one, single character
           - in: query
             name: parent_id
             schema:
               type: int
             description: The id of the parent task
           - in: query
-            name: run_id
+            name: job_id
             schema:
               type: int
             description: The run id that belongs to the task
           - in: query
             name: name
             schema:
               type: str
@@ -197,89 +212,188 @@
               type: string
             description: >-
               Database description to match with a LIKE operator. \n
               * The percent sign (%) represents zero, one, or multiple
               characters\n
               * underscore sign (_) represents one, single character
           - in: query
-            name: result_id
+            name: run_id
             schema:
               type: int
-            description: A result id that belongs to the task
+            description: A run id that belongs to the task
           - in: query
             name: include
             schema:
               type: array
               items:
                 type: string
-            description: Include 'results' to get task results. Include
-              'metadata' to get pagination metadata. Note that this will
-              put the actual data in an envelope.
+            description: Include 'results' to get task results.
           - in: query
             name: status
             schema:
               type: string
             description: Filter by task status, e.g. 'active' for active
               tasks, 'completed' for finished or 'crashed' for failed tasks.
           - in: query
             name: page
             schema:
               type: integer
-            description: Page number for pagination
+            description: Page number for pagination (default=1)
           - in: query
             name: per_page
             schema:
               type: integer
-            description: Number of items per page
+            description: Number of items per page (default=10)
+          - in: query
+            name: sort
+            schema:
+              type: string
+            description: >-
+              Sort by one or more fields, separated by a comma. Use a minus
+              sign (-) in front of the field to sort in descending order.
 
         responses:
           200:
             description: Ok
           400:
-            description: Non-allowed parameter values
+            description: Non-allowed or wrong parameter values
           401:
             description: Unauthorized
 
         security:
             - bearerAuth: []
 
         tags: ["Task"]
         """
         q = g.session.query(db.Task)
         args = request.args
 
-        # obtain organization id
         auth_org_id = self.obtain_organization_id()
 
         # check permissions and apply filter if neccassary
         if not self.r.v_glo.can():
-            if self.r.v_org.can():
+            if self.r.v_col.can():
                 q = q.join(db.Collaboration).join(db.Organization)\
                     .filter(db.Collaboration.organizations.any(id=auth_org_id))
+            elif self.r.v_org.can():
+                q = q.join(db.Organization)\
+                    .filter(db.Task.init_org_id == auth_org_id)
+            elif self.r.v_own.can():
+                q = q.filter(db.Task.init_user_id == g.user.id)
             else:
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
+        # if results are included, check permissions on results
+        if self.is_included('results'):
+            max_scope_task = self.r.get_max_scope(P.VIEW)
+            if not self.r_run.has_at_least_scope(max_scope_task, P.VIEW):
+                max_scope_run = self.r_run.get_max_scope(P.VIEW)
+                return {
+                    'msg': 'You cannot view the results of all tasks, as you '
+                    f'are allowed to view tasks with scope {max_scope_task} '
+                    f'but you can only view results with scope {max_scope_run}'
+                }, HTTPStatus.UNAUTHORIZED
+
+        if 'collaboration_id' in args:
+            if not self.r.can_for_col(P.VIEW, args['collaboration_id']):
+                return {'msg': 'You lack the permission to view tasks '
+                        f'from collaboration {args["collaboration_id"]}!'}, \
+                    HTTPStatus.UNAUTHORIZED
+            q = q.join(db.Collaboration).filter(
+                db.Collaboration.id == args['collaboration_id'])
 
-        # filter based on arguments
-        for param in ['initiator_id', 'init_user_id', 'collaboration_id',
-                      'parent_id', 'run_id']:
-            if param in args:
-                q = q.filter(getattr(db.Task, param) == args[param])
-        for param in ['name', 'image', 'description', 'database', 'status']:
+        if 'init_org_id' in args:
+            if not self.r.can_for_org(P.VIEW, args['init_org_id']):
+                return {'msg': 'You lack the permission to view tasks '
+                        f'from organization id={args["init_org_id"]}!'}, \
+                    HTTPStatus.UNAUTHORIZED
+            q = q.filter(db.Task.init_org_id == args['init_org_id'])
+
+        if 'init_user_id' in args:
+            init_user = db.User.get(args['init_user_id'])
+            if not init_user:
+                return {'msg': f'User id={args["init_user_id"]} does not '
+                        'exist!'}, HTTPStatus.BAD_REQUEST
+            elif not self.r.can_for_org(P.VIEW, init_user.organization_id) \
+                    and not (self.r.v_own.can() and g.user and
+                             init_user.id == g.user.id):
+                return {'msg': 'You lack the permission to view tasks '
+                        f'from user id={args["init_user_id"]}!'}, \
+                    HTTPStatus.UNAUTHORIZED
+            q = q.filter(db.Task.init_user_id == args['init_user_id'])
+
+        if 'parent_id' in args:
+            parent = db.Task.get(args['parent_id'])
+            if not parent:
+                return {'msg': f'Parent task id={args["parent_id"]} does not '
+                        'exist!'}, HTTPStatus.BAD_REQUEST
+            elif not self.r.can_for_col(P.VIEW, parent.collaboration_id):
+                return {'msg': 'You lack the permission to view tasks '
+                        'from the collaboration that the task with parent_id='
+                        f'{parent.collaboration_id} belongs to!'}, \
+                    HTTPStatus.UNAUTHORIZED
+            q = q.filter(db.Task.parent_id == args['parent_id'])
+
+        if 'job_id' in args:
+            task_in_job = q.session.query(db.Task).filter(
+                db.Task.job_id == args['job_id']).first()
+            if not task_in_job:
+                return {'msg': f'Job id={args["job_id"]} does not exist!'}, \
+                    HTTPStatus.BAD_REQUEST
+            elif not self.r.can_for_col(P.VIEW, task_in_job.collaboration_id):
+                return {'msg': 'You lack the permission to view tasks '
+                        'from the collaboration that the task with job_id='
+                        f'{task_in_job.collaboration_id} belongs to!'}, \
+                    HTTPStatus.UNAUTHORIZED
+            q = q.filter(db.Task.job_id == args['job_id'])
+
+        for param in ['name', 'image', 'description', 'status']:
             if param in args:
                 q = q.filter(getattr(db.Task, param).like(args[param]))
-        if 'result_id' in args:
-            q = q.join(db.Result).filter(db.Result.id == args['result_id'])
 
+        if 'run_id' in args:
+            run = db.Run.get(args['run_id'])
+            if not run:
+                return {'msg': f'Run id={args["run_id"]} does not exist!'}, \
+                    HTTPStatus.BAD_REQUEST
+            elif not self.r.can_for_col(P.VIEW, run.collaboration_id):
+                return {'msg': 'You lack the permission to view tasks '
+                        'from the collaboration that the run with id='
+                        f'{run.collaboration_id} belongs to!'}, \
+                    HTTPStatus.UNAUTHORIZED
+            q = q.join(db.Run).filter(db.Run.id == args['run_id'])
+
+        if 'database' in args:
+            q = q.join(db.TaskDatabase)\
+                 .filter(db.TaskDatabase.database == args['database'])
+
+        if 'is_user_created' in args:
+            try:
+                user_created = int(args['is_user_created'])
+                if user_created == 0:
+                    q = q.filter(db.Task.parent_id.isnot(None))
+                else:
+                    q = q.filter(db.Task.parent_id.is_(None))
+            except ValueError:
+                return {"msg": (
+                    "Invalid value for 'is_user_created' provided: "
+                    f"'{args['is_user_created']}'. Should be an integer."
+                )}, HTTPStatus.BAD_REQUEST
+
+        # order to get latest task first
         q = q.order_by(desc(db.Task.id))
+
         # paginate tasks
-        page = Pagination.from_query(q, request)
+        try:
+            page = Pagination.from_query(query=q, request=request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         # serialization schema
-        schema = task_result_schema if self.is_included('result') else\
+        schema = task_result_schema if self.is_included('results') else\
             task_schema
 
         return self.response(page, schema)
 
     @only_for(("user", "container"))
     def post(self):
         """Adds new computation task
@@ -291,27 +405,27 @@
           `Container`.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Task|Global|Create|❌|❌|Create a new task|\n
-          |Task|Organization|Create|❌|✅|Create a new task for a specific
+          |Task|Collaboration|Create|❌|✅|Create a new task for a specific
           collaboration in which your organization participates|\n
 
           ## Accessed as `User`\n
-          This endpoint is accessible to users. A new `run_id` is
+          This endpoint is accessible to users. A new `job_id` is
           created when a user creates a task. The user needs to be within an
           organization that is part of the collaboration to which the task is
           posted.\n
 
           ## Accessed as `Container`\n
           When this endpoint is accessed by an algorithm container, it is
           considered to be a child-task of the container, and will get the
-          `run_id` from the initial task. Containers have limited permissions
+          `job_id` from the initial task. Containers have limited permissions
           to create tasks: they are only allowed to create tasks in the same
           collaboration using the same image.\n
 
         requestBody:
           content:
             application/json:
               schema:
@@ -331,14 +445,20 @@
 
         security:
           - bearerAuth: []
 
         tags: ["Task"]
         """
         data = request.get_json()
+        # validate request body
+        errors = task_input_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
         collaboration_id = data.get('collaboration_id')
         collaboration = db.Collaboration.get(collaboration_id)
 
         if not collaboration:
             return {"msg": f"Collaboration id={collaboration_id} not found!"},\
                    HTTPStatus.NOT_FOUND
 
@@ -390,56 +510,60 @@
                        "you are participating in!"
             }, HTTPStatus.UNAUTHORIZED
 
         # Create the new task in the database
         image = data.get('image', '')
 
         # verify permissions
-        if g.user:
-            if not self.r.c_glo.can():
-                c_orgs = collaboration.organizations
-                if not (self.r.c_org.can() and g.user.organization in c_orgs):
-                    return {'msg': 'You lack the permission to do that!'}, \
-                        HTTPStatus.UNAUTHORIZED
+        if g.user and not self.r.can_for_col(P.CREATE, collaboration.id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
 
         elif g.container:
             # verify that the container has permissions to create the task
             if not self.__verify_container_permissions(g.container, image,
                                                        collaboration_id):
                 return {"msg": "Container-token is not valid"}, \
                     HTTPStatus.UNAUTHORIZED
 
-        # permissions ok, create record
+        # permissions ok, create task record and TaskDatabase records
         task = db.Task(collaboration=collaboration, name=data.get('name', ''),
                        description=data.get('description', ''), image=image,
-                       database=data.get('database', ''),
-                       initiator=init_org)
+                       init_org=init_org)
 
-        # create run_id. Users can only create top-level -tasks (they will not
-        # have sub-tasks). Therefore, always create a new run_id. Tasks created
+        # create job_id. Users can only create top-level -tasks (they will not
+        # have sub-tasks). Therefore, always create a new job_id. Tasks created
         # by containers are always sub-tasks
         if g.user:
-            task.run_id = task.next_run_id()
+            task.job_id = task.next_job_id()
             task.init_user_id = g.user.id
-            log.debug(f"New run_id {task.run_id}")
+            log.debug(f"New job_id {task.job_id}")
         elif g.container:
             task.parent_id = g.container["task_id"]
             parent = db.Task.get(g.container["task_id"])
-            task.run_id = parent.run_id
+            task.job_id = parent.job_id
             task.init_user_id = parent.init_user_id
             log.debug(f"Sub task from parent_id={task.parent_id}")
 
         # ok commit session...
         task.save()
 
+        # save the databases that the task uses
+        databases = data.get('databases')
+        if not isinstance(databases, list):
+            databases = [databases]
+        for database in databases:
+            db_record = db.TaskDatabase(task_id=task.id, database=database)
+            db_record.save()
+
         # send socket event that task has been created
         self.socketio.emit(
             "task_created", {
                 "task_id": task.id,
-                "run_id": task.run_id,
+                "job_id": task.job_id,
                 "collaboration_id": collaboration_id,
                 "init_org_id": init_org.id,
             }, room=f"collaboration_{collaboration_id}", namespace='/tasks'
         )
 
         # if the 'master'-flag is set to true the (master) task is executed on
         # a node in the collaboration from the organization to which the user
@@ -459,33 +583,34 @@
             if not assign_orgs:
                 return {'msg': 'You\'re trying to create a master task. '
                         'However you do not have a node yourself in this '
                         'collaboration!'}, HTTPStatus.BAD_REQUEST
         else:
             assign_orgs = organizations_json_list
 
-        # now we need to create results for the nodes to fill. Each node
-        # receives their instructions from a result, not from the task itself
+        # now we need to create runs for the nodes to fill. Each node
+        # receives their instructions from an algorithm run record, not from
+        # the task itself
         log.debug(f"Assigning task to {len(assign_orgs)} nodes.")
         for org in assign_orgs:
             organization = db.Organization.get(org['id'])
             log.debug(f"Assigning task to '{organization.name}'.")
             input_ = org.get('input')
             # FIXME: legacy input from the client, could be removed at some
             # point
             if isinstance(input_, dict):
                 input_ = json.dumps(input_).encode(STRING_ENCODING)
-            # Create result
-            result = db.Result(
+            # Create run
+            run = db.Run(
                 task=task,
                 organization=organization,
                 input=input_,
                 status=TaskStatus.PENDING
             )
-            result.save()
+            run.save()
 
         # notify nodes a new task available (only to online nodes), nodes that
         # are offline will receive this task on sign in.
         self.socketio.emit('new_task', task.id, namespace='/tasks',
                            room=f'collaboration_{task.collaboration_id}')
 
         # add some logging
@@ -497,15 +622,15 @@
                       f"{g.container['node_id']}"
                       f" for (master) task_id={g.container['task_id']}")
 
         log.debug(f" url: '{url_for('task_with_id', id=task.id)}'")
         log.debug(f" name: '{task.name}'")
         log.debug(f" image: '{task.image}'")
 
-        return task_schema.dump(task, many=False).data, HTTPStatus.CREATED
+        return task_schema.dump(task, many=False), HTTPStatus.CREATED
 
     @staticmethod
     def __verify_container_permissions(container, image, collaboration_id):
         """Validates that the container is allowed to create the task."""
 
         # check that the image is allowed: algorithm containers can only
         # create tasks with the same image
@@ -513,15 +638,15 @@
             log.warning((f"Container from node={container['node_id']} "
                         f"attempts to post a task using illegal image!?"))
             log.warning(f"  task image: {image}")
             log.warning(f"  container image: {container['image']}")
             return False
 
         # check master task is not completed yet
-        if db.Task.get(container["task_id"]).complete:
+        if has_task_finished(db.Task.get(container["task_id"]).status):
             log.warning(
                 f"Container from node={container['node_id']} "
                 f"attempts to start sub-task for a completed "
                 f"task={container['task_id']}"
             )
             return False
 
@@ -583,15 +708,18 @@
           Returns the task specified by the id.
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Task|Global|View|❌|❌|View any task|\n
-          |Task|Organization|View|✅|✅|View any task in your organization|
+          |Task|Collaboration|View|✅|✅|View any task in your collaborations|
+          |Task|Organization|View|❌|❌|View any task that your organization
+          created|\n
+          |Task|Own|View|❌|❌|View any task that you created|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
@@ -617,44 +745,51 @@
 
         tags: ["Task"]
         """
         task = db.Task.get(id)
         if not task:
             return {"msg": f"task id={id} is not found"}, HTTPStatus.NOT_FOUND
 
-        # determine the organization to which the auth belongs
-        auth_org = self.obtain_auth_organization()
-
         # obtain schema
         schema = task_result_schema if request.args.get('include') == \
             'results' else task_schema
 
         # check permissions
-        if not self.r.v_glo.can():
-            org_ids = [org.id for org in task.collaboration.organizations]
-            if not (self.r.v_org.can() and auth_org.id in org_ids):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
+        if not self.r.can_for_org(P.VIEW, task.init_org_id) \
+                and not (self.r.v_own.can() and g.user and
+                         task.init_user_id == g.user.id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
+        # if results are included, check permissions for results
+        if self.is_included('results') and not \
+                self.r_run.can_for_org(P.VIEW, task.init_org_id) \
+                and not (self.r.v_own.can() and g.user and
+                         task.init_user_id == g.user.id):
+            return {'msg': 'You lack the permission to view results for this '
+                    'task!'}, HTTPStatus.UNAUTHORIZED
 
-        return schema.dump(task, many=False).data, HTTPStatus.OK
+        return schema.dump(task, many=False), HTTPStatus.OK
 
     @with_user
     def delete(self, id):
         """Remove task
         ---
         description: >-
-          Remove tasks and their results.\n
+          Remove tasks and their runs.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |Task|Global|Delete|❌|❌|Delete a task|\n
-          |Task|Organization|Delete|❌|❌|Delete a task from a collaboration
+          |Task|Collaboration|Delete|❌|❌|Delete a task from a collaboration
           in which your organization participates|\n
+          |Task|Organization|Delete|❌|❌|Delete a task that your organization
+          initiated|\n
+          |Task|Own|Delete|❌|❌|Delete a task you created yourself|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
@@ -674,112 +809,48 @@
           - bearerAuth: []
 
         tags: ["Task"]
         """
 
         task = db.Task.get(id)
         if not task:
-            return {"msg": f"task id={id} not found"}, HTTPStatus.NOT_FOUND
+            return {"msg": f"Task id={id} not found"}, HTTPStatus.NOT_FOUND
 
         # validate permissions
-        if not self.r.d_glo.can():
-            orgs = task.collaboration.organizations
-            if not (self.r.d_org.can() and g.user.organization in orgs):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
+        if not self.r.can_for_org(P.DELETE, task.init_org_id) and \
+                not (self.r.d_own.can() and task.init_user_id == g.user.id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
 
         # kill the task if it is still running
         if not has_task_finished(task.status):
             kill_task(task, self.socketio)
 
-        # retrieve results that belong to this task
+        # retrieve runs that belong to this task
         log.info(f'Removing task id={task.id}')
-        for result in task.results:
-            log.info(f" Removing result id={result.id}")
-            result.delete()
+        for run in task.runs:
+            log.info(f" Removing run id={run.id}")
+            run.delete()
+
+        # delete child/grandchild/... tasks
+        Task._delete_subtasks(task)
 
         # permissions ok, delete...
         task.delete()
 
-        return {"msg": f"task id={id} and its result successfully deleted"}, \
-            HTTPStatus.OK
-
-
-class TaskResult(ServicesResources):
-    """Resource for /api/task/<int:id>/result"""
-
-    def __init__(self, socketio, mail, api, permissions, config):
-        super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, "result")
-
-    @only_for(['user', 'container'])
-    def get(self, id):
-        """Return the results for a specific task
-        ---
-        description: >-
-          Returns the task's results specified by the task id.\n
-
-          ### Permission Table\n
-          |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-          Description|\n
-          |--|--|--|--|--|--|\n
-          |Result|Global|View|❌|❌|View any result|\n
-          |Result|Organization|View|✅|✅|View results for the
-          collaborations in which your organization participates with|\n
-
-          Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            description: Task id
-            required: true
-          - in: query
-            name: include
-            schema:
-              type: string
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
-            name: page
-            schema:
-              type: integer
-            description: Page number for pagination
-          - in: query
-            name: per_page
-            schema:
-              type: integer
-            description: Number of items per page
-
-        responses:
-          200:
-            description: Ok
-          404:
-            description: Task not found
-          401:
-            description: Unauthorized
-
-        security:
-            - bearerAuth: []
+        return {"msg": f"task id={id} and its algorithm run data have been "
+                       "successfully deleted"}, HTTPStatus.OK
 
-        tags: ["Task"]
+    @staticmethod
+    def _delete_subtasks(task: db.Task) -> None:
         """
-        task = db.Task.get(id)
-        if not task:
-            return {"msg": f"Task id={id} not found"}, HTTPStatus.NOT_FOUND
-
-        # obtain organization model
-        org = self.obtain_auth_organization()
-
-        if not self.r.v_glo.can():
-            c_orgs = task.collaboration.organizations
-            if not (self.r.v_org.can() and org in c_orgs):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
-
-        # pagination
-        page = Pagination.from_list(task.results, request)
+        Delete subtasks recursively.
 
-        # model serialization
-        return self.response(page, task_result_schema2)
+        Parameters
+        ----------
+        task : db.Task
+            Task to delete.
+        """
+        for child_task in task.children:
+            Task._delete_subtasks(child_task)
+            log.info(f" Removing child task id={child_task.id}")
+            child_task.delete()
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/token.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 # -*- coding: utf-8 -*-
 """
 Resources below '/<api_base>/token'
 """
 import logging
 import pyotp
 
-from typing import Union
 from flask import request, g
 from flask_jwt_extended import (
     jwt_required,
     create_access_token,
     create_refresh_token,
     get_jwt_identity
 )
 from flask_restful import Api
 from http import HTTPStatus
 
 from vantage6 import server
+from vantage6.common.task_status import has_task_finished
 from vantage6.server import db
 from vantage6.server.model.user import User
 from vantage6.server.resource import (
     with_node,
     ServicesResources
 )
 from vantage6.server.resource.common.auth_helper import (
   user_login, create_qr_uri
 )
+from vantage6.server.resource.common.input_schema import (
+    TokenAlgorithmInputSchema,
+    TokenNodeInputSchema,
+    TokenUserInputSchema
+)
 
 module_name = __name__.split('.')[-1]
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
     """
@@ -76,14 +81,19 @@
         path+'/refresh',
         endpoint='refresh_token',
         methods=('POST',),
         resource_class_kwargs=services
     )
 
 
+user_token_input_schema = TokenUserInputSchema()
+node_token_input_schema = TokenNodeInputSchema()
+algorithm_token_input_schema = TokenAlgorithmInputSchema()
+
+
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 class UserToken(ServicesResources):
     """resource for api/token"""
 
     def post(self):
@@ -119,26 +129,24 @@
             description: Password and/or two-factor authentication token
               incorrect.
 
         tags: ["Authentication"]
         """
         log.debug("Authenticate user using username and password")
 
-        if not request.is_json:
-            log.warning('Authentication failed because no JSON body was '
-                        'provided!')
-            return {"msg": "Missing JSON in request"}, HTTPStatus.BAD_REQUEST
+        body = request.get_json()
+        # validate request body
+        errors = user_token_input_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         # Check JSON body
-        username = request.json.get('username', None)
-        password = request.json.get('password', None)
-        if not username and password:
-            msg = "Username and/or password missing in JSON body"
-            log.error(msg)
-            return {"msg": msg}, HTTPStatus.BAD_REQUEST
+        username = body.get('username')
+        password = body.get('password')
 
         user, code = user_login(self.config, username, password, self.mail)
         if code != HTTPStatus.OK:  # login failed
             log.error(f"Failed to login for user='{username}'")
             return user, code
 
         is_mfa_enabled = self.config.get('two_factor_auth', False)
@@ -146,15 +154,15 @@
             if user.otp_secret is None:
                 # server requires mfa but user hasn't set it up yet. Return
                 # an URI to generate a QR code
                 log.info(f'Redirecting user {username} to setup MFA')
                 return create_qr_uri(user), HTTPStatus.OK
             else:
                 # 2nd authentication factor: check the OTP secret of the user
-                mfa_code = request.json.get('mfa_code')
+                mfa_code = body.get('mfa_code')
                 if not mfa_code:
                     # note: this is not treated as error, but simply guide
                     # user to also fill in second factor
                     return {"msg": "Please include your two-factor "
                             "authentication code"}, HTTPStatus.OK
                 elif not self.validate_2fa_token(user, mfa_code):
                     return {
@@ -164,23 +172,23 @@
 
         token = _get_token_dict(user, self.api)
 
         log.info(f"Succesfull login from {username}")
         return token, HTTPStatus.OK, {'jwt-token': token['access_token']}
 
     @staticmethod
-    def validate_2fa_token(user: User, mfa_code: Union[int, str]) -> bool:
+    def validate_2fa_token(user: User, mfa_code: int | str) -> bool:
         """
         Check whether the 6-digit two-factor authentication code is valid
 
         Parameters
         ----------
         user: User
             The SQLAlchemy model of the user who is authenticating
-        mfa_code:
+        mfa_code: int | str
             A six-digit TOTP code from an authenticator app
 
         Returns
         -------
         bool
           Whether six-digit code is valid or not
         """
@@ -215,28 +223,24 @@
           401:
             description: Invalid API key
 
         tags: ["Authentication"]
         """
         log.debug("Authenticate Node using api key")
 
-        if not request.is_json:
-            log.warning('Authentication failed because no JSON body was '
-                        'provided!')
-            return {"msg": "Missing JSON in request"}, HTTPStatus.BAD_REQUEST
+        body = request.get_json()
+        # validate request body
+        errors = node_token_input_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         # Check JSON body
-        api_key = request.json.get('api_key', None)
-        if not api_key:
-            msg = "api_key missing in JSON body"
-            log.error(msg)
-            return {"msg": msg}, HTTPStatus.BAD_REQUEST
-
+        api_key = request.json.get('api_key')
         node = db.Node.get_by_api_key(api_key)
-
         if not node:  # login failed
             log.error("Api key is not recognized")
             return {"msg": "Api key is not recognized!"}, \
                 HTTPStatus.UNAUTHORIZED
 
         token = _get_token_dict(node, self.api)
 
@@ -269,18 +273,23 @@
           401:
             description: Key request for invalid image or task
 
         tags: ["Authentication"]
         """
         log.debug("Creating a token for a container running on a node")
 
-        data = request.get_json()
+        body = request.get_json()
+        # validate request body
+        errors = algorithm_token_input_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
-        task_id = data.get("task_id")
-        claim_image = data.get("image")
+        task_id = body.get("task_id")
+        claim_image = body.get("image")
 
         db_task = db.Task.get(task_id)
         if not db_task:
             log.warning(f"Node {g.node.id} attempts to generate key for task "
                         f"{task_id} that does not exist")
             return {"msg": "Master task does not exist!"}, \
                 HTTPStatus.BAD_REQUEST
@@ -302,29 +311,29 @@
                 f" which is outside its collaboration "
                 f"({g.node.collaboration_id}/{db_task.collaboration_id})."
             )
             return {"msg": "You are not within the collaboration"}, \
                 HTTPStatus.UNAUTHORIZED
 
         # validate that the task not has been finished yet
-        if db_task.complete:
+        if has_task_finished(db_task.status):
             log.warning(f"Node {g.node.id} attempts to generate a key for "
                         f"completed task {task_id}")
             return {"msg": "Task is already finished!"}, HTTPStatus.BAD_REQUEST
 
         # container identity consists of its node_id,
         # task_id, collaboration_id and image_id
         container = {
             "client_type": "container",
             "node_id": g.node.id,
             "organization_id": g.node.organization_id,
             "collaboration_id": g.node.collaboration_id,
             "task_id": task_id,
             "image": claim_image,
-            "database": db_task.database
+            "databases": [db_entry.database for db_entry in db_task.databases]
         }
         token = create_access_token(container, expires_delta=False)
 
         return {'container_token': token}, HTTPStatus.OK
 
 
 class RefreshToken(ServicesResources):
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/user.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: utf-8 -*-
 import logging
 import sqlalchemy.exc
 
 from http import HTTPStatus
 from flask import g, request
-from flask_restful import reqparse, Api
+from flask_restful import Api
 
 from vantage6.common import logger_name
 from vantage6.server import db
 from vantage6.server.permission import (
     Scope as S,
     Operation as P,
-    PermissionManager
+    PermissionManager,
+    RuleCollection
 )
 from vantage6.server.resource import (
+    get_org_ids_from_collabs,
     with_user,
     ServicesResources
 )
-from vantage6.server.resource.pagination import Pagination
-from vantage6.server.resource.common._schema import UserSchema
+from vantage6.server.resource.common.input_schema import UserInputSchema
+from vantage6.server.resource.common.pagination import Pagination
+from vantage6.server.resource.common.output_schema import UserSchema
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
@@ -68,45 +71,53 @@
     ----------
     permissions : PermissionManager
         Permission manager instance to which permissions are added
     """
     add = permissions.appender(module_name)
     add(S.GLOBAL, P.VIEW,
         description='View any user')
+    add(S.COLLABORATION, P.VIEW,
+        description='View users from your collaboration')
     add(S.ORGANIZATION, P.VIEW,
         description='View users from your organization')
     add(S.GLOBAL, P.CREATE,
         description='Create a new user for any organization')
+    add(S.COLLABORATION, P.CREATE,
+        description='Create a new user for organizations in your '
+                    'collaborations')
     add(S.ORGANIZATION, P.CREATE,
         description='Create a new user for your organization')
-    add(S.GLOBAL, P.EDIT,
-        description='Edit any user')
+    add(S.GLOBAL, P.EDIT, description='Edit any user')
+    add(S.COLLABORATION, P.EDIT,
+        description='Edit any user in your collaborations')
     add(S.ORGANIZATION, P.EDIT,
         description='Edit users from your organization')
     add(S.OWN, P.EDIT,
         description='Edit your own info')
-    add(S.GLOBAL, P.DELETE,
-        description='Delete any user')
+    add(S.GLOBAL, P.DELETE, description='Delete any user')
+    add(S.COLLABORATION, P.DELETE,
+        description='Delete any user in your collaborations')
     add(S.ORGANIZATION, P.DELETE,
         description='Delete users from your organization')
     add(S.OWN, P.DELETE,
         description='Delete your own account')
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 user_schema = UserSchema()
+user_input_schema = UserInputSchema()
 
 
 class UserBase(ServicesResources):
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
+        self.r: RuleCollection = getattr(self.permissions, module_name)
 
 
 class Users(UserBase):
 
     @with_user
     def get(self):
         """List users
@@ -115,14 +126,16 @@
             Returns a list of users that you are allowed to see.
 
             ### Permission Table\n
             |Rule name|Scope|Operation|Assigned to node|Assigned to container|
             Description|\n
             |--|--|--|--|--|--|\n
             |User|Global|View|❌|❌|View any user details|\n
+            |User|Collaboration|View|❌|❌|View user details from your
+            collaborations|\n
             |User|Organization|View|❌|❌|View users from your organization|\n
 
             Accessible to users.
 
         parameters:
           - in: query
             name: username
@@ -135,14 +148,19 @@
               * underscore sign (_) represents one, single character
           - in: query
             name: organization_id
             schema:
               type: integer
             description: Organization id
           - in: query
+            name: collaboration_id
+            schema:
+              type: integer
+            description: Collaboration id
+          - in: query
             name: firstname
             schema:
               type: string
             description: >-
               Name to match with a LIKE operator. \n
               * The percent sign (%) represents zero, one, or multiple
               characters\n
@@ -182,73 +200,117 @@
             description: Show only users seen since this date
           - in: query
             name: last_seen_till
             schema:
               type: date (yyyy-mm-dd)
             description: Show only users last seen before this date
           - in: query
-            name: include
-            schema:
-              type: string
-            description: Include 'metadata' to get pagination metadata. Note
-              that this will put the actual data in an envelope.
-          - in: query
             name: page
             schema:
               type: integer
-            description: Page number for pagination
+            description: Page number for pagination (default=1)
           - in: query
             name: per_page
             schema:
               type: integer
-            description: Number of items per page
+            description: Number of items per page (default=10)
+          - in: query
+            name: sort
+            schema:
+              type: string
+            description: >-
+              Sort by one or more fields, separated by a comma. Use a minus
+              sign (-) in front of the field to sort in descending order.
 
         responses:
           200:
             description: Ok
           401:
             description: Unauthorized
+          400:
+            description: Invalid values provided for request parameters
 
         security:
             - bearerAuth: []
 
         tags: ["User"]
         """
         args = request.args
         q = g.session.query(db.User)
 
         # filter by any field of this endpoint
         for param in ['username', 'firstname', 'lastname', 'email']:
             if param in args:
                 q = q.filter(getattr(db.User, param).like(args[param]))
         if 'organization_id' in args:
+            if not self.r.can_for_org(P.VIEW, args['organization_id']):
+                return {
+                    'msg': 'You lack the permission view users from the '
+                    f'organization with id {args["organization_id"]}!'
+                }, HTTPStatus.UNAUTHORIZED
             q = q.filter(db.User.organization_id == args['organization_id'])
         if 'last_seen_till' in args:
             q = q.filter(db.User.last_seen <= args['last_seen_till'])
         if 'last_seen_from' in args:
             q = q.filter(db.User.last_seen >= args['last_seen_from'])
 
         # find users with a particulare role or rule assigned
         if 'role_id' in args:
+            role = db.Role.get(args['role_id'])
+            if not role:
+                return {
+                    'msg': f'Role with id={args["role_id"]} does not exist!'
+                }, HTTPStatus.BAD_REQUEST
+            elif not self.r.can_for_org(P.VIEW, role.organization_id):
+                return {
+                    'msg': 'You lack the permission view users from the '
+                    f'organization that role with id={role.organization_id} '
+                    'belongs to!'
+                }, HTTPStatus.UNAUTHORIZED
             q = q.join(db.Permission).join(db.Role)\
                  .filter(db.Role.id == args['role_id'])
+
         if 'rule_id' in args:
+            rule = db.Rule.query.get(args['rule_id'])
+            if not rule:
+                return {
+                    'msg': f'Rule with id={args["rule_id"]} does not exist!'
+                }, HTTPStatus.BAD_REQUEST
             q = q.join(db.UserPermission).join(db.Rule)\
                  .filter(db.Rule.id == args['rule_id'])
 
+        if 'collaboration_id' in args:
+            if not self.r.can_for_col(P.VIEW, args['collaboration_id']):
+                return {
+                    'msg': 'You lack the permission view all users from '
+                    f'collaboration {args["collaboration_id"]}!'
+                }, HTTPStatus.UNAUTHORIZED
+            q = q.filter(db.User.organization_id.in_(
+                get_org_ids_from_collabs(g.user, args['collaboration_id'])
+            ))
+
         # check permissions and apply filter if neccessary
         if not self.r.v_glo.can():
-            if self.r.v_org.can():
+            if self.r.v_col.can():
+                q = q.filter(db.User.organization_id.in_(
+                    [org.id
+                     for col in g.user.organization.collaborations
+                     for org in col.organizations]
+                ))
+            elif self.r.v_org.can():
                 q = q.filter(db.User.organization_id == g.user.organization_id)
             else:
                 return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
         # paginate results
-        page = Pagination.from_query(q, request)
+        try:
+            page = Pagination.from_query(query=q, request=request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         # model serialization
         return self.response(page, user_schema)
 
     @with_user
     def post(self):
         """Create user
@@ -257,14 +319,16 @@
           Creates new user from the request data to the users organization.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |User|Global|Create|❌|❌|Create a new user|\n
+          |User|Collaboration|Create|❌|❌|Create a new user for any
+          organization in your collaborations|\n
           |User|Organization|Create|❌|❌|Create a new user as part of your
           organization|\n
 
           Accessible to users.
 
         requestBody:
           content:
@@ -311,52 +375,43 @@
             description: Organization id does not exist
 
         security:
           - bearerAuth: []
 
         tags: ["User"]
         """
-        parser = reqparse.RequestParser()
-        parser.add_argument("username", type=str, required=True)
-        parser.add_argument("firstname", type=str, required=True)
-        parser.add_argument("lastname", type=str, required=True)
-        # TODO password should be send to the email, rather than setting it
-        parser.add_argument("password", type=str, required=True)
-        parser.add_argument("email", type=str, required=True)
-        parser.add_argument("organization_id", type=int, required=False,
-                            help="This is only used if you're root")
-        parser.add_argument("roles", type=int, action="append", required=False)
-        parser.add_argument("rules", type=int, action="append", required=False)
-        data = parser.parse_args()
+        data = request.get_json()
+        # validate request body
+        errors = user_input_schema.validate(data)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
         # check unique constraints
         if db.User.username_exists(data["username"]):
             return {"msg": "username already exists."}, HTTPStatus.BAD_REQUEST
 
         if db.User.exists("email", data["email"]):
             return {"msg": "email already exists."}, HTTPStatus.BAD_REQUEST
 
         # check if the organization has been provided, if this is the case the
         # user needs global permissions in case it is not their own
         organization_id = g.user.organization_id
-        if data['organization_id']:
+        if data.get('organization_id'):
             if data['organization_id'] != organization_id:
                 if self.r.c_glo.can():
                     # check if organization exists
                     org = db.Organization.get(data['organization_id'])
                     if not org:
                         return {'msg': "Organization does not exist."}, \
                             HTTPStatus.NOT_FOUND
-                else:  # not-root user cant create users for other organization
-                    return {'msg': 'You lack the permission to do that!'}, \
-                        HTTPStatus.UNAUTHORIZED
             organization_id = data['organization_id']
 
         # check that user is allowed to create users
-        if not (self.r.c_glo.can() or self.r.c_org.can()):
+        if not self.r.can_for_org(P.CREATE, organization_id):
             return {'msg': 'You lack the permission to do that!'}, \
                 HTTPStatus.UNAUTHORIZED
 
         # process the required roles. It is only possible to assign roles with
         # rules that you already have permission to. This way we ensure you can
         # never extend your power on your own.
         potential_roles = data.get("roles")
@@ -376,15 +431,15 @@
                             role_.organization.id != organization_id):
                         return {'msg': (
                             "You can't assign that role as the role belongs to"
                             " a different organization than the user."
                         )}, HTTPStatus.UNAUTHORIZED
 
         # You can only assign rules that you already have to others.
-        potential_rules = data["rules"]
+        potential_rules = data.get("rules")
         rules = []
         if potential_rules:
             rules = [db.Rule.get(rule) for rule in potential_rules
                      if db.Rule.get(rule)]
             denied = self.permissions.check_user_rules(rules)
             if denied:
                 return denied, HTTPStatus.UNAUTHORIZED
@@ -404,15 +459,15 @@
         # check if the password meets password criteria
         msg = user.set_password(data["password"])
         if msg:
             return {"msg": msg}, HTTPStatus.BAD_REQUEST
 
         user.save()
 
-        return user_schema.dump(user).data, HTTPStatus.CREATED
+        return user_schema.dump(user), HTTPStatus.CREATED
 
 
 class User(UserBase):
 
     @with_user
     def get(self, id):
         """Get user
@@ -421,14 +476,16 @@
             Returns the user specified by the id.\n
 
             ### Permission Table\n
             |Rule name|Scope|Operation|Assigned to node|Assigned to container|
             Description|\n
             |-- |--|--|--|--|--|\n
             |User|Global|View|❌|❌|View any user details|\n
+            |User|Collaboration|View|❌|❌|View users from your
+            collaborations|\n
             |User|Organization|View|❌|❌|View users from your
             organization|\n
             |User|Organization|Own|❌|❌|View details about your own user|\n
 
             Accessible to users.
 
         parameters:
@@ -453,26 +510,20 @@
         tags: ["User"]
         """
         user = db.User.get(id)
         if not user:
             return {"msg": f"user id={id} is not found"}, HTTPStatus.NOT_FOUND
 
         same_user = g.user.id == user.id
-        same_org = g.user.organization.id == user.organization_id
 
-        # allow user to be returned if:
-        # 1. auth can see all users
-        # 2. auth can see organization users and user is within organization
-        # 3. auth is requesting own user details
-        if (
-            self.r.v_glo.can() or
-            (self.r.v_org.can() and same_org) or
-            same_user
-        ):
-            return user_schema.dump(user, many=False).data, HTTPStatus.OK
+        # allow user to be returned if authenticated user can view users from
+        # that organization or if the user is the same as the authenticated
+        # user.
+        if (same_user or self.r.can_for_org(P.VIEW, user.organization_id)):
+            return user_schema.dump(user, many=False), HTTPStatus.OK
         else:
             return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
     @with_user
     def patch(self, id):
         """Update user
@@ -481,15 +532,16 @@
           Update user information.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |User|Global|Edit|❌|❌|Edit any user|\n
-          |User|Organization|Edit|❌|❌|Edit any user in your organization|\n
+          |User|Collaboration|Edit|❌|❌|Edit users in your collaborations|\n
+          |User|Organization|Edit|❌|❌|Edit users in your organization|\n
           |User|Own|Edit|❌|❌|Edit your own user account|\n
 
           Accessible to users.
 
         requestBody:
           content:
             application/json:
@@ -539,79 +591,63 @@
 
         security:
           - bearerAuth: []
 
         tags: ["User"]
         """
         user = db.User.get(id)
-
         if not user:
             return {"msg": f"user id={id} not found"}, \
                 HTTPStatus.NOT_FOUND
 
-        if not self.r.e_glo.can():
-            if not (self.r.e_org.can() and user.organization ==
-                    g.user.organization):
-                if not (self.r.e_own.can() and user == g.user):
-                    return {'msg': 'You lack the permission to do that!'}, \
-                        HTTPStatus.UNAUTHORIZED
-
-        parser = reqparse.RequestParser()
-        parser.add_argument("username", type=str, required=False)
-        parser.add_argument("firstname", type=str, required=False)
-        parser.add_argument("lastname", type=str, required=False)
-        parser.add_argument("email", type=str, required=False)
-        data = parser.parse_args()
-
-        # check if user defined a password, which is deprecated
-        # FIXME BvB 22-06-29: with time, this check may be removed. Now it is
-        # here for backwards compatibility (if people have scripts using this,
-        # this makes them aware something changed)
-        request_json = request.get_json()
-        if request_json.get("password"):
+        data = request.get_json()
+        # validate request body
+        errors = user_input_schema.validate(data, partial=True)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+        if data.get("password"):
             return {"msg": "You cannot change your password here!"}, \
                 HTTPStatus.BAD_REQUEST
 
-        if data["username"] is not None:
-            if data["username"] == '':
-                return {
-                    "msg": "Empty username is not allowed!"
-                }, HTTPStatus.BAD_REQUEST
-            elif user.username != data["username"]:
+        # check permissions
+        if not (self.r.e_own.can() and user == g.user) and \
+                not self.r.can_for_org(P.EDIT, user.organization_id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
+
+        # update user and check for unique constraints
+        if data.get("username") is not None:
+            if user.username != data["username"]:
                 if db.User.exists("username", data["username"]):
                     return {
                         "msg": "User with that username already exists"
                     }, HTTPStatus.BAD_REQUEST
                 elif user.id != g.user.id:
                     return {
                         "msg": "You cannot change the username of another user"
                     }, HTTPStatus.BAD_REQUEST
             user.username = data["username"]
-        if data["firstname"] is not None:
+        if data.get("firstname") is not None:
             user.firstname = data["firstname"]
-        if data["lastname"] is not None:
+        if data.get("lastname") is not None:
             user.lastname = data["lastname"]
-        if data["email"] is not None:
-            if data["email"] == '':
-                return {
-                    "msg": "Empty email is not allowed!"
-                }, HTTPStatus.BAD_REQUEST
-            elif (user.email != data["email"] and
+        if data.get("email") is not None:
+            if (user.email != data["email"] and
                     db.User.exists("email", data["email"])):
                 return {
                     "msg": "User with that email already exists."
                 }, HTTPStatus.BAD_REQUEST
             user.email = data["email"]
 
         # request parser is awefull with lists
-        json_data = request.get_json()
-        if 'roles' in json_data:
+        if 'roles' in data:
             # validate that these roles exist
             roles = []
-            for role_id in json_data['roles']:
+            for role_id in data['roles']:
                 role = db.Role.get(role_id)
                 if not role:
                     return {'msg': f'Role={role_id} can not be found!'}, \
                         HTTPStatus.NOT_FOUND
                 roles.append(role)
 
             # validate that user is not changing their own roles
@@ -645,18 +681,18 @@
                         "this user but that is not allowed because they have "
                         f"permissions you don't have: {denied['msg']} (and "
                         "they do!)"
                     )}, HTTPStatus.UNAUTHORIZED
 
             user.roles = roles
 
-        if 'rules' in json_data:
+        if 'rules' in data:
             # validate that these rules exist
             rules = []
-            for rule_id in json_data['rules']:
+            for rule_id in data['rules']:
                 rule = db.Rule.get(rule_id)
                 if not rule:
                     return {'msg': f'Rule={rule_id} can not be found!'}, \
                         HTTPStatus.NOT_FOUND
                 rules.append(rule)
 
             # validate that user is not changing their own rules
@@ -685,43 +721,50 @@
             user.save()
         except sqlalchemy.exc.IntegrityError as e:
             log.error(e)
             user.session.rollback()
             return {
                 "msg": "User could not be updated with those parameters."
             }, HTTPStatus.BAD_REQUEST
-            # TODO BvB 2021-08-27 return msg that user was not updated?
 
-        return user_schema.dump(user).data, HTTPStatus.OK
+        return user_schema.dump(user), HTTPStatus.OK
 
     @with_user
     def delete(self, id):
         """Remove user.
         ---
         description: >-
           Delete a user account permanently.\n
 
           ### Permission Table\n
           |Rule name|Scope|Operation|Assigned to node|Assigned to container|
           Description|\n
           |--|--|--|--|--|--|\n
           |User|Global|Delete|❌|❌|Delete any user|\n
+          |User|Collaboration|Delete|❌|❌|Delete users from your
+          collaboration|\n
           |User|Organization|Delete|❌|❌|Delete users from your
           organization|\n
           |User|Own|Delete|❌|❌|Delete your own account|\n
 
           Accessible to users.
 
         parameters:
           - in: path
             name: id
             schema:
               type: integer
             description: User id
             required: true
+          - in: query
+            name: delete_dependents
+            schema:
+              type: boolean
+            description: If set to true, the user will be deleted along with
+              all tasks they created (default=False)
 
         responses:
           200:
             description: Ok
           404:
             description: User not found
           401:
@@ -733,18 +776,32 @@
         tags: ["User"]
         """
         user = db.User.get(id)
         if not user:
             return {"msg": f"user id={id} not found"}, \
                 HTTPStatus.NOT_FOUND
 
-        if not self.r.d_glo.can():
-            if not (self.r.d_org.can() and user.organization ==
-                    g.user.organization):
-                if not (self.r.d_own.can() and user == g.user):
-                    return {'msg': 'You lack the permission to do that!'}, \
-                        HTTPStatus.UNAUTHORIZED
+        if not (self.r.d_own.can() and user == g.user) and \
+                not self.r.can_for_org(P.DELETE, user.organization_id):
+            return {'msg': 'You lack the permission to do that!'}, \
+                HTTPStatus.UNAUTHORIZED
+
+        # check if user created any tasks
+        if user.created_tasks:
+            params = request.args
+            if not params.get('delete_dependents', False):
+                return {
+                    "msg": f"User has created {len(user.created_tasks)} tasks."
+                    " Please delete those first, or set the "
+                    "`delete_dependents` parameter to true to delete them "
+                    "automatically together with this user."
+                }, HTTPStatus.BAD_REQUEST
+            else:
+                log.warn(f"Deleting {len(user.created_tasks)} tasks created by"
+                         f" user id={id}")
+                for task in user.created_tasks:
+                    task.delete()
 
         user.delete()
         log.info(f"user id={id} is removed from the database")
         return {"msg": f"user id={id} is removed from the database"}, \
             HTTPStatus.OK
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/version.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/vpn.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/vpn.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from flask import request
 from flask_restful import Api
 import requests
 from requests_oauthlib import OAuth2Session
 
 from vantage6.common import logger_name
 from vantage6.server.resource import with_node, ServicesResources
+from vantage6.server.resource.common.input_schema import (
+    VPNConfigUpdateInputSchema
+)
 from vantage6.server.exceptions import (
     VPNConfigException, VPNPortalAuthException
 )
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
@@ -54,14 +57,17 @@
         path + '/update',
         endpoint='vpn_config_update',
         methods=('POST',),
         resource_class_kwargs=services
     )
 
 
+vpn_config_schema = VPNConfigUpdateInputSchema()
+
+
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 class VPNConfig(ServicesResources):
 
     @with_node
     def get(self):
@@ -164,27 +170,29 @@
 
         security:
             - bearerAuth: []
 
         tags: ["VPN"]
 
         """
+        body = request.get_json()
+
+        # validate request body
+        errors = vpn_config_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
         # check if the VPN server is configured
         if not self._is_server_configured():
             return {'msg': 'This server does not support VPN'}, \
                 HTTPStatus.NOT_IMPLEMENTED
 
-        # retrieve user based on email or username
-        body = request.get_json()
-        vpn_config = body.get("vpn_config")
-        if not vpn_config:
-            return {"msg": "vpn_config is missing!"}, \
-                HTTPStatus.BAD_REQUEST
-
         # refresh keypair by calling EduVPN API
+        vpn_config = body.get("vpn_config")
         try:
             vpn_connector = EduVPNConnector(self.config['vpn_server'])
             ovpn_config = vpn_connector.refresh_keypair(vpn_config)
         except VPNPortalAuthException as e:
             log.error("Could not obtain VPN configuration file")
             log.error(e)
             return {
```

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/resource/websocket_test.py` & `vantage6-server-4.0.0a2/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc4/vantage6/server/websockets.py` & `vantage6-server-4.0.0a2/vantage6/server/websockets.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,26 +125,26 @@
         Parameters
         ----------
         user: Authenticatable
             User that is to be added to the rooms
         """
         # check for which collab rooms the user has permission to enter
         session.user = db.User.get(session.auth_id)
-        if session.user.can('event', Scope.GLOBAL, Operation.VIEW):
+        if session.user.can('event', Scope.GLOBAL, Operation.RECEIVE):
             # user joins all collaboration rooms
             collabs = db.Collaboration.get()
             for collab in collabs:
                 session.rooms.append(f'collaboration_{collab.id}')
         elif session.user.can(
-                'event', Scope.COLLABORATION, Operation.VIEW):
+                'event', Scope.COLLABORATION, Operation.RECEIVE):
             # user joins all collaboration rooms that their organization
             # participates in
             for collab in user.organization.collaborations:
                 session.rooms.append(f'collaboration_{collab.id}')
-        elif session.user.can('event', Scope.ORGANIZATION, Operation.VIEW):
+        elif session.user.can('event', Scope.ORGANIZATION, Operation.RECEIVE):
             # user joins collaboration subrooms that include only messages
             # relevant to their own node
             for collab in user.organization.collaborations:
                 session.rooms.append(
                     f'collaboration_{collab.id}_organization_'
                     f'{user.organization.id}'
                 )
@@ -153,14 +153,18 @@
         """
         Client that disconnects is removed from all rooms they were in.
 
         If nodes disconnect, their status is also set to offline and users may
         be alerted to that. Also, any information on the node (e.g.
         configuration) is removed from the database.
         """
+        if not self.__is_identified_client():
+            self.log.debug('Client disconnected before identification')
+            return
+
         for room in session.rooms:
             # self.__leave_room_and_notify(room)
             self.__leave_room_and_notify(room)
 
         auth = db.Authenticatable.get(session.auth_id)
         auth.status = 'offline'
         auth.save()
@@ -229,39 +233,39 @@
         """
         # only allow nodes to send this event
         if session.type != 'node':
             self.log.warn('Only nodes can send algorithm status changes! '
                           f'{session.type} {session.auth_id} is not allowed.')
             return
 
-        result_id = data.get('result_id')
+        run_id = data.get('run_id')
         task_id = data.get('task_id')
         collaboration_id = data.get('collaboration_id')
         status = data.get('status')
         node_id = data.get('node_id')
         organization_id = data.get('organization_id')
         parent_id = data.get('parent_id')
 
-        run_id = db.Result.get(result_id).task.run_id
+        job_id = db.Run.get(run_id).task.job_id
 
         # log event in server logs
-        msg = (f"A container for run_id={run_id} and result_id={result_id} "
+        msg = (f"A container for job_id={job_id} and run_id={run_id} "
                f"in collaboration_id={collaboration_id} on node_id={node_id}")
         if has_task_failed(status):
             self.log.critical(f"{msg} exited with status={status}.")
         else:
             self.log.info(f"{msg} has a new status={status}.")
 
         # emit task status change to other nodes/users in the collaboration
         emit(
             "algorithm_status_change", {
                 "status": status,
-                "result_id": result_id,
-                "task_id": task_id,
                 "run_id": run_id,
+                "task_id": task_id,
+                "job_id": job_id,
                 "collaboration_id": collaboration_id,
                 "node_id": node_id,
                 "organization_id": organization_id,
                 "parent_id": parent_id,
             }, room=f"collaboration_{collaboration_id}"
         )
 
@@ -290,21 +294,27 @@
         # failed)
         self.__clean_node_data(node=node)
 
         # store (new) node config
         to_store = []
         for k, v in node_config.items():
             # add single item or list of items
-            if not isinstance(v, list):
-                to_store.append(db.NodeConfig(node_id=node.id, key=k, value=v))
-            else:
+            if isinstance(v, list):
                 to_store.extend([
                     db.NodeConfig(node_id=node.id, key=k, value=i)
                     for i in v
                 ])
+            elif isinstance(v, dict):
+                to_store.extend([
+                    db.NodeConfig(node_id=node.id, key=inner_key,
+                                  value=inner_val)
+                    for inner_key, inner_val in v.items()
+                ])
+            else:
+                to_store.append(db.NodeConfig(node_id=node.id, key=k, value=v))
 
         node.config = to_store
         node.save()
 
         # cleanup (e.g. database session)
         self.__cleanup()
 
@@ -379,14 +389,26 @@
                     'org_id': node.organization.id
                 },
                 namespace='/tasks',
                 room=room
             )
 
     @staticmethod
+    def __is_identified_client() -> bool:
+        """
+        Check if client has been identified as an authenticated user or node
+
+        Returns
+        -------
+        bool
+            True if client has been identified, False otherwise
+        """
+        return hasattr(session, 'auth_id')
+
+    @staticmethod
     def __clean_node_data(node: db.Node) -> None:
         """
         Remove any information from the database that the node shared about
         e.g. its configuration
 
         Parameters
         ----------
```

### Comparing `vantage6-server-3.9.0rc4/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-4.0.0a2/vantage6_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a2 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.9.0rc4/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-4.0.0a2/vantage6_server.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 vantage6/server/db.py
 vantage6/server/default_roles.py
 vantage6/server/exceptions.py
 vantage6/server/globals.py
 vantage6/server/mail_service.py
 vantage6/server/permission.py
 vantage6/server/session.py
+vantage6/server/utils.py
 vantage6/server/websockets.py
 vantage6/server/wsgi.py
 vantage6/server/_data/example_fixtures.yaml
-vantage6/server/_data/node_config_skeleton.yaml
-vantage6/server/_data/server_config_skeleton.yaml
-vantage6/server/_data/testnodeconfiguration.yaml
 vantage6/server/_data/unittest_config.yaml
 vantage6/server/_data/unittest_fixtures.yaml
 vantage6/server/_data/dev/fixtures.yaml
 vantage6/server/_data/dev/node_a.yaml
 vantage6/server/_data/dev/node_b.yaml
 vantage6/server/_data/dev/server.yaml
 vantage6/server/cli/__init__.py
@@ -35,41 +33,45 @@
 vantage6/server/model/base.py
 vantage6/server/model/collaboration.py
 vantage6/server/model/member.py
 vantage6/server/model/node.py
 vantage6/server/model/node_config.py
 vantage6/server/model/organization.py
 vantage6/server/model/permission.py
-vantage6/server/model/result.py
 vantage6/server/model/role.py
 vantage6/server/model/role_rule_association.py
 vantage6/server/model/rule.py
+vantage6/server/model/run.py
 vantage6/server/model/task.py
+vantage6/server/model/task_database.py
 vantage6/server/model/user.py
+vantage6/server/model/common/utils.py
 vantage6/server/resource/__init__.py
 vantage6/server/resource/collaboration.py
 vantage6/server/resource/event.py
 vantage6/server/resource/health.py
 vantage6/server/resource/node.py
 vantage6/server/resource/organization.py
-vantage6/server/resource/pagination.py
 vantage6/server/resource/port.py
 vantage6/server/resource/recover.py
 vantage6/server/resource/result.py
 vantage6/server/resource/role.py
 vantage6/server/resource/rule.py
+vantage6/server/resource/run.py
 vantage6/server/resource/stats.py
 vantage6/server/resource/task.py
 vantage6/server/resource/token.py
 vantage6/server/resource/user.py
 vantage6/server/resource/version.py
 vantage6/server/resource/vpn.py
 vantage6/server/resource/websocket_test.py
-vantage6/server/resource/common/_schema.py
 vantage6/server/resource/common/auth_helper.py
+vantage6/server/resource/common/input_schema.py
+vantage6/server/resource/common/output_schema.py
+vantage6/server/resource/common/pagination.py
 vantage6/server/resource/common/swagger_templates.py
 vantage6_server.egg-info/PKG-INFO
 vantage6_server.egg-info/SOURCES.txt
 vantage6_server.egg-info/dependency_links.txt
 vantage6_server.egg-info/entry_points.txt
 vantage6_server.egg-info/requires.txt
 vantage6_server.egg-info/top_level.txt
```

