# Comparing `tmp/qctrl_client-7.1.0.tar.gz` & `tmp/qctrl_client-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_client-7.1.0.tar", max compression
+gzip compressed data, was "qctrl_client-7.2.0.tar", max compression
```

## Comparing `qctrl_client-7.1.0.tar` & `qctrl_client-7.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    36653 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/LICENSE
--rw-r--r--   0        0        0      214 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/README.md
--rw-r--r--   0        0        0     2614 2023-06-28 00:43:28.480008 qctrl_client-7.1.0/pyproject.toml
--rw-r--r--   0        0        0      747 2023-06-28 00:43:28.488008 qctrl_client-7.1.0/qctrlclient/__init__.py
--rw-r--r--   0        0        0      686 2023-06-28 00:43:28.496008 qctrl_client-7.1.0/qctrlclient/auth/__init__.py
--rw-r--r--   0        0        0     1831 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/base.py
--rw-r--r--   0        0        0     4969 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/cli.py
--rw-r--r--   0        0        0      972 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/helpers.py
--rw-r--r--   0        0        0     1042 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/keycloak.py
--rw-r--r--   0        0        0     4308 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/oidc.py
--rw-r--r--   0        0        0     1801 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/password.py
--rw-r--r--   0        0        0     3096 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/redirect_listener.py
--rw-r--r--   0        0        0     1516 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/auth/service_account.py
--rw-r--r--   0        0        0     7742 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/client.py
--rw-r--r--   0        0        0      809 2023-06-28 00:43:28.492008 qctrl_client-7.1.0/qctrlclient/core/__init__.py
--rw-r--r--   0        0        0     2999 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/core/functions.py
--rw-r--r--   0        0        0      995 2023-06-28 00:43:06.079832 qctrl_client-7.1.0/qctrlclient/core/products.py
--rw-r--r--   0        0        0      638 2023-06-28 00:43:28.492008 qctrl_client-7.1.0/qctrlclient/core/router/__init__.py
--rw-r--r--   0        0        0    11628 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/core/router/api.py
--rw-r--r--   0        0        0     1189 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/core/router/base.py
--rw-r--r--   0        0        0     1197 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/core/router/local.py
--rw-r--r--   0        0        0     2677 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/core/settings.py
--rw-r--r--   0        0        0     1179 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/core/utils.py
--rw-r--r--   0        0        0     1329 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/defaults.py
--rw-r--r--   0        0        0     2172 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/exceptions.py
--rw-r--r--   0        0        0     1357 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/globals.py
--rw-r--r--   0        0        0     1424 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/pytest_plugin.py
--rw-r--r--   0        0        0      601 2023-06-28 00:43:28.496008 qctrl_client-7.1.0/qctrlclient/transports/__init__.py
--rw-r--r--   0        0        0     4625 2023-06-28 00:43:06.083832 qctrl_client-7.1.0/qctrlclient/transports/requests_transport.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/LICENSE
+-rw-r--r--   0        0        0      214 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/README.md
+-rw-r--r--   0        0        0     2614 2023-07-18 04:03:28.678655 qctrl_client-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-07-18 04:03:28.690655 qctrl_client-7.2.0/qctrlclient/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-18 04:03:28.690655 qctrl_client-7.2.0/qctrlclient/auth/__init__.py
+-rw-r--r--   0        0        0     1831 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/qctrlclient/auth/base.py
+-rw-r--r--   0        0        0     4969 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/qctrlclient/auth/cli.py
+-rw-r--r--   0        0        0      972 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/helpers.py
+-rw-r--r--   0        0        0     1042 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/keycloak.py
+-rw-r--r--   0        0        0     4308 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/oidc.py
+-rw-r--r--   0        0        0     1801 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/password.py
+-rw-r--r--   0        0        0     3096 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/redirect_listener.py
+-rw-r--r--   0        0        0     1516 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/service_account.py
+-rw-r--r--   0        0        0     7742 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/client.py
+-rw-r--r--   0        0        0      809 2023-07-18 04:03:28.686655 qctrl_client-7.2.0/qctrlclient/core/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/functions.py
+-rw-r--r--   0        0        0      995 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/products.py
+-rw-r--r--   0        0        0      638 2023-07-18 04:03:28.686655 qctrl_client-7.2.0/qctrlclient/core/router/__init__.py
+-rw-r--r--   0        0        0    12547 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/router/api.py
+-rw-r--r--   0        0        0     1189 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/router/base.py
+-rw-r--r--   0        0        0     1197 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/router/local.py
+-rw-r--r--   0        0        0     2677 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/settings.py
+-rw-r--r--   0        0        0     1179 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/utils.py
+-rw-r--r--   0        0        0     1329 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/defaults.py
+-rw-r--r--   0        0        0     2172 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/exceptions.py
+-rw-r--r--   0        0        0     1357 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/globals.py
+-rw-r--r--   0        0        0     1424 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/pytest_plugin.py
+-rw-r--r--   0        0        0      601 2023-07-18 04:03:28.690655 qctrl_client-7.2.0/qctrlclient/transports/__init__.py
+-rw-r--r--   0        0        0     4625 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/transports/requests_transport.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.2.0/PKG-INFO
```

### Comparing `qctrl_client-7.1.0/LICENSE` & `qctrl_client-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/pyproject.toml` & `qctrl_client-7.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-client"
-version = "7.1.0"
+version = "7.2.0"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl_client-7.1.0/qctrlclient/__init__.py` & `qctrl_client-7.2.0/qctrlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/__init__.py` & `qctrl_client-7.2.0/qctrlclient/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/base.py` & `qctrl_client-7.2.0/qctrlclient/auth/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/cli.py` & `qctrl_client-7.2.0/qctrlclient/auth/cli.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/helpers.py` & `qctrl_client-7.2.0/qctrlclient/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/keycloak.py` & `qctrl_client-7.2.0/qctrlclient/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/oidc.py` & `qctrl_client-7.2.0/qctrlclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/password.py` & `qctrl_client-7.2.0/qctrlclient/auth/password.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/redirect_listener.py` & `qctrl_client-7.2.0/qctrlclient/auth/redirect_listener.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/auth/service_account.py` & `qctrl_client-7.2.0/qctrlclient/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/client.py` & `qctrl_client-7.2.0/qctrlclient/client.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/__init__.py` & `qctrl_client-7.2.0/qctrlclient/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/functions.py` & `qctrl_client-7.2.0/qctrlclient/core/functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/products.py` & `qctrl_client-7.2.0/qctrlclient/core/products.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/router/__init__.py` & `qctrl_client-7.2.0/qctrlclient/core/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/router/api.py` & `qctrl_client-7.2.0/qctrlclient/core/router/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 import json
 from dataclasses import dataclass
 from enum import Enum
+from functools import cached_property
 from typing import (
     Any,
     Dict,
     List,
     Optional,
 )
 from warnings import warn
@@ -70,14 +71,24 @@
         The name of the organization.
     """
 
     organization_id: str
     slug: str
     name: str
 
+    def to_dict(self) -> Dict[str, str]:
+        """
+        The dictionary representation of the organization.
+        """
+        return {
+            "id": self.organization_id,
+            "slug": self.slug,
+            "name": self.name,
+        }
+
 
 @dataclass
 class Action:
     """Simple client-side representation of the Action
     model.
 
     Parameters
@@ -155,63 +166,83 @@
 
     def _validate(self):
         """Performs validation checks on the settings."""
 
         if not self._settings.product:
             raise GraphQLClientError("`product` must be configured in settings")
 
-        organizations = self._get_organizations()
+        self._check_has_organizations()
+        self._check_must_set_organization()
+        self._check_organization_permission()
 
-        # if organization explicitly configured by user
+    def _check_must_set_organization(self):
         if self._settings.organization:
-            self._check_organization_permission(organizations)
+            return
 
-        # if no organizations found
-        elif not organizations:
-            show_error_message("No organizations found")
-
-        # if exactly one organization found
-        elif len(organizations) == 1:
-            self._settings.organization = organizations[0].slug
-
-        # if multiple organizations found
-        else:
+        if len(self._organizations) > 1:
             error_message = "You are assigned to multiple organizations. "
             error_message += "Please configure an organization:\n\n"
 
-            for organization in organizations:
+            for organization in self._organizations:
                 error_message += f"- {organization.slug}\n"
 
             show_error_message(error_message)
 
-    def _check_organization_permission(self, organizations: List[Organization]):
+    def _check_has_organizations(self):
+        # if no organizations found
+        if not self._organizations:
+            show_error_message("No organizations found")
+
+    def _check_organization_permission(self):
         """Checks that the user is assigned to the configured
         organization. Requires that the `organization` setting
         is configured.
 
         Parameters
         ----------
         organizations : List[Organization]
             List of organizations that the user is assigned to which provide
             access to the corresponding product.
         """
 
         assigned = False
 
-        for organization in organizations:
+        if not self._settings.organization:
+            return
+
+        for organization in self._organizations:
             if organization.slug == self._settings.organization:
                 assigned = True
                 break
 
         if not assigned:
             show_error_message(
                 f"Configured organization not found: `{self._settings.organization}`"
             )
 
-    def _get_organizations(self) -> List[Organization]:
+    @property
+    def _organization(self) -> Organization:
+        """Returns the organization that the user is assigned to
+        which provides access to the configured product.
+        """
+
+        if self._settings.organization:
+            for organization in self._organizations:
+                if organization.slug == self._settings.organization:
+                    return organization
+
+        if len(self._organizations) == 1:
+            return self._organizations[0]
+
+        raise GraphQLClientError(
+            f"Configured organization not found: `{self._settings.organization}`"
+        )
+
+    @cached_property
+    def _organizations(self) -> List[Organization]:
         """Returns the list of organizations that the user is
         assigned to which provide access to the configured product.
         """
 
         query = gql.gql(
             """
             query {
@@ -327,15 +358,16 @@
         package_versions = {}
 
         for package in self._TRACKED_PACKAGES:
             package_versions[package] = get_installed_version(package)
 
         return {
             "package_versions": package_versions,
-            "organization_slug": self._settings.organization,
+            "organization_slug": self._organization.slug,
+            "organization": self._organization.to_dict(),
         }
 
     @staticmethod
     def _handle_warnings(warnings_data: List[Dict[str, Any]]):
         """Handles warnings returned when starting a workflow."""
 
         for warning_data in warnings_data:
```

### Comparing `qctrl_client-7.1.0/qctrlclient/core/router/base.py` & `qctrl_client-7.2.0/qctrlclient/core/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/router/local.py` & `qctrl_client-7.2.0/qctrlclient/core/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/settings.py` & `qctrl_client-7.2.0/qctrlclient/core/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/core/utils.py` & `qctrl_client-7.2.0/qctrlclient/core/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/defaults.py` & `qctrl_client-7.2.0/qctrlclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/exceptions.py` & `qctrl_client-7.2.0/qctrlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/globals.py` & `qctrl_client-7.2.0/qctrlclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/pytest_plugin.py` & `qctrl_client-7.2.0/qctrlclient/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/transports/__init__.py` & `qctrl_client-7.2.0/qctrlclient/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/qctrlclient/transports/requests_transport.py` & `qctrl_client-7.2.0/qctrlclient/transports/requests_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.1.0/PKG-INFO` & `qctrl_client-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-client
-Version: 7.1.0
+Version: 7.2.0
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

