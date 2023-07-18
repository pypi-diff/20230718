# Comparing `tmp/django-admin-commands2-1.1.1.tar.gz` & `tmp/django-admin-commands2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-commands2-1.1.1.tar", last modified: Wed Feb 15 10:45:35 2023, max compression
+gzip compressed data, was "django-admin-commands2-1.1.2.tar", last modified: Tue Jul 18 09:18:46 2023, max compression
```

## Comparing `django-admin-commands2-1.1.1.tar` & `django-admin-commands2-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-02-15 10:45:35.984554 django-admin-commands2-1.1.1/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1510 2023-02-15 10:45:20.000000 django-admin-commands2-1.1.1/LICENSE
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      193 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.1/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5254 2023-02-15 10:45:35.984554 django-admin-commands2-1.1.1/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3705 2023-02-15 06:11:17.000000 django-admin-commands2-1.1.1/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-02-15 10:45:35.984554 django-admin-commands2-1.1.1/admin_commands/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-02-15 10:43:31.000000 django-admin-commands2-1.1.1/admin_commands/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5466 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.1/admin_commands/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      464 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.1/admin_commands/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      552 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.1/admin_commands/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      313 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.1/admin_commands/forms.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-02-15 10:45:35.984554 django-admin-commands2-1.1.1/admin_commands/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2121 2023-02-10 19:33:30.000000 django-admin-commands2-1.1.1/admin_commands/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.1/admin_commands/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2538 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.1/admin_commands/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-02-15 10:45:35.980554 django-admin-commands2-1.1.1/admin_commands/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-02-15 10:45:35.984554 django-admin-commands2-1.1.1/admin_commands/templates/admin_commands/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1729 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.1/admin_commands/templates/admin_commands/execute_command.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4851 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.1/admin_commands/tests.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1276 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.1/admin_commands/utils.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       63 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.1/admin_commands/views.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-02-15 10:45:35.984554 django-admin-commands2-1.1.1/django_admin_commands2.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     5254 2023-02-15 10:45:35.000000 django-admin-commands2-1.1.1/django_admin_commands2.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      645 2023-02-15 10:45:35.000000 django-admin-commands2-1.1.1/django_admin_commands2.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-02-15 10:45:35.000000 django-admin-commands2-1.1.1/django_admin_commands2.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       12 2023-02-15 10:45:35.000000 django-admin-commands2-1.1.1/django_admin_commands2.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       21 2023-02-15 10:45:35.000000 django-admin-commands2-1.1.1/django_admin_commands2.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1458 2023-02-15 10:45:35.984554 django-admin-commands2-1.1.1/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-admin-commands2-1.1.1/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1510 2023-02-15 10:45:20.000000 django-admin-commands2-1.1.2/LICENSE
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      193 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.2/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5217 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3705 2023-02-15 06:11:17.000000 django-admin-commands2-1.1.2/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/admin_commands/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-07-18 09:18:43.000000 django-admin-commands2-1.1.2/admin_commands/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5414 2023-07-18 09:17:59.000000 django-admin-commands2-1.1.2/admin_commands/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      464 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      552 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      313 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/forms.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/admin_commands/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2121 2023-02-10 19:33:30.000000 django-admin-commands2-1.1.2/admin_commands/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.2/admin_commands/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2538 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/models.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.253682 django-admin-commands2-1.1.2/admin_commands/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/admin_commands/templates/admin_commands/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1729 2023-02-15 05:55:10.000000 django-admin-commands2-1.1.2/admin_commands/templates/admin_commands/execute_command.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4851 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/tests.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1276 2023-02-15 05:54:25.000000 django-admin-commands2-1.1.2/admin_commands/utils.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       63 2023-02-09 09:31:02.000000 django-admin-commands2-1.1.2/admin_commands/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5217 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      645 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       12 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       21 2023-07-18 09:18:46.000000 django-admin-commands2-1.1.2/django_admin_commands2.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1458 2023-07-18 09:18:46.257682 django-admin-commands2-1.1.2/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-admin-commands2-1.1.2/setup.py
```

### Comparing `django-admin-commands2-1.1.1/LICENSE` & `django-admin-commands2-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/PKG-INFO` & `django-admin-commands2-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: django-admin-commands2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Execute management commands via admin with ease and control.
 Home-page: https://github.com/KUWAITNET/django-admin-commands
 Author: Ramez Ashraf
 Author-email: ramez@kuwaitnet.com
-License: UNKNOWN
 Project-URL: Source, https://github.com/KUWAITNET/django-admin-commands
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -135,9 +133,7 @@
                 # This is the queryset that is used to filter the commands that are shown in the admin.
                 # You can override this to customize the queryset for the user
                 return super().get_queryset(request)
 
         admin.site.unregister(ManagementCommands)
         admin.site.register(ManagementCommands, CustomManagementCommandsAdmin)
 
-
-
```

### Comparing `django-admin-commands2-1.1.1/README.rst` & `django-admin-commands2-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/admin_commands/admin.py` & `django-admin-commands2-1.1.2/admin_commands/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.contrib import admin
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponseNotFound
 from django.shortcuts import render
 from django.template.defaultfilters import linebreaksbr
 from django.urls import reverse
-from django.utils.encoding import force_text
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 
 from .app_settings import ADMIN_COMMANDS_CONFIG
 from .forms import ExecuteCommandForm
 from .models import ManagementCommand, CallCommandLog
@@ -85,15 +84,15 @@
 
         else:
             form = ExecuteCommandForm(initial={'command': command.pk})
 
         opts = self.model._meta
         context = dict(
             self.admin_site.each_context(request),
-            module_name=force_text(opts.verbose_name_plural),
+            module_name=str(opts.verbose_name_plural),
             has_add_permission=self.has_add_permission(request),
             opts=opts,
             command=command,
             actions_on_top=self.actions_on_top,
             actions_on_bottom=self.actions_on_bottom,
             actions_selection_counter=self.actions_selection_counter,
             preserved_filters=self.get_preserved_filters(request),
```

### Comparing `django-admin-commands2-1.1.1/admin_commands/apps.py` & `django-admin-commands2-1.1.2/admin_commands/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/admin_commands/migrations/0001_initial.py` & `django-admin-commands2-1.1.2/admin_commands/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/admin_commands/models.py` & `django-admin-commands2-1.1.2/admin_commands/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/admin_commands/templates/admin_commands/execute_command.html` & `django-admin-commands2-1.1.2/admin_commands/templates/admin_commands/execute_command.html`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/admin_commands/tests.py` & `django-admin-commands2-1.1.2/admin_commands/tests.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/admin_commands/utils.py` & `django-admin-commands2-1.1.2/admin_commands/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/django_admin_commands2.egg-info/PKG-INFO` & `django-admin-commands2-1.1.2/django_admin_commands2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: django-admin-commands2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Execute management commands via admin with ease and control.
 Home-page: https://github.com/KUWAITNET/django-admin-commands
 Author: Ramez Ashraf
 Author-email: ramez@kuwaitnet.com
-License: UNKNOWN
 Project-URL: Source, https://github.com/KUWAITNET/django-admin-commands
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -135,9 +133,7 @@
                 # This is the queryset that is used to filter the commands that are shown in the admin.
                 # You can override this to customize the queryset for the user
                 return super().get_queryset(request)
 
         admin.site.unregister(ManagementCommands)
         admin.site.register(ManagementCommands, CustomManagementCommandsAdmin)
 
-
-
```

### Comparing `django-admin-commands2-1.1.1/django_admin_commands2.egg-info/SOURCES.txt` & `django-admin-commands2-1.1.2/django_admin_commands2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-commands2-1.1.1/setup.cfg` & `django-admin-commands2-1.1.2/setup.cfg`

 * *Files identical despite different names*

