# Comparing `tmp/anti-clustering-0.2.1.tar.gz` & `tmp/anti_clustering-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anti-clustering-0.2.1.tar", max compression
+gzip compressed data, was "anti_clustering-0.3.0.tar", max compression
```

## Comparing `anti-clustering-0.2.1.tar` & `anti_clustering-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    10692 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/LICENSE
--rw-r--r--   0        0        0     3531 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/README.md
--rw-r--r--   0        0        0      997 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/__init__.py
--rw-r--r--   0        0        0     6683 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/_base.py
--rw-r--r--   0        0        0     3580 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/_cluster_swap_heuristic.py
--rw-r--r--   0        0        0     3231 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/_union_find.py
--rw-r--r--   0        0        0       22 2022-09-09 13:15:04.155053 anti-clustering-0.2.1/anti_clustering/_version.py
--rw-r--r--   0        0        0     5456 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/exact_cluster_editing.py
--rw-r--r--   0        0        0     3118 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/exchange_heuristic.py
--rw-r--r--   0        0        0     1242 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/naive_random_heuristic.py
--rw-r--r--   0        0        0     3780 2022-09-09 13:14:43.258909 anti-clustering-0.2.1/anti_clustering/simulated_annealing_heuristic.py
--rw-r--r--   0        0        0      490 2022-09-09 13:15:04.155053 anti-clustering-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 anti-clustering-0.2.1/setup.py
--rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 anti-clustering-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10692 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3644 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/README.md
+-rw-r--r--   0        0        0      997 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/__init__.py
+-rw-r--r--   0        0        0     6817 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/_base.py
+-rw-r--r--   0        0        0     3581 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/_cluster_swap_heuristic.py
+-rw-r--r--   0        0        0     3491 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/_union_find.py
+-rw-r--r--   0        0        0       22 2023-07-18 11:47:06.569830 anti_clustering-0.3.0/anti_clustering/_version.py
+-rw-r--r--   0        0        0     5372 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/exact_cluster_editing.py
+-rw-r--r--   0        0        0     3135 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/exchange_heuristic.py
+-rw-r--r--   0        0        0     1243 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/naive_random_heuristic.py
+-rw-r--r--   0        0        0     4530 2023-07-18 11:46:46.769778 anti_clustering-0.3.0/anti_clustering/simulated_annealing_heuristic.py
+-rw-r--r--   0        0        0      536 2023-07-18 11:47:06.569830 anti_clustering-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 anti_clustering-0.3.0/PKG-INFO
```

### Comparing `anti-clustering-0.2.1/LICENSE` & `anti_clustering-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anti-clustering-0.2.1/README.md` & `anti_clustering-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Anti-clustering
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A generic Python library for solving the anti-clustering problem. While clustering algorithms will achieve high similarity within a cluster and low similarity between clusters, the anti-clustering algorithms will achieve the opposite; namely to minimise similarity within a cluster and maximise the similarity between clusters.
 Currently, a handful of algorithms are implemented in this library:
 * An exact approach using a BIP formulation.
 * An enumerated exchange heuristic.
 * A simulated annealing heuristic.
```

### Comparing `anti-clustering-0.2.1/anti_clustering/__init__.py` & `anti_clustering-0.3.0/anti_clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `anti-clustering-0.2.1/anti_clustering/_base.py` & `anti_clustering-0.3.0/anti_clustering/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,144 +21,139 @@
 from scipy.spatial.distance import squareform, pdist
 from sklearn.preprocessing import MinMaxScaler
 from anti_clustering._union_find import UnionFind
 
 
 class AntiClustering(ABC):
     """Generic anti-clustering interface."""
+
     def __init__(self, verbose=False):
         self.verbose = verbose
 
     def run(
         self,
         df: pd.DataFrame,
         numerical_columns: Optional[List[str]],
         categorical_columns: Optional[List[str]],
         num_groups: int,
-        destination_column: str
+        destination_column: str,
     ) -> pd.DataFrame:
-        # pylint: disable = R0913
         """
         Run anti clustering algorithm on dataset.
         :param df: The dataset to run anti-clustering on.
         :param numerical_columns: Columns in dataset to use for anti-clustering containing numbers.
         :param categorical_columns: Columns in dataset to use for anti-clustering containing strings or dates.
         :param num_groups: Number of anti-clusters to generate.
         :param destination_column: The column to write results to.
         :return: The original dataframe with a destination_column added.
         """
         numerical_columns = [] if numerical_columns is None else numerical_columns
         categorical_columns = [] if categorical_columns is None else categorical_columns
 
         prepared_df = self._prepare_data(
-            df=df,
-            numerical_columns=numerical_columns,
-            categorical_columns=categorical_columns
+            df=df, numerical_columns=numerical_columns, categorical_columns=categorical_columns
         )
 
         distance_matrix = self._get_distance_matrix(
-            df=prepared_df,
-            numerical_columns=numerical_columns,
-            categorical_columns=categorical_columns
+            df=prepared_df, numerical_columns=numerical_columns, categorical_columns=categorical_columns
         )
 
         cluster_assignment = self._solve(distance_matrix=distance_matrix, num_groups=num_groups)
 
         return self._post_process(
             df=df,
             numerical_columns=numerical_columns,
             categorical_columns=categorical_columns,
             destination_column=destination_column,
-            cluster_assignment_matrix=cluster_assignment
+            cluster_assignment_matrix=cluster_assignment,
         )
 
     @abstractmethod
     def _solve(self, distance_matrix: npt.NDArray[float], num_groups: int) -> npt.NDArray[bool]:
         """
         Abstract solve signature. To be implemented in subclasses.
         :param distance_matrix: The distance matrix of elements.
         :param num_groups: Number of anti-clusters to generate.
         :return:
         """
 
-    def _prepare_data(self, df: pd.DataFrame, numerical_columns: List[str], categorical_columns: List[str]) -> pd.DataFrame:
+    def _prepare_data(
+        self, df: pd.DataFrame, numerical_columns: List[str], categorical_columns: List[str]
+    ) -> pd.DataFrame:
         """
         Prepare data for solving.
         :param df: The input dataframe.
         :param numerical_columns: Columns in dataset to use for anti-clustering containing numbers.
         :param categorical_columns: Columns in dataset to use for anti-clustering containing strings or dates.
         :return: the prepared dataframe.
         """
         if numerical_columns is None and categorical_columns is None:
-            raise ValueError('Both numerical and categorical columns cannot be None.')
-
-        df = df.copy()
+            raise ValueError("Both numerical and categorical columns cannot be None.")
 
         # Normalize to interval [0, 1]
         if len(numerical_columns) > 0:
             scaler = MinMaxScaler()
-            df[numerical_columns] = scaler.fit_transform(df[numerical_columns])
+            transformed_columns = scaler.fit_transform(df[numerical_columns])
+            df = df.assign(**{col: transformed_columns[:, i] for i, col in enumerate(numerical_columns)})
 
         return df
 
     def _post_process(
         self,
         df: pd.DataFrame,
         numerical_columns: List[str],
         categorical_columns: List[str],
         destination_column: str,
-        cluster_assignment_matrix: npt.NDArray[bool]
+        cluster_assignment_matrix: npt.NDArray[bool],
     ) -> pd.DataFrame:
         # pylint: disable = R0913
         """
         Postprocess results and prepare for returning to caller.
         :param df: The input dataframe.
         :param numerical_columns: Columns in dataset to use for anti-clustering containing numbers.
         :param categorical_columns: Columns in dataset to use for anti-clustering containing strings or dates.
         :param destination_column: The column to write results to.
-        :param cluster_assignment_matrix: A matrix containing for each pair of elements if they belong to the same anti-cluster.
+        :param cluster_assignment_matrix: A matrix containing for each pair of elements if they belong to the same
+        anti-cluster.
         :return: The inputted dataframe with the new destination column.
         """
         components = UnionFind(len(df))
 
         for j in range(len(df)):
             for i in range(0, j):
                 if cluster_assignment_matrix[i][j] == 1:
                     components.union(i, j)
 
-        df[destination_column] = [components.find(i) for i in range(len(df))]
+        df = df.assign(**{destination_column: [components.find(i) for i in range(len(df))]})
 
         # Normalize cluster labels. The algorithm assignment of cluster labels may be non-deterministic.
         # Ensure that all labels are enumerated starting from 0 without gaps.
         cluster_labels = df.sort_values(by=[*numerical_columns, *categorical_columns])[destination_column].unique()
-        mapping = {
-            k: i for i, k in enumerate(cluster_labels)
-        }
-        df = df.replace({'Cluster': mapping})
+        mapping = {k: i for i, k in enumerate(cluster_labels)}
+        df = df.replace({destination_column: mapping})
 
         return df
 
     def _get_distance_matrix(
-        self,
-        df: pd.DataFrame,
-        numerical_columns: List[str],
-        categorical_columns: List[str]
+        self, df: pd.DataFrame, numerical_columns: List[str], categorical_columns: List[str]
     ) -> npt.NDArray[float]:
         """
         Calculate distance matrix between each pair of elements. Numeric columns default to Euclidean distance and
         categorical columns default to Hamming distance.
         :param df: The input dataframe.
         :param numerical_columns: Columns in dataset to use for anti-clustering containing numbers.
         :param categorical_columns: Columns in dataset to use for anti-clustering containing strings or dates.
         :return: The distance matrix.
         """
 
-        d = 0
+        categorical_distance = 0
         if len(categorical_columns) > 0:
-            d = squareform(pdist(df[categorical_columns].apply(lambda x: pd.factorize(x)[0]), metric='hamming'))
+            categorical_distance = squareform(
+                pdist(df[categorical_columns].apply(lambda x: pd.factorize(x)[0]), metric="hamming")
+            )
 
-        c = 0
+        numeric_distance = 0
         if len(numerical_columns) > 0:
             numerical_data = df[numerical_columns].to_numpy()
-            c = scipy.spatial.distance_matrix(numerical_data, numerical_data)
+            numeric_distance = scipy.spatial.distance_matrix(numerical_data, numerical_data)
 
-        return c + d
+        return numeric_distance + categorical_distance
```

### Comparing `anti-clustering-0.2.1/anti_clustering/_cluster_swap_heuristic.py` & `anti_clustering-0.3.0/anti_clustering/_cluster_swap_heuristic.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import numpy.typing as npt
 from anti_clustering._base import AntiClustering
 from anti_clustering._union_find import UnionFind
 
 
 class ClusterSwapHeuristic(AntiClustering, ABC):
     """Abstract class containing utilities for cluster swap-based heuristics."""
+
     def __init__(self, verbose: bool = False, random_seed: int = None):
         super().__init__(verbose=verbose)
         self.rnd = random.Random(random_seed)
 
     def _get_exchanges(self, cluster_assignment: npt.NDArray[bool], i: int) -> npt.NDArray[int]:
         """
         Given a cluster assignment matrix and element index, will return possible indexes to swap anti-clusters with.
```

### Comparing `anti-clustering-0.2.1/anti_clustering/_union_find.py` & `anti_clustering-0.3.0/anti_clustering/_union_find.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,84 +16,85 @@
 
 Based on:
 Sedgewick, R. & Wayne, K. (2011), Algorithms, 4th Edition. , Addison-Wesley .
 """
 
 from typing import TypeVar, Generic
 
-T = TypeVar('T')  # pylint: disable=C0103
+T = TypeVar("T")  # pylint: disable=C0103
 
 
 class UnionFind(Generic[T]):
     """
     A union find data structure for collecting results of the anti-clustering algorithm.
     This implementation uses the weighted quick union with path compression.
     """
+
     # A mapping from an element to its parent. If a parent maps to itself, it is the root of the component.
     _parent = {}
     _size = {}
     components_count = 0
 
     def __init__(self, initial_components_count: int):
         """
         Initialize UnionFind with components.
         :param initial_components_count: The initial number of components.
         """
         self.components_count = initial_components_count
         self._parent = {i: i for i in range(initial_components_count)}
         self._size = {i: 1 for i in range(initial_components_count)}
 
-    def _find(self, a: T) -> T:
+    def _find(self, element: T) -> T:
         """
-        Find the root of component of element a.
-        :param a: Element to find root of.
+        Find the root of component of element.
+        :param element: Element to find root of.
         :return: The root of the component.
         """
         # Compresses path while iterating up the tree.
-        while a != self._parent[a]:
-            b = self._parent[a]
-            self._parent[a] = self._parent[b]
-            a = b
+        while element != self._parent[element]:
+            parent = self._parent[element]
+            self._parent[element] = self._parent[parent]
+            element = parent
 
-        return a
+        return element
 
-    def find(self, a: T) -> T:
+    def find(self, element: T) -> T:
         """
-        Find the root of component of element a.
-        :param a: Element to find root of.
+        Find the root of component of element.
+        :param element: Element to find root of.
         :return: The root of the component.
         """
-        return self._find(a)
+        return self._find(element)
 
-    def union(self, a: T, b: T) -> None:
+    def union(self, element_1: T, element_2: T) -> None:
         """
         Unify components of two elements.
-        :param a: Element to unify.
-        :param b: Other element to unify.
+        :param element_1: Element to unify.
+        :param element_2: Other element to unify.
         :return:
         """
-        if a == b:
+        if element_1 == element_2:
             return
 
-        x = self._find(a)
-        y = self._find(b)
+        root_1 = self._find(element_1)
+        root_2 = self._find(element_2)
 
-        if x == y:
+        if root_1 == root_2:
             return
 
         # Weighted union - the smaller component becomes the child of the root of the larger component.
-        if self._size[x] < self._size[y]:
-            self._parent[x] = y
-            self._size[y] += self._size[x]
+        if self._size[root_1] < self._size[root_2]:
+            self._parent[root_1] = root_2
+            self._size[root_2] += self._size[root_1]
         else:
-            self._parent[y] = x
-            self._size[x] += self._size[y]
+            self._parent[root_2] = root_1
+            self._size[root_1] += self._size[root_2]
         self.components_count -= 1
 
-    def connected(self, a: T, b: T) -> bool:
+    def connected(self, element_1: T, element_2: T) -> bool:
         """
-        Check if element a and b are in the same component.
-        :param a: Element to check.
-        :param b: Other element to check.
-        :return: Whether a and b are in the same component.
+        Check if element 1 and 2 are in the same component.
+        :param element_1: Element to check.
+        :param element_2: Other element to check.
+        :return: Whether 1 and 2 are in the same component.
         """
-        return self._find(a) == self._find(b)
+        return self._find(element_1) == self._find(element_2)
```

### Comparing `anti-clustering-0.2.1/anti_clustering/exact_cluster_editing.py` & `anti_clustering-0.3.0/anti_clustering/exact_cluster_editing.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,124 +26,117 @@
 from anti_clustering._base import AntiClustering
 
 
 class ExactClusterEditingAntiClustering(AntiClustering):
     """
     MIP formulation for solving the anti-clustering problem.
     """
+
     def __init__(self, verbose: bool = False, solver_id: str = "SCIP"):
         super().__init__(verbose=verbose)
         self.solver_id = solver_id
 
     def _solve(self, distance_matrix: npt.NDArray[float], num_groups: int) -> npt.NDArray[bool]:
         solver: pywraplp.Solver = pywraplp.Solver.CreateSolver(self.solver_id)
 
         if self.verbose:
             solver.EnableOutput()
 
         min_group_size = np.floor(len(distance_matrix) / num_groups)
         max_group_size = np.ceil(len(distance_matrix) / num_groups)
 
         # Cluster assignment are modelled as boolean assignments.
-        x = np.asarray([
+        x = np.asarray(
             [
-                (solver.BoolVar(f'x_[{i}][{j}]'))
-                if j > i else False
-                for j in range(len(distance_matrix))
+                [(solver.BoolVar(f"x_[{i}][{j}]")) if j > i else False for j in range(len(distance_matrix))]
+                for i in range(len(distance_matrix))
             ]
-            for i in range(len(distance_matrix))])
+        )
 
         if self.verbose:
             print("Making cluster assignment constraints")
 
         # Cluster assignment constraints
         for k in range(len(distance_matrix)):
             for j in range(0, k):
                 for i in range(0, j):
                     self._add_constraint(
                         solver=solver,
                         vars_=[x[i][j], x[i][k], x[j][k]],
                         coeffs=[-1.0, 1.0, 1.0],
                         ub=1.0,
-                        lb=-solver.infinity()
+                        lb=-solver.infinity(),
                     )
 
                     self._add_constraint(
                         solver=solver,
                         vars_=[x[i][j], x[i][k], x[j][k]],
                         coeffs=[1.0, -1.0, 1.0],
                         ub=1.0,
-                        lb=-solver.infinity()
+                        lb=-solver.infinity(),
                     )
 
                     self._add_constraint(
                         solver=solver,
                         vars_=[x[i][j], x[i][k], x[j][k]],
                         coeffs=[1.0, 1.0, -1.0],
                         ub=1.0,
-                        lb=-solver.infinity()
+                        lb=-solver.infinity(),
                     )
 
         if self.verbose:
             print("Making cluster size constraints")
 
         # Cluster size constraints. Differently to original paper, we allow anti-clusters to be of different size if
         # number of groups does not divide number og elements.
         for i in range(len(distance_matrix)):
             self._add_constraint(
                 solver=solver,
                 vars_=[x[i][j] for j in range(i + 1, len(distance_matrix))] + [x[k][i] for k in range(0, i)],
                 coeffs=[1.0 for j in range(i + 1, len(distance_matrix))] + [1.0 for k in range(0, i)],
                 ub=max_group_size - 1.0 if i + 1 < len(distance_matrix) else solver.infinity(),
-                lb=min_group_size - 1.0 if i > 0 else -solver.infinity()
+                lb=min_group_size - 1.0 if i > 0 else -solver.infinity(),
             )
 
         if self.verbose:
             print("Making objective")
 
         # Maximise internal anti-cluster distance
         solver.Maximize(np.multiply(x, distance_matrix).sum())
 
         if self.verbose:
             print("Solving")
 
         status = solver.Solve()
 
         if status != 0:
-            raise ValueError('Optimization failed!')
+            raise ValueError("Optimization failed!")
 
-        cluster_assignment = np.asarray([
+        cluster_assignment = np.asarray(
             [
-                bool(x[i][j].solution_value())
-                if j > i else None
-                for j in range(len(distance_matrix))
+                [bool(x[i][j].solution_value()) if j > i else None for j in range(len(distance_matrix))]
+                for i in range(len(distance_matrix))
             ]
-            for i in range(len(distance_matrix))
-        ])
+        )
 
         return cluster_assignment
 
     def _add_constraint(
-        self,
-        solver: pywraplp.Solver,
-        lb: float,
-        ub: float,
-        coeffs: List[float],
-        vars_: List[pywraplp.Variable]
+        self, solver: pywraplp.Solver, lb: float, ub: float, coeffs: List[float], vars_: List[pywraplp.Variable]
     ) -> pywraplp.Constraint:
         # pylint: disable = R0913
         """
         Utility for adding constraints in the Google OR-Tools framework. Adds single constraint on the form:
         lb <= c_1x_1 + c_2x_2 + ... <= ub
         :param solver: The OR-Tools solver.
         :param lb: Lower bound.
         :param ub: Upper bound.
         :param coeffs: A list of coefficients. Each index must correspond to the same index in vars_.
         :param vars_: A list of decision variables. Each index must correspond to the same index in coeffs.
         :return: The OR-Tools constraint.
         """
         constr: pywraplp.Constraint = solver.Constraint(lb, ub)
 
-        for (coeff, var) in zip(coeffs, vars_):
+        for coeff, var in zip(coeffs, vars_):
             constr.SetCoefficient(var, coeff)
 
         return constr
```

### Comparing `anti-clustering-0.2.1/anti_clustering/exchange_heuristic.py` & `anti_clustering-0.3.0/anti_clustering/exchange_heuristic.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,40 +24,42 @@
 from anti_clustering._cluster_swap_heuristic import ClusterSwapHeuristic
 
 
 class ExchangeHeuristicAntiClustering(ClusterSwapHeuristic):
     """
     The exchange heuristic to solving the anti-clustering problem.
     """
+
     def __init__(self, verbose: bool = False, random_seed: int = None):
         super().__init__(verbose=verbose, random_seed=random_seed)
 
     def _solve(self, distance_matrix: npt.NDArray[float], num_groups: int) -> npt.NDArray[bool]:
         # Starts with random cluster assignment
         cluster_assignment = self._get_random_clusters(num_groups=num_groups, num_elements=len(distance_matrix))
 
         if self.verbose:
             print("Solving")
 
         # Initial objective value
         current_objective = self._calculate_objective(cluster_assignment, distance_matrix)
         for i in range(len(distance_matrix)):
             if self.verbose and i % 5 == 0:
-                print(f'Iteration {i + 1} of {len(distance_matrix)}')
+                print(f"Iteration {i + 1} of {len(distance_matrix)}")
 
             # Get list of possible swaps
             exchange_indices = self._get_exchanges(cluster_assignment, i)
 
             if len(exchange_indices) == 0:
                 continue
 
             # Calculate objective value for all possible swaps.
             # List contains tuples of obj. val. and swapped element index.
             exchanges = [
-                (self._calculate_objective(self._swap(cluster_assignment, i, j), distance_matrix), j) for j in exchange_indices
+                (self._calculate_objective(self._swap(cluster_assignment, i, j), distance_matrix), j)
+                for j in exchange_indices
             ]
 
             # Find best swap
             best_exchange = max(exchanges)
 
             # If best swap is better than current objective value then complete swap
             if best_exchange[0] > current_objective:
```

### Comparing `anti-clustering-0.2.1/anti_clustering/naive_random_heuristic.py` & `anti_clustering-0.3.0/anti_clustering/naive_random_heuristic.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 from anti_clustering._cluster_swap_heuristic import ClusterSwapHeuristic
 
 
 class NaiveRandomHeuristicAntiClustering(ClusterSwapHeuristic):
     """
     The naive randomized way of solving the anti-clustering problem.
     """
+
     def __init__(self, verbose: bool = False, random_seed: int = None):
         super().__init__(verbose=verbose, random_seed=random_seed)
 
     def _solve(self, distance_matrix: npt.NDArray[float], num_groups: int) -> npt.NDArray[bool]:
         return self._get_random_clusters(num_groups=num_groups, num_elements=len(distance_matrix))
```

### Comparing `anti-clustering-0.2.1/anti_clustering/simulated_annealing_heuristic.py` & `anti_clustering-0.3.0/anti_clustering/simulated_annealing_heuristic.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,87 +8,104 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A simulated annealing approach to solving the anti-clustering problem.
+A simulated annealing with restarts approach to solving the anti-clustering problem.
 """
 
 import math
 import numpy as np
 import numpy.typing as npt
 from anti_clustering._cluster_swap_heuristic import ClusterSwapHeuristic
 
 
 class SimulatedAnnealingHeuristicAntiClustering(ClusterSwapHeuristic):
     """
-    A simulated annealing approach to solving the anti-clustering problem.
+    A simulated annealing with restarts approach to solving the anti-clustering problem.
     """
+
     def __init__(
         self,
         verbose: bool = False,
         random_seed: int = None,
         alpha: float = 0.9,
         iterations: int = 2000,
-        starting_temperature: float = 10
+        starting_temperature: float = 100,
+        restarts: int = 9,
     ):
         # pylint: disable = R0913
         super().__init__(verbose=verbose, random_seed=random_seed)
         self.alpha = alpha
         self.iterations = iterations
         self.starting_temperature = starting_temperature
+        self.restarts = restarts
 
     def _solve(self, distance_matrix: npt.NDArray[float], num_groups: int) -> npt.NDArray[bool]:
         # Start with random cluster assignment
         cluster_assignment = self._get_random_clusters(num_groups=num_groups, num_elements=len(distance_matrix))
 
         if self.verbose:
             print("Solving")
 
-        temperature = self.starting_temperature
-        # Initial objective value
-        objective = self._calculate_objective(cluster_assignment, distance_matrix)
-        for iteration in range(self.iterations):
-            if self.verbose and iteration % 5 == 0:
-                print(f'Iteration {iteration + 1} of {self.iterations}')
-
-            # Select random element
-            i = self.rnd.randint(0, len(distance_matrix) - 1)
-            # Get possible swaps
-            possible_exchanges = self._get_exchanges(cluster_assignment, i)
-            if len(possible_exchanges) == 0:
-                continue
-            # Select random possible swap.
-            j = possible_exchanges[self.rnd.randint(0, len(possible_exchanges)-1)]
-
-            new_cluster_assignment = self._swap(cluster_assignment, i, j)
-            new_objective = self._calculate_objective(new_cluster_assignment, distance_matrix)
-
-            # Select solution as current if accepted
-            if self._accept(new_objective - objective, temperature):
-                objective = new_objective
-                cluster_assignment = new_cluster_assignment
+        candidate_solutions = []
+
+        for restart in range(self.restarts):
+            temperature = self.starting_temperature
+            # Initial objective value
+            objective = self._calculate_objective(cluster_assignment, distance_matrix)
+            for iteration in range(self.iterations):
+                if self.verbose and iteration % 5 == 0:
+                    print(f"Iteration {iteration + 1} of {self.iterations}")
+
+                # Select random element
+                i = self.rnd.randint(0, len(distance_matrix) - 1)
+                # Get possible swaps
+                possible_exchanges = self._get_exchanges(cluster_assignment, i)
+                if len(possible_exchanges) == 0:
+                    continue
+                # Select random possible swap.
+                j = possible_exchanges[self.rnd.randint(0, len(possible_exchanges) - 1)]
+
+                new_cluster_assignment = self._swap(cluster_assignment, i, j)
+                new_objective = self._calculate_objective(new_cluster_assignment, distance_matrix)
+
+                # Select solution as current if accepted
+                if self._accept(new_objective - objective, temperature):
+                    objective = new_objective
+                    cluster_assignment = new_cluster_assignment
+
+                # Cool down temperature
+                temperature = temperature * self.alpha
+
+            candidate_solutions.append((objective, cluster_assignment))
+
+            if self.verbose:
+                print(f"Restart {restart + 1} of {self.restarts}")
+
+            # Cold restart, select random cluster assignment
+            cluster_assignment = self._get_random_clusters(num_groups=num_groups, num_elements=len(distance_matrix))
 
-            # Cool down temperature
-            temperature = temperature * self.alpha
+        # Select best solution, maximizing objective
+        _, best_cluster_assignment = max(candidate_solutions, key=lambda x: x[0])
 
-        return cluster_assignment
+        return best_cluster_assignment
 
     def _calculate_objective(self, cluster_assignment: npt.NDArray[bool], distance_matrix: npt.NDArray[float]) -> float:
         """
         Calculate objective value
         :param cluster_assignment: Cluster assignment
         :param distance_matrix: Distance matrix
         :return: Objective value
         """
         return np.multiply(cluster_assignment, distance_matrix).sum()
 
     def _accept(self, delta: float, temperature: float) -> bool:
         """
-        Simulated annealing acceptance function. Notice d/t is negated because this is a maximisation problem.
+        Simulated annealing acceptance function. Notice d/t is used instead of -d/t because we are maximizing.
         :param delta: Difference in objective
         :param temperature: Current temperature
         :return: Whether the solution is accepted or not.
         """
         return delta >= 0 or math.exp(delta / temperature) >= self.rnd.uniform(0, 1)
```

### Comparing `anti-clustering-0.2.1/setup.py` & `anti_clustering-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,85 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: anti-clustering
+Version: 0.3.0
+Summary: Generic Anti-Clustering
+Author: Matthias Als
+Author-email: mata@ecco.com
+Requires-Python: >=3.8,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.23.1,<2.0.0)
+Requires-Dist: ortools (==9.6.2534)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
+Requires-Dist: scipy (>=1.9.0,<2.0.0)
+Description-Content-Type: text/markdown
+
+# Anti-clustering
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A generic Python library for solving the anti-clustering problem. While clustering algorithms will achieve high similarity within a cluster and low similarity between clusters, the anti-clustering algorithms will achieve the opposite; namely to minimise similarity within a cluster and maximise the similarity between clusters.
+Currently, a handful of algorithms are implemented in this library:
+* An exact approach using a BIP formulation.
+* An enumerated exchange heuristic.
+* A simulated annealing heuristic.
+
+Keep in mind anti-clustering is computationally difficult problem and may run slow even for small instance sizes. The current ILP does not finish in reasonable time when anti-clustering the Iris dataset (150 data points).
+
+The two former approaches are implemented as described in following paper:\
+*Papenberg, M., & Klau, G. W. (2021). Using anticlustering to partition data sets into equivalent parts.
+Psychological Methods, 26(2), 161–174. [DOI](https://doi.org/10.1037/met0000301). [Preprint](https://psyarxiv.com/3razc/)* \
+The paper is accompanied by a library for the R programming language: [anticlust](https://github.com/m-Py/anticlust).
+
+Differently to the [anticlust](https://github.com/m-Py/anticlust) R package, this library currently only have one objective function. 
+In this library the objective will maximise intra-cluster distance: Euclidean distance for numerical columns and Hamming distance for categorical columns.
+
+## Use cases
+Within software testing, anti-clustering can be used for generating test and control groups in AB-testing.
+Example: You have a webshop with a number of users. The webshop is undergoing active development and you have a new feature coming up. 
+This feature should be tested against as many different users as possible without testing against the entire user-base. 
+For that you can create a maximally diverse subset of the user-base to test against (the A group). 
+The remaining users (B group) will not test this feature. For dividing the user-base you can use the anti-clustering algorithms. 
+A and B groups should be as similar as possible to have a reliable basis of comparison, but internally in group A (and B) the elements should be as dissimilar as possible.
+
+This is just one use case, probably many more exists.
+
+## Installation
+
+The anti-clustering package is available on [PyPI](https://pypi.org/project/anti-clustering/). To install it, run the following command:
+
+```bash
+pip install anti-clustering
+```
+
+The package currently supports Python 3.8 and above. 
+
+## Usage
+The input to the algorithm is a Pandas dataframe with each row representing a data point. The output is the same dataframe with an extra column containing integer encoded cluster labels. Below is an example based on the Iris dataset:
+```python
+from anti_clustering import ExactClusterEditingAntiClustering
+from sklearn import datasets
+import pandas as pd
+
+iris_data = datasets.load_iris(as_frame=True)
+iris_df = pd.DataFrame(data=iris_data.data, columns=iris_data.feature_names)
+
+algorithm = ExactClusterEditingAntiClustering()
+
+df = algorithm.run(
+    df=iris_df,
+    numerical_columns=list(iris_df.columns),
+    categorical_columns=None,
+    num_groups=2,
+    destination_column='Cluster'
+)
+```
 
-packages = \
-['anti_clustering']
+## Contributions
+If you have any suggestions or have found a bug, feel free to open issues. If you have implemented a new algorithm or know how to tweak the existing ones; PRs are very appreciated.
 
-package_data = \
-{'': ['*']}
+## License
+This library is licensed under the Apache 2.0 license.
 
-install_requires = \
-['numpy>=1.23.1,<1.24.0',
- 'ortools==9.3.10497',
- 'pandas>=1.4.4,<1.5.0',
- 'scikit-learn>=1.1.1,<1.2.0',
- 'scipy>=1.9.0,<1.10.0']
-
-setup_kwargs = {
-    'name': 'anti-clustering',
-    'version': '0.2.1',
-    'description': 'Generic Anti-Clustering',
-    'long_description': "# Anti-clustering\n\nA generic Python library for solving the anti-clustering problem. While clustering algorithms will achieve high similarity within a cluster and low similarity between clusters, the anti-clustering algorithms will achieve the opposite; namely to minimise similarity within a cluster and maximise the similarity between clusters.\nCurrently, a handful of algorithms are implemented in this library:\n* An exact approach using a BIP formulation.\n* An enumerated exchange heuristic.\n* A simulated annealing heuristic.\n\nKeep in mind anti-clustering is computationally difficult problem and may run slow even for small instance sizes. The current ILP does not finish in reasonable time when anti-clustering the Iris dataset (150 data points).\n\nThe two former approaches are implemented as described in following paper:\\\n*Papenberg, M., & Klau, G. W. (2021). Using anticlustering to partition data sets into equivalent parts.\nPsychological Methods, 26(2), 161–174. [DOI](https://doi.org/10.1037/met0000301). [Preprint](https://psyarxiv.com/3razc/)* \\\nThe paper is accompanied by a library for the R programming language: [anticlust](https://github.com/m-Py/anticlust).\n\nDifferently to the [anticlust](https://github.com/m-Py/anticlust) R package, this library currently only have one objective function. \nIn this library the objective will maximise intra-cluster distance: Euclidean distance for numerical columns and Hamming distance for categorical columns.\n\n## Use cases\nWithin software testing, anti-clustering can be used for generating test and control groups in AB-testing.\nExample: You have a webshop with a number of users. The webshop is undergoing active development and you have a new feature coming up. \nThis feature should be tested against as many different users as possible without testing against the entire user-base. \nFor that you can create a maximally diverse subset of the user-base to test against (the A group). \nThe remaining users (B group) will not test this feature. For dividing the user-base you can use the anti-clustering algorithms. \nA and B groups should be as similar as possible to have a reliable basis of comparison, but internally in group A (and B) the elements should be as dissimilar as possible.\n\nThis is just one use case, probably many more exists.\n\n## Installation\n\nThe anti-clustering package is available on [PyPI](https://pypi.org/project/anti-clustering/). To install it, run the following command:\n\n```bash\npip install anti-clustering\n```\n\nThe package currently supports Python 3.8 and above. \n\n## Usage\nThe input to the algorithm is a Pandas dataframe with each row representing a data point. The output is the same dataframe with an extra column containing integer encoded cluster labels. Below is an example based on the Iris dataset:\n```python\nfrom anti_clustering import ExactClusterEditingAntiClustering\nfrom sklearn import datasets\nimport pandas as pd\n\niris_data = datasets.load_iris(as_frame=True)\niris_df = pd.DataFrame(data=iris_data.data, columns=iris_data.feature_names)\n\nalgorithm = ExactClusterEditingAntiClustering()\n\ndf = algorithm.run(\n    df=iris_df,\n    numerical_columns=list(iris_df.columns),\n    categorical_columns=None,\n    num_groups=2,\n    destination_column='Cluster'\n)\n```\n\n## Contributions\nIf you have any suggestions or have found a bug, feel free to open issues. If you have implemented a new algorithm or know how to tweak the existing ones; PRs are very appreciated.\n\n## License\nThis library is licensed under the Apache 2.0 license.\n",
-    'author': 'Matthias Als',
-    'author_email': 'mata@ecco.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

