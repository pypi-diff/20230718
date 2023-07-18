# Comparing `tmp/edc_test_utils-0.3.8-py3-none-any.whl.zip` & `tmp/edc_test_utils-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 22427 bytes, number of entries: 17
+Zip file size: 22501 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      161 b- defN 21-Jan-28 19:31 edc_test_utils/__init__.py
 -rw-r--r--  2.0 unx     1948 b- defN 21-Mar-01 04:08 edc_test_utils/default_installed_apps.py
--rw-r--r--  2.0 unx     9172 b- defN 21-Mar-29 22:21 edc_test_utils/default_test_settings.py
+-rw-r--r--  2.0 unx     9339 b- defN 21-Apr-23 01:09 edc_test_utils/default_test_settings.py
 -rw-r--r--  2.0 unx      511 b- defN 21-Feb-06 15:24 edc_test_utils/func_main.py
 -rw-r--r--  2.0 unx     3561 b- defN 21-Feb-06 15:24 edc_test_utils/natural_key_test_helper.py
 -rw-r--r--  2.0 unx     2998 b- defN 21-Feb-06 15:24 edc_test_utils/show_urls.py
 -rw-r--r--  2.0 unx     1015 b- defN 21-Feb-06 15:24 edc_test_utils/webtest.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-04 23:16 edc_test_utils/tests/__init__.py
 -rw-r--r--  2.0 unx      358 b- defN 20-Mar-15 01:41 edc_test_utils/tests/models.py
 -rw-r--r--  2.0 unx     1800 b- defN 21-Feb-06 15:24 edc_test_utils/tests/tests.py
 -rw-r--r--  2.0 unx      116 b- defN 21-Feb-06 15:24 edc_test_utils/tests/urls.py
--rw-r--r--  2.0 unx        0 b- defN 21-Mar-29 22:21 edc_test_utils-0.3.8.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx    35149 b- defN 21-Mar-29 22:21 edc_test_utils-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1606 b- defN 21-Mar-29 22:21 edc_test_utils-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Mar-29 22:21 edc_test_utils-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 21-Mar-29 22:21 edc_test_utils-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1482 b- defN 21-Mar-29 22:21 edc_test_utils-0.3.8.dist-info/RECORD
-17 files, 59984 bytes uncompressed, 19953 bytes compressed:  66.7%
+-rw-r--r--  2.0 unx        0 b- defN 21-Apr-23 01:10 edc_test_utils-0.3.9.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx    35149 b- defN 21-Apr-23 01:10 edc_test_utils-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1606 b- defN 21-Apr-23 01:10 edc_test_utils-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Apr-23 01:10 edc_test_utils-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 21-Apr-23 01:10 edc_test_utils-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1482 b- defN 21-Apr-23 01:10 edc_test_utils-0.3.9.dist-info/RECORD
+17 files, 60151 bytes uncompressed, 20027 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: edc_test_utils/tests/tests.py
 Comment: 
 
 Filename: edc_test_utils/tests/urls.py
 Comment: 
 
-Filename: edc_test_utils-0.3.8.dist-info/AUTHORS.rst
+Filename: edc_test_utils-0.3.9.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: edc_test_utils-0.3.8.dist-info/LICENSE
+Filename: edc_test_utils-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_test_utils-0.3.8.dist-info/METADATA
+Filename: edc_test_utils-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_test_utils-0.3.8.dist-info/WHEEL
+Filename: edc_test_utils-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_test_utils-0.3.8.dist-info/top_level.txt
+Filename: edc_test_utils-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_test_utils-0.3.8.dist-info/RECORD
+Filename: edc_test_utils-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edc_test_utils/default_test_settings.py

```diff
@@ -1,8 +1,9 @@
 import os
+import pdb
 import sys
 from uuid import uuid4
 
 import arrow
 from dateutil.relativedelta import relativedelta
 from django import VERSION
 
@@ -114,15 +115,14 @@
             if use_test_urls:
                 self.settings.update(ROOT_URLCONF=f"{self.app_name}.tests.urls")
             else:
                 self.settings.update(ROOT_URLCONF=f"{self.app_name}.urls")
 
     def _update_defaults(self):
         """Assumes BASE_DIR, APP_NAME are in kwargs."""
-
         self.settings.update(
             ALLOWED_HOSTS=["localhost"],
             # AUTH_USER_MODEL='custom_user.CustomUser',
             STATIC_URL="/static/",
             DATABASES={
                 # required for tests when acting as a server that deserializes
                 "default": {
@@ -158,19 +158,21 @@
                 "django.contrib.sites.middleware.CurrentSiteMiddleware",
             ],
             LANGUAGE_CODE="en-us",
             TIME_ZONE="UTC",
             USE_I18N=True,
             USE_L10N=True,
             USE_TZ=True,
+            DEFAULT_AUTO_FIELD="django.db.models.BigAutoField",
             EDC_BOOTSTRAP=3,
             GIT_DIR=self.base_dir,
             LIVE_SYSTEM=False,
             REVIEWER_SITE_ID=0,
             SITE_ID=SiteID(default=1) if SiteID else 1,
+            SILENCED_SYSTEM_CHECKS=["sites.E101"],  # The SITE_ID setting must be an integer
             SECRET_KEY=uuid4().hex,
             HOLIDAY_FILE=os.path.join(self.base_dir, self.app_name, "tests", "holidays.csv"),
             INDEX_PAGE_LABEL="",
             DASHBOARD_URL_NAMES={},
             DASHBOARD_BASE_TEMPLATES={},
             EMAIL_BACKEND="django.core.mail.backends.locmem.EmailBackend",
             EMAIL_CONTACTS={
```

## Comparing `edc_test_utils-0.3.8.dist-info/LICENSE` & `edc_test_utils-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_test_utils-0.3.8.dist-info/METADATA` & `edc_test_utils-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-test-utils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Class and functions for tests for clinicedc/edc projects
 Home-page: http://github.com/clinicedc/edc-test-model
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc tests
 Platform: UNKNOWN
```

## Comparing `edc_test_utils-0.3.8.dist-info/RECORD` & `edc_test_utils-0.3.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 edc_test_utils/__init__.py,sha256=bs5ODGmyiBRGN7eU7z6zAs2dNHqltinCkS-fRuI-ByM,161
 edc_test_utils/default_installed_apps.py,sha256=s6yrw1ZVx1-0dHAi1HwPhogfqX8xDBSBDjypYe1Sa10,1948
-edc_test_utils/default_test_settings.py,sha256=yFY4SPwmpVWCZH98Ci6fdUdIGxtc5sFZcOhW1Tyi2rI,9172
+edc_test_utils/default_test_settings.py,sha256=jEaboroJkZKH3AZII4Uq2g-ZtOeAxKgfNB3YEmzFh50,9339
 edc_test_utils/func_main.py,sha256=nFQWGOsK83eXIg8ncdgzwUne9QovuMcEinzUTpbslic,511
 edc_test_utils/natural_key_test_helper.py,sha256=8ptSS048_kVN8xljJIM6CN_lGmrDy5kKlnaROtgzWHM,3561
 edc_test_utils/show_urls.py,sha256=jI-Xmkx3gCJ8BuLhoxF8siYAHVEmvjCemZqGN-F2Ack,2998
 edc_test_utils/webtest.py,sha256=Jmud1fYbuRll2__llTVbVnq0yOtxnsqQWgdCu-NUKso,1015
 edc_test_utils/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_test_utils/tests/models.py,sha256=br0omxhWx_gn87Se2QSosZMmEb2CNliehov6H_050OY,358
 edc_test_utils/tests/tests.py,sha256=gzbwDEMO9Q4qfWzEq485WQQzha81avCzz3-5cMMUehU,1800
 edc_test_utils/tests/urls.py,sha256=CjGPtSGO4dflUXAQOEQXr5HdeyhFl9brQhgR-ONQ4cw,116
-edc_test_utils-0.3.8.dist-info/AUTHORS.rst,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-edc_test_utils-0.3.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-edc_test_utils-0.3.8.dist-info/METADATA,sha256=P-B3iQNAPgfnEKmQ5CD1aBUXsKM3fm-_HIHDnXQ2aAU,1606
-edc_test_utils-0.3.8.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-edc_test_utils-0.3.8.dist-info/top_level.txt,sha256=zs9BqZvOXZr6scQgntQLT5-YCfLOXGwvhWdpxzbmR2w,15
-edc_test_utils-0.3.8.dist-info/RECORD,,
+edc_test_utils-0.3.9.dist-info/AUTHORS.rst,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+edc_test_utils-0.3.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+edc_test_utils-0.3.9.dist-info/METADATA,sha256=v-pTHorxxtG17seih2SDwSxEmY0-zJsBVesSN_Kblxw,1606
+edc_test_utils-0.3.9.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+edc_test_utils-0.3.9.dist-info/top_level.txt,sha256=zs9BqZvOXZr6scQgntQLT5-YCfLOXGwvhWdpxzbmR2w,15
+edc_test_utils-0.3.9.dist-info/RECORD,,
```

