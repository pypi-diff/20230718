# Comparing `tmp/mortardata-0.1.4.tar.gz` & `tmp/mortardata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mortardata-0.1.4.tar", max compression
+gzip compressed data, was "mortardata-0.1.5.tar", max compression
```

## Comparing `mortardata-0.1.4.tar` & `mortardata-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1586 2023-07-17 03:29:05.945204 mortardata-0.1.4/README.md
--rw-r--r--   0        0        0     7294 2023-07-17 23:44:16.562516 mortardata-0.1.4/mortardata/__init__.py
--rw-r--r--   0        0        0      481 2023-07-17 23:43:38.558198 mortardata-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 mortardata-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1363 2023-07-18 00:14:52.477966 mortardata-0.1.5/README.md
+-rw-r--r--   0        0        0     7377 2023-07-17 23:56:35.108713 mortardata-0.1.5/mortardata/__init__.py
+-rw-r--r--   0        0        0      481 2023-07-18 00:14:59.334024 mortardata-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 mortardata-0.1.5/PKG-INFO
```

### Comparing `mortardata-0.1.4/mortardata/__init__.py` & `mortardata-0.1.5/mortardata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         f = (
             (ds.field("uuid").isin(uuids))
             & (ds.field("time") <= pa.scalar(end, type=pa.timestamp("us", tz="UTC")))
             & (ds.field("time") >= pa.scalar(start, type=pa.timestamp("us", tz="UTC")))
         )
         if sites is not None:
             print([s[4:-1] for s in sites])
+            log.info(f"Fetching data for {sites} with {start=} {end=} ({limit=})")
             f &= ds.field("collection").isin([s[4:-1] for s in sites])
         for batch in tqdm.tqdm(
             self.ds.to_batches(
                 columns=["time", "value", "collection", "uri"], filter=f
             ),
             desc="Downloading data from s3",
             unit="batches",
```

### Comparing `mortardata-0.1.4/PKG-INFO` & `mortardata-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mortardata
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: BSD-3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -34,45 +34,34 @@
 
 Then use as follows:
 
 
 ```python
 from mortardata import Client
 
+# connect client
 c = Client()
 
-all_points = """
+vav_points = """
 PREFIX brick: <https://brickschema.org/schema/Brick#>
 PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
 PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX ref: <https://brickschema.org/schema/Brick/ref#>
-SELECT ?point ?type ?uuid WHERE {
-    ?point rdf:type/rdfs:subClassOf* brick:Point ;
-           rdf:type ?type ;
-           ref:hasExternalReference [ ref:hasTimeseriesId ?uuid ] .
+SELECT ?equip ?point ?id WHERE {
+    ?equip rdf:type/rdfs:subClassOf* brick:VAV ;
+          brick:hasPoint ?point .
+    ?point ref:hasExternalReference/ref:hasTimeseriesId ?id .
 }"""
-df = c.sparql(all_points.strip())
-df.to_csv("all_points.csv")
-print(df.head())
-
-query1 = """
-PREFIX brick: <https://brickschema.org/schema/Brick#>
-PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
-PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
-PREFIX ref: <https://brickschema.org/schema/Brick/ref#>
-SELECT ?sen_point ?sen ?equip ?equip_type WHERE {
-    ?equip rdf:type ?equip_type .
-    ?sen_point rdf:type brick:Supply_Air_Temperature_Sensor ;
-               brick:isPointOf ?equip ;
-               ref:hasExternalReference [ ref:hasTimeseriesId ?sen ] .
-} LIMIT 10"""
-df = c.sparql(query1)
-df.to_csv("query1_sparql.csv")
-print(df.head())
+# get metadata for first 20 sites
+df = c.sparql(vav_points, sites=c.sites[:20]) 
+# most operations return dataframes
+df.to_csv("vav_points.csv")
 
-df = c.data_sparql(query1, start="2016-01-01", end="2016-02-01", limit=1e6, sites=['bldg2','bldg5'])
+# get timeseries data into a dataframe for 2 sites, maximum of 1 million points for January 2016
+df = c.data_sparql(vav_points, start="2016-01-01", end="2016-02-01", limit=1e6, sites=['urn:bldg2#','urn:bldg5#'])
 print(df.head())
 
-res = c.data_sparql_to_csv(query1, "query1.csv", sites=['bldg2','bldg5'])
-print(res)
+# similar to the above, but streams data directly into a CSV file. Can be helpful for extra large downloads
+num = c.data_sparql_to_csv(vav_points, "vav_data.csv", limit=1e6, sites=['urn:bldg2#','urn:bldg5#'])
+print(f"Downloaded {num} datapoints")
 ```
```

