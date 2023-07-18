# Comparing `tmp/chess-hic-0.3.7.tar.gz` & `tmp/chess-hic-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-hic-0.3.7.tar", last modified: Wed May 19 12:57:20 2021, max compression
+gzip compressed data, was "chess-hic-0.3.8.tar", last modified: Tue Jul 18 13:39:02 2023, max compression
```

## Comparing `chess-hic-0.3.7.tar` & `chess-hic-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 12:57:20.181055 chess-hic-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (121)     9379 2021-05-19 12:57:11.000000 chess-hic-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2021-05-19 12:57:20.181055 chess-hic-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-05-19 12:57:11.000000 chess-hic-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 12:57:20.177055 chess-hic-0.3.7/bin/
--rw-r--r--   0 runner    (1001) docker     (121)    23871 2021-05-19 12:57:11.000000 chess-hic-0.3.7/bin/chess
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 12:57:20.181055 chess-hic-0.3.7/chess/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15890 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     3925 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/cross_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     9159 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/get_structures.py
--rw-r--r--   0 runner    (1001) docker     (121)    20499 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6461 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/oe.py
--rw-r--r--   0 runner    (1001) docker     (121)    17741 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/sim.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-19 12:57:11.000000 chess-hic-0.3.7/chess/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 12:57:20.181055 chess-hic-0.3.7/chess_hic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2021-05-19 12:57:20.000000 chess-hic-0.3.7/chess_hic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-05-19 12:57:20.000000 chess-hic-0.3.7/chess_hic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-19 12:57:20.000000 chess-hic-0.3.7/chess_hic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-05-19 12:57:20.000000 chess-hic-0.3.7/chess_hic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-05-19 12:57:20.000000 chess-hic-0.3.7/chess_hic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-05-19 12:57:20.181055 chess-hic-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2021-05-19 12:57:11.000000 chess-hic-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:39:02.797016 chess-hic-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-18 13:38:50.000000 chess-hic-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-18 13:39:02.797016 chess-hic-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-18 13:38:50.000000 chess-hic-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:39:02.793016 chess-hic-0.3.8/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-18 13:38:50.000000 chess-hic-0.3.8/bin/chess
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:39:02.797016 chess-hic-0.3.8/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15890 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/cross_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/get_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/oe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 13:38:50.000000 chess-hic-0.3.8/chess/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:39:02.797016 chess-hic-0.3.8/chess_hic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-18 13:39:02.000000 chess-hic-0.3.8/chess_hic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-18 13:39:02.000000 chess-hic-0.3.8/chess_hic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:39:02.000000 chess-hic-0.3.8/chess_hic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 13:39:02.000000 chess-hic-0.3.8/chess_hic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 13:39:02.000000 chess-hic-0.3.8/chess_hic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 13:39:02.797016 chess-hic-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-18 13:38:51.000000 chess-hic-0.3.8/setup.py
```

### Comparing `chess-hic-0.3.7/LICENSE` & `chess-hic-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/PKG-INFO` & `chess-hic-0.3.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: chess-hic
-Version: 0.3.7
+Version: 0.3.8
 Summary: Quantitative comparison and automatic feature extraction for chromatin contact data.
 Home-page: https://github.com/vaquerizaslab/chess
-License: UNKNOWN
-Description: # chess-hic
-        
-        [![PyPI version](https://badge.fury.io/py/chess-hic.svg)](https://badge.fury.io/py/chess-hic)
-        [![Documentation Status](https://readthedocs.org/projects/chess-hic/badge/?version=latest)](https://chess-hic.readthedocs.io/en/latest/?badge=latest)
-        
-        CHESS is a tool for the comparison and automatic feature extraction for chromatin contact data,
-        developed in the [Vaquerizas Lab](https://www.vaquerizaslab.org/).
-        
-        If you use CHESS in your research, please cite the [CHESS paper](https://www.nature.com/articles/s41588-020-00712-y).
-        
-        Please check out the [online documentation](https://chess-hic.readthedocs.io/en/latest/index.html)
-        for detailed installation and usage instructions.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# chess-hic
+
+[![PyPI version](https://badge.fury.io/py/chess-hic.svg)](https://badge.fury.io/py/chess-hic)
+[![Documentation Status](https://readthedocs.org/projects/chess-hic/badge/?version=latest)](https://chess-hic.readthedocs.io/en/latest/?badge=latest)
+
+CHESS is a tool for the comparison and automatic feature extraction for chromatin contact data,
+developed in the [Vaquerizas Lab](https://www.vaquerizaslab.org/).
+
+If you use CHESS in your research, please cite the [CHESS paper](https://www.nature.com/articles/s41588-020-00712-y).
+
+Please check out the [online documentation](https://chess-hic.readthedocs.io/en/latest/index.html)
+for detailed installation and usage instructions.
```

### Comparing `chess-hic-0.3.7/README.md` & `chess-hic-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/bin/chess` & `chess-hic-0.3.8/bin/chess`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/chess/commands.py` & `chess-hic-0.3.8/chess/commands.py`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/chess/cross_correlation.py` & `chess-hic-0.3.8/chess/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/chess/get_structures.py` & `chess-hic-0.3.8/chess/get_structures.py`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/chess/helpers.py` & `chess-hic-0.3.8/chess/helpers.py`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/chess/oe.py` & `chess-hic-0.3.8/chess/oe.py`

 * *Files identical despite different names*

### Comparing `chess-hic-0.3.7/chess/sim.py` & `chess-hic-0.3.8/chess/sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     uM = filter_uniform_filter(M, size=size)
     vM = filter_uniform_filter(M, size=size, func=np.nanvar)
     SN = np.nanmean(np.abs(uM) / vM)
 
     return float(SN)
 
 
-def filter_uniform_filter(M, size=7, no_data_val=None,
-                          func=np.nanmean):
+def filter_uniform_filter(M, size=7, no_data_val=None, func=np.nanmean):
     """Apply func to sliding window on input matrix.
 
     Adaption from:
     www.programcreek.com/python/example/93943/scipy.ndimage.uniform_filter
     This is equivalent to scipy.ndimage.uniform_filter, but can handle nan's,
     and can use numpy nanmean/median/max/min functions.
     :param M: input data, numpy matrix.
@@ -47,31 +46,30 @@
     :returns: func of the matrix A filtered by a uniform kernel of size=size
     """
 
     assert size % 2 == 1, 'Please supply an odd size'
     assert M.dtype == np.dtype('float64'), 'Input must have dtype(float64)'
     rows, cols = M.shape
 
-    padded_A = np.empty(shape=(rows + size-1,
-                               cols + size-1),
+    padded_A = np.empty(shape=(rows + size - 1, cols + size - 1),
                         dtype=M.dtype)
     padded_A[:] = np.nan
     rows_pad, cols_pad = padded_A.shape
 
     if no_data_val:
         mask = M == no_data_val
         M[mask] = np.nan
 
     upleft_data_start = int((size - 1) / 2)
     rl, cl = rows_pad - upleft_data_start, cols_pad - upleft_data_start
-    padded_A[upleft_data_start: rl, upleft_data_start: cl] = M.copy()
+    padded_A[upleft_data_start:rl, upleft_data_start:cl] = M.copy()
 
     n, m = M.shape
     strided_data = as_strided(padded_A, (n, m, size, size),
-                              padded_A.strides+padded_A.strides)
+                              padded_A.strides + padded_A.strides)
     strided_data = strided_data.copy().reshape((n, m, size**2))
 
     return func(strided_data, axis=2)
 
 
 def find_masked_rows(m, masking_value=0):
     """Find rows in m filled with masking value.
@@ -100,52 +98,62 @@
     idxs = target_rows
     m_removed = np.delete(m, idxs, 0)
     m_removed = np.delete(m_removed, idxs, 1)
 
     return m_removed
 
 
-def comparison_worker(input_queue, output_queue,
-                      reference_edges, reference_regions,
-                      query_edges, query_regions,
+def comparison_worker(input_queue,
+                      output_queue,
+                      reference_edges,
+                      reference_regions,
+                      query_edges,
+                      query_regions,
                       min_bins=20,
                       keep_unmappable_bins=False,
                       absolute_window_size=None,
                       relative_window_size=1.,
                       mappability_cutoff=0.1,
                       default_value=1):
     worker_id = uuid.uuid4()
     try:
         while True:
             data = input_queue.get(block=True)
             if data is None:
                 break
             pair, compute_sn = data
 
-            pair_ix, ssim, sn = compare_pair(pair,
-                                             reference_edges, reference_regions,
-                                             query_edges, query_regions,
-                                             min_bins=min_bins,
-                                             keep_unmappable_bins=keep_unmappable_bins,
-                                             absolute_window_size=absolute_window_size,
-                                             relative_window_size=relative_window_size,
-                                             mappability_cutoff=mappability_cutoff,
-                                             default_value=default_value,
-                                             compute_sn=compute_sn)
+            pair_ix, ssim, sn = compare_pair(
+                pair,
+                reference_edges,
+                reference_regions,
+                query_edges,
+                query_regions,
+                min_bins=min_bins,
+                keep_unmappable_bins=keep_unmappable_bins,
+                absolute_window_size=absolute_window_size,
+                relative_window_size=relative_window_size,
+                mappability_cutoff=mappability_cutoff,
+                default_value=default_value,
+                compute_sn=compute_sn)
             output_queue.put((pair_ix, ssim, sn))
     except Exception as e:
-        logger.error("Worker {} encountered a problem: {}".format(worker_id, e))
+        logger.error("Worker {} encountered a problem: {}".format(
+            worker_id, e))
         output_queue.put(e)
 
     logger.info("Worker {} exited gracefully".format(worker_id))
 
 
-def chunk_comparison_worker(input_queue, output_queue,
-                            reference_edges, reference_regions,
-                            query_edges, query_regions,
+def chunk_comparison_worker(input_queue,
+                            output_queue,
+                            reference_edges,
+                            reference_regions,
+                            query_edges,
+                            query_regions,
                             min_bins=20,
                             keep_unmappable_bins=False,
                             absolute_window_size=None,
                             relative_window_size=1.,
                             mappability_cutoff=0.1,
                             default_value=1):
     worker_id = uuid.uuid4()
@@ -158,64 +166,78 @@
                 break
             chunk, compute_sn = data
 
             results = []
             for pair in chunk:
                 pair_ix, reference_region, query_region = pair
                 try:
-                    if previous_reference[0] is not None and reference_region == previous_reference[0]:
+                    if previous_reference[
+                            0] is not None and reference_region == previous_reference[
+                                0]:
                         reference, ref_rs = previous_reference[1]
                     else:
-                        reference, ref_rs = sub_matrix_from_edges_dict(reference_edges,
-                                                                       reference_regions,
-                                                                       reference_region,
-                                                                       default_weight=default_value)
-                        previous_reference = [reference_region, (reference, ref_rs)]
-
-                    if previous_query[0] is not None and query_region == previous_query[0]:
+                        reference, ref_rs = sub_matrix_from_edges_dict(
+                            reference_edges,
+                            reference_regions,
+                            reference_region,
+                            default_weight=default_value)
+                        previous_reference = [
+                            reference_region, (reference, ref_rs)
+                        ]
+
+                    if previous_query[
+                            0] is not None and query_region == previous_query[
+                                0]:
                         query, qry_rs = previous_query[1]
                     else:
-                        query, qry_rs = sub_matrix_from_edges_dict(query_edges,
-                                                                   query_regions,
-                                                                   query_region,
-                                                                   default_weight=default_value)
+                        query, qry_rs = sub_matrix_from_edges_dict(
+                            query_edges,
+                            query_regions,
+                            query_region,
+                            default_weight=default_value)
                         previous_query = [query_region, (query, qry_rs)]
                 except ValueError:
                     results.append([pair_ix, np.nan, np.nan])
                     continue
 
-                pair_ix, ssim, sn = compare_matrix_pair(reference, reference_region,
-                                                        query, query_region,
-                                                        pair_ix=pair_ix,
-                                                        min_bins=min_bins,
-                                                        keep_unmappable_bins=keep_unmappable_bins,
-                                                        absolute_window_size=absolute_window_size,
-                                                        relative_window_size=relative_window_size,
-                                                        mappability_cutoff=mappability_cutoff,
-                                                        default_value=default_value,
-                                                        compute_sn=compute_sn)
+                pair_ix, ssim, sn = compare_matrix_pair(
+                    reference,
+                    reference_region,
+                    query,
+                    query_region,
+                    pair_ix=pair_ix,
+                    min_bins=min_bins,
+                    keep_unmappable_bins=keep_unmappable_bins,
+                    absolute_window_size=absolute_window_size,
+                    relative_window_size=relative_window_size,
+                    mappability_cutoff=mappability_cutoff,
+                    default_value=default_value,
+                    compute_sn=compute_sn)
                 results.append([pair_ix, ssim, sn])
             output_queue.put(results)
     except Exception as e:
-        logger.error("Worker {} encountered a problem: {}".format(worker_id, e))
+        logger.error("Worker {} encountered a problem: {}".format(
+            worker_id, e))
         output_queue.put(e)
 
     logger.debug("Worker {} exited gracefully".format(worker_id))
 
 
-def compare_pair(pair, reference_edges, reference_regions,
-                 query_edges, query_regions,
+def compare_pair(pair,
+                 reference_edges,
+                 reference_regions,
+                 query_edges,
+                 query_regions,
                  min_bins=20,
                  keep_unmappable_bins=False,
                  absolute_window_size=None,
                  relative_window_size=1.,
                  mappability_cutoff=0.1,
                  default_value=1,
-                 compute_sn=True
-                 ):
+                 compute_sn=True):
     """Run comparison of given Hi-C matrices without any background model.
 
     Compare given submatrices of the full Hi-C matrices in sampleID2hic.
     All submatrices (specified in pairs) have to be of the same size.
     The assignment of reference and query samples is arbitrary in this case,
     but has to be consistent.
     :param edges: edges dictionary
@@ -250,35 +272,46 @@
     :returns: results dictionary of form:
               {
                 pair_id: (similarity_score, signal_to_noise_value)
               }
     """
     pair_ix, reference_region, query_region = pair
     try:
-        reference, ref_rs = sub_matrix_from_edges_dict(reference_edges, reference_regions,
-                                                       reference_region, default_weight=default_value)
-        query, qry_rs = sub_matrix_from_edges_dict(query_edges, query_regions,
-                                                   query_region, default_weight=default_value)
+        reference, ref_rs = sub_matrix_from_edges_dict(
+            reference_edges,
+            reference_regions,
+            reference_region,
+            default_weight=default_value)
+        query, qry_rs = sub_matrix_from_edges_dict(
+            query_edges,
+            query_regions,
+            query_region,
+            default_weight=default_value)
     except ValueError:
         return pair_ix, np.nan, np.nan
 
-    return compare_matrix_pair(reference, reference_region,
-                               query, query_region,
+    return compare_matrix_pair(reference,
+                               reference_region,
+                               query,
+                               query_region,
                                pair_ix=pair_ix,
                                min_bins=min_bins,
                                keep_unmappable_bins=keep_unmappable_bins,
                                absolute_window_size=absolute_window_size,
                                relative_window_size=relative_window_size,
                                mappability_cutoff=mappability_cutoff,
                                default_value=default_value,
                                compute_sn=compute_sn)
 
 
-def compare_matrix_pair(reference, reference_region,
-                        query, query_region, pair_ix=None,
+def compare_matrix_pair(reference,
+                        reference_region,
+                        query,
+                        query_region,
+                        pair_ix=None,
                         min_bins=20,
                         keep_unmappable_bins=False,
                         absolute_window_size=None,
                         relative_window_size=1.,
                         mappability_cutoff=0.1,
                         default_value=1,
                         compute_sn=True):
@@ -328,26 +361,35 @@
         window_size -= 1
 
     # prevent from going lower than three.
     # breaks at ws = 1 because of 0 division, and 2 is not odd.
     window_size = max(window_size, 3)
 
     # actual comparison
-    curr_ssim = structural_similarity(reference, query, win_size=window_size)
+    dmax = max(reference.max(), query.max())
+    dmin = min(reference.min(), query.min())
+    drange = dmax - dmin
+    curr_ssim = structural_similarity(reference,
+                                      query,
+                                      win_size=window_size,
+                                      data_range=drange)
     if compute_sn:
         curr_sn = SN(reference, query)
     else:
         curr_sn = None
 
     return pair_ix, curr_ssim, curr_sn
 
 
-def compare_structures(reference_edges, reference_regions,
-                       query_edges, query_regions,
-                       pairs, worker_ID,
+def compare_structures(reference_edges,
+                       reference_regions,
+                       query_edges,
+                       query_regions,
+                       pairs,
+                       worker_ID,
                        min_bins=20,
                        keep_unmappable_bins=False,
                        absolute_window_size=None,
                        relative_window_size=1.,
                        mappability_cutoff=0.1,
                        default_value=1):
     """Run comparison of given Hi-C matrices without any background model.
@@ -390,23 +432,26 @@
               }
     """
 
     results = {}  # store the ssim in here
     no_pass = set()
 
     for pair in pairs:
-        pair_ix, ssim, sn = compare_pair(pair,
-                                         reference_edges, reference_regions,
-                                         query_edges, query_regions,
-                                         min_bins=min_bins,
-                                         keep_unmappable_bins=keep_unmappable_bins,
-                                         absolute_window_size=absolute_window_size,
-                                         relative_window_size=relative_window_size,
-                                         mappability_cutoff=mappability_cutoff,
-                                         default_value=default_value)
+        pair_ix, ssim, sn = compare_pair(
+            pair,
+            reference_edges,
+            reference_regions,
+            query_edges,
+            query_regions,
+            min_bins=min_bins,
+            keep_unmappable_bins=keep_unmappable_bins,
+            absolute_window_size=absolute_window_size,
+            relative_window_size=relative_window_size,
+            mappability_cutoff=mappability_cutoff,
+            default_value=default_value)
         if np.isnan(ssim):
             no_pass.add(pair_ix)
             results[pair_ix] = (np.nan, np.nan)
         else:
             results[pair_ix] = (ssim, sn)
 
     logger.debug('[WORKER #{}]: Done!'.format(worker_ID))
```

### Comparing `chess-hic-0.3.7/chess_hic.egg-info/PKG-INFO` & `chess-hic-0.3.8/chess_hic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: chess-hic
-Version: 0.3.7
+Version: 0.3.8
 Summary: Quantitative comparison and automatic feature extraction for chromatin contact data.
 Home-page: https://github.com/vaquerizaslab/chess
-License: UNKNOWN
-Description: # chess-hic
-        
-        [![PyPI version](https://badge.fury.io/py/chess-hic.svg)](https://badge.fury.io/py/chess-hic)
-        [![Documentation Status](https://readthedocs.org/projects/chess-hic/badge/?version=latest)](https://chess-hic.readthedocs.io/en/latest/?badge=latest)
-        
-        CHESS is a tool for the comparison and automatic feature extraction for chromatin contact data,
-        developed in the [Vaquerizas Lab](https://www.vaquerizaslab.org/).
-        
-        If you use CHESS in your research, please cite the [CHESS paper](https://www.nature.com/articles/s41588-020-00712-y).
-        
-        Please check out the [online documentation](https://chess-hic.readthedocs.io/en/latest/index.html)
-        for detailed installation and usage instructions.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# chess-hic
+
+[![PyPI version](https://badge.fury.io/py/chess-hic.svg)](https://badge.fury.io/py/chess-hic)
+[![Documentation Status](https://readthedocs.org/projects/chess-hic/badge/?version=latest)](https://chess-hic.readthedocs.io/en/latest/?badge=latest)
+
+CHESS is a tool for the comparison and automatic feature extraction for chromatin contact data,
+developed in the [Vaquerizas Lab](https://www.vaquerizaslab.org/).
+
+If you use CHESS in your research, please cite the [CHESS paper](https://www.nature.com/articles/s41588-020-00712-y).
+
+Please check out the [online documentation](https://chess-hic.readthedocs.io/en/latest/index.html)
+for detailed installation and usage instructions.
```

### Comparing `chess-hic-0.3.7/setup.py` & `chess-hic-0.3.8/setup.py`

 * *Files identical despite different names*

