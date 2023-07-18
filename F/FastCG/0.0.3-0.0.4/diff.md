# Comparing `tmp/FastCG-0.0.3.tar.gz` & `tmp/FastCG-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastCG-0.0.3.tar", last modified: Mon May 22 16:26:47 2023, max compression
+gzip compressed data, was "FastCG-0.0.4.tar", last modified: Tue Jul 18 10:35:02 2023, max compression
```

## Comparing `FastCG-0.0.3.tar` & `FastCG-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.542010 FastCG-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.506594 FastCG-0.0.3/FastCG/
--rw-rw-rw-   0        0        0       40 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.532526 FastCG-0.0.3/FastCG/generators/
--rw-rw-rw-   0        0        0    21815 2023-05-22 16:25:27.000000 FastCG-0.0.3/FastCG/generators/GeneratorBase.py
--rw-rw-rw-   0        0        0     8419 2023-05-22 16:25:27.000000 FastCG-0.0.3/FastCG/generators/ProbKnnGenerator.py
--rw-rw-rw-   0        0        0      162 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.541012 FastCG-0.0.3/FastCG/utils/
--rw-rw-rw-   0        0        0     1524 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/utils/SmartCondition.py
--rw-rw-rw-   0        0        0      148 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-04-30 18:15:03.000000 FastCG-0.0.3/FastCG/utils/logger.py
--rw-rw-rw-   0        0        0     6320 2023-05-22 16:25:27.000000 FastCG-0.0.3/FastCG/utils/util_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:26:47.518561 FastCG-0.0.3/FastCG.egg-info/
--rw-rw-rw-   0        0        0      452 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 16:26:47.000000 FastCG-0.0.3/FastCG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      452 2023-05-22 16:26:47.542010 FastCG-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8491 2023-04-30 18:15:03.000000 FastCG-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 16:26:47.542010 FastCG-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1070 2023-05-22 16:26:06.000000 FastCG-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:35:02.142428 FastCG-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-18 10:35:02.126319 FastCG-0.0.4/FastCG/
+-rw-rw-rw-   0        0        0       40 2023-04-30 18:15:03.000000 FastCG-0.0.4/FastCG/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:35:02.136445 FastCG-0.0.4/FastCG/generators/
+-rw-rw-rw-   0        0        0    24323 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/generators/GeneratorBase.py
+-rw-rw-rw-   0        0        0    23061 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/generators/Optika.py
+-rw-rw-rw-   0        0        0    11433 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/generators/ProbKnnGenerator.py
+-rw-rw-rw-   0        0        0      207 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:35:02.141431 FastCG-0.0.4/FastCG/utils/
+-rw-rw-rw-   0        0        0     4851 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/utils/Benchmark.py
+-rw-rw-rw-   0        0        0     4451 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/utils/Comparison.py
+-rw-rw-rw-   0        0        0    10353 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/utils/Face.py
+-rw-rw-rw-   0        0        0     6651 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/utils/GS.py
+-rw-rw-rw-   0        0        0     1524 2023-04-30 18:15:03.000000 FastCG-0.0.4/FastCG/utils/SmartCondition.py
+-rw-rw-rw-   0        0        0      280 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-04-30 18:15:03.000000 FastCG-0.0.4/FastCG/utils/logger.py
+-rw-rw-rw-   0        0        0     8658 2023-07-18 10:31:58.000000 FastCG-0.0.4/FastCG/utils/util_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:35:02.134297 FastCG-0.0.4/FastCG.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-07-18 10:35:02.000000 FastCG-0.0.4/FastCG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-07-18 10:35:02.000000 FastCG-0.0.4/FastCG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:35:02.000000 FastCG-0.0.4/FastCG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-07-18 10:35:02.000000 FastCG-0.0.4/FastCG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 10:35:02.000000 FastCG-0.0.4/FastCG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      452 2023-07-18 10:35:02.141431 FastCG-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8525 2023-07-18 10:31:58.000000 FastCG-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:35:02.142428 FastCG-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2023-07-18 10:34:51.000000 FastCG-0.0.4/setup.py
```

### Comparing `FastCG-0.0.3/FastCG/generators/GeneratorBase.py` & `FastCG-0.0.4/FastCG/generators/GeneratorBase.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,44 +5,57 @@
 from FastCG.utils import SmartCondition
 from FastCG.utils.logger import Logger
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.patches import Rectangle
 from IPython.display import display
-
+import json
+from sklearn.preprocessing import LabelEncoder
 
 
 class GeneratorBase():
 
     configuration_schema = {'features_to_change': {'type': list, 'schema': {'type': str}, 'required': True, 'minlength': 1},
                             'increase_only': {'type': list, 'schema': {'type': str}, 'required': False},
                             'decrease_only': {'type': list, 'schema': {'type': str}, 'required': False},
                             'max_features_to_change' : {'type': int, 'required': True, 'min': 1, 'default': 2},
+                            'Categorical_features' : {'type': list, 'schema': {'type': str}, 'required': False}, 
                             'target': {'type': str, 'required': True},
-                            'ID': {'type': str, 'required': False}}
+                            'ID': {'type': str, 'required': False}, 
+                            "feature_range": {'type': dict, 'required': False, 'schema': {'type': dict, 'schema': {'type': list, 'schema': {'type': float}}}},
+
+    }
     
-    def __init__(self, all_data, model, config, target, condition, verbose=0):
+    def __init__(self, all_data, model, config, target, condition, verbose=1):
         """
         Base class for all generators
 
         Parameters
         ----------
         all_data : list
             List of all data
         model : ModelBase
             Model to be used to generate data
-        config : dict
+        config : dict or str (json)
             Configuration for the generator
         verbose : int
             Verbosity level, 0 means only show warning, 1 means show info, 2 means show debug
         """
         self.all_data = all_data.copy()
+
+        # check if config is json
+        if isinstance(config, str):
+            try:
+                config = json.loads(config)
+            except:
+                raise ValueError("Invalid JSON format for config")
+        
         if not self._is_valid_config(config):
-            raise ValueError("Invalid config")
+            raise ValueError("Invalid config format (not the same as schema)")
         self.config = config
         self.verbose = verbose
         self.model = model
 
         Logger.set_verbosity(verbose)
 
         self.target = target
@@ -168,15 +181,23 @@
         Returns
         -------
         chunk : list
             List of data that contains counterfactual targets
             """
         data_to_generate = []
         for index, obs in chunk.iterrows():
-            pred_result = self.model.predict(obs.to_frame().T.drop(self.id, axis=1))
+            #turn obs features to categorical if needed 
+            obs = obs.to_frame().T
+            #convert the numerical features to int if needed 
+            for col in obs.columns:
+                if col not in self.config['categorical_features']:
+                    obs[col] = obs[col].astype(int)
+                if col in self.config["categorical_features"]:
+                    obs[col] = obs[col].astype("category")     
+            pred_result = self.model.predict(obs.drop(self.id, axis=1))
             if not self.smart_condition(pred_result):
                 preprocessed_obs = self._preprocess_counterfactual_targets(obs)
                 data_to_generate.append((obs,preprocessed_obs))
         return data_to_generate
 
     
     def generate(self, data, n_jobs=-1, chunk_size=1000) -> tuple:
@@ -420,36 +441,54 @@
         -------
         None
     
         """
         results = pd.DataFrame()
         counterfactual = counterfactual_list.get(key)
         self.obs = self.all_data[self.all_data[self.id] == key].copy().drop(self.config["target"], axis=1)
-        for col in self.all_data.columns:
-            if col != self.config["target"]:
+        category_cols = self.obs.select_dtypes(include=["object", "category"]).columns
+        for col in self.all_data.drop(self.config["target"], axis=1).columns:
+            if col not in category_cols:
                 results.loc[0, col] = self.obs[col].values[0].astype(int)
                 results.loc[1, col] = counterfactual[col].values[0].astype(int)
+            else:
+                results.loc[0, col] = self.obs[col].values[0]
+                results.loc[1, col] = counterfactual[col].values[0]
+        categorical_cols = results[results.select_dtypes(include=["object", "category"]).columns]
+        results = results[results.select_dtypes(exclude=["object", "category"]).columns].astype(str)
         results = results.T
         results.columns = ["Original", "Counterfactual"]
-        self.counterfactual = results["Counterfactual"].to_frame().T
-        results["Difference"] = results["Counterfactual"] - results["Original"]
-        results["% Difference"] = results["Difference"] / results["Original"] * 100 
-        results["% Difference"] = results["% Difference"].fillna(0)
-        results["% Difference"] = results["% Difference"].replace([np.inf, -np.inf], 0)
-        # print("In order to change the prediction from ", self.obs[self.config["target"]].values[0], " to ", counterfactual[self.config["target"]].values[0], " do the following:")
+        self.counterfactual = results["Counterfactual"].to_frame()
+        results["Difference"] = results["Counterfactual"].astype(float) - results["Original"].astype(float)
+        results["% Difference"] = (results["Difference"] / results["Original"].astype(float)) * 100
+        results = results.round(2)
+        #remmove null values and inf values
+        results = results.replace([np.inf, -np.inf, np.nan], 0)
+        #combine with the categorical columns 
+        for col in category_cols:
+            results.loc[col, "Original"] = categorical_cols[col].values[0]
+            results.loc[col, "Counterfactual"] = categorical_cols[col].values[1]
+            if results["Original"][col] == results["Counterfactual"][col]:
+                results.loc[col, "Difference"] = "Same category"
+                results.loc[col, "% Difference"] = "Same category"
+            else:
+                results.loc[col, "Difference"] = "Changed category"
+                results.loc[col, "% Difference"] = "Changed category"
         print("-------------------------------------------------------------------")
         print("ID: ", key)
         print("-------------------------------------------------------------------")
         for row in results.iterrows():
-            if row[0] == self.id:
-                    continue
-            if results["Difference"][row[0]] > 0:
+            if results["Difference"][row[0]] == "Same category":
+                print(row[0], " is the same")
+            elif results["Difference"][row[0]] != "Same category":
+                print(row[0], " changed from ", row[1]["Original"], " to ", row[1]["Counterfactual"])
+            if  isinstance(results["Difference"][row[0]], float) and results["Difference"][row[0]] > 0:
                 print("Increase ", row[0], " by ", row[1]["% Difference"], "%") 
                 print("Increase ", row[0], " by ", row[1]["Difference"], " units")
-            elif results["Difference"][row[0]] < 0:
+            elif isinstance(results["Difference"][row[0]], float) and results["Difference"][row[0]] < 0:
                 print("Decrease ", row[0], " by ", row[1]["% Difference"], "%")
                 print("Decrease ", row[0], " by ", row[1]["Difference"], " units")
 
         if show_plot:
             self.plot_the_counterfactual(self.obs, self.counterfactual)
 
         display(results)
@@ -514,17 +553,14 @@
 
 
         # mock df with 3 columns 
         df = counterfactual.reset_index(drop=True)
         #turn the df to int values
         df = df.astype(int)
         df2 = df2.astype(int)
-
-        print(df2.shape)
-        print(counterfactual.shape)
         # display(obs)
         # display(counterfactual)
         # diff df 
         df3 = df - df2
 
 
         # max of df and df2
@@ -540,14 +576,17 @@
 
         # df_gray contains the minimum value between df and df2
         df_gray = df_min
 
         # plot the data, overlay the plots in the following order green,red and then gray
         fig, ax = plt.subplots(figsize=(10, 5))
         plt.xticks(rotation=90)
+        plt.ylabel("Value")
+        plt.xlabel("Feature")
+        plt.ylim(0, 1.1 * df.values.max())
         # green bar is only outline of the bar
 
         width = 0.5
         ax.bar(df_green.columns, df_green.iloc[0], hatch='//', linewidth=2, edgecolor='green', fill=False, width=width)
         ax.bar(df_red.columns, df_red.iloc[0], color='gray',linewidth=2, edgecolor='red', hatch='//', width=width,  )
         ax.bar(df_gray.columns, df_gray.iloc[0], color='gray',linewidth=2, edgecolor='gray', hatch='', width=width)
 
@@ -559,15 +598,14 @@
             if col not in patches:
                 patches[col] = []
             patches[col].append(p)
 
 
         for index,col_x in enumerate(patches):
 
-
             label_data = df3.iloc[0, index].round(2)
             if label_data > 0:
                 label = u'$\u25B2$' + f'{label_data}'
             elif label_data < 0:
                 label = u'$\u25BC$' + f'{label_data}'
             else:
                 label = ''
@@ -577,7 +615,11 @@
             width = patches[col_x][0].get_width() / 2
             # add the text label
             ax.annotate(label,
                         (col_x + width, max_height),
                         ha='center', va='center', 
                         fontsize=11, color='green' if label_data > 0 else 'red', 
                         xytext=(0, 8), textcoords='offset points')
+            
+        # add the legend
+        ax.legend(['Increase', 'Decrease', 'No Change'], loc='upper left', bbox_to_anchor=(1, 1))
+        plt.show()
```

### Comparing `FastCG-0.0.3/FastCG/generators/ProbKnnGenerator.py` & `FastCG-0.0.4/FastCG/generators/ProbKnnGenerator.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,31 +26,59 @@
         self.features_to_use = \
             find_feature_improtance_Anova(
                 self.data_matching_condition, 
                 self.config["max_features_to_change"],
                 self.config["features_to_change"], 
                 self.config["target"]
                 )
+
+        self.features_to_use = self.config["features_to_change"]
         if "increase_only" in self.config and self.config["increase_only"] is not None:
             self.features_increase_only = self.config["increase_only"]
         else: 
             self.features_increase_only = []
+            
         if "decrease_only" in self.config and self.config["decrease_only"] is not None:
             self.features_decrease_only = self.config["decrease_only"]
         else: 
             self.features_decrease_only = []
+
         Logger.info("Features to use: " + str(self.features_to_use))
         Logger.info("Features to increase: " + str(self.features_increase_only))
         Logger.info("Features to decrease: " + str(self.features_decrease_only))
 
+        # Find all categorical features based on the dataset types
+        # this is regardless of the config as we need to know the categorical features to properly handle the distance calculation
+        self.categorical_features = self.data_matching_condition[self.features_to_use].select_dtypes(include=['object', 'category']).columns
+        if "categorical_features" in self.config and self.config["categorical_features"] is not None:
+            # Add the categorical features from the config to the list of categorical features found in the dataset
+            self.categorical_features = self.categorical_features.union(self.config["categorical_features"])
+            Logger.info("You have provided the following categorical features: " + str(self.config["categorical_features"]))
+        elif len(self.categorical_features) > 0:
+            Logger.info("We have found " + str(len(self.categorical_features)) + " categorical features: " + str(self.categorical_features))
+
+        if "feature_range" in self.config and self.config["feature_range"] is not None:
+            self.feature_range = self.config["feature_range"]
+        else:
+            self.feature_range = (self.data_matching_condition[self.features_to_use].min(), self.data_matching_condition[self.features_to_use].max())
+            Logger.info("Feature range: " + str(self.feature_range))
+
+        self.all_data = self.all_data.copy()
         self.all_data_features_to_use = self.all_data[self.features_to_use]
         self.all_data["ID"] = self.all_data.index
         self.id = "ID"
-        self.normalizer = StandardScaler().fit(self.all_data_features_to_use)
-        self.data_normalized_features_to_use = self.normalizer.transform(self.all_data_features_to_use)
+        #check if we have categorical features 
+        categorical_features_in_features_to_change = self.all_data_features_to_use.select_dtypes(include=['object', 'category']).columns
+        if len(categorical_features_in_features_to_change) > 0:
+            features_to_normalize = self.all_data_features_to_use.drop(categorical_features_in_features_to_change, axis=1)
+            self.normalizer = StandardScaler().fit(features_to_normalize)
+            self.data_normalized_features_to_use = self.normalizer.transform(features_to_normalize)
+        else:
+            self.normalizer = StandardScaler().fit(self.all_data_features_to_use)
+            self.data_normalized_features_to_use = self.normalizer.transform(self.all_data_features_to_use)
         
         self.n_components = choose_pca_components(self.data_normalized_features_to_use, 0.75)
         self.pca = PCA(n_components=self.n_components).fit(self.data_normalized_features_to_use)
         self.features_pca = ['principal component ' + str(i) for i in range(1, self.n_components+1)]
         self.data_pca = convert_to_pca(self.data_matching_condition, self.pca, self.normalizer, self.features_to_use, self.features_pca)
         self.data_centroid, self.kmean_lables = find_centroid(self.data_pca.drop(self.config["target"], axis=1).copy()[self.features_pca],features_pca=self.features_pca)
 
@@ -58,15 +86,15 @@
         self.nbrs = NearestNeighbors(n_neighbors=2).fit(self.data_centroid) #TODO: move n_neighbors to config
 
     def _preprocess_generate(self, data) -> None:
         self.current_data = data
         self.current_data["ID"] = self.current_data.index
     
     def _preprocess_counterfactual_targets(self, obs) -> pd.DataFrame:
-        data_to_genrate = convert_to_pca(obs.to_frame().T, self.pca, self.normalizer, self.features_to_use, self.features_pca)
+        data_to_genrate = convert_to_pca(obs, self.pca, self.normalizer, self.features_to_use, self.features_pca)
         data_to_genrate = data_to_genrate.fillna(0)
         return data_to_genrate
 
     def __init__(self, all_data, model, config, target, condition,verbose=0):
         super().__init__(all_data, model, config, target, condition,verbose)
 
     def _generate_single(self, original_obs, processed_obs):
@@ -75,26 +103,31 @@
         base_obs = self.current_data[self.current_data[self.id] == processed_obs[self.id].values[0]]
         cf = {}
         for idx in indices:
             counterfactual = processed_obs.copy()
             for feature in self.features_pca: 
                 counterfactual[feature] = self.data_pca[feature].iloc[idx]
             
-            counterfactual = convert_from_pca(counterfactual,base_obs, self.pca, self.normalizer, self.features_to_use, self.features_pca)
+            counterfactual = convert_from_pca(counterfactual, base_obs, self.pca, self.normalizer, self.features_to_use, self.features_pca)
             # to_continue = False
             for feature in self.features_increase_only:
-                if counterfactual[feature].values[0] < original_obs[feature]:
-                    counterfactual[feature].values[0] = original_obs[feature]*2
+                if counterfactual[feature].values[0] < original_obs[feature].values[0]:
+                    counterfactual[feature].values[0] = original_obs[feature].values[0]*2
             for feature in self.features_decrease_only:
-                if counterfactual[feature].values[0] > original_obs[feature]:
-                    counterfactual[feature].values[0] = original_obs[feature]/2            
+                if counterfactual[feature].values[0] > original_obs[feature].values[0]:
+                    counterfactual[feature].values[0] = original_obs[feature].values[0]/2
+            #check if the counterfactual is in the feature range the user provided 
+            for key, value in self.feature_range.items():
+                if counterfactual[key].values[0] > (base_obs[key].values[0])*(1+value[1]):
+                    counterfactual[key].values[0] = (base_obs[key].values[0])*(1+value[1])
+                if counterfactual[key].values[0] < (base_obs[key].values[0])*(1+value[0]):
+                    counterfactual[key].values[0] = (base_obs[key].values[0])*(1+value[0])
             tmp_counterfactual = counterfactual.copy()
             if self.config["target"] in tmp_counterfactual:
                     tmp_counterfactual = counterfactual.drop(self.config["target"], axis=1)
-
             if self.smart_condition.check(self.model.predict(tmp_counterfactual.drop(self.id, axis=1)))[0]:
                 # return counterfactual
                 distance = obs_distance(counterfactual.copy(), base_obs.copy(), self.config["target"])
                 if distance not in cf:
                     cf[distance] = counterfactual.copy()
         if cf:
             return cf[min(cf.keys())]
@@ -133,26 +166,33 @@
             for member in cluster_members[:max_index]:
                 idx = self.data_pca.iloc[member].name
                 if idx not in index:
                     index.append(idx)
         
         weights = []
         data_cluster = self.data_pca.loc[index] 
+        for feature in data_cluster.select_dtypes(include=['category']).columns:
+            data_cluster[feature] = data_cluster[feature].astype('category').cat.codes
+            obs_original[feature] = obs_original[feature].astype('category').cat.codes
         for feature in data_cluster.drop(self.config["target"], axis=1).columns: 
             if feature == self.id:
                 weights.append(0)  
             elif feature not in self.features_pca: 
                 weights.append(1)
             else:
                 weights.append(0)
         w_minkowski = partial(minkowski, p=2, w=weights)
         n_neigh = min(5, len(data_cluster))
-        nbrs = NearestNeighbors(n_neighbors=n_neigh, metric=w_minkowski).fit(data_cluster.drop(self.config["target"], axis=1))
-        indices = nbrs.kneighbors(obs_original, return_distance=False)
-        return indices[0]
+        try:
+            nbrs = NearestNeighbors(n_neighbors=n_neigh, metric=w_minkowski).fit(data_cluster.drop(self.config["target"], axis=1))
+            indices = nbrs.kneighbors(obs_original, return_distance=False)
+            return indices[0]
+        except Exception as e:
+            Logger.error("Error in KNN on cluster: " + str(e))
+            raise e
     
     def _postprocess_valid_data(self, data) -> list:        
         improve_cf = {}
         for couterfactual in tqdm(data, desc="Improving counterfactuals with binary search"):
             id_key = couterfactual[self.id].values[0]
             original_obs = self.all_data[self.all_data[self.id] == couterfactual[self.id].values[0]].drop(self.config["target"], axis=1).copy()
             cf = couterfactual.copy()
```

### Comparing `FastCG-0.0.3/FastCG/utils/SmartCondition.py` & `FastCG-0.0.4/FastCG/utils/SmartCondition.py`

 * *Files identical despite different names*

### Comparing `FastCG-0.0.3/FastCG/utils/logger.py` & `FastCG-0.0.4/FastCG/utils/logger.py`

 * *Files identical despite different names*

### Comparing `FastCG-0.0.3/README.md` & `FastCG-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,19 @@
 # step two - import and create a generator
 
 from FastCG.generators import ProbKnnGenerator
 
 # step three - create a config for the generator
 
 config = {"features_to_change": ['Current Loan Amount', 'Term', 'Credit Score', 'Annual Income', 'Monthly Debt'],
-              "increase_only": ['Credit Score', 'Annual Income'],
-              "decrease_only": ['Monthly Debt'],
+              "increase_only": ['Credit Score', 'Annual Income'], # optional
+              "decrease_only": ['Monthly Debt'], # optional
               "max_features_to_change": 2,
-              "ID": 'Loan ID',
-              "target": 'Loan Status'
+              "ID": 'Loan ID', # optional
+              "target": 'Loan Status' 
               }
 
 # step four - create a generator
 cfg_generator = ProbKnnGenerator(df,log_reg,config,target=1,condition='==') 
 
 # step five - generate the counterfactuals
```

### Comparing `FastCG-0.0.3/setup.py` & `FastCG-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Counterfactual Generation Package'
 LONG_DESCRIPTION = 'A package that makes it easy generate counterfactuals in a fast manner'
 
 setup(
     name="FastCG",
     version=VERSION,
     description=DESCRIPTION,
```

