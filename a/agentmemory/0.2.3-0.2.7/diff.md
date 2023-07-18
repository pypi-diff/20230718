# Comparing `tmp/agentmemory-0.2.3.tar.gz` & `tmp/agentmemory-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.2.3.tar", last modified: Fri Jul 14 11:38:18 2023, max compression
+gzip compressed data, was "agentmemory-0.2.7.tar", last modified: Tue Jul 18 13:44:27 2023, max compression
```

## Comparing `agentmemory-0.2.3.tar` & `agentmemory-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 11:38:18.405667 agentmemory-0.2.3/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.3/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 11:38:18.405429 agentmemory-0.2.3/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)    11205 2023-07-14 01:24:31.000000 agentmemory-0.2.3/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 11:38:18.403547 agentmemory-0.2.3/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1104 2023-07-14 11:38:14.000000 agentmemory-0.2.3/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    24951 2023-07-14 11:37:49.000000 agentmemory-0.2.3/agentmemory/main.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 11:38:18.405178 agentmemory-0.2.3/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 11:38:18.000000 agentmemory-0.2.3/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-14 11:38:18.000000 agentmemory-0.2.3/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-14 11:38:18.000000 agentmemory-0.2.3/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-14 11:38:18.000000 agentmemory-0.2.3/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-14 11:38:18.000000 agentmemory-0.2.3/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-14 11:38:18.405724 agentmemory-0.2.3/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-14 11:38:14.000000 agentmemory-0.2.3/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-18 13:44:27.321830 agentmemory-0.2.7/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.7/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11200 2023-07-18 13:44:27.321605 agentmemory-0.2.7/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)    10642 2023-07-18 13:18:07.000000 agentmemory-0.2.7/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-18 13:44:27.318996 agentmemory-0.2.7/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      881 2023-07-18 13:44:19.000000 agentmemory-0.2.7/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    24359 2023-07-18 13:20:57.000000 agentmemory-0.2.7/agentmemory/main.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-18 13:44:27.321296 agentmemory-0.2.7/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11200 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-18 13:44:27.321878 agentmemory-0.2.7/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1267 2023-07-18 13:44:19.000000 agentmemory-0.2.7/setup.py
```

### Comparing `agentmemory-0.2.3/LICENSE` & `agentmemory-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.2.3/PKG-INFO` & `agentmemory-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.2.3
+Version: 0.2.7
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -135,36 +135,35 @@
 delete_memory("conversation", 1)
 ```
 
 # Documentation
 
 ## Create a Memory
 
-#### `create_memory(category, text, id=None, embedding=None, metadata=None, persist=True)`
+#### `create_memory(category, text, id=None, embedding=None, metadata=None)`
 
 Create a new memory in a collection.
 
 ##### Arguments
 
 ```
 # Required
 category (str): Category of the collection.
 text (str): Document text.
 
 # Optional
 id (str): Unique id. Generated incrementally unless set.
 metadata (dict): Metadata.
 embedding (array): Embedding of the document. Defaults to None. Use if you already have an embedding.
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
->>> create_memory(category='sample_category', text='sample_text', id='sample_id', metadata={'sample_key': 'sample_value'}, persist=True)
+>>> create_memory(category='sample_category', text='sample_text', id='sample_id', metadata={'sample_key': 'sample_value'})
 ```
 
 ## Search Memory
 
 #### `search_memory(category, search_text, n_results=5, min_distance=None, max_distance=None, filter_metadata=None, contains_text=None, include_embeddings=True)`
 
 Search a collection with given query texts.
@@ -261,56 +260,54 @@
 
 ```python
 >>> get_memories("books", sort_order="asc", n_results=10)
 ```
 
 ## Update a Memory
 
-#### `update_memory(category, id, text=None, metadata=None, persist=True)`
+#### `update_memory(category, id, text=None, metadata=None)`
 
 Update a memory with new text and/or metadata.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category of the memory.
 id (str/int): The ID of the memory.
 
 # Optional
 text (str): The new text of the memory. Defaults to None.
 metadata (dict): The new metadata of the memory. Defaults to None.
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 # with keyword arguments
-update_memory(category="conversation", id=1, text="Okay, I will open the podbay doors.", metadata={ "speaker": "HAL", "sentiment": "positive" }, persist=True)
+update_memory(category="conversation", id=1, text="Okay, I will open the podbay doors.", metadata={ "speaker": "HAL", "sentiment": "positive" })
 
 # with positional arguments
 update_memory("conversation", 1, "Okay, I will open the podbay doors.")
 ```
 
 ## Delete a Memory
 
-#### `delete_memory(category, id, contains_metadata=None, contains_text=None, persist=True)`
+#### `delete_memory(category, id, contains_metadata=None, contains_text=None)`
 
 Delete a memory by ID.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category of the memory.
 id (str/int): The ID of the memory.
 
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> delete_memory("books", "1")
 ```
@@ -336,26 +333,25 @@
 
 ```python
 >>> memory_exists("books", "1")
 ```
 
 ## Wipe an Entire Category of Memories
 
-#### `wipe_category(category, persist=True)`
+#### `wipe_category(category)`
 
 Delete an entire category of memories.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category to delete.
 
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> wipe_category("books")
 ```
@@ -382,23 +378,22 @@
 
 ```python
 >>> count_memories("books")
 ```
 
 ## Wipe All Memories
 
-#### `wipe_all_memories(persist=True)`
+#### `wipe_all_memories()`
 
 Delete all memories across all categories.
 
 ##### Arguments
 
 ```
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> wipe_all_memories()
 ```
@@ -425,17 +420,14 @@
 
 ##### Example
 
 ```python
     >>> save_memory()
 ```
 
-Sure, here's a Markdown formatted version that can be used in a `README.md` file:
-
-````markdown
 # Memory Management with ChromaDB
 
 This document provides a guide to using the memory management functions provided in the module.
 
 ## Functions
 
 ### Export Memories to JSON
@@ -451,15 +443,14 @@
 - dict: A dictionary with collection names as keys and lists of memories as values.
 
 ##### Example
 
 ```python
 >>> export_memory_to_json()
 ```
-````
 
 ### Export Memories to File
 
 The `export_memory_to_file` function exports all memories to a JSON file, optionally including embeddings.
 
 ##### Arguments
 
@@ -506,13 +497,14 @@
 
 In the above Markdown, you may replace "ChromaDB" with the actual name of the module if it's different. You can include this in your `README.md` file to give your users a guide on how to use these functions.
 
 # Publishing
 
 ```bash
 bash publish.sh --version=<version> --username=<pypi_username> --password=<pypi_password>
-````
+```
 
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
+````
```

### Comparing `agentmemory-0.2.3/README.md` & `agentmemory-0.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -118,36 +118,35 @@
 delete_memory("conversation", 1)
 ```
 
 # Documentation
 
 ## Create a Memory
 
-#### `create_memory(category, text, id=None, embedding=None, metadata=None, persist=True)`
+#### `create_memory(category, text, id=None, embedding=None, metadata=None)`
 
 Create a new memory in a collection.
 
 ##### Arguments
 
 ```
 # Required
 category (str): Category of the collection.
 text (str): Document text.
 
 # Optional
 id (str): Unique id. Generated incrementally unless set.
 metadata (dict): Metadata.
 embedding (array): Embedding of the document. Defaults to None. Use if you already have an embedding.
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
->>> create_memory(category='sample_category', text='sample_text', id='sample_id', metadata={'sample_key': 'sample_value'}, persist=True)
+>>> create_memory(category='sample_category', text='sample_text', id='sample_id', metadata={'sample_key': 'sample_value'})
 ```
 
 ## Search Memory
 
 #### `search_memory(category, search_text, n_results=5, min_distance=None, max_distance=None, filter_metadata=None, contains_text=None, include_embeddings=True)`
 
 Search a collection with given query texts.
@@ -244,56 +243,54 @@
 
 ```python
 >>> get_memories("books", sort_order="asc", n_results=10)
 ```
 
 ## Update a Memory
 
-#### `update_memory(category, id, text=None, metadata=None, persist=True)`
+#### `update_memory(category, id, text=None, metadata=None)`
 
 Update a memory with new text and/or metadata.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category of the memory.
 id (str/int): The ID of the memory.
 
 # Optional
 text (str): The new text of the memory. Defaults to None.
 metadata (dict): The new metadata of the memory. Defaults to None.
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 # with keyword arguments
-update_memory(category="conversation", id=1, text="Okay, I will open the podbay doors.", metadata={ "speaker": "HAL", "sentiment": "positive" }, persist=True)
+update_memory(category="conversation", id=1, text="Okay, I will open the podbay doors.", metadata={ "speaker": "HAL", "sentiment": "positive" })
 
 # with positional arguments
 update_memory("conversation", 1, "Okay, I will open the podbay doors.")
 ```
 
 ## Delete a Memory
 
-#### `delete_memory(category, id, contains_metadata=None, contains_text=None, persist=True)`
+#### `delete_memory(category, id, contains_metadata=None, contains_text=None)`
 
 Delete a memory by ID.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category of the memory.
 id (str/int): The ID of the memory.
 
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> delete_memory("books", "1")
 ```
@@ -319,26 +316,25 @@
 
 ```python
 >>> memory_exists("books", "1")
 ```
 
 ## Wipe an Entire Category of Memories
 
-#### `wipe_category(category, persist=True)`
+#### `wipe_category(category)`
 
 Delete an entire category of memories.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category to delete.
 
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> wipe_category("books")
 ```
@@ -365,23 +361,22 @@
 
 ```python
 >>> count_memories("books")
 ```
 
 ## Wipe All Memories
 
-#### `wipe_all_memories(persist=True)`
+#### `wipe_all_memories()`
 
 Delete all memories across all categories.
 
 ##### Arguments
 
 ```
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> wipe_all_memories()
 ```
@@ -408,17 +403,14 @@
 
 ##### Example
 
 ```python
     >>> save_memory()
 ```
 
-Sure, here's a Markdown formatted version that can be used in a `README.md` file:
-
-````markdown
 # Memory Management with ChromaDB
 
 This document provides a guide to using the memory management functions provided in the module.
 
 ## Functions
 
 ### Export Memories to JSON
@@ -434,15 +426,14 @@
 - dict: A dictionary with collection names as keys and lists of memories as values.
 
 ##### Example
 
 ```python
 >>> export_memory_to_json()
 ```
-````
 
 ### Export Memories to File
 
 The `export_memory_to_file` function exports all memories to a JSON file, optionally including embeddings.
 
 ##### Arguments
 
@@ -489,14 +480,15 @@
 
 In the above Markdown, you may replace "ChromaDB" with the actual name of the module if it's different. You can include this in your `README.md` file to give your users a guide on how to use these functions.
 
 # Publishing
 
 ```bash
 bash publish.sh --version=<version> --username=<pypi_username> --password=<pypi_password>
-````
+```
 
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
 <img src="resources/youcreatethefuture.jpg">
+````
```

### Comparing `agentmemory-0.2.3/agentmemory/main.py` & `agentmemory-0.2.7/agentmemory/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 import os
 import datetime
 
 import chromadb
 
-persistent_path = None
+persist_directory = None
 client = None
 
 
-def create_memory(category, text, metadata={}, embedding=None, id=None, persist=True):
+def create_memory(category, text, metadata={}, embedding=None, id=None):
     """
     Create a new memory in a collection.
 
     Arguments:
     category (str): Category of the collection.
     text (str): Document text.
     id (str): Unique id.
     metadata (dict): Metadata.
-    persist (bool, optional): Whether to persist the changes to disk. Defaults to True.
 
     Returns:
     None
 
     Example:
     >>> create_memory('sample_category', 'sample_text', id='sample_id', metadata={'sample_key': 'sample_value'})
     """
@@ -37,25 +36,29 @@
 
     # if no id is provided, generate one based on count of documents in collection
     if id is None:
         id = str(memories.count())
         # pad the id with zeros to make it 16 digits long
         id = id.zfill(16)
 
+    # for each field in metadata...
+    # if the field is a boolean, convert it to a string
+    for key, value in metadata.items():
+        if isinstance(value, bool):
+            print(f"WARNING: Boolean metadata field {key} converted to string")
+            metadata[key] = str(value)
+
     # insert the document into the collection
     memories.upsert(
         ids=[str(id)],
         documents=[text],
         metadatas=[metadata],
         embeddings=[embedding] if embedding is not None else None,
     )
 
-    if persist:
-        persist_memory()
-
     debug_log(f"Created memory {id}: {text}", metadata)
 
 
 def search_memory(
     category,
     search_text,
     n_results=5,
@@ -95,23 +98,32 @@
     # check if contains_text is provided and format it for the query
     if contains_text is not None:
         contains_text = {"$contains": contains_text}
 
     # get or create the collection
     memories = client.get_or_create_collection(category)
 
-    if(memories.count()) == 0:
+    if (memories.count()) == 0:
         return []
 
     # min n_results to prevent searching for more elements than are available
     n_results = min(n_results, memories.count())
 
     # get the types to include
     include_types = get_include_types(include_embeddings, include_distances)
 
+    # filter_metadata is a dictionary of metadata to filter by
+    if filter_metadata is not None and len(filter_metadata.keys()) > 1:
+        # map each key:value in filter_metadata to an object shaped like { "key": { "$eq": "value" } }
+        filter_metadata = [
+            {key: {"$eq": value}} for key, value in filter_metadata.items()
+        ]
+
+        filter_metadata = {"$and": filter_metadata}
+
     # perform the query and get the response
     query = memories.query(
         query_texts=[search_text],
         where=filter_metadata,
         where_document=contains_text,
         n_results=n_results,
         include=include_types,
@@ -211,14 +223,23 @@
     include_types = get_include_types(include_embeddings, False)
 
     where_document = None
 
     if contains_text is not None:
         where_document = {"$contains": contains_text}
 
+    # filter_metadata is a dictionary of metadata to filter by
+    if filter_metadata is not None and len(filter_metadata.keys()) > 1:
+        # map each key:value in filter_metadata to an object shaped like { "key": { "$eq": "value" } }
+        filter_metadata = [
+            {key: {"$eq": value}} for key, value in filter_metadata.items()
+        ]
+
+        filter_metadata = {"$and": filter_metadata}
+
     # Retrieve all memories that meet the given metadata filter
     memories = memories.get(
         where=filter_metadata, where_document=where_document, include=include_types
     )
 
     # Convert the collection to list format
     memories = chroma_collection_to_list(memories)
@@ -230,24 +251,23 @@
     memories = memories[:n_results]
 
     debug_log(f"Got memories from category {category}", memories)
 
     return memories
 
 
-def update_memory(category, id, text=None, metadata=None, persist=True):
+def update_memory(category, id, text=None, metadata=None):
     """
     Update a memory with new text and/or metadata.
 
     Arguments:
         category (str): The category of the memory.
         id (str/int): The ID of the memory.
         text (str, optional): The new text of the memory. Defaults to None.
         metadata (dict, optional): The new metadata of the memory. Defaults to None.
-        persist (bool, optional): Whether to persist the changes to disk. Defaults to True.
 
     Returns:
         None
 
     Raises:
         Exception: If neither text nor metadata is provided.
 
@@ -268,31 +288,27 @@
 
     documents = [text] if text is not None else None
     metadatas = [metadata] if metadata is not None else None
 
     # Update the memory with the new text and/or metadata
     memories.update(ids=[str(id)], documents=documents, metadatas=metadatas)
 
-    if persist:
-        persist_memory()
-
     debug_log(
         f"Updated memory {id} in category {category}",
         {"documents": documents, "metadatas": metadatas},
     )
 
 
-def delete_memory(category, id, persist=True):
+def delete_memory(category, id):
     """
     Delete a memory by ID.
 
     Arguments:
         category (str): The category of the memory.
         id (str/int): The ID of the memory.
-        persist (bool, optional): Whether to persist the changes to disk. Defaults to True.
 
     Returns:
         None
 
     Example:
         >>> delete_memory("books", "1")
     """
@@ -304,17 +320,14 @@
 
     if memory_exists(category, id) is False:
         debug_log(f"WARNING: Tried could not delete memory {id} in category {category}")
         return
     # Delete the memory
     memories.delete(ids=[str(id)])
 
-    if persist:
-        persist_memory()
-
     debug_log(f"Deleted memory {id} in category {category}")
 
 
 def memory_exists(category, id, includes_metadata=None):
     """
     Check if a memory with a specific ID exists in a given category.
 
@@ -344,40 +357,36 @@
         f"Checking if memory {id} exists in category {category}. Exists: {exists}"
     )
 
     # Return True if at least one memory was found, False otherwise
     return exists
 
 
-def wipe_category(category, persist=True):
+def wipe_category(category):
     """
     Delete an entire category of memories.
 
     Arguments:
         category (str): The category to delete.
-        persist (bool, optional): Whether to persist the changes to disk. Defaults to True.
 
     Example:
         >>> wipe_category("books")
     """
 
     collection = None
 
     try:
         collection = client.get_collection(category)  # Check if the category exists
-    except:
-        pass
+    except Exception:
+        debug_log(f"WARNING: Tried to wipe category {category} but it does not exist")
 
     if collection is not None:
         # Delete the entire category
         client.delete_collection(category)
 
-        if persist:
-            client.persist()
-
 
 def count_memories(category):
     """
     Count the number of memories in a given category.
 
     Arguments:
         category (str): The category of the memories.
@@ -396,117 +405,88 @@
 
     debug_log(f"Counted memories in {category}: {memories.count()}")
 
     # Return the count of memories
     return memories.count()
 
 
-def wipe_all_memories(persist=True):
+def wipe_all_memories():
     """
     Delete all memories across all categories.
 
-    Arguments:
-        persist (bool, optional): Whether to persist the changes to disk. Defaults to True.
-
     Example:
         >>> wipe_all_memories()
     """
 
     check_client_initialized()  # client is lazy loaded, so make sure it is is initialized
+    client = get_chroma_client()
+    collections = client.list_collections()
 
-    # Reset the entire client, which deletes all collections and their memories
-    client.reset()
+    # Iterate over all collections
+    for collection in collections:
+        client.delete_collection(collection.name)
 
-    if persist:
-        persist_memory()
 
-    debug_log(f"Wiped all memories")
+    debug_log("Wiped all memories")
 
 
 def check_client_initialized():
     """
     Check if the client has been initialized, and initialize it if not.
 
     Example:
         >>> check_client_initialized()
     """
     global client
+    global persist_directory
     if client is None:
-        if persistent_path is not None:
-            client = chromadb.Client(
-                chromadb.Settings(
-                    chroma_db_impl="duckdb+parquet", persist_directory=persistent_path
-                )
-            )
-        else:
-            client = chromadb.Client(
-                chromadb.Settings(
-                    chroma_db_impl="duckdb+parquet", persist_directory="./memory"
-                )
-            )
+        if persist_directory is None:
+            persist_directory="./memory"
+        
+        client = chromadb.PersistentClient(persist_directory)
 
     debug_log(f"Checking if client is initialized")
 
 
 def set_storage_path(path):
     """
     Set the path to persist the database to.
 
     Arguments:
         path (string): the path to save to
 
     Example:
         >>> set_storage_path("path/to/persistent/directory")
     """
-    global persistent_path
+    global persist_directory
     global client
-    persistent_path = path
-    if client is not None:
-        persist_memory()
-    client = chromadb.Client(
-        chromadb.Settings(
-            chroma_db_impl="duckdb+parquet", persist_directory=persistent_path
-        )
-    )
+    persist_directory = path
+
+    # reset path
+    if persist_directory is None:
+            persist_directory="./memory"
+    
+    client = chromadb.PersistentClient(persist_directory)
 
     debug_log(f"Set storage path to {path}")
 
 
 def save_memory():
     """
     Save the database to disk.
 
     Example:
         >>> save_to_disk()
     """
     check_client_initialized()  # client is lazy loaded, so make sure it is is initialized
-    persist_memory()
 
     debug_log(f"Saved memory")
 
 
 def export_memory_to_json(include_embeddings=True):
-    collections = get_chroma_client().list_collections()
-
-    print("Collections")
-    print(collections)
-
-    collections_dict = {}
-
-    for collection in collections:
-        print(collection)
-        collection_name = collection["name"]
-        collections_dict[collection_name] = []
-        memories = get_memories(collection_name, include_embeddings=include_embeddings)
-        for memory in memories:
-            collections_dict[collection_name].append(memory)
-    return collections_dict
-
-
-def export_memory_to_json(include_embeddings=True):
     """
     Export all memories to a dictionary, optionally including embeddings.
 
     Arguments:
         include_embeddings (bool, optional): Whether to include memory embeddings in the output.
                                              Defaults to True.
 
@@ -573,33 +553,29 @@
 
     Example:
         >>> import_json_to_memory(data)
     """
 
     # If replace flag is set to True, wipe out all existing memories
     if replace:
-        wipe_all_memories(False)
+        wipe_all_memories()
 
     # Iterate over all collections in the input data
     for category in data:
         # Iterate over all memories in the current collection
         for memory in data[category]:
             # Create a new memory in the current category
             create_memory(
                 category,
                 text=memory["document"],
                 metadata=memory["metadata"],
                 id=memory["id"],
                 embedding=memory.get("embedding", None),
-                persist=False,
             )
 
-    # Once all memories have been created, persist them to disk
-    persist_memory()
-
 
 def import_file_to_memory(path="./memory.json", replace=True):
     """
     Import memories from a JSON file into the current database.
 
     Arguments:
         path (str, optional): The path to the input file. Defaults to "./memory.json".
@@ -625,34 +601,28 @@
     # Check if the DEBUG_MEMORY environment variable is set to 'true'
     if os.getenv("DEBUG_MEMORY", "false").lower() == "true":
         if dict is not None:
             message = message + f" ({json.dumps(dict)})"
         print(message)
 
 
-def persist_memory():
-    if persistent_path is not None:
-        client.persist()
-        debug_log(f"Persisted memory")
-
-
 def get_chroma_client():
     """
     Get the chromadb client.
 
     Returns:
     chromadb.Client: Chromadb client.
 
     Example:
     >>> get_chroma_client()
     <chromadb.client.Client object at 0x7f7b9c2f0d00>
     """
     global client
     check_client_initialized()  # client is lazy loaded, so make sure it is is initialized
-    debug_log(f"Getting chroma client")
+    debug_log("Getting chroma client")
     return client
 
 
 def chroma_collection_to_list(collection):
     """
     Function to convert collection (dictionary) to list.
 
@@ -713,15 +683,15 @@
                 "metadata": metadata,
                 "document": document,
                 "embedding": embedding,
                 "distance": distance,
                 "id": id,
             }
         )
-    debug_log(f"Collection to list", {"collection": collection, "list": list})
+    debug_log("Collection to list", {"collection": collection, "list": list})
     return list
 
 
 def list_to_chroma_collection(list):
     """
     Function to convert list (of dictionaries) to collection (dictionary).
 
@@ -759,15 +729,15 @@
     # delete keys from collection if no values are present
     if len(collection["embeddings"]) == 0:
         del collection["embeddings"]
 
     if len(collection["distances"]) == 0:
         del collection["distances"]
 
-    debug_log(f"List to collection", {"collection": collection, "list": list})
+    debug_log("List to collection", {"collection": collection, "list": list})
     return collection
 
 
 def flatten_arrays(collection):
     """
     Function to flatten the arrays in the collection.
 
@@ -781,15 +751,15 @@
     >>> flatten_arrays(collection)
     {'metadatas': ['...'], 'documents': ['...'], 'ids': ['...'], 'embeddings': ['...'], 'distances': ['...']}
     """
 
     # Iterate over each key in collection
     for key in collection:
         # If no values, continue to next iteration
-        if collection[key] == None:
+        if collection[key] is None:
             continue
         # Flatten the arrays into a single array for each key
         collection[key] = [item for sublist in collection[key] for item in sublist]
 
     return collection
 
 
@@ -815,9 +785,9 @@
     if include_embeddings:
         include_types.append("embeddings")
 
     # include distances if specified
     if include_distances:
         include_types.append("distances")
 
-    debug_log(f"Get include types", {"include_types": include_types})
+    debug_log("Get include types", {"include_types": include_types})
     return include_types
```

### Comparing `agentmemory-0.2.3/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.2.7/agentmemory.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.2.3
+Version: 0.2.7
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -135,36 +135,35 @@
 delete_memory("conversation", 1)
 ```
 
 # Documentation
 
 ## Create a Memory
 
-#### `create_memory(category, text, id=None, embedding=None, metadata=None, persist=True)`
+#### `create_memory(category, text, id=None, embedding=None, metadata=None)`
 
 Create a new memory in a collection.
 
 ##### Arguments
 
 ```
 # Required
 category (str): Category of the collection.
 text (str): Document text.
 
 # Optional
 id (str): Unique id. Generated incrementally unless set.
 metadata (dict): Metadata.
 embedding (array): Embedding of the document. Defaults to None. Use if you already have an embedding.
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
->>> create_memory(category='sample_category', text='sample_text', id='sample_id', metadata={'sample_key': 'sample_value'}, persist=True)
+>>> create_memory(category='sample_category', text='sample_text', id='sample_id', metadata={'sample_key': 'sample_value'})
 ```
 
 ## Search Memory
 
 #### `search_memory(category, search_text, n_results=5, min_distance=None, max_distance=None, filter_metadata=None, contains_text=None, include_embeddings=True)`
 
 Search a collection with given query texts.
@@ -261,56 +260,54 @@
 
 ```python
 >>> get_memories("books", sort_order="asc", n_results=10)
 ```
 
 ## Update a Memory
 
-#### `update_memory(category, id, text=None, metadata=None, persist=True)`
+#### `update_memory(category, id, text=None, metadata=None)`
 
 Update a memory with new text and/or metadata.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category of the memory.
 id (str/int): The ID of the memory.
 
 # Optional
 text (str): The new text of the memory. Defaults to None.
 metadata (dict): The new metadata of the memory. Defaults to None.
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 # with keyword arguments
-update_memory(category="conversation", id=1, text="Okay, I will open the podbay doors.", metadata={ "speaker": "HAL", "sentiment": "positive" }, persist=True)
+update_memory(category="conversation", id=1, text="Okay, I will open the podbay doors.", metadata={ "speaker": "HAL", "sentiment": "positive" })
 
 # with positional arguments
 update_memory("conversation", 1, "Okay, I will open the podbay doors.")
 ```
 
 ## Delete a Memory
 
-#### `delete_memory(category, id, contains_metadata=None, contains_text=None, persist=True)`
+#### `delete_memory(category, id, contains_metadata=None, contains_text=None)`
 
 Delete a memory by ID.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category of the memory.
 id (str/int): The ID of the memory.
 
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> delete_memory("books", "1")
 ```
@@ -336,26 +333,25 @@
 
 ```python
 >>> memory_exists("books", "1")
 ```
 
 ## Wipe an Entire Category of Memories
 
-#### `wipe_category(category, persist=True)`
+#### `wipe_category(category)`
 
 Delete an entire category of memories.
 
 ##### Arguments
 
 ```
 # Required
 category (str): The category to delete.
 
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> wipe_category("books")
 ```
@@ -382,23 +378,22 @@
 
 ```python
 >>> count_memories("books")
 ```
 
 ## Wipe All Memories
 
-#### `wipe_all_memories(persist=True)`
+#### `wipe_all_memories()`
 
 Delete all memories across all categories.
 
 ##### Arguments
 
 ```
 # Optional
-persist (bool): Whether to persist the changes to disk. Defaults to True.
 ```
 
 ##### Example
 
 ```python
 >>> wipe_all_memories()
 ```
@@ -425,17 +420,14 @@
 
 ##### Example
 
 ```python
     >>> save_memory()
 ```
 
-Sure, here's a Markdown formatted version that can be used in a `README.md` file:
-
-````markdown
 # Memory Management with ChromaDB
 
 This document provides a guide to using the memory management functions provided in the module.
 
 ## Functions
 
 ### Export Memories to JSON
@@ -451,15 +443,14 @@
 - dict: A dictionary with collection names as keys and lists of memories as values.
 
 ##### Example
 
 ```python
 >>> export_memory_to_json()
 ```
-````
 
 ### Export Memories to File
 
 The `export_memory_to_file` function exports all memories to a JSON file, optionally including embeddings.
 
 ##### Arguments
 
@@ -506,13 +497,14 @@
 
 In the above Markdown, you may replace "ChromaDB" with the actual name of the module if it's different. You can include this in your `README.md` file to give your users a guide on how to use these functions.
 
 # Publishing
 
 ```bash
 bash publish.sh --version=<version> --username=<pypi_username> --password=<pypi_password>
-````
+```
 
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
+````
```

### Comparing `agentmemory-0.2.3/setup.py` & `agentmemory-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import os
 from setuptools import setup
 
 long_description = ""
 with open("README.md", "r") as fh:
     long_description = fh.read()
     # search for any lines that contain <img and remove them
     long_description = long_description.split('\n')
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.2.3',
+    version='0.2.7',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

