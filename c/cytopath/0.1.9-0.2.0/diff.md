# Comparing `tmp/cytopath-0.1.9.tar.gz` & `tmp/cytopath-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cytopath-0.1.9.tar", last modified: Sun Nov 27 23:39:35 2022, max compression
+gzip compressed data, was "dist/cytopath-0.2.0.tar", last modified: Tue Jul 18 00:37:17 2023, max compression
```

## Comparing `cytopath-0.1.9.tar` & `cytopath-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-27 23:39:35.193019 cytopath-0.1.9/
--rw-------   0 ubuntu    (1000) ubuntu    (1000)     1799 2021-06-11 14:57:59.000000 cytopath-0.1.9/.gitignore
--rw-------   0 ubuntu    (1000) ubuntu    (1000)     1520 2021-06-11 14:57:59.000000 cytopath-0.1.9/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2022-11-27 23:39:35.193019 cytopath-0.1.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1743 2022-11-27 23:36:54.000000 cytopath-0.1.9/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-27 23:39:35.105019 cytopath-0.1.9/cytopath/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-11-27 23:36:54.000000 cytopath-0.1.9/cytopath/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20812 2022-11-27 23:36:54.000000 cytopath-0.1.9/cytopath/markov_chain_sampler.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      561 2022-02-15 05:04:27.000000 cytopath-0.1.9/cytopath/plotting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-27 23:39:35.149019 cytopath-0.1.9/cytopath/plotting_functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2022-02-15 05:04:27.000000 cytopath-0.1.9/cytopath/plotting_functions/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5537 2021-07-30 14:28:04.000000 cytopath-0.1.9/cytopath/plotting_functions/plot_alignment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6429 2022-03-26 21:22:07.000000 cytopath-0.1.9/cytopath/plotting_functions/plot_radial_heatmap.py
--rw-------   0 ubuntu    (1000) ubuntu    (1000)      718 2021-06-11 14:58:00.000000 cytopath-0.1.9/cytopath/plotting_functions/plot_sampling.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-27 23:39:35.193019 cytopath-0.1.9/cytopath/trajectory_estimation/
--rw-------   0 ubuntu    (1000) ubuntu    (1000)      126 2021-06-11 14:58:00.000000 cytopath-0.1.9/cytopath/trajectory_estimation/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21416 2022-11-27 23:36:54.000000 cytopath-0.1.9/cytopath/trajectory_estimation/cyto_path.py
--rw-------   0 ubuntu    (1000) ubuntu    (1000)     5539 2021-06-11 14:58:00.000000 cytopath-0.1.9/cytopath/trajectory_estimation/cytopath_merger.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17680 2022-11-27 23:36:54.000000 cytopath-0.1.9/cytopath/trajectory_estimation/sample_clustering.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4237 2022-11-27 23:36:54.000000 cytopath-0.1.9/cytopath/trajectory_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22853 2022-11-27 23:36:54.000000 cytopath-0.1.9/cytopath/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-27 23:39:35.105019 cytopath-0.1.9/cytopath.egg-info/
--rw-------   0 ubuntu    (1000) ubuntu    (1000)      751 2022-11-27 23:39:35.000000 cytopath-0.1.9/cytopath.egg-info/PKG-INFO
--rw-------   0 ubuntu    (1000) ubuntu    (1000)      693 2022-11-27 23:39:35.000000 cytopath-0.1.9/cytopath.egg-info/SOURCES.txt
--rw-------   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-27 23:39:35.000000 cytopath-0.1.9/cytopath.egg-info/dependency_links.txt
--rw-------   0 ubuntu    (1000) ubuntu    (1000)       98 2022-11-27 23:39:35.000000 cytopath-0.1.9/cytopath.egg-info/requires.txt
--rw-------   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-27 23:39:35.000000 cytopath-0.1.9/cytopath.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-11-27 23:39:35.193019 cytopath-0.1.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2022-11-27 23:36:54.000000 cytopath-0.1.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 00:37:17.682652 cytopath-0.2.0/
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)     1799 2021-06-11 14:57:59.000000 cytopath-0.2.0/.gitignore
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)     1520 2021-06-11 14:57:59.000000 cytopath-0.2.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-07-18 00:37:17.682652 cytopath-0.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2204 2023-07-18 00:33:37.000000 cytopath-0.2.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 00:37:17.682652 cytopath-0.2.0/cytopath/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-11-27 23:36:54.000000 cytopath-0.2.0/cytopath/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21003 2023-07-17 22:45:20.000000 cytopath-0.2.0/cytopath/markov_chain_sampler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-17 22:24:53.000000 cytopath-0.2.0/cytopath/plotting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 00:37:17.682652 cytopath-0.2.0/cytopath/plotting_functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2022-02-15 05:04:27.000000 cytopath-0.2.0/cytopath/plotting_functions/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-07-17 22:41:53.000000 cytopath-0.2.0/cytopath/plotting_functions/plot_alignment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6429 2022-03-26 21:22:07.000000 cytopath-0.2.0/cytopath/plotting_functions/plot_radial_heatmap.py
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)      718 2021-06-11 14:58:00.000000 cytopath-0.2.0/cytopath/plotting_functions/plot_sampling.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 00:37:17.682652 cytopath-0.2.0/cytopath/trajectory_estimation/
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)      126 2021-06-11 14:58:00.000000 cytopath-0.2.0/cytopath/trajectory_estimation/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21621 2023-07-15 16:15:39.000000 cytopath-0.2.0/cytopath/trajectory_estimation/cyto_path.py
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-07-14 16:26:40.000000 cytopath-0.2.0/cytopath/trajectory_estimation/cytopath_merger.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9649 2023-07-18 00:02:59.000000 cytopath-0.2.0/cytopath/trajectory_estimation/sample_clustering.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4172 2023-07-18 00:05:44.000000 cytopath-0.2.0/cytopath/trajectory_inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22853 2022-11-27 23:36:54.000000 cytopath-0.2.0/cytopath/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 00:37:17.682652 cytopath-0.2.0/cytopath.egg-info/
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)      701 2023-07-18 00:37:17.000000 cytopath-0.2.0/cytopath.egg-info/PKG-INFO
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)      693 2023-07-18 00:37:17.000000 cytopath-0.2.0/cytopath.egg-info/SOURCES.txt
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-18 00:37:17.000000 cytopath-0.2.0/cytopath.egg-info/dependency_links.txt
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)       85 2023-07-18 00:37:17.000000 cytopath-0.2.0/cytopath.egg-info/requires.txt
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-18 00:37:17.000000 cytopath-0.2.0/cytopath.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-18 00:37:17.682652 cytopath-0.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2023-07-18 00:19:04.000000 cytopath-0.2.0/setup.py
```

### Comparing `cytopath-0.1.9/.gitignore` & `cytopath-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cytopath-0.1.9/LICENSE` & `cytopath-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cytopath-0.1.9/PKG-INFO` & `cytopath-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cytopath
-Version: 0.1.9
+Version: 0.2.0
 Summary: Simulation based inference of differentiation trajectories from RNA velocity fields.
 Home-page: https://github.com/aron0093/cytopath
-Download-URL: https://github.com/aron0093/cytopath/archive/v_019.tar.gz
+Download-URL: https://github.com/aron0093/cytopath/archive/v_020.tar.gz
 Author: Revant Gupta
 Author-email: revant.gupta.93@gmail.com
 License: BSD 3-Clause License
 Keywords: Trajectory Inference,single-cell RNA sequencing,RNA velocity
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
```

### Comparing `cytopath-0.1.9/cytopath/markov_chain_sampler.py` & `cytopath-0.2.0/cytopath/markov_chain_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
         print('Max number ({}) of iterations reached.'.format(max_iter))
         convergence_check = max_iter
     
     state_history = state_history_max_iter[:convergence_check]
     return state_history, state_history_max_iter, convergence_check
 
 def sampling(data, auto_adjust=True, matrix_key = 'T_forward', cluster_key = 'louvain', max_steps=10, min_sim_ratio=0.6, rounds_limit=10, traj_number=50, sim_number=500,
-                end_point_probability=0.99, root_cell_probability=0.99, end_points=None, root_cells=None, end_clusters=None, root_clusters=None, min_clusters=3, tol=1e-3,
-                normalize=False, unique=True, num_cores=1, copy=False):
+             end_point_probability=0.99, root_cell_probability=0.99, end_points=None, root_cells=None, end_clusters=None, root_clusters=None, min_clusters=2, 
+             max_iter=200, tol=1e-3, normalize=False, unique=True, num_cores=1, copy=False):
     
     """Markov sampling of cell sequences starting from defined root cells to defined terminal regions based on a cell-cell transition probability matrix.
     Arguments
     ---------
     adata: :class:`~anndata.AnnData`
         Annotated data matrix with transition probabilities, end points and clustering.
     auto_adjust: `Boolean` (default: True)
@@ -119,16 +119,18 @@
         Numerical indices of the cells considered to be end points for manual annotation. Precendence over end_point_probability and end_clusters.
     root_cells: `list` (default: None)
         Numerical indices of the cells considered to be root states for manual annotation. Precendence over root_state_probability and root_clusters.
     end_clusters: `list` (default: None)
         Cluster IDs to be considered end points. Precendence over end_point_probability.
     root_clusters: `list` (default: None)
         Cluster IDs to be considered root states. Precendence over root_state_probability.
-    min_clusters: `integer` (default:3)
+    min_clusters: `integer` (default:2)
         Minium number of clusters covered by each simulation. (cluster_key)
+    max_iter: `integer` (default: 200)
+        Maximum simulation iterations to test to auto-select max_steps.
     tol: `float` (default:1e-3)
         Convergence criteria for Markov sampling.
     normalize: 'Boolean' (default: False)
         Toggle row sum normalization.
     unique: 'Boolean' (default:True)
         Only keep unique samples.
     num_cores: 'integer' (default:1)
@@ -231,15 +233,15 @@
     # Retrieve all end point cells
     if not end_points:
         if not end_clusters:
             try:
                 end_points = np.asarray(np.where(np.asarray(adata.obs["end_points"]) >= end_point_probability))[0]
                 #TODO
                 '''
-                 # Recluster end points if based on probability
+                # Recluster end points if based on probability
                 end_points_adata = adata[end_points]
                 scvelo.tl.louvain(end_points_adata)
                 adata.obs['updated_'+cluster_key] = adata.obs[cluster_key].astype(str).values
                 adata.obs.iloc[end_points, adata.obs.columns.get_loc('updated_'+cluster_key)] = 'End_'+ end_points_adata.obs['louvain'].astype(str).values
                 
                 del end_points_adata
                 cluster_key = 'updated_'+cluster_key
@@ -251,14 +253,17 @@
                 raise ValueError('End points must be provided in adata.obs["end_points"]. Run cytopath.terminal_states')
         else:
             end_points = np.asarray(np.where(np.asarray(adata.obs[cluster_key].isin(end_clusters))))[0]        
 
     adata.uns['run_info']['end_points'] = end_points
     end_point_clusters = adata.obs[cluster_key][end_points].astype(str).values
     end_clusters_ = np.unique(end_point_clusters)
+
+    if len(end_clusters_)==0:
+        raise ValueError('Terminal cluster set is empty.')
     
     # Adjust simulation parameters based on data
     if auto_adjust:
         print('Adjusting simulation parameters based on dataset properties. Set auto_adjust=False if this is unwanted.')
 
         # Initial number of simulations
         traj_number = math.ceil(np.log10(adata.shape[0])*traj_number) # Dataset size 
@@ -266,29 +271,28 @@
         sim_number = math.ceil(traj_number*len(end_clusters_)*np.log2(len(root_cells)+1)) # scale number of simulations by number of terminal regions and root cells
         print('Number of initial simulations (sim_number) set to {}'.format(sim_number))
 
         # Initial number of simulation steps
         max_steps = iterate_state_probability(adata, matrix_key=matrix_key, 
                                               init = (adata.obs['root_cells']/adata.obs['root_cells'].sum()).values, 
                                               stationary=(adata.obs['end_points']/adata.obs['end_points'].sum()).values, 
-                                              max_iter=200, tol=tol)[-1]
+                                              max_iter=max_iter, tol=tol)[-1]
         print('Number of initial simulation steps (max_steps) set to {}'.format(max_steps)) 
 
     # Initialize all empty lists
     glob_all_seq = []
     glob_prob_all_seq = []
     glob_cluster_seq_all = []
     sim_number_ = max(int(sim_number/len(root_cells)),1) # Number of simulations can't be less than 1
 
     # Define variables for conditional
     traj_num = [0]
     ratio_obtained = 0
 
     count = 0 # Iterate sampling runs
-    old_step_increment=0
     # Resample samples until the number of trajectories for each end point has been reached.
     while (min(traj_num) < traj_number): # or (ratio_obtained < 0.1)
 
         print()
         print("Sampling round: {}".format(count))
         count+=1
 
@@ -350,15 +354,15 @@
             traj_num.append(len(all_seq_cluster))
         
         # Increase sampling steps till min_sim_ratio of simulations end at a end point
         ratio_obtained = np.round(sum(traj_num)/(sim_number_*len(root_cells)), 6)
         ratio_min = np.round(min(traj_num)/traj_number, 4)
 
         if count==rounds_limit+1:
-            if (min(traj_num) < min_sim_ratio*traj_number) or (ratio_obtained < 0.1):
+            if (min(traj_num) < min_sim_ratio*traj_number): #or (ratio_obtained < 0.1):
 
                 print('{} % of required simulations obtained for lagging end point {}.'.format(np.round(ratio_min*100, 2),
                                                                                                             end_clusters_[np.argmin(traj_num)]))
                 print('{} % of simulations reached atleast one endpoint after {} rounds.'.format(np.round(ratio_obtained*100, 4), 
                                                                                                     rounds_limit))
                 raise ValueError('Sampling failed. Try lowering min_sim_ratio or increase rounds_limit.')
```

### Comparing `cytopath-0.1.9/cytopath/plotting.py` & `cytopath-0.2.0/cytopath/plotting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .plotting_functions.plot_alignment import pl_cytopath_alignment
 from .plotting_functions.plot_sampling import pl_cytopath_sampling
 from .plotting_functions.plot_radial_heatmap import radial_heatmap
 
-def plot_trajectories(data, directory='', basis='', size=10, figsize=(12,3), save_type='svg', smoothing=False):
-    pl_cytopath_alignment(data, folder=directory, basis=basis, size=size, figsize=figsize, smoothing=smoothing, save_type=save_type)
+def plot_trajectories(data, basis='', smoothing=False, figsize=(15,4), size=3, 
+                      show=True, save=False, save_type='png', directory=''):
+    pl_cytopath_alignment(data, basis=basis, smoothing=smoothing, figsize=figsize, size=size, 
+                          show=show, save=save, save_type=save_type, folder=directory,)
 
 def plot_sampling(data, directory='', basis=''):
     pl_cytopath_sampling(data, folder=directory, basis=basis)
```

### Comparing `cytopath-0.1.9/cytopath/plotting_functions/plot_alignment.py` & `cytopath-0.2.0/cytopath/plotting_functions/plot_alignment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 import numpy as np
+
 from scipy import spatial
+
 import matplotlib.pyplot as plt
       
-def pl_cytopath_alignment(adata, basis="umap", folder="", figsize=(12,3), save_type='svg', size = 10, smoothing=False):
+def fft_smoothing(coords):
+
+    #TODO: More relevant procedure required
+    signal = coords[:,0] + 1j*coords[:,1]
+
+    # FFT and frequencies
+    fft = np.fft.fft(signal)
+    freq = np.fft.fftfreq(signal.shape[-1])
+
+    # filter
+    cutoff = 0.1
+    fft[np.abs(freq) > cutoff] = 0
+
+    # IFFT
+    signal_filt = np.fft.ifft(fft)
+
+    coords[:,0] = signal_filt.real
+    coords[:,1] = signal_filt.imag
+
+    return coords
+
+def pl_cytopath_alignment(adata, basis="umap", smoothing=False, figsize=(15,4), size = 3, 
+                          show=True, save=False,save_type='png', folder=""):
     
     map_state = adata.obsm['X_'+basis]
     av_allign_score_glob=[]
     std_allign_score_glob=[]
     
     step_time = adata.uns['trajectories']['step_time']
     fate_prob = adata.uns['trajectories']['cell_fate_probability']
 
     sequence=0
-   
+
+    # TODO: Separate per step average alignment score calculation from plotting
     for end_point_cluster in adata.uns['run_info']["end_point_clusters"]:
-        trajectories = adata.uns['trajectories']["cells_along_trajectories_each_step"][np.where(adata.uns['trajectories']["cells_along_trajectories_each_step"]["End point"]==end_point_cluster)[0]]
+        trajectories = adata.uns['trajectories']["cells_along_trajectories_each_step"]\
+                       [np.where(adata.uns['trajectories']["cells_along_trajectories_each_step"]["End point"]==end_point_cluster)[0]]
         for i in range(adata.uns['run_info']['trajectory_count'][end_point_cluster]):
 
             av_trajectories=trajectories[np.where(trajectories["Trajectory"]==i)[0]]
             av_allign_score=np.zeros((len(np.unique(av_trajectories["Step"]))))
             std_allign_score=np.zeros((len(np.unique(av_trajectories["Step"]))))
             for l in range(len(np.unique(av_trajectories["Step"]))):
                 av_allign_score[l]=np.average((av_trajectories[np.where(av_trajectories["Step"]==l)[0]]["Allignment Score"]))
                 std_allign_score[l]=np.std((av_trajectories[np.where(av_trajectories["Step"]==l)[0]]["Allignment Score"]))
             
-            # TODO: Separate per step average alignment score calculation from plotting
-
             # Plotting
             path = folder+"_end_point_"+end_point_cluster+"_cytopath_"+str(i)+\
                  "occurance"+str(adata.uns['run_info']["trajectories_sample_counts"][end_point_cluster][i])+"."+save_type
 
             fig, (ax1, ax2, ax3) = plt.subplots(nrows=1, ncols=3, figsize=figsize) 
             ax1.plot(range(len(np.unique(av_trajectories["Step"]))), av_allign_score, color='black')
             ax1.fill_between(range(len(np.unique(av_trajectories["Step"]))), 
                              av_allign_score+std_allign_score, av_allign_score-std_allign_score, facecolor='grey', alpha=0.6)
             ax1.set_ylabel('Mean/std. of alignment scores per step')
             ax1.set_xlabel('Steps')
             
             # Plot step size for aligned cells
-            sc_step = ax2.scatter(map_state[:,0], map_state[:,1], alpha=0.6, s=size, color="grey")
-            sc_step = ax2.scatter(map_state[:,0], map_state[:,1], alpha=0.9, s=size, c=step_time[sequence,:], cmap='YlGnBu')
+            sc_step = ax2.scatter(map_state[:,0], map_state[:,1], alpha=0.6, s=size, color="whitesmoke")
+            sc_step = ax2.scatter(map_state[:,0], map_state[:,1], alpha=0.9, s=size, 
+                                  vmin=0, vmax=np.nanmax(step_time), c=step_time[sequence,:], cmap='YlGnBu')
             fig.colorbar(sc_step, ax=ax2, label='Step time')
 
             ax2.set_ylabel(basis.upper()+' 2')
             ax2.set_xlabel(basis.upper()+' 1')
 
+            ax2.set_title('End point: {}-{} Support: {}/{}'.format(end_point_cluster, i, 
+                                                                adata.uns['run_info']['trajectories_sample_counts'][end_point_cluster][i],
+                                                                int(adata.uns['samples']['cell_sequences'].shape[0]/\
+                                                                adata.uns['run_info']['end_point_clusters'].shape[0])))
+
             # Plot alignment score
-            sc_score = ax3.scatter(map_state[:,0], map_state[:,1], alpha=0.6, s=size, color="grey")
-            sc_score = ax3.scatter(map_state[:,0], map_state[:,1], alpha=0.9, s=size, c=fate_prob[sequence,:], cmap='YlGnBu')
+            sc_score = ax3.scatter(map_state[:,0], map_state[:,1], alpha=0.6, s=size, color="whitesmoke")
+            sc_score = ax3.scatter(map_state[:,0], map_state[:,1], alpha=0.9, s=size, 
+                                   vmin=0, vmax=1, c=fate_prob[sequence,:], cmap='Reds')
             fig.colorbar(sc_score, ax=ax3, label='Cell fate probability')
 
             ax3.set_ylabel(basis.upper()+' 2')
             ax3.set_xlabel(basis.upper()+' 1')
 
             # Plot trajectory
             if basis in adata.uns['run_info']['trajectory_basis']:
-
                 coords = np.array(adata.uns['trajectories']['trajectories_coordinates'][end_point_cluster]['trajectory_'+str(i)+'_coordinates'])
 
-                if smoothing == True:
-                    #TODO: More relevant procedure required
-                    signal = coords[:,0] + 1j*coords[:,1]
-
-                    # FFT and frequencies
-                    fft = np.fft.fft(signal)
-                    freq = np.fft.fftfreq(signal.shape[-1])
-
-                    # filter
-                    cutoff = 0.1
-                    fft[np.abs(freq) > cutoff] = 0
-
-                    # IFFT
-                    signal_filt = np.fft.ifft(fft)
-
-                    coords[:,0] = signal_filt.real
-                    coords[:,1] = signal_filt.imag
-
-                ax2.plot(coords[:, 0], coords[:, 1], color='black')
-                ax3.plot(coords[:, 0], coords[:, 1], color='black')
-
             elif ('pca' in adata.uns['run_info']['trajectory_basis']) and (basis != 'pca'):
-
                 coords_ = np.array(adata.uns['trajectories']['trajectories_coordinates'][end_point_cluster]['trajectory_'+str(i)+'_coordinates'])
 
                 cell_sequences=[]
                 for j in range(len(coords_)):
                     cell_sequences.append(spatial.KDTree(adata.obsm['X_pca']).query(coords_[j])[1])
                 
                 coords = map_state[cell_sequences]
 
-                if smoothing == True:
-                    #TODO: More relevant procedure required
-                    signal = coords[:,0] + 1j*coords[:,1]
-
-                    # FFT and frequencies
-                    fft = np.fft.fft(signal)
-                    freq = np.fft.fftfreq(signal.shape[-1])
-
-                    # filter
-                    cutoff = 0.1
-                    fft[np.abs(freq) > cutoff] = 0
-
-                    # IFFT
-                    signal_filt = np.fft.ifft(fft)
-
-                    coords[:,0] = signal_filt.real
-                    coords[:,1] = signal_filt.imag
+            if smoothing == True:
+                coords = fft_smoothing(coords)
+                
+            ax2.plot(coords[:, 0], coords[:, 1], color='black')
+            ax3.plot(coords[:, 0], coords[:, 1], color='black')
 
-                ax2.plot(coords[:, 0], coords[:, 1], color='black')
-                ax3.plot(coords[:, 0], coords[:, 1], color='black')
+            plt.tight_layout()
 
-            fig.savefig(path, bbox_inches='tight', dpi=300)
+            if save:
+                fig.savefig(path, bbox_inches='tight', dpi=300)
+            if show:
+                plt.show()
             # End plotting
 
             sequence+=1
 
             av_allign_score_glob.append(av_allign_score)                                
-            std_allign_score_glob.append(std_allign_score)
+            std_allign_score_glob.append(std_allign_score)
+
+
```

### Comparing `cytopath-0.1.9/cytopath/plotting_functions/plot_radial_heatmap.py` & `cytopath-0.2.0/cytopath/plotting_functions/plot_radial_heatmap.py`

 * *Files identical despite different names*

### Comparing `cytopath-0.1.9/cytopath/plotting_functions/plot_sampling.py` & `cytopath-0.2.0/cytopath/plotting_functions/plot_sampling.py`

 * *Files identical despite different names*

### Comparing `cytopath-0.1.9/cytopath/trajectory_estimation/cyto_path.py` & `cytopath-0.2.0/cytopath/trajectory_estimation/cyto_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 import pandas as pd
 from scipy import spatial
 
 from scvelo.preprocessing.neighbors import get_connectivities
 
 from joblib import Parallel, delayed
-
 from tqdm.auto import tqdm
 
 from ..utils import cosine_similarity
 
-def surrogate_cell_neighborhood_finder(adata, end_point, map_state, fill_cluster=True, n_neighbors=30, cluster_freq=0.1, mode='distances', recurse_neighbors=True):
+def surrogate_cell_neighborhood_finder(adata, end_point, map_state, fill_cluster=True, n_neighbors=30, 
+                                       cluster_freq=0.05, mode='distances', recurse_neighbors=True):
     """Finds surrogate cell and uses the scvelo neighborhood graph to finds its recursive neighbors. 
        Applicable when mean is used to compute trajectory coordinates. Default is median.
     
     Arguments
     ---------
     adata: :class:`~anndata.AnnData`
         Annotated data matrix with end points.
@@ -47,17 +47,18 @@
         for j in range(len(final_sequences[i])):
             local_neighs.append(neighborhood[final_sequences[i][j]].nonzero()[1])
             
             if fill_cluster:
                 raise NotImplementedError('Fill cluster not implemented.')
 
         neighborhood_sequence.append(local_neighs)
-    return neighborhood_sequence, cell_sequences
+    return neighborhood_sequence
 
-def cell_neighborhood_finder(adata, map_state, end_point, neighbors_basis='pca', fill_cluster=True, n_neighbors_cluster='auto', cluster_freq = 0.3, n_neighbors='auto'):
+def cell_neighborhood_finder(adata, map_state, end_point, neighbors_basis='pca', fill_cluster=True, 
+                             n_neighbors_cluster='auto', cluster_freq = 0.05, n_neighbors='auto'):
     """Finds the nearest neighbors along the average trajectory.
     
     Arguments
     ---------
     adata: :class:`~anndata.AnnData`
         Annotated data matrix with end points.
     end_point: `string`
@@ -76,20 +77,20 @@
     Returns list of arrays containing the sequence of neighborhoods along the trajectory.
     """
     # Cell neighborhood of trajectory
     final_cluster=adata.uns['trajectories']["trajectories_coordinates"][end_point]
 
     # Cluster assignment
     if n_neighbors_cluster=='auto':
-        min_cluster_size = adata.obs[adata.uns['run_info']['cluster_key']].value_counts().min()
-        n_neighbors_cluster = min_cluster_size - min_cluster_size*cluster_freq
+        # mean_cluster_size = adata.obs[adata.uns['run_info']['cluster_key']].value_counts().mean()
+        # n_neighbors_cluster = int(np.ceil(mean_cluster_size*cluster_freq))
+        # TODO: Adaptive width search 
+        n_neighbors_cluster = int(adata.shape[0]/100)
         if n_neighbors_cluster < 10:
             n_neighbors_cluster = 10
-        if adata.shape[0]/200 > 10:
-            n_neighbors_cluster = adata.shape[0]/200
             
         adata.uns['run_info']['n_neighbors_cluster'] = n_neighbors_cluster
     
     # Find clusters composing the trajectory
     compositional_clusters = []
     for i in tqdm(range(len(final_cluster))):
         final_cluster_sequence=final_cluster['trajectory_{}_coordinates'.format(i)]
@@ -252,66 +253,71 @@
     """
     final_cluster = adata.uns['trajectories']["trajectories_coordinates"][end_point]
     directional_neighborhood_sequence = neighborhood_sequence
     if cut_off is not None:
         for i in tqdm(range(len(final_cluster))):
             cutoff_score = cut_off
             for j in range(0, len(neighborhood_sequence[i])):
-                 directional_neighborhood_sequence[i][j] = np.delete(directional_neighborhood_sequence[i][j], np.where(all_scores[i][j]<=cutoff_score))
+                 directional_neighborhood_sequence[i][j] = np.delete(directional_neighborhood_sequence[i][j], 
+                                                                     np.where(all_scores[i][j]<=cutoff_score))
                  all_scores[i][j] = np.delete(all_scores[i][j], np.where(all_scores[i][j]<=cutoff_score))
     return directional_neighborhood_sequence, all_scores
     
-def cytopath(adata, basis="umap", neighbors_basis='pca', surrogate_cell=False, fill_cluster=True, n_neighbors_cluster='auto', cluster_freq=0.3, n_neighbors='auto', cut_off=0.0, num_cores=1):
+def cytopath(adata, basis="umap", neighbors_basis='pca', surrogate_cell=False, fill_cluster=True, 
+             n_neighbors_cluster='auto', cluster_freq=0.05, n_neighbors='auto', cut_off=0.0, num_cores=1):
     """Calculates the average time step for each cell.
 
     Arguments
     ---------
     adata: :class:`~anndata.AnnData`
         Annotated data matrix with end points.
     basis: `str/list` (default: umap)
-        The space in which the neighboring cells should be searched. If None imputed expression is used. If list, imputed expression from supplied genes is used.
+        The space in which the neighboring cells should be searched. If None imputed expression is used. 
+        If list, imputed expression from supplied genes is used.
     surrogate_cell: `Boolean` (default:False)
         Whether or not a surrogate cell should be used for the neighborhood search
     fill_cluster: `Boolean` (default:True)
         Enforce only cells in compostional clusters are assigned score.
     n_neighbors_cluster: `integer` (Default:30)
         Number of cells to consider for determining compositional clusters
-    cluster_freq: `float` (Default: 0.3)
+    cluster_freq: `float` (Default: 0.05)
         Frequency of cell cluster cells per step to consider as compositonal cluster
     n_neighbors:  `str/int/float` (default:'auto')
         Number of neighbors to searched along the average trajectory.
     cut_off: `float` (default:0.0)
         Cuttof for the directionality score along the average trajectory for the cells.
     Returns
     -------
     Returns adata.uns['trajectories']["cells_along_trajectories"]: List of arrays, which denote the average step for cell.
     adata.uns['trajectories']["cells_along_trajectories_each_step"]: List of arrays containing the cell indexes for each step
     """
     cell_score=[]
-    step_ordering_trajectory=[]
     cells_trajectory=[]
     
     adata.uns['trajectories']['compositional_clusters'] = {}
     
     if basis is None:
         map_state = adata.layers['Ms']
     elif type(basis) == list:
         map_state = adata[:, basis].layers['Ms']
     else:
         map_state = adata.obsm['X_'+basis]
 
     for end_point_cluster in adata.uns['trajectories']["trajectories_coordinates"].keys():
         if surrogate_cell:
             print('Anchoring trajectories for end point {} to cells in dataset and computing neighborhoods'.format(end_point_cluster))
-            neighborhood_sequence, cell_sequences = surrogate_cell_neighborhood_finder(adata, end_point_cluster, map_state, mode='distances', fill_cluster=fill_cluster, n_neighbors_cluster=n_neighbors_cluster,
-                                                                                    cluster_freq=cluster_freq, n_neighbors=n_neighbors, recurse_neighbors=True)
+            neighborhood_sequence = surrogate_cell_neighborhood_finder(adata, end_point_cluster, map_state, mode='distances', 
+                                                                       fill_cluster=fill_cluster, n_neighbors_cluster=n_neighbors_cluster, 
+                                                                       cluster_freq=cluster_freq, n_neighbors=n_neighbors, 
+                                                                       recurse_neighbors=True)
         else:
             print('Computing neighborhoods of trajectories for end point {} at each step'.format(end_point_cluster))
-            neighborhood_sequence = cell_neighborhood_finder(adata, map_state, end_point=end_point_cluster, neighbors_basis=neighbors_basis, fill_cluster=fill_cluster, n_neighbors_cluster=n_neighbors_cluster, cluster_freq=cluster_freq,
-                                                             n_neighbors=n_neighbors)
+            neighborhood_sequence = cell_neighborhood_finder(adata, map_state, end_point=end_point_cluster, neighbors_basis=neighbors_basis, 
+                                                             fill_cluster=fill_cluster, n_neighbors_cluster=n_neighbors_cluster, 
+                                                             cluster_freq=cluster_freq, n_neighbors=n_neighbors)
 
         print('Computing alignment score of cells in trajectory neighborhood w.r.t. trajectories for end point  {}'.format(end_point_cluster))
         all_scores=directionality_score(adata, neighborhood_sequence=neighborhood_sequence, end_point=end_point_cluster, map_state=map_state, num_cores=num_cores)
 
         print('Removing cells below cutoff threshold from trajectories for end point  {} (i.e. cells neighborhood)'.format(end_point_cluster))
         directional_neighborhood_sequence, all_scores = cutoff_score(adata, end_point=end_point_cluster, neighborhood_sequence=neighborhood_sequence, 
                                                                   all_scores=all_scores, cut_off=cut_off)
@@ -377,21 +383,21 @@
         step_ = cytopath_data_.groupby(['End point', 'Trajectory', 'Cell'])['Step'].sum()
 
         cytopath_data_ = cytopath_data_.groupby(['End point', 'Trajectory', 'Cell']).mean()
         cytopath_data_['Step'] = step_
 
     adata.uns['trajectories']['cells_along_trajectories'] = cytopath_data_.to_records()
     
-    adata.uns['trajectories']['step_time'] = pd.DataFrame(index=np.arange(adata.shape[0])).merge(cytopath_data_.reset_index().pivot(index='Cell', columns=['End point', 'Trajectory'], 
-                                                                                                                                    values='Step'), 
-                                                                                                 left_index=True, right_index=True, how='left').T.values
-    
-    
-    cell_fate_prob = pd.DataFrame(index=np.arange(adata.shape[0])).merge(cytopath_data_.reset_index().pivot(index='Cell', columns=['End point', 'Trajectory'], values='Allignment Score'), 
-                                                                         left_index=True, right_index=True, how='left')
+    step_time_df = cytopath_data_.reset_index().pivot(index='Cell', columns=['End point', 'Trajectory'], values='Step')
+    step_time_df.columns = step_time_df.columns.to_flat_index()
+    adata.uns['trajectories']['step_time'] = pd.DataFrame(index=np.arange(adata.shape[0])).merge(step_time_df, left_index=True, right_index=True, how='left').T.values
+    
+    cell_fate_prob_df = cytopath_data_.reset_index().pivot(index='Cell', columns=['End point', 'Trajectory'], values='Allignment Score')
+    cell_fate_prob_df.columns = cell_fate_prob_df.columns.to_flat_index()
+    cell_fate_prob = pd.DataFrame(index=np.arange(adata.shape[0])).merge(cell_fate_prob_df, left_index=True, right_index=True, how='left')
     cell_fate_prob = cell_fate_prob.fillna(0).div(cell_fate_prob.sum(axis=1), axis=0)    
     adata.uns['trajectories']['cell_fate_probability'] = cell_fate_prob.T.values
```

### Comparing `cytopath-0.1.9/cytopath/trajectory_estimation/cytopath_merger.py` & `cytopath-0.2.0/cytopath/trajectory_estimation/cytopath_merger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import pandas as pd
 from tqdm import tqdm
 from joblib import Parallel, delayed
 
 def cytopath_merger(adata, overlap=0.5, num_cores=1):
     """
     Arguments
     ---------
```

### Comparing `cytopath-0.1.9/cytopath/trajectory_inference.py` & `cytopath-0.2.0/cytopath/trajectory_inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 from .trajectory_estimation.sample_clustering import sample_clustering
 from .trajectory_estimation.cyto_path import cytopath, estimate_cell_data
 from .trajectory_estimation.cytopath_merger import cytopath_merger
 
-def trajectories(data, smoothing=False, alignment_cutoff=0.0, basis='umap', neighbors_basis='pca', fill_cluster=True, n_neighbors_cluster='auto', cluster_freq=0.15,
-                 groupby='mean', weighted=True, surrogate_cell=False, n_neighbors_alignment='auto', cluster_num=None, method = 'kmeans', distance='euclidean', num_cores=1, copy=False):
+def trajectories(data, alignment_cutoff=0.0, basis='umap', neighbors_basis='pca', fill_cluster=True, n_neighbors_cluster='auto', 
+                 cluster_freq=0.05, groupby='mean', weighted=True, surrogate_cell=False, n_neighbors_alignment='auto', cluster_num=None, 
+                 support=0.25, distance='euclidean', num_cores=1, copy=False):
 
     """Trajectory inference using simulations on the transition proabability matrix.
     
     Arguments
     ---------
     adata: :class:`~anndata.AnnData`
         Annotated data matrix with end points.
-    smoothing: Boolean (default:False)
-        Whether or not to smooth over the trajectories.
     alignment_cutoff: float (default:0.0)
         Minimum alignment score to consider a cell-step alignment valid
     basis: str/list (default: umap)
         The space in which the neighboring cells should be searched. If None imputed expression is used. If list, imputed expression from supplied genes is used.
     neighbors_basis: str (default: pca)
         The space used to find neighboring cells of trajectory steps.
     fill_cluster: `Boolean` (default:True)
         Enforce only cells in compostional clusters are assigned score.
     n_neighbors_cluster: `integer` (Default:30)
         Number of cells to consider for determining compositional clusters
-    cluster_freq: `float` (Default: 0.15)
+    cluster_freq: `float` (Default: 0.05)
         Frequency of cell cluster cells per step to consider as compositonal cluster
     groupby:  `str` (default: mean)
         One of max, min, median or mean. Grouping method for determing alignment score per cell per trajectory
     weighted: `Boolean` (default:False)
         If groupby is mean, reports mean pseduotime weighted by alignment score if true.
     surrogate_cell: `Boolean` (default:False)
         Whether or not a surrogate cell should be used for the neighborhood search
     n_neighbors_alignment:  `str/int/float` (default:'auto')
         Number of neighbors to searched along the average trajectory.
     cluster_num:  list (default:None)
         Number of trajectories (clusters) to be expected for each terminal region.
-    method: str (default:'kmeans'):
-        Which clustering method to use.
+    support: float(default:0.25)
+        Minimum ratio of samples that must support a trajectory
     distance: str (default:'cosine'):
         Which distabce metric to use (see py-hausdorff for details)
     num_cores: 'integer' (default:1)
         Number of cpu cores to use.
     copy: 'Boolean' (default: False)
         Create a copy of the anndata object or work inplace.
     Returns
@@ -53,19 +52,20 @@
     """
 
     adata = data.copy() if copy else data
     
     if 'X_pca' not in adata.obsm.keys(): raise ValueError('Compute PCA using cytopath.scvelo.pp.pca')
 
     # Clustering of cell sequences to obtain trajectories
-    sample_clustering(adata, basis=basis, smoothing=smoothing, 
-                          cluster_num=cluster_num, method=method, distance=distance)
+    sample_clustering(adata, basis=basis, cluster_num=cluster_num, 
+                      support=support, distance=distance, num_cores=num_cores)
 
     # Align cells along trajectories
-    cytopath(adata, basis=basis, neighbors_basis=neighbors_basis, surrogate_cell=surrogate_cell, fill_cluster=fill_cluster, cluster_freq=cluster_freq, n_neighbors_cluster=n_neighbors_cluster,
+    cytopath(adata, basis=basis, neighbors_basis=neighbors_basis, surrogate_cell=surrogate_cell, fill_cluster=fill_cluster, 
+             cluster_freq=cluster_freq, n_neighbors_cluster=n_neighbors_cluster,
              n_neighbors=n_neighbors_alignment, cut_off=alignment_cutoff, num_cores=num_cores)
     
     # Estimate pseudotime, cell fate prob and alignment score at cell level
     estimate_cell_data(adata, groupby=groupby, weighted=weighted)
 
     return adata if copy else None
```

### Comparing `cytopath-0.1.9/cytopath/utils.py` & `cytopath-0.2.0/cytopath/utils.py`

 * *Files identical despite different names*

### Comparing `cytopath-0.1.9/cytopath.egg-info/PKG-INFO` & `cytopath-0.2.0/cytopath.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cytopath
-Version: 0.1.9
+Version: 0.2.0
 Summary: Simulation based inference of differentiation trajectories from RNA velocity fields.
 Home-page: https://github.com/aron0093/cytopath
-Download-URL: https://github.com/aron0093/cytopath/archive/v_019.tar.gz
+Download-URL: https://github.com/aron0093/cytopath/archive/v_020.tar.gz
 Author: Revant Gupta
 Author-email: revant.gupta.93@gmail.com
 License: BSD 3-Clause License
 Keywords: Trajectory Inference,single-cell RNA sequencing,RNA velocity
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
```

### Comparing `cytopath-0.1.9/cytopath.egg-info/SOURCES.txt` & `cytopath-0.2.0/cytopath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cytopath-0.1.9/setup.py` & `cytopath-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
   name='cytopath',
-  version='0.1.9',
+  version='0.2.0',
   description='Simulation based inference of differentiation trajectories from RNA velocity fields.',
   license='BSD 3-Clause License',
   packages=find_packages(),
   author = 'Revant Gupta',
   author_email = 'revant.gupta.93@gmail.com',
   url = 'https://github.com/aron0093/cytopath',
-  download_url = 'https://github.com/aron0093/cytopath/archive/v_019.tar.gz',
+  download_url = 'https://github.com/aron0093/cytopath/archive/v_020.tar.gz',
   keywords = ['Trajectory Inference', 'single-cell RNA sequencing', 'RNA velocity'],
   install_requires=[
-          'numpy>=1.20.0',
-          'scipy',
-          'anndata',
           'scvelo>=0.1.25',
+          'numpy==1.23.5',
           'joblib',
           'fastdtw',
           'hausdorff',
+          'scikit-learn>=1.3.0',
           'tqdm',
-	  'networkit',
-	  'tabulate',
-	  'numba'
+	        'numba'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: BSD License',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
   ])
```

