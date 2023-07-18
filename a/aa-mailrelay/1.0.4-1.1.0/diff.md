# Comparing `tmp/aa-mailrelay-1.0.4.tar.gz` & `tmp/aa_mailrelay-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-mailrelay-1.0.4.tar", last modified: Sun Jul 24 15:27:26 2022, max compression
+gzip compressed data, was "aa_mailrelay-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa-mailrelay-1.0.4.tar` & `aa_mailrelay-1.1.0.tar`

### file list

```diff
@@ -1,59 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.092774 aa-mailrelay-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5073 2022-07-24 15:27:26.092774 aa-mailrelay-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4183 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.081773 aa-mailrelay-1.0.4/aa_mailrelay.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5073 2022-07-24 15:27:25.000000 aa-mailrelay-1.0.4/aa_mailrelay.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1200 2022-07-24 15:27:26.000000 aa-mailrelay-1.0.4/aa_mailrelay.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-24 15:27:25.000000 aa-mailrelay-1.0.4/aa_mailrelay.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2022-07-24 15:27:25.000000 aa-mailrelay-1.0.4/aa_mailrelay.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-24 15:27:25.000000 aa-mailrelay-1.0.4/aa_mailrelay.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.085774 aa-mailrelay-1.0.4/mailrelay/
--rw-rw-rw-   0 root         (0) root         (0)      102 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5737 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      631 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.085774 aa-mailrelay-1.0.4/mailrelay/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1253 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/core/xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.086774 aa-mailrelay-1.0.4/mailrelay/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     4329 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/migrations/0002_django4_update.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7431 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.076773 aa-mailrelay-1.0.4/mailrelay/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.086774 aa-mailrelay-1.0.4/mailrelay/static/mailrelay/
--rw-rw-rw-   0 root         (0) root         (0)     1137 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/static/mailrelay/mailrelay_logo.png
--rw-rw-rw-   0 root         (0) root         (0)     3090 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.078773 aa-mailrelay-1.0.4/mailrelay/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.077773 aa-mailrelay-1.0.4/mailrelay/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.077773 aa-mailrelay-1.0.4/mailrelay/templates/admin/mailrelay/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.087774 aa-mailrelay-1.0.4/mailrelay/templates/admin/mailrelay/relayconfig/
--rw-rw-rw-   0 root         (0) root         (0)      296 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/templates/admin/mailrelay/relayconfig/change_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.087774 aa-mailrelay-1.0.4/mailrelay/templates/mailrelay/
--rw-rw-rw-   0 root         (0) root         (0)      335 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/templates/mailrelay/base.html
--rw-rw-rw-   0 root         (0) root         (0)      478 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/templates/mailrelay/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.090774 aa-mailrelay-1.0.4/mailrelay/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3032 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     3588 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/test_core_xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    12456 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     6749 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1142 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/mailrelay/views.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-07-24 15:27:26.093774 aa-mailrelay-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1649 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-24 15:27:26.092774 aa-mailrelay-1.0.4/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)     9781 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/testauth/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2022-07-24 15:27:17.000000 aa-mailrelay-1.0.4/testauth/wsgi.py
+-rw-r--r--   0        0        0     1070 2023-07-18 12:52:50.441169 aa_mailrelay-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4183 2023-07-18 12:52:50.441169 aa_mailrelay-1.1.0/README.md
+-rw-r--r--   0        0        0      182 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/__init__.py
+-rw-r--r--   0        0        0     5924 2023-07-18 13:56:50.889942 aa_mailrelay-1.1.0/mailrelay/admin.py
+-rw-r--r--   0        0        0      669 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/app_settings.py
+-rw-r--r--   0        0        0      192 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/apps.py
+-rw-r--r--   0        0        0      204 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/auth_hooks.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:08:09.838526 aa_mailrelay-1.1.0/mailrelay/core/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/core/xml_converter.py
+-rw-r--r--   0        0        0     1998 2023-07-18 13:09:43.490081 aa_mailrelay-1.1.0/mailrelay/managers.py
+-rw-r--r--   0        0        0     4328 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/migrations/0001_initial.py
+-rw-r--r--   0        0        0      632 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/migrations/0002_django4_update.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:08:09.838526 aa_mailrelay-1.1.0/mailrelay/migrations/__init__.py
+-rw-r--r--   0        0        0     7773 2023-07-18 13:09:43.490081 aa_mailrelay-1.1.0/mailrelay/models.py
+-rw-r--r--   0        0        0     1137 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/static/mailrelay/mailrelay_logo.png
+-rw-r--r--   0        0        0     3135 2023-07-18 13:09:43.490081 aa_mailrelay-1.1.0/mailrelay/tasks.py
+-rw-r--r--   0        0        0      296 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/templates/admin/mailrelay/relayconfig/change_list.html
+-rw-r--r--   0        0        0      335 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/templates/mailrelay/base.html
+-rw-r--r--   0        0        0      478 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/templates/mailrelay/index.html
+-rw-r--r--   0        0        0        0 2023-07-18 14:08:09.842526 aa_mailrelay-1.1.0/mailrelay/tests/__init__.py
+-rw-r--r--   0        0        0     3320 2023-07-18 13:56:50.889942 aa_mailrelay-1.1.0/mailrelay/tests/factories.py
+-rw-r--r--   0        0        0     5629 2023-07-18 13:56:50.889942 aa_mailrelay-1.1.0/mailrelay/tests/test_admin.py
+-rw-r--r--   0        0        0     1380 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/tests/test_core_xml_converter.py
+-rw-r--r--   0        0        0     3307 2023-07-18 12:52:50.445169 aa_mailrelay-1.1.0/mailrelay/tests/test_integration.py
+-rw-r--r--   0        0        0    12289 2023-07-18 13:56:50.889942 aa_mailrelay-1.1.0/mailrelay/tests/test_models.py
+-rw-r--r--   0        0        0     6694 2023-07-18 13:56:50.889942 aa_mailrelay-1.1.0/mailrelay/tests/test_tasks.py
+-rw-r--r--   0        0        0      370 2023-07-18 12:52:50.449169 aa_mailrelay-1.1.0/mailrelay/tests/test_utils.py
+-rw-r--r--   0        0        0     1439 2023-07-18 12:52:50.449169 aa_mailrelay-1.1.0/mailrelay/tests/test_views.py
+-rw-r--r--   0        0        0      272 2023-07-18 12:52:50.449169 aa_mailrelay-1.1.0/mailrelay/urls.py
+-rw-r--r--   0        0        0      531 2023-07-18 12:52:50.449169 aa_mailrelay-1.1.0/mailrelay/utils.py
+-rw-r--r--   0        0        0     1218 2023-07-18 12:52:50.449169 aa_mailrelay-1.1.0/mailrelay/views.py
+-rw-r--r--   0        0        0     1772 2023-07-18 12:52:50.449169 aa_mailrelay-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 aa_mailrelay-1.1.0/PKG-INFO
```

### Comparing `aa-mailrelay-1.0.4/LICENSE` & `aa_mailrelay-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-mailrelay-1.0.4/PKG-INFO` & `aa_mailrelay-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: aa-mailrelay
-Version: 1.0.4
-Summary: An app for relaying Eve mails to Discord
-Home-page: https://gitlab.com/ErikKalkoken/aa-mailrelay
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Version: 1.1.0
+Summary: An app for relaying Eve mails to Discord.
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: aa-memberaudit>=2
+Requires-Dist: allianceauth-app-utils>=1.19
+Requires-Dist: allianceauth>=3
+Requires-Dist: discordproxy>=1
+Requires-Dist: django-eveuniverse>=1
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-mailrelay
 
 # Mailrelay
 
 An app for relaying Eve mails to Discord.
 
 [![release](https://img.shields.io/pypi/v/aa-mailrelay?label=release)](https://pypi.org/project/aa-mailrelay/)
 [![python](https://img.shields.io/pypi/pyversions/aa-mailrelay)](https://pypi.org/project/aa-mailrelay/)
@@ -117,8 +119,7 @@
 Name | Description | Default
 -- | -- | --
 `MAILRELAY_DISCORD_TASK_TIMEOUT`| Timeout for asynchronous Discord requests in seconds. | `60`
 `MAILRELAY_DISCORD_USER_TIMEOUT`| Timeout for user facing Discord requests in seconds. | `30`
 `MAILRELAY_OLDEST_MAIL_HOURS`| Oldest mail to be forwarded in hours. | `2`
 `MAILRELAY_RELAY_GRACE_MINUTES`| Max time in minutes since last successful service run before config is reported as down. | `30`
 
-
```

### Comparing `aa-mailrelay-1.0.4/README.md` & `aa_mailrelay-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-mailrelay-1.0.4/mailrelay/admin.py` & `aa_mailrelay-1.1.0/mailrelay/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Admin site for Mail Relay."""
+# pylint: disable=missing-class-docstring,missing-function-docstring
+
 from collections import defaultdict
 
 from discordproxy.client import DiscordClient
 from discordproxy.exceptions import DiscordProxyException
 
 from django.conf import settings
 from django.contrib import admin
@@ -15,14 +18,16 @@
 from .app_settings import MAILRELAY_DISCORD_USER_TIMEOUT
 from .models import DiscordCategory, DiscordChannel, RelayConfig
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class RelayConfigForm(ModelForm):
+    """Form for RelayConfig objects."""
+
     class Meta:
         model = RelayConfig
         fields = (
             "character",
             "mail_category",
             "discord_channel",
             "ping_type",
@@ -78,15 +83,15 @@
         return str(obj.discord_channel)
 
     @admin.display(boolean=True)
     def _is_service_up(self, obj) -> bool:
         return obj.is_service_up
 
     def _organization(self, obj) -> str:
-        eve_character = obj.character.character_ownership.character
+        eve_character = obj.character.eve_character
         return format_html(
             "{}<br>{}",
             eve_character.corporation_name,
             eve_character.alliance_name if eve_character.alliance_name else "",
         )
 
     @admin.action(description="Send test message for selected configurations")
@@ -109,40 +114,46 @@
             else:
                 items_count += 1
         if items_count:
             self.message_user(
                 request, f"Submitted {items_count} successful test message(s)."
             )
 
-    if settings.DEBUG:
+    @admin.action(description="Resend mails for selected configurations")
+    def resent_mails(self, request, queryset):
+        items_count = 0
+        mails_count = 0
+        for obj in queryset:
+            obj.mails_sent.clear()
+            new_mails_qs = obj.new_mails_queryset()
+            mails_sent = 0
+            for mail in new_mails_qs:
+                try:
+                    obj.send_mail(mail, timeout=MAILRELAY_DISCORD_USER_TIMEOUT)
+                except DiscordProxyException as ex:
+                    logger.error(
+                        "%s: Failed to send test message for", obj, exc_info=True
+                    )
+                    self.message_user(
+                        request,
+                        f"{obj}: Failed to send test message: {ex}",
+                        level="WARNING",
+                    )
+                else:
+                    mails_sent += 1
 
-        @admin.action(description="Resend mails for selected configurations")
-        def resent_mails(self, request, queryset):
-            items_count = 0
-            for obj in queryset:
-                obj.mails_sent.clear()
-                new_mails_qs = obj.new_mails_queryset()
-                for mail in new_mails_qs:
-                    try:
-                        obj.send_mail(mail, timeout=MAILRELAY_DISCORD_USER_TIMEOUT)
-                    except DiscordProxyException as ex:
-                        logger.error(
-                            "%s: Failed to send test message for", obj, exc_info=True
-                        )
-                        self.message_user(
-                            request,
-                            f"{obj}: Failed to send test message: {ex}",
-                            level="WARNING",
-                        )
+            if mails_sent > 0:
+                mails_count += mails_sent
                 items_count += 1
-            if items_count > 0:
-                self.message_user(
-                    request,
-                    f"Resent {new_mails_qs.count()} mails for {items_count} config(s).",
-                )
+
+        if items_count > 0:
+            self.message_user(
+                request,
+                f"Resent {mails_count} mails for {items_count} config(s).",
+            )
 
 
 if settings.DEBUG:
 
     @admin.register(DiscordChannel)
     class DiscordChannelAdmin(admin.ModelAdmin):
         list_display = ("id", "name", "category")
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/core/xml_converter.py` & `aa_mailrelay-1.1.0/mailrelay/core/xml_converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+"""Converters for XML."""
+
 import unicodedata
 
 from bs4 import BeautifulSoup
 
 from eveuniverse.core import evexml
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
-from .. import __title__
+from mailrelay import __title__
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def eve_xml_to_discord_markup(xml_doc: str) -> str:
     """Converts Eve Online xml to Discord markup."""
     xml_doc = unicodedata.normalize("NFKC", xml_doc)
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/managers.py` & `aa_mailrelay-1.1.0/mailrelay/managers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+"""Managers for Mail Relay."""
+
+from typing import Optional
+
 from discordproxy.client import Channel, DiscordClient
 
 from django.conf import settings
 from django.db import models
 
 
 class DiscordChannelManager(models.Manager):
-    def sync(self, timeout: int = None) -> int:
+    """Manager for DiscordChannel."""
+
+    def sync(self, timeout: Optional[int] = None) -> int:
         """Synchronize list of guild channels objects with the Discord server.
 
         Args:
         - timeout: timeout for request to Discord in seconds
 
         Returns:
         number of channels
@@ -18,25 +24,27 @@
 
         try:
             guild_id = int(settings.DISCORD_GUILD_ID)
         except AttributeError:
             raise ValueError(
                 "Can not find Discord guild ID in settings. "
                 "Is the Discord service configured?"
-            )
+            ) from None
         client = DiscordClient(timeout=timeout)
         channels = client.get_guild_channels(guild_id)
+        # pylint: disable=no-member
         categories = {
             obj.id: obj for obj in channels if obj.type == Channel.Type.GUILD_CATEGORY
         }
         for category in categories.values():
             DiscordCategory.objects.update_or_create(
                 id=category.id, defaults={"name": category.name}
             )
         channel_ids = set()
+        # pylint: disable=no-member
         text_channels = [obj for obj in channels if obj.type == Channel.Type.GUILD_TEXT]
         for channel in text_channels:
             if channel.parent_id and channel.parent_id in categories:
                 category_id = channel.parent_id
             else:
                 category_id = None
             self.update_or_create(
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/migrations/0001_initial.py` & `aa_mailrelay-1.1.0/mailrelay/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.9 on 2022-01-02 20:11
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("memberaudit", "0006_add_current_ship"),
     ]
 
     operations = [
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/migrations/0002_django4_update.py` & `aa_mailrelay-1.1.0/mailrelay/migrations/0002_django4_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.0.3 on 2022-03-02 17:25
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("memberaudit", "0007_add_exports_permission"),
         ("mailrelay", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/models.py` & `aa_mailrelay-1.1.0/mailrelay/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Models for Mail Relay."""
+
 import datetime as dt
 from typing import List, Optional
 
 from discordproxy.client import DiscordClient
 from discordproxy.discord_api_pb2 import Embed
 from memberaudit.models import Character, CharacterMail
 
@@ -19,20 +21,26 @@
 from .managers import DiscordChannelManager
 from .utils import chunks_by_lines
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class RelayConfig(models.Model):
+    """A configuration for mail relay."""
+
     class ChannelPingType(models.TextChoices):
+        """A ping type."""
+
         NONE = "PN", "(none)"
         HERE = "PH", "@here"
         EVERYBODY = "PE", "@everybody"  # TODO: Rename to EVERYONE with next migration
 
     class MailCategory(models.TextChoices):
+        """A mail category."""
+
         ALL = "AL", "All mails"
         ALLIANCE = "AM", "Alliance mails"
         CORPORATION = "CM", "Corporation mails"
 
     character = models.ForeignKey(Character, on_delete=models.CASCADE)
     discord_channel = models.ForeignKey(
         "DiscordChannel", on_delete=models.SET_NULL, null=True
@@ -67,16 +75,18 @@
     )
 
     def __str__(self) -> str:
         return f"#{self.pk}"
 
     @property
     def is_service_up(self) -> Optional[bool]:
+        """Return True if service is up, else False."""
         if not self.last_service_run_at:
             return None
+
         return now() - self.last_service_run_at < dt.timedelta(
             minutes=MAILRELAY_RELAY_GRACE_MINUTES
         )
 
     def new_mails_queryset(self) -> models.QuerySet:
         """Determine which mails have not yet been sent."""
         oldest_timestamp = now() - dt.timedelta(hours=MAILRELAY_OLDEST_MAIL_HOURS)
@@ -85,37 +95,39 @@
             self.character.mails.select_related("sender")
             .exclude(pk__in=self.mails_sent.values_list("pk", flat=True))
             .filter(timestamp__gte=oldest_timestamp)
         )
         if self.mail_category == self.MailCategory.ALL:
             pass
         elif self.mail_category == self.MailCategory.ALLIANCE:
-            alliance_id = self.character.character_ownership.character.alliance_id
+            alliance_id = self.character.eve_character.alliance_id
             if alliance_id:
                 new_mails_qs = new_mails_qs.filter(recipients__id=alliance_id)
             else:
                 new_mails_qs = new_mails_qs.none()
         elif self.mail_category == self.MailCategory.CORPORATION:
-            corporation_id = self.character.character_ownership.character.corporation_id
+            corporation_id = self.character.eve_character.corporation_id
             new_mails_qs = new_mails_qs.filter(recipients__id=corporation_id)
         else:
             raise NotImplementedError(f"Unknown mail category: {self.mail_category}")
         return new_mails_qs
 
-    def send_mail(self, mail: CharacterMail, timeout: int = None) -> None:
+    def send_mail(self, mail: CharacterMail, timeout: Optional[int] = None) -> None:
         """Send one mail to channel.
 
         Args:
         - mail: mail to be sent
         - timeout: timeout for request to Discord in seconds
         """
         if not mail.body:
             return
+
         if not self.discord_channel:
             raise ValueError(f"No channel configured for config {self}")
+
         client = DiscordClient(timeout=timeout)
         embeds = self._generate_embeds(mail)
         for num, embed in enumerate(embeds, start=1):
             content = self._content_with_mentions() if num == 1 else ""
             client.create_channel_message(
                 channel_id=self.discord_channel.id, content=content, embed=embed
             )
@@ -136,17 +148,19 @@
             title = "Eve"
         return f"{mention}**New {title} Mail**"
 
     def _generate_embeds(self, mail: CharacterMail) -> List[Embed]:
         recipients = ", ".join(
             [obj.name_plus for obj in mail.recipients.order_by("name")]
         )
+        from_name = mail.sender.name_plus if mail.sender else "?"
+        sent_text = mail.timestamp.strftime(DATETIME_FORMAT) if mail.timestamp else "?"
         full_description = (
-            f"**From**: {mail.sender.name_plus}\n"
-            f"**Sent**: {mail.timestamp.strftime(DATETIME_FORMAT)}\n"
+            f"**From**: {from_name}\n"
+            f"**Sent**: {sent_text}\n"
             f"**To**: {recipients}\n\n"
         )
         full_description += eve_xml_to_discord_markup(mail.body)
         description_chunks = chunks_by_lines(full_description, 3500)
         chunks_count = len(description_chunks)
         footer_icon_url = static_file_absolute_url("mailrelay/mailrelay_logo.png")
         embeds = []
@@ -167,14 +181,16 @@
     def record_service_run(self):
         """Record successful service run."""
         self.last_service_run_at = now()
         self.save(update_fields=["last_service_run_at"])
 
 
 class DiscordChannel(models.Model):
+    """A Discord channel."""
+
     id = models.BigIntegerField(primary_key=True)
     name = models.CharField(max_length=100, db_index=True)
     category = models.ForeignKey(
         "DiscordCategory",
         on_delete=models.SET_DEFAULT,
         default=None,
         null=True,
@@ -187,13 +203,15 @@
     def __str__(self) -> str:
         if self.category:
             return f"{self.category.name} / {self.name}"
         return str(self.name)
 
 
 class DiscordCategory(models.Model):
+    """A Discord category."""
+
     id = models.BigIntegerField(primary_key=True)
     name = models.CharField(max_length=100, db_index=True)
     last_update_at = models.DateTimeField(auto_now=True)
 
     def __str__(self) -> str:
         return str(self.name)
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/static/mailrelay/mailrelay_logo.png` & `aa_mailrelay-1.1.0/mailrelay/static/mailrelay/mailrelay_logo.png`

 * *Files identical despite different names*

### Comparing `aa-mailrelay-1.0.4/mailrelay/tasks.py` & `aa_mailrelay-1.1.0/mailrelay/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Tasks for Mail Relay."""
+
 from celery import chain, shared_task
 from discordproxy.exceptions import DiscordProxyException
 from memberaudit.models import Character
 from memberaudit.tasks import (
     update_character_mail_bodies,
     update_character_mail_headers,
     update_character_mail_labels,
@@ -68,15 +70,15 @@
 
 @shared_task
 def forward_mail_to_discord(config_pk, mail_pk):
     """Forward one mail to Discord."""
     config = RelayConfig.objects.select_related("character", "discord_channel").get(
         pk=config_pk
     )
-    mail = config.character.mails.get(pk=mail_pk)
+    mail = config.character.mails.get(pk=mail_pk)  # type: ignore
     try:
         config.send_mail(mail=mail, timeout=MAILRELAY_DISCORD_TASK_TIMEOUT)
     except DiscordProxyException as ex:
         logger.error(
             "%s: Failed to send mail %s due to error from Discord Proxy. Will try again later: %s",
             config,
             mail,
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/tests/factories.py` & `aa_mailrelay-1.1.0/mailrelay/tests/factories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime as dt
 
+from discordproxy.discord_api_pb2 import Channel
 from memberaudit.models import CharacterMail, MailEntity
 from pytz import utc
 
 from django.contrib.auth.models import User
 from eveuniverse.models import EveEntity
 
-from ..models import DiscordCategory, DiscordChannel, RelayConfig
+from mailrelay.models import DiscordCategory, DiscordChannel, RelayConfig
 
 
 class FakeRequest(object):
     def __init__(self, user=None):
         self.user = user
 
 
@@ -66,15 +67,15 @@
             "subject": f"subject #{mail_id}",
             "is_read": False,
             "mail_id": mail_id,
             "sender": sender,
         }
     )
     mail = CharacterMail.objects.create(**kwargs)
-    recipient_ids += [character.character_ownership.character.character_id]
+    recipient_ids += [character.eve_character.character_id]
     recipient_objs = [
         MailEntity.objects.update_or_create_from_eve_entity_id(id=recipient_id)[0]
         for recipient_id in recipient_ids
     ]
     mail.recipients.add(*recipient_objs)
     return mail
 
@@ -101,7 +102,18 @@
 
 def create_superuser(**kwargs):
     return User.objects.create_superuser(**kwargs)
 
 
 def create_fake_request(**kwargs):
     return FakeRequest(**kwargs)
+
+
+# Discordproxy
+
+
+def create_discordproxy_channel(**kwargs) -> Channel:
+    if "id" not in kwargs:
+        kwargs["id"] = next(unique_ids)
+    if "type" not in kwargs:
+        kwargs["type"] = Channel.Type.GUILD_TEXT
+    return Channel(**kwargs)
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/tests/test_admin.py` & `aa_mailrelay-1.1.0/mailrelay/tests/test_admin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from unittest.mock import patch
 
 from discordproxy.exceptions import DiscordProxyException
 from memberaudit.tests.utils import add_memberaudit_character_to_user
 
 from django.contrib.admin.sites import AdminSite
 from django.test import TestCase
+from django.utils.timezone import now
 
 from app_utils.testing import create_fake_user
 
-from ..admin import RelayConfigAdmin
-from ..models import RelayConfig
+from mailrelay.admin import RelayConfigAdmin
+from mailrelay.models import RelayConfig
+
 from .factories import (
+    create_character_mail,
     create_discord_category,
     create_discord_channel,
+    create_eve_entities_from_evecharacter,
+    create_eve_entity,
     create_fake_request,
     create_relay_config,
     create_superuser,
 )
 
 ADMIN_MODULE = "mailrelay.admin"
+MODELS_MODULE = "mailrelay.models"
 
 
 class TestRelayConfigAdmin(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.modeladmin = RelayConfigAdmin(model=RelayConfig, admin_site=AdminSite())
@@ -93,7 +99,46 @@
         # given
         create_discord_channel(name="City Hall")
         self.client.force_login(self.admin_user)
         # when
         response = self.client.get("/admin/mailrelay/relayconfig/")
         # then
         self.assertEqual(response.status_code, 200)
+
+    @patch(ADMIN_MODULE + ".RelayConfigAdmin.message_user")
+    @patch(ADMIN_MODULE + ".RelayConfig.send_mail")
+    def test_action_resent_mails_should_sent(self, mock_send_mail, mock_message_user):
+        # given
+        create_eve_entities_from_evecharacter(self.character.eve_character)
+        create_eve_entity(id=1002, name="Peter Parker")
+        create_character_mail(character=self.character, sender_id=1002, timestamp=now())
+        create_relay_config(character=self.character)
+        request = create_fake_request(user=self.admin_user)
+        queryset = RelayConfig.objects.all()
+        # when
+        self.modeladmin.resent_mails(request, queryset)
+        # then
+        self.assertEqual(mock_send_mail.call_count, 1)
+        self.assertTrue(mock_message_user.called)
+        _, kwargs = mock_message_user.call_args
+        self.assertNotIn("level", kwargs)
+
+    @patch(ADMIN_MODULE + ".RelayConfigAdmin.message_user")
+    @patch(ADMIN_MODULE + ".RelayConfig.send_mail")
+    def test_action_resent_mails_should_sent_should_handle_error(
+        self, mock_send_mail, mock_message_user
+    ):
+        # given
+        mock_send_mail.side_effect = DiscordProxyException
+        create_eve_entities_from_evecharacter(self.character.eve_character)
+        create_eve_entity(id=1002, name="Peter Parker")
+        create_character_mail(character=self.character, sender_id=1002, timestamp=now())
+        create_relay_config(character=self.character)
+        request = create_fake_request(user=self.admin_user)
+        queryset = RelayConfig.objects.all()
+        # when
+        self.modeladmin.resent_mails(request, queryset)
+        # then
+        self.assertEqual(mock_send_mail.call_count, 1)
+        self.assertTrue(mock_message_user.called)
+        _, kwargs = mock_message_user.call_args
+        self.assertEqual(kwargs["level"], "WARNING")
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/tests/test_core_xml_converter.py` & `aa_mailrelay-1.1.0/mailrelay/tests/test_core_xml_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.test import TestCase
 
-from ..core.xml_converter import eve_xml_to_discord_markup
+from mailrelay.core.xml_converter import eve_xml_to_discord_markup
 
 
 class TestXmlToMarkup(TestCase):
     def test_should_replace_line_breaks(self):
         # when
         result = eve_xml_to_discord_markup("alpha<br>bravo<br><br>charlie")
         # then
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/tests/test_integration.py` & `aa_mailrelay-1.1.0/mailrelay/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from memberaudit.tests.utils import add_memberaudit_character_to_user
 from pytz import utc
 
 from django.test import override_settings
 
 from app_utils.testing import NoSocketsTestCase, create_fake_user
 
-from ..models import RelayConfig
-from ..tasks import forward_new_mails
+from mailrelay.models import RelayConfig
+from mailrelay.tasks import forward_new_mails
+
 from .factories import (
     create_character_mail,
     create_eve_entities_from_evecharacter,
     create_eve_entity,
     create_relay_config,
 )
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/tests/test_models.py` & `aa_mailrelay-1.1.0/mailrelay/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import datetime as dt
 from unittest.mock import patch
 
 from discordproxy.client import Channel
-from discordproxy.tests.factories import create_discordproxy_channel
 from memberaudit.tests.utils import add_memberaudit_character_to_user
 from pytz import utc
 
 from app_utils.testing import NoSocketsTestCase, create_fake_user
 
-from ..models import DiscordCategory, DiscordChannel, RelayConfig
+from mailrelay.models import DiscordCategory, DiscordChannel, RelayConfig
+
 from .factories import (
     create_character_mail,
     create_discord_category,
     create_discord_channel,
+    create_discordproxy_channel,
     create_eve_entities_from_evecharacter,
     create_eve_entity,
     create_relay_config,
 )
 
 MODELS_PATH = "mailrelay.models"
 MANAGERS_PATH = "mailrelay.managers"
@@ -24,17 +25,15 @@
 
 class TestRelayConfigNewMailsQueryset(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         user = create_fake_user(1001, "Bruce Wayne")
         cls.character = add_memberaudit_character_to_user(user, 1001)
-        create_eve_entities_from_evecharacter(
-            cls.character.character_ownership.character
-        )
+        create_eve_entities_from_evecharacter(cls.character.eve_character)
         create_eve_entity(id=1002, name="Peter Parker")
 
     def test_should_return_corporation_mails_only(self):
         # given
         corporation_mail = create_character_mail(
             character=self.character, sender_id=1002, recipient_ids=[2001]
         )
@@ -75,18 +74,18 @@
             {alliance_mail.pk}, set(result.values_list("pk", flat=True))
         )
 
     def test_should_not_return_alliance_mails(self):
         # given
         user = create_fake_user(1003, "Clark Kent", 2009, "Wayne Food", "WYF")
         character = add_memberaudit_character_to_user(user, 1003)
-        character.character_ownership.character.alliance_id = None
-        character.character_ownership.character.alliance_name = ""
-        character.character_ownership.character.save()
-        create_eve_entities_from_evecharacter(character.character_ownership.character)
+        character.eve_character.alliance_id = None
+        character.eve_character.alliance_name = ""
+        character.eve_character.save()
+        create_eve_entities_from_evecharacter(character.eve_character)
         create_character_mail(character=character, sender_id=1002, recipient_ids=[3001])
         create_character_mail(character=character, sender_id=1002)
         create_character_mail(character=character, sender_id=1002, recipient_ids=[2001])
         config = create_relay_config(
             character=character, mail_category=RelayConfig.MailCategory.ALLIANCE
         )
         # when
@@ -145,17 +144,15 @@
 @patch(MODELS_PATH + ".DiscordClient.create_channel_message")
 class TestRelayConfigSendMail(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         user = create_fake_user(1001, "Bruce Wayne")
         cls.character = add_memberaudit_character_to_user(user, 1001)
-        create_eve_entities_from_evecharacter(
-            cls.character.character_ownership.character
-        )
+        create_eve_entities_from_evecharacter(cls.character.eve_character)
         create_eve_entity(id=1002, name="Peter Parker")
 
     def test_should_send_valid_mail(self, mock_create_channel_message):
         # given
         mail = create_character_mail(character=self.character, sender_id=1002)
         config = create_relay_config(character=self.character)
         # when
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/tests/test_tasks.py` & `aa_mailrelay-1.1.0/mailrelay/tests/test_tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from memberaudit.tests.utils import add_memberaudit_character_to_user
 from pytz import utc
 
 from django.test import override_settings
 
 from app_utils.testing import NoSocketsTestCase, create_fake_user
 
-from ..tasks import (
+from mailrelay.tasks import (
     forward_mail_to_discord,
     forward_new_mails,
     forward_new_mails_for_config,
 )
+
 from .factories import (
     create_character_mail,
     create_eve_entities_from_evecharacter,
     create_eve_entity,
     create_relay_config,
 )
 
@@ -71,15 +72,15 @@
 @patch(MODELS_PATH + ".RelayConfig.send_mail")
 class TestForwardNewMailsOneConfig(NoSocketsTestCase):
     def test_should_forward_all_mails(self, mock_send_mail):
         # given
         mock_send_mail.return_value = True
         user = create_fake_user(1001, "Bruce Wayne")
         character = add_memberaudit_character_to_user(user, 1001)
-        create_eve_entities_from_evecharacter(character.character_ownership.character)
+        create_eve_entities_from_evecharacter(character.eve_character)
         create_eve_entity(id=1002, name="Peter Parker")
         mail_1 = create_character_mail(
             character=character, sender_id=1002, recipient_ids=[2001]
         )
         mail_2 = create_character_mail(character=character, sender_id=1002)
         config = create_relay_config(character=character)
         # when
@@ -93,15 +94,15 @@
         self.assertIsNotNone(config.last_service_run_at)
 
     def test_handle_no_new_mails(self, mock_send_mail):
         # given
         mock_send_mail.return_value = True
         user = create_fake_user(1001, "Bruce Wayne")
         character = add_memberaudit_character_to_user(user, 1001)
-        create_eve_entities_from_evecharacter(character.character_ownership.character)
+        create_eve_entities_from_evecharacter(character.eve_character)
         create_eve_entity(id=1002, name="Peter Parker")
         mail = create_character_mail(character=character, sender_id=1002)
         config = create_relay_config(character=character)
         config.mails_sent.add(mail)
         # when
         with patch(MODELS_PATH + ".now") as mock_now:
             mock_now.return_value = dt.datetime(2021, 12, 24, 12, 30, tzinfo=utc)
@@ -116,15 +117,15 @@
 @patch(MODELS_PATH + ".RelayConfig.send_mail")
 class TestForwardMailToDiscord(NoSocketsTestCase):
     def test_should_send_mail(self, mock_send_mail):
         # given
         mock_send_mail.return_value = True
         user = create_fake_user(1001, "Bruce Wayne")
         character = add_memberaudit_character_to_user(user, 1001)
-        create_eve_entities_from_evecharacter(character.character_ownership.character)
+        create_eve_entities_from_evecharacter(character.eve_character)
         create_eve_entity(id=1002, name="Peter Parker")
         mail = create_character_mail(character=character, sender_id=1002)
         config = create_relay_config(character=character)
         # when
         forward_mail_to_discord(config_pk=config.pk, mail_pk=mail.pk)
         # then
         self.assertEqual(mock_send_mail.call_count, 1)
@@ -135,15 +136,15 @@
         # given
         my_error = DiscordProxyTimeoutError(
             status=GrpcStatusCode.DEADLINE_EXCEEDED, details="test"
         )
         mock_send_mail.side_effect = my_error
         user = create_fake_user(1001, "Bruce Wayne")
         character = add_memberaudit_character_to_user(user, 1001)
-        create_eve_entities_from_evecharacter(character.character_ownership.character)
+        create_eve_entities_from_evecharacter(character.eve_character)
         create_eve_entity(id=1002, name="Peter Parker")
         mail = create_character_mail(character=character, sender_id=1002)
         config = create_relay_config(character=character)
         # when
         forward_mail_to_discord(config_pk=config.pk, mail_pk=mail.pk)
         # then
         pass
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/tests/test_views.py` & `aa_mailrelay-1.1.0/mailrelay/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from discordproxy.exceptions import DiscordProxyException
 
 from django.test import RequestFactory
 
 from app_utils.testing import NoSocketsTestCase
 
-from ..views import admin_update_discord_channels
+from mailrelay.views import admin_update_discord_channels
+
 from .factories import create_superuser
 
 VIEWS_PATH = "mailrelay.views"
 
 
 @patch(VIEWS_PATH + ".DiscordChannel.objects.sync")
 @patch(VIEWS_PATH + ".messages")
```

### Comparing `aa-mailrelay-1.0.4/mailrelay/views.py` & `aa_mailrelay-1.1.0/mailrelay/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Views for Mail Relay."""
+
 from discordproxy.exceptions import DiscordProxyException
 
 from django.contrib import messages
 from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required
 from django.shortcuts import redirect
 
@@ -14,14 +16,15 @@
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 @login_required
 @staff_member_required
 def admin_update_discord_channels(request):
+    """View to update the discord channels."""
     try:
         channels_count = DiscordChannel.objects.sync(
             timeout=MAILRELAY_DISCORD_USER_TIMEOUT
         )
         messages.success(
             request, f"Successfully updated {channels_count} channels from Discord."
         )
```

