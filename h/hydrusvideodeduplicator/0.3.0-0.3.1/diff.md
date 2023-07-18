# Comparing `tmp/hydrusvideodeduplicator-0.3.0.tar.gz` & `tmp/hydrusvideodeduplicator-0.3.1.tar.gz`

## Comparing `hydrusvideodeduplicator-0.3.0.tar` & `hydrusvideodeduplicator-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/Dockerfile
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/docker-compose.yml
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/docker-entrypoint.sh
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    21111 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36865 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
--rw-r--r--   0        0        0    23627 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
--rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/__main__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/LICENSE
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/README.md
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/docker-compose.yml
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/docker-entrypoint.sh
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    21169 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36865 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    23627 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/README.md
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.3.1/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.3.0/docker-compose.yml` & `hydrusvideodeduplicator-0.3.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/docker-entrypoint.sh` & `hydrusvideodeduplicator-0.3.1/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/dedup.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,30 +378,31 @@
         it = iter(iterable)
         while batch := tuple(islice(it, n)):
             yield batch
 
     @staticmethod
     def batched_and_save_db(
         db: SqliteDict,
-        n: int,
-        chunk_size: int | None = None,
+        batch_size: int = 1,
+        chunk_size: int = 1,
     ) -> Generator[dict[str, dict[str, Any]], Any, None]:
         """
         Batch rows of into rows of length n and save changes after each batch or after chunk_size batches.
         """
-        assert n >= 1
-        assert chunk_size is None or chunk_size >= 1
-        if chunk_size is None:
-            chunk_size = n
+        assert batch_size >= 1
+        assert chunk_size >= 1
         it = iter(db.items())
-        while batch_items := dict(islice(it, 1)):
+        chunk_counter = 0
+        while batch_items := dict(islice(it, batch_size)):
             yield batch_items
+            chunk_counter += 1
 
-            # Save changes after each batch
-            db.commit()
+            # Save changes after chunk_size batches
+            if chunk_counter % chunk_size == 0:
+                db.commit()
 
     def is_files_deleted_hydrus(self, file_hashes: Iterable[str]) -> dict[str, bool]:
         """
         Check if files are trashed or deleted in Hydrus
         Returns a dictionary of hash : trashed_or_not
         """
         videos_metadata = self.client.get_file_metadata(hashes=file_hashes, only_return_basic_information=False)[
@@ -425,19 +426,19 @@
         Update the search cache to clamp the farthest_search_index to the current length of the database
         """
         assert new_total is None or new_total >= 0
 
         if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos"):
             return
 
-        CHUNK_SIZE = 256
+        BATCH_SIZE = 256
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c", outer_stack=False) as hashdb:
             if new_total is None:
                 new_total = len(hashdb)
-            for batched_items in HydrusVideoDeduplicator.batched_and_save_db(hashdb, CHUNK_SIZE):
+            for batched_items in HydrusVideoDeduplicator.batched_and_save_db(hashdb, BATCH_SIZE):
                 for item in batched_items.items():
                     row = hashdb[item[0]]
                     if 'farthest_search_index' in row and row['farthest_search_index'] > new_total:
                         row['farthest_search_index'] = new_total
                         hashdb[item[0]] = row
 
     def clear_trashed_files_from_db(self) -> None:
@@ -460,24 +461,24 @@
                     with tqdm(
                         dynamic_ncols=True,
                         total=total,
                         desc="Clearing trashed videos",
                         unit="video",
                         colour="BLUE",
                     ) as pbar:
-                        CHUNK_SIZE = 32
-                        for batched_items in self.batched_and_save_db(hashdb, CHUNK_SIZE):
+                        BATCH_SIZE = 32
+                        for batched_items in self.batched_and_save_db(hashdb, BATCH_SIZE):
                             is_trashed_result = self.is_files_deleted_hydrus(batched_items.keys())
                             for result in is_trashed_result.items():
                                 video_hash = result[0]
                                 is_trashed = result[1]
                                 if is_trashed is True:
                                     del hashdb[video_hash]
                                     delete_count += 1
-                            pbar.update(min(CHUNK_SIZE, total - pbar.n))
+                            pbar.update(min(BATCH_SIZE, total - pbar.n))
                 except Exception as exc:
                     print("[red] Error while clearing trashed videos cache.")
                     print(exc)
                     self.hydlog.error(exc)
                 finally:
                     if delete_count > 0:
                         print(f"Cleared {delete_count} trashed videos from the database.")
```

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/containers.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/types/containers.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,28 +90,24 @@
         while i < self.HASH256_NUM_SLOTS:
             n += self.hammingNorm16(self.w[i])
             i += 1
         return n
 
     def hammingDistance(self, that):
         n = 0
-        i = 0
-        while i < self.HASH256_NUM_SLOTS:
-            n += self.hammingNorm16(int((self.w[i] ^ that.w[i])))
-            i += 1
+        for w1, w2 in zip(self.w, that.w):
+            n += self.hammingNorm16(int(w1 ^ w2))
         return n
 
     def hammingDistanceLE(self, that, d) -> bool:
         e = 0
-        i = 0
-        while i < self.HASH256_NUM_SLOTS:
-            e += self.hammingNorm16(int((self.w[i] ^ that.w[i])))
+        for w1, w2 in zip(self.w, that.w):
+            e += self.hammingNorm16(int(w1 ^ w2))
             if e > d:
                 return False
-            i += 1
         return True
 
     def setBit(self, k):
         self.w[(k & 255) >> 4] |= 1 << (k & 15)
 
     def flipBit(self, k):
         self.w[(k & 255) >> 4] ^= 1 << (k & 15)
```

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py` & `hydrusvideodeduplicator-0.3.1/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def feature_match_count(
         query_features: list[VpdqFeature],
         target_features: list[VpdqFeature],
         distance_tolerance: float,
     ) -> int:
         return sum(
             any(
-                query_feature.pdq_hash.hammingDistance(target_feature.pdq_hash) <= distance_tolerance
+                query_feature.pdq_hash.hammingDistanceLE(target_feature.pdq_hash, distance_tolerance)
                 for target_feature in target_features
             )
             for query_feature in query_features
         )
 
     @staticmethod
     def match_hash(
```

### Comparing `hydrusvideodeduplicator-0.3.0/.gitignore` & `hydrusvideodeduplicator-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/LICENSE` & `hydrusvideodeduplicator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/README.md` & `hydrusvideodeduplicator-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 
 For more information check out the [wiki](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/faq)
 
 ---
 
 ## [Installation:](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/Installation)
 #### Dependencies:
-- Python >=3.10
-- FFmpeg
+- [Python](https://www.python.org/downloads/) >=3.10
 
 ```sh
 python3 -m pip install hydrusvideodeduplicator
 ```
 
 ---
 
@@ -46,15 +45,15 @@
 For full list of options see `--help` or the [usage page.](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/Usage)
 
 ---
 
 ## TODO:
 - [ ] Option to rollback and remove potential duplicates
 - [ ] OR predicates for --query
-- [ ] Parallelize hashing and duplicate search
+- [x] Parallelize hashing and duplicate search
 - [ ] Automatically generate access key with Hydrus API
 - [x] Docker container
 - [ ] Upload Docker container to Docker Hub (GitHub Action)
 - [x] Pure Python port of vpdq
 - [x] Windows compatibility without WSL or Docker
 
 ---
```

### Comparing `hydrusvideodeduplicator-0.3.0/pyproject.toml` & `hydrusvideodeduplicator-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.3.0/PKG-INFO` & `hydrusvideodeduplicator-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.3.0
+Version: 0.3.1
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator
 Author-email: hydrusvideodeduplicator <applenannerapple@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -53,16 +53,15 @@
 
 For more information check out the [wiki](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/faq)
 
 ---
 
 ## [Installation:](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/Installation)
 #### Dependencies:
-- Python >=3.10
-- FFmpeg
+- [Python](https://www.python.org/downloads/) >=3.10
 
 ```sh
 python3 -m pip install hydrusvideodeduplicator
 ```
 
 ---
 
@@ -75,15 +74,15 @@
 For full list of options see `--help` or the [usage page.](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/Usage)
 
 ---
 
 ## TODO:
 - [ ] Option to rollback and remove potential duplicates
 - [ ] OR predicates for --query
-- [ ] Parallelize hashing and duplicate search
+- [x] Parallelize hashing and duplicate search
 - [ ] Automatically generate access key with Hydrus API
 - [x] Docker container
 - [ ] Upload Docker container to Docker Hub (GitHub Action)
 - [x] Pure Python port of vpdq
 - [x] Windows compatibility without WSL or Docker
 
 ---
```

