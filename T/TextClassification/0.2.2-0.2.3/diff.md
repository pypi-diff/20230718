# Comparing `tmp/TextClassification-0.2.2-py2.py3-none-any.whl.zip` & `tmp/TextClassification-0.2.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8416 bytes, number of entries: 9
+Zip file size: 8425 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 text_classification/__init__.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 14:01 text_classification/binary_classification.py
--rw-rw-rw-  2.0 fat     3688 b- defN 23-Jul-18 09:20 text_classification/image_classification.py
+-rw-rw-rw-  2.0 fat     3762 b- defN 23-Jul-18 09:37 text_classification/image_classification.py
 -rw-rw-rw-  2.0 fat     5718 b- defN 23-Jul-17 14:57 text_classification/multiple_classification.py
 -rw-rw-rw-  2.0 fat     3176 b- defN 23-Jul-17 13:45 text_classification/text_classification.py
--rw-rw-rw-  2.0 fat     4110 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 09:20 TextClassification-0.2.2.dist-info/RECORD
-9 files, 20829 bytes uncompressed, 6954 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 fat     4110 b- defN 23-Jul-18 09:37 TextClassification-0.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 09:37 TextClassification-0.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 09:37 TextClassification-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      831 b- defN 23-Jul-18 09:37 TextClassification-0.2.3.dist-info/RECORD
+9 files, 20903 bytes uncompressed, 6963 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: text_classification/multiple_classification.py
 Comment: 
 
 Filename: text_classification/text_classification.py
 Comment: 
 
-Filename: TextClassification-0.2.2.dist-info/METADATA
+Filename: TextClassification-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: TextClassification-0.2.2.dist-info/WHEEL
+Filename: TextClassification-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: TextClassification-0.2.2.dist-info/top_level.txt
+Filename: TextClassification-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: TextClassification-0.2.2.dist-info/RECORD
+Filename: TextClassification-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## text_classification/image_classification.py

```diff
@@ -7,29 +7,30 @@
         self.test_size = test_size
         self.num_epochs = num_epochs
         self.batch_size = batch_size
         self.checkpoint = checkpoint
         self.labels = None
         self.label2id = {}
         self.id2label = {}
+    image_processor = AutoImageProcessor.from_pretrained(checkpoint)
 
     def load_dataset(self):
         from datasets import load_dataset
         dataset = load_dataset("imagefolder", data_dir=self.data_dir, split="train")
         dataset = dataset.train_test_split(test_size=self.test_size)
         self.labels = dataset["train"].features["label"].names
         for i, label in enumerate(self.labels):
             self.label2id[label] = str(i)
             self.id2label[str(i)] = label
         return dataset
     def compute_metrics(eval_pred):
         predictions, labels = eval_pred
         predictions = np.argmax(predictions, axis=1)
         return accuracy.compute(predictions=predictions, references=labels)
-
+    
     def create_transforms(self):
         from torchvision.transforms import RandomResizedCrop, Compose, Normalize, ToTensor
 
         image_processor = AutoImageProcessor.from_pretrained(self.checkpoint)
         normalize = Normalize(mean=image_processor.image_mean, std=image_processor.image_std)
         size = (
             image_processor.size["shortest_edge"]
```

## Comparing `TextClassification-0.2.2.dist-info/METADATA` & `TextClassification-0.2.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TextClassification
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create Text Classification Fine-Tunning Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: transformers,datasets
 Classifier: Programming Language :: Python :: 3
```

## Comparing `TextClassification-0.2.2.dist-info/RECORD` & `TextClassification-0.2.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 text_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 text_classification/binary_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-text_classification/image_classification.py,sha256=eKm7g57HDi4p_vfWB2v38BHMbL7HpFlhVMiZs-WT4fE,3688
+text_classification/image_classification.py,sha256=SMwomBvBWT6kJ44H-zQLGFGahzzwJet9Exlqtw5T0hM,3762
 text_classification/multiple_classification.py,sha256=j_WumOQly-AvEbZEtahrVqyKnZF-laoPGXLgobVoLiY,5718
 text_classification/text_classification.py,sha256=cLU3etNXV1FZ0ajpPGvpKGk00CcWdMB73zgEwoeD3jo,3176
-TextClassification-0.2.2.dist-info/METADATA,sha256=NMqqxc8q08IH1dSSWrHMtE-aZGASHTdxBRTod71nQV4,4110
-TextClassification-0.2.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-TextClassification-0.2.2.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
-TextClassification-0.2.2.dist-info/RECORD,,
+TextClassification-0.2.3.dist-info/METADATA,sha256=8BlRs7kzbFBxTswqmiab87g5tUEkWM960ehzPw1ZFeI,4110
+TextClassification-0.2.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+TextClassification-0.2.3.dist-info/top_level.txt,sha256=JlmvPyi7tlMLXeNz2B0RUE96UYbtdgZxWUrZCo8VOgQ,20
+TextClassification-0.2.3.dist-info/RECORD,,
```

