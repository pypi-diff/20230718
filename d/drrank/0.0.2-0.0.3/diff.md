# Comparing `tmp/drrank-0.0.2.tar.gz` & `tmp/drrank-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drrank-0.0.2.tar", last modified: Tue Jul 18 21:13:44 2023, max compression
+gzip compressed data, was "drrank-0.0.3.tar", last modified: Tue Jul 18 21:18:23 2023, max compression
```

## Comparing `drrank-0.0.2.tar` & `drrank-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 21:13:44.438637 drrank-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-18 21:09:47.000000 drrank-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    11926 2023-07-18 21:13:44.434593 drrank-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11361 2023-07-18 21:09:47.000000 drrank-0.0.2/README.md
--rw-rw-rw-   0        0        0      849 2023-07-18 21:12:59.000000 drrank-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 21:13:44.438868 drrank-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 21:13:44.414597 drrank-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-07-18 21:09:47.000000 drrank-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:13:44.431597 drrank-0.0.2/src/drrank.egg-info/
--rw-rw-rw-   0        0        0    11926 2023-07-18 21:13:44.000000 drrank-0.0.2/src/drrank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-07-18 21:13:44.000000 drrank-0.0.2/src/drrank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 21:13:44.000000 drrank-0.0.2/src/drrank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-18 21:13:44.000000 drrank-0.0.2/src/drrank.egg-info/requires.txt
--rw-rw-rw-   0        0        0       84 2023-07-18 21:13:44.000000 drrank-0.0.2/src/drrank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    19665 2023-07-18 21:09:47.000000 drrank-0.0.2/src/drrank.py
--rw-rw-rw-   0        0        0    14046 2023-07-18 21:09:47.000000 drrank-0.0.2/src/drrank_distribution.py
--rw-rw-rw-   0        0        0     1205 2023-07-18 21:09:47.000000 drrank-0.0.2/src/drrank_loss.py
--rw-rw-rw-   0        0        0     2228 2023-07-18 21:09:47.000000 drrank-0.0.2/src/drrank_prior.py
--rw-rw-rw-   0        0        0      245 2023-07-18 21:09:47.000000 drrank-0.0.2/src/drrank_utils.py
--rw-rw-rw-   0        0        0     1172 2023-07-18 21:09:47.000000 drrank-0.0.2/src/simul_pij.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:18:23.225430 drrank-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 21:09:47.000000 drrank-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    11910 2023-07-18 21:18:23.222428 drrank-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11345 2023-07-18 21:17:10.000000 drrank-0.0.3/README.md
+-rw-rw-rw-   0        0        0      849 2023-07-18 21:17:39.000000 drrank-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 21:18:23.225430 drrank-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 21:18:23.204432 drrank-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-07-18 21:09:47.000000 drrank-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:18:23.218464 drrank-0.0.3/src/drrank.egg-info/
+-rw-rw-rw-   0        0        0    11910 2023-07-18 21:18:23.000000 drrank-0.0.3/src/drrank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-07-18 21:18:23.000000 drrank-0.0.3/src/drrank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:18:23.000000 drrank-0.0.3/src/drrank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-18 21:18:23.000000 drrank-0.0.3/src/drrank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       84 2023-07-18 21:18:23.000000 drrank-0.0.3/src/drrank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19665 2023-07-18 21:09:47.000000 drrank-0.0.3/src/drrank.py
+-rw-rw-rw-   0        0        0    14046 2023-07-18 21:09:47.000000 drrank-0.0.3/src/drrank_distribution.py
+-rw-rw-rw-   0        0        0     1205 2023-07-18 21:09:47.000000 drrank-0.0.3/src/drrank_loss.py
+-rw-rw-rw-   0        0        0     2228 2023-07-18 21:09:47.000000 drrank-0.0.3/src/drrank_prior.py
+-rw-rw-rw-   0        0        0      245 2023-07-18 21:09:47.000000 drrank-0.0.3/src/drrank_utils.py
+-rw-rw-rw-   0        0        0     1172 2023-07-18 21:09:47.000000 drrank-0.0.3/src/simul_pij.py
```

### Comparing `drrank-0.0.2/LICENSE` & `drrank-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drrank-0.0.2/PKG-INFO` & `drrank-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drrank
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implement the Empirical Bayes ranking scheme developed in Kline, Rose, and Walters (2023)
 Author-email: "Evan K. Rose" <ekrose@gmail.com>
 Project-URL: Homepage, https://github.com/ekrose/drrank
 Project-URL: Bug Tracker, https://github.com/ekrose/drrank/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -96,15 +96,15 @@
 
 ```python
 
 # Plot the estimated prior distribution
 G.plot_estimates(save_path = "example/prior_distribution.jpg")
 ```
 
-![prior_distribution](https://github.com/ekrose/drrank/blob/estimate_pis/example/prior_distribution.jpg?raw=true)
+![prior_distribution](https://github.com/ekrose/drrank/blob/main/example/prior_distribution.jpg?raw=true)
 
 Within the function you can specify the following arguments:
 - *g_theta*: provide your own prior distribution G. `None` implies the function will utilize the estimated G from the *estimate_prior()* method (default = `None`).
 - *show_plot*: whether to show the plot or not (default = `True`).
 - *save_path*: path to where the plot will be saved. `None` implies the graph will not be saved (default = `None`).
 
 ### 3. Estimation of posterior features and $P$ matrix
@@ -200,15 +200,15 @@
 from drrank import fig_ranks
 
 # Merge the results with the identity of our observations
 results['firstname'] = data.firstname
 fig_ranks(ranking = results, posterior_features = G.posterior_df, ylabels = 'firstname', save_path = 'example/name_ranking.jpg')
 ```
 
-![name_ranking](https://github.com/ekrose/drrank/blob/estimate_pis/example/name_ranking.jpg?raw=true)
+![name_ranking](https://github.com/ekrose/drrank/blob/main/example/name_ranking.jpg?raw=true)
 
 Within the function you can specify the following arguments:
 - *results*: ranking results from *drrank.fit*
 - *posterior_features*: posterior features computed through *G.compute_posteriors()*
 - *ylabels*: optional, specify the column in *results* where we have stored the labels of each observation (default = `None`)
 - *show_plot*: whether to show the plot or not (default = `True`)
 - *save_path*: path to where the plot will be saved; `None` implies the graph will not be saved (default = `None`)
```

### Comparing `drrank-0.0.2/README.md` & `drrank-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ```python
 
 # Plot the estimated prior distribution
 G.plot_estimates(save_path = "example/prior_distribution.jpg")
 ```
 
-![prior_distribution](https://github.com/ekrose/drrank/blob/estimate_pis/example/prior_distribution.jpg?raw=true)
+![prior_distribution](https://github.com/ekrose/drrank/blob/main/example/prior_distribution.jpg?raw=true)
 
 Within the function you can specify the following arguments:
 - *g_theta*: provide your own prior distribution G. `None` implies the function will utilize the estimated G from the *estimate_prior()* method (default = `None`).
 - *show_plot*: whether to show the plot or not (default = `True`).
 - *save_path*: path to where the plot will be saved. `None` implies the graph will not be saved (default = `None`).
 
 ### 3. Estimation of posterior features and $P$ matrix
@@ -186,15 +186,15 @@
 from drrank import fig_ranks
 
 # Merge the results with the identity of our observations
 results['firstname'] = data.firstname
 fig_ranks(ranking = results, posterior_features = G.posterior_df, ylabels = 'firstname', save_path = 'example/name_ranking.jpg')
 ```
 
-![name_ranking](https://github.com/ekrose/drrank/blob/estimate_pis/example/name_ranking.jpg?raw=true)
+![name_ranking](https://github.com/ekrose/drrank/blob/main/example/name_ranking.jpg?raw=true)
 
 Within the function you can specify the following arguments:
 - *results*: ranking results from *drrank.fit*
 - *posterior_features*: posterior features computed through *G.compute_posteriors()*
 - *ylabels*: optional, specify the column in *results* where we have stored the labels of each observation (default = `None`)
 - *show_plot*: whether to show the plot or not (default = `True`)
 - *save_path*: path to where the plot will be saved; `None` implies the graph will not be saved (default = `None`)
```

### Comparing `drrank-0.0.2/pyproject.toml` & `drrank-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "wheel"
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drrank"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Evan K. Rose", email="ekrose@gmail.com" },
 ]
 description = "Implement the Empirical Bayes ranking scheme developed in Kline, Rose, and Walters (2023)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `drrank-0.0.2/src/drrank.egg-info/PKG-INFO` & `drrank-0.0.3/src/drrank.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drrank
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implement the Empirical Bayes ranking scheme developed in Kline, Rose, and Walters (2023)
 Author-email: "Evan K. Rose" <ekrose@gmail.com>
 Project-URL: Homepage, https://github.com/ekrose/drrank
 Project-URL: Bug Tracker, https://github.com/ekrose/drrank/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -96,15 +96,15 @@
 
 ```python
 
 # Plot the estimated prior distribution
 G.plot_estimates(save_path = "example/prior_distribution.jpg")
 ```
 
-![prior_distribution](https://github.com/ekrose/drrank/blob/estimate_pis/example/prior_distribution.jpg?raw=true)
+![prior_distribution](https://github.com/ekrose/drrank/blob/main/example/prior_distribution.jpg?raw=true)
 
 Within the function you can specify the following arguments:
 - *g_theta*: provide your own prior distribution G. `None` implies the function will utilize the estimated G from the *estimate_prior()* method (default = `None`).
 - *show_plot*: whether to show the plot or not (default = `True`).
 - *save_path*: path to where the plot will be saved. `None` implies the graph will not be saved (default = `None`).
 
 ### 3. Estimation of posterior features and $P$ matrix
@@ -200,15 +200,15 @@
 from drrank import fig_ranks
 
 # Merge the results with the identity of our observations
 results['firstname'] = data.firstname
 fig_ranks(ranking = results, posterior_features = G.posterior_df, ylabels = 'firstname', save_path = 'example/name_ranking.jpg')
 ```
 
-![name_ranking](https://github.com/ekrose/drrank/blob/estimate_pis/example/name_ranking.jpg?raw=true)
+![name_ranking](https://github.com/ekrose/drrank/blob/main/example/name_ranking.jpg?raw=true)
 
 Within the function you can specify the following arguments:
 - *results*: ranking results from *drrank.fit*
 - *posterior_features*: posterior features computed through *G.compute_posteriors()*
 - *ylabels*: optional, specify the column in *results* where we have stored the labels of each observation (default = `None`)
 - *show_plot*: whether to show the plot or not (default = `True`)
 - *save_path*: path to where the plot will be saved; `None` implies the graph will not be saved (default = `None`)
```

### Comparing `drrank-0.0.2/src/drrank.py` & `drrank-0.0.3/src/drrank.py`

 * *Files identical despite different names*

### Comparing `drrank-0.0.2/src/drrank_distribution.py` & `drrank-0.0.3/src/drrank_distribution.py`

 * *Files identical despite different names*

### Comparing `drrank-0.0.2/src/drrank_loss.py` & `drrank-0.0.3/src/drrank_loss.py`

 * *Files identical despite different names*

### Comparing `drrank-0.0.2/src/drrank_prior.py` & `drrank-0.0.3/src/drrank_prior.py`

 * *Files identical despite different names*

### Comparing `drrank-0.0.2/src/simul_pij.py` & `drrank-0.0.3/src/simul_pij.py`

 * *Files identical despite different names*

