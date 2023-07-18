# Comparing `tmp/work_helper-0.1.2.tar.gz` & `tmp/work_helper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work_helper-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "work_helper-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `work_helper-0.1.2.tar` & `work_helper-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3299 2023-07-06 09:22:47.552925 work_helper-0.1.2/.gitignore
--rw-r--r--   0        0        0      137 2023-05-26 09:35:55.498254 work_helper-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     1096 2023-05-26 05:27:24.425923 work_helper-0.1.2/LICENSE
--rw-r--r--   0        0        0      587 2023-07-06 09:22:47.552925 work_helper-0.1.2/helper/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:19:44.138475 work_helper-0.1.2/helper/base/__init__.py
--rw-r--r--   0        0        0      964 2023-05-26 09:37:12.856686 work_helper-0.1.2/helper/base/logger.py
--rw-r--r--   0        0        0     6082 2023-07-06 10:18:17.669528 work_helper-0.1.2/helper/ddl.py
--rw-r--r--   0        0        0     7470 2023-07-06 09:22:47.553805 work_helper-0.1.2/helper/etl.py
--rw-r--r--   0        0        0     2781 2023-06-29 05:45:56.244212 work_helper-0.1.2/helper/hello.py
--rw-r--r--   0        0        0     2425 2023-06-13 09:22:21.003065 work_helper-0.1.2/helper/helm.py
--rw-r--r--   0        0        0     1787 2023-06-16 08:50:08.249839 work_helper-0.1.2/helper/pack.py
--rwxr-xr-x   0        0        0       31 2023-07-07 08:28:54.281342 work_helper-0.1.2/publish.bat
--rw-r--r--   0        0        0      586 2023-07-07 08:54:34.601578 work_helper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    28606 2023-07-06 08:51:45.579410 work_helper-0.1.2/samples/ddl.sample.xlsx
--rw-r--r--   0        0        0    64824 2023-07-06 08:44:39.364263 work_helper-0.1.2/samples/etl.sample.xlsx
--rw-r--r--   0        0        0      228 1970-01-01 00:00:00.000000 work_helper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3299 2023-07-06 09:22:47.552925 work_helper-0.1.3/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-26 09:35:55.498254 work_helper-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1096 2023-05-26 05:27:24.425923 work_helper-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1028 2023-07-18 03:54:36.061632 work_helper-0.1.3/helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:19:44.138475 work_helper-0.1.3/helper/base/__init__.py
+-rw-r--r--   0        0        0      964 2023-05-26 09:37:12.856686 work_helper-0.1.3/helper/base/logger.py
+-rw-r--r--   0        0        0     6823 2023-07-11 02:47:38.373322 work_helper-0.1.3/helper/ddl.py
+-rw-r--r--   0        0        0     7590 2023-07-11 03:22:11.612966 work_helper-0.1.3/helper/etl.py
+-rw-r--r--   0        0        0     2781 2023-06-29 05:45:56.244212 work_helper-0.1.3/helper/hello.py
+-rw-r--r--   0        0        0     2425 2023-06-13 09:22:21.003065 work_helper-0.1.3/helper/helm.py
+-rw-r--r--   0        0        0     1787 2023-06-16 08:50:08.249839 work_helper-0.1.3/helper/pack.py
+-rwxr-xr-x   0        0        0       31 2023-07-07 08:28:54.281342 work_helper-0.1.3/publish.bat
+-rw-r--r--   0        0        0      586 2023-07-07 08:54:34.601578 work_helper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    28606 2023-07-06 08:51:45.579410 work_helper-0.1.3/samples/ddl.sample.xlsx
+-rw-r--r--   0        0        0    64824 2023-07-06 08:44:39.364263 work_helper-0.1.3/samples/etl.sample.xlsx
+-rw-r--r--   0        0        0      228 1970-01-01 00:00:00.000000 work_helper-0.1.3/PKG-INFO
```

### Comparing `work_helper-0.1.2/.gitignore` & `work_helper-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/LICENSE` & `work_helper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/helper/base/logger.py` & `work_helper-0.1.3/helper/base/logger.py`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/helper/ddl.py` & `work_helper-0.1.3/helper/etl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,152 +1,192 @@
 import argparse
+from helper import EnhancedWriter
 from helper.base.logger import log
 from openpyxl import load_workbook, Workbook
 from openpyxl.worksheet.worksheet import Worksheet
 from openpyxl.cell.read_only import ReadOnlyCell
 import os
 from typing import Protocol
-from helper import EnhancedWriter
+from io import StringIO
 
-__version__ = "0.0.2"
+__version__ = "0.0.6"
 
 
 class Args(Protocol):
     file: str
-    lowercase: bool
+    dest: str
 
 
 class DataRow:
     def __init__(self, data) -> None:
         self.data = data
 
     def __getitem__(self, key):
         return self.data[key]
 
-    @property
-    def table_schema(self) -> str:
-        """表schema名"""
-        return self.data[0]
+    def is_main_table(self) -> bool:
+        return self.data[6] == "MAIN TABLE"
+
+    def is_join(self) -> bool:
+        return self.data[6] is not None and not self.is_main_table()
 
     @property
-    def table_name(self) -> str:
-        """表名"""
-        return self.data[2]
+    def join_type(self) -> str:
+        return self.data[6]
 
     @property
-    def table_cn_name(self) -> str:
-        """表中文名称"""
-        return self.data[1]
+    def source_table(self) -> str:
+        """源表名称"""
+        return self.data[10]
 
     @property
     def column_name(self) -> str:
-        """列名"""
-        return self.data[4]
+        """目标表列名"""
+        return self.data[0]
 
     @property
     def column_cn_name(self) -> str:
-        """中文列名"""
-        return self.data[3]
+        """目标表中文列名"""
+        return self.data[1]
 
     @property
-    def column_type(self) -> str:
+    def mapping_rule(self) -> str:
         """映射规则"""
-        return self.data[5]
+        return self.data[15]
 
     @property
-    def column_is_pk(self) -> bool:
-        """是否主键"""
-        return self.data[6] == "Y"
+    def source_table_id(self) -> str:
+        """源表别名"""
+        return self.data[9]
 
     @property
-    def column_null_str(self) -> str:
-        """是否非空字符串"""
-        if self.data[7] == "Y":
-            return "NOT NULL"
-        return "NULL"
+    def join_on_condition(self) -> str:
+        """JOIN表的ON条件"""
+        return self.data[7]
 
     @property
-    def column_default_value(self) -> str:
-        """默认值"""
-        return self.data[11]
+    def where_condition(self) -> str:
+        """主表行的SQL查询条件"""
+        return self.data[19]
 
 
 class DataGroup:
-    def __init__(self, group_id, title) -> None:
+    def __init__(self, group_id) -> None:
         self.data: list[DataRow] = []
         self.group_id = group_id
-        self.title = title
 
-    def get_primary_keys(self):
-        keys = filter(lambda x: x.column_is_pk, self.data)
-        return list(map(lambda x: x.column_name, keys))
+    def main_table(self):
+        return next(x for x in self.data if x.is_main_table())
 
     def write_sql(self, w: EnhancedWriter):
-        first_row = self.data[0]
-        w.writeln(
-            f"-- Table: {first_row.table_schema}.{first_row.table_name} {self.title}"
-        )
-        pks = self.get_primary_keys()
-        w.writeln(f"CREATE TABLE {first_row.table_schema}.{first_row.table_name} (")
+        w.write("SELECT\n")
         for i in range(len(self.data)):
             d = self.data[i]
-            w.write(f"    {d.column_name} {d.column_type} {d.column_null_str}")
-            if d.column_default_value is not None:
-                w.write(f" DEFAULT {d.column_default_value}")
-            if i < len(self.data) - 1 or len(pks) > 0:
+            w.write(f"    {d.mapping_rule} AS {d.column_name}")
+            if i < len(self.data) - 1:
                 w.write(",")
-            w.writeln(f"    -- {d.column_cn_name}")
-        if len(pks) > 0:
-            w.writeln(
-                f"    CONSTRAINT pk_{self.group_id} PRIMARY KEY ({','.join(pks)})"
-            )
+            w.write(f"    -- {d.column_cn_name}")
+            w.write("\n")
 
-        w.writeln(f");")
-
-        w.writeln(
-            f"COMMENT ON TABLE {first_row.table_schema}.{first_row.table_name} IS '{self.title}';"
-        )
-        for i in range(len(self.data)):
-            d = self.data[i]
-            w.writeln(
-                f"COMMENT ON COLUMN {d.table_schema}.{d.table_name}.{d.column_name} IS '{d.column_cn_name}';"
+        mt = self.main_table()
+        w.write(f"FROM {mt.source_table} {mt.source_table_id}\n")
+        for d in filter(lambda x: x.is_join(), self.data):
+            w.write(
+                f"{d.join_type} {d.source_table} {d.source_table_id} {d.join_on_condition}\n"
             )
+        w.write(f"{mt.where_condition};\n")
+
+    def __str__(self) -> str:
+        sio = StringIO()
+        self.write_sql(sio)
+        return sio.getvalue()
 
 
 class ModelFile:
     def __init__(self, sheet: Worksheet) -> None:
-
-        # self.source_tables = sheet[1]
-        # self.target_table_name = sheet["B4"].value
-        # self.target_table_chinese_name = sheet["B3"].value
-        # self.description = sheet["B5"].value
-        # self.target_table_type = None
-        # self.load_type = None
-        # self.logic_increment = None
-
         self.sheet_name = sheet.title
+        self.meta = []
+        for row in range(2, 12):
+            self.meta.append((sheet.cell(row, 1).value, sheet.cell(row, 2).value))
+
         groups = {}
 
-        for v in sheet.iter_rows(min_row=3, values_only=True):
-            if v[2] is not None:
-                gid = v[2]
+        for v in sheet.iter_rows(min_row=14, values_only=True):
+            if v[0] is not None:
+                gid = v[5]
                 if gid not in groups:
-                    groups[gid] = DataGroup(gid, sheet.title)
+                    groups[gid] = DataGroup(gid)
                 group: DataGroup = groups[gid]
                 group.data.append(DataRow(v))
 
         self.data: list[DataGroup] = list(groups.values())
 
-    def generate_ddl_file(self, writer: EnhancedWriter, args: Args):
+    @property
+    def target_table_name(self) -> str:
+        return self.meta[2][1]
+
+    def table_info(self):
+        array = self.target_table_name.split(".")
+        if len(array) == 1:
+            return None, self.target_table_name
+        return array[0], array[1]
+
+    def write_meta_comments(self, writer: EnhancedWriter):
+        for kv in self.meta:
+            key = str(kv[0]).replace("\n", " ")
+            vs = str(kv[1]).split("\n")
+            writer.write(f"-- {key.ljust(10,chr(12288))}: {vs[0]}\n")
+            if len(vs) > 1:
+                for v in vs[1:]:
+                    writer.write(f"-- {''.ljust(10,chr(12288))}  {v}\n")
+
+    def write_content(self, writer: EnhancedWriter):
+        self.write_meta_comments(writer)
+        writer.writeln()
+        self.write_postgre_procedure(writer)
+
+    def write_postgre_procedure(self, writer: EnhancedWriter):
+        info = self.table_info()
+        function_name = "dcx_" + info[1]
+        if info[0] is not None:
+            function_name = f"{info[0]}.dcx_{info[1]}"
+        writer.writeln(
+            f"CREATE OR REPLACE FUNCTION {function_name}(IN p_date int4, OUT p_srccnt int4, OUT p_dstcnt int4) AS $$"
+        )
+        writer.writeln("BEGIN")
+        writer.writeln()
+
+        temp_table_name = "tmp_" + info[1]
+        writer.writeln(f"DROP TABLE IF EXISTS {temp_table_name};")
+        writer.writeln(
+            f"CREATE TEMPORARY TABLE {temp_table_name} AS (SELECT * FROM {self.target_table_name} WHERE 1=2);"
+        )
         for group in self.data:
             if group.group_id is None:
                 continue
-            group.write_sql(writer)
-            writer.writeln()
-            log.info(f"生成DDL脚本:{group.group_id}")
+            writer.writeln(f"-- Group {group.group_id}")
+            writer.writeln(f"INSERT INTO {temp_table_name}")
+            writer.writeln(group, 4)
+
+        writer.writeln(f"DELETE FROM {self.target_table_name} WHERE dcdate=p_date;")
+        writer.writeln(
+            f"INSERT INTO {self.target_table_name} SELECT * FROM {temp_table_name};"
+        )
+        writer.writeln()
+        writer.writeln(f"SELECT count(1) INTO p_srccnt FROM {temp_table_name};")
+        writer.writeln("p_dstcnt := p_srccnt;")
+        writer.writeln()
+        writer.writeln("END;")
+        writer.writeln("$$ LANGUAGE plpgsql;")
+
+    def generate_etl_file(self, args: Args):
+        file = os.path.join(args.dest, f"{self.target_table_name}.sql")
+        with EnhancedWriter(file) as writer:
+            self.write_content(writer)
+        log.info(f"生成脚本：{self.sheet_name} > {file}")
 
 
 def find_model_file():
     cwd = os.getcwd()
     entrys = os.listdir(cwd)
 
     for entry in entrys:
@@ -157,18 +197,20 @@
             and not entry.startswith("~$")
         ):
             return file
     return None
 
 
 def is_model_sheet(sheet: Worksheet):
-    v: ReadOnlyCell = sheet["A2"]
-    if v.value == "Schema":
-        return True
-    return False
+    if sheet.max_row < 13:
+        return False
+    A13: ReadOnlyCell = sheet["A13"]
+    if A13.value != "目标字段英文名":
+        return False
+    return True
 
 
 def load_model_file(args: Args):
 
     book: Workbook = load_workbook(
         args.file, read_only=True, data_only=True, keep_vba=False
     )
@@ -178,34 +220,33 @@
         if is_model_sheet(sheet):
             model = ModelFile(sheet)
             yield model
 
 
 def main():
 
-    parser = argparse.ArgumentParser(description="DDL脚本生成程序")
+    parser = argparse.ArgumentParser(description="ETL脚本生成程序")
     parser.add_argument(
         "--version", action="version", version=__version__, help="显示程序版本号"
     )
-    parser.add_argument("file", type=str, nargs="?", default=None, help="Excel字典文件")
-    parser.add_argument("--lowercase", action="store_false", help="将表名和字段名强制转换为小写")
+    parser.add_argument("file", type=str, nargs="?", default=None, help="Excel模型文件")
+    parser.add_argument("--dest", default=".", type=str, help="设定文件生成目录")
 
     args: Args = parser.parse_args()
 
     log.info(f"{parser.description} {__version__}")
 
     if args.file is None:
         args.file = find_model_file()
 
     if args.file is None:
-        log.error("未找到Excel字典文件")
+        log.error("未找到Excel模型文件")
         exit(1)
 
-    file = f"{args.file}.sql"
-    with open(file, mode="w", encoding="utf-8") as writer:
-        e_writer = EnhancedWriter(writer)
-        for model in load_model_file(args):
-            model.generate_ddl_file(e_writer, args)
+    os.makedirs(args.dest, exist_ok=True)
+
+    for model in load_model_file(args):
+        model.generate_etl_file(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `work_helper-0.1.2/helper/hello.py` & `work_helper-0.1.3/helper/hello.py`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/helper/helm.py` & `work_helper-0.1.3/helper/helm.py`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/helper/pack.py` & `work_helper-0.1.3/helper/pack.py`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/pyproject.toml` & `work_helper-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/samples/ddl.sample.xlsx` & `work_helper-0.1.3/samples/ddl.sample.xlsx`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.2/samples/etl.sample.xlsx` & `work_helper-0.1.3/samples/etl.sample.xlsx`

 * *Files identical despite different names*

