# Comparing `tmp/python_shinkansen-0.7.0.tar.gz` & `tmp/python_shinkansen-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_shinkansen-0.7.0.tar", max compression
+gzip compressed data, was "python_shinkansen-0.7.1.tar", max compression
```

## Comparing `python_shinkansen-0.7.0.tar` & `python_shinkansen-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      519 2023-06-05 05:46:51.804149 python_shinkansen-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-05 05:46:51.804292 python_shinkansen-0.7.0/shinkansen/__init__.py
--rw-r--r--   0        0        0     3904 2022-10-25 19:58:12.923345 python_shinkansen-0.7.0/shinkansen/common.py
--rw-r--r--   0        0        0     6478 2022-10-25 20:00:08.857266 python_shinkansen-0.7.0/shinkansen/jws.py
--rw-r--r--   0        0        0    12652 2023-06-05 05:39:29.564730 python_shinkansen-0.7.0/shinkansen/payins.py
--rw-r--r--   0        0        0    10203 2023-06-05 04:29:18.480681 python_shinkansen-0.7.0/shinkansen/payouts.py
--rw-r--r--   0        0        0     7818 2023-06-05 04:17:49.043149 python_shinkansen-0.7.0/shinkansen/responses.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 python_shinkansen-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      519 2023-07-17 22:02:17.185425 python_shinkansen-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-17 22:02:22.878807 python_shinkansen-0.7.1/shinkansen/__init__.py
+-rw-r--r--   0        0        0     3904 2022-10-25 19:58:12.923345 python_shinkansen-0.7.1/shinkansen/common.py
+-rw-r--r--   0        0        0     6478 2022-10-25 20:00:08.857266 python_shinkansen-0.7.1/shinkansen/jws.py
+-rw-r--r--   0        0        0    12652 2023-06-05 05:39:29.564730 python_shinkansen-0.7.1/shinkansen/payins.py
+-rw-r--r--   0        0        0    10245 2023-07-17 22:00:50.066362 python_shinkansen-0.7.1/shinkansen/payouts.py
+-rw-r--r--   0        0        0     7818 2023-06-05 04:17:49.043149 python_shinkansen-0.7.1/shinkansen/responses.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 python_shinkansen-0.7.1/PKG-INFO
```

### Comparing `python_shinkansen-0.7.0/pyproject.toml` & `python_shinkansen-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "python-shinkansen"
 packages = [
     {include = "shinkansen"}
 ]
-version = "0.7.0"
+version = "0.7.1"
 description = "Python helpers for Shinkansen"
 authors = ["Leonardo Soto M. <leo.soto@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 jwcrypto = "^1.4.0"
 cryptography = "^41.0.0"
```

### Comparing `python_shinkansen-0.7.0/shinkansen/common.py` & `python_shinkansen-0.7.1/shinkansen/common.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.7.0/shinkansen/jws.py` & `python_shinkansen-0.7.1/shinkansen/jws.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.7.0/shinkansen/payins.py` & `python_shinkansen-0.7.1/shinkansen/payins.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.7.0/shinkansen/payouts.py` & `python_shinkansen-0.7.1/shinkansen/payouts.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,31 +219,36 @@
                     ),
                     creditor=PayoutCreditor(
                         name=t["creditor"]["name"],
                         identification=PersonId(
                             id_schema=t["creditor"]["identification"]["id_schema"],
                             id=t["creditor"]["identification"]["id"],
                         ),
-                        financial_institution=FinancialInstitution(
-                            fin_id_schema=t["creditor"]["financial_institution"][
-                                "fin_id_schema"
-                            ],
-                            fin_id=t["creditor"]["financial_institution"]["fin_id"],
+                        financial_institution=cls._optional_fi(
+                            t["creditor"].get("financial_institution")
                         ),
                         account=t["creditor"]["account"],
                         account_type=t["creditor"]["account_type"],
                         email=t["creditor"]["email"],
                     ),
                     execution_date=t["execution_date"],
                     transaction_id=t["transaction_id"],
                 )
                 for t in json_dict["document"]["transactions"]
             ],
         )
 
+    @classmethod
+    def _optional_fi(self, d: dict):
+        if d is None:
+            return None
+        return FinancialInstitution(
+            fin_id_schema=d.get("fin_id_schema"), fin_id=d.get("fin_id")
+        )
+
     @property
     def id(self) -> str:
         """Returns the ID of the message"""
         return self.header.message_id
 
     def signature(
         self,
```

### Comparing `python_shinkansen-0.7.0/shinkansen/responses.py` & `python_shinkansen-0.7.1/shinkansen/responses.py`

 * *Files identical despite different names*

### Comparing `python_shinkansen-0.7.0/PKG-INFO` & `python_shinkansen-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-shinkansen
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python helpers for Shinkansen
 Author: Leonardo Soto M.
 Author-email: leo.soto@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

