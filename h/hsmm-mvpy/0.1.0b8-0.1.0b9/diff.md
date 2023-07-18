# Comparing `tmp/hsmm_mvpy-0.1.0b8.tar.gz` & `tmp/hsmm_mvpy-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b8.tar", last modified: Mon Jul 17 22:22:34 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b9.tar", last modified: Tue Jul 18 05:12:42 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b8.tar` & `hsmm_mvpy-0.1.0b9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b8/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    24957 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22591 2023-07-17 22:09:09.000000 hsmm_mvpy-0.1.0b8/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      848 2023-07-17 22:21:32.000000 hsmm_mvpy-0.1.0b8/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      229 2023-07-12 12:31:26.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     7130 2023-07-17 21:14:25.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/clusters.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    60568 2023-07-17 21:23:44.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     6659 2023-07-17 21:55:30.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/resample.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    14197 2023-07-17 21:23:49.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41218 2023-07-17 20:48:35.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    26816 2023-07-16 16:24:07.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    24957 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      395 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       86 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-18 05:12:42.364106 hsmm_mvpy-0.1.0b9/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b9/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    24970 2023-07-18 05:12:42.364106 hsmm_mvpy-0.1.0b9/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22591 2023-07-17 22:09:09.000000 hsmm_mvpy-0.1.0b9/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      861 2023-07-18 05:12:16.000000 hsmm_mvpy-0.1.0b9/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-07-18 05:12:42.364106 hsmm_mvpy-0.1.0b9/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-18 05:12:42.364106 hsmm_mvpy-0.1.0b9/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-18 05:12:42.364106 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      229 2023-07-12 12:31:26.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     7130 2023-07-17 21:14:25.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/clusters.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    60741 2023-07-18 05:10:44.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     6607 2023-07-18 04:58:34.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/resample.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    14208 2023-07-18 04:48:25.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41218 2023-07-17 20:48:35.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    26816 2023-07-16 16:24:07.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-18 05:12:42.364106 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    24970 2023-07-18 05:12:42.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      395 2023-07-18 05:12:42.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-07-18 05:12:42.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       86 2023-07-18 05:12:42.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-07-18 05:12:42.000000 hsmm_mvpy-0.1.0b9/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b8/LICENSE.md` & `hsmm_mvpy-0.1.0b9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b8/PKG-INFO` & `hsmm_mvpy-0.1.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -29,19 +29,19 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: Homepage, https://github.com/GWeindel/hmp
-Project-URL: Bug Tracker, https://github.com/GWeindel/hmp/issues
+Project-URL: Homepage, https://github.com/GWeindel/hsmm_mvpy
+Project-URL: Bug Tracker, https://github.com/GWeindel/hsmm_mvpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
```

### Comparing `hsmm_mvpy-0.1.0b8/README.md` & `hsmm_mvpy-0.1.0b9/README.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b8/pyproject.toml` & `hsmm_mvpy-0.1.0b9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta8"
+version = "0.1.0-beta9"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
 license = { file="LICENSE.md" }
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies=["mne >=1.0.0",
 "numpy",
 "xarray",
@@ -26,9 +26,9 @@
 "statsmodels",
 "seaborn",
 "scipy",
 "netcdf4",
 "more_itertools"]
 
 [project.urls]
-"Homepage" = "https://github.com/GWeindel/hmp"
-"Bug Tracker" = "https://github.com/GWeindel/hmp/issues"
+"Homepage" = "https://github.com/GWeindel/hsmm_mvpy"
+"Bug Tracker" = "https://github.com/GWeindel/hsmm_mvpy/issues"
```

### Comparing `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/clusters.py` & `hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/clusters.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from scipy.stats import gamma as sp_gamma
 import matplotlib.pyplot as plt
 from matplotlib.colors import LinearSegmentedColormap
 from hsmm_mvpy import utils
 from itertools import cycle
 
 
-try:
-    __IPYTHON__
-    from tqdm.notebook import tqdm
-except NameError:
-    import tqdm.tqdm
+# try:
+#     __IPYTHON__
+#     from tqdm.notebook import tqdm
+# except NameError:
+from tqdm import tqdm
 
 default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold', 'brown']
 
                    
 class hmp:
     
     def __init__(self, data, eeg_data=None, sfreq=None, offset=0, cpus=1, event_width=50, shape=2, estimate_magnitudes=True, estimate_parameters=True, template=None, location=None, distribution='gamma', em_method="mean"):
@@ -231,19 +231,19 @@
             elif len(np.shape(initial_m)) == 3:
                 magnitudes = initial_m
                 if len(np.shape(initial_p)) == 3:
                     parameters = initial_p
                 else:
                     parameters = np.tile(parameters, (len(magnitudes),1,1))
             if cpus>1: 
+                inputs = zip(itertools.repeat(n_events), magnitudes, parameters, itertools.repeat(maximization),
+                        itertools.repeat(magnitudes_to_fix),itertools.repeat(parameters_to_fix), itertools.repeat(max_iteration), itertools.repeat(tolerance), itertools.repeat(min_iteration))
                 with mp.Pool(processes=cpus) as pool:
-
-                    estimates = pool.starmap(self.EM, 
-                        zip(itertools.repeat(n_events), magnitudes, parameters, itertools.repeat(maximization),
-                        itertools.repeat(magnitudes_to_fix),itertools.repeat(parameters_to_fix), itertools.repeat(max_iteration), itertools.repeat(tolerance), itertools.repeat(min_iteration)))   
+                        estimates = list(tqdm(pool.imap(self._EM_star, inputs), total=len(magnitudes)))
+ 
             else:#avoids problems if called in an already parallel function
                 estimates = []
                 for pars, mags in zip(parameters, magnitudes):
                     estimates.append(self.EM(n_events, mags, pars, maximization,\
                     magnitudes_to_fix, parameters_to_fix, max_iteration, tolerance, min_iteration))
                 resetwarnings()
             lkhs_sp = [x[0] for x in estimates]
@@ -328,14 +328,17 @@
             xreventprobs = xreventprobs.transpose('iteration','trial_x_participant','samples','event')
         estimated = xr.merge((xrlikelihoods, xrparams, xrmags, xreventprobs, xrtraces))
 
         if verbose:
             print(f"Parameters estimated for {n_events} events model")
         return estimated
     
+    def _EM_star(self, args): #for tqdm usage
+        return self.EM(*args)
+    
     def EM(self, n_events, magnitudes, parameters,  maximization=True, magnitudes_to_fix=None, parameters_to_fix=None, max_iteration=1e3, tolerance=1e-4, min_iteration=1):  
         '''
         Expectation maximization function underlying fit
         ''' 
         if not isinstance(maximization, bool):#Backward compatibility with previous versions
             warn('Deprecated use of the threshold function, use maximization and tolerance arguments. Setting tolerance at 1 for compatibility')
             maximization = {1:True, 0:False}[maximization]
@@ -787,30 +790,32 @@
             grid = np.zeros((n_events, 1, self.n_dims))
         else: 
             grid = np.array([x for x in product(np.linspace(lower_bound,upper_bound,size), repeat=self.n_dims)])
 
         if verbose:
             print(f'Number of potential magnitudes: {len(grid)}') 
 
-        if n_samples is None or n_samples > len(grid):
+        if n_samples is None:
             n_samples = len(grid)
+        if n_samples > len(grid):
+            method='random'
         if decimate:
             n_samples = int(np.rint(len(grid) / decimate))
             
         if method is None and len(grid) != n_samples:
             grid = grid[::len(grid)//n_samples]
             n_samples = len(grid)
             if verbose:
                 print(f'Because of decimation {len(grid)} will be estimated.')
         gen_mags = np.zeros((n_events, n_samples, self.n_dims))
         for event in range(n_events):
             if method is None:
                 gen_mags[event,:,:] = grid
             elif method == "random":
-                gen_mags[event,:,:] = grid[np.random.choice(range(len(grid)), size=n_samples, replace=False)]
+                gen_mags[event,:,:] = grid[np.random.choice(range(len(grid)), size=n_samples, replace=True)]
         gen_mags = np.transpose(gen_mags, axes=(1,0,2))
         return gen_mags
     
     def _grid_search(self, n_stages, n_points=None, verbose=True, start_time=0, end_time=None, iter_limit=np.inf, step=1, offset=None, method='slide'):
         '''
         This function decomposes the mean RT into a grid with points. Ideal case is to have a grid with one sample = one search point but the number
         of possibilities badly scales with the length of the RT and the number of stages. Therefore the iter_limit is used to select an optimal number
```

### Comparing `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/resample.py` & `hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/resample.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         data_type = 'raw'
     else:
         data_type = 'transformed'
     if verbose:
         print(f'Bootstrapping {data_type} on {n_iterations} iterations')
     data_views, data, dim, order = _gen_dataset(data, dim, n_iterations)
     
-    #calculate estimates, returns lkhs, mags, times
     inputs = zip(itertools.repeat(data), itertools.repeat(dim), data_views, itertools.repeat(order), 
                 itertools.repeat(init), 
                 itertools.repeat(positions), itertools.repeat(init.sfreq), np.arange(n_iterations),
                 itertools.repeat(tolerance), itertools.repeat(decimate), itertools.repeat(summarize), itertools.repeat(verbose),
                 itertools.repeat(plots),itertools.repeat(cpus), itertools.repeat(trace), itertools.repeat(path))
     with mp.Pool(processes=cpus) as pool:
             boot = list(tqdm(pool.imap(_boot_star, inputs), total=n_iterations))
```

### Comparing `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/simulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         if subj_file in os.listdir(path) and not overwrite:
             subj_file = path+subj_file
             warn(f'{subj_file} exists no new simulation performed', UserWarning)
             files_subj.append(subj_file)
             files_subj.append(subj_file.split('.fif')[0]+'_generating_events.npy')
             files.append(files_subj)
         else:
-            subj_file = path+subj_file
+            subj_file = op.join(path, subj_file)
             print(f'Simulating {subj_file}')
             sources_subj = sources[subj]
             # stim_onset occurs every x samples.
             events = np.zeros((n_trials, 3), int)
             stim_onsets =  2000+max_trial_length * np.arange(n_trials)#2000 = offset of first stim
             events[:,0] = stim_onsets#last event 
             events[:,2] = 1#trigger 1 = stimulus 
@@ -272,15 +272,15 @@
     for source in range(len(name_sources)):
         sources.append([name_sources[source], frequency, amplitude, \
                           gamma(shape, scale=times[source])])
 
     file = 'dataset_tutorial2' #Name of the file to save
 
     #Simulating and recover information on electrode location and true time onset of the simulated events
-    files = simulate(sources, n_trials, cpus,file, overwrite=True, location=25, seed=seed)
+    files = simulate(sources, n_trials, cpus,file, overwrite=False, location=25, seed=seed)
     generating_events = np.load(files[1])
     number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
     random_source_times = np.reshape(np.diff(generating_events[:,0], prepend=0),(n_trials,number_of_sources+1))[:,1:]/(sfreq/resample_freq)#By-trial generated event times
 
     #Reading the necessary info to read the EEG data
     resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
     event_id = {'stimulus':1}
```

### Comparing `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/utils.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b9/src/hsmm_mvpy/visu.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b9/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -29,19 +29,19 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: Homepage, https://github.com/GWeindel/hmp
-Project-URL: Bug Tracker, https://github.com/GWeindel/hmp/issues
+Project-URL: Homepage, https://github.com/GWeindel/hsmm_mvpy
+Project-URL: Bug Tracker, https://github.com/GWeindel/hsmm_mvpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 HsMM MVpy
 ==========
 
 ![](plots/general_illustration.png)
```

