# Comparing `tmp/gnss_lib_py-0.1.8.tar.gz` & `tmp/gnss_lib_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnss_lib_py-0.1.8.tar", max compression
+gzip compressed data, was "gnss_lib_py-0.1.9.tar", max compression
```

## Comparing `gnss_lib_py-0.1.8.tar` & `gnss_lib_py-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2022-12-17 05:33:47.992891 gnss_lib_py-0.1.8/LICENSE
--rw-r--r--   0        0        0     6739 2022-12-17 05:33:47.992891 gnss_lib_py-0.1.8/README.md
--rw-r--r--   0        0        0        0 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/__init__.py
--rw-r--r--   0        0        0     9371 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/algorithms/gnss_filters.py
--rw-r--r--   0        0        0     3801 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/algorithms/residuals.py
--rw-r--r--   0        0        0     7676 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/algorithms/snapshot.py
--rw-r--r--   0        0        0    22692 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/parsers/android.py
--rw-r--r--   0        0        0    15433 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/parsers/ephemeris.py
--rw-r--r--   0        0        0    48095 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/parsers/navdata.py
--rw-r--r--   0        0        0    34694 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/parsers/precise_ephemerides.py
--rw-r--r--   0        0        0     1759 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/utils/constants.py
--rw-r--r--   0        0        0    18580 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/utils/coordinates.py
--rw-r--r--   0        0        0      888 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/utils/file_operations.py
--rw-r--r--   0        0        0    11986 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/utils/filters.py
--rw-r--r--   0        0        0    23083 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/utils/sim_gnss.py
--rw-r--r--   0        0        0    13429 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/utils/time_conversions.py
--rw-r--r--   0        0        0    32194 2022-12-17 05:33:48.032892 gnss_lib_py-0.1.8/gnss_lib_py/utils/visualizations.py
--rw-r--r--   0        0        0     1352 2022-12-17 05:33:48.064893 gnss_lib_py-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8117 1970-01-01 00:00:00.000000 gnss_lib_py-0.1.8/setup.py
--rw-r--r--   0        0        0     8262 1970-01-01 00:00:00.000000 gnss_lib_py-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-05 22:56:56.120860 gnss_lib_py-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6739 2023-05-05 22:56:56.120860 gnss_lib_py-0.1.9/README.md
+-rw-r--r--   0        0        0      796 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/__init__.py
+-rw-r--r--   0        0        0     9603 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/algorithms/gnss_filters.py
+-rw-r--r--   0        0        0     3314 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/algorithms/residuals.py
+-rw-r--r--   0        0        0     9890 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/algorithms/snapshot.py
+-rw-r--r--   0        0        0    23478 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/android.py
+-rw-r--r--   0        0        0    21479 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/ephemeris.py
+-rw-r--r--   0        0        0    56305 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/navdata.py
+-rw-r--r--   0        0        0    31911 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/precise_ephemerides.py
+-rw-r--r--   0        0        0     9291 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/parsers/smart_loc.py
+-rw-r--r--   0        0        0     2658 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/constants.py
+-rw-r--r--   0        0        0    19067 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/coordinates.py
+-rw-r--r--   0        0        0      888 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/file_operations.py
+-rw-r--r--   0        0        0    11986 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/filters.py
+-rw-r--r--   0        0        0    25777 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/sim_gnss.py
+-rw-r--r--   0        0        0    13571 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/time_conversions.py
+-rw-r--r--   0        0        0    32216 2023-05-05 22:56:56.172863 gnss_lib_py-0.1.9/gnss_lib_py/utils/visualizations.py
+-rw-r--r--   0        0        0     1389 2023-05-05 22:56:56.204865 gnss_lib_py-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8295 1970-01-01 00:00:00.000000 gnss_lib_py-0.1.9/PKG-INFO
```

### Comparing `gnss_lib_py-0.1.8/LICENSE` & `gnss_lib_py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.8/README.md` & `gnss_lib_py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/algorithms/gnss_filters.py` & `gnss_lib_py-0.1.9/gnss_lib_py/algorithms/gnss_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from gnss_lib_py.parsers.navdata import NavData
 from gnss_lib_py.algorithms.snapshot import solve_wls
 from gnss_lib_py.utils.coordinates import ecef_to_geodetic
 from gnss_lib_py.utils.filters import BaseExtendedKalmanFilter
 
 def solve_gnss_ekf(measurements, init_dict = None,
-                   params_dict = None):
+                   params_dict = None, delta_t_decimals=-2):
     """Runs a GNSS Extended Kalman Filter across each timestep.
 
     Runs an Extended Kalman Filter across each timestep and adds a new
     row for the receiver's position and clock bias.
 
     Parameters
     ----------
@@ -46,23 +46,24 @@
                           ])
 
     if init_dict is None:
         init_dict = {}
 
     if "state_0" not in init_dict:
         pos_0 = None
-        for _, _, measurement_subset in measurements.loop_time("gps_millis"):
+        for _, _, measurement_subset in measurements.loop_time("gps_millis",
+                                        delta_t_decimals=delta_t_decimals):
             pos_0 = solve_wls(measurement_subset)
             if pos_0 is not None:
                 break
 
         state_0 = np.zeros((7,1))
         if pos_0 is not None:
-            state_0[:3,0] = pos_0[["x_rx_m","y_rx_m","z_rx_m"]]
-            state_0[6,0] = pos_0[["b_rx_m"]]
+            state_0[:3,0] = pos_0[["x_rx_wls_m","y_rx_wls_m","z_rx_wls_m"]]
+            state_0[6,0] = pos_0[["b_rx_wls_m"]]
 
         init_dict["state_0"] = state_0
 
     if "sigma_0" not in init_dict:
         sigma_0 = np.eye(init_dict["state_0"].size)
         init_dict["sigma_0"] = sigma_0
 
@@ -116,27 +117,28 @@
     if states.size == 0:
         warnings.warn("No valid state estimate computed in solve_gnss_ekf, "\
                     + "returning None.", RuntimeWarning)
         return None
 
     state_estimate = NavData()
     state_estimate["gps_millis"] = states[:,0]
-    state_estimate["x_rx_m"] = states[:,1]
-    state_estimate["y_rx_m"] = states[:,2]
-    state_estimate["z_rx_m"] = states[:,3]
-    state_estimate["vx_rx_mps"] = states[:,4]
-    state_estimate["vy_rx_mps"] = states[:,5]
-    state_estimate["vz_rx_mps"] = states[:,6]
-    state_estimate["b_rx_m"] = states[:,7]
-
-    lat,lon,alt = ecef_to_geodetic(state_estimate[["x_rx_m","y_rx_m",
-                                   "z_rx_m"]].reshape(3,-1))
-    state_estimate["lat_rx_deg"] = lat
-    state_estimate["lon_rx_deg"] = lon
-    state_estimate["alt_rx_deg"] = alt
+    state_estimate["x_rx_ekf_m"] = states[:,1]
+    state_estimate["y_rx_ekf_m"] = states[:,2]
+    state_estimate["z_rx_ekf_m"] = states[:,3]
+    state_estimate["vx_rx_ekf_mps"] = states[:,4]
+    state_estimate["vy_rx_ekf_mps"] = states[:,5]
+    state_estimate["vz_rx_ekf_mps"] = states[:,6]
+    state_estimate["b_rx_ekf_m"] = states[:,7]
+
+    lat,lon,alt = ecef_to_geodetic(state_estimate[["x_rx_ekf_m",
+                                                   "y_rx_ekf_m",
+                                                   "z_rx_ekf_m"]].reshape(3,-1))
+    state_estimate["lat_rx_ekf_deg"] = lat
+    state_estimate["lon_rx_ekf_deg"] = lon
+    state_estimate["alt_rx_ekf_deg"] = alt
 
     return state_estimate
 
 class GNSSEKF(BaseExtendedKalmanFilter):
     """GNSS-only EKF implementation.
 
     States: 3D position, 3D velocity and clock bias (in m).
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/algorithms/residuals.py` & `gnss_lib_py-0.1.9/gnss_lib_py/algorithms/residuals.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ----------
     measurements : gnss_lib_py.parsers.navdata.NavData
         Instance of the NavData class
     receiver_state : gnss_lib_py.parsers.navdata.NavData
         Either estimated or ground truth receiver position in ECEF frame
         in meters and the estimated or ground truth receiver clock bias
         also in meters as an instance of the NavData class with the
-        following rows: x_*_m, y_*_m, z_*_m, b_*_m.
+        following rows: x_rx*_m, y_rx*_m, z_rx*_m, b_rx*_m.
     inplace : bool
         If False, will return new NavData instance with gps_millis and
         reisuals. If True, will add a "residuals_m" rows in the
         current NavData instance.
 
     Returns
     -------
@@ -35,58 +35,45 @@
 
     """
 
     # verify corrected pseudoranges exist in inputs
     measurements.in_rows(["gps_millis","corr_pr_m"])
     receiver_state.in_rows(["gps_millis"])
 
-    # check for receiver_state indexes
-    rx_idxs = {"x_*_m" : [],
-               "y_*_m" : [],
-               "z_*_m" : [],
-               "b_*_m" : [],
-               }
-    for name, indexes in rx_idxs.items():
-        indexes = [row for row in receiver_state.rows
-                      if row.startswith(name.split("*",maxsplit=1)[0])
-                       and row.endswith(name.split("*",maxsplit=1)[1])]
-        if len(indexes) > 1:
-            raise KeyError("Multiple possible row indexes for " \
-                         + name \
-                         + ". Unable to resolve for solve_wls.")
-        if len(indexes) == 0:
-            raise KeyError("Missing required " + name + " row for " \
-                        + "solve_wls.")
-        # must call dictionary to avoid pass by value
-        rx_idxs[name] = indexes[0]
+
+    rx_idxs = receiver_state.find_wildcard_indexes(["x_rx*_m",
+                                                    "y_rx*_m",
+                                                    "z_rx*_m",
+                                                    "b_rx*_m"],
+                                                    max_allow=1)
 
     residuals = []
     for timestamp, _, measurement_subset in measurements.loop_time("gps_millis"):
 
         pos_sv_m = measurement_subset[["x_sv_m","y_sv_m","z_sv_m"]].T
         pos_sv_m = np.atleast_2d(pos_sv_m)
 
         num_svs = pos_sv_m.shape[0]
 
         corr_pr_m = measurement_subset["corr_pr_m"].reshape(-1,1)
 
         # find time index for receiver_state NavData instance
         rx_t_idx = np.argmin(np.abs(receiver_state["gps_millis"] - timestamp))
 
-        rx_pos = receiver_state[[rx_idxs["x_*_m"],
-                                 rx_idxs["y_*_m"],
-                                 rx_idxs["z_*_m"]],
+        rx_pos = receiver_state[[rx_idxs["x_rx*_m"][0],
+                                 rx_idxs["y_rx*_m"][0],
+                                 rx_idxs["z_rx*_m"][0]],
                                  rx_t_idx].reshape(1,-1)
         pos_rx_m = np.tile(rx_pos, (num_svs, 1))
 
         # assumes the use of corrected pseudoranges with the satellite
         # clock bias already removed
         gt_pr_m = np.linalg.norm(pos_rx_m - pos_sv_m, axis = 1,
                                  keepdims = True) \
-                + receiver_state[rx_idxs["b_*_m"],rx_t_idx]
+                + receiver_state[rx_idxs["b_rx*_m"][0],rx_t_idx]
 
         # calculate residual
         residuals_epoch = corr_pr_m - gt_pr_m
         residuals += residuals_epoch.reshape(-1).tolist()
 
     if inplace:
         # add measurements to measurement class
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/algorithms/snapshot.py` & `gnss_lib_py-0.1.9/gnss_lib_py/algorithms/snapshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,67 +2,96 @@
 
 This module contains point solution methods for estimating position
 at a single GNSS measurement epoch. Position is solved using the
 Weighted Least Squares algorithm.
 
 """
 
-__authors__ = "D. Knowles, Shubh Gupta, Bradley Collicott"
+__authors__ = "D. Knowles, A. Kanhere, Shubh Gupta, Bradley Collicott"
 __date__ = "25 Jan 2022"
 
 import warnings
 
 import numpy as np
 
 from gnss_lib_py.parsers.navdata import NavData
 from gnss_lib_py.utils.coordinates import ecef_to_geodetic
 
-def solve_wls(measurements, weight_type = None,
-              only_bias = False, tol = 1e-7, max_count = 20):
+def solve_wls(measurements, weight_type = None, only_bias = False,
+              receiver_state=None, tol = 1e-7, max_count = 20,
+              delta_t_decimals=-2):
     """Runs weighted least squares across each timestep.
 
     Runs weighted least squares across each timestep and adds a new
     row for the receiver's position and clock bias.
 
     The option for only_bias allows the user to only calculate the clock
     bias if the receiver position is already known. Only the bias term
     in rx_est_m will be updated if only_bias is set to True.
 
+    If only_bias is set to True, then the receiver position must also
+    be passed in as the receiver_state
+
+    receiver_state : gnss_lib_py.parsers.navdata.NavData
+        Either estimated or ground truth receiver position in ECEF frame
+        in meters as an instance of the NavData class with the
+        following rows: ``x_rx*_m``, `y_rx*_m``, ``z_rx*_m``,
+        ``gps_millis``.
+
     Parameters
     ----------
     measurements : gnss_lib_py.parsers.navdata.NavData
         Instance of the NavData class
     weight_type : string
         Must either be None or the name of a row in measurements
     only_bias : bool
         If True, then only the receiver clock bias is estimated.
         Otherwise, both position and clock bias are estimated.
+    receiver_state : gnss_lib_py.parsers.navdata.NavData
+        Only used if only_bias is set to True, see description above.
+        Receiver position in ECEF frame in meters as an instance of the
+        NavData class with at least the following rows: ``x_rx*_m``,
+        ``y_rx*_m``, ``z_rx*_m``, ``gps_millis``.
     tol : float
         Tolerance used for the convergence check.
     max_count : int
         Number of maximum iterations before process is aborted and
         solution returned.
+    delta_t_decimals : int
+            Decimal places after which times are considered equal.
 
     Returns
     -------
     state_estimate : gnss_lib_py.parsers.navdata.NavData
         Estimated receiver position in ECEF frame in meters and the
         estimated receiver clock bias also in meters as an instance of
         the NavData class with shape (4 x # unique timesteps) and
-        the following rows: x_rx_m, y_rx_m, z_rx_m, b_rx_m.
+        the following rows: gps_millis, x_rx_wls_m, y_rx_wls_m,
+        z_rx_wls_m, b_rx_wls_m, lat_rx_wls_deg, lon_rx_wls_deg,
+        alt_rx_wls_deg.
 
     """
 
     # check that all necessary rows exist
     measurements.in_rows(["x_sv_m","y_sv_m","z_sv_m","gps_millis"])
 
+    if only_bias:
+        if receiver_state is None:
+            raise RuntimeError("receiver_state needed in WLS " \
+                    + "for only_bias.")
+
+        rx_rows_to_find = ['x_rx*_m', 'y_rx*_m', 'z_rx*_m']
+        rx_idxs = receiver_state.find_wildcard_indexes(
+                                               rx_rows_to_find,
+                                               max_allow=1)
     states = []
+    runtime_error_idxs = {}
 
     position = np.zeros((4,1))
-    for timestamp, _, measurement_subset in measurements.loop_time("gps_millis"):
+    for timestamp, _, measurement_subset in measurements.loop_time("gps_millis", delta_t_decimals=delta_t_decimals):
 
         pos_sv_m = measurement_subset[["x_sv_m","y_sv_m","z_sv_m"]].T
         pos_sv_m = np.atleast_2d(pos_sv_m)
 
         corr_pr_m = measurement_subset["corr_pr_m"].reshape(-1,1)
 
         # remove NaN indexes
@@ -76,42 +105,56 @@
             else:
                 raise TypeError("WLS weights must be None or row"\
                                 +" in NavData")
         else:
             weights = None
 
         try:
+            if only_bias:
+                position = np.vstack((
+                                  receiver_state.where("gps_millis",
+                                  timestamp)[[rx_idxs["x_rx*_m"][0],
+                                              rx_idxs["y_rx*_m"][0],
+                                              rx_idxs["z_rx*_m"][0]]
+                                              ,0].reshape(-1,1),
+                                             position[3])) # clock bias
             position = wls(position, pos_sv_m, corr_pr_m, weights,
                            only_bias, tol, max_count)
             states.append([timestamp] + np.squeeze(position).tolist())
         except RuntimeError as error:
-            warnings.warn("RuntimeError encountered at gps_millis: " \
-                        + str(int(timestamp)) + " RuntimeError: " \
-                        + str(error), RuntimeWarning)
+            if str(error) not in runtime_error_idxs:
+                runtime_error_idxs[str(error)] = [str(int(timestamp))]
+            else:
+                runtime_error_idxs[str(error)].append(str(int(timestamp)))
             states.append([timestamp, np.nan, np.nan, np.nan, np.nan])
 
     states = np.array(states)
 
     state_estimate = NavData()
     state_estimate["gps_millis"] = states[:,0]
-    state_estimate["x_rx_m"] = states[:,1]
-    state_estimate["y_rx_m"] = states[:,2]
-    state_estimate["z_rx_m"] = states[:,3]
-    state_estimate["b_rx_m"] = states[:,4]
+    state_estimate["x_rx_wls_m"] = states[:,1]
+    state_estimate["y_rx_wls_m"] = states[:,2]
+    state_estimate["z_rx_wls_m"] = states[:,3]
+    state_estimate["b_rx_wls_m"] = states[:,4]
+
+    for error,timestamps in runtime_error_idxs.items():
+        warnings.warn(error + " Encountered at " + str(len(timestamps))\
+                    + " gps_millis of: " \
+                + ", ".join(timestamps), RuntimeWarning)
 
     if np.isnan(states[:,1:]).all():
         warnings.warn("No valid state estimate computed in WLS, "\
                     + "returning NaNs.", RuntimeWarning)
         return state_estimate
 
-    lat,lon,alt = ecef_to_geodetic(state_estimate[["x_rx_m","y_rx_m",
-                                   "z_rx_m"]].reshape(3,-1))
-    state_estimate["lat_rx_deg"] = lat
-    state_estimate["lon_rx_deg"] = lon
-    state_estimate["alt_rx_deg"] = alt
+    lat,lon,alt = ecef_to_geodetic(state_estimate[["x_rx_wls_m","y_rx_wls_m",
+                                   "z_rx_wls_m"]].reshape(3,-1))
+    state_estimate["lat_rx_wls_deg"] = lat
+    state_estimate["lon_rx_wls_deg"] = lon
+    state_estimate["alt_rx_wls_deg"] = alt
 
     return state_estimate
 
 def wls(rx_est_m, pos_sv_m, corr_pr_m, weights = None,
         only_bias = False, tol = 1e-7, max_count = 20):
     """Weighted least squares solver for GNSS measurements.
 
@@ -154,15 +197,15 @@
 
     """
 
     rx_est_m = rx_est_m.copy() # don't change referenced value
 
     count = 0
     num_svs = pos_sv_m.shape[0]
-    if num_svs < 4:
+    if num_svs < 4 and not only_bias:
         raise RuntimeError("Need at least four satellites for WLS.")
     pos_x_delta = np.inf*np.ones((4,1))
 
     # load weights
     if weights is None:
         weight_matrix = np.eye(num_svs)
     elif isinstance(weights, np.ndarray):
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/parsers/android.py` & `gnss_lib_py-0.1.9/gnss_lib_py/parsers/android.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import csv
 import warnings
 
 import numpy as np
 import pandas as pd
 
 from gnss_lib_py.parsers.navdata import NavData
+from gnss_lib_py.utils.coordinates import wrap_0_to_2pi
 from gnss_lib_py.utils.coordinates import geodetic_to_ecef
 from gnss_lib_py.utils.coordinates import ecef_to_geodetic
 from gnss_lib_py.utils.time_conversions import unix_to_gps_millis
 from gnss_lib_py.utils.time_conversions import gps_to_unix_millis
 
 class AndroidDerived2021(NavData):
     """Class handling derived measurements from Android dataset.
@@ -267,36 +268,42 @@
 
         Notes
         -----
         Corrections incorporated from Kaggle notes hosted here:
         https://www.kaggle.com/code/gymf123/tips-notes-from-the-competition-hosts
         """
         # Correcting reported altitude
-        self['alt_gt_m'] = self['alt_gt_m'] - 61.
-        gt_lla = np.transpose(np.vstack([self['lat_gt_deg'],
-                                         self['lon_gt_deg'],
-                                         self['alt_gt_m']]))
+        self['alt_rx_gt_m'] = self['alt_rx_gt_m'] - 61.
+        gt_lla = np.transpose(np.vstack([self['lat_rx_gt_deg'],
+                                         self['lon_rx_gt_deg'],
+                                         self['alt_rx_gt_m']]))
         gt_ecef = geodetic_to_ecef(gt_lla)
-        self["x_gt_m"] = gt_ecef[:,0]
-        self["y_gt_m"] = gt_ecef[:,1]
-        self["z_gt_m"] = gt_ecef[:,2]
+        self["x_rx_gt_m"] = gt_ecef[:,0]
+        self["y_rx_gt_m"] = gt_ecef[:,1]
+        self["z_rx_gt_m"] = gt_ecef[:,2]
+
+        # convert bearing degrees to heading in radians
+        self["heading_rx_gt_rad"] = np.deg2rad(self["heading_rx_gt_rad"])
+        self["heading_rx_gt_rad"] = wrap_0_to_2pi(self["heading_rx_gt_rad"])
 
     @staticmethod
     def _row_map():
         """Map of row names from loaded ground truth to gnss_lib_py standard
 
         Returns
         -------
         row_map : Dict
             Dictionary of the form {old_name : new_name}
         """
-        row_map = {'latDeg' : 'lat_gt_deg',
-                   'lngDeg' : 'lon_gt_deg',
-                   'heightAboveWgs84EllipsoidM' : 'alt_gt_m',
-                   'millisSinceGpsEpoch' : 'gps_millis'
+        row_map = {'latDeg' : 'lat_rx_gt_deg',
+                   'lngDeg' : 'lon_rx_gt_deg',
+                   'heightAboveWgs84EllipsoidM' : 'alt_rx_gt_m',
+                   'millisSinceGpsEpoch' : 'gps_millis',
+                   'speedMps' : 'v_rx_gt_mps',
+                   'courseDegree' : 'heading_rx_gt_rad',
                 }
         return row_map
 
 
 class AndroidGroundTruth2022(AndroidGroundTruth2021):
     """Class handling ground truth from Android dataset.
 
@@ -305,41 +312,48 @@
 
     def postprocess(self):
         """Android derived specific postprocessing for NavData()
 
         Notes
         -----
         """
-        if np.any(np.isnan(self['alt_gt_m'])):
+        if np.any(np.isnan(self['alt_rx_gt_m'])):
             warnings.warn("Some altitude values were missing, using 0m ", RuntimeWarning)
-            self['alt_gt_m'] = np.nan_to_num(self['alt_gt_m'])
-        gt_lla = np.transpose(np.vstack([self['lat_gt_deg'],
-                                         self['lon_gt_deg'],
-                                         self['alt_gt_m']]))
+            self['alt_rx_gt_m'] = np.nan_to_num(self['alt_rx_gt_m'])
+        gt_lla = np.transpose(np.vstack([self['lat_rx_gt_deg'],
+                                         self['lon_rx_gt_deg'],
+                                         self['alt_rx_gt_m']]))
         gt_ecef = geodetic_to_ecef(gt_lla)
-        self["x_gt_m"] = gt_ecef[:,0]
-        self["y_gt_m"] = gt_ecef[:,1]
-        self["z_gt_m"] = gt_ecef[:,2]
+        self["x_rx_gt_m"] = gt_ecef[:,0]
+        self["y_rx_gt_m"] = gt_ecef[:,1]
+        self["z_rx_gt_m"] = gt_ecef[:,2]
 
         # add gps milliseconds
         self["gps_millis"] = unix_to_gps_millis(self['unix_millis'])
 
+        # convert bearing degrees to heading in radians
+        self["heading_rx_gt_rad"] = np.deg2rad(self["heading_rx_gt_rad"])
+        self["heading_rx_gt_rad"] = wrap_0_to_2pi(self["heading_rx_gt_rad"])
+
     @staticmethod
     def _row_map():
         """Map row names from loaded data to gnss_lib_py standard
 
         Returns
         -------
         row_map : Dict
             Dictionary of the form {old_name : new_name}
         """
-        row_map = {'LatitudeDegrees' : 'lat_gt_deg',
-                   'LongitudeDegrees' : 'lon_gt_deg',
-                   'AltitudeMeters' : 'alt_gt_m',
-                   'UnixTimeMillis' : 'unix_millis'
+        row_map = {'LatitudeDegrees' : 'lat_rx_gt_deg',
+                   'LongitudeDegrees' : 'lon_rx_gt_deg',
+                   'AltitudeMeters' : 'alt_rx_gt_m',
+                   'SpeedMps' : 'v_rx_gt_mps',
+                   'BearingDegrees' : 'heading_rx_gt_rad',
+                   'UnixTimeMillis' : 'unix_millis',
+
                 }
         return row_map
 
 class AndroidRawImu(NavData):
     """Class handling IMU measurements from raw Android dataset.
 
     Inherits from NavData().
@@ -537,42 +551,42 @@
     """Converts from gnss_lib_py receiver state to Kaggle submission.
 
     Parameters
     ----------
     state_estimate : gnss_lib_py.parsers.navdata.NavData
         Estimated receiver position in latitude and longitude as an
         instance of the NavData class with the following
-        rows: ``gps_millis``, ``lat_*_deg``, ``lon_*_deg``.
+        rows: ``gps_millis``, ``lat_rx*_deg``, ``lon_rx*_deg``.
     trip_id : string
         Value for the tripId column in kaggle submission which is a
         fusion of the data and phone type.
 
     Returns
     -------
     output : gnss_lib_py.parsers.navdata.NavData
         NavData structure ready for Kaggle submission.
 
     """
 
     state_estimate.in_rows("gps_millis")
-    wildcards = state_estimate.find_wildcard_indexes(["lat_*_deg",
-                            "lon_*_deg"],max_allow = 1)
+    wildcards = state_estimate.find_wildcard_indexes(["lat_rx*_deg",
+                            "lon_rx*_deg"],max_allow = 1)
 
     output = NavData()
     output["tripId"] = np.array([trip_id] * state_estimate.shape[1])
     output["UnixTimeMillis"] = gps_to_unix_millis(state_estimate["gps_millis"])
     output.orig_dtypes["UnixTimeMillis"] = np.int64
-    output["LatitudeDegrees"] = state_estimate[wildcards["lat_*_deg"]]
-    output["LongitudeDegrees"] = state_estimate[wildcards["lon_*_deg"]]
+    output["LatitudeDegrees"] = state_estimate[wildcards["lat_rx*_deg"]]
+    output["LongitudeDegrees"] = state_estimate[wildcards["lon_rx*_deg"]]
 
     output.interpolate("UnixTimeMillis",["LatitudeDegrees",
                                          "LongitudeDegrees"],inplace=True)
     return output
 
-def solve_kaggle_dataset(folder_path, solver, verbose=False, *args):
+def solve_kaggle_dataset(folder_path, solver, verbose=False, *args, **kwargs):
     """Run solver on all kaggle traces.
 
     Additional ``*args`` arguments are passed into the ``solver``
     function.
 
     Parameters
     ----------
@@ -610,15 +624,15 @@
                 # convert data to Measurement class
                 derived_data = AndroidDerived2022(data_path)
 
                 if verbose:
                     print("solving:",trace_name,phone_type)
 
                 # compute state estimate using provided solver function
-                state_estimate = solver(derived_data, *args)
+                state_estimate = solver(derived_data, *args, **kwargs)
 
                 trip_id = "/".join([trace_name,phone_type])
                 output = prepare_kaggle_submission(state_estimate,
                                                    trip_id)
 
                 # concatenate solution to previous solutions
                 solution.concat(navdata=output, inplace=True)
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/parsers/ephemeris.py` & `gnss_lib_py-0.1.9/gnss_lib_py/parsers/ephemeris.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 """Functions to download, save and process satellite ephemeris files.
 
+The Ephemeris Manager provides broadcast ephemeris for specific
+satellites at a specific timestep. The EphemerisManager class should be
+initialized and then the ``get_ephemeris`` function can be used to
+retrieve ephemeris for specific satellites. ``get_ephemeris`` returns
+the most recent broadcast ephemeris for the provided list of satellites
+that was broadcast BEFORE the provided timestamp. For example GPS daily
+ephemeris files contain data at a two hour frequency, so if the
+timestamp provided is 5am, then ``get_ephemeris`` will return the 4am
+data but not 6am. If provided a timestamp between midnight and 2am then
+the ephemeris from around midnight (might be the day before) will be
+provided. If no list of satellites is provided, then ``get_ephemeris``
+will return data for all satellites.
+
+When multiple observations are provided for the same satellite and same
+timestep, the Ephemeris Manager will only return the first instance.
+This is applicable when requesting ephemeris for multi-GNSS for the
+current day. Same-day multi GNSS data is pulled from  same day. For
+same-day multi-GNSS from https://igs.org/data/ which often has multiple
+observations.
+
 """
 
 __authors__ = "Shubh Gupta, Ashwin Kanhere"
 __date__ = "13 July 2021"
 
 import os
 import shutil
 import gzip
 import ftplib
 from ftplib import FTP_TLS, FTP
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timezone
 
 import unlzw3
 import georinex
 import numpy as np
 import pandas as pd
 
 import gnss_lib_py.utils.constants as consts
+from gnss_lib_py.parsers.navdata import NavData
+from gnss_lib_py.utils.time_conversions import datetime_to_gps_millis, tzinfo_to_utc
 
 
 class EphemerisManager():
     """Download, store and process ephemeris files
 
     Attributes
     ----------
     data_directory : string
         Directory to store/read ephemeris files
     data : pd.Dataframe
         Ephemeris parameters
     leapseconds : int
         Leap seconds to add to UTC time to get GPS time
+    verbose : bool
+        If true, prints debugging statements.
 
     Notes
     -----
     Class code taken from https://github.com/johnsonmitchelld/gnss-analysis/blob/main/gnssutils/ephemeris_manager.py
 
     The associated license is copied below:
 
@@ -65,101 +89,189 @@
     DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
     SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
     CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
     OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
     """
-    def __init__(self, data_directory=os.path.join(os.getcwd(), 'data', 'ephemeris')):
+    def __init__(self, data_directory=os.path.join(os.getcwd(), 'data', 'ephemeris'),
+                 verbose=False):
         self.data_directory = data_directory
         nasa_dir = os.path.join(data_directory, 'nasa')
         igs_dir = os.path.join(data_directory, 'igs')
         os.makedirs(nasa_dir, exist_ok=True)
         os.makedirs(igs_dir, exist_ok=True)
         self.data = None
         self.leapseconds = None
+        self.verbose = verbose
+
+    def get_ephemeris(self, timestamp, satellites=None):
+        """Return ephemeris DataFrame for satellites input.
 
-    def get_ephemeris(self, timestamp, satellites):
-        """Return ephemeris DataFrame for satellites input
+        The Ephemeris Manager provides broadcast ephemeris for specific
+        satellites at a specific timestep. The EphemerisManager class
+        should be initialized and then the ``get_ephemeris`` function
+        can be used to retrieve ephemeris for specific satellites.
+        ``get_ephemeris`` returns the most recent broadcast ephemeris
+        for the provided list of satellites that was broadcast BEFORE
+        the provided timestamp. For example GPS daily ephemeris files
+        contain data at a two hour frequency, so if the timestamp
+        provided is 5am, then ``get_ephemeris`` will return the 4am data
+        but not 6am. If provided a timestamp between midnight and 2am
+        then the ephemeris from around midnight (might be the day
+        before) will be provided. If no list of satellites is provided,
+        then ``get_ephemeris`` will return data for all satellites.
+
+        When multiple observations are provided for the same satellite
+        and same timestep, the Ephemeris Manager will only return the
+        first instance. This is applicable when requesting ephemeris for
+        multi-GNSS for the current day. Same-day multi GNSS data is
+        pulled from  same day. For same-day multi-GNSS from
+        https://igs.org/data/ which often has multiple observations.
 
         Parameters
         ----------
         timestamp : datetime.datetime
-            Time of clock
+            Ephemeris data is returned for the timestamp day and
+            includes all broadcast ephemeris whose broadcast timestamps
+            happen before the given timestamp variable. Timezone should
+            be added manually and is interpreted as UTC if not added.
         satellites : List
-            List of satellites ['Const_IDSVID']
+            List of satellite IDs as a string, for example ['G01','E11',
+            'R06']. Defaults to None which returns get_ephemeris for
+            all satellites.
 
         Returns
         -------
-        data : pd.DataFrame
-            DataFrame containing ephemeris entries corresponding to timestamp
+        data : gnss_lib_py.parsers.navdata.NavData
+            ephemeris entries corresponding to timestamp
+
+        Notes
+        -----
+        The Galileo week ``GALWeek`` is identical to the GPS Week
+        ``GPSWeek``. See http://acc.igs.org/misc/rinex304.pdf page A26
 
         """
         systems = EphemerisManager.get_constellations(satellites)
+        # add UTC timezone if datatime os offset-naive
+        timestamp = tzinfo_to_utc(timestamp)
         if not isinstance(self.data, pd.DataFrame):
-            self.load_data(timestamp, systems)
+            same_day = (datetime.now(timezone.utc) - timestamp).days <= 0
+            self.load_data(timestamp, systems, same_day)
         data = self.data
-        if satellites:
+        if satellites is not None:
             data = data.loc[data['sv'].isin(satellites)]
-        data = data.loc[data['time'] < timestamp]
-        data = data.sort_values('time').groupby(
+        time_cropped_data = data.loc[data['time'] < timestamp]
+        time_cropped_data = time_cropped_data.sort_values('time').groupby(
             'sv').last().drop(labels = 'index', axis = 'columns')
+        if satellites is not None and len(time_cropped_data) < len(satellites):
+            # if no data available for the given day, try looking at the
+            # previous day, may occur when a time near to midnight
+            # is provided. For example, 12:01am
+            if len(time_cropped_data) != 0:
+                satellites = list(set(satellites) - set(time_cropped_data.index))
+            systems = EphemerisManager.get_constellations(satellites)
+            prev_day_timestamp = datetime(year=timestamp.year,
+                                          month=timestamp.month,
+                                          day=timestamp.day - 1,
+                                          hour=23,
+                                          minute=59,
+                                          second=59,
+                                          microsecond=999999,
+                                          tzinfo=timezone.utc,
+                                          )
+            self.load_data(prev_day_timestamp, systems, False)
+            prev_data = self.data
+            if satellites is not None:
+                prev_data = prev_data.loc[prev_data['sv'].isin(satellites)]
+            prev_data = prev_data.sort_values('time').groupby(
+                'sv').last().drop(labels = 'index', axis = 'columns')
+            data = pd.concat((time_cropped_data,prev_data))
+        else:
+            data = time_cropped_data
         data['Leap Seconds'] = self.leapseconds
-        return data
-
-    def get_leapseconds(self, timestamp):
-        """Output saved leapseconds
-
-        Returns
-        -------
-        lp_seconds : float
-            Leap seconds between GPS and UTC time
-        """
-        lp_seconds = self.leapseconds
-        return lp_seconds
+        # Convert data DataFrame to NavData instance
+        # Move sv to DataFrame columns, reset index
+        data = data.reset_index()
+        # Replace datetime with gps_millis
+        gps_millis = [datetime_to_gps_millis(df_row['time']) \
+                        for _, df_row in data.iterrows()]
+        data['gps_millis'] = gps_millis
+        data = data.drop(columns=['time'])
+        data = data.rename(columns={"sv":"sv_id"})
+        if "GPSWeek" in data.columns:
+            data = data.rename(columns={"GPSWeek":"gps_week"})
+            if "GALWeek" in data.columns:
+                data["gps_week"] = np.where(pd.isnull(data["gps_week"]),
+                                                      data["GALWeek"],
+                                                      data["gps_week"])
+        elif "GALWeek" in data.columns:
+            data = data.rename(columns={"GALWeek":"gps_week"})
+        if len(data) == 0:
+            raise RuntimeError("No ephemeris data available for the " \
+                             + "given satellites")
+        data_navdata = NavData(pandas_df=data)
+        data_navdata['gnss_sv_id'] = data_navdata['sv_id']
+        gnss_chars = [sv_id[0] for sv_id in np.atleast_1d(data_navdata['sv_id'])]
+        gnss_nums = [sv_id[1:] for sv_id in np.atleast_1d(data_navdata['sv_id'])]
+        gnss_id = [consts.CONSTELLATION_CHARS[gnss_char] for gnss_char in gnss_chars]
+        data_navdata['gnss_id'] = np.asarray(gnss_id)
+        data_navdata['sv_id'] = np.asarray(gnss_nums, dtype=int)
+        return data_navdata
 
-    def load_data(self, timestamp, constellations=None):
+    def load_data(self, timestamp, constellations=None, same_day=False):
         """Load ephemeris into class instance
 
         Parameters
         ----------
-
         timestamp : datetime.datetime
-            Time of clock
-
+            Ephemeris data is returned for the timestamp day and
+            includes all broadcast ephemeris whose broadcast timestamps
+            happen before the given timestamp variable. Timezone should
+            be added manually and is interpreted as UTC if not added.
         constellations : Set
-            Set of satellites {"ConstIDSVID"}
+            Set of satellites For example, set({"G","R","E"}).
+        same_day : bool
+            Whether or not ephemeris is for same-day aquisition.
 
         """
         filepaths = EphemerisManager.get_filepaths(timestamp)
         data_list = []
-        timestamp_age = datetime.now(timezone.utc) - timestamp
+
         if constellations == None:
             for fileinfo in filepaths.values():
-                data = self.get_ephemeris_dataframe(fileinfo)
+                data = self.get_ephemeris_dataframe(fileinfo,
+                                                    constellations)
                 data_list.append(data)
         else:
             legacy_systems = set(['G', 'R'])
             legacy_systems_only = len(constellations - legacy_systems) == 0
-            if timestamp_age.days > 0:
+            if not same_day:
                 if legacy_systems_only:
-                    data_list.append(self.get_ephemeris_dataframe(
-                        filepaths['nasa_daily_gps']))
+                    if 'G' in constellations:
+                        data_list.append(self.get_ephemeris_dataframe(
+                            filepaths['nasa_daily_gps'],
+                            constellations=None))
                     if 'R' in constellations:
                         data_list.append(self.get_ephemeris_dataframe(
-                            filepaths['nasa_daily_glonass']))
+                            filepaths['nasa_daily_glonass'],
+                            constellations=None))
                 else:
                     data_list.append(self.get_ephemeris_dataframe(
-                        filepaths['nasa_daily_combined']))
+                        filepaths['nasa_daily_combined'],
+                        constellations))
             else:
-                data_list.append(self.get_ephemeris_dataframe(
-                    filepaths['nasa_daily_gps']))
-                if not legacy_systems_only:
+                if legacy_systems_only and 'G' in constellations:
+                    data_list.append(self.get_ephemeris_dataframe(
+                        filepaths['nasa_daily_gps'],
+                        constellations=None))
+                else:
                     data_list.append(self.get_ephemeris_dataframe(
-                        filepaths['bkg_daily_combined']))
+                        filepaths['bkg_daily_combined'],
+                        constellations))
 
         data = pd.DataFrame()
         for new_data in data_list:
             data = pd.concat((data,new_data), ignore_index=True)
 
         data.reset_index(inplace=True)
         data.sort_values('time', inplace=True, ignore_index=True)
@@ -181,49 +293,44 @@
         data : pd.DataFrame
             Parsed ephemeris DataFrame
         """
         filepath = fileinfo['filepath']
         url = fileinfo['url']
         directory = os.path.split(filepath)[0]
         filename = os.path.split(filepath)[1]
-        if url == 'igs.bkg.bund.de':
+        if url == 'igs-ftp.bkg.bund.de':
             dest_filepath = os.path.join(self.data_directory, 'igs', filename)
         else:
             dest_filepath = os.path.join(self.data_directory, 'nasa', filename)
         decompressed_filename = os.path.splitext(dest_filepath)[0]
-        if not os.path.isfile(decompressed_filename):
-            if url == 'gdc.cddis.eosdis.nasa.gov':
-                secure = True
-            else:
-                secure = False
-            try:
-                self.retrieve_file(url, directory, filename,
-                                   dest_filepath, secure)
-                self.decompress_file(dest_filepath)
-            except ftplib.error_perm as err:
-                print('ftp error')
-                return pd.DataFrame()
+        if not os.path.isfile(decompressed_filename): # pragma: no cover
+            self.retrieve_file(url, directory, filename,
+                               dest_filepath)
         if not self.leapseconds:
             self.leapseconds = EphemerisManager.load_leapseconds(
                 decompressed_filename)
-        if constellations:
+        if constellations is not None:
             data = georinex.load(decompressed_filename,
-                                 use=constellations).to_dataframe()
+                                 use=constellations,
+                                 verbose=self.verbose).to_dataframe()
         else:
-            data = georinex.load(decompressed_filename).to_dataframe()
+            data = georinex.load(decompressed_filename,
+                                 verbose=self.verbose).to_dataframe()
         data.dropna(how='all', inplace=True)
         data.reset_index(inplace=True)
         data['source'] = decompressed_filename
         data['t_oc'] = pd.to_numeric(data['time'] - datetime(1980, 1, 6, 0, 0, 0))
+        #TODO: Use a constant for the time of GPS clock start
         data['t_oc']  = 1e-9 * data['t_oc'] - consts.WEEKSEC * np.floor(1e-9 * data['t_oc'] / consts.WEEKSEC)
         data['time'] = data['time'].dt.tz_localize('UTC')
         data.rename(columns={'M0': 'M_0', 'Eccentricity': 'e', 'Toe': 't_oe', 'DeltaN': 'deltaN', 'Cuc': 'C_uc', 'Cus': 'C_us',
                              'Cic': 'C_ic', 'Crc': 'C_rc', 'Cis': 'C_is', 'Crs': 'C_rs', 'Io': 'i_0', 'Omega0': 'Omega_0'}, inplace=True)
         return data
 
+
     @staticmethod
     def get_filetype(timestamp):
         """Get file extension of IGS file based on timestamp
 
         Parameters
         ----------
         timestamp : datetime.datetime
@@ -260,45 +367,42 @@
             for line in f:
                 if 'LEAP SECONDS' in line:
                     read_lp_sec = int(line.split()[0])
                     return read_lp_sec
                 if 'END OF HEADER' in line:
                     return None
 
+        return None
+
     @staticmethod
     def get_constellations(satellites):
         """Convert list of satellites to set
 
         Parameters
         ----------
         satellites : List
             List of satellites of form [ConstIDSVID]
 
         Returns
         -------
         systems : Set or None
             Set representation of satellites for which ephemeris is needed
         """
-        if type(satellites) is list:
+        if isinstance(satellites, list):
             systems = set()
             for sat in satellites:
                 systems.add(sat[0])
             return systems
-        else:
-            return None
 
-    @staticmethod
-    def calculate_toc(timestamp):
-        """I think this is equivalent of datetime_to_tow()
-        #TODO: See if this function is needed or can be deleted
-        """
-        pass
+        return None
+
+    def retrieve_file(self, url, directory, filename, dest_filepath):
+        """Copy ephemeris file from FTP filepath to local directory.
 
-    def retrieve_file(self, url, directory, filename, dest_filepath, secure=False):
-        """Copy ephemeris file from FTP filepath to local directory
+        Also decompresses file.
 
         Parameters
         ----------
         url : String
             FTP server location
 
         directory : String
@@ -306,30 +410,35 @@
 
         filename : String
             Filename in which ephemeris files are stored (both locally and globally)
 
         dest_filepath : String
             Directory where downloaded ephemeris files are stored locally
 
-        secure : Bool
-            Whether to make secure FTP connection
-
         """
-        print('Retrieving ' + directory + '/' + filename + ' from ' + url)
+
+        secure = bool(url == 'gdc.cddis.eosdis.nasa.gov')
+
+        if self.verbose:
+            print('Retrieving ' + directory + '/' + filename + ' from ' + url)
         ftp = self.connect(url, secure)
         src_filepath = directory + '/' + filename
         try:
             with open(dest_filepath, 'wb') as handle:
                 ftp.retrbinary(
                     'RETR ' + src_filepath, handle.write)
         except ftplib.error_perm as err:
-            print('Failed to retrieve ' + src_filepath + ' from ' + url)
-            print(err)
             os.remove(dest_filepath)
-            raise ftplib.error_perm
+            raise ftplib.error_perm(str(err) + ' Failed to retrieve ' \
+                                  + src_filepath + ' from ' + url)
+
+        ftp.quit()
+        if ftp is not None: # try closing if still active
+            ftp.close()
+        self.decompress_file(dest_filepath)
 
     def decompress_file(self, filepath):
         """Decompress downloaded file ephemeris file in same destination location
 
         Parameters
         ----------
         filepath : String
@@ -369,31 +478,14 @@
             ftp.login()
             ftp.prot_p()
         else:
             ftp = FTP(url)
             ftp.login()
         return ftp
 
-    def listdir(self, url, directory, secure):
-        """Display files on server that match input filename
-
-        Parameters
-        ----------
-        url : String
-            URL of FTP server
-
-        directory : String
-            Directory in FTP server where relevant ephemeris files are stored
-        """
-        # TODO: Function not called anywhere, consider folding into existing function calls or deleting
-        ftp = self.connect(url, secure)
-        dirlist = ftp.nlst(directory)
-        dirlist = [x for x in dirlist]
-        print(dirlist)
-
     @staticmethod
     def get_filepaths(timestamp):
         """Generate filepaths for all ephemeris files
 
         Parameters
         ----------
         timestamp : datetime.datetime
@@ -428,16 +520,10 @@
         directory = '/IGS/BRDC/' + \
             str(timetuple.tm_year) + '/' + \
             str(timetuple.tm_yday).zfill(3) + '/'
         filename = 'BRDC00WRD_S_' + \
             str(timetuple.tm_year) + \
             str(timetuple.tm_yday).zfill(3) + '0000_01D_MN.rnx.gz'
         filepaths['bkg_daily_combined'] = {
-            'filepath': directory + filename, 'url': 'igs.bkg.bund.de'}
+            'filepath': directory + filename, 'url': 'igs-ftp.bkg.bund.de'}
 
         return filepaths
-
-
-if __name__ == '__main__':
-    repo = EphemerisManager()
-    target_time = datetime(2021, 1, 9, 12, 0, 0, tzinfo=timezone.utc)
-    data = repo.get_ephemeris(target_time, ['G01', 'G03'])
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/parsers/navdata.py` & `gnss_lib_py-0.1.9/gnss_lib_py/parsers/navdata.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,24 +35,29 @@
         Additional arguments (e.g. ``sep`` or ``header``) passed into
         ``pd.read_csv`` if csv_path is not None.
 
     Attributes
     ----------
     arr_dtype : numpy.dtype
         Type of values stored in data array
+    orig_dtypes : pandas.core.series.Series
+        Type of each original column if reading from a csv or Pandas
+        dataframe.
     array : np.ndarray
         Array containing data, dimension M x N
     map : Dict
         Map of the form {pandas column name : array row number }
     str_map : Dict
         Map of the form {pandas column name : {array value : string}}.
         Map is of the form {pandas column name : {}} for non string rows.
-    orig_dtypes : pandas.core.series.Series
-        Type of each original column if reading from a csv or Pandas
-        dataframe.
+    num_cols : int
+        Number of columns in array containing data, set to 0 by default
+        for empty NavData
+    curr_cols : int
+        Current number of column for iterator, set to 0 by default
 
     """
     def __init__(self, csv_path=None, pandas_df=None, numpy_array=None,
                  **kwargs):
         # For a Pythonic implementation,
         # including all attributes as None in the beginning
         self.arr_dtype = np.float64 # default value
@@ -226,15 +231,15 @@
                                           if row not in self.rows]
 
             for row in combined_rows:
                 combined_row = np.array([])
                 # combine data from existing and new instance
                 for data in [self, navdata]:
                     if row in data.rows:
-                        new_row = data[row]
+                        new_row = np.atleast_1d(data[row])
                     elif len(data) == 0:
                         continue
                     else:
                         # add np.nan for missing values
                         new_row = np.empty((len(data),))
                         new_row.fill(np.nan)
                     combined_row = np.concatenate((combined_row,
@@ -256,97 +261,150 @@
                 self.orig_dtypes = new_navdata.orig_dtypes.copy()
 
         if inplace:
             return None
         return new_navdata
 
     def where(self, key_idx, value, condition="eq"):
-        """Return NavData where conditions are met for the given row
+        """Return NavData where conditions are met for the given row.
+
+        For string rows, only the "eq" and "neq" conditions are valid.
+        The "value" argument can contain either a string, np.nan or an
+        array-like object of strings. If an array-like object of strings
+        is passed in then np.isin() is used to check the condition
+        meaning that the returned subset will contain one of the values
+        in the "value" array-like object for the "eq" condition or none
+        of the values in the "value" array-like object for the "neq"
+        condition.
+
+        For non-string rows, all valid conditions are listed in the
+        "condition" argument description. The "value" argument can either
+        contain a numeric or an array-like object of numerics for both
+        the "eq" and "neq" conditions.
+        If an array-like object is passed then the returned subset will
+        contain one of the values in the "value" array-like object for
+        the "eq" condition or none of the values in the "value"
+        array-like object for the "neq" condition.
+        For the "between" condition, the two limit values must be passed
+        into the "value" argument as an array-like object.
 
         Parameters
         ----------
         key_idx : string/int
             Key or index of the row in which conditions will be checked
-        value : float/list
-            Number (or list of two numbers for ) to compare array values
-            against
+        value : float/int/str/array-like
+            Value that the row is checked against, array-like object
+            possible for "eq", "neq", or "between" conditions.
         condition : string
             Condition type (greater than ("greater")/ less than ("lesser")/
             equal to ("eq")/ greater than or equal to ("geq")/
             lesser than or equal to ("leq") / in between ("between")
-            inclusive of the provided limits
+            inclusive of the provided limits / not equal to ("neq"))
 
         Returns
         -------
         new_navdata : gnss_lib_py.parsers.navdata.NavData
             NavData with columns where given condition is satisfied
             for specified row
         """
         new_cols = self.argwhere(key_idx, value, condition)
         if new_cols.size == 0:
             return self.remove(cols=list(range(len(self))))
         new_navdata = self.copy(cols=new_cols)
         return new_navdata
 
     def argwhere(self, key_idx, value, condition="eq"):
-        """Return columns where conditions are met for the given row
+        """Return columns where conditions are met for the given row.
+
+        For string rows, only the "eq" and "neq" conditions are valid.
+        The "value" argument can contain either a string, np.nan or an
+        array-like object of strings. If an array-like object of strings
+        is passed in then np.isin() is used to check the condition
+        meaning that the returned subset will contain one of the values
+        in the "value" array-like object for the "eq" condition or none
+        of the values in the "value" array-like object for the "neq"
+        condition.
+
+        For non-string rows, all valid conditions are listed in the
+        "condition" argument description. The "value" argument can either
+        contain a numeric or an array-like object of numerics for both
+        the "eq" and "neq" conditions.
+        If an array-like object is passed then the returned subset will
+        contain one of the values in the "value" array-like object for
+        the "eq" condition or none of the values in the "value"
+        array-like object for the "neq" condition.
+        For the "between" condition, the two limit values must be passed
+        into the "value" argument as an array-like object.
 
         Parameters
         ----------
         key_idx : string/int
             Key or index of the row in which conditions will be checked
-        value : float/list
-            Number (or list of two numbers for ) to compare array values against
+        value : float/int/str/array-like
+            Value that the row is checked against, array-like object
+            possible for "eq", "neq", or "between" conditions.
         condition : string
             Condition type (greater than ("greater")/ less than ("lesser")/
             equal to ("eq")/ greater than or equal to ("geq")/
-            lesser than or equal to ("leq") / in between ("between"))
+            lesser than or equal to ("leq") / in between ("between")
+            inclusive of the provided limits / not equal to ("neq"))
 
         Returns
         -------
         new_cols : list
             Columns in NavData where given condition is satisfied
             for specified row
         """
         rows, _ = self._parse_key_idx(key_idx)
-        inv_map = self.inv_map
         row_list, row_str = self._get_str_rows(rows)
         if len(row_list)>1:
             error_msg = "where does not currently support multiple rows"
             raise NotImplementedError(error_msg)
         row = row_list[0]
         row_str = row_str[0]
-        new_cols = None
+        new_cols = np.array([])
         if row_str:
             # Values in row are strings
             if condition not in ("eq","neq"):
-                raise ValueError("Inequality comparison not valid for strings")
-            key = inv_map[row]
-            for str_key, str_value in self.str_map[key].items():
-                if str_value==str(value):
-                    if condition == "eq":
-                        new_cols = np.argwhere(self.array[row, :]==str_key)
-                        break
-                    # condition == "neq"
-                    new_cols = np.argwhere(self.array[row, :]!=str_key)
-                    break
-            if new_cols is None:
-                new_cols = np.array([])
+                raise ValueError("Unsupported where condition for strings")
+            if isinstance(value,str):
+                str_check = [str(value)]
+            elif isinstance(value,(np.ndarray,list,tuple,set)):
+                str_check = [str(v) for v in value]
+            elif np.isnan(value):
+                str_check = [str(np.nan)]
+            else:
+                raise ValueError("Value must be string or array-like " \
+                               + "for string condition checks")
             # Extract columns where condition holds true and return new NavData
+            if condition == "eq":
+                new_cols = np.argwhere(np.isin(self[row, :],str_check))
+            else:
+                # condition == "neq"
+                new_cols = np.argwhere(~np.isin(self[row, :],str_check))
+
         else:
             # Values in row are numerical
             # Find columns where value can be found and return new NavData
             if condition=="eq":
-                if not isinstance(value,str) and np.isnan(value):
+                if isinstance(value,(np.ndarray,list,tuple,set)):
+                    # use numpy's isin() condition if list of values
+                    new_cols = np.argwhere(np.isin(self.array[row, :],
+                                           value))
+                elif not isinstance(value,str) and np.isnan(value):
                     # check isinstance b/c np.isnan can't handle strings
                     new_cols = np.argwhere(np.isnan(self.array[row, :]))
                 else:
                     new_cols = np.argwhere(self.array[row, :]==value)
             elif condition=="neq":
-                if not isinstance(value,str) and np.isnan(value):
+                if isinstance(value,(np.ndarray,list,tuple,set)):
+                    # use numpy's isin() condition if list of values
+                    new_cols = np.argwhere(~np.isin(self.array[row, :],
+                                           value))
+                elif not isinstance(value,str) and np.isnan(value):
                     # check isinstance b/c np.isnan can't handle strings
                     new_cols = np.argwhere(~np.isnan(self.array[row, :]))
                 else:
                     new_cols = np.argwhere(self.array[row, :]!=value)
             elif condition == "leq":
                 new_cols = np.argwhere(self.array[row, :]<=value)
             elif condition == "geq":
@@ -360,22 +418,67 @@
                 new_cols = np.argwhere(np.logical_and(self.array[row, :]>=value[0],
                                         self.array[row, :]<= value[1]))
             else:
                 raise ValueError("Condition not implemented")
         new_cols = np.squeeze(new_cols)
         return new_cols
 
-    def loop_time(self, time_row, tol_decimals=2):
+    def sort(self, order=None, ind=None, ascending=True,
+             inplace=False):
+        """Sort values along given row or using given index
+
+        Parameters
+        ----------
+        order : string/int
+            Key or index of the row on which NavData will be sorted
+        ind : list/np.ndarray
+            Ordering of indices to be used for sorting
+        ascending : bool
+            If true, sorts "ascending", otherwise sorts "descending"
+        inplace : bool
+            If False, will return new NavData instance with rows
+            sorted. If True, will sorted data rows in the
+            current NavData instance.
+
+        Returns
+        -------
+        new_navdata : gnss_lib_py.parsers.navdata.NavData or None
+            If inplace is False, returns NavData instance after renaming
+            specified rows. If inplace is True, returns
+            None.
+
+        """
+        if ind is None:
+            assert order is not None, \
+            "Provide 'order' arg as row on which NavData is sorted"
+            if ascending:
+                ind = np.argsort(self[order])
+            else:
+                ind = np.argsort(-self[order])
+
+        if not inplace:
+            new_navdata = self.copy()   # create copy to return
+        for row_idx in range(self.shape[0]):
+            if inplace:
+                self.array[row_idx,:] = self.array[row_idx,ind]
+            else:
+                new_navdata.array[row_idx,:] = new_navdata.array[row_idx,ind]
+
+        if inplace:
+            return None
+        return new_navdata
+
+    def loop_time(self, time_row, delta_t_decimals=2):
         """Generator object to loop over columns from same times.
 
         Parameters
         ----------
         time_row : string/int
             Key or index of the row in which times are stored.
-        tol_decimals : int
+        delta_t_decimals : int
             Decimal places after which times are considered equal.
 
         Yields
         ------
         timestamp : float
             Current timestamp.
         delta_t : float
@@ -383,24 +486,28 @@
         new_navdata : gnss_lib_py.parsers.navdata.NavData
             NavData with same time, up to given decimal tolerance.
 
         """
 
         times = self[time_row]
         times_unique = np.sort(np.unique(np.around(times,
-                                         decimals=tol_decimals)))
+                                         decimals=delta_t_decimals)))
         for time_idx, time in enumerate(times_unique):
             if time_idx==0:
                 delta_t = 0
             else:
                 delta_t = time-times_unique[time_idx-1]
-            new_navdata = self.where(time_row, [time-10**(-tol_decimals),
-                                                time+10**(-tol_decimals)],
+            new_navdata = self.where(time_row, [time-10**(-delta_t_decimals),
+                                                time+10**(-delta_t_decimals)],
                                                 condition="between")
-            yield time, delta_t, new_navdata
+            if len(np.unique(new_navdata[time_row]))==1:
+                frame_time = new_navdata[time_row, 0]
+            else:
+                frame_time = time
+            yield frame_time, delta_t, new_navdata
 
     def is_str(self, row_name):
         """Check whether a row contained string values.
 
         Parameters
         ----------
         row_name : string
@@ -733,33 +840,46 @@
             raise KeyError("input to in_rows must be a single row " \
                          + "index or list/np.ndarray/tuple of indexes")
 
         if len(missing_rows) > 0:
             raise KeyError(", ".join(missing_rows) + " row(s) are" \
                            + " missing from NavData object.")
 
-    def find_wildcard_indexes(self, wildcards, max_allow = None):
+    def find_wildcard_indexes(self, wildcards, max_allow = None,
+                              excludes = None):
         """Searches for indexes matching wildcard search input.
 
         For example, a search for ``x_*_m`` would find ``x_rx_m`` or
         ``x_sv_m`` or ``x_alpha_beta_gamma_m`` depending on the rows
         existing in the NavData instance.
 
+        The ``excludes`` variable allows you to exclude indexes when
+        trying to match a wildcard. For example, if there are rows named
+        ``pr_raw_m``and ``pr_raw_sigma_m`` then the input
+        ``wildcards="pr_*_m", excludes=None`` would return
+        ``{"pr_*_m", ["pr_raw_m","pr_raw_sigma_m"]}`` but with the excludes
+        parameter set, the input ``wildcards="pr_*_m", excludes="pr_*_sigma_m"``
+        would only return ``{"pr_*_m", ["pr_raw_m"]}``
+
         Will return an error no index is found matching the wildcard or
         if more than ``max_allow`` indexes are found.
 
-        Currently only allows for a single wildcard per index.
+        Currently only allows for a single wildcard '*' per index.
 
         Parameters
         ----------
         wildcards : array-like or str
             List/tuple/np.ndarray/set of indexes for which to search.
         max_allow : int or None
             Maximum number of valid indexes to allow before throwing an
             error. If None, then no limit is placed.
+        excludes : array-like or str
+            List or string to exclude for each wildcard in wildcards.
+            Must be the same length as wildcards. Allowed to include a
+            wildcard '*' character but not necessary.
 
         Returns
         -------
         wildcard_indexes : dict
             Dictionary of the form {"search_term", [indexes,...]},
 
         """
@@ -768,26 +888,54 @@
             wildcards = [wildcards]
         if not isinstance(wildcards, (list,tuple,np.ndarray,set)):
             raise TypeError("wildcards input in find_wildcard_indexes" \
                          +  " must be array-like or single string")
         if not (isinstance(max_allow,int) or max_allow is None):
             raise TypeError("max_allow input in find_wildcard_indexes" \
                           + " must be an integer or None.")
+        # handle exclude types
+        if isinstance(excludes,str):
+            excludes = [excludes]
+        if excludes is None:
+            excludes = [None] * len(wildcards)
+        if not isinstance(excludes, (list,tuple,np.ndarray,set)):
+            raise TypeError("excludes input in find_wildcard_indexes" \
+                         +  " must be array-like, single string, " \
+                         + "or None for each wildcard")
+        if len(excludes) != len(wildcards):
+            raise TypeError("excludes input must match length of " \
+                          + "wildcard input.")
+        for ex_idx, exclude in enumerate(excludes):
+            if exclude is None or isinstance(exclude,str):
+                excludes[ex_idx] = [exclude]
+            if not isinstance(excludes[ex_idx], (list,tuple,np.ndarray,set)):
+                raise TypeError("excludes input in find_wildcard_indexes" \
+                             +  " must be array-like, single string, " \
+                             + "or None for each wildcard")
 
         wildcard_indexes = {}
 
-        for wildcard in wildcards:
+        for wild_idx, wildcard in enumerate(wildcards):
             if not isinstance(wildcard,str):
                 raise TypeError("wildcards must be strings")
             if wildcard.count("*") != 1:
                 raise RuntimeError("One wildcard '*' and only one "\
                           + "wildcard must be present in search string")
             indexes = [row for row in self.rows
                    if row.startswith(wildcard.split("*",maxsplit=1)[0])
                     and row.endswith(wildcard.split("*",maxsplit=1)[1])]
+            if excludes[wild_idx] is not None:
+                for exclude in excludes[wild_idx]:
+                    if exclude is not None:
+                        if '*' in exclude:
+                            indexes = [row for row in indexes
+                                     if not (row.startswith(exclude.split("*",maxsplit=1)[0])
+                                     and row.endswith(exclude.split("*",maxsplit=1)[1]))]
+                        else:
+                            indexes = [row for row in indexes if exclude != row]
             if max_allow is not None and len(indexes) > max_allow:
                 raise KeyError("More than " + str(max_allow) \
                              + " possible row indexes for "  + wildcard)
             if len(indexes) == 0:
                 raise KeyError("Missing " + wildcard + " row.")
 
             wildcard_indexes[wildcard] = indexes
@@ -1047,23 +1195,46 @@
         if self.curr_col >= self.num_cols:
             raise StopIteration
         x_curr = self.copy(rows=None, cols=self.curr_col)
         self.curr_col += 1
         return x_curr
 
     def __str__(self):
+        """Creates string representation of NavData object
+
+        Returns
+        -------
+        str_out : str
+            String representation of Navdata object, based on equivalent
+            Pandas string
+        """
         str_out = str(self.pandas_df())
         str_out = str_out.replace("DataFrame","NavData")
         str_out = str_out.replace("Columns","Rows")
         # swap rows and columns when printing for NavData consistency
         str_out = re.sub(r"(.*)\[(\d+)\srows\sx\s(\d+)\scolumns\](.*)",
                          r'\g<1>[\g<3> rows x \g<2> columns]\g<4>',
                          str_out)
         return str_out
 
+    def __repr__(self):  # pragma: no cover
+        """Evaluated string representation of Navdata object
+
+        For NavData objects, this is similar to the str method and is
+        defined separately to avoid having to add a `print` method
+        before each display command in Jupyter notebooks
+
+        Returns
+        -------
+        rep_out : str
+            Evaluated string representation object
+        """
+        rep_out = str(self)
+        return rep_out
+
     def __len__(self):
         """Return length of class
 
         Returns
         -------
         length : int
             Number of time steps in NavData
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/parsers/precise_ephemerides.py` & `gnss_lib_py-0.1.9/gnss_lib_py/parsers/precise_ephemerides.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from gnss_lib_py.utils.time_conversions import datetime_to_gps_millis
 import gnss_lib_py.utils.constants as consts
 
 # Define the number of sats to create arrays for
 NUMSATS = {'gps': (32, 'G'),
            'galileo': (36, 'E'),
            'beidou': (46, 'C'),
-           'glonass': (24, 'R'),
+           'glonass': (26, 'R'), # 26 total GLONASS satellites in orbit
            'qzss': (3, 'J')}
 
 class Sp3:
     """Class handling satellite position data from precise ephemerides
 
     """
     def __init__(self):
@@ -497,40 +497,48 @@
     clk_iref_old = -1 * np.ones( (len(clk_parsed_file),))
     satfunc_t_old = np.empty( (len(clk_parsed_file),), dtype=object)
     satfunc_t_old[:] = np.nan
 
     # Compute satellite information for desired time steps
     unique_timesteps = np.unique(navdata["gps_millis"])
 
+    # add satellite indexes if not present already.
+    sv_idx_keys = ['x_sv_m', 'y_sv_m', 'z_sv_m', \
+                'vx_sv_mps','vy_sv_mps','vz_sv_mps', \
+                'b_sv_m', 'b_dot_sv_mps']
+    for sv_idx_key in sv_idx_keys:
+        if sv_idx_key not in navdata.rows:
+            navdata[sv_idx_key] = np.nan
+
     for t_idx, timestep in enumerate(unique_timesteps):
 
         # Compute indices where gps_millis match, sort them
         # sorting is done for consistency across all satellite pos. estimation
         # algorithms as ephemerismanager inherently sorts based on prns
         idxs = np.where(navdata["gps_millis"] == timestep)[0]
         sorted_idxs = idxs[np.argsort(navdata["sv_id", idxs], axis = 0)]
 
         if verbose:
             print(t_idx, timestep, idxs, sorted_idxs)
             print('misc: ', navdata['gps_millis', sorted_idxs], \
                             navdata['gnss_id', sorted_idxs], \
                             navdata['sv_id', sorted_idxs], \
-                            navdata['signal_type', sorted_idxs])
+                            )
 
-        # this if else condition can be removed later after navdata has been
-        # fixed to represent one data point as an array as well
-        if len(sorted_idxs)==1:
-            visible_sats = np.array([navdata["sv_id", sorted_idxs]])
-        else:
-            visible_sats = navdata["sv_id", sorted_idxs]
+        visible_sats = np.atleast_1d(navdata["sv_id", sorted_idxs])
 
         for sv_idx, prn in enumerate(visible_sats):
 
             prn = int(prn)
 
+            # continue if no sp3 or clk data availble
+            if len(sp3_parsed_file[prn].tym) == 0 \
+                or len(clk_parsed_file[prn].tym) == 0:
+                continue
+
             # Perform nearest time step search to compute iref values for sp3 and clk
             sp3_iref = np.argmin(abs(np.array(sp3_parsed_file[prn].tym) - \
                                      (timestep - navdata_offset) ))
             clk_iref = np.argmin(abs(np.array(clk_parsed_file[prn].tym) - \
                                      (timestep - navdata_offset) ))
 
             if verbose:
@@ -609,82 +617,58 @@
                           navdata["vz_sv_mps", sorted_idxs[sv_idx]] - satvel_sp3[2] )
 
                 print('Android-sp3 Clk Error (m): ', \
                           navdata["b_sv_m", sorted_idxs[sv_idx]] - consts.C * satbias_clk, \
                           navdata["b_dot_sv_mps", sorted_idxs[sv_idx]] - consts.C * satdrift_clk)
                 print(' ')
 
-            # update x_sv_m of navdata with the estimated values from .sp3 files
+            # update *_sv_m of navdata with the estimated values from .sp3 files
             navdata['x_sv_m', sorted_idxs[sv_idx]] = np.array([satpos_sp3[0]])
-            if not (navdata["x_sv_m", sorted_idxs[sv_idx]] - satpos_sp3[0] == 0.0):
-                raise RuntimeError("x_sv_m of navdata not correctly updated")
-
-            # update y_sv_m of navdata with the estimated values from .sp3 files
             navdata['y_sv_m', sorted_idxs[sv_idx]] = np.array([satpos_sp3[1]])
-            if not (navdata["y_sv_m", sorted_idxs[sv_idx]] - satpos_sp3[1] == 0.0):
-                raise RuntimeError("y_sv_m of navdata not correctly updated")
-
-            # update z_sv_m of navdata with the estimated values from .sp3 files
             navdata['z_sv_m', sorted_idxs[sv_idx]] = np.array([satpos_sp3[2]])
-            if not (navdata["z_sv_m", sorted_idxs[sv_idx]] - satpos_sp3[2] == 0.0):
-                raise RuntimeError("z_sv_m of navdata not correctly updated")
 
-            # update vx_sv_mps of navdata with the estimated values from .sp3 files
+            # update v*_sv_mps of navdata with the estimated values from .sp3 files
             navdata["vx_sv_mps", sorted_idxs[sv_idx]] = np.array([satvel_sp3[0]])
-            if not (navdata["vx_sv_mps", sorted_idxs[sv_idx]] - satvel_sp3[0] == 0.0):
-                raise RuntimeError("vx_sv_mps of navdata not correctly updated")
-
-            # update vy_sv_mps of navdata with the estimated values from .sp3 files
             navdata["vy_sv_mps", sorted_idxs[sv_idx]] = np.array([satvel_sp3[1]])
-            if not (navdata["vy_sv_mps", sorted_idxs[sv_idx]] - satvel_sp3[1] == 0.0):
-                raise RuntimeError("vy_sv_mps of navdata not correctly updated")
-
-            # update vz_sv_mps of navdata with the estimated values from .sp3 files
             navdata["vz_sv_mps", sorted_idxs[sv_idx]] = np.array([satvel_sp3[2]])
-            if not (navdata["vz_sv_mps", sorted_idxs[sv_idx]] - satvel_sp3[2] == 0.0):
-                raise RuntimeError("vz_sv_mps of navdata not correctly updated")
 
-            # update b_sv_m of navdata with the estimated values from .clk files
+            # update clock data of navdata with the estimated values from .clk files
             navdata["b_sv_m", sorted_idxs[sv_idx]] = np.array([consts.C * satbias_clk])
-            if not (navdata["b_sv_m", sorted_idxs[sv_idx]] - consts.C * satbias_clk == 0.0):
-                raise RuntimeError("b_sv_m of navdata not correctly updated")
-
-            # update b_dot_sv_mps of navdata with the estimated values from .clk files
             navdata["b_dot_sv_mps", sorted_idxs[sv_idx]] = np.array([consts.C * satdrift_clk])
-            if not (navdata["b_dot_sv_mps", sorted_idxs[sv_idx]] - \
-                                            consts.C * satdrift_clk == 0.0):
-                raise RuntimeError("b_dot_sv_mps of navdata not correctly updated")
 
     return navdata
 
 def multi_gnss_from_precise_eph(navdata, sp3_path, clk_path, \
-                                        gnss_consts, verbose = False):
+                                        constellations, verbose = False):
     """Compute satellite information using .sp3 and .clk for multiple GNSS
 
     Parameters
     ----------
     navdata : gnss_lib_py.parsers.navdata.NavData
         Instance of the NavData class that depicts android derived dataset
-    sp3_parsed_file : list
-        Instance with list of gnss_lib_py.parsers.precise_ephemerides.Sp3
-    clk_parsed_file : list
-        Instance with array of gnss_lib_py.parsers.precise_ephemerides.Clk
+    sp3_path : path
+        File path for .sp3 file to extract precise ephemerides
+    clk_path : path
+        File path for .clk file to extract precise ephemerides
+    constellations : array-like
+        The GNSS constellations for which you want to extract precise
+        ephemeris, (e.g. ['gps','glonass'])
     verbose : bool
         Flag (True/False) for whether to print intermediate steps useful
         for debugging/reviewing (the default is False)
 
     Returns
     -------
     navdata : gnss_lib_py.parsers.navdata.NavData
         Updated NavData class with satellite information computed using
         precise ephemerides from .sp3 and .clk files
     """
 
     navdata_prcs_merged = NavData()
-    for sv in gnss_consts:
+    for sv in constellations:
         navdata_prcs_gnss = navdata.where('gnss_id', sv)
 
         sp3_parsed_gnss = parse_sp3(sp3_path, constellation = sv)
         clk_parsed_gnss = parse_clockfile(clk_path, constellation = sv)
         derived_prcs_gnss = single_gnss_from_precise_eph(navdata_prcs_gnss, \
                                                                  sp3_parsed_gnss, \
                                                                  clk_parsed_gnss, \
@@ -739,73 +723,52 @@
         ephem = repo.get_ephemeris(rxdatetime, satellites = desired_sats)
 
         if verbose:
             print(t_idx, timestep, idxs, sorted_idxs)
             print('misc: ', navdata['gps_millis', sorted_idxs], \
                             navdata['gnss_id', sorted_idxs], \
                             navdata['sv_id', sorted_idxs], \
-                            navdata['signal_type', sorted_idxs], \
                             desired_sats, rxdatetime)
 
             satpos_android = np.transpose([ navdata["x_sv_m", sorted_idxs], \
                                             navdata["y_sv_m", sorted_idxs], \
                                             navdata["z_sv_m", sorted_idxs] ])
             satvel_android = np.transpose([ navdata["vx_sv_mps", sorted_idxs], \
                                                navdata["vy_sv_mps", sorted_idxs], \
                                                navdata["vz_sv_mps", sorted_idxs] ])
             print('android:', satpos_android, satvel_android)
 
         # compute satellite position and velocity based on ephem and gps_time
         # Transform satellite position to account for earth's rotation
         gps_week, gps_tow = gps_millis_to_tow(timestep - navdata_offset)
         get_sat_from_ephem = find_sat(ephem, gps_tow, gps_week)
-        satpos_ephemeris = np.transpose([get_sat_from_ephem.x.values, \
-                                         get_sat_from_ephem.y.values, \
-                                         get_sat_from_ephem.z.values])
-        satvel_ephemeris = np.transpose([get_sat_from_ephem.vx.values, \
-                                         get_sat_from_ephem.vy.values, \
-                                         get_sat_from_ephem.vz.values])
+        satpos_ephemeris = np.transpose([get_sat_from_ephem["x_sv_m"], \
+                                         get_sat_from_ephem["y_sv_m"], \
+                                         get_sat_from_ephem["z_sv_m"]])
+        satvel_ephemeris = np.transpose([get_sat_from_ephem["vx_sv_mps"], \
+                                         get_sat_from_ephem["vy_sv_mps"], \
+                                         get_sat_from_ephem["vz_sv_mps"]])
         trans_time = navdata["raw_pr_m", sorted_idxs] / consts.C
         del_x = (consts.OMEGA_E_DOT * satpos_ephemeris[:,1] * trans_time)
         del_y = (-consts.OMEGA_E_DOT * satpos_ephemeris[:,0] * trans_time)
         satpos_ephemeris[:,0] = satpos_ephemeris[:,0] + del_x
         satpos_ephemeris[:,1] = satpos_ephemeris[:,1] + del_y
 
         if verbose:
             print('after ephemeris:', satpos_ephemeris, satvel_ephemeris)
             print('nav-android Pos Error: ', \
                       np.linalg.norm(satpos_ephemeris - satpos_android, axis=1) )
             print('nav-android Vel Error: ', \
                       np.linalg.norm(satvel_ephemeris - satvel_android, axis=1) )
             print(' ')
 
-        # update x_sv_m of navdata with the estimated values from .n files
+        # update *_sv_m of navdata with the estimated values from .n files
         navdata["x_sv_m", sorted_idxs] = satpos_ephemeris[:,0]
-        if not max(abs(navdata["x_sv_m", sorted_idxs] - satpos_ephemeris[:,0])) == 0.0:
-            raise RuntimeError("x_sv_m of navdata not correctly updated")
-
-        # update y_sv_m of navdata with the estimated values from .n files
         navdata["y_sv_m", sorted_idxs] = satpos_ephemeris[:,1]
-        if not max(abs(navdata["y_sv_m", sorted_idxs] - satpos_ephemeris[:,1])) == 0.0:
-            raise RuntimeError("y_sv_m of navdata not correctly updated")
-
-        # update z_sv_m of navdata with the estimated values from .n files
         navdata["z_sv_m", sorted_idxs] = satpos_ephemeris[:,2]
-        if not max(abs(navdata["z_sv_m", sorted_idxs] - satpos_ephemeris[:,2])) == 0.0:
-            raise RuntimeError("z_sv_m of navdata not correctly updated")
 
-        # update vx_sv_mps of navdata with the estimated values from .n files
+        # update v*_sv_mps of navdata with the estimated values from .n files
         navdata["vx_sv_mps", sorted_idxs] = satvel_ephemeris[:,0]
-        if not max(abs(navdata["vx_sv_mps", sorted_idxs] - satvel_ephemeris[:,0])) == 0.0:
-            raise RuntimeError("vx_sv_mps of navdata not correctly updated")
-
-        # update vy_sv_mps of navdata with the estimated values from .n files
         navdata["vy_sv_mps", sorted_idxs] = satvel_ephemeris[:,1]
-        if not max(abs(navdata["vy_sv_mps", sorted_idxs] - satvel_ephemeris[:,1])) == 0.0:
-            raise RuntimeError("vy_sv_mps of navdata not correctly updated")
-
-        # update vz_sv_mps of navdata with the estimated values from .n files
         navdata["vz_sv_mps", sorted_idxs] = satvel_ephemeris[:,2]
-        if not max(abs(navdata["vz_sv_mps", sorted_idxs] - satvel_ephemeris[:,2])) == 0.0:
-            raise RuntimeError("vz_sv_mps of navdata not correctly updated")
 
     return navdata
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/utils/constants.py` & `gnss_lib_py-0.1.9/gnss_lib_py/utils/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 
 Based on the UIUC ECE 456 implementation [1]_.
 
 References
 ----------
 .. [1] Makela, Jonathan, ECE 456, Global Nav Satellite Systems,
    Fall 2017. University of Illinois Urbana-Champaign. Coding Assignments.
+.. [2] International GNSS Service (IGS), RINEX Working Group and Radio
+   Technical Commission for Maritime Servies Special Committee. RINEX
+   Version 3.04. http://acc.igs.org/misc/rinex304.pdf
 
 """
 
 __authors__ = "Ashwin Kanhere"
 __date__ = "13 July 2021"
 
-from numpy import sqrt
 from datetime import datetime, timezone
+from numpy import sqrt
+
 
 A = 6378137.
 """float : Semi-major axis (radius) of the Earth [m]."""
 
 B = 6356752.3145
 """float : Semi-minor axis (radius) of the Earth [m]."""
 
@@ -60,7 +64,26 @@
 """float : Acceleration due to gravity ENU frame of reference [m/s]."""
 
 WEEKSEC = 604800
 """ int : Number of seconds in a week [s]."""
 
 GPS_EPOCH_0 = datetime(1980, 1, 6, 0, 0, 0, 0, tzinfo=timezone.utc)
 """ datetime.datetime: Starting time for GPS epoch"""
+
+TROPO_DELAY_C1 = 2.47
+"""float : First coefficient of simplified tropospheric delay model developed in [1]_."""
+
+TROPO_DELAY_C2 = 0.0121
+"""float : Second coefficient of simplified tropospheric delay model developed in [1]_."""
+
+TROPO_DELAY_C3 = 1.33e-4
+"""float : Third coefficient of simplified tropospheric delay model developed in [1]_."""
+
+CONSTELLATION_CHARS = {'G':'gps',
+                       'R':'glonass',
+                       'S':'sbas',
+                       'C':'beidou',
+                       'E':'galileo',
+                       'J':'qzss',
+                       'I':'irnss',
+                       }
+"""dict : Satellite System identifier from Rinex specification p13 in [2]_."""
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/utils/coordinates.py` & `gnss_lib_py-0.1.9/gnss_lib_py/utils/coordinates.py`

 * *Files 4% similar despite different names*

```diff
@@ -396,80 +396,79 @@
     for multiple satellites at the same time.
 
     Parameters
     ----------
     rx_pos : np.ndarray
         1x3 vector containing ECEF [X, Y, Z] coordinate of receiver
     sv_pos : np.ndarray
-        Nx3 array  containing ECEF [X, Y, Z] coordinates of satellites
+        3xN array  containing ECEF [X, Y, Z] coordinates of satellites
 
     Returns
     -------
     el_az : np.ndarray
-        Nx2 array containing the elevation and azimuth from the
+        2XN array containing the elevation and azimuth from the
         receiver to the requested satellites. Elevation and azimuth are
         given in decimal degrees.
 
     Notes
     -----
     Code based on method by J. Makela.
     AE 456, Global Navigation Sat Systems, University of Illinois
     Urbana-Champaign. Fall 2017
 
     """
 
     # conform receiver position to correct shape
     rx_pos = np.atleast_2d(rx_pos)
-    if rx_pos.shape == (3,1):
+    if rx_pos.shape == (1,3):
         rx_pos = rx_pos.T
-    if rx_pos.shape != (1,3):
+    if rx_pos.shape != (3, 1):
         raise RuntimeError("Receiver ECEF position must be a " \
-                          + "np.ndarray of shape 1x3.")
+                          + "np.ndarray of shape 3x1.")
 
     # conform satellite position to correct shape
     sv_pos = np.atleast_2d(sv_pos)
-    if sv_pos.shape[1] != 3:
+    if sv_pos.shape[0] != 3:
         raise RuntimeError("Satellite ECEF position(s) must be a " \
-                          + "np.ndarray of shape Nx3.")
+                          + "np.ndarray of shape 3xN.")
 
     # Convert the receiver location to WGS84
     rx_lla = ecef_to_geodetic(rx_pos)
 
     # Create variables with the latitude and longitude in radians
-    rx_lat, rx_lon = np.deg2rad(rx_lla[0,:2])
+    rx_lat, rx_lon = np.deg2rad(rx_lla[:2,0])
 
     # Create the 3 x 3 transform matrix from ECEF to VEN
     ecef_to_ven = np.array([[ np.cos(rx_lat)*np.cos(rx_lon),
                               np.cos(rx_lat)*np.sin(rx_lon),
                               np.sin(rx_lat)],
                             [-np.sin(rx_lon),
                               np.cos(rx_lon),
                               0.     ],
                             [-np.sin(rx_lat)*np.cos(rx_lon),
                              -np.sin(rx_lat)*np.sin(rx_lon),
                               np.cos(rx_lat)]])
 
     # Replicate the rx_pos array to be the same size as the satellite array
-    rx_array = np.tile(rx_pos,(len(sv_pos),1))
+    rx_array = np.tile(rx_pos,(1, sv_pos.shape[1]))
 
     # Calculate the normalized pseudorange for each satellite
     pseudorange = (sv_pos - rx_array) / np.linalg.norm(sv_pos - rx_array,
-                                             axis=1, keepdims=True)
+                                             axis=0, keepdims=True)
 
     # Perform the transform of the normalized pseudorange from ECEF to VEN
-    p_ven = np.dot(ecef_to_ven, pseudorange.T)
-
+    p_ven = np.dot(ecef_to_ven, pseudorange)
     # Calculate elevation and azimuth in degrees
-    el_az = np.zeros([sv_pos.shape[0],2])
-    el_az[:,0] = np.rad2deg((np.pi/2. - np.arccos(p_ven[0,:])))
-    el_az[:,1] = np.rad2deg(np.arctan2(p_ven[1,:],p_ven[2,:]))
+    el_az = np.zeros([2, sv_pos.shape[1]])
+    el_az[0,:] = np.rad2deg((np.pi/2. - np.arccos(p_ven[0,:])))
+    el_az[1,:] = np.rad2deg(np.arctan2(p_ven[1,:],p_ven[2,:]))
 
     # wrap from 0 to 360
-    while np.any(el_az[:,1] < 0):
-        el_az[:,1][el_az[:,1] < 0] += 360
+    while np.any(el_az[1, :] < 0):
+        el_az[1, :][el_az[1, :] < 0] += 360
 
     return el_az
 
 def add_el_az(navdata, receiver_state, inplace=False):
     """Adds elevation and azimuth to NavData object.
 
     Parameters
@@ -477,15 +476,16 @@
     navdata : gnss_lib_py.parsers.navdata.NavData
         Instance of the NavData class. Must include ``gps_millis`` as
         well as satellite ECEF positions as ``x_sv_m``, ``y_sv_m``,
         ``z_sv_m``, ``gnss_id`` and ``sv_id``.
     receiver_state : gnss_lib_py.parsers.navdata.NavData
         Either estimated or ground truth receiver position in ECEF frame
         in meters as an instance of the NavData class with the
-        following rows: ``x_*_m``, ``y_*_m``, ``z_*_m``, ``gps_millis``.
+        following rows: ``x_rx*_m``, ``y_rx*_m``, ``z_rx*_m``,
+        ``gps_millis``.
     inplace : bool
         If false (default) will add elevation and azimuth to a new
         NavData instance. If true, will add elevation and azimuth to the
         existing NavData instance.
 
     Returns
     -------
@@ -500,49 +500,70 @@
 
     # check for missing rows
     navdata.in_rows(["gps_millis","x_sv_m","y_sv_m","z_sv_m",
                      "gnss_id","sv_id"])
     receiver_state.in_rows(["gps_millis"])
 
     # check for receiver_state indexes
-    rx_idxs = receiver_state.find_wildcard_indexes(["x_*_m","y_*_m",
-                                                    "z_*_m"],max_allow=1)
+    rx_idxs = receiver_state.find_wildcard_indexes(["x_rx*_m",
+                                                    "y_rx*_m",
+                                                    "z_rx*_m"],max_allow=1)
 
     sv_el_az = None
     for timestamp, _, navdata_subset in navdata.loop_time("gps_millis"):
 
-        pos_sv_m = navdata_subset[["x_sv_m","y_sv_m","z_sv_m"]].T
+        pos_sv_m = navdata_subset[["x_sv_m","y_sv_m","z_sv_m"]]
 
         # find time index for receiver_state NavData instance
         rx_t_idx = np.argmin(np.abs(receiver_state["gps_millis"] - timestamp))
 
-        pos_rx_m = receiver_state[[rx_idxs["x_*_m"][0],
-                                   rx_idxs["y_*_m"][0],
-                                   rx_idxs["z_*_m"][0]],
-                                   rx_t_idx].reshape(1,-1)
+        pos_rx_m = receiver_state[[rx_idxs["x_rx*_m"][0],
+                                   rx_idxs["y_rx*_m"][0],
+                                   rx_idxs["z_rx*_m"][0]],
+                                   rx_t_idx].reshape(-1,1)
 
         timestep_el_az = ecef_to_el_az(pos_rx_m, pos_sv_m)
 
         if sv_el_az is None:
-            sv_el_az = timestep_el_az.T
+            sv_el_az = timestep_el_az
         else:
-            sv_el_az = np.hstack((sv_el_az,timestep_el_az.T))
+            sv_el_az = np.hstack((sv_el_az,timestep_el_az))
 
     if inplace:
         navdata["el_sv_deg"] = sv_el_az[0,:]
         navdata["az_sv_deg"] = sv_el_az[1,:]
         return navdata
 
     data_el_az = NavData()
     data_el_az["gps_millis"] = navdata["gps_millis"]
     data_el_az["gnss_id"] = navdata["gnss_id"]
     data_el_az["sv_id"] = navdata["sv_id"]
     data_el_az["x_sv_m"] = navdata["x_sv_m"]
     data_el_az["y_sv_m"] = navdata["y_sv_m"]
     data_el_az["z_sv_m"] = navdata["z_sv_m"]
-    data_el_az[rx_idxs["x_*_m"][0]] = receiver_state[rx_idxs["x_*_m"][0]]
-    data_el_az[rx_idxs["y_*_m"][0]] = receiver_state[rx_idxs["y_*_m"][0]]
-    data_el_az[rx_idxs["z_*_m"][0]] = receiver_state[rx_idxs["z_*_m"][0]]
+    data_el_az[rx_idxs["x_rx*_m"][0]] = receiver_state[rx_idxs["x_rx*_m"][0]]
+    data_el_az[rx_idxs["y_rx*_m"][0]] = receiver_state[rx_idxs["y_rx*_m"][0]]
+    data_el_az[rx_idxs["z_rx*_m"][0]] = receiver_state[rx_idxs["z_rx*_m"][0]]
     data_el_az["el_sv_deg"] = sv_el_az[0,:]
     data_el_az["az_sv_deg"] = sv_el_az[1,:]
 
     return data_el_az
+
+def wrap_0_to_2pi(angles):
+    """Wraps an arbitrary radian between [0, 2pi).
+
+    Angles must be in radians.
+
+    Parameters
+    ----------
+    angles : np.ndarray
+        Array of angles in radians to wrap between 0 and 2pi.
+
+    Returns
+    -------
+    angles : np.ndarray
+        Angles wrapped between 0 and 2pi in radians.
+
+    """
+    angles = np.mod(angles, 2*np.pi)
+
+    return angles
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/utils/file_operations.py` & `gnss_lib_py-0.1.9/gnss_lib_py/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/utils/filters.py` & `gnss_lib_py-0.1.9/gnss_lib_py/utils/filters.py`

 * *Files identical despite different names*

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/utils/sim_gnss.py` & `gnss_lib_py-0.1.9/gnss_lib_py/utils/sim_gnss.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 __date__ = "16 July 2021"
 
 import numpy as np
 import pandas as pd
 from numpy.random import default_rng
 
 import gnss_lib_py.utils.constants as consts
-from gnss_lib_py.utils.coordinates import ecef_to_geodetic, ecef_to_el_az
+from gnss_lib_py.utils.coordinates import ecef_to_geodetic
+from gnss_lib_py.utils.time_conversions import gps_millis_to_tow
+from gnss_lib_py.parsers.navdata import NavData
 # TODO: Check if any of the functions are sorting the dataframe w.r.t SV while
 # processing the measurements
 
 
 def sats_from_el_az(elaz_deg):
     """Generate NED satellite positions at given elevation and azimuth.
 
@@ -59,17 +61,21 @@
     prns : List
         Satellite PRNs in input DataFrame
     sv_pos : ndarray
         ECEF satellite positions
     sv_vel : ndarray
         ECEF satellite x, y and z velocities
     """
-    prns   = [int(prn[1:]) for prn in sv_posvel.index]
-    sv_pos = sv_posvel.filter(['x', 'y', 'z'])
-    sv_vel   = sv_posvel.filter(['vx', 'vy', 'vz'])
+
+    try:
+        prns   = [int(prn[1:]) for prn in sv_posvel.index]
+    except:
+        prns   = [int(prn) for prn in sv_posvel.index]
+    sv_pos = sv_posvel.filter(['x_sv_m', 'y_sv_m', 'z_sv_m'])
+    sv_vel   = sv_posvel.filter(['vx_sv_mps', 'vy_sv_mps', 'vz_sv_mps'])
     sv_pos = sv_pos.to_numpy()
     sv_vel   = sv_vel.to_numpy()
     return prns, sv_pos, sv_vel
     # TODO: Remove prns from function output if not needed
 
 def simulate_measures(gpsweek, gpstime, ephem, pos, bias, b_dot, vel,
                       prange_sigma = 6., doppler_sigma=0.1, sv_posvel=None):
@@ -219,22 +225,24 @@
     """
 
     # Find positions and velocities of all satellites
     approx_posvel = find_sat(ephem, gpstime - consts.T_TRANS, gpsweek)
 
     # Find elevation and azimuth angles for all satellites
     _, approx_pos, _ = _extract_pos_vel_arr(approx_posvel)
-    approx_el_az = ecef_to_el_az(np.reshape(rx_ecef, [1, 3]), approx_pos)
+    approx_el_az = find_elaz(np.reshape(rx_ecef, [1, 3]), approx_pos)
     # Keep attributes of only those satellites which are visible
     keep_ind = approx_el_az[:,0] > el_mask
     # prns = approx_posvel.index.to_numpy()[keep_ind]
     # TODO: Remove above statement if superfluous
     # TODO: Check that a copy of the ephemeris is being generated, also if it is
     # needed
-    eph = ephem.loc[keep_ind, :]
+    ephem_df = ephem.pandas_df()
+    eph = ephem_df.loc[keep_ind, :]
+    eph = NavData(pandas_df=eph)
     return eph
 
 
 def _find_sv_location(gpsweek, gpstime, ephem, pos, sv_posvel=None):
     """Return satellite positions, difference from rx_pos position and ranges.
 
     Parameters
@@ -259,31 +267,31 @@
         Difference between satellite positions and receiver position
     true_range : ndarray
         Distance between satellite and receiver positions
 
     """
     pos = np.reshape(pos, [1, 3])
     if sv_posvel is None:
-        satellites = len(ephem.index)
+        satellites = len(ephem)
         sv_posvel = find_sat(ephem, gpstime - consts.T_TRANS, gpsweek)
         del_pos, true_range = _find_delxyz_range(sv_posvel, pos, satellites)
         t_corr = true_range/consts.C
 
         # Find satellite locations at (a more accurate) time of transmission
         sv_posvel = find_sat(ephem, gpstime-t_corr, gpsweek)
     else:
         satellites = len(sv_posvel.index)
     del_pos, true_range = _find_delxyz_range(sv_posvel, pos, satellites)
     t_corr = true_range/consts.C
     # Corrections for the rotation of the Earth during transmission
     # _, sv_pos, sv_vel = _extract_pos_vel_arr(sv_posvel)
-    del_x = consts.OMEGA_E_DOT*sv_posvel['x'] * t_corr
-    del_y = consts.OMEGA_E_DOT*sv_posvel['y'] * t_corr
-    sv_posvel['x'] = sv_posvel['x'] + del_x
-    sv_posvel['y'] = sv_posvel['y'] + del_y
+    del_x = consts.OMEGA_E_DOT*sv_posvel['x_sv_m'] * t_corr
+    del_y = consts.OMEGA_E_DOT*sv_posvel['y_sv_m'] * t_corr
+    sv_posvel['x_sv_m'] = sv_posvel['x_sv_m'] + del_x
+    sv_posvel['y_sv_m'] = sv_posvel['y_sv_m'] + del_y
     return sv_posvel, del_pos, true_range
 
 
 
 def _find_delxyz_range(sv_posvel, pos, satellites):
     """Return difference of satellite and rx_pos positions and range between them.
 
@@ -363,24 +371,25 @@
 
     ecc        = ephem['e']     # eccentricity
     omega    = ephem['omega'] # argument of perigee
     omega_0  = ephem['Omega_0']
     sqrt_sma = ephem['sqrtA'] # sqrt of semi-major axis
     sma      = sqrt_sma**2      # semi-major axis
 
+    ephem['GPSWeek'], ephem["tow"] = gps_millis_to_tow(ephem["gps_millis"])
     sqrt_mu_A = np.sqrt(consts.MU_EARTH) * sqrt_sma**-3 # mean angular motion
     gpsweek_diff = (np.mod(gpsweek,1024) - np.mod(ephem['GPSWeek'],1024))*604800.
 
     # if np.size(times_all)==1:
     #     times_all = times_all*np.ones(len(ephem))
     # else:
     #     times_all = np.reshape(times_all, len(ephem))
     # times = times_all
     sv_posvel = pd.DataFrame()
-    sv_posvel.loc[:,'sv'] = ephem.index
+    sv_posvel.loc[:,'sv'] = ephem["sv_id"]
     sv_posvel.set_index('sv', inplace=True)
     #TODO: Check if 'dt' or 'times' should be stored in the final DataFrame
     sv_posvel.loc[:,'times'] = times
 
     dt = times - ephem['t_oe'] + gpsweek_diff
 
     # Calculate the mean anomaly with corrections
@@ -451,35 +460,35 @@
     dyp = dr*np.sin(phi) + r*np.cos(phi)*du
     # Find satellite position in ECEF coordinates
     cos_omega = np.cos(omega)
     sin_omega = np.sin(omega)
     cos_i = np.cos(i)
     sin_i = np.sin(i)
 
-    sv_posvel.loc[:,'x'] = xp*cos_omega - yp*cos_i*sin_omega
-    sv_posvel.loc[:,'y'] = xp*sin_omega + yp*cos_i*cos_omega
-    sv_posvel.loc[:,'z'] = yp*sin_i
+    sv_posvel.loc[:,'x_sv_m'] = xp*cos_omega - yp*cos_i*sin_omega
+    sv_posvel.loc[:,'y_sv_m'] = xp*sin_omega + yp*cos_i*cos_omega
+    sv_posvel.loc[:,'z_sv_m'] = yp*sin_i
     # TODO: Add satellite clock bias here using the 'clock corrections' not to
     # be used but compared against SP3 and Android data
 
     ############################################
     ######  Lines added for velocity (4)  ######
     ############################################
     omega_dot = ephem['OmegaDot'] - consts.OMEGA_E_DOT
-    sv_posvel.loc[:,'vx'] = (dxp * cos_omega
+    sv_posvel.loc[:,'vx_sv_mps'] = (dxp * cos_omega
                          - dyp * cos_i*sin_omega
                          + yp  * sin_omega*sin_i*di
                          - (xp * sin_omega + yp*cos_i*cos_omega)*omega_dot)
 
-    sv_posvel.loc[:,'vy'] = (dxp * sin_omega
+    sv_posvel.loc[:,'vy_sv_mps'] = (dxp * sin_omega
                          + dyp * cos_i * cos_omega
                          - yp  * sin_i * cos_omega * di
                          + (xp * cos_omega - (yp*cos_i*sin_omega)) * omega_dot)
 
-    sv_posvel.loc[:,'vz'] = dyp*sin_i + yp*cos_i*di
+    sv_posvel.loc[:,'vz_sv_mps'] = dyp*sin_i + yp*cos_i*di
     return sv_posvel
 
 
 def correct_pseudorange(gpstime, gpsweek, ephem, pr_meas, rx_ecef=[[None]]):
     """Incorporate corrections in measurements.
 
     Incorporate clock corrections (relativistic, drift), tropospheric and
@@ -618,15 +627,15 @@
         gpsweek = np.array(gpsweek)
 
     # Determine the satellite locations
     sv_posvel = find_sat(ephem, gpstime, gpsweek)
     _, sv_pos, _ = _extract_pos_vel_arr(sv_posvel)
 
     # compute elevation and azimuth
-    el_az = ecef_to_el_az(rx_ecef, sv_pos)
+    el_az = find_elaz(rx_ecef, sv_pos)
     el_r  = np.deg2rad(el_az[:,0])
 
     # Calculate the WGS-84 latitude/longitude of the receiver
     rx_lla = ecef_to_geodetic(rx_ecef)
     height = rx_lla[:,2]
 
     # Force height to be positive
@@ -639,14 +648,89 @@
     c_1 = 2.47
     c_2 = 0.0121
     c_3 = 1.33e-4
     tropo_delay = c_1/(np.sin(el_r)+c_2) * np.exp(-height*c_3)/consts.C
 
     return tropo_delay
 
+
+def find_elaz(rx_pos, sv_pos):
+    """Calculate the elevation and azimuth from a single receiver to multiple
+    satellites.
+
+    Parameters
+    ----------
+    rx_pos : ndarray
+        1x3 vector containing [X, Y, Z] coordinate of receiver
+    sv_pos : ndarray
+        Nx3 array  containing [X, Y, Z] coordinates of satellites
+
+    Returns
+    -------
+    el_az : ndarray
+        Nx2 array containing the elevation and azimuth from the
+        receiver to the requested satellites. Elevation and azimuth are
+        given in decimal degrees.
+
+    Notes
+    -----
+    Code written by J. Makela.
+    AE 456, Global Navigation Sat Systems, University of Illinois
+    Urbana-Champaign. Fall 2017
+
+    """
+
+    # check for 1D case:
+    dim = len(rx_pos.shape)
+    if dim == 1:
+        rx_pos = np.reshape(rx_pos,(1,3))
+
+    dim = len(sv_pos.shape)
+    if dim == 1:
+        sv_pos = np.reshape(sv_pos,(1,3))
+
+    # Convert the receiver location to WGS84
+    rx_lla = ecef_to_geodetic(rx_pos)
+    assert np.shape(rx_lla)==(1,3)
+
+    # Create variables with the latitude and longitude in radians
+    lat = np.deg2rad(rx_lla[0,0])
+    lon = np.deg2rad(rx_lla[0,1])
+
+    # Create the 3 x 3 transform matrix from ECEF to ecef_to_ven
+    cos_lon = np.cos(lon)
+    cos_lat = np.cos(lat)
+    sin_lon = np.sin(lon)
+    sin_lat = np.sin(lat)
+    ecef_to_ven = np.array([[ cos_lat*cos_lon,  cos_lat*sin_lon, sin_lat],
+                            [-sin_lon        ,  cos_lon        , 0.     ],
+                            [-sin_lat*cos_lon, -sin_lat*sin_lon, cos_lat]])
+
+    # Replicate the rx_pos array to be the same size as the satellite array
+    rx_array = np.ones_like(sv_pos) * rx_pos
+
+    # Calculate the pseudorange for each satellite
+    p = sv_pos - rx_array
+
+    # Calculate the length of this vector
+    n = np.array([np.sqrt(p[:,0]**2 + p[:,1]**2 + p[:,2]**2)])
+
+    # Create the normalized unit vector
+    p = p / (np.ones_like(p) * n.T)
+
+    # Perform the transform of the normalized pseudorange from ECEF to VEN
+    p_ven = np.dot(ecef_to_ven, p.T)
+
+    # Calculate elevation and azimuth in degrees
+    el_az = np.zeros([sv_pos.shape[0],2])
+    el_az[:,0] = np.rad2deg((np.pi/2. - np.arccos(p_ven[0,:])))
+    el_az[:,1] = np.rad2deg(np.arctan2(p_ven[1,:],p_ven[2,:]))
+
+    return el_az
+
 def _compute_eccentric_anomoly(M, e, tol=1e-5, max_iter=10):
     """Compute the eccentric anomaly from mean anomaly using the Newton-Raphson
     method using equation: f(E) = M - E + e * sin(E) = 0.
 
     Parameters
     ----------
     M : pd.DataFrame
@@ -667,11 +751,11 @@
     E = M
     for _ in np.arange(0, max_iter):
         f    = M - E + e * np.sin(E)
         dfdE = e*np.cos(E) - 1.
         dE   = -f / dfdE
         E    = E + dE
 
-    if any(dE.iloc[:] > tol):
+    if any(dE > tol):
         print("Eccentric Anomaly may not have converged: dE = ", dE)
 
     return E
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/utils/time_conversions.py` & `gnss_lib_py-0.1.9/gnss_lib_py/utils/time_conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     """
     if isinstance(gps_time, datetime):
         curr_time = gps_time
     else:
         curr_time = GPS_EPOCH_0 + timedelta(milliseconds=gps_time)
         curr_time = curr_time.replace(tzinfo=timezone.utc)
-    curr_time = _check_tzinfo(curr_time)
+    curr_time = tzinfo_to_utc(curr_time)
     if curr_time < GPS_EPOCH_0:
         raise RuntimeError("Need input time after GPS epoch " \
                            + str(GPS_EPOCH_0))
     for row_num, time_frame in enumerate(LEAPSECONDS_TABLE):
         if curr_time >= time_frame:
             out_leapsecs = len(LEAPSECONDS_TABLE)-1 - row_num
             break
@@ -116,15 +116,15 @@
     -------
     gps_week : int
         GPS week.
     tow : float
         GPS time of week [s].
 
     """
-    t_datetime = _check_tzinfo(t_datetime)
+    t_datetime = tzinfo_to_utc(t_datetime)
     if t_datetime < GPS_EPOCH_0:
         raise RuntimeError("Input time must be after GPS epoch " \
                          + str(GPS_EPOCH_0))
     if add_leap_secs:
         out_leapsecs = get_leap_seconds(t_datetime)
         t_datetime = t_datetime + timedelta(seconds=out_leapsecs)
         if verbose: # pragma: no cover
@@ -228,15 +228,15 @@
 
     Returns
     -------
     unix_millis : float
         Milliseconds since UNIX Epoch (1/1/1970 UTC).
 
     """
-    t_datetime = _check_tzinfo(t_datetime)
+    t_datetime = tzinfo_to_utc(t_datetime)
     unix_millis = 1000*(t_datetime - UNIX_EPOCH_0).total_seconds()
     return unix_millis
 
 def datetime_to_gps_millis(t_datetime, add_leap_secs=True):
     """Convert datetime to milliseconds since GPS Epoch.
 
     GPS Epoch starts at the 6th January 1980.
@@ -388,30 +388,33 @@
             unix_millis[t_idx] = datetime_to_unix_millis(t_utc)
         gps_millis = gps_millis.astype(np.int64)
     else:
         t_utc = gps_millis_to_datetime(gps_millis, rem_leap_secs=rem_leap_secs)
         unix_millis = np.int64(datetime_to_unix_millis(t_utc))
     return unix_millis
 
-def _check_tzinfo(t_datetime):
+def tzinfo_to_utc(t_datetime):
     """Raises warning if time doesn't have timezone and converts to UTC.
 
+    If datetime object is offset-naive, then this function will
+    interpret the timezone as UTC and add the appropriate timezone info.
+
     Parameters
     ----------
     t_datetime : datetime.datetime
         Datetime object with no timezone, UTC timezone, or local
         timezone.
 
     Returns
     -------
     t_datetime: datetime.datetime
         Datetime object in UTC, added if no timezone was given and
         converted to UTC if datetime was in local timezone.
 
     """
-    if not hasattr(t_datetime, 'tzinfo') or not t_datetime.tzinfo:
+    if not hasattr(t_datetime, 'tzinfo') or t_datetime.tzinfo is None:
         warnings.warn("No time zone info found in datetime, assuming UTC",\
                         RuntimeWarning)
         t_datetime = t_datetime.replace(tzinfo=timezone.utc)
     if t_datetime.tzinfo != timezone.utc:
         t_datetime = t_datetime.astimezone(timezone.utc)
     return t_datetime
```

### Comparing `gnss_lib_py-0.1.8/gnss_lib_py/utils/visualizations.py` & `gnss_lib_py-0.1.9/gnss_lib_py/utils/visualizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 __authors__ = "D. Knowles"
 __date__ = "27 Jan 2022"
 
 import os
 import pathlib
+from math import floor
 from multiprocessing import Process
 
 import numpy as np
 import pandas as pd
 from cycler import cycler
 import plotly.express as px
 import plotly.graph_objects as go
@@ -247,15 +248,15 @@
     navdata : gnss_lib_py.parsers.navdata.NavData
         Instance of the NavData class. Must include ``gps_millis`` as
         well as satellite ECEF positions as ``x_sv_m``, ``y_sv_m``,
         ``z_sv_m``, ``gnss_id`` and ``sv_id``.
     receiver_state : gnss_lib_py.parsers.navdata.NavData
         Either estimated or ground truth receiver position in ECEF frame
         in meters as an instance of the NavData class with the
-        following rows: ``x_*_m``, ``y_*_m``, ``z_*_m``, ``gps_millis``.
+        following rows: ``x_rx*_m``, ``y_rx*_m``, ``z_rx*_m``, ``gps_millis``.
     save : bool
         Saves figure if true to file specified by ``fname`` or defaults
         to the Results folder otherwise.
     prefix : string
         File prefix to add to filename.
     fname : string or path-like
         Path to save figure to. If not None, ``fname`` is passed
@@ -404,17 +405,17 @@
 
     for idx, traj_data in enumerate(args):
         if not isinstance(traj_data, NavData):
             raise TypeError("Input(s) to plot_map() must be of type " \
                           + "NavData.")
 
         # check for lat/lon indexes
-        traj_idxs = traj_data.find_wildcard_indexes(["lat_*_deg",
-                                                     "lon_*_deg"],
-                                                     max_allow=1)
+        traj_idxs = traj_data.find_wildcard_indexes(
+                    wildcards=["lat_*_deg","lon_*_deg"], max_allow=1,
+                    excludes=[["lat_sigma_*_deg"],["lon_sigma_*_deg"]])
 
         label_name = _get_label({"":"_".join((traj_idxs["lat_*_deg"][0].split("_"))[1:-1])})
 
         data = {"latitude" : traj_data[traj_idxs["lat_*_deg"][0]],
                 "longitude" : traj_data[traj_idxs["lon_*_deg"][0]],
                 "Trajectory" : [label_name] * len(traj_data),
                 }
@@ -802,15 +803,15 @@
 
     # assumed Mercator projection
     margin = 2.5
     height = (maxlat - minlat) * margin * width_to_height
     width = (maxlon - minlon) * margin
     lon_zoom = np.interp(width , lon_zoom_range, range(20, 0, -1))
     lat_zoom = np.interp(height, lon_zoom_range, range(20, 0, -1))
-    zoom = round(min(lon_zoom, lat_zoom), 2)
+    zoom = floor(min(lon_zoom, lat_zoom))
 
     return zoom, center
 
 def _save_plotly(figures, titles=None, prefix="", fnames=None,
                  width=730, height=520): # pragma: no cover
     """Saves figures to file.
```

### Comparing `gnss_lib_py-0.1.8/pyproject.toml` & `gnss_lib_py-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gnss-lib-py"
-version = "0.1.8"
+version = "0.1.9"
 description = "Modular Python tool for parsing, analyzing, and visualizing Global Navigation Satellite Systems (GNSS) data and state estimates"
 authors = ["Derek Knowles <dcknowles@stanford.edu>",
            "Ashwin Kanhere <akanhere@stanford.edu>",
            ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Stanford-NavLab/gnss_lib_py"
@@ -15,37 +15,39 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, < 3.12"
 numpy = "^1.21.0"
-pandas = "^1.3.0"
+pandas = "^2.0.0"
 DateTime = "^4.3"
 georinex = "^1.15.0"
 unlzw3 = "^0.2.1"
 reindent = "^3.5.1"
 pynmea2 = "^1.18.0"
-pytest = "^6.2.5"
+pytest = ">=7.2"
 pylint = "^2.11.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 scipy = "^1.7.3"
 jupyter = "^1.0.0"
 pytest-lazy-fixture = "^0.6.3"
 matplotlib = "^3.5.1"
 plotly = "^5.8.0"
 kaleido = "0.2.1"
+requests = "^2.29.0"
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = "^4.1.1"
 sphinx-rtd-theme = "^0.5.2"
 sphinxcontrib-napoleon = "^0.7"
 notebook = "^6.4.2"
 ipykernel = "^6.0.3"
 jupyter = "^1.0.0"
 pylint-exit = "^1.2.0"
 nbsphinx = "^0.8.9"
 nbsphinx-link = "^1.3.0"
+tqdm = "^4.65.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gnss_lib_py-0.1.8/setup.py` & `gnss_lib_py-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,178 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gnss-lib-py
+Version: 0.1.9
+Summary: Modular Python tool for parsing, analyzing, and visualizing Global Navigation Satellite Systems (GNSS) data and state estimates
+Home-page: https://github.com/Stanford-NavLab/gnss_lib_py
+License: MIT
+Keywords: gnss
+Author: Derek Knowles
+Author-email: dcknowles@stanford.edu
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: DateTime (>=4.3,<5.0)
+Requires-Dist: georinex (>=1.15.0,<2.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: plotly (>=5.8.0,<6.0.0)
+Requires-Dist: pylint (>=2.11.1,<3.0.0)
+Requires-Dist: pynmea2 (>=1.18.0,<2.0.0)
+Requires-Dist: pytest (>=7.2)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
+Requires-Dist: pytest-lazy-fixture (>=0.6.3,<0.7.0)
+Requires-Dist: reindent (>=3.5.1,<4.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: scipy (>=1.7.3,<2.0.0)
+Requires-Dist: unlzw3 (>=0.2.1,<0.3.0)
+Project-URL: Documentation, https://gnss-lib-py.readthedocs.io/en/latest/
+Description-Content-Type: text/markdown
+
+[![build](https://github.com/Stanford-NavLab/gnss_lib_py/actions/workflows/build.yml/badge.svg)](https://github.com/Stanford-NavLab/gnss_lib_py/actions/workflows/build.yml)
+[![codecov](https://codecov.io/gh/Stanford-NavLab/gnss_lib_py/branch/main/graph/badge.svg?token=1FBGEWRFM6)](https://codecov.io/gh/Stanford-NavLab/gnss_lib_py)
+[![Documentation Status](https://readthedocs.org/projects/gnss_lib_py/badge/?version=latest)](https://gnss_lib_py.readthedocs.io/en/latest/?badge=latest)
+
+gnss_lib_py
+===========
+
+`gnss_lib_py` is a modular Python tool for parsing, analyzing, and
+visualizing Global Navigation Satellite Systems (GNSS) data and state
+estimates.
+It also provides an intuitive and modular framework allowing users to
+quickly prototype, implement, and visualize GNSS algorithms.
+`gnss_lib_py` is modular in the sense that multiple types of
+algorithms can be easily exchanged for each other and extendable in
+facilitating user-specific extensions of existing implementations.
+
+<img src="https://raw.githubusercontent.com/Stanford-NavLab/gnss_lib_py/main/docs/source/img/skyplot.png" alt="satellite skyplot" width="600"/>
+
+`gnss_lib_py` contains parsers for common file types used for
+storing GNSS measurements, benchmark algorithms for processing
+measurements into state estimates and visualization tools for measurements
+and state estimates.
+The modularity of `gnss_lib_py` is made possibly by the unifying
+`NavData` class, which contains methods to add, remove and modify
+numeric and string data consistently.
+We provide standard row names for `NavData` elements on the
+[reference page](https://gnss-lib-py.readthedocs.io/en/latest/reference/reference.html).
+These names ensure cross compatability between different datasets and
+algorithms.
+
+Documentation
+-------------
+Full documentation is available on our [readthedocs website](https://gnss-lib-py.readthedocs.io/en/latest/index.html).
+
+
+Code Organization
+-----------------
+
+`gnss_lib_py` is organized as:
+
+```bash
+
+   ├── data/                          # Location for data files
+      └── unit_test/                  # Data files for unit testing
+   ├── dev/                           # Code users do not wish to commit
+   ├── docs/                          # Documentation files
+   ├── gnss_lib_py/                   # gnss_lib_py source files
+        ├── algorithms/               # Navigation algorithms
+        ├── parsers/                  # Data parsers
+        ├── utils/                    # GNSS and common utilities
+        └── __init__.py
+   ├── notebooks/                     # Interactive Jupyter notebooks
+        ├── tutorials/                # Notebooks with tutorial code
+   ├── results/                       # Location for result images/files
+   ├── tests/                         # Tests for source files
+      ├── algorithms/                 # Tests for files in algorithms
+      ├── parsers/                    # Tests for files in parsers
+      ├── utils/                      # Tests for files in utils
+      └── test_gnss_lib_py.py         # High level checks for repository
+   ├── CONTRIBUTORS.md                # List of contributors
+   ├── build_docs.sh                  # Bash script to build docs
+   ├── poetry.lock                    # Poetry specific Lock file
+   ├── pyproject.toml                 # List of package dependencies
+   └── requirements.txt               # List of packages for pip install
+```
+In the directory organization above:
+
+  * The `algorithms` directory contains localization algorithms that
+    work by passing in a `NavData` class. Currently, the following
+    algorithms are implemented in the `algorithms`:
+
+      * Weighted Least Squares
+      * Extended Kalman Filter
+      * Calculating pseudorange residuals
+      * Calculating multi-GNSS satellite PVT information
+  * The data parsers in the `parsers` directory allow for either loading
+    GNSS data into `gnss_lib_py`'s unifying `NavData` class or parsing
+    precise ephemerides data.
+    Currently, the following datasets and types are supported:
+
+      * [2021 Google Android Derived Dataset](https://www.kaggle.com/c/google-smartphone-decimeter-challenge)
+      * [2022 Google Android Derived Dataset](https://www.kaggle.com/competitions/smartphone-decimeter-2022)
+      * [Precise Ephemeris Data](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/gnss_mgex.html)
+
+  * The `utils` directory contains utilities used to handle
+    GNSS measurements, time conversions, visualizations, satellite
+    simulation, file operations, etc.
+
+Installation
+------------
+
+`gnss_lib_py` is available through `pip` installation with:
+
+```
+pip install gnss-lib-py
+```
+
+For directions on how to install an editable or developer installation of `gnss_lib_py` on Linux, MacOS, and Windows, please
+see the [install instructions](https://gnss-lib-py.readthedocs.io/en/latest/install.html).
+
+Tutorials
+---------
+We have a range of tutorials on how to easily use this project. They can
+all be found in the [tutorials section](https://gnss-lib-py.readthedocs.io/en/latest/tutorials/tutorials.html).
+
+Reference
+---------
+References on the package contents, explanation of the benefits of our
+custom NavData class, and function-level documentation can all be
+found in the [reference section](https://gnss-lib-py.readthedocs.io/en/latest/reference/reference.html).
+
+Contributing
+------------
+If you have a bug report or would like to contribute to our repository,
+please follow the guide on the [contributing page](https://gnss-lib-py.readthedocs.io/en/latest/contributing/contributing.html).
+
+Troubleshooting
+---------------
+Answers to common questions can be found in the [troubleshooting section](https://gnss-lib-py.readthedocs.io/en/latest/troubleshooting.html).
+
+Attribution
+-----------
+This project is a product of the [Stanford NAV Lab](https://navlab.stanford.edu/)
+and currently maintained by Ashwin Kanhere and Derek Knowles. If using
+this project in your own work please cite the following:
+
+```
+
+   @inproceedings{knowlesmodular2022,
+      title = {A Modular and Extendable GNSS Python Library},
+      author={Knowles, Derek and Kanhere, Ashwin V and Bhamidipati, Sriramya and Gao, Grace},
+      booktitle={Proceedings of the 35th International Technical Meeting of the Satellite Division of The Institute of Navigation (ION GNSS+ 2022)},
+      institution = {Stanford University},
+      year = {2022 [Online]},
+      url = {https://github.com/Stanford-NavLab/gnss_lib_py},
+   }
+```
 
-packages = \
-['gnss_lib_py',
- 'gnss_lib_py.algorithms',
- 'gnss_lib_py.parsers',
- 'gnss_lib_py.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['DateTime>=4.3,<5.0',
- 'georinex>=1.15.0,<2.0.0',
- 'jupyter>=1.0.0,<2.0.0',
- 'kaleido==0.2.1',
- 'matplotlib>=3.5.1,<4.0.0',
- 'numpy>=1.21.0,<2.0.0',
- 'pandas>=1.3.0,<2.0.0',
- 'plotly>=5.8.0,<6.0.0',
- 'pylint>=2.11.1,<3.0.0',
- 'pynmea2>=1.18.0,<2.0.0',
- 'pytest-cov>=3.0.0,<4.0.0',
- 'pytest-lazy-fixture>=0.6.3,<0.7.0',
- 'pytest>=6.2.5,<7.0.0',
- 'reindent>=3.5.1,<4.0.0',
- 'scipy>=1.7.3,<2.0.0',
- 'unlzw3>=0.2.1,<0.3.0']
-
-setup_kwargs = {
-    'name': 'gnss-lib-py',
-    'version': '0.1.8',
-    'description': 'Modular Python tool for parsing, analyzing, and visualizing Global Navigation Satellite Systems (GNSS) data and state estimates',
-    'long_description': '[![build](https://github.com/Stanford-NavLab/gnss_lib_py/actions/workflows/build.yml/badge.svg)](https://github.com/Stanford-NavLab/gnss_lib_py/actions/workflows/build.yml)\n[![codecov](https://codecov.io/gh/Stanford-NavLab/gnss_lib_py/branch/main/graph/badge.svg?token=1FBGEWRFM6)](https://codecov.io/gh/Stanford-NavLab/gnss_lib_py)\n[![Documentation Status](https://readthedocs.org/projects/gnss_lib_py/badge/?version=latest)](https://gnss_lib_py.readthedocs.io/en/latest/?badge=latest)\n\ngnss_lib_py\n===========\n\n`gnss_lib_py` is a modular Python tool for parsing, analyzing, and\nvisualizing Global Navigation Satellite Systems (GNSS) data and state\nestimates.\nIt also provides an intuitive and modular framework allowing users to\nquickly prototype, implement, and visualize GNSS algorithms.\n`gnss_lib_py` is modular in the sense that multiple types of\nalgorithms can be easily exchanged for each other and extendable in\nfacilitating user-specific extensions of existing implementations.\n\n<img src="https://raw.githubusercontent.com/Stanford-NavLab/gnss_lib_py/main/docs/source/img/skyplot.png" alt="satellite skyplot" width="600"/>\n\n`gnss_lib_py` contains parsers for common file types used for\nstoring GNSS measurements, benchmark algorithms for processing\nmeasurements into state estimates and visualization tools for measurements\nand state estimates.\nThe modularity of `gnss_lib_py` is made possibly by the unifying\n`NavData` class, which contains methods to add, remove and modify\nnumeric and string data consistently.\nWe provide standard row names for `NavData` elements on the\n[reference page](https://gnss-lib-py.readthedocs.io/en/latest/reference/reference.html).\nThese names ensure cross compatability between different datasets and\nalgorithms.\n\nDocumentation\n-------------\nFull documentation is available on our [readthedocs website](https://gnss-lib-py.readthedocs.io/en/latest/index.html).\n\n\nCode Organization\n-----------------\n\n`gnss_lib_py` is organized as:\n\n```bash\n\n   ├── data/                          # Location for data files\n      └── unit_test/                  # Data files for unit testing\n   ├── dev/                           # Code users do not wish to commit\n   ├── docs/                          # Documentation files\n   ├── gnss_lib_py/                   # gnss_lib_py source files\n        ├── algorithms/               # Navigation algorithms\n        ├── parsers/                  # Data parsers\n        ├── utils/                    # GNSS and common utilities\n        └── __init__.py\n   ├── notebooks/                     # Interactive Jupyter notebooks\n        ├── tutorials/                # Notebooks with tutorial code\n   ├── results/                       # Location for result images/files\n   ├── tests/                         # Tests for source files\n      ├── algorithms/                 # Tests for files in algorithms\n      ├── parsers/                    # Tests for files in parsers\n      ├── utils/                      # Tests for files in utils\n      └── test_gnss_lib_py.py         # High level checks for repository\n   ├── CONTRIBUTORS.md                # List of contributors\n   ├── build_docs.sh                  # Bash script to build docs\n   ├── poetry.lock                    # Poetry specific Lock file\n   ├── pyproject.toml                 # List of package dependencies\n   └── requirements.txt               # List of packages for pip install\n```\nIn the directory organization above:\n\n  * The `algorithms` directory contains localization algorithms that\n    work by passing in a `NavData` class. Currently, the following\n    algorithms are implemented in the `algorithms`:\n\n      * Weighted Least Squares\n      * Extended Kalman Filter\n      * Calculating pseudorange residuals\n      * Calculating multi-GNSS satellite PVT information\n  * The data parsers in the `parsers` directory allow for either loading\n    GNSS data into `gnss_lib_py`\'s unifying `NavData` class or parsing\n    precise ephemerides data.\n    Currently, the following datasets and types are supported:\n\n      * [2021 Google Android Derived Dataset](https://www.kaggle.com/c/google-smartphone-decimeter-challenge)\n      * [2022 Google Android Derived Dataset](https://www.kaggle.com/competitions/smartphone-decimeter-2022)\n      * [Precise Ephemeris Data](https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/gnss_mgex.html)\n\n  * The `utils` directory contains utilities used to handle\n    GNSS measurements, time conversions, visualizations, satellite\n    simulation, file operations, etc.\n\nInstallation\n------------\n\n`gnss_lib_py` is available through `pip` installation with:\n\n```\npip install gnss-lib-py\n```\n\nFor directions on how to install an editable or developer installation of `gnss_lib_py` on Linux, MacOS, and Windows, please\nsee the [install instructions](https://gnss-lib-py.readthedocs.io/en/latest/install.html).\n\nTutorials\n---------\nWe have a range of tutorials on how to easily use this project. They can\nall be found in the [tutorials section](https://gnss-lib-py.readthedocs.io/en/latest/tutorials/tutorials.html).\n\nReference\n---------\nReferences on the package contents, explanation of the benefits of our\ncustom NavData class, and function-level documentation can all be\nfound in the [reference section](https://gnss-lib-py.readthedocs.io/en/latest/reference/reference.html).\n\nContributing\n------------\nIf you have a bug report or would like to contribute to our repository,\nplease follow the guide on the [contributing page](https://gnss-lib-py.readthedocs.io/en/latest/contributing/contributing.html).\n\nTroubleshooting\n---------------\nAnswers to common questions can be found in the [troubleshooting section](https://gnss-lib-py.readthedocs.io/en/latest/troubleshooting.html).\n\nAttribution\n-----------\nThis project is a product of the [Stanford NAV Lab](https://navlab.stanford.edu/)\nand currently maintained by Ashwin Kanhere and Derek Knowles. If using\nthis project in your own work please cite the following:\n\n```\n\n   @inproceedings{knowlesmodular2022,\n      title = {A Modular and Extendable GNSS Python Library},\n      author={Knowles, Derek and Kanhere, Ashwin V and Bhamidipati, Sriramya and Gao, Grace},\n      booktitle={Proceedings of the 35th International Technical Meeting of the Satellite Division of The Institute of Navigation (ION GNSS+ 2022)},\n      institution = {Stanford University},\n      year = {2022 [Online]},\n      url = {https://github.com/Stanford-NavLab/gnss_lib_py},\n   }\n```\n\nAdditionally, we would like to thank [all contributors](https://github.com/Stanford-NavLab/gnss_lib_py/blob/main/CONTRIBUTORS.md) to this project.\n',
-    'author': 'Derek Knowles',
-    'author_email': 'dcknowles@stanford.edu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Stanford-NavLab/gnss_lib_py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
+Additionally, we would like to thank [all contributors](https://github.com/Stanford-NavLab/gnss_lib_py/blob/main/CONTRIBUTORS.md) to this project.
 
-
-setup(**setup_kwargs)
```

