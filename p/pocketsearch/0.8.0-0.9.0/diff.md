# Comparing `tmp/pocketsearch-0.8.0.tar.gz` & `tmp/pocketsearch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.8.0.tar", last modified: Sat Jun 17 10:05:35 2023, max compression
+gzip compressed data, was "pocketsearch-0.9.0.tar", last modified: Sat Jul  1 17:15:52 2023, max compression
```

## Comparing `pocketsearch-0.8.0.tar` & `pocketsearch-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.522325 pocketsearch-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.522325 pocketsearch-0.8.0/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    46516 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24733 2023-06-17 10:05:26.000000 pocketsearch-0.8.0/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:05:35.526325 pocketsearch-0.8.0/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 10:05:35.000000 pocketsearch-0.8.0/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:15:52.798200 pocketsearch-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-01 17:15:43.000000 pocketsearch-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-07-01 17:15:52.794200 pocketsearch-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-07-01 17:15:43.000000 pocketsearch-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:15:52.798200 pocketsearch-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 17:15:43.000000 pocketsearch-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:15:52.794200 pocketsearch-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:15:52.794200 pocketsearch-0.9.0/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    50817 2023-07-01 17:15:43.000000 pocketsearch-0.9.0/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28216 2023-07-01 17:15:43.000000 pocketsearch-0.9.0/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:15:52.794200 pocketsearch-0.9.0/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-07-01 17:15:52.000000 pocketsearch-0.9.0/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-01 17:15:52.000000 pocketsearch-0.9.0/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:15:52.000000 pocketsearch-0.9.0/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 17:15:52.000000 pocketsearch-0.9.0/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.8.0/LICENSE` & `pocketsearch-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.8.0/PKG-INFO` & `pocketsearch-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.8.0
+Version: 0.9.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -19,19 +19,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Indexing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pocketsearch
-pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
+pocketsearch is a pure-Python full text indexing search engine based on sqlite and the [FTS5](https://www.sqlite.org/fts5.html) extension. It provides
 
-- Support for full text search
 - A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
 - Support for multi-field indices including text, numeric and date search
+- Support for prefix and initial token queries
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
 pocketsearch is currently being tested on data from Wikipedia, indexing more than 6 million abstracts. If you 
 are interested in preliminary performance tests, have a look at https://github.com/kaykay-dv/pocketsearch/tree/development/tests.
 
@@ -118,14 +118,29 @@
 If you want to search for substrings, you can use prefix queries, by 
 providing the allow_prefix lookup:
 
 ```Python
 print(pocket_search.search(text__allow_prefix="hel*")[0].text)
 ```
 
+Please note, that prefix queries might get very slow as the index grows. To 
+optimize performance, you can use prefix indices as described in the chapter 
+on "schemas" in this README.
+
+## Initial token queries
+
+If you want to search only the first token at the begining of a document, use the 
+allow_initial_token lookup:
+
+```Python
+pocket_search.search(text__allow_initial_token="^hello")
+```
+
+This will only match results that have 'hello' at the very beginning. 
+
 ## Phrase queries
 
 If you want to search for phrases, use quotation marks:
 
 ```Python
 pocket_search.search(text='"this is" "a phrase"').count()
 ```
@@ -170,15 +185,15 @@
 [Hello] World !
 ```
 
 The positional arguments of the highlight method represent the fields you want to hightlight. 
 
 If you have very long text, you might want to only show a snippet with all terms found in your +
 search results. This can be done with the snippet method. Assuming we have the article 
-on inverted indices (https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
+on Wikipedia article on [inverted indices](https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
 
 ```Python
 pocket_search.search(text="inverted file").snippet("text",snippet_length=16)[0].text
 'In computer science, an *inverted* index (also referred to as a postings list, postings *file*, or...'
 ```
 
 Similar to the highlight method, the snippet method highlights tokens found. snippet_length defines 
@@ -220,48 +235,80 @@
 | Numeric      | Numeric  |
 | Blob         | Blob  |
 | Date         | Date  |
 | Datetime     | Datetime  |
 
 Following options are available for fields:
 
-* index - if the field is a Text field, a full text search index is created, otherwise a standard sqlite3 index is created
-* is_id_field - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
+* **index** - if the field is a Text field, a full text search index is created, otherwise a standard sqlite3 index is created
+* **is_id_field** - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
 
 With respect to naming your fields following restrictions apply:
 
 * Fields may not start with an underscore.
 * Fields may not contain double underscores.
 
-> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
+Moreover field names may not be composed of reserved SQL keywords.
+
+> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document. The ID field is used to delete or 
+update documents.
+
+## Queries on multi-field indices
 
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
 # Searches documents that contain "world" in text AND have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
-> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
+> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND.
+
+### AND/OR queries on multiple fields
 
-However, you can join 2 queries (resulting in a UNION statement in SQL):
+Similar to the Django web framework, you can use "Q Objects" to express OR queries on multiple fields:
 
 ```Python
-q = pocket_search.search(text="world") | pocket_search.search(filename="a.txt")
-for result in q:
-    print(result.text)
+from pocketsearch import Q
+# Search for documents where text="world" OR filename="a.txt"
+q = pocket_search.search(Q(text="world") | Q(filename="a.txt"))
+# Search for documents where text="world" AND filename="a.txt"
+q = pocket_search.search(Q(text="world") & Q(filename="a.txt"))
 ```
 
-The result will contain all documents containing either "world" or where the filename is "a.text".
+Please note, that you either have to use one notation or the other. You cannot mix 
+Q objects with keyword arguments and you can only provide one field per Q object:
+
+```Python
+# This will NOT work:
+pocket_search.search(Q(text="world") , filename="a.txt")
+# This will work neither:
+pocket_search.search(Q(text="world",filename="a.txt"))
+```
+
+
+## Setting prefix indices
+To speed up prefix queries, you can setup prefix indices:
+
+```Python
+    class PrefixIndex1(Schema):
+        '''
+        Simple schema that sets a prefix index for 
+        2,3 and 4 characters
+        '''
+        class Meta:
+            prefix_index=[2,3,4]
+        body = Text(index=True)
+```
 
-This option is currently experimental and still has issues, espcially when accessing results through indexing. 
+This will create prefix indices for 2,3 and 4 character prefixes.
 
 # Inserting, updating and deleting data
 
 ## Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
@@ -431,17 +478,17 @@
         sqlite_tokenchars = None
         sqlite_separators = None    
 
     text = Text(index=True)
     filename = Text(is_id_field=True)
 ```
 
-# Multiple indicies in one database
+# Multiple indices in one database
 
-You can have multiple indicies in one database (only databases written to disk) by setting 
+You can have multiple indices in one database (only databases written to disk) by setting 
 the "index_name" option:
 
 ```Python
 pocket_search = PocketSearch(db_name="my_db.db",index_name="Product",schema=Product)
 ```
 
 # Contribute
```

### Comparing `pocketsearch-0.8.0/README.md` & `pocketsearch-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pocketsearch
-pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
+pocketsearch is a pure-Python full text indexing search engine based on sqlite and the [FTS5](https://www.sqlite.org/fts5.html) extension. It provides
 
-- Support for full text search
 - A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
 - Support for multi-field indices including text, numeric and date search
+- Support for prefix and initial token queries
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
 pocketsearch is currently being tested on data from Wikipedia, indexing more than 6 million abstracts. If you 
 are interested in preliminary performance tests, have a look at https://github.com/kaykay-dv/pocketsearch/tree/development/tests.
 
@@ -94,14 +94,29 @@
 If you want to search for substrings, you can use prefix queries, by 
 providing the allow_prefix lookup:
 
 ```Python
 print(pocket_search.search(text__allow_prefix="hel*")[0].text)
 ```
 
+Please note, that prefix queries might get very slow as the index grows. To 
+optimize performance, you can use prefix indices as described in the chapter 
+on "schemas" in this README.
+
+## Initial token queries
+
+If you want to search only the first token at the begining of a document, use the 
+allow_initial_token lookup:
+
+```Python
+pocket_search.search(text__allow_initial_token="^hello")
+```
+
+This will only match results that have 'hello' at the very beginning. 
+
 ## Phrase queries
 
 If you want to search for phrases, use quotation marks:
 
 ```Python
 pocket_search.search(text='"this is" "a phrase"').count()
 ```
@@ -146,15 +161,15 @@
 [Hello] World !
 ```
 
 The positional arguments of the highlight method represent the fields you want to hightlight. 
 
 If you have very long text, you might want to only show a snippet with all terms found in your +
 search results. This can be done with the snippet method. Assuming we have the article 
-on inverted indices (https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
+on Wikipedia article on [inverted indices](https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
 
 ```Python
 pocket_search.search(text="inverted file").snippet("text",snippet_length=16)[0].text
 'In computer science, an *inverted* index (also referred to as a postings list, postings *file*, or...'
 ```
 
 Similar to the highlight method, the snippet method highlights tokens found. snippet_length defines 
@@ -196,48 +211,80 @@
 | Numeric      | Numeric  |
 | Blob         | Blob  |
 | Date         | Date  |
 | Datetime     | Datetime  |
 
 Following options are available for fields:
 
-* index - if the field is a Text field, a full text search index is created, otherwise a standard sqlite3 index is created
-* is_id_field - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
+* **index** - if the field is a Text field, a full text search index is created, otherwise a standard sqlite3 index is created
+* **is_id_field** - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
 
 With respect to naming your fields following restrictions apply:
 
 * Fields may not start with an underscore.
 * Fields may not contain double underscores.
 
-> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
+Moreover field names may not be composed of reserved SQL keywords.
+
+> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document. The ID field is used to delete or 
+update documents.
+
+## Queries on multi-field indices
 
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
 # Searches documents that contain "world" in text AND have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
-> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
+> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND.
+
+### AND/OR queries on multiple fields
 
-However, you can join 2 queries (resulting in a UNION statement in SQL):
+Similar to the Django web framework, you can use "Q Objects" to express OR queries on multiple fields:
 
 ```Python
-q = pocket_search.search(text="world") | pocket_search.search(filename="a.txt")
-for result in q:
-    print(result.text)
+from pocketsearch import Q
+# Search for documents where text="world" OR filename="a.txt"
+q = pocket_search.search(Q(text="world") | Q(filename="a.txt"))
+# Search for documents where text="world" AND filename="a.txt"
+q = pocket_search.search(Q(text="world") & Q(filename="a.txt"))
 ```
 
-The result will contain all documents containing either "world" or where the filename is "a.text".
+Please note, that you either have to use one notation or the other. You cannot mix 
+Q objects with keyword arguments and you can only provide one field per Q object:
+
+```Python
+# This will NOT work:
+pocket_search.search(Q(text="world") , filename="a.txt")
+# This will work neither:
+pocket_search.search(Q(text="world",filename="a.txt"))
+```
+
+
+## Setting prefix indices
+To speed up prefix queries, you can setup prefix indices:
+
+```Python
+    class PrefixIndex1(Schema):
+        '''
+        Simple schema that sets a prefix index for 
+        2,3 and 4 characters
+        '''
+        class Meta:
+            prefix_index=[2,3,4]
+        body = Text(index=True)
+```
 
-This option is currently experimental and still has issues, espcially when accessing results through indexing. 
+This will create prefix indices for 2,3 and 4 character prefixes.
 
 # Inserting, updating and deleting data
 
 ## Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
@@ -407,17 +454,17 @@
         sqlite_tokenchars = None
         sqlite_separators = None    
 
     text = Text(index=True)
     filename = Text(is_id_field=True)
 ```
 
-# Multiple indicies in one database
+# Multiple indices in one database
 
-You can have multiple indicies in one database (only databases written to disk) by setting 
+You can have multiple indices in one database (only databases written to disk) by setting 
 the "index_name" option:
 
 ```Python
 pocket_search = PocketSearch(db_name="my_db.db",index_name="Product",schema=Product)
 ```
 
 # Contribute
```

### Comparing `pocketsearch-0.8.0/setup.py` & `pocketsearch-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.8.0",
+    version = "0.9.0",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
```

### Comparing `pocketsearch-0.8.0/src/pocketsearch/__init__.py` & `pocketsearch-0.9.0/src/pocketsearch/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -222,28 +222,30 @@
         set proper defaults.
         '''
         sqlite_tokenize = "unicode61"
         sqlite_remove_diacritics = None
         sqlite_categories = None
         sqlite_tokenchars = None
         sqlite_separators = None
+        prefix_index = None
 
     RESERVED_KEYWORDS = [
         'ABORT', 'ACTION', 'ADD', 'AFTER', 'ALL', 'ALTER', 'ANALYZE', 'AND', 'AS', 'ASC', 'ATTACH', 'AUTOINCREMENT',
         'BEFORE', 'BEGIN', 'BETWEEN', 'BY', 'CASCADE', 'CASE', 'CAST', 'CHECK', 'COLLATE', 'COLUMN', 'COMMIT',
         'CONFLICT', 'CONSTRAINT', 'CREATE', 'CROSS', 'CURRENT_DATE', 'CURRENT_TIME', 'CURRENT_TIMESTAMP', 'DATABASE',
         'DEFAULT', 'DEFERRABLE', 'DEFERRED', 'DELETE', 'DESC', 'DETACH', 'DISTINCT', 'DROP', 'EACH', 'ELSE', 'END',
         'CONTENT', 'ESCAPE', 'EXCEPT', 'EXCLUSIVE', 'EXISTS', 'EXPLAIN', 'FAIL', 'FOR', 'FOREIGN', 'FROM', 'FULL', 'GLOB',
         'GROUP', 'HAVING', 'IF', 'IGNORE', 'IMMEDIATE', 'IN', 'INDEX', 'INDEXED', 'INITIALLY', 'INNER', 'INSERT',
         'INSTEAD', 'INTERSECT', 'INTO', 'IS', 'ISNULL', 'JOIN', 'KEY', 'LEFT', 'LIKE', 'LIMIT', 'MATCH', 'NATURAL',
         'NO', 'NOT', 'NOTNULL', 'NULL', 'OF', 'OFFSET', 'ON', 'OR', 'ORDER', 'OUTER', 'PLAN', 'PRAGMA', 'PRIMARY',
         'QUERY', 'RAISE', 'RECURSIVE', 'REFERENCES', 'REGEXP', 'REINDEX', 'RELEASE', 'RENAME', 'REPLACE', 'RESTRICT',
         'RIGHT', 'ROLLBACK', 'ROW', 'SAVEPOINT', 'SELECT', 'SET', 'TABLE', 'TEMP', 'TEMPORARY', 'THEN', 'TO',
         'TRANSACTION', 'TRIGGER', 'UNION', 'UNIQUE', 'UPDATE', 'USING', 'VACUUM', 'VALUES', 'VIEW', 'VIRTUAL', 'WHEN',
-        'WHERE', 'WITH', 'WITHOUT'
+        'WHERE', 'WITH', 'WITHOUT','NAME','FIELDS','FIELDS_INDEX','FIELDS_WITH_DEFAULT',
+        'REVERSE_LOOKUP','ID_FIELD'
     ]
 
     class SchemaError(Exception):
         '''
         Thrown, if the schema cannot be generated.
         '''
 
@@ -445,14 +447,15 @@
         return self.table_name
 
 
 LU_EQ = "eq"
 LU_BOOL = "allow_boolean"
 LU_NEG = "allow_negation"
 LU_PREFIX = "allow_prefix"
+LU_INITIAL_TOKEN = "allow_initial_token"
 LU_GTE = "gte"
 LU_LTE = "lte"
 LU_GT = "gt"
 LU_LT = "lt"
 LU_YEAR = "year"
 LU_MONTH = "month"
 LU_DAY = "day"
@@ -460,14 +463,15 @@
 LU_MINUTE = "minute"
 
 LOOKUPS = {
     LU_EQ: [],  # valid for all field types
     LU_BOOL: [Text],
     LU_NEG: [Text],
     LU_PREFIX: [Text],
+    LU_INITIAL_TOKEN: [Text],
     LU_GTE: [Int],
     LU_LTE: [Int],
     LU_GT: [Int],
     LU_LT: [Int],
     LU_YEAR: [Date, Datetime],
     LU_MONTH: [Date, Datetime],
     LU_DAY: [Date, Datetime],
@@ -487,21 +491,23 @@
                  value,
                  sql_query,
                  lookup):
         super().__init__(sql_query)
         self.field = field
         self.value = value
         self.keywords = []
-        self.operators = ["-", ".", "^"]
+        self.operators = ["-", "."]
         if not(LU_BOOL in lookup.names):
             self.keywords = self.keywords + ["AND", "OR"]
         if not(LU_NEG in lookup.names):
             self.keywords.append("NOT")
         if not(LU_PREFIX in lookup.names):
             self.operators.append("*")
+        if not(LU_INITIAL_TOKEN in lookup.names):
+            self.operators.append("^")
 
 
 class MatchFilter(Filter):
     '''
     Full text match filter in where clause
     '''
 
@@ -513,16 +519,17 @@
                 return value.replace(v, '"%s"' % v)
         for ch in self.operators:
             if ch in value:
                 return value.replace(value, '"%s"' % value)
         return value
 
     def to_sql(self):
-        self.sql_query.add_value(self._escape(self.value))
-        return "%s MATCH ?" % self.field.get_full_qualified_name()
+        v = "%s:%s" % (self.field.name,self._escape(self.value))
+        #self.sql_query.add_value(v)
+        return v
 
 
 class BooleanFilter(SQLQueryComponent):
     '''
     Referenced field in WHERE clause that
     is not part of the FTS5 index.
     '''
@@ -643,30 +650,48 @@
 
     def to_sql(self):
         return "{table_left}.{left_field}={table_right}.{right_field}".format(table_left=self.table_left.to_sql(),
                                                                               table_right=self.table_right.to_sql(),
                                                                               left_field=self.left_field,
                                                                               right_field=self.right_field)
 
+class And(SQLQueryComponent):
+    '''
+    AND keyword in sql query
+    '''
+
+    def to_sql(self):
+        return "AND"
+
+class Or(SQLQueryComponent):
+    '''
+    OR keyword in sql query
+    '''
+
+    def to_sql(self):
+        return "OR"
 
 class SQLQuery:
     '''
     Helper class that constructs the SQLQuery from
     individual SQLQueryComponent objects
     '''
 
     def __init__(self, search_instance):
         self.search_instance = search_instance
         self.v_select = []
         self.v_from_tables = []
         self.v_joins = []
         self.v_where = []
+        self.v_where_fts = []
         self.v_order_by = []
         self.v_limit_and_offset = None
         self.query_args = []
+        self.boolean_query=False
+        self.connect_fts_clause=None
 
     def count(self):
         '''
         Add a count(*) expression to the current query
         '''
         self.v_select.clear()
         self.v_select.append(Count(sql_query=self))
@@ -717,27 +742,46 @@
             self.v_joins.clear()
         self.v_joins.append(Join(table_left=table_left,
                                  table_right=table_right,
                                  left_field=left_field,
                                  right_field=right_field,
                                  sql_query=self))
 
-    def where(self, field, lookup, clear=False):
+    def where(self, field, lookup, operator, clear=False):
         '''
         Set filter items.
         '''
         if clear:
             self.v_where.clear()
-        if field.fts_enabled():
-            filter_clazz = MatchFilter
         else:
-            filter_clazz = BooleanFilter
-        if field.__class__ is Date:
-            filter_clazz = DateFilter
-        self.v_where.append(filter_clazz(field=field, value=lookup.value, lookup=lookup, sql_query=self))
+            if field.fts_enabled():
+                filter_clazz = MatchFilter
+            else:
+                filter_clazz = BooleanFilter
+            if field.__class__ is Date:
+                filter_clazz = DateFilter
+            if field.fts_enabled():
+                if operator is not None:
+                    if len(self.v_where) > 0 and len(self.v_where_fts) == 0:
+                        self.connect_fts_clause=operator(self)
+                    else:
+                        self.v_where_fts.append(operator(self))
+                self.v_where_fts.append(filter_clazz(field=field, value=lookup.value, lookup=lookup, sql_query=self))
+            else:
+                if operator is not None:
+                    if len(self.v_where_fts) > 0 and len(self.v_where) == 0:
+                        self.connect_fts_clause=operator(self)
+                    else:
+                        self.v_where.append(operator(self))
+                else:
+                    if len(self.v_where)>0:
+                        self.v_where.append(And(self))
+                self.v_where.append(filter_clazz(field=field, value=lookup.value, lookup=lookup, sql_query=self))
+
+
 
     def order_by(self, field, sort_dir=None, clear=False):
         '''
         Adds an order_by clause to the current statement. sort_dir can either be "+" (ascending)
         or "-" (descending)
         '''
         if clear:
@@ -767,53 +811,101 @@
         stmt.append(",".join([s.to_sql() for s in self.v_select]))
         stmt.append("FROM")
         stmt.append(",".join([t.to_sql() for t in self.v_from_tables]))
         if self.v_joins or self.v_where:
             stmt.append("WHERE")
             stmt.append(" AND ".join([j.to_sql() for j in self.v_joins]))
             if self.v_where:
-                stmt.append("AND")
-                stmt.append(" AND ".join([w.to_sql() for w in self.v_where]))
+                stmt.append("AND (")
+                stmt.append(" ".join([w.to_sql() for w in self.v_where]))
+                stmt.append(" ) ")
+            if self.v_where_fts:
+                if self.connect_fts_clause:
+                    stmt.append(self.connect_fts_clause.to_sql())
+                else:
+                    stmt.append(" AND ")
+                table_name="%s_fts" % self.search_instance.schema.name
+                stmt.append(table_name)
+                stmt.append("MATCH ?")
+                val = " ".join([w.to_sql() for w in self.v_where_fts])                
+                self.add_value(val)
         if len(self.v_order_by) > 0:
             stmt.append("ORDER BY")
         stmt.append(",".join([o.to_sql() for o in self.v_order_by]))
         if self.v_limit_and_offset is not None:
             stmt.append(self.v_limit_and_offset.to_sql())
         return " ".join(stmt), self.query_args
 
+class QExpr:
+
+    def __init__(self,**kwargs):
+        if len(kwargs)>1:
+            raise Query.QueryError("Only one keyword argument allowed in Q objects.")
+        self.kwargs=kwargs
+        self.operator=None
+
+    def __repr__(self):
+        return "<QExpr:%s %s>" % (self.operator,self.kwargs)
+
+class Q:
+
+    def __init__(self,**kwargs):
+        self.q_exprs = [QExpr(**kwargs)]
+
+    def __or__(self,obj):
+        for q_expr in obj.q_exprs:
+            q_expr.operator=Or
+            self.q_exprs.append(q_expr)
+        return self
+
+    def __and__(self,obj):
+        for q_expr in obj.q_exprs:
+            q_expr.operator=And
+            self.q_exprs.append(q_expr)
+        return self
+
+    def __repr__(self):
+        return " ".join([str(ex) for ex in self.q_exprs])
+
+    def __iter__(self):
+        return iter(self.q_exprs)
 
 class Query:
     '''
     The Query class is responsible for managing and constructing SQL queries
     against the index. Most of the work is delegated to the SQLQuery class
     which builds the actual SQL query.
     '''
 
     class QueryError(Exception):
         '''
         Raised if the query could not be correctly interpreted.
         '''
 
-    def __init__(self, search_instance, arguments):
+    def __init__(self, search_instance, arguments, q_arguments):
         self.search_instance = search_instance
         self.arguments = arguments
         self.sql_query = SQLQuery(search_instance=search_instance)
         self.unions = []
         for field in self.search_instance.schema.get_fields():
             self.sql_query.select(field=field)
-        for argument in arguments.values():
-            for lookup in argument.lookups:
-                self.sql_query.where(field=argument.field, lookup=lookup)
-        #self.sql_query.select("rank")
+        if len(arguments)>0:
+            for argument in arguments.values():
+                for lookup in argument.lookups:
+                    self.sql_query.where(field=argument.field, lookup=lookup , operator = None)
+        else:
+            for q_expr in q_arguments:
+                for argument in q_expr.arguments.values():
+                    for lookup in argument.lookups:
+                        self.sql_query.where(field=argument.field,lookup=lookup , operator = q_expr.operator)
         self.sql_query.table(table_name=self.search_instance.schema.name)
         self.sql_query.table(table_name="%s_fts" % self.search_instance.schema.name)
         self.sql_query.join(self.sql_query.v_from_tables[0], self.sql_query.v_from_tables[1], "id", "rowid")
         self.sql_query.order_by("+rank")
         self.sql_query.limit_and_offset(limit=10, offset=0)
-        #self._defaults_set = True
         self._default_order_by_set = True
         self._default_values_set = True
         self.is_aggregate_query = False
 
     def _defaults_set(self):
         # Returns true if any default parameters set for .values and .order_by
         # clauses have been changed
@@ -876,19 +968,21 @@
         self.unions.append(obj)
         return self
 
     def values(self, *args):
         '''
         Set the values you want to have in the search result list.
         '''
-        self._default_values_set = False
         for a in args:
             field = self.search_instance.schema.get_field(a, raise_exception=True)
             self.sql_query.select(field,clear=self._default_values_set)
             self._default_values_set = False
+        # Propagate this to union queries as well:
+        for query in self.unions:
+            query.values(*args)
         return self
 
     def highlight(self,*args,marker_start="*",marker_end="*"):
         '''
         Marks given field for highlight
         '''
         for a in args:
@@ -922,15 +1016,15 @@
 
     def _query(self):
         if len(self.unions) > 0:
             self._adapt_union_queries()
         stmt, query_args = self.sql_query.to_sql()
         for query in self.unions:
             u_stmt, u_ar = query.sql_query.to_sql()
-            stmt += " UNION ALL " + u_stmt
+            stmt += " UNION " + u_stmt
             query_args = query_args + u_ar
         if self.is_aggregate_query:
             count = 0
             for sub_count in self.search_instance.execute_sql(stmt, *query_args):
                 count = count+sub_count["COUNT(*)"]
             return count
         return self._build_results(self.search_instance.execute_sql(stmt, *query_args))
@@ -1062,14 +1156,26 @@
         for option in dir(m):
             if option.startswith("sqlite") and getattr(m, option) is not None:
                 options.append("%s=\"%s\"" % (option.split("sqlite_")[1:][0], getattr(m, option)))
         if len(options) == 0:
             return ""
         return "," + ",".join(options)
 
+    def _create_prefix_index(self):
+        prefix_index = self.schema._meta.prefix_index
+        if prefix_index is not None:
+            if not(isinstance(prefix_index,list)):
+                raise self.schema.SchemaError("prefix_index must be list containing positive integer values")
+            if not(all(isinstance(item, int) and item > 0 for item in prefix_index)):
+                raise self.schema.SchemaError("prefix_index list should only contain positive integer values.")
+            # eliminate duplicates
+            prefix_index = set(prefix_index)
+            return ", prefix='{prefix_index}'".format(prefix_index=" ".join(str(item) for item in prefix_index))
+        return ""
+
     def _create_table(self, index_name):
         '''
         Private method to create the SQL tables used by the index.
         '''
         fields = []
         index_fields = []
         default_index_fields = []  # non-FTS index fields
@@ -1077,21 +1183,21 @@
             if (not(field.hidden)):
                 if field.index and field.fts_enabled():
                     index_fields.append(field)
                 elif field.index and not(field.fts_enabled()):
                     default_index_fields.append(field)
                 fields.append(field)
         if len(index_fields) == 0:
-            raise IndexError("Schema does not have a single indexable field.")
+            raise IndexError("Schema does not have a single indexable FTS field.")
         sql_table = '''
         CREATE TABLE IF NOT EXISTS %s(%s)
         ''' % (index_name, ", ".join([field.to_sql() for field in fields]))
         sql_virtual_table = '''
-        CREATE VIRTUAL TABLE IF NOT EXISTS %s_fts USING fts5(%s, content='%s', content_rowid='id' %s);
-        ''' % (index_name, ", ".join([field.to_sql(index_table=True) for field in fields if field.fts_enabled()]), index_name, self._create_additional_options())
+        CREATE VIRTUAL TABLE IF NOT EXISTS %s_fts USING fts5(%s, content='%s', content_rowid='id' %s %s);
+        ''' % (index_name, ", ".join([field.to_sql(index_table=True) for field in fields if field.fts_enabled()]), index_name, self._create_additional_options(), self._create_prefix_index())
         # Trigger definitions:
         sql_trigger_insert = '''
         CREATE TRIGGER IF NOT EXISTS {index_name}_ai AFTER INSERT ON {index_name} BEGIN
         INSERT INTO {index_name}_fts(rowid, {cols}) VALUES (new.id, {new_cols});
         END;'''
         sql_trigger_delete = '''
         CREATE TRIGGER IF NOT EXISTS {index_name}_ad AFTER DELETE ON {index_name} BEGIN
@@ -1130,15 +1236,15 @@
                 referenced_fields[comp[0]].append(self.Lookup(["eq"], kwargs[kwarg]))
         for f, lookups in referenced_fields.items():
             if f not in self.schema.fields:
                 raise self.FieldError("Unknown field '%s' - it is not defined in the schema." % f)
             for lookup in lookups:
                 for name in lookup.names:
                     if not(name) in LOOKUPS:
-                        raise self.FieldError("Unknown lookup: '%s' in %s" % (lookup, f))
+                        raise self.FieldError("Unknown lookup: '%s' in field '%s'" % (name, f))
         arguments = {}
         for field in self.schema:
             if field.name not in referenced_fields and not(for_search) and field.name not in ["id", "rank"]:
                 raise self.FieldError("Missing field '%s' in keyword arguments." % field.name)
             if field.name in referenced_fields:
                 arguments[field.name] = self.Argument(field, referenced_fields[field.name])
         return arguments
@@ -1251,20 +1357,26 @@
         the rowid is not found, no deletion is done and no error is thrown.
         '''
         self.assure_writeable()
         sql = "delete from %s where id = ?" % (self.schema.name)
         self.cursor.execute(sql, (rowid,))
         self.commit()
 
-    def search(self, **kwargs):
+    def search(self, *args, **kwargs):
         '''
         Searches the index. Keyword arguments must correspond to
         '''
+        if len(args)>0 and len(kwargs)>0:
+            raise Query.QueryError("Cannot mix Q objects and keyword arguments.")
+        if len(args)>0:
+            for q_expr in args[0]:
+                q_expr.arguments = self.get_arguments(q_expr.kwargs)
+            return Query(search_instance=self,arguments=[],q_arguments=args[0])
         arguments = self.get_arguments(kwargs)
-        return Query(self, arguments)
+        return Query(search_instance=self, arguments=arguments,q_arguments=[])
 
 
 class IndexReader(abc.ABC):
     '''
     An abstract base class for index readers. Reader classes
     scan through a source (e.g. the file system or some web site)
     and retrieve documents that should be indexed.
```

### Comparing `pocketsearch-0.8.0/src/pocketsearch/tests.py` & `pocketsearch-0.9.0/src/pocketsearch/tests.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 import unittest
 import tempfile
 import datetime
 
-from pocketsearch import FileSystemReader, Text, PocketSearch, Schema, Query, Field, Int, Real, Blob, Date, Datetime, IdField
+from pocketsearch import FileSystemReader, Text, PocketSearch, Schema, Query, Field, Int, Real, Blob, Date, Datetime, IdField, Q
 
 
 class Movie(Schema):
     '''
     A simple movie schema we use for tests.
     '''
 
@@ -156,14 +156,25 @@
         # by default, prefix search is not supported:
         self.assertEqual(self.pocket_search.search(text="fran*").count(), 0)
 
     def test_search_prefix_explicit(self):
         # by default, prefix search is not supported:
         self.assertEqual(self.pocket_search.search(text__allow_prefix="fran*").count(), 1)
 
+    def test_initial_token_queries_implicit(self):
+        self.pocket_search.insert(text="Paris is not the capital of england.")
+        # in this case, the ^ operator will be ignored and 2 matches found:
+        self.assertEqual(self.pocket_search.search(text="^england").count(), 2)
+
+    def test_initial_token_queries_explicit(self):
+        self.pocket_search.insert(text="Paris is not the capital of england.")
+        # search for results where england can be found at the begining:
+        self.assertEqual(self.pocket_search.search(text__allow_initial_token="^england").count(), 1)
+        self.assertEqual(self.pocket_search.search(text__allow_initial_token__allow_prefix="^engl*").count(),1)
+
     def test_search_and_or_query_default(self):
         # by default, AND/OR queries are not supported:
         self.assertEqual(self.pocket_search.search(text='france AND paris').count(), 0)
         self.assertEqual(self.pocket_search.search(text='france OR paris').count(), 0)
 
     def test_combined_lookups(self):
         self.assertEqual(self.pocket_search.search(text__allow_boolean__allow_prefix='france OR engl*').count(), 2)
@@ -174,14 +185,81 @@
         self.assertEqual(self.pocket_search.search(text__allow_boolean='france OR paris').count(), 1)
         self.assertEqual(self.pocket_search.search(text__allow_boolean='france OR england OR fence').count(), 3)
 
     def test_negation_default(self):
         # By default, negation is not supported
         self.assertEqual(self.pocket_search.search(text="NOT france").count(), 0)
 
+class PrefixIndexTest(unittest.TestCase):
+    '''
+    Test creation of prefix indices
+    '''
+
+    class PrefixIndex1(Schema):
+        '''
+        Simple schema that sets a prefix index for 
+        2,3 and 4 characters
+        '''
+        class Meta:
+            prefix_index=[2,3,4]
+        body = Text(index=True)
+
+    class PrefixIndex2(Schema):
+        '''
+        Prefix index definition with negative numbers
+        '''
+        class Meta:
+            prefix_index=[2,-3,4]
+        body = Text(index=True)
+
+    class PrefixIndex3(Schema):
+        '''
+        Prefix index definition, wrong data type
+        '''
+        class Meta:
+            prefix_index="2,3,4"
+
+        body = Text(index=True)
+
+    class PrefixIndex4(Schema):
+        '''
+        Prefix index definition with duplicate values
+        '''
+        class Meta:
+            prefix_index=[2,2,4]
+        body = Text(index=True)        
+
+    class PrefixIndex5(Schema):
+        '''
+        Prefix index definition with duplicate values
+        '''
+        class Meta:
+            prefix_index=[0,1]
+        body = Text(index=True)  
+
+    class PrefixIndex6(Schema):
+        '''
+        Prefix index definition with non-integer values
+        '''
+        class Meta:
+            prefix_index=["0",1]
+        body = Text(index=True) 
+
+    def test_create_prefix_index(self):
+        '''
+        Test creation of prefix index
+        '''
+        PocketSearch(schema=self.PrefixIndex1)
+        with self.assertRaises(Schema.SchemaError):
+            PocketSearch(schema=self.PrefixIndex2)
+        with self.assertRaises(Schema.SchemaError):            
+            PocketSearch(schema=self.PrefixIndex3)
+        PocketSearch(schema=self.PrefixIndex4)
+        with self.assertRaises(Schema.SchemaError):
+            PocketSearch(schema=self.PrefixIndex6)
 
 class PhraseSearch(unittest.TestCase):
 
     def test_search_phrase(self):
         pocket_search = PocketSearch(writeable=True)
         pocket_search.insert(text="This is a phrase")
         pocket_search.insert(text="a phrase this is")
@@ -269,53 +347,82 @@
         results = self.pocket_search.search(text="is")[0:2]
         results[0]
 
     def test_iteration(self):
         for idx, item in enumerate(self.pocket_search.search(text="is")):
             item.text  # just check, if it possible to call the attribute
 
-    def test_combine_search_results_1(self):
-        '''
-        These are all invalid queries. When we perform
-        a union order by or value arguments cannot be
-        provided. UC: order_by in second query
-        '''
-        with self.assertRaises(Query.QueryError):
-            q = self.pocket_search.search(text="paris") | self.pocket_search.search(text="england").order_by("rank")
-
-    def test_combine_search_results_2(self):
-        '''
-        These are all invalid queries. When we perform
-        a union order by or value arguments cannot be
-        provided. UC: order_by in first query
-        '''
-        with self.assertRaises(Query.QueryError):
-            q = self.pocket_search.search(text="paris").order_by("rank") | self.pocket_search.search(text="england")
-
-    def test_combine_search_results_3(self):
-        '''
-        These are all invalid queries. When we perform
-        a union order by or value arguments cannot be
-        provided.  UC: values in both queries
-        '''        
-        with self.assertRaises(Query.QueryError):
-            q = self.pocket_search.search(text="paris").values("id") | self.pocket_search.search(text="paris").values("id")
-
-    def test_combine_search_results(self):
-        # This is a correct query:
-        q1 = self.pocket_search.search(text="paris") | self.pocket_search.search(text="england")
-        self.assertEqual(q1.count(), 2)
-
     def test_order_by_override_default_order_by(self):
         # This should override the default rank sorting by the text sorting
         r = self.pocket_search.search(text="is").values("id", "rank", "text").order_by("-text")
         self.assertEqual(r[0].text, self.data[0])
         self.assertEqual(r[1].text, self.data[2])
         self.assertEqual(r[2].text, self.data[1])
 
+class QTests(unittest.TestCase):
+    '''
+    Tests the behavior of the Q operator
+    '''
+
+    class Product(Schema):
+        '''
+        Schema with Two-field FTS index
+        '''
+        code = Text(index=True)
+        product = Text(index=True)
+        price = Int()
+
+    def setUp(self):
+        self.pocketsearch = PocketSearch(schema=self.Product)
+        for code,name,price in [
+            ("A01","Apple",4),
+            ("A02","Peach",7),
+            ("A03","Orange",8),
+            ("B01","Grapefruit",5),
+            ("B02","Banana",9),
+            ("C01","Apple and Orange",3),            
+        ]:
+            self.pocketsearch.insert(code=code,product=name,price=price)
+
+    def test_phrase_query(self):
+        q = self.pocketsearch.search(Q(product='"apple and orange"'))
+        self.assertEqual(q.count(),1)        
+        q = self.pocketsearch.search(Q(product='orange and apple'))
+        self.assertEqual(q.count(),1)        
+
+    def test_initial_token_query(self):
+        # This should only bring one result back:
+        q = self.pocketsearch.search(Q(price__gte=3) & Q(product__allow_initial_token="^Orange"))
+        self.assertEqual(q.count(),1)
+
+    def test_and(self):
+        q = self.pocketsearch.search(Q(product="Apple") & Q(code__allow_prefix="A*") & Q(price__gte=2))
+        self.assertEqual(q.count(),1)
+        # Test the other way around:
+        q = self.pocketsearch.search(Q(price__gte=2) & Q(product="Apple") & Q(code__allow_prefix="A*"))
+        self.assertEqual(q.count(),1)        
+        # Mixed
+        q = self.pocketsearch.search(Q(code__allow_prefix="A*") & Q(price__gte=2) & Q(product="Apple"))
+        self.assertEqual(q.count(),1) 
+
+    def test_or(self):
+        q = self.pocketsearch.search(Q(price__gte=9) | Q(price__lte=3)) 
+        self.assertEqual(q.count(),2)
+
+    def test_combined_and_or(self):
+        q = self.pocketsearch.search(Q(price__gte=1) & Q(price__lte=5) & Q(product="Apple") | Q(product="Orange"))
+        self.assertEqual(q.count(),2)
+
+    def test_mixed_q_query(self):
+        with self.assertRaises(Query.QueryError):
+            self.pocketsearch.search(Q(price__gte=1) & Q(price__lte=5), product="apple")
+
+    def test_q_objects_multiple_kw_arguments(self):
+        with self.assertRaises(Query.QueryError):
+            self.pocketsearch.search(Q(price__gte=1,price__lte=5))
 
 class IDFieldTest(unittest.TestCase):
 
     class IdSchema(Schema):
 
         text = Text(index=True)
         file_name = Text(is_id_field=True)
```

### Comparing `pocketsearch-0.8.0/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.9.0/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.8.0
+Version: 0.9.0
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -19,19 +19,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Indexing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pocketsearch
-pocketsearch is a pure-Python full text indexing search engine based on sqlite and the FTS5 extension. It provides
+pocketsearch is a pure-Python full text indexing search engine based on sqlite and the [FTS5](https://www.sqlite.org/fts5.html) extension. It provides
 
-- Support for full text search
 - A simple API (inspired by the ORM layer of the Django web framework) for defining schemas and searching
 - Support for multi-field indices including text, numeric and date search
+- Support for prefix and initial token queries
 
 It does not have any external dependencies other than Python itself. pocketsearch has been tested on Python 3.8, 
 Python 3.9, Python 3.10 and Python 3.11.
 
 pocketsearch is currently being tested on data from Wikipedia, indexing more than 6 million abstracts. If you 
 are interested in preliminary performance tests, have a look at https://github.com/kaykay-dv/pocketsearch/tree/development/tests.
 
@@ -118,14 +118,29 @@
 If you want to search for substrings, you can use prefix queries, by 
 providing the allow_prefix lookup:
 
 ```Python
 print(pocket_search.search(text__allow_prefix="hel*")[0].text)
 ```
 
+Please note, that prefix queries might get very slow as the index grows. To 
+optimize performance, you can use prefix indices as described in the chapter 
+on "schemas" in this README.
+
+## Initial token queries
+
+If you want to search only the first token at the begining of a document, use the 
+allow_initial_token lookup:
+
+```Python
+pocket_search.search(text__allow_initial_token="^hello")
+```
+
+This will only match results that have 'hello' at the very beginning. 
+
 ## Phrase queries
 
 If you want to search for phrases, use quotation marks:
 
 ```Python
 pocket_search.search(text='"this is" "a phrase"').count()
 ```
@@ -170,15 +185,15 @@
 [Hello] World !
 ```
 
 The positional arguments of the highlight method represent the fields you want to hightlight. 
 
 If you have very long text, you might want to only show a snippet with all terms found in your +
 search results. This can be done with the snippet method. Assuming we have the article 
-on inverted indices (https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
+on Wikipedia article on [inverted indices](https://en.wikipedia.org/wiki/Inverted_index) in our database we can extract snippets like this:
 
 ```Python
 pocket_search.search(text="inverted file").snippet("text",snippet_length=16)[0].text
 'In computer science, an *inverted* index (also referred to as a postings list, postings *file*, or...'
 ```
 
 Similar to the highlight method, the snippet method highlights tokens found. snippet_length defines 
@@ -220,48 +235,80 @@
 | Numeric      | Numeric  |
 | Blob         | Blob  |
 | Date         | Date  |
 | Datetime     | Datetime  |
 
 Following options are available for fields:
 
-* index - if the field is a Text field, a full text search index is created, otherwise a standard sqlite3 index is created
-* is_id_field - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
+* **index** - if the field is a Text field, a full text search index is created, otherwise a standard sqlite3 index is created
+* **is_id_field** - a schema can only have one IDField. It is used by the .insert_or_update method to decide if a document should be inserted or an existing document should be updated.
 
 With respect to naming your fields following restrictions apply:
 
 * Fields may not start with an underscore.
 * Fields may not contain double underscores.
 
-> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document.
+Moreover field names may not be composed of reserved SQL keywords.
+
+> **_NOTE:_**  While not explicitly set, pocketsearch automatically adds an "id" field to the schema (using the INTEGER data type plus the AUTOINCREMENT option of sqlite). It is used as the primary key for each document. The ID field is used to delete or 
+update documents.
+
+## Queries on multi-field indices
 
 Once the schema is created, you can query multiple fields:
 
 ```Python
 # Searches field text for "world"
 pocket_search.search(text="world")
 # Searches documents that contain "world" in text AND have "a.txt" is a filename.
 # Please note: as "filename" has not set its index option, only exact matches 
 # will be considered.
 pocket_search.search(text="world",filename="a.txt")
 ```
 
-> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND. Currently, there is no way to express OR queries in the .search method.
+> **_NOTE:_**  When using multiple fields in search, the default boolean operation is AND.
+
+### AND/OR queries on multiple fields
 
-However, you can join 2 queries (resulting in a UNION statement in SQL):
+Similar to the Django web framework, you can use "Q Objects" to express OR queries on multiple fields:
 
 ```Python
-q = pocket_search.search(text="world") | pocket_search.search(filename="a.txt")
-for result in q:
-    print(result.text)
+from pocketsearch import Q
+# Search for documents where text="world" OR filename="a.txt"
+q = pocket_search.search(Q(text="world") | Q(filename="a.txt"))
+# Search for documents where text="world" AND filename="a.txt"
+q = pocket_search.search(Q(text="world") & Q(filename="a.txt"))
 ```
 
-The result will contain all documents containing either "world" or where the filename is "a.text".
+Please note, that you either have to use one notation or the other. You cannot mix 
+Q objects with keyword arguments and you can only provide one field per Q object:
+
+```Python
+# This will NOT work:
+pocket_search.search(Q(text="world") , filename="a.txt")
+# This will work neither:
+pocket_search.search(Q(text="world",filename="a.txt"))
+```
+
+
+## Setting prefix indices
+To speed up prefix queries, you can setup prefix indices:
+
+```Python
+    class PrefixIndex1(Schema):
+        '''
+        Simple schema that sets a prefix index for 
+        2,3 and 4 characters
+        '''
+        class Meta:
+            prefix_index=[2,3,4]
+        body = Text(index=True)
+```
 
-This option is currently experimental and still has issues, espcially when accessing results through indexing. 
+This will create prefix indices for 2,3 and 4 character prefixes.
 
 # Inserting, updating and deleting data
 
 ## Handling updates and deletes
 
 Using the id of a document, you can run updates:
 
@@ -431,17 +478,17 @@
         sqlite_tokenchars = None
         sqlite_separators = None    
 
     text = Text(index=True)
     filename = Text(is_id_field=True)
 ```
 
-# Multiple indicies in one database
+# Multiple indices in one database
 
-You can have multiple indicies in one database (only databases written to disk) by setting 
+You can have multiple indices in one database (only databases written to disk) by setting 
 the "index_name" option:
 
 ```Python
 pocket_search = PocketSearch(db_name="my_db.db",index_name="Product",schema=Product)
 ```
 
 # Contribute
```

