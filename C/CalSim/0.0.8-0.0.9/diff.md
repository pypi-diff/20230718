# Comparing `tmp/calsim-0.0.8.tar.gz` & `tmp/calsim-0.0.9.tar.gz`

## Comparing `calsim-0.0.8.tar` & `calsim-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/__init__.py
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/control.py
--rwxr-xr-x   0        0        0     6022 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/controller.py
--rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/depth_cam.py
--rwxr-xr-x   0        0        0    23005 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/dynamics.py
--rwxr-xr-x   0        0        0     6118 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/environment.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/exceptions.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/manipulator.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/obstacle.py
--rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/run_simulation.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/sim_utils.py
--rwxr-xr-x   0        0        0     7878 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/state_estimation.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/tests.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/transforms.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/twist.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/tests/test_double_pend.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/tests/test_planar_qrotor.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 calsim-0.0.8/tests/test_double_pend.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.8/tests/test_simulation_simple.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.8/LICENSE
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 calsim-0.0.8/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 calsim-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/__init__.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/control.py
+-rwxr-xr-x   0        0        0     6240 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/controller.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/depth_cam.py
+-rwxr-xr-x   0        0        0    23005 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/dynamics.py
+-rwxr-xr-x   0        0        0     6118 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/environment.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/exceptions.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/manipulator.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/obstacle.py
+-rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/run_simulation.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/sim_utils.py
+-rwxr-xr-x   0        0        0     7878 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/state_estimation.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/tests.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/transforms.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/core/twist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/tests/test_depth_cam.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/tests/test_double_pend.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 calsim-0.0.9/src/CalSim/tests/test_planar_qrotor.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.9/LICENSE
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 calsim-0.0.9/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 calsim-0.0.9/PKG-INFO
```

### Comparing `calsim-0.0.8/src/CalSim/core/control.py` & `calsim-0.0.9/src/CalSim/core/control.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/controller.py` & `calsim-0.0.9/src/CalSim/core/controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import numpy as np
 from .state_estimation import *
 
 """
 File containing controllers 
 """
 class Controller:
-    def __init__(self, observer, lyapunovBarrierList = None, trajectory = None, uBounds = None):
+    def __init__(self, observer, lyapunovBarrierList = None, trajectory = None, depthCam = None):
         """
         Skeleton class for feedback controllers
         Args:
             observer (Observer): state observer object
             lyapunov (List of LyapunovBarrier): list of LyapunovBarrier objects
             trajectory (Trajectory): trajectory for the controller to track (could just be a constant point!)
-            uBounds ((Dynamics.singleInputDimn x 2) numpy array): minimum and maximum input values to the system
+            depthCam (PlanarDepthCam or Lidar): depth camera object
         """
         #store input parameters
         self.observer = observer
         self.lyapunovBarrierList = lyapunovBarrierList
         self.trajectory = trajectory
-        self.uBounds = uBounds
         
         #store input
         self._u = np.zeros((self.observer.singleInputDimn, 1))
     
     def eval_input(self, t):
         """
         Solve for and return control input
@@ -42,55 +41,59 @@
         """
         return self._u
     
 class FFController(Controller):
     """
     Class for a simple feedforward controller.
     """
-    def __init__(self, observer, lyapunovBarrierList = None, trajectory = None, uBounds = None):
+    def __init__(self, observer, lyapunovBarrierList = None, trajectory = None, depthCam = None):
         """
         Init function for a ff controller
         Args:
             observer (Observer): state observer object
             ff (NumPy Array): constant feedforward input to send to system
             lyapunov (List of LyapunovBarrier): list of LyapunovBarrier objects
             trajectory (Trajectory): trajectory for the controller to track (could just be a constant point!)
-            uBounds ((Dynamics.singleInputDimn x 2) numpy array): minimum and maximum input values to the system
         """
         self.ff = np.array([[9.81*0.92, 0]]).T
-        super().__init__(observer, lyapunovBarrierList, trajectory, uBounds)
+        self.depthCam = depthCam
+        super().__init__(observer, lyapunovBarrierList, trajectory)
     
     def eval_input(self, t):
         """
         Solve for and return control input
         Inputs:
             t (float): time in simulation
         Returns:
             u ((Dynamics.singleInputDimn x 1)): input vector, as determined by controller
         """
+        if self.depthCam is not None:
+            #test the depth camera
+            self.depthCam.get_pointcloud()
+
         self._u = self.ff
         return self._u
 
 class ControllerManager(Controller):
-    def __init__(self, observerManager, ControlType, barrierManager = None, trajectoryManager = None, lidarManager = None):
+    def __init__(self, observerManager, ControlType, barrierManager = None, trajectoryManager = None, depthManager = None):
         """
         Managerial class that points to N controller instances for the system. Interfaces
         directly with the overall system dynamics object.
         Args:
             observerManager (ObserverManager)
             barrierManager (BarrierManager)
             trajectoryManager (TrajectoryManager)
-            lidarManager (LidarManager)
+            depthManager (LidarManager or DepthManager)
             ControlType (Class Name): Name of a class for a controller
         """
         #store input parameters
         self.observerManager = observerManager
         self.barrierManager = barrierManager
         self.trajectoryManager = trajectoryManager
-        self.lidarManager = lidarManager
+        self.depthManager = depthManager
         self.ControlType = ControlType
 
         #store the input parameter (should not be called directly but with get_input)
         self._u = None
 
         #get the number of agents in the system
         self.N = self.observerManager.dynamics.N
@@ -117,16 +120,23 @@
             #get the ith barrier object
             try:
                 barrierI = self.barrierManager.get_barrier_list_i(i)
             except:
                 print("No barrier/lyapunov object passed in.")
                 barrierI = None
 
+            #get the ith depth camera object
+            try:
+                depthI = self.depthManager.get_depth_cam_i(i)
+            except:
+                print("No depth camera/LIDAR object passed in.")
+                depthI = None
+
             #create a controller of the specified type
-            self.controllerDict[i] = self.ControlType(egoObsvI, barrierI, trajI)
+            self.controllerDict[i] = self.ControlType(egoObsvI, barrierI, trajI, depthI)
 
     def eval_input(self, t):
         """
         Solve for and return control input for all N agents. Solves for the input ui to 
         each agent in the system and assembles all of the input vectors into a large 
         input vector for the entire system.
         Inputs:
```

### Comparing `calsim-0.0.8/src/CalSim/core/depth_cam.py` & `calsim-0.0.9/src/CalSim/core/depth_cam.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         #store an attribute for the number of points to be sampled per obstacle
         self.numPts = 1000//self.obstacleManager.NumObs
 
         #store an attribute for the pointcloud data
         self._ptcloudData = {}
 
-    def calc_pointcloud_world(self):
+    def calc_ptcloud_world(self):
         """
         Calculate the pointcloud of the environment using the obstalce manager
         This is calculated in the world frame. As this is a planar camera
         the x coordinate is always zero - pointcloud is generated in YZ plane.
         Inputs:
             None
         Returns:
@@ -55,17 +55,17 @@
 
             #calculate a sample of points on the obstacle in the YZ plane
             for j in range(self.numPts):
                 #calculate an angle theta to sample around the circle
                 thetaJ = j*2*np.pi/self.numPts
 
                 #calculate each coordinate
-                self.xList.append(0)
-                self.yList.append(qCenter[1, 0] + r*np.cos(thetaJ))
-                self.zList.append(qCenter[2, 0] + r*np.sin(thetaJ))
+                xList.append(0)
+                yList.append(qCenter[1, 0] + r*np.cos(thetaJ))
+                zList.append(qCenter[2, 0] + r*np.sin(thetaJ))
 
         #assemble and return the pointcloud in the world frame
         return np.array([xList, yList, zList])
     
     def compute_rotation(self, theta):
         """
         Compute the rotation matrix from the quadrotor frame to the world frame
@@ -75,30 +75,30 @@
             Rsq: rotation matrix between spatial and quadrotor frames
         """
         Rsq = np.array([[1, 0, 0], 
                         [0, np.cos(theta), -np.sin(theta)], 
                         [0, np.sin(theta), np.cos(theta)]])
         return Rsq
     
-    def calc_pointcloud(self):
+    def calc_ptcloud(self):
         """
         Calculates the pointcloud in the frame of quadrotor i, updates the 
         self._ptcloudData attribute.
         """
         #use the observer to get the position and angle
         state = self.observer.get_state() #(x, y, z, theta, x_dot, y_dot, z_dot, theta_dot)
 
         #get position and angle of the quadrotor
         q, theta = state[0:3].reshape((3, 1)), state[3, 0]
 
         #compute rotation matrix to spatial frame
         Rsq = self.compute_rotation(theta)
 
         #compute pointcloud in world frame
-        ptcloudWorld = self.calc_pointcloud_world()
+        ptcloudWorld = self.calc_ptcloud_world()
 
         #transform pointcloud
         ptcloudQrotor = Rsq.T @ (ptcloudWorld - q)
 
         #store in the pointcloud attribute
         self._ptcloudData["ptcloud"] = ptcloudQrotor
         self._ptcloudData["stateVec"] = q
```

### Comparing `calsim-0.0.8/src/CalSim/core/dynamics.py` & `calsim-0.0.9/src/CalSim/core/dynamics.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/environment.py` & `calsim-0.0.9/src/CalSim/core/environment.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/manipulator.py` & `calsim-0.0.9/src/CalSim/core/manipulator.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/obstacle.py` & `calsim-0.0.9/src/CalSim/core/obstacle.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/sim_utils.py` & `calsim-0.0.9/src/CalSim/core/sim_utils.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/state_estimation.py` & `calsim-0.0.9/src/CalSim/core/state_estimation.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/transforms.py` & `calsim-0.0.9/src/CalSim/core/transforms.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/core/twist.py` & `calsim-0.0.9/src/CalSim/core/twist.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/src/CalSim/tests/test_double_pend.py` & `calsim-0.0.9/src/CalSim/tests/test_double_pend.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/LICENSE` & `calsim-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/README.md` & `calsim-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `calsim-0.0.8/pyproject.toml` & `calsim-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CalSim"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Massimiliano de Sa", email="mz.desa@berkeley.edu" },
 ]
 description = "Simulator package for Berkeley robotics course."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calsim-0.0.8/PKG-INFO` & `calsim-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSim
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simulator package for Berkeley robotics course.
 Project-URL: Homepage, https://github.com/mzdesa/CalSim
 Project-URL: Bug Tracker, https://github.com/mzdesa/CalSim
 Author-email: Massimiliano de Sa <mz.desa@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

