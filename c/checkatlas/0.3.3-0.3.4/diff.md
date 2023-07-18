# Comparing `tmp/checkatlas-0.3.3.tar.gz` & `tmp/checkatlas-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.3.3.tar", max compression
+gzip compressed data, was "checkatlas-0.3.4.tar", max compression
```

## Comparing `checkatlas-0.3.3.tar` & `checkatlas-0.3.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1506 2023-07-15 15:46:21.660234 checkatlas-0.3.3/LICENSE
--rw-r--r--   0        0        0     4452 2023-07-15 15:46:21.660234 checkatlas-0.3.3/README.md
--rw-r--r--   0        0        0      111 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/__init__.py
--rw-r--r--   0        0        0     4652 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/__main__.py
--rw-r--r--   0        0        0    24201 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/atlas.py
--rw-r--r--   0        0        0     4715 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/cellranger.py
--rw-r--r--   0        0        0     8485 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/checkatlas.py
--rw-r--r--   0        0        0     2785 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/checkatlas_workflow.py
--rw-r--r--   0        0        0       45 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4108 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0    20177 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/seurat.py
--rw-r--r--   0        0        0      107 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/__init__.py
--rw-r--r--   0        0        0     4563 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/checkatlas_arguments.py
--rw-r--r--   0        0        0     4239 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/checkatlas_workflow_arguments.py
--rw-r--r--   0        0        0     2759 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/files.py
--rw-r--r--   0        0        0     2065 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/folders.py
--rw-r--r--   0        0        0     6267 2023-07-15 15:46:21.660234 checkatlas-0.3.3/checkatlas/utils/obsolete_arguments.py
--rw-r--r--   0        0        0     1410 2023-07-15 15:46:21.852237 checkatlas-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 checkatlas-0.3.3/setup.py
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-18 07:39:52.282545 checkatlas-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4452 2023-07-18 07:39:52.282545 checkatlas-0.3.4/README.md
+-rw-r--r--   0        0        0      111 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4652 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24756 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/atlas.py
+-rw-r--r--   0        0        0     4715 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/cellranger.py
+-rw-r--r--   0        0        0     8756 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0     2766 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/checkatlas_workflow.py
+-rw-r--r--   0        0        0       45 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      254 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4108 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-18 07:39:52.282545 checkatlas-0.3.4/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20177 2023-07-18 07:39:52.286545 checkatlas-0.3.4/checkatlas/seurat.py
+-rw-r--r--   0        0        0      107 2023-07-18 07:39:52.286545 checkatlas-0.3.4/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4563 2023-07-18 07:39:52.286545 checkatlas-0.3.4/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     4239 2023-07-18 07:39:52.286545 checkatlas-0.3.4/checkatlas/utils/checkatlas_workflow_arguments.py
+-rw-r--r--   0        0        0     2759 2023-07-18 07:39:52.286545 checkatlas-0.3.4/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     2065 2023-07-18 07:39:52.286545 checkatlas-0.3.4/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2023-07-18 07:39:52.286545 checkatlas-0.3.4/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1410 2023-07-18 07:39:52.486545 checkatlas-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 checkatlas-0.3.4/setup.py
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.4/PKG-INFO
```

### Comparing `checkatlas-0.3.3/LICENSE` & `checkatlas-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/README.md` & `checkatlas-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/__main__.py` & `checkatlas-0.3.4/checkatlas/__main__.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/atlas.py` & `checkatlas-0.3.4/checkatlas/atlas.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import warnings
 
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from anndata import AnnData
 from anndata import _io as _io
+from sklearn.utils.fixes import _object_dtype_isnan
 
 from . import cellranger, checkatlas
 from .metrics import metrics
 from .utils import files, folders
 
 """
 Atlas module for AnnData (Scanpy)
@@ -247,28 +248,31 @@
     obs_keys = list()
     # Get keys from OBS_CLUSTERS
     for obs_key in adata.obs_keys():
         for obs_key_celltype in args.obs_cluster:
             if obs_key_celltype in obs_key:
                 if type(adata.obs[obs_key].dtype) == pd.CategoricalDtype:
                     obs_keys.append(obs_key)
-    # Remove keys with only one category
+    # Remove keys with only one category and no NaN in the array
     obs_keys_final = list()
     for obs_key in obs_keys:
         annotations = adata.obs[obs_key]
-        categories_temp = annotations.cat.categories
-        # remove nan if found
-        categories = categories_temp.dropna()
-        if True in categories.isin(["nan"]):
-            index = categories.get_loc("nan")
-            categories = categories.delete(index)
-        # Add obs_key with more than one category (with Nan removed)
-        if len(categories) != 1:
-            logger.debug(f"Add obs_key {obs_key} with cat {categories_temp}")
-            obs_keys_final.append(obs_key)
+        if not _object_dtype_isnan(annotations).any():
+            categories_temp = annotations.cat.categories
+            # remove nan if found
+            categories = categories_temp.dropna()
+            if True in categories.isin(["nan"]):
+                index = categories.get_loc("nan")
+                categories = categories.delete(index)
+            # Add obs_key with more than one category (with Nan removed)
+            if len(categories) != 1:
+                logger.debug(
+                    f"Add obs_key {obs_key} with cat {categories_temp}"
+                )
+                obs_keys_final.append(obs_key)
     return sorted(obs_keys_final)
 
 
 def get_viable_obsm(adata: AnnData, args: argparse.Namespace) -> list:
     """
     TO DO
     Search viable obsm for dimensionality reduction metric
@@ -575,15 +579,23 @@
         folders.CLUSTER,
         checkatlas.TSV_EXTENSION,
         args.path,
     )
     header = ["Clust_Sample", "obs"] + args.metric_cluster
     df_cluster = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(adata, args)
-    obsm_key_representation = "X_umap"
+    obsm_keys = get_viable_obsm(adata, args)
+    r = re.compile(".*umap*.")
+    obsm_umap_keys = list(filter(r.match, obsm_keys))
+    r = re.compile(".*tsne*.")
+    obsm_tsne_keys = list(filter(r.match, obsm_keys))
+    if len(obsm_umap_keys) > 0:
+        obsm_key_representation = obsm_umap_keys[0]
+    elif len(obsm_tsne_keys) > 0:
+        obsm_key_representation = obsm_tsne_keys[0]
 
     if len(obs_keys) > 0:
         logger.debug(f"Calc clustering metrics for {atlas_name}")
         for obs_key in obs_keys:
             dict_line = {
                 "Clust_Sample": [atlas_name + "_" + obs_key],
                 "obs": [obs_key],
```

### Comparing `checkatlas-0.3.3/checkatlas/cellranger.py` & `checkatlas-0.3.4/checkatlas/cellranger.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/checkatlas.py` & `checkatlas-0.3.4/checkatlas/checkatlas.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,26 +109,29 @@
     # Save the list of atlas taken into account
     chk_files.save_list_scanpy(clean_scanpy_list, checkatlas_path)
     chk_files.save_list_cellranger(clean_cellranger_list, checkatlas_path)
     chk_files.save_list_seurat(clean_seurat_list, checkatlas_path)
 
 
 def read_list_atlases(checkatlas_path: str) -> tuple:
-    clean_scanpy_list = pd.read_csv(
-        chk_files.get_table_scanpy_path(checkatlas_path)
-    )
-    clean_scanpy_list.index = clean_scanpy_list[ATLAS_NAME_KEY]
-    clean_cellranger_list = pd.read_csv(
-        chk_files.get_table_cellranger_path(checkatlas_path)
-    )
-    clean_cellranger_list.index = clean_cellranger_list[ATLAS_NAME_KEY]
-    clean_seurat_list = pd.read_csv(
-        chk_files.get_table_seurat_path(checkatlas_path)
-    )
-    clean_seurat_list.index = clean_seurat_list[ATLAS_NAME_KEY]
+    if os.path.exists(chk_files.get_table_scanpy_path(checkatlas_path)):
+        clean_scanpy_list = pd.read_csv(
+            chk_files.get_table_scanpy_path(checkatlas_path)
+        )
+        clean_scanpy_list.index = clean_scanpy_list[ATLAS_NAME_KEY]
+    if os.path.exists(chk_files.get_table_cellranger_path(checkatlas_path)):
+        clean_cellranger_list = pd.read_csv(
+            chk_files.get_table_cellranger_path(checkatlas_path)
+        )
+        clean_cellranger_list.index = clean_cellranger_list[ATLAS_NAME_KEY]
+    if os.path.exists(chk_files.get_table_seurat_path(checkatlas_path)):
+        clean_seurat_list = pd.read_csv(
+            chk_files.get_table_seurat_path(checkatlas_path)
+        )
+        clean_seurat_list.index = clean_seurat_list[ATLAS_NAME_KEY]
     return clean_scanpy_list, clean_cellranger_list, clean_seurat_list
 
 
 def generate_fig_html(checkatlas_path: str, type_viz: str):
     logger.info("Generate html reports with all figs for {type}")
     # shutil.copy2(os.path.join(f["root"], f["fn"]), fig_dir
     if type_viz == "qc":
```

### Comparing `checkatlas-0.3.3/checkatlas/checkatlas_workflow.py` & `checkatlas-0.3.4/checkatlas/checkatlas_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         logger.setLevel(getattr(logging, "DEBUG"))
     else:
         logger.setLevel(getattr(logging, "INFO"))
 
     logger.debug(f"Program arguments: {args}")
 
     process = args.process
-    print(process)
     if process == PROCESS_TYPE[0]:
         logger.debug(f"Search path {args.path} with checkatlas_workflow")
         logger.debug(f"Transform path to absolute:{args.path}")
         args.path = os.path.abspath(args.path)
         logger.debug(f"Check checkatlas folders in:{args.path}")
         folders.checkatlas_folders(args.path)
         logger.info("Searching Seurat, Cellranger and Scanpy files")
```

### Comparing `checkatlas-0.3.3/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.3.4/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/metrics/metrics.py` & `checkatlas-0.3.4/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.3.4/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.3.4/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.3.4/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.3.4/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/seurat.py` & `checkatlas-0.3.4/checkatlas/seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/utils/checkatlas_arguments.py` & `checkatlas-0.3.4/checkatlas/utils/checkatlas_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         "use in the clustering metric calculus."
         "Example: --obs_cluster celltype leuven seurat_clusters",
     )
     metric_options.add_argument(
         "--metric_cluster",
         nargs="+",
         type=str,
-        # default=["silhouette", "davies_bouldin"],
-        default=["davies_bouldin"],
+        default=["silhouette", "davies_bouldin"],
+        # default=["davies_bouldin"],
         help="Specify the list of clustering metrics to calculate.\n"
         "   Example: --metric_cluster silhouette davies_bouldin\n"
         f"   List of cluster metrics: {cluster.__all__}",
     )
     metric_options.add_argument(
         "--metric_annot",
         nargs="+",
@@ -119,16 +119,16 @@
         f"   Example: --metric_annot rand_index"
         f"   List of annotation metrics: {annot.__all__}",
     )
     metric_options.add_argument(
         "--metric_dimred",
         nargs="+",
         type=str,
-        # default=["kruskal_stress"],
-        default=[],
+        # default=[],
+        default=["kruskal_stress"],
         help="Specify the list of dimensionality reduction "
         "metrics to calculate.\n"
         "   Example: --metric_dimred kruskal_stress\n"
         f"   List of dim. red. metrics: {dimred.__all__}",
     )
     return parser
```

### Comparing `checkatlas-0.3.3/checkatlas/utils/checkatlas_workflow_arguments.py` & `checkatlas-0.3.4/checkatlas/utils/checkatlas_workflow_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/utils/files.py` & `checkatlas-0.3.4/checkatlas/utils/files.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/utils/folders.py` & `checkatlas-0.3.4/checkatlas/utils/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/checkatlas/utils/obsolete_arguments.py` & `checkatlas-0.3.4/checkatlas/utils/obsolete_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.3/pyproject.toml` & `checkatlas-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.3.3"
+version = "0.3.4"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
```

### Comparing `checkatlas-0.3.3/setup.py` & `checkatlas-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main',
                      'checkatlas-workflow = '
                      'checkatlas.checkatlas_workflow:main']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
```

### Comparing `checkatlas-0.3.3/PKG-INFO` & `checkatlas-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.3.3
+Version: 0.3.4
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: BSD 3-Clause
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

