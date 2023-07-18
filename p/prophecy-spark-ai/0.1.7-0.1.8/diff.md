# Comparing `tmp/prophecy_spark_ai-0.1.7-py3-none-any.whl.zip` & `tmp/prophecy_spark_ai-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10232 bytes, number of entries: 15
+Zip file size: 10251 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/__init__.py
 -rw-r--r--  2.0 unx     3790 b- defN 23-Jun-21 06:15 spark_ai/spark.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/dbs/__init__.py
 -rw-r--r--  2.0 unx     2241 b- defN 23-Jun-21 06:15 spark_ai/dbs/pinecone.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/files/__init__.py
 -rw-r--r--  2.0 unx     1049 b- defN 23-Jun-21 06:15 spark_ai/files/pdf.py
 -rw-r--r--  2.0 unx      513 b- defN 23-Jun-21 06:15 spark_ai/files/text.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:15 spark_ai/llms/__init__.py
 -rw-r--r--  2.0 unx     2746 b- defN 23-Jun-21 06:15 spark_ai/llms/openai.py
 -rw-r--r--  2.0 unx      689 b- defN 23-Jun-22 23:34 spark_ai/webapps/__init__.py
--rw-r--r--  2.0 unx     9643 b- defN 23-Jun-21 06:15 spark_ai/webapps/slack.py
--rw-r--r--  2.0 unx     3603 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1205 b- defN 23-Jun-24 18:53 prophecy_spark_ai-0.1.7.dist-info/RECORD
-15 files, 25580 bytes uncompressed, 8224 bytes compressed:  67.8%
+-rw-r--r--  2.0 unx     9664 b- defN 23-Jul-18 05:36 spark_ai/webapps/slack.py
+-rw-r--r--  2.0 unx     3603 b- defN 23-Jul-18 05:37 prophecy_spark_ai-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 05:37 prophecy_spark_ai-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-18 05:37 prophecy_spark_ai-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1205 b- defN 23-Jul-18 05:37 prophecy_spark_ai-0.1.8.dist-info/RECORD
+15 files, 25601 bytes uncompressed, 8243 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: spark_ai/webapps/__init__.py
 Comment: 
 
 Filename: spark_ai/webapps/slack.py
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.7.dist-info/METADATA
+Filename: prophecy_spark_ai-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.7.dist-info/WHEEL
+Filename: prophecy_spark_ai-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.7.dist-info/top_level.txt
+Filename: prophecy_spark_ai-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: prophecy_spark_ai-0.1.7.dist-info/RECORD
+Filename: prophecy_spark_ai-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_ai/webapps/slack.py

```diff
@@ -222,15 +222,15 @@
 
         return messages
 
     def write_messages(self, df: DataFrame):
         if not df.isStreaming:
             raise TypeError("Slack messages write is for streaming pipelines only")
 
-        df.writeStream.foreachBatch(self._write_batch).start()
+        df.writeStream.outputMode("update").foreachBatch(self._write_batch).start()
 
     def _write_batch(self, df_batch: DataFrame, epoch_id: int):
         responses = df_batch.collect()
         for response in responses:
             client = WebClient(token=self.token)
 
             try:
```

## Comparing `prophecy_spark_ai-0.1.7.dist-info/METADATA` & `prophecy_spark_ai-0.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-spark-ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: High-performance AI/ML library for Spark to build and deploy your LLM applications in production.
 Home-page: https://github.com/prophecy-io/spark-ai
 Keywords: python,prophecy
 Description-Content-Type: text/markdown
 Requires-Dist: slack-sdk (>=3.21.3)
 Requires-Dist: openai[datalib] (>=0.27.8)
 Requires-Dist: pinecone-client (>=2.2.2)
```

## Comparing `prophecy_spark_ai-0.1.7.dist-info/RECORD` & `prophecy_spark_ai-0.1.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 spark_ai/dbs/pinecone.py,sha256=qRXL4w7wLXKENiMB-ODozpfQ14uSUA034JP8OzLiEYA,2241
 spark_ai/files/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 spark_ai/files/pdf.py,sha256=_xLoM9NJ3b_Xln0Y0qFZ4JYDOlmnDofUxQQEl8FxmN8,1049
 spark_ai/files/text.py,sha256=UIb9kVsouB-bXtjb823oh2z1mDXUwR8qnMnbuBzQIzM,513
 spark_ai/llms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 spark_ai/llms/openai.py,sha256=e55mYL8l1SHKsX-AY1DKkhutk5d9yeaOJALsQ-CwUgQ,2746
 spark_ai/webapps/__init__.py,sha256=cxeMGWd3705XuYVs0qez_MLfJboRLAgiK0_Lg7ULHJ8,689
-spark_ai/webapps/slack.py,sha256=k-yG3EyTZc8-gvXJaDMRnMNzCOkgeH4BYYIqZPi9x88,9643
-prophecy_spark_ai-0.1.7.dist-info/METADATA,sha256=NA3unu-4y_JFIkV3fSc0G5JkXpLJbewFh_GDBuI8nqQ,3603
-prophecy_spark_ai-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-prophecy_spark_ai-0.1.7.dist-info/top_level.txt,sha256=uriwjszTLG2ldv6q-y4J72iKjOjTn2hIFC2lcPsQBvw,9
-prophecy_spark_ai-0.1.7.dist-info/RECORD,,
+spark_ai/webapps/slack.py,sha256=qTwSKB05R8T73vCpxlmcYUeUSWumo2qkclud5dVoUwM,9664
+prophecy_spark_ai-0.1.8.dist-info/METADATA,sha256=RuHJv7uGwg-mZqFWflpa4i12GUYDAQpi4Pnxj9cHOgQ,3603
+prophecy_spark_ai-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+prophecy_spark_ai-0.1.8.dist-info/top_level.txt,sha256=uriwjszTLG2ldv6q-y4J72iKjOjTn2hIFC2lcPsQBvw,9
+prophecy_spark_ai-0.1.8.dist-info/RECORD,,
```

