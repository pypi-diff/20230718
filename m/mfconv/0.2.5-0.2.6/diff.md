# Comparing `tmp/mfconv-0.2.5.tar.gz` & `tmp/mfconv-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfconv-0.2.5.tar", last modified: Thu Jun  8 21:19:59 2023, max compression
+gzip compressed data, was "mfconv-0.2.6.tar", last modified: Tue Jul 18 16:44:06 2023, max compression
```

## Comparing `mfconv-0.2.5.tar` & `mfconv-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 21:19:59.880508 mfconv-0.2.5/
--rw-rw-rw-   0        0        0     1080 2023-04-21 17:04:38.000000 mfconv-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1092 2023-06-08 21:19:59.880508 mfconv-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-04-21 17:04:38.000000 mfconv-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 21:19:59.864879 mfconv-0.2.5/mfconv/
--rw-rw-rw-   0        0        0       27 2023-06-08 20:50:08.000000 mfconv-0.2.5/mfconv/__init__.py
--rw-rw-rw-   0        0        0     7243 2023-06-07 21:33:38.000000 mfconv-0.2.5/mfconv/plotter.py
-drwxrwxrwx   0        0        0        0 2023-06-08 21:19:59.880508 mfconv-0.2.5/mfconv.egg-info/
--rw-rw-rw-   0        0        0     1092 2023-06-08 21:19:59.000000 mfconv-0.2.5/mfconv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-08 21:19:59.000000 mfconv-0.2.5/mfconv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 21:19:59.000000 mfconv-0.2.5/mfconv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-08 21:19:59.000000 mfconv-0.2.5/mfconv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-21 17:04:38.000000 mfconv-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 21:19:59.880508 mfconv-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1539 2023-06-08 21:01:20.000000 mfconv-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:44:06.810377 mfconv-0.2.6/
+-rw-rw-rw-   0        0        0     1080 2023-04-21 17:04:38.000000 mfconv-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1092 2023-07-18 16:44:06.810377 mfconv-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-04-21 17:04:38.000000 mfconv-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 16:44:06.810377 mfconv-0.2.6/mfconv/
+-rw-rw-rw-   0        0        0       27 2023-06-08 20:50:08.000000 mfconv-0.2.6/mfconv/__init__.py
+-rw-rw-rw-   0        0        0     7590 2023-07-17 16:14:51.000000 mfconv-0.2.6/mfconv/plotter.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:44:06.810377 mfconv-0.2.6/mfconv.egg-info/
+-rw-rw-rw-   0        0        0     1092 2023-07-18 16:44:06.000000 mfconv-0.2.6/mfconv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-18 16:44:06.000000 mfconv-0.2.6/mfconv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 16:44:06.000000 mfconv-0.2.6/mfconv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 16:44:06.000000 mfconv-0.2.6/mfconv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:04:38.000000 mfconv-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 16:44:06.810377 mfconv-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1539 2023-07-18 16:43:16.000000 mfconv-0.2.6/setup.py
```

### Comparing `mfconv-0.2.5/LICENSE.txt` & `mfconv-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mfconv-0.2.5/PKG-INFO` & `mfconv-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfconv
-Version: 0.2.5
+Version: 0.2.6
 Summary: a python package to plot modflow convergence while you run a model
 Home-page: https://github.com/gmezacuadra/mfconv
 Author: Gustavo Meza-Cuadra
 Author-email: gmeza-cuadra@flosolutions.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `mfconv-0.2.5/mfconv/plotter.py` & `mfconv-0.2.6/mfconv/plotter.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,23 @@
      
 MF_VERSION_LINE_MATCH = {
         'mf6': (3, 2, 4),
         'mf-usg': (2, 1, 3),
         'mf-surfact': 'TODO'
     }
 
-def get_convergence_data(mf_version, lst_file_name, mode):
+def get_convergence_data(mf_version, file_dir, lst_file_name, worker_folder_name, mode):
     """
     Parses a MODFLOW list file to return convergence data
 
     Args:
         mf_version (str): MODFLOW version (default: 'mf6)
-        lst_file (str): MODFLOW list file, including directory (default: 'mfsim.lst')
+        file_dir (str): Working directory for lst file or agent folders
+        lst_file_name (str): Name of the simulation list file (default: 'mfsim.lst')
+        worker_folder_name (str): Name of the worker folders (default: 'agent')
         mode (str): Specifies whether it is a solo or multiple worker run (default: 'solo')
 
     Return:
         max_heads (list): list of maximum heads at every outer iteration
         max_head_cells (list): a list of tuples containing the maximum head cells for each outer iteration
     """
 
@@ -67,30 +69,29 @@
                         max_heads_temp.append(max_head)
                         max_head_cells_temp.append(max_head_cell)
 
         ## Append back to the main lists
         max_heads.append(max_heads_temp)
         max_head_cells.append(max_head_cells_temp)
 
-    ## Check for list file
-    if os.path.exists(lst_file_name):
-        
-        ## If function in solo run mode, then runs through once
-        if mode == 'solo':
-            read_lst_file(lst_file_name)
-            return max_heads[0], max_head_cells[0]
+    # ## Check for list file
+    # if os.path.exists(lst_file_name):
         
-        ## If function in multi worker mode, then runs in a loop
-        elif mode == 'multi':
-            for dir in os.listdir(os.getcwd()):
-                if dir.startswith('agent') and dir[len('agent'):].isdigit():
-                    agent_folder = dir
-                    agent_folder_lst = os.path.join(agent_folder, lst_file_name)
-                    read_lst_file(agent_folder_lst)
-            return max_heads, max_head_cells
+    ## If function in solo run mode, then runs through once
+    if mode == 'solo':
+        read_lst_file(file_dir)
+        return max_heads[0], max_head_cells[0]
+    
+    ## If function in multi worker mode, then runs in a loop
+    elif mode == 'multi':
+        for dir in os.listdir(file_dir):
+            if dir.startswith(worker_folder_name) and dir[len(worker_folder_name):].isdigit():
+                agent_folder = os.path.join(dir, lst_file_name)
+                read_lst_file(agent_folder)
+        return max_heads, max_head_cells
     
 def plot_convergence_data(mf_version, ax, max_heads, max_head_cells):
     """
     Plots the data fetched from MODFLOW list file.
 
     Args:
         mf_version (str): MODFLOW version (default: 'mf6)
@@ -129,33 +130,37 @@
     Args:
         root_folder (str): Root folder path (default: current working directory)
         mf_version (str): MODFLOW version (default: 'mf6')
         lst_file_name (str): Name of the simulation list file (default: 'mfsim.lst')
         worker_folder_name (str): Name of the worker folders (default: 'agent')
         mode (str): Specifies whether it is a solo or multiple worker run (default: 'solo')
     """
-    print('Plotter is running in infinite loop so ctrl+c to exit when done')
-    
-    lst_file_dir = os.path.join(root_folder, lst_file_name)
+    print('\n***************************************************************')
+    print('Plotter is running in infinite loop, ctrl+c to exit when done')
+    print('***************************************************************\n')
     
     ## Infinte loop to run the data fetcher and plotter
     if mode == 'solo':
+    
+        lst_file_dir = os.path.join(root_folder, lst_file_name)
 
         ## Create figure and axes outside of infinite loop
         fig, ax = plt.subplots()
         
         ## Infinite loop of data fetching and plotting
         while True:
             max_heads, max_head_cells = get_convergence_data(mf_version, lst_file_dir, mode)
             plot_convergence_data(mf_version, ax, max_heads, max_head_cells)
             plt.pause(5)
             ax.clear()
 
     ## Infinte loop to run the data fetcher and plotter in looped fashion
     elif mode == 'multi':
+    
+        agents_folders_dir = root_folder
         
         # Iterate through folders looking for workers for plotting
         n_subplots = 0
         for dir in os.listdir(root_folder):
             if dir.startswith(worker_folder_name) and dir[len(worker_folder_name):].isdigit():
                 n_subplots += 1
         
@@ -164,13 +169,13 @@
         n_cols = int(np.ceil(n_subplots / n_rows))
 
         ## Create figure and axes outside of infinite loop
         fig, axes = plt.subplots(n_rows, n_cols, figsize=(10,10))
         
         ## Infinite loop of data fetching and plotting in multiplots
         while True:
-            max_heads, max_head_cells = get_convergence_data(mf_version, lst_file_dir, mode)
+            max_heads, max_head_cells = get_convergence_data(mf_version, agents_folders_dir, lst_file_name, worker_folder_name, mode)
             for ax, m_h, m_h_c in zip(axes.ravel(), max_heads, max_head_cells): ## TODO: Delete spare plots
                 plot_convergence_data(mf_version, ax, m_h, m_h_c)
             plt.pause(5)
             for ax in axes.ravel():
                 ax.clear()
```

### Comparing `mfconv-0.2.5/mfconv.egg-info/PKG-INFO` & `mfconv-0.2.6/mfconv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfconv
-Version: 0.2.5
+Version: 0.2.6
 Summary: a python package to plot modflow convergence while you run a model
 Home-page: https://github.com/gmezacuadra/mfconv
 Author: Gustavo Meza-Cuadra
 Author-email: gmeza-cuadra@flosolutions.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `mfconv-0.2.5/setup.py` & `mfconv-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Use the README.md content for the long description:
 with io.open("README.md", encoding="utf-8") as fileObj:
     long_description = fileObj.read()
 
 setup(
     name="mfconv",
-    version='0.2.5',
+    version='0.2.6',
     url="https://github.com/gmezacuadra/mfconv",
     author="Gustavo Meza-Cuadra",
     author_email="gmeza-cuadra@flosolutions.com",
     description=("""a python package to plot modflow convergence while you run a model"""),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

