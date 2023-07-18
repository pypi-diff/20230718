# Comparing `tmp/django_azure_communication_email-1.0.0.tar.gz` & `tmp/django_azure_communication_email-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_communication_email-1.0.0.tar", max compression
+gzip compressed data, was "django_azure_communication_email-1.0.1.tar", max compression
```

## Comparing `django_azure_communication_email-1.0.0.tar` & `django_azure_communication_email-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/LICENSE
--rw-r--r--   0        0        0     2060 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/README.md
--rw-r--r--   0        0        0      238 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/django_azure_communication_email/__init__.py
--rw-r--r--   0        0        0     2342 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/django_azure_communication_email/attachment.py
--rw-r--r--   0        0        0     5445 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/django_azure_communication_email/backend.py
--rw-r--r--   0        0        0      526 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/django_azure_communication_email/settings.py
--rw-r--r--   0        0        0      818 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/django_azure_communication_email/utils.py
--rw-r--r--   0        0        0     1852 2023-07-18 08:45:19.335394 django_azure_communication_email-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 django_azure_communication_email-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2060 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/README.md
+-rw-r--r--   0        0        0      238 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/django_azure_communication_email/__init__.py
+-rw-r--r--   0        0        0     2342 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/django_azure_communication_email/attachment.py
+-rw-r--r--   0        0        0     5445 2023-07-18 15:53:00.227124 django_azure_communication_email-1.0.1/django_azure_communication_email/backend.py
+-rw-r--r--   0        0        0      526 2023-07-18 15:53:00.231124 django_azure_communication_email-1.0.1/django_azure_communication_email/settings.py
+-rw-r--r--   0        0        0      818 2023-07-18 15:53:00.231124 django_azure_communication_email-1.0.1/django_azure_communication_email/utils.py
+-rw-r--r--   0        0        0     2003 2023-07-18 15:53:00.231124 django_azure_communication_email-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 django_azure_communication_email-1.0.1/PKG-INFO
```

### Comparing `django_azure_communication_email-1.0.0/LICENSE` & `django_azure_communication_email-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.0/README.md` & `django_azure_communication_email-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.0/django_azure_communication_email/attachment.py` & `django_azure_communication_email-1.0.1/django_azure_communication_email/attachment.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.0/django_azure_communication_email/backend.py` & `django_azure_communication_email-1.0.1/django_azure_communication_email/backend.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.0/django_azure_communication_email/settings.py` & `django_azure_communication_email-1.0.1/django_azure_communication_email/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.0/django_azure_communication_email/utils.py` & `django_azure_communication_email-1.0.1/django_azure_communication_email/utils.py`

 * *Files identical despite different names*

### Comparing `django_azure_communication_email-1.0.0/pyproject.toml` & `django_azure_communication_email-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-communication-email"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Django email backend for Azure Communication Email service."
 authors = ["Dmitrii Azarenko <dmitrii@retechlabs.com>"]
 maintainers = []
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/rebotics/django-azure-communication-email"
 packages = [{include = "django_azure_communication_email"}]
@@ -23,14 +23,18 @@
     'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/rebotics/django-azure-communication-email/issues"
+"Company Website" = "https://retechlabs.com"
+
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 Django = ">=2.2,<4.3"
 azure-identity = "~1.13"
 azure-communication-email = "~1.0"
```

### Comparing `django_azure_communication_email-1.0.0/PKG-INFO` & `django_azure_communication_email-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-communication-email
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django email backend for Azure Communication Email service.
 Home-page: https://github.com/rebotics/django-azure-communication-email
 License: Apache-2.0
 Keywords: django,email,azure
 Author: Dmitrii Azarenko
 Author-email: dmitrii@retechlabs.com
 Requires-Python: >=3.8,<3.12
@@ -24,14 +24,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (>=2.2,<4.3)
 Requires-Dist: azure-communication-email (>=1.0,<1.1)
 Requires-Dist: azure-identity (>=1.13,<1.14)
+Project-URL: Bug Tracker, https://github.com/rebotics/django-azure-communication-email/issues
+Project-URL: Company Website, https://retechlabs.com
 Project-URL: Repository, https://github.com/rebotics/django-azure-communication-email
 Description-Content-Type: text/markdown
 
 # Django Azure Communication Email
 
 [![Unit tests](https://github.com/rebotics/django-azure-communication-email/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/rebotics/django-azure-communication-email/actions/workflows/ci.yml)
 [![PyPI version](https://badge.fury.io/py/django-azure-communication-email.svg)](https://badge.fury.io/py/django-azure-communication-email)
```

