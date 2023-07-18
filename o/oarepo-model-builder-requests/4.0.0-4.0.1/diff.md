# Comparing `tmp/oarepo-model-builder-requests-4.0.0.tar.gz` & `tmp/oarepo-model-builder-requests-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-requests-4.0.0.tar", last modified: Mon Jul  3 15:19:33 2023, max compression
+gzip compressed data, was "oarepo-model-builder-requests-4.0.1.tar", last modified: Tue Jul 18 10:10:21 2023, max compression
```

## Comparing `oarepo-model-builder-requests-4.0.0.tar` & `oarepo-model-builder-requests-4.0.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/requests_model/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/requests_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/requests_model/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/tests/test_custom_action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.378476 oarepo-model-builder-requests-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-18 10:10:21.378476 oarepo-model-builder-requests-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/components/requests_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/components/requests_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/components/requests_model/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/datatypes/components/requests_model/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/invenio_requests_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/invenio_requests_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/invenio_requests_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.378476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:10:21.374476 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-18 10:10:21.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-18 10:10:21.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:10:21.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-18 10:10:21.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 10:10:21.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 10:10:21.000000 oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 10:10:21.378476 oarepo-model-builder-requests-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:07:03.000000 oarepo-model-builder-requests-4.0.1/setup.py
```

### Comparing `oarepo-model-builder-requests-4.0.0/LICENSE` & `oarepo-model-builder-requests-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.0/PKG-INFO` & `oarepo-model-builder-requests-4.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: oarepo-model-builder-requests
-Version: 4.0.0
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
 # OARepo model builder requests
 Plugin for oarepo-model-builder to allow specifying requests 
 tied to the base model, based on invenio requests. <br>
 
 Requests are requests for an action concerning an instance of the model (called 
 topic in this context), 
 for example to publish the topic. 
@@ -19,36 +12,48 @@
 
 
 By default, along with changing the request status,
 the generated accept action fetches the associated record. It's up to the 
 developer to decide what to do with it further.
 
 
-Types of requests can be added to the model through "requests" section 
+Requests can be added to the model through "requests" section 
 in the yaml file of the model. There can be any number of them.
 Options in the yaml:
-
-* `class` Class for the Type of the request. 
+* `module` Module in which the request is stored. The type and action modules are derived from it but can override the default.
+* `type` Settings for the type class of the request. 
 Used if the user wants to use a custom request type class.
+  * `module`
+  * `class`
+  * `bases`
+  * `imports`
+  * `generate` True by defualt, False is 
+  typically used when user provides custom Type class.
+  * `parent-actions` Request type class specifies actions that can be performed by the request. By default the class imports its parent's possible actions, but this behavior can be customized if the parent class has different structure for some reason.
 
-* `generate` True by defualt, False is 
-typically used when user provides custom Type class.
-
-* `bases`
-Base classes for the Type class.
 * `actions`
 A list of customized actions by this type of request. Only the accept action is supported for now.
-
+  * `module` 
   * `class` Analogous to type class for the action. By default 
 it's [invenio_requests.customizations.AcceptAction](https://github.com/inveniosoftware/invenio-requests/blob/master/invenio_requests/customizations/actions.py).
-
+  * `bases`
+  * `imports`
   * `generate` Analogous to type class for the action.
 
   * `bases` Analogous to type class bases for the action.
 
+It also allows specifying the topic record resolver used. The resolver is tied to the topic class therefore it's generated on record level instead of the request.
+Configurable options:
+  * `module`
+  * `class`
+  * `bases`
+  * `imports`
+  * `generate`
+  * `custom-proxy-class` The resolver can use different proxy record resolution class. This is needed for resolving drafts because they don't have registered PIDs.
+
 ## Examples
 
 For example, the requests plugin can be used for approving
 a thesis. The accept action can be used for approval.
 A simple yaml entry at the root level can be used:
 ```yaml
 requests:
```

### Comparing `oarepo-model-builder-requests-4.0.0/README.md` & `oarepo-model-builder-requests-4.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: oarepo-model-builder-requests
+Version: 4.0.1
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE
+
 # OARepo model builder requests
 Plugin for oarepo-model-builder to allow specifying requests 
 tied to the base model, based on invenio requests. <br>
 
 Requests are requests for an action concerning an instance of the model (called 
 topic in this context), 
 for example to publish the topic. 
@@ -12,36 +19,48 @@
 
 
 By default, along with changing the request status,
 the generated accept action fetches the associated record. It's up to the 
 developer to decide what to do with it further.
 
 
-Types of requests can be added to the model through "requests" section 
+Requests can be added to the model through "requests" section 
 in the yaml file of the model. There can be any number of them.
 Options in the yaml:
-
-* `class` Class for the Type of the request. 
+* `module` Module in which the request is stored. The type and action modules are derived from it but can override the default.
+* `type` Settings for the type class of the request. 
 Used if the user wants to use a custom request type class.
+  * `module`
+  * `class`
+  * `bases`
+  * `imports`
+  * `generate` True by defualt, False is 
+  typically used when user provides custom Type class.
+  * `parent-actions` Request type class specifies actions that can be performed by the request. By default the class imports its parent's possible actions, but this behavior can be customized if the parent class has different structure for some reason.
 
-* `generate` True by defualt, False is 
-typically used when user provides custom Type class.
-
-* `bases`
-Base classes for the Type class.
 * `actions`
 A list of customized actions by this type of request. Only the accept action is supported for now.
-
+  * `module` 
   * `class` Analogous to type class for the action. By default 
 it's [invenio_requests.customizations.AcceptAction](https://github.com/inveniosoftware/invenio-requests/blob/master/invenio_requests/customizations/actions.py).
-
+  * `bases`
+  * `imports`
   * `generate` Analogous to type class for the action.
 
   * `bases` Analogous to type class bases for the action.
 
+It also allows specifying the topic record resolver used. The resolver is tied to the topic class therefore it's generated on record level instead of the request.
+Configurable options:
+  * `module`
+  * `class`
+  * `bases`
+  * `imports`
+  * `generate`
+  * `custom-proxy-class` The resolver can use different proxy record resolution class. This is needed for resolving drafts because they don't have registered PIDs.
+
 ## Examples
 
 For example, the requests plugin can be used for approving
 a thesis. The accept action can be used for approval.
 A simple yaml entry at the root level can be used:
 ```yaml
 requests:
```

### Comparing `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2` & `oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2`

 * *Files 24% similar despite different names*

```diff
@@ -4,11 +4,13 @@
 {% for request_data in vars.requests.values() %}
 {{ request_data.type.class|generate_import }}
 {% endfor %}
 
 
 
 REQUESTS_REGISTERED_TYPES = [{% for request_data in vars.requests.values() %}{{ request_data.type.class|base_name }}, {% endfor %}]
+{% if not vars.record_resolver.skip %}
 REQUESTS_ENTITY_RESOLVERS = [
         UserResolver(),
         {{ vars.record_resolver.class|base_name }}(record_cls={{ vars.record.class|base_name }}, service_id="{{ vars.service_config.service_id }}", type_key="{{ vars.module.prefix_snake }}")
-    ]
+    ]
+{% endif %}
```

### Comparing `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2` & `oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,19 @@
-{% for request_data in vars.requests.values() %}
-    {% if request_data.type.generate %}
-{{ request_data.actions['approve'].class|generate_import }}
-{{ request_data.type.imports|generate_import }}
-{% endif %}
-{% endfor %}
+{{ request.actions['approve'].class|generate_import }}
+{{ request.type.imports|generate_import }}
 
-{% for request_name, request_data in vars.requests.items() %}
-{% if request_data.type.generate %}
-class {{ request_data.type|class_header }}:
+class {{ request.type|class_header }}:
 
     type_id = "{{ request_name }}"
     name = "{{ request_name.capitalize() }}"
 
     available_actions = {
-        **RequestType.available_actions,
-        "accept": {{ request_data.actions['approve'].class|base_name }}
+        {{ request.type.parent_actions }},
+        "accept": {{ request.actions['approve'].class|base_name }}
     }
 
     allowed_topic_ref_types = ["{{ vars.module.prefix_snake }}"] # On the Request record object, the topic is referenced by pid. This pid is
                                          # extracted by Resolver subclassed from RecordResolver, which has hardcoded
                                          # {"record": {pid}} as reference value. This reference is then by
                                          # setattr set on the Request record topic ReferencedEntityField, and the set
                                          # operation checks, whether this key is in allowed_topic_ref_types
     #TODO would it make sense to customize the topic ref types?
-{% endif %}
-{% endfor %}
```

### Comparing `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2` & `oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2` & `oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     request_record_input_data,
 ):
     receiver_user = users[1]
     sender_identity = identity_simple
     receiver_identity = identity_simple_2
     request_types = app.extensions["invenio-requests"].request_type_registry
     for request_type in request_types:
-        if request_type.__module__ != "{{ vars.requests_modules.types_module }}": #not a generated request
+        if request_type.__module__ != "thesis.records.requests.assign_doi.types": #not a generated request
             continue
         request = submit_request(
             sender_identity,
             data=request_record_input_data,
             topic=example_topic,
             request_type=request_type,
             receiver=receiver_user,
```

### Comparing `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/PKG-INFO` & `oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-requests
-Version: 4.0.0
+Version: 4.0.1
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder requests
 Plugin for oarepo-model-builder to allow specifying requests 
 tied to the base model, based on invenio requests. <br>
@@ -19,36 +19,48 @@
 
 
 By default, along with changing the request status,
 the generated accept action fetches the associated record. It's up to the 
 developer to decide what to do with it further.
 
 
-Types of requests can be added to the model through "requests" section 
+Requests can be added to the model through "requests" section 
 in the yaml file of the model. There can be any number of them.
 Options in the yaml:
-
-* `class` Class for the Type of the request. 
+* `module` Module in which the request is stored. The type and action modules are derived from it but can override the default.
+* `type` Settings for the type class of the request. 
 Used if the user wants to use a custom request type class.
+  * `module`
+  * `class`
+  * `bases`
+  * `imports`
+  * `generate` True by defualt, False is 
+  typically used when user provides custom Type class.
+  * `parent-actions` Request type class specifies actions that can be performed by the request. By default the class imports its parent's possible actions, but this behavior can be customized if the parent class has different structure for some reason.
 
-* `generate` True by defualt, False is 
-typically used when user provides custom Type class.
-
-* `bases`
-Base classes for the Type class.
 * `actions`
 A list of customized actions by this type of request. Only the accept action is supported for now.
-
+  * `module` 
   * `class` Analogous to type class for the action. By default 
 it's [invenio_requests.customizations.AcceptAction](https://github.com/inveniosoftware/invenio-requests/blob/master/invenio_requests/customizations/actions.py).
-
+  * `bases`
+  * `imports`
   * `generate` Analogous to type class for the action.
 
   * `bases` Analogous to type class bases for the action.
 
+It also allows specifying the topic record resolver used. The resolver is tied to the topic class therefore it's generated on record level instead of the request.
+Configurable options:
+  * `module`
+  * `class`
+  * `bases`
+  * `imports`
+  * `generate`
+  * `custom-proxy-class` The resolver can use different proxy record resolution class. This is needed for resolving drafts because they don't have registered PIDs.
+
 ## Examples
 
 For example, the requests plugin can be used for approving
 a thesis. The accept action can be used for approval.
 A simple yaml entry at the root level can be used:
 ```yaml
 requests:
```

### Comparing `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/SOURCES.txt` & `oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 oarepo_model_builder_requests.egg-info/entry_points.txt
 oarepo_model_builder_requests.egg-info/requires.txt
 oarepo_model_builder_requests.egg-info/top_level.txt
 oarepo_model_builder_requests/datatypes/__init__.py
 oarepo_model_builder_requests/datatypes/components/__init__.py
 oarepo_model_builder_requests/datatypes/components/requests_model/__init__.py
 oarepo_model_builder_requests/datatypes/components/requests_model/requests.py
+oarepo_model_builder_requests/datatypes/components/requests_model/resolver.py
 oarepo_model_builder_requests/invenio/__init__.py
 oarepo_model_builder_requests/invenio/invenio_requests_actions.py
 oarepo_model_builder_requests/invenio/invenio_requests_config.py
 oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
 oarepo_model_builder_requests/invenio/invenio_requests_types.py
 oarepo_model_builder_requests/invenio/invenio_requests_views.py
 oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
@@ -26,9 +27,8 @@
 oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
 oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
 oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
 oarepo_model_builder_requests/tests/__init__.py
 oarepo_model_builder_requests/tests/invenio_requests_conftest.py
 oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
 oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
-oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
-tests/test_custom_action.py
+oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
```

### Comparing `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/entry_points.txt` & `oarepo-model-builder-requests-4.0.1/oarepo_model_builder_requests.egg-info/entry_points.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+[oarepo_model_builder.builders.draft]
+2210-invenio_requests_actions = oarepo_model_builder_requests.invenio.invenio_requests_actions:InvenioRequestsActionsBuilder
+2211-invenio_requests_resolvers = oarepo_model_builder_requests.invenio.invenio_requests_resolvers:InvenioRequestsResolversBuilder
+2212-invenio_requests_types = oarepo_model_builder_requests.invenio.invenio_requests_types:InvenioRequestsTypesBuilder
+2215-invenio_requests_config = oarepo_model_builder_requests.invenio.invenio_requests_config:InvenioRequestsConfigBuilder
+
+[oarepo_model_builder.builders.draft_files]
+2210-invenio_requests_actions = oarepo_model_builder_requests.invenio.invenio_requests_actions:InvenioRequestsActionsBuilder
+2211-invenio_requests_resolvers = oarepo_model_builder_requests.invenio.invenio_requests_resolvers:InvenioRequestsResolversBuilder
+2212-invenio_requests_types = oarepo_model_builder_requests.invenio.invenio_requests_types:InvenioRequestsTypesBuilder
+2215-invenio_requests_config = oarepo_model_builder_requests.invenio.invenio_requests_config:InvenioRequestsConfigBuilder
+
 [oarepo_model_builder.builders.record]
 2210-invenio_requests_actions = oarepo_model_builder_requests.invenio.invenio_requests_actions:InvenioRequestsActionsBuilder
 2211-invenio_requests_resolvers = oarepo_model_builder_requests.invenio.invenio_requests_resolvers:InvenioRequestsResolversBuilder
 2212-invenio_requests_types = oarepo_model_builder_requests.invenio.invenio_requests_types:InvenioRequestsTypesBuilder
 2214-invenio_requests_views = oarepo_model_builder_requests.invenio.invenio_requests_views:InvenioRequestsViewsBuilder
 2215-invenio_requests_config = oarepo_model_builder_requests.invenio.invenio_requests_config:InvenioRequestsConfigBuilder
-2216-invenio_requests_conftest = oarepo_model_builder_requests.tests.invenio_requests_conftest:InvenioRequestsConftestBuilder
-2219-invenio_requests_test_requests = oarepo_model_builder_requests.tests.invenio_requests_test_requests:InvenioRequestsTestRequestsBuilder
 
 [oarepo_model_builder.datatypes.components]
 invenio_requests = oarepo_model_builder_requests.datatypes.components:requests_components
 
 [oarepo_model_builder.templates]
 98-requests_templates = oarepo_model_builder_requests.invenio
 99-requests_tests_templates = oarepo_model_builder_requests.tests
```

