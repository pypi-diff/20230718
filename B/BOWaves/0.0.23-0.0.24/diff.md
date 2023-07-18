# Comparing `tmp/BOWaves-0.0.23.tar.gz` & `tmp/BOWaves-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BOWaves-0.0.23.tar", last modified: Mon Jul 10 20:14:17 2023, max compression
+gzip compressed data, was "dist/BOWaves-0.0.24.tar", last modified: Tue Jul 18 19:18:43 2023, max compression
```

## Comparing `BOWaves-0.0.23.tar` & `BOWaves-0.0.24.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-10 20:14:17.000000 BOWaves-0.0.23/
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-10 20:14:17.000000 BOWaves-0.0.23/BOWaves/
--rw-rw-r--   0 austin    (1000) austin    (1000)       71 2023-07-10 18:54:10.000000 BOWaves-0.0.23/BOWaves/__init__.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-10 20:14:17.000000 BOWaves-0.0.23/BOWaves/scripts/
--rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-07-10 19:49:06.000000 BOWaves-0.0.23/BOWaves/scripts/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      945 2023-07-10 19:41:48.000000 BOWaves-0.0.23/BOWaves/scripts/gen_morlet_signal.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     4936 2023-07-10 19:46:42.000000 BOWaves-0.0.23/BOWaves/scripts/run_sikmeans.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-10 20:14:17.000000 BOWaves-0.0.23/BOWaves/sikmeans/
--rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-07-10 19:46:55.000000 BOWaves-0.0.23/BOWaves/sikmeans/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)    18963 2023-07-10 19:41:49.000000 BOWaves-0.0.23/BOWaves/sikmeans/sikmeans_core.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-10 20:14:17.000000 BOWaves-0.0.23/BOWaves/utilities/
--rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-07-10 19:47:06.000000 BOWaves-0.0.23/BOWaves/utilities/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1223 2023-07-10 19:41:49.000000 BOWaves-0.0.23/BOWaves/utilities/datasets.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     5606 2023-07-10 14:42:58.000000 BOWaves-0.0.23/BOWaves/utilities/sikmeans_utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)    10799 2023-06-21 15:59:47.000000 BOWaves-0.0.23/BOWaves/utilities/utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     4016 2023-07-10 14:42:58.000000 BOWaves-0.0.23/BOWaves/utilities/wrappers.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-10 20:14:17.000000 BOWaves-0.0.23/BOWaves.egg-info/
--rw-rw-r--   0 austin    (1000) austin    (1000)      620 2023-07-10 20:14:16.000000 BOWaves-0.0.23/BOWaves.egg-info/PKG-INFO
--rw-rw-r--   0 austin    (1000) austin    (1000)      475 2023-07-10 20:14:16.000000 BOWaves-0.0.23/BOWaves.egg-info/SOURCES.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)        1 2023-07-10 20:14:16.000000 BOWaves-0.0.23/BOWaves.egg-info/dependency_links.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)        8 2023-07-10 20:14:16.000000 BOWaves-0.0.23/BOWaves.egg-info/top_level.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)      620 2023-07-10 20:14:17.000000 BOWaves-0.0.23/PKG-INFO
--rw-rw-r--   0 austin    (1000) austin    (1000)     1413 2023-07-10 15:48:51.000000 BOWaves-0.0.23/README.md
--rw-rw-r--   0 austin    (1000) austin    (1000)       38 2023-07-10 20:14:17.000000 BOWaves-0.0.23/setup.cfg
--rw-rw-r--   0 austin    (1000) austin    (1000)     1139 2023-07-10 20:13:46.000000 BOWaves-0.0.23/setup.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-18 19:18:43.000000 BOWaves-0.0.24/
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves/
+-rw-rw-r--   0 austin    (1000) austin    (1000)       71 2023-07-18 14:19:23.000000 BOWaves-0.0.24/BOWaves/__init__.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves/scripts/
+-rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-07-18 14:19:23.000000 BOWaves-0.0.24/BOWaves/scripts/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      945 2023-07-18 14:19:23.000000 BOWaves-0.0.24/BOWaves/scripts/gen_morlet_signal.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     5125 2023-07-18 14:31:17.000000 BOWaves-0.0.24/BOWaves/scripts/run_sikmeans.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves/sikmeans/
+-rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-07-18 14:19:23.000000 BOWaves-0.0.24/BOWaves/sikmeans/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1184 2023-07-18 18:10:36.000000 BOWaves-0.0.24/BOWaves/sikmeans/sample_data_gen.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)    25664 2023-07-18 18:40:19.000000 BOWaves-0.0.24/BOWaves/sikmeans/sikmeans_core.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves/utilities/
+-rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-07-18 14:19:23.000000 BOWaves-0.0.24/BOWaves/utilities/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1223 2023-07-18 14:19:23.000000 BOWaves-0.0.24/BOWaves/utilities/datasets.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     5607 2023-07-18 14:28:56.000000 BOWaves-0.0.24/BOWaves/utilities/sikmeans_utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)    11409 2023-07-18 18:00:07.000000 BOWaves-0.0.24/BOWaves/utilities/utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     9698 2023-07-18 14:28:56.000000 BOWaves-0.0.24/BOWaves/utilities/wrappers.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves.egg-info/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      620 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves.egg-info/PKG-INFO
+-rw-rw-r--   0 austin    (1000) austin    (1000)      511 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves.egg-info/SOURCES.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)        1 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves.egg-info/dependency_links.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)        8 2023-07-18 19:18:43.000000 BOWaves-0.0.24/BOWaves.egg-info/top_level.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)      620 2023-07-18 19:18:43.000000 BOWaves-0.0.24/PKG-INFO
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1920 2023-07-18 19:13:03.000000 BOWaves-0.0.24/README.md
+-rw-rw-r--   0 austin    (1000) austin    (1000)       38 2023-07-18 19:18:43.000000 BOWaves-0.0.24/setup.cfg
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1139 2023-07-18 19:18:36.000000 BOWaves-0.0.24/setup.py
```

### Comparing `BOWaves-0.0.23/BOWaves/scripts/gen_morlet_signal.py` & `BOWaves-0.0.24/BOWaves/scripts/gen_morlet_signal.py`

 * *Files identical despite different names*

### Comparing `BOWaves-0.0.23/BOWaves/scripts/run_sikmeans.py` & `BOWaves-0.0.24/BOWaves/scripts/run_sikmeans.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from argparse import ArgumentParser
-import os
 from time import perf_counter
-os.unsetenv('OMP_THREAD_LIMIT')
 from pathlib import Path
 import numpy as np
 
 import os
 import sys
 import matplotlib.pyplot as plt
+os.unsetenv('OMP_THREAD_LIMIT')
 
 currentdir = os.path.dirname(os.path.abspath(__file__))
 parentdir = os.path.dirname(currentdir)
 sys.path.insert(0, parentdir)
 
 from BOWaves.sikmeans.sikmeans_core import shift_invariant_k_means
 
@@ -26,14 +25,15 @@
 parser.add_argument("--window-len", type=int, default=768,
                     help="Length of non-overlapping window length")
 parser.add_argument('--num-clusters', type=int,
                     default=128, help='Number of clusters')
 parser.add_argument('--visualize', default=True, help="Print out codebooks")
 parser.add_argument('--visualize_cutoff', type=int, default=5,
                     help="Only centroids with this many occurrences or above are visualized. Set to zero to visualize all")
+# TODO - make metric and init type as command line arguments
 
 args = parser.parse_args()
 win_len = args.window_len
 root = Path(args.root)
 data_dir = root.joinpath('data', args.experiment)
 data_dir.mkdir(exist_ok=True)
 
@@ -43,14 +43,23 @@
 
 
 fpath = list(data_dir.glob('*.npz'))[0]
 with np.load(fpath, allow_pickle=True) as data:
     T = data['T']
     splice = data['splice']
 
+data = np.load(fpath)
+# for key in data.keys():
+#     print(key)
+
+data = data['T']
+#calculate variance before splitting into windows
+variance = np.var(data)
+#print("Variance: ", variance)
+
 tot_win = np.sum(np.diff(np.r_[0, splice, T.size])//win_len)
 X = np.zeros((tot_win, win_len))
 start_arr = np.r_[0, splice]
 end_arr = np.r_[splice, T.size]
 start_x = 0
 for start, end in zip(start_arr, end_arr):
     segment = T[start:end]
@@ -135,9 +144,8 @@
 
     # Save the plot to images subdirectory
     img_dir = root.joinpath('img')#, args.experiment)
     img_dir.mkdir(exist_ok=True)
     img_dir_exp = img_dir.joinpath(args.experiment)
     img_dir_exp.mkdir(exist_ok=True)
 
-    img_file = str(out_file).replace('.npz', '_img')
-    plt.savefig(str(img_dir_exp) + '/' + img_file)
+    img_file = str(out_file).replace('.npz', '_img')
```

### Comparing `BOWaves-0.0.23/BOWaves/sikmeans/sikmeans_core.py` & `BOWaves-0.0.24/BOWaves/sikmeans/sikmeans_core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,159 @@
 """Shift-invariant k-means"""
 
 import sys
 import warnings
+from pathlib import Path
+from time import perf_counter
+import matplotlib.pyplot as plt
 
 import numpy as np
 import scipy.sparse as sp
 
 from sklearn.utils.extmath import stable_cumsum, squared_norm, row_norms
 from sklearn.exceptions import ConvergenceWarning
 
 from BOWaves.utilities import sikmeans_utils, wrappers
 
 
+
+def run(experiment, root, centroid_len=512, win_len=768, num_clusters=128, visualize=True, visualize_cutoff=5):
+    """
+
+    Parameters
+    ----------
+    experiment: This is the name of the experiment and what you should call your subdirectory.
+    root: Path to the root folder.
+    centroid_len: Length of centroids. Default=512
+    win_len: Non-overlapping window length. Default=768
+    num_clusters: Number of clusters. Default=128
+    visualize: Whether or not to visualize the results, output to /img. Default=True
+    visualize_cutoff: Only centroids with this many occurences or above are visualized. Default=5
+
+    Returns
+    -------
+    Returns nothing, but prints out values and saves visualizations and numpy data to img and results folders, respectively.
+    """
+
+    t_start = perf_counter()
+
+    root = Path(root)
+    data_dir = root.joinpath('data', experiment)
+    data_dir.mkdir(exist_ok=True)
+
+    results_dir = root.joinpath('results')
+    results_dir.mkdir(exist_ok=True)
+
+    results_dir = root.joinpath('results', experiment)
+    results_dir.mkdir(exist_ok=True)
+
+    fpath = list(data_dir.glob('*.npz'))[0]
+    with np.load(fpath, allow_pickle=True) as data:
+        T = data['T']
+        splice = data['splice']
+
+    data = np.load(fpath)
+
+    data = data['T']
+    # calculate variance before splitting into windows
+    variance = np.var(data)
+
+    tot_win = np.sum(np.diff(np.r_[0, splice, T.size]) // win_len)
+    X = np.zeros((tot_win, win_len))
+    start_arr = np.r_[0, splice]
+    end_arr = np.r_[splice, T.size]
+    start_x = 0
+    for start, end in zip(start_arr, end_arr):
+        segment = T[start:end]
+        n_win = segment.size // win_len
+        i_win = np.arange(0, n_win * win_len, win_len)
+        i_win = i_win[:, None] + np.arange(win_len)[None, :]
+        X[start_x:start_x + n_win] = segment[i_win]
+        start_x = start_x + n_win
+
+    k, P = num_clusters, centroid_len
+    metric, init = 'cosine', 'random'
+    n_runs, rng = 30, 13
+    centroids, labels, shifts, distances, _, _ = shift_invariant_k_means(
+        X, k, P, metric=metric, init=init, n_init=n_runs, rng=rng, verbose=True)
+
+    out_file = f'sikmeans_k-{k}_P-{P}_wlen-{win_len}.npz'
+    out_file_full = results_dir.joinpath(out_file)
+    with out_file_full.open('wb') as f:
+        np.savez(f, centroids=centroids, labels=labels,
+                 shifts=shifts, distances=distances)
+
+    t_stop = perf_counter()
+    print(f'Finished after {t_stop - t_start} seconds!')
+
+    # out_file = f'sikmeans_k-128_P-512_wlen-768.npz'
+    # out_file_full = results_dir.joinpath(out_file)
+
+    if visualize:
+        with np.load(out_file_full) as data:
+            centroids = data['centroids']
+            labels = data['labels']
+            shifts = data['shifts']
+            distances = data['distances']
+
+        unique_labels, cluster_size = np.unique(labels, return_counts=True)
+
+        # Sort centroids in descending order of cluster size
+        isort = np.argsort(-cluster_size)
+        centroids = centroids[isort]
+        unique_labels = unique_labels[isort]
+        cluster_size = cluster_size[isort]
+        # Determine the grid dimensions based on the number of centroids
+
+        # determine number of centroids over some cluster size cutoff
+        # args.visualize_cutoff = 5
+        number = 0
+        for i in cluster_size:
+            if i >= visualize_cutoff:
+                number += 1
+
+        num_centroids = len(centroids)
+        num_rows = int(np.ceil(np.sqrt(number)))
+        num_cols = int(np.ceil(number / num_rows))
+
+        # Create subplots with the determined grid dimensions
+        fig, axs = plt.subplots(num_rows, num_cols, figsize=(12, 8))
+
+        # Flatten the axs array if necessary
+        if num_centroids == 1:
+            axs = np.array([axs])
+
+        # Iterate over the centroids and plot each as a waveform in a separate subplot
+        for i, centroid in enumerate(centroids):
+            if cluster_size[i] >= 5:
+                # Determine the subplot indices
+                row_idx = i // num_cols
+                col_idx = i % num_cols
+
+                # Plot the waveform in the corresponding subplot
+                axs[row_idx, col_idx].plot(centroid)
+                # axs[row_idx, col_idx].set_title(f"Centroid {i + 1}")
+                axs[row_idx, col_idx].set_title(cluster_size[i])
+
+        # Remove empty subplots if the number of centroids is not a perfect square
+        if num_centroids % num_cols != 0:
+            for i in range(num_centroids, num_rows * num_cols):
+                axs.flatten()[i].axis('off')
+
+        # Adjust the spacing between subplots
+        plt.tight_layout()
+
+        # Save the plot to images subdirectory
+        img_dir = root.joinpath('img')  # , args.experiment)
+        img_dir.mkdir(exist_ok=True)
+        img_dir_exp = img_dir.joinpath(experiment)
+        img_dir_exp.mkdir(exist_ok=True)
+
+        img_file = str(out_file).replace('.npz', '_img')
+
 ###############################################################################
 # Initialization
 
 
 def init_centroids(X, n_clusters, centroid_length, metric='euclidean',\
     init='k-means++', x_squared_norms=None, rng=None, **kwargs):
     """
@@ -24,15 +162,15 @@
     Parameters
     ----------
     X (numpy.ndarray):
         Training data. Rows are samples.
     n_clusters (int):
         Number of initial seed centroids
     centroid_length (int):
-        Lenght of each centroid
+        Length of each centroid
     init ('k-means++', 'random', numpy.ndarray, or a function):
         Method for initialization. If it's a function, it should have this
         call signature:
         centroids, shifts = init(
             X, n_clusters, centroid_length, rng, **kwargs).
         rng must be a Generator instance.
     x_squared_norms (numpy.ndarray or None):
@@ -385,21 +523,28 @@
     best_labels, best_shifts, best_centroids = None, None, None
     best_distances, best_inertia = None, None
 
     # Init
     centroids = init_centroids(
         X, n_clusters, centroid_length, metric, init, x_squared_norms, rng)
 
+    #The below is Dr. B's additions from the Jupyter notebook.
+    #I've added the update step function to the utils file.
+    #Adding here to test before PR
+    labels, shifts, distances = _assignment_step(
+        X, centroids, metric, x_squared_norms)
+    centroids = _init_centroids_update_step(
+        X, centroid_length, n_clusters, labels, shifts) # NEW
+
     if verbose:
         print('Initialization completed.')
 
     for iteration in range(max_iter):
         centroids_old = centroids.copy()
-        labels, shifts, distances = _asignment_step(
-            X, centroids, metric, x_squared_norms)
+        labels, shifts, distances = _assignment_step(X, centroids, metric, x_squared_norms)
         centroids = _centroids_update_step(
             X, centroid_length, n_clusters, labels, shifts)
 
         inertia = distances.sum()
 
         if verbose:
             print("Iteration %2d, inertia %.3f" % (iteration, inertia))
@@ -408,55 +553,58 @@
             best_labels = labels.copy()
             best_shifts = shifts.copy()
             best_centroids = centroids.copy()
             best_distances = distances
             best_inertia = inertia
 
         centroid_change = squared_norm(centroids_old - centroids)
+        #print(centroid_change, tol)
         if centroid_change <= tol:
             if verbose:
                 print("Converged at iteration %d: "
                       "centroid changes %e within tolerance %e"
                       % (iteration, centroid_change, tol))
             break
 
     if centroid_change > 0:
         # rerun asingment step in case of non-convergence so that predicted
         # labels match cluster centers
-        best_labels, best_shifts, distances = _asignment_step(
-            X, best_centroids, metric, x_squared_norms)
+        best_labels, best_shifts, distances = _assignment_step(X, best_centroids, metric, x_squared_norms)
         best_inertia = distances.sum()
 
     return best_centroids, best_labels, best_shifts, best_distances, best_inertia, iteration+1
 
 
-def _asignment_step(X, centroids, metric, x_squared_norms):
+def _assignment_step(X, centroids, metric, x_squared_norms):
     """
     Find the index of the shifted centroid that is closest to each sample
 
     Parameters
     ----------
     X (numpy.ndarray):
         Training data. Rows of X are samples.
     centroids (numpy.ndarray):
         Centroids of the clusters.
     x_squared_norms (numpy.ndarray):
-        Squared euclidean norm of rows of X. This is used to speed up the
-        computation of the euclidean distances between samples and centroids.
+        Squared Euclidean norm of rows of X. This is used to speed up the
+        computation of the Euclidean distances between samples and centroids.
 
     Returns
     -------
     labels (numpy.ndarray):
         centroids[labels[i]] is the centroid closest to sample X[i]
     shifts (numpy.ndarray):
         X[i, shifts[i]:shifts[i]+centroid_length] is the window in X[i]  closest to centroids[labels[i]].
     distances (numpy.ndarray):
         distances[i] is the distance of X[i, shifts[i]:shifts[i]+ centroid_length] to the closest centroid.
     """
 
+    #for testing
+    #metric = 'euclidean'
+
     labels, shifts, distances =\
         wrappers.si_pairwise_distances_argmin_min(
             X, centroids, metric, x_squared_norms)
 
     # Samples whose distance to the silent waveform (i.e, their own norm) is
     # smaller than the smallest distance to one cluster are left unassigned.
 #    xsn = x_squared_norms[shifts, np.arange(X.shape[0])]
@@ -479,7 +627,42 @@
         centroids[cluster_id] += sample[shift:shift+centroid_length]
 
     # NOTE: Some clusters might be empty
     cluster_id, cluster_size = np.unique(labels, return_counts=True)
     centroids[cluster_id, :] /= cluster_size[:, np.newaxis]
 
     return centroids
+
+
+def _init_centroids_update_step(X, centroid_length, n_clusters, labels, shifts):
+    """
+    Update the cluster centroids
+    """
+
+    cluster_ids, _ = np.unique(labels, return_counts=True)
+    centroids = np.zeros((n_clusters, centroid_length))
+    n_samples, sample_length = X.shape
+    # adjust the shifts such that after adjustment the median shift is
+    max_shift = sample_length - centroid_length
+    opt_shift = max_shift/2
+    adjusts = np.zeros((n_clusters))
+    for k in cluster_ids:
+        shifts_k = shifts[labels==k]
+        adjusts[k] = opt_shift-np.median(shifts_k)
+
+    cluster_sizes = np.zeros((n_clusters,1))
+    for sample_id, sample in enumerate(X):
+        cluster_id = labels[sample_id]
+        temp = shifts[sample_id]+adjusts[cluster_id]
+        if temp >= 0 and temp <= max_shift:
+            shift = np.floor(temp).astype(int)
+            centroids[cluster_id] += sample[shift:shift+centroid_length]
+            cluster_sizes[cluster_id] += 1
+
+    # NOTE: Some clusters might be empty drop them
+    #centroids/= cluster_sizes
+    for k in np.where(cluster_sizes==0)[0]:
+        centroids[k,:] = 0
+    for k in np.nonzero(cluster_sizes)[0]:
+        centroids[k,:]/= cluster_sizes[k]
+
+    return centroids
```

### Comparing `BOWaves-0.0.23/BOWaves/utilities/datasets.py` & `BOWaves-0.0.24/BOWaves/utilities/datasets.py`

 * *Files identical despite different names*

### Comparing `BOWaves-0.0.23/BOWaves/utilities/sikmeans_utils.py` & `BOWaves-0.0.24/BOWaves/utilities/sikmeans_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,7 +166,8 @@
         col_id = np.arange(window_length).reshape((1, 1, window_length))
         row_id = np.arange(n_rows).reshape(n_rows, 1, 1)
 
     # After broadcasting, col_id.shape=(n_rows,n_offsets,window_length)
     col_id = col_id + offset
 
     return array[row_id, col_id]
+
```

### Comparing `BOWaves-0.0.23/BOWaves/utilities/utils.py` & `BOWaves-0.0.24/BOWaves/utilities/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from pathlib import Path
 
 # Pattern for path to file rx < id > .mat
 FILE_ID_PAT = '.*/rx(?P<id>\d+).mat$'
 RX_GLOB = 'rx*.mat'
 
 def get_project_root() -> str:
-    return str(Path(__file__).parent.parent)
+    # three parents since nested in package form now
+    # need to find the root of the users. Is this correct or will this be different when someone imports it?
+    return str(Path(__file__).parent.parent.parent)
+
 
 def check_rng(seed):
     """Turn seed into a np.random.Generator instance
 
     Parameters
     ----------
     seed : None, int or instance of Generator
@@ -338,7 +341,26 @@
         )
 
     def __call__(self, caller):
         fn_name = f'_{caller}'
         fn = getattr(self, fn_name)
 
         return fn()
+
+
+# May redo this later to automatically adjust tolerance by variance. otherwise use np.var() call for variance.
+# def variance(data):
+#     """
+#     This is for finding the variance of a time series signal, so that we can adjust the tolerance of the kmeans.
+#
+#     Parameters
+#     ----------
+#     data: Numpy array.
+#
+#     Returns
+#     -------
+#     variance: Float. What the variance of the time series is
+#     """
+#
+#
+#
+#     pass
```

### Comparing `BOWaves-0.0.23/BOWaves.egg-info/PKG-INFO` & `BOWaves-0.0.24/BOWaves.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BOWaves
-Version: 0.0.23
+Version: 0.0.24
 Summary: Learning representative waveforms
 Author: ameek2 (CNIEL @ UD)
 Author-email: <austin.meek10@gmail.com>
 Keywords: python,EEG,time series,dictionary learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BOWaves-0.0.23/PKG-INFO` & `BOWaves-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BOWaves
-Version: 0.0.23
+Version: 0.0.24
 Summary: Learning representative waveforms
 Author: ameek2 (CNIEL @ UD)
 Author-email: <austin.meek10@gmail.com>
 Keywords: python,EEG,time series,dictionary learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BOWaves-0.0.23/README.md` & `BOWaves-0.0.24/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
-# shift_kmeans demo
+# Bag of Waves
 
 This is a demo of the shift invariant k-means algorithm. Currently this is run on synthetic morlet data.
 
 By default, the morlet data and results from running sikmeans on it are included in the repo.
 
 If you'd like to run this on data of your own, create a subdirectory with the experiment name you'd like in both the data and results directories.
-The data needs to be in .npz format. Then, navigate to the scripts subdirectory in your terminal and run the following command:
+The data needs to be in .npz format. Then import the core API call from BOWaves.sikmeans.sikmeans_core as such:
 
-python run_sikmeans.py EXPERIMENT_NAME --root='root/directory'
+    from BOWaves.sikmeans.sikmeans_core import run
+    run('experiment_name', '/path/to/root/directory')
+
+Additionally, if you want to run the code on some sample synthetic Morlet signal data:
+
+    from BOWaves.sikmeans.sample_data_gen import generate_morlet_signal
+    generate_morlet_signal()
+
+If you've cloned the repo (use API when importing as package from pypi) and you'd like to still use the command line method to run the code, navigate to the scripts subdirectory in your terminal and run the following command:
+
+    python run_sikmeans.py EXPERIMENT_NAME --root='root/directory'
 
 There are other command line options available which you can find by checking run_sikmeans.py. 
-By default the script will save an image of the centroids it finds within your data that have at least 5 occurrences or more. This is a hyperparameter.
+By default, the script will save an image of the centroids it finds within your data that have at least 5 occurrences or more. This is a hyperparameter.
 
 Please let me (Austin Meek) know if you have any questions.
 
 ## Install
 
     pip install BOWaves
```

### Comparing `BOWaves-0.0.23/setup.py` & `BOWaves-0.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # import os
 #
 # here = os.path.abspath(os.path.dirname(__file__))
 #
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.0.23'
+VERSION = '0.0.24'
 DESCRIPTION = 'Learning representative waveforms'
 LONG_DESCRIPTION = 'Learning representative waveforms for time series clustering and dictionary learning'
 
 # Setting up
 setup(
     name="BOWaves",
     version=VERSION,
```

