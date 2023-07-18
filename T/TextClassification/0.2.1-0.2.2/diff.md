# Comparing `tmp/TextClassification-0.2.1-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.2.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8398 bytes, number of entries: 9
+Zip file size: 8416 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
--rw-rw-rw-  2.0 fat     3649 b- defN 23-Jul-18 09:11 text_classification/image_classification.py
+-rw-rw-rw-  2.0 fat     3688 b- defN 23-Jul-18 09:20 text_classification/image_classification.py
 -rw-rw-rw-  2.0 fat     5718 b- defN 23-Jul-17 14:57 text_classification/multiple_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     4110 b- defN 23-Jul-18 09:12 TextClassification-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 09:12 TextClassification-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 09:12 TextClassification-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 09:12 TextClassification-0.2.1.dist-info/RECORD
-9 files, 20790 bytes uncompressed, 6936 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 fat     4110 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/RECORD
+9 files, 20829 bytes uncompressed, 6954 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: text_classification/multiple_classification.py
 Comment: 
 
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.2.1.dist-info/METADATA
+Filename: TextClassification-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.2.1.dist-info/WHEEL
+Filename: TextClassification-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.2.1.dist-info/top_level.txt
+Filename: TextClassification-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.2.1.dist-info/RECORD
+Filename: TextClassification-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text_classification/image_classification.py

```diff
@@ -1,8 +1,8 @@
-from transformers import AutoImageProcessor, AutoModelForImageClassification, Trainer, TrainingArguments, pipeline
+from transformers import AutoImageProcessor, AutoModelForImageClassification, Trainer, TrainingArguments, pipeline,DefaultDataCollator
 import numpy as np
 
 class ImageClassifier:
     def __init__(self, checkpoint, data_dir, test_size=0.2, num_epochs=3, batch_size=16):
         self.data_dir = data_dir
         self.test_size = test_size
         self.num_epochs = num_epochs
@@ -46,15 +46,15 @@
         return transforms
 
     def train(self):
         dataset = self.load_dataset()
         transforms = self.create_transforms()
         dataset = dataset.with_transform(transforms)
 
-        data_collator = DefaultDataCollator()
+        data_collator = DefaultDataCollator(return_tensors="tf")
 
         model = AutoModelForImageClassification.from_pretrained(
             self.checkpoint,
             num_labels=len(self.labels),
             id2label=self.id2label,
             label2id=self.label2id,
         )
```

## Comparing `TextClassification-0.2.1.dist-info/METADATA` & `TextClassification-0.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextClassification
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create Text Classification Fine-Tunning Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: transformers,datasets
 Classifier: Programming Language :: Python :: 3
```

## Comparing `TextClassification-0.2.1.dist-info/RECORD` & `TextClassification-0.2.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-text_classification/image_classification.py,sha256=szRQIHvpjNZ-wcrMGk2pGPHDPU4I2Ul6w9rJdYZNmEE,3649
+text_classification/image_classification.py,sha256=eKm7g57HDi4p_vfWB2v38BHMbL7HpFlhVMiZs-WT4fE,3688
 text_classification/multiple_classification.py,sha256=j_WumOQly-AvEbZEtahrVqyKnZF-laoPGXLgobVoLiY,5718
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.2.1.dist-info/METADATA,sha256=6a4TKklCiCDfmn-aViPOUJT6K4DnZutry08O0D2t0Oc,4110
-TextClassification-0.2.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.2.1.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.2.1.dist-info/RECORD,,
+TextClassification-0.2.2.dist-info/METADATA,sha256=NMqqxc8q08IH1dSSWrHMtE-aZGASHTdxBRTod71nQV4,4110
+TextClassification-0.2.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.2.2.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.2.2.dist-info/RECORD,,
```

