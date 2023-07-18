# Comparing `tmp/pulumiverse_harbor-3.9.3.tar.gz` & `tmp/pulumiverse_harbor-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_harbor-3.9.3.tar", last modified: Sun Jul  2 08:26:58 2023, max compression
+gzip compressed data, was "pulumiverse_harbor-3.9.4.tar", last modified: Tue Jul 18 11:46:31 2023, max compression
```

## Comparing `pulumiverse_harbor-3.9.3.tar` & `pulumiverse_harbor-3.9.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.426092 pulumiverse_harbor-3.9.3/pulumiverse_harbor/
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    45640 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15274 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/immutable_tag_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/interrogation_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28683 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22644 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/purge_audit_log.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/retention_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/robot_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:46:31.075632 pulumiverse_harbor-3.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-18 11:46:31.075632 pulumiverse_harbor-3.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:46:31.075632 pulumiverse_harbor-3.9.4/pulumiverse_harbor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:46:31.075632 pulumiverse_harbor-3.9.4/pulumiverse_harbor/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45640 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15274 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/immutable_tag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/interrogation_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28683 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/project_member_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/project_member_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22777 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/project_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/purge_audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/retention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/robot_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:46:31.075632 pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-18 11:46:31.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-18 11:46:31.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:46:31.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:46:31.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 11:46:31.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 11:46:31.000000 pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:46:31.075632 pulumiverse_harbor-3.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-18 11:46:30.000000 pulumiverse_harbor-3.9.4/setup.py
```

### Comparing `pulumiverse_harbor-3.9.3/PKG-INFO` & `pulumiverse_harbor-3.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_harbor
-Version: 3.9.3
+Version: 3.9.4
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.9.3/README.md` & `pulumiverse_harbor-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/__init__.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/_inputs.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/_utilities.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/vars.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_auth.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_auth.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_email.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_email.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_security.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_security.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_system.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/config_system.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/garbage_collection.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/garbage_collection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_project.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_registry.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/group.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/immutable_tag_rule.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/immutable_tag_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/interrogation_services.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/interrogation_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/label.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/label.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/outputs.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_group.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/project_member_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_user.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/project_member_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_webhook.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/project_webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  skip_cert_verify: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ProjectWebhook resource.
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
-        :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
+        :param pulumi.Input[str] project_id: The project id (**/projects/ID**) of the harbor that webhook related to.
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
         """
         pulumi.set(__self__, "address", address)
@@ -86,15 +86,15 @@
     def notify_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "notify_type", value)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Input[str]:
         """
-        The project id of the harbor that webhook related to.
+        The project id (**/projects/ID**) of the harbor that webhook related to.
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "project_id", value)
 
@@ -176,15 +176,15 @@
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
-        :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
+        :param pulumi.Input[str] project_id: The project id (**/projects/ID**) of the harbor that webhook related to.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if auth_header is not None:
             pulumi.set(__self__, "auth_header", auth_header)
         if description is not None:
@@ -286,15 +286,15 @@
     def notify_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "notify_type", value)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The project id of the harbor that webhook related to.
+        The project id (**/projects/ID**) of the harbor that webhook related to.
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_id", value)
 
@@ -334,15 +334,15 @@
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
-        :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
+        :param pulumi.Input[str] project_id: The project id (**/projects/ID**) of the harbor that webhook related to.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectWebhookArgs,
@@ -429,15 +429,15 @@
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
         :param pulumi.Input[str] name: The name of the webhook that will be created in harbor.
         :param pulumi.Input[str] notify_type: The notification type either `http` or `slack`
-        :param pulumi.Input[str] project_id: The project id of the harbor that webhook related to.
+        :param pulumi.Input[str] project_id: The project id (**/projects/ID**) of the harbor that webhook related to.
         :param pulumi.Input[bool] skip_cert_verify: checks the for validate SSL certificate.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectWebhookState.__new__(_ProjectWebhookState)
 
         __props__.__dict__["address"] = address
@@ -507,15 +507,15 @@
         """
         return pulumi.get(self, "notify_type")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Output[str]:
         """
-        The project id of the harbor that webhook related to.
+        The project id (**/projects/ID**) of the harbor that webhook related to.
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter(name="skipCertVerify")
     def skip_cert_verify(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/provider.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/purge_audit_log.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/purge_audit_log.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/registry.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/replication.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/replication.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/retention_policy.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/retention_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/robot_account.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/robot_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/tasks.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/tasks.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor/user.py` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor/user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/PKG-INFO` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-harbor
-Version: 3.9.3
+Version: 3.9.4
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/SOURCES.txt` & `pulumiverse_harbor-3.9.4/pulumiverse_harbor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.3/setup.py` & `pulumiverse_harbor-3.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.3"
-PLUGIN_VERSION = "3.9.3"
+VERSION = "3.9.4"
+PLUGIN_VERSION = "3.9.4"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'harbor', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-harbor'])
         except OSError as error:
```

