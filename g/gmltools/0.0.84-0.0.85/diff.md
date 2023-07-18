# Comparing `tmp/gmltools-0.0.84.tar.gz` & `tmp/gmltools-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.84.tar", last modified: Tue Jul 18 13:00:55 2023, max compression
+gzip compressed data, was "gmltools-0.0.85.tar", last modified: Tue Jul 18 13:06:13 2023, max compression
```

## Comparing `gmltools-0.0.84.tar` & `gmltools-0.0.85.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.597740 gmltools-0.0.84/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.84/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.84/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-07-18 13:00:55.597740 gmltools-0.0.84/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.84/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.473860 gmltools-0.0.84/dist/
--rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.84/dist/gmltools-0.0.80.tar.gz
--rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.84/dist/gmltools-0.0.81.tar.gz
--rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.84/dist/gmltools-0.0.82.tar.gz
--rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.84/environment.txt
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.84/gmltools.yml
--rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.84/gmltools2.yml
--rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.84/gmltools3.yml
--rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.84/gmltools4.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.84/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-07-18 13:00:16.000000 gmltools-0.0.84/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 13:00:55.598739 gmltools-0.0.84/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-07-18 13:00:08.000000 gmltools-0.0.84/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.328127 gmltools-0.0.84/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.490912 gmltools-0.0.84/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.84/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.84/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.512910 gmltools-0.0.84/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.84/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    45883 2023-06-29 11:50:55.000000 gmltools-0.0.84/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.544165 gmltools-0.0.84/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.84/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.84/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.84/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.84/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   160542 2023-07-18 12:59:28.000000 gmltools-0.0.84/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.84/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.84/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.566185 gmltools-0.0.84/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.84/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.84/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.84/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.596739 gmltools-0.0.84/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.84/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.84/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.84/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.84/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.497913 gmltools-0.0.84/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-07-18 13:00:55.000000 gmltools-0.0.84/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.204385 gmltools-0.0.85/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.85/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.85/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-07-18 13:06:13.203384 gmltools-0.0.85/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.85/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.178419 gmltools-0.0.85/dist/
+-rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.85/dist/gmltools-0.0.80.tar.gz
+-rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.85/dist/gmltools-0.0.81.tar.gz
+-rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.85/dist/gmltools-0.0.82.tar.gz
+-rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.85/environment.txt
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.85/gmltools.yml
+-rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.85/gmltools2.yml
+-rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.85/gmltools3.yml
+-rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.85/gmltools4.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.85/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-07-18 13:05:53.000000 gmltools-0.0.85/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:06:13.204385 gmltools-0.0.85/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-07-18 13:05:44.000000 gmltools-0.0.85/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.145424 gmltools-0.0.85/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.182386 gmltools-0.0.85/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.85/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.85/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.189384 gmltools-0.0.85/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.85/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    45883 2023-06-29 11:50:55.000000 gmltools-0.0.85/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.196385 gmltools-0.0.85/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.85/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.85/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.85/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.85/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   160474 2023-07-18 13:05:36.000000 gmltools-0.0.85/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.85/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.85/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.198384 gmltools-0.0.85/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.85/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.85/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.85/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.202384 gmltools-0.0.85/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.85/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.85/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.85/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.85/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:06:13.187384 gmltools-0.0.85/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-07-18 13:06:12.000000 gmltools-0.0.85/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-07-18 13:06:13.000000 gmltools-0.0.85/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:06:12.000000 gmltools-0.0.85/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-07-18 13:06:12.000000 gmltools-0.0.85/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 13:06:12.000000 gmltools-0.0.85/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.84/LICENSE` & `gmltools-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/Models.ipynb` & `gmltools-0.0.85/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/PKG-INFO` & `gmltools-0.0.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.84
+Version: 0.0.85
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.84/README.md` & `gmltools-0.0.85/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/dist/gmltools-0.0.80.tar.gz` & `gmltools-0.0.85/dist/gmltools-0.0.80.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/dist/gmltools-0.0.81.tar.gz` & `gmltools-0.0.85/dist/gmltools-0.0.81.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/dist/gmltools-0.0.82.tar.gz` & `gmltools-0.0.85/dist/gmltools-0.0.82.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/gmltools.yml` & `gmltools-0.0.85/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/gmltools2.yml` & `gmltools-0.0.85/gmltools2.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/gmltools3.yml` & `gmltools-0.0.85/gmltools3.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/gmltools4.yml` & `gmltools-0.0.85/gmltools4.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/mltools.yml` & `gmltools-0.0.85/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/pyproject.toml` & `gmltools-0.0.85/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.84"
+version = "0.0.85"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.84/setup.py` & `gmltools-0.0.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.84',
+    'version': '0.0.85',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.84/src/gmltools/To_Do.txt` & `gmltools-0.0.85/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/eda/eda.py` & `gmltools-0.0.85/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/models/bayes.py` & `gmltools-0.0.85/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.85/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/models/dummy_model.py` & `gmltools-0.0.85/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/models/model.py` & `gmltools-0.0.85/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -892,15 +892,15 @@
         model_ : sklearn model
             Trained model.
 
         """
 
         print(" INFO: Agurments params must start as 'KNN__param'" + '\n' "INFO: Default params in Documentation for Random Forest are: ", knn_default_params_clf)
         print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}', f'bayes_n_iter = {bayes_n_iter}',
-               f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+               f'bayes_pbounds = {bayes_pbounds}', f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'n_jobs = {n_jobs}')
         assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
         assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
         assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter values"
         assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter values"
         assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
         assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
         assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
@@ -920,15 +920,15 @@
         select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
-        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+        self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
                                     'scoring':str(scoring), 'cv':str(self.cv),  'sample_weight':str(sample_weight)}
```

### Comparing `gmltools-0.0.84/src/gmltools/models/models_info.py` & `gmltools-0.0.85/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.85/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.85/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.85/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.85/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.85/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.85/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.84/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.85/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.84
+Version: 0.0.85
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.84/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.85/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

