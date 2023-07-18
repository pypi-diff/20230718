# Comparing `tmp/pierskarsenbarg_pulumi_sdm-1.2.0.tar.gz` & `tmp/pierskarsenbarg_pulumi_sdm-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.2.0.tar", last modified: Fri Jun 16 09:48:19 2023, max compression
+gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.3.0.tar", last modified: Tue Jul 18 13:47:17 2023, max compression
```

## Comparing `pierskarsenbarg_pulumi_sdm-1.2.0.tar` & `pierskarsenbarg_pulumi_sdm-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   599747 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   999495 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)   150822 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/secret_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:48:19.000000 pierskarsenbarg_pulumi_sdm-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-16 09:48:18.000000 pierskarsenbarg_pulumi_sdm-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   756526 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1293623 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154776 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/secret_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/setup.py
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg_pulumi_sdm
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/README.md` & `pierskarsenbarg_pulumi_sdm-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/__init__.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/_utilities.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/_utilities.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/account.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account.py`

 * *Files 22% similar despite different names*

```diff
@@ -102,14 +102,42 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  service: Optional[pulumi.Input[pulumi.InputType['AccountServiceArgs']]] = None,
                  user: Optional[pulumi.Input[pulumi.InputType['AccountUserArgs']]] = None,
                  __props__=None):
         """
+        Accounts are users that have access to strongDM. There are two types of accounts:
+         1. **Users:** humans who are authenticated through username and password or SSO.
+         2. **Service Accounts:** machines that are authenticated using a service token.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        test_user = sdm.Account("test-user", user=sdm.AccountUserArgs(
+            email="albob@strongdm.com",
+            first_name="al",
+            last_name="bob",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        test_service = sdm.Account("test-service", service=sdm.AccountServiceArgs(
+            name="test-service",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         Account can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/account:Account example a-12345678
         ```
@@ -123,14 +151,42 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AccountArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Accounts are users that have access to strongDM. There are two types of accounts:
+         1. **Users:** humans who are authenticated through username and password or SSO.
+         2. **Service Accounts:** machines that are authenticated using a service token.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        test_user = sdm.Account("test-user", user=sdm.AccountUserArgs(
+            email="albob@strongdm.com",
+            first_name="al",
+            last_name="bob",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        test_service = sdm.Account("test-service", service=sdm.AccountServiceArgs(
+            name="test-service",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         Account can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/account:Account example a-12345678
         ```
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account_attachment.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,14 +94,27 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_id: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        AccountAttachments assign an account to a role.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        test_account_attachment = sdm.AccountAttachment("testAccountAttachment",
+            account_id="a-00000054",
+            role_id="r-12355562")
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         AccountAttachment can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/accountAttachment:AccountAttachment example aa-12345678
         ```
@@ -114,14 +127,27 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AccountAttachmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        AccountAttachments assign an account to a role.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        test_account_attachment = sdm.AccountAttachment("testAccountAttachment",
+            account_id="a-00000054",
+            role_id="r-12355562")
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         AccountAttachment can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/accountAttachment:AccountAttachment example aa-12345678
         ```
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/config/vars.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/vars.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_account.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -212,25 +212,25 @@
     __args__['suspended'] = suspended
     __args__['tags'] = tags
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getAccount:getAccount', __args__, opts=opts, typ=GetAccountResult).value
 
     return AwaitableGetAccountResult(
-        accounts=__ret__.accounts,
-        email=__ret__.email,
-        external_id=__ret__.external_id,
-        first_name=__ret__.first_name,
-        id=__ret__.id,
-        ids=__ret__.ids,
-        last_name=__ret__.last_name,
-        name=__ret__.name,
-        suspended=__ret__.suspended,
-        tags=__ret__.tags,
-        type=__ret__.type)
+        accounts=pulumi.get(__ret__, 'accounts'),
+        email=pulumi.get(__ret__, 'email'),
+        external_id=pulumi.get(__ret__, 'external_id'),
+        first_name=pulumi.get(__ret__, 'first_name'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        last_name=pulumi.get(__ret__, 'last_name'),
+        name=pulumi.get(__ret__, 'name'),
+        suspended=pulumi.get(__ret__, 'suspended'),
+        tags=pulumi.get(__ret__, 'tags'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_account)
 def get_account_output(email: Optional[pulumi.Input[Optional[str]]] = None,
                        external_id: Optional[pulumi.Input[Optional[str]]] = None,
                        first_name: Optional[pulumi.Input[Optional[str]]] = None,
                        id: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,19 +117,19 @@
     __args__['accountId'] = account_id
     __args__['id'] = id
     __args__['roleId'] = role_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getAccountAttachment:getAccountAttachment', __args__, opts=opts, typ=GetAccountAttachmentResult).value
 
     return AwaitableGetAccountAttachmentResult(
-        account_attachments=__ret__.account_attachments,
-        account_id=__ret__.account_id,
-        id=__ret__.id,
-        ids=__ret__.ids,
-        role_id=__ret__.role_id)
+        account_attachments=pulumi.get(__ret__, 'account_attachments'),
+        account_id=pulumi.get(__ret__, 'account_id'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        role_id=pulumi.get(__ret__, 'role_id'))
 
 
 @_utilities.lift_output_func(get_account_attachment)
 def get_account_attachment_output(account_id: Optional[pulumi.Input[Optional[str]]] = None,
                                   id: Optional[pulumi.Input[Optional[str]]] = None,
                                   role_id: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAccountAttachmentResult]:
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_node.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,22 +167,22 @@
     __args__['name'] = name
     __args__['tags'] = tags
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getNode:getNode', __args__, opts=opts, typ=GetNodeResult).value
 
     return AwaitableGetNodeResult(
-        bind_address=__ret__.bind_address,
-        id=__ret__.id,
-        ids=__ret__.ids,
-        listen_address=__ret__.listen_address,
-        name=__ret__.name,
-        nodes=__ret__.nodes,
-        tags=__ret__.tags,
-        type=__ret__.type)
+        bind_address=pulumi.get(__ret__, 'bind_address'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        listen_address=pulumi.get(__ret__, 'listen_address'),
+        name=pulumi.get(__ret__, 'name'),
+        nodes=pulumi.get(__ret__, 'nodes'),
+        tags=pulumi.get(__ret__, 'tags'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_node)
 def get_node_output(bind_address: Optional[pulumi.Input[Optional[str]]] = None,
                     id: Optional[pulumi.Input[Optional[str]]] = None,
                     listen_address: Optional[pulumi.Input[Optional[str]]] = None,
                     name: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,20 +134,20 @@
     __args__['id'] = id
     __args__['remoteIdentityGroupId'] = remote_identity_group_id
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getRemoteIdentity:getRemoteIdentity', __args__, opts=opts, typ=GetRemoteIdentityResult).value
 
     return AwaitableGetRemoteIdentityResult(
-        account_id=__ret__.account_id,
-        id=__ret__.id,
-        ids=__ret__.ids,
-        remote_identities=__ret__.remote_identities,
-        remote_identity_group_id=__ret__.remote_identity_group_id,
-        username=__ret__.username)
+        account_id=pulumi.get(__ret__, 'account_id'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        remote_identities=pulumi.get(__ret__, 'remote_identities'),
+        remote_identity_group_id=pulumi.get(__ret__, 'remote_identity_group_id'),
+        username=pulumi.get(__ret__, 'username'))
 
 
 @_utilities.lift_output_func(get_remote_identity)
 def get_remote_identity_output(account_id: Optional[pulumi.Input[Optional[str]]] = None,
                                id: Optional[pulumi.Input[Optional[str]]] = None,
                                remote_identity_group_id: Optional[pulumi.Input[Optional[str]]] = None,
                                username: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,18 +102,18 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getRemoteIdentityGroup:getRemoteIdentityGroup', __args__, opts=opts, typ=GetRemoteIdentityGroupResult).value
 
     return AwaitableGetRemoteIdentityGroupResult(
-        id=__ret__.id,
-        ids=__ret__.ids,
-        name=__ret__.name,
-        remote_identity_groups=__ret__.remote_identity_groups)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        name=pulumi.get(__ret__, 'name'),
+        remote_identity_groups=pulumi.get(__ret__, 'remote_identity_groups'))
 
 
 @_utilities.lift_output_func(get_remote_identity_group)
 def get_remote_identity_group_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                                      name: Optional[pulumi.Input[Optional[str]]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRemoteIdentityGroupResult]:
     """
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_resource.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         if username and not isinstance(username, str):
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -79,14 +82,17 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def resources(self) -> Sequence['outputs.GetResourceResourceResult']:
         """
         A single element list containing a map, where each key lists one of the following objects:
@@ -106,14 +112,17 @@
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 class AwaitableGetResourceResult(GetResourceResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -152,40 +161,43 @@
             "env": "dev",
             "region": "us-west",
         },
         type="mysql")
     ```
 
 
+    :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
     :param str id: Unique identifier of the Resource.
     :param str name: Unique human-readable name of the Resource.
+    :param int port: The port to dial to initiate a connection from the egress node to this resource.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
     :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str username: The username to authenticate with.
     """
     __args__ = dict()
     __args__['hostname'] = hostname
     __args__['id'] = id
     __args__['name'] = name
     __args__['port'] = port
     __args__['tags'] = tags
     __args__['type'] = type
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getResource:getResource', __args__, opts=opts, typ=GetResourceResult).value
 
     return AwaitableGetResourceResult(
-        hostname=__ret__.hostname,
-        id=__ret__.id,
-        ids=__ret__.ids,
-        name=__ret__.name,
-        port=__ret__.port,
-        resources=__ret__.resources,
-        tags=__ret__.tags,
-        type=__ret__.type,
-        username=__ret__.username)
+        hostname=pulumi.get(__ret__, 'hostname'),
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        name=pulumi.get(__ret__, 'name'),
+        port=pulumi.get(__ret__, 'port'),
+        resources=pulumi.get(__ret__, 'resources'),
+        tags=pulumi.get(__ret__, 'tags'),
+        type=pulumi.get(__ret__, 'type'),
+        username=pulumi.get(__ret__, 'username'))
 
 
 @_utilities.lift_output_func(get_resource)
 def get_resource_output(hostname: Optional[pulumi.Input[Optional[str]]] = None,
                         id: Optional[pulumi.Input[Optional[str]]] = None,
                         name: Optional[pulumi.Input[Optional[str]]] = None,
                         port: Optional[pulumi.Input[Optional[int]]] = None,
@@ -207,13 +219,16 @@
             "env": "dev",
             "region": "us-west",
         },
         type="mysql")
     ```
 
 
+    :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
     :param str id: Unique identifier of the Resource.
     :param str name: Unique human-readable name of the Resource.
+    :param int port: The port to dial to initiate a connection from the egress node to this resource.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
     :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
+    :param str username: The username to authenticate with.
     """
     ...
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_role.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_role.py`

 * *Files 15% similar despite different names*

```diff
@@ -123,20 +123,20 @@
     __args__['id'] = id
     __args__['name'] = name
     __args__['tags'] = tags
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getRole:getRole', __args__, opts=opts, typ=GetRoleResult).value
 
     return AwaitableGetRoleResult(
-        id=__ret__.id,
-        ids=__ret__.ids,
-        managed_by=__ret__.managed_by,
-        name=__ret__.name,
-        roles=__ret__.roles,
-        tags=__ret__.tags)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        managed_by=pulumi.get(__ret__, 'managed_by'),
+        name=pulumi.get(__ret__, 'name'),
+        roles=pulumi.get(__ret__, 'roles'),
+        tags=pulumi.get(__ret__, 'tags'))
 
 
 @_utilities.lift_output_func(get_role)
 def get_role_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                     name: Optional[pulumi.Input[Optional[str]]] = None,
                     tags: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleResult]:
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -123,20 +123,20 @@
     __args__['name'] = name
     __args__['tags'] = tags
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getSecretStore:getSecretStore', __args__, opts=opts, typ=GetSecretStoreResult).value
 
     return AwaitableGetSecretStoreResult(
-        id=__ret__.id,
-        ids=__ret__.ids,
-        name=__ret__.name,
-        secret_stores=__ret__.secret_stores,
-        tags=__ret__.tags,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        ids=pulumi.get(__ret__, 'ids'),
+        name=pulumi.get(__ret__, 'name'),
+        secret_stores=pulumi.get(__ret__, 'secret_stores'),
+        tags=pulumi.get(__ret__, 'tags'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_secret_store)
 def get_secret_store_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                             name: Optional[pulumi.Input[Optional[str]]] = None,
                             tags: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                             type: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,16 +77,16 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['publicKey'] = public_key
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getSshCaPubkey:getSshCaPubkey', __args__, opts=opts, typ=GetSshCaPubkeyResult).value
 
     return AwaitableGetSshCaPubkeyResult(
-        id=__ret__.id,
-        public_key=__ret__.public_key)
+        id=pulumi.get(__ret__, 'id'),
+        public_key=pulumi.get(__ret__, 'public_key'))
 
 
 @_utilities.lift_output_func(get_ssh_ca_pubkey)
 def get_ssh_ca_pubkey_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                              public_key: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSshCaPubkeyResult]:
     """
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/node.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/node.py`

 * *Files 16% similar despite different names*

```diff
@@ -98,14 +98,43 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  gateway: Optional[pulumi.Input[pulumi.InputType['NodeGatewayArgs']]] = None,
                  relay: Optional[pulumi.Input[pulumi.InputType['NodeRelayArgs']]] = None,
                  __props__=None):
         """
+        Nodes make up the strongDM network, and allow your users to connect securely to your resources.
+         There are two types of nodes:
+         1. **Relay:** creates connectivity to your datasources, while maintaining the egress-only nature of your firewall
+         2. **Gateways:** a relay that also listens for connections from strongDM clients
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        gateway = sdm.Node("gateway", gateway=sdm.NodeGatewayArgs(
+            bind_address="0.0.0.0:21222",
+            listen_address="165.23.40.1:21222",
+            name="test-gateway",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        relay = sdm.Node("relay", relay=sdm.NodeRelayArgs(
+            name="test-relay",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         Node can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/node:Node example n-12345678
         ```
@@ -118,14 +147,43 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[NodeArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Nodes make up the strongDM network, and allow your users to connect securely to your resources.
+         There are two types of nodes:
+         1. **Relay:** creates connectivity to your datasources, while maintaining the egress-only nature of your firewall
+         2. **Gateways:** a relay that also listens for connections from strongDM clients
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        gateway = sdm.Node("gateway", gateway=sdm.NodeGatewayArgs(
+            bind_address="0.0.0.0:21222",
+            listen_address="165.23.40.1:21222",
+            name="test-gateway",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        relay = sdm.Node("relay", relay=sdm.NodeRelayArgs(
+            name="test-relay",
+            tags={
+                "env": "dev",
+                "region": "us-west",
+            },
+        ))
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         Node can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/node:Node example n-12345678
         ```
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/outputs.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/outputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from . import _utilities
 from . import outputs
 
 __all__ = [
     'AccountService',
     'AccountUser',
     'NodeGateway',
+    'NodeGatewayMaintenanceWindow',
     'NodeRelay',
+    'NodeRelayMaintenanceWindow',
     'ResourceAks',
     'ResourceAksBasicAuth',
     'ResourceAksServiceAccount',
     'ResourceAksServiceAccountUserImpersonation',
     'ResourceAksUserImpersonation',
     'ResourceAmazonEks',
     'ResourceAmazonEksInstanceProfile',
@@ -32,14 +34,15 @@
     'ResourceAws',
     'ResourceAwsConsole',
     'ResourceAwsConsoleStaticKeyPair',
     'ResourceAzure',
     'ResourceAzureCertificate',
     'ResourceAzureMysql',
     'ResourceAzurePostgres',
+    'ResourceAzurePostgresManagedIdentity',
     'ResourceBigQuery',
     'ResourceCassandra',
     'ResourceCitus',
     'ResourceClustrix',
     'ResourceCockroach',
     'ResourceDb2I',
     'ResourceDb2Luw',
@@ -107,15 +110,17 @@
     'SecretStoreVaultToken',
     'GetAccountAccountResult',
     'GetAccountAccountServiceResult',
     'GetAccountAccountUserResult',
     'GetAccountAttachmentAccountAttachmentResult',
     'GetNodeNodeResult',
     'GetNodeNodeGatewayResult',
+    'GetNodeNodeGatewayMaintenanceWindowResult',
     'GetNodeNodeRelayResult',
+    'GetNodeNodeRelayMaintenanceWindowResult',
     'GetRemoteIdentityGroupRemoteIdentityGroupResult',
     'GetRemoteIdentityRemoteIdentityResult',
     'GetResourceResourceResult',
     'GetResourceResourceAkResult',
     'GetResourceResourceAksBasicAuthResult',
     'GetResourceResourceAksServiceAccountResult',
     'GetResourceResourceAksServiceAccountUserImpersonationResult',
@@ -132,14 +137,15 @@
     'GetResourceResourceAwResult',
     'GetResourceResourceAwsConsoleResult',
     'GetResourceResourceAwsConsoleStaticKeyPairResult',
     'GetResourceResourceAzureResult',
     'GetResourceResourceAzureCertificateResult',
     'GetResourceResourceAzureMysqlResult',
     'GetResourceResourceAzurePostgreResult',
+    'GetResourceResourceAzurePostgresManagedIdentityResult',
     'GetResourceResourceBigQueryResult',
     'GetResourceResourceCassandraResult',
     'GetResourceResourceCitusResult',
     'GetResourceResourceClustrixResult',
     'GetResourceResourceCockroachResult',
     'GetResourceResourceDb2IResult',
     'GetResourceResourceDb2LuwResult',
@@ -389,16 +395,20 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "listenAddress":
             suggest = "listen_address"
         elif key == "bindAddress":
             suggest = "bind_address"
+        elif key == "connectsTo":
+            suggest = "connects_to"
         elif key == "gatewayFilter":
             suggest = "gateway_filter"
+        elif key == "maintenanceWindows":
+            suggest = "maintenance_windows"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in NodeGateway. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         NodeGateway.__key_warning(key)
         return super().__getitem__(key)
@@ -406,40 +416,48 @@
     def get(self, key: str, default = None) -> Any:
         NodeGateway.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  listen_address: str,
                  bind_address: Optional[str] = None,
+                 connects_to: Optional[str] = None,
                  device: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  location: Optional[str] = None,
+                 maintenance_windows: Optional[Sequence['outputs.NodeGatewayMaintenanceWindow']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None,
                  version: Optional[str] = None):
         """
         :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
         :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
-        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
-        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
+        :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
+        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
+        :param Sequence['NodeGatewayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         pulumi.set(__self__, "listen_address", listen_address)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
+        if connects_to is not None:
+            pulumi.set(__self__, "connects_to", connects_to)
         if device is not None:
             pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if location is not None:
             pulumi.set(__self__, "location", location)
+        if maintenance_windows is not None:
+            pulumi.set(__self__, "maintenance_windows", maintenance_windows)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
         if version is not None:
@@ -458,38 +476,54 @@
     def bind_address(self) -> Optional[str]:
         """
         The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
         """
         return pulumi.get(self, "bind_address")
 
     @property
+    @pulumi.getter(name="connectsTo")
+    def connects_to(self) -> Optional[str]:
+        """
+        ConnectsTo can be used to restrict the peering between relays and gateways.
+        """
+        return pulumi.get(self, "connects_to")
+
+    @property
     @pulumi.getter
     def device(self) -> Optional[str]:
         """
-        Device is a read only device name uploaded by the gateway process when  it comes online.
+        Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
-        GatewayFilter can be used to restrict the peering between relays and gateways.
+        GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         """
         return pulumi.get(self, "gateway_filter")
 
     @property
     @pulumi.getter
     def location(self) -> Optional[str]:
         """
         Location is a read only network location uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "location")
 
     @property
+    @pulumi.getter(name="maintenanceWindows")
+    def maintenance_windows(self) -> Optional[Sequence['outputs.NodeGatewayMaintenanceWindow']]:
+        """
+        Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
+        """
+        return pulumi.get(self, "maintenance_windows")
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
@@ -512,88 +546,154 @@
         """
         Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "version")
 
 
 @pulumi.output_type
+class NodeGatewayMaintenanceWindow(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "cronSchedule":
+            suggest = "cron_schedule"
+        elif key == "requireIdleness":
+            suggest = "require_idleness"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in NodeGatewayMaintenanceWindow. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        NodeGatewayMaintenanceWindow.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        NodeGatewayMaintenanceWindow.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cron_schedule: str,
+                 require_idleness: bool):
+        pulumi.set(__self__, "cron_schedule", cron_schedule)
+        pulumi.set(__self__, "require_idleness", require_idleness)
+
+    @property
+    @pulumi.getter(name="cronSchedule")
+    def cron_schedule(self) -> str:
+        return pulumi.get(self, "cron_schedule")
+
+    @property
+    @pulumi.getter(name="requireIdleness")
+    def require_idleness(self) -> bool:
+        return pulumi.get(self, "require_idleness")
+
+
+@pulumi.output_type
 class NodeRelay(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "gatewayFilter":
+        if key == "connectsTo":
+            suggest = "connects_to"
+        elif key == "gatewayFilter":
             suggest = "gateway_filter"
+        elif key == "maintenanceWindows":
+            suggest = "maintenance_windows"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in NodeRelay. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         NodeRelay.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         NodeRelay.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
+                 connects_to: Optional[str] = None,
                  device: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  location: Optional[str] = None,
+                 maintenance_windows: Optional[Sequence['outputs.NodeRelayMaintenanceWindow']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None,
                  version: Optional[str] = None):
         """
-        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
-        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
+        :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
+        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
+        :param Sequence['NodeRelayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
+        if connects_to is not None:
+            pulumi.set(__self__, "connects_to", connects_to)
         if device is not None:
             pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if location is not None:
             pulumi.set(__self__, "location", location)
+        if maintenance_windows is not None:
+            pulumi.set(__self__, "maintenance_windows", maintenance_windows)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
+    @pulumi.getter(name="connectsTo")
+    def connects_to(self) -> Optional[str]:
+        """
+        ConnectsTo can be used to restrict the peering between relays and gateways.
+        """
+        return pulumi.get(self, "connects_to")
+
+    @property
     @pulumi.getter
     def device(self) -> Optional[str]:
         """
-        Device is a read only device name uploaded by the gateway process when  it comes online.
+        Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
-        GatewayFilter can be used to restrict the peering between relays and gateways.
+        GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         """
         return pulumi.get(self, "gateway_filter")
 
     @property
     @pulumi.getter
     def location(self) -> Optional[str]:
         """
         Location is a read only network location uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "location")
 
     @property
+    @pulumi.getter(name="maintenanceWindows")
+    def maintenance_windows(self) -> Optional[Sequence['outputs.NodeRelayMaintenanceWindow']]:
+        """
+        Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
+        """
+        return pulumi.get(self, "maintenance_windows")
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
@@ -616,14 +716,52 @@
         """
         Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "version")
 
 
 @pulumi.output_type
+class NodeRelayMaintenanceWindow(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "cronSchedule":
+            suggest = "cron_schedule"
+        elif key == "requireIdleness":
+            suggest = "require_idleness"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in NodeRelayMaintenanceWindow. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        NodeRelayMaintenanceWindow.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        NodeRelayMaintenanceWindow.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cron_schedule: str,
+                 require_idleness: bool):
+        pulumi.set(__self__, "cron_schedule", cron_schedule)
+        pulumi.set(__self__, "require_idleness", require_idleness)
+
+    @property
+    @pulumi.getter(name="cronSchedule")
+    def cron_schedule(self) -> str:
+        return pulumi.get(self, "cron_schedule")
+
+    @property
+    @pulumi.getter(name="requireIdleness")
+    def require_idleness(self) -> bool:
+        return pulumi.get(self, "require_idleness")
+
+
+@pulumi.output_type
 class ResourceAks(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bindInterface":
             suggest = "bind_interface"
         elif key == "certificateAuthority":
@@ -669,18 +807,26 @@
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
@@ -708,50 +854,65 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -765,24 +926,33 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -843,21 +1013,26 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -876,34 +1051,40 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -918,19 +1099,25 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -952,14 +1139,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceAksServiceAccount(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1001,22 +1191,28 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -1037,34 +1233,40 @@
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -1079,24 +1281,33 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -1119,14 +1330,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class ResourceAksServiceAccountUserImpersonation(dict):
@@ -1164,22 +1376,26 @@
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -1196,34 +1412,40 @@
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -1238,14 +1460,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -1268,14 +1493,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class ResourceAksUserImpersonation(dict):
@@ -1321,18 +1547,24 @@
                  egress_filter: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
@@ -1356,50 +1588,65 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -1413,14 +1660,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -1503,18 +1753,29 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str cluster_name: The name of the cluster to connect to.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str region: The AWS region to connect to.
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
@@ -1547,50 +1808,65 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> str:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -1604,39 +1880,57 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -1713,18 +2007,27 @@
                  remote_identity_healthcheck_username: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str cluster_name: The name of the cluster to connect to.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str region: The AWS region to connect to.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
@@ -1753,45 +2056,57 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> str:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -1805,34 +2120,49 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -1909,18 +2239,27 @@
                  remote_identity_healthcheck_username: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str cluster_name: The name of the cluster to connect to.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str region: The AWS region to connect to.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
@@ -1949,45 +2288,57 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> str:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -2001,34 +2352,49 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -2105,18 +2471,27 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str cluster_name: The name of the cluster to connect to.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str region: The AWS region to connect to.
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
@@ -2145,50 +2520,65 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> str:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -2202,29 +2592,41 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -2293,16 +2695,23 @@
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
-        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str region: The AWS region to connect to.
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
@@ -2335,60 +2744,81 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -2449,20 +2879,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -2482,53 +2918,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -2550,19 +2998,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceAthena(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2608,17 +3062,24 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str athena_output: The AWS S3 output location.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "athena_output", athena_output)
         pulumi.set(__self__, "name", name)
         if access_key is not None:
@@ -2643,68 +3104,89 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="athenaOutput")
     def athena_output(self) -> str:
+        """
+        The AWS S3 output location.
+        """
         return pulumi.get(self, "athena_output")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -2769,20 +3251,28 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -2805,63 +3295,81 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -2883,19 +3391,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceAuroraPostgres(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2933,20 +3447,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -2967,63 +3488,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -3045,14 +3584,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceAws(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3097,17 +3639,23 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str healthcheck_region: The AWS region healthcheck requests should attempt to connect to.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_region", healthcheck_region)
         pulumi.set(__self__, "name", name)
         if access_key is not None:
@@ -3130,63 +3678,81 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="healthcheckRegion")
     def healthcheck_region(self) -> str:
+        """
+        The AWS region healthcheck requests should attempt to connect to.
+        """
         return pulumi.get(self, "healthcheck_region")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -3260,18 +3826,26 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  session_expiry: Optional[int] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str region: The AWS region to connect to.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool enable_env_variables: If true, prefer environment variables to authenticate connection even if EC2 roles are configured.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param int session_expiry: The length of time in seconds AWS console sessions will live before needing to reauthenticate.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subdomain", subdomain)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -3303,81 +3877,105 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="enableEnvVariables")
     def enable_env_variables(self) -> Optional[bool]:
+        """
+        If true, prefer environment variables to authenticate connection even if EC2 roles are configured.
+        """
         return pulumi.get(self, "enable_env_variables")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="sessionExpiry")
     def session_expiry(self) -> Optional[int]:
+        """
+        The length of time in seconds AWS console sessions will live before needing to reauthenticate.
+        """
         return pulumi.get(self, "session_expiry")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -3438,18 +4036,27 @@
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  session_expiry: Optional[int] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str region: The AWS region to connect to.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param int session_expiry: The length of time in seconds AWS console sessions will live before needing to reauthenticate.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "subdomain", subdomain)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
@@ -3483,86 +4090,113 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="sessionExpiry")
     def session_expiry(self) -> Optional[int]:
+        """
+        The length of time in seconds AWS console sessions will live before needing to reauthenticate.
+        """
         return pulumi.get(self, "session_expiry")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -3608,20 +4242,24 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str app_id: The application ID to authenticate with.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * sql_server_kerberos_ad:
+        :param str tenant_id: The Azure AD directory (tenant) ID with which to authenticate.
+               * sql_server_kerberos_ad:
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -3646,40 +4284,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="appId")
     def app_id(self) -> Optional[str]:
+        """
+        The application ID to authenticate with.
+        """
         return pulumi.get(self, "app_id")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -3702,14 +4349,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
+        The Azure AD directory (tenant) ID with which to authenticate.
         * sql_server_kerberos_ad:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
 class ResourceAzureCertificate(dict):
@@ -3751,20 +4399,24 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str app_id: The application ID to authenticate with.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * sql_server_kerberos_ad:
+        :param str tenant_id: The Azure AD directory (tenant) ID with which to authenticate.
+               * sql_server_kerberos_ad:
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if client_certificate is not None:
@@ -3789,40 +4441,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="appId")
     def app_id(self) -> Optional[str]:
+        """
+        The application ID to authenticate with.
+        """
         return pulumi.get(self, "app_id")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -3845,14 +4506,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
+        The Azure AD directory (tenant) ID with which to authenticate.
         * sql_server_kerberos_ad:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
 class ResourceAzureMysql(dict):
@@ -3895,20 +4557,28 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -3931,63 +4601,81 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -4009,19 +4697,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceAzurePostgres(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4059,20 +4753,216 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
+        """
+        pulumi.set(__self__, "database", database)
+        pulumi.set(__self__, "hostname", hostname)
+        pulumi.set(__self__, "name", name)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if override_database is not None:
+            pulumi.set(__self__, "override_database", override_database)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
+        return pulumi.get(self, "database")
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter(name="overrideDatabase")
+    def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
+        return pulumi.get(self, "override_database")
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
+class ResourceAzurePostgresManagedIdentity(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "bindInterface":
+            suggest = "bind_interface"
+        elif key == "egressFilter":
+            suggest = "egress_filter"
+        elif key == "overrideDatabase":
+            suggest = "override_database"
+        elif key == "portOverride":
+            suggest = "port_override"
+        elif key == "secretStoreId":
+            suggest = "secret_store_id"
+        elif key == "useAzureSingleServerUsernames":
+            suggest = "use_azure_single_server_usernames"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ResourceAzurePostgresManagedIdentity. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ResourceAzurePostgresManagedIdentity.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ResourceAzurePostgresManagedIdentity.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 database: str,
+                 hostname: str,
+                 name: str,
+                 bind_interface: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 override_database: Optional[bool] = None,
+                 password: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 use_azure_single_server_usernames: Optional[bool] = None,
+                 username: Optional[str] = None):
+        """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -4087,69 +4977,89 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if use_azure_single_server_usernames is not None:
+            pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -4169,16 +5079,27 @@
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
+    @pulumi.getter(name="useAzureSingleServerUsernames")
+    def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
+        return pulumi.get(self, "use_azure_single_server_usernames")
+
+    @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceBigQuery(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4214,20 +5135,25 @@
                  port_override: Optional[int] = None,
                  private_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str project: The project to connect to.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str private_key: The private key used to authenticate with the server.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project", project)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -4244,53 +5170,65 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def project(self) -> str:
+        """
+        The project to connect to.
+        """
         return pulumi.get(self, "project")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> Optional[str]:
+        """
+        The private key used to authenticate with the server.
+        """
         return pulumi.get(self, "private_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -4312,14 +5250,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceCassandra(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4356,20 +5297,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -4389,53 +5336,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -4457,19 +5416,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceCitus(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4507,20 +5472,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -4541,63 +5513,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -4619,14 +5609,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceClustrix(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4667,20 +5660,28 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -4703,63 +5704,81 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -4781,19 +5800,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceCockroach(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4831,20 +5856,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -4865,63 +5897,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -4943,14 +5993,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceDb2I(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4987,20 +6040,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -5019,53 +6078,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -5087,19 +6158,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceDb2Luw(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5134,20 +6211,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -5166,58 +6249,73 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -5239,14 +6337,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceDocumentDbHost(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5283,20 +6384,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str auth_database: The authentication database to use.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -5315,58 +6422,73 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> str:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -5388,14 +6510,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceDocumentDbReplicaSet(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5437,20 +6562,27 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str auth_database: The authentication database to use.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str replica_set: The name of the mongo replicaset.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool connect_to_replica: Set to connect to a replica instead of the primary node.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5470,63 +6602,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> str:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> str:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="connectToReplica")
     def connect_to_replica(self) -> Optional[bool]:
+        """
+        Set to connect to a replica instead of the primary node.
+        """
         return pulumi.get(self, "connect_to_replica")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -5548,14 +6698,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceDruid(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5589,20 +6742,25 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -5620,53 +6778,65 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -5688,14 +6858,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceDynamoDb(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5739,17 +6912,24 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
-        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str region: The AWS region to connect to.
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
@@ -5773,68 +6953,89 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -5895,20 +7096,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -5928,53 +7135,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -5996,19 +7215,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceElasticacheRedis(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6045,20 +7270,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -6078,53 +7309,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -6146,19 +7389,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceGcp(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6191,16 +7440,19 @@
                  keyfile: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str scopes: Space separated scopes that this login should assume into when authenticating.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str keyfile: The service account keyfile to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "scopes", scopes)
         if bind_interface is not None:
@@ -6225,40 +7477,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def scopes(self) -> str:
+        """
+        Space separated scopes that this login should assume into when authenticating.
+        """
         return pulumi.get(self, "scopes")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def keyfile(self) -> Optional[str]:
+        """
+        The service account keyfile to authenticate with.
+        """
         return pulumi.get(self, "keyfile")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -6325,19 +7586,24 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -6359,35 +7625,41 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -6401,32 +7673,41 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
+        """
+        The service account key to authenticate with.
+        """
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -6479,19 +7760,22 @@
                  egress_filter: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -6509,35 +7793,41 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -6559,14 +7849,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
+        """
+        The service account key to authenticate with.
+        """
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -6620,20 +7913,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -6654,63 +7954,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -6732,14 +8050,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceHttpAuth(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6782,19 +8103,25 @@
                  default_path: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  headers_blacklist: Optional[str] = None,
                  host_override: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str healthcheck_path: This path will be used to check the health of your site.
         :param str name: Unique human-readable name of the Resource.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
-        :param str url: * kubernetes:
-        :param str bind_interface: Bind interface
+        :param str url: The base address of your website without the path.
+               * kubernetes:
+        :param str auth_header: The content to set as the authorization header.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str default_path: Automatically redirect to this path upon connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str headers_blacklist: Header names (e.g. Authorization), to omit from logs.
+        :param str host_override: The host header will be overwritten with this field if provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "subdomain", subdomain)
         pulumi.set(__self__, "url", url)
@@ -6814,14 +8141,17 @@
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="healthcheckPath")
     def healthcheck_path(self) -> str:
+        """
+        This path will be used to check the health of your site.
+        """
         return pulumi.get(self, "healthcheck_path")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
@@ -6836,52 +8166,65 @@
         """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def url(self) -> str:
         """
+        The base address of your website without the path.
         * kubernetes:
         """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter(name="authHeader")
     def auth_header(self) -> Optional[str]:
+        """
+        The content to set as the authorization header.
+        """
         return pulumi.get(self, "auth_header")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="defaultPath")
     def default_path(self) -> Optional[str]:
+        """
+        Automatically redirect to this path upon connecting.
+        """
         return pulumi.get(self, "default_path")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="headersBlacklist")
     def headers_blacklist(self) -> Optional[str]:
+        """
+        Header names (e.g. Authorization), to omit from logs.
+        """
         return pulumi.get(self, "headers_blacklist")
 
     @property
     @pulumi.getter(name="hostOverride")
     def host_override(self) -> Optional[str]:
+        """
+        The host header will be overwritten with this field if provided.
+        """
         return pulumi.get(self, "host_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -6939,21 +8282,28 @@
                  headers_blacklist: Optional[str] = None,
                  host_override: Optional[str] = None,
                  password: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str healthcheck_path: This path will be used to check the health of your site.
         :param str name: Unique human-readable name of the Resource.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
-        :param str url: * kubernetes:
-        :param str bind_interface: Bind interface
+        :param str url: The base address of your website without the path.
+               * kubernetes:
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str default_path: Automatically redirect to this path upon connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str headers_blacklist: Header names (e.g. Authorization), to omit from logs.
+        :param str host_override: The host header will be overwritten with this field if provided.
+        :param str password: The password to authenticate with.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "subdomain", subdomain)
         pulumi.set(__self__, "url", url)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -6973,14 +8323,17 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="healthcheckPath")
     def healthcheck_path(self) -> str:
+        """
+        This path will be used to check the health of your site.
+        """
         return pulumi.get(self, "healthcheck_path")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
@@ -6995,52 +8348,65 @@
         """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def url(self) -> str:
         """
+        The base address of your website without the path.
         * kubernetes:
         """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="defaultPath")
     def default_path(self) -> Optional[str]:
+        """
+        Automatically redirect to this path upon connecting.
+        """
         return pulumi.get(self, "default_path")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="headersBlacklist")
     def headers_blacklist(self) -> Optional[str]:
+        """
+        Header names (e.g. Authorization), to omit from logs.
+        """
         return pulumi.get(self, "headers_blacklist")
 
     @property
     @pulumi.getter(name="hostOverride")
     def host_override(self) -> Optional[str]:
+        """
+        The host header will be overwritten with this field if provided.
+        """
         return pulumi.get(self, "host_override")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -7054,14 +8420,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceHttpNoAuth(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7101,19 +8470,24 @@
                  default_path: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  headers_blacklist: Optional[str] = None,
                  host_override: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str healthcheck_path: This path will be used to check the health of your site.
         :param str name: Unique human-readable name of the Resource.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
-        :param str url: * kubernetes:
-        :param str bind_interface: Bind interface
+        :param str url: The base address of your website without the path.
+               * kubernetes:
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str default_path: Automatically redirect to this path upon connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str headers_blacklist: Header names (e.g. Authorization), to omit from logs.
+        :param str host_override: The host header will be overwritten with this field if provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "subdomain", subdomain)
         pulumi.set(__self__, "url", url)
@@ -7131,14 +8505,17 @@
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="healthcheckPath")
     def healthcheck_path(self) -> str:
+        """
+        This path will be used to check the health of your site.
+        """
         return pulumi.get(self, "healthcheck_path")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
@@ -7153,47 +8530,57 @@
         """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def url(self) -> str:
         """
+        The base address of your website without the path.
         * kubernetes:
         """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="defaultPath")
     def default_path(self) -> Optional[str]:
+        """
+        Automatically redirect to this path upon connecting.
+        """
         return pulumi.get(self, "default_path")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="headersBlacklist")
     def headers_blacklist(self) -> Optional[str]:
+        """
+        Header names (e.g. Authorization), to omit from logs.
+        """
         return pulumi.get(self, "headers_blacklist")
 
     @property
     @pulumi.getter(name="hostOverride")
     def host_override(self) -> Optional[str]:
+        """
+        The host header will be overwritten with this field if provided.
+        """
         return pulumi.get(self, "host_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -7259,18 +8646,26 @@
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
@@ -7298,50 +8693,65 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -7355,24 +8765,33 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -7433,21 +8852,26 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -7466,34 +8890,40 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -7508,19 +8938,25 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -7542,14 +8978,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceKubernetesServiceAccount(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7591,22 +9030,28 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -7627,34 +9072,40 @@
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -7669,24 +9120,33 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -7709,14 +9169,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class ResourceKubernetesServiceAccountUserImpersonation(dict):
@@ -7754,22 +9215,26 @@
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -7786,34 +9251,40 @@
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -7828,14 +9299,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -7858,14 +9332,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class ResourceKubernetesUserImpersonation(dict):
@@ -7911,18 +9386,24 @@
                  egress_filter: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
@@ -7946,50 +9427,65 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -8003,14 +9499,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -8075,20 +9574,28 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -8111,63 +9618,81 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -8189,19 +9714,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMemcached(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -8233,17 +9764,20 @@
                  egress_filter: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -8260,48 +9794,57 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -8366,20 +9909,28 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -8402,63 +9953,81 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -8480,19 +10049,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMongoHost(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -8532,20 +10107,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str auth_database: The authentication database to use.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -8566,58 +10148,73 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> str:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -8639,19 +10236,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMongoLegacyHost(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -8694,20 +10297,28 @@
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str auth_database: The authentication database to use.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str replica_set: The name of the mongo replicaset.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -8730,63 +10341,81 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> str:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> Optional[str]:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -8808,19 +10437,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMongoLegacyReplicaset(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -8866,20 +10501,29 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str auth_database: The authentication database to use.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str replica_set: The name of the mongo replicaset.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool connect_to_replica: Set to connect to a replica instead of the primary node.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8903,68 +10547,89 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> str:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> str:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="connectToReplica")
     def connect_to_replica(self) -> Optional[bool]:
+        """
+        Set to connect to a replica instead of the primary node.
+        """
         return pulumi.get(self, "connect_to_replica")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -8986,19 +10651,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMongoReplicaSet(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9044,20 +10715,29 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str auth_database: The authentication database to use.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str replica_set: The name of the mongo replicaset.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool connect_to_replica: Set to connect to a replica instead of the primary node.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9081,68 +10761,89 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> str:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> str:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="connectToReplica")
     def connect_to_replica(self) -> Optional[bool]:
+        """
+        Set to connect to a replica instead of the primary node.
+        """
         return pulumi.get(self, "connect_to_replica")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -9164,19 +10865,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMongoShardedCluster(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9215,20 +10922,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str auth_database: The authentication database to use.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -9247,53 +10960,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> str:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -9315,19 +11040,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMtlsMysql(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9380,20 +11111,32 @@
                  secret_store_id: Optional[str] = None,
                  server_name: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str server_name: Server name for TLS verification (unverified by StrongDM if empty)
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -9424,91 +11167,121 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
+        """
+        Server name for TLS verification (unverified by StrongDM if empty)
+        """
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -9522,19 +11295,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMtlsPostgres(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9584,20 +11363,31 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  server_name: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str server_name: Server name for TLS verification (unverified by StrongDM if empty)
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -9626,91 +11416,121 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
+        """
+        Server name for TLS verification (unverified by StrongDM if empty)
+        """
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -9724,14 +11544,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceMysql(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9772,20 +11595,28 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -9808,63 +11639,81 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -9886,19 +11735,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceNeptune(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9930,17 +11785,20 @@
                  egress_filter: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -9957,48 +11815,57 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -10067,17 +11934,25 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
-        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str region: The AWS region to connect to.
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
@@ -10103,73 +11978,97 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -10231,20 +12130,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10264,58 +12170,73 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -10337,19 +12258,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourcePostgres(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -10387,20 +12314,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -10421,63 +12355,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -10499,14 +12451,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourcePresto(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -10544,20 +12499,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -10578,58 +12540,73 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -10651,19 +12628,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceRabbitmqAmqp091(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -10700,20 +12683,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -10733,53 +12722,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -10801,19 +12802,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceRawTcp(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -10845,17 +12852,20 @@
                  egress_filter: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -10872,48 +12882,57 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -10974,20 +12993,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool downgrade_nla_connections: When set, network level authentication will not be used. May resolve unexpected authentication errors to older servers. When set, healthchecks cannot detect if a provided username / password pair is correct.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if downgrade_nla_connections is not None:
             pulumi.set(__self__, "downgrade_nla_connections", downgrade_nla_connections)
@@ -11007,58 +13032,73 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="downgradeNlaConnections")
     def downgrade_nla_connections(self) -> Optional[bool]:
+        """
+        When set, network level authentication will not be used. May resolve unexpected authentication errors to older servers. When set, healthchecks cannot detect if a provided username / password pair is correct.
+        """
         return pulumi.get(self, "downgrade_nla_connections")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -11080,14 +13120,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceRedis(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -11124,20 +13167,26 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -11157,53 +13206,65 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -11225,19 +13286,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceRedshift(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -11275,20 +13342,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -11309,63 +13383,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -11387,14 +13479,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSingleStore(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -11435,20 +13530,28 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -11471,63 +13574,81 @@
             pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -11549,19 +13670,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSnowflake(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -11596,20 +13723,26 @@
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str schema: The Schema to use to direct initial requests.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -11628,58 +13761,73 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -11701,14 +13849,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSnowsight(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -11744,18 +13895,21 @@
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  port_override: Optional[int] = None,
                  saml_metadata: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str healthcheck_username: The StrongDM user email to use for healthchecks.
         :param str name: Unique human-readable name of the Resource.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str saml_metadata: The Metadata for your snowflake IDP integration
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_username", healthcheck_username)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "subdomain", subdomain)
         if bind_interface is not None:
@@ -11770,14 +13924,17 @@
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="healthcheckUsername")
     def healthcheck_username(self) -> str:
+        """
+        The StrongDM user email to use for healthchecks.
+        """
         return pulumi.get(self, "healthcheck_username")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
@@ -11792,34 +13949,40 @@
         """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="samlMetadata")
     def saml_metadata(self) -> Optional[str]:
+        """
+        The Metadata for your snowflake IDP integration
+        """
         return pulumi.get(self, "saml_metadata")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -11874,20 +14037,28 @@
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str schema: The Schema to use to direct initial requests.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -11910,68 +14081,89 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -11993,14 +14185,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSqlServerAzureAd(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -12044,21 +14239,30 @@
                  schema: Optional[str] = None,
                  secret: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str client_id: The Azure AD application (client) ID with which to authenticate.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str schema: The Schema to use to direct initial requests.
+        :param str secret: The Azure AD client secret (application password) with which to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * sql_server_kerberos_ad:
+        :param str tenant_id: The Azure AD directory (tenant) ID with which to authenticate.
+               * sql_server_kerberos_ad:
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if client_id is not None:
@@ -12083,73 +14287,97 @@
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> Optional[str]:
+        """
+        The Azure AD application (client) ID with which to authenticate.
+        """
         return pulumi.get(self, "client_id")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter
     def secret(self) -> Optional[str]:
+        """
+        The Azure AD client secret (application password) with which to authenticate.
+        """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -12172,14 +14400,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
+        The Azure AD directory (tenant) ID with which to authenticate.
         * sql_server_kerberos_ad:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
 class ResourceSqlServerKerberosAd(dict):
@@ -12227,20 +14456,31 @@
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  server_spn: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str keytab: The keytab file in base64 format containing an entry with the principal name (username@realm) and key version number with which to authenticate.
+        :param str krb_config: The Kerberos 5 configuration file (krb5.conf) specifying the Active Directory server (KDC) for the configured realm.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str realm: The Active Directory domain (realm) to which the configured username belongs.
+        :param str schema: The Schema to use to direct initial requests.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str server_spn: The Service Principal Name of the Microsoft SQL Server instance in Active Directory.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -12269,91 +14509,121 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def keytab(self) -> Optional[str]:
+        """
+        The keytab file in base64 format containing an entry with the principal name (username@realm) and key version number with which to authenticate.
+        """
         return pulumi.get(self, "keytab")
 
     @property
     @pulumi.getter(name="krbConfig")
     def krb_config(self) -> Optional[str]:
+        """
+        The Kerberos 5 configuration file (krb5.conf) specifying the Active Directory server (KDC) for the configured realm.
+        """
         return pulumi.get(self, "krb_config")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def realm(self) -> Optional[str]:
+        """
+        The Active Directory domain (realm) to which the configured username belongs.
+        """
         return pulumi.get(self, "realm")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serverSpn")
     def server_spn(self) -> Optional[str]:
+        """
+        The Service Principal Name of the Microsoft SQL Server instance in Active Directory.
+        """
         return pulumi.get(self, "server_spn")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -12367,14 +14637,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSsh(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -12419,20 +14692,28 @@
                  port_override: Optional[int] = None,
                  public_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param bool allow_deprecated_key_exchanges: Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str key_type: The key type to use e.g. rsa-2048 or ed25519
+        :param bool port_forwarding: Whether port forwarding is allowed through this server.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str public_key: The public key to append to a server's authorized keys. This will be generated after resource creation.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
@@ -12455,68 +14736,89 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
     def allow_deprecated_key_exchanges(self) -> Optional[bool]:
+        """
+        Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        """
         return pulumi.get(self, "allow_deprecated_key_exchanges")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="keyType")
     def key_type(self) -> Optional[str]:
+        """
+        The key type to use e.g. rsa-2048 or ed25519
+        """
         return pulumi.get(self, "key_type")
 
     @property
     @pulumi.getter(name="portForwarding")
     def port_forwarding(self) -> Optional[bool]:
+        """
+        Whether port forwarding is allowed through this server.
+        """
         return pulumi.get(self, "port_forwarding")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[str]:
+        """
+        The public key to append to a server's authorized keys. This will be generated after resource creation.
+        """
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -12538,14 +14840,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSshCert(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -12593,20 +14898,29 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param bool allow_deprecated_key_exchanges: Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str key_type: The key type to use e.g. rsa-2048 or ed25519
+        :param bool port_forwarding: Whether port forwarding is allowed through this server.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
@@ -12631,73 +14945,97 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
     def allow_deprecated_key_exchanges(self) -> Optional[bool]:
+        """
+        Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        """
         return pulumi.get(self, "allow_deprecated_key_exchanges")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="keyType")
     def key_type(self) -> Optional[str]:
+        """
+        The key type to use e.g. rsa-2048 or ed25519
+        """
         return pulumi.get(self, "key_type")
 
     @property
     @pulumi.getter(name="portForwarding")
     def port_forwarding(self) -> Optional[bool]:
+        """
+        Whether port forwarding is allowed through this server.
+        """
         return pulumi.get(self, "port_forwarding")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -12719,14 +15057,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSshCustomerKey(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -12768,20 +15109,27 @@
                  port_override: Optional[int] = None,
                  private_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param bool allow_deprecated_key_exchanges: Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool port_forwarding: Whether port forwarding is allowed through this server.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str private_key: The private key used to authenticate with the server.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
@@ -12802,63 +15150,81 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> int:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
     def allow_deprecated_key_exchanges(self) -> Optional[bool]:
+        """
+        Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        """
         return pulumi.get(self, "allow_deprecated_key_exchanges")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="portForwarding")
     def port_forwarding(self) -> Optional[bool]:
+        """
+        Whether port forwarding is allowed through this server.
+        """
         return pulumi.get(self, "port_forwarding")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> Optional[str]:
+        """
+        The private key used to authenticate with the server.
+        """
         return pulumi.get(self, "private_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -12880,14 +15246,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSybase(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -12921,20 +15290,25 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -12952,53 +15326,65 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -13020,14 +15406,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceSybaseIq(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -13061,20 +15450,25 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -13092,53 +15486,65 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -13160,14 +15566,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceTeradata(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -13201,20 +15610,25 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -13232,53 +15646,65 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -13300,14 +15726,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ResourceTrino(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -13342,20 +15771,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str name: Unique human-readable name of the Resource.
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -13374,58 +15809,73 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def database(self) -> str:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -13447,25 +15897,29 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class SecretStoreAws(dict):
     def __init__(__self__, *,
                  name: str,
                  region: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
+        :param str region: The AWS region to target e.g. us-east-1
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
@@ -13476,14 +15930,17 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> str:
+        """
+        The AWS region to target e.g. us-east-1
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -13512,15 +15969,16 @@
 
     def __init__(__self__, *,
                  name: str,
                  vault_uri: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
-        :param str vault_uri: * cyberark_conjur:
+        :param str vault_uri: The URI of the key vault to target e.g. https://myvault.vault.azure.net
+               * cyberark_conjur:
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "vault_uri", vault_uri)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
@@ -13532,14 +15990,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="vaultUri")
     def vault_uri(self) -> str:
         """
+        The URI of the key vault to target e.g. https://myvault.vault.azure.net
         * cyberark_conjur:
         """
         return pulumi.get(self, "vault_uri")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
@@ -13569,25 +16028,29 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  app_url: str,
                  name: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str app_url: The URL of the Cyberark instance
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "app_url", app_url)
         pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="appUrl")
     def app_url(self) -> str:
+        """
+        The URL of the Cyberark instance
+        """
         return pulumi.get(self, "app_url")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the SecretStore.
@@ -13623,25 +16086,29 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  app_url: str,
                  name: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str app_url: The URL of the Cyberark instance
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "app_url", app_url)
         pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="appUrl")
     def app_url(self) -> str:
+        """
+        The URL of the Cyberark instance
+        """
         return pulumi.get(self, "app_url")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the SecretStore.
@@ -13677,25 +16144,29 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  app_url: str,
                  name: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str app_url: The URL of the Cyberark instance
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "app_url", app_url)
         pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="appUrl")
     def app_url(self) -> str:
+        """
+        The URL of the Cyberark instance
+        """
         return pulumi.get(self, "app_url")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the SecretStore.
@@ -13735,16 +16206,18 @@
     def __init__(__self__, *,
                  name: str,
                  server_url: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_name: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
+        :param str server_url: The URL of the Delinea instance
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_name: * gcp_store:
+        :param str tenant_name: The tenant name to target
+               * gcp_store:
         """
         pulumi.set(__self__, "name", name)
         if server_url is not None:
             pulumi.set(__self__, "server_url", server_url)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tenant_name is not None:
@@ -13757,28 +16230,32 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="serverUrl")
     def server_url(self) -> Optional[str]:
+        """
+        The URL of the Delinea instance
+        """
         return pulumi.get(self, "server_url")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantName")
     def tenant_name(self) -> Optional[str]:
         """
+        The tenant name to target
         * gcp_store:
         """
         return pulumi.get(self, "tenant_name")
 
 
 @pulumi.output_type
 class SecretStoreGcpStore(dict):
@@ -13801,14 +16278,15 @@
 
     def __init__(__self__, *,
                  name: str,
                  project_id: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
+        :param str project_id: The GCP project ID to target.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project_id", project_id)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
@@ -13819,14 +16297,17 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> str:
+        """
+        The GCP project ID to target.
+        """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -13856,14 +16337,16 @@
     def __init__(__self__, *,
                  name: str,
                  server_address: str,
                  namespace: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param str namespace: The namespace to make requests within
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "server_address", server_address)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if tags is not None:
@@ -13876,19 +16359,25 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="serverAddress")
     def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
         return pulumi.get(self, "server_address")
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -13926,15 +16415,20 @@
                  client_key_path: str,
                  name: str,
                  server_address: str,
                  ca_cert_path: Optional[str] = None,
                  namespace: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str client_cert_path: A path to a client certificate file accessible by a Node
+        :param str client_key_path: A path to a client key file accessible by a Node
         :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param str ca_cert_path: A path to a CA file accessible by a Node
+        :param str namespace: The namespace to make requests within
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "client_cert_path", client_cert_path)
         pulumi.set(__self__, "client_key_path", client_key_path)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "server_address", server_address)
         if ca_cert_path is not None:
@@ -13943,42 +16437,57 @@
             pulumi.set(__self__, "namespace", namespace)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clientCertPath")
     def client_cert_path(self) -> str:
+        """
+        A path to a client certificate file accessible by a Node
+        """
         return pulumi.get(self, "client_cert_path")
 
     @property
     @pulumi.getter(name="clientKeyPath")
     def client_key_path(self) -> str:
+        """
+        A path to a client key file accessible by a Node
+        """
         return pulumi.get(self, "client_key_path")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="serverAddress")
     def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
         return pulumi.get(self, "server_address")
 
     @property
     @pulumi.getter(name="caCertPath")
     def ca_cert_path(self) -> Optional[str]:
+        """
+        A path to a CA file accessible by a Node
+        """
         return pulumi.get(self, "ca_cert_path")
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -14008,14 +16517,16 @@
     def __init__(__self__, *,
                  name: str,
                  server_address: str,
                  namespace: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
+        :param str server_address: The URL of the Vault to target
+        :param str namespace: The namespace to make requests within
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "server_address", server_address)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if tags is not None:
@@ -14028,19 +16539,25 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="serverAddress")
     def server_address(self) -> str:
+        """
+        The URL of the Vault to target
+        """
         return pulumi.get(self, "server_address")
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -14300,51 +16817,59 @@
 @pulumi.output_type
 class GetNodeNodeGatewayResult(dict):
     def __init__(__self__, *,
                  device: str,
                  location: str,
                  version: str,
                  bind_address: Optional[str] = None,
+                 connects_to: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  listen_address: Optional[str] = None,
+                 maintenance_windows: Optional[Sequence['outputs.GetNodeNodeGatewayMaintenanceWindowResult']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
+        :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
-        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
+        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str id: Unique identifier of the Relay.
         :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
+        :param Sequence['GetNodeNodeGatewayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "device", device)
         pulumi.set(__self__, "location", location)
         pulumi.set(__self__, "version", version)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
+        if connects_to is not None:
+            pulumi.set(__self__, "connects_to", connects_to)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if listen_address is not None:
             pulumi.set(__self__, "listen_address", listen_address)
+        if maintenance_windows is not None:
+            pulumi.set(__self__, "maintenance_windows", maintenance_windows)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def device(self) -> str:
         """
-        Device is a read only device name uploaded by the gateway process when  it comes online.
+        Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter
     def location(self) -> str:
         """
@@ -14365,18 +16890,26 @@
     def bind_address(self) -> Optional[str]:
         """
         The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
         """
         return pulumi.get(self, "bind_address")
 
     @property
+    @pulumi.getter(name="connectsTo")
+    def connects_to(self) -> Optional[str]:
+        """
+        ConnectsTo can be used to restrict the peering between relays and gateways.
+        """
+        return pulumi.get(self, "connects_to")
+
+    @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
-        GatewayFilter can be used to restrict the peering between relays and gateways.
+        GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         """
         return pulumi.get(self, "gateway_filter")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
@@ -14389,14 +16922,22 @@
     def listen_address(self) -> Optional[str]:
         """
         The public hostname/port tuple at which the gateway will be accessible to clients.
         """
         return pulumi.get(self, "listen_address")
 
     @property
+    @pulumi.getter(name="maintenanceWindows")
+    def maintenance_windows(self) -> Optional[Sequence['outputs.GetNodeNodeGatewayMaintenanceWindowResult']]:
+        """
+        Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
+        """
+        return pulumi.get(self, "maintenance_windows")
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
@@ -14406,49 +16947,76 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class GetNodeNodeGatewayMaintenanceWindowResult(dict):
+    def __init__(__self__, *,
+                 cron_schedule: str,
+                 require_idleness: bool):
+        pulumi.set(__self__, "cron_schedule", cron_schedule)
+        pulumi.set(__self__, "require_idleness", require_idleness)
+
+    @property
+    @pulumi.getter(name="cronSchedule")
+    def cron_schedule(self) -> str:
+        return pulumi.get(self, "cron_schedule")
+
+    @property
+    @pulumi.getter(name="requireIdleness")
+    def require_idleness(self) -> bool:
+        return pulumi.get(self, "require_idleness")
+
+
+@pulumi.output_type
 class GetNodeNodeRelayResult(dict):
     def __init__(__self__, *,
                  device: str,
                  location: str,
                  version: str,
+                 connects_to: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  id: Optional[str] = None,
+                 maintenance_windows: Optional[Sequence['outputs.GetNodeNodeRelayMaintenanceWindowResult']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
+        :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
-        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
+        :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str id: Unique identifier of the Relay.
+        :param Sequence['GetNodeNodeRelayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "device", device)
         pulumi.set(__self__, "location", location)
         pulumi.set(__self__, "version", version)
+        if connects_to is not None:
+            pulumi.set(__self__, "connects_to", connects_to)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
+        if maintenance_windows is not None:
+            pulumi.set(__self__, "maintenance_windows", maintenance_windows)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def device(self) -> str:
         """
-        Device is a read only device name uploaded by the gateway process when  it comes online.
+        Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
 
     @property
     @pulumi.getter
     def location(self) -> str:
         """
@@ -14461,30 +17029,46 @@
     def version(self) -> str:
         """
         Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "version")
 
     @property
+    @pulumi.getter(name="connectsTo")
+    def connects_to(self) -> Optional[str]:
+        """
+        ConnectsTo can be used to restrict the peering between relays and gateways.
+        """
+        return pulumi.get(self, "connects_to")
+
+    @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
-        GatewayFilter can be used to restrict the peering between relays and gateways.
+        GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         """
         return pulumi.get(self, "gateway_filter")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Relay.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="maintenanceWindows")
+    def maintenance_windows(self) -> Optional[Sequence['outputs.GetNodeNodeRelayMaintenanceWindowResult']]:
+        """
+        Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
+        """
+        return pulumi.get(self, "maintenance_windows")
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
@@ -14494,14 +17078,33 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class GetNodeNodeRelayMaintenanceWindowResult(dict):
+    def __init__(__self__, *,
+                 cron_schedule: str,
+                 require_idleness: bool):
+        pulumi.set(__self__, "cron_schedule", cron_schedule)
+        pulumi.set(__self__, "require_idleness", require_idleness)
+
+    @property
+    @pulumi.getter(name="cronSchedule")
+    def cron_schedule(self) -> str:
+        return pulumi.get(self, "cron_schedule")
+
+    @property
+    @pulumi.getter(name="requireIdleness")
+    def require_idleness(self) -> bool:
+        return pulumi.get(self, "require_idleness")
+
+
+@pulumi.output_type
 class GetRemoteIdentityGroupRemoteIdentityGroupResult(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None):
         """
         :param str id: Unique identifier of the RemoteIdentityGroup.
         :param str name: Unique human-readable name of the RemoteIdentityGroup.
@@ -14602,14 +17205,15 @@
                  aurora_postgres: Sequence['outputs.GetResourceResourceAuroraPostgreResult'],
                  aws: Sequence['outputs.GetResourceResourceAwResult'],
                  aws_console_static_key_pairs: Sequence['outputs.GetResourceResourceAwsConsoleStaticKeyPairResult'],
                  aws_consoles: Sequence['outputs.GetResourceResourceAwsConsoleResult'],
                  azure_certificates: Sequence['outputs.GetResourceResourceAzureCertificateResult'],
                  azure_mysqls: Sequence['outputs.GetResourceResourceAzureMysqlResult'],
                  azure_postgres: Sequence['outputs.GetResourceResourceAzurePostgreResult'],
+                 azure_postgres_managed_identities: Sequence['outputs.GetResourceResourceAzurePostgresManagedIdentityResult'],
                  azures: Sequence['outputs.GetResourceResourceAzureResult'],
                  big_queries: Sequence['outputs.GetResourceResourceBigQueryResult'],
                  cassandras: Sequence['outputs.GetResourceResourceCassandraResult'],
                  cituses: Sequence['outputs.GetResourceResourceCitusResult'],
                  clustrixes: Sequence['outputs.GetResourceResourceClustrixResult'],
                  cockroaches: Sequence['outputs.GetResourceResourceCockroachResult'],
                  db2_is: Sequence['outputs.GetResourceResourceDb2IResult'],
@@ -14682,14 +17286,15 @@
         pulumi.set(__self__, "aurora_postgres", aurora_postgres)
         pulumi.set(__self__, "aws", aws)
         pulumi.set(__self__, "aws_console_static_key_pairs", aws_console_static_key_pairs)
         pulumi.set(__self__, "aws_consoles", aws_consoles)
         pulumi.set(__self__, "azure_certificates", azure_certificates)
         pulumi.set(__self__, "azure_mysqls", azure_mysqls)
         pulumi.set(__self__, "azure_postgres", azure_postgres)
+        pulumi.set(__self__, "azure_postgres_managed_identities", azure_postgres_managed_identities)
         pulumi.set(__self__, "azures", azures)
         pulumi.set(__self__, "big_queries", big_queries)
         pulumi.set(__self__, "cassandras", cassandras)
         pulumi.set(__self__, "cituses", cituses)
         pulumi.set(__self__, "clustrixes", clustrixes)
         pulumi.set(__self__, "cockroaches", cockroaches)
         pulumi.set(__self__, "db2_is", db2_is)
@@ -14844,14 +17449,19 @@
 
     @property
     @pulumi.getter(name="azurePostgres")
     def azure_postgres(self) -> Sequence['outputs.GetResourceResourceAzurePostgreResult']:
         return pulumi.get(self, "azure_postgres")
 
     @property
+    @pulumi.getter(name="azurePostgresManagedIdentities")
+    def azure_postgres_managed_identities(self) -> Sequence['outputs.GetResourceResourceAzurePostgresManagedIdentityResult']:
+        return pulumi.get(self, "azure_postgres_managed_identities")
+
+    @property
     @pulumi.getter
     def azures(self) -> Sequence['outputs.GetResourceResourceAzureResult']:
         return pulumi.get(self, "azures")
 
     @property
     @pulumi.getter(name="bigQueries")
     def big_queries(self) -> Sequence['outputs.GetResourceResourceBigQueryResult']:
@@ -15164,19 +17774,27 @@
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -15210,31 +17828,40 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -15248,14 +17875,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -15269,29 +17899,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -15328,22 +17970,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
@@ -15368,15 +18015,15 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -15391,14 +18038,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -15412,24 +18062,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -15451,14 +18110,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceAksServiceAccountResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -15472,23 +18134,29 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
@@ -15515,15 +18183,15 @@
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -15538,14 +18206,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -15559,29 +18230,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -15604,14 +18287,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class GetResourceResourceAksServiceAccountUserImpersonationResult(dict):
@@ -15625,23 +18309,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
@@ -15664,15 +18352,15 @@
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -15687,14 +18375,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -15708,19 +18399,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -15743,14 +18440,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class GetResourceResourceAksUserImpersonationResult(dict):
@@ -15766,19 +18464,25 @@
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -15808,31 +18512,40 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -15846,14 +18559,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -15867,19 +18583,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -15917,18 +18639,25 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -15957,35 +18686,41 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -15999,34 +18734,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -16069,19 +18819,30 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str cluster_name: The name of the cluster to connect to.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -16120,45 +18881,57 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> Optional[str]:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="healthcheckNamespace")
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
@@ -16180,44 +18953,65 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -16258,19 +19052,28 @@
                  remote_identity_healthcheck_username: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str cluster_name: The name of the cluster to connect to.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -16306,39 +19109,48 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> Optional[str]:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="healthcheckNamespace")
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
@@ -16360,39 +19172,57 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -16433,19 +19263,28 @@
                  remote_identity_healthcheck_username: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str cluster_name: The name of the cluster to connect to.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -16481,39 +19320,48 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> Optional[str]:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="healthcheckNamespace")
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
@@ -16535,39 +19383,57 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -16608,19 +19474,28 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str cluster_name: The name of the cluster to connect to.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -16655,45 +19530,57 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> Optional[str]:
+        """
+        The name of the cluster to connect to.
+        """
         return pulumi.get(self, "cluster_name")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="healthcheckNamespace")
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
@@ -16715,34 +19602,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -16779,21 +19681,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -16818,29 +19726,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -16854,24 +19765,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -16893,19 +19813,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceAthenaResult(dict):
     def __init__(__self__, *,
                  access_key: Optional[str] = None,
@@ -16919,18 +19845,25 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str output: The AWS S3 output location.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -16959,21 +19892,24 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -16996,39 +19932,57 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def output(self) -> Optional[str]:
+        """
+        The AWS S3 output location.
+        """
         return pulumi.get(self, "output")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -17067,21 +20021,29 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -17110,34 +20072,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -17151,29 +20119,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -17195,19 +20175,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceAuroraPostgreResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -17221,21 +20207,28 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -17262,34 +20255,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -17303,29 +20302,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -17347,14 +20358,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceAwResult(dict):
     def __init__(__self__, *,
                  access_key: Optional[str] = None,
@@ -17367,18 +20381,24 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str healthcheck_region: The AWS region healthcheck requests should attempt to connect to.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -17405,35 +20425,41 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="healthcheckRegion")
     def healthcheck_region(self) -> Optional[str]:
+        """
+        The AWS region healthcheck requests should attempt to connect to.
+        """
         return pulumi.get(self, "healthcheck_region")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -17447,29 +20473,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -17508,19 +20546,27 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  session_expiry: Optional[int] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param bool enable_env_variables: If true, prefer environment variables to authenticate connection even if EC2 roles are configured.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param int session_expiry: The length of time in seconds AWS console sessions will live before needing to reauthenticate.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -17551,29 +20597,32 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="enableEnvVariables")
     def enable_env_variables(self) -> Optional[bool]:
+        """
+        If true, prefer environment variables to authenticate connection even if EC2 roles are configured.
+        """
         return pulumi.get(self, "enable_env_variables")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -17587,52 +20636,73 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="sessionExpiry")
     def session_expiry(self) -> Optional[int]:
+        """
+        The length of time in seconds AWS console sessions will live before needing to reauthenticate.
+        """
         return pulumi.get(self, "session_expiry")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -17664,19 +20734,28 @@
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  session_expiry: Optional[int] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param int session_expiry: The length of time in seconds AWS console sessions will live before needing to reauthenticate.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -17708,21 +20787,24 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -17745,57 +20827,81 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="sessionExpiry")
     def session_expiry(self) -> Optional[int]:
+        """
+        The length of time in seconds AWS console sessions will live before needing to reauthenticate.
+        """
         return pulumi.get(self, "session_expiry")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -17822,22 +20928,26 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str app_id: The application ID to authenticate with.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * sql_server_kerberos_ad:
+        :param str tenant_id: The Azure AD directory (tenant) ID with which to authenticate.
+               * sql_server_kerberos_ad:
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -17857,21 +20967,24 @@
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter(name="appId")
     def app_id(self) -> Optional[str]:
+        """
+        The application ID to authenticate with.
+        """
         return pulumi.get(self, "app_id")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -17894,19 +21007,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -17929,14 +21048,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
+        The Azure AD directory (tenant) ID with which to authenticate.
         * sql_server_kerberos_ad:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
 class GetResourceResourceAzureCertificateResult(dict):
@@ -17949,22 +21069,26 @@
                  name: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str app_id: The application ID to authenticate with.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * sql_server_kerberos_ad:
+        :param str tenant_id: The Azure AD directory (tenant) ID with which to authenticate.
+               * sql_server_kerberos_ad:
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if client_certificate is not None:
             pulumi.set(__self__, "client_certificate", client_certificate)
@@ -17984,27 +21108,33 @@
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter(name="appId")
     def app_id(self) -> Optional[str]:
+        """
+        The application ID to authenticate with.
+        """
         return pulumi.get(self, "app_id")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -18026,14 +21156,17 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -18056,14 +21189,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
+        The Azure AD directory (tenant) ID with which to authenticate.
         * sql_server_kerberos_ad:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
 class GetResourceResourceAzureMysqlResult(dict):
@@ -18080,21 +21214,29 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -18123,34 +21265,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -18164,29 +21312,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -18208,19 +21368,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceAzurePostgreResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -18234,21 +21400,28 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -18275,34 +21448,219 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
+        return pulumi.get(self, "database")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="overrideDatabase")
+    def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
+        return pulumi.get(self, "override_database")
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
+class GetResourceResourceAzurePostgresManagedIdentityResult(dict):
+    def __init__(__self__, *,
+                 bind_interface: Optional[str] = None,
+                 database: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 hostname: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 override_database: Optional[bool] = None,
+                 password: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 use_azure_single_server_usernames: Optional[bool] = None,
+                 username: Optional[str] = None):
+        """
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
+        :param str id: Unique identifier of the Resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
+        """
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if database is not None:
+            pulumi.set(__self__, "database", database)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if hostname is not None:
+            pulumi.set(__self__, "hostname", hostname)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if override_database is not None:
+            pulumi.set(__self__, "override_database", override_database)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if use_azure_single_server_usernames is not None:
+            pulumi.set(__self__, "use_azure_single_server_usernames", use_azure_single_server_usernames)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter
+    def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -18316,29 +21674,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -18358,16 +21728,27 @@
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
+    @pulumi.getter(name="useAzureSingleServerUsernames")
+    def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
+        return pulumi.get(self, "use_azure_single_server_usernames")
+
+    @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceBigQueryResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -18379,21 +21760,26 @@
                  private_key: Optional[str] = None,
                  project: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str private_key: The private key used to authenticate with the server.
+        :param str project: The project to connect to.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
@@ -18416,29 +21802,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -18452,24 +21841,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> Optional[str]:
+        """
+        The private key used to authenticate with the server.
+        """
         return pulumi.get(self, "private_key")
 
     @property
     @pulumi.getter
     def project(self) -> Optional[str]:
+        """
+        The project to connect to.
+        """
         return pulumi.get(self, "project")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -18491,14 +21889,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceCassandraResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -18511,21 +21912,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -18550,29 +21957,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -18586,24 +21996,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -18625,19 +22044,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceCitusResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -18651,21 +22076,28 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -18692,34 +22124,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -18733,29 +22171,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -18777,14 +22227,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceClustrixResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -18799,21 +22252,29 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -18842,34 +22303,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -18883,29 +22350,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -18927,19 +22406,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceCockroachResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -18953,21 +22438,28 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -18994,34 +22486,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -19035,29 +22533,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -19079,14 +22589,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceDb2IResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -19099,21 +22612,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -19138,29 +22657,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -19174,24 +22696,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -19213,19 +22744,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceDb2LuwResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -19238,21 +22775,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -19277,34 +22820,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -19318,24 +22867,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -19357,14 +22915,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceDocumentDbHostResult(dict):
     def __init__(__self__, *,
                  auth_database: Optional[str] = None,
@@ -19377,21 +22938,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str auth_database: The authentication database to use.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -19415,35 +22982,41 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> Optional[str]:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -19457,24 +23030,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -19496,14 +23078,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceDocumentDbReplicaSetResult(dict):
     def __init__(__self__, *,
                  auth_database: Optional[str] = None,
@@ -19517,21 +23102,28 @@
                  port_override: Optional[int] = None,
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str auth_database: The authentication database to use.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool connect_to_replica: Set to connect to a replica instead of the primary node.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str replica_set: The name of the mongo replicaset.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if connect_to_replica is not None:
             pulumi.set(__self__, "connect_to_replica", connect_to_replica)
@@ -19557,40 +23149,49 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> Optional[str]:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="connectToReplica")
     def connect_to_replica(self) -> Optional[bool]:
+        """
+        Set to connect to a replica instead of the primary node.
+        """
         return pulumi.get(self, "connect_to_replica")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -19604,24 +23205,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> Optional[str]:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -19643,14 +23253,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceDruidResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -19662,21 +23275,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -19699,29 +23317,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -19735,24 +23356,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -19774,14 +23404,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceDynamoDbResult(dict):
     def __init__(__self__, *,
                  access_key: Optional[str] = None,
@@ -19795,18 +23428,25 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -19835,35 +23475,41 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -19877,34 +23523,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -19941,21 +23602,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -19980,29 +23647,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -20016,24 +23686,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -20055,19 +23734,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceElasticacheRediResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -20080,21 +23765,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -20119,29 +23810,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -20155,24 +23849,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -20194,19 +23897,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceGcpResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -20216,18 +23925,21 @@
                  name: Optional[str] = None,
                  port_override: Optional[int] = None,
                  scopes: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
+        :param str keyfile: The service account keyfile to authenticate with.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str scopes: Space separated scopes that this login should assume into when authenticating.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -20249,15 +23961,15 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -20272,32 +23984,41 @@
         Unique identifier of the Resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def keyfile(self) -> Optional[str]:
+        """
+        The service account keyfile to authenticate with.
+        """
         return pulumi.get(self, "keyfile")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def scopes(self) -> Optional[str]:
+        """
+        Space separated scopes that this login should assume into when authenticating.
+        """
         return pulumi.get(self, "scopes")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -20334,20 +24055,25 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
@@ -20374,34 +24100,40 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="healthcheckNamespace")
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
@@ -20423,32 +24155,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
+        """
+        The service account key to authenticate with.
+        """
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -20475,20 +24216,23 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str service_account_key: The service account key to authenticate with.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
@@ -20511,34 +24255,40 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="healthcheckNamespace")
     def healthcheck_namespace(self) -> Optional[str]:
         """
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
@@ -20568,14 +24318,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
+        """
+        The service account key to authenticate with.
+        """
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -20605,21 +24358,28 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -20646,34 +24406,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -20687,29 +24453,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -20731,14 +24509,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceHttpAuthResult(dict):
     def __init__(__self__, *,
                  auth_header: Optional[str] = None,
@@ -20751,22 +24532,28 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  url: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
-        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str auth_header: The content to set as the authorization header.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str default_path: Automatically redirect to this path upon connecting.
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str headers_blacklist: Header names (e.g. Authorization), to omit from logs.
+        :param str healthcheck_path: This path will be used to check the health of your site.
+        :param str host_override: The host header will be overwritten with this field if provided.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str url: * kubernetes:
+        :param str url: The base address of your website without the path.
+               * kubernetes:
         """
         if auth_header is not None:
             pulumi.set(__self__, "auth_header", auth_header)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if default_path is not None:
             pulumi.set(__self__, "default_path", default_path)
@@ -20790,50 +24577,65 @@
             pulumi.set(__self__, "tags", tags)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter(name="authHeader")
     def auth_header(self) -> Optional[str]:
+        """
+        The content to set as the authorization header.
+        """
         return pulumi.get(self, "auth_header")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="defaultPath")
     def default_path(self) -> Optional[str]:
+        """
+        Automatically redirect to this path upon connecting.
+        """
         return pulumi.get(self, "default_path")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="headersBlacklist")
     def headers_blacklist(self) -> Optional[str]:
+        """
+        Header names (e.g. Authorization), to omit from logs.
+        """
         return pulumi.get(self, "headers_blacklist")
 
     @property
     @pulumi.getter(name="healthcheckPath")
     def healthcheck_path(self) -> Optional[str]:
+        """
+        This path will be used to check the health of your site.
+        """
         return pulumi.get(self, "healthcheck_path")
 
     @property
     @pulumi.getter(name="hostOverride")
     def host_override(self) -> Optional[str]:
+        """
+        The host header will be overwritten with this field if provided.
+        """
         return pulumi.get(self, "host_override")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -20872,14 +24674,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
         """
+        The base address of your website without the path.
         * kubernetes:
         """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class GetResourceResourceHttpBasicAuthResult(dict):
@@ -20895,22 +24698,29 @@
                  password: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  url: Optional[str] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str default_path: Automatically redirect to this path upon connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str headers_blacklist: Header names (e.g. Authorization), to omit from logs.
+        :param str healthcheck_path: This path will be used to check the health of your site.
+        :param str host_override: The host header will be overwritten with this field if provided.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str url: * kubernetes:
+        :param str url: The base address of your website without the path.
+               * kubernetes:
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if default_path is not None:
             pulumi.set(__self__, "default_path", default_path)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -20937,44 +24747,56 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="defaultPath")
     def default_path(self) -> Optional[str]:
+        """
+        Automatically redirect to this path upon connecting.
+        """
         return pulumi.get(self, "default_path")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="headersBlacklist")
     def headers_blacklist(self) -> Optional[str]:
+        """
+        Header names (e.g. Authorization), to omit from logs.
+        """
         return pulumi.get(self, "headers_blacklist")
 
     @property
     @pulumi.getter(name="healthcheckPath")
     def healthcheck_path(self) -> Optional[str]:
+        """
+        This path will be used to check the health of your site.
+        """
         return pulumi.get(self, "healthcheck_path")
 
     @property
     @pulumi.getter(name="hostOverride")
     def host_override(self) -> Optional[str]:
+        """
+        The host header will be overwritten with this field if provided.
+        """
         return pulumi.get(self, "host_override")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -20988,14 +24810,17 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -21018,21 +24843,25 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
         """
+        The base address of your website without the path.
         * kubernetes:
         """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceHttpNoAuthResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -21044,22 +24873,27 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  url: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str default_path: Automatically redirect to this path upon connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str headers_blacklist: Header names (e.g. Authorization), to omit from logs.
+        :param str healthcheck_path: This path will be used to check the health of your site.
+        :param str host_override: The host header will be overwritten with this field if provided.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str url: * kubernetes:
+        :param str url: The base address of your website without the path.
+               * kubernetes:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if default_path is not None:
             pulumi.set(__self__, "default_path", default_path)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -21082,44 +24916,56 @@
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="defaultPath")
     def default_path(self) -> Optional[str]:
+        """
+        Automatically redirect to this path upon connecting.
+        """
         return pulumi.get(self, "default_path")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="headersBlacklist")
     def headers_blacklist(self) -> Optional[str]:
+        """
+        Header names (e.g. Authorization), to omit from logs.
+        """
         return pulumi.get(self, "headers_blacklist")
 
     @property
     @pulumi.getter(name="healthcheckPath")
     def healthcheck_path(self) -> Optional[str]:
+        """
+        This path will be used to check the health of your site.
+        """
         return pulumi.get(self, "healthcheck_path")
 
     @property
     @pulumi.getter(name="hostOverride")
     def host_override(self) -> Optional[str]:
+        """
+        The host header will be overwritten with this field if provided.
+        """
         return pulumi.get(self, "host_override")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -21158,14 +25004,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
         """
+        The base address of your website without the path.
         * kubernetes:
         """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class GetResourceResourceKuberneteResult(dict):
@@ -21183,19 +25030,27 @@
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -21229,31 +25084,40 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -21267,14 +25131,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -21288,29 +25155,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -21347,22 +25226,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
@@ -21387,15 +25271,15 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -21410,14 +25294,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -21431,24 +25318,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -21470,14 +25366,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceKubernetesServiceAccountResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -21491,23 +25390,29 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
@@ -21534,15 +25439,15 @@
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -21557,14 +25462,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -21578,29 +25486,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -21623,14 +25543,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class GetResourceResourceKubernetesServiceAccountUserImpersonationResult(dict):
@@ -21644,23 +25565,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str token: * kubernetes_user_impersonation:
+        :param str token: The API token to authenticate with.
+               * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
             pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
@@ -21683,15 +25608,15 @@
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
@@ -21706,14 +25631,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -21727,19 +25655,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -21762,14 +25696,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         """
+        The API token to authenticate with.
         * kubernetes_user_impersonation:
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class GetResourceResourceKubernetesUserImpersonationResult(dict):
@@ -21785,19 +25720,25 @@
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -21827,31 +25768,40 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
@@ -21865,14 +25815,17 @@
         The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         """
         return pulumi.get(self, "healthcheck_namespace")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -21886,19 +25839,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -21937,21 +25896,29 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -21980,34 +25947,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -22021,29 +25994,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -22065,19 +26050,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMemcachedResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -22087,18 +26078,21 @@
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -22120,29 +26114,32 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -22156,19 +26153,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -22207,21 +26210,29 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -22250,34 +26261,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -22291,29 +26308,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -22335,19 +26364,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMongoHostResult(dict):
     def __init__(__self__, *,
                  auth_database: Optional[str] = None,
@@ -22361,21 +26396,28 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str auth_database: The authentication database to use.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -22401,35 +26443,41 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> Optional[str]:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -22443,24 +26491,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -22482,19 +26539,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMongoLegacyHostResult(dict):
     def __init__(__self__, *,
                  auth_database: Optional[str] = None,
@@ -22509,21 +26572,29 @@
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str auth_database: The authentication database to use.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str replica_set: The name of the mongo replicaset.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -22551,35 +26622,41 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> Optional[str]:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -22593,29 +26670,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> Optional[str]:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -22637,19 +26726,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMongoLegacyReplicasetResult(dict):
     def __init__(__self__, *,
                  auth_database: Optional[str] = None,
@@ -22665,21 +26760,30 @@
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str auth_database: The authentication database to use.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool connect_to_replica: Set to connect to a replica instead of the primary node.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str replica_set: The name of the mongo replicaset.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if connect_to_replica is not None:
             pulumi.set(__self__, "connect_to_replica", connect_to_replica)
@@ -22709,40 +26813,49 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> Optional[str]:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="connectToReplica")
     def connect_to_replica(self) -> Optional[bool]:
+        """
+        Set to connect to a replica instead of the primary node.
+        """
         return pulumi.get(self, "connect_to_replica")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -22756,29 +26869,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> Optional[str]:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -22800,19 +26925,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMongoReplicaSetResult(dict):
     def __init__(__self__, *,
                  auth_database: Optional[str] = None,
@@ -22828,21 +26959,30 @@
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str auth_database: The authentication database to use.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool connect_to_replica: Set to connect to a replica instead of the primary node.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str replica_set: The name of the mongo replicaset.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if connect_to_replica is not None:
             pulumi.set(__self__, "connect_to_replica", connect_to_replica)
@@ -22872,40 +27012,49 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> Optional[str]:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="connectToReplica")
     def connect_to_replica(self) -> Optional[bool]:
+        """
+        Set to connect to a replica instead of the primary node.
+        """
         return pulumi.get(self, "connect_to_replica")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -22919,29 +27068,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="replicaSet")
     def replica_set(self) -> Optional[str]:
+        """
+        The name of the mongo replicaset.
+        """
         return pulumi.get(self, "replica_set")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -22963,19 +27124,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMongoShardedClusterResult(dict):
     def __init__(__self__, *,
                  auth_database: Optional[str] = None,
@@ -22988,21 +27155,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str auth_database: The authentication database to use.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -23026,35 +27199,41 @@
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
     def auth_database(self) -> Optional[str]:
+        """
+        The authentication database to use.
+        """
         return pulumi.get(self, "auth_database")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -23068,19 +27247,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -23102,19 +27287,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMtlsMysqlResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -23133,21 +27324,33 @@
                  secret_store_id: Optional[str] = None,
                  server_name: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str server_name: Server name for TLS verification (unverified by StrongDM if empty)
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
             pulumi.set(__self__, "client_certificate", client_certificate)
@@ -23184,49 +27387,64 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -23240,42 +27458,57 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
+        """
+        Server name for TLS verification (unverified by StrongDM if empty)
+        """
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -23289,19 +27522,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMtlsPostgreResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -23319,21 +27558,32 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  server_name: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str certificate_authority: The CA to authenticate TLS connections with.
+        :param str client_certificate: The certificate to authenticate TLS connections with.
+        :param str client_key: The key to authenticate TLS connections with.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str server_name: Server name for TLS verification (unverified by StrongDM if empty)
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
             pulumi.set(__self__, "client_certificate", client_certificate)
@@ -23368,49 +27618,64 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="certificateAuthority")
     def certificate_authority(self) -> Optional[str]:
+        """
+        The CA to authenticate TLS connections with.
+        """
         return pulumi.get(self, "certificate_authority")
 
     @property
     @pulumi.getter(name="clientCertificate")
     def client_certificate(self) -> Optional[str]:
+        """
+        The certificate to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_certificate")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> Optional[str]:
+        """
+        The key to authenticate TLS connections with.
+        """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -23424,42 +27689,57 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
+        """
+        Server name for TLS verification (unverified by StrongDM if empty)
+        """
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -23473,14 +27753,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceMysqlResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -23495,21 +27778,29 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -23538,34 +27829,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -23579,29 +27876,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -23623,19 +27932,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceNeptuneResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -23645,18 +27960,21 @@
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -23678,29 +27996,32 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -23714,19 +28035,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -23765,18 +28092,26 @@
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str access_key: The Access Key ID to use to authenticate.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str endpoint: The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str region: The AWS region to connect to.
+        :param str role_arn: The role to assume after logging in.
+        :param str role_external_id: The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        :param str secret_access_key: The Secret Access Key to use to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -23807,35 +28142,41 @@
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
+        """
+        The Access Key ID to use to authenticate.
+        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
+        """
+        The neptune endpoint to connect to as in endpoint.region.neptune.amazonaws.com
+        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -23849,39 +28190,57 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to connect to.
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
+        """
+        The role to assume after logging in.
+        """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
+        """
+        The external ID to associate with assume role requests. Does nothing if a role ARN is not provided.
+        """
         return pulumi.get(self, "role_external_id")
 
     @property
     @pulumi.getter(name="secretAccessKey")
     def secret_access_key(self) -> Optional[str]:
+        """
+        The Secret Access Key to use to authenticate.
+        """
         return pulumi.get(self, "secret_access_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -23919,21 +28278,28 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -23960,34 +28326,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24001,24 +28373,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -24040,19 +28421,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourcePostgreResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -24066,21 +28453,28 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -24107,34 +28501,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24148,29 +28548,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -24192,14 +28604,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourcePrestoResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -24213,21 +28628,28 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -24254,34 +28676,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24295,24 +28723,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -24334,19 +28771,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceRabbitmqAmqp091Result(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -24359,21 +28802,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -24398,29 +28847,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24434,24 +28886,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -24473,19 +28934,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceRawTcpResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -24495,18 +28962,21 @@
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -24528,29 +28998,32 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24564,19 +29037,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -24613,21 +29092,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param bool downgrade_nla_connections: When set, network level authentication will not be used. May resolve unexpected authentication errors to older servers. When set, healthchecks cannot detect if a provided username / password pair is correct.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if downgrade_nla_connections is not None:
             pulumi.set(__self__, "downgrade_nla_connections", downgrade_nla_connections)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -24652,34 +29137,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="downgradeNlaConnections")
     def downgrade_nla_connections(self) -> Optional[bool]:
+        """
+        When set, network level authentication will not be used. May resolve unexpected authentication errors to older servers. When set, healthchecks cannot detect if a provided username / password pair is correct.
+        """
         return pulumi.get(self, "downgrade_nla_connections")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24693,24 +29184,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -24732,14 +29232,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceRediResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -24752,21 +29255,27 @@
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool tls_required: If set, TLS must be used to connect to this resource.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -24791,29 +29300,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24827,24 +29339,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -24866,19 +29387,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
+        """
+        If set, TLS must be used to connect to this resource.
+        """
         return pulumi.get(self, "tls_required")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceRedshiftResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -24892,21 +29419,28 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -24933,34 +29467,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -24974,29 +29514,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -25018,14 +29570,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSingleStoreResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -25040,21 +29595,29 @@
                  require_native_auth: Optional[bool] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  use_azure_single_server_usernames: Optional[bool] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param bool require_native_auth: Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param bool use_azure_single_server_usernames: If true, appends the hostname to the username when hitting a database.azure.com address
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -25083,34 +29646,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -25124,29 +29693,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="requireNativeAuth")
     def require_native_auth(self) -> Optional[bool]:
+        """
+        Whether native auth (mysql_native_password) is used for all connections (for backwards compatibility)
+        """
         return pulumi.get(self, "require_native_auth")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -25168,19 +29749,25 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="useAzureSingleServerUsernames")
     def use_azure_single_server_usernames(self) -> Optional[bool]:
+        """
+        If true, appends the hostname to the username when hitting a database.azure.com address
+        """
         return pulumi.get(self, "use_azure_single_server_usernames")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSnowflakeResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -25193,21 +29780,27 @@
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str schema: The Schema to use to direct initial requests.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -25232,34 +29825,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -25273,24 +29872,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -25312,14 +29920,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSnowsightResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -25329,18 +29940,21 @@
                  name: Optional[str] = None,
                  port_override: Optional[int] = None,
                  saml_metadata: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str healthcheck_username: The StrongDM user email to use for healthchecks.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str saml_metadata: The Metadata for your snowflake IDP integration
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -25362,29 +29976,32 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter(name="healthcheckUsername")
     def healthcheck_username(self) -> Optional[str]:
+        """
+        The StrongDM user email to use for healthchecks.
+        """
         return pulumi.get(self, "healthcheck_username")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -25398,19 +30015,25 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="samlMetadata")
     def saml_metadata(self) -> Optional[str]:
+        """
+        The Metadata for your snowflake IDP integration
+        """
         return pulumi.get(self, "saml_metadata")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -25449,21 +30072,29 @@
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str schema: The Schema to use to direct initial requests.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -25492,34 +30123,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -25533,34 +30170,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -25582,14 +30234,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSqlServerAzureAdResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -25605,22 +30260,31 @@
                  schema: Optional[str] = None,
                  secret: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str client_id: The Azure AD application (client) ID with which to authenticate.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str schema: The Schema to use to direct initial requests.
+        :param str secret: The Azure AD client secret (application password) with which to authenticate.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * sql_server_kerberos_ad:
+        :param str tenant_id: The Azure AD directory (tenant) ID with which to authenticate.
+               * sql_server_kerberos_ad:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
         if database is not None:
             pulumi.set(__self__, "database", database)
@@ -25651,39 +30315,48 @@
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> Optional[str]:
+        """
+        The Azure AD application (client) ID with which to authenticate.
+        """
         return pulumi.get(self, "client_id")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -25697,34 +30370,49 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter
     def secret(self) -> Optional[str]:
+        """
+        The Azure AD client secret (application password) with which to authenticate.
+        """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -25747,14 +30435,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
+        The Azure AD directory (tenant) ID with which to authenticate.
         * sql_server_kerberos_ad:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
 class GetResourceResourceSqlServerKerberosAdResult(dict):
@@ -25774,21 +30463,32 @@
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  server_spn: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
+        :param str keytab: The keytab file in base64 format containing an entry with the principal name (username@realm) and key version number with which to authenticate.
+        :param str krb_config: The Kerberos 5 configuration file (krb5.conf) specifying the Active Directory server (KDC) for the configured realm.
         :param str name: Unique human-readable name of the Resource.
+        :param bool override_database: If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str realm: The Active Directory domain (realm) to which the configured username belongs.
+        :param str schema: The Schema to use to direct initial requests.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str server_spn: The Service Principal Name of the Microsoft SQL Server instance in Active Directory.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -25823,98 +30523,128 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def keytab(self) -> Optional[str]:
+        """
+        The keytab file in base64 format containing an entry with the principal name (username@realm) and key version number with which to authenticate.
+        """
         return pulumi.get(self, "keytab")
 
     @property
     @pulumi.getter(name="krbConfig")
     def krb_config(self) -> Optional[str]:
+        """
+        The Kerberos 5 configuration file (krb5.conf) specifying the Active Directory server (KDC) for the configured realm.
+        """
         return pulumi.get(self, "krb_config")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="overrideDatabase")
     def override_database(self) -> Optional[bool]:
+        """
+        If set, the database configured cannot be changed by users. This setting is not recommended for most use cases, as some clients will insist their database has changed when it has not, leading to user confusion.
+        """
         return pulumi.get(self, "override_database")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter
     def realm(self) -> Optional[str]:
+        """
+        The Active Directory domain (realm) to which the configured username belongs.
+        """
         return pulumi.get(self, "realm")
 
     @property
     @pulumi.getter
     def schema(self) -> Optional[str]:
+        """
+        The Schema to use to direct initial requests.
+        """
         return pulumi.get(self, "schema")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="serverSpn")
     def server_spn(self) -> Optional[str]:
+        """
+        The Service Principal Name of the Microsoft SQL Server instance in Active Directory.
+        """
         return pulumi.get(self, "server_spn")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
@@ -25928,14 +30658,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSshResult(dict):
     def __init__(__self__, *,
                  public_key: str,
@@ -25950,21 +30683,29 @@
                  port_forwarding: Optional[bool] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str public_key: The public key to append to a server's authorized keys. This will be generated after resource creation.
+        :param bool allow_deprecated_key_exchanges: Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
+        :param str key_type: The key type to use e.g. rsa-2048 or ed25519
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param bool port_forwarding: Whether port forwarding is allowed through this server.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         pulumi.set(__self__, "public_key", public_key)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -25991,76 +30732,97 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> str:
+        """
+        The public key to append to a server's authorized keys. This will be generated after resource creation.
+        """
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
     def allow_deprecated_key_exchanges(self) -> Optional[bool]:
+        """
+        Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        """
         return pulumi.get(self, "allow_deprecated_key_exchanges")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="keyType")
     def key_type(self) -> Optional[str]:
+        """
+        The key type to use e.g. rsa-2048 or ed25519
+        """
         return pulumi.get(self, "key_type")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portForwarding")
     def port_forwarding(self) -> Optional[bool]:
+        """
+        Whether port forwarding is allowed through this server.
+        """
         return pulumi.get(self, "port_forwarding")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -26082,14 +30844,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSshCertResult(dict):
     def __init__(__self__, *,
                  allow_deprecated_key_exchanges: Optional[bool] = None,
@@ -26105,21 +30870,30 @@
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param bool allow_deprecated_key_exchanges: Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
+        :param str key_type: The key type to use e.g. rsa-2048 or ed25519
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param bool port_forwarding: Whether port forwarding is allowed through this server.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str remote_identity_group_id: The ID of the remote identity group to use for remote identity connections.
+        :param str remote_identity_healthcheck_username: The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -26149,81 +30923,105 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
     def allow_deprecated_key_exchanges(self) -> Optional[bool]:
+        """
+        Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        """
         return pulumi.get(self, "allow_deprecated_key_exchanges")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="keyType")
     def key_type(self) -> Optional[str]:
+        """
+        The key type to use e.g. rsa-2048 or ed25519
+        """
         return pulumi.get(self, "key_type")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portForwarding")
     def port_forwarding(self) -> Optional[bool]:
+        """
+        Whether port forwarding is allowed through this server.
+        """
         return pulumi.get(self, "port_forwarding")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="remoteIdentityGroupId")
     def remote_identity_group_id(self) -> Optional[str]:
+        """
+        The ID of the remote identity group to use for remote identity connections.
+        """
         return pulumi.get(self, "remote_identity_group_id")
 
     @property
     @pulumi.getter(name="remoteIdentityHealthcheckUsername")
     def remote_identity_healthcheck_username(self) -> Optional[str]:
+        """
+        The username to use for healthchecks, when clients otherwise connect with their own remote identity username.
+        """
         return pulumi.get(self, "remote_identity_healthcheck_username")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -26245,14 +31043,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSshCustomerKeyResult(dict):
     def __init__(__self__, *,
                  allow_deprecated_key_exchanges: Optional[bool] = None,
@@ -26266,21 +31067,28 @@
                  port_override: Optional[int] = None,
                  private_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param bool allow_deprecated_key_exchanges: Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param bool port_forwarding: Whether port forwarding is allowed through this server.
+        :param int port_override: The local port used by clients to connect to this resource.
+        :param str private_key: The private key used to authenticate with the server.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -26306,35 +31114,41 @@
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
     def allow_deprecated_key_exchanges(self) -> Optional[bool]:
+        """
+        Whether deprecated, insecure key exchanges are allowed for use to connect to the target ssh server.
+        """
         return pulumi.get(self, "allow_deprecated_key_exchanges")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -26348,29 +31162,41 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portForwarding")
     def port_forwarding(self) -> Optional[bool]:
+        """
+        Whether port forwarding is allowed through this server.
+        """
         return pulumi.get(self, "port_forwarding")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> Optional[str]:
+        """
+        The private key used to authenticate with the server.
+        """
         return pulumi.get(self, "private_key")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -26392,14 +31218,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSybaseResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -26411,21 +31240,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -26448,29 +31282,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -26484,24 +31321,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -26523,14 +31369,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceSybaseIqResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -26542,21 +31391,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -26579,29 +31433,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -26615,24 +31472,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -26654,14 +31520,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceTeradataResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -26673,21 +31542,26 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
@@ -26710,29 +31584,32 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -26746,24 +31623,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -26785,14 +31671,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetResourceResourceTrinoResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
@@ -26805,21 +31694,27 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
-        :param str bind_interface: Bind interface
+        :param str bind_interface: The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
+        :param str database: The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str hostname: The host to dial to initiate a connection from the egress node to this resource.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
+        :param str password: The password to authenticate with.
+        :param int port: The port to dial to initiate a connection from the egress node to this resource.
+        :param int port_override: The local port used by clients to connect to this resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str username: The username to authenticate with.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -26844,34 +31739,40 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
-        Bind interface
+        The bind interface is the IP address to which the port override of a resource is bound (for example, 127.0.0.1). It is automatically generated if not provided.
         """
         return pulumi.get(self, "bind_interface")
 
     @property
     @pulumi.getter
     def database(self) -> Optional[str]:
+        """
+        The initial database to connect to. This setting does not by itself prevent switching to another database after connecting.
+        """
         return pulumi.get(self, "database")
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
+        """
+        The host to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the Resource.
@@ -26885,24 +31786,33 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
+        """
+        The password to authenticate with.
+        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
+        """
+        The port to dial to initiate a connection from the egress node to this resource.
+        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
+        """
+        The local port used by clients to connect to this resource.
+        """
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
@@ -26924,14 +31834,17 @@
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
+        """
+        The username to authenticate with.
+        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetRoleRoleResult(dict):
     def __init__(__self__, *,
                  managed_by: str,
@@ -27078,14 +31991,15 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  region: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
+        :param str region: The AWS region to target e.g. us-east-1
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if region is not None:
@@ -27108,14 +32022,17 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
+        """
+        The AWS region to target e.g. us-east-1
+        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -27130,15 +32047,16 @@
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  vault_uri: Optional[str] = None):
         """
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str vault_uri: * cyberark_conjur:
+        :param str vault_uri: The URI of the key vault to target e.g. https://myvault.vault.azure.net
+               * cyberark_conjur:
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
@@ -27169,27 +32087,29 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="vaultUri")
     def vault_uri(self) -> Optional[str]:
         """
+        The URI of the key vault to target e.g. https://myvault.vault.azure.net
         * cyberark_conjur:
         """
         return pulumi.get(self, "vault_uri")
 
 
 @pulumi.output_type
 class GetSecretStoreSecretStoreCyberarkConjurResult(dict):
     def __init__(__self__, *,
                  app_url: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str app_url: The URL of the Cyberark instance
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if app_url is not None:
             pulumi.set(__self__, "app_url", app_url)
         if id is not None:
@@ -27198,14 +32118,17 @@
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="appUrl")
     def app_url(self) -> Optional[str]:
+        """
+        The URL of the Cyberark instance
+        """
         return pulumi.get(self, "app_url")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the SecretStore.
@@ -27233,14 +32156,15 @@
 class GetSecretStoreSecretStoreCyberarkPamResult(dict):
     def __init__(__self__, *,
                  app_url: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str app_url: The URL of the Cyberark instance
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if app_url is not None:
             pulumi.set(__self__, "app_url", app_url)
         if id is not None:
@@ -27249,14 +32173,17 @@
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="appUrl")
     def app_url(self) -> Optional[str]:
+        """
+        The URL of the Cyberark instance
+        """
         return pulumi.get(self, "app_url")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the SecretStore.
@@ -27284,14 +32211,15 @@
 class GetSecretStoreSecretStoreCyberarkPamExperimentalResult(dict):
     def __init__(__self__, *,
                  app_url: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str app_url: The URL of the Cyberark instance
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if app_url is not None:
             pulumi.set(__self__, "app_url", app_url)
         if id is not None:
@@ -27300,14 +32228,17 @@
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="appUrl")
     def app_url(self) -> Optional[str]:
+        """
+        The URL of the Cyberark instance
+        """
         return pulumi.get(self, "app_url")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the SecretStore.
@@ -27338,16 +32269,18 @@
                  name: Optional[str] = None,
                  server_url: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_name: Optional[str] = None):
         """
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
+        :param str server_url: The URL of the Delinea instance
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_name: * gcp_store:
+        :param str tenant_name: The tenant name to target
+               * gcp_store:
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if server_url is not None:
             pulumi.set(__self__, "server_url", server_url)
@@ -27371,28 +32304,32 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="serverUrl")
     def server_url(self) -> Optional[str]:
+        """
+        The URL of the Delinea instance
+        """
         return pulumi.get(self, "server_url")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantName")
     def tenant_name(self) -> Optional[str]:
         """
+        The tenant name to target
         * gcp_store:
         """
         return pulumi.get(self, "tenant_name")
 
 
 @pulumi.output_type
 class GetSecretStoreSecretStoreGcpStoreResult(dict):
@@ -27400,14 +32337,15 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  project_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
+        :param str project_id: The GCP project ID to target.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project_id is not None:
@@ -27430,14 +32368,17 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[str]:
+        """
+        The GCP project ID to target.
+        """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -27452,14 +32393,16 @@
                  name: Optional[str] = None,
                  namespace: Optional[str] = None,
                  server_address: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str server_address: The URL of the Vault to target
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
@@ -27484,19 +32427,25 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="serverAddress")
     def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
         return pulumi.get(self, "server_address")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -27512,16 +32461,21 @@
                  client_key_path: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  namespace: Optional[str] = None,
                  server_address: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str ca_cert_path: A path to a CA file accessible by a Node
+        :param str client_cert_path: A path to a client certificate file accessible by a Node
+        :param str client_key_path: A path to a client key file accessible by a Node
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str server_address: The URL of the Vault to target
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if ca_cert_path is not None:
             pulumi.set(__self__, "ca_cert_path", ca_cert_path)
         if client_cert_path is not None:
             pulumi.set(__self__, "client_cert_path", client_cert_path)
         if client_key_path is not None:
@@ -27536,24 +32490,33 @@
             pulumi.set(__self__, "server_address", server_address)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="caCertPath")
     def ca_cert_path(self) -> Optional[str]:
+        """
+        A path to a CA file accessible by a Node
+        """
         return pulumi.get(self, "ca_cert_path")
 
     @property
     @pulumi.getter(name="clientCertPath")
     def client_cert_path(self) -> Optional[str]:
+        """
+        A path to a client certificate file accessible by a Node
+        """
         return pulumi.get(self, "client_cert_path")
 
     @property
     @pulumi.getter(name="clientKeyPath")
     def client_key_path(self) -> Optional[str]:
+        """
+        A path to a client key file accessible by a Node
+        """
         return pulumi.get(self, "client_key_path")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Unique identifier of the SecretStore.
@@ -27567,19 +32530,25 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="serverAddress")
     def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
         return pulumi.get(self, "server_address")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -27594,14 +32563,16 @@
                  name: Optional[str] = None,
                  namespace: Optional[str] = None,
                  server_address: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
+        :param str namespace: The namespace to make requests within
+        :param str server_address: The URL of the Vault to target
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
@@ -27626,19 +32597,25 @@
         Unique human-readable name of the SecretStore.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[str]:
+        """
+        The namespace to make requests within
+        """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="serverAddress")
     def server_address(self) -> Optional[str]:
+        """
+        The URL of the Vault to target
+        """
         return pulumi.get(self, "server_address")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/provider.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/provider.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/remote_identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_id: Optional[pulumi.Input[str]] = None,
                  remote_identity_group_id: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        RemoteIdentities define the username to be used for a specific account
+         when connecting to a remote resource using that group.
+
         ## Import
 
         RemoteIdentity can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/remoteIdentity:RemoteIdentity example i-12345678
         ```
@@ -147,14 +150,17 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RemoteIdentityArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        RemoteIdentities define the username to be used for a specific account
+         when connecting to a remote resource using that group.
+
         ## Import
 
         RemoteIdentity can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/remoteIdentity:RemoteIdentity example i-12345678
         ```
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/resource.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                  aws: Optional[pulumi.Input['ResourceAwsArgs']] = None,
                  aws_console: Optional[pulumi.Input['ResourceAwsConsoleArgs']] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs']] = None,
                  azure: Optional[pulumi.Input['ResourceAzureArgs']] = None,
                  azure_certificate: Optional[pulumi.Input['ResourceAzureCertificateArgs']] = None,
                  azure_mysql: Optional[pulumi.Input['ResourceAzureMysqlArgs']] = None,
                  azure_postgres: Optional[pulumi.Input['ResourceAzurePostgresArgs']] = None,
+                 azure_postgres_managed_identity: Optional[pulumi.Input['ResourceAzurePostgresManagedIdentityArgs']] = None,
                  big_query: Optional[pulumi.Input['ResourceBigQueryArgs']] = None,
                  cassandra: Optional[pulumi.Input['ResourceCassandraArgs']] = None,
                  citus: Optional[pulumi.Input['ResourceCitusArgs']] = None,
                  clustrix: Optional[pulumi.Input['ResourceClustrixArgs']] = None,
                  cockroach: Optional[pulumi.Input['ResourceCockroachArgs']] = None,
                  db2_i: Optional[pulumi.Input['ResourceDb2IArgs']] = None,
                  db2_luw: Optional[pulumi.Input['ResourceDb2LuwArgs']] = None,
@@ -97,14 +98,16 @@
                  teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None,
                  trino: Optional[pulumi.Input['ResourceTrinoArgs']] = None):
         """
         The set of arguments for constructing a Resource resource.
         :param pulumi.Input['ResourceAwsConsoleArgs'] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs'] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input['ResourceAzurePostgresManagedIdentityArgs'] azure_postgres_managed_identity: AzurePostgresManagedIdentity is currently unstable, and its API may change, or it may be removed, without a major
+               version bump.
         :param pulumi.Input['ResourceMongoHostArgs'] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoReplicaSetArgs'] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoShardedClusterArgs'] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMtlsMysqlArgs'] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceSnowsightArgs'] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceTrinoArgs'] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
@@ -146,14 +149,16 @@
             pulumi.set(__self__, "azure", azure)
         if azure_certificate is not None:
             pulumi.set(__self__, "azure_certificate", azure_certificate)
         if azure_mysql is not None:
             pulumi.set(__self__, "azure_mysql", azure_mysql)
         if azure_postgres is not None:
             pulumi.set(__self__, "azure_postgres", azure_postgres)
+        if azure_postgres_managed_identity is not None:
+            pulumi.set(__self__, "azure_postgres_managed_identity", azure_postgres_managed_identity)
         if big_query is not None:
             pulumi.set(__self__, "big_query", big_query)
         if cassandra is not None:
             pulumi.set(__self__, "cassandra", cassandra)
         if citus is not None:
             pulumi.set(__self__, "citus", citus)
         if clustrix is not None:
@@ -462,14 +467,27 @@
         return pulumi.get(self, "azure_postgres")
 
     @azure_postgres.setter
     def azure_postgres(self, value: Optional[pulumi.Input['ResourceAzurePostgresArgs']]):
         pulumi.set(self, "azure_postgres", value)
 
     @property
+    @pulumi.getter(name="azurePostgresManagedIdentity")
+    def azure_postgres_managed_identity(self) -> Optional[pulumi.Input['ResourceAzurePostgresManagedIdentityArgs']]:
+        """
+        AzurePostgresManagedIdentity is currently unstable, and its API may change, or it may be removed, without a major
+        version bump.
+        """
+        return pulumi.get(self, "azure_postgres_managed_identity")
+
+    @azure_postgres_managed_identity.setter
+    def azure_postgres_managed_identity(self, value: Optional[pulumi.Input['ResourceAzurePostgresManagedIdentityArgs']]):
+        pulumi.set(self, "azure_postgres_managed_identity", value)
+
+    @property
     @pulumi.getter(name="bigQuery")
     def big_query(self) -> Optional[pulumi.Input['ResourceBigQueryArgs']]:
         return pulumi.get(self, "big_query")
 
     @big_query.setter
     def big_query(self, value: Optional[pulumi.Input['ResourceBigQueryArgs']]):
         pulumi.set(self, "big_query", value)
@@ -1035,14 +1053,15 @@
                  aws: Optional[pulumi.Input['ResourceAwsArgs']] = None,
                  aws_console: Optional[pulumi.Input['ResourceAwsConsoleArgs']] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs']] = None,
                  azure: Optional[pulumi.Input['ResourceAzureArgs']] = None,
                  azure_certificate: Optional[pulumi.Input['ResourceAzureCertificateArgs']] = None,
                  azure_mysql: Optional[pulumi.Input['ResourceAzureMysqlArgs']] = None,
                  azure_postgres: Optional[pulumi.Input['ResourceAzurePostgresArgs']] = None,
+                 azure_postgres_managed_identity: Optional[pulumi.Input['ResourceAzurePostgresManagedIdentityArgs']] = None,
                  big_query: Optional[pulumi.Input['ResourceBigQueryArgs']] = None,
                  cassandra: Optional[pulumi.Input['ResourceCassandraArgs']] = None,
                  citus: Optional[pulumi.Input['ResourceCitusArgs']] = None,
                  clustrix: Optional[pulumi.Input['ResourceClustrixArgs']] = None,
                  cockroach: Optional[pulumi.Input['ResourceCockroachArgs']] = None,
                  db2_i: Optional[pulumi.Input['ResourceDb2IArgs']] = None,
                  db2_luw: Optional[pulumi.Input['ResourceDb2LuwArgs']] = None,
@@ -1099,14 +1118,16 @@
                  teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None,
                  trino: Optional[pulumi.Input['ResourceTrinoArgs']] = None):
         """
         Input properties used for looking up and filtering Resource resources.
         :param pulumi.Input['ResourceAwsConsoleArgs'] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs'] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input['ResourceAzurePostgresManagedIdentityArgs'] azure_postgres_managed_identity: AzurePostgresManagedIdentity is currently unstable, and its API may change, or it may be removed, without a major
+               version bump.
         :param pulumi.Input['ResourceMongoHostArgs'] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoReplicaSetArgs'] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoShardedClusterArgs'] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMtlsMysqlArgs'] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceSnowsightArgs'] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceTrinoArgs'] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
@@ -1148,14 +1169,16 @@
             pulumi.set(__self__, "azure", azure)
         if azure_certificate is not None:
             pulumi.set(__self__, "azure_certificate", azure_certificate)
         if azure_mysql is not None:
             pulumi.set(__self__, "azure_mysql", azure_mysql)
         if azure_postgres is not None:
             pulumi.set(__self__, "azure_postgres", azure_postgres)
+        if azure_postgres_managed_identity is not None:
+            pulumi.set(__self__, "azure_postgres_managed_identity", azure_postgres_managed_identity)
         if big_query is not None:
             pulumi.set(__self__, "big_query", big_query)
         if cassandra is not None:
             pulumi.set(__self__, "cassandra", cassandra)
         if citus is not None:
             pulumi.set(__self__, "citus", citus)
         if clustrix is not None:
@@ -1464,14 +1487,27 @@
         return pulumi.get(self, "azure_postgres")
 
     @azure_postgres.setter
     def azure_postgres(self, value: Optional[pulumi.Input['ResourceAzurePostgresArgs']]):
         pulumi.set(self, "azure_postgres", value)
 
     @property
+    @pulumi.getter(name="azurePostgresManagedIdentity")
+    def azure_postgres_managed_identity(self) -> Optional[pulumi.Input['ResourceAzurePostgresManagedIdentityArgs']]:
+        """
+        AzurePostgresManagedIdentity is currently unstable, and its API may change, or it may be removed, without a major
+        version bump.
+        """
+        return pulumi.get(self, "azure_postgres_managed_identity")
+
+    @azure_postgres_managed_identity.setter
+    def azure_postgres_managed_identity(self, value: Optional[pulumi.Input['ResourceAzurePostgresManagedIdentityArgs']]):
+        pulumi.set(self, "azure_postgres_managed_identity", value)
+
+    @property
     @pulumi.getter(name="bigQuery")
     def big_query(self) -> Optional[pulumi.Input['ResourceBigQueryArgs']]:
         return pulumi.get(self, "big_query")
 
     @big_query.setter
     def big_query(self, value: Optional[pulumi.Input['ResourceBigQueryArgs']]):
         pulumi.set(self, "big_query", value)
@@ -2039,14 +2075,15 @@
                  aws: Optional[pulumi.Input[pulumi.InputType['ResourceAwsArgs']]] = None,
                  aws_console: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']]] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']]] = None,
                  azure: Optional[pulumi.Input[pulumi.InputType['ResourceAzureArgs']]] = None,
                  azure_certificate: Optional[pulumi.Input[pulumi.InputType['ResourceAzureCertificateArgs']]] = None,
                  azure_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']]] = None,
                  azure_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresArgs']]] = None,
+                 azure_postgres_managed_identity: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresManagedIdentityArgs']]] = None,
                  big_query: Optional[pulumi.Input[pulumi.InputType['ResourceBigQueryArgs']]] = None,
                  cassandra: Optional[pulumi.Input[pulumi.InputType['ResourceCassandraArgs']]] = None,
                  citus: Optional[pulumi.Input[pulumi.InputType['ResourceCitusArgs']]] = None,
                  clustrix: Optional[pulumi.Input[pulumi.InputType['ResourceClustrixArgs']]] = None,
                  cockroach: Optional[pulumi.Input[pulumi.InputType['ResourceCockroachArgs']]] = None,
                  db2_i: Optional[pulumi.Input[pulumi.InputType['ResourceDb2IArgs']]] = None,
                  db2_luw: Optional[pulumi.Input[pulumi.InputType['ResourceDb2LuwArgs']]] = None,
@@ -2113,14 +2150,16 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input[pulumi.InputType['ResourceAzurePostgresManagedIdentityArgs']] azure_postgres_managed_identity: AzurePostgresManagedIdentity is currently unstable, and its API may change, or it may be removed, without a major
+               version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoHostArgs']] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoReplicaSetArgs']] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoShardedClusterArgs']] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMtlsMysqlArgs']] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceTrinoArgs']] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
@@ -2171,14 +2210,15 @@
                  aws: Optional[pulumi.Input[pulumi.InputType['ResourceAwsArgs']]] = None,
                  aws_console: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']]] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']]] = None,
                  azure: Optional[pulumi.Input[pulumi.InputType['ResourceAzureArgs']]] = None,
                  azure_certificate: Optional[pulumi.Input[pulumi.InputType['ResourceAzureCertificateArgs']]] = None,
                  azure_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']]] = None,
                  azure_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresArgs']]] = None,
+                 azure_postgres_managed_identity: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresManagedIdentityArgs']]] = None,
                  big_query: Optional[pulumi.Input[pulumi.InputType['ResourceBigQueryArgs']]] = None,
                  cassandra: Optional[pulumi.Input[pulumi.InputType['ResourceCassandraArgs']]] = None,
                  citus: Optional[pulumi.Input[pulumi.InputType['ResourceCitusArgs']]] = None,
                  clustrix: Optional[pulumi.Input[pulumi.InputType['ResourceClustrixArgs']]] = None,
                  cockroach: Optional[pulumi.Input[pulumi.InputType['ResourceCockroachArgs']]] = None,
                  db2_i: Optional[pulumi.Input[pulumi.InputType['ResourceDb2IArgs']]] = None,
                  db2_luw: Optional[pulumi.Input[pulumi.InputType['ResourceDb2LuwArgs']]] = None,
@@ -2260,14 +2300,15 @@
             __props__.__dict__["aws"] = aws
             __props__.__dict__["aws_console"] = aws_console
             __props__.__dict__["aws_console_static_key_pair"] = aws_console_static_key_pair
             __props__.__dict__["azure"] = azure
             __props__.__dict__["azure_certificate"] = azure_certificate
             __props__.__dict__["azure_mysql"] = azure_mysql
             __props__.__dict__["azure_postgres"] = azure_postgres
+            __props__.__dict__["azure_postgres_managed_identity"] = azure_postgres_managed_identity
             __props__.__dict__["big_query"] = big_query
             __props__.__dict__["cassandra"] = cassandra
             __props__.__dict__["citus"] = citus
             __props__.__dict__["clustrix"] = clustrix
             __props__.__dict__["cockroach"] = cockroach
             __props__.__dict__["db2_i"] = db2_i
             __props__.__dict__["db2_luw"] = db2_luw
@@ -2350,14 +2391,15 @@
             aws: Optional[pulumi.Input[pulumi.InputType['ResourceAwsArgs']]] = None,
             aws_console: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']]] = None,
             aws_console_static_key_pair: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']]] = None,
             azure: Optional[pulumi.Input[pulumi.InputType['ResourceAzureArgs']]] = None,
             azure_certificate: Optional[pulumi.Input[pulumi.InputType['ResourceAzureCertificateArgs']]] = None,
             azure_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']]] = None,
             azure_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresArgs']]] = None,
+            azure_postgres_managed_identity: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresManagedIdentityArgs']]] = None,
             big_query: Optional[pulumi.Input[pulumi.InputType['ResourceBigQueryArgs']]] = None,
             cassandra: Optional[pulumi.Input[pulumi.InputType['ResourceCassandraArgs']]] = None,
             citus: Optional[pulumi.Input[pulumi.InputType['ResourceCitusArgs']]] = None,
             clustrix: Optional[pulumi.Input[pulumi.InputType['ResourceClustrixArgs']]] = None,
             cockroach: Optional[pulumi.Input[pulumi.InputType['ResourceCockroachArgs']]] = None,
             db2_i: Optional[pulumi.Input[pulumi.InputType['ResourceDb2IArgs']]] = None,
             db2_luw: Optional[pulumi.Input[pulumi.InputType['ResourceDb2LuwArgs']]] = None,
@@ -2419,14 +2461,16 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input[pulumi.InputType['ResourceAzurePostgresManagedIdentityArgs']] azure_postgres_managed_identity: AzurePostgresManagedIdentity is currently unstable, and its API may change, or it may be removed, without a major
+               version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoHostArgs']] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoReplicaSetArgs']] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoShardedClusterArgs']] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMtlsMysqlArgs']] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceTrinoArgs']] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
@@ -2451,14 +2495,15 @@
         __props__.__dict__["aws"] = aws
         __props__.__dict__["aws_console"] = aws_console
         __props__.__dict__["aws_console_static_key_pair"] = aws_console_static_key_pair
         __props__.__dict__["azure"] = azure
         __props__.__dict__["azure_certificate"] = azure_certificate
         __props__.__dict__["azure_mysql"] = azure_mysql
         __props__.__dict__["azure_postgres"] = azure_postgres
+        __props__.__dict__["azure_postgres_managed_identity"] = azure_postgres_managed_identity
         __props__.__dict__["big_query"] = big_query
         __props__.__dict__["cassandra"] = cassandra
         __props__.__dict__["citus"] = citus
         __props__.__dict__["clustrix"] = clustrix
         __props__.__dict__["cockroach"] = cockroach
         __props__.__dict__["db2_i"] = db2_i
         __props__.__dict__["db2_luw"] = db2_luw
@@ -2625,14 +2670,23 @@
 
     @property
     @pulumi.getter(name="azurePostgres")
     def azure_postgres(self) -> pulumi.Output[Optional['outputs.ResourceAzurePostgres']]:
         return pulumi.get(self, "azure_postgres")
 
     @property
+    @pulumi.getter(name="azurePostgresManagedIdentity")
+    def azure_postgres_managed_identity(self) -> pulumi.Output[Optional['outputs.ResourceAzurePostgresManagedIdentity']]:
+        """
+        AzurePostgresManagedIdentity is currently unstable, and its API may change, or it may be removed, without a major
+        version bump.
+        """
+        return pulumi.get(self, "azure_postgres_managed_identity")
+
+    @property
     @pulumi.getter(name="bigQuery")
     def big_query(self) -> pulumi.Output[Optional['outputs.ResourceBigQuery']]:
         return pulumi.get(self, "big_query")
 
     @property
     @pulumi.getter
     def cassandra(self) -> pulumi.Output[Optional['outputs.ResourceCassandra']]:
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/role.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/role.py`

 * *Files 10% similar despite different names*

```diff
@@ -145,14 +145,47 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_rules: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
+        A Role has a list of access rules which determine which Resources the members
+         of the Role have access to. An Account can be a member of multiple Roles via
+         AccountAttachments.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import json
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        engineers = sdm.Role("engineers", tags={
+            "foo": "bar",
+        })
+        example_role = sdm.Role("example-role", access_rules=json.dumps([
+            {
+                "tags": {
+                    "env": "staging",
+                },
+            },
+            {
+                "type": "postgres",
+                "tags": {
+                    "region": "us-west",
+                    "env": "dev",
+                },
+            },
+            {
+                "ids": ["rs-093e6f3061eb4dad"],
+            },
+        ]))
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         Role can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/role:Role example r-12345678
         ```
@@ -166,14 +199,47 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[RoleArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        A Role has a list of access rules which determine which Resources the members
+         of the Role have access to. An Account can be a member of multiple Roles via
+         AccountAttachments.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import json
+        import pierskarsenbarg_pulumi_sdm as sdm
+
+        engineers = sdm.Role("engineers", tags={
+            "foo": "bar",
+        })
+        example_role = sdm.Role("example-role", access_rules=json.dumps([
+            {
+                "tags": {
+                    "env": "staging",
+                },
+            },
+            {
+                "type": "postgres",
+                "tags": {
+                    "region": "us-west",
+                    "env": "dev",
+                },
+            },
+            {
+                "ids": ["rs-093e6f3061eb4dad"],
+            },
+        ]))
+        ```
+        This resource can be imported using the import command.
+
         ## Import
 
         Role can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/role:Role example r-12345678
         ```
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm/secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/secret_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,18 @@
                  delinea_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreDelineaStoreArgs']]] = None,
                  gcp_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreGcpStoreArgs']]] = None,
                  vault_approle: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultApproleArgs']]] = None,
                  vault_tls: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTlsArgs']]] = None,
                  vault_token: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTokenArgs']]] = None,
                  __props__=None):
         """
+        A SecretStore is a server where resource secrets (passwords, keys) are stored.
+         Coming soon support for HashiCorp Vault and AWS Secret Store.
+        This resource can be imported using the import command.
+
         ## Import
 
         SecretStore can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/secretStore:SecretStore example se-12345678
         ```
@@ -314,14 +318,18 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SecretStoreArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        A SecretStore is a server where resource secrets (passwords, keys) are stored.
+         Coming soon support for HashiCorp Vault and AWS Secret Store.
+        This resource can be imported using the import command.
+
         ## Import
 
         SecretStore can be imported using the id, e.g.,
 
         ```sh
          $ pulumi import sdm:index/secretStore:SecretStore example se-12345678
         ```
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg-pulumi-sdm
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt` & `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.2.0/setup.py` & `pierskarsenbarg_pulumi_sdm-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.2.0"
-PLUGIN_VERSION = "1.2.0"
+VERSION = "1.3.0"
+PLUGIN_VERSION = "1.3.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'sdm', PLUGIN_VERSION, '--server', 'github://api.github.com/pierskarsenbarg/pulumi-sdm'])
         except OSError as error:
```

