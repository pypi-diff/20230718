# Comparing `tmp/pulumi_frontegg-0.2.26.tar.gz` & `tmp/pulumi_frontegg-0.2.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_frontegg-0.2.26.tar", last modified: Thu Jun 15 06:06:30 2023, max compression
+gzip compressed data, was "pulumi_frontegg-0.2.27.tar", last modified: Tue Jul 18 19:30:28 2023, max compression
```

## Comparing `pulumi_frontegg-0.2.26.tar` & `pulumi_frontegg-0.2.27.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.901745 pulumi_frontegg-0.2.26/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 06:06:30.901745 pulumi_frontegg-0.2.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.897745 pulumi_frontegg-0.2.26/pulumi_frontegg/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67966 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/allowed_origin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.897745 pulumi_frontegg-0.2.26/pulumi_frontegg/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/get_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    66319 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/permission_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    19522 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    84582 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.897745 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:06:30.901745 pulumi_frontegg-0.2.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:28.008392 pulumi_frontegg-0.2.27/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-18 19:30:28.008392 pulumi_frontegg-0.2.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:28.004392 pulumi_frontegg-0.2.27/pulumi_frontegg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67966 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/allowed_origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:28.008392 pulumi_frontegg-0.2.27/pulumi_frontegg/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/get_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66319 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/permission_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84582 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/pulumi_frontegg/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:28.008392 pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-18 19:30:28.000000 pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-18 19:30:28.000000 pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:30:28.000000 pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:30:28.000000 pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 19:30:28.000000 pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 19:30:28.000000 pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:30:28.008392 pulumi_frontegg-0.2.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-18 19:30:27.000000 pulumi_frontegg-0.2.27/setup.py
```

### Comparing `pulumi_frontegg-0.2.26/PKG-INFO` & `pulumi_frontegg-0.2.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_frontegg
-Version: 0.2.26
+Version: 0.2.27
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/__init__.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/_inputs.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/_utilities.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.26/"
+	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.27/"
```

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/allowed_origin.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/allowed_origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/config/vars.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/config/vars.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,21 @@
     def client_id(self) -> Optional[str]:
         """
         The client ID for a Frontegg portal API key.
         """
         return __config__.get('clientId')
 
     @property
+    def environment_id(self) -> Optional[str]:
+        """
+        The client ID from environment settings.
+        """
+        return __config__.get('environmentId')
+
+    @property
     def portal_base_url(self) -> Optional[str]:
         """
         The Frontegg portal url. Override to change region. Defaults to EU url.
         """
         return __config__.get('portalBaseUrl')
 
     @property
```

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/get_permission.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/get_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/outputs.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/permission.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/permission_category.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/permission_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/provider.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  client_id: pulumi.Input[str],
                  secret_key: pulumi.Input[str],
                  api_base_url: Optional[pulumi.Input[str]] = None,
+                 environment_id: Optional[pulumi.Input[str]] = None,
                  portal_base_url: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] client_id: The client ID for a Frontegg portal API key.
         :param pulumi.Input[str] secret_key: The corresponding secret key for the API key.
         :param pulumi.Input[str] api_base_url: The Frontegg api url. Override to change region. Defaults to EU url.
+        :param pulumi.Input[str] environment_id: The client ID from environment settings.
         :param pulumi.Input[str] portal_base_url: The Frontegg portal url. Override to change region. Defaults to EU url.
         """
         pulumi.set(__self__, "client_id", client_id)
         pulumi.set(__self__, "secret_key", secret_key)
         if api_base_url is not None:
             pulumi.set(__self__, "api_base_url", api_base_url)
+        if environment_id is not None:
+            pulumi.set(__self__, "environment_id", environment_id)
         if portal_base_url is not None:
             pulumi.set(__self__, "portal_base_url", portal_base_url)
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Input[str]:
         """
@@ -65,14 +69,26 @@
         return pulumi.get(self, "api_base_url")
 
     @api_base_url.setter
     def api_base_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_base_url", value)
 
     @property
+    @pulumi.getter(name="environmentId")
+    def environment_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The client ID from environment settings.
+        """
+        return pulumi.get(self, "environment_id")
+
+    @environment_id.setter
+    def environment_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "environment_id", value)
+
+    @property
     @pulumi.getter(name="portalBaseUrl")
     def portal_base_url(self) -> Optional[pulumi.Input[str]]:
         """
         The Frontegg portal url. Override to change region. Defaults to EU url.
         """
         return pulumi.get(self, "portal_base_url")
 
@@ -84,27 +100,29 @@
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_base_url: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
+                 environment_id: Optional[pulumi.Input[str]] = None,
                  portal_base_url: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The provider type for the frontegg package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] api_base_url: The Frontegg api url. Override to change region. Defaults to EU url.
         :param pulumi.Input[str] client_id: The client ID for a Frontegg portal API key.
+        :param pulumi.Input[str] environment_id: The client ID from environment settings.
         :param pulumi.Input[str] portal_base_url: The Frontegg portal url. Override to change region. Defaults to EU url.
         :param pulumi.Input[str] secret_key: The corresponding secret key for the API key.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -129,14 +147,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_base_url: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
+                 environment_id: Optional[pulumi.Input[str]] = None,
                  portal_base_url: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -144,19 +163,20 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["api_base_url"] = api_base_url
             if client_id is None and not opts.urn:
                 raise TypeError("Missing required property 'client_id'")
             __props__.__dict__["client_id"] = client_id
+            __props__.__dict__["environment_id"] = None if environment_id is None else pulumi.Output.secret(environment_id)
             __props__.__dict__["portal_base_url"] = portal_base_url
             if secret_key is None and not opts.urn:
                 raise TypeError("Missing required property 'secret_key'")
             __props__.__dict__["secret_key"] = None if secret_key is None else pulumi.Output.secret(secret_key)
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secretKey"])
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["environmentId", "secretKey"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'frontegg',
             resource_name,
             __props__,
             opts)
 
@@ -173,14 +193,22 @@
     def client_id(self) -> pulumi.Output[str]:
         """
         The client ID for a Frontegg portal API key.
         """
         return pulumi.get(self, "client_id")
 
     @property
+    @pulumi.getter(name="environmentId")
+    def environment_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        The client ID from environment settings.
+        """
+        return pulumi.get(self, "environment_id")
+
+    @property
     @pulumi.getter(name="portalBaseUrl")
     def portal_base_url(self) -> pulumi.Output[Optional[str]]:
         """
         The Frontegg portal url. Override to change region. Defaults to EU url.
         """
         return pulumi.get(self, "portal_base_url")
```

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/redirect_uri.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/role.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/tenant.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/user.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/webhook.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/webhook.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,33 +15,29 @@
 class WebhookArgs:
     def __init__(__self__, *,
                  description: pulumi.Input[str],
                  enabled: pulumi.Input[bool],
                  events: pulumi.Input[Sequence[pulumi.Input[str]]],
                  secret: pulumi.Input[str],
                  url: pulumi.Input[str],
-                 environment_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Webhook resource.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] secret: A secret to include with the event.
         :param pulumi.Input[str] url: The URL to send events to.
-        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "events", events)
         pulumi.set(__self__, "secret", secret)
         pulumi.set(__self__, "url", url)
-        if environment_id is not None:
-            pulumi.set(__self__, "environment_id", environment_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Input[str]:
         """
@@ -98,26 +94,14 @@
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
-    @pulumi.getter(name="environmentId")
-    def environment_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The ID of the environment of webhook.
-        """
-        return pulumi.get(self, "environment_id")
-
-    @environment_id.setter
-    def environment_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "environment_id", value)
-
-    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         A human-readable name for the webhook.
         """
         return pulumi.get(self, "name")
 
@@ -128,42 +112,38 @@
 
 @pulumi.input_type
 class _WebhookState:
     def __init__(__self__, *,
                  created_at: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
-                 environment_id: Optional[pulumi.Input[str]] = None,
                  events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  vendor_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Webhook resources.
         :param pulumi.Input[str] created_at: The timestamp at which the webhook was created.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
-        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         :param pulumi.Input[str] secret: A secret to include with the event.
         :param pulumi.Input[str] type: The type of the webhook.
         :param pulumi.Input[str] url: The URL to send events to.
         :param pulumi.Input[str] vendor_id: The ID of the vendor that owns the webhook.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
-        if environment_id is not None:
-            pulumi.set(__self__, "environment_id", environment_id)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if secret is not None:
             pulumi.set(__self__, "secret", secret)
         if type is not None:
@@ -206,26 +186,14 @@
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
-    @pulumi.getter(name="environmentId")
-    def environment_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The ID of the environment of webhook.
-        """
-        return pulumi.get(self, "environment_id")
-
-    @environment_id.setter
-    def environment_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "environment_id", value)
-
-    @property
     @pulumi.getter
     def events(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The names of the events to subscribe to.
         """
         return pulumi.get(self, "events")
 
@@ -297,27 +265,25 @@
 class Webhook(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
-                 environment_id: Optional[pulumi.Input[str]] = None,
                  events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Webhook resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
-        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         :param pulumi.Input[str] secret: A secret to include with the event.
         :param pulumi.Input[str] url: The URL to send events to.
         """
         ...
     @overload
@@ -340,15 +306,14 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
-                 environment_id: Optional[pulumi.Input[str]] = None,
                  events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -360,15 +325,14 @@
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
             __props__.__dict__["description"] = description
             if enabled is None and not opts.urn:
                 raise TypeError("Missing required property 'enabled'")
             __props__.__dict__["enabled"] = enabled
-            __props__.__dict__["environment_id"] = environment_id
             if events is None and not opts.urn:
                 raise TypeError("Missing required property 'events'")
             __props__.__dict__["events"] = events
             __props__.__dict__["name"] = name
             if secret is None and not opts.urn:
                 raise TypeError("Missing required property 'secret'")
             __props__.__dict__["secret"] = secret
@@ -387,15 +351,14 @@
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             enabled: Optional[pulumi.Input[bool]] = None,
-            environment_id: Optional[pulumi.Input[str]] = None,
             events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             secret: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
             url: Optional[pulumi.Input[str]] = None,
             vendor_id: Optional[pulumi.Input[str]] = None) -> 'Webhook':
         """
@@ -404,30 +367,28 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The timestamp at which the webhook was created.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
-        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         :param pulumi.Input[str] secret: A secret to include with the event.
         :param pulumi.Input[str] type: The type of the webhook.
         :param pulumi.Input[str] url: The URL to send events to.
         :param pulumi.Input[str] vendor_id: The ID of the vendor that owns the webhook.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _WebhookState.__new__(_WebhookState)
 
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["description"] = description
         __props__.__dict__["enabled"] = enabled
-        __props__.__dict__["environment_id"] = environment_id
         __props__.__dict__["events"] = events
         __props__.__dict__["name"] = name
         __props__.__dict__["secret"] = secret
         __props__.__dict__["type"] = type
         __props__.__dict__["url"] = url
         __props__.__dict__["vendor_id"] = vendor_id
         return Webhook(resource_name, opts=opts, __props__=__props__)
@@ -453,22 +414,14 @@
     def enabled(self) -> pulumi.Output[bool]:
         """
         Whether the webhook is enabled.
         """
         return pulumi.get(self, "enabled")
 
     @property
-    @pulumi.getter(name="environmentId")
-    def environment_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The ID of the environment of webhook.
-        """
-        return pulumi.get(self, "environment_id")
-
-    @property
     @pulumi.getter
     def events(self) -> pulumi.Output[Sequence[str]]:
         """
         The names of the events to subscribe to.
         """
         return pulumi.get(self, "events")
```

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg/workspace.py` & `pulumi_frontegg-0.2.27/pulumi_frontegg/workspace.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/PKG-INFO` & `pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-frontegg
-Version: 0.2.26
+Version: 0.2.27
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/SOURCES.txt` & `pulumi_frontegg-0.2.27/pulumi_frontegg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.26/setup.py` & `pulumi_frontegg-0.2.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = '0.2.26'
-PLUGIN_VERSION = '0.2.26'
+VERSION = '0.2.27'
+PLUGIN_VERSION = '0.2.27'
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'frontegg', PLUGIN_VERSION, '--server', 'https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.26/'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'frontegg', PLUGIN_VERSION, '--server', 'https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.27/'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the frontegg resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

