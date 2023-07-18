# Comparing `tmp/price2bq_mg-1.0.0.tar.gz` & `tmp/price2bq_mg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "price2bq_mg-1.0.0.tar", max compression
+gzip compressed data, was "price2bq_mg-1.0.1.tar", max compression
```

## Comparing `price2bq_mg-1.0.0.tar` & `price2bq_mg-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-06-05 15:21:35.669023 price2bq_mg-1.0.0/LICENSE
--rw-r--r--   0        0        0      160 2023-06-05 15:21:35.669095 price2bq_mg-1.0.0/README.md
--rw-r--r--   0        0        0     1329 2023-06-05 15:24:45.768508 price2bq_mg-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-05 15:21:35.669937 price2bq_mg-1.0.0/src/price2bq_mg/__init__.py
--rw-r--r--   0        0        0     8981 2023-06-05 15:24:45.595407 price2bq_mg-1.0.0/src/price2bq_mg/main.py
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 price2bq_mg-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-05 15:21:35.669023 price2bq_mg-1.0.1/LICENSE
+-rw-r--r--   0        0        0      160 2023-06-05 15:21:35.669095 price2bq_mg-1.0.1/README.md
+-rw-r--r--   0        0        0     1329 2023-07-18 07:46:39.974358 price2bq_mg-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-05 15:21:35.669937 price2bq_mg-1.0.1/src/price2bq_mg/__init__.py
+-rw-r--r--   0        0        0     8969 2023-07-18 07:43:57.873088 price2bq_mg-1.0.1/src/price2bq_mg/main.py
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 price2bq_mg-1.0.1/PKG-INFO
```

### Comparing `price2bq_mg-1.0.0/LICENSE` & `price2bq_mg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `price2bq_mg-1.0.0/pyproject.toml` & `price2bq_mg-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "price2bq_mg"
-version = "1.0.0"
+version = "1.0.1"
 description = "Экспорт файлов c площадок 'Яндекс Недвижимость', 'Авито' 'Циан' в BigQuery"
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.11"
 pandas = "^2"
```

### Comparing `price2bq_mg-1.0.0/src/price2bq_mg/main.py` & `price2bq_mg-1.0.1/src/price2bq_mg/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,18 @@
     bq = Client(bq_path_token, bq_project_id)
     bq.upload_table(df, bq_table, schema)
     return start_date, finish_date
 
 
 def prepare_cian(path_file: str) -> pd.DataFrame:
     df = pd.read_excel(path_file, sheet_name="Статистика звонков")
-    df = df.rename(columns={"Id": "id", "Дата": "call_datetime", "Номер пользователя": "incoming_number",
+    df = df.rename(columns={"Id": "id", "Дата": "call_datetime", "Входящий номер": "incoming_number",
                             "Подменный номер клиента": "substitute_client_number",
                             "Подменный номер застройщика": "replacement_builder_number",
-                            "Номер застройщика": "outgoing_number", "Название ЖК": "object", "Статус": "status",
+                            "Исходящий номер": "outgoing_number", "Название ЖК": "object", "Статус": "status",
                             "Разговор": "call_duration", "Тариф": "tariff", "Аукцион": "auction",
                             "Cписано в баллах": "written_in_points", "Тип": "type_of_call", "Тип лида": "type_of_lead",
                             "Сумма": "final_cost"})
     df["tariff"] = df["tariff"].replace({"\xa0": ""}, regex=True).astype(int)
     df["auction"] = df["auction"].replace({"\xa0": ""}, regex=True).astype(int)
     df["final_cost"] = df["final_cost"].replace({"\xa0": ""}, regex=True).astype(int)
     df["written_in_points"] = df["auction"].replace({"\xa0": ""}, regex=True).astype(int)
```

### Comparing `price2bq_mg-1.0.0/PKG-INFO` & `price2bq_mg-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: price2bq-mg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Экспорт файлов c площадок 'Яндекс Недвижимость', 'Авито' 'Циан' в BigQuery
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bq-easy-zfullio (>=1,<2)
```

