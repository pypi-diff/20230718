# Comparing `tmp/metabolights_utils-0.9.1.tar.gz` & `tmp/metabolights_utils-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolights_utils-0.9.1.tar", max compression
+gzip compressed data, was "metabolights_utils-0.9.2.tar", max compression
```

## Comparing `metabolights_utils-0.9.1.tar` & `metabolights_utils-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,56 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.1/LICENSE
--rw-r--r--   0        0        0      127 2023-07-11 10:00:54.645345 metabolights_utils-0.9.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 10:49:29.981642 metabolights_utils-0.9.1/metabolights_utils/__init__.py
--rw-r--r--   0        0        0     4695 2023-07-11 08:58:03.250729 metabolights_utils-0.9.1/metabolights_utils/isa_metadata.py
--rw-r--r--   0        0        0        0 2023-07-10 10:51:24.233594 metabolights_utils-0.9.1/metabolights_utils/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 12:23:13.111498 metabolights_utils-0.9.1/metabolights_utils/models/isa/__init__.py
--rw-r--r--   0        0        0      513 2023-07-10 12:23:39.994055 metabolights_utils-0.9.1/metabolights_utils/models/isa/assay_file.py
--rw-r--r--   0        0        0      390 2023-07-10 12:23:40.058905 metabolights_utils-0.9.1/metabolights_utils/models/isa/assignment_file.py
--rw-r--r--   0        0        0     7596 2023-07-11 09:02:02.875380 metabolights_utils-0.9.1/metabolights_utils/models/isa/collector/db_metadata_collector.py
--rw-r--r--   0        0        0     4469 2023-07-11 08:43:05.453662 metabolights_utils-0.9.1/metabolights_utils/models/isa/collector/folder_metadata_collector.py
--rw-r--r--   0        0        0     5162 2023-07-11 08:54:31.586364 metabolights_utils-0.9.1/metabolights_utils/models/isa/common.py
--rw-r--r--   0        0        0     2046 2023-07-10 12:23:13.309473 metabolights_utils-0.9.1/metabolights_utils/models/isa/enums.py
--rw-r--r--   0        0        0    20295 2023-07-11 08:59:23.469787 metabolights_utils-0.9.1/metabolights_utils/models/isa/investigation_file.py
--rw-r--r--   0        0        0      933 2023-07-10 21:58:40.074714 metabolights_utils-0.9.1/metabolights_utils/models/isa/messages.py
--rw-r--r--   0        0        0     1387 2023-07-10 12:23:38.572167 metabolights_utils-0.9.1/metabolights_utils/models/isa/metabolights_study.py
--rw-r--r--   0        0        0     6583 2023-07-11 09:06:15.678113 metabolights_utils-0.9.1/metabolights_utils/models/isa/parser/common.py
--rw-r--r--   0        0        0    21356 2023-07-11 10:11:34.361845 metabolights_utils-0.9.1/metabolights_utils/models/isa/parser/investigation_parser.py
--rw-r--r--   0        0        0    16736 2023-07-11 09:07:28.571579 metabolights_utils-0.9.1/metabolights_utils/models/isa/parser/isa_table_parser.py
--rw-r--r--   0        0        0      448 2023-07-10 23:58:31.586413 metabolights_utils-0.9.1/metabolights_utils/models/isa/samples_file.py
--rw-r--r--   0        0        0      992 2023-07-10 12:23:38.571936 metabolights_utils-0.9.1/metabolights_utils/models/isa/study_db_metadata.py
--rw-r--r--   0        0        0      620 2023-07-10 12:23:40.261669 metabolights_utils-0.9.1/metabolights_utils/models/isa/study_folder_metadata.py
--rw-r--r--   0        0        0     1326 2023-07-11 11:56:19.738156 metabolights_utils-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 metabolights_utils-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3259 2023-07-17 20:48:23.394069 metabolights_utils-0.9.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 10:49:29.981642 metabolights_utils-0.9.2/metabolights_utils/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-18 12:41:51.755776 metabolights_utils-0.9.2/metabolights_utils/common.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:23.231059 metabolights_utils-0.9.2/metabolights_utils/isatab/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:19:51.764169 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-15 14:29:29.004862 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/assay_file_helper.py
+-rw-r--r--   0        0        0     1260 2023-07-15 14:29:28.898072 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/assignment_file_helper.py
+-rw-r--r--   0        0        0     1512 2023-07-14 08:36:13.926789 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/base_isa_file_helper.py
+-rw-r--r--   0        0        0     5829 2023-07-17 20:54:44.959168 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/base_isa_table_file_helper.py
+-rw-r--r--   0        0        0    10677 2023-07-17 21:37:37.333171 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/investigation_file_helper.py
+-rw-r--r--   0        0        0      698 2023-07-15 14:29:29.056606 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/sample_file_helper.py
+-rw-r--r--   0        0        0     1682 2023-07-17 20:52:46.971222 metabolights_utils-0.9.2/metabolights_utils/isatab/investigation_file_reader.py
+-rw-r--r--   0        0        0     2050 2023-07-14 08:12:36.253515 metabolights_utils-0.9.2/metabolights_utils/isatab/investigation_file_writer.py
+-rw-r--r--   0        0        0     8102 2023-07-15 15:46:43.496883 metabolights_utils-0.9.2/metabolights_utils/isatab/isa_table_file_reader.py
+-rw-r--r--   0        0        0     2909 2023-07-18 17:00:04.330628 metabolights_utils-0.9.2/metabolights_utils/isatab/isa_table_file_writer.py
+-rw-r--r--   0        0        0     1844 2023-07-18 16:48:05.150888 metabolights_utils-0.9.2/metabolights_utils/isatab/isatab_file_helper.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:51:24.233594 metabolights_utils-0.9.2/metabolights_utils/models/__init__.py
+-rw-r--r--   0        0        0      442 2023-07-18 12:41:42.144955 metabolights_utils-0.9.2/metabolights_utils/models/common.py
+-rw-r--r--   0        0        0      149 2023-07-12 17:00:03.147342 metabolights_utils-0.9.2/metabolights_utils/models/enums.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:23:13.111498 metabolights_utils-0.9.2/metabolights_utils/models/isa/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-17 20:42:23.361722 metabolights_utils-0.9.2/metabolights_utils/models/isa/assay_file.py
+-rw-r--r--   0        0        0      402 2023-07-17 20:41:02.431487 metabolights_utils-0.9.2/metabolights_utils/models/isa/assignment_file.py
+-rw-r--r--   0        0        0    10881 2023-07-17 21:24:19.800755 metabolights_utils-0.9.2/metabolights_utils/models/isa/common.py
+-rw-r--r--   0        0        0      478 2023-07-12 16:53:15.362181 metabolights_utils-0.9.2/metabolights_utils/models/isa/enums.py
+-rw-r--r--   0        0        0    10817 2023-07-17 21:27:02.610563 metabolights_utils-0.9.2/metabolights_utils/models/isa/investigation_file.py
+-rw-r--r--   0        0        0    17617 2023-07-17 20:53:30.375766 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/common.py
+-rw-r--r--   0        0        0     9125 2023-07-16 16:31:04.548645 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/filter.py
+-rw-r--r--   0        0        0    21626 2023-07-17 21:25:57.104435 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/investigation_parser.py
+-rw-r--r--   0        0        0    17992 2023-07-17 20:54:45.872793 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/isa_table_parser.py
+-rw-r--r--   0        0        0     5159 2023-07-16 16:31:08.768258 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/sort.py
+-rw-r--r--   0        0        0      457 2023-07-17 20:43:34.998092 metabolights_utils-0.9.2/metabolights_utils/models/isa/samples_file.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:31:33.134362 metabolights_utils-0.9.2/metabolights_utils/models/metabolights/__init__.py
+-rw-r--r--   0        0        0     1077 2023-07-17 20:39:40.816755 metabolights_utils-0.9.2/metabolights_utils/models/metabolights/metabolights_study.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:36:01.541604 metabolights_utils-0.9.2/metabolights_utils/models/parser/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-15 08:09:31.938967 metabolights_utils-0.9.2/metabolights_utils/models/parser/common.py
+-rw-r--r--   0        0        0      148 2023-07-15 08:10:44.291129 metabolights_utils-0.9.2/metabolights_utils/models/parser/enums.py
+-rw-r--r--   0        0        0        0 2023-07-18 12:31:01.631181 metabolights_utils-0.9.2/metabolights_utils/tsv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:19:49.880266 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/__init__.py
+-rw-r--r--   0        0        0     3413 2023-07-18 12:46:07.521346 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/add_column.py
+-rw-r--r--   0        0        0     3201 2023-07-18 12:49:27.614018 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/add_row.py
+-rw-r--r--   0        0        0     1342 2023-07-18 15:49:15.831466 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/base.py
+-rw-r--r--   0        0        0     3351 2023-07-18 13:49:23.813831 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/copy_column.py
+-rw-r--r--   0        0        0     3097 2023-07-18 15:16:49.116854 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/copy_row.py
+-rw-r--r--   0        0        0     2423 2023-07-18 14:00:02.070569 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/delete_column.py
+-rw-r--r--   0        0        0     2012 2023-07-18 12:45:05.682152 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/delete_row.py
+-rw-r--r--   0        0        0     2780 2023-07-18 13:38:55.025530 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/move_column.py
+-rw-r--r--   0        0        0     3372 2023-07-18 12:45:05.343441 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/move_row.py
+-rw-r--r--   0        0        0     3062 2023-07-18 16:25:10.033932 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_cell.py
+-rw-r--r--   0        0        0     3384 2023-07-18 14:51:21.210651 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_column.py
+-rw-r--r--   0        0        0     2047 2023-07-18 14:15:45.293287 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_column_header.py
+-rw-r--r--   0        0        0     2294 2023-07-18 15:46:46.103848 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_row.py
+-rw-r--r--   0        0        0     3549 2023-07-18 15:46:02.737733 metabolights_utils-0.9.2/metabolights_utils/tsv/model.py
+-rw-r--r--   0        0        0     5701 2023-07-18 16:14:32.052914 metabolights_utils-0.9.2/metabolights_utils/tsv/tsv_file_updater.py
+-rw-r--r--   0        0        0     1310 2023-07-18 17:31:44.686363 metabolights_utils-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 metabolights_utils-0.9.2/PKG-INFO
```

### Comparing `metabolights_utils-0.9.1/LICENSE` & `metabolights_utils-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.1/metabolights_utils/models/isa/parser/investigation_parser.py` & `metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/investigation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import os
 import re
 import sys
+from io import IOBase
 from typing import Dict, List, Tuple, Union
 
+import humps
 from pydantic import BaseModel
 
 from metabolights_utils.models.isa import investigation_file as model
-from metabolights_utils.models.isa.common import Comment, IsaAbstractModel
-from metabolights_utils.models.isa.enums import ParserMessageType
-from metabolights_utils.models.isa.messages import ParserMessage
+from metabolights_utils.models.isa.common import (
+    INVESTIGATION_FILE_INITIAL_ROWS_SET,
+    INVESTIGATION_FILE_STUDY_ROWS_SET,
+    Comment,
+    IsaAbstractModel,
+)
 from metabolights_utils.models.isa.parser.common import read_investigation_file
+from metabolights_utils.models.parser.common import ParserMessage
+from metabolights_utils.models.parser.enums import ParserMessageType
 
 model_module_name = model.__name__
 
 
 def parse_investigation_from_fs(
-    file_path,
+    file_path: str,
 ) -> Tuple[Union[model.Investigation, None], List[ParserMessage]]:
     messages: List[ParserMessage] = []
     basename = os.path.basename(file_path)
     if not os.path.exists(file_path):
         print(f"File does not exist: {basename}")
         message = ParserMessage(short="File does not exist", type=ParserMessageType.CRITICAL)
         message.detail = f"File does not exist: {basename}"
@@ -30,19 +37,19 @@
         print(f"File is empty: {basename}")
         message = ParserMessage(short="File is empty", type=ParserMessageType.CRITICAL)
         message.detail = f"File is empty: {basename}"
         messages.append(message)
         return None, messages
 
     with open(file_path, "r") as f:
-        investigation = get_investigation(basename, f, file_path, messages=messages)
+        investigation = get_investigation(f, file_path, messages=messages)
         return investigation, messages
 
 
-def get_investigation(file_name, file_path_or_buffer, source, messages: List[ParserMessage]):
+def get_investigation(file_buffer: IOBase, file_path: str, messages: List[ParserMessage]):
     if messages is None:
         messages = []
     index_map = {}
     initial_part = []
     study_parts = []
     initial_part_index_map = {}
     study_parts_index_map = []
@@ -50,17 +57,15 @@
     ignore_comments = []
     inital_part_comments = {}
     study_part_comment = {}
     study_part_comment_list = []
     is_study_part = False
     current_section = ""
 
-    result: Dict[int, Dict[int, str]] = read_investigation_file(
-        file_name, file_path_or_buffer, messages
-    )
+    result: Dict[int, Dict[int, str]] = read_investigation_file(file_buffer, messages)
     if result is None:
         return model.Investigation()
 
     tab: Dict[int, Dict[int, str]] = result
     for line in tab.keys():
         if len(tab[line]) == 0:
             message = ParserMessage(short="Empty line", type=ParserMessageType.WARNING)
@@ -69,16 +74,16 @@
             messages.append(message)
             index_map[line] = ""
             continue
         index_string = tab[line][0]
         index_map[line] = index_string
 
         if (
-            index_string not in model.INVESTIGATION_FILE_INITIAL_ROWS_SET
-            and index_string not in model.INVESTIGATION_FILE_STUDY_ROWS_SET
+            index_string not in INVESTIGATION_FILE_INITIAL_ROWS_SET
+            and index_string not in INVESTIGATION_FILE_STUDY_ROWS_SET
         ):
             if index_string.startswith("#"):
                 ignore_comments.append(line)
                 messages.append(
                     ParserMessage(
                         type=ParserMessageType.INFO,
                         short="File comment line",
@@ -120,15 +125,15 @@
             message.detail = f"Line {str(line + 1)}: {index_string} is not valid section start"
             messages.append(message)
             message.line = str(line)
 
         if not is_study_part:
             if index_string == "STUDY":
                 is_study_part = True
-            elif index_string not in model.INVESTIGATION_FILE_INITIAL_ROWS_SET:
+            elif index_string not in INVESTIGATION_FILE_INITIAL_ROWS_SET:
                 message = ParserMessage(
                     short="Unexpected line in the section", type=ParserMessageType.ERROR
                 )
                 message.detail = f"Unexpected line in {str(line  + 1)}"
                 message.line = str(line)
                 messages.append(message)
                 continue
@@ -143,38 +148,38 @@
                 study_part = []
                 study_part_index = {}
                 study_part_comment = {}
                 study_parts_index_map.append(study_part_index)
                 study_part_comment_list.append(study_part_comment)
                 study_parts.append(study_part)
 
-            if index_string not in model.INVESTIGATION_FILE_STUDY_ROWS_SET:
+            if index_string not in INVESTIGATION_FILE_STUDY_ROWS_SET:
                 message = ParserMessage(
                     short="Unexpected line in the study section",
                     type=ParserMessageType.ERROR,
                 )
                 message.detail = f"Unexpected line in {str(line  + 1)}"
                 message.line = str(line)
                 messages.append(message)
                 continue
             if study_part or new_study_part:
                 study_part.append(index_string)
                 study_part_index[index_string] = line
 
     studies = build_studies(
-        source,
+        file_path,
         messages,
         study_parts,
         study_parts_index_map,
         study_part_comment_list,
         tab,
     )
 
     investigation, _ = build_investigation(
-        source,
+        file_path,
         initial_part_index_map,
         tab,
         studies,
         inital_part_comments,
         messages=messages,
     )
     return investigation
@@ -256,14 +261,19 @@
         comments_map=comments_map,
         messages=messages,
     )
     investigation.studies = studies
     return investigation, messages
 
 
+def set_value(obj, key, value):
+    camel_key = humps.decamelize(key)
+    setattr(obj, camel_key, value)
+
+
 def assign_by_field_name(
     file_path,
     data: BaseModel,
     index_map: dict,
     tab: dict,
     messages: List[ParserMessage],
     prefix="",
@@ -363,15 +373,15 @@
                                         field_definition["search_header"],
                                     ]
                                 )
                             else:
                                 search_field = f"{name_prefix} {field_definition['search_header']}"
 
                         item_list = []
-                        setattr(data, key, item_list)
+                        set_value(data, key, item_list)
 
                         if search_field not in index_map:
                             print(
                                 f"{search_field} is not in file. Skipping {field_name} in {file_path}"
                             )
                             continue
                         index = index_map[search_field]
@@ -413,15 +423,15 @@
                             items["$ref"].replace("#/definitions/", "").replace("#/$defs/", "")
                         )
                         ref_class = getattr(
                             sys.modules[model_module_name],
                             ref_class_name,
                         )
                         instance = ref_class()
-                        setattr(data, key, [instance])
+                        set_value(data, key, [instance])
                         assign_by_field_name(
                             file_path,
                             instance,
                             index_map,
                             tab,
                             prefix=field_name,
                             value_index=value_index,
@@ -441,32 +451,33 @@
                             ):
                                 continue
                             if (
                                 "seperator" in item_field_definition
                                 and item_field_definition["seperator"]
                             ):
                                 separator = item_field_definition["seperator"]
-                            item_val = getattr(instance, item_key) or ""
+                            attribute_key = humps.decamelize(item_key)
+                            item_val = getattr(instance, attribute_key) or ""
                             seperated_values = item_val.split(separator)
                             for _ in range(len(seperated_values)):
                                 instance_count = len(new_instances)
                                 values_count = len(seperated_values)
                                 if instance_count < values_count:
                                     for _ in range(instance_count, values_count):
                                         new_instances.append(ref_class())
                                 for j in range(values_count):
-                                    setattr(new_instances[j], item_key, seperated_values[j])
+                                    set_value(new_instances[j], item_key, seperated_values[j])
                         count = len(new_instances)
                         for i in range(len(new_instances)):
                             instance_item = new_instances[count - i - 1]
                             if IsaAbstractModel.is_empty_model(model=instance_item):
                                 new_instances.pop()
                             else:
                                 break
-                        setattr(data, key, new_instances)
+                        set_value(data, key, new_instances)
                     else:
                         message = ParserMessage(
                             short="Reference item is not valid",
                             type=ParserMessageType.WARNING,
                         )
                         message.detail = f"Reference item is not valid {data_type} "
                         messages.append(message)
@@ -482,30 +493,30 @@
                 if field_name not in index_map:
                     message = ParserMessage(
                         short="Index is not defined", type=ParserMessageType.WARNING
                     )
                     message.detail = f"{field_name} is not in {file_path}. "
                     messages.append(message)
                     print(f"{field_name} is not in {file_path}. Skipping")
-                    setattr(data, key, "")
+                    set_value(data, key, "")
                     continue
                 index = index_map[field_name]
                 value = ""
                 if len(tab[index]) > value_index:
                     value = tab[index][value_index]
                 else:
                     value = ""
-                setattr(data, key, str(value) or "")
+                set_value(data, key, str(value) or "")
             elif data_type == "ref":
                 ref_class_name = ref_object_definition.replace("#/definitions/", "").replace(
                     "#/$defs/", ""
                 )
                 ref_class = getattr(sys.modules[model_module_name], ref_class_name)
                 instance = ref_class()
-                setattr(data, key, instance)
+                set_value(data, key, instance)
                 assign_by_field_name(
                     file_path,
                     instance,
                     index_map,
                     tab,
                     prefix=field_name,
                     value_index=value_index,
```

### Comparing `metabolights_utils-0.9.1/metabolights_utils/models/isa/parser/isa_table_parser.py` & `metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/isa_table_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import os
 import re
-from io import TextIOWrapper
+from io import IOBase
 from typing import List, Tuple, Union
 
-from pandas import DataFrame
-
 from metabolights_utils.models.isa.common import IsaTableColumn, IsaTableFile
-from metabolights_utils.models.isa.enums import (
-    ColumnsStructure,
-    IsaTableAdditionalColumn,
-    ParserMessageType,
+from metabolights_utils.models.isa.enums import ColumnsStructure, IsaTableAdditionalColumn
+from metabolights_utils.models.isa.parser.common import (
+    SelectedTsvFileContent,
+    TsvFileFilterOption,
+    read_table_file,
 )
-from metabolights_utils.models.isa.messages import ParserMessage
-from metabolights_utils.models.isa.parser.common import read_table_file
+from metabolights_utils.models.isa.parser.sort import TsvFileSortOption
+from metabolights_utils.models.parser.common import ParserMessage
+from metabolights_utils.models.parser.enums import ParserMessageType
 
 
 def parse_isa_table_sheet_from_fs(
-    file_path, expected_patterns: Union[None, List[List[str]]] = None, **kwargs
+    file_path: str,
+    expected_patterns: Union[None, List[List[str]]] = None,
+    selected_columns: Union[None, List[str]] = None,
+    offset: Union[int, None] = None,
+    limit: Union[int, None] = None,
+    filter_options: List[TsvFileFilterOption] = None,
+    sort_options: List[TsvFileSortOption] = None,
 ) -> Tuple[IsaTableFile, List[ParserMessage]]:
     basename = os.path.basename(file_path)
     dirname = os.path.basename(os.path.dirname(file_path))
     messages: List[ParserMessage] = []
     if not file_path:
         message = ParserMessage(short="File path is not valid", type=ParserMessageType.CRITICAL)
         message.detail = "File path is not valid"
@@ -42,36 +48,44 @@
         message.detail = f"File is empty: {basename} in {dirname}"
         messages.append(message)
         return IsaTableFile(), messages
     basename = os.path.basename(file_path)
 
     with open(file_path, "r") as f:
         read_messages: List[ParserMessage] = []
-        isa_table = get_isa_table(
-            basename,
+        isa_table: IsaTableFile = get_isa_table(
             f,
+            basename,
             messages=read_messages,
             expected_patterns=expected_patterns,
-            **kwargs,
+            selected_columns=selected_columns,
+            offset=offset,
+            limit=limit,
+            filter_options=filter_options,
+            sort_options=sort_options,
         )
         if isa_table.table.columns:
             messages.extend(read_messages)
             messages = [x for x in messages if x.type != ParserMessageType.INFO]
             return isa_table, messages
 
     with open(file_path, "r", errors="backslashreplace") as f:
-        read_messages = []
+        read_messages: List[ParserMessage] = []
         isa_table = get_isa_table(
-            basename,
             f,
+            basename,
             messages=read_messages,
             expected_patterns=expected_patterns,
-            **kwargs,
+            selected_columns=selected_columns,
+            offset=offset,
+            limit=limit,
+            filter_options=filter_options,
+            sort_options=sort_options,
         )
-        isa_table.filePath = basename
+        isa_table.file_path = basename
 
         if isa_table.table.columns:
             message = ParserMessage(
                 short="File is read utf-8 encoding and invalid characters errors are replaced with backslash",
                 type=ParserMessageType.WARNING,
             )
             message.detail = (
@@ -83,124 +97,123 @@
             messages = [x for x in messages if x.type != ParserMessageType.INFO]
             return isa_table, messages
     messages = [x for x in messages if x.type != ParserMessageType.INFO]
     return isa_table, messages
 
 
 def get_isa_table(
-    file_name,
-    file_path_or_buffer: TextIOWrapper,
+    file_path_or_buffer: IOBase,
+    file_name: str,
     messages: List[ParserMessage],
-    expected_patterns,
-    **kwargs,
+    expected_patterns: List[List[str]],
+    selected_columns: Union[None, List[str]] = None,
+    offset: Union[int, None] = None,
+    limit: Union[int, None] = None,
+    filter_options: List[TsvFileFilterOption] = None,
+    sort_options: List[TsvFileSortOption] = None,
 ):
     study_table = IsaTableFile()
     if messages is None:
         messages = []
     if not expected_patterns:
         expected_patterns = []
     file_path_or_buffer.seek(0)
-    df: DataFrame = read_table_file(
-        file_name,
+    content: SelectedTsvFileContent = read_table_file(
         file_path_or_buffer,
         messages,
-        header=0,
-        delimiter="\t",
-        dtype=str,
-        **kwargs,
+        selected_columns,
+        offset,
+        limit,
+        filter_options,
+        sort_options,
     )
-    if df is None:
+    if content is None:
         return study_table
     return update_isa_table_file(
         study_table,
-        df,
+        content,
         file_name,
-        file_path_or_buffer,
         messages,
         expected_patterns,
-        **kwargs,
     )
 
 
 def update_isa_table_file(
     study_table: IsaTableFile,
-    df: DataFrame,
+    content: SelectedTsvFileContent,
     file_name: str,
-    file_path_or_buffer: TextIOWrapper,
     messages: List[ParserMessage],
     expected_patterns,
-    **kwargs,
 ):
-    columns = list(df.columns)
+    # columns = list(df.columns)
+    columns = [x.column_name for x in content.columns]
+    column_indices = {x.column_name: x.column_index for x in content.columns}
     first_column_name = None
     for column_name in columns:
         if not first_column_name:
             first_column_name = column_name
         cleaned_column_name = get_cleaned_header(column_name)
 
         if not len(cleaned_column_name.strip()) or len(cleaned_column_name) != len(
             cleaned_column_name.strip()
         ):
             message = ParserMessage(type=ParserMessageType.ERROR)
-            column_index = columns.index(column_name)
+            column_index = column_indices[column_name]
             message.column = str(column_index)
             if len(cleaned_column_name.strip()) > 0:
                 message.short = "Column header starts or ends with space"
                 message.detail = (
                     f"'{column_name}' header at column {column_index + 1} "
                     + "ends or starts with space."
                 )
             else:
                 message.short = "Column header is empty"
                 message.detail = f"'{column_name}' header at column {column_index + 1}  is empty."
             messages.append(message)
 
     headers = get_headers(columns, expected_patterns=expected_patterns, messages=messages)
     study_table.table.headers = headers
-    if first_column_name:
-        file_path_or_buffer.seek(0)
-        total_df: DataFrame = read_table_file(
-            file_name,
-            file_path_or_buffer,
-            [],
-            delimiter="\t",
-            usecols=[first_column_name],
-            dtype=str,
-        )
-        if total_df is not None:
-            study_table.table.totalRowCount = len(total_df.index)
-    if "skiprows" in kwargs and kwargs["skiprows"] and len(kwargs["skiprows"]) > 0:
-        offset = len(kwargs["skiprows"])
-        if offset < study_table.table.totalRowCount:
-            study_table.table.rowOffset = len(kwargs["skiprows"])
-        else:
-            study_table.table.rowOffset = 0
-
-    data = df.to_dict(orient="list")
-    study_table.table.data = data
+    study_table.table.total_row_count = content.total_rows
+    study_table.table.row_offset = content.offset
+    study_table.table.row_count = content.limit
+    study_table.table.filtered_total_row_count = content.total_filtered_rows
+    study_table.table.selected_column_count = content.selected_column_count
+    study_table.table.total_column_count = content.total_columns
+    study_table.table.filter_options = content.filter_options
+    study_table.table.sort_options = content.sort_options
+
+    filtered_data = {}
+
+    for column in content.columns:
+        if not study_table.table.row_indices:
+            study_table.table.row_indices = [x for x in column.rows]
+        filtered_data[column.column_name] = [column.rows[x] for x in column.rows]
+    study_table.table.column_indices = [column.column_index for column in content.columns]
+    # data = df.to_dict(orient="list")
+    study_table.table.data = filtered_data
     study_table.table.columns = columns
-    study_table.table.rowCount = len(df.index)
-    study_table.filePath = file_name
+    # study_table.table.row_count = len(content.columns[0].rows)
+    study_table.file_path = file_name
 
     return study_table
 
 
 MULTI_COLUMN_TEMPLATES = {
     ColumnsStructure.ONTOLOGY_COLUMN: {
-        "columnNames": [
+        "column_names": [
             IsaTableAdditionalColumn.TERM_SOURCE_REF,
             IsaTableAdditionalColumn.TERM_ACCSSION_NUMBER,
         ],
         "searchPatterns": [
             "(Term Source REF)(\.\d+)?",
             "(Term Accession Number)(\.\d+)?",
         ],
     },
     ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY: {
-        "columnNames": [
+        "column_names": [
             IsaTableAdditionalColumn.UNIT,
             IsaTableAdditionalColumn.TERM_SOURCE_REF,
             IsaTableAdditionalColumn.TERM_ACCSSION_NUMBER,
         ],
         "searchPatterns": [
             "(Unit)(\.\d+)?",
             "(Term Source REF)(\.\d+)?",
@@ -211,16 +224,16 @@
 
 additional_column_templates = [
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY]["searchPatterns"],
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.ONTOLOGY_COLUMN]["searchPatterns"],
 ]
 
 additional_column_headers = [
-    MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY]["columnNames"],
-    MULTI_COLUMN_TEMPLATES[ColumnsStructure.ONTOLOGY_COLUMN]["columnNames"],
+    MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY]["column_names"],
+    MULTI_COLUMN_TEMPLATES[ColumnsStructure.ONTOLOGY_COLUMN]["column_names"],
 ]
 
 multiple_columns_additional_header_patterns = MULTI_COLUMN_TEMPLATES[
     ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY
 ]["searchPatterns"]
 
 
@@ -271,21 +284,21 @@
         for i in range(len(expected_patterns)):
             result = re.search(expected_patterns[i][0], column_name)
             if result and result.groups():
                 pattern_index = i
                 expected_header = result and result.groups()
                 break
 
-        column = IsaTableColumn(columnIndex=str(column_index), colummnStructure=column_structure)
-        column.columnName = column_name
-        column.columnHeader = cleaned_column_name
+        column = IsaTableColumn(column_index=str(column_index), colummn_structure=column_structure)
+        column.column_name = column_name
+        column.column_header = cleaned_column_name
         linked_columns = []
 
         if column_structure == ColumnsStructure.ADDITIONAL_COLUMN:
-            column.columnCategory = "Additional"
+            column.column_category = "Additional"
             message.type = ParserMessageType.CRITICAL
             message.short = (
                 "Additional column header"
                 + f"'{cleaned_column_name}'"
                 + "is not linked to a previous header."
             )
         elif column_structure == ColumnsStructure.SINGLE_COLUMN:
@@ -303,26 +316,26 @@
                 cleaned_column_name,
                 pattern_index,
                 expected_header,
                 message,
                 column,
             )
         else:
-            column.additionalColumns = additional_column_headers
+            column.additional_columns = additional_column_headers
             additional_column_index = column_index
 
-            for additional_column in column.additionalColumns:
+            for additional_column in column.additional_columns:
                 additional_column_index = additional_column_index + 1
                 linked_column = IsaTableColumn(
-                    columnIndex=str(additional_column_index),
-                    colummnStructure=ColumnsStructure.LINKED_COLUMN,
+                    column_index=str(additional_column_index),
+                    colummn_structure=ColumnsStructure.LINKED_COLUMN,
                 )
-                linked_column.columnHeader = additional_column
-                linked_column.columnCategory = "Linked Column"
-                linked_column.columnName = columns[additional_column_index]
+                linked_column.column_header = additional_column
+                linked_column.column_category = "Linked Column"
+                linked_column.column_name = columns[additional_column_index]
                 linked_columns.append(linked_column)
 
             update_as_multi_column(
                 expected_patterns,
                 cleaned_column_name,
                 pattern_index,
                 expected_header,
@@ -341,57 +354,57 @@
     return headers
 
 
 def update_message(messages, column_index, message, column):
     if not message.detail:
         column_message = " ".join(
             [
-                f"Column {(column.columnIndex + 1):03}: '{column.columnCategory}' column",
-                f"column name: '{column.columnHeader}'",
+                f"Column {(column.column_index + 1):03}: '{column.column_category}' column",
+                f"column name: '{column.column_header}'",
             ]
         )
         message.detail = column_message
     if not message.short:
-        message.short = f"'{column.columnCategory}' column: '{column.columnHeader}'"
+        message.short = f"'{column.column_category}' column: '{column.column_header}'"
     message.column = str(column_index)
     messages.append(message)
 
 
 def update_as_multi_column(
     expected_patterns,
     cleaned_column_name,
     pattern_index,
     expected_header,
     message: ParserMessage,
     column: IsaTableColumn,
 ):
     if expected_header:
-        column.columnSearchPattern = expected_patterns[pattern_index][0]
-        column.columnCategory = expected_patterns[pattern_index][1]
-        column.columnPrefix = expected_patterns[pattern_index][1]
+        column.column_search_pattern = expected_patterns[pattern_index][0]
+        column.column_category = expected_patterns[pattern_index][1]
+        column.column_prefix = expected_patterns[pattern_index][1]
     else:
-        column.columnCategory = "Undefined"
+        column.column_category = "Undefined"
         message.type = ParserMessageType.INFO
         message.short = f"Multi column '{cleaned_column_name}' is not in expected column list."
 
 
 def update_as_invalid_column(
     expected_patterns,
     cleaned_column_name,
     pattern_index,
     expected_header,
     message: ParserMessage,
     column: IsaTableColumn,
 ):
     if expected_header:
-        column.columnSearchPattern = expected_patterns[pattern_index][0]
-        column.columnPrefix = expected_patterns[pattern_index][1]
-        column.columnCategory = expected_patterns[pattern_index][1]
+        column.column_search_pattern = expected_patterns[pattern_index][0]
+        column.column_prefix = expected_patterns[pattern_index][1]
+        column.column_category = expected_patterns[pattern_index][1]
     else:
-        column.columnCategory = "Invalid"
+        column.column_category = "Invalid"
         message.type = ParserMessageType.CRITICAL
         message.short = (
             f"Multi column '{cleaned_column_name}'"
             + " has invalid or unordered additional headers."
         )
 
 
@@ -400,19 +413,19 @@
     cleaned_column_name,
     pattern_index,
     expected_header,
     message: ParserMessage,
     column: IsaTableColumn,
 ):
     if expected_header:
-        column.columnSearchPattern = expected_patterns[pattern_index][0]
-        column.columnCategory = expected_patterns[pattern_index][1]
-        column.columnPrefix = expected_patterns[pattern_index][1]
+        column.column_search_pattern = expected_patterns[pattern_index][0]
+        column.column_category = expected_patterns[pattern_index][1]
+        column.column_prefix = expected_patterns[pattern_index][1]
     else:
-        column.columnCategory = "Undefined"
+        column.column_category = "Undefined"
         message.type = ParserMessageType.INFO
         message.short = f"Single column '{cleaned_column_name}' is not in expected column list."
 
 
 def define_column_structure(column_index, columns):
     column_is_additional = False
     for additional_column_pattern in multiple_columns_additional_header_patterns:
```

### Comparing `metabolights_utils-0.9.1/pyproject.toml` & `metabolights_utils-0.9.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabolights-utils"
-version = "0.9.1"
+version = "0.9.2"
 description = "Metabolights common models, utility methods and classes for python-based Metabolights projects."
 authors = ["Ozgur Yurekten <ozgur@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "metabolights_utils"}]
 license = "Apache-2.0"
 homepage = "https://github.com/EBI-Metabolights"
 repository = "https://github.com/EBI-Metabolights/metabolights-utils"
@@ -17,16 +17,15 @@
     "Topic :: Scientific/Engineering :: Bio-Informatics"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.9"
 psycopg2-binary = ">=2.8"
 pydantic = "1.10.11"
-pandas = "0.25.3"
-numpy = "1.18.2"
+pyhumps = "^3.8.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 flake8-bugbear = "^23.7.10"
```

