# Comparing `tmp/py3seed-0.1.4.tar.gz` & `tmp/py3seed-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.1.4.tar", last modified: Mon Jul 17 08:24:11 2023, max compression
+gzip compressed data, was "py3seed-0.1.5.tar", last modified: Tue Jul 18 02:14:22 2023, max compression
```

## Comparing `py3seed-0.1.4.tar` & `py3seed-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.309841 py3seed-0.1.4/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.4/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:24:11.309965 py3seed-0.1.4/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.4/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.4/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-17 08:24:11.310570 py3seed-0.1.4/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.4/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.287514 py3seed-0.1.4/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.301378 py3seed-0.1.4/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.4/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.4/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.4/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.4/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.305923 py3seed-0.1.4/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.4/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    20437 2023-07-17 08:12:35.000000 py3seed-0.1.4/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.4/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.4/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.4/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.4/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57699 2023-07-13 02:24:43.000000 py3seed-0.1.4/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.4/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14318 2023-07-17 08:23:47.000000 py3seed-0.1.4/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.4/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.304924 py3seed-0.1.4/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-17 08:24:11.000000 py3seed-0.1.4/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:24:11.309329 py3seed-0.1.4/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.4/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6333 2023-07-13 03:38:58.000000 py3seed-0.1.4/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.4/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.4/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.4/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 02:14:22.221631 py3seed-0.1.5/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.5/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-18 02:14:22.221751 py3seed-0.1.5/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.5/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.5/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-18 02:14:22.222406 py3seed-0.1.5/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.5/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 02:14:22.198979 py3seed-0.1.5/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 02:14:22.214118 py3seed-0.1.5/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.5/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.5/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.5/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.5/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 02:14:22.217770 py3seed-0.1.5/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.5/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    20437 2023-07-17 08:12:35.000000 py3seed-0.1.5/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.5/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.5/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.5/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.5/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.1.5/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.5/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14546 2023-07-18 02:11:03.000000 py3seed-0.1.5/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.5/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 02:14:22.216869 py3seed-0.1.5/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-18 02:14:22.000000 py3seed-0.1.5/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-18 02:14:22.000000 py3seed-0.1.5/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-18 02:14:22.000000 py3seed-0.1.5/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-18 02:14:22.000000 py3seed-0.1.5/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-18 02:14:22.000000 py3seed-0.1.5/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-18 02:14:22.000000 py3seed-0.1.5/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 02:14:22.221042 py3seed-0.1.5/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.5/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6419 2023-07-18 02:13:30.000000 py3seed-0.1.5/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.5/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.5/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.5/tests/test_mongosupport.py
```

### Comparing `py3seed-0.1.4/LICENSE` & `py3seed-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/PKG-INFO` & `py3seed-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.4/setup.cfg` & `py3seed-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.1.4
+version = 0.1.5
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.1.4/src/py3seed/__init__.py` & `py3seed-0.1.5/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/__main__.py` & `py3seed-0.1.5/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/admin.py` & `py3seed-0.1.5/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/cachesupport.py` & `py3seed-0.1.5/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/commands/gen.py` & `py3seed-0.1.5/src/py3seed/commands/gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/error.py` & `py3seed-0.1.5/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/inflection.py` & `py3seed-0.1.5/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/log.py` & `py3seed-0.1.5/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/merge3.py` & `py3seed-0.1.5/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/model.py` & `py3seed-0.1.5/src/py3seed/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
                     save_field = ModelField(
                         name=field.save_field_name,
                         type_=List[id_type] if f_origin is list else id_type,
                         required=field.required,
                         editable=False,  # save field value will be updated by its source field, so no need to render in form
                         source_field_name=ann_name,  # Mark the source field
                     )
-                    # back_field_name should always has a meaningful value, if it is none, do not create back field in related object
+                    # back_field_name should always have a meaningful value, if it is none, do not create back field in related object
                     # e.g,
                     # project.activities.user -> user, no need to create back_field in user model as it is hard to search all the activities for user
                     # in such case, we need to create activity model, activity.project -> project.activities, activity.user -> user.activities
                     if field.back_field_name is None:
                         pass
                     #
                     relations[ann_name] = value
```

### Comparing `py3seed-0.1.4/src/py3seed/mongosupport.py` & `py3seed-0.1.5/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed/utils.py` & `py3seed-0.1.5/src/py3seed/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import math
 import os
 import re
 import shutil
 import stat
 import logging
 
-from py3seed import inflection, LayoutError
+from py3seed import inflection, LayoutError, Format
 
 logger = logging.getLogger('pyseed')
 
 
 def force_delete(func, path, exc_info):
     """ Error handler for `shutil.rmtree()` equivalent to `rm -rf`.
 
@@ -77,15 +77,15 @@
             'name_title': name_title,  # => Sample Model
             'name_title_lower': name_title.lower(),  # => sample model
             'name_title_lower_plural': inflection.pluralize(name_title.lower()),  # => sample models
         }
 
 
 # Match span
-SPAN_REGEX = re.compile(r'^(.*)#([a-zA-Z_-]*)([0-9]+)$')
+SPAN_REGEX = re.compile(r'^(.*)#([a-zA-Z_-]*)([0-9]*)$')
 
 
 def parse_layout(body, schema):
     """ Parse layout defined in a model action.
     e.g,
     'demo/user-profile': {              # action name
         'domains': ['www'],             # domains that this action is available
@@ -248,15 +248,16 @@
         # Parse span at the end, e.g, a?param=1#summary4
         span_match = SPAN_REGEX.match(column_str)
         if span_match:
             column_str = span_match.group(1)
             if span_match.group(2):
                 ret.update({'format': span_match.group(2)})  # -> summary
             #
-            ret.update({'span': int(span_match.group(3))})  # -> 4
+            if span_match.group(3):
+                ret.update({'span': int(span_match.group(3))})  # -> 4
         # Parse params, e.g, a?param=1#4
         if '?' in column_str:
             column_str, column_params = _parse_query_str(column_str)
             ret.update({'params': column_params})
         #
         ret.update({'name': column_str})
         #
@@ -311,28 +312,30 @@
     return {
         'action': action,
         'params': params,
         'rows': rows
     }
 
 
-def get_layout_fields(layout):
+def get_layout_fields(layout, skip_formats=Format.SUMMARY):
     """ Do not recursively parse inner object/array, only return current level field names. """
     for row in layout:
         for col in row:
             col_name = col['name']
+            col_format = col.get('format', '')
             if not col_name:
                 pass
             elif col_name == '-':
                 pass
-            elif col_name.replace('.', '').isdigit():
-                # Need to get fields under a group
+            elif col_name.replace('.', '').isdigit() and col_format not in skip_formats:
+                # Need to get fields under a group, but not summary group as it is only for displaying and do not have
                 yield from get_layout_fields(col['rows'])
             else:
                 # Return current level field names, do not recursively parse inner object/array
+
                 yield col_name
 
 
 class Pagination(object):
     """ Pagination support. """
 
     def __init__(self, page, per_page, total_count):
```

### Comparing `py3seed-0.1.4/src/py3seed/websupport.py` & `py3seed-0.1.5/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.1.5/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.4/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.1.5/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/tests/test_cachesupport.py` & `py3seed-0.1.5/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/tests/test_gen.py` & `py3seed-0.1.5/tests/test_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           email          point#4,
           phone
           create_time
     '''
     user_schema = User.schema()
     # Team members
     team_members_layout = '''#!read?title=Members
-        1#summary4,    members#8                                                  
+        1#summary,     members#8                                                  
           logo           avatar, name, status, roles, email, phone, team_join_time
           name         
           phone                                                                
           members                                                                   
           create_time  
     '''
     team_schema = Team.schema()
@@ -93,18 +93,21 @@
     assert first_row[1]['rows'][4][0]['span'] == 4
     assert first_row[1]['rows'][4][1]['name'] == ''
 
     # Team member layout
     layout = parse_layout(team_members_layout, team_schema)
     assert layout['action'] == 'read'
     first_row = layout['rows'][0]
+    assert 'span' not in first_row[0]
+    assert first_row[0]['format'] == 'summary'
     assert len(first_row[1]['rows'][0]) == 7
     assert first_row[1]['rows'][0][0]['name'] == 'avatar'
 
 
+
 def test_gen():
     """ Test Generation. """
     # Change working folder
     os.chdir('tests')
     #
     # Init
     #
```

### Comparing `py3seed-0.1.4/tests/test_merge3.py` & `py3seed-0.1.5/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/tests/test_model.py` & `py3seed-0.1.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.4/tests/test_mongosupport.py` & `py3seed-0.1.5/tests/test_mongosupport.py`

 * *Files identical despite different names*

