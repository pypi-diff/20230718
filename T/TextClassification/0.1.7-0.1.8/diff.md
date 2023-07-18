# Comparing `tmp/TextClassification-0.1.7-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 6391 bytes, number of entries: 8
+Zip file size: 8547 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
+-rw-rw-rw-  2.0 fat     4643 b- defN 23-Jul-18 06:26 text_classification/image_classification.py
 -rw-rw-rw-  2.0 fat     5718 b- defN 23-Jul-17 14:57 text_classification/multiple_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     1861 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 23-Jul-17 14:57 TextClassification-0.1.7.dist-info/RECORD
-8 files, 14792 bytes uncompressed, 5091 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     4085 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/RECORD
+9 files, 21759 bytes uncompressed, 7085 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: text_classification/__init__.py
 Comment: 
 
 Filename: text_classification/binary_classification.py
 Comment: 
 
+Filename: text_classification/image_classification.py
+Comment: 
+
 Filename: text_classification/multiple_classification.py
 Comment: 
 
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.1.7.dist-info/METADATA
+Filename: TextClassification-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.1.7.dist-info/WHEEL
+Filename: TextClassification-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.1.7.dist-info/top_level.txt
+Filename: TextClassification-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.1.7.dist-info/RECORD
+Filename: TextClassification-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `TextClassification-0.1.7.dist-info/RECORD` & `TextClassification-0.1.8.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
+text_classification/image_classification.py,sha256=A7Gwjk__PENoNdcIMctMSLjHbnLp4GRBorO29K0OycQ,4643
 text_classification/multiple_classification.py,sha256=j_WumOQly-AvEbZEtahrVqyKnZF-laoPGXLgobVoLiY,5718
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.1.7.dist-info/METADATA,sha256=hhmYJNeYaq4pEcvdnns-ztyO18jZ7d9q6IRPD0CTjRo,1861
-TextClassification-0.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.1.7.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.1.7.dist-info/RECORD,,
+TextClassification-0.1.8.dist-info/METADATA,sha256=ligJ-aOb6mJb7A380xdis5dHYvVATgxEhQNewiBxKAM,4085
+TextClassification-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.1.8.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.1.8.dist-info/RECORD,,
```

