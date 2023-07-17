# Comparing `tmp/mortardata-0.1.3.tar.gz` & `tmp/mortardata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mortardata-0.1.3.tar", max compression
+gzip compressed data, was "mortardata-0.1.4.tar", max compression
```

## Comparing `mortardata-0.1.3.tar` & `mortardata-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1586 2023-07-17 03:29:05.945204 mortardata-0.1.3/README.md
--rw-r--r--   0        0        0     5743 2023-07-17 03:27:49.132559 mortardata-0.1.3/mortardata/__init__.py
--rw-r--r--   0        0        0      442 2023-07-17 03:29:14.793278 mortardata-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 mortardata-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1586 2023-07-17 03:29:05.945204 mortardata-0.1.4/README.md
+-rw-r--r--   0        0        0     7294 2023-07-17 23:44:16.562516 mortardata-0.1.4/mortardata/__init__.py
+-rw-r--r--   0        0        0      481 2023-07-17 23:43:38.558198 mortardata-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 mortardata-0.1.4/PKG-INFO
```

### Comparing `mortardata-0.1.3/README.md` & `mortardata-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mortardata-0.1.3/mortardata/__init__.py` & `mortardata-0.1.4/mortardata/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from itertools import groupby
+import time
+from loguru import logger as log
 import os
+from functools import cache, cached_property
 import base64
 import lzma
 import tqdm
 import io
+import grequests
 import requests
 import pandas as pd
 from rdflib.plugins.sparql.results.jsonresults import JSONResultParser
 import functools
 import pyarrow as pa
 import pyarrow.dataset as ds
 import pyarrow.compute as pc
@@ -26,47 +31,78 @@
                 yield prefix, namespace
 
         rdflib.namespace.NamespaceManager.namespaces = namespaces
 
         self._s3 = fs.S3FileSystem(region=os.getenv("MORTARDATA_S3_REGION"))
         self._bucket = os.getenv("MORTARDATA_S3_BUCKET")
         self._sparql_endpoint = os.getenv("MORTARDATA_QUERY_ENDPOINT")
+        self._sites_endpoint = os.getenv("MORTARDATA_SITES_ENDPOINT")
         
         self.ds = ds.parquet_dataset(
             f"{self._bucket}/_metadata", partitioning="hive", filesystem=self._s3
         )
+        log.info("Connected to Parquet dataset")
 
     def _table_exists(self, table):
         try:
             res = self.data_cache.table(table)
             return res is not None
         except RuntimeError:
             return False
 
-    def sparql(self, query):
-        res = requests.post(self._sparql_endpoint, data=query)
+    @cached_property
+    def sites(self):
+        t0 = time.time()
+        res = requests.get(self._sites_endpoint)
+        sites = res.json()
+        log.info(f"Fetched {len(sites)} sites in {time.time()-t0:.2f}sec")
+        return sites
+
+
+    def sparql(self, query, sites=None):
+        body = {'query': query}
+        if sites is not None:
+            body['sites'] = sites
+            log.info(f"Dispatching parallel SPARQL queries for {len(sites)} sites")
+            sparql_requests = (
+                grequests.post(self._sparql_endpoint, json={'query': query, 'sites': [site]})
+                for site in sites
+            )
+            responses = grequests.imap(sparql_requests, size=len(sites))
+            dfs = []
+            for res in responses:
+                if not res.ok:
+                    raise Exception(res.content)
+                b = io.BytesIO(lzma.decompress(base64.urlsafe_b64decode(res.content)))
+                resp = JSONResultParser().parse(b)
+                df = pd.DataFrame.from_records(list(resp), columns=[str(c) for c in resp.vars])
+                log.info(f"Fetched {len(df)} SPARQL rows")
+                dfs.append(df)
+            return functools.reduce(lambda x, y: pd.concat([x, y], axis=0), dfs)
+        res = requests.post(self._sparql_endpoint, json=body)
         if not res.ok:
             raise Exception(res.content)
         b = io.BytesIO(lzma.decompress(base64.urlsafe_b64decode(res.content)))
         res = JSONResultParser().parse(b)
         df = pd.DataFrame.from_records(list(res), columns=[str(c) for c in res.vars])
         return df
 
     def _to_batches(self, sparql, sites=None, start=None, end=None, limit=None):
-        res = self.sparql(sparql)
+        res = self.sparql(sparql, sites=sites)
         start = pd.to_datetime("2000-01-01T00:00:00Z" if not start else start)
         end = pd.to_datetime("2100-01-01T00:00:00Z" if not end else end)
         uuids = list(set([str(item) for row in res.values for item in row]))
         f = (
             (ds.field("uuid").isin(uuids))
             & (ds.field("time") <= pa.scalar(end, type=pa.timestamp("us", tz="UTC")))
             & (ds.field("time") >= pa.scalar(start, type=pa.timestamp("us", tz="UTC")))
         )
         if sites is not None:
-            f &= ds.field("collection").isin(sites)
+            print([s[4:-1] for s in sites])
+            f &= ds.field("collection").isin([s[4:-1] for s in sites])
         for batch in tqdm.tqdm(
             self.ds.to_batches(
                 columns=["time", "value", "collection", "uri"], filter=f
             ),
             desc="Downloading data from s3",
             unit="batches",
         ):
```

### Comparing `mortardata-0.1.3/PKG-INFO` & `mortardata-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: mortardata
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: BSD-3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: grequests (>=0.7.0,<0.8.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: rdflib (>=6.3.2,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
```

