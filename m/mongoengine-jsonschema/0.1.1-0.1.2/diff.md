# Comparing `tmp/mongoengine-jsonschema-0.1.1.tar.gz` & `tmp/mongoengine-jsonschema-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoengine-jsonschema-0.1.1.tar", last modified: Sun Jun 11 08:40:41 2023, max compression
+gzip compressed data, was "mongoengine-jsonschema-0.1.2.tar", last modified: Tue Jul 18 18:15:09 2023, max compression
```

## Comparing `mongoengine-jsonschema-0.1.1.tar` & `mongoengine-jsonschema-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     1069 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/LICENSE
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       42 2023-06-11 08:37:25.000000 mongoengine-jsonschema-0.1.1/MANIFEST.in
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     5383 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/PKG-INFO
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     4386 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/README.md
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        5 2023-06-11 08:40:29.000000 mongoengine-jsonschema-0.1.1/VERSION
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)      108 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/pyproject.toml
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       47 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/requirements.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       38 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/setup.cfg
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     2251 2023-06-11 08:40:29.000000 mongoengine-jsonschema-0.1.1/setup.py
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/src/
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       35 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/__init__.py
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)    12892 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/mixin.py
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)     5383 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/PKG-INFO
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)      477 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/SOURCES.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        1 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/dependency_links.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)        1 2023-06-11 08:40:34.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/not-zip-safe
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       48 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/requires.txt
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)       23 2023-06-11 08:40:41.000000 mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/top_level.txt
-drwxr-xr-x   0 symphonicity  (1000) symphonicity  (1000)        0 2023-06-11 08:40:41.375231 mongoengine-jsonschema-0.1.1/tests/
--rw-r--r--   0 symphonicity  (1000) symphonicity  (1000)    31337 2023-06-11 07:44:43.000000 mongoengine-jsonschema-0.1.1/tests/test_json_schema.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     1069 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/LICENSE
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       42 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/MANIFEST.in
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     5545 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/PKG-INFO
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     4548 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/README.md
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        6 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/VERSION
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      108 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/pyproject.toml
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       47 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/requirements.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       38 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/setup.cfg
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     2251 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/setup.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/src/
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       35 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/__init__.py
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)    13133 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/mixin.py
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)     5545 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/PKG-INFO
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)      477 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)        1 2023-07-18 18:14:58.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/not-zip-safe
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       48 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/requires.txt
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)       23 2023-07-18 18:15:09.000000 mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/top_level.txt
+drwxrwxr-x   0 yossi     (1000) yossi     (1000)        0 2023-07-18 18:15:09.413392 mongoengine-jsonschema-0.1.2/tests/
+-rw-rw-r--   0 yossi     (1000) yossi     (1000)    31999 2023-07-18 18:14:09.000000 mongoengine-jsonschema-0.1.2/tests/test_json_schema.py
```

### Comparing `mongoengine-jsonschema-0.1.1/LICENSE` & `mongoengine-jsonschema-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.1/PKG-INFO` & `mongoengine-jsonschema-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoengine-jsonschema
-Version: 0.1.1
+Version: 0.1.2
 Summary: MongoEngine JSON Schema Generator
 Home-page: https://github.com/symphonicityy/mongoengine-jsonschema
 Author: Yusuf Eroglu
 Author-email: myusuferoglu@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/README.md
 Project-URL: Code, https://github.com/symphonicityy/mongoengine-jsonschema
@@ -85,31 +85,32 @@
 
 ### Example
 Check out [example.md](https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/example.md) for a more extensive example.
 
 ### Features
 - Inheritance is supported. Make sure you add mixin to parent class.
 - `additionalProperties` is set to `False` for `DynamicDocument` and `DynamicEmbeddedDocument` classes.
-- `required` keyword can be removed by setting `strict` argument to `False` (`.json_schema(strict=False)`). This is useful for partial validation, e.g. when updating documents using HTTP PATCH method.
+- `required` keyword can be removed by setting `strict` argument to `False` (`.json_schema(strict=False)`). This is useful for partial validation when updating documents using HTTP PATCH method.
 - Constraints for special `StringField` types such as `EmailField`, `URLField`, `UUIDField`, `DateTimeField` etc. are applied to schema using `format` and/or `pattern` keywords.
 - Fields derived from `GeoJsonBaseField` can be validated for both array and object types as supported by MongoEngine.
 - Field arguments/constraints `required`, `min_length`, `max_length`, `min_value`, `max_value`, `default`, `choices`, `regex` and `url_regex` (for `URLField`) are supported and reflected to schema.
 - Excluding a field from schema is possible with setting field argument `exclude_from_schema` to `True`. Example: 
     ```python 
     name = me.StringField(exclude_from_schema=True)
     ```
 - Auto-generates human-friendly (first-letter capitalized, separate words) `title` from both document (PascalCase) and field names (snake_case). Keeps uppercase acronyms as is, e.g. `page_URL` -> `Page URL`.
-- For `ListField` types, `required=True` means it cannot be empty, therefore schema defines this constraint with `minItems` keyword.
+- For `ListField` types, `required=True` means it cannot be empty, therefore, schema defines this constraint with `minItems` keyword.
+- Custom schemas can be defined directly in model class with `_JSONSCHEMA` class attribute. Setting a `_JSONSCHEMA` attribute will bypass JSON schema generation.
 
 ### Limitations
 - `FileField`, `ImageField` fields are not supported
-- `PolygonField` and `MultiPoligonField` must start and end at the same point but this is not enforced by generated schema
+- `PolygonField` and `MultiPolygonField` must start and end at the same point, but this is not enforced by generated schema
 - `schemes` argument is ignored for `URLField`
 - `domain_whitelist`, `allow_utf8_user`, `allow_ip_domain` arguments are ignored for `EmailField`
-- Following fields are defined in schema as strings and may require field specific conversion before assigning to a document's attribute:
+- The following fields are defined in schema as strings and may require field specific conversion before assigning to a document's attribute:
     - `ObjectIdField`
     - `BinaryField`
     - `DateTimeField`
     - `ComplexDateTimeField`
     - `DateField`
     - `ReferenceField`
     - `LazyReferenceField`
```

### Comparing `mongoengine-jsonschema-0.1.1/README.md` & `mongoengine-jsonschema-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -60,31 +60,32 @@
 
 ### Example
 Check out [example.md](https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/example.md) for a more extensive example.
 
 ### Features
 - Inheritance is supported. Make sure you add mixin to parent class.
 - `additionalProperties` is set to `False` for `DynamicDocument` and `DynamicEmbeddedDocument` classes.
-- `required` keyword can be removed by setting `strict` argument to `False` (`.json_schema(strict=False)`). This is useful for partial validation, e.g. when updating documents using HTTP PATCH method.
+- `required` keyword can be removed by setting `strict` argument to `False` (`.json_schema(strict=False)`). This is useful for partial validation when updating documents using HTTP PATCH method.
 - Constraints for special `StringField` types such as `EmailField`, `URLField`, `UUIDField`, `DateTimeField` etc. are applied to schema using `format` and/or `pattern` keywords.
 - Fields derived from `GeoJsonBaseField` can be validated for both array and object types as supported by MongoEngine.
 - Field arguments/constraints `required`, `min_length`, `max_length`, `min_value`, `max_value`, `default`, `choices`, `regex` and `url_regex` (for `URLField`) are supported and reflected to schema.
 - Excluding a field from schema is possible with setting field argument `exclude_from_schema` to `True`. Example: 
     ```python 
     name = me.StringField(exclude_from_schema=True)
     ```
 - Auto-generates human-friendly (first-letter capitalized, separate words) `title` from both document (PascalCase) and field names (snake_case). Keeps uppercase acronyms as is, e.g. `page_URL` -> `Page URL`.
-- For `ListField` types, `required=True` means it cannot be empty, therefore schema defines this constraint with `minItems` keyword.
+- For `ListField` types, `required=True` means it cannot be empty, therefore, schema defines this constraint with `minItems` keyword.
+- Custom schemas can be defined directly in model class with `_JSONSCHEMA` class attribute. Setting a `_JSONSCHEMA` attribute will bypass JSON schema generation.
 
 ### Limitations
 - `FileField`, `ImageField` fields are not supported
-- `PolygonField` and `MultiPoligonField` must start and end at the same point but this is not enforced by generated schema
+- `PolygonField` and `MultiPolygonField` must start and end at the same point, but this is not enforced by generated schema
 - `schemes` argument is ignored for `URLField`
 - `domain_whitelist`, `allow_utf8_user`, `allow_ip_domain` arguments are ignored for `EmailField`
-- Following fields are defined in schema as strings and may require field specific conversion before assigning to a document's attribute:
+- The following fields are defined in schema as strings and may require field specific conversion before assigning to a document's attribute:
     - `ObjectIdField`
     - `BinaryField`
     - `DateTimeField`
     - `ComplexDateTimeField`
     - `DateField`
     - `ReferenceField`
     - `LazyReferenceField`
```

### Comparing `mongoengine-jsonschema-0.1.1/setup.py` & `mongoengine-jsonschema-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema/mixin.py` & `mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema/mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,14 +350,23 @@
                           validating JSONs when updating documents using HTTP PATCH method.
 
         Returns:
             dict
         """
 
         cls._STRICT = strict
+
+        try:
+            schema = getattr(cls, '_JSONSCHEMA')
+            if not cls._STRICT and 'required' in schema.keys():
+                del schema['required']
+            return schema
+        except AttributeError:
+            pass
+
         model_properties = cls._parse()
         required_list = []
         for k, v in model_properties.items():
             req = v.get('required', False)
             if type(req) is bool:
                 if req:
                     required_list.append(k)
```

### Comparing `mongoengine-jsonschema-0.1.1/src/mongoengine_jsonschema.egg-info/PKG-INFO` & `mongoengine-jsonschema-0.1.2/src/mongoengine_jsonschema.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoengine-jsonschema
-Version: 0.1.1
+Version: 0.1.2
 Summary: MongoEngine JSON Schema Generator
 Home-page: https://github.com/symphonicityy/mongoengine-jsonschema
 Author: Yusuf Eroglu
 Author-email: myusuferoglu@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/README.md
 Project-URL: Code, https://github.com/symphonicityy/mongoengine-jsonschema
@@ -85,31 +85,32 @@
 
 ### Example
 Check out [example.md](https://github.com/symphonicityy/mongoengine-jsonschema/blob/main/example.md) for a more extensive example.
 
 ### Features
 - Inheritance is supported. Make sure you add mixin to parent class.
 - `additionalProperties` is set to `False` for `DynamicDocument` and `DynamicEmbeddedDocument` classes.
-- `required` keyword can be removed by setting `strict` argument to `False` (`.json_schema(strict=False)`). This is useful for partial validation, e.g. when updating documents using HTTP PATCH method.
+- `required` keyword can be removed by setting `strict` argument to `False` (`.json_schema(strict=False)`). This is useful for partial validation when updating documents using HTTP PATCH method.
 - Constraints for special `StringField` types such as `EmailField`, `URLField`, `UUIDField`, `DateTimeField` etc. are applied to schema using `format` and/or `pattern` keywords.
 - Fields derived from `GeoJsonBaseField` can be validated for both array and object types as supported by MongoEngine.
 - Field arguments/constraints `required`, `min_length`, `max_length`, `min_value`, `max_value`, `default`, `choices`, `regex` and `url_regex` (for `URLField`) are supported and reflected to schema.
 - Excluding a field from schema is possible with setting field argument `exclude_from_schema` to `True`. Example: 
     ```python 
     name = me.StringField(exclude_from_schema=True)
     ```
 - Auto-generates human-friendly (first-letter capitalized, separate words) `title` from both document (PascalCase) and field names (snake_case). Keeps uppercase acronyms as is, e.g. `page_URL` -> `Page URL`.
-- For `ListField` types, `required=True` means it cannot be empty, therefore schema defines this constraint with `minItems` keyword.
+- For `ListField` types, `required=True` means it cannot be empty, therefore, schema defines this constraint with `minItems` keyword.
+- Custom schemas can be defined directly in model class with `_JSONSCHEMA` class attribute. Setting a `_JSONSCHEMA` attribute will bypass JSON schema generation.
 
 ### Limitations
 - `FileField`, `ImageField` fields are not supported
-- `PolygonField` and `MultiPoligonField` must start and end at the same point but this is not enforced by generated schema
+- `PolygonField` and `MultiPolygonField` must start and end at the same point, but this is not enforced by generated schema
 - `schemes` argument is ignored for `URLField`
 - `domain_whitelist`, `allow_utf8_user`, `allow_ip_domain` arguments are ignored for `EmailField`
-- Following fields are defined in schema as strings and may require field specific conversion before assigning to a document's attribute:
+- The following fields are defined in schema as strings and may require field specific conversion before assigning to a document's attribute:
     - `ObjectIdField`
     - `BinaryField`
     - `DateTimeField`
     - `ComplexDateTimeField`
     - `DateField`
     - `ReferenceField`
     - `LazyReferenceField`
```

### Comparing `mongoengine-jsonschema-0.1.1/tests/test_json_schema.py` & `mongoengine-jsonschema-0.1.2/tests/test_json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,24 @@
     field = me.StringField()
 
 
 class ExampleDocumentInheritedNoMixinParent(ExampleBaseNoMixinDocument, JsonSchemaMixin):
     field = me.StringField()
 
 
+class ExampleDocumentWithCustomSchema(me.Document, JsonSchemaMixin):
+    _JSONSCHEMA = {
+        '$id': '/schemas/ExampleDocumentWithCustomSchema',
+        'type': 'object',
+        'title': 'Example Document With Custom Schema',
+        'properties': {},
+        'additionalProperties': False
+    }
+
+
 class ExampleDocument(me.Document, JsonSchemaMixin):
     binary_field = me.BinaryField()
     boolean_field = me.BooleanField(required=True)
     cached_reference_field = me.CachedReferenceField(ExampleReferencedDocument)
     complex_datetime_field = me.ComplexDateTimeField()
     datetime_field = me.DateTimeField()
     date_field = me.DateField()
@@ -171,14 +181,24 @@
         assert 'required' in schema.keys()
         assert schema['required'] == ['boolean_field']
 
     def test_not_strict(self):
         schema = ExampleDocument.json_schema(strict=False)
         assert 'required' not in schema.keys()
 
+    def test_custom_schema(self):
+        schema = ExampleDocumentWithCustomSchema.json_schema()
+        assert schema == {
+            '$id': '/schemas/ExampleDocumentWithCustomSchema',
+            'type': 'object',
+            'title': 'Example Document With Custom Schema',
+            'properties': {},
+            'additionalProperties': False
+        }
+
 
 class TestDocumentSchemaProps:
     def test_binary_field(self, example_schema):
         assert example_schema['properties']['binary_field']['type'] == 'string'
 
     def test_cached_reference_field(self, example_schema):
         assert example_schema['properties']['cached_reference_field']['type'] == 'string'
```

