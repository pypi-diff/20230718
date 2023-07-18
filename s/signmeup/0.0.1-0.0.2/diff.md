# Comparing `tmp/signmeup-0.0.1.tar.gz` & `tmp/signmeup-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\signmeup-0.0.1.tar", last modified: Mon Jul 17 12:29:51 2023, max compression
+gzip compressed data, was "dist\signmeup-0.0.2.tar", last modified: Tue Jul 18 13:00:08 2023, max compression
```

## Comparing `signmeup-0.0.1.tar` & `signmeup-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:51.011960 signmeup-0.0.1/
--rw-rw-rw-   0        0        0       41 2023-07-17 11:11:18.000000 signmeup-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4789 2023-07-17 12:29:51.010961 signmeup-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4248 2023-06-27 18:55:07.000000 signmeup-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:50.971068 signmeup-0.0.1/accounts/
--rw-rw-rw-   0        0        0        0 2023-06-22 09:09:29.000000 signmeup-0.0.1/accounts/__init__.py
--rw-rw-rw-   0        0        0      167 2023-07-05 18:55:29.000000 signmeup-0.0.1/accounts/admin.py
--rw-rw-rw-   0        0        0      154 2023-06-22 09:09:29.000000 signmeup-0.0.1/accounts/apps.py
--rw-rw-rw-   0        0        0     2213 2023-07-16 18:29:42.000000 signmeup-0.0.1/accounts/middleware.py
--rw-rw-rw-   0        0        0     4681 2023-07-12 13:39:25.000000 signmeup-0.0.1/accounts/models.py
--rw-rw-rw-   0        0        0     2622 2023-07-12 13:43:59.000000 signmeup-0.0.1/accounts/serializers.py
--rw-rw-rw-   0        0        0    10580 2023-07-16 19:09:18.000000 signmeup-0.0.1/accounts/tests.py
--rw-rw-rw-   0        0        0      634 2023-07-16 18:26:16.000000 signmeup-0.0.1/accounts/urls.py
--rw-rw-rw-   0        0        0     9366 2023-07-16 18:43:40.000000 signmeup-0.0.1/accounts/views.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:50.982040 signmeup-0.0.1/core/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:06:04.000000 signmeup-0.0.1/core/__init__.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:11.000000 signmeup-0.0.1/core/asgi.py
--rw-rw-rw-   0        0        0     4223 2023-07-12 13:53:36.000000 signmeup-0.0.1/core/settings.py
--rw-rw-rw-   0        0        0      852 2023-07-16 17:48:44.000000 signmeup-0.0.1/core/urls.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:01.000000 signmeup-0.0.1/core/wsgi.py
--rw-rw-rw-   0        0        0       42 2023-07-17 12:29:51.011960 signmeup-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1364 2023-07-17 12:29:36.000000 signmeup-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:50.993010 signmeup-0.0.1/signmeup/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:06:04.000000 signmeup-0.0.1/signmeup/__init__.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:11.000000 signmeup-0.0.1/signmeup/asgi.py
--rw-rw-rw-   0        0        0     4223 2023-07-12 13:53:36.000000 signmeup-0.0.1/signmeup/settings.py
--rw-rw-rw-   0        0        0      852 2023-07-16 17:48:44.000000 signmeup-0.0.1/signmeup/urls.py
--rw-rw-rw-   0        0        0      407 2023-07-12 13:52:01.000000 signmeup-0.0.1/signmeup/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:29:51.007971 signmeup-0.0.1/signmeup.egg-info/
--rw-rw-rw-   0        0        0     4789 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      205 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-17 12:29:50.000000 signmeup-0.0.1/signmeup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:08.037393 signmeup-0.0.2/
+-rw-rw-rw-   0        0        0       41 2023-07-17 11:11:18.000000 signmeup-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      135 2023-07-18 13:00:08.036396 signmeup-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4248 2023-06-27 18:55:07.000000 signmeup-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:07.971046 signmeup-0.0.2/accounts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 09:09:29.000000 signmeup-0.0.2/accounts/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-07-05 18:55:29.000000 signmeup-0.0.2/accounts/admin.py
+-rw-rw-rw-   0        0        0      154 2023-06-22 09:09:29.000000 signmeup-0.0.2/accounts/apps.py
+-rw-rw-rw-   0        0        0     2213 2023-07-16 18:29:42.000000 signmeup-0.0.2/accounts/middleware.py
+-rw-rw-rw-   0        0        0     4681 2023-07-12 13:39:25.000000 signmeup-0.0.2/accounts/models.py
+-rw-rw-rw-   0        0        0     2622 2023-07-12 13:43:59.000000 signmeup-0.0.2/accounts/serializers.py
+-rw-rw-rw-   0        0        0    10580 2023-07-16 19:09:18.000000 signmeup-0.0.2/accounts/tests.py
+-rw-rw-rw-   0        0        0      634 2023-07-16 18:26:16.000000 signmeup-0.0.2/accounts/urls.py
+-rw-rw-rw-   0        0        0     9366 2023-07-16 18:43:40.000000 signmeup-0.0.2/accounts/views.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:08.008946 signmeup-0.0.2/core/
+-rw-rw-rw-   0        0        0        0 2023-06-22 08:06:04.000000 signmeup-0.0.2/core/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-07-12 13:52:11.000000 signmeup-0.0.2/core/asgi.py
+-rw-rw-rw-   0        0        0     4223 2023-07-12 13:53:36.000000 signmeup-0.0.2/core/settings.py
+-rw-rw-rw-   0        0        0      852 2023-07-16 17:48:44.000000 signmeup-0.0.2/core/urls.py
+-rw-rw-rw-   0        0        0      407 2023-07-12 13:52:01.000000 signmeup-0.0.2/core/wsgi.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:00:08.037393 signmeup-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2023-07-18 12:59:10.000000 signmeup-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:08.032406 signmeup-0.0.2/signmeup.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-18 13:00:07.000000 signmeup-0.0.2/signmeup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-07-18 13:00:07.000000 signmeup-0.0.2/signmeup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:00:07.000000 signmeup-0.0.2/signmeup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 13:00:07.000000 signmeup-0.0.2/signmeup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      205 2023-07-18 13:00:07.000000 signmeup-0.0.2/signmeup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 13:00:07.000000 signmeup-0.0.2/signmeup.egg-info/top_level.txt
```

### Comparing `signmeup-0.0.1/PKG-INFO` & `signmeup-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: signmeup
-Version: 0.0.1
-Summary: Sign Me Up API Package
-Home-page: https://github.com/yourusername/signmeup
-Author: Your Name
-Author-email: yourname@example.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-
 # Sign-Me-Up
 
 Sign-Me-Up is a Django REST framework -based user registration API that allows users to sign up, verify their email addresses, and create user accounts. It provides a secure and scalable solution for managing user registration in your web application.
 
 ## Features
 
 - User registration with email verification
```

### Comparing `signmeup-0.0.1/accounts/middleware.py` & `signmeup-0.0.2/accounts/middleware.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/models.py` & `signmeup-0.0.2/accounts/models.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/serializers.py` & `signmeup-0.0.2/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/tests.py` & `signmeup-0.0.2/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/urls.py` & `signmeup-0.0.2/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/accounts/views.py` & `signmeup-0.0.2/accounts/views.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/core/settings.py` & `signmeup-0.0.2/core/settings.py`

 * *Files identical despite different names*

### Comparing `signmeup-0.0.1/core/urls.py` & `signmeup-0.0.2/core/urls.py`

 * *Files identical despite different names*

