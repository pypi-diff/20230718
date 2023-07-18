# Comparing `tmp/hpfrec-0.2.5.post9.tar.gz` & `tmp/hpfrec-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpfrec-0.2.5.post9.tar", last modified: Sun Mar 19 16:47:14 2023, max compression
+gzip compressed data, was "hpfrec-0.2.6.tar", last modified: Mon Jul  3 18:27:48 2023, max compression
```

## Comparing `hpfrec-0.2.5.post9.tar` & `hpfrec-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-19 16:47:14.110584 hpfrec-0.2.5.post9/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2020-07-07 19:42:30.000000 hpfrec-0.2.5.post9/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)       86 2020-07-07 19:42:22.000000 hpfrec-0.2.5.post9/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      329 2023-03-19 16:47:14.110584 hpfrec-0.2.5.post9/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)    10182 2023-03-19 16:27:22.000000 hpfrec-0.2.5.post9/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-19 16:47:14.110584 hpfrec-0.2.5.post9/hpfrec/
--rw-r--r--   0 david     (1000) david     (1000)    58458 2022-05-30 19:58:02.000000 hpfrec-0.2.5.post9/hpfrec/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      619 2023-03-19 16:26:27.000000 hpfrec-0.2.5.post9/hpfrec/cython_double.pyx
--rw-r--r--   0 david     (1000) david     (1000)      785 2023-03-19 16:26:45.000000 hpfrec-0.2.5.post9/hpfrec/cython_float.pyx
--rw-r--r--   0 david     (1000) david     (1000)    32609 2021-07-13 04:12:33.000000 hpfrec-0.2.5.post9/hpfrec/cython_loops.pxi
--rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:48.000000 hpfrec-0.2.5.post9/hpfrec/return0.pyx
--rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:50.000000 hpfrec-0.2.5.post9/hpfrec/return1.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-19 16:47:14.110584 hpfrec-0.2.5.post9/hpfrec.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      329 2023-03-19 16:47:14.000000 hpfrec-0.2.5.post9/hpfrec.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      342 2023-03-19 16:47:14.000000 hpfrec-0.2.5.post9/hpfrec.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-03-19 16:47:14.000000 hpfrec-0.2.5.post9/hpfrec.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-03-19 16:47:14.000000 hpfrec-0.2.5.post9/hpfrec.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        7 2023-03-19 16:47:14.000000 hpfrec-0.2.5.post9/hpfrec.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       95 2021-04-15 15:58:17.000000 hpfrec-0.2.5.post9/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       79 2023-03-19 16:47:14.114584 hpfrec-0.2.5.post9/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    10190 2023-03-19 16:46:50.000000 hpfrec-0.2.5.post9/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:27:48.958666 hpfrec-0.2.6/
+-rw-r--r--   0 david     (1000) david     (1000)     1317 2020-07-07 19:42:30.000000 hpfrec-0.2.6/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)       86 2020-07-07 19:42:22.000000 hpfrec-0.2.6/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      323 2023-07-03 18:27:48.958666 hpfrec-0.2.6/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     9089 2023-03-28 18:57:18.000000 hpfrec-0.2.6/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:27:48.958666 hpfrec-0.2.6/hpfrec/
+-rw-r--r--   0 david     (1000) david     (1000)    58449 2023-07-03 18:23:35.000000 hpfrec-0.2.6/hpfrec/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      619 2023-03-19 16:26:27.000000 hpfrec-0.2.6/hpfrec/cython_double.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      785 2023-03-19 16:26:45.000000 hpfrec-0.2.6/hpfrec/cython_float.pyx
+-rw-r--r--   0 david     (1000) david     (1000)    32584 2023-07-03 18:24:17.000000 hpfrec-0.2.6/hpfrec/cython_loops.pxi
+-rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:48.000000 hpfrec-0.2.6/hpfrec/return0.pyx
+-rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:50.000000 hpfrec-0.2.6/hpfrec/return1.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:27:48.958666 hpfrec-0.2.6/hpfrec.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      323 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      342 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)        7 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       95 2021-04-15 15:58:17.000000 hpfrec-0.2.6/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       79 2023-07-03 18:27:48.958666 hpfrec-0.2.6/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    10273 2023-07-03 18:26:58.000000 hpfrec-0.2.6/setup.py
```

### Comparing `hpfrec-0.2.5.post9/LICENSE` & `hpfrec-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hpfrec-0.2.5.post9/README.md` & `hpfrec-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 Y_ui ~ Poisson(Theta_u' Beta_i)
 ```
 The parameters are fit using mean-field approximation (a form of Bayesian variational inference) with coordinate ascent (updating each parameter separately until convergence).
 
 ## Installation
 
+**Note:** requires a C compiler configured for Python. See [this guide](https://github.com/david-cortes/installing-optimized-libraries) for instructions.
+
 Package is available on PyPI, can be installed with:
 
 ```
 pip install hpfrec
 ```
 
 Or if that fails:
@@ -61,18 +63,14 @@
 or, for forcing a maximum-compatibility x86-64 binary:
 ```
 export CFLAGS="-march=x86-64"
 pip install hpfrec
 ```
 ** *
 
-As it contains Cython code, it requires a C compiler. In Windows, this usually means it requires a Visual Studio Build Tools installation (with MSVC140 component for `conda`) (or MinGW + GCC), and if using Anaconda, might also require configuring it to use said Visual Studio instead of MinGW, otherwise the installation from `pip` might fail. For more details see this guide:
-[Cython Extensions On Windows](https://github.com/cython/cython/wiki/CythonExtensionsOnWindows)
-
-
 ## Sample usage
 
 ```python
 import pandas as pd, numpy as np
 from hpfrec import HPF
 
 ## Generating sample counts data
@@ -178,19 +176,11 @@
 
 For faster fitting and predictions, use SciPy and NumPy libraries compiled against MKL or OpenBLAS. These come by default with MKL in Anaconda installations.
 
 The constructor for HPF allows some parameters to make it run faster (if you know what you're doing): these are `allow_inconsistent_math=True`, `full_llk=False`, `stop_crit='diff-norm'`, `reindex=False`, `verbose=False`. See the documentation for more details.
 
 Using stochastic variational inference, which fits the data in smaller batches containing all the user-item interactions only for subsets of users, might converge in fewer iterations (epochs), but the results tend be slightly worse.
 
-## Troubleshooting
-
-* Package uses only one CPU core: make sure that your C compiler supports OpenMP (both Visual Studio and GCC do in default installations, but with MinGW you might need additional modules).
-* Error with `vcvarsall.bat`: see installation instructions (you need to configure your Python installation to use Visual Studio and set the correct paths to libraries). If you are using Python 2, try installing under a Python 3 environment instead and the problem might disappear.
-* Parameters turn to NaN: you might have run into an unlucky parmeter initialization. Try using a different random seed, or changing the number of latent factors (`k`). If passing `reindex=False`, try changing to `reindex=True`.
-
-The package has only been tested under Python 3.6.
-
 ## References
 * [1] Gopalan, Prem, Jake M. Hofman, and David M. Blei. "Scalable Recommendation with Hierarchical Poisson Factorization." UAI. 2015.
 * [2] Gopalan, Prem, Jake M. Hofman, and David M. Blei. "Scalable recommendation with poisson factorization." arXiv preprint arXiv:1311.1704 (2013).
 * [3] Hoffman, Matthew D., et al. "Stochastic variational inference." The Journal of Machine Learning Research 14.1 (2013): 1303-1347.
```

### Comparing `hpfrec-0.2.5.post9/hpfrec/__init__.py` & `hpfrec-0.2.6/hpfrec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd, numpy as np
 import multiprocessing, os, warnings
 from . import cython_loops_float, cython_loops_double, _check_openmp
 import ctypes, types, inspect
-from scipy.sparse import coo_matrix, csr_matrix
+from scipy.sparse import coo_array, issparse
 ### TODO: don't do this, use iloc/loc and make copies instead
 pd.options.mode.chained_assignment = None
 
 class HPF:
 	"""
 	Hierarchical Poisson Factorization
 
@@ -377,19 +377,19 @@
 		----
 		Fitting in mini-batches is more prone to numerical instability and compared to full-batch
 		variational inference, it is more likely that all your parameters will turn to NaNs (which
 		means the optimization procedure failed).
 
 		Parameters
 		----------
-		counts_df : pandas data frame (nobs, 3) or coo_matrix
+		counts_df : pandas data frame (nobs, 3) or coo_array
 			Input data with one row per non-zero observation, consisting of triplets ('UserId', 'ItemId', 'Count').
 			Must containin columns 'UserId', 'ItemId', and 'Count'.
 			Combinations of users and items not present are implicitly assumed to be zero by the model.
-			Can also pass a sparse coo_matrix, in which case 'reindex' will be forced to 'False'.
+			Can also pass a sparse coo_array, in which case 'reindex' will be forced to 'False'.
 		val_set : pandas data frame (nobs, 3)
 			Validation set on which to monitor log-likelihood. Same format as counts_df.
 
 		Returns
 		-------
 		self : obj
 			Copy of this object
@@ -441,26 +441,26 @@
 		elif input_df.__class__.__name__ == 'DataFrame':
 			assert input_df.shape[0] > 0
 			assert 'UserId' in input_df.columns.values
 			assert 'ItemId' in input_df.columns.values
 			assert 'Count' in input_df.columns.values
 			input_df = input_df[['UserId', 'ItemId', 'Count']]
 			
-		elif input_df.__class__.__name__ == 'coo_matrix':
+		elif issparse(input_df) and (input_df.format == "coo"):
 			self.nusers = input_df.shape[0]
 			self.nitems = input_df.shape[1]
 			input_df = pd.DataFrame({
 				'UserId' : input_df.row,
 				'ItemId' : input_df.col,
 				'Count' : input_df.data
 				})
 			self.reindex = False
 			calc_n = False
 		else:
-			raise ValueError("'input_df' must be a pandas data frame, numpy array, or scipy sparse coo_matrix.")
+			raise ValueError("'input_df' must be a pandas data frame, numpy array, or scipy sparse coo_array.")
 
 		if self.stop_crit in ['maxiter', 'diff-norm']:
 			thr = 0
 		else:
 			thr = 0.9
 		self.input_df = input_df
 		obs_zero = self.input_df.Count.values <= thr
@@ -535,24 +535,24 @@
 		elif val_set.__class__.__name__ == 'DataFrame':
 			assert val_set.shape[0] > 0
 			assert 'UserId' in val_set.columns.values
 			assert 'ItemId' in val_set.columns.values
 			assert 'Count' in val_set.columns.values
 			self.val_set = val_set[['UserId', 'ItemId', 'Count']]
 
-		elif val_set.__class__.__name__ == 'coo_matrix':
+		elif issparse(val_set) and (val_set.format == "coo"):
 			assert val_set.shape[0] <= self.nusers
 			assert val_set.shape[1] <= self.nitems
 			self.val_set = pd.DataFrame({
 				'UserId' : val_set.row,
 				'ItemId' : val_set.col,
 				'Count'  : val_set.data
 				})
 		else:
-			raise ValueError("'val_set' must be a pandas data frame, numpy array, or sparse coo_matrix.")
+			raise ValueError("'val_set' must be a pandas data frame, numpy array, or sparse coo_array.")
 			
 		if self.stop_crit == 'val-llk':
 			thr = 0
 		else:
 			thr = 0.9
 		obs_zero = self.val_set.Count.values <= thr
 		if obs_zero.sum() > 0:
@@ -587,16 +587,15 @@
 			self.val_set['ItemId'] = self.val_set.ItemId.astype(cython_loops.obj_ind_type)
 		return None
 			
 	def _store_metadata(self, for_partial_fit=False):
 		cython_loops = cython_loops_float if self.use_float else cython_loops_double
 		if self.verbose and for_partial_fit:
 			print("Creating user indices for stochastic optimization...")
-		X = coo_matrix((self.input_df.Count.values, (self.input_df.UserId.values, self.input_df.ItemId.values)), shape=(self.nusers, self.nitems))
-		X = csr_matrix(X)
+		X = coo_array((self.input_df.Count.values, (self.input_df.UserId.values, self.input_df.ItemId.values)), shape=(self.nusers, self.nitems)).tocsr()
 		self._n_seen_by_user = X.indptr[1:] - X.indptr[:-1]
 		if for_partial_fit:
 			self._st_ix_user = X.indptr.astype(cython_loops.obj_ind_type)
 			self.input_df.sort_values('UserId', inplace=True)
 		else:
 			self._st_ix_user = X.indptr[:-1]
 		self.seen = X.indices
```

### Comparing `hpfrec-0.2.5.post9/hpfrec/cython_double.pyx` & `hpfrec-0.2.6/hpfrec/cython_double.pyx`

 * *Files identical despite different names*

### Comparing `hpfrec-0.2.5.post9/hpfrec/cython_float.pyx` & `hpfrec-0.2.6/hpfrec/cython_float.pyx`

 * *Files identical despite different names*

### Comparing `hpfrec-0.2.5.post9/hpfrec/cython_loops.pxi` & `hpfrec-0.2.6/hpfrec/cython_loops.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,16 @@
 
 def cast_ind_type(n):
 	return <ind_type> n
 
 ### Procedures reusable by package ctpfrec
 ##########################################
 def get_csc_data(ix_u, ix_i, Y, nU, nI):
-	from scipy.sparse import coo_matrix, csc_matrix
-	X = coo_matrix((Y, (ix_u, ix_i)), shape=(nU, nI))
-	X = csc_matrix(X)
+	from scipy.sparse import coo_array
+	X = coo_array((Y, (ix_u, ix_i)), shape=(nU, nI)).tocsc()
 	return X.indptr.astype(obj_ind_type), X.indices.astype(obj_ind_type), X.data.astype(c_real_t)
 
 def get_unique_items_batch(np.ndarray[ind_type, ndim=1] users_this_batch,
 						   np.ndarray[ind_type, ndim=1] st_ix_u,
 						   np.ndarray[ind_type, ndim=1] ix_i, int nthreads,
 						   return_ix=False):
 	cdef ind_type nusers_batch = users_this_batch.shape[0]
```

### Comparing `hpfrec-0.2.5.post9/setup.py` & `hpfrec-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,19 +116,22 @@
         arg_omp4 = "-qopenmp"
         arg_omp5 = "-xopenmp"
         is_apple = sys.platform[:3].lower() == "dar"
         args_apple_omp = ["-Xclang", "-fopenmp", "-lomp"]
         args_apple_omp2 = ["-Xclang", "-fopenmp", "-L/usr/local/lib", "-lomp", "-I/usr/local/include"]
         has_brew_omp = False
         if is_apple:
-            res_brew_pref = subprocess.run(["brew", "--prefix", "libomp"], capture_output=silent_tests)
-            if res_brew_pref.returncode == EXIT_SUCCESS:
-                has_brew_omp = True
-                brew_omp_prefix = res_brew_pref.stdout.decode().strip()
-                args_apple_omp3 = ["-Xclang", "-fopenmp", f"-L{brew_omp_prefix}/lib", "-lomp", f"-I{brew_omp_prefix}/include"]
+            try:
+                res_brew_pref = subprocess.run(["brew", "--prefix", "libomp"], capture_output=True)
+                if res_brew_pref.returncode == EXIT_SUCCESS:
+                    brew_omp_prefix = res_brew_pref.stdout.decode().strip()
+                    args_apple_omp3 = ["-Xclang", "-fopenmp", f"-L{brew_omp_prefix}/lib", "-lomp", f"-I{brew_omp_prefix}/include"]
+                    has_brew_omp = True
+            except Exception as e:
+                pass
 
 
         if self.test_supports_compile_arg(arg_omp1, with_omp=True):
             for e in self.extensions:
                 e.extra_compile_args.append(arg_omp1)
                 e.extra_link_args.append(arg_omp1)
         elif is_apple and self.test_supports_compile_arg(args_apple_omp, with_omp=True):
@@ -206,15 +209,15 @@
     packages = ['hpfrec'],
     install_requires=[
      'pandas>=0.24',
      'numpy>=1.18',
      'scipy',
      'cython'
 ],
-    version = '0.2.5-9',
+    version = '0.2.6',
     description = 'Hierarchical Poisson matrix factorization for recommender systems',
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/hpfrec',
     keywords = ['poisson', 'probabilistic', 'non-negative', 'factorization', 'variational inference', 'collaborative filtering'],
     classifiers = [],
 
     cmdclass = {'build_ext': build_ext_subclass},
```

