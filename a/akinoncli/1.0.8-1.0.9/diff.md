# Comparing `tmp/akinoncli-1.0.8.tar.gz` & `tmp/akinoncli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akinoncli-1.0.8.tar", last modified: Fri Apr  8 14:54:40 2022, max compression
+gzip compressed data, was "akinoncli-1.0.9.tar", last modified: Tue Apr 12 10:34:26 2022, max compression
```

## Comparing `akinoncli-1.0.8.tar` & `akinoncli-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-04-08 14:54:30.000000 akinoncli-1.0.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2022-04-08 14:54:30.000000 akinoncli-1.0.8/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-04-08 14:54:30.000000 akinoncli-1.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)    17094 2022-04-08 14:54:40.739349 akinoncli-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    16569 2022-04-08 14:54:30.000000 akinoncli-1.0.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/akinoncli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/akinoncli/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13513 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/client/client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/akinoncli/controllers/
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4605 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/account.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/applications.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/clusters.py
--rw-rw-rw-   0 root         (0) root         (0)    22155 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/projects.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/public_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     3667 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/controllers/users.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/akinoncli/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      451 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/core/exc.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/core/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/akinoncli/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/ext/output_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/main.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/akinoncli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-08 14:54:30.000000 akinoncli-1.0.8/akinoncli/plugins/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-08 14:54:40.739349 akinoncli-1.0.8/akinoncli.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    17094 2022-04-08 14:54:40.000000 akinoncli-1.0.8/akinoncli.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      863 2022-04-08 14:54:40.000000 akinoncli-1.0.8/akinoncli.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-04-08 14:54:40.000000 akinoncli-1.0.8/akinoncli.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       71 2022-04-08 14:54:40.000000 akinoncli-1.0.8/akinoncli.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-04-08 14:54:40.000000 akinoncli-1.0.8/akinoncli.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-04-08 14:54:40.000000 akinoncli-1.0.8/akinoncli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-04-08 14:54:30.000000 akinoncli-1.0.8/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-04-08 14:54:30.000000 akinoncli-1.0.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-04-08 14:54:40.743349 akinoncli-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1315 2022-04-08 14:54:30.000000 akinoncli-1.0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2022-04-12 10:34:19.000000 akinoncli-1.0.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2022-04-12 10:34:19.000000 akinoncli-1.0.9/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      137 2022-04-12 10:34:19.000000 akinoncli-1.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    17145 2022-04-12 10:34:26.842365 akinoncli-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16620 2022-04-12 10:34:19.000000 akinoncli-1.0.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/akinoncli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/akinoncli/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13513 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/client/client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/akinoncli/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4605 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     6435 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/applications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/clusters.py
+-rw-rw-rw-   0 root         (0) root         (0)    22155 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/public_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/controllers/users.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/akinoncli/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      451 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/core/exc.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/core/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/akinoncli/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/ext/output_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/akinoncli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-12 10:34:19.000000 akinoncli-1.0.9/akinoncli/plugins/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-12 10:34:26.842365 akinoncli-1.0.9/akinoncli.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    17145 2022-04-12 10:34:26.000000 akinoncli-1.0.9/akinoncli.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      863 2022-04-12 10:34:26.000000 akinoncli-1.0.9/akinoncli.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2022-04-12 10:34:26.000000 akinoncli-1.0.9/akinoncli.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       71 2022-04-12 10:34:26.000000 akinoncli-1.0.9/akinoncli.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       86 2022-04-12 10:34:26.000000 akinoncli-1.0.9/akinoncli.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       10 2022-04-12 10:34:26.000000 akinoncli-1.0.9/akinoncli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       94 2022-04-12 10:34:19.000000 akinoncli-1.0.9/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-04-12 10:34:19.000000 akinoncli-1.0.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-04-12 10:34:26.846365 akinoncli-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2022-04-12 10:34:19.000000 akinoncli-1.0.9/setup.py
```

### Comparing `akinoncli-1.0.8/LICENSE.md` & `akinoncli-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/PKG-INFO` & `akinoncli-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akinoncli
-Version: 1.0.8
+Version: 1.0.9
 Summary: CLI for Akinon Cloud Commerce
 Home-page: https://bitbucket.org/akinonteam/akinon-cli/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -143,27 +143,28 @@
 $ git tag 1.0
 $ git push akinon --tags
 ```
 
 The building process can be started by CLI when the tag is pushed.
 ___
 
-*  `akinoncli application build {app_id} {tag}`
+*  `akinoncli application build {app_id} {tag} {--note}`
 
 Starts the building process for the given tag.
 
-| Parameter      | Description | Required |
-| ----------- | ----------- | ----------- |
-| app_id      | Application ID | Yes |
-| tag         | Tag | Yes |
+| Parameter | Description | Required |
+|----------| ----------- | ----------- |
+| app_id   | Application ID | Yes |
+| tag      | Tag | Yes |
+| --note   | Note | No
 
 
 **Example**
 ```
-$ akinoncli application build 1 1.0
+$ akinoncli application build 1 1.0 --note="test note for the build"
 ```
 
 ___
 *  `akinoncli application versions {app_id}`
 
 Lists the built versions of the application.
```

### Comparing `akinoncli-1.0.8/README.md` & `akinoncli-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -125,27 +125,28 @@
 $ git tag 1.0
 $ git push akinon --tags
 ```
 
 The building process can be started by CLI when the tag is pushed.
 ___
 
-*  `akinoncli application build {app_id} {tag}`
+*  `akinoncli application build {app_id} {tag} {--note}`
 
 Starts the building process for the given tag.
 
-| Parameter      | Description | Required |
-| ----------- | ----------- | ----------- |
-| app_id      | Application ID | Yes |
-| tag         | Tag | Yes |
+| Parameter | Description | Required |
+|----------| ----------- | ----------- |
+| app_id   | Application ID | Yes |
+| tag      | Tag | Yes |
+| --note   | Note | No
 
 
 **Example**
 ```
-$ akinoncli application build 1 1.0
+$ akinoncli application build 1 1.0 --note="test note for the build"
 ```
 
 ___
 *  `akinoncli application versions {app_id}`
 
 Lists the built versions of the application.
```

### Comparing `akinoncli-1.0.8/akinoncli/client/client.py` & `akinoncli-1.0.9/akinoncli/client/client.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/controllers/account.py` & `akinoncli-1.0.9/akinoncli/controllers/account.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/controllers/applications.py` & `akinoncli-1.0.9/akinoncli/controllers/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,22 +106,28 @@
             (['id'], {
                 'help': 'Application ID',
                 'action': 'store',
             }),
             (['tag'], {
                 'help': 'App Version',
                 'action': 'store',
+            }),
+            (['--note'], {
+                'help': 'Version Note',
+                'action': 'store'
             })
         ]
     )
     def build(self):
         app_id = self.app.pargs.id
         data = {
             'tag': self.app.pargs.tag,
         }
+        if self.app.pargs.note is not None:
+            data['patch_notes'] = self.app.pargs.note
         response = self.app.client.build_application(app_id, data)
         if response.is_succeed:
             self.app.render({}, renderer_type='text', custom_text="Build process has been started.")
         else:
             self.app.render({}, renderer_type='text', custom_text=response.data["non_field_errors"])
 
     @ex(
```

### Comparing `akinoncli-1.0.8/akinoncli/controllers/auth.py` & `akinoncli-1.0.9/akinoncli/controllers/auth.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/controllers/base.py` & `akinoncli-1.0.9/akinoncli/controllers/base.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/controllers/clusters.py` & `akinoncli-1.0.9/akinoncli/controllers/clusters.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/controllers/projects.py` & `akinoncli-1.0.9/akinoncli/controllers/projects.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/controllers/public_keys.py` & `akinoncli-1.0.9/akinoncli/controllers/public_keys.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/controllers/users.py` & `akinoncli-1.0.9/akinoncli/controllers/users.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/ext/output_renderer.py` & `akinoncli-1.0.9/akinoncli/ext/output_renderer.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli/main.py` & `akinoncli-1.0.9/akinoncli/main.py`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/akinoncli.egg-info/PKG-INFO` & `akinoncli-1.0.9/akinoncli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akinoncli
-Version: 1.0.8
+Version: 1.0.9
 Summary: CLI for Akinon Cloud Commerce
 Home-page: https://bitbucket.org/akinonteam/akinon-cli/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -143,27 +143,28 @@
 $ git tag 1.0
 $ git push akinon --tags
 ```
 
 The building process can be started by CLI when the tag is pushed.
 ___
 
-*  `akinoncli application build {app_id} {tag}`
+*  `akinoncli application build {app_id} {tag} {--note}`
 
 Starts the building process for the given tag.
 
-| Parameter      | Description | Required |
-| ----------- | ----------- | ----------- |
-| app_id      | Application ID | Yes |
-| tag         | Tag | Yes |
+| Parameter | Description | Required |
+|----------| ----------- | ----------- |
+| app_id   | Application ID | Yes |
+| tag      | Tag | Yes |
+| --note   | Note | No
 
 
 **Example**
 ```
-$ akinoncli application build 1 1.0
+$ akinoncli application build 1 1.0 --note="test note for the build"
 ```
 
 ___
 *  `akinoncli application versions {app_id}`
 
 Lists the built versions of the application.
```

### Comparing `akinoncli-1.0.8/akinoncli.egg-info/SOURCES.txt` & `akinoncli-1.0.9/akinoncli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akinoncli-1.0.8/setup.py` & `akinoncli-1.0.9/setup.py`

 * *Files identical despite different names*

