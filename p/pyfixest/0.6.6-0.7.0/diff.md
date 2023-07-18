# Comparing `tmp/pyfixest-0.6.6.tar.gz` & `tmp/pyfixest-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.6.6.tar", max compression
+gzip compressed data, was "pyfixest-0.7.0.tar", max compression
```

## Comparing `pyfixest-0.6.6.tar` & `pyfixest-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.6.6/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.6.6/pyfixest/__init__.py
--rw-r--r--   0        0        0     4330 2023-06-22 18:59:48.885238 pyfixest-0.6.6/pyfixest/demean.py
--rw-r--r--   0        0        0    21004 2023-07-06 20:11:17.320736 pyfixest-0.6.6/pyfixest/feols.py
--rw-r--r--   0        0        0    45465 2023-06-22 18:59:48.886235 pyfixest-0.6.6/pyfixest/fixest.py
--rw-r--r--   0        0        0    20302 2023-06-04 20:23:08.754381 pyfixest-0.6.6/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.6.6/pyfixest/ssc_utils.py
--rw-r--r--   0        0        0     1312 2023-06-04 20:23:04.808444 pyfixest-0.6.6/pyfixest/utils.py
--rw-r--r--   0        0        0      939 2023-07-06 20:17:01.934736 pyfixest-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     2617 2023-06-04 20:23:08.766777 pyfixest-0.6.6/readme.md
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 pyfixest-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.7.0/pyfixest/__init__.py
+-rw-r--r--   0        0        0     4450 2023-07-14 20:18:32.655093 pyfixest-0.7.0/pyfixest/demean.py
+-rw-r--r--   0        0        0      669 2023-07-18 09:46:04.593817 pyfixest-0.7.0/pyfixest/exceptions.py
+-rw-r--r--   0        0        0    23413 2023-07-18 10:38:25.626648 pyfixest-0.7.0/pyfixest/feols.py
+-rw-r--r--   0        0        0    43168 2023-07-18 10:29:24.099434 pyfixest-0.7.0/pyfixest/fixest.py
+-rw-r--r--   0        0        0    17641 2023-07-18 10:25:33.991093 pyfixest-0.7.0/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.7.0/pyfixest/ssc_utils.py
+-rw-r--r--   0        0        0     1312 2023-06-04 20:23:04.808444 pyfixest-0.7.0/pyfixest/utils.py
+-rw-r--r--   0        0        0      939 2023-07-18 10:39:16.952418 pyfixest-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2617 2023-06-04 20:23:08.766777 pyfixest-0.7.0/readme.md
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 pyfixest-0.7.0/PKG-INFO
```

### Comparing `pyfixest-0.6.6/LICENSE.md` & `pyfixest-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.6.6/pyfixest/demean.py` & `pyfixest-0.7.0/pyfixest/demean.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,117 @@
 import numpy as np
 import scipy.sparse as sp
-from numba import njit, prange
+from numba import njit, prange, types, typed, float64, int64
 from formulaic import model_matrix
 
+#@njit(float64[:](float64[:], int64[:], float64[:]))
+@njit
+def _ave3(x, f, w):
+
+    N = len(x)
+
+    #wx_dict = {}
+    #w_dict = {}
+
+    wx_dict = typed.Dict.empty(key_type=types.int64, value_type=types.float64)
+    w_dict = typed.Dict.empty(key_type=types.int64, value_type=types.float64)
+
+    # Compute weighted sums using a dictionary
+    for i in range(N):
+        j = f[i]
+        if j in wx_dict:
+            wx_dict[j] += w[i] * x[i]
+        else:
+            wx_dict[j] = w[i] * x[i]
 
+        if j in w_dict:
+            w_dict[j] += w[i]
+        else:
+            w_dict[j] = w[i]
 
-@njit(parallel = True, cache = False, fastmath = False)
-def demean(cx, flist, weights, tol = 1e-08, maxiter = 2000):
+    wxw_vec = np.zeros_like(f, dtype=x.dtype)
+
+    for i in range(N):
+        j = f[i]
+        wxw_vec[i] = wx_dict[j] / w_dict[j]
+
+    return wxw_vec
+
+
+#@njit(float64[:,:](float64[:,:], int64[:,:], float64[:,:], float64, int64))
+@njit(parallel = True)
+def demean(cx, fmat, weights, tol = 1e-08, maxiter = 2000):
 
     '''
-    Demean a Matrix cx by fixed effects in flist.
+    Demean a Matrix cx by fixed effects in fmat.
     The fixed effects are weighted by weights. Convervence tolerance
     is set to 1e-08 for the sum of absolute differences.
     Args:
-        cx: Matrix to be demeaned
-        flist: Matrix of fixed effects
+        x: Matrix to be demeaned
+        fmat: Matrix of fixed effects
         weights: Weights for fixed effects
         tol: Convergence tolerance. 1e-08 by default.
     Returns
         res: Demeaned matrix of dimension cx.shape
     '''
-    N = cx.shape[0]
-    fixef_vars = flist.shape[1]
-    K = cx.shape[1]
 
-    res = np.zeros((N,K))
+    #cx = x.copy()
 
+    fixef_vars = fmat.shape[1]
+    K = cx.shape[1]
+
+    res = np.zeros_like(cx)
 
     for k in prange(K):
 
         cxk = cx[:,k].copy()
         oldxk = cxk - 1
 
-        converged = False
-        for _ in range(maxiter):
+        # initiate
+        weighted_ave = np.empty_like(cxk)
+        fvec = np.empty_like(cxk)
 
-            oldxk = cxk.copy()
+        for _ in range(maxiter):
 
             for i in range(fixef_vars):
-                fmat = flist[:,i]
-                weighted_ave = _ave3(cxk, fmat, weights)
-                cxk = cxk - weighted_ave
+                fvec = fmat[:,i]
+                weighted_ave[:] = _ave3(cxk, fvec, weights)
+                cxk -= weighted_ave
 
-            if np.sum(np.abs(cxk - oldxk)) < tol:
-                converged = True
+            if (np.abs(cxk - oldxk)).max() < tol:
                 break
 
+            oldxk = cxk.copy()
+
+
         res[:,k] = cxk
 
     return res
 
 
+@njit
+def _ave2(x, f, w):
+
+    N =  len(x)
+    weighted_ave = np.zeros(N)
+    uvals = _unique2(f)
+
+    for j in uvals:
+        selector = f == j
+        cxkj = x[selector]
+        wj = w[selector]
+        wsum = np.zeros(1)
+        wx = np.zeros(1)
+        for l in range(len(cxkj)):
+            wsum += wj[l]
+            wx += wj[l] * cxkj[l]
+        weighted_ave[selector] = wx / wsum
+
+    return weighted_ave
+
 
 @njit
 def _unique2(x):
     '''
     Returns the unique values of a numpy array as a list
     Args:
         A numpy array.
@@ -87,73 +144,14 @@
     for j in range(len(wxw)):
         selector = f == j
         wxw_long[selector] = wxw[j]
 
     return wxw_long
 
 
-from numba import njit, prange
-from numba.typed import Dict
-
-@njit
-def _ave3(x, f, w):
-
-    N = len(x)
-
-    wx_dict = {}
-    w_dict = {}
-
-    # Compute weighted sums using a dictionary
-    for i in range(N):
-        j = f[i]
-        if j in wx_dict:
-            wx_dict[j] += w[i] * x[i]
-        else:
-            wx_dict[j] = w[i] * x[i]
-
-        if j in w_dict:
-            w_dict[j] += w[i]
-        else:
-            w_dict[j] = w[i]
-
-    # Convert the dictionaries to arrays
-    wx = np.zeros_like(f, dtype=x.dtype)
-    w = np.zeros_like(f, dtype=w.dtype)
-
-    for i in range(N):
-        j = f[i]
-        wx[i] = wx_dict[j]
-        w[i] = w_dict[j]
-
-    # Compute the average
-    wxw_long = wx / w
-
-    return wxw_long
-
-@njit
-def _ave2(x, f, w):
-
-    N =  len(x)
-    weighted_ave = np.zeros(N)
-    uvals = _unique2(f)
-
-    for j in uvals:
-        selector = f == j
-        cxkj = x[selector]
-        wj = w[selector]
-        wsum = np.zeros(1)
-        wx = np.zeros(1)
-        for l in range(len(cxkj)):
-            wsum += wj[l]
-            wx += wj[l] * cxkj[l]
-        weighted_ave[selector] = wx / wsum
-
-    return weighted_ave
-
-
 def getfe(uhat, fe_fml, data):
 
   '''
   Get fixed effects estimates after running a regression on demeaned data.
     Args:
         uhat: Residuals from a regression on demeaned data.
         fe_fml: A one sided formula with the fixed effects.
```

### Comparing `pyfixest-0.6.6/pyfixest/feols.py` & `pyfixest-0.7.0/pyfixest/feols.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 import warnings
 
 from importlib import import_module
 from typing import Union, List, Dict
 from scipy.stats import norm, t
 from pyfixest.ssc_utils import get_ssc
+from pyfixest.exceptions import VcovTypeNotSupportedError, NanInClusterVarError
 
 
 class Feols:
 
     """
     A class for estimating regression models with high-dimensional fixed effects via
     ordinary least squares.
@@ -139,15 +140,17 @@
 
         _check_vcov_input(vcov, self.data)
 
         self.vcov_type, self.vcov_type_detail, self.is_clustered, self.clustervar = _deparse_vcov_input(vcov, self.has_fixef, self.is_iv)
 
         if self.is_iv:
             if self.vcov_type in ["CRV3"]:
-                raise ValueError("CRV3 inference is not supported for IV regressions.")
+                raise VcovTypeNotSupportedError(
+                    "CRV3 inference is not supported for IV regressions."
+                )
 
         # compute vcov
         if self.vcov_type == 'iid':
 
             self.ssc = get_ssc(
                 ssc_dict = self.ssc_dict,
                 N = self.N,
@@ -202,15 +205,18 @@
             cluster_df = self.data[self.clustervar]
             # if there are missings - delete them!
 
             if cluster_df.dtype != "category":
                 cluster_df = pd.Categorical(cluster_df)
 
             if cluster_df.isna().any():
-                raise ValueError("CRV inference not supported with missing values in the cluster variable. Please drop missing values before running the regression.")
+                raise NanInClusterVarError(
+                    "CRV inference not supported with missing values in the cluster variable."
+                    "Please drop missing values before running the regression."
+                )
 
             _, clustid = pd.factorize(cluster_df)
 
             self.G = len(clustid)
 
             self.ssc = get_ssc(
                 ssc_dict = self.ssc_dict,
@@ -247,15 +253,17 @@
                 # if not, either error or turn fixefs into dummies
                 # for now: don't allow for use with fixed effects
 
                 #if self.has_fixef:
                 #    raise ValueError("CRV3 inference is currently not supported with fixed effects.")
 
                 if self.is_iv:
-                    raise ValueError("CRV3 inference is not supported with IV estimation.")
+                    raise VcovTypeNotSupportedError(
+                        "CRV3 inference is not supported with IV estimation."
+                    )
 
                 k_params = self.k
 
                 beta_hat = self.beta_hat
 
                 clusters = clustid
                 n_groups = self.G
@@ -287,15 +295,15 @@
                     Fixest_ = getattr(fixest_module, 'Fixest')
 
                     for ixg, g in enumerate(clusters):
                         # direct leave one cluster out implementation
                         data = self.data[~np.equal(ixg, group)]
                         model = Fixest_(data)
                         model.feols(self.fml, vcov = "iid")
-                        beta_jack[ixg,:] = model.coef()["Estimate"].to_numpy()
+                        beta_jack[ixg,:] = model.coef().to_numpy()
 
 
                 # optional: beta_bar in MNW (2022)
                 #center = "estimate"
                 #if center == 'estimate':
                 #    beta_center = beta_hat
                 #else:
@@ -320,33 +328,33 @@
 
         Returns
         -------
         None
 
         '''
 
-        self.se = (
+        self._se = (
             np.sqrt(np.diagonal(self.vcov))
         )
 
-        self.tstat = (
-            self.beta_hat / self.se
+        self._tstat = (
+            self.beta_hat / self._se
         )
 
         if self.vcov_type in ["iid", "hetero"]:
             df = self.N - self.k
         else:
             df = self.G - 1
-        self.pvalue = (
-            2*(1-t.cdf(np.abs(self.tstat), df))
+        self._pvalue = (
+            2*(1-t.cdf(np.abs(self._tstat), df))
         )
 
         z = norm.ppf(1 - (alpha / 2))
         self.conf_int = (
-            np.array([z * self.se - self.beta_hat, z * self.se + self.beta_hat])
+            np.array([z * self._se - self.beta_hat, z * self._se + self.beta_hat])
         )
 
 
     def get_Ftest(self, vcov, is_iv = False):
 
         '''
         compute an F-test statistic of the form H0: R*beta = q
@@ -396,19 +404,23 @@
 
         try:
             from wildboottest.wildboottest import WildboottestCL, WildboottestHC
         except ImportError:
             print("Module 'wildboottest' not found. Please install 'wildboottest'. Note that it 'wildboottest 'requires Python < 3.11 due to its dependency on 'numba'.")
 
         if self.is_iv:
-            raise ValueError("Wild cluster bootstrap is not supported with IV estimation.")
+            raise VcovTypeNotSupportedError(
+                "Wild cluster bootstrap is not supported with IV estimation."
+            )
         if self.has_fixef:
-            raise ValueError("Wild cluster bootstrap is not supported with fixed effects.")
+            raise VcovTypeNotSupportedError(
+                "Wild cluster bootstrap is not supported with fixed effects."
+            )
 
-        xnames = self.coefnames.to_list()
+        xnames = self.coefnames
         Y = self.Y.flatten()
         X = self.X
 
         # later: allow r <> 0 and custom R
         R = np.zeros(len(xnames))
         R[xnames.index(param)] = 1
         r = 0
@@ -474,14 +486,76 @@
         '''
 
         self.r_squared = 1 - np.sum(self.u_hat ** 2) / \
             np.sum((self.Y - np.mean(self.Y))**2)
         self.adj_r_squared = (self.N - 1) / (self.N - self.k) * self.r_squared
 
 
+    def tidy(self) -> pd.DataFrame:
+
+        '''
+        Return a tidy pd.DataFrame with the point estimates, standard errors, t statistics and p-values.
+        Returns:
+            tidy_df (pd.DataFrame): A tidy pd.DataFrame with the regression results.
+        '''
+
+        tidy_df = pd.DataFrame(
+                    {
+                        'coefnames': self.coefnames,
+                        'Estimate': self.beta_hat,
+                        'Std. Error': self._se,
+                        't value': self._tstat,
+                        'Pr(>|t|)': self._pvalue,
+                        'confint_lower': self.conf_int[0],
+                        'confint_upper': self.conf_int[1]
+                    }
+                )
+
+        return tidy_df.set_index("coefnames")
+
+    def coef(self) -> pd.Series:
+
+        '''
+        Return a pd.Series with estimated regression coefficients.
+        '''
+        return self.tidy()['Estimate']
+
+    def se(self) -> pd.Series:
+        '''
+        Return a pd.Series with standard errors of the estimated regression model.
+        '''
+        return self.tidy()['Std. Error']
+
+    def tstat(self) -> pd.Series:
+        '''
+        Return a pd.Series with t-statistics of the estimated regression model.
+        '''
+        return self.tidy()['t value']
+
+    def pvalue(self) -> pd.Series:
+        '''
+        Return a pd.Series with p-values of the estimated regression model.
+        '''
+        return self.tidy()['Pr(>|t|)']
+
+    def confint(self) -> pd.DataFrame:
+
+        '''
+        Return a pd.DataFrame with confidence intervals for the estimated regression model.
+        '''
+        return self.tidy()[['confint_lower', 'confint_upper']]
+
+
+    def resid(self) -> np.ndarray:
+        '''
+        Returns a one dimensional np.array with the residuals of the estimated regression model.
+        '''
+        return self.u_hat
+
+
 
 def _check_vcov_input(vcov, data):
 
     '''
     Check the input for the vcov argument in the Feols class.
     Args:
         vcov (dict, str, list): The vcov argument passed to the Feols class.
@@ -532,17 +606,21 @@
         vcov_type = "iid"
         is_clustered = False
     elif vcov_type_detail in ["hetero", "HC1", "HC2", "HC3"]:
         vcov_type = "hetero"
         is_clustered = False
         if vcov_type_detail in ["HC2", "HC3"]:
             if has_fixef:
-                raise ValueError("HC2 and HC3 inference types are not supported for regressions with fixed effects.")
+                raise VcovTypeNotSupportedError(
+                    "HC2 and HC3 inference types are not supported for regressions with fixed effects."
+                )
             if is_iv:
-                raise ValueError("HC2 and HC3 inference types are not supported for IV regressions.")
+                raise VcovTypeNotSupportedError(
+                    "HC2 and HC3 inference types are not supported for IV regressions."
+                )
     elif vcov_type_detail in ["CRV1", "CRV3"]:
         vcov_type = "CRV"
         is_clustered = True
 
     if is_clustered:
         clustervar = list(vcov.values())[0]
     else:
@@ -572,7 +650,10 @@
 
     if X.ndim != 2:
         raise ValueError("X must be a 2D array")
     if Z.ndim != 2:
         raise ValueError("Z must be a 2D array")
 
 
+
+
+
```

### Comparing `pyfixest-0.6.6/pyfixest/fixest.py` & `pyfixest-0.7.0/pyfixest/fixest.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,385 +8,30 @@
 from typing import Any, Union, Dict, Optional, List, Tuple
 from scipy.stats import norm
 from formulaic import model_matrix
 
 from pyfixest.feols import Feols
 from pyfixest.FormulaParser import FixestFormulaParser, _flatten_list
 from pyfixest.ssc_utils import ssc
-
-
-class DepvarIsNotNumericError(Exception):
-    pass
+from pyfixest.exceptions import MatrixNotFullRankError, MultiEstNotSupportedError
 
 
 class Fixest:
 
     def __init__(self, data: pd.DataFrame) -> None:
         '''
         A class for fixed effects regression modeling.
         Args:
             data: The input pd.DataFrame for the object.
         Returns:
             None
         '''
 
         self.data = data
-        self.model_res = dict()
-
-    def _clean_fe(self, data, fval):
-
-        fval_list = fval.split("+")
-
-        # find interacted fixed effects via "^"
-        interacted_fes = [x for x in fval_list if len(x.split('^')) > 1]
-            
-        varying_slopes = [x for x in fval_list if len(x.split('/')) > 1]
-
-        for x in interacted_fes:
-            vars = x.split("^")
-            data[x] = data[vars].apply(lambda x: '^'.join(
-                x.dropna().astype(str)) if x.notna().all() else np.nan, axis=1)
-        
-        fe = data[fval_list]
-        # all fes to factors / categories
-
-        if varying_slopes != []: 
-          
-            for x in varying_slopes: 
-                mm_vs = model_matrix("-1 + " + x, data)
-            
-            fe = pd.concat([fe, mm_vs], axis = 1)
-        
-        fe_na = fe.isna().any(axis=1)
-        fe = fe.apply(lambda x: pd.factorize(x)[0])
-        fe = fe.to_numpy()
-
-        return fe, fe_na
-
-    def _demean_model(self, data: pd.DataFrame, fval: str, ivars: List[str], drop_ref: str) -> None:
-        '''
-        Demean all regressions for a specification of fixed effects.
-
-        Args:
-            data: The input pd.DataFrame for the object. Either self.data or a subset thereof (for split sample estimation).
-            fval: A specification of fixed effects. A string indicating the fixed effects to be demeaned,
-                such as "X4" or "X3 + X2".
-            ivars: A list of strings indicating the interacted variables via i().
-            drop_ref: A string indicating the reference category for the interacted variables. The reference
-                      category is dropped from the regression.
-
-        Returns:
-            None
-        '''
-
-        YXZ_dict = dict()
-        na_dict = dict()
-        var_dict = dict()
-
-        if fval != "0":
-            fe, fe_na = self._clean_fe(data, fval)
-            fe_na = list(fe_na[fe_na == True])
-        else:
-            fe = None
-            fe_na = None
-
-        dict2fe = self.fml_dict2.get(fval)
-        if self.is_iv:
-            dict2fe_iv = self.fml_dict2_iv.get(fval)
-
-        # create lookup table with NA index key
-        # for each regression, check if lookup table already
-        # populated with "demeaned" data for some (or all)
-        # variables of the model. if demeaned variable for
-        # NA key already exists -> use it. else rerun demeaning
-        # algorithm
-
-        lookup_demeaned_data = dict()
-
-        # loop over both dict2fe and dict2fe_iv (if the latter is not None)
-        for depvar in dict2fe.keys():
-
-            # [(0, 'X1+X2'), (1, ['X1+X3'])]
-            for _, covar in enumerate(dict2fe.get(depvar)):
-
-                covar2 = covar
-                depvar2 = depvar
-
-                fml = depvar2 + " ~ " + covar2
-
-                if self.is_iv:
-                    instruments2 = dict2fe_iv.get(depvar)[0]
-                    endogvar_list = list(set(covar2.split("+")) - set(instruments2.split("+")))#[0]
-                    instrument_list = list(set(instruments2.split("+")) - set(covar2.split("+")))#[0]
-
-                    fml2 = "+".join(instrument_list) + "+" + fml
-
-                else:
-                    fml2 = fml
-
-                lhs, rhs = model_matrix(fml2, data)
-
-                untransformed_depvar = _find_untransformed_depvar(depvar2)
-
-                Y = lhs[[depvar]]
-                X = rhs
-                if self.is_iv:
-                    I = lhs[instrument_list]
-
-                # get NA index before converting Y to numpy array
-                na_index = list(set(data.index) - set(Y.index))
-
-                # drop variables before collecting variable names
-                if self.ivars is not None:
-                    if drop_ref is not None:
-                        X = X.drop(drop_ref, axis=1)
-
-                y_names = list(Y.columns)
-                x_names = list(X.columns)
-                yxz_names = list(y_names) + list(x_names)
-                if self.is_iv:
-                    iv_names = list(I.columns)
-                    x_names_copy = x_names.copy()
-                    x_names_copy = [x for x in x_names_copy if x not in endogvar_list]
-                    z_names = x_names_copy + instrument_list
-                    cols = yxz_names + iv_names
-                else:
-                    iv_names = None
-                    z_names = None
-                    cols = yxz_names
-
-                if self.ivars is not None:
-                    self.icovars = [s for s in x_names if s.startswith(
-                        ivars[0]) and s.endswith(ivars[1])]
-                else:
-                    self.icovars = None
-
-
-                Y = Y.to_numpy()
-                X = X.to_numpy()
-                if self.is_iv:
-                    I = I.to_numpy()
-
-                if Y.shape[1] > 1:
-                    raise ValueError(
-                        "Dependent variable must be a single column. Please make sure that the dependent variable" + depvar2 + "is of a numeric type (int or float).")
-
-                # variant 1: if there are fixed effects to be projected out
-                if fe is not None:
-                    na_index = (na_index + fe_na)
-                    fe2 = np.delete(fe, na_index, axis=0)
-                    # drop intercept
-                    intercept_index = x_names.index("Intercept")
-                    X = np.delete(X, intercept_index, axis = 1)
-                    x_names.remove("Intercept")
-                    yxz_names.remove("Intercept")
-                    if self.is_iv:
-                        z_names.remove("Intercept")
-                        cols.remove("Intercept")
-
-                    # check if variables have already been demeaned
-                    Y = np.delete(Y, fe_na, axis=0)
-                    X = np.delete(X, fe_na, axis=0)
-                    if self.is_iv:
-                        I = np.delete(I, fe_na, axis=0)
-
-                    if self.is_iv:
-                        YXZ = np.concatenate([Y, X, I], axis = 1)
-                    else:
-                        YXZ = np.concatenate([Y, X], axis=1)
-
-                    na_index_str = ','.join(str(x) for x in na_index)
-
-                    # check if looked dict has data for na_index
-                    if lookup_demeaned_data.get(na_index_str) is not None:
-                        # get data out of lookup table: list of [algo, data]
-                        algorithm, YXZ_demeaned_old = lookup_demeaned_data.get(
-                            na_index_str)
-
-                        # get not yet demeaned covariates
-                        var_diff_names = list(
-                            set(yxz_names) - set(YXZ_demeaned_old.columns))[0]
-                        var_diff_index = list(yxz_names).index(var_diff_names)
-                        var_diff = YXZ[:, var_diff_index]
-                        if var_diff.ndim == 1:
-                            var_diff = var_diff.reshape(len(var_diff), 1)
-
-                        YXZ_demean_new = algorithm.residualize(var_diff)
-                        YXZ_demeaned = np.concatenate(
-                            [YXZ_demeaned_old, YXZ_demean_new], axis=1)
-                        YXZ_demeaned = pd.DataFrame(YXZ_demeaned)
-
-                        YXZ_demeaned.columns = list(
-                            YXZ_demeaned_old.columns) + [var_diff_names]
-
-                    else:
-                        # not data demeaned yet for NA combination
-                        algorithm = pyhdfe.create(
-                            ids=fe2,
-                            residualize_method='map',
-                            drop_singletons=self.drop_singletons,
-                        )
-
-                        if self.drop_singletons == True and algorithm.singletons != 0 and algorithm.singletons is not None:
-                            print(algorithm.singletons, "columns are dropped due to singleton fixed effects.")
-                            dropped_singleton_indices = (
-                                np.where(algorithm._singleton_indices))[0].tolist()
-                            na_index += dropped_singleton_indices
-
-                        YXZ_demeaned = algorithm.residualize(YXZ)
-                        YXZ_demeaned = pd.DataFrame(YXZ_demeaned)
-
-                        YXZ_demeaned.columns = cols
-
-                    lookup_demeaned_data[na_index_str] = [
-                        algorithm, YXZ_demeaned]
-
-                else:
-                    # if no fixed effects
-                    if self.is_iv:
-                        YXZ = np.concatenate([Y, X, I], axis=1)
-                    else:
-                        YXZ = np.concatenate([Y, X], axis=1)
-
-                    YXZ_demeaned = pd.DataFrame(YXZ)
-
-                    YXZ_demeaned.columns = cols
-
-                YXZ_dict[fml] = YXZ_demeaned
-                na_dict[fml] = na_index
-                var_dict[fml] = dict({
-                    'y_names': y_names,
-                    'x_names': x_names,
-                    'iv_names': iv_names,
-                    'z_names': z_names
-                })
-
-
-        return YXZ_dict, na_dict, var_dict
-
-    def _demean_all_models(self, fixef_keys, ivars, drop_ref, estimate_full_model, estimate_split_model):
-
-        '''
-        demean multiple models. essentially, the function loops
-        over all split var and fixed effects variables and demeans the
-        specified dependend variables and covariates
-        Args:
-            fixef_keys: fixed effect variables
-            ivars: interaction variables
-            drop_ref: drop reference category
-            estimate_full_model: boolean, whether to estimate the full model
-            estimate_split_model: boolean, whether to estimate the split model
-        '''
-
-        if estimate_full_model:
-            for _, fval in enumerate(fixef_keys):
-                self.demeaned_data_dict[fval] = []
-                self.dropped_data_dict[fval] = []
-                self.yxz_name_dict[fval] = []
-                data = self.data
-                demeaned_data, dropped_data, yxz_name_dict= self._demean_model(
-                    data, fval, ivars, drop_ref)
-                self.demeaned_data_dict[fval].append(demeaned_data)
-                self.dropped_data_dict[fval].append(dropped_data)
-                self.yxz_name_dict[fval].append(yxz_name_dict)
-
-        if estimate_split_model:
-            for _, fval in enumerate(fixef_keys):
-                self.demeaned_data_dict[fval] = []
-                self.dropped_data_dict[fval] = []
-                self.yxz_name_dict[fval] = []
-                for x in self.split_categories:
-                    sub_data = self.data[x == self.splitvar]
-                    demeaned_data, dropped_data, yxz_name_dict = self._demean_model(
-                        sub_data, fval, ivars, drop_ref)
-                    self.demeaned_data_dict[fval].append(demeaned_data)
-                    self.dropped_data_dict[fval].append(dropped_data)
-                    self.yxz_name_dict[fval].append(yxz_name_dict)
-
-    def _estimate_all_models(self, vcov):
-
-        # estimate models based on demeaned model matrix and dependent variables
-        for _, fval in enumerate(self.fml_dict.keys()):
-            model_splits = self.demeaned_data_dict[fval]
-            for x, _ in enumerate(model_splits):
-                model_frames = model_splits[x]
-                for _, fml in enumerate(model_frames):
-
-                    # get the (demeaned) model frame. key is fml without fixed effects
-                    model_frame = model_frames[fml]
-
-                    # update formula with fixed effect. fval is "0" for no fixed effect
-                    if fval == "0":
-                        fml2 = fml
-                    else:
-                        fml2 = fml + "|" + fval
-
-                    # formula log: add information on sample split
-                    if self.splitvar is not None:
-                        split_log = str(self.split_categories[x])
-                        full_fml = fml2 + "| split =" + split_log
-                    else:
-                        split_log = None
-                        full_fml = fml2
-
-                    name_dict = self.yxz_name_dict[fval][0][fml]
-                    depvar_name = name_dict["y_names"]
-                    xvar_names = name_dict["x_names"]
-                    if name_dict["z_names"] is None:
-                        zvar_names = name_dict["x_names"]
-                    else:
-                        zvar_names = name_dict["z_names"]
-
-                    Y = model_frame[depvar_name]
-                    X = model_frame[xvar_names]
-                    Z = model_frame[zvar_names]
-
-                    colnames = X.columns
-                    zcolnames = Z.columns
-
-                    Y = Y.to_numpy()
-                    X = X.to_numpy()
-                    Z = Z.to_numpy()
-
-                    N = X.shape[0]
-                    k = X.shape[1]
-
-                    # check for multicollinearity
-                    _multicollinearity_checks(X, Z, self.ivars, fml2)
-
-                    FEOLS = Feols(Y, X, Z)
-                    FEOLS.is_iv = self.is_iv
-                    FEOLS.fml = fml2
-                    FEOLS.ssc_dict = self.ssc_dict
-                    if self.is_iv:
-                        FEOLS.get_fit(estimator = "2sls")
-                    else:
-                        FEOLS.get_fit(estimator = "ols")
-                    FEOLS.na_index = self.dropped_data_dict[fval][x][fml]
-                    FEOLS.data = self.data.iloc[~self.data.index.isin(
-                        FEOLS.na_index), :]
-                    FEOLS.N = N
-                    FEOLS.k = k
-                    if fval != "0":
-                        FEOLS.has_fixef = True
-                        FEOLS.fixef = fval
-                    else:
-                        FEOLS.has_fixef = False
-
-                    vcov_type = _get_vcov_type(vcov, fval)
-
-                    FEOLS.vcov_log = vcov_type
-                    FEOLS.split_log = x
-                    FEOLS.get_vcov(vcov=vcov_type)
-                    FEOLS.get_inference()
-                    FEOLS.coefnames = colnames
-                    if self.icovars is not None:
-                        FEOLS.icovars = self.icovars
-                    self.model_res[full_fml] = FEOLS
-
+        self.all_fitted_models = dict()
 
 
     def feols(self, fml: str, vcov: Union[None, str, Dict[str, str]] = None, ssc=ssc(), fixef_rm: str = "none") -> None:
         '''
         Method for fixed effects regression modeling using the PyHDFE package for projecting out fixed effects.
         Args:
             fml (str): A three-sided formula string using fixest formula syntax. Supported syntax includes:
@@ -445,96 +90,420 @@
             2. Create a dictionary of formulas for each dependent variable.
             3. demean all models and store the data
             4. fit all models
         '''
 
         self.fml = fml.replace(" ", "")
         self.split = None
+        self.method = "feols"
 
         # deparse formula, at least partially
         fxst_fml = FixestFormulaParser(fml)
 
         if fxst_fml.is_iv:
             self.is_iv = True
         else:
             self.is_iv = False
 
         # add function argument to these methods for IV
-        fxst_fml.get_fml_dict()
-        fxst_fml.get_var_dict()
-        fxst_fml._transform_fml_dict()
-
-        if self.is_iv:
-            # create required dicts for first stage IV regressions
-            fxst_fml.get_fml_dict(iv = True)
-            fxst_fml.get_var_dict(iv = True)
-            fxst_fml._transform_fml_dict(iv = True)
+        fxst_fml.get_new_fml_dict() # fxst_fml.fml_dict_new
 
-
-        self.fml_dict = fxst_fml.fml_dict
-        self.var_dict = fxst_fml.var_dict
-        self.fml_dict2 = fxst_fml.fml_dict2
+        self.fml_dict = fxst_fml.fml_dict_new
 
         if self.is_iv:
-            self.fml_dict_iv = fxst_fml.fml_dict_iv
-            self.var_dict_iv = fxst_fml.var_dict_iv
-            self.fml_dict2_iv = fxst_fml.fml_dict2_iv
+            fxst_fml.get_new_fml_dict(iv = True) # fxst_fml.fml_dict_new
+            self.fml_dict_iv = fxst_fml.fml_dict_new_iv
         else:
-            self.fml_dict_iv = self.fml_dict
-            self.var_dict_iv = self.var_dict
-            self.fml_dict2_iv = self.fml_dict2
+            self.fml_dict_iv = None
 
         self.ivars = fxst_fml.ivars
 
-
         self.ssc_dict = ssc
         self.drop_singletons = _drop_singletons(fixef_rm)
 
         # get all fixed effects combinations
-        fixef_keys = list(self.var_dict.keys())
+        fixef_keys = list(self.fml_dict.keys())
 
-        ivars, drop_ref = _clean_ivars(self.ivars, self.data)
+        self.ivars, self.drop_ref = _clean_ivars(self.ivars, self.data)
 
-        # dropped_data_dict and demeaned_data_dict are
-        # dictionaries with keys for each fixed effects combination and
-        # has values of lists of demeaned dataframes
-        # the list is a singelton list unless split sample estimation is used
-        # e.g it looks like this (without split estimation):
-        # {'fe1': [demeaned_data_df], 'fe1+fe2': [demeaned_data_df]}
-        # and like this (with split estimation):
-        # {'fe1': [demeaned_data_df1, demeaned_data_df2], 'fe1+fe2': [demeaned_data_df1, demeaned_data_df2]}
-        # the lists are sorted in the order of the split variable
-
-        self.dropped_data_dict = dict()
-        self.demeaned_data_dict = dict()
         # names of depvar, X, Z matrices
         self.yxz_name_dict = dict()
 
-        estimate_full_model = True
-        estimate_split_model = False
         # currently no fsplit allowed
         fsplit = None
 
-        self.splitvar, _, estimate_split_model, estimate_full_model = _prepare_split_estimation(self.split, fsplit, self.data, self.var_dict)
+        self.splitvar, _, self.estimate_split_model, self.estimate_full_model = _prepare_split_estimation(self.split, fsplit, self.data, self.fml_dict)
 
         # demean all models: based on fixed effects x split x missing value combinations
-        self._demean_all_models(fixef_keys, ivars, drop_ref, estimate_full_model, estimate_split_model)
+        self._estimate_all_models2(vcov, fixef_keys)
 
         # create self.is_fixef_multi flag
         self._is_multiple_estimation()
 
         if self.is_fixef_multi and self.is_iv:
-            raise ValueError("Multiple Estimations is currently not supported with IV. This is mostly due to insufficient testing and will be possible with the next release of PyFixest.")
-
-        # estimate all regression models based on demeaned data
-        self._estimate_all_models(vcov = vcov)
+            raise MultiEstNotSupportedError(
+                "Multiple Estimations is currently not supported with IV."
+                "This is mostly due to insufficient testing and will be possible with the next release of PyFixest."
+            )
 
         return self
 
 
+    def _clean_fe(self, data, fval):
+
+        '''
+        Function that transform and cleans fixed effects.
+        '''
+
+        fval_list = fval.split("+")
+
+        # find interacted fixed effects via "^"
+        interacted_fes = [x for x in fval_list if len(x.split('^')) > 1]
+
+        varying_slopes = [x for x in fval_list if len(x.split('/')) > 1]
+
+        for x in interacted_fes:
+            vars = x.split("^")
+            data[x] = data[vars].apply(lambda x: '^'.join(
+                x.dropna().astype(str)) if x.notna().all() else np.nan, axis=1)
+
+        fe = data[fval_list]
+        # all fes to factors / categories
+
+        if varying_slopes != []:
+
+            for x in varying_slopes:
+                mm_vs = model_matrix("-1 + " + x, data)
+
+            fe = pd.concat([fe, mm_vs], axis = 1)
+
+        fe_na = fe.isna().any(axis=1)
+        fe = fe.apply(lambda x: pd.factorize(x)[0])
+        fe = fe.to_numpy()
+
+        return fe, fe_na
+
+
+    def _model_matrix_fixest(self, depvar, covar, fval):
+
+        '''
+        Create model matrices for fixed effects estimation. Preprocesses the data and then calls
+        formulaic.model_matrix() to create the model matrices.
+
+        Args:
+            depvar: dependent variable. string. E.g. "Y"
+            covar: covariates. string. E.g. "X1 + X2"
+            fval: fixed effects. string. E.g. "fe1 + fe2". "0" if no fixed effects.
+        Returns:
+            Y: a pd.DataFrame of the dependent variable.
+            X: a pd.DataFrame of the covariates
+            I: a pd.DataFrame of the Instruments. None if no IV.
+            fe: a pd.DataFrame of the fixed effects. None if no fixed effects specified.
+            na_index: a np.array with indices of dropped columns.
+            fe_na: a np.array with indices of dropped columns due to fixed effect singletons / NaNs in the fixed effects
+            na_index_str: na_index, but as a comma separated string. Used for caching of demeaned variables
+            z_names: names of all covariates, minus the endogeneous variables, plus the instruments. None if no IV.
+        '''
+
+        if fval != "0":
+            fe, fe_na = self._clean_fe(self.data, fval)
+            fe_na = list(fe_na[fe_na == True])
+            fe = pd.DataFrame(fe)
+        else:
+            fe = None
+            fe_na = None
+
+        if self.is_iv:
+            dict2fe_iv = self.fml_dict_iv.get(fval)
+
+        covar2 = covar
+        depvar2 = depvar
+
+        fml = depvar2 + " ~ " + covar2
+
+        if self.is_iv:
+            instruments2 = dict2fe_iv.get("Y")[0].split("~")[1]
+            endogvar_list = list(set(covar2.split("+")) - set(instruments2.split("+")))#[0]
+            instrument_list = list(set(instruments2.split("+")) - set(covar2.split("+")))#[0]
+
+            fml2 = "+".join(instrument_list) + "+" + fml
+
+        else:
+            fml2 = fml
+
+        lhs, rhs = model_matrix(fml2, self.data)
+
+        Y = lhs[[depvar]]
+        X = pd.DataFrame(rhs)
+        if self.is_iv:
+            I = lhs[instrument_list]
+            I = pd.DataFrame(I)
+        else:
+            I = None
+
+        # get NA index before converting Y to numpy array
+        na_index = list(set(self.data.index) - set(Y.index))
+
+        # drop variables before collecting variable names
+        if self.ivars is not None:
+            if self.drop_ref is not None:
+                X = X.drop(self.drop_ref, axis=1)
+
+        y_names = list(Y.columns)
+        x_names = list(X.columns)
+        yxz_names = list(y_names) + list(x_names)
+
+        if self.is_iv:
+            iv_names = list(I.columns)
+            x_names_copy = x_names.copy()
+            x_names_copy = [x for x in x_names_copy if x not in endogvar_list]
+            z_names = x_names_copy + instrument_list
+            cols = yxz_names + iv_names
+        else:
+            iv_names = None
+            z_names = None
+            cols = yxz_names
+
+        if self.ivars is not None:
+            self.icovars = [s for s in x_names if s.startswith(
+                self.ivars[0]) and s.endswith(self.ivars[1])]
+        else:
+            self.icovars = None
+
+        if Y.shape[1] > 1:
+            raise ValueError(
+                "Dependent variable must be a single column."
+                "Please make sure that the dependent variable" + depvar2 + "is of a numeric type (int or float)."
+           )
+
+        if fe is not None:
+            na_index = (na_index + fe_na)
+            fe = fe.drop(na_index, axis=0)
+            # drop intercept
+            X = X.drop('Intercept', axis = 1)
+            x_names.remove("Intercept")
+            yxz_names.remove("Intercept")
+            if self.is_iv:
+                z_names.remove("Intercept")
+                cols.remove("Intercept")
+
+            # check if variables have already been demeaned
+            Y = Y.drop(fe_na, axis=0)
+            X = X.drop(fe_na, axis=0)
+            if self.is_iv:
+                I = I.drop(fe_na, axis=0)
+
+        na_index_str = ','.join(str(x) for x in na_index)
+
+        return Y, X, I, fe, na_index, fe_na, na_index_str, z_names
+
+
+    def _demean_model2(self, Y, X, I, fe, lookup_demeaned_data, na_index_str):
+
+        '''
+        Demeans a single regression model. If the model has fixed effects, the fixed effects are demeaned using the PyHDFE package.
+        Prior to demeaning, the function checks if some of the variables have already been demeaned and uses values from the cache
+        `lookup_demeaned_data` if possible. If the model has no fixed effects, the function does not demean the data.
+
+        Args:
+            Y: a pd.DataFrame of the dependent variable.
+            X: a pd.DataFrame of the covariates
+            I: a pd.DataFrame of the Instruments. None if no IV.
+            fe: a pd.DataFrame of the fixed effects. None if no fixed effects specified.
+            lookup_demeaned_data: a dictionary with keys for each fixed effects combination and potentially values of demeaned data.frames.
+                The function checks this dictionary to see if some of the variables have already been demeaned.
+            na_index_str: a string with indices of dropped columns. Used for caching of demeaned variables.
+
+        Returns:
+            Yd: a pd.DataFrame of the demeaned dependent variable.
+            Xd: a pd.DataFrame of the demeaned covariates
+            Id: a pd.DataFrame of the demeaned Instruments. None if no IV.
+        '''
+
+        if I is not None:
+            YXZ = pd.concat([Y, X, I], axis = 1)
+        else:
+            YXZ = pd.concat([Y, X], axis = 1)
+
+        yxz_names = YXZ.columns
+        YXZ = YXZ.to_numpy()
+
+        if fe is not None:
+
+            # check if looked dict has data for na_index
+            if lookup_demeaned_data.get(na_index_str) is not None:
+                # get data out of lookup table: list of [algo, data]
+                algorithm, YXZ_demeaned_old = lookup_demeaned_data.get(na_index_str)
+
+                # get not yet demeaned covariates
+                var_diff_names = list(set(yxz_names) - set(YXZ_demeaned_old.columns))[0]
+                var_diff_index = list(yxz_names).index(var_diff_names)
+                var_diff = YXZ[:, var_diff_index]
+                if var_diff.ndim == 1:
+                    var_diff = var_diff.reshape(len(var_diff), 1)
+
+                YXZ_demean_new = algorithm.residualize(var_diff)
+                YXZ_demeaned = np.concatenate([YXZ_demeaned_old, YXZ_demean_new], axis=1)
+                YXZ_demeaned = pd.DataFrame(YXZ_demeaned)
+
+                YXZ_demeaned.columns = list(YXZ_demeaned_old.columns) + [var_diff_names]
+
+            else:
+
+                # not data demeaned yet for NA combination
+                algorithm = pyhdfe.create(
+                    ids=fe,
+                    residualize_method='map',
+                    drop_singletons=self.drop_singletons,
+                )
+
+                if self.drop_singletons == True and algorithm.singletons != 0 and algorithm.singletons is not None:
+                    print(algorithm.singletons, "columns are dropped due to singleton fixed effects.")
+                    dropped_singleton_indices = np.where(algorithm._singleton_indices)[0].tolist()
+                    na_index += dropped_singleton_indices
+
+                YXZ_demeaned = algorithm.residualize(YXZ)
+                YXZ_demeaned = pd.DataFrame(YXZ_demeaned)
+
+                YXZ_demeaned.columns = yxz_names
+
+            lookup_demeaned_data[na_index_str] = [algorithm, YXZ_demeaned]
+
+        else:
+            # nothing to demean here
+            pass
+
+            YXZ_demeaned = pd.DataFrame(YXZ)
+            YXZ_demeaned.columns = yxz_names
+
+        # get demeaned Y, X, I (if no fixef, equal to Y, X, I)
+        Yd = YXZ_demeaned[Y.columns]
+        Xd = YXZ_demeaned[X.columns]
+        Id = None
+        if I is not None:
+            Id = YXZ_demeaned[I.columns]
+
+
+        return Yd, Xd, Id
+
+
+
+    def _estimate_all_models2(self, vcov, fixef_keys):
+
+        '''
+        demean multiple models. essentially, the function loops
+        over all split var and fixed effects variables and demeans the
+        specified dependend variables and covariates
+        Args:
+            fixef_keys: fixed effect variables
+            ivars: interaction variables
+            drop_ref: drop reference category
+            estimate_full_model: boolean, whether to estimate the full model
+            estimate_split_model: boolean, whether to estimate the split model
+        '''
+
+
+        if self.estimate_full_model:
+
+            for _, fval in enumerate(fixef_keys):
+
+                dict2fe = self.fml_dict.get(fval)
+
+                # dictionary to cache demeaned data with index: na_index_str
+                lookup_demeaned_data = dict()
+
+                # loop over both dictfe and dictfe_iv (if the latter is not None)
+                for depvar in dict2fe.keys():
+
+                    for _, fml_linear in enumerate(dict2fe.get(depvar)):
+
+                        if self.method == "feols":
+
+                            if isinstance(fml_linear, list):
+                                fml_linear = fml_linear[0]
+
+                            covar = fml_linear.split("~")[1]
+
+                            # get Y, X, Z, fe, NA indices for model
+                            Y, X, I, fe, na_index, _, na_index_str, z_names = self._model_matrix_fixest(depvar, covar, fval)
+
+                            y_names = Y.columns.tolist()
+                            x_names = X.columns.tolist()
+
+                            fml = get_fml(y_names, x_names, fval)
+
+                            # demean Y, X, Z, if not already done in previous estimation
+                            Yd, Xd, Id = self._demean_model2(Y, X, I, fe, lookup_demeaned_data, na_index_str)
+                            if self.is_iv:
+                                Zd = pd.concat([Xd, Id], axis = 1)[z_names]
+                            else:
+                                Zd = Xd
+
+                            Yd = Yd.to_numpy()
+                            Xd = Xd.to_numpy()
+                            Zd = Zd.to_numpy()
+
+                            # check for multicollinearity
+                            _multicollinearity_checks(Xd, Zd, self.ivars, fml)
+
+                            # initiate OLS class
+                            FEOLS = Feols(Y = Yd, X = Xd, Z = Zd)
+
+                            # estimation
+                            if self.is_iv:
+                                FEOLS.get_fit(estimator = "2sls")
+                                FEOLS.is_iv = True
+                            else:
+                                FEOLS.get_fit(estimator = "ols")
+                                FEOLS.is_iv = False
+
+                            # some bookkeeping
+                            FEOLS.fml = fml
+                            FEOLS.ssc_dict = self.ssc_dict
+                            FEOLS.na_index = na_index
+                            # data never makes it to Feols() class. needed for ex post
+                            # clustered vcov estimation when clustervar not in model params
+                            FEOLS.data = self.data.iloc[~self.data.index.isin(na_index)]
+                            if fval != "0":
+                                FEOLS.has_fixef = True
+                                FEOLS.fixef = fval
+                            else:
+                                FEOLS.has_fixef = False
+                                FEOLS.fixef = None
+                            #FEOLS.split_log = x
+
+
+                            # inference
+                            vcov_type = _get_vcov_type(vcov, fval)
+
+                            FEOLS.vcov_log = vcov_type
+                            FEOLS.get_vcov(vcov=vcov_type)
+                            FEOLS.get_inference()
+                            FEOLS.coefnames = x_names
+                            if self.icovars is not None:
+                                FEOLS.icovars = self.icovars
+                            else:
+                                FEOLS.icovars = None
+
+                            self.all_fitted_models[fml] = FEOLS
+
+                        elif self.method == "fepois":
+
+                          # estimation via FEPOIS
+                          pass
+
+                        else:
+
+                            raise ValueError(
+                                "Estimation method not supported. Please use 'feols' or 'fepois'."
+                            )
+
+
+
+
     def _is_multiple_estimation(self):
 
         '''
         helper method to check if multiple regression models will be estimated
         '''
 
         self.is_fixef_multi = False
@@ -558,17 +527,17 @@
                 or {"CRV3":"clustervar"} for CRV3 inference.
         Returns:
             None
         '''
 
         self.vcov_log = vcov
 
-        for model in list(self.model_res.keys()):
+        for model in list(self.all_fitted_models.keys()):
 
-            fxst = self.model_res[model]
+            fxst = self.all_fitted_models[model]
             fxst.vcov_log = vcov
 
             fxst.get_vcov(vcov=vcov)
             fxst.get_inference()
 
         return self
 
@@ -589,32 +558,23 @@
                 - t value: the t-values of the estimated coefficients
                 - Pr(>|t|): the p-values of the estimated coefficients
                 If `type` is set to "markdown", the resulting DataFrame will be returned as a
                 markdown-formatted string with three decimal places.
         '''
 
         res = []
-        for x in list(self.model_res.keys()):
+        for x in list(self.all_fitted_models.keys()):
 
-            fxst = self.model_res[x]
+            fxst = self.all_fitted_models[x]
+            df = fxst.tidy().reset_index()
+            df["fml"] = fxst.fml
+            res.append(df)
 
-            res.append(
-                pd.DataFrame(
-                    {
-                        'fml': x,
-                        'coefnames': fxst.coefnames,
-                        'Estimate': fxst.beta_hat,
-                        'Std. Error': fxst.se,
-                        't value': fxst.tstat,
-                        'Pr(>|t|)': fxst.pvalue
-                    }
-                )
-            )
 
-        res = pd.concat(res, axis=0).set_index('fml')
+        res = pd.concat(res, axis=0).set_index(['fml', 'coefnames'])
         if type == "markdown":
             return res.to_markdown(floatfmt=".3f")
         else:
             return res
 
     def summary(self) -> None:
         '''
@@ -622,39 +582,31 @@
         For each model, the method prints a header indicating the fixed-effects and the
         dependent variable, followed by a table of coefficient estimates with standard
         errors, t-values, and p-values.
         Returns:
             None
         '''
 
-        for x in list(self.model_res.keys()):
+        for x in list(self.all_fitted_models.keys()):
 
             split = x.split("|")
             if len(split) > 1:
                 fe = split[1]
             else:
                 fe = None
             depvar = split[0].split("~")[0]
-            fxst = self.model_res[x]
-            df = pd.DataFrame(
-                {
-                    '': fxst.coefnames,
-                    'Estimate': fxst.beta_hat,
-                    'Std. Error': fxst.se,
-                    't value': fxst.tstat,
-                    'Pr(>|t|)': fxst.pvalue
-                }
-            )
+            fxst = self.all_fitted_models[x]
+
+            df = fxst.tidy()
 
             if fxst.is_iv:
                 estimation_method = "IV"
             else:
                 estimation_method = "OLS"
 
-
             print('###')
             print('')
             print('Model: ', estimation_method)
             print('Dep. var.: ', depvar)
             if fe is not None:
                 print('Fixed effects: ', fe)
             # if fxst.split_log is not None:
@@ -667,53 +619,46 @@
 
     def coef(self) -> pd.DataFrame:
         '''
         Obtain the coefficients of the fitted models.
         Returns:
             A pd.DataFrame with coefficient names and Estimates. The key indicates which models the estimated statistic derives from.
         '''
-
-        df = self.tidy()
-        return df[['coefnames', 'Estimate']]
+        return self.tidy()["Estimate"]
 
     def se(self)-> pd.DataFrame:
         '''
         Obtain the standard errors of the fitted models.
 
         Returns:
             A pd.DataFrame with coefficient names and standard error estimates. The key indicates which models the estimated statistic derives from.
 
         '''
+        return self.tidy()["Std. Error"]
 
-        df = self.tidy()
-        return df[['coefnames', 'Std. Error']]
 
     def tstat(self)-> pd.DataFrame:
         '''
         Obtain the t-statistics of the fitted models.
 
          Returns:
             A pd.DataFrame with coefficient names and estimated t-statistics. The key indicates which models the estimated statistic derives from.
 
         '''
-
-        df = self.tidy()
-        return df[['coefnames', 't value']]
+        return self.tidy()["t value"]
 
     def pvalue(self) -> pd.DataFrame:
         '''
         Obtain the p-values of the fitted models.
 
         Returns:
             A pd.DataFrame with coefficient names and p-values. The key indicates which models the estimated statistic derives from.
 
         '''
-
-        df = self.tidy()
-        return df[['coefnames', 'Pr(>|t|)']]
+        return self.tidy()["Pr(>|t|)"]
 
     def iplot(self, alpha: float = 0.05, figsize: tuple = (10, 10), yintercept: Union[int, str, None] = None, xintercept: Union[int, str, None] = None, rotate_xticks: int = 0) -> None:
         '''
         Plot model coefficients with confidence intervals for variable interactions specified via the `i()` syntax.
         Args:
             alpha: float, optional. The significance level for the confidence intervals. Default is 0.05.
             figsize: tuple, optional. The size of the figure. Default is (10, 10).
@@ -723,29 +668,25 @@
             None
         '''
 
         ivars = self.icovars
 
         if ivars is None:
             raise ValueError(
-                "The estimated models did not have ivars / 'i()' model syntax. In consequence, the '.iplot()' method is not supported.")
-
-        ivars_keys = self.ivars.keys()
-        if ivars_keys is not None:
-            ref = list(ivars_keys)[0]
-        else:
-            ref = None
+                "The estimated models did not have ivars / 'i()' model syntax."
+                "In consequence, the '.iplot()' method is not supported."
+            )
 
         if "Intercept" in ivars:
             ivars.remove("Intercept")
 
-        df = self.tidy()
+        df = self.tidy().reset_index()
 
         df = df[df.coefnames.isin(ivars)]
-        models = df.index.unique()
+        models = df.fml.unique()
 
         _coefplot(
             models=models,
             figsize=figsize,
             alpha=alpha,
             yintercept=yintercept,
             xintercept=xintercept,
@@ -762,16 +703,16 @@
             yintercept (float): the value of the y-intercept. Default is 0.
             figtitle (str): the title of the figure. Default is None.
             figtext (str): the text at the bottom of the figure. Default is None.
         Returns:
             None
         '''
 
-        df = self.tidy()
-        models = df.index.unique()
+        df = self.tidy().reset_index()
+        models = df.fml.unique()
 
         _coefplot(
             models=models,
             figsize=figsize,
             alpha=alpha,
             yintercept=yintercept,
             xintercept=None,
@@ -799,17 +740,17 @@
 
         Returns:
             A pd.DataFrame with bootstrapped t-statistic and p-value. The index indicates which model the estimated statistic derives from.
         '''
 
 
         res = []
-        for x in list(self.model_res.keys()):
+        for x in list(self.all_fitted_models.keys()):
 
-            fxst = self.model_res[x]
+            fxst = self.all_fitted_models[x]
 
             if hasattr(fxst, 'clustervar'):
                 cluster = fxst.clustervar
             else:
                 cluster = None
 
             boot_res = fxst.get_wildboottest(B, cluster, param,  weights_type, impose_null, bootstrap_type, seed, adj, cluster_adj)
@@ -830,21 +771,42 @@
             )
 
         res = pd.concat(res, axis=1).T.set_index('fml')
 
         return res
 
 
+    def fetch_model(self, i: Union[int, str]):
+
+        '''
+        Utility method to fetch a model of class Feols from the Fixest class.
+        Args:
+            i (int or str): The index of the model to fetch.
+        Returns:
+            A Feols object.
+        '''
+
+        if isinstance(i, str):
+            i = int(i)
+
+        keys = list(self.all_fitted_models.keys())
+        if i >= len(keys):
+            raise IndexError(f"Index {i} is larger than the number of fitted models.")
+        key = keys[i]
+        print("Model: ", key)
+        model = self.all_fitted_models[key]
+        return model
+
 def _coefplot(models: List, df: pd.DataFrame, figsize: Tuple[int, int], alpha: float, yintercept: Optional[int] = None,
               xintercept: Optional[int] = None, is_iplot: bool = False,
               rotate_xticks: float = 0) -> None:
     """
         Plot model coefficients with confidence intervals.
         Args:
-            models (list): A list of fitted models.
+            models (list): A list of fitted models indices.
             figsize (tuple): The size of the figure.
             alpha (float): The significance level for the confidence intervals.
             yintercept (int or None): The value at which to draw a horizontal line on the plot.
             xintercept (int or None): The value at which to draw a vertical line on the plot.
             df (pandas.DataFrame): The dataframe containing the data used for the model fitting.
             is_iplot (bool): If True, plot variable interactions specified via the `i()` syntax.
             rotate_xticks (float): The angle in degrees to rotate the xticks labels. Default is 0 (no rotation).
@@ -855,37 +817,30 @@
     if len(models) > 1:
 
         fig, ax = plt.subplots(len(models), gridspec_kw={
                                'hspace': 0.5}, figsize=figsize)
 
         for x, model in enumerate(models):
 
-            df_model = df.xs(model)
-            coef = df_model["Estimate"].values
+            df_model = df.reset_index().set_index("fml").xs(model)
+            coef = df_model["Estimate"]
             conf_l = coef - \
-                df_model["Std. Error"].values * norm.ppf(1 - alpha / 2)
+                df_model["Std. Error"] * norm.ppf(1 - alpha / 2)
             conf_u = coef + \
-                df_model["Std. Error"].values * norm.ppf(1 - alpha / 2)
+                df_model["Std. Error"] * norm.ppf(1 - alpha / 2)
             coefnames = df_model["coefnames"].values.tolist()
 
             # could be moved out of the for loop, as the same ivars for all
             # models.
 
             if is_iplot == True:
                 fig.suptitle("iplot")
                 coefnames = [(i) for string in coefnames for i in re.findall(
                     r'\[T\.([\d\.\-]+)\]', string)]
 
-            # in the future: add reference category
-            # if ref is not None:
-            #    coef = np.append(coef, 0)
-            #    conf_l = np.append(conf_l, 0)
-            #    conf_u = np.append(conf_u, 0)
-            #    coefnames = np.append(coefnames, ref)
-
             ax[x].scatter(coefnames, coef, color="b", alpha=0.8)
             ax[x].scatter(coefnames, conf_u, color="b",
                           alpha=0.8, marker="_", s=100)
             ax[x].scatter(coefnames, conf_l, color="b",
                           alpha=0.8, marker="_", s=100)
             ax[x].vlines(coefnames, ymin=conf_l,
                          ymax=conf_u, color="b", alpha=0.8)
@@ -901,34 +856,26 @@
 
     else:
 
         fig, ax = plt.subplots(figsize=figsize)
 
         model = models[0]
 
-        df_model = df.xs(model)
+        df_model = df.reset_index().set_index("fml").xs(model)
+
         coef = df_model["Estimate"].values
         conf_l = coef - df_model["Std. Error"].values * norm.ppf(1 - alpha / 2)
         conf_u = coef + df_model["Std. Error"].values * norm.ppf(1 - alpha / 2)
         coefnames = df_model["coefnames"].values.tolist()
 
         if is_iplot == True:
             fig.suptitle("iplot")
             coefnames = [(i) for string in coefnames for i in re.findall(
                 r'\[T\.([\d\.\-]+)\]', string)]
 
-        # in the future: add reference category
-        # if ref is not None:
-        #    coef = np.append(coef, 0)
-        #    conf_l = np.append(conf_l, 0)
-        #    conf_u = np.append(conf_u, 0)
-        #    coefnames = np.append(coefnames, ref)
-
-            # c = next(color)
-
         ax.scatter(coefnames, coef, color="b", alpha=0.8)
         ax.scatter(coefnames, conf_u, color="b", alpha=0.8, marker="_", s=100)
         ax.scatter(coefnames, conf_l, color="b", alpha=0.8, marker="_", s=100)
         ax.vlines(coefnames, ymin=conf_l, ymax=conf_u, color="b", alpha=0.8)
         if yintercept is not None:
             ax.axhline(yintercept, color='red', linestyle='--', alpha=0.5)
         if xintercept is not None:
@@ -957,15 +904,15 @@
         raise ValueError("Column " + ivars[0] + " is not of type 'O' or 'category', which is required in the first position of i(). Instead it is of type " +
                         i0_type.name + ". If a reference level is set, it is required that the variable in the first position of 'i()' is of type 'O' or 'category'.")
         if not i1_type in ['int64', 'float64', 'int32', 'float32']:
             raise ValueError("Column " + ivars[1] + " is not of type 'int' or 'float', which is required in the second position of i(). Instead it is of type " +
                             i1_type.name + ". If a reference level is set, iti is required that the variable in the second position of 'i()' is of type 'int' or 'float'.")
 
 
-def _prepare_split_estimation(split, fsplit, data, var_dict):
+def _prepare_split_estimation(split, fsplit, data, fml_dict):
 
     '''
     Cleans the input for the split estimation.
     Checks if the split variables are of the correct type.
 
     Args:
         split (str): The name of the variable used for the split estimation.
@@ -978,15 +925,16 @@
         estimate_split_model (bool): Whether to estimate the split model.
         estimate_full_model (bool): Whether to estimate the full model.
     '''
 
     if split is not None:
         if fsplit is not None:
             raise ValueError(
-                "Cannot specify both split and fsplit. Please specify only one of the two.")
+                "Cannot specify both split and fsplit. Please specify only one of the two."
+            )
         else:
             splitvar = data[split]
             estimate_full_model = False
             estimate_split_model = True
             splitvar_name = split
     elif fsplit is not None:
         splitvar = data[fsplit]
@@ -999,51 +947,76 @@
         estimate_split_model = False
         estimate_full_model = True
 
 
     if splitvar is not None:
         split_categories = np.unique(splitvar)
         if splitvar_name not in data.columns:
-            raise ValueError("Split variable " +
-                            splitvar + " not found in data.")
-        if splitvar_name in var_dict.keys():
-            raise ValueError("Split variable " + splitvar +
-                            " cannot be a fixed effect variable.")
+            raise ValueError(
+                "Split variable " +
+                splitvar + " not found in data."
+                )
+        if splitvar_name in fml_dict.keys():
+            raise ValueError(
+                "Split variable " + splitvar +
+                " cannot be a fixed effect variable."
+            )
         if splitvar.dtype.name != "category":
             splitvar = pd.Categorical(splitvar)
 
     return splitvar, splitvar_name, estimate_split_model, estimate_full_model
 
+
+def get_fml(y_names, x_names, fval):
+
+    y_names = y_names[0]
+    fml = y_names + " ~ " + "+".join(x_names)
+    if fval != "0":
+        fml += " | " + fval
+
+    return fml.replace(" ", "")
+
+
 def _multicollinearity_checks(X, Z, ivars, fml2):
 
     '''
     Checks for multicollinearity in the design matrices X and Z.
     Args:
         X (numpy.ndarray): The design matrix X.
         Z (numpy.ndarray): The design matrix (with instruments) Z.
         ivars (list): The list of variables specified in the i() syntax.
         fml2 (str): The formula string.
 
     '''
 
     if np.linalg.matrix_rank(X) < min(X.shape):
         if ivars is not None:
-            raise ValueError("The design Matrix X does not have full rank for the regression with fml" + fml2 +
-                            ". The model is skipped. As you are running a regression via `i()` syntax, maybe you need to drop a level via i(var1, var2, ref = ...)?")
+            raise MatrixNotFullRankError(
+                'The design Matrix X does not have full rank for the regression with fml" + fml2 + "."'
+                'The model is skipped.'
+                'As you are running a regression via `i()` syntax, maybe you need to drop a level via i(var1, var2, ref = ...)?'
+                )
         else:
-            raise ValueError(
-                    "The design Matrizx X does not have full rank for the regression with fml" + fml2 + ". The model is skipped. ")
+            raise MatrixNotFullRankError(
+                    'The design Matrix X does not have full rank for the regression with fml" + fml2 + "."'
+                    'The model is skipped. '
+                )
 
     if np.linalg.matrix_rank(Z) < min(Z.shape):
         if ivars is not None:
-            raise ValueError("The design Matrix Z does not have full rank for the regression with fml" + fml2 +
-                            ". The model is skipped. As you are running a regression via `i()` syntax, maybe you need to drop a level via i(var1, var2, ref = ...)?")
+            raise MatrixNotFullRankError(
+                'The design Matrix Z does not have full rank for the regression with fml" + fml2 + "."'
+                'The model is skipped.'
+                'As you are running a regression via `i()` syntax, maybe you need to drop a level via i(var1, var2, ref = ...)?"'
+                )
         else:
-            raise ValueError(
-                    "The design Matrix Z does not have full rank for the regression with fml" + fml2 + ". The model is skipped. ")
+            raise MatrixNotFullRankError(
+                    'The design Matrix Z does not have full rank for the regression with fml" + fml2 + "."'
+                    'The model is skipped.'
+                )
 
 def _get_vcov_type(vcov, fval):
 
 
     '''
     Passes the specified vcov type. If no vcov type specified, sets the default vcov type as iid if no fixed effect
     is included in the model, and CRV1 clustered by the first fixed effect if a fixed effect is included in the model.
```

### Comparing `pyfixest-0.6.6/pyfixest/FormulaParser.py` & `pyfixest-0.7.0/pyfixest/FormulaParser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import re
-
-class FixedEffectInteractionError(Exception):
-    pass
-
-class CovariateInteractionError(Exception):
-    pass
-
-class DuplicateKeyError(Exception):
-    pass
-
+from pyfixest.exceptions import (
+    DuplicateKeyError,
+    EndogVarsAsCovarsError,
+    InstrumentsAsCovarsError,
+    UnderDeterminedIVError,
+    UnsupportedMultipleEstimationSyntax
+)
 
 class FixestFormulaParser:
 
 
     """
     A class for parsing a formula string into its individual components.
 
@@ -36,99 +33,110 @@
         Constructor method that initializes the object with a given formula.
 
         Args:
         fml (str): A two-formula string in the form "Y1 + Y2 ~ X1 + X2 | FE1 + FE2".
 
         Returns:
             None
+
         """
 
         #fml =' Y + Y2 ~  i(X1, X2) |csw0(X3, X4)'
 
         # Clean up the formula string
         fml = "".join(fml.split())
 
         # Split the formula string into its components
         fml_split = fml.split('|')
         depvars, covars = fml_split[0].split("~")
-          
+
         if len(fml_split) == 1:
             fevars = "0"
             endogvars = None
             instruments = None
         elif len(fml_split) == 2:
             if "~" in fml_split[1]:
                 fevars = "0"
                 endogvars, instruments = fml_split[1].split("~")
                 # add endogeneous variable to "covars" - yes, bad naming
-                
-                
-                # check if any of the instruments or endogeneous variables are also specified 
+
+
+                # check if any of the instruments or endogeneous variables are also specified
                 # as covariates
                 if any(element in covars.split("+") for element in endogvars.split("+")):
-                    raise ValueError("Endogeneous variables are specified as covariates in the first part of the three-part formula. This is not allowed.")
-                
+                    raise EndogVarsAsCovarsError(
+                        "Endogeneous variables are specified as covariates in the first part of the three-part formula. This is not allowed."
+                        )
+
                 if any(element in covars.split("+") for element in instruments.split("+")):
-                    raise ValueError("Instruments are specified as covariates in the first part of the three-part formula. This is not allowed.")
-                
-                if covars == "1": 
+                    raise InstrumentsAsCovarsError(
+                        "Instruments are specified as covariates in the first part of the three-part formula. This is not allowed."
+                    )
+
+                if covars == "1":
                     covars = endogvars
-                else: 
+                else:
                     covars = endogvars + "+" +  covars
             else:
                 fevars = fml_split[1]
                 endogvars = None
                 instruments = None
         elif len(fml_split) == 3:
             fevars = fml_split[1]
             endogvars, instruments = fml_split[2].split("~")
 
-            # check if any of the instruments or endogeneous variables are also specified 
+            # check if any of the instruments or endogeneous variables are also specified
             # as covariates
             if any(element in covars.split("+") for element in endogvars.split("+")):
-                raise ValueError("Endogeneous variables are specified as covariates in the first part of the three-part formula. This is not allowed.")
-                
+                raise EndogVarsAsCovarsError(
+                    "Endogeneous variables are specified as covariates in the first part of the three-part formula. This is not allowed."
+                )
+
             if any(element in covars.split("+") for element in instruments.split("+")):
-                raise ValueError("Instruments are specified as covariates in the first part of the three-part formula. This is not allowed.")
+                raise InstrumentsAsCovarsError(
+                    "Instruments are specified as covariates in the first part of the three-part formula. This is not allowed."
+                )
 
             # add endogeneous variable to "covars" - yes, bad naming
-            if covars == "1": 
+            if covars == "1":
                 covars = endogvars
-            else: 
+            else:
                 covars = endogvars + "+" +  covars
 
         if endogvars is not None:
             if len(endogvars) > len(instruments):
-                raise ValueError("The IV system is underdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables.")
-            #elif len(endogvars) < len(instruments):
-            #    raise ValueError("The IV system is overdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables.")
+                raise UnderDeterminedIVError(
+                    "The IV system is underdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables."
+                )
             else:
                 pass
 
         # Parse all individual formula components into lists
         self.depvars = depvars.split("+")
         self.covars = _unpack_fml(covars)
         self.fevars = _unpack_fml(fevars)
         # no fancy syntax for endogvars, instruments allowed
         self.endogvars = endogvars
         self.instruments = instruments
 
+        # clean instruments
         if instruments is not None:
             self.is_iv = True
             # all rhs variables for the first stage (endog variable replaced with instrument)
             first_stage_covars_list = covars.split("+")
             first_stage_covars_list[first_stage_covars_list.index(endogvars)] = instruments
             self.first_stage_covars_list = "+".join(first_stage_covars_list)
             self.covars_first_stage = _unpack_fml(self.first_stage_covars_list)
             self.depvars_first_stage = endogvars
         else:
             self.is_iv = False
             self.covars_first_stage = None
             self.depvars_first_stage = None
 
+        # parse i() syntax
         if self.covars.get("i") is not None:
             self.ivars = dict()
             i_split = self.covars.get("i")[-1].split("=")
             if len(i_split) > 1:
                 ref = self.covars.get("i")[-1].split("=")[1]
                 ivar_list = self.covars.get("i")[:-1]
                 self.covars["i"] = self.covars.get("i")[:-1]
@@ -141,128 +149,56 @@
         else:
             self.ivars = None
 
 
         # Pack the formula components back into strings
         self.covars_fml = _pack_to_fml(self.covars)
         self.fevars_fml = _pack_to_fml(self.fevars)
-        if instruments is not None: 
+        if instruments is not None:
             self.covars_first_stage_fml = _pack_to_fml(self.covars_first_stage)
-        else: 
+        else:
             self.covars_first_stage_fml = None
-        #if "^" in self.covars:
-        #    raise CovariateInteractionError("Please use 'i()' or ':' syntax to interact covariates.")
-
-        #for  x in ["i", ":"]:
-        #    if x in self.fevars:
-        #        raise FixedEffectInteractionError("Interacting fixed effects via", x, " is not allowed. Please use '^' to interact fixed effects.")
 
 
+    def get_new_fml_dict(self, iv = False):
 
+        '''
+        Get a nested dictionary of all formulas.
 
-
-    def get_fml_dict(self, iv = False):
-
-        """
-        Returns a dictionary of all fevars & formula without fevars. The keys are the fixed effect variable combinations.
-        The values are lists of formula strings that do not include the fixed effect variables.
-
-        Args:
-            iv (bool): If True, the formula dictionary will be returned for the first stage of an IV regression.
-                       If False, the formula dictionary will be returned for the second stage of an IV regression / OLS regression.
+        Parameters:
+            iv: bool (default: False)
+                If True, the formulas for the first stage are returned. Otherwise, the formulas for the second stage are returned.
         Returns:
-            dict: A dictionary of the form {"fe1+fe2": ['Y1 ~ X', 'Y2~X'], "fe1+fe3": ['Y1 ~ X', 'Y2~X']} where
-            the keys are the fixed effect variable combinations and the values are lists of formula strings
-            that do not include the fixed effect variables.
-            If IV is True, creates an instance named fml_dict_iv. Otherwise, creates an instance named fml_dict.
-        """
-
+            fml_dict: dict
+                A nested dictionary of all formulas. The dictionary has the following structure: first, a dictionary with the
+                fixed effects combinations as keys. Then, for each fixed effect combination, a dictionary with the dependent variables
+                as keys. Finally, for each dependent variable, a list of formulas as values.
+
+                Here is an example:
+                    fml = Y1 + Y2 ~ X1 + X2 | FE1 + FE2 is transformed into: {"FE1 + FE2": {"Y1": "Y2 ~X1+X2", "Y2":"X1+X2"}}
+        '''
 
         fml_dict = dict()
+
         for fevar in self.fevars_fml:
-            res = []
+            res = dict()
             for depvar in self.depvars:
+                res[depvar] = []
                 if iv:
                     for covar in self.covars_first_stage_fml:
-                        res.append(depvar + '~' + covar)
+                        res[depvar].append(depvar + '~' + covar)
                 else:
                     for covar in self.covars_fml:
-                        res.append(depvar + '~' + covar)
+                        res[depvar].append(depvar + '~' + covar)
             fml_dict[fevar] = res
 
         if iv:
-            self.fml_dict_iv = fml_dict
+            self.fml_dict_new_iv = fml_dict
         else:
-            self.fml_dict = fml_dict
-
-    def _transform_fml_dict(self, iv = False):
-
-        fml_dict2 = dict()
-
-        if iv:
-
-            for fe in self.fml_dict_iv.keys():
-
-                fml_dict2[fe] = dict()
-
-                for fml in self.fml_dict_iv.get(fe):
-                    depvars, covars = fml.split("~")
-                    if fml_dict2[fe].get(depvars) is None:
-                        fml_dict2[fe][depvars] = [covars]
-                    else:
-                        fml_dict2[fe][depvars].append(covars)
-        else:
-
-          for fe in self.fml_dict.keys():
-
-              fml_dict2[fe] = dict()
-
-              for fml in self.fml_dict.get(fe):
-                  depvars, covars = fml.split("~")
-                  if fml_dict2[fe].get(depvars) is None:
-                      fml_dict2[fe][depvars] = [covars]
-                  else:
-                      fml_dict2[fe][depvars].append(covars)
-
-        if iv:
-            self.fml_dict2_iv = fml_dict2
-        else:
-            self.fml_dict2 = fml_dict2
-
-
-
-    def get_var_dict(self, iv = False):
-
-        """
-        Create a dictionary of all fevars and list of covars and depvars used in regression with those fevars.
-        The keys are the fixed effect variable combinations. The values are lists of variables (dependent variables and covariates) of
-        the resespective regressions.
-
-        Args:
-            iv (bool): If True, the formula dictionary will be returned for the first stage of an IV regression.
-
-        Returns:
-            dict: A dictionary of the form {"fe1+fe2": ['Y1', 'X1', 'X2'], "fe1+fe3": ['Y1', 'X1', 'X2']} where
-            the keys are the fixed effect variable combinations and the values are lists of variables
-            (dependent variables and covariates) used in the regression with those fixed effect variables.
-
-        """
-        var_dict = dict()
-        if iv:
-            for fevar in self.fevars_fml:
-                var_dict[fevar] = _flatten_list(self.depvars) + _flatten_list(list(self.covars_first_stage.values()))
-
-        else:
-            for fevar in self.fevars_fml:
-                var_dict[fevar] = _flatten_list(self.depvars) + _flatten_list(list(self.covars.values()))
-
-        if iv:
-            self.var_dict_iv = var_dict
-        else:
-            self.var_dict = var_dict
+            self.fml_dict_new = fml_dict
 
 
 def _unpack_fml(x):
 
     '''
     Given a formula string `x` - e.g. 'X1 + csw(X2, X3)' - , splits it into its constituent variables and their types (if any),
     and returns a dictionary containing the result. The dictionary has the following keys: 'constant', 'sw', 'sw0', 'csw'.
@@ -314,33 +250,33 @@
     res_s = dict()
     res_s['constant'] = []
 
     for var in var_split:
 
         # Check if this variable contains a switch
         varlist, sw_type = _find_sw(var)
-        
+
         # If there's no switch, just add the variable to the list
         if sw_type is None:
             if _is_varying_slopes(var):
                 varlist, sw_type = _transform_varying_slopes(var)
-                for x in varlist.split("+"): 
+                for x in varlist.split("+"):
                     res_s['constant'].append(x)
-            else: 
+            else:
                 res_s['constant'].append(varlist)
 
         # If there'_ a switch, unpack it and add it to the list
         else:
             if sw_type in ['sw', 'sw0', 'csw', 'csw0', 'i']:
                 _check_duplicate_key(res_s, sw_type)
                 res_s[sw_type] = varlist
-            elif sw_type == "varying_slopes": 
+            elif sw_type == "varying_slopes":
                 res_s[sw_type] = varlist
             else:
-                raise ValueError("Unsupported switch type")
+                raise UnsupportedMultipleEstimationSyntax("Unsupported switch type")
 
     # Sort the list by type (strings first, then lists)
     #res_s.sort(key=lambda x: 0 if isinstance(x, str) else 1)
 
     return res_s
 
 
@@ -519,32 +455,36 @@
         key (str): The key to check for in the dictionary.
 
     Returns:
         None
     '''
 
     if key == 'i' and 'i' in my_dict:
-        raise DuplicateKeyError("Duplicate key found: " + key + ". Fixed effect syntax i() can only be used once in the input formula.")
+        raise DuplicateKeyError(
+            "Duplicate key found: " + key + ". Fixed effect syntax i() can only be used once in the input formula."
+            )
     else:
         for key in ['sw', 'csw', 'sw0', 'csw0']:
             if key in my_dict:
-                raise DuplicateKeyError("Duplicate key found: " + key + ". Multiple estimation syntax can only be used once on the rhs of the two-sided formula.")
+                raise DuplicateKeyError(
+                    "Duplicate key found: " + key + ". Multiple estimation syntax can only be used once on the rhs of the two-sided formula."
+                    )
             else:
                 None
-                
-                
-def _is_varying_slopes(x): 
-          
+
+
+def _is_varying_slopes(x):
+
     pattern = r'\[.*\]'
     match = re.search(pattern, x)
     if match:
         return True
     else:
         return False
-            
+
 def _transform_varying_slopes(x):
     parts = x.split('[')
     a = parts[0]
     b = parts[1].replace(']', '')
     transformed_string = f"{a}/{b}"
     return transformed_string, "varying_slopes"
```

### Comparing `pyfixest-0.6.6/pyfixest/ssc_utils.py` & `pyfixest-0.7.0/pyfixest/ssc_utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.6.6/pyfixest/utils.py` & `pyfixest-0.7.0/pyfixest/utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.6.6/readme.md` & `pyfixest-0.7.0/readme.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.6.6/PKG-INFO` & `pyfixest-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfixest
-Version: 0.6.6
+Version: 0.7.0
 Summary: Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation.
 Home-page: https://s3alfisc.github.io/pyfixest/
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

