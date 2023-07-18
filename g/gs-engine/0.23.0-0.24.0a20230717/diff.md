# Comparing `tmp/gs_engine-0.23.0-py2.py3-none-macosx_11_0_x86_64.whl.zip` & `tmp/gs_engine-0.24.0a20230717-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11833 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      804 b- defN 23-Jul-04 11:01 gs_engine-0.23.0.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 23-Jul-04 10:44 gs_engine-0.23.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-04 10:44 gs_engine-0.23.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21671 b- defN 23-Jul-04 10:44 gs_engine-0.23.0.dist-info/METADATA
--rw-r--r--  2.0 unx      694 b- defN 23-Jul-04 08:42 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx     1573 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      503 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/log4rs.yml
-9 files, 26006 bytes uncompressed, 10443 bytes compressed:  59.8%
+Zip file size: 11917 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-17 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-17 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    21680 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jul-17 20:31 gs_engine-0.24.0a20230717.dist-info/RECORD
+9 files, 26058 bytes uncompressed, 10455 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: gs_engine-0.23.0.dist-info/RECORD
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.23.0.dist-info/WHEEL
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.23.0.dist-info/top_level.txt
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: gs_engine-0.23.0.dist-info/METADATA
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: gs_engine-0.24.0a20230717.dist-info/METADATA
 Comment: 
 
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: gs_engine-0.24.0a20230717.dist-info/WHEEL
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: gs_engine-0.24.0a20230717.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: gs_engine-0.24.0a20230717.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## graphscope.runtime/conf/frontend.vineyard.properties

```diff
@@ -10,12 +10,13 @@
 # e.g. 1.2.3.4:1234,1.2.3.5:1234
 pegasus.hosts = PEGASUS_HOSTS
 
 # graph schema path
 graph.schema = GRAPH_SCHEMA
 
 ## Frontend Config
-gremlin.server.port = FRONTEND_SERVICE_PORT
+gremlin.server.port = FRONTEND_GREMLIN_PORT
 
+neo4j.bolt.server.port = FRONTEND_CYPHER_PORT
 # disable the authentication if username or password is not set
 #auth.username = default
 #auth.password = default
```

## Comparing `gs_engine-0.23.0.dist-info/METADATA` & `gs_engine-0.24.0a20230717.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.23.0
+Version: 0.24.0a20230717
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

