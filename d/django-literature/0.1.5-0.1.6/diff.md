# Comparing `tmp/django_literature-0.1.5.tar.gz` & `tmp/django_literature-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_literature-0.1.5.tar", max compression
+gzip compressed data, was "django_literature-0.1.6.tar", max compression
```

## Comparing `django_literature-0.1.5.tar` & `django_literature-0.1.6.tar`

### file list

```diff
@@ -1,57 +1,55 @@
--rw-r--r--   0        0        0     1089 2023-05-05 10:10:02.273202 django_literature-0.1.5/LICENSE
--rw-r--r--   0        0        0     2343 2023-05-05 10:10:02.273202 django_literature-0.1.5/README.md
--rw-r--r--   0        0        0       22 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/__init__.py
--rw-r--r--   0        0        0     6237 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/admin.py
--rw-r--r--   0        0        0        0 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/api/__init__.py
--rw-r--r--   0        0        0      398 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/api/serialize.py
--rw-r--r--   0        0        0      249 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/api/urls.py
--rw-r--r--   0        0        0      370 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/api/views.py
--rw-r--r--   0        0        0      250 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/apps.py
--rw-r--r--   0        0        0     2514 2023-05-05 10:10:02.273202 django_literature-0.1.5/literature/choices.py
--rw-r--r--   0        0        0      724 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/conf.py
--rw-r--r--   0        0        0    36128 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/csl_map.py
--rw-r--r--   0        0        0      985 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/drf.py
--rw-r--r--   0        0        0      761 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/fields.py
--rw-r--r--   0        0        0     4965 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/forms.py
--rw-r--r--   0        0        0     2576 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/formset.py
--rw-r--r--   0        0        0     1932 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/managers.py
--rw-r--r--   0        0        0    13989 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/migrations/0001_initial.py
--rw-r--r--   0        0        0      655 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/migrations/0002_alter_literature_published.py
--rw-r--r--   0        0        0      478 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/migrations/0003_literature_csl.py
--rw-r--r--   0        0        0     2871 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py
--rw-r--r--   0        0        0      577 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py
--rw-r--r--   0        0        0        0 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/migrations/__init__.py
--rw-r--r--   0        0        0     8578 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/models.py
--rw-r--r--   0        0        0     4667 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/static/literature/icons/icons.svg
--rw-r--r--   0        0        0     1513 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/static/literature/icons/three-dots.svg
--rw-r--r--   0        0        0     3106 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/static/literature/js/admin/change_list.js
--rw-r--r--   0        0        0     3111 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/static/literature/js/datatablesHyperlink.js
--rw-r--r--   0        0        0     1715 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/static/literature/js/main copy.js
--rw-r--r--   0        0        0     2012 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/static/literature/js/main.js
--rw-r--r--   0        0        0    74730 2023-05-05 10:10:02.277202 django_literature-0.1.5/literature/static/vendor/DataTables/datatables.min.css
--rw-r--r--   0        0        0  2452970 2023-05-05 10:10:02.297204 django_literature-0.1.5/literature/static/vendor/DataTables/datatables.min.js
--rw-r--r--   0        0        0  2274000 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/static/vendor/js/citation.js
--rw-r--r--   0        0        0     6071 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/base.html
--rw-r--r--   0        0        0     2370 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/admin/change_list.html
--rw-r--r--   0        0        0     2085 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/admin/search.html
--rw-r--r--   0        0        0      615 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/author_detail.html
--rw-r--r--   0        0        0     1349 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/author_list.html
--rw-r--r--   0        0        0       73 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/bibliography.html
--rw-r--r--   0        0        0      665 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/citation/bootstrap.html
--rw-r--r--   0        0        0      465 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/citation/plain_text.html
--rw-r--r--   0        0        0      332 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/literature_detail.html
--rw-r--r--   0        0        0     1591 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/literature_form.html
--rw-r--r--   0        0        0      788 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/literature_form1.html
--rw-r--r--   0        0        0      186 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/literature_list.html
--rw-r--r--   0        0        0      301 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/widgets/identifier.html
--rw-r--r--   0        0        0     1128 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/widgets/pdf_viewer.html
--rw-r--r--   0        0        0     1120 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/widgets/postgres_array_widget.html
--rw-r--r--   0        0        0      348 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templates/literature/widgets/preview.html
--rw-r--r--   0        0        0        0 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templatetags/__init__.py
--rw-r--r--   0        0        0      568 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/templatetags/literature.py
--rw-r--r--   0        0        0      429 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/urls.py
--rw-r--r--   0        0        0     1241 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/utils.py
--rw-r--r--   0        0        0     3040 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/views.py
--rw-r--r--   0        0        0      828 2023-05-05 10:10:02.309205 django_literature-0.1.5/literature/widgets.py
--rw-r--r--   0        0        0     3948 2023-05-05 10:10:34.960198 django_literature-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 django_literature-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-18 18:09:47.100732 django_literature-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3150 2023-07-18 18:09:47.100732 django_literature-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/__init__.py
+-rw-r--r--   0        0        0     6267 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/admin.py
+-rw-r--r--   0        0        0        0 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/api/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/api/serialize.py
+-rw-r--r--   0        0        0      370 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/api/views.py
+-rw-r--r--   0        0        0      250 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/apps.py
+-rw-r--r--   0        0        0     2514 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/choices.py
+-rw-r--r--   0        0        0      724 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/conf.py
+-rw-r--r--   0        0        0    36128 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/csl_map.py
+-rw-r--r--   0        0        0      998 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/drf.py
+-rw-r--r--   0        0        0      761 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/fields.py
+-rw-r--r--   0        0        0     4948 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/forms.py
+-rw-r--r--   0        0        0     2576 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/formset.py
+-rw-r--r--   0        0        0     1932 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/managers.py
+-rw-r--r--   0        0        0        0 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/migrations/__init__.py
+-rw-r--r--   0        0        0     8578 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/models.py
+-rw-r--r--   0        0        0     4667 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/static/literature/icons/icons.svg
+-rw-r--r--   0        0        0     1513 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/static/literature/icons/three-dots.svg
+-rw-r--r--   0        0        0     3106 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/static/literature/js/admin/change_list.js
+-rw-r--r--   0        0        0     3111 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/static/literature/js/datatablesHyperlink.js
+-rw-r--r--   0        0        0     1715 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/static/literature/js/main copy.js
+-rw-r--r--   0        0        0     2012 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/static/literature/js/main.js
+-rw-r--r--   0        0        0    61850 2023-07-18 18:09:47.104733 django_literature-0.1.6/literature/static/vendor/DataTables/bootstrap4/datatables.min.css
+-rw-r--r--   0        0        0  2683944 2023-07-18 18:09:47.120733 django_literature-0.1.6/literature/static/vendor/DataTables/bootstrap4/datatables.min.js
+-rw-r--r--   0        0        0    63567 2023-07-18 18:09:47.120733 django_literature-0.1.6/literature/static/vendor/DataTables/bootstrap5/datatables.min.css
+-rw-r--r--   0        0        0  2684319 2023-07-18 18:09:47.124733 django_literature-0.1.6/literature/static/vendor/DataTables/bootstrap5/datatables.min.js
+-rw-r--r--   0        0        0    74730 2023-07-18 18:09:47.124733 django_literature-0.1.6/literature/static/vendor/DataTables/datatables/datatables.min.css
+-rw-r--r--   0        0        0  2452970 2023-07-18 18:09:47.140733 django_literature-0.1.6/literature/static/vendor/DataTables/datatables/datatables.min.js
+-rw-r--r--   0        0        0  2274000 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/static/vendor/js/citation.js
+-rw-r--r--   0        0        0     6071 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/base.html
+-rw-r--r--   0        0        0     2370 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/admin/change_list.html
+-rw-r--r--   0        0        0     2085 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/admin/search.html
+-rw-r--r--   0        0        0      615 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/author_detail.html
+-rw-r--r--   0        0        0     1349 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/author_list.html
+-rw-r--r--   0        0        0       73 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/bibliography.html
+-rw-r--r--   0        0        0      665 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/citation/bootstrap.html
+-rw-r--r--   0        0        0      465 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/citation/plain_text.html
+-rw-r--r--   0        0        0      332 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/literature_detail.html
+-rw-r--r--   0        0        0     1591 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/literature_form.html
+-rw-r--r--   0        0        0      788 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/literature_form1.html
+-rw-r--r--   0        0        0      186 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/literature_list.html
+-rw-r--r--   0        0        0      301 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/widgets/identifier.html
+-rw-r--r--   0        0        0     1128 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/widgets/pdf_viewer.html
+-rw-r--r--   0        0        0     1120 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/widgets/postgres_array_widget.html
+-rw-r--r--   0        0        0      348 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templates/literature/widgets/preview.html
+-rw-r--r--   0        0        0        0 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templatetags/__init__.py
+-rw-r--r--   0        0        0      568 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/templatetags/literature.py
+-rw-r--r--   0        0        0      429 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/urls.py
+-rw-r--r--   0        0        0     1241 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/utils.py
+-rw-r--r--   0        0        0     3040 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/views.py
+-rw-r--r--   0        0        0      828 2023-07-18 18:09:47.148733 django_literature-0.1.6/literature/widgets.py
+-rw-r--r--   0        0        0     3948 2023-07-18 18:10:19.701145 django_literature-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4483 1970-01-01 00:00:00.000000 django_literature-0.1.6/PKG-INFO
```

### Comparing `django_literature-0.1.5/LICENSE` & `django_literature-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/admin.py` & `django_literature-0.1.6/literature/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         #         ]
         #     },
         # ),
     ]
 
     endpoint = {
         "fields": "__all__",
+        "include_str": False,
         "page_size": 1000,
         "permission_classes": [IsAdminUser, DjangoModelPermissions],
     }
 
     def get_dt_fields(self):
         new_dict = {}
         for field, value in sorted(csl_fields.items()):
```

### Comparing `django_literature-0.1.5/literature/choices.py` & `django_literature-0.1.6/literature/choices.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/conf.py` & `django_literature-0.1.6/literature/conf.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/csl_map.py` & `django_literature-0.1.6/literature/csl_map.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/drf.py` & `django_literature-0.1.6/literature/drf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
     def changelist_view(self, request, extra_context=None):
         extra_context = extra_context or {}
         extra_context["datatables_fields"] = self.get_dt_fields()
         return super().changelist_view(request, extra_context=extra_context)
 
     def register_endpoint(self):
-        return router.register(endpoint=Endpoint(model=self.model, **self.endpoint))
+        return router.register(endpoint=Endpoint(model=self.model, **self.endpoint), url="admin")
 
     def get_dt_fields(self):
         return []
```

### Comparing `django_literature-0.1.5/literature/fields.py` & `django_literature-0.1.6/literature/fields.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/forms.py` & `django_literature-0.1.6/literature/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from django import forms
 from django.forms.models import ModelForm, construct_instance, model_to_dict
 from django.utils.translation import gettext as _
 from formset.collection import FormCollection
 from formset.fieldset import FieldsetMixin
 from formset.renderers import bootstrap
 from formset.richtext.widgets import RichTextarea
-from formset.widgets import (
-    DateInput,
-    DualSortableSelector,
-    UploadedFileInput,
-)
+from formset.widgets import DateInput, DualSortableSelector, UploadedFileInput
 
 from .models import Literature, SupplementaryMaterial
 from .widgets import OnlineSearchWidget, PreviewWidget
 
 
 class CitationJSFormMixin(forms.Form):
     """A mixin that adds a hidden text field for the CSL JSON data and a preview field
```

### Comparing `django_literature-0.1.5/literature/formset.py` & `django_literature-0.1.6/literature/formset.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/managers.py` & `django_literature-0.1.6/literature/managers.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/models.py` & `django_literature-0.1.6/literature/models.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/literature/icons/icons.svg` & `django_literature-0.1.6/literature/static/literature/icons/icons.svg`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/literature/icons/three-dots.svg` & `django_literature-0.1.6/literature/static/literature/icons/three-dots.svg`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/literature/js/admin/change_list.js` & `django_literature-0.1.6/literature/static/literature/js/admin/change_list.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/literature/js/datatablesHyperlink.js` & `django_literature-0.1.6/literature/static/literature/js/datatablesHyperlink.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/literature/js/main copy.js` & `django_literature-0.1.6/literature/static/literature/js/main copy.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/literature/js/main.js` & `django_literature-0.1.6/literature/static/literature/js/main.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/vendor/DataTables/datatables.min.css` & `django_literature-0.1.6/literature/static/vendor/DataTables/datatables/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/vendor/DataTables/datatables.min.js` & `django_literature-0.1.6/literature/static/vendor/DataTables/datatables/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/static/vendor/js/citation.js` & `django_literature-0.1.6/literature/static/vendor/js/citation.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/base.html` & `django_literature-0.1.6/literature/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/admin/change_list.html` & `django_literature-0.1.6/literature/templates/literature/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/admin/search.html` & `django_literature-0.1.6/literature/templates/literature/admin/search.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/author_detail.html` & `django_literature-0.1.6/literature/templates/literature/author_detail.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/author_list.html` & `django_literature-0.1.6/literature/templates/literature/author_list.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/citation/bootstrap.html` & `django_literature-0.1.6/literature/templates/literature/citation/bootstrap.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/literature_form.html` & `django_literature-0.1.6/literature/templates/literature/literature_form.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/literature_form1.html` & `django_literature-0.1.6/literature/templates/literature/literature_form1.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/widgets/pdf_viewer.html` & `django_literature-0.1.6/literature/templates/literature/widgets/pdf_viewer.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templates/literature/widgets/postgres_array_widget.html` & `django_literature-0.1.6/literature/templates/literature/widgets/postgres_array_widget.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/templatetags/literature.py` & `django_literature-0.1.6/literature/templatetags/literature.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/utils.py` & `django_literature-0.1.6/literature/utils.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/views.py` & `django_literature-0.1.6/literature/views.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/literature/widgets.py` & `django_literature-0.1.6/literature/widgets.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.5/pyproject.toml` & `django_literature-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-literature"
-version = "v0.1.5"
+version = "v0.1.6"
 description = "A scientific literature management tool for Django"
 authors = ["Sam Jennings <samuel.scott.jennings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "literature"}]
 homepage = "https://github.com/SSJenny90/django-literature"
 keywords = ["django", "literature", "publications", "scientific", "research"]
```

