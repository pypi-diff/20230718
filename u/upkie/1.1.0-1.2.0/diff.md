# Comparing `tmp/upkie-1.1.0.tar.gz` & `tmp/upkie-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkie-1.1.0.tar", last modified: Fri Jul  7 10:12:08 2023, max compression
+gzip compressed data, was "upkie-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `upkie-1.1.0.tar` & `upkie-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     8466 2023-07-07 10:12:07.583809 upkie-1.1.0/README.md
--rw-r--r--   0        0        0     1909 2023-07-07 10:12:07.579809 upkie-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      695 2023-07-07 10:12:07.579809 upkie-1.1.0/upkie/__init__.py
--rw-r--r--   0        0        0     1084 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/BUILD
--rw-r--r--   0        0        0     1236 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/__init__.py
--rw-r--r--   0        0        0     2809 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/standing_reward.py
--rw-r--r--   0        0        0      549 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/BUILD
--rw-r--r--   0        0        0     2530 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/upkie_base_env_test.py
--rw-r--r--   0        0        0     2446 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/upkie_servos_env_test.py
--rw-r--r--   0        0        0     2330 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/upkie_wheels_env_test.py
--rw-r--r--   0        0        0     8703 2023-07-07 10:12:07.559810 upkie-1.1.0/upkie/envs/upkie_base_env.py
--rw-r--r--   0        0        0     7363 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/upkie_servos_env.py
--rw-r--r--   0        0        0     6573 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/upkie_wheels_env.py
--rw-r--r--   0        0        0      327 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/BUILD
--rw-r--r--   0        0        0      822 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/__init__.py
--rw-r--r--   0        0        0     5477 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/base_pitch.py
--rw-r--r--   0        0        0      305 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/tests/BUILD
--rw-r--r--   0        0        0     3105 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/tests/base_pitch_test.py
--rw-r--r--   0        0        0     1081 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/BUILD
--rw-r--r--   0        0        0     1896 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/clamp.py
--rw-r--r--   0        0        0     1137 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/datetime_now_string.h
--rw-r--r--   0        0        0      803 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/exceptions.py
--rw-r--r--   0        0        0     2820 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/filters.py
--rw-r--r--   0        0        0     2433 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/pinocchio.py
--rw-r--r--   0        0        0     1231 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/realtime.py
--rw-r--r--   0        0        0     1983 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/spdlog.py
--rw-r--r--   0        0        0      634 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/BUILD
--rw-r--r--   0        0        0     1303 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/clamp_test.py
--rw-r--r--   0        0        0      986 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/datetime_now_string_test.cpp
--rw-r--r--   0        0        0     2232 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/pinocchio_test.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 upkie-1.1.0/setup.py
--rw-r--r--   0        0        0     9927 1970-01-01 00:00:00.000000 upkie-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     8466 2023-07-18 17:10:44.858627 upkie-1.2.0/README.md
+-rw-r--r--   0        0        0     1890 2023-07-18 17:10:44.858627 upkie-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/__init__.py
+-rw-r--r--   0        0        0     1090 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/BUILD
+-rw-r--r--   0        0        0     1275 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/__init__.py
+-rw-r--r--   0        0        0     2809 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/standing_reward.py
+-rw-r--r--   0        0        0      549 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/tests/BUILD
+-rw-r--r--   0        0        0     2530 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/tests/upkie_base_env_test.py
+-rw-r--r--   0        0        0     2446 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/tests/upkie_servos_env_test.py
+-rw-r--r--   0        0        0     2330 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/tests/upkie_wheels_env_test.py
+-rw-r--r--   0        0        0     8982 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/upkie_base_env.py
+-rw-r--r--   0        0        0     7387 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/upkie_servos_env.py
+-rw-r--r--   0        0        0     7085 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/envs/upkie_wheels_env.py
+-rw-r--r--   0        0        0      356 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/observers/base_pitch/BUILD
+-rw-r--r--   0        0        0      902 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/observers/base_pitch/__init__.py
+-rw-r--r--   0        0        0     5612 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/observers/base_pitch/base_pitch.py
+-rw-r--r--   0        0        0      305 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/observers/base_pitch/tests/BUILD
+-rw-r--r--   0        0        0     3105 2023-07-18 17:10:44.854627 upkie-1.2.0/upkie/observers/base_pitch/tests/base_pitch_test.py
+-rw-r--r--   0        0        0     1171 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/BUILD
+-rw-r--r--   0        0        0     1896 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/clamp.py
+-rw-r--r--   0        0        0     1137 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/datetime_now_string.h
+-rw-r--r--   0        0        0      803 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/exceptions.py
+-rw-r--r--   0        0        0     2820 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/filters.py
+-rw-r--r--   0        0        0     2433 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/pinocchio.py
+-rw-r--r--   0        0        0     1207 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/realtime.py
+-rw-r--r--   0        0        0     1900 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/rotations.py
+-rw-r--r--   0        0        0     1983 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/spdlog.py
+-rw-r--r--   0        0        0      634 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/tests/BUILD
+-rw-r--r--   0        0        0     1303 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/tests/clamp_test.py
+-rw-r--r--   0        0        0      986 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/tests/datetime_now_string_test.cpp
+-rw-r--r--   0        0        0     2232 2023-07-18 17:10:44.858627 upkie-1.2.0/upkie/utils/tests/pinocchio_test.py
+-rw-r--r--   0        0        0     9900 1970-01-01 00:00:00.000000 upkie-1.2.0/PKG-INFO
```

### Comparing `upkie-1.1.0/README.md` & `upkie-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/pyproject.toml` & `upkie-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,20 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "gym >=0.21.0",
+    "gymnasium >=0.28.1",
     "loop-rate-limiters >=0.4.0",
     "mpacklog >=3.0.0",
     "numpy >=1.22.0",
-    "qpsolvers >=1.9.1",
     "upkie_description >=1.2.0",
-    "vulp >=1.1.1",
+    "vulp >=1.2.1",
 ]
 keywords = ["wheeled", "biped", "robot", "balance", "motion", "control", "robotics"]
 
 [project.urls]
 Documentation = "https://tasts-robots.org/doc/upkie/"
 Source = "https://github.com/tasts-robots/upkie"
 Tracker = "https://github.com/tasts-robots/upkie/issues"
```

### Comparing `upkie-1.1.0/upkie/__init__.py` & `upkie-1.2.0/upkie/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python module to control Upkie wheeled bipeds."""
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
```

### Comparing `upkie-1.1.0/upkie/envs/BUILD` & `upkie-1.2.0/upkie/envs/BUILD`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     srcs = [
         "standing_reward.py",
         "upkie_base_env.py",
     ],
     deps = [
         "@upkie//observers/base_pitch",
         "@vulp//spine:python",
-        requirement("gym"),
+        requirement("gymnasium"),
         requirement("loop_rate_limiters"),
         requirement("pyyaml"),
         requirement("upkie_description"),
     ],
 )
 
 py_library(
```

### Comparing `upkie-1.1.0/upkie/envs/__init__.py` & `upkie-1.2.0/upkie/envs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import gym
+import gymnasium as gym
 
 from .upkie_base_env import UpkieBaseEnv
 from .upkie_servos_env import UpkieServosEnv
 from .upkie_wheels_env import UpkieWheelsEnv
 
 
 def register():
-    gym.envs.register(
+    gym.envs.registration.register(
         id=f"UpkieServosEnv-v{UpkieServosEnv.version}",
         entry_point="upkie.envs:UpkieServosEnv",
         max_episode_steps=1_000_000_000,
     )
-    gym.envs.register(
+    gym.envs.registration.register(
         id=f"UpkieWheelsEnv-v{UpkieWheelsEnv.version}",
         entry_point="upkie.envs:UpkieWheelsEnv",
         max_episode_steps=1_000_000_000,
     )
 
 
 __all__ = [
```

### Comparing `upkie-1.1.0/upkie/envs/standing_reward.py` & `upkie-1.2.0/upkie/envs/standing_reward.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/envs/tests/BUILD` & `upkie-1.2.0/upkie/envs/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/envs/tests/upkie_base_env_test.py` & `upkie-1.2.0/upkie/envs/tests/upkie_base_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/envs/tests/upkie_servos_env_test.py` & `upkie-1.2.0/upkie/envs/tests/upkie_servos_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/envs/tests/upkie_wheels_env_test.py` & `upkie-1.2.0/upkie/envs/tests/upkie_wheels_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/envs/upkie_base_env.py` & `upkie-1.2.0/upkie/envs/upkie_base_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 import asyncio
 from typing import Dict, Optional, Tuple, Union
 
-import gym
+import gymnasium as gym
 import numpy as np
 from loop_rate_limiters import AsyncRateLimiter, RateLimiter
 from vulp.spine import SpineInterface
 
 from upkie.observers.base_pitch import compute_base_pitch_from_imu
 
 DEFAULT_CONFIG = {
@@ -53,15 +53,15 @@
 class UpkieBaseEnv(abc.ABC, gym.Env):
 
     """!
     Base class for Upkie environments.
 
     This class has the following attributes:
 
-    - ``config``: Configuration dictionary, also sent to the spine.
+    - ``config``: Configuration dictionary sent to the spine.
     - ``fall_pitch``: Fall pitch angle, in radians.
 
     @note This environment is made to run on a single CPU thread rather than on
     GPU/TPU. The downside for reinforcement learning is that computations are
     not massively parallel. The upside is that it simplifies deployment to the
     real robot, as it relies on the same spine interface that runs on Upkie.
     """
@@ -79,15 +79,15 @@
         fall_pitch: float,
         frequency: Optional[float],
         shm_name: str,
     ) -> None:
         """!
         Initialize environment.
 
-        @param config Configuration dictionary, also sent to the spine.
+        @param config Configuration dictionary sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
         @param frequency Regulated frequency of the control loop, in Hz. Set to
             ``None`` to disable loop frequency regulation.
         @param shm_name Name of shared-memory file.
         """
         if config is None:
             config = DEFAULT_CONFIG
@@ -106,30 +106,30 @@
         """
         self._spine.stop()
 
     def reset(
         self,
         *,
         seed: Optional[int] = None,
-        return_info: bool = False,
+        return_info: bool = True,
         options: Optional[dict] = None,
     ) -> Union[np.ndarray, Tuple[np.ndarray, Dict]]:
         """!
         Resets the spine and get an initial observation.
 
-        @param seed Will be used once we upgrade to gym >= 0.21.0.
+        @param seed It is not used yet but should be. TODO(perrin-isir)
         @param return_info If true, return the dictionary observation as an
             extra info dictionary.
         @param options Currently unused.
         @returns
             - ``observation``: the initial vectorized observation.
             - ``info``: an optional dictionary containing extra information.
                 It is only returned if ``return_info`` is set to true.
         """
-        # super().reset(seed=seed)  # we are pinned at gym==0.21.0
+        # super().reset(seed=seed)
         self.__reset_rates()
         self._spine.stop()
         self._spine.start(self.config)
         self._spine.get_observation()  # might be a pre-reset observation
         observation_dict = self._spine.get_observation()
         self.parse_first_observation(observation_dict)
         observation = self.vectorize_observation(observation_dict)
@@ -145,71 +145,79 @@
             return
         try:
             asyncio.get_running_loop()
             self.__async_rate = AsyncRateLimiter(self.__frequency)
         except RuntimeError:  # not asyncio
             self.__rate = RateLimiter(self.__frequency)
 
-    def step(self, action: np.ndarray) -> Tuple[np.ndarray, float, bool, dict]:
+    def step(
+        self,
+        action: np.ndarray,
+    ) -> Tuple[np.ndarray, float, bool, bool, dict]:
         """!
         Run one timestep of the environment's dynamics. When the end of the
         episode is reached, you are responsible for calling `reset()` to reset
         the environment's state.
 
         @param action Action from the agent.
         @returns
             - ``observation``: Agent's observation of the environment.
             - ``reward``: Amount of reward returned after previous action.
-            - ``done``: Whether the agent reaches the terminal state, which can
-              be a good or a bad thing. If true, the user needs to call
-              :func:`reset()`.
+            - ``terminated``: Whether the agent reaches the terminal state,
+              which can be a good or a bad thing. If true, the user needs to
+              call :func:`reset()`.
+            - ``truncated'': Whether the episode is reaching max number of
+              steps.
             - ``info``: Contains auxiliary diagnostic information (helpful for
               debugging, logging, and sometimes learning).
         """
         action_dict = self.dictionarize_action(action)
         if self.__rate is not None:
             self.__rate.sleep()  # wait until clock tick to send the action
         return self.__step(action_dict)
 
     async def async_step(
         self, action: np.ndarray
-    ) -> Tuple[np.ndarray, float, bool, dict]:
+    ) -> Tuple[np.ndarray, float, bool, bool, dict]:
         """!
         Run one timestep of the environment's dynamics using asynchronous I/O.
         When the end of the episode is reached, you are responsible for calling
         `reset()` to reset the environment's state.
 
         @param action Action from the agent.
         @returns
             - ``observation``: Agent's observation of the environment.
             - ``reward``: Amount of reward returned after previous action.
-            - ``done``: Whether the agent reaches the terminal state, which can
-              be a good or a bad thing. If true, the user needs to call
-              :func:`reset()`.
+            - ``terminated``: Whether the agent reaches the terminal state,
+              which can be a good or a bad thing. If true, the user needs to
+              call :func:`reset()`.
+            - ``truncated'': Whether the episode is truncated (reaching max
+              number of steps).
             - ``info``: Contains auxiliary diagnostic information (helpful for
               debugging, logging, and sometimes learning).
         """
         action_dict = self.dictionarize_action(action)
         if self.__async_rate is not None:
             await self.__async_rate.sleep()  # send action at next clock tick
         return self.__step(action_dict)
 
     def __step(
         self, action_dict: dict
-    ) -> Tuple[np.ndarray, float, bool, dict]:
+    ) -> Tuple[np.ndarray, float, bool, bool, dict]:
         self._spine.set_action(action_dict)
         observation_dict = self._spine.get_observation()
         observation = self.vectorize_observation(observation_dict)
         reward = self.reward.get(observation)
-        done = self.detect_fall(observation_dict)
+        terminated = self.detect_fall(observation_dict)
+        truncated = False
         info = {
             "action": action_dict,
             "observation": observation_dict,
         }
-        return observation, reward, done, info
+        return observation, reward, terminated, truncated, info
 
     def detect_fall(self, observation_dict: dict) -> bool:
         """!
         Detect a fall based on the body-to-world pitch angle.
 
         @param observation_dict Observation dictionary with an "imu" key.
         @returns True if and only if a fall is detected.
```

### Comparing `upkie-1.1.0/upkie/envs/upkie_servos_env.py` & `upkie-1.2.0/upkie/envs/upkie_servos_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # limitations under the License.
 
 from typing import Optional
 
 import numpy as np
 import pinocchio as pin
 import upkie_description
-from gym import spaces
+from gymnasium import spaces
 
 from upkie.utils.clamp import clamp_and_warn
 from upkie.utils.pinocchio import (
     box_position_limits,
     box_torque_limits,
     box_velocity_limits,
 )
@@ -178,15 +178,15 @@
         Extract observation vector from a full observation dictionary.
 
         @param observation_dict Full observation dictionary from the spine.
         @returns Observation vector.
         """
         nq, nv = self.robot.model.nq, self.robot.model.nv
         model = self.robot.model
-        obs = np.empty(nq + 2 * nv)
+        obs = np.empty(nq + 2 * nv, dtype=np.float32)
         for joint in self.__joints:
             i = model.getJointId(joint) - 1
             obs[i] = observation_dict["servo"][joint]["position"]
             obs[nq + i] = observation_dict["servo"][joint]["velocity"]
             obs[nq + nv + i] = observation_dict["servo"][joint]["torque"]
         return obs
```

### Comparing `upkie-1.1.0/upkie/envs/upkie_wheels_env.py` & `upkie-1.2.0/upkie/envs/upkie_wheels_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,61 +16,59 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 from typing import Optional
 
 import numpy as np
-from gym import spaces
+from gymnasium import spaces
 
-from upkie.observers.base_pitch import compute_base_pitch_from_imu
+from upkie.observers.base_pitch import (
+    compute_base_angular_velocity_from_imu,
+    compute_base_pitch_from_imu,
+)
 
 from .standing_reward import StandingReward
 from .upkie_base_env import UpkieBaseEnv
 
 MAX_BASE_PITCH: float = np.pi
 MAX_GROUND_POSITION: float = float("inf")
-MAX_IMU_ANGULAR_VELOCITY: float = 1000.0  # rad/s
+MAX_BASE_ANGULAR_VELOCITY: float = 1000.0  # rad/s
 
 
 class UpkieWheelsEnv(UpkieBaseEnv):
 
     """!
     Upkie with full observation but only wheel velocity actions.
 
-    The environment has the following attributes:
-
-    - ``fall_pitch``: Fall pitch angle, in radians.
-    - ``max_ground_velocity``: Maximum commanded ground velocity in m/s.
-    - ``version``: Environment version number.
-    - ``wheel_radius``: Wheel radius in [m].
-
     Vectorized observations have the following structure:
 
     <table>
         <tr>
             <td><strong>Index</strong></td>
             <td><strong>Description</strong></td>
             </tr>
         <tr>
             <td>0</td>
-            <td>Base pitch in rad.</td>
+            <td>Pitch angle of the base with respect to the world vertical, in
+            radians. This angle is positive when the robot leans forward.</td>
         </tr>
         <tr>
             <td>1</td>
-            <td>Position of the average wheel contact point, in m.</td>
+            <td>Position of the average wheel contact point, in meters.</td>
         </tr>
         <tr>
             <td>2</td>
-            <td>Velocity of the average wheel contact point, in m/s.</td>
+            <td>Body angular velocity of the base frame along its lateral axis,
+            in radians per seconds.</td>
         </tr>
         <tr>
             <td>3</td>
-            <td>Body angular velocity of the IMU frame along its y-axis, in
-            rad/s.</td>
+            <td>Velocity of the average wheel contact point, in meters per
+            seconds.</td>
         </tr>
     </table>
 
     Vectorized actions have the following structure:
 
     <table>
         <tr>
@@ -79,19 +77,24 @@
             </tr>
         <tr>
             <td>``0``</td>
             <td>Ground velocity in [m] / [s].</td>
         </tr>
     </table>
 
-    The reward function is defined in @ref
-    envs.standing_reward.StandingReward "StandingReward".
+    The environment has the following attributes:
 
-    See also @ref envs.upkie_base_env.UpkieBaseEnv "UpkieBaseEnv" for notes on
-    using this environment.
+    - ``fall_pitch``: Fall pitch angle, in radians.
+    - ``max_ground_velocity``: Maximum commanded ground velocity in m/s.
+    - ``version``: Environment version number.
+    - ``wheel_radius``: Wheel radius in [m].
+
+    The reward function is defined in @ref envs.standing_reward.StandingReward
+    "StandingReward". See also @ref envs.upkie_base_env.UpkieBaseEnv
+    "UpkieBaseEnv" for notes on using this environment.
     """
 
     fall_pitch: float
     max_ground_velocity: float
     version: int = 3
     wheel_radius: float
 
@@ -127,16 +130,16 @@
             shm_name=shm_name,
         )
 
         observation_limit = np.array(
             [
                 MAX_BASE_PITCH,
                 MAX_GROUND_POSITION,
+                MAX_BASE_ANGULAR_VELOCITY,
                 max_ground_velocity,
-                MAX_IMU_ANGULAR_VELOCITY,
             ],
             dtype=np.float32,
         )
 
         # gym.Env: action_space
         self.action_space = spaces.Box(
             -np.float32(max_ground_velocity),
@@ -178,19 +181,26 @@
         """!
         Extract observation vector from a full observation dictionary.
 
         @param observation_dict Full observation dictionary from the spine.
         @returns Observation vector.
         """
         imu = observation_dict["imu"]
-        obs = np.empty(4)
-        obs[0] = compute_base_pitch_from_imu(imu["orientation"])
-        obs[1] = observation_dict["wheel_odometry"]["position"]
-        obs[2] = observation_dict["wheel_odometry"]["velocity"]
-        obs[3] = observation_dict["imu"]["angular_velocity"][1]
+        pitch_base_in_world = compute_base_pitch_from_imu(imu["orientation"])
+        angular_velocity_base_in_base = compute_base_angular_velocity_from_imu(
+            observation_dict["imu"]["angular_velocity"]
+        )
+        ground_position = observation_dict["wheel_odometry"]["position"]
+        ground_velocity = observation_dict["wheel_odometry"]["velocity"]
+
+        obs = np.empty(4, dtype=np.float32)
+        obs[0] = pitch_base_in_world
+        obs[1] = ground_position
+        obs[2] = angular_velocity_base_in_base[1]
+        obs[3] = ground_velocity
         return obs
 
     def dictionarize_action(self, action: np.ndarray) -> dict:
         """!
         Convert action vector into a spine action dictionary.
 
         @param action Action vector.
```

### Comparing `upkie-1.1.0/upkie/observers/base_pitch/base_pitch.py` & `upkie-1.2.0/upkie/observers/base_pitch/base_pitch.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # limitations under the License.
 
 from typing import Optional, Tuple
 
 import numpy as np
 
 from upkie.utils.clamp import clamp
+from upkie.utils.rotations import rotation_matrix_from_quaternion
 
 
 def compute_pitch_frame_in_parent(
     orientation_frame_in_parent: np.ndarray,
 ) -> float:
     """
     Get pitch angle of a given frame relative to the parent vertical.
@@ -68,80 +69,30 @@
         heading_in_parent *= -1.0
     sign = +1 if sagittal[2] < 0 else -1
     cos_pitch = clamp(np.dot(sagittal, heading_in_parent), -1.0, 1.0)
     pitch: float = sign * np.arccos(cos_pitch)
     return pitch
 
 
-def rotation_matrix_from_quaternion(
-    quat: Tuple[float, float, float, float]
-) -> np.ndarray:
-    """
-    Convert a unit quaternion to the matrix representing the same rotation.
-
-    Args:
-        quat: Unit quaternion to convert, in ``[w, x, y, z]`` format.
-
-    Returns:
-        Rotation matrix corresponding to this quaternion.
-
-    See `Conversion between quaternions and rotation matrices`_.
-
-    .. _`Conversion between quaternions and rotation matrices`:
-        https://en.wikipedia.org/wiki/Conversion_between_quaternions_and_Euler_angles#Rotation_matrices
-    """
-    if abs(np.dot(quat, quat) - 1.0) > 1e-5:
-        raise ValueError(f"Quaternion {quat} is not normalized")
-    qw, qx, qy, qz = quat
-    return np.array(
-        [
-            [
-                1 - 2 * (qy ** 2 + qz ** 2),
-                2 * (qx * qy - qz * qw),
-                2 * (qw * qy + qx * qz),
-            ],
-            [
-                2 * (qx * qy + qz * qw),
-                1 - 2 * (qx ** 2 + qz ** 2),
-                2 * (qy * qz - qx * qw),
-            ],
-            [
-                2 * (qx * qz - qy * qw),
-                2 * (qy * qz + qx * qw),
-                1 - 2 * (qx ** 2 + qy ** 2),
-            ],
-        ]
-    )
-
-
-def compute_base_pitch_from_imu(
+def compute_base_orientation_from_imu(
     quat_imu_in_ars: Tuple[float, float, float, float],
     rotation_base_to_imu: Optional[np.ndarray] = None,
-) -> float:
-    """
-    Get pitch angle of the base frame relative to the world frame.
+) -> np.ndarray:
+    """Get the orientation of the base frame with respect to the world frame.
 
     Args:
         quat_imu_in_ars: Quaternion representing the rotation matrix from
             the IMU frame to the  attitude reference system (ARS) frame, in
             ``[w, x, y, z]`` format.
         rotation_base_to_imu: Rotation matrix from the base frame to the IMU
             frame. When not specified, the default Upkie mounting orientation
             is used.
 
     Returns:
-        Angle from the world z-axis (unit vector opposite to gravity) to the
-        base z-axis. Equivalently, angle that the sagittal vector of the base
-        frame makes with the heading vector.
-
-    Note:
-        The output pitch angle is for the base (x-axis pointing forward), but
-        the input orientation is that of the IMU. Keep in mind that the IMU
-        frame is turned 180 degrees around the yaw axis of the base frame.
-
+        Rotation matrix from the base frame to the world frame.
     """
     if rotation_base_to_imu is None:
         # Default Upkie mounting orientation: USB connectors of the raspi
         # pointing to the left of the robot (XT-30 of the pi3hat to the right)
         rotation_base_to_imu = np.diag([-1.0, 1.0, -1.0])
 
     rotation_imu_to_ars = rotation_matrix_from_quaternion(quat_imu_in_ars)
@@ -150,9 +101,58 @@
     # whereas our world frame has +x forward, +y left and +z up:
     # https://github.com/mjbots/pi3hat/blob/ab632c82bd501b9fcb6f8200df0551989292b7a1/docs/reference.md#orientation
     rotation_ars_to_world = np.diag([1.0, -1.0, -1.0])
 
     rotation_base_to_world = (
         rotation_ars_to_world @ rotation_imu_to_ars @ rotation_base_to_imu
     )
+    return rotation_base_to_world
+
+
+def compute_base_pitch_from_imu(
+    quat_imu_in_ars: Tuple[float, float, float, float],
+    rotation_base_to_imu: Optional[np.ndarray] = None,
+) -> float:
+    """Get pitch angle of the base frame relative to the world frame.
+
+    Args:
+        quat_imu_in_ars: Quaternion representing the rotation matrix from
+            the IMU frame to the  attitude reference system (ARS) frame, in
+            ``[w, x, y, z]`` format.
+        rotation_base_to_imu: Rotation matrix from the base frame to the IMU
+            frame. When not specified, the default Upkie mounting orientation
+            is used.
+
+    Returns:
+        Angle from the world z-axis (unit vector opposite to gravity) to the
+        base z-axis. This angle is positive when the base leans forward.
+    """
+    rotation_base_to_world = compute_base_orientation_from_imu(
+        quat_imu_in_ars, rotation_base_to_imu
+    )
     pitch_base_in_world = compute_pitch_frame_in_parent(rotation_base_to_world)
     return pitch_base_in_world
+
+
+def compute_base_angular_velocity_from_imu(
+    angular_velocity_imu_in_imu: np.ndarray,
+) -> np.ndarray:
+    """
+    Kron
+
+        R_{WI}
+        Rdot_{WI} = R_{WI} (I_omega_{WI} x)
+        R_{WB} = R_WI R_IB
+        Rdot_{WB} = Rdot_WI R_IB
+                  = R_WI (I_omega_WI x) R_IB
+                  = R_WI R_IB (B_omega_WIx)
+                  = R_WB (B_omega_WIx) = R_WB (B_omega_WBx)
+        thus:
+           B_omega_WB = R_BI I_omega_WI
+    """
+    # TODO(scaron): move to config
+    rotation_base_to_imu = np.diag([-1.0, 1.0, -1.0])
+    rotation_imu_to_base = rotation_base_to_imu.T
+    angular_velocity_base_in_base = (
+        rotation_imu_to_base @ angular_velocity_imu_in_imu
+    )
+    return angular_velocity_base_in_base
```

### Comparing `upkie-1.1.0/upkie/observers/base_pitch/tests/base_pitch_test.py` & `upkie-1.2.0/upkie/observers/base_pitch/tests/base_pitch_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/BUILD` & `upkie-1.2.0/upkie/utils/BUILD`

 * *Files 16% similar despite different names*

```diff
@@ -48,24 +48,30 @@
 
 py_library(
     name = "realtime",
     srcs = ["realtime.py"],
 )
 
 py_library(
+    name = "rotations",
+    srcs = ["rotations.py"],
+)
+
+py_library(
     name = "spdlog",
     srcs = ["spdlog.py"],
 )
 
 py_library(
     name = "python",
     deps = [
         ":clamp",
         ":exceptions",
         ":filters",
         ":pinocchio",
         ":realtime",
+        ":rotations",
         ":spdlog",
     ],
 )
 
 add_lint_tests()
```

### Comparing `upkie-1.1.0/upkie/utils/clamp.py` & `upkie-1.2.0/upkie/utils/clamp.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/datetime_now_string.h` & `upkie-1.2.0/upkie/utils/datetime_now_string.h`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/exceptions.py` & `upkie-1.2.0/upkie/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/filters.py` & `upkie-1.2.0/upkie/utils/filters.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/pinocchio.py` & `upkie-1.2.0/upkie/utils/pinocchio.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/realtime.py` & `upkie-1.2.0/upkie/utils/realtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,22 +19,20 @@
 Real-time configuration.
 """
 
 import os
 
 
 def configure_cpu(cpu: int):
-    """
+    """!
     Set the current thread to run on a given CPU core.
 
     This function is meant to be used in conjunction with the ``isolcpus``
     kernel parameter. Check out the Raspberry Pi page in the documentation.
 
-    Args:
-        cpu: CPU core for this thread (on the Pi, CPUID in {0, 1, 2, 3}).
+    @param cpu CPU core for this thread (on the Pi, CPUID in {0, 1, 2, 3}).
 
-    Notes:
-        Calling this function affects only a single thread. A thread created
-        with ``pthread_create`` will then inherit the CPU affinity mask of its
-        parent.
+    @note Calling this function affects only a single thread. A thread created
+    with ``pthread_create`` will then inherit the CPU affinity mask of its
+    parent.
     """
     os.sched_setaffinity(0, {cpu})
```

### Comparing `upkie-1.1.0/upkie/utils/spdlog.py` & `upkie-1.2.0/upkie/utils/spdlog.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/tests/BUILD` & `upkie-1.2.0/upkie/utils/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/tests/clamp_test.py` & `upkie-1.2.0/upkie/utils/tests/clamp_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/tests/datetime_now_string_test.cpp` & `upkie-1.2.0/upkie/utils/tests/datetime_now_string_test.cpp`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/upkie/utils/tests/pinocchio_test.py` & `upkie-1.2.0/upkie/utils/tests/pinocchio_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.1.0/PKG-INFO` & `upkie-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upkie
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python module to control Upkie wheeled bipeds.
 Keywords: wheeled,biped,robot,balance,motion,control,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -15,21 +15,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: gym >=0.21.0
+Requires-Dist: gymnasium >=0.28.1
 Requires-Dist: loop-rate-limiters >=0.4.0
 Requires-Dist: mpacklog >=3.0.0
 Requires-Dist: numpy >=1.22.0
-Requires-Dist: qpsolvers >=1.9.1
 Requires-Dist: upkie_description >=1.2.0
-Requires-Dist: vulp >=1.1.1
+Requires-Dist: vulp >=1.2.1
 Project-URL: Changelog, https://github.com/tasts-robots/upkie/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://tasts-robots.org/doc/upkie/
 Project-URL: Source, https://github.com/tasts-robots/upkie
 Project-URL: Tracker, https://github.com/tasts-robots/upkie/issues
 
 # Upkie wheeled biped
```

