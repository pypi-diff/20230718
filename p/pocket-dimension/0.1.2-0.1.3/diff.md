# Comparing `tmp/pocket_dimension-0.1.2.tar.gz` & `tmp/pocket_dimension-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocket_dimension-0.1.2.tar", last modified: Tue Oct  4 00:53:12 2022, max compression
+gzip compressed data, was "pocket_dimension-0.1.3.tar", last modified: Tue Jul 18 03:03:37 2023, max compression
```

## Comparing `pocket_dimension-0.1.2.tar` & `pocket_dimension-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2022-10-04 00:53:12.028350 pocket_dimension-0.1.2/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    35149 2022-09-22 20:48:51.000000 pocket_dimension-0.1.2/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      575 2022-10-04 00:53:12.028350 pocket_dimension-0.1.2/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      970 2022-09-30 00:17:29.000000 pocket_dimension-0.1.2/README.rst
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2022-10-04 00:53:12.028350 pocket_dimension-0.1.2/pocket_dimension/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1167 2022-10-04 00:11:02.000000 pocket_dimension-0.1.2/pocket_dimension/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    15147 2022-09-30 21:51:48.000000 pocket_dimension-0.1.2/pocket_dimension/random_projection.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    16303 2022-09-30 20:59:20.000000 pocket_dimension-0.1.2/pocket_dimension/vectorizer.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2022-10-04 00:53:12.028350 pocket_dimension-0.1.2/pocket_dimension.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      575 2022-10-04 00:53:12.000000 pocket_dimension-0.1.2/pocket_dimension.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      398 2022-10-04 00:53:12.000000 pocket_dimension-0.1.2/pocket_dimension.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2022-10-04 00:53:12.000000 pocket_dimension-0.1.2/pocket_dimension.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       89 2022-10-04 00:53:12.000000 pocket_dimension-0.1.2/pocket_dimension.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       17 2022-10-04 00:53:12.000000 pocket_dimension-0.1.2/pocket_dimension.egg-info/top_level.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       89 2022-09-29 23:28:03.000000 pocket_dimension-0.1.2/pyproject.toml
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      849 2022-10-04 00:53:12.028350 pocket_dimension-0.1.2/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       68 2022-09-23 01:42:55.000000 pocket_dimension-0.1.2/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2022-10-04 00:53:12.028350 pocket_dimension-0.1.2/tests/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2022-09-23 02:57:18.000000 pocket_dimension-0.1.2/tests/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    14458 2022-09-30 21:05:16.000000 pocket_dimension-0.1.2/tests/test_pocket_dimension.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-18 03:03:37.193199 pocket_dimension-0.1.3/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    35149 2023-03-21 23:11:38.000000 pocket_dimension-0.1.3/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1546 2023-07-18 03:03:37.193199 pocket_dimension-0.1.3/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      970 2023-03-21 23:11:38.000000 pocket_dimension-0.1.3/README.rst
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-18 03:03:37.193199 pocket_dimension-0.1.3/pocket_dimension/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1167 2023-07-18 03:00:55.000000 pocket_dimension-0.1.3/pocket_dimension/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    15946 2023-07-18 03:00:55.000000 pocket_dimension-0.1.3/pocket_dimension/random_projection.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    17908 2023-07-18 03:00:55.000000 pocket_dimension-0.1.3/pocket_dimension/vectorizer.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-18 03:03:37.193199 pocket_dimension-0.1.3/pocket_dimension.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1546 2023-07-18 03:03:37.000000 pocket_dimension-0.1.3/pocket_dimension.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      380 2023-07-18 03:03:37.000000 pocket_dimension-0.1.3/pocket_dimension.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-07-18 03:03:37.000000 pocket_dimension-0.1.3/pocket_dimension.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       89 2023-07-18 03:03:37.000000 pocket_dimension-0.1.3/pocket_dimension.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       17 2023-07-18 03:03:37.000000 pocket_dimension-0.1.3/pocket_dimension.egg-info/top_level.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       89 2023-03-21 23:11:38.000000 pocket_dimension-0.1.3/pyproject.toml
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      885 2023-07-18 03:03:37.193199 pocket_dimension-0.1.3/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       68 2023-03-21 23:11:38.000000 pocket_dimension-0.1.3/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-18 03:03:37.193199 pocket_dimension-0.1.3/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    17468 2023-07-18 03:00:55.000000 pocket_dimension-0.1.3/tests/test_pocket_dimension.py
```

### Comparing `pocket_dimension-0.1.2/LICENSE` & `pocket_dimension-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pocket_dimension-0.1.2/README.rst` & `pocket_dimension-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pocket_dimension-0.1.2/pocket_dimension/__init__.py` & `pocket_dimension-0.1.3/pocket_dimension/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 
 from pocket_dimension.random_projection import (
     random_projection,
     distributional_johnson_lindenstrauss_optimal_delta,
     random_sparse_vectors,
     JustInTimeRandomProjection,
```

### Comparing `pocket_dimension-0.1.2/pocket_dimension/random_projection.py` & `pocket_dimension-0.1.3/pocket_dimension/random_projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+"""
+Pocket Dimension provides a memory-efficient, dense, random projection of sparse vectors
+and then applies this to Term Frequency (TF) and Term Frequency, Inverse Document
+Frequency (TFIDF) data.
+
+Copyright (C) 2022 Matthew Hendrey & Brendan Murphy
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
 from numba import njit, prange, float32, int64, uint64
 import numpy as np
 from sklearn.random_projection import (
     BaseRandomProjection,
     johnson_lindenstrauss_min_dim,
 )
 from sklearn.exceptions import DataDimensionalityWarning
@@ -58,15 +79,15 @@
     indices : np.ndarray, shape=(nnz,), dtype=int64
         The column indices of the nonzero elements in the sparse csr_matrix
     indptr : np.ndarray, shape=(n_rows+1,), dtype=int64
         Pointers into `data` and `indices` to indicate where the rows start and stop.
         If you have just a single record, then indtpr=[0, len(data)]
     d : int
         Embedding dimension of dense vectors.
-    
+
     Returns
     -------
     X : np.ndarray, shape=(n_rows, d), dtype=float32
         Dense 2-d array containing the randomly projected dense vectors for each row of
         the input sparse matrix.
     """
     assert data.shape == indices.shape, "Shape of data and indices do not match"
@@ -111,30 +132,30 @@
     M. Skorski. *Johnson-Lindenstrauss Transforms with Best Confidence*,
     Proceedings of Machine Learning Research **134**, 1 (2021)
 
     which can be found at http://proceedings.mlr.press/v134/skorski21a/skorski21a.pdf
 
     If :math:`\mathbf{A}` is the random projection matrix, then :math:`\delta` is the
     probability of exceeding error limits given by
-    
+
     .. math::
 
         \delta = \mathbb{P} \lbrack \\vert \Vert \mathbf{A}x \Vert^2_2 -
         \Vert x \Vert^2_2 \\vert > \epsilon \Vert x \Vert^2_2 {\\rbrack}
-    
-    
+
+
     Parameters
     ----------
     sparse_dim : int
         Original dimension of the data
     n_components : int
         Embedding dimension
     eps : float
         Error rate
-    
+
     Returns
     -------
     delta : float
         The best probability of failure that you can expect
     """
     a = n_components / 2.0
     b = (sparse_dim - n_components) / 2.0
@@ -155,15 +176,15 @@
     else:
         return delta
 
 
 def random_sparse_vectors(
     n_samples: int,
     *,
-    sparse_dim: int = 2 ** 31 - 1,
+    sparse_dim: int = 2**31 - 1,
     min_n_features: int = 20,
     max_n_features: int = 100,
     normalize: bool = False,
     rng: np.random.Generator = None,
 ) -> csr_matrix:
     """
     Randomly generate sparse vectors for testing
@@ -187,15 +208,15 @@
     -------
     csr_matrix
         Shape is (n_samples, sparse_dim)
     """
     if rng is None:
         rng = np.random.default_rng()
 
-    if sparse_dim >= 2 ** 31:
+    if sparse_dim >= 2**31:
         raise ValueError(
             f"{sparse_dim=:,} must be below 2**31 due to csr_matrix limits"
         )
     n_features = rng.integers(min_n_features, max_n_features, n_samples)
     data = rng.uniform(1.0, 20.0, np.sum(n_features)).astype(np.float32)
     data = data * rng.choice([-1, 1], np.sum(n_features)).astype(np.float32)
     indices = rng.integers(0, sparse_dim, np.sum(n_features)).astype(np.int32)
@@ -239,45 +260,45 @@
     than SparseRandomProjection.
 
     Parameters
     ----------
     n_components : int or 'auto', default = 'auto'
         Dimensionality of the target projection space. If not a multiple of 64, then
         it will be rounded down to the nearest multiple of 64.
-        
+
         If 'auto', then it will pick a dimensionality that satisfies the
         Johnson-Lindenstrauss Lemma based upon the ``eps`` parameter. The
         dimensionality will then be rounded up to the nearest multiple of 64
         to ensure you satisfy the conditions in the lemma.
-        
+
         **NOTE** This can yield a very conservative estimate of the required
         dimensionality.
     eps : float, default = 0.1
         Parameter to control the quality of the embedding according to the
         Johnson-Lindenstrauss Lemma. This is used if ``n_components`` is 'auto'.
         This represents the error rate between distances in the sparse dimension
         and the resulting lower embedding dimension. Smaller values of ``eps``
         give larger values of ``n_components``.
-    
+
     Attributes
     ----------
     n_components_ : int
         Dimensionality of the embedding dimension. It will be a multiple of 64.
-    
+
     Examples
     --------
 
     ::
 
         import numpy as np
         from pocket_dimension.random_projection import (
             JustInTimeRandomProjection,
             random_sparse_vectors,
         )
-        
+
         n_components = 256
         sparse_dim = 1_073_741_824
         n_samples = 100_000
         X = random_sparse_vectors(n_samples, sparse_dim=sparse_dim, normalize=True)
 
         transformer = JustInTimeRandomProjection(n_components)
         # No need to fit if provide a value for n_components at initialization
@@ -357,15 +378,15 @@
         matrix.
 
         Parameters
         ----------
         X : csr_matrix
             The input data to project into a smaller dimensional space. Shape is
             (n_samples, sparse_dim)
-        
+
         Returns
         -------
         np.ndarray
             Projected data of shape (n_samples, n_components)
         """
         check_is_fitted(self)
         X = self._validate_data(
@@ -390,14 +411,14 @@
 
         Parameters
         ----------
         n_components : int
             The embedding dimension
         n_features : int
             The sparse starting dimension
-        
+
         Returns
         -------
         np.ndarray
             Empty array to conform to BaseRandomProjection, the parent class
         """
         return np.array([])
```

### Comparing `pocket_dimension-0.1.2/pocket_dimension/vectorizer.py` & `pocket_dimension-0.1.3/pocket_dimension/vectorizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     Parameters
     ----------
     doc_freq : float32
         Number of records that contain this particular feature.
     n_records : float32
         Total number of records in the data set.
-    
+
     Returns
     -------
     float32
     """
     idf = np.log10(max(float32(1.0), n_records / (float32(1.0) + doc_freq)))
     return idf
 
@@ -120,18 +120,20 @@
     """
 
     def __init__(
         self,
         d: int,
         *,
         cms_file: Union[str, Path] = None,
-        hash_dim: int = 2 ** 31 - 1,
+        hash_dim: int = 2**31 - 1,
         minDF: int = 1,
-        maxDF: int = 2 ** 32 - 1,
+        maxDF: int = 2**32 - 1,
         temperature: float = 1.0,
+        min_n_features: int = 1,
+        min_n_observations: int = 1,
         filter: str = None,
         filter_out: bool = True,
     ):
         """
         Initialize the a Term-Frequency vectorizer. All optional parameters must be
         passed as keyword arguments. That is, everything but the embedding dimension
         `d`.
@@ -155,34 +157,47 @@
             Maximum document frequency (number of records with this feature) a feature
             can have to be included in the embedding. Default is 2\*\*32 - 1.
         temperature : float, optional
             Option to reshape the term frequency vector by raising each count to
             (1/temperature). Using a value above 1.0 flattens the values relative to
             each other. Using a value below 1.0 sharpens the contrast of values
             relative to each other.
+        min_n_features : int, optional
+            Must have at least this many features in order to create a vector. Useful
+            as a data quality check. Default is 1
+        min_n_observations : int, optional
+            Must have at least his many observations in order to create a vector.
+            Useful as a data quality check. This is the sum of counts over the
+            different features for a given item. Default is 1
         filter : pybloomfilter3, option
             Bloom filter to use for filtering features before creating sparse vectors.
             Default is None
         filter_out : bool, optional
             If True, then remove features that are in the filter before making the
             sparse vector. If False, then only use features that are in the filter in
             the sparse vector. Not used if `filter` is None. Default is True.
         """
         if d % 64 != 0:
             d = 64 * max(1, int(d // 64))
             logger.warning(f"d is not a multiple of 64. Changing it to {d}")
         assert d < hash_dim, f"{d=:} must be less than {hash_dim=:}"
-        assert temperature > 0.0, f"{temperature=:} must be positive value"
+        assert temperature > 0.0, f"{temperature=:} must be non-negative value"
+        assert min_n_features > 0, f"{min_n_features=:} must be positive integer"
+        assert (
+            min_n_observations > 0
+        ), f"{min_n_observations=:} must be positive integer"
         assert minDF <= maxDF, f"{minDF} must be <= {maxDF}"
 
         self.d = d
         self.hash_dim = hash_dim
         self.minDF = minDF
         self.maxDF = maxDF
         self.temperature = temperature
+        self.min_n_features = min_n_features
+        self.min_n_observations = min_n_observations
         self.filter_out = filter_out
         self.one_over_temp = 1.0 / temperature
         self.hasher = FeatureHasher(
             hash_dim, input_type="pair", alternate_sign=True, dtype="float32"
         )
         self.jit_rp = JustInTimeRandomProjection(n_components=self.d)
 
@@ -205,15 +220,15 @@
         the random projection. The vectors are then normalized to unit length.
 
         Parameters
         ----------
         records: Iterable[Dict]
             Iterable of records where each record has
             {"id": str, "features": List[bytes], "counts": List[int]}
-        
+
         Returns
         -------
         X : np.ndarray, shape = [n_records, d]
             Resulting dense vector representation of the records. Each vector is
             normalized to unit length.
         ids : np.ndarray, shape = [n_records,]
             Array listing the record's id in order to track which row in X corresponds
@@ -244,99 +259,119 @@
         **NOTE** For TFVectorizer, this simply returns 1.0. Included here for
         compatability with TFIDFVectorizer
 
         Parameters
         ----------
         doc_freq : float
             A document frequency
-        
+
         Returns
         -------
         idf : float
             The inverse document frequency
         """
         return 1.0
 
-    def yield_features_counts(
+    def filter_reweight_features(
         self, features: List[bytes], counts: List[int]
-    ) -> Tuple[bytes, float]:
+    ) -> List[Tuple[bytes, float]]:
         """
-        Yield the individual feature and count where the count is scaled by raising it
-        to :math:`1/temperature` and then multiplied by the idf value. For TFVectorizer
-        the idf = 1.0.
-
-        If ``minDF` and ``maxDF`` or a ``filter`` is provided, then the individual
-        features will be filtered appropriately. Only those that pass the filters will
-        contribute to the final vector.
+        Filter the features accordingly and reweight the associated counts. The counts
+        are scaled by raising them to :math:`1/temperature` and then multiplied by the
+        ``idf`` value. For TFVectorizer :math:`idf=1.0`.
+
+        Features will be filtered out if their document frequency is not within
+        [``minDF``, ``maxDF``] and if a ``filter`` is provided during initialization.
+        Only those features that pass the filters will contribute to the final vector.
+
+        After filtering, a final check is done to ensure that there are at least
+        ``min_n_features`` features remaining and that there are at least
+        ``min_n_observations`` observations of those features. Otherwise an empty list
+        is returned.
 
         Parameters
         ----------
         features : List[bytes]
             List of the individual features. These will be hashed by the FeatureHasher
             to turn into a sparse vector representation
         counts : List[int]
             Number of times that feature is present in a given record.
-        
-        Yields
+
+        Returns
         ------
-        Tuple[bytes, float]
+        List[Tuple[bytes, float]]
         """
-        if self.temperature != 1.0:
-            counts = np.array(counts) ** self.one_over_temp
+        values = np.array(counts) ** self.one_over_temp
 
-        for f, c in zip(features, counts):
+        features_values = []
+        n_features = 0
+        n_observations = 0
+        for i in range(len(features)):
+            f = features[i]
+            v = values[i]
             doc_freq = self.cms[f]
             if ((f in self.filter) != self.filter_out) and (
                 self.minDF <= doc_freq and doc_freq <= self.maxDF
             ):
-                yield (f, c * self._idf(doc_freq))
+                features_values.append((f, v * self._idf(doc_freq)))
+                n_features += 1
+                n_observations += counts[i]
+
+        if (
+            n_features >= self.min_n_features
+            and n_observations >= self.min_n_observations
+        ):
+            return features_values
+        else:
+            return []
 
     def yield_record(self, records: Iterable[Dict], ids: List):
         """
-        Yields a generator of an individual record's features/counts.
+        Yields a list of an individual record's (features, values) where the values are
+        the counts after reweighting them by ``temperature`` and/or ``idf``.
 
         Parameters
         ----------
         records : Iterable[Dict]
             An iterable of records where each records is a dict of
             {"id": str, "features": List[bytes], "counts": List[int]}
         ids : List
             Pass in an empty list which will be returned with corresponding ids from
             the `records` passed in
-        
+
         Yields
         ------
-        Generator
-            Of the appropriate individual (features,counts) for a given record
+        List[Tuple[bytes, float]]
+            Of the appropriate individual (feature, value) for a given record
         """
         for rec in records:
             ids.append(rec["id"])
-            yield self.yield_features_counts(rec["features"], rec["counts"])
+            yield self.filter_reweight_features(rec["features"], rec["counts"])
 
 
 class TFIDFVectorizer(TFVectorizer):
     """
     Randomly project records by first applying a high-dimensional feature hasher
     to create a sparse vector representation of the tf-idf and then applying the
     random projection to a dense embedding dimension.
 
     .. math::
 
         tfidf = c^{1/temp} \log{10}(n\_records / (doc\_freq + 1))
-    
+
     """
 
     def __init__(
         self,
         d: int,
         cms_file: Union[str, Path],
         *,
-        hash_dim: int = 2 ** 31 - 1,
+        hash_dim: int = 2**31 - 1,
         minDF: int = 1,
-        maxDF: int = 2 ** 32 - 1,
+        maxDF: int = 2**32 - 1,
         temperature: float = 1.0,
         filter: str = None,
         filter_out: bool = True,
     ):
         """
         Initialize a Term-Frequency, Inverse Document-Frequency vectorizer. All
         optional parameters must be passed as keyword arguments. That is, everything
@@ -395,14 +430,14 @@
         max is used because we are using a count-min sketch to estimate the document
         frequencies which may result in the denominator be bigger than N.
 
         Parameters
         ----------
         doc_freq : float
             A document frequency
-        
+
         Returns
         -------
         idf : float
             The inverse document frequency
         """
         return numba_idf(doc_freq, self.cms.n_records())
```

### Comparing `pocket_dimension-0.1.2/setup.cfg` & `pocket_dimension-0.1.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 	Documentation = https://mhendrey.github.io/pocket_dimension
 author = Matthew Hendrey
 author_email = matthew.hendrey@gmail.com
 classifiers = 
 	Programming Language :: Python :: 3
 license = GNU GPLv3
 description = Memory-efficient, dense, random projection of sparse vectors
+long_description = file: README.rst
 keywords = numba, random projection, term-frequency, tfidf, dimension reduction
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires =
```

### Comparing `pocket_dimension-0.1.2/tests/test_pocket_dimension.py` & `pocket_dimension-0.1.3/tests/test_pocket_dimension.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,29 +45,32 @@
     Calculate the distance between two sparse vectors
     """
     total = 0.0
     for idx, value in zip(S1.indices, S1.data):
         if idx in S2.indices:
             total += (value - S2.data[idx]) ** 2
         else:
-            total += value ** 2
+            total += value**2
     for idx, value in zip(S2.indices, S2.data):
         if idx in S1.indices:
             total += 0.0  # already accounted for above
         else:
-            total += value ** 2
+            total += value**2
     return total
 
 
 def test_johnson_lindenstrauss(
-    n: int = 40, min_n_features: int = 5, max_n_features: int = 100, eps: float = 0.05,
+    n: int = 40,
+    min_n_features: int = 5,
+    max_n_features: int = 100,
+    eps: float = 0.05,
 ):
     """
     Test the the Johnson-Lindenstrauss Lemma holds between the sparse vectors and the
-    randomly projected dense vectors. This uses the results found in 
+    randomly projected dense vectors. This uses the results found in
 
     https://cs.stanford.edu/people/mmahoney/cs369m/Lectures/lecture1.pdf
 
     This checkes that the ratio of the distance between two vectors in the embedding
     to the distance between the original sparse vectors is between (1-eps) and (1+eps).
     The embedding dimension is determined by the requested error rate, eps.
 
@@ -114,15 +117,15 @@
 
 
 def test_distributional_johnson_lindenstrauss(
     n: int = 1000,
     min_n_features: int = 5,
     max_n_features: int = 100,
     eps: float = 0.1,
-    delta_pad: float = 0.005,
+    delta_pad: float = 0.01,
 ):
     """
     Test the statistical guarantees of the Distributional Johnson-Lindenstrauss Lemma
     using a method for finding the best possible delta (failure rate) for a given
     epsilon (error rate) of the difference of the L2 norm between vectors in the
     original dimension (x) and the lower embedding dimension (Ax) described in
 
@@ -146,43 +149,43 @@
     max_n_features : int, optional
         Maximum number of features any given vector may have. Default is 100
     eps : float, optional
         Error rate. Default is 0.1
     delta_pad : float, optional
         Amount by which we pad the calculated best delta value. This is done to reduce
         the probability of failure given the vagaries of running statistical tests.
-        Default is 0.005
+        Default is 0.01
     """
     S = random_sparse_vectors(
         n, min_n_features=min_n_features, max_n_features=max_n_features
     )
 
     for d in [64, 128, 256, 512, 1024, 2048]:
         X = random_projection(
             S.data.astype(np.float32),
             S.indices.astype(np.int64),
             S.indptr.astype(np.int64),
             d,
         )
         delta = (
-            distributional_johnson_lindenstrauss_optimal_delta(2 ** 31 - 1, d, eps)
+            distributional_johnson_lindenstrauss_optimal_delta(2**31 - 1, d, eps)
             + delta_pad
         )
         metric = np.zeros(n)
         for i in range(n):
             x2 = np.sum(np.square(X[i]))
             s2 = np.sum(np.square(S[i].data))
             metric[i] = np.abs(x2 / s2 - 1)
         failure_prob = metric[metric > eps].shape[0] / metric.shape[0]
         assert failure_prob <= delta, f"{failure_prob=:.4f} exceeded {delta=:.4f}"
 
 
 def test_tf(d: int = 64):
     """
-    Basic test that things look right. 
+    Basic test that things look right.
 
     Parameters
     ----------
     d : int, optional
         Embedding dimension. Default is 64
     """
     records = [
@@ -192,22 +195,22 @@
     ]
 
     embedder = TFVectorizer(d)
     X, ids = embedder(records)
 
     assert X.shape == (3, d)
     assert X.dtype == np.float32
-    cosine_0_2 = X[0].dot(X[1])
-    assert cosine_0_2 == approx(1.0), f"{cosine_0_2=:.5f} should be 1.0"
+    cosine_0_1 = X[0].dot(X[1])
+    assert cosine_0_1 == approx(1.0), f"{cosine_0_1=:.5f} should be 1.0"
     assert ids.shape == (3,)
     assert ids[0] == "one"
     assert ids[1] == "two"
     assert ids[2] == "three"
-    cosine_1_3 = X[0].dot(X[2])
-    assert cosine_1_3 < 0.25, f"{cosine_1_3=:.5f} should be small"
+    cosine_0_2 = X[0].dot(X[2])
+    assert cosine_0_2 < 0.25, f"{cosine_0_2=:.5f} should be small"
 
 
 def test_tf_filter(tmp_path, d: int = 64):
     """
     Testing the bloom filter & filter_out parameters for the TFVectorizer
     """
     records = [
@@ -316,15 +319,61 @@
 
     """
     Test that we drop "e" and "f" from records one & two. They should now match
     the unfiltered three record.
     """
     embedder = TFVectorizer(d, cms_file=cms_file, minDF=3, maxDF=100)
     X, _ = embedder(records)
-    for i in range(2):
+    for i in range(3):
+        assert X[i].dot(X_nofilter[2]) == approx(1.0), f"{i} was not filtered"
+
+    """
+    Test that we get back no results if min_n_features is not enough
+    """
+    embedder = TFVectorizer(d, cms_file=cms_file, minDF=3, maxDF=100, min_n_features=5)
+    X, _ = embedder(records)
+    assert X.shape == (0, d), f"{X.shape} should be (0, {d})"
+
+    """
+    Test that we get back results if min_n_features enough
+    """
+    embedder = TFVectorizer(d, cms_file=cms_file, minDF=3, maxDF=100, min_n_features=4)
+    X, _ = embedder(records)
+    assert X.shape == (3, d), f"{X.shape} should be (3, {d})"
+    for i in range(3):
+        assert X[i].dot(X_nofilter[2]) == approx(1.0), f"{i} was not filtered"
+
+    """
+    Test that we get back no results if min_n_observations is not met
+    """
+    embedder = TFVectorizer(
+        d,
+        cms_file=cms_file,
+        minDF=3,
+        maxDF=100,
+        min_n_features=4,
+        min_n_observations=11,
+    )
+    X, _ = embedder(records)
+    assert X.shape == (0, d), f"{X.shape} should be (0, {d})"
+
+    """
+    Test that we get back results if min_n_observations is met
+    """
+    embedder = TFVectorizer(
+        d,
+        cms_file=cms_file,
+        minDF=3,
+        maxDF=100,
+        min_n_features=4,
+        min_n_observations=10,
+    )
+    X, _ = embedder(records)
+    assert X.shape == (3, d), f"{X.shape} should be (3, {d})"
+    for i in range(3):
         assert X[i].dot(X_nofilter[2]) == approx(1.0), f"{i} was not filtered"
 
 
 def test_tf_temp(d: int = 64):
     """
     Test that changing the temperature used during embedding changes the cosine in an
     expected way
@@ -403,15 +452,19 @@
             "counts": [1, 2, 3, 4, 5],
         },
         {
             "id": "two",
             "features": [b"a", b"b", b"c", b"d", b"e"],
             "counts": [1, 2, 3, 4, 5],
         },
-        {"id": "three", "features": [b"a", b"b", b"c", b"d"], "counts": [1, 2, 3, 4],},
+        {
+            "id": "three",
+            "features": [b"a", b"b", b"c", b"d"],
+            "counts": [1, 2, 3, 4],
+        },
     ]
     cms_file = str(tmp_path / "tf_cms.npz")
     cms = CountMin("linear", width=300)
     cms.n_added_records[1] = 500
     cms.update([b"a"] * 3)
     cms.update([b"b"] * 5)
     cms.update([b"c"] * 10)
@@ -423,7 +476,51 @@
     Test that with no filtering, the records have cosine != 1.0
     """
     embedder = TFIDFVectorizer(d, cms_file=cms_file)
     X, _ = embedder(records)
 
     # Now the b"e" should contribute nothing to the vector since idf = 0.0
     assert X[0].dot(X[2]) == approx(1.0)
+
+
+def test_tf_data_quality(d: int = 64):
+    """
+    Test that records without minimium data quality (min_n_features &
+    min_n_observations) return vectors
+
+    Parameters
+    ----------
+    d : int, optional
+        Embedding dimension. Default is 64
+    """
+    records = [
+        {"id": "one", "features": [b"a", b"b", b"c"], "counts": [6, 6, 6]},
+        {"id": "two", "features": [b"a", b"b", b"c"], "counts": [5, 5, 5]},
+        {"id": "three", "features": [b"a", b"b", b"c"], "counts": [1, 1, 1]},
+        {"id": "four", "features": [b"a", b"b"], "counts": [20, 20]},
+        {"id": "five", "features": [b"a", b"b"], "counts": [1, 1]},
+    ]
+
+    embedder = TFVectorizer(d, min_n_features=3, min_n_observations=15)
+    X, ids = embedder(records)
+    assert X.shape == (2, d)
+    assert ids[0] == "one"
+    assert ids[1] == "two"
+    cosine_0_1 = X[0].dot(X[1])
+    assert cosine_0_1 == approx(1.0), f"{cosine_0_1=:.5f} should be 1.0"
+
+    embedder = TFVectorizer(d, min_n_features=3, min_n_observations=16)
+    X, ids = embedder(records)
+    assert X.shape == (1, d)
+    assert ids[0] == "one"
+
+    embedder = TFVectorizer(d, min_n_features=2, min_n_observations=3)
+    X, ids = embedder(records)
+    assert X.shape == (4, d)
+    assert ids[0] == "one"
+    assert ids[1] == "two"
+    assert ids[2] == "three"
+    assert ids[3] == "four"
+    cosine_0_1 = X[0].dot(X[1])
+    assert cosine_0_1 == approx(1.0), f"{cosine_0_1=:.5f} should be 1.0"
+    cosine_0_2 = X[0].dot(X[2])
+    assert cosine_0_2 == approx(1.0), f"{cosine_0_2=:.5f} should be 1.0"
```

