# Comparing `tmp/graphene-django-3.1.2.tar.gz` & `tmp/graphene-django-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-3.1.2.tar", last modified: Sat Jun 17 06:42:35 2023, max compression
+gzip compressed data, was "graphene-django-3.1.3.tar", last modified: Tue Jul 18 12:15:29 2023, max compression
```

## Comparing `graphene-django-3.1.2.tar` & `graphene-django-3.1.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-17 06:42:31.000000 graphene-django-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 06:42:31.000000 graphene-django-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-17 06:42:35.762130 graphene-django-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-17 06:42:31.000000 graphene-django-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-17 06:42:31.000000 graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-17 06:42:31.000000 graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/exception/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/exception/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/exception/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/sql/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/debug/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/debug/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/filter/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/array_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/global_id_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/list_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filters/typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/filterset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/filter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_contains_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_exact_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_overlap_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_enum_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_in_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/tests/test_typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/forms/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/forms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/test_djangoinputobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/forms/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/management/commands/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/serializer_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/rest_framework/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/test_field_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/rest_framework/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/graphene_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/static/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/static/graphene_django/graphiql.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.754130 graphene-django-3.1.2/graphene_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/templates/graphene/
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/templates/graphene/graphiql.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/issues/test_520.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/schema_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_get_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    49738 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/urls_inherited.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/tests/urls_pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.762130 graphene-django-3.1.2/graphene_django/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/tests/test_str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-06-17 06:42:31.000000 graphene-django-3.1.2/graphene_django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:42:35.758130 graphene-django-3.1.2/graphene_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 06:42:35.000000 graphene-django-3.1.2/graphene_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-17 06:42:35.762130 graphene-django-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-17 06:42:31.000000 graphene-django-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.204828 graphene-django-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-18 12:15:22.000000 graphene-django-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 12:15:22.000000 graphene-django-3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-18 12:15:29.204828 graphene-django-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-18 12:15:22.000000 graphene-django-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.180827 graphene-django-3.1.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.180827 graphene-django-3.1.3/examples/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.180827 graphene-django-3.1.3/examples/cookbook/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.180827 graphene-django-3.1.3/examples/cookbook/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.188827 graphene-django-3.1.3/examples/cookbook/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-18 12:15:22.000000 graphene-django-3.1.3/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.180827 graphene-django-3.1.3/examples/cookbook-plain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.180827 graphene-django-3.1.3/examples/cookbook-plain/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.180827 graphene-django-3.1.3/examples/cookbook-plain/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.188827 graphene-django-3.1.3/examples/cookbook-plain/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-18 12:15:22.000000 graphene-django-3.1.3/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.192827 graphene-django-3.1.3/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.192827 graphene-django-3.1.3/graphene_django/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.192827 graphene-django-3.1.3/graphene_django/debug/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/exception/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/exception/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.196827 graphene-django-3.1.3/graphene_django/debug/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/sql/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.196827 graphene-django-3.1.3/graphene_django/debug/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/debug/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.196827 graphene-django-3.1.3/graphene_django/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.196827 graphene-django-3.1.3/graphene_django/filter/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/filters/array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/filters/global_id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/filters/list_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/filters/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/filters/typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/filterset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/filter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_array_field_contains_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_array_field_exact_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_array_field_overlap_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_enum_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_in_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/tests/test_typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/tests/test_djangoinputobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/forms/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/management/commands/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/serializer_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/rest_framework/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/tests/test_field_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/rest_framework/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.184827 graphene-django-3.1.3/graphene_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/static/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/static/graphene_django/graphiql.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.184827 graphene-django-3.1.3/graphene_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.200827 graphene-django-3.1.3/graphene_django/templates/graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/templates/graphene/graphiql.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.204828 graphene-django-3.1.3/graphene_django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.204828 graphene-django-3.1.3/graphene_django/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/issues/test_520.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/schema_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_get_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49738 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/urls_inherited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/tests/urls_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.204828 graphene-django-3.1.3/graphene_django/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/utils/str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.204828 graphene-django-3.1.3/graphene_django/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/utils/tests/test_str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/utils/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-07-18 12:15:22.000000 graphene-django-3.1.3/graphene_django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:15:29.192827 graphene-django-3.1.3/graphene_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-18 12:15:29.000000 graphene-django-3.1.3/graphene_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-18 12:15:29.000000 graphene-django-3.1.3/graphene_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:15:29.000000 graphene-django-3.1.3/graphene_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:15:29.000000 graphene-django-3.1.3/graphene_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 12:15:29.000000 graphene-django-3.1.3/graphene_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 12:15:29.000000 graphene-django-3.1.3/graphene_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-18 12:15:29.204828 graphene-django-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-18 12:15:22.000000 graphene-django-3.1.3/setup.py
```

### Comparing `graphene-django-3.1.2/LICENSE` & `graphene-django-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/PKG-INFO` & `graphene-django-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.1.2
+Version: 3.1.3
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
```

### Comparing `graphene-django-3.1.2/README.md` & `graphene-django-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.1.3/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.1.3/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/converter.py` & `graphene-django-3.1.3/graphene_django/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/debug/middleware.py` & `graphene-django-3.1.3/graphene_django/debug/middleware.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/debug/sql/tracking.py` & `graphene-django-3.1.3/graphene_django/debug/sql/tracking.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/debug/sql/types.py` & `graphene-django-3.1.3/graphene_django/debug/sql/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/debug/tests/test_query.py` & `graphene-django-3.1.3/graphene_django/debug/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/fields.py` & `graphene-django-3.1.3/graphene_django/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/__init__.py` & `graphene-django-3.1.3/graphene_django/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/fields.py` & `graphene-django-3.1.3/graphene_django/filter/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/filters/__init__.py` & `graphene-django-3.1.3/graphene_django/filter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/filters/array_filter.py` & `graphene-django-3.1.3/graphene_django/filter/filters/array_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/filters/global_id_filter.py` & `graphene-django-3.1.3/graphene_django/filter/filters/global_id_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/filters/list_filter.py` & `graphene-django-3.1.3/graphene_django/filter/filters/list_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/filters/range_filter.py` & `graphene-django-3.1.3/graphene_django/filter/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/filters/typed_filter.py` & `graphene-django-3.1.3/graphene_django/filter/filters/typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/filterset.py` & `graphene-django-3.1.3/graphene_django/filter/filterset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/conftest.py` & `graphene-django-3.1.3/graphene_django/filter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/filters.py` & `graphene-django-3.1.3/graphene_django/filter/tests/filters.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_contains_filter.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_array_field_contains_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_exact_filter.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_array_field_exact_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_array_field_overlap_filter.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_array_field_overlap_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_enum_filtering.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_enum_filtering.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_fields.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_in_filter.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_in_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_range_filter.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/tests/test_typed_filter.py` & `graphene-django-3.1.3/graphene_django/filter/tests/test_typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/filter/utils.py` & `graphene-django-3.1.3/graphene_django/filter/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/forms/converter.py` & `graphene-django-3.1.3/graphene_django/forms/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/forms/forms.py` & `graphene-django-3.1.3/graphene_django/forms/forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/forms/mutation.py` & `graphene-django-3.1.3/graphene_django/forms/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/forms/tests/test_converter.py` & `graphene-django-3.1.3/graphene_django/forms/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/forms/tests/test_djangoinputobject.py` & `graphene-django-3.1.3/graphene_django/forms/tests/test_djangoinputobject.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/forms/tests/test_mutation.py` & `graphene-django-3.1.3/graphene_django/forms/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/forms/types.py` & `graphene-django-3.1.3/graphene_django/forms/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/management/commands/graphql_schema.py` & `graphene-django-3.1.3/graphene_django/management/commands/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/registry.py` & `graphene-django-3.1.3/graphene_django/registry.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/rest_framework/mutation.py` & `graphene-django-3.1.3/graphene_django/rest_framework/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/rest_framework/serializer_converter.py` & `graphene-django-3.1.3/graphene_django/rest_framework/serializer_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/rest_framework/tests/test_field_converter.py` & `graphene-django-3.1.3/graphene_django/rest_framework/tests/test_field_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py` & `graphene-django-3.1.3/graphene_django/rest_framework/tests/test_multiple_model_serializers.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/rest_framework/tests/test_mutation.py` & `graphene-django-3.1.3/graphene_django/rest_framework/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/settings.py` & `graphene-django-3.1.3/graphene_django/settings.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/static/graphene_django/graphiql.js` & `graphene-django-3.1.3/graphene_django/static/graphene_django/graphiql.js`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/templates/graphene/graphiql.html` & `graphene-django-3.1.3/graphene_django/templates/graphene/graphiql.html`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/issues/test_520.py` & `graphene-django-3.1.3/graphene_django/tests/issues/test_520.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/models.py` & `graphene-django-3.1.3/graphene_django/tests/models.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/schema.py` & `graphene-django-3.1.3/graphene_django/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/schema_view.py` & `graphene-django-3.1.3/graphene_django/tests/schema_view.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_command.py` & `graphene-django-3.1.3/graphene_django/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_converter.py` & `graphene-django-3.1.3/graphene_django/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_fields.py` & `graphene-django-3.1.3/graphene_django/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_forms.py` & `graphene-django-3.1.3/graphene_django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_get_queryset.py` & `graphene-django-3.1.3/graphene_django/tests/test_get_queryset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_query.py` & `graphene-django-3.1.3/graphene_django/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_schema.py` & `graphene-django-3.1.3/graphene_django/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_types.py` & `graphene-django-3.1.3/graphene_django/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_utils.py` & `graphene-django-3.1.3/graphene_django/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/tests/test_views.py` & `graphene-django-3.1.3/graphene_django/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/types.py` & `graphene-django-3.1.3/graphene_django/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/utils/testing.py` & `graphene-django-3.1.3/graphene_django/utils/testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/utils/tests/test_testing.py` & `graphene-django-3.1.3/graphene_django/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/utils/utils.py` & `graphene-django-3.1.3/graphene_django/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django/views.py` & `graphene-django-3.1.3/graphene_django/views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django.egg-info/PKG-INFO` & `graphene-django-3.1.3/graphene_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.1.2
+Version: 3.1.3
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
```

### Comparing `graphene-django-3.1.2/graphene_django.egg-info/SOURCES.txt` & `graphene-django-3.1.3/graphene_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/graphene_django.egg-info/requires.txt` & `graphene-django-3.1.3/graphene_django.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/setup.cfg` & `graphene-django-3.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `graphene-django-3.1.2/setup.py` & `graphene-django-3.1.3/setup.py`

 * *Files identical despite different names*

