# Comparing `tmp/xnbtd-0.0.5.tar.gz` & `tmp/xnbtd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnbtd-0.0.5.tar", max compression
+gzip compressed data, was "xnbtd-0.0.6.tar", max compression
```

## Comparing `xnbtd-0.0.5.tar` & `xnbtd-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.5/LICENSE
--rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.5/README.md
--rwxr-xr-x   0        0        0     3622 2023-07-18 15:19:52.480760 xnbtd-0.0.5/pyproject.toml
--rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.5/xnbtd/__init__.py
--rwxr-xr-x   0        0        0      273 2023-07-18 13:35:27.207150 xnbtd-0.0.5/xnbtd/admin.py
--rwxr-xr-x   0        0        0      133 2023-07-18 13:03:47.393025 xnbtd-0.0.5/xnbtd/apps.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.5/xnbtd/asgi.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.5/xnbtd/plannings/__init__.py
--rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.5/xnbtd/plannings/admin.py
--rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.5/xnbtd/plannings/apps.py
--rwxr-xr-x   0        0        0      581 2023-07-18 14:53:44.000000 xnbtd-0.0.5/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0      953 2023-07-18 14:52:57.562365 xnbtd-0.0.5/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0      829 2023-07-17 14:22:40.773228 xnbtd-0.0.5/xnbtd/plannings/migrations/0001_initial.py
--rwxr-xr-x   0        0        0      575 2023-07-17 14:22:40.771240 xnbtd-0.0.5/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py
--rwxr-xr-x   0        0        0        0 2023-07-17 11:22:12.330780 xnbtd-0.0.5/xnbtd/plannings/migrations/__init__.py
--rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.5/xnbtd/plannings/models.py
--rwxr-xr-x   0        0        0      324 2023-07-18 15:17:40.412906 xnbtd-0.0.5/xnbtd/plannings/templatetags/events.py
--rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.5/xnbtd/publish.py
--rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.5/xnbtd/settings/__init__.py
--rwxr-xr-x   0        0        0     5609 2023-07-18 13:27:11.137051 xnbtd-0.0.5/xnbtd/settings/base.py
--rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.5/xnbtd/settings/local.py
--rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.5/xnbtd/settings/prod.py
--rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.5/xnbtd/settings/test.py
--rwxr-xr-x   0        0        0     1421 2023-07-18 14:49:38.558100 xnbtd-0.0.5/xnbtd/templates/admin/index.html
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-0.0.5/xnbtd/tours/__init__.py
--rwxr-xr-x   0        0        0     6654 2023-07-18 15:17:40.498280 xnbtd-0.0.5/xnbtd/tours/admin.py
--rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.5/xnbtd/tours/apps.py
--rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.5/xnbtd/tours/forms.py
--rwxr-xr-x   0        0        0     3622 2023-07-18 14:53:44.000000 xnbtd-0.0.5/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     6757 2023-07-18 14:52:57.461646 xnbtd-0.0.5/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0     6465 2023-07-17 14:22:40.889949 xnbtd-0.0.5/xnbtd/tours/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-07-12 14:57:11.196824 xnbtd-0.0.5/xnbtd/tours/migrations/__init__.py
--rwxr-xr-x   0        0        0     4249 2023-07-17 14:22:40.864888 xnbtd-0.0.5/xnbtd/tours/models.py
--rwxr-xr-x   0        0        0      113 2023-07-18 13:08:06.430521 xnbtd-0.0.5/xnbtd/urls.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.5/xnbtd/wsgi.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.6/LICENSE
+-rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.6/README.md
+-rwxr-xr-x   0        0        0     3622 2023-07-18 16:05:17.721174 xnbtd-0.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0      162 2023-07-17 13:09:46.529352 xnbtd-0.0.6/xnbtd/__init__.py
+-rwxr-xr-x   0        0        0      279 2023-07-18 15:51:08.615278 xnbtd-0.0.6/xnbtd/admin.py
+-rwxr-xr-x   0        0        0      133 2023-07-18 13:03:47.393025 xnbtd-0.0.6/xnbtd/apps.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.6/xnbtd/asgi.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.6/xnbtd/plannings/__init__.py
+-rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.6/xnbtd/plannings/admin.py
+-rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.6/xnbtd/plannings/apps.py
+-rwxr-xr-x   0        0        0      581 2023-07-18 14:53:44.000000 xnbtd-0.0.6/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0      953 2023-07-18 14:52:57.562365 xnbtd-0.0.6/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0      829 2023-07-17 14:22:40.773228 xnbtd-0.0.6/xnbtd/plannings/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0      575 2023-07-17 14:22:40.771240 xnbtd-0.0.6/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 11:22:12.330780 xnbtd-0.0.6/xnbtd/plannings/migrations/__init__.py
+-rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.6/xnbtd/plannings/models.py
+-rwxr-xr-x   0        0        0      324 2023-07-18 15:17:40.412906 xnbtd-0.0.6/xnbtd/plannings/templatetags/events.py
+-rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.6/xnbtd/publish.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.6/xnbtd/settings/__init__.py
+-rwxr-xr-x   0        0        0     5600 2023-07-18 15:56:50.287511 xnbtd-0.0.6/xnbtd/settings/base.py
+-rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.6/xnbtd/settings/local.py
+-rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.6/xnbtd/settings/prod.py
+-rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.6/xnbtd/settings/test.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-0.0.6/xnbtd/tours/__init__.py
+-rwxr-xr-x   0        0        0     6654 2023-07-18 15:17:40.498280 xnbtd-0.0.6/xnbtd/tours/admin.py
+-rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.6/xnbtd/tours/apps.py
+-rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.6/xnbtd/tours/forms.py
+-rwxr-xr-x   0        0        0     3622 2023-07-18 14:53:44.000000 xnbtd-0.0.6/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     6757 2023-07-18 14:52:57.461646 xnbtd-0.0.6/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0     6465 2023-07-17 14:22:40.889949 xnbtd-0.0.6/xnbtd/tours/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-12 14:57:11.196824 xnbtd-0.0.6/xnbtd/tours/migrations/__init__.py
+-rwxr-xr-x   0        0        0     4249 2023-07-17 14:22:40.864888 xnbtd-0.0.6/xnbtd/tours/models.py
+-rwxr-xr-x   0        0        0      113 2023-07-18 13:08:06.430521 xnbtd-0.0.6/xnbtd/urls.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.6/xnbtd/wsgi.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-0.0.6/PKG-INFO
```

### Comparing `xnbtd-0.0.5/LICENSE` & `xnbtd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/README.md` & `xnbtd-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/pyproject.toml` & `xnbtd-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnbtd"
-version = "0.0.5"
+version = "0.0.6"
 description = "xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings."
 authors = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
 maintainers = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
```

### Comparing `xnbtd-0.0.5/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-0.0.6/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po` & `xnbtd-0.0.6/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/plannings/migrations/0001_initial.py` & `xnbtd-0.0.6/xnbtd/plannings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py` & `xnbtd-0.0.6/xnbtd/plannings/migrations/0002_alter_event_date_alter_event_title.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/publish.py` & `xnbtd-0.0.6/xnbtd/publish.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/settings/base.py` & `xnbtd-0.0.6/xnbtd/settings/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
     'django.middleware.locale.LocaleMiddleware',
 ]
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
-        "DIRS": [str(__Path(BASE_PATH, 'xnbtd', 'templates'))],
+        "DIRS": [str(__Path(BASE_PATH, 'templates'))],
         "APP_DIRS": True,
         "OPTIONS": {
             "context_processors": [
                 "django.template.context_processors.debug",
                 "django.template.context_processors.request",
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
```

### Comparing `xnbtd-0.0.5/xnbtd/settings/local.py` & `xnbtd-0.0.6/xnbtd/settings/local.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/tours/admin.py` & `xnbtd-0.0.6/xnbtd/tours/admin.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-0.0.6/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/tours/locale/fr/LC_MESSAGES/django.po` & `xnbtd-0.0.6/xnbtd/tours/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/tours/migrations/0001_initial.py` & `xnbtd-0.0.6/xnbtd/tours/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/xnbtd/tours/models.py` & `xnbtd-0.0.6/xnbtd/tours/models.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.5/PKG-INFO` & `xnbtd-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnbtd
-Version: 0.0.5
+Version: 0.0.6
 Summary: xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings.
 Home-page: https://github.com/eldertek/xnbtd
 License: GPL-3.0-or-later
 Author: André Théo LAURET
 Author-email: andrelauret@eclipse-technology.eu
 Maintainer: André Théo LAURET
 Maintainer-email: andrelauret@eclipse-technology.eu
```

