# Comparing `tmp/OTTAR-0.4.0.tar.gz` & `tmp/OTTAR-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OTTAR-0.4.0.tar", last modified: Wed Dec 14 15:52:59 2022, max compression
+gzip compressed data, was "OTTAR-0.5.0.tar", last modified: Tue Jul 18 11:37:24 2023, max compression
```

## Comparing `OTTAR-0.4.0.tar` & `OTTAR-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 awickert  (1000) awickert  (1000)        0 2022-12-14 15:52:59.855222 OTTAR-0.4.0/
--rw-rw-r--   0 awickert  (1000) awickert  (1000)    35149 2022-04-22 11:12:10.000000 OTTAR-0.4.0/LICENSE
-drwxrwxr-x   0 awickert  (1000) awickert  (1000)        0 2022-12-14 15:52:59.855222 OTTAR-0.4.0/OTTAR.egg-info/
--rw-rw-r--   0 awickert  (1000) awickert  (1000)     7889 2022-12-14 15:52:59.000000 OTTAR-0.4.0/OTTAR.egg-info/PKG-INFO
--rw-rw-r--   0 awickert  (1000) awickert  (1000)      213 2022-12-14 15:52:59.000000 OTTAR-0.4.0/OTTAR.egg-info/SOURCES.txt
--rw-rw-r--   0 awickert  (1000) awickert  (1000)        1 2022-12-14 15:52:59.000000 OTTAR-0.4.0/OTTAR.egg-info/dependency_links.txt
--rw-rw-r--   0 awickert  (1000) awickert  (1000)       30 2022-12-14 15:52:59.000000 OTTAR-0.4.0/OTTAR.egg-info/requires.txt
--rw-rw-r--   0 awickert  (1000) awickert  (1000)        6 2022-12-14 15:52:59.000000 OTTAR-0.4.0/OTTAR.egg-info/top_level.txt
--rw-rw-r--   0 awickert  (1000) awickert  (1000)     7889 2022-12-14 15:52:59.859222 OTTAR-0.4.0/PKG-INFO
--rw-rw-r--   0 awickert  (1000) awickert  (1000)     6917 2022-12-14 15:50:03.000000 OTTAR-0.4.0/README.md
-drwxrwxr-x   0 awickert  (1000) awickert  (1000)        0 2022-12-14 15:52:59.855222 OTTAR-0.4.0/ottar/
--rw-rw-r--   0 awickert  (1000) awickert  (1000)      172 2022-04-26 09:10:09.000000 OTTAR-0.4.0/ottar/__init__.py
--rw-rw-r--   0 awickert  (1000) awickert  (1000)    34121 2022-12-04 09:36:15.000000 OTTAR-0.4.0/ottar/ottar.py
--rw-r--r--   0 awickert  (1000) awickert  (1000)      132 2022-12-14 15:52:59.859222 OTTAR-0.4.0/setup.cfg
--rw-rw-r--   0 awickert  (1000) awickert  (1000)     1283 2022-12-14 15:50:30.000000 OTTAR-0.4.0/setup.py
+drwxrwxr-x   0 awickert  (1001) awickert  (1001)        0 2023-07-18 11:37:24.824383 OTTAR-0.5.0/
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)    35149 2023-04-22 15:14:09.000000 OTTAR-0.5.0/LICENSE
+drwxrwxr-x   0 awickert  (1001) awickert  (1001)        0 2023-07-18 11:37:24.824383 OTTAR-0.5.0/OTTAR.egg-info/
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     8178 2023-07-18 11:37:24.000000 OTTAR-0.5.0/OTTAR.egg-info/PKG-INFO
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)      213 2023-07-18 11:37:24.000000 OTTAR-0.5.0/OTTAR.egg-info/SOURCES.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)        1 2023-07-18 11:37:24.000000 OTTAR-0.5.0/OTTAR.egg-info/dependency_links.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)       30 2023-07-18 11:37:24.000000 OTTAR-0.5.0/OTTAR.egg-info/requires.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)        6 2023-07-18 11:37:24.000000 OTTAR-0.5.0/OTTAR.egg-info/top_level.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     8178 2023-07-18 11:37:24.824383 OTTAR-0.5.0/PKG-INFO
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     7206 2023-07-06 19:32:34.000000 OTTAR-0.5.0/README.md
+drwxrwxr-x   0 awickert  (1001) awickert  (1001)        0 2023-07-18 11:37:24.824383 OTTAR-0.5.0/ottar/
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)      172 2023-04-22 15:14:09.000000 OTTAR-0.5.0/ottar/__init__.py
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)    35953 2023-07-08 15:31:04.000000 OTTAR-0.5.0/ottar/ottar.py
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)      132 2023-07-18 11:37:24.824383 OTTAR-0.5.0/setup.cfg
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     1283 2023-07-18 09:18:59.000000 OTTAR-0.5.0/setup.py
```

### Comparing `OTTAR-0.4.0/LICENSE` & `OTTAR-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OTTAR-0.4.0/OTTAR.egg-info/PKG-INFO` & `OTTAR-0.5.0/OTTAR.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OTTAR
-Version: 0.4.0
+Version: 0.5.0
 Summary: Ode To Transient Ancho de los Rivers: Transient evolution of river-channel width
 Home-page: https://github.com/MNiMORPH/ottar
 Author: Andrew D. Wickert
 Author-email: awickert@umn.edu
 License: UNKNOWN
 Project-URL: Source and README, https://github.com/MNiMORPH/OTTAR
 Project-URL: CSDMS repository, https://csdms.colorado.edu/wiki/Model:OTTAR
@@ -63,18 +63,19 @@
 
 | **Variable** 	| **Description**                                                                                                                                                                                                                                                                                                   	| **Typical value(s)**        	|
 |------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|-----------------------------	|
 | `h_banks`    	    | **Stream-bank height**. This is the thickness of material that must be removed for the river to widen by one unit lateral distance.                                                                                                                                                                                            	| 1-5 m                       	|
 | `S`          	    | **Channel downstream-directed slope**. This is used to compute shear stresses and (if necessary) flow depth from water discharge.                                                                                                                                                                                              	| 10<sup>&minus;3</sup>             	|
 | `b0`         	    | **Initial width**. Starting width of a channel.                                                                                                                                                                                                                                                                                	| 1&ndash;1000 m                   	|
 | `tau_crit`   	    | **Critical shear stress required to start eroding muddy banks**. At this stress, the flow begins to be able to detach particles. When set up to perform an **inversion** using data on river widening and past flows, this is one of two key parameters to be estimated for rivers with detachment-limited banks. 	| 1&ndash;10 Pa                     	|
+| `tau_star_crit_sed` | **Critical shear stress required initiate sediment motion**. This defaults to 0.0495 from the Wong & Parker (2006) rebuild of the Meyer-Peter & Müller (1948) sediment-transport equation. 	| 0.03&ndash;0.06                     	|
 | `k_d`        	    | **Cohesive-detachment erosion-rate coefficient**. This determines the rate of erosion as a function of shear stress above critical. When set up to perform an **inversion** using data on river widening and past flows, this is the other of two key parameters to be estimated.                         	| ~10<sup>&minus;7</sup> m / (Pa s) 	|
-| `k_E`        	    | **Noncohesive erosion-rate (entrainment) coefficient**. This relates Shields stress above critical to sediment entrainment rate.                         	| ~0.1&ndash;1 / s 	|
-| `f_stickiness`    | **Fraction of suspended-load particles contacting the bank that "stick" to it**. This modulates the turbulence-driven lateral-transport term and its impact on channel-narrowing rate, and comprises the abillity of banks to trap sediment and to hold it.                                                                                                                                                                                                                                  	| ~0.01&ndash;1              	|
-| `k_n_noncohesive` | **Narrowing coefficient (noncohesive sediment)**. Trapping and holding efficiency in regards to noncohesive sediment; this may be due to deep pits between grains and/or other bank-rougness properties.                                                                                                                                                                                                                                                                                     	| ~0.01&ndash;1              	|
+| `k_E`        	    | **Noncohesive erosion-rate (entrainment) coefficient**. This relates theoretical sediment entrainment rate via near-bank Shields stress to bank-retreat rate via erosion.                         	| ~0.01&ndash;1       |
+| `f_stickiness`    | **Fraction of suspended-load particles contacting the bank that "stick" to it**. This modulates the turbulence-driven lateral-transport term and its impact on channel-narrowing rate, and comprises the abillity of banks to trap sediment and to hold it.                                                                                                                                                                                                                                  	| 0&ndash;1              	|
+| `k_n_noncohesive` | **Narrowing coefficient (noncohesive sediment)**. Trapping and holding efficiency in regards to noncohesive sediment; this may be due to deep pits between grains and/or other bank-rougness properties.                                                                                                                                                                                                                                                                                     	| 0&ndash;1              	|
 | `Parker_epsilon`  | **Excess bed shear-stress factor**. $\tau_b = (1+\epsilon) \tau_\beta$, where $\tau_b$ is bed shear stress and $\tau_\beta$ is bank shear stress.                                                                                                                                                                           	| 0.2                            	|
 | `intermittency`  | **Intermittency**. Fraction of the time that the discharge given is active. This is always equal to 1 for a full hydrograph, and is $\leq$ 1 when a characteristic "geomorphically effective" discharge is considered. It can be thought of as a time-dialation factor.                                                        	| 10<sup>&minus;3</sup>&ndash;1                	|
 | `D`          	    | **Sediment median grain size**. This is the median size of the material both in transport and in the banks, and is required for bedload and/or noncohesive-sediment-dominated systems. It may also be specified for rivers dominated by susepended load and bank cohesion, though will likely play a more minor role in these.	| 10<sup>&minus;4</sup>&ndash;1 m                       	|
 
 #### Key input data sets and parameters (FlowDepthDoubleManning)
 
 *This step is used to compute flow depths from a discharge time series, and may be skipped if you already posess a time series of flow depth*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `OTTAR-0.4.0/PKG-INFO` & `OTTAR-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OTTAR
-Version: 0.4.0
+Version: 0.5.0
 Summary: Ode To Transient Ancho de los Rivers: Transient evolution of river-channel width
 Home-page: https://github.com/MNiMORPH/ottar
 Author: Andrew D. Wickert
 Author-email: awickert@umn.edu
 License: UNKNOWN
 Project-URL: Source and README, https://github.com/MNiMORPH/OTTAR
 Project-URL: CSDMS repository, https://csdms.colorado.edu/wiki/Model:OTTAR
@@ -63,18 +63,19 @@
 
 | **Variable** 	| **Description**                                                                                                                                                                                                                                                                                                   	| **Typical value(s)**        	|
 |------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|-----------------------------	|
 | `h_banks`    	    | **Stream-bank height**. This is the thickness of material that must be removed for the river to widen by one unit lateral distance.                                                                                                                                                                                            	| 1-5 m                       	|
 | `S`          	    | **Channel downstream-directed slope**. This is used to compute shear stresses and (if necessary) flow depth from water discharge.                                                                                                                                                                                              	| 10<sup>&minus;3</sup>             	|
 | `b0`         	    | **Initial width**. Starting width of a channel.                                                                                                                                                                                                                                                                                	| 1&ndash;1000 m                   	|
 | `tau_crit`   	    | **Critical shear stress required to start eroding muddy banks**. At this stress, the flow begins to be able to detach particles. When set up to perform an **inversion** using data on river widening and past flows, this is one of two key parameters to be estimated for rivers with detachment-limited banks. 	| 1&ndash;10 Pa                     	|
+| `tau_star_crit_sed` | **Critical shear stress required initiate sediment motion**. This defaults to 0.0495 from the Wong & Parker (2006) rebuild of the Meyer-Peter & Müller (1948) sediment-transport equation. 	| 0.03&ndash;0.06                     	|
 | `k_d`        	    | **Cohesive-detachment erosion-rate coefficient**. This determines the rate of erosion as a function of shear stress above critical. When set up to perform an **inversion** using data on river widening and past flows, this is the other of two key parameters to be estimated.                         	| ~10<sup>&minus;7</sup> m / (Pa s) 	|
-| `k_E`        	    | **Noncohesive erosion-rate (entrainment) coefficient**. This relates Shields stress above critical to sediment entrainment rate.                         	| ~0.1&ndash;1 / s 	|
-| `f_stickiness`    | **Fraction of suspended-load particles contacting the bank that "stick" to it**. This modulates the turbulence-driven lateral-transport term and its impact on channel-narrowing rate, and comprises the abillity of banks to trap sediment and to hold it.                                                                                                                                                                                                                                  	| ~0.01&ndash;1              	|
-| `k_n_noncohesive` | **Narrowing coefficient (noncohesive sediment)**. Trapping and holding efficiency in regards to noncohesive sediment; this may be due to deep pits between grains and/or other bank-rougness properties.                                                                                                                                                                                                                                                                                     	| ~0.01&ndash;1              	|
+| `k_E`        	    | **Noncohesive erosion-rate (entrainment) coefficient**. This relates theoretical sediment entrainment rate via near-bank Shields stress to bank-retreat rate via erosion.                         	| ~0.01&ndash;1       |
+| `f_stickiness`    | **Fraction of suspended-load particles contacting the bank that "stick" to it**. This modulates the turbulence-driven lateral-transport term and its impact on channel-narrowing rate, and comprises the abillity of banks to trap sediment and to hold it.                                                                                                                                                                                                                                  	| 0&ndash;1              	|
+| `k_n_noncohesive` | **Narrowing coefficient (noncohesive sediment)**. Trapping and holding efficiency in regards to noncohesive sediment; this may be due to deep pits between grains and/or other bank-rougness properties.                                                                                                                                                                                                                                                                                     	| 0&ndash;1              	|
 | `Parker_epsilon`  | **Excess bed shear-stress factor**. $\tau_b = (1+\epsilon) \tau_\beta$, where $\tau_b$ is bed shear stress and $\tau_\beta$ is bank shear stress.                                                                                                                                                                           	| 0.2                            	|
 | `intermittency`  | **Intermittency**. Fraction of the time that the discharge given is active. This is always equal to 1 for a full hydrograph, and is $\leq$ 1 when a characteristic "geomorphically effective" discharge is considered. It can be thought of as a time-dialation factor.                                                        	| 10<sup>&minus;3</sup>&ndash;1                	|
 | `D`          	    | **Sediment median grain size**. This is the median size of the material both in transport and in the banks, and is required for bedload and/or noncohesive-sediment-dominated systems. It may also be specified for rivers dominated by susepended load and bank cohesion, though will likely play a more minor role in these.	| 10<sup>&minus;4</sup>&ndash;1 m                       	|
 
 #### Key input data sets and parameters (FlowDepthDoubleManning)
 
 *This step is used to compute flow depths from a discharge time series, and may be skipped if you already posess a time series of flow depth*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `OTTAR-0.4.0/README.md` & `OTTAR-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,19 @@
 
 | **Variable** 	| **Description**                                                                                                                                                                                                                                                                                                   	| **Typical value(s)**        	|
 |------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|-----------------------------	|
 | `h_banks`    	    | **Stream-bank height**. This is the thickness of material that must be removed for the river to widen by one unit lateral distance.                                                                                                                                                                                            	| 1-5 m                       	|
 | `S`          	    | **Channel downstream-directed slope**. This is used to compute shear stresses and (if necessary) flow depth from water discharge.                                                                                                                                                                                              	| 10<sup>&minus;3</sup>             	|
 | `b0`         	    | **Initial width**. Starting width of a channel.                                                                                                                                                                                                                                                                                	| 1&ndash;1000 m                   	|
 | `tau_crit`   	    | **Critical shear stress required to start eroding muddy banks**. At this stress, the flow begins to be able to detach particles. When set up to perform an **inversion** using data on river widening and past flows, this is one of two key parameters to be estimated for rivers with detachment-limited banks. 	| 1&ndash;10 Pa                     	|
+| `tau_star_crit_sed` | **Critical shear stress required initiate sediment motion**. This defaults to 0.0495 from the Wong & Parker (2006) rebuild of the Meyer-Peter & Müller (1948) sediment-transport equation. 	| 0.03&ndash;0.06                     	|
 | `k_d`        	    | **Cohesive-detachment erosion-rate coefficient**. This determines the rate of erosion as a function of shear stress above critical. When set up to perform an **inversion** using data on river widening and past flows, this is the other of two key parameters to be estimated.                         	| ~10<sup>&minus;7</sup> m / (Pa s) 	|
-| `k_E`        	    | **Noncohesive erosion-rate (entrainment) coefficient**. This relates Shields stress above critical to sediment entrainment rate.                         	| ~0.1&ndash;1 / s 	|
-| `f_stickiness`    | **Fraction of suspended-load particles contacting the bank that "stick" to it**. This modulates the turbulence-driven lateral-transport term and its impact on channel-narrowing rate, and comprises the abillity of banks to trap sediment and to hold it.                                                                                                                                                                                                                                  	| ~0.01&ndash;1              	|
-| `k_n_noncohesive` | **Narrowing coefficient (noncohesive sediment)**. Trapping and holding efficiency in regards to noncohesive sediment; this may be due to deep pits between grains and/or other bank-rougness properties.                                                                                                                                                                                                                                                                                     	| ~0.01&ndash;1              	|
+| `k_E`        	    | **Noncohesive erosion-rate (entrainment) coefficient**. This relates theoretical sediment entrainment rate via near-bank Shields stress to bank-retreat rate via erosion.                         	| ~0.01&ndash;1       |
+| `f_stickiness`    | **Fraction of suspended-load particles contacting the bank that "stick" to it**. This modulates the turbulence-driven lateral-transport term and its impact on channel-narrowing rate, and comprises the abillity of banks to trap sediment and to hold it.                                                                                                                                                                                                                                  	| 0&ndash;1              	|
+| `k_n_noncohesive` | **Narrowing coefficient (noncohesive sediment)**. Trapping and holding efficiency in regards to noncohesive sediment; this may be due to deep pits between grains and/or other bank-rougness properties.                                                                                                                                                                                                                                                                                     	| 0&ndash;1              	|
 | `Parker_epsilon`  | **Excess bed shear-stress factor**. $\tau_b = (1+\epsilon) \tau_\beta$, where $\tau_b$ is bed shear stress and $\tau_\beta$ is bank shear stress.                                                                                                                                                                           	| 0.2                            	|
 | `intermittency`  | **Intermittency**. Fraction of the time that the discharge given is active. This is always equal to 1 for a full hydrograph, and is $\leq$ 1 when a characteristic "geomorphically effective" discharge is considered. It can be thought of as a time-dialation factor.                                                        	| 10<sup>&minus;3</sup>&ndash;1                	|
 | `D`          	    | **Sediment median grain size**. This is the median size of the material both in transport and in the banks, and is required for bedload and/or noncohesive-sediment-dominated systems. It may also be specified for rivers dominated by susepended load and bank cohesion, though will likely play a more minor role in these.	| 10<sup>&minus;4</sup>&ndash;1 m                       	|
 
 #### Key input data sets and parameters (FlowDepthDoubleManning)
 
 *This step is used to compute flow depths from a discharge time series, and may be skipped if you already posess a time series of flow depth*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `OTTAR-0.4.0/ottar/ottar.py` & `OTTAR-0.5.0/ottar/ottar.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     Transient adjustments to river-channel width
     """
 
     def __init__(self, h_banks, S, b0, tau_crit=None, k_d=None, k_E=None,
                        f_stickiness=0., k_n_noncohesive=0.,
                        Parker_epsilon=0.2, intermittency=1.,
-                       D=None):
+                       D=None, tau_star_crit_sed=0.0495):
 
         # Starting values (None) -- D in this too, but set in inputs
         self.channel_n = None
         self.tau_crit_sed = None
         #self.u_star_crit_sed = None
         
         # Input variables
@@ -44,15 +44,15 @@
         self.bi = self.b[-1]
 
         # Constants
         self.g = 9.807
         self.rho = 1000.
         self.porosity = 0.35
         # For sediment (used in bed load calculations)
-        self.tau_star_crit_sed = 0.0495 # Wong & Parker (2006): sediment grains
+        self.tau_star_crit_sed = tau_star_crit_sed # Default: Wong & Parker 06
         self.rho_s = 2650. # Quartz assumed
         self.SECONDS_IN_DAY = 86400
 
         # Derived constants
         if self.D is not None:
             self.tau_crit_sed = self.tau_star_crit_sed * \
                                   ( (self.rho_s - self.rho) * self.g * self.D)
@@ -79,20 +79,20 @@
         # (Equals 1/(1+self.Parker_epsilon) * bed shear stress)
         self.tau_bank_series = [np.nan]
 
     def dynamic_time_step(self, max_fract_to_equilib=0.1):
         # Currently part of a big, messy "update" step
         pass
 
-    def initialize_flow_calculations(self, channel_n, fp_k, fp_P ):
+    def initialize_flow_calculations(self, channel_n, fp_k, fp_P, use_Rh ):
         """
         Hard-code for double Manning
         """
         self.channel_n = channel_n
-        self.hclass = FlowDepthDoubleManning()
+        self.hclass = FlowDepthDoubleManning(use_Rh)
         self.hclass.initialize( channel_n, fp_k, fp_P,
                                 self.h_banks, self.b[-1], self.S)
 
 
     def initialize_timeseries(self, t, Q):
         self.t = list(t)
         self.Q = list(Q)
@@ -141,16 +141,17 @@
         minimal organic/cohesive matter.
         """
 
         # Inefficient but complete: compute both and compare.
         # That is, unless D is not set, in which case, a fully cohesive system
         # is assumed
         
-        # If not specified to evolve via bedload
-        if self.D is None:
+        # If not specified to evolve via bed load:
+        # No grain size and/or no erosional coefficient
+        if (self.D is None) or (self.k_E is None):
             self.db_widening = self.widen_cohesive()
             self.db_widening_cohesive_control.append( True )
         # Else if not specified to evolve via suspended load
         elif self.tau_crit is None:
             self.db_widening = self.widen_noncohesive()
             self.db_widening_cohesive_control.append( False )
         # Otherwise, use rate-limiting one of the both
@@ -198,81 +199,124 @@
     def widen_noncohesive(self):
         """
         Widening set by sediment entrainment that is proportional to
         (tau* - tau*_c).
         All entrained sediment tumbles to the channel bed, where tau* is
         higher and the sediment is transported away.
         """
-        #print("Noncohesive_control")
-        # Tau*
-        self.tau_star_bank = self.tau_bank / ( (self.rho_s - self.rho) *
-                                                self.g * self.D )
 
         if self.tau_star_bank > self.tau_star_crit_sed:
             # We assume the bank shape of Parker (1978), which is plausible
             # and allows the entire bank region to experience
             # the exact same shear stress regardless of flow depth.
             # We unexactly but not so unrealistically assume that this
             # shape is similar regardless of the flow depth.
             
             # 2* because erosion & deposition are symmetrical across banks
 
             # Incorporate symmetry, porosity, and (if a full hydrograph is
             # not being used) intermittency
             # Note: Porosity here but not in cohesive case (via convention
             # of empirical shear--detachment rule used there)
+            
+            # Overall general form (h<=h_banks):
+            # 3.6 K h/h_banks (tau*-tau*_c) D/t_flight
+            # 3.6 --> pi/4 * 4.6: coefficient for bed-sediment concentration
+            # K --> coefficient; how many hops down bank? unconsidered terms?
+            # h/h_banks --> length of erosion compared to total length to erode
+            # D --> Erosional distance scale from one grain being removed
+            # t_flight --> Length of time in transport; scales relationship
+            #              between concentration and detachment rate
+            #              (longer flight time --> lower detachment rate
+            #              required to attain concentration)
+
+            # WHAT TO DO IF CONC > 1?
+            
+            t_flight = 10.6 * (self.D / 
+                                ( (self.rho_s - self.rho)/self.rho)
+                                * self.g )**.5
             if self.h < self.h_banks:
-                db_widening = 2 * self.k_E * self.h/self.h_banks \
+                db_widening = 2 * 3.6 * self.k_E * self.h/self.h_banks \
                            * ( self.tau_star_bank - self.tau_star_crit_sed ) \
                            * self.D \
+                           / t_flight \
                            * self.dt * self.intermittency \
                            / (1 - self.porosity)
             else:
-                db_widening = 2 * self.k_E \
+                db_widening = 2 * 3.6 * self.k_E \
                            * ( self.tau_star_bank - self.tau_star_crit_sed ) \
                            * self.D \
+                           / t_flight \
                            * self.dt * self.intermittency \
                            / (1 - self.porosity)
         # Otherwise, no erosion
         else:
             db_widening = 0.
 
         return db_widening
         
-    def narrow_suspended_load(self, recompute_utkh=False):
-        if recompute_utkh == True:
-            self.compute__u_star__tau_bed()
-            self.K_Ey = 0.13 * h * self.u_star_bed
+    def narrow_suspended_load(self):
         # Narrowing -- flipped sign convention of conc diff (so no $-$ needed)
         qsy = self.f_stickiness * self.K_Ey * \
                 self.sed_conc_diff__suspended_load()
         return 2*qsy*self.dt / ( (1-self.porosity) * self.h_banks )
 
-    def narrow_bed_load(self, recompute_utk=False):
-        # Requires grain size for both concentration difference
-        # (handled elsewhere: becomes 0 if D not set)
-        # and for thickness of layer in motion
-        # No bed-load narrowing if not a system with bed load
+    def narrow_bed_load(self):
+        """
+        Lateral sediment velocity is proportional to downstream sediment
+        velocity. This equation gives the bank-ward depth-integrated flux
+        and then rescales it to bank lateral position change
+        """
         if self.D is None:
             return 0
-        if recompute_utk == True:
-            self.compute__u_star__tau_bed()
-            self.K_Ey = 0.13 * h * self.u_star_bed
+        if self.tau_star_bed < self.tau_star_crit_sed:
+            return 0
         # Narrowing
-        qsy = self.k_n_noncohesive * self.K_Ey * self.D * \
-                self.sed_conc_diff__bed_load()
-        return 2*qsy*self.dt / ( (1-self.porosity) * self.h_banks )
+        # Overall: bankward - channel-ward
+        # qsby = u_{s,b}/4 * 3.6 (tau*_b-tau^*_c)/2 * (2/3)D
+        # Channel to bank
+        usx_ch = 4.4 * (self.u_star_bed - self.u_star_crit_sed) \
+                    + 0.11 * ((self.rho_s - self.rho)/self.rho)**.5 \
+                    * self.g**.5 * self.D**.5
+        f_Am_ch = np.min( 
+                    ( 3.6 * (self.tau_star_bed - self.tau_star_crit_sed),
+                    1.) )
+        # f_Am_ch/2. is because half of the sediment goes in each direction
+        qsy_ch = usx_ch/4. * f_Am_ch/2. * 2/3.*self.D
+        # Bank to channel
+        if self.u_star_bank < self.u_star_crit_sed:
+            qsy_bank = 0
+        else:
+            usx_bank = 4.4 * (self.u_star_bank - self.u_star_crit_sed) \
+                        + 0.11 * ((self.rho_s - self.rho)/self.rho)**.5 \
+                        * self.g**.5 * self.D**.5
+            f_Am_bank = np.min( 
+                            ( 3.6 * (self.tau_star_bank - self.tau_star_crit_sed),
+                            1.) )
+            qsy_bank = usx_bank/4. * f_Am_bank/2. * 2/3.*self.D
+        # Together, net bankward transport
+        qsy = qsy_ch - qsy_bank
+        # Return effect on banks.
+        # Multiplied by two: Both sides
+        # Amplified by porosity in banks
+        # Reduced by bank height (conversion to lateral rate of motion)
+        return self.k_n_noncohesive \
+                  *2*qsy*self.dt / ( (1-self.porosity) * self.h_banks )
 
-    def compute__u_star__tau_bed(self):
+    def compute__u_star__tau__K_Ey(self):
         self.u_star_bank = (self.tau_bank / self.rho)**.5
+        if self.D is not None:
+            self.tau_star_bank = self.tau_bank / ( (self.rho_s - self.rho) *
+                                                    self.g * self.D )
         self.tau_bed = self.tau_bank * (1 + self.Parker_epsilon)
         self.u_star_bed = (self.tau_bed / self.rho)**.5
         if self.D is not None:
             self.tau_star_bed = self.tau_bed / \
-                            ( (self.rho_s - self.rho)**.5 * self.g * self.D )
+                            ( (self.rho_s - self.rho) * self.g * self.D )
+        self.K_Ey = 0.13 * self.h * self.u_star_bed
 
     def narrow(self):
         """
         Narrow based turbulent diffusion of sediment towards the banks
         (easy to visualize for suspended load; more of a discrete Brownian
         process for bed load)
         
@@ -297,15 +341,14 @@
             # (2003) "Predicting Transverse Turbulent Diffusivity in Straight
             # Alluvial Rivers"
             # This is probably assuming that h < (b/2) or something
             # 
             # K_Ey Should also scale with lateral velocity variability that
             # moves bedload from side to side
             # This could be good to revisit experimentally
-            self.compute__u_star__tau_bed()
             self.K_Ey = 0.13 * self.h * self.u_star_bed
 
             # Noncohesive (bed load) + cohesive (suspended load)
             self.db_narrowing = self.narrow_bed_load() + \
                                 self.narrow_suspended_load()
             
         # Record narrowing rate
@@ -412,53 +455,26 @@
             return ( 1 - (1/(1+self.Parker_epsilon))**(7/4.) ) \
                     * (self.g * self.h_banks * self.S)**(3.5/2.) \
 
         # (later)
         # Concentration gradient calcualted over min(h, h_beta):
         # This sets distance from banks over which side-wall drag is important
 
-
-
-    def sed_conc_diff__bed_load(self):
-        #print("BEDLOAD")
-        # Early exit if no grain size specified: no bed load desired
-        if self.D is None or self.tau_star_crit_sed is None:
-            return 0
-        # Sediment concentrations / exit early if no change needed
-        if self.tau_star_bed < self.tau_star_crit_sed:
-            # If no sediment transport, no narrowing
-            return 0
-        # Otherwise, continuing
-        # Radice: primarily concentration difference, with velocity
-        # approximately constant.
-        # Suspended sediment: 1x u* for velocity, and the rest for
-        # concentration (then integrate over depth if qs desired)
-        # (which it isn't, here)
-        # Similarly I posit, u* **2 --> concentration
-        #                    u*     --> velocity
-        # for u* **3 total in relationship (w/ critical stress, of course)
-        sed_conc_center_prop = (self.tau_star_bed - self.tau_star_crit_sed)**2
-        if self.u_star_bank < self.tau_star_crit_sed:
-            sed_conc_edge_prop = 0.
-        else:
-            sed_conc_edge_prop = (self.tau_star_bank - self.tau_star_crit_sed)**2
-                
-        # sed_conc_diff_prop
-        return (sed_conc_center_prop - sed_conc_edge_prop)
-
-
     def update(self, dt, Qi, max_fract_to_equilib=0.1):
         """
         Euler forward wtih dynamic inner-loop time stepping
         Only widening; no narrowing
         """
         dt_outer = dt
         bi_outer = self.b[-1]
         self.hclass.set_b( bi_outer )
         h = self.hclass.compute_depth( Qi )
+        # Use depth, not hydraulic radius, because the Parker_eposilon
+        # factor is intended to convert the channel-centerline stress 
+        # into a near-bank stress.
         self.tau_bank = self.rho * self.g * h * self.S / (1 + self.Parker_epsilon)
         # Record tau_bank in its series
         # Record narrowing rate
         if self.tau_bank > self.tau_crit:
             self.bi = self.b[-1]
             dt_remaining = dt
             while dt_remaining != 0:
@@ -498,14 +514,16 @@
         self.dt = dt
         # Current discharge and shear stress
         # Is this updated for the rating-curve 2x Manning approach?
         h = self.hclass.compute_depth( Qi )
         self.tau_bank = self.rho * self.g * h * self.S \
                 / (1 + self.Parker_epsilon)
         self.h = h # For the widening, at least for now
+        # Update variables needed for computations
+        self.compute__u_star__tau__K_Ey()
         # Compute widening
         self.widen()
         #self.b.append(self.bi + self.db_widening)
         self.narrow()
         self.h_series.append(h) # h is based on previous b but associated with
                                 # the discharge that created current b
         self.b.append(self.bi + self.db_widening - self.db_narrowing)
@@ -577,19 +595,25 @@
         self.db_dt__day__widening_series = self.db_widening_series / dt_days
         self.db_dt__day__narrowing_series = self.db_narrowing_series / dt_days
 
     def plotb(self):
         """
         Plot channel width over time
         """
+        # Manage typing of time stamp for plotting
+        # Required with newer Pandas
+        if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
+            _t = self.t
+        else:
+            _t = list(np.array(self.t)/86400.)
         #b_eq = self.get_equilibriumWidth(self.Qi)
         plt.figure()
         #plt.hlines(b_eq, self.t[0], self.t[-1]/86400.,
         #           '.5', label='Equilibrium width', linewidth=2)
-        plt.plot(self.t/86400., self.b, 'k-', label='Transient width',
+        plt.plot(_t, self.b, 'k-', label='Transient width',
                  linewidth=2)
         plt.xlabel('Time [days of flood]')
         plt.ylabel('Channel width [m]')
         #plt.legend(loc='lower right')
         plt.tight_layout()
         plt.show()
         
@@ -613,68 +637,68 @@
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             ax2.set_xlabel('Date', fontsize=16)
         else:
             ax2.set_xlabel('Days since start', fontsize=16)
         plt.tight_layout()
         plt.show()
         
-    def plotWideningNarrowingStress(self):
+    def plotWideningNarrowingStress(self, legend_loc=None):
         """
         Plot rates of widening and narrowing alongside bank stress
         """
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             _t = self.t
         else:
             _t = list(np.array(self.t)/86400.)
         plt.figure(figsize=(12,8))
         ax1 = plt.subplot(2,1,1)
         ax2 = plt.subplot(2,1,2)
         ax1.plot(_t, self.db_dt__day__widening_series, 'k-', linewidth=2, label='Widening')
-        ax1.plot(_t, self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
-        ax1.legend()
+        ax1.plot(_t, -self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
+        ax1.legend(loc=legend_loc, fontsize=12)
         ax1.set_ylabel('Channel width\nchange rate [m/day]', fontsize=16)
         ax2.plot(_t, self.tau_bank_series, 'k-', linewidth=2)
         ax2.set_ylabel('Bank shear stress [Pa]', fontsize=16)
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             ax2.set_xlabel('Date', fontsize=16)
         else:
             ax2.set_xlabel('Days since start', fontsize=16)
         plt.tight_layout()
         plt.show()
         
-    def plotWidthWideningNarrowingStress(self):
+    def plotWidthWideningNarrowingStress(self, legend_loc=None):
         """
         Plot width and rates of widening and narrowing alongside bank stress
         """
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             _t = self.t
         else:
             _t = list(np.array(self.t)/86400.)
         plt.figure(figsize=(8,8))
         ax1 = plt.subplot(3,1,1)
         ax2 = plt.subplot(3,1,2)
         ax3 = plt.subplot(3,1,3)
         ax1.plot(_t, self.b, 'k-', linewidth=2)
         ax1.set_ylabel('Channel width [m]', fontsize=12)
         ax2.plot(_t, self.db_dt__day__widening_series, 'k-', linewidth=2, label='Widening')
-        ax2.plot(_t, self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
-        ax2.legend()
+        ax2.plot(_t, -self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
+        ax2.legend(loc=legend_loc, fontsize=12)
         ax2.set_ylabel('Channel width\nchange rate [m/day]', fontsize=12)
         ax3.plot(_t, self.tau_bank_series, 'k-', linewidth=2)
         ax3.plot( [_t[0], _t[-1]] , [self.tau_crit, self.tau_crit], '--', 
                    color='.5', linewidth=1)
         ax3.set_ylabel('Bank shear stress [Pa]', fontsize=12)
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             ax3.set_xlabel('Date', fontsize=16)
         else:
             ax3.set_xlabel('Days since start', fontsize=16)
         plt.tight_layout()
         plt.show()
         
-    def plotDischargeWidthWideningNarrowingStress(self):
+    def plotDischargeWidthWideningNarrowingStress(self, legend_loc=None):
         """
         Plot discharge, width, and rates of widening and narrowing alongside
         bank stress
         """
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             _t = self.t
         else:
@@ -685,29 +709,29 @@
         ax2 = plt.subplot(4,1,3)
         ax3 = plt.subplot(4,1,4)
         ax0.plot(_t, self.Q, 'k-', linewidth=2)
         ax0.set_ylabel('River discharge [m$^3$/s]', fontsize=12)
         ax1.plot(_t, self.b, 'k-', linewidth=2)
         ax1.set_ylabel('Channel width [m]', fontsize=12)
         ax2.plot(_t, self.db_dt__day__widening_series, 'k-', linewidth=2, label='Widening')
-        ax2.plot(_t, self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
-        ax2.legend()
+        ax2.plot(_t, -self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
+        ax2.legend(loc=legend_loc, fontsize=12)
         ax2.set_ylabel('Channel width\nchange rate [m/day]', fontsize=12)
         ax3.plot(_t, self.tau_bank_series, 'k-', linewidth=2)
         ax3.plot( [_t[0], _t[-1]] , [self.tau_crit, self.tau_crit], '--', 
                    color='.5', linewidth=1)
         ax3.set_ylabel('Bank shear stress [Pa]', fontsize=12)
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             ax3.set_xlabel('Date', fontsize=16)
         else:
             ax3.set_xlabel('Days since start', fontsize=16)
         plt.tight_layout()
         plt.show()
         
-    def plotDischargeWidthWideningNarrowingGrainstressratio(self):
+    def plotDischargeWidthWideningNarrowingGrainstressratio(self, legend_loc=None):
         """
         Plot discharge, width, and rates of widening and narrowing alongside
         bank stress divided by critical stress to move particles
         """
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             _t = self.t
         else:
@@ -718,16 +742,16 @@
         ax2 = plt.subplot(4,1,3)
         ax3 = plt.subplot(4,1,4)
         ax0.plot(_t, self.Q, 'k-', linewidth=2)
         ax0.set_ylabel('River discharge [m$^3$/s]', fontsize=12)
         ax1.plot(_t, self.b, 'k-', linewidth=2)
         ax1.set_ylabel('Channel width [m]', fontsize=12)
         ax2.plot(_t, self.db_dt__day__widening_series, 'k-', linewidth=2, label='Widening')
-        ax2.plot(_t, self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
-        ax2.legend()
+        ax2.plot(_t, -self.db_dt__day__narrowing_series, '-', color='.5', linewidth=2, label='Narrowing')
+        ax2.legend(loc=legend_loc, fontsize=12)
         ax2.set_ylabel('Channel width\nchange rate [m/day]', fontsize=12)
         ax3.plot(_t, np.array(self.tau_bank_series)/self.tau_crit_sed, 'k-', linewidth=2)
         ax3.plot( [_t[0], _t[-1]] , [1, 1], '--', 
                    color='.5', linewidth=1)
         ax3.set_ylabel('Ratio: Bank stress \n/ critical stress', fontsize=12)
         if type(self.t[0]) == pd._libs.tslibs.timestamps.Timestamp:
             ax3.set_xlabel('Date', fontsize=16)
@@ -756,16 +780,17 @@
 from scipy.optimize import fsolve
 
 class FlowDepthDoubleManning( object ):
     """
     Use Manning's equation to obtain flow depth from river discharge,
     using a conversion from ManningFit.py outputs
     """
-    def __init__(self):
-        pass
+    def __init__(self, use_Rh):
+        # Default to using hyraulic radius and not just depth
+        self.use_Rh = use_Rh
 
     def set_n(self, _var):
         self.n = _var
 
     def set_k(self, _var):
         self.k = _var
 
@@ -781,16 +806,21 @@
     def set_S(self, _var):
         self.S = _var
 
     def set_Q(self, _var):
         self.Q = _var
 
     def flow_depth_from_Manning_discharge( self, h ):
+        # Does the flow go overbank?
         ob = h > self.h_bank
-        return self.b/self.n * h**(5/3.) * self.S**0.5 \
+        if self.use_Rh:
+            _r = h*self.b / (2*h + self.b)
+        else:
+            _r = h
+        return self.b/self.n * _r**(5/3.) * self.S**0.5 \
                   + ob*self.k*(h-self.h_bank)**(ob*self.P) - self.Q
 
     def compute_depth(self, Q=None):
         if Q is not None:
             self.Q = Q
         if Q == 0:
             return 0
@@ -817,7 +847,8 @@
         Not exactly running anything, but to follow standard CSDMS I(U)RF
         Same as "update" step
         """
         return self.update(Q)
 
     def finalize(self):
         pass
+
```

### Comparing `OTTAR-0.4.0/setup.py` & `OTTAR-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OTTAR",
-    version="0.4.0",
+    version="0.5.0",
     author="Andrew D. Wickert",
     author_email="awickert@umn.edu",
     description="Ode To Transient Ancho de los Rivers: Transient evolution of river-channel width",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MNiMORPH/ottar",
     install_requires=[
```

