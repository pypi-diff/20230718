# Comparing `tmp/TextClassification-0.1.9-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8547 bytes, number of entries: 9
+Zip file size: 8552 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
--rw-rw-rw-  2.0 fat     4644 b- defN 23-Jul-18 06:50 text_classification/image_classification.py
+-rw-rw-rw-  2.0 fat     4646 b- defN 23-Jul-18 06:59 text_classification/image_classification.py
 -rw-rw-rw-  2.0 fat     5718 b- defN 23-Jul-17 14:57 text_classification/multiple_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     4110 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/RECORD
-9 files, 21785 bytes uncompressed, 7085 bytes compressed:  67.5%
+-rw-rw-rw-  2.0 fat     4110 b- defN 23-Jul-18 07:00 TextClassification-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 07:00 TextClassification-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 07:00 TextClassification-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 07:00 TextClassification-0.2.0.dist-info/RECORD
+9 files, 21787 bytes uncompressed, 7090 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: text_classification/multiple_classification.py
 Comment: 
 
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.1.9.dist-info/METADATA
+Filename: TextClassification-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.1.9.dist-info/WHEEL
+Filename: TextClassification-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.1.9.dist-info/top_level.txt
+Filename: TextClassification-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.1.9.dist-info/RECORD
+Filename: TextClassification-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text_classification/image_classification.py

```diff
@@ -90,16 +90,16 @@
             tokenizer=self.image_processor,
             compute_metrics=self.compute_metrics,
         )
 
     def train(self):
         self.trainer.train()
 
-    def push_to_hub(self):
-        self.trainer.push_to_hub()
+   # def push_to_hub(self):
+       # self.trainer.push_to_hub()
 
     def load_pipeline(self):
         self.tokenizer = self.image_processor
         self.model = AutoModelForImageClassification.from_pretrained("my_awesome_food_model")
         self.classifier = pipeline("image-classification", model=self.model)
 
     def infer(self, image):
```

## Comparing `TextClassification-0.1.9.dist-info/METADATA` & `TextClassification-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextClassification
-Version: 0.1.9
+Version: 0.2.0
 Summary: Create Text Classification Fine-Tunning Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: transformers,datasets
 Classifier: Programming Language :: Python :: 3
```

## Comparing `TextClassification-0.1.9.dist-info/RECORD` & `TextClassification-0.2.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-text_classification/image_classification.py,sha256=hhVS-tDCUOuFTh-uwuuJPwQCg_7Q7VFz96CKiI4t-a4,4644
+text_classification/image_classification.py,sha256=A1DB4wBhbQ16YdkeZT7ZeBA4gNHBY5gGk3a_d_F7ZHg,4646
 text_classification/multiple_classification.py,sha256=j_WumOQly-AvEbZEtahrVqyKnZF-laoPGXLgobVoLiY,5718
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.1.9.dist-info/METADATA,sha256=UmZUqpezMuIV2xynXWDSnapTVJMJ7mMboI73AVJRiHU,4110
-TextClassification-0.1.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.1.9.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.1.9.dist-info/RECORD,,
+TextClassification-0.2.0.dist-info/METADATA,sha256=bsotG1bK3D35Ns31bQmytIT1b7t3i3mNzbpSbdjLSOA,4110
+TextClassification-0.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.2.0.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.2.0.dist-info/RECORD,,
```

