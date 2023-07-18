# Comparing `tmp/ctpfrec-0.1.8.tar.gz` & `tmp/ctpfrec-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ctpfrec-0.1.8.tar", last modified: Tue Jul  7 20:06:42 2020, max compression
+gzip compressed data, was "dist/ctpfrec-0.1.9.tar", last modified: Wed Jul  8 18:00:55 2020, max compression
```

## Comparing `ctpfrec-0.1.8.tar` & `ctpfrec-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/
--rw-r--r--   0 david     (1000) david     (1000)      139 2020-05-29 17:03:36.000000 ctpfrec-0.1.8/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      443 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     8389 2020-05-29 18:02:00.000000 ctpfrec-0.1.8/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/ctpfrec/
--rw-r--r--   0 david     (1000) david     (1000)    80131 2020-07-07 20:02:03.000000 ctpfrec-0.1.8/ctpfrec/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    33279 2020-07-07 20:00:05.000000 ctpfrec-0.1.8/ctpfrec/cy.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/ctpfrec.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      443 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/ctpfrec.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      244 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/ctpfrec.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/ctpfrec.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       52 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/ctpfrec.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        8 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/ctpfrec.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       78 2020-07-07 19:59:21.000000 ctpfrec-0.1.8/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       79 2020-07-07 20:06:42.000000 ctpfrec-0.1.8/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)     1750 2020-07-07 19:59:31.000000 ctpfrec-0.1.8/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-07-08 18:00:55.000000 ctpfrec-0.1.9/
+-rw-r--r--   0 david     (1000) david     (1000)      160 2020-07-08 17:56:36.000000 ctpfrec-0.1.9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      443 2020-07-08 18:00:55.000000 ctpfrec-0.1.9/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     8389 2020-05-29 18:02:00.000000 ctpfrec-0.1.9/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-07-08 18:00:55.000000 ctpfrec-0.1.9/ctpfrec/
+-rw-r--r--   0 david     (1000) david     (1000)    83059 2020-07-08 17:54:02.000000 ctpfrec-0.1.9/ctpfrec/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)    32770 2020-07-08 17:38:45.000000 ctpfrec-0.1.9/ctpfrec/cy.pxi
+-rw-r--r--   0 david     (1000) david     (1000)      638 2020-07-08 17:36:58.000000 ctpfrec-0.1.9/ctpfrec/cy_double.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      803 2020-07-08 17:43:19.000000 ctpfrec-0.1.9/ctpfrec/cy_float.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-07-08 18:00:55.000000 ctpfrec-0.1.9/ctpfrec.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      443 2020-07-08 18:00:54.000000 ctpfrec-0.1.9/ctpfrec.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      287 2020-07-08 18:00:54.000000 ctpfrec-0.1.9/ctpfrec.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2020-07-08 18:00:54.000000 ctpfrec-0.1.9/ctpfrec.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       52 2020-07-08 18:00:54.000000 ctpfrec-0.1.9/ctpfrec.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)        8 2020-07-08 18:00:54.000000 ctpfrec-0.1.9/ctpfrec.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       78 2020-07-07 19:59:21.000000 ctpfrec-0.1.9/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       79 2020-07-08 18:00:55.000000 ctpfrec-0.1.9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)     1877 2020-07-08 17:52:35.000000 ctpfrec-0.1.9/setup.py
```

### Comparing `ctpfrec-0.1.8/README.md` & `ctpfrec-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ctpfrec-0.1.8/ctpfrec/__init__.py` & `ctpfrec-0.1.9/ctpfrec/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd, numpy as np
 import multiprocessing, os, warnings
-from . import cy
+from . import cy_double, cy_float
 import ctypes, types, inspect
-from hpfrec import HPF, cython_loops_float as cython_loops
+from hpfrec import HPF, cython_loops_float, cython_loops_double
 pd.options.mode.chained_assignment = None
 
 
 class CTPF:
 	"""
 	Collaborative Topic Poisson Factorization
 
@@ -133,14 +133,19 @@
 	maxiter : int or None
 		Maximum number of iterations for which to run the optimization procedure. This corresponds to epochs when
 		fitting in batches of users. Recommended to use a lower number when passing a batch size.
 	check_every : None or int
 		Calculate log-likelihood every N iterations.
 	verbose : bool
 		Whether to print convergence messages.
+	use_float : bool
+		Whether to use the C float type (typically ``np.float32``). Using float types (as compared to double)
+		results in less memory usage and faster operations, but it has less numeric precision and the results
+		will be slightly worse compared to using double.
+		If passing ``False``, will use C double (typically ``np.float64``).
 	random_seed : int or None
 		Random seed to use when starting the parameters.
 	ncores : int
 		Number of cores to use to parallelize computations.
 		If set to -1, will use the maximum available on the computer.
 	initialize_hpf : bool
 		Whether to initialize the Theta and Beta matrices using hierarchical Poisson factorization
@@ -241,15 +246,15 @@
 	----------
 	[1] Content-based recommendations with poisson factorization (Gopalan, P.K., Charlin, L. and Blei, D., 2014)
 	"""
 	
 	def __init__(self, k=50, a=.3, b=.3, c=.3, d=.3, e=.3, f=.3, g=.3, h=.3,
 				 stop_crit='train-llk', stop_thr=1e-3, reindex=True,
 				 miniter=25, maxiter=70, check_every=10, verbose=True,
-				 random_seed=None, ncores=-1, initialize_hpf=True,
+				 use_float=True, random_seed=None, ncores=-1, initialize_hpf=True,
 				 standardize_items=False, rescale_factors=False,
 				 missing_items='include', step_size=lambda x: 1-1/np.sqrt(x+1),
 				 allow_inconsistent_math=False, full_llk=False,
 				 keep_data=True, save_folder=None, produce_dicts=True,
 				 sum_exp_trick=False, keep_all_objs=True):
 
 		## checking input
@@ -367,14 +372,15 @@
 		self.keep_data = bool(keep_data)
 		self.maxiter = maxiter
 		self.miniter = miniter
 		self.check_every = check_every
 		self.stop_thr = stop_thr
 		self.save_folder = save_folder
 		self.verbose = verbose
+		self.use_float = bool(use_float)
 		self.produce_dicts = bool(produce_dicts)
 		self.full_llk = bool(full_llk)
 		self.keep_all_objs = bool(keep_all_objs)
 		self.sum_exp_trick = bool(sum_exp_trick)
 		self.initialize_hpf = bool(initialize_hpf)
 		self.standardize_items = bool(standardize_items)
 		self.rescale_factors = bool(rescale_factors)
@@ -697,18 +703,19 @@
 			col2 = 'AttributeId'
 		else:
 			self._unexpected_err_msg()
 
 		return col1, col2, subj
 
 	def _cast_df(self, df, ttl):
+		cy = cy_float if self.use_float else cy_double
 		col1, col2, subj = self._cols_from_ttl(ttl)
 		df[col1] = df[col1].values.astype(cy.obj_ind_type)
 		df[col2] = df[col2].values.astype(cy.obj_ind_type)
-		df['Count'] = df.Count.astype(ctypes.c_float)
+		df['Count'] = df.Count.astype(ctypes.c_float if self.use_float else ctypes.c_double if self.use_float else ctypes.c_double)
 		return df
 
 	def _check_df(self, df, ttl):
 		col1, col2, subj = self._cols_from_ttl(ttl)
 
 		if isinstance(df, np.ndarray):
 			assert len(df.shape) > 1
@@ -873,24 +880,24 @@
 						self.Kappa_shp = self.Kappa_shp[:self._take_ix_userattr, :]
 					del self._take_ix_userattr
 				del self._need_filter_kappa
 		return None
 
 	def _initalize_parameters(self):
 		## TODO: make this function more modular
+		## TODO: improve the way of adding random noise in the initialization
 
-		rng = np.random.default_rng(seed = self.random_seed \
-									if (self.random_seed is not None) and (self.random_seed > 0) else None)
+		rng = np.random.Generator(np.random.MT19937(seed = self.random_seed))
 
 		if self.initialize_hpf:
 			if self.verbose:
 				print("Initializing Theta and Beta through HPF...")
 				print("")
 			h = HPF(k=self.k, verbose=self.verbose, reindex=True, produce_dicts=False, stop_crit='diff-norm',
-					stop_thr=self.stop_thr, random_seed=self.random_seed, keep_all_objs=False,
+					stop_thr=self.stop_thr, random_seed=self.random_seed, keep_all_objs=False, use_float=self.use_float,
 					sum_exp_trick=self.sum_exp_trick, allow_inconsistent_math=self.allow_inconsistent_math,)
 			h.fit(self._words_df.rename(columns={'ItemId':'UserId', 'WordId':'ItemId'}).copy())
 			if (h.nusers == self.nitems) and (h.nitems == self.nwords):
 				## if using missing_items='include', it should always enter this section
 				order_theta = np.argsort(h.user_mapping_)
 				order_beta = np.argsort(h.item_mapping_)
 				self.Theta_shp = h.Theta[order_theta].copy()
@@ -909,43 +916,43 @@
 					items_take = np.in1d(h.user_mapping_, ids_counts_df)
 					## for which words to take, need to forcibly determine intersection
 					items_words_df = self._words_df.ItemId.unique()
 					items_intersect = np.in1d(items_words_df, ids_counts_df)
 					words_include = self._words_df.WordId.loc[np.in1d(self._words_df.ItemId, items_words_df[items_intersect])].unique()
 					words_take = pd.Categorical(words_include, h.item_mapping_).codes
 
-				self.Theta_shp = (self.c * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float)
+				self.Theta_shp = (self.c * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 				self.Theta_shp[h.user_mapping_[items_take],:] = h.Theta[items_take].copy()
 
-				self.Beta_shp = (self.a * 2*rng.beta(20, 20, size=(self.nwords, self.k))).astype(ctypes.c_float)
+				self.Beta_shp = (self.a * 2*rng.beta(20, 20, size=(self.nwords, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 				self.Beta_shp[h.item_mapping_[words_take],:] = h.Beta[words_take].copy()
 				
 				self.Theta_rte = self.d + self.Beta_shp.sum(axis=0, keepdims=True)
 				self.Beta_rte = self.b + self.Theta_shp.sum(axis=0, keepdims=True)
 
 			if np.isnan(self.Theta_shp).sum().sum() > 0:
 				warnings.warn("NaNs produced in initialization of Theta, will use a random start.")
-				self.Theta_shp = (self.c * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float)
-				self.Theta_rte = (self.d * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
+				self.Theta_shp = (self.c * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+				self.Theta_rte = (self.d * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 			if np.isnan(self.Beta_shp).sum().sum() > 0:
 				warnings.warn("NaNs produced in initialization of Beta, will use a random start.")
-				self.Beta_shp = (self.a * 2*rng.beta(20, 20, size=(self.nwords, self.k))).astype(ctypes.c_float)
-				self.Beta_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
+				self.Beta_shp = (self.a * 2*rng.beta(20, 20, size=(self.nwords, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+				self.Beta_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 			if self.verbose:
 				print("**********************************")
 				print("")
 
 			if self._has_user_df:
-				self.Omega_shp = (self.e * 2*rng.beta(20, 20, size=(self.nusers, self.k))).astype(ctypes.c_float)
-				self.Omega_rte = (self.f * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
+				self.Omega_shp = (self.e * 2*rng.beta(20, 20, size=(self.nusers, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+				self.Omega_rte = (self.f * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 				if self.verbose:
 					print("Initializing Kappa through HPF...")
 					print("")
 				h = HPF(k=self.k, verbose=self.verbose, reindex=True, produce_dicts=False, stop_crit='diff-norm',
-					stop_thr=self.stop_thr, random_seed=self.random_seed, keep_all_objs=False,
+					stop_thr=self.stop_thr, random_seed=self.random_seed, keep_all_objs=False, use_float=self.use_float,
 					sum_exp_trick=self.sum_exp_trick, allow_inconsistent_math=self.allow_inconsistent_math)
 				h.fit(self._user_df.rename(columns={'AttributeId':'ItemId'}).copy())
 				
 				if h.nitems == self.nuserattr:
 					## if using missing_items='include', it should always enter this section
 					order_kappa = np.argsort(h.item_mapping_)
 					self.Kappa_shp = h.Beta[order_kappa].copy()
@@ -957,52 +964,52 @@
 					else:
 						users_counts_df = self._counts_df.UserId.unique()
 						users_user_df = self._user_df.UserId.unique()
 						users_intersect = np.in1d(users_user_df, users_counts_df)
 						attr_include = self._user_df.AttributeId.loc[np.in1d(self._user_df.UserId, users_user_df[users_intersect])].unique()
 						attr_take = pd.Categorical(attr_include, h.item_mapping_).codes
 
-					self.Kappa_shp = (self.a * 2*rng.beta(20, 20, size=(self.nuserattr, self.k))).astype(ctypes.c_float)
+					self.Kappa_shp = (self.a * 2*rng.beta(20, 20, size=(self.nuserattr, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 					self.Kappa_shp[h.item_mapping_[attr_take],:] = h.Beta[attr_take].copy()
 					self.Kappa_rte = self.b + h.Theta.sum(axis=0, keepdims=True)
 					del h
 
 
 				if np.isnan(self.Kappa_shp).sum().sum() > 0:
 					warnings.warn("NaNs produced in initialization of Kappa, will use a random start.")
-					self.Kappa_shp = (self.a * 2*rng.beta(20, 20, size=(self.nuserattr, self.k))).astype(ctypes.c_float)
-					self.Kappa_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
+					self.Kappa_shp = (self.a * 2*rng.beta(20, 20, size=(self.nuserattr, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+					self.Kappa_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 				if self.verbose:
 					print("**********************************")
 					print("")
 			else:
-				self.Kappa_shp = np.empty((0,0), dtype=ctypes.c_float)
-				self.Kappa_rte = np.empty((0,0), dtype=ctypes.c_float)
+				self.Kappa_shp = np.empty((0,0), dtype=ctypes.c_float if self.use_float else ctypes.c_double)
+				self.Kappa_rte = np.empty((0,0), dtype=ctypes.c_float if self.use_float else ctypes.c_double)
 		else:
-			self.Beta_shp = (self.a * 2*rng.beta(20, 20, size=(self.nwords, self.k))).astype(ctypes.c_float)
-			self.Theta_shp = (self.c * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float)
-			self.Beta_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
-			self.Theta_rte = (self.d * 2*rng.beta(20, 203, size=(1, self.k))).astype(ctypes.c_float)
+			self.Beta_shp = (self.a * 2*rng.beta(20, 20, size=(self.nwords, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+			self.Theta_shp = (self.c * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+			self.Beta_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+			self.Theta_rte = (self.d * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 			if self._has_user_df:
-				self.Kappa_shp = (self.a * 2*rng.beta(20, 20, size=(self.nuserattr, self.k))).astype(ctypes.c_float)
-				self.Kappa_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
+				self.Kappa_shp = (self.a * 2*rng.beta(20, 20, size=(self.nuserattr, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+				self.Kappa_rte = (self.b * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 			else:
-				self.Kappa_shp = np.empty((0,0), dtype=ctypes.c_float)
-				self.Kappa_rte = np.empty((0,0), dtype=ctypes.c_float)
+				self.Kappa_shp = np.empty((0,0), dtype=ctypes.c_float if self.use_float else ctypes.c_double)
+				self.Kappa_rte = np.empty((0,0), dtype=ctypes.c_float if self.use_float else ctypes.c_double)
 		
-		self.Eta_shp = (self.e * 2*rng.beta(20, 20, size=(self.nusers, self.k))).astype(ctypes.c_float)
-		self.Epsilon_shp = (self.g * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float)
-		self.Eta_rte = (self.f * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
-		self.Epsilon_rte = (self.h * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
+		self.Eta_shp = (self.e * 2*rng.beta(20, 20, size=(self.nusers, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+		self.Epsilon_shp = (self.g * 2*rng.beta(20, 20, size=(self.nitems, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+		self.Eta_rte = (self.f * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+		self.Epsilon_rte = (self.h * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 		if self._has_user_df:
-			self.Omega_shp = (self.e * 2*rng.beta(20, 20, size=(self.nusers, self.k))).astype(ctypes.c_float)
-			self.Omega_rte = (self.f * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float)
+			self.Omega_shp = (self.e * 2*rng.beta(20, 20, size=(self.nusers, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
+			self.Omega_rte = (self.f * 2*rng.beta(20, 20, size=(1, self.k))).astype(ctypes.c_float if self.use_float else ctypes.c_double)
 		else:
-			self.Omega_shp = np.empty((0,0), dtype=ctypes.c_float)
-			self.Omega_rte = np.empty((0,0), dtype=ctypes.c_float)
+			self.Omega_shp = np.empty((0,0), dtype=ctypes.c_float if self.use_float else ctypes.c_double)
+			self.Omega_rte = np.empty((0,0), dtype=ctypes.c_float if self.use_float else ctypes.c_double)
 
 		self._divide_parameters(add_beta=False)
 
 	def _divide_parameters(self, add_beta=False):
 		self.Theta = self.Theta_shp / self.Theta_rte
 		self.Eta = self.Eta_shp / self.Eta_rte
 		self.Epsilon = self.Epsilon_shp / self.Epsilon_rte
@@ -1102,44 +1109,47 @@
 		else:
 			has_df = False
 		if has_df and has_coo:
 			raise ValueError("Cannot mix 'coo_matrix' and 'DataFrame' as inputs.")
 		if has_coo:
 			self.reindex = False
 
+		cy = cy_float if self.use_float else cy_double
+		cython_loops = cython_loops_float if self.use_float else cython_loops_double
+
 		## running each sub-process
 		if self.verbose:
 			self._print_st_msg()
 		self._process_data(counts_df, words_df, user_df)
 		if self.verbose:
 			self._print_data_info()
 		if (val_set is not None) and (self.stop_crit!='diff-norm') and (self.stop_crit!='train-llk'):
 			HPF._process_valset(self, val_set)
 		else:
 			self.val_set = pd.DataFrame({
 				'UserId': np.empty(0, dtype=cy.obj_ind_type),
 				'ItemId': np.empty(0, dtype=cy.obj_ind_type),
-				'Count': np.empty(0, dtype=ctypes.c_float)})
+				'Count': np.empty(0, dtype=ctypes.c_float if self.use_float else ctypes.c_double)})
 		if not self._has_user_df:
 			self._user_df = pd.DataFrame({'UserId':np.empty(0, dtype=cy.obj_ind_type),
 				'AttributeId':np.empty(0, dtype=cy.obj_ind_type),
-				'Count':np.empty(0, dtype=ctypes.c_float)})
+				'Count':np.empty(0, dtype=ctypes.c_float if self.use_float else ctypes.c_double)})
 		if self.verbose:
 			print("Initializing parameters...")
 		self._initalize_parameters()
 		self._divide_parameters(add_beta=False)
 		if self.missing_items == 'exclude':
 			self._exclude_missing_from_index()
 			self._filter_words_df()
 			if self._has_user_df:
 				self._filter_user_df()
 			else:
 				self._user_df = pd.DataFrame({'UserId':np.empty(0, dtype=cy.obj_ind_type),
 											  'AttributeId':np.empty(0, dtype=cy.obj_ind_type),
-											  'Count':np.empty(0, dtype=ctypes.c_float)})
+											  'Count':np.empty(0, dtype=ctypes.c_float if self.use_float else ctypes.c_double)})
 
 		## fitting the model
 		self.niter = cy.fit_ctpf(
 			self.Theta_shp, self.Theta_rte, self.Beta_shp, self.Beta_rte,
 			self.Eta_shp, self.Eta_rte, self.Epsilon_shp, self.Epsilon_rte,
 			self.Omega_shp, self.Omega_rte, self.Kappa_shp, self.Kappa_rte,
 			self.Theta, self.Eta, self.Epsilon, self.Omega,
@@ -1348,14 +1358,17 @@
 		----------
 		user : array-like (npred,) or obj
 			User(s) for which to predict each item.
 		item: array-like (npred,) or obj
 			Item(s) for which to predict for each user.
 		"""
 		assert self.is_fitted
+		cy = cy_float if self.use_float else cy_double
+		cython_loops = cython_loops_float if self.use_float else cython_loops_double
+
 		if isinstance(user, list) or isinstance(user, tuple):
 			user = np.array(user)
 		if isinstance(item, list) or isinstance(item, tuple):
 			item = np.array(item)
 		if user.__class__.__name__=='Series':
 			user = user.values
 		if item.__class__.__name__=='Series':
@@ -1493,14 +1506,16 @@
 
 		words_df, new_item_mapping = self._process_extra_df(words_df, ttl='words_df')
 		words_df['ItemId'] -= self.nitems
 		new_max_id = words_df.ItemId.max() + 1
 		if new_max_id <= 0:
 			raise ValueError("Numeration of item IDs overlaps with IDs passed to '.fit'.")
 
+		cy = cy_float if self.use_float else cy_double
+		cython_loops = cython_loops_float if self.use_float else cython_loops_double
 		new_Theta_shp, temp = cy.calc_item_factors(
 					words_df, new_max_id, maxiter, cython_loops.cast_ind_type(self.k), stop_thr, random_seed, ncores,
 					cython_loops.cast_real_t(self.a), cython_loops.cast_real_t(self.b),
 					cython_loops.cast_real_t(self.c), cython_loops.cast_real_t(self.d),
 					self.Theta_rte, self.Beta_shp, self.Beta_rte
 					)
 
@@ -1587,14 +1602,16 @@
 		new_max_id = user_df.UserId.max() + 1
 		if new_max_id <= 0:
 			raise ValueError("Numeration of item IDs overlaps with IDs passed to '.fit'.")
 
 		## Will reuse the exact same function from the add items, need to change names accordingly
 		user_df.rename(columns={'UserId':'ItemId', 'AttributeId':'WordId'}, inplace=True)
 
+		cy = cy_float if self.use_float else cy_double
+		cython_loops = cython_loops_float if self.use_float else cython_loops_double
 		new_Omega_shp, temp = cy.calc_item_factors(
 					user_df, new_max_id, maxiter, cython_loops.cast_ind_type(self.k),
 					stop_thr, random_seed, ncores,
 					cython_loops.cast_real_t(self.a), cython_loops.cast_real_t(self.b),
 					cython_loops.cast_real_t(self.c), cython_loops.cast_real_t(self.d),
 					self.Omega_rte, self.Kappa_shp, self.Kappa_rte
 					)
@@ -1618,14 +1635,16 @@
 		if self.rescale_factors:
 			raise ValueError("Cannot produce new factors when using 'rescale_factors=True'.")
 		assert self.is_fitted
 		if not self.keep_all_objs:
 			msg = "Can only add " + err_subj + "s to a fitted model when called with 'keep_all_objs=True'."
 			raise ValueError(msg)
 
+		cython_loops = cython_loops_float if self.use_float else cython_loops_double
+
 		if ncores is None:
 			ncores = 1 
 		if ncores < 1:
 			ncores = multiprocessing.cpu_count()
 		assert ncores>0
 		assert isinstance(ncores, int)
 		ncores = cython_loops.cast_int(ncores)
@@ -1693,17 +1712,17 @@
 					return_ix=True, return_temp=False
 					)
 
 		## Adding the new parameters
 		new_Theta = new_Theta_shp / self.Theta_rte
 		self.Theta_shp = np.r_[self.Theta_shp, new_Theta]
 		self.Theta = np.r_[self.Theta, new_Theta_shp]
-		self.Epsilon = np.r_[self.Epsilon, np.zeros((int(new_max_id), int(self.k)), dtype=ctypes.c_float)]
-		self.Epsilon_shp = np.r_[self.Epsilon_shp, np.zeros((int(new_max_id), int(self.k)), dtype=ctypes.c_float)]
-		self.Epsilon_rte = np.r_[self.Epsilon_rte, np.zeros((int(new_max_id), int(self.k)), dtype=ctypes.c_float)]
+		self.Epsilon = np.r_[self.Epsilon, np.zeros((int(new_max_id), int(self.k)), dtype=ctypes.c_float if self.use_float else ctypes.c_double)]
+		self.Epsilon_shp = np.r_[self.Epsilon_shp, np.zeros((int(new_max_id), int(self.k)), dtype=ctypes.c_float if self.use_float else ctypes.c_double)]
+		self.Epsilon_rte = np.r_[self.Epsilon_rte, np.zeros((int(new_max_id), int(self.k)), dtype=ctypes.c_float if self.use_float else ctypes.c_double)]
 		self._M2 = np.r_[self._M2, new_Theta]
 
 
 		## Adding the new IDs
 		if self.reindex:
 			self.item_mapping_ = new_item_mapping
 			if self.produce_dicts:
@@ -1771,14 +1790,17 @@
 		if user_df is not None:
 			if not self._has_user_df:
 				raise ValueError("Can only use 'user_df' when the model was fit to user side information.")
 
 		if (counts_df is None) and (not self._has_user_df):
 			raise ValueError("Must pass 'counts_df' to add a new user.")
 
+		cy = cy_float if self.use_float else cy_double
+		cython_loops = cython_loops_float if self.use_float else cython_loops_double
+
 		
 		if (counts_df is not None) and (user_df is not None) and self._has_user_df:
 			## factors based on both attributes and interactions
 			user_df, counts_df, new_user_mapping = self._process_extra_df(user_df, ttl='user_df', df2=counts_df)
 			counts_df['UserId'] -= self.nusers
 			user_df['UserId'] -= self.nusers
 			new_max_id = int(max(counts_df.UserId.max(), user_df.UserId.max()) + 1)
@@ -1822,31 +1844,31 @@
 
 			## Adding the new parameters
 			new_Eta = new_Eta_shp / self.Eta_rte
 			self.Eta_shp = np.r_[self.Eta_shp, new_Eta_shp]
 			self.Eta = np.r_[self.Eta, new_Eta]
 			self._M1 = np.r_[self._M1, new_Eta]
 			if self._has_user_df:
-				self.Omega = np.r_[self.Omega, np.zeros((new_max_id, self.k), dtype=ctypes.c_float)]
-				self.Omega_shp = np.r_[self.Omega_shp, np.zeros((new_max_id, self.k), dtype=ctypes.c_float)]
+				self.Omega = np.r_[self.Omega, np.zeros((new_max_id, self.k), dtype=ctypes.c_float if self.use_float else ctypes.c_double)]
+				self.Omega_shp = np.r_[self.Omega_shp, np.zeros((new_max_id, self.k), dtype=ctypes.c_float if self.use_float else ctypes.c_double)]
 
 		## factors based on user attributes
 		else:
 			new_Omega_shp, new_user_mapping, new_max_id = self._predict_user_factors(
 					user_df=user_df, maxiter=maxiter, ncores=ncores,
 					random_seed=random_seed, stop_thr=stop_thr,
 					return_ix=True, return_temp=False
 					)
 
 			## Adding the new parameters
 			new_Omega = new_Omega_shp / self.Omega_rte
 			self.Omega_shp = np.r_[self.Omega_shp, new_Omega_shp]
 			self.Omega = np.r_[self.Omega, new_Omega]
-			self.Eta = np.r_[self.Eta, np.zeros((new_max_id, self.k), dtype=ctypes.c_float)]
-			self.Eta_shp = np.r_[self.Eta_shp, np.zeros((new_max_id, self.k), dtype=ctypes.c_float)]
+			self.Eta = np.r_[self.Eta, np.zeros((new_max_id, self.k), dtype=ctypes.c_float if self.use_float else ctypes.c_double)]
+			self.Eta_shp = np.r_[self.Eta_shp, np.zeros((new_max_id, self.k), dtype=ctypes.c_float if self.use_float else ctypes.c_double)]
 			self._M1 = np.r_[self._M1, new_Omega]
 
 		
 		## updating the list of seen items for these users
 		if self.keep_data and (counts_df is not None):
 			for u in range(int(new_max_id)):
 				items_this_user = counts_df.ItemId.values[counts_df.UserId == u]
@@ -1893,14 +1915,15 @@
 		-------
 		llk : dict
 			Dictionary containing the calculated log-likelihood and the number of
 			observations that were used to calculate it.
 		"""
 		assert self.is_fitted
 		HPF._process_valset(self, counts_df, valset=False)
+		cython_loops = cython_loops_float if self.use_float else cython_loops_double
 		out = {'llk': cython_loops.calc_llk(self.val_set.Count.values,
 											self.val_set.UserId.values,
 											self.val_set.ItemId.values,
 											self._M1,
 											self._M2,
 											cython_loops.cast_int(self.k),
 											cython_loops.cast_int(self.ncores),
```

### Comparing `ctpfrec-0.1.8/ctpfrec/cy.pyx` & `ctpfrec-0.1.9/ctpfrec/cy.pxi`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,12 @@
 import numpy as np
 cimport numpy as np
 cimport cython
 from cython.parallel cimport prange
-from scipy.linalg.cython_blas cimport sdot
 from scipy.special.cython_special cimport psi, gamma, loggamma
-## TODO: use libc.math once Cython 0.30 is released
-# from libc.math cimport log, logf, exp, expf, HUGE_VALF, HUGE_VALL
-cdef extern from "<math.h>":
-	double log(double x) nogil
-	float logf(float) nogil
-	long double logl(long double) nogil
-	double exp(double x) nogil
-	float expf(float) nogil
-	const double HUGE_VAL
-	const float HUGE_VALF
-	const long double HUGE_VALL
-import ctypes
-from hpfrec import cython_loops_float as cython_loops
 import time
 
 ## Note: As of the end of 2018, MSVC is still stuck with OpenMP 2.0 (released 2002), which does not support
 ## parallel for loops with unsigend iterators. If you are using a different compiler, this part can be safely removed
 IF UNAME_SYSNAME == "Windows":
 	obj_ind_type = ctypes.c_longlong
 	ctypedef long long ind_type
@@ -32,81 +18,81 @@
 	ctypedef size_t ind_type
 	ctypedef long double long_double_type
 	obj_long_double_type = ctypes.c_longdouble
 	LD_HUGE_VAL = HUGE_VALL
 
 ### Main function
 #################
-def fit_ctpf(np.ndarray[float, ndim=2] Theta_shp, np.ndarray[float, ndim=2] Theta_rte,
-			 np.ndarray[float, ndim=2] Beta_shp, np.ndarray[float, ndim=2] Beta_rte,
-			 np.ndarray[float, ndim=2] Eta_shp, np.ndarray[float, ndim=2] Eta_rte,
-			 np.ndarray[float, ndim=2] Eps_shp, np.ndarray[float, ndim=2] Eps_rte,
-			 np.ndarray[float, ndim=2] Omega_shp, np.ndarray[float, ndim=2] Omega_rte,
-			 np.ndarray[float, ndim=2] Kappa_shp, np.ndarray[float, ndim=2] Kappa_rte,
-			 np.ndarray[float, ndim=2] Theta, np.ndarray[float, ndim=2] Eta,
-			 np.ndarray[float, ndim=2] Eps, np.ndarray[float, ndim=2] Omega,
+def fit_ctpf(np.ndarray[real_t, ndim=2] Theta_shp, np.ndarray[real_t, ndim=2] Theta_rte,
+			 np.ndarray[real_t, ndim=2] Beta_shp, np.ndarray[real_t, ndim=2] Beta_rte,
+			 np.ndarray[real_t, ndim=2] Eta_shp, np.ndarray[real_t, ndim=2] Eta_rte,
+			 np.ndarray[real_t, ndim=2] Eps_shp, np.ndarray[real_t, ndim=2] Eps_rte,
+			 np.ndarray[real_t, ndim=2] Omega_shp, np.ndarray[real_t, ndim=2] Omega_rte,
+			 np.ndarray[real_t, ndim=2] Kappa_shp, np.ndarray[real_t, ndim=2] Kappa_rte,
+			 np.ndarray[real_t, ndim=2] Theta, np.ndarray[real_t, ndim=2] Eta,
+			 np.ndarray[real_t, ndim=2] Eps, np.ndarray[real_t, ndim=2] Omega,
 			 user_df, has_user_df,
 			 df, W, ind_type k, step_size, has_step_size, int sum_exp_trick,
-			 float a, float b, float c, float d, float e, float f, float g, float h,
+			 real_t a, real_t b, real_t c, real_t d, real_t e, real_t f, real_t g, real_t h,
 			 int nthreads, int maxiter, int miniter, int check_every,
 			 stop_crit, stop_thr, verbose, save_folder,
 			 int allow_inconsistent, int has_valset, int full_llk,
 			 val_df
 			 ):
 	# TODO: implement stochastic variational inference taking CSR data and small Z-X-Y matrices (take from hpfrec)
 	# TODO: for the SVI model with user and item info, alternate between epochs of users and items
 	cdef ind_type nR = df.shape[0]
 	cdef ind_type nW = W.shape[0]
 	cdef ind_type nusers = Eta_shp.shape[0]
 	cdef ind_type nitems = Theta_shp.shape[0]
 	cdef ind_type nwords = Beta_shp.shape[0]
-	cdef np.ndarray[float, ndim=1] Warr = W.Count.values
+	cdef np.ndarray[real_t, ndim=1] Warr = W.Count.values
 	cdef np.ndarray[ind_type, ndim=1] ix_d_w = W.ItemId.values
 	cdef np.ndarray[ind_type, ndim=1] ix_v_w = W.WordId.values
-	cdef np.ndarray[float, ndim=1] Rarr = df.Count.values
+	cdef np.ndarray[real_t, ndim=1] Rarr = df.Count.values
 	cdef np.ndarray[ind_type, ndim=1] ix_u_r = df.UserId.values
 	cdef np.ndarray[ind_type, ndim=1] ix_d_r = df.ItemId.values
 
-	cdef np.ndarray[float, ndim=1] Rval = val_df.Count.values
+	cdef np.ndarray[real_t, ndim=1] Rval = val_df.Count.values
 	cdef np.ndarray[ind_type, ndim=1] ix_u_val = val_df.UserId.values
 	cdef np.ndarray[ind_type, ndim=1] ix_d_val = val_df.ItemId.values
 	cdef ind_type nRv = val_df.shape[0]
 
-	cdef np.ndarray[float, ndim=1] Qarr
+	cdef np.ndarray[real_t, ndim=1] Qarr
 	cdef np.ndarray[ind_type, ndim=1] ix_u_q, ix_a_q
 	cdef ind_type nQ, nattr
 	if has_user_df:
 		Qarr = user_df.Count.values
 		ix_u_q = user_df.UserId.values
 		ix_a_q = user_df.AttributeId.values
 		nQ = user_df.shape[0]
 		nattr = Kappa_shp.shape[0]
 
-	cdef np.ndarray[float, ndim=2] Theta_shp_prev, Theta_rte_prev, Beta_shp_prev, Beta_rte_prev
-	cdef np.ndarray[float, ndim=2] Theta_prev
+	cdef np.ndarray[real_t, ndim=2] Theta_shp_prev, Theta_rte_prev, Beta_shp_prev, Beta_rte_prev
+	cdef np.ndarray[real_t, ndim=2] Theta_prev
 	if stop_crit == 'diff-norm':
 		Theta_prev = Theta.copy()
 	else:
-		Theta_prev = np.empty((0,0), dtype=ctypes.c_float)
+		Theta_prev = np.empty((0,0), dtype=c_real_t)
 	cdef long_double_type last_crit = - LD_HUGE_VAL
 	cdef np.ndarray[long_double_type, ndim=1] errs = np.zeros(2, dtype=obj_long_double_type)
 
 	if verbose>0:
-		print "Allocating intermediate matrices..."
-	cdef np.ndarray[float, ndim=2] Z  = np.empty((nW, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Ya = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yb = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yc, Yd, X
+		print("Allocating intermediate matrices...")
+	cdef np.ndarray[real_t, ndim=2] Z  = np.empty((nW, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Ya = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yb = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yc, Yd, X
 	if has_user_df:
-		Yc = np.empty((nR, k), dtype=ctypes.c_float)
-		Yd = np.empty((nR, k), dtype=ctypes.c_float)
-		X  = np.empty((nQ, k), dtype=ctypes.c_float)
+		Yc = np.empty((nR, k), dtype=c_real_t)
+		Yd = np.empty((nR, k), dtype=c_real_t)
+		X  = np.empty((nQ, k), dtype=c_real_t)
 
 	if verbose>0:
-		print "Initializing optimization procedure..."
+		print("Initializing optimization procedure...")
 	cdef double st_time = time.time()
 
 	for i in range(maxiter):
 
 		## regular model without user side info
 		if not has_user_df:
 			## update Z (phi)
@@ -128,16 +114,16 @@
 				Theta_shp[:,:] = step_size(i) * Theta_shp + (1 - step_size(i)) * Theta_shp_prev
 				Theta_rte[:,:] = (1 - step_size(i))*Theta_rte + step_size(i) * (d + \
 									(Beta_shp/Beta_rte).sum(axis=0, keepdims=True) + \
 									Eta.sum(axis=0, keepdims=True))
 			else:
 				Theta_rte[:,:] = d + (Beta_shp/Beta_rte).sum(axis=0, keepdims=True) + Eta.sum(axis=0, keepdims=True)
 			## FIXME: for some reason, Theta_shp and Theta_rte get wrong results, but can be somehow fixed by adding this:
-			Theta_shp = Theta_shp + np.zeros((Theta_shp.shape[0], Theta_shp.shape[1]), dtype=ctypes.c_float)
-			Theta_rte = Theta_rte + np.zeros((Theta_rte.shape[0], Theta_rte.shape[1]), dtype=ctypes.c_float)
+			Theta_shp = Theta_shp + np.zeros((Theta_shp.shape[0], Theta_shp.shape[1]), dtype=c_real_t)
+			Theta_rte = Theta_rte + np.zeros((Theta_rte.shape[0], Theta_rte.shape[1]), dtype=c_real_t)
 			Theta[:,:] = Theta_shp / Theta_rte
 
 			## update beta
 			if has_step_size:
 				Beta_shp_prev = Beta_shp.copy()
 			Beta_shp[:,:] = a
 			update_Beta_shp(&Beta_shp[0,0], &Z[0,0], &ix_v_w[0], nW, k, nthreads)
@@ -191,16 +177,16 @@
 				Theta_shp[:,:] = step_size(i) * Theta_shp + (1 - step_size(i)) * Theta_shp_prev
 				Theta_rte[:,:] = (1 - step_size(i))*Theta_rte + step_size(i) * (d + \
 									(Beta_shp/Beta_rte).sum(axis=0, keepdims=True) + \
 									(Omega + Eta).sum(axis=0, keepdims=True))
 			else:
 				Theta_rte[:,:] = d + (Beta_shp/Beta_rte).sum(axis=0, keepdims=True) + (Omega + Eta).sum(axis=0, keepdims=True)
 			## FIXME: for some reason, Theta_shp and Theta_rte get wrong results, but can be somehow fixed by adding this:
-			Theta_shp = Theta_shp + np.zeros((Theta_shp.shape[0], Theta_shp.shape[1]), dtype=ctypes.c_float)
-			Theta_rte = Theta_rte + np.zeros((Theta_rte.shape[0], Theta_rte.shape[1]), dtype=ctypes.c_float)
+			Theta_shp = Theta_shp + np.zeros((Theta_shp.shape[0], Theta_shp.shape[1]), dtype=c_real_t)
+			Theta_rte = Theta_rte + np.zeros((Theta_rte.shape[0], Theta_rte.shape[1]), dtype=c_real_t)
 			Theta[:,:] = Theta_shp / Theta_rte
 
 			## Beta_shp := a + sum_i(Z)
 			## Beta_rte := b + sum_i(Theta)
 			if has_step_size:
 				Beta_shp_prev = Beta_shp.copy()
 			Beta_shp[:,:] = a
@@ -214,16 +200,16 @@
 			## Omega_shp := c + sum_a(X) + sum_i(Ya + Yc)
 			## Omega_rte := d + sum_a(Kappa) + sum_i(Theta + Eps)
 			Omega_shp[:,:] = c
 			update_Theta_shp_wuser(&Omega_shp[0,0], &X[0,0], &Ya[0,0], &Yc[0,0],
 						     &ix_u_q[0], &ix_u_r[0], nQ, nR, k, allow_inconsistent, nthreads)
 			Omega_rte[:,:] = d + (Kappa_shp/Kappa_rte).sum(axis=0, keepdims=True) + (Theta + Eps).sum(axis=0, keepdims=True)
 			## FIXME: for some reason, Omega_shp and Omega_rte get wrong results, but can be somehow fixed by adding this:
-			Omega_shp = Omega_shp + np.zeros((Omega_shp.shape[0], Omega_shp.shape[1]), dtype=ctypes.c_float)
-			Omega_rte = Omega_rte + np.zeros((Omega_rte.shape[0], Omega_rte.shape[1]), dtype=ctypes.c_float)
+			Omega_shp = Omega_shp + np.zeros((Omega_shp.shape[0], Omega_shp.shape[1]), dtype=c_real_t)
+			Omega_rte = Omega_rte + np.zeros((Omega_rte.shape[0], Omega_rte.shape[1]), dtype=c_real_t)
 			Omega[:,:] = Omega_shp / Omega_rte
 
 			## Kappa_shp := a + sum_u(X)
 			## Kappa_rte := b + sum_u(Omega)
 			if has_step_size:
 				Kappa_shp_prev = Kappa_shp.copy()
 			Kappa_shp[:,:] = a
@@ -291,27 +277,27 @@
 						Eta_rte, Eps_shp, Eps_rte])
 
 	return i
 
 ### Helpers
 ###########
 def assess_convergence(int i, check_every, stop_crit, last_crit, stop_thr,
-					   np.ndarray[float, ndim=2] Theta, np.ndarray[float, ndim=2] Theta_prev,
-					   np.ndarray[float, ndim=2] Eta, np.ndarray[float, ndim=2] Eps,
+					   np.ndarray[real_t, ndim=2] Theta, np.ndarray[real_t, ndim=2] Theta_prev,
+					   np.ndarray[real_t, ndim=2] Eta, np.ndarray[real_t, ndim=2] Eps,
 					   ind_type nY,
-					   np.ndarray[float, ndim=1] Y, np.ndarray[ind_type, ndim=1] ix_u, np.ndarray[ind_type, ndim=1] ix_i, ind_type nYv,
-					   np.ndarray[float, ndim=1] Yval, np.ndarray[ind_type, ndim=1] ix_u_val, np.ndarray[ind_type, ndim=1] ix_i_val,
+					   np.ndarray[real_t, ndim=1] Y, np.ndarray[ind_type, ndim=1] ix_u, np.ndarray[ind_type, ndim=1] ix_i, ind_type nYv,
+					   np.ndarray[real_t, ndim=1] Yval, np.ndarray[ind_type, ndim=1] ix_u_val, np.ndarray[ind_type, ndim=1] ix_i_val,
 					   np.ndarray[long_double_type, ndim=1] errs, ind_type k, int nthreads, int verbose, int full_llk, has_valset):
 
-	cdef np.ndarray[float, ndim=2] M2
+	cdef np.ndarray[real_t, ndim=2] M2
 
 	if stop_crit == 'diff-norm':
 		last_crit = np.linalg.norm(Theta - Theta_prev)
 		if verbose:
-			cython_loops.print_norm_diff(i+1, check_every, <float> last_crit)
+			cython_loops.print_norm_diff(i+1, check_every, <real_t> last_crit)
 		if last_crit < stop_thr:
 			return True, last_crit
 		Theta_prev[:,:] = Theta.copy()
 
 	else:
 
 		M2 = Theta + Eps
@@ -340,28 +326,28 @@
 				last_crit = errs[0]
 	
 	return False, last_crit
 
 ### Functions for updating without refitting
 ############################################
 def calc_item_factors(W, ind_type nitems, int maxiter, ind_type k, stop_thr, random_seed, int nthreads,
-					  float a, float b, float c, float d,
-					  np.ndarray[float, ndim=2] Theta_rte,
-					  np.ndarray[float, ndim=2] Beta_shp, np.ndarray[float, ndim=2] Beta_rte):
-	cdef np.ndarray[float, ndim=1] Warr = W.Count.values
+					  real_t a, real_t b, real_t c, real_t d,
+					  np.ndarray[real_t, ndim=2] Theta_rte,
+					  np.ndarray[real_t, ndim=2] Beta_shp, np.ndarray[real_t, ndim=2] Beta_rte):
+	cdef np.ndarray[real_t, ndim=1] Warr = W.Count.values
 	cdef np.ndarray[ind_type, ndim=1] ix_i_w = W.ItemId.values
 	cdef np.ndarray[ind_type, ndim=1] ix_v_w = W.WordId.values
 	cdef ind_type nW = W.shape[0]
 
 	rng = np.random.default_rng(seed = random_seed if random_seed > 0 else None)
 
-	cdef np.ndarray[float, ndim=2] Theta_shp = (a * 2*rng.beta(20, 20, size=(nitems, k))).astype(ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Theta_prev = Theta_shp.copy()
-	cdef np.ndarray[float, ndim=2] Z = np.empty((nW, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Zconst = np.empty((nW, k), dtype=ctypes.c_float)
+	cdef np.ndarray[real_t, ndim=2] Theta_shp = (a * 2*rng.beta(20, 20, size=(nitems, k))).astype(c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Theta_prev = Theta_shp.copy()
+	cdef np.ndarray[real_t, ndim=2] Z = np.empty((nW, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Zconst = np.empty((nW, k), dtype=c_real_t)
 	update_Z_const_pred(&Zconst[0,0], &Theta_rte[0,0], &Beta_shp[0,0], &Beta_rte[0,0],
 						&ix_i_w[0], &ix_v_w[0], nW, k, nthreads)
 
 	for i in range(maxiter):
 		update_Z_var_pred(&Z[0,0], &Zconst[0,0], &Warr[0], &Theta_shp[0,0], &ix_i_w[0],
 						  nW, k, nthreads)
 		Theta_shp[:,:] = c
@@ -372,29 +358,29 @@
 			break
 		else:
 			Theta_prev[:,:] = Theta_shp.copy()
 
 	return Theta_shp, Z
 
 def calc_user_factors(df, ind_type nusers, int maxiter, ind_type k, stop_thr, random_seed, int nthreads,
-					  float e, np.ndarray[float, ndim=2] Eta_rte,
-					  np.ndarray[float, ndim=2] Theta_shp, np.ndarray[float, ndim=2] Theta_rte,
-					  np.ndarray[float, ndim=2] Eps_shp, np.ndarray[float, ndim=2] Eps_rte):
+					  real_t e, np.ndarray[real_t, ndim=2] Eta_rte,
+					  np.ndarray[real_t, ndim=2] Theta_shp, np.ndarray[real_t, ndim=2] Theta_rte,
+					  np.ndarray[real_t, ndim=2] Eps_shp, np.ndarray[real_t, ndim=2] Eps_rte):
 	cdef ind_type nR = df.shape[0]
-	cdef np.ndarray[float, ndim=1] Rarr = df.Count.values
+	cdef np.ndarray[real_t, ndim=1] Rarr = df.Count.values
 	cdef np.ndarray[ind_type, ndim=1] ix_u_r = df.UserId.values
 	cdef np.ndarray[ind_type, ndim=1] ix_i_r = df.ItemId.values
-	cdef np.ndarray[float, ndim=2] Ya = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Ya_const = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yb = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yb_const = np.empty((nR, k), dtype=ctypes.c_float)
+	cdef np.ndarray[real_t, ndim=2] Ya = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Ya_const = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yb = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yb_const = np.empty((nR, k), dtype=c_real_t)
 
 	rng = np.random.default_rng(seed = random_seed if random_seed > 0 else None)
-	cdef np.ndarray[float, ndim=2] Eta_shp = e * 2*rng.beta(20, 20, size=(nusers, k)).astype(ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Eta_prev = Eta_shp.copy()
+	cdef np.ndarray[real_t, ndim=2] Eta_shp = e * 2*rng.beta(20, 20, size=(nusers, k)).astype(c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Eta_prev = Eta_shp.copy()
 
 	## reusing the same functions for items with different parameters only
 	update_Z_const_pred(&Ya_const[0,0], &Eta_rte[0,0], &Theta_shp[0,0], &Theta_rte[0,0],
 						&ix_u_r[0], &ix_i_r[0], nR, k, nthreads)
 	update_Z_const_pred(&Yb_const[0,0], &Eta_rte[0,0], &Eps_shp[0,0], &Eps_rte[0,0],
 						&ix_u_r[0], &ix_i_r[0], nR, k, nthreads)
 
@@ -411,42 +397,42 @@
 			break
 		else:
 			Eta_prev = Eta_shp.copy()
 
 	return Eta_shp
 
 def calc_user_factors_full(df, user_df, ind_type nusers, int maxiter, ind_type k, stop_thr, random_seed, int nthreads,
-					  float c, float e, np.ndarray[float, ndim=2] Omega_rte, np.ndarray[float, ndim=2] Eta_rte,
-					  np.ndarray[float, ndim=2] Theta_shp, np.ndarray[float, ndim=2] Theta_rte,
-					  np.ndarray[float, ndim=2] Eps_shp, np.ndarray[float, ndim=2] Eps_rte,
-					  np.ndarray[float, ndim=2] Kappa_shp, np.ndarray[float, ndim=2] Kappa_rte):
+					  real_t c, real_t e, np.ndarray[real_t, ndim=2] Omega_rte, np.ndarray[real_t, ndim=2] Eta_rte,
+					  np.ndarray[real_t, ndim=2] Theta_shp, np.ndarray[real_t, ndim=2] Theta_rte,
+					  np.ndarray[real_t, ndim=2] Eps_shp, np.ndarray[real_t, ndim=2] Eps_rte,
+					  np.ndarray[real_t, ndim=2] Kappa_shp, np.ndarray[real_t, ndim=2] Kappa_rte):
 	cdef ind_type nR = df.shape[0]
-	cdef np.ndarray[float, ndim=1] Rarr = df.Count.values
+	cdef np.ndarray[real_t, ndim=1] Rarr = df.Count.values
 	cdef np.ndarray[ind_type, ndim=1] ix_u_r = df.UserId.values
 	cdef np.ndarray[ind_type, ndim=1] ix_i_r = df.ItemId.values
 
-	cdef np.ndarray[float, ndim=2] Ya = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Ya_const = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yb = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yb_const = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yc = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yc_const = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yd = np.empty((nR, k), dtype=ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Yd_const = np.empty((nR, k), dtype=ctypes.c_float)
+	cdef np.ndarray[real_t, ndim=2] Ya = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Ya_const = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yb = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yb_const = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yc = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yc_const = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yd = np.empty((nR, k), dtype=c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Yd_const = np.empty((nR, k), dtype=c_real_t)
 
 	cdef ind_type nQ = user_df.shape[0]
-	cdef np.ndarray[float, ndim=1] Qarr = user_df.Count.values
+	cdef np.ndarray[real_t, ndim=1] Qarr = user_df.Count.values
 	cdef np.ndarray[ind_type, ndim=1] ix_u_q = user_df.UserId.values
 	cdef np.ndarray[ind_type, ndim=1] ix_a_q = user_df.AttributeId.values
-	cdef np.ndarray[float, ndim=2] X = np.empty((nQ, k), dtype=ctypes.c_float)
+	cdef np.ndarray[real_t, ndim=2] X = np.empty((nQ, k), dtype=c_real_t)
 
 	rng = np.random.default_rng(seed = random_seed if random_seed > 0 else None)
-	cdef np.ndarray[float, ndim=2] Eta_shp = e * 2*rng.beta(20, 20, size=(nusers, k)).astype(ctypes.c_float)
-	cdef np.ndarray[float, ndim=2] Eta_prev = Eta_shp.copy()
-	cdef np.ndarray[float, ndim=2] Omega_shp = c * 2*rng.beta(20, 20, size=(nusers, k)).astype(ctypes.c_float)
+	cdef np.ndarray[real_t, ndim=2] Eta_shp = e * 2*rng.beta(20, 20, size=(nusers, k)).astype(c_real_t)
+	cdef np.ndarray[real_t, ndim=2] Eta_prev = Eta_shp.copy()
+	cdef np.ndarray[real_t, ndim=2] Omega_shp = c * 2*rng.beta(20, 20, size=(nusers, k)).astype(c_real_t)
 
 	## reusing the same functions for items with different parameters only
 	update_Z_const_pred(&Ya_const[0,0], &Omega_rte[0,0], &Theta_shp[0,0], &Theta_rte[0,0],
 						&ix_u_r[0], &ix_i_r[0], nR, k, nthreads)
 	update_Z_const_pred(&Yb_const[0,0], &Eta_rte[0,0], &Theta_shp[0,0], &Theta_rte[0,0],
 						&ix_u_r[0], &ix_i_r[0], nR, k, nthreads)
 	update_Z_const_pred(&Yc_const[0,0], &Omega_rte[0,0], &Eps_shp[0,0], &Eps_rte[0,0],
@@ -483,35 +469,35 @@
 
 ### Fast and parallel C functions
 #################################
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Z(float* Z, float* Theta_shp, float* Theta_rte,
-					 float* Beta_shp, float* Beta_rte, float* W,
+cdef void update_Z(real_t* Z, real_t* Theta_shp, real_t* Theta_rte,
+					 real_t* Beta_shp, real_t* Beta_rte, real_t* W,
 					 ind_type* ix_d, ind_type* ix_v, int sum_exp_trick,
 					 ind_type nW, ind_type K, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_z, st_ix_theta, st_ix_beta
-	cdef float sumrow, maxval
+	cdef real_t sumrow, maxval
 
 	if sum_exp_trick:
 		for i in prange(nW, schedule='static', num_threads=nthreads):
 			st_ix_z = i * K
 			st_ix_theta = ix_d[i] * K
 			st_ix_beta = ix_v[i] * K
 			sumrow = 0
-			maxval =  - HUGE_VALF
+			maxval =  - HUGE_VAL_T
 			for k in range(K):
 				Z[st_ix_z + k] = psi(Theta_shp[st_ix_theta + k]) - log(Theta_rte[k]) + psi(Beta_shp[st_ix_beta + k]) - log(Beta_rte[k])
 				if Z[st_ix_z + k] > maxval:
 					maxval = Z[st_ix_z + k]
 			for k in range(K):
-				Z[st_ix_z + k] = expf(Z[st_ix_z + k] - maxval)
+				Z[st_ix_z + k] = exp_t(Z[st_ix_z + k] - maxval)
 				sumrow += Z[st_ix_z + k]
 			for k in range(K):
 				Z[st_ix_z + k] *= W[i] / sumrow
 
 	else:
 		for i in prange(nW, schedule='static', num_threads=nthreads):
 			st_ix_z = i * K
@@ -525,80 +511,80 @@
 				Z[st_ix_z + k] *= W[i] / sumrow
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Z_const_pred(float* Z, float* Theta_rte, float* Beta_shp, float* Beta_rte,
+cdef void update_Z_const_pred(real_t* Z, real_t* Theta_rte, real_t* Beta_shp, real_t* Beta_rte,
 							  ind_type* ix_d, ind_type* ix_v, ind_type nW, ind_type K, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_z, st_ix_beta
 
 	for i in prange(nW, schedule='static', num_threads=nthreads):
 		st_ix_z = i * K
 		st_ix_beta = ix_v[i] * K
 		for k in range(K):
 			Z[st_ix_z + k] = - log(Theta_rte[k]) + psi(Beta_shp[st_ix_beta + k]) - log(Beta_rte[k])
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Z_var_pred(float* Z, float* Zconst, float* W, float* Theta_shp, ind_type* ix_d,
+cdef void update_Z_var_pred(real_t* Z, real_t* Zconst, real_t* W, real_t* Theta_shp, ind_type* ix_d,
 							ind_type nW, ind_type K, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_z, st_ix_theta
-	cdef float sumrow, maxval
+	cdef real_t sumrow, maxval
 
 	for i in prange(nW, schedule='static', num_threads=nthreads):
 		st_ix_z = i * K
 		st_ix_theta = ix_d[i] * K
 		sumrow = 0
-		maxval = - HUGE_VALF
+		maxval = - HUGE_VAL_T
 		for k in range(K):
 			Z[st_ix_z + k] = Theta_shp[st_ix_theta + k] + Zconst[st_ix_z + k]
 			if Z[st_ix_z + k] > maxval:
 				maxval = Z[st_ix_z + k]
 		for k in range(K):
-			Z[st_ix_z + k] = expf(Z[st_ix_z + k] - maxval)
+			Z[st_ix_z + k] = exp_t(Z[st_ix_z + k] - maxval)
 			sumrow += Z[st_ix_z + k]
 		for k in range(K):
 			Z[st_ix_z + k] *= W[i] / sumrow
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Y(float* Ya, float* Yb, float* Eta_shp, float* Eta_rte, float* Theta_shp, float* Theta_rte,
-				   float* Eps_shp, float* Eps_rte, float* R, ind_type* ix_u_r, ind_type* ix_d_r, int sum_exp_trick,
+cdef void update_Y(real_t* Ya, real_t* Yb, real_t* Eta_shp, real_t* Eta_rte, real_t* Theta_shp, real_t* Theta_rte,
+				   real_t* Eps_shp, real_t* Eps_rte, real_t* R, ind_type* ix_u_r, ind_type* ix_d_r, int sum_exp_trick,
 				   ind_type nR, ind_type K, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_y, st_ix_u, st_ix_d, ix_2
-	cdef float E_eta, sumrow, maxval
+	cdef real_t E_eta, sumrow, maxval
 
 	if sum_exp_trick:
 		for i in prange(nR, schedule='static', num_threads=nthreads):
 			st_ix_u = ix_u_r[i] * K
 			st_ix_d = ix_d_r[i] * K
 			st_ix_y = i * K
 			sumrow = 0
-			maxval = - HUGE_VALF
+			maxval = - HUGE_VAL_T
 			for k in range(K):
 				E_eta = psi(Eta_shp[st_ix_u + k]) - log(Eta_rte[k])
 				ix_2 = st_ix_d + k
 				Ya[st_ix_y + k] = E_eta + psi(Theta_shp[ix_2]) - log(Theta_rte[k])
 				Yb[st_ix_y + k] = E_eta + psi(Eps_shp[ix_2]) - log(Eps_rte[k])
 				if Ya[st_ix_y + k] > maxval:
 					maxval = Ya[st_ix_y + k]
 				if Yb[st_ix_y + k] > maxval:
 					maxval = Yb[st_ix_y + k]
 			for k in range(K):
-				Ya[st_ix_y + k] = expf(Ya[st_ix_y + k] - maxval)
-				Yb[st_ix_y + k] = expf(Yb[st_ix_y + k] - maxval)
+				Ya[st_ix_y + k] = exp_t(Ya[st_ix_y + k] - maxval)
+				Yb[st_ix_y + k] = exp_t(Yb[st_ix_y + k] - maxval)
 				sumrow += Ya[st_ix_y + k] + Yb[st_ix_y + k]
 			for k in range(K):
 				Ya[st_ix_y + k] *= R[i] / sumrow
 				Yb[st_ix_y + k] *= R[i] / sumrow
 
 	else:
 
@@ -618,54 +604,54 @@
 				Yb[st_ix_y + k] *= R[i] / sumrow
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Y_csr(float* Ya, float* Yb, float* Eta_shp, float* Eta_rte,
-					   float* Theta_shp, float* Theta_rte, float* Eps_shp, float* Eps_rte,
-					   float* R, ind_type* ix_u_r, ind_type* docs_batch, ind_type* st_ix_doc,
+cdef void update_Y_csr(real_t* Ya, real_t* Yb, real_t* Eta_shp, real_t* Eta_rte,
+					   real_t* Theta_shp, real_t* Theta_rte, real_t* Eps_shp, real_t* Eps_rte,
+					   real_t* R, ind_type* ix_u_r, ind_type* docs_batch, ind_type* st_ix_doc,
 					   ind_type ndocs, ind_type K, int nthreads) nogil:
 	cdef ind_type d, did, nobs, i, k
 	cdef ind_type st_ix_y, st_ix_u, st_ix_d, ix_2
-	cdef float E_eta, sumrow, maxval
+	cdef real_t E_eta, sumrow, maxval
 
 	## comment: using schedule='dynamic' results in NA values
 	for d in prange(ndocs, schedule='static', num_threads=nthreads):
 		did = docs_batch[d]
 		nobs = st_ix_doc[did + 1] - st_ix_doc[did]
 		st_ix_d = did * K
 		for i in range(nobs):
 			st_ix_u = ix_u_r[i + st_ix_doc[did]] * K
 			st_ix_y = i * K
 			sumrow = 0
-			maxval = - HUGE_VALF
+			maxval = - HUGE_VAL_T
 			for k in range(K):
 				E_eta = psi(Eta_shp[st_ix_u + k]) - log(Eta_rte[k])
 				ix_2 = st_ix_d + k
 				Ya[st_ix_y + k] = E_eta + psi(Theta_shp[ix_2]) - log(Theta_rte[k])
 				Yb[st_ix_y + k] = E_eta + psi(Eps_shp[ix_2]) - log(Eps_rte[k])
 				if Ya[st_ix_y + k] > maxval:
 					maxval = Ya[st_ix_y + k]
 				if Yb[st_ix_y + k] > maxval:
 					maxval = Yb[st_ix_y + k]
 			for k in range(K):
-				Ya[st_ix_y + k] = expf(Ya[st_ix_y + k] - maxval)
-				Yb[st_ix_y + k] = expf(Yb[st_ix_y + k] - maxval)
+				Ya[st_ix_y + k] = exp_t(Ya[st_ix_y + k] - maxval)
+				Yb[st_ix_y + k] = exp_t(Yb[st_ix_y + k] - maxval)
 				sumrow += Ya[st_ix_y + k] + Yb[st_ix_y + k]
 			for k in range(K):
 				Ya[st_ix_y + k] *= R[i] / sumrow
 				Yb[st_ix_y + k] *= R[i] / sumrow
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Theta_shp(float* Theta_shp, float* Z, float* Ya,
+cdef void update_Theta_shp(real_t* Theta_shp, real_t* Z, real_t* Ya,
 						   ind_type* ix_d_w, ind_type* ix_d_r, ind_type nW, ind_type nR, ind_type K,
 						   int allow_inconsistent, int nthreads) nogil:
 	cdef ind_type i, j, k
 	cdef ind_type st_ix_theta, st_ix_z, st_ix_y
 	if allow_inconsistent:
 		for i in prange(nW, schedule='static', num_threads=nthreads):
 			st_ix_theta = ix_d_w[i] * K
@@ -689,15 +675,15 @@
 			for k in range(K):
 				Theta_shp[st_ix_theta + k] += Ya[st_ix_y + k]
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Theta_shp_wuser(float* Theta_shp, float* Z, float* Ya, float* Yb,
+cdef void update_Theta_shp_wuser(real_t* Theta_shp, real_t* Z, real_t* Ya, real_t* Yb,
 						   ind_type* ix_d_w, ind_type* ix_d_r, ind_type nW, ind_type nR, ind_type K,
 						   int allow_inconsistent, int nthreads) nogil:
 	cdef ind_type i, j, k
 	cdef ind_type st_ix_theta, st_ix_z, st_ix_y
 	if allow_inconsistent:
 		for i in prange(nW, schedule='static', num_threads=nthreads):
 			st_ix_theta = ix_d_w[i] * K
@@ -721,56 +707,56 @@
 			for k in range(K):
 				Theta_shp[st_ix_theta + k] += Ya[st_ix_y + k] + Yb[st_ix_y + k]
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Theta_shp_pred(float* Theta_shp, float* Z, ind_type* ix_d,
+cdef void update_Theta_shp_pred(real_t* Theta_shp, real_t* Z, ind_type* ix_d,
 								ind_type nW, ind_type K, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_theta, st_ix_z
 	for i in prange(nW, schedule='static', num_threads=nthreads):
 		st_ix_theta = ix_d[i] * K
 		st_ix_z = i * K
 		for k in range(K):
 			Theta_shp[st_ix_theta + k] += Z[st_ix_z + k]
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Beta_shp(float* Beta_shp, float* Z, ind_type* ix_v, ind_type nW, ind_type K, int nthreads) nogil:
+cdef void update_Beta_shp(real_t* Beta_shp, real_t* Z, ind_type* ix_v, ind_type nW, ind_type K, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_beta, st_ix_Z
 	for i in prange(nW, schedule='static', num_threads=nthreads):
 		st_ix_Z = i * K
 		st_ix_beta = ix_v[i] * K
 		for k in range(K):
 			Beta_shp[st_ix_beta + k] += Z[st_ix_Z + k]
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Eta_shp(float* Eta_shp, float* Ya, float* Yb,
+cdef void update_Eta_shp(real_t* Eta_shp, real_t* Ya, real_t* Yb,
 						 ind_type* ix_u, ind_type nR, ind_type K, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_y, st_ix_eta
 	for i in prange(nR, schedule='static', num_threads=nthreads):
 		st_ix_eta = ix_u[i] * K
 		st_ix_y = i * K
 		for k in range(K):
 			Eta_shp[st_ix_eta + k] += Ya[st_ix_y + k] + Yb[st_ix_y + k]
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void update_Eps_shp(float* Eps_shp, float* Yb, ind_type* ix_d, ind_type nR, ind_type K,
+cdef void update_Eps_shp(real_t* Eps_shp, real_t* Yb, ind_type* ix_d, ind_type nR, ind_type K,
 						 int allow_inconsistent, int nthreads) nogil:
 	cdef ind_type i, k
 	cdef ind_type st_ix_eps, st_ix_y
 	if allow_inconsistent:
 		for i in prange(nR, schedule='static', num_threads=nthreads):
 			st_ix_eps = ix_d[i] * K
 			st_ix_y = i * K
@@ -784,41 +770,41 @@
 				Eps_shp[st_ix_eps + k] += Yb[st_ix_y + k]
 
 ## this function was copy-pasted from hpfrec, thus the variable names
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
 @cython.cdivision(True)
-cdef void llk_plus_rmse(float* T, float* B, float* Y,
+cdef void llk_plus_rmse(real_t* T, real_t* B, real_t* Y,
 						ind_type* ix_u, ind_type* ix_i, ind_type nY, ind_type kszt,
 						long_double_type* out, int nthreads, int add_mse, int full_llk) nogil:
 	cdef ind_type i
 	cdef int one = 1
-	cdef float yhat
+	cdef real_t yhat
 	cdef long_double_type out1 = 0
 	cdef long_double_type out2 =  0
 	cdef int k = <int> kszt
 	if add_mse:
 		if full_llk:
 			for i in prange(nY, schedule='static', num_threads=nthreads):
-				yhat = sdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one)
+				yhat = tdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one)
 				out1 += Y[i]*log(yhat) - loggamma(Y[i] + 1)
 				out2 += (Y[i] - yhat)**2
 		else:
 			for i in prange(nY, schedule='static', num_threads=nthreads):
-				yhat = sdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one)
-				out1 += Y[i]*logf(yhat)
+				yhat = tdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one)
+				out1 += Y[i]*log_t(yhat)
 				out2 += (Y[i] - yhat)**2
 		out[0] = out1
 		out[1] = out2
 	else:
 		if full_llk:
 			for i in prange(nY, schedule='static', num_threads=nthreads):
-				out1 += Y[i]*log(sdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one)) - loggamma(Y[i] + 1)
+				out1 += Y[i]*log(tdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one)) - loggamma(Y[i] + 1)
 			out[0] = out1
 		else:
 			for i in prange(nY, schedule='static', num_threads=nthreads):
-				out1 += Y[i]*logf(sdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one))
+				out1 += Y[i]*log_t(tdot(&k, &T[ix_u[i] * kszt], &one, &B[ix_i[i] * kszt], &one))
 			out[0] = out1
 	### Comment: adding += directly to *out triggers compiler optimizations that produce
 	### different (and wrong) results across different runs.
```

### Comparing `ctpfrec-0.1.8/setup.py` & `ctpfrec-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,22 @@
     install_requires=[
      'pandas>=0.24',
      'numpy>=1.17',
      'scipy',
      'cython',
      'hpfrec>=0.2.3'
 ],
-    version = '0.1.8',
+    version = '0.1.9',
     description = 'Collaborative topic Poisson factorization for recommender systems',
     author = 'David Cortes',
     author_email = 'david.cortes.rivera@gmail.com',
     url = 'https://github.com/david-cortes/ctpfrec',
     keywords = ['collaborative', 'topic', 'modeling', 'poisson', 'probabilistic', 'non-negative', 'factorization',
                             'variational inference', 'collaborative filtering', 'cold-start'],
     classifiers = [],
 
     cmdclass = {'build_ext': build_ext_subclass},
-    ext_modules = [Extension("ctpfrec.cy", sources=["ctpfrec/cy.pyx"], include_dirs=[numpy.get_include()]),
+    ext_modules = [
+      Extension("ctpfrec.cy_double", sources=["ctpfrec/cy_double.pyx"], include_dirs=[numpy.get_include()]),
+      Extension("ctpfrec.cy_float", sources=["ctpfrec/cy_float.pyx"], include_dirs=[numpy.get_include()])
         ]
 )
```

