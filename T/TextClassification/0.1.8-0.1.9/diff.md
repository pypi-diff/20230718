# Comparing `tmp/TextClassification-0.1.8-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 8547 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
--rw-rw-rw-  2.0 fat     4643 b- defN 23-Jul-18 06:26 text_classification/image_classification.py
+-rw-rw-rw-  2.0 fat     4644 b- defN 23-Jul-18 06:50 text_classification/image_classification.py
 -rw-rw-rw-  2.0 fat     5718 b- defN 23-Jul-17 14:57 text_classification/multiple_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     4085 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 06:27 TextClassification-0.1.8.dist-info/RECORD
-9 files, 21759 bytes uncompressed, 7085 bytes compressed:  67.4%
+-rw-rw-rw-  2.0 fat     4110 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 06:50 TextClassification-0.1.9.dist-info/RECORD
+9 files, 21785 bytes uncompressed, 7085 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: text_classification/multiple_classification.py
 Comment: 
 
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.1.8.dist-info/METADATA
+Filename: TextClassification-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.1.8.dist-info/WHEEL
+Filename: TextClassification-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.1.8.dist-info/top_level.txt
+Filename: TextClassification-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.1.8.dist-info/RECORD
+Filename: TextClassification-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text_classification/image_classification.py

```diff
@@ -73,15 +73,15 @@
             gradient_accumulation_steps=gradient_accumulation_steps,
             per_device_eval_batch_size=per_device_eval_batch_size,
             num_train_epochs=num_train_epochs,
             warmup_ratio=warmup_ratio,
             logging_steps=logging_steps,
             load_best_model_at_end=True,
             metric_for_best_model="accuracy",
-            push_to_hub=True,
+           # push_to_hub=True,
         )
 
         self.data_collator = DefaultDataCollator()
         self.trainer = Trainer(
             model=self.model,
             args=training_args,
             data_collator=self.data_collator,
```

## Comparing `TextClassification-0.1.8.dist-info/METADATA` & `TextClassification-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: TextClassification
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create Text Classification Fine-Tunning Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: transformers,datasets
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: transformers (==4.27.0)
 Requires-Dist: datasets (==2.9)
+Requires-Dist: evaluate
 
 # Text Classification with NLP Models and Transformers
 
 ## Introduction
 This Python package provides a simple and efficient solution for text classification tasks using Natural Language Processing (NLP) models and Transformer-based encoder-decoder models. It supports both binary classification and multiple classification scenarios, allowing you to train, evaluate, and deploy state-of-the-art models for classifying text data.
 
 ## Features
```

## Comparing `TextClassification-0.1.8.dist-info/RECORD` & `TextClassification-0.1.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-text_classification/image_classification.py,sha256=A7Gwjk__PENoNdcIMctMSLjHbnLp4GRBorO29K0OycQ,4643
+text_classification/image_classification.py,sha256=hhVS-tDCUOuFTh-uwuuJPwQCg_7Q7VFz96CKiI4t-a4,4644
 text_classification/multiple_classification.py,sha256=j_WumOQly-AvEbZEtahrVqyKnZF-laoPGXLgobVoLiY,5718
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.1.8.dist-info/METADATA,sha256=ligJ-aOb6mJb7A380xdis5dHYvVATgxEhQNewiBxKAM,4085
-TextClassification-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.1.8.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.1.8.dist-info/RECORD,,
+TextClassification-0.1.9.dist-info/METADATA,sha256=UmZUqpezMuIV2xynXWDSnapTVJMJ7mMboI73AVJRiHU,4110
+TextClassification-0.1.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.1.9.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.1.9.dist-info/RECORD,,
```

