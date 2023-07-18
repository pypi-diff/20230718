# Comparing `tmp/hermessplitter-3.1.1-py3-none-any.whl.zip` & `tmp/hermessplitter-3.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 13990 bytes, number of entries: 20
+Zip file size: 13995 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-24 13:22 hermessplitter/__init__.py
 -rw-rw-rw-  2.0 fat     4260 b- defN 22-Jul-14 10:48 hermessplitter/functions.py
--rw-rw-rw-  2.0 fat    10505 b- defN 23-Jul-11 07:59 hermessplitter/main.py
+-rw-rw-rw-  2.0 fat    10515 b- defN 23-Jul-18 08:00 hermessplitter/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Mar-21 07:21 hermessplitter/db/__init__.py
 -rw-rw-rw-  2.0 fat     5952 b- defN 22-Sep-21 10:54 hermessplitter/db/db_funcs.py
 -rw-rw-rw-  2.0 fat      667 b- defN 23-Mar-07 06:56 hermessplitter/db/init_db.py
 -rw-rw-rw-  2.0 fat     2521 b- defN 22-Jul-14 10:31 hermessplitter/db/tables.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Mar-21 10:13 hermessplitter/db/tests/__init__.py
 -rw-rw-rw-  2.0 fat     2639 b- defN 22-Jun-20 05:53 hermessplitter/db/tests/db_funcs_test.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Apr-08 04:12 hermessplitter/fast_api/__init__.py
 -rw-rw-rw-  2.0 fat     2209 b- defN 22-Apr-08 04:37 hermessplitter/fast_api/functions.py
 -rw-rw-rw-  2.0 fat     2630 b- defN 22-Sep-20 11:08 hermessplitter/fast_api/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-25 12:23 hermessplitter/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1246 b- defN 22-Apr-25 08:02 hermessplitter/tests/hermes_activate_tests.py
 -rw-rw-rw-  2.0 fat      527 b- defN 22-Mar-21 12:51 hermessplitter/tests/test_functions.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-11 09:07 hermessplitter-3.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      812 b- defN 23-Jul-11 09:07 hermessplitter-3.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 09:07 hermessplitter-3.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-11 09:07 hermessplitter-3.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1739 b- defN 23-Jul-11 09:07 hermessplitter-3.1.1.dist-info/RECORD
-20 files, 36905 bytes uncompressed, 11100 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-18 08:01 hermessplitter-3.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      812 b- defN 23-Jul-18 08:01 hermessplitter-3.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 08:01 hermessplitter-3.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-18 08:01 hermessplitter-3.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1739 b- defN 23-Jul-18 08:01 hermessplitter-3.1.2.dist-info/RECORD
+20 files, 36915 bytes uncompressed, 11105 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: hermessplitter/tests/hermes_activate_tests.py
 Comment: 
 
 Filename: hermessplitter/tests/test_functions.py
 Comment: 
 
-Filename: hermessplitter-3.1.1.dist-info/LICENSE
+Filename: hermessplitter-3.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: hermessplitter-3.1.1.dist-info/METADATA
+Filename: hermessplitter-3.1.2.dist-info/METADATA
 Comment: 
 
-Filename: hermessplitter-3.1.1.dist-info/WHEEL
+Filename: hermessplitter-3.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: hermessplitter-3.1.1.dist-info/top_level.txt
+Filename: hermessplitter-3.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hermessplitter-3.1.1.dist-info/RECORD
+Filename: hermessplitter-3.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hermessplitter/main.py

```diff
@@ -54,15 +54,15 @@
             return
         super().make_new_record(car_number, carrier, record_id)
         self.set_status(True)
         self.activate(carnum=car_number, record_id=record_id,
                       client=carrier)
 
     def make_final_record(self, weight, record_id):
-        self.make_log_hermes_db(weight, record_id)
+        self.make_log_hermes_db(weight, record_id=record_id)
 
     def turn_off_logging(self):
         self.blocked = False
         self.set_status(False)
 
     def activate(self, carnum, record_id, client=None):
         """ Активировать HERMES """
```

## Comparing `hermessplitter-3.1.1.dist-info/LICENSE` & `hermessplitter-3.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hermessplitter-3.1.1.dist-info/METADATA` & `hermessplitter-3.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermessplitter
-Version: 3.1.1
+Version: 3.1.2
 Author: punchyarchy
 Author-email: ksmdrmvscthny@gmail.com
 License-File: LICENSE
 Requires-Dist: SQLAlchemy (==1.4.29)
 Requires-Dist: ws-one (==1.12.41)
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
```

## Comparing `hermessplitter-3.1.1.dist-info/RECORD` & `hermessplitter-3.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 hermessplitter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hermessplitter/functions.py,sha256=6A9Y7RL1wOrQ-d_hapT50mmF-RXRArWbvCltFwKBUQA,4260
-hermessplitter/main.py,sha256=wATJhKVwYNmVbl5qzsVR6FJkh0L1tm4-Pdt_KeMmLjo,10505
+hermessplitter/main.py,sha256=iCsDTFmp3poLB_ddLQEN8s4h7WNoVJBTvCh_lZh-E5A,10515
 hermessplitter/db/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hermessplitter/db/db_funcs.py,sha256=MpaTF2THXVnvt_Yk1k97KGhsHL_Zzmn3Ieiozv2-aPc,5952
 hermessplitter/db/init_db.py,sha256=9BKEwAcjt5dCURQnAP2fx4MgNR9oXUT1htgFEVpeMg0,667
 hermessplitter/db/tables.py,sha256=3B4MvCSp2qe0JyB4e2KAHwwNtQkKOU61Pl8KmGbuTp0,2521
 hermessplitter/db/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hermessplitter/db/tests/db_funcs_test.py,sha256=um5hCpGsCaX59GYHjeeatSpRpl5YzWhAAeL5CKlLJnI,2639
 hermessplitter/fast_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hermessplitter/fast_api/functions.py,sha256=sJ_WzdgdmYoqCQZrgVBp_EdtKGNbnY0YayC7TIBc7h0,2209
 hermessplitter/fast_api/main.py,sha256=oPcoJmUynz72RtNCu0uuQc6LZ0gjN1W7UWlEthe-cUs,2630
 hermessplitter/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hermessplitter/tests/hermes_activate_tests.py,sha256=RGqzkPxSQTSK5wkkXj68aBsM-vrSa79B6u4Oz8RtX_s,1246
 hermessplitter/tests/test_functions.py,sha256=mZd3MF_VSLYmGqh6s4_ML6vvMVrVotOxa54G5AnDYdk,527
-hermessplitter-3.1.1.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-hermessplitter-3.1.1.dist-info/METADATA,sha256=TEd6NKo__K4jw_xbTjP-CSDvV-Bdr-j9cDx84gC3-_k,812
-hermessplitter-3.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hermessplitter-3.1.1.dist-info/top_level.txt,sha256=-irUC62Hn3T0w6CMiftA9yscS2o58MvzLskpUJtx7zI,15
-hermessplitter-3.1.1.dist-info/RECORD,,
+hermessplitter-3.1.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+hermessplitter-3.1.2.dist-info/METADATA,sha256=uwckltZc0LPZYmVSwvolhVSl1AyqthHPJPpN-GSm2BU,812
+hermessplitter-3.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hermessplitter-3.1.2.dist-info/top_level.txt,sha256=-irUC62Hn3T0w6CMiftA9yscS2o58MvzLskpUJtx7zI,15
+hermessplitter-3.1.2.dist-info/RECORD,,
```

