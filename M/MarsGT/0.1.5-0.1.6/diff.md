# Comparing `tmp/MarsGT-0.1.5.tar.gz` & `tmp/MarsGT-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MarsGT-0.1.5.tar", last modified: Sat Jul 15 14:37:18 2023, max compression
+gzip compressed data, was "MarsGT-0.1.6.tar", last modified: Tue Jul 18 10:30:51 2023, max compression
```

## Comparing `MarsGT-0.1.5.tar` & `MarsGT-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-15 14:37:18.089431 MarsGT-0.1.5/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.5/MANIFEST.in
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-15 14:37:18.049436 MarsGT-0.1.5/MarsGT/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.5/MarsGT/__init__.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 08:36:23.000000 MarsGT-0.1.5/MarsGT/conv.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8699 2023-07-15 14:23:39.000000 MarsGT-0.1.5/MarsGT/egrn.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21360 2023-06-03 08:36:23.000000 MarsGT-0.1.5/MarsGT/marsgt_model.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7786 2023-06-03 08:36:23.000000 MarsGT-0.1.5/MarsGT/utils.py
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-15 14:37:18.075434 MarsGT-0.1.5/MarsGT.egg-info/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1054 2023-07-15 14:37:17.000000 MarsGT-0.1.5/MarsGT.egg-info/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-07-15 14:37:17.000000 MarsGT-0.1.5/MarsGT.egg-info/SOURCES.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-07-15 14:37:17.000000 MarsGT-0.1.5/MarsGT.egg-info/dependency_links.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      406 2023-07-15 14:37:17.000000 MarsGT-0.1.5/MarsGT.egg-info/requires.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-07-15 14:37:17.000000 MarsGT-0.1.5/MarsGT.egg-info/top_level.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1054 2023-07-15 14:37:18.087435 MarsGT-0.1.5/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.5/README.md
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-07-15 14:37:18.090431 MarsGT-0.1.5/setup.cfg
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1183 2023-07-15 14:29:47.000000 MarsGT-0.1.5/setup.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-18 10:30:51.069644 MarsGT-0.1.6/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.6/MANIFEST.in
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-18 10:30:51.005649 MarsGT-0.1.6/MarsGT/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.6/MarsGT/__init__.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 08:36:23.000000 MarsGT-0.1.6/MarsGT/conv.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8824 2023-07-18 10:28:20.000000 MarsGT-0.1.6/MarsGT/egrn.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21360 2023-06-03 08:36:23.000000 MarsGT-0.1.6/MarsGT/marsgt_model.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7805 2023-07-18 10:28:36.000000 MarsGT-0.1.6/MarsGT/utils.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-18 10:30:51.057646 MarsGT-0.1.6/MarsGT.egg-info/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1091 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-07-18 10:30:49.000000 MarsGT-0.1.6/MarsGT.egg-info/SOURCES.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/dependency_links.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      406 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/requires.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/top_level.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1091 2023-07-18 10:30:51.068648 MarsGT-0.1.6/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.6/README.md
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-07-18 10:30:51.070648 MarsGT-0.1.6/setup.cfg
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1183 2023-07-18 10:30:06.000000 MarsGT-0.1.6/setup.py
```

### Comparing `MarsGT-0.1.5/MarsGT/conv.py` & `MarsGT-0.1.6/MarsGT/conv.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.5/MarsGT/egrn.py` & `MarsGT-0.1.6/MarsGT/egrn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,160 +1,165 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-import numpy as np
-import scipy.sparse as sp
-import anndata as ad
-from collections import Counter
-import pandas as pd
-
-
-def peak_Sparse(peak_feature, gene_feature, device):
-    # Find the non-zero elements in peak_feature
-    peak_row = torch.where(peak_feature != 0)[0].to(device)
-    peak_col = torch.where(peak_feature != 0)[1].to(device)
-    peak_data = peak_feature[torch.where(peak_feature != 0)]
-
-    # Initialize tensors for combined peak data
-    peak_combine_row = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
-    peak_combine_col = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
-    peak_combine_data = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]))
-
-    non_count = 0
-    for peak_num in range(peak_feature.shape[0]):
-        # Calculate the peak sum
-        peak_sum = len(peak_row[peak_row == peak_num])
-
-        # Initialize a tensor for peak indices
-        peak_init = torch.zeros((gene_feature.shape[0], peak_sum), dtype=torch.int32).to(device)
-        for id in range(gene_feature.shape[0]):
-            peak_init[id,] = id + peak_num * gene_feature.shape[0]
-
-        # Update the combined peak data tensors
-        peak_combine_row[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_row[peak_row == peak_num] + peak_init - peak_num).reshape(1, -1)
-        peak_combine_col[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_col[peak_row == peak_num]).repeat(gene_feature.shape[0])
-        peak_combine_data[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_data[peak_row == peak_num]).repeat(gene_feature.shape[0])
-
-        non_count += peak_sum * gene_feature.shape[0]
-
-    # Create the final sparse peak_feature tensor
-    peak_feature_ori = torch.sparse.FloatTensor(torch.vstack((peak_combine_row, peak_combine_col)).long(), peak_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], peak_feature.shape[1])))
-    return peak_feature_ori.to(device)
-
-
-def gene_Sparse(peak_feature, gene_feature, device):
-    # Find the non-zero elements in gene_feature
-    gene_row = torch.where(gene_feature != 0)[0].to(device)
-    gene_col = torch.where(gene_feature != 0)[1].to(device)
-    gene_data = gene_feature[torch.where(gene_feature != 0)]
-
-    # Initialize a tensor for gene indices
-    gene_init = torch.zeros((peak_feature.shape[0], len(gene_row)), dtype=torch.int32).to(device)
-    for peak_id in range(peak_feature.shape[0]):
-        gene_init[peak_id] = gene_row + peak_id * gene_feature.shape[0]
-
-    # Update the combined gene data tensors
-    gene_combine_row = gene_init.reshape(1, -1)[0]
-    gene_combine_col = gene_col.repeat(1, peak_feature.shape[0])[0]
-    gene_combine_data = gene_data.repeat(peak_feature.shape[0])
-
-    # Create the final sparse gene_feature tensor
-    gene_feature_ori = torch.sparse.FloatTensor(torch.vstack((gene_combine_row, gene_combine_col)), gene_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], gene_feature.shape[1])))
-    return gene_feature_ori.to(device)
-
-
-def gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names):
-    y = ad.AnnData(RNA_matrix.transpose(), dtype='int32')
-    y.var_names=gene_names[0]
-    y.obs['pred'] = np.array(pred_label,dtype='int64')
-    y.obs['pred'] = y.obs['pred'].astype("category")
-    # Store the prediction results as a sparse matrix, where rows represent cells and columns represent cluster labels. A value of 1 at the corresponding position indicates that the cell belongs to that cluster.
-    cell_emb_binary = sp.coo_matrix((np.ones(len(y.obs['pred'])),(np.array(range(len(y.obs['pred']))),list(y.obs['pred']))))
-    cell_emb_binary.todense()
-
-    adata_atac_all = ATAC_matrix[:,nodes_id]
-    adata_rna_all = RNA_matrix[:,nodes_id]
-
-    ATAC_matrix_ct = adata_atac_all*(cell_emb_binary)
-    RNA_matrix_ct = adata_rna_all*(cell_emb_binary)
-    RNA_matrix_ct = RNA_matrix_ct/np.sum(cell_emb_binary,axis=0)
-    ATAC_matrix_ct = ATAC_matrix_ct/np.sum(cell_emb_binary,axis=0)
-
-    rna_matrix = RNA_matrix_ct
-    m = range(rna_matrix.shape[0])
-    gene_peak = RP_matrix
-    gp = gene_peak.reshape(gene_peak.shape[1]*rna_matrix.shape[0],1).todense()
-    gene_emb_enh = ATAC_matrix_ct[list(range (ATAC_matrix_ct.shape[0]))*rna_matrix.shape[0]]
-    peak_emb_enh = RNA_matrix_ct[[v for v in m for i in range(ATAC_matrix_ct.shape[0])]]
-    egrn = np.multiply(gene_emb_enh, peak_emb_enh)
-    egrn = np.multiply(egrn,gp)
-    return egrn
-
-
-def small_gene_Peak_Score(pred_label,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,choice_cluser):  
-    y = ad.AnnData(RNA_matrix.transpose(), dtype='int32')
-    y.var_names=gene_names[0]
-    y.obs['pred'] = np.array(pred_label,dtype='int64')
-    cell_emb_binary = sp.coo_matrix((np.ones(len(y.obs['pred'])),(np.array(range(len(y.obs['pred']))),list(y.obs['pred']))))
-    cell_emb_binary.todense()
-
-    adata_atac_all = ATAC_matrix
-    adata_rna_all = RNA_matrix
-
-    ATAC_matrix_ct = adata_atac_all*(cell_emb_binary)
-    RNA_matrix_ct = adata_rna_all*(cell_emb_binary)
-    
-    RNA_matrix_ct = RNA_matrix_ct/np.sum(cell_emb_binary,axis=0)
-    ATAC_matrix_ct = ATAC_matrix_ct/np.sum(cell_emb_binary,axis=0)
-
-    rna_matrix = RNA_matrix_ct
-    m = range(rna_matrix.shape[0])
-    gene_peak = RP_matrix
-    gp = gene_peak.reshape(gene_peak.shape[1]*rna_matrix.shape[0],1).todense()
-    gene_emb_enh = ATAC_matrix_ct[list(range (ATAC_matrix_ct.shape[0]))*rna_matrix.shape[0]]
-    peak_emb_enh = RNA_matrix_ct[[v for v in m for i in range(ATAC_matrix_ct.shape[0])]]
-    egrn = np.multiply(gene_emb_enh, peak_emb_enh)
-    egrn = np.multiply(egrn,gp)
-    gn = np.array(gene_names[0])[[v for v in m for i in range(ATAC_matrix.shape[0])]]
-    pn = np.array(peak_names[0])[list(range (ATAC_matrix.shape[0]))*RNA_matrix.shape[0]]
-    data = np.array(np.squeeze(egrn[:,choice_cluser]))[0]
-    gene_peak_score_Dict = {'gene': gn, 'peak': pn, 'score':data}
-    gene_peak_score_df = pd.DataFrame(data = gene_peak_score_Dict)
-    gene_peak_score = gene_peak_score_df[gene_peak_score_df['score'] > 0]
-    gene_peak_score = gene_peak_score.drop_duplicates(['gene','peak'])
-    gene_peak_score = gene_peak_score.sort_values(by="score",ascending=False)
-    
-    return gene_peak_score_df,gene_peak_score
-
-
-def egrn_calculate(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,threshold=0):
-    print('We are currently performing calculations for EGRN. Please bear with us as this process will take approximately around 10 minutes.')
-    
-    try:
-        egrn = gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names)
-        label_num = len(Counter(pred_label))
-        print('class_num:',label_num)
-        gn = np.array(gene_names[0])[[v for v in range(RNA_matrix.shape[0]) for i in range(ATAC_matrix.shape[0])]]
-        pn = np.array(peak_names[0])[list(range (ATAC_matrix.shape[0]))*RNA_matrix.shape[0]]
-        egrn_df = pd.DataFrame(columns=['gene', 'peak', 'score', 'class'])
-        print('We are currently conducting filtering and categorization operations.')
-        for i in range(label_num):
-            data = np.array(np.squeeze(egrn[:,i]))[0]
-            gene_peak_score_Dict = {'gene': gn, 'peak': pn, 'score':data}
-            gene_peak_score_df = pd.DataFrame(data = gene_peak_score_Dict)
-            gene_peak_score = gene_peak_score_df[gene_peak_score_df['score'] >threshold]
-            gene_peak_score = gene_peak_score.drop_duplicates(['gene','peak'])
-            gene_peak_score = gene_peak_score.sort_values(by="score",ascending=False)
-            gene_peak_score['class'] = i
-            egrn_df = egrn_df.append(gene_peak_score)
-    
-    except:
-        print('An error occurred with gene_Peak_Score. We will try using small_gene_Peak_Score instead.')
-        egrn_df = pd.DataFrame(columns=['gene', 'peak', 'score', 'class'])
-        Total_name = list(range(len(Counter(pred_label))))
-        for i in range(len(Counter(pred_label))):
-            Total_gene_peak_score_df,Total_gene_peak_score = gene_Peak_Score(pred_label,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,choice_cluser=i)
-            Total_gene_peak_score_df = Total_gene_peak_score_df[Total_gene_peak_score_df['score'] > threshold]
-            Total_gene_peak_score_df['class'] = Total_name[i]
-            egrn_df = egrn_df.append(Total_gene_peak_score_df.sort_values(by="score",ascending=False))
-            
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+import numpy as np
+import scipy.sparse as sp
+import anndata as ad
+from collections import Counter
+import pandas as pd
+
+
+def peak_Sparse(peak_feature, gene_feature, device):
+    # Find the non-zero elements in peak_feature
+    peak_row = torch.where(peak_feature != 0)[0].to(device)
+    peak_col = torch.where(peak_feature != 0)[1].to(device)
+    peak_data = peak_feature[torch.where(peak_feature != 0)]
+
+    # Initialize tensors for combined peak data
+    peak_combine_row = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
+    peak_combine_col = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]), dtype=torch.int32)
+    peak_combine_data = torch.zeros((peak_row.shape[0] * gene_feature.shape[0]))
+
+    non_count = 0
+    for peak_num in range(peak_feature.shape[0]):
+        # Calculate the peak sum
+        peak_sum = len(peak_row[peak_row == peak_num])
+
+        # Initialize a tensor for peak indices
+        peak_init = torch.zeros((gene_feature.shape[0], peak_sum), dtype=torch.int32).to(device)
+        for id in range(gene_feature.shape[0]):
+            peak_init[id,] = id + peak_num * gene_feature.shape[0]
+
+        # Update the combined peak data tensors
+        peak_combine_row[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_row[peak_row == peak_num] + peak_init - peak_num).reshape(1, -1)
+        peak_combine_col[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_col[peak_row == peak_num]).repeat(gene_feature.shape[0])
+        peak_combine_data[non_count:non_count + peak_sum * gene_feature.shape[0]] = (peak_data[peak_row == peak_num]).repeat(gene_feature.shape[0])
+
+        non_count += peak_sum * gene_feature.shape[0]
+
+    # Create the final sparse peak_feature tensor
+    peak_feature_ori = torch.sparse.FloatTensor(torch.vstack((peak_combine_row, peak_combine_col)).long(), peak_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], peak_feature.shape[1])))
+    return peak_feature_ori.to(device)
+
+
+def gene_Sparse(peak_feature, gene_feature, device):
+    # Find the non-zero elements in gene_feature
+    gene_row = torch.where(gene_feature != 0)[0].to(device)
+    gene_col = torch.where(gene_feature != 0)[1].to(device)
+    gene_data = gene_feature[torch.where(gene_feature != 0)]
+
+    # Initialize a tensor for gene indices
+    gene_init = torch.zeros((peak_feature.shape[0], len(gene_row)), dtype=torch.int32).to(device)
+    for peak_id in range(peak_feature.shape[0]):
+        gene_init[peak_id] = gene_row + peak_id * gene_feature.shape[0]
+
+    # Update the combined gene data tensors
+    gene_combine_row = gene_init.reshape(1, -1)[0]
+    gene_combine_col = gene_col.repeat(1, peak_feature.shape[0])[0]
+    gene_combine_data = gene_data.repeat(peak_feature.shape[0])
+
+    # Create the final sparse gene_feature tensor
+    gene_feature_ori = torch.sparse.FloatTensor(torch.vstack((gene_combine_row, gene_combine_col)), gene_combine_data, torch.Size((gene_feature.shape[0] * peak_feature.shape[0], gene_feature.shape[1])))
+    return gene_feature_ori.to(device)
+
+
+def gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names):
+    y = ad.AnnData(RNA_matrix.transpose(), dtype='int32')
+    y.var_names=gene_names[0]
+    y.obs['pred'] = np.array(pred_label,dtype='int64')
+    y.obs['pred'] = y.obs['pred'].astype("category")
+    # Store the prediction results as a sparse matrix, where rows represent cells and columns represent cluster labels. A value of 1 at the corresponding position indicates that the cell belongs to that cluster.
+    cell_emb_binary = sp.coo_matrix((np.ones(len(y.obs['pred'])),(np.array(range(len(y.obs['pred']))),list(y.obs['pred']))))
+    cell_emb_binary.todense()
+
+    adata_atac_all = ATAC_matrix[:,nodes_id]
+    adata_rna_all = RNA_matrix[:,nodes_id]
+
+    ATAC_matrix_ct = adata_atac_all*(cell_emb_binary)
+    RNA_matrix_ct = adata_rna_all*(cell_emb_binary)
+    RNA_matrix_ct = RNA_matrix_ct/np.sum(cell_emb_binary,axis=0)
+    ATAC_matrix_ct = ATAC_matrix_ct/np.sum(cell_emb_binary,axis=0)
+
+    rna_matrix = RNA_matrix_ct
+    m = range(rna_matrix.shape[0])
+    gene_peak = RP_matrix
+    gp = gene_peak.reshape(gene_peak.shape[1]*rna_matrix.shape[0],1).todense()
+    gene_emb_enh = ATAC_matrix_ct[list(range (ATAC_matrix_ct.shape[0]))*rna_matrix.shape[0]]
+    peak_emb_enh = RNA_matrix_ct[[v for v in m for i in range(ATAC_matrix_ct.shape[0])]]
+    egrn = np.multiply(gene_emb_enh, peak_emb_enh)
+    egrn = np.multiply(egrn,gp)
+    return egrn
+
+
+def small_gene_Peak_Score(pred_label,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,choice_cluser):  
+    y = ad.AnnData(RNA_matrix.transpose(), dtype='int32')
+    y.var_names=gene_names[0]
+    y.obs['pred'] = np.array(pred_label,dtype='int64')
+    cell_emb_binary = sp.coo_matrix((np.ones(len(y.obs['pred'])),(np.array(range(len(y.obs['pred']))),list(y.obs['pred']))))
+    cell_emb_binary.todense()
+
+    adata_atac_all = ATAC_matrix
+    adata_rna_all = RNA_matrix
+
+    ATAC_matrix_ct = adata_atac_all*(cell_emb_binary)
+    RNA_matrix_ct = adata_rna_all*(cell_emb_binary)
+    
+    RNA_matrix_ct = RNA_matrix_ct/np.sum(cell_emb_binary,axis=0)
+    ATAC_matrix_ct = ATAC_matrix_ct/np.sum(cell_emb_binary,axis=0)
+
+    rna_matrix = RNA_matrix_ct
+    m = range(rna_matrix.shape[0])
+    gene_peak = RP_matrix
+    gp = gene_peak.reshape(gene_peak.shape[1]*rna_matrix.shape[0],1).todense()
+    gene_emb_enh = ATAC_matrix_ct[list(range (ATAC_matrix_ct.shape[0]))*rna_matrix.shape[0]]
+    peak_emb_enh = RNA_matrix_ct[[v for v in m for i in range(ATAC_matrix_ct.shape[0])]]
+    egrn = np.multiply(gene_emb_enh, peak_emb_enh)
+    egrn = np.multiply(egrn,gp)
+    gn = np.array(gene_names[0])[[v for v in m for i in range(ATAC_matrix.shape[0])]]
+    pn = np.array(peak_names[0])[list(range (ATAC_matrix.shape[0]))*RNA_matrix.shape[0]]
+    data = np.array(np.squeeze(egrn[:,choice_cluser]))[0]
+    gene_peak_score_Dict = {'gene': gn, 'peak': pn, 'score':data}
+    gene_peak_score_df = pd.DataFrame(data = gene_peak_score_Dict)
+    gene_peak_score = gene_peak_score_df[gene_peak_score_df['score'] > 0]
+    gene_peak_score = gene_peak_score.drop_duplicates(['gene','peak'])
+    gene_peak_score = gene_peak_score.sort_values(by="score",ascending=False)
+    
+    return gene_peak_score_df,gene_peak_score
+
+
+def egrn_calculate(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,threshold=0):
+    print('We are currently performing calculations for EGRN. Please bear with us as this process will take approximately around 10 minutes.')
+    
+    try:
+        egrn = gene_Peak_Score(pred_label,nodes_id,RNA_matrix,ATAC_matrix,RP_matrix,gene_names)
+        label_num = len(Counter(pred_label))
+        print('class_num:',label_num)
+        gn = np.array(gene_names[0])[[v for v in range(RNA_matrix.shape[0]) for i in range(ATAC_matrix.shape[0])]]
+        pn = np.array(peak_names[0])[list(range (ATAC_matrix.shape[0]))*RNA_matrix.shape[0]]
+        egrn_df = pd.DataFrame(columns=['gene', 'peak', 'score', 'class'])
+        print('We are currently conducting filtering and categorization operations.')
+        for i in range(label_num):
+            data = np.array(np.squeeze(egrn[:,i]))[0]
+            gene_peak_score_Dict = {'gene': gn, 'peak': pn, 'score':data}
+            gene_peak_score_df = pd.DataFrame(data = gene_peak_score_Dict)
+            gene_peak_score = gene_peak_score_df[gene_peak_score_df['score'] >threshold]
+            gene_peak_score = gene_peak_score.drop_duplicates(['gene','peak'])
+            gene_peak_score = gene_peak_score.sort_values(by="score",ascending=False)
+            gene_peak_score['class'] = i
+            egrn_df = egrn_df.append(gene_peak_score)
+    
+    except:
+        try:
+            print('An error occurred with gene_Peak_Score. We will try using small_gene_Peak_Score instead.')
+            egrn_df = pd.DataFrame(columns=['gene', 'peak', 'score', 'class'])
+            Total_name = list(range(len(Counter(pred_label))))
+            for i in range(len(Counter(pred_label))):
+                Total_gene_peak_score_df,Total_gene_peak_score = small_gene_Peak_Score(pred_label,RNA_matrix,ATAC_matrix,RP_matrix,gene_names,peak_names,choice_cluser=i)
+                Total_gene_peak_score_df = Total_gene_peak_score_df[Total_gene_peak_score_df['score'] > threshold]
+                Total_gene_peak_score_df['class'] = Total_name[i]
+                egrn_df = egrn_df.append(Total_gene_peak_score_df.sort_values(by="score",ascending=False))
+        except:
+            print('You are encountering memory shortage issues, please follow the tutorial instructions to address it.')
+            egrn_df = pd.DataFrame(columns=['gene', 'peak', 'score', 'class'])
+            pass
+            
     return egrn_df
```

### Comparing `MarsGT-0.1.5/MarsGT/marsgt_model.py` & `MarsGT-0.1.6/MarsGT/marsgt_model.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.5/MarsGT/utils.py` & `MarsGT-0.1.6/MarsGT/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,25 +110,24 @@
     print(
         '\tWhen the number of cells is less than or equal to 500, it is recommended to set the resolution value to 0.2.')
     print('\tWhen the number of cells is within the range of 500 to 5000, the resolution value should be set to 0.5.')
     print('\tWhen the number of cells is greater than 5000, the resolution value should be set to 0.8.')
 
     def segment_function(x):
         if x <= 500:
-            return 0.2
+            return 0.2,5
         elif x <= 5000:
-            return 0.5
+            return 0.5,10
         else:
-            return 0.8
-
+            return 0.8,15
     adata = ad.AnnData(RNA_matrix.transpose(), dtype='int32')
+    resolution,n_neighbors = segment_function(adata.shape[0])
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     sc.pp.neighbors(adata, n_neighbors=n_neighbors, n_pcs=n_pcs)
-    resolution = segment_function(adata.shape[0])
     sc.tl.leiden(adata, resolution)
     #     sc.tl.umap(adata)
     #     sc.pl.umap(adata, color=['leiden'])
     return adata.obs['leiden']
 
 
 def purity_score(y_true, y_pred):
```

### Comparing `MarsGT-0.1.5/MarsGT.egg-info/PKG-INFO` & `MarsGT-0.1.6/MarsGT.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.5
+Version: 0.1.6
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
 Provides-Extra: torch_cluster
 
@@ -24,7 +26,9 @@
 ```bash
 pip install -r requirements.txt
 ```
 * use pip to install MarsGT:
 ```bash
 pip install MarsGT
 ```
+
+
```

### Comparing `MarsGT-0.1.5/PKG-INFO` & `MarsGT-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.5
+Version: 0.1.6
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ==3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
 Provides-Extra: torch_cluster
 
@@ -24,7 +26,9 @@
 ```bash
 pip install -r requirements.txt
 ```
 * use pip to install MarsGT:
 ```bash
 pip install MarsGT
 ```
+
+
```

### Comparing `MarsGT-0.1.5/README.md` & `MarsGT-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.5/setup.py` & `MarsGT-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="MarsGT",
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'anndata==0.8.0',
         'dill==0.3.4',
         'matplotlib==3.5.1',
         'numpy==1.22.3',
         'pandas==1.4.2',
```

