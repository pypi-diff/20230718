# Comparing `tmp/alerta-blackout-regex-3.0.0.tar.gz` & `tmp/alerta-blackout-regex-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alerta-blackout-regex-3.0.0.tar", last modified: Tue Oct 25 08:41:51 2022, max compression
+gzip compressed data, was "alerta-blackout-regex-3.1.0.tar", last modified: Tue Jul 18 14:03:43 2023, max compression
```

## Comparing `alerta-blackout-regex-3.0.0.tar` & `alerta-blackout-regex-3.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:41:51.647989 alerta-blackout-regex-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11343 2022-10-25 08:41:36.000000 alerta-blackout-regex-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3437 2022-10-25 08:41:51.647989 alerta-blackout-regex-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-10-25 08:41:36.000000 alerta-blackout-regex-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:41:51.647989 alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3437 2022-10-25 08:41:51.000000 alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-10-25 08:41:51.000000 alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 08:41:51.000000 alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-25 08:41:51.000000 alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-25 08:41:51.000000 alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 08:41:51.000000 alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     8358 2022-10-25 08:41:36.000000 alerta-blackout-regex-3.0.0/blackout_regex.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-10-25 08:41:51.651989 alerta-blackout-regex-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-25 08:41:36.000000 alerta-blackout-regex-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:43.055954 alerta-blackout-regex-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-18 14:03:36.000000 alerta-blackout-regex-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-18 14:03:43.055954 alerta-blackout-regex-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-18 14:03:36.000000 alerta-blackout-regex-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:43.055954 alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-18 14:03:43.000000 alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 14:03:43.000000 alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:03:43.000000 alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 14:03:43.000000 alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 14:03:43.000000 alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:03:43.000000 alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-18 14:03:36.000000 alerta-blackout-regex-3.1.0/blackout_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 14:03:43.055954 alerta-blackout-regex-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 14:03:36.000000 alerta-blackout-regex-3.1.0/setup.py
```

### Comparing `alerta-blackout-regex-3.0.0/LICENSE` & `alerta-blackout-regex-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alerta-blackout-regex-3.0.0/PKG-INFO` & `alerta-blackout-regex-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta-blackout-regex
-Version: 3.0.0
+Version: 3.1.0
 Summary: Alerta Blackout enhancement plugin
 Home-page: https://github.com/mirceaulinic/alerta-blackout-regex
 Author: Mircea Ulinic
 Author-email: ping@mirceaulinic.net
 License: Apache License 2.0
 License-File: LICENSE
 
@@ -35,15 +35,15 @@
     That said, the plugin has been changed to process the alert in 
     ``pre_receive`` and therefore before the alert has been correlated. As the 
     Blackouts are retrieved from the Alerta API as unfortunately there's no 
     other way to gather the Blackouts from a plugin via other internal 
     mechanisms, processing each and every alert throguh `pre_receive` would put 
     a lot more workload on your Alerta API. To reduce this, the 
     `blackout_regex` plugin now caches the Blackouts locally, into a file. To 
-    fine tune this behaviour for your own setuo you are able to set a few 
+    fine tune this behaviour for your own setup you are able to set a few 
     environment variables. See more details below, under the _Configuration_ 
     section.
 
 .. note::
 
     Starting with version 3.0.0 onwards, the plugin will gather the list of 
     Blackouts straight from the database (instead of using the API, as
```

### Comparing `alerta-blackout-regex-3.0.0/README.rst` & `alerta-blackout-regex-3.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     That said, the plugin has been changed to process the alert in 
     ``pre_receive`` and therefore before the alert has been correlated. As the 
     Blackouts are retrieved from the Alerta API as unfortunately there's no 
     other way to gather the Blackouts from a plugin via other internal 
     mechanisms, processing each and every alert throguh `pre_receive` would put 
     a lot more workload on your Alerta API. To reduce this, the 
     `blackout_regex` plugin now caches the Blackouts locally, into a file. To 
-    fine tune this behaviour for your own setuo you are able to set a few 
+    fine tune this behaviour for your own setup you are able to set a few 
     environment variables. See more details below, under the _Configuration_ 
     section.
 
 .. note::
 
     Starting with version 3.0.0 onwards, the plugin will gather the list of 
     Blackouts straight from the database (instead of using the API, as
```

### Comparing `alerta-blackout-regex-3.0.0/alerta_blackout_regex.egg-info/PKG-INFO` & `alerta-blackout-regex-3.1.0/alerta_blackout_regex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta-blackout-regex
-Version: 3.0.0
+Version: 3.1.0
 Summary: Alerta Blackout enhancement plugin
 Home-page: https://github.com/mirceaulinic/alerta-blackout-regex
 Author: Mircea Ulinic
 Author-email: ping@mirceaulinic.net
 License: Apache License 2.0
 License-File: LICENSE
 
@@ -35,15 +35,15 @@
     That said, the plugin has been changed to process the alert in 
     ``pre_receive`` and therefore before the alert has been correlated. As the 
     Blackouts are retrieved from the Alerta API as unfortunately there's no 
     other way to gather the Blackouts from a plugin via other internal 
     mechanisms, processing each and every alert throguh `pre_receive` would put 
     a lot more workload on your Alerta API. To reduce this, the 
     `blackout_regex` plugin now caches the Blackouts locally, into a file. To 
-    fine tune this behaviour for your own setuo you are able to set a few 
+    fine tune this behaviour for your own setup you are able to set a few 
     environment variables. See more details below, under the _Configuration_ 
     section.
 
 .. note::
 
     Starting with version 3.0.0 onwards, the plugin will gather the list of 
     Blackouts straight from the database (instead of using the API, as
```

### Comparing `alerta-blackout-regex-3.0.0/blackout_regex.py` & `alerta-blackout-regex-3.1.0/blackout_regex.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 =====================
 
 Alerta plugin to enhance the blackout system.
 """
 import re
 import logging
 
-from alerta.app import db
+from alerta.models.blackout import Blackout
 from alerta.plugins import PluginBase
+from alerta.exceptions import BlackoutPeriod
 
 log = logging.getLogger("alerta.plugins.blackout_regex")
 
 
 def parse_tags(tag_list):
     return {k: v for k, v in (i.split("=", 1) for i in tag_list if "=" in i)}
 
 
 class BlackoutRegex(PluginBase):
     def _fetch_blackouts(self):
         try:
-            count = db.get_blackouts_count()
-            log.debug("There are %d Blackouts currently open", count)
-            blackouts = db.get_blackouts(page=1, page_size=count)
+            # retrieve all blackouts from the DB.
+            # use the alerta blackout model to retrieve the blackouts.
+            # The model standardizes the data returned from mongodb and postgres db.
+            count = Blackout.count()
+            log.debug(f"There are {count} Blackouts currently open")
+            blackouts = Blackout.find_all(page=1, page_size=count)
             log.debug("Retrieved Blackouts from the DB:")
             log.debug(blackouts)
         except Exception:
             log.debug("Unable to retrieve the Blackouts from the DB", exc_info=True)
             blackouts = []
         return blackouts
 
@@ -49,14 +53,18 @@
 
         if alert.status == "closed":
             log.debug("Alert %s status is closed, ignoring", alert.id)
             return alert
 
         blackouts = self._fetch_blackouts()
 
+        NOTIFICATION_BLACKOUT = self.get_config(
+            "NOTIFICATION_BLACKOUT", default=False, type=bool
+        )
+
         alert_tags = parse_tags(alert.tags)
 
         # When an alert matches a blackout, this plugin adds a special tag
         # ``regex_blackout`` that points to the blackout ID matched.
         # This facilitates the blackout matching, by simply checking if the
         # blackout is still open.
         if "regex_blackout" in alert_tags:
@@ -110,14 +118,28 @@
                     continue
                 match = True
                 log.debug(
                     "%s matched %s",
                     blackout.environment,
                     alert.environment,
                 )
+            if blackout.customer:
+                if not re.search(blackout.customer, alert.customer):
+                    log.debug(
+                        "%s doesn't match the blackout customer %s",
+                        alert.customer,
+                        blackout.customer,
+                    )
+                    continue
+                match = True
+                log.debug(
+                    "%s matched %s",
+                    blackout.customer,
+                    alert.customer,
+                )
             if blackout.group:
                 if not re.search(blackout.group, alert.group):
                     log.debug(
                         "%s doesn't match the blackout group %s",
                         alert.group,
                         blackout.group,
                     )
@@ -178,14 +200,19 @@
                         "%s don't seem to match the blackout tag(s) %s",
                         str(alert_tags),
                         str(blackout_tags),
                     )
                     continue
                 match = True
             if match:
+                if not NOTIFICATION_BLACKOUT:
+                    log.debug(
+                        f"Suppressed alert during blackout period (id={alert.id})"
+                    )
+                    raise BlackoutPeriod("Suppressed alert during blackout period")
                 log.debug(
                     "Alert %s seems to match (regex) blackout %s. "
                     "Adding regex_blackout and status",
                     alert.id,
                     blackout.id,
                 )
                 alert.tags.extend(["regex_blackout={}".format(blackout.id)])
```

### Comparing `alerta-blackout-regex-3.0.0/setup.py` & `alerta-blackout-regex-3.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __author__ = "Mircea Ulinic <ping@mirceaulinic.net>"
 
 with codecs.open("README.rst", "r", encoding="utf8") as file:
     long_description = file.read()
 
 setup(
     name="alerta-blackout-regex",
-    version="3.0.0",
+    version="3.1.0",
     author="Mircea Ulinic",
     author_email="ping@mirceaulinic.net",
     py_modules=["blackout_regex"],
     description="Alerta Blackout enhancement plugin",
     long_description=long_description,
     include_package_data=True,
     zip_safe=True,
```

