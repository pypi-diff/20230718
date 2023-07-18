# Comparing `tmp/kuplift-0.0.2.tar.gz` & `tmp/kuplift-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuplift-0.0.2.tar", last modified: Wed Jul 12 19:13:17 2023, max compression
+gzip compressed data, was "kuplift-0.0.3.tar", last modified: Tue Jul 18 13:29:33 2023, max compression
```

## Comparing `kuplift-0.0.2.tar` & `kuplift-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:13:17.336010 kuplift-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 19:13:07.000000 kuplift-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-12 19:13:17.336010 kuplift-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-12 19:13:07.000000 kuplift-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:13:17.336010 kuplift-0.0.2/kuplift/
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/BayesianDecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/BayesianRandomForest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/BinaryDiscretizationFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/FeatureSelection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/HelperFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/Tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/UMODL_SearchAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/UnivariateEncoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-12 19:13:07.000000 kuplift-0.0.2/kuplift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:13:17.336010 kuplift-0.0.2/kuplift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-12 19:13:17.000000 kuplift-0.0.2/kuplift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-12 19:13:17.000000 kuplift-0.0.2/kuplift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:13:17.000000 kuplift-0.0.2/kuplift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 19:13:17.000000 kuplift-0.0.2/kuplift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 19:13:17.000000 kuplift-0.0.2/kuplift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 19:13:17.336010 kuplift-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-12 19:13:07.000000 kuplift-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:13:17.336010 kuplift-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-12 19:13:07.000000 kuplift-0.0.2/test/test.py
--rw-r--r--   0 runner    (1001) docker     (123)   149105 2023-07-12 19:13:07.000000 kuplift-0.0.2/test/test_BayesianDecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)   146337 2023-07-12 19:13:07.000000 kuplift-0.0.2/test/test_BayesianRandomForest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-12 19:13:07.000000 kuplift-0.0.2/test/test_FeatureSelection.py
--rw-r--r--   0 runner    (1001) docker     (123)   246158 2023-07-12 19:13:07.000000 kuplift-0.0.2/test/test_UnvariateEncoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.791177 kuplift-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 13:29:13.000000 kuplift-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 13:29:33.791177 kuplift-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-18 13:29:13.000000 kuplift-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.787177 kuplift-0.0.3/kuplift/
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/BayesianDecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/BayesianRandomForest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/BinaryDiscretizationFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/FeatureSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/HelperFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30719 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/UMODL_SearchAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/UnivariateEncoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-18 13:29:13.000000 kuplift-0.0.3/kuplift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.791177 kuplift-0.0.3/kuplift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 13:29:33.000000 kuplift-0.0.3/kuplift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 13:29:33.791177 kuplift-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-18 13:29:13.000000 kuplift-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:29:33.791177 kuplift-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149105 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_BayesianDecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146337 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_BayesianRandomForest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_FeatureSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246158 2023-07-18 13:29:13.000000 kuplift-0.0.3/test/test_UnvariateEncoding.py
```

### Comparing `kuplift-0.0.2/LICENSE` & `kuplift-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.2/README.md` & `kuplift-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 
-## Bibliothèque Kuplift
+## kuplift package
 
+<p  align="center">
+  <img src="https://raw.githubusercontent.com/UData-Orange/kuplift/main/docs/source/logo.png" width="310" />
+</p>
 
-Kuplift is a _Python_ package that provides a series of uplift modeling methods based on recent research work. Kuplift allows users to easily use the following algorithms:
 
-1. Encoding data using a discretization method for treatment effect (uplift) modeling called _UMODL_[^fn1]
+kuplift is a _Python_ package that provides a series of uplift modeling methods based on recent research work. kuplift allows users to easily use the following algorithms:
+
+1. Encoding data using a discretization method for treatment effect (uplift) modeling called _UMODL_.
     
-2.  Variable selection for uplift modeling with _UMODL-FS_.[^fn1]
+2.  Variable selection for uplift modeling with _UMODL-FS_.
     
-3. Learning a Bayesian decision tree model for uplift modeling with _UB-DT_.[^fn2]
+3. Learning a Bayesian decision tree model for uplift modeling with _UB-DT_.
     
-4.  Learning a random forest model for uplift modeling with _UB-RF_.[^fn2]
+4.  Learning a random forest model for uplift modeling with _UB-RF_.
 
 **How to install**:
 
 ```python
-pip install Kuplift
+pip install kuplift
 ```
 
 **User Guide**:
 
 ```python
+import kuplift as kp
 import pandas as pd
 
 df = pd.read_csv("dataname.csv")
 
-# Discrétisation univariée:
-ue = UnivariateEncoding()
+# Univariate variable transformation:
+ue = kp.UnivariateEncoding()
 encoded_data = ue.fit_transform(df, "treatment", "outcome")
 
-# Sélection de variables
-fs = FeatureSelection()
+# Feature selection
+fs = kp.FeatureSelection()
 important_vars = fs.filter(df, "treatment", "outcome")
 
-# Arbre de décisions
-tree = BayesianDecisionTree(df, "treatment", "outcome")
+# Uplift Bayesian Decision Tree
+tree = kp.BayesianDecisionTree(df, "treatment", "outcome")
 tree.fit()
 preds = tree.predict(df[column_names])
 
-# Forêt d'arbres
-forest = BayesianRandomForest(df, "treatment", "outcome", nb_trees)
+# Uplift Bayesian Random Forest
+forest = kp.BayesianRandomForest(df, "treatment", "outcome", nb_trees)
 forest.fit()
 preds = forest.predict(df[features])
 ```
 
+**Documentation**:
+
+Refer to the documentation at https://udata-orange.github.io/kuplift/
+
+**References**:
 
-[^fn1]: Rafla, M., Voisine, N., Crémilleux, B., & Boullé, M. (2023, March). A non-parametric bayesian approach for uplift discretization and feature selection. **_ECML PKDD 2022_**
+Rafla, M., Voisine, N., Crémilleux, B., & Boullé, M. (2023, March). A non-parametric bayesian approach for uplift discretization and feature selection. **_ECML PKDD 2022_**
 
-[^fn2]: Rafla, M., Voisine, N., & Crémilleux, B. (2023, May). Parameter-free Bayesian decision trees for uplift modeling. **_PAKDD 2023_**
+Rafla, M., Voisine, N., & Crémilleux, B. (2023, May). Parameter-free Bayesian decision trees for uplift modeling. **_PAKDD 2023_**
```

### Comparing `kuplift-0.0.2/kuplift/BayesianDecisionTree.py` & `kuplift-0.0.3/kuplift/BayesianDecisionTree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 from math import log
 from .HelperFunctions import (
     log_fact,
     universal_code_natural_numbers,
@@ -82,36 +82,42 @@
             )  # Dictionary containing Nodes as key and their values are another dictionary each with attribute:CostSplit
 
             for terminal_node in self.terminal_nodes:
                 # This if condition is here to not to repeat calculations of candidate splits
                 if terminal_node.candidate_splits_vs_criterion is None:
                     node_vs_candidate_splits_costs[
                         terminal_node
-                    ] = terminal_node.discretize_vars_and_get_attributes_splits_costs()
+                    ] = (
+                        terminal_node.discretize_vars_and_get_attributes_splits_costs()
+                    )
                 else:
                     node_vs_candidate_splits_costs[
                         terminal_node
                     ] = terminal_node.candidate_splits_vs_criterion.copy()
 
                 if len(node_vs_candidate_splits_costs[terminal_node]) == 0:
                     continue
 
                 # Update Costs
                 for attribute in node_vs_candidate_splits_costs[terminal_node]:
                     if attribute in self.feature_subset:
-                        node_vs_candidate_splits_costs[terminal_node][attribute] += (
+                        node_vs_candidate_splits_costs[terminal_node][
+                            attribute
+                        ] += (
                             self.prob_kt
                             + self.prob_attribute_selection
                             + encoding_of_internal_and_leaves_and_w_with_extra_nodes
                             + self.leaf_prior
                             + self.tree_likelihood
                             + self.prior_of_internal_nodes
                         )
                     else:
-                        node_vs_candidate_splits_costs[terminal_node][attribute] += (
+                        node_vs_candidate_splits_costs[terminal_node][
+                            attribute
+                        ] += (
                             prob_kt_plus_one
                             + encoding_of_internal_and_leaves_and_w_with_extra_nodes
                             + prob_of_attribute_selection_among_subset_attributes_plus_one
                             + self.leaf_prior
                             + self.tree_likelihood
                             + self.prior_of_internal_nodes
                         )
@@ -122,29 +128,33 @@
                     node_vs_candidate_splits_costs[terminal_node],
                     key=node_vs_candidate_splits_costs[terminal_node].get,
                 )
 
                 node_vs_best_attribute_corresponding_to_the_best_cost[
                     terminal_node
                 ] = key_of_the_minimal_val
-                node_vs_best_cost[terminal_node] = node_vs_candidate_splits_costs[
+                node_vs_best_cost[
                     terminal_node
-                ][key_of_the_minimal_val]
+                ] = node_vs_candidate_splits_costs[terminal_node][
+                    key_of_the_minimal_val
+                ]
 
             if len(list(node_vs_best_cost)) == 0:
                 break
 
             optimal_node_attribute_to_split_up = min(
                 node_vs_best_cost, key=node_vs_best_cost.get
             )
             optimal_val = node_vs_best_cost[optimal_node_attribute_to_split_up]
             optimal_node = optimal_node_attribute_to_split_up
-            optimal_attribute = node_vs_best_attribute_corresponding_to_the_best_cost[
-                optimal_node_attribute_to_split_up
-            ]
+            optimal_attribute = (
+                node_vs_best_attribute_corresponding_to_the_best_cost[
+                    optimal_node_attribute_to_split_up
+                ]
+            )
 
             if optimal_val < self.tree_criterion:
                 self.tree_criterion = optimal_val
                 if optimal_attribute not in self.feature_subset:
                     self.feature_subset.append(optimal_attribute)
                     self.k_t += 1
                 new_left_leaf, new_right_leaf = optimal_node.perform_split(
```

### Comparing `kuplift-0.0.2/kuplift/BayesianRandomForest.py` & `kuplift-0.0.3/kuplift/BayesianRandomForest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 from math import log
 import numpy as np
 import random
 from .HelperFunctions import (
@@ -175,32 +175,33 @@
         Dataframe containing data.
     treatment_col : pd.Series
         Treatment column.
     outcome_col : pd.Series
         Outcome column.
     n_trees : int
         Number of trees in a forest.
+    vars_subset : boolean
+        Use a random subset of the variables for each tree in the forest
     """
 
     def __init__(
         self,
         data,
         treatment_col,
         y_col,
         n_trees,
-        not_all_vars=False,
-        weighted_average=False,
+        vars_subset=False,
         random_state=10,
     ):
         self.list_of_trees = []
         self.data = data
         random.seed(random_state)
-        self.weighted_average = weighted_average
+        
         # Randomly select columns for the data
-        if not_all_vars:
+        if vars_subset:
             cols = list(self.data.columns)
             cols.remove(treatment_col)
             cols.remove(y_col)
             print("cols before are ", cols)
             cols = random.sample(cols, int(np.sqrt(len(cols))))
             print("cols after are ", cols)
             self.data = self.data[cols + [treatment_col, y_col]]
@@ -211,29 +212,31 @@
     def fit(self):
         """
         Fit a decision tree algorithm
         """
         for tree in self.list_of_trees:
             tree.grow_tree()
 
-    def predict(self, X_test):
+    def predict(self, X_test, weighted_average=False):
         """
         Predict the uplift value for each example in X_test
 
         Parameters
         ----------
         X_test : pd.Dataframe
             Dataframe containing test data.
+        weighted_average : boolean
+            Give a weight for the predictions of each tree according to its cost (default = False)
 
         Returns
         -------
         y_pred_list(ndarray, shape=(num_samples, 1))
             An array containing the predicted uplift for each sample.
         """
-        if self.weighted_average == False:
+        if weighted_average == False:
             list_of_preds = []
 
             for tree in self.list_of_trees:
                 list_of_preds.append(np.array(tree.predict(X_test)))
             return np.mean(list_of_preds, axis=0)
         else:
             list_of_criterion = []
```

### Comparing `kuplift-0.0.2/kuplift/BinaryDiscretizationFunctions.py` & `kuplift-0.0.3/kuplift/BinaryDiscretizationFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 import bisect
 from math import log
 import pandas as pd
 import time
@@ -107,20 +107,24 @@
     res_t += res_t_temp
 
     prior_two_tmp = res_t
     stop_counter(0)
 
     right_merge_w = None
     if not null_model:
-        if (prior_one_tmp + likelihood_one_tmp) < (prior_two_tmp + likelihood_two_tmp):
+        if (prior_one_tmp + likelihood_one_tmp) < (
+            prior_two_tmp + likelihood_two_tmp
+        ):
             right_merge_w = 0
         else:
             right_merge_w = 1
     else:
-        if (prior_one_tmp + likelihood_one_tmp) > (prior_two_tmp + likelihood_two_tmp):
+        if (prior_one_tmp + likelihood_one_tmp) > (
+            prior_two_tmp + likelihood_two_tmp
+        ):
             right_merge_w = 0
         else:
             right_merge_w = 1
 
     prior_one = (1 - right_merge_w) * prior_one_tmp
     prior_two = right_merge_w * prior_two_tmp
     likelihood_one = (1 - right_merge_w) * likelihood_one_tmp
@@ -128,15 +132,20 @@
     sum_of_priors_and_likelihoods = (
         prior_one + prior_two + likelihood_one + likelihood_two
     )
     return sum_of_priors_and_likelihoods
 
 
 def split_interval(
-    df, col_name, treatment_col_name, output_col_name, null_model_value, granularite=16
+    df,
+    col_name,
+    treatment_col_name,
+    output_col_name,
+    null_model_value,
+    granularite=16,
 ):  # i is interval index in IntervalsList
     data = df[[col_name, treatment_col_name, output_col_name]].values.tolist()
 
     data = SortedKeyList(data, key=itemgetter(0))
     data_nitj = [0, 0, 0, 0]  # The frequency of treatment class
     for interval_list in data:
         data_nitj[int((interval_list[1] * 2) + interval_list[2])] += 1
@@ -149,15 +158,17 @@
     # Get all the unique values in the data i.e All unique values between left and right bounds
     unique_values_in_both_intervals = list(
         data.irange_key(left_bound, right_bound, (including_left_border, True))
     )
     unique_values_in_both_intervals = list(
         map(itemgetter(0), unique_values_in_both_intervals)
     )
-    unique_values_in_both_intervals = list(set(unique_values_in_both_intervals))
+    unique_values_in_both_intervals = list(
+        set(unique_values_in_both_intervals)
+    )
     unique_values_in_both_intervals.sort()  # Sort the unique values
 
     splits = {}
 
     previous_left_interval = [0, 0, 0, 0]
     prev_val = None
 
@@ -170,26 +181,32 @@
 
         if prev_val is None:  # Enters here only for the first unique value
             left_split = list(
                 data.irange_key(left_bound, val, (True, True))
             )  # Get a list of all data between left_bound and current unique value
             left_interval = [0, 0, 0, 0]
             for interval_list in left_split:
-                left_interval[int((interval_list[1] * 2) + interval_list[2])] += 1
+                left_interval[
+                    int((interval_list[1] * 2) + interval_list[2])
+                ] += 1
         else:
             left_split = list(data.irange_key(prev_val, val, (False, True)))
             left_interval = [0, 0, 0, 0]
             for interval_list in left_split:
-                left_interval[int((interval_list[1] * 2) + interval_list[2])] += 1
+                left_interval[
+                    int((interval_list[1] * 2) + interval_list[2])
+                ] += 1
             """
             New Left Interval frequencies is the sum of the previous left
             interval (bounded between Smallest value and prev_val) and the
             new left interval (bounded between prev_val and val)
             """
-            left_interval = list(map(add, previous_left_interval, left_interval))
+            left_interval = list(
+                map(add, previous_left_interval, left_interval)
+            )
 
         # the nitj for the right split (Which we call the right_interval)
         # will be the difference between the old nitj and the left_interval
         prev_val = val
         previous_left_interval = left_interval.copy()
 
         """
@@ -222,15 +239,17 @@
                 )
             splits[val] = split_criterion_val_left_and_right
     best_split = None
 
     # If dictionary splits contain value, get the minimal one
     if splits:
         best_split = min(splits, key=splits.get)  # To be optimized maybe
-        left_split = list(data.irange_key(left_bound, best_split, (True, True)))
+        left_split = list(
+            data.irange_key(left_bound, best_split, (True, True))
+        )
         left_interval = [0, 0, 0, 0]
         for interval_list in left_split:
             left_interval[int((interval_list[1] * 2) + interval_list[2])] += 1
         right_interval = list(map(sub, data_nitj, left_interval))
 
         index_of_last_row_in_left_data = bisect.bisect_right(
             df[col_name].tolist(), best_split
@@ -253,15 +272,19 @@
 
 
 def exec(df, attributeToDiscretize, treatment_col_name, output_col_name):
     null_model_value = calc_null_model(
         df, attributeToDiscretize, treatment_col_name, output_col_name
     )
     return split_interval(
-        df, attributeToDiscretize, treatment_col_name, output_col_name, null_model_value
+        df,
+        attributeToDiscretize,
+        treatment_col_name,
+        output_col_name,
+        null_model_value,
     )
 
 
 def umodl_binary_discretization(data, T, Y, attributeToDiscretize):
     df = pd.DataFrame()
     df = data.copy()
     treatment_col_name = T.name
```

### Comparing `kuplift-0.0.2/kuplift/FeatureSelection.py` & `kuplift-0.0.3/kuplift/FeatureSelection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
-import sys
+import multiprocessing as mp
 from .HelperFunctions import preprocess_data
 from .UMODL_SearchAlgorithm import execute_greedy_search_and_post_opt
 
 
 class FeatureSelection:
     """
     The FeatureSelection implements the feature selection algorithm 'UMODL-FS'
@@ -57,46 +57,118 @@
                 var_vs_importance[feature],
                 var_vs_disc[feature],
             ) = execute_greedy_search_and_post_opt(
                 data[[feature, treatment_col, y_col]]
             )
         # sort the dictionary by values in ascending order
         var_vs_importance = {
-            k: v for k, v in sorted(var_vs_importance.items(), key=lambda item: item[1])
+            k: v
+            for k, v in sorted(
+                var_vs_importance.items(), key=lambda item: item[1]
+            )
         }
         return var_vs_importance
 
-    def filter(self, data, treatment_col, y_col):
+    @staticmethod
+    def get_the_best_var_parallel(args):
+        """
+        Parameters
+        ----------
+        data : pd.Dataframe
+            Dataframe containing data.
+        treatment_col : pd.Series
+            Treatment column.
+        y_col : pd.Series
+            Outcome column.
+
+        Returns
+        -------
+        dict
+            A Python dictionary containing the sorted variable importance,
+            where the keys represent the variable names and the values denote
+            their respective importance.
+
+        For example: return a dictionary
+                    var_vs_importance={"age":2.2,"job":2.3}
+        """
+        data, treatment_col, y_col = args[0], args[1], args[2]
+
+        features = list(data.columns)
+        feature = features[0]
+        features.remove(treatment_col)
+        features.remove(y_col)
+        print("feature is ", feature)
+        var_vs_importance = {}
+        var_vs_disc = {}
+        (
+            var_vs_importance[feature],
+            var_vs_disc[feature],
+        ) = execute_greedy_search_and_post_opt(
+            data[[feature, treatment_col, y_col]]
+        )
+        return (feature, var_vs_importance[feature])
+
+    def filter(
+        self, data, treatment_col, y_col, parallelized=False, num_processes=5
+    ):
         """
         This function runs the feature selection algorithm 'UMODL-FS',
         ranking variables based on their importance in the given data.
 
         Parameters
         ----------
         data : pd.Dataframe
             Dataframe containing feature variables.
         treatment_col : pd.Series
             Treatment column.
         y_col : pd.Series
             Outcome column.
+        parallelized : Boolean
+            Whether to run the code on several processes (default = 5)
+        num_processes : int
+            number of processes to use in parallel (default = 5)
 
         Returns
         -------
         Python Dictionary
             Variables names and their corresponding importance value (Sorted).
         """
-        stdout_origin = sys.stdout
-        sys.stdout = open("log.txt", "w")
-
         cols = list(data.columns)
 
         cols.remove(treatment_col)
         cols.remove(y_col)
         data = data[cols + [treatment_col, y_col]]
         data = preprocess_data(data, treatment_col, y_col)
 
-        list_of_vars_importance = self.__get_the_best_var(data, treatment_col, y_col)
+        if parallelized == True:
+            pool = mp.Pool(processes=num_processes)
+
+            arguments_to_pass_in_parallel = []
+            for col in cols:
+                arguments_to_pass_in_parallel.append(
+                    [data[[col, treatment_col, y_col]], treatment_col, y_col]
+                )
+            list_of_tuples_feature_vs_importance = pool.map(
+                FeatureSelection.get_the_best_var_parallel,
+                arguments_to_pass_in_parallel,
+            )
+            pool.close()
+
+            # transform tuple to dict
+            list_of_tuples_feature_vs_importance = dict(
+                list_of_tuples_feature_vs_importance
+            )
 
-        sys.stdout.close()
-        sys.stdout = stdout_origin
+            list_of_vars_importance = {
+                k: v
+                for k, v in sorted(
+                    list_of_tuples_feature_vs_importance.items(),
+                    key=lambda item: item[1],
+                )
+            }
+
+        else:
+            list_of_vars_importance = self.__get_the_best_var(
+                data, treatment_col, y_col
+            )
 
         return list_of_vars_importance
```

### Comparing `kuplift-0.0.2/kuplift/HelperFunctions.py` & `kuplift-0.0.3/kuplift/HelperFunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 from math import log
 
 _log_fact_table = []
 
@@ -56,15 +56,17 @@
         Value of the result.
     """
     d_log2 = log(2.0)
     d_cost = 0.0
     d_logI = log(1.0 * k) / d_log2
 
     if k < 1:
-        raise ValueError("Universal code is defined for natural numbers over 1")
+        raise ValueError(
+            "Universal code is defined for natural numbers over 1"
+        )
     else:
         while d_logI > 0:
             d_cost += d_logI
             d_logI = log(d_logI) / d_log2
         return d_cost
 
 
@@ -107,15 +109,17 @@
     float
         Value of the result.
     """
     dC0 = 2.86511  # First value computed following the given estimation formula, as e(3)=65536 + d_log2^5 / (1-d_log2)
     d_log2 = log(2.0)
 
     if k < 1:
-        raise ValueError("Universal code is defined for natural numbers over 1")
+        raise ValueError(
+            "Universal code is defined for natural numbers over 1"
+        )
     else:
         d_cost = log(dC0) / d_log2  # Initialize code length cost to log_2(dC0)
         d_cost += log_2_star(k)  # Add log_2*(k)
         d_cost *= d_log2  # Go back to the natural log
         return d_cost
 
 
@@ -162,36 +166,44 @@
         data[cat_col] = data[cat_col].fillna("NAN_VAL")
         dict_val_vs_uplift = {}
         for val in data[cat_col].value_counts().index:
             if val == "NAN_VAL":
                 continue
             dataset_slice = data[data[cat_col] == val]
             t0j0 = dataset_slice[
-                (dataset_slice[treatment_col] == 0) & (dataset_slice[y_col] == 0)
+                (dataset_slice[treatment_col] == 0)
+                & (dataset_slice[y_col] == 0)
             ].shape[0]
             t0j1 = dataset_slice[
-                (dataset_slice[treatment_col] == 0) & (dataset_slice[y_col] == 1)
+                (dataset_slice[treatment_col] == 0)
+                & (dataset_slice[y_col] == 1)
             ].shape[0]
             t1j0 = dataset_slice[
-                (dataset_slice[treatment_col] == 1) & (dataset_slice[y_col] == 0)
+                (dataset_slice[treatment_col] == 1)
+                & (dataset_slice[y_col] == 0)
             ].shape[0]
             t1j1 = dataset_slice[
-                (dataset_slice[treatment_col] == 1) & (dataset_slice[y_col] == 1)
+                (dataset_slice[treatment_col] == 1)
+                & (dataset_slice[y_col] == 1)
             ].shape[0]
 
             if (t1j1 + t1j0) == 0:
                 uplift_in_this_slice = -1
             elif (t0j1 + t0j1) == 0:
                 uplift_in_this_slice = 0
             else:
-                uplift_in_this_slice = (t1j1 / (t1j1 + t1j0)) - (t0j1 / (t0j1 + t0j1))
+                uplift_in_this_slice = (t1j1 / (t1j1 + t1j0)) - (
+                    t0j1 / (t0j1 + t0j1)
+                )
             dict_val_vs_uplift[val] = uplift_in_this_slice
         ordered_dict = {
             k: v
-            for k, v in sorted(dict_val_vs_uplift.items(), key=lambda item: item[1])
+            for k, v in sorted(
+                dict_val_vs_uplift.items(), key=lambda item: item[1]
+            )
         }
 
         data[cat_col] = data[cat_col].replace(["NAN_VAL"], -1)
         encoded_i = 0
         for k, v in ordered_dict.items():
             data[cat_col] = data[cat_col].replace([k], encoded_i)
             encoded_i += 1
```

### Comparing `kuplift-0.0.2/kuplift/Node.py` & `kuplift-0.0.3/kuplift/Node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 from .BinaryDiscretizationFunctions import umodl_binary_discretization
 from .HelperFunctions import (
     log_fact,
     log_binomial_coefficient,
@@ -33,18 +33,26 @@
         # Initialize attributes
         self.id = ID
         self.treatment = treatment_col
         self.output = y_col
         self.n = data.shape[0]
         self.nj = data[data[self.output] == 1].shape[0]
         self.ntj = [
-            data[(data[self.treatment] == 0) & (data[self.output] == 0)].shape[0],
-            data[(data[self.treatment] == 0) & (data[self.output] == 1)].shape[0],
-            data[(data[self.treatment] == 1) & (data[self.output] == 0)].shape[0],
-            data[(data[self.treatment] == 1) & (data[self.output] == 1)].shape[0],
+            data[(data[self.treatment] == 0) & (data[self.output] == 0)].shape[
+                0
+            ],
+            data[(data[self.treatment] == 0) & (data[self.output] == 1)].shape[
+                0
+            ],
+            data[(data[self.treatment] == 1) & (data[self.output] == 0)].shape[
+                0
+            ],
+            data[(data[self.treatment] == 1) & (data[self.output] == 1)].shape[
+                0
+            ],
         ]
         self.x = data.iloc[:, :-2].copy()
         self.t = data.iloc[:, -2].copy()
         self.y = data.iloc[:, -1].copy()
 
         try:
             if (self.ntj[2] + self.ntj[3]) == 0:
@@ -60,15 +68,17 @@
                 denum = 0.00001
             else:
                 denum = self.ntj[0] + self.ntj[1]
             self.outcome_prob_in_ctrl = self.ntj[1] / denum
         except Exception:
             self.outcome_prob_in_ctrl = 0
 
-        self.average_uplift = self.outcome_prob_in_trt - self.outcome_prob_in_ctrl
+        self.average_uplift = (
+            self.outcome_prob_in_trt - self.outcome_prob_in_ctrl
+        )
         self.attribute = None
         self.split_threshold = None
         self.is_leaf = True
         self.candidate_splits_vs_data_left_data_right = None
         self.candidate_splits_vs_criterion = None
         self.left_node = None
         self.right_node = None
@@ -99,15 +109,17 @@
             number_of_treatment + 1, 1
         ) + log_binomial_coefficient(number_of_control + 1, 1)
         tree_likelihood_w_one = (
             log_fact(number_of_treatment)
             - log_fact(self.ntj[2])
             - log_fact(self.ntj[3])
         ) + (
-            log_fact(number_of_control) - log_fact(self.ntj[0]) - log_fact(self.ntj[1])
+            log_fact(number_of_control)
+            - log_fact(self.ntj[0])
+            - log_fact(self.ntj[1])
         )
 
         if (leaf_prior_w_zero + tree_likelihood_w_zero) < (
             leaf_prior_w_one + tree_likelihood_w_one
         ):
             w = 0
             leaf_prior = leaf_prior_w_zero
@@ -136,31 +148,39 @@
         attribute_to_split_vs_left_and_right_data = {}
         for attribute in features:
             if (
                 len(self.x[attribute].value_counts()) == 1
                 or len(self.x[attribute].value_counts()) == 0
             ):
                 continue
-            disc_res = umodl_binary_discretization(self.x, self.t, self.y, attribute)
+            disc_res = umodl_binary_discretization(
+                self.x, self.t, self.y, attribute
+            )
             if disc_res == -1:
                 continue
-            data_left, data_right, threshold = disc_res[0], disc_res[1], disc_res[2]
+            data_left, data_right, threshold = (
+                disc_res[0],
+                disc_res[1],
+                disc_res[2],
+            )
             attribute_to_split_vs_left_and_right_data[attribute] = [
                 data_left,
                 data_right,
                 threshold,
             ]
 
         self.candidate_splits_vs_data_left_data_right = (
             attribute_to_split_vs_left_and_right_data.copy()
         )
         candidate_splits_vs_criterion = self.__get_attributes_splits_costs(
             attribute_to_split_vs_left_and_right_data
         )
-        self.candidate_splits_vs_criterion = candidate_splits_vs_criterion.copy()
+        self.candidate_splits_vs_criterion = (
+            candidate_splits_vs_criterion.copy()
+        )
         return candidate_splits_vs_criterion.copy()
 
     def __get_attributes_splits_costs(self, dict_of_each_att_vs_effectifs):
         # Prior of Internal node is only the combinatorial calculations
         criterion_to_be_internal = (
             self.__calc_prior_of_internal_node()
         )  # In case we split this node, it will be no more a leaf but an internal node
@@ -200,16 +220,16 @@
             self.right_node = _Node(
                 self.candidate_splits_vs_data_left_data_right[attribute][1],
                 self.treatment,
                 self.output,
                 ID=self.id * 2 + 1,
             )
             self.attribute = attribute
-            self.split_threshold = self.candidate_splits_vs_data_left_data_right[
-                attribute
-            ][2]
+            self.split_threshold = (
+                self.candidate_splits_vs_data_left_data_right[attribute][2]
+            )
             del self.x
             del self.t
             del self.y
             del self.candidate_splits_vs_data_left_data_right
 
             return self.left_node, self.right_node
```

### Comparing `kuplift-0.0.2/kuplift/Tree.py` & `kuplift-0.0.3/kuplift/Tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 import numpy as np
 import pandas as pd
 from math import log
 from .HelperFunctions import (
@@ -28,15 +28,17 @@
         Treatment column.
     y_col : pd.Series
         Outcome column.
     """
 
     def __init__(self, data, treatment_col, y_col):  # ordered data as argument
         self.nodes_ids = 0
-        self.root_node = _Node(data, treatment_col, y_col, ID=self.nodes_ids + 1)
+        self.root_node = _Node(
+            data, treatment_col, y_col, ID=self.nodes_ids + 1
+        )
         self.terminal_nodes = [self.root_node]
         self.internal_nodes = []
 
         self.k = len(list(data.columns))
         self.k_t = 1
         self.features = list(data.columns)
         self.feature_subset = []
@@ -83,21 +85,25 @@
             self.prior_of_internal_nodes = 0
             self.prob_attribute_selection = 0
         else:
             prior_of_internal_nodes = 0
             for internal_node in self.internal_nodes:
                 prior_of_internal_nodes += internal_node.prior_of_internal_node
             self.prior_of_internal_nodes = prior_of_internal_nodes
-            self.prob_attribute_selection = log(self.k_t) * len(self.internal_nodes)
+            self.prob_attribute_selection = log(self.k_t) * len(
+                self.internal_nodes
+            )
 
     def __calc_encoding(self):
         self.encoding_of_being_a_leaf_node_and_containing_te = (
             len(self.terminal_nodes) * log(2) * 2
         )
-        self.encoding_of_being_an_internal_node = len(self.internal_nodes) * log(2)
+        self.encoding_of_being_an_internal_node = len(
+            self.internal_nodes
+        ) * log(2)
 
     def __calc_leaf_prior(self):
         leaf_priors = 0
         for leaf_node in self.terminal_nodes:
             leaf_priors += leaf_node.prior_leaf
         self.leaf_prior = leaf_priors
 
@@ -214,15 +220,17 @@
                 + "|--- "
                 + " "
                 + str(row["SplittedAttribute"])
                 + " >= "
                 + str(row["SplitThreshold"])
                 + "\n"
             )
-            text_desc = self.export_tree(IdValue * 2 + 1, numTabs + 1, text_desc)
+            text_desc = self.export_tree(
+                IdValue * 2 + 1, numTabs + 1, text_desc
+            )
         else:
             #         print(" id ",str(IdValue),"is leaf")
             text_desc = createTabs(text_desc, numTabs)
             text_desc += "|--- Leaf \n"
             text_desc = createTabs(text_desc, numTabs + 1)
             try:
                 text_desc = (
```

### Comparing `kuplift-0.0.2/kuplift/UMODL_SearchAlgorithm.py` & `kuplift-0.0.3/kuplift/UMODL_SearchAlgorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 import numpy as np
 from math import log
 from operator import add, sub, itemgetter
 from sortedcontainers import SortedKeyList
@@ -74,34 +74,39 @@
             )
         else:
             nitj_interval = self.nitj.copy()
 
         # Likelihood 1
         likelihood_denum = 0
         for j in range(2):
-            likelihood_denum += log_fact((nitj_interval[j] + nitj_interval[j + 2]))
+            likelihood_denum += log_fact(
+                (nitj_interval[j] + nitj_interval[j + 2])
+            )
         likelihood_one_tmp = log_fact(np.sum(nitj_interval)) - likelihood_denum
         # Likelihood 2
         res_t = 0
         for t in range(2):
             likelihood_denum = 0
             for j in range(2):
                 likelihood_denum += log_fact(nitj_interval[t + t * 1 + j])
             res_t += (
-                log_fact(nitj_interval[t + t * 1] + nitj_interval[t + t * 1 + 1])
+                log_fact(
+                    nitj_interval[t + t * 1] + nitj_interval[t + t * 1 + 1]
+                )
                 - likelihood_denum
             )
         likelihood_two_tmp = res_t
         # Prior 1
         prior_one_tmp = log_binomial_coefficient(np.sum(nitj_interval) + 1, 1)
         # Prior 2
         res_t = 0
         for t in range(2):
             res_t_temp = log_binomial_coefficient(
-                (nitj_interval[t + t * 1] + nitj_interval[t + t * 1 + 1]) + 1, 1
+                (nitj_interval[t + t * 1] + nitj_interval[t + t * 1 + 1]) + 1,
+                1,
             )
             res_t += res_t_temp
         prior_two_tmp = res_t
 
         if mode == "DeltaCalc":
             if (prior_one_tmp + likelihood_one_tmp) < (
                 prior_two_tmp + likelihood_two_tmp
@@ -147,15 +152,17 @@
                     sum_of_priors_and_likelihoods
                 )
             if calc_null_two:
                 self.sum_of_priors_and_likelihoods_with_one_w = (
                     sum_of_priors_and_likelihoods
                 )
             else:
-                self.sum_of_priors_and_likelihoods = sum_of_priors_and_likelihoods
+                self.sum_of_priors_and_likelihoods = (
+                    sum_of_priors_and_likelihoods
+                )
 
         elif mode == "init":
             sum_of_priors_and_likelihoods = (
                 ((1 - self.w) * prior_one_tmp)
                 + (self.w * prior_two_tmp)
                 + ((1 - self.w) * likelihood_one_tmp)
                 + ((self.w) * likelihood_two_tmp)
@@ -193,32 +200,38 @@
 
     def insert(self, interval, index):
         nitj = interval.nitj
         included_right_frontier = interval.included_right_frontier
         W_value = interval.w
 
         if (index > self.count) | (index < 0):
-            raise ValueError(f"Index out of range: {index}, size: {self.count}")
+            raise ValueError(
+                f"Index out of range: {index}, size: {self.count}"
+            )
 
         if index == self.count:
             self.append([nitj, included_right_frontier, W_value])
             return
 
         if index == 0:
-            self.head.previous = _Interval([nitj, included_right_frontier, W_value])
+            self.head.previous = _Interval(
+                [nitj, included_right_frontier, W_value]
+            )
             self.head.previous.next = self.head
             self.head = self.head.previous
             self.count += 1
             self.i += 1
             return
 
         start = self.head
         for _ in range(index):
             start = start.next
-        start.previous.next = _Interval([nitj, included_right_frontier, W_value])
+        start.previous.next = _Interval(
+            [nitj, included_right_frontier, W_value]
+        )
         start.previous.next.previous = start.previous
         start.previous.next.next = start
         start.previous = start.previous.next
         self.count += 1
         self.i += 1
         return
 
@@ -243,15 +256,17 @@
         )
         self.count -= 1
         self.i -= 1
         return
 
     def remove(self, index):
         if (index >= self.count) | (index < 0):
-            raise ValueError(f"Index out of range: {index}, size: {self.count}")
+            raise ValueError(
+                f"Index out of range: {index}, size: {self.count}"
+            )
 
         if index == 0:
             self.head = self.head.next
             self.head.previous = None
             self.count -= 1
             self.i -= 1
             return
@@ -359,21 +374,25 @@
         left_interval_node = dll.get_nth(left_interval_node)
 
     right_interval_node = left_interval_node.next
     if right_interval_node is None:
         # it means the left interval node is the last node and cannot be merged
         left_interval_node.right_merge_delta = -1
         return
-    old_left_interval_node_criterion = left_interval_node.sum_of_priors_and_likelihoods
+    old_left_interval_node_criterion = (
+        left_interval_node.sum_of_priors_and_likelihoods
+    )
 
-    left_interval_node_criterion = left_interval_node.calculate_priors_and_likelihoods(
-        mode
+    left_interval_node_criterion = (
+        left_interval_node.calculate_priors_and_likelihoods(mode)
     )
 
-    right_interval_node_criterion = right_interval_node.sum_of_priors_and_likelihoods
+    right_interval_node_criterion = (
+        right_interval_node.sum_of_priors_and_likelihoods
+    )
 
     new_criterion_value = (
         dll.modl_value
         - right_interval_node_criterion
         - old_left_interval_node_criterion
         - log_binomial_coefficient(dll.n + dll.i - 1, dll.i - 1)
         - ((dll.i) * log(2))
@@ -422,18 +441,16 @@
             old_left_interval_node_criterion = (
                 interval_to_be_merged.sum_of_priors_and_likelihoods
             )
             old_right_interval_node_criterion = (
                 interval_right_of_the_merge.sum_of_priors_and_likelihoods
             )
 
-            left_interval_node_criterion = (
-                interval_to_be_merged.calculate_priors_and_likelihoods(
-                    mode="MergeAndUpdate"
-                )
+            left_interval_node_criterion = interval_to_be_merged.calculate_priors_and_likelihoods(
+                mode="MergeAndUpdate"
             )  # it will update w, Priors, lkelihoods and sum_of_priors_and_likelihoods
             intervals.modl_value = (
                 intervals.modl_value
                 - old_right_interval_node_criterion
                 - old_left_interval_node_criterion
                 - log_binomial_coefficient(
                     intervals.n + intervals.i - 1, intervals.i - 1
@@ -461,50 +478,60 @@
                 best_merges.remove(
                     (
                         interval_left_to_new_interval.right_merge_delta,
                         interval_left_to_new_interval,
                     )
                 )
                 criterion_delta_for_one_adjacent_interval_merge(
-                    intervals, interval_left_to_new_interval, index_passed=False
+                    intervals,
+                    interval_left_to_new_interval,
+                    index_passed=False,
                 )
                 best_merges.add(
                     (
                         interval_left_to_new_interval.right_merge_delta,
                         interval_left_to_new_interval,
                     )
                 )
             elif interval_left_to_new_interval is None:
                 criterion_delta_for_one_adjacent_interval_merge(
                     intervals, interval_to_be_merged, index_passed=False
                 )
                 best_merges.add(
-                    (interval_to_be_merged.right_merge_delta, interval_to_be_merged)
+                    (
+                        interval_to_be_merged.right_merge_delta,
+                        interval_to_be_merged,
+                    )
                 )
             else:
                 best_merges.remove(
                     (
                         interval_left_to_new_interval.right_merge_delta,
                         interval_left_to_new_interval,
                     )
                 )
                 criterion_delta_for_one_adjacent_interval_merge(
-                    intervals, interval_left_to_new_interval, index_passed=False
+                    intervals,
+                    interval_left_to_new_interval,
+                    index_passed=False,
                 )
                 best_merges.add(
                     (
                         interval_left_to_new_interval.right_merge_delta,
                         interval_left_to_new_interval,
                     )
                 )
                 criterion_delta_for_one_adjacent_interval_merge(
                     intervals, interval_to_be_merged, index_passed=False
                 )
                 best_merges.add(
-                    (interval_to_be_merged.right_merge_delta, interval_to_be_merged)
+                    (
+                        interval_to_be_merged.right_merge_delta,
+                        interval_to_be_merged,
+                    )
                 )
         else:
             break
     stop_counter(3)
 
 
 def merge(interval, intervals, number_of_merges=1):
@@ -518,23 +545,27 @@
             map(add, neighbours_to_merge[-1].nitj.copy(), merged_intervals)
         )
         sum_of_old_priors_and_likelihoods += neighbours_to_merge[
             -1
         ].sum_of_priors_and_likelihoods
 
     interval.nitj = merged_intervals
-    interval.included_right_frontier = neighbours_to_merge[-1].included_right_frontier
+    interval.included_right_frontier = neighbours_to_merge[
+        -1
+    ].included_right_frontier
     # NOW WE HAVE TO SEARCH for the old values of the sum of prior and likelihoods !!!!
     left_interval_node_criterion = interval.calculate_priors_and_likelihoods(
         mode="MergeAndUpdate"
     )  # it will update w, Priors, lkelihoods and sum_of_priors_and_likelihoods
     intervals.modl_value = (
         intervals.modl_value
         - sum_of_old_priors_and_likelihoods
-        - log_binomial_coefficient(intervals.n + intervals.i - 1, intervals.i - 1)
+        - log_binomial_coefficient(
+            intervals.n + intervals.i - 1, intervals.i - 1
+        )
         - ((intervals.i) * log(2))
         + log_binomial_coefficient(
             intervals.n + intervals.i - number_of_merges - 1,
             intervals.i - number_of_merges - 1,
         )
         + ((intervals.i - number_of_merges) * log(2))
         + left_interval_node_criterion
@@ -558,35 +589,43 @@
     right_bound = interval.included_right_frontier
     unique_values_in_both_intervals = list(
         data.irange_key(left_bound, right_bound, (including_left_border, True))
     )
     unique_values_in_both_intervals = list(
         map(itemgetter(0), unique_values_in_both_intervals)
     )
-    unique_values_in_both_intervals = list(set(unique_values_in_both_intervals))
+    unique_values_in_both_intervals = list(
+        set(unique_values_in_both_intervals)
+    )
     unique_values_in_both_intervals.sort()
     splits = {}
     left_and_right_interval_of_splits = {}
     previous_left_interval = [0, 0, 0, 0]
     prev_val = None
 
     for val in unique_values_in_both_intervals:
         if prev_val is None:
             left_split = list(
                 data.irange_key(left_bound, val, (including_left_border, True))
             )
             left_interval = [0, 0, 0, 0]
             for interval_list in left_split:
-                left_interval[int((interval_list[1] * 2) + interval_list[2])] += 1
+                left_interval[
+                    int((interval_list[1] * 2) + interval_list[2])
+                ] += 1
         else:
             left_split = list(data.irange_key(prev_val, val, (False, True)))
             left_interval = [0, 0, 0, 0]
             for interval_list in left_split:
-                left_interval[int((interval_list[1] * 2) + interval_list[2])] += 1
-            left_interval = list(map(add, previous_left_interval, left_interval))
+                left_interval[
+                    int((interval_list[1] * 2) + interval_list[2])
+                ] += 1
+            left_interval = list(
+                map(add, previous_left_interval, left_interval)
+            )
 
         prev_val = val
         previous_left_interval = left_interval
 
         right_interval = list(map(sub, interval.nitj, left_interval))
 
         Left_interval = _Interval([left_interval, val, 0])
@@ -600,36 +639,42 @@
         criterion_two = Right_interval.calculate_priors_and_likelihoods(
             mode="MergeAndUpdate"
         )
 
         split_criterion_val_left_and_right = (
             intervals.modl_value
             - interval.sum_of_priors_and_likelihoods
-            - log_binomial_coefficient(intervals.n + intervals.i - 1, intervals.i - 1)
+            - log_binomial_coefficient(
+                intervals.n + intervals.i - 1, intervals.i - 1
+            )
             - ((intervals.i) * log(2))
             + criterion_one
             + criterion_two
             + log_binomial_coefficient(intervals.n + intervals.i, intervals.i)
             + ((intervals.i + 1) * log(2))
         )
 
         if split_criterion_val_left_and_right < intervals.modl_value:
             splits[val] = split_criterion_val_left_and_right
-            left_and_right_interval_of_splits[val] = [left_interval, right_interval]
+            left_and_right_interval_of_splits[val] = [
+                left_interval,
+                right_interval,
+            ]
     split_done = False
     best_split = None
     if splits:
         best_split = min(splits, key=splits.get)  # To be optimized maybe
         left_interval = left_and_right_interval_of_splits[best_split][0]
         right_interval = left_and_right_interval_of_splits[best_split][1]
 
         Left_interval = interval
         right_bound_of_the_right_interval = interval.included_right_frontier
         intervals.insert(
-            _Interval([right_interval, right_bound_of_the_right_interval, 0]), i + 1
+            _Interval([right_interval, right_bound_of_the_right_interval, 0]),
+            i + 1,
         )
         Right_interval = intervals.get_nth(i + 1)
 
         Left_interval.nitj = left_interval
         Left_interval.included_right_frontier = best_split
 
         Left_interval.calculate_priors_and_likelihoods(
@@ -783,31 +828,33 @@
         except Exception:
             piYT0 = 0
         if method == "ED":
             absolute_sum += (((piYT1) - (piYT0)) ** 2) * Ni / intervals.n  # ED
         elif method == "Chi":
             if piYT0 < 0.1**6:
                 piYT0 = 0.1**6
-            absolute_sum += ((((piYT1) - (piYT0)) ** 2) / piYT0) * Ni / intervals.n
+            absolute_sum += (
+                ((((piYT1) - (piYT0)) ** 2) / piYT0) * Ni / intervals.n
+            )
         elif method == "KL":
             if piYT0 < 0.1**6:
                 piYT0 = 0.1**6
             elif piYT0 > 1 - 0.1**6:
                 piYT0 = 1 - 0.1**6
             absolute_sum += ((piYT1) * log(piYT1 / piYT0)) * Ni / intervals.n
         interval = interval.next
     return absolute_sum
 
 
 def execute_greedy_search_and_post_opt(df):
     treatment_col_name = df.columns[1]
     y_name = df.columns[2]
 
-    df[treatment_col_name] = df[treatment_col_name].astype(int)
-    df[y_name] = df[y_name].astype(int)
+    df = df.astype({treatment_col_name:'int'})
+    df = df.astype({y_name:'int'})
 
     df = df.values.tolist()
     df = sorted(df, key=itemgetter(0))
     intervals = _DLL()
     intervals.n = len(df)
 
     intervals, intervals.modl_value, w = create_elementary_discretization(
@@ -823,15 +870,18 @@
     )  # Get all the costs of 'all possible merges of two adjacent intervals' sorted
     best_merges = SortedKeyList(best_merges, key=itemgetter(0))
 
     # Start greedy search
     greedy_search(best_merges, intervals, intervals.n)
 
     # Post Optimization steps
-    intervals_num, umodl_val, intervals, info = post_optimization_to_be_repeated(
-        intervals, df
-    )
+    (
+        intervals_num,
+        umodl_val,
+        intervals,
+        info,
+    ) = post_optimization_to_be_repeated(intervals, df)
 
     bounds = info[2]
     feature_level_ed = calculate_feature_level(intervals)
 
     return [feature_level_ed, bounds]
```

### Comparing `kuplift-0.0.2/kuplift/UnivariateEncoding.py` & `kuplift-0.0.3/kuplift/UnivariateEncoding.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 import pandas as pd
 import multiprocessing as mp
 from .HelperFunctions import preprocess_data
 from .UMODL_SearchAlgorithm import execute_greedy_search_and_post_opt
@@ -22,15 +22,17 @@
     """
 
     def __init__(self):
         self.var_vs_disc = {}
         self.treatment_col = ""
         self.y_col = ""
 
-    def fit_transform(self, data, treatment_col, y_col):
+    def fit_transform(
+        self, data, treatment_col, y_col, parallelized=False, num_processes=5
+    ):
         """
         fit_transform() learns a discretisation model using UMODL and transforms the data.
 
         Parameters
         ----------
         data : pd.Dataframe
             Dataframe containing feature variables.
@@ -40,57 +42,67 @@
             Outcome column.
 
         Returns
         -------
         pd.Dataframe
             Pandas Dataframe that contains encoded data.
         """
-        self.fit(data, treatment_col, y_col)
+        self.fit(data, treatment_col, y_col, parallelized, num_processes)
         data = self.transform(data)
         return data
 
-    def fit(self, data, treatment_col, y_col,parallelized=False,num_processes=5):
+    def fit(
+        self, data, treatment_col, y_col, parallelized=False, num_processes=5
+    ):
         """
          fit() learns a discretisation model using the UMODL approach
 
         Parameters
         ----------
         data : pd.Dataframe
             Dataframe containing feature variables.
         treatment_col : pd.Series
             Treatment column.
         y_col : pd.Series
             Outcome column.
+        parallelized : Boolean
+            Whether to run the code on several processes (default = 5)
+        num_processes : int
+            number of processes to use in parallel (default = 5)
         """
         self.treatment_col = treatment_col
         self.y_col = y_col
 
         cols = list(data.columns)
         cols.remove(treatment_col)
         cols.remove(y_col)
 
         data = data[cols + [treatment_col, y_col]]
         data = preprocess_data(data, treatment_col, y_col)
-        
+
         var_vs_importance = {}
         self.var_vs_disc = {}
-        
-        
-        if parallelized==True:
+
+        if parallelized == True:
             pool = mp.Pool(processes=num_processes)
-            
-            arguments_to_pass_in_parallel=[]
+
+            arguments_to_pass_in_parallel = []
             for col in cols:
-                arguments_to_pass_in_parallel.append([data[[col,treatment_col,y_col]]])
-            list_of_tuples_feature_vs_importance = pool.map(execute_greedy_search_and_post_opt, arguments_to_pass_in_parallel)
+                arguments_to_pass_in_parallel.append(
+                    [data[[col, treatment_col, y_col]]]
+                )
+            list_of_tuples_feature_vs_importance = pool.map(
+                execute_greedy_search_and_post_opt,
+                arguments_to_pass_in_parallel,
+            )
             pool.close()
-            
+
             for el in list_of_tuples_feature_vs_importance:
-                col=el[0]
-                if len(el[2])==1:
+                col = el[0]
+                if len(el[2]) == 1:
                     self.var_vs_disc[col] = None
                 else:
                     self.var_vs_disc[col] = el[2][:-1]
 
         else:
             for col in cols:
                 (
@@ -122,18 +134,20 @@
         cols = list(data.columns)
         cols.remove(self.treatment_col)
         cols.remove(self.y_col)
         for col in cols:
             if self.var_vs_disc[col] is None:
                 data.drop(col, inplace=True, axis=1)
             else:
-                minBoundary=min(data[col].min(),self.var_vs_disc[col][0]-0.001)
-                maxBoundary=max(data[col].max(),self.var_vs_disc[col][-1]+0.001)
+                minBoundary = min(
+                    data[col].min(), self.var_vs_disc[col][0] - 0.001
+                )
+                maxBoundary = max(
+                    data[col].max(), self.var_vs_disc[col][-1] + 0.001
+                )
                 data[col] = pd.cut(
                     data[col],
-                    bins=[minBoundary]
-                    + self.var_vs_disc[col]
-                    + [maxBoundary],
+                    bins=[minBoundary] + self.var_vs_disc[col] + [maxBoundary],
                 )
                 data[col] = data[col].astype("category")
                 data[col] = data[col].cat.codes
         return data
```

### Comparing `kuplift-0.0.2/kuplift.egg-info/SOURCES.txt` & `kuplift-0.0.3/kuplift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.2/test/test.py` & `kuplift-0.0.3/test/test.py`

 * *Files identical despite different names*

### Comparing `kuplift-0.0.2/test/test_BayesianDecisionTree.py` & `kuplift-0.0.3/test/test_BayesianDecisionTree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 from kuplift.BayesianDecisionTree import BayesianDecisionTree
 
 
 def test_predict(test_dataframe):
```

### Comparing `kuplift-0.0.2/test/test_BayesianRandomForest.py` & `kuplift-0.0.3/test/test_BayesianRandomForest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 from kuplift.BayesianRandomForest import BayesianRandomForest
 
 
 def test_predict(test_dataframe):
```

### Comparing `kuplift-0.0.2/test/test_FeatureSelection.py` & `kuplift-0.0.3/test/test_FeatureSelection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 from kuplift.FeatureSelection import FeatureSelection
 
 
 def test_filter(test_dataframe):
```

### Comparing `kuplift-0.0.2/test/test_UnvariateEncoding.py` & `kuplift-0.0.3/test/test_UnvariateEncoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ######################################################################################
 # Copyright (c) 2023 Orange - All Rights Reserved                             #
 # * This software is the confidential and proprietary information of Orange.         #
 # * You shall not disclose such Restricted Information and shall use it only in      #
 #   accordance with the terms of the license agreement you entered into with Orange  #
-#   named the "Kuplift - Python Library Evaluation License".                          #
+#   named the "kuplift - Python Library Evaluation License".                          #
 # * Unauthorized copying of this file, via any medium is strictly prohibited.        #
 # * See the "LICENSE.md" file for more details.                                      #
 ######################################################################################
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from kuplift.UnivariateEncoding import UnivariateEncoding
```

