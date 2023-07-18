# Comparing `tmp/mars_text_embedding_sdk_python-0.1.0.tar.gz` & `tmp/mars_text_embedding_sdk_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mars_text_embedding_sdk_python-0.1.0.tar", max compression
+gzip compressed data, was "mars_text_embedding_sdk_python-0.1.2.tar", max compression
```

## Comparing `mars_text_embedding_sdk_python-0.1.0.tar` & `mars_text_embedding_sdk_python-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-27 16:40:14.535890 mars_text_embedding_sdk_python-0.1.0/README.md
--rw-r--r--   0        0        0     1761 2023-06-27 16:51:06.765056 mars_text_embedding_sdk_python-0.1.0/mars_text_embedding_sdk_python/__init__.py
--rw-r--r--   0        0        0      370 2023-06-27 16:43:03.830892 mars_text_embedding_sdk_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mars_text_embedding_sdk_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-27 16:40:14.535890 mars_text_embedding_sdk_python-0.1.2/README.md
+-rw-r--r--   0        0        0     1734 2023-07-18 13:17:59.357071 mars_text_embedding_sdk_python-0.1.2/mars_text_embedding_sdk_python/__init__.py
+-rw-r--r--   0        0        0      433 2023-07-18 13:25:07.725770 mars_text_embedding_sdk_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 mars_text_embedding_sdk_python-0.1.2/PKG-INFO
```

### Comparing `mars_text_embedding_sdk_python-0.1.0/mars_text_embedding_sdk_python/__init__.py` & `mars_text_embedding_sdk_python-0.1.2/mars_text_embedding_sdk_python/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from numpy import array
 from requests import post
 from dataclasses import dataclass
 from typing import Optional, List
 
 @dataclass
 class Result:
 
@@ -9,48 +10,44 @@
     error:  Optional[str]   = None
 
 @dataclass
 class EmbeddingSDK:
     
     url: str
 
-    def __call__(self, text_list: List[List[str]]) -> Result:
+    def __call__(self, text_list: List[List[str]], dims: int = 100) -> Result:
 
         """
             Converts a list of sentences, or list of list of strings, into a list of embeddings.
             Each list of strings will be converted into a single embedding.
 
             :param text_list: A list of sentences, or list of list of strings, to be converted into embeddings.
+            :param dims: The number of dimensions of the embedding. Must be 3, 5 or 100.
             :return: A list of embeddings, or a list of list of embeddings, depending on the input.
         """
 
         try:
             response = post(
                 self.url, 
                 json={
                     "query": """
                         query TextQuery($sentences: [[String!]!]!) {
-                            textCollection(corpuses: $sentences) {
-                                embedded
-                            }
+                            textCollection(corpuses: $sentences, model: D"""+str(dims)+""")
                         }
                     """,
                     "variables": {
                         "sentences": text_list,
                     }
                 }
             )
 
             if response.status_code == 200:
                 if "errors" in response.json():
                     return Result(error=response.json()["errors"][0]["message"])
                 return Result(
-                    data=list(
-                        map(
-                            lambda x: x['embedded'],
-                            response.json()["data"]["textCollection"]
-                        )
+                    data=array(
+                        response.json()["data"]["textCollection"]
                     )
                 )
 
         except Exception as e:
             return Result(error=str(e))
```

