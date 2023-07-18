# Comparing `tmp/gc-ims-tools-0.1.5.tar.gz` & `tmp/gc-ims-tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gc-ims-tools-0.1.5.tar", last modified: Wed Mar  8 12:07:38 2023, max compression
+gzip compressed data, was "gc-ims-tools-0.1.6.tar", last modified: Mon Jul 17 13:23:58 2023, max compression
```

## Comparing `gc-ims-tools-0.1.5.tar` & `gc-ims-tools-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 12:07:38.740825 gc-ims-tools-0.1.5/
--rw-rw-rw-   0        0        0     1527 2023-03-08 12:07:38.740825 gc-ims-tools-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      961 2022-12-06 07:52:46.000000 gc-ims-tools-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-08 12:07:38.740825 gc-ims-tools-0.1.5/gc_ims_tools.egg-info/
--rw-rw-rw-   0        0        0     1527 2023-03-08 12:07:38.000000 gc-ims-tools-0.1.5/gc_ims_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-03-08 12:07:38.000000 gc-ims-tools-0.1.5/gc_ims_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 12:07:38.000000 gc-ims-tools-0.1.5/gc_ims_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-03-08 12:07:38.000000 gc-ims-tools-0.1.5/gc_ims_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-08 12:07:38.000000 gc-ims-tools-0.1.5/gc_ims_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-08 12:07:38.740825 gc-ims-tools-0.1.5/ims/
--rw-rw-rw-   0        0        0      783 2023-03-08 12:06:01.000000 gc-ims-tools-0.1.5/ims/__init__.py
--rw-rw-rw-   0        0        0    39829 2023-03-07 10:20:01.000000 gc-ims-tools-0.1.5/ims/dataset.py
--rw-rw-rw-   0        0        0    20862 2023-03-07 10:20:11.000000 gc-ims-tools-0.1.5/ims/gcims.py
--rw-rw-rw-   0        0        0     4193 2023-03-07 10:20:11.000000 gc-ims-tools-0.1.5/ims/hca.py
--rw-rw-rw-   0        0        0     9023 2023-03-08 11:57:14.000000 gc-ims-tools-0.1.5/ims/pca.py
--rw-rw-rw-   0        0        0    13587 2023-03-07 10:18:44.000000 gc-ims-tools-0.1.5/ims/plsda.py
--rw-rw-rw-   0        0        0    15484 2023-03-07 10:20:11.000000 gc-ims-tools-0.1.5/ims/plsr.py
--rw-rw-rw-   0        0        0     2227 2023-03-07 10:20:11.000000 gc-ims-tools-0.1.5/ims/utils.py
--rw-rw-rw-   0        0        0      108 2021-11-23 08:26:56.000000 gc-ims-tools-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      772 2023-03-08 12:07:38.740825 gc-ims-tools-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0       75 2021-12-13 13:52:13.000000 gc-ims-tools-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:23:58.729911 gc-ims-tools-0.1.6/
+-rw-rw-rw-   0        0        0     1527 2023-07-17 13:23:58.729911 gc-ims-tools-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2022-12-06 07:52:46.000000 gc-ims-tools-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:23:58.729911 gc-ims-tools-0.1.6/gc_ims_tools.egg-info/
+-rw-rw-rw-   0        0        0     1527 2023-07-17 13:23:58.000000 gc-ims-tools-0.1.6/gc_ims_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-07-17 13:23:58.000000 gc-ims-tools-0.1.6/gc_ims_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:23:58.000000 gc-ims-tools-0.1.6/gc_ims_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-17 13:23:58.000000 gc-ims-tools-0.1.6/gc_ims_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-17 13:23:58.000000 gc-ims-tools-0.1.6/gc_ims_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 13:23:58.729911 gc-ims-tools-0.1.6/ims/
+-rw-rw-rw-   0        0        0      783 2023-07-17 13:21:03.000000 gc-ims-tools-0.1.6/ims/__init__.py
+-rw-rw-rw-   0        0        0    41473 2023-07-17 12:38:55.000000 gc-ims-tools-0.1.6/ims/dataset.py
+-rw-rw-rw-   0        0        0    28882 2023-07-17 08:33:59.000000 gc-ims-tools-0.1.6/ims/gcims.py
+-rw-rw-rw-   0        0        0     4193 2023-04-20 12:36:39.000000 gc-ims-tools-0.1.6/ims/hca.py
+-rw-rw-rw-   0        0        0     9023 2023-03-08 11:57:14.000000 gc-ims-tools-0.1.6/ims/pca.py
+-rw-rw-rw-   0        0        0    13587 2023-03-07 10:18:44.000000 gc-ims-tools-0.1.6/ims/plsda.py
+-rw-rw-rw-   0        0        0    15484 2023-03-07 10:20:11.000000 gc-ims-tools-0.1.6/ims/plsr.py
+-rw-rw-rw-   0        0        0     3291 2023-05-26 07:09:05.000000 gc-ims-tools-0.1.6/ims/utils.py
+-rw-rw-rw-   0        0        0      108 2021-11-23 08:26:56.000000 gc-ims-tools-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      784 2023-07-17 13:23:58.729911 gc-ims-tools-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0       75 2021-12-13 13:52:13.000000 gc-ims-tools-0.1.6/setup.py
```

### Comparing `gc-ims-tools-0.1.5/PKG-INFO` & `gc-ims-tools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gc-ims-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Analyze GC-IMS data.
 Home-page: https://github.com/Charisma-Mannheim/gc-ims-tools
 Author: Charisma-Mannheim
 Author-email: charisma@hs-mannheim.de
 License: BSD 3-clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gc-ims-tools-0.1.5/README.md` & `gc-ims-tools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gc-ims-tools-0.1.5/gc_ims_tools.egg-info/PKG-INFO` & `gc-ims-tools-0.1.6/gc_ims_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gc-ims-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Analyze GC-IMS data.
 Home-page: https://github.com/Charisma-Mannheim/gc-ims-tools
 Author: Charisma-Mannheim
 Author-email: charisma@hs-mannheim.de
 License: BSD 3-clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gc-ims-tools-0.1.5/ims/__init__.py` & `gc-ims-tools-0.1.6/ims/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 (standard file format for G.A.S Dortmund instruments).
 
 * Preprocessing steps and utilities (alignment, resampling, plotting etc.).
 
 * Scripted statistical workflows with prebuilt plots
 for common algorithms.
 """
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 __author__ = "Competency Center for Chemometrics Mannheim"
 __credits__ = "Competency Center for Chemometrics Mannheim"
 
 from ims.gcims import Spectrum
 from ims.dataset import Dataset
 from ims.pca import PCA_Model
 from ims.plsr import PLSR
```

### Comparing `gc-ims-tools-0.1.5/ims/dataset.py` & `gc-ims-tools-0.1.6/ims/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -914,28 +914,81 @@
 
         self.data = means
         self.samples = list(u_samples)
         self.labels = labels
         self.preprocessing.append("mean()")
         return self
 
+    def asymcorr(self, lam=1e7, p=1e-3, niter=20):
+        """
+        Retention time baseline correction using asymmetric least squares.
+
+        Parameters
+        ----------
+        lam : float, optional
+            Controls smoothness. Larger numbers return smoother curves,
+            by default 1e7
+
+        p : float, optional
+            Controls asymmetry, by default 1e-3
+
+        niter : int, optional
+            Number of iterations during optimization,
+            by default 20
+
+        Returns
+        -------
+        Dataset
+        """
+        self.data = [Spectrum.asymcorr(i, lam, p, niter) for i in self.data]
+        self.preprocessing.append("asymcorr")
+        return self
+
+    def savgol(self, window_length=10, polyorder=2, direction="both"):
+        """
+        Applys a Savitzky-Golay filter to intensity values.
+        Can be applied in the drift time, retention time or both directions.
+
+        Parameters
+        ----------
+        window_length : int, optional
+            The length of the filter window, by default 10
+
+        polyorder : int, optional
+            The order of the polynomial used to fit the samples, by default 2
+
+        direction : str, optional
+            The direction in which to apply the filter.
+            Can be 'drift time', 'retention time' or 'both'.
+            By default 'both'
+
+        Returns
+        -------
+        Dataset
+        """
+        self.data = [
+            Spectrum.savgol(i, window_length, polyorder, direction) for i in self.data
+        ]
+        self.preprocessing.append("savgol")
+        return self
+
     def tophat(self, size=15):
         """
         Applies white tophat filter on data matrix as a baseline correction.
         Size parameter is the diameter of the circular structuring element.
         (Slow with large size values.)
 
         Parameters
         ----------
         size : int, optional
             Size of structuring element, by default 15.
 
         Returns
         -------
-        ims.Dataset
+        Dataset
         """
         self.data = [Spectrum.tophat(i, size) for i in self.data]
         self.preprocessing.append("tophat")
         return self
 
     def sub_first_rows(self, n=1):
         """
```

### Comparing `gc-ims-tools-0.1.5/ims/gcims.py` & `gc-ims-tools-0.1.6/ims/gcims.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,24 +8,30 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.ticker import AutoMinorLocator
 from datetime import datetime
 from time import ctime
 from skimage.morphology import white_tophat, disk
 from zipfile import ZipFile
+from ims.utils import asymcorr
+from findpeaks import findpeaks
+from scipy.signal import savgol_filter
+from scipy import ndimage as ndi
+from skimage.segmentation import watershed
 
 
 class Spectrum:
     """
     Represents one GCIMS-Spectrum with the data matrix,
     retention and drift time coordinates.
     Sample or file name and timestamp are included unique identifiers.
 
     This class contains all methods that can be applied on a per spectrum basis,
-    like I/O, plotting and some preprocessing tools. Methods that return a Spectrum change the instance inplace. Use the copy method.
+    like I/O, plotting and some preprocessing tools.
+    Methods that return a Spectrum change the instance inplace. Use the copy method.
 
 
     Parameters
     ----------
     name : str
         File or sample name as a unique identifier.
         Reader methods set this attribute to the file name without extension.
@@ -51,14 +57,15 @@
 
     def __init__(self, name, values, ret_time, drift_time, time):
         self.name = name
         self.values = values
         self.ret_time = ret_time
         self.drift_time = drift_time
         self.time = time
+        self.peak_table = None
         self._drift_time_label = "Drift time [ms]"
 
     def __repr__(self):
         return f"GC-IMS Spectrum: {self.name}"
 
     # add, radd and truediv are implemented to calculate means easily
     def __add__(self, other):
@@ -332,14 +339,253 @@
             f.create_dataset("values", data=self.values)
             f.create_dataset("ret_time", data=self.ret_time)
             f.create_dataset("drift_time", data=self.drift_time)
             f.attrs["name"] = self.name
             f.attrs["time"] = datetime.strftime(self.time, "%Y-%m-%dT%H:%M:%S")
             f.attrs["drift_time_label"] = self._drift_time_label
 
+    def find_peaks(self, limit=None, denoise="fastnl", window=30, verbose=0):
+        """
+        Automated GC-IMS peak detection based on persistent homology.
+
+        Parameters
+        ----------
+        spectrum : ims.Spectrum
+            GC-IMS spectrum to use.
+
+        limit : float
+            Values > limit are active search areas to detect regions of interest (ROI).
+            If None limit is selected by the minimum persistence score,
+            by default None.
+
+        denoise : string, (default : 'fastnl', None to disable)
+            Filtering method to remove noise:
+                * None
+                * 'fastnl'
+                * 'bilateral'
+                * 'lee'
+                * 'lee_enhanced'
+                * 'kuan'
+                * 'frost'
+                * 'median'
+                * 'mean'
+
+        window : int, (default : 30)
+            Denoising window. Increasing the window size may removes noise better but may also removes details of image in certain denoising methods.
+
+        verbose : int (default : 3)
+            Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace.
+
+        Returns
+        -------
+        pandas.DataFrame
+            Peak table with drift and retention times,
+            the correspondig x and y indices,
+            birth and death levels and scores.
+
+        References
+        ----------
+        Taskesen, E. (2020). findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image). (Version 2.3.1) [Computer software]. https://erdogant.github.io/findpeaks
+        """
+        if limit is None:
+            fp = findpeaks(
+                method="topology",
+                limit=0,
+                scale=True,
+                denoise=denoise,
+                window=window,
+                verbose=verbose,
+            )
+            fp.fit(self.values)
+            limit = fp.results["persistence"]["score"].min()
+
+        # actual peak detection
+        fp = findpeaks(
+            method="topology",
+            limit=limit,
+            scale=True,
+            denoise=denoise,
+            window=window,
+            verbose=verbose,
+        )
+        fp.fit(self.values)
+
+        # reindex to ensure consistent numbering and start at 1
+        df = fp.results["persistence"].reset_index(drop=True)
+        df.index = df.index + 1
+        df.index.name = "peak number"
+
+        df["x"] = df["x"].astype("int")
+        df["y"] = df["y"].astype("int")
+
+        # add the drift and retention time values for all indices
+        df.insert(0, "drift_time", self.drift_time[df["x"].values])
+        df.insert(2, "ret_time", self.ret_time[df["y"].values])
+        df.insert(0, "compound", "")
+
+        self.peak_table = df
+        return self
+
+    def plot_peaks(self):
+        """
+        Plots GC-IMS spectrum with peak labels from findpeaks method.
+
+        Returns
+        -------
+        matplotlib.pyplot.axes
+        """
+        if self.peak_table is None:
+            raise ValueError("Call 'find_peaks' method first.")
+
+        # call ims.Spectrum.plot method
+        _, ax = self.plot()
+
+        # iterate over peak table and add labels
+        for i, row in self.peak_table.iterrows():
+            x = row["drift_time"]
+            y = row["ret_time"]
+            label = f"{i} {row['compound']}"
+            ax.text(x, y, label, c="yellow", fontsize=12)
+
+        return ax
+
+    def plot_persistence(self):
+        """
+        Persistance plot of birth vs death levels from findpeak method.
+
+        Returns
+        -------
+        matplotlib.pyplot.axes
+        """
+        if self.peak_table is None:
+            raise ValueError("Call 'find_peaks' method first.")
+        
+        x = self.peak_table["birth_level"].values
+        y = self.peak_table["death_level"].values
+
+        ax = plt.subplot()
+        ax.plot(x, y, ".", c="tab:blue")
+
+        # draw line across plot
+        X = np.c_[x, y]
+        ax.plot([np.min(X), np.max(X)], [np.min(X), np.max(X)], "--", c="tab:grey")
+
+        # set axis limits and labels
+        ax.set_xlim((np.min(X), np.max(X)))
+        ax.set_ylim((np.min(X), np.max(X)))
+        ax.set_xlabel("Birth level")
+        ax.set_ylabel("Death level")
+
+        # add peak labels
+        for i, row in self.peak_table.iterrows():
+            x = row["birth_level"]
+            y = row["death_level"]
+            label = f"{i} {row['compound']}"
+            ax.text(x, y, label)
+
+        return ax
+
+    def watershed_segmentation(self, threshold):
+        """
+        Finds boundaries for overlapping peaks using watershed segmentation.
+        Requires peak_table for starting coordinates.
+
+        Parameters
+        ----------
+        threshold : int
+            Threshold is used to binarize the intensity values to calculate the distances.
+
+        Returns
+        -------
+        numpy.ndarray
+            Labels array with same shape as intensity values.
+        """
+        if self.peak_table is None:
+            raise ValueError("Call 'find_peaks' method first.")
+        
+        # Binarize intensity values
+        image = np.copy(self.values) >= threshold
+
+        # Generate the markers as local maxima of the distance to the background
+        distance = ndi.distance_transform_edt(image)
+
+        # Use x and y coordinates from the peak table
+        coords = self.peak_table[["y", "x"]].values
+
+        # Watershed segmentation according to scikit-image tutorial
+        mask = np.zeros(distance.shape, dtype=bool)
+        mask[tuple(coords.T)] = True
+        markers, _ = ndi.label(mask)
+        labels = watershed(-distance, markers, mask=image)
+        return labels
+
+    def asymcorr(self, lam=1e7, p=1e-3, niter=20):
+        """
+        Retention time baseline correction using asymmetric least squares.
+
+        Parameters
+        ----------
+        lam : float, optional
+            Controls smoothness. Larger numbers return smoother curves,
+            by default 1e7
+
+        p : float, optional
+            Controls asymmetry, by default 1e-3
+
+        niter : int, optional
+            Number of iterations during optimization,
+            by default 20
+
+        Returns
+        -------
+        Spectrum
+        """
+        for i in range(self.values.shape[1]):
+            y = self.values[:, i]
+            self.values[:, i] = asymcorr(y, lam=lam, p=p, niter=niter)
+
+        return self
+
+    def savgol(self, window_length=10, polyorder=2, direction="both"):
+        """
+        Applys a Savitzky-Golay filter to intensity values.
+        Can be applied in the drift time, retention time or both directions.
+
+        Parameters
+        ----------
+        window_length : int, optional
+            The length of the filter window, by default 10
+
+        polyorder : int, optional
+            The order of the polynomial used to fit the samples, by default 2
+
+        direction : str, optional
+            The direction in which to apply the filter.
+            Can be 'drift time', 'retention time' or 'both'.
+            By default 'both'
+
+        Returns
+        -------
+        Spectrum
+        """
+        if direction == "drift time":
+            axis = 1
+        elif direction == "retention time":
+            axis = 0
+        elif direction == "both":
+            self.values = savgol_filter(self.values, window_length, polyorder, axis=0)
+            axis = 1
+        else:
+            raise ValueError(
+                "Only 'drift time', 'retention time' or 'both' are valid options!"
+            )
+
+        self.values = savgol_filter(self.values, window_length, polyorder, axis=axis)
+        return self
+
     def tophat(self, size=15):
         """
         Applies white tophat filter on data matrix as a baseline correction.
         Size parameter is the diameter of the circular structuring element.
         (Slow with large size values.)
 
         Parameters
@@ -362,15 +608,14 @@
 
         Returns
         -------
         Spectrum
         """
         fl = self.values[0 : n - 1, :].mean(axis=0)
         self.values = self.values - fl
-        # self.values[self.values < 0] = 0
         return self
 
     def riprel(self):
         """
         Replaces drift time coordinate with RIP relative values.
         Useful to cut away the RIP because it´s position is set to 1.
 
@@ -571,15 +816,15 @@
 
         idx_start = np.abs(self.ret_time - start).argmin()
         idx_stop = np.abs(self.ret_time - stop).argmin()
         self.ret_time = self.ret_time[idx_start:idx_stop]
         self.values = self.values[idx_start:idx_stop, :]
         return self
 
-    def plot(self, vmin=30, vmax=400, width=9, height=10):
+    def plot(self, vmin=30, vmax=400, width=8, height=8):
         """
         Plots Spectrum using matplotlibs imshow.
         Use %matplotlib widget in IPython or %matplotlib notebook
         in jupyter notebooks to get an interactive plot widget.
         Returning the figure is needed to make the export plot utilities possible.
 
         Parameters
@@ -603,15 +848,14 @@
 
         Example
         -------
         >>> import ims
         >>> sample = ims.Spectrum.read_mea("sample.mea")
         >>> fig, ax = sample.plot()
         """
-
         fig, ax = plt.subplots(figsize=(width, height))
 
         plt.imshow(
             self.values,
             origin="lower",
             aspect="auto",
             cmap="RdBu_r",
```

### Comparing `gc-ims-tools-0.1.5/ims/hca.py` & `gc-ims-tools-0.1.6/ims/hca.py`

 * *Files identical despite different names*

### Comparing `gc-ims-tools-0.1.5/ims/pca.py` & `gc-ims-tools-0.1.6/ims/pca.py`

 * *Files identical despite different names*

### Comparing `gc-ims-tools-0.1.5/ims/plsda.py` & `gc-ims-tools-0.1.6/ims/plsda.py`

 * *Files identical despite different names*

### Comparing `gc-ims-tools-0.1.5/ims/plsr.py` & `gc-ims-tools-0.1.6/ims/plsr.py`

 * *Files identical despite different names*

### Comparing `gc-ims-tools-0.1.5/ims/utils.py` & `gc-ims-tools-0.1.6/ims/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import numpy as np
+from scipy import sparse
+from scipy.sparse.linalg import spsolve
+from scipy.spatial import ConvexHull
 
 
 def vip_scores(W, T, Q):
     """
     Calculates variable importance in projection (VIP) scores
     from PLS X weights, X scores, and y loadings.
 
@@ -69,7 +72,45 @@
 
     exp_var = (t_tp @ p_tp.T) ** 2
     exp_res = (X - exp_var) ** 2
 
     ss_expl = np.sum(exp_var, axis=0)
     ss_res = np.sum(exp_res, axis=0)
     return ss_expl / ss_res
+
+
+def asymcorr(y, lam=1e7, p=1e-3, niter=20):
+    """
+    Baseline correction using asymmetric least squares.
+
+    Parameters
+    ----------
+    y : numpy.ndarray of shape (1,)
+        Input spectrum or chromatogram.
+
+    lam : float, optional
+        Controls smoothness. Larger numbers return smoother curves,
+        by default 1e7.
+
+    p : float, optional
+        Controls asymmetry, by default 1e-3.
+
+    niter : int, optional
+        Number of iterations during optimization,
+        by default 20.
+
+    Returns
+    -------
+    numpy.ndarray of shape (1,)
+        Copy of input y with baseline subtracted.
+    """
+    L = len(y)
+    D = sparse.diags([1, -2, 1], [0, -1, -2], shape=(L, L - 2))
+    w = np.ones(L)
+
+    for _ in range(niter):
+        W = sparse.spdiags(w, 0, L, L)
+        Z = W + lam * D.dot(D.transpose())
+        z = spsolve(Z, w * y)
+        w = p * (y > z) + (1 - p) * (y < z)
+
+    return y - z
```

### Comparing `gc-ims-tools-0.1.5/setup.cfg` & `gc-ims-tools-0.1.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 632d 696d 732d 746f 6f6c 730d   = gc-ims-tools.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e35  .version = 0.1.5
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e36  .version = 0.1.6
 00000030: 0d0a 6175 7468 6f72 203d 2043 6861 7269  ..author = Chari
 00000040: 736d 612d 4d61 6e6e 6865 696d 0d0a 6175  sma-Mannheim..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2063 6861  thor_email = cha
 00000060: 7269 736d 6140 6873 2d6d 616e 6e68 6569  risma@hs-mannhei
 00000070: 6d2e 6465 0d0a 6465 7363 7269 7074 696f  m.de..descriptio
 00000080: 6e20 3d20 416e 616c 797a 6520 4743 2d49  n = Analyze GC-I
 00000090: 4d53 2064 6174 612e 0d0a 6c6f 6e67 5f64  MS data...long_d
@@ -39,11 +39,11 @@
 00000260: 6972 6573 203d 203e 3d33 2e38 0d0a 696e  ires = >=3.8..in
 00000270: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
 00000280: 200d 0a09 6e75 6d70 790d 0a09 7061 6e64   ...numpy...pand
 00000290: 6173 0d0a 0973 6369 7079 0d0a 096d 6174  as...scipy...mat
 000002a0: 706c 6f74 6c69 620d 0a09 7365 6162 6f72  plotlib...seabor
 000002b0: 6e0d 0a09 6835 7079 0d0a 0973 6369 6b69  n...h5py...sciki
 000002c0: 742d 6c65 6172 6e0d 0a09 7363 696b 6974  t-learn...scikit
-000002d0: 2d69 6d61 6765 0d0a 0d0a 5b65 6767 5f69  -image....[egg_i
-000002e0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000002f0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000300: 0d0a 0d0a                                ....
+000002d0: 2d69 6d61 6765 0d0a 0966 696e 6470 6561  -image...findpea
+000002e0: 6b73 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ks....[egg_info]
+000002f0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000300: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

