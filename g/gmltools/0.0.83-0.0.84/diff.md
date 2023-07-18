# Comparing `tmp/gmltools-0.0.83.tar.gz` & `tmp/gmltools-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.83.tar", last modified: Wed Jun 28 09:37:46 2023, max compression
+gzip compressed data, was "gmltools-0.0.84.tar", last modified: Tue Jul 18 13:00:55 2023, max compression
```

## Comparing `gmltools-0.0.83.tar` & `gmltools-0.0.84.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.438974 gmltools-0.0.83/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.83/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.83/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-06-28 09:37:46.438112 gmltools-0.0.83/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.83/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.403406 gmltools-0.0.83/dist/
--rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.83/dist/gmltools-0.0.80.tar.gz
--rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.83/dist/gmltools-0.0.81.tar.gz
--rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.83/dist/gmltools-0.0.82.tar.gz
--rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.83/environment.txt
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.83/gmltools.yml
--rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.83/gmltools2.yml
--rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.83/gmltools3.yml
--rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.83/gmltools4.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.83/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-06-28 09:36:57.000000 gmltools-0.0.83/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 09:37:46.438974 gmltools-0.0.83/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-06-28 09:36:47.000000 gmltools-0.0.83/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.307060 gmltools-0.0.83/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.406433 gmltools-0.0.83/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.83/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.83/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.417984 gmltools-0.0.83/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.83/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    45883 2023-06-28 09:35:43.000000 gmltools-0.0.83/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.429950 gmltools-0.0.83/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.83/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.83/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.83/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.83/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   160613 2023-06-14 08:54:19.000000 gmltools-0.0.83/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.83/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    33620 2023-06-28 09:35:46.000000 gmltools-0.0.83/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.432940 gmltools-0.0.83/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.83/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.83/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.83/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.437115 gmltools-0.0.83/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.83/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.83/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.83/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.83/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:37:46.412998 gmltools-0.0.83/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-06-28 09:37:45.000000 gmltools-0.0.83/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-06-28 09:37:46.000000 gmltools-0.0.83/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 09:37:45.000000 gmltools-0.0.83/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-06-28 09:37:45.000000 gmltools-0.0.83/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 09:37:45.000000 gmltools-0.0.83/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.597740 gmltools-0.0.84/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.84/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.84/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-07-18 13:00:55.597740 gmltools-0.0.84/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.84/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.473860 gmltools-0.0.84/dist/
+-rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.84/dist/gmltools-0.0.80.tar.gz
+-rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.84/dist/gmltools-0.0.81.tar.gz
+-rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.84/dist/gmltools-0.0.82.tar.gz
+-rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.84/environment.txt
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.84/gmltools.yml
+-rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.84/gmltools2.yml
+-rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.84/gmltools3.yml
+-rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.84/gmltools4.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.84/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-07-18 13:00:16.000000 gmltools-0.0.84/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:00:55.598739 gmltools-0.0.84/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-07-18 13:00:08.000000 gmltools-0.0.84/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.328127 gmltools-0.0.84/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.490912 gmltools-0.0.84/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.84/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.84/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.512910 gmltools-0.0.84/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.84/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    45883 2023-06-29 11:50:55.000000 gmltools-0.0.84/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.544165 gmltools-0.0.84/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.84/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.84/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.84/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.84/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   160542 2023-07-18 12:59:28.000000 gmltools-0.0.84/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.84/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.84/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.566185 gmltools-0.0.84/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.84/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.84/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.84/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.596739 gmltools-0.0.84/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.84/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.84/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.84/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.84/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:55.497913 gmltools-0.0.84/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-07-18 13:00:55.000000 gmltools-0.0.84/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 13:00:54.000000 gmltools-0.0.84/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.83/LICENSE` & `gmltools-0.0.84/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/Models.ipynb` & `gmltools-0.0.84/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/PKG-INFO` & `gmltools-0.0.84/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.83
+Version: 0.0.84
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.83/README.md` & `gmltools-0.0.84/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/dist/gmltools-0.0.80.tar.gz` & `gmltools-0.0.84/dist/gmltools-0.0.80.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/dist/gmltools-0.0.81.tar.gz` & `gmltools-0.0.84/dist/gmltools-0.0.81.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/dist/gmltools-0.0.82.tar.gz` & `gmltools-0.0.84/dist/gmltools-0.0.82.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/gmltools.yml` & `gmltools-0.0.84/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/gmltools2.yml` & `gmltools-0.0.84/gmltools2.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/gmltools3.yml` & `gmltools-0.0.84/gmltools3.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/gmltools4.yml` & `gmltools-0.0.84/gmltools4.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/mltools.yml` & `gmltools-0.0.84/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/pyproject.toml` & `gmltools-0.0.84/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.83"
+version = "0.0.84"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.83/setup.py` & `gmltools-0.0.84/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.83',
+    'version': '0.0.84',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.83/src/gmltools/To_Do.txt` & `gmltools-0.0.84/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/eda/eda.py` & `gmltools-0.0.84/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/models/bayes.py` & `gmltools-0.0.84/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.84/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/models/dummy_model.py` & `gmltools-0.0.84/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/models/model.py` & `gmltools-0.0.84/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -830,16 +830,15 @@
         
 
 
     #do the same for knn_classifier
     def KNN_Classifier(self,ordinal_cat_cols=None, scoring='accuracy',
                         grid_params={'KNN__n_neighbors': [3,10,25,60]},
                         random_params=None, random_n_iter=10,  bayes_pbounds=None,
-                        bayes_int_params=None, bayes_n_iter=30, sample_weight=None,
-                        random_state=None, n_jobs=-1):
+                        bayes_int_params=None, bayes_n_iter=30, sample_weight=None, n_jobs=-1):
           
         """
         This method performs a K-Nearest Neighbors classification model with grid search or bayesian optimization.
 
         Parameters
         ----------
         X_train : pandas dataframe
@@ -912,15 +911,15 @@
             assert all('KNN__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'KNN__'"
         elif bayes_pbounds is not None:
             assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
             assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
         
         preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
         pipe = Pipeline(steps=[('Prep', preprocessor),
-                            ('KNN', KNeighborsClassifier(n_jobs=n_jobs, random_state=random_state))]) # Model always the last step
+                            ('KNN', KNeighborsClassifier(n_jobs=n_jobs))]) # Model always the last step
         #Select Grid Search, Random Search or Bayesian Optimization
         select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
```

### Comparing `gmltools-0.0.83/src/gmltools/models/models_info.py` & `gmltools-0.0.84/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.84/src/gmltools/models/timeseriesplit.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,11 +802,11 @@
         test_days=[]
         train_real_index,test_real_index=self.get_index_splits(X)
         for day in test_real_index:
             day_=np.unique(day.date)
             test_days.append(day_[0].strftime("%Y-%m-%d"))
         return test_days
     def __repr__(self):
-        return "TimeSeriesWindowSplit(initial={}, increment_size={}, gap={}, intra_gap={})".format(
+        return "TimeSeriesWindowGapSplit(initial={}, increment_size={}, gap={}, intra_gap={})".format(
             self.initial, self.increment_size, self.gap, self.intra_gap
         )
```

### Comparing `gmltools-0.0.83/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.84/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.84/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.84/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.84/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.84/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.83/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.84/src/gmltools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.83
+Version: 0.0.84
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.83/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.84/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

