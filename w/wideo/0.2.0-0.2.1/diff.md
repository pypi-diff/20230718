# Comparing `tmp/wideo-0.2.0.tar.gz` & `tmp/wideo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wideo-0.2.0.tar", max compression
+gzip compressed data, was "wideo-0.2.1.tar", max compression
```

## Comparing `wideo-0.2.0.tar` & `wideo-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      674 2023-07-10 13:18:51.111670 wideo-0.2.0/README.md
--rw-r--r--   0        0        0      469 2023-07-10 13:18:51.115670 wideo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1584 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/__init__.py
--rw-r--r--   0        0        0      767 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/admin_urls.py
--rw-r--r--   0        0        0      174 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/apps.py
--rw-r--r--   0        0        0      376 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/blocks.py
--rw-r--r--   0        0        0     2494 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/codecs.py
--rw-r--r--   0        0        0       92 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/exceptions.py
--rw-r--r--   0        0        0     7167 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/ffmpeg.py
--rw-r--r--   0        0        0      329 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/fields.py
--rw-r--r--   0        0        0      334 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/forms.py
--rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/commands/__init__.py
--rw-r--r--   0        0        0      321 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/commands/delete_orphan_uploaded_videos.py
--rw-r--r--   0        0        0      557 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/commands/encode_videos.py
--rw-r--r--   0        0        0     9737 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/0001_initial.py
--rw-r--r--   0        0        0      676 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/0002_lock.py
--rw-r--r--   0        0        0     2955 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/0003_uploadedvideochunk.py
--rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/__init__.py
--rw-r--r--   0        0        0     6373 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/models.py
--rw-r--r--   0        0        0      777 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/permissions.py
--rw-r--r--   0        0        0     1544 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/signals.py
--rw-r--r--   0        0        0     1301 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/storage.py
--rw-r--r--   0        0        0      636 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/tasks.py
--rw-r--r--   0        0        0      179 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/blocks/video.html
--rw-r--r--   0        0        0     3771 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/forms/file.html
--rw-r--r--   0        0        0      190 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/forms/file_edit.html
--rw-r--r--   0        0        0      179 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/icons/video.svg
--rw-r--r--   0        0        0      457 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/preview/plyr_styles.html
--rw-r--r--   0        0        0     1757 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/preview/video_source.html
--rw-r--r--   0        0        0      124 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/video.html
--rw-r--r--   0        0        0     3303 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/add.html
--rw-r--r--   0        0        0     1621 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/confirm_delete.html
--rw-r--r--   0        0        0     2690 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/edit.html
--rw-r--r--   0        0        0     4455 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/index.html
--rw-r--r--   0        0        0     2586 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/results.html
--rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/results_video.html
--rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templatetags/__init__.py
--rw-r--r--   0        0        0      231 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templatetags/settings.py
--rw-r--r--   0        0        0    14570 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/views.py
--rw-r--r--   0        0        0      612 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/wagtail_hooks.py
--rw-r--r--   0        0        0      126 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/widgets.py
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 wideo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      674 2023-07-18 16:14:31.846315 wideo-0.2.1/README.md
+-rw-r--r--   0        0        0      469 2023-07-18 16:14:31.854315 wideo-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1584 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/__init__.py
+-rw-r--r--   0        0        0      767 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/admin_urls.py
+-rw-r--r--   0        0        0      174 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/apps.py
+-rw-r--r--   0        0        0      376 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/blocks.py
+-rw-r--r--   0        0        0     2494 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/codecs.py
+-rw-r--r--   0        0        0       92 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/exceptions.py
+-rw-r--r--   0        0        0     7167 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/ffmpeg.py
+-rw-r--r--   0        0        0      329 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/fields.py
+-rw-r--r--   0        0        0      334 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/forms.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/management/commands/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/management/commands/delete_orphan_uploaded_videos.py
+-rw-r--r--   0        0        0      557 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/management/commands/encode_videos.py
+-rw-r--r--   0        0        0     9737 2023-07-18 16:14:31.854315 wideo-0.2.1/src/wideo/migrations/0001_initial.py
+-rw-r--r--   0        0        0      676 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/migrations/0002_lock.py
+-rw-r--r--   0        0        0     2955 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/migrations/0003_uploadedvideochunk.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/migrations/__init__.py
+-rw-r--r--   0        0        0     6373 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/models.py
+-rw-r--r--   0        0        0      777 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/permissions.py
+-rw-r--r--   0        0        0     1544 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/signals.py
+-rw-r--r--   0        0        0     1301 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/storage.py
+-rw-r--r--   0        0        0      636 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/tasks.py
+-rw-r--r--   0        0        0      179 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/blocks/video.html
+-rw-r--r--   0        0        0     4210 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/forms/file.html
+-rw-r--r--   0        0        0      190 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/forms/file_edit.html
+-rw-r--r--   0        0        0      179 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/icons/video.svg
+-rw-r--r--   0        0        0      457 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/preview/plyr_styles.html
+-rw-r--r--   0        0        0     1757 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/preview/video_source.html
+-rw-r--r--   0        0        0      124 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/video.html
+-rw-r--r--   0        0        0     3303 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/videos/add.html
+-rw-r--r--   0        0        0     1621 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/videos/confirm_delete.html
+-rw-r--r--   0        0        0     2690 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/videos/edit.html
+-rw-r--r--   0        0        0     4455 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/videos/index.html
+-rw-r--r--   0        0        0     2586 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/videos/results.html
+-rw-r--r--   0        0        0        0 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templates/wideo/videos/results_video.html
+-rw-r--r--   0        0        0        0 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templatetags/__init__.py
+-rw-r--r--   0        0        0      231 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/templatetags/settings.py
+-rw-r--r--   0        0        0    14570 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/views.py
+-rw-r--r--   0        0        0      612 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/wagtail_hooks.py
+-rw-r--r--   0        0        0      126 2023-07-18 16:14:31.858315 wideo-0.2.1/src/wideo/widgets.py
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 wideo-0.2.1/PKG-INFO
```

### Comparing `wideo-0.2.0/README.md` & `wideo-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/__init__.py` & `wideo-0.2.1/src/wideo/__init__.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/admin_urls.py` & `wideo-0.2.1/src/wideo/admin_urls.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/codecs.py` & `wideo-0.2.1/src/wideo/codecs.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/ffmpeg.py` & `wideo-0.2.1/src/wideo/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/management/commands/encode_videos.py` & `wideo-0.2.1/src/wideo/management/commands/encode_videos.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/migrations/0001_initial.py` & `wideo-0.2.1/src/wideo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/migrations/0002_lock.py` & `wideo-0.2.1/src/wideo/migrations/0002_lock.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/migrations/0003_uploadedvideochunk.py` & `wideo-0.2.1/src/wideo/migrations/0003_uploadedvideochunk.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/models.py` & `wideo-0.2.1/src/wideo/models.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/permissions.py` & `wideo-0.2.1/src/wideo/permissions.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/signals.py` & `wideo-0.2.1/src/wideo/signals.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/storage.py` & `wideo-0.2.1/src/wideo/storage.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/tasks.py` & `wideo-0.2.1/src/wideo/tasks.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/templates/wideo/forms/file.html` & `wideo-0.2.1/src/wideo/templates/wideo/forms/file.html`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,31 @@
 {% load i18n %}
 {% load settings %}
 {% block form_field %}
     <input type="hidden" name="{{ widget.name }}" required>
 
     <script>
         function getCookie(name) {
-            const cookie = document.cookie.split(";")
-                .map(cookie => cookie.split("="))
-                .find(cookie => cookie[0] === name);
+            let cookieValue = null;
 
-            return cookie ? cookie[1] : "";
+            if (document.cookie && document.cookie !== "") {
+                const cookies = document.cookie.split(";");
+
+                for (let i = 0; i < cookies.length; i++) {
+                    const cookie = cookies[i].trim();
+
+                    // Does this cookie string begin with the name we want?
+                    if (cookie.substring(0, name.length + 1) === (name + "=")) {
+                        cookieValue = decodeURIComponent(cookie.substring(name.length + 1));
+                        break;
+                    }
+                }
+            }
+
+            return cookieValue;
         }
 
         function setSubmitDisabled(disabled) {
             for (const button of document.getElementsByTagName("input")) {
                 if (button.type === "submit") {
                     button.disabled = disabled;
                 }
```

### Comparing `wideo-0.2.0/src/wideo/templates/wideo/preview/video_source.html` & `wideo-0.2.1/src/wideo/templates/wideo/preview/video_source.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/templates/wideo/videos/add.html` & `wideo-0.2.1/src/wideo/templates/wideo/videos/add.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/templates/wideo/videos/confirm_delete.html` & `wideo-0.2.1/src/wideo/templates/wideo/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/templates/wideo/videos/edit.html` & `wideo-0.2.1/src/wideo/templates/wideo/videos/edit.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/templates/wideo/videos/index.html` & `wideo-0.2.1/src/wideo/templates/wideo/videos/index.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/templates/wideo/videos/results.html` & `wideo-0.2.1/src/wideo/templates/wideo/videos/results.html`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/views.py` & `wideo-0.2.1/src/wideo/views.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/src/wideo/wagtail_hooks.py` & `wideo-0.2.1/src/wideo/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wideo-0.2.0/PKG-INFO` & `wideo-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wideo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Add video goodness to your Wagtail website
 License: WTFPL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

