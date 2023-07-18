# Comparing `tmp/simpleoptions-0.3.1.tar.gz` & `tmp/simpleoptions-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleoptions-0.3.1.tar", last modified: Thu Mar 30 12:14:41 2023, max compression
+gzip compressed data, was "simpleoptions-0.6.1.tar", last modified: Tue Jul 18 15:38:43 2023, max compression
```

## Comparing `simpleoptions-0.3.1.tar` & `simpleoptions-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 12:14:41.893987 simpleoptions-0.3.1/
--rw-rw-rw-   0        0        0     1090 2019-07-25 00:43:58.000000 simpleoptions-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-03-30 12:14:41.892986 simpleoptions-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4403 2023-03-30 12:13:28.000000 simpleoptions-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-30 12:14:41.894987 simpleoptions-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-03-28 16:42:34.000000 simpleoptions-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 12:14:41.791977 simpleoptions-0.3.1/simpleoptions/
--rw-rw-rw-   0        0        0      217 2023-03-30 12:12:05.000000 simpleoptions-0.3.1/simpleoptions/__init__.py
--rw-rw-rw-   0        0        0     9971 2023-03-30 12:12:06.000000 simpleoptions-0.3.1/simpleoptions/environment.py
--rw-rw-rw-   0        0        0     1489 2023-03-30 12:12:05.000000 simpleoptions-0.3.1/simpleoptions/option.py
--rw-rw-rw-   0        0        0    20407 2023-03-30 12:12:07.000000 simpleoptions-0.3.1/simpleoptions/options_agent.py
--rw-rw-rw-   0        0        0     1510 2023-03-30 12:12:06.000000 simpleoptions-0.3.1/simpleoptions/primitive_option.py
-drwxrwxrwx   0        0        0        0 2023-03-30 12:14:41.862984 simpleoptions-0.3.1/simpleoptions.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-03-30 12:14:41.000000 simpleoptions-0.3.1/simpleoptions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-03-30 12:14:41.000000 simpleoptions-0.3.1/simpleoptions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 12:14:41.000000 simpleoptions-0.3.1/simpleoptions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-03-30 12:14:41.000000 simpleoptions-0.3.1/simpleoptions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-30 12:14:41.000000 simpleoptions-0.3.1/simpleoptions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 12:14:41.888985 simpleoptions-0.3.1/test/
--rw-rw-rw-   0        0        0     1279 2023-03-28 16:24:33.000000 simpleoptions-0.3.1/test/test_discounted_sum.py
--rw-rw-rw-   0        0        0     4869 2023-03-30 12:12:06.000000 simpleoptions-0.3.1/test/test_intra_option_update.py
--rw-rw-rw-   0        0        0     8406 2023-03-30 12:12:06.000000 simpleoptions-0.3.1/test/test_macro_q_update.py
--rw-rw-rw-   0        0        0     2343 2023-03-30 12:12:06.000000 simpleoptions-0.3.1/test/test_run_agent.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.285380 simpleoptions-0.6.1/
+-rw-rw-rw-   0        0        0     1090 2019-07-25 00:43:58.000000 simpleoptions-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-07-18 15:38:43.285380 simpleoptions-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4403 2023-03-30 12:13:28.000000 simpleoptions-0.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 15:38:43.286380 simpleoptions-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2023-07-18 15:35:49.000000 simpleoptions-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.250871 simpleoptions-0.6.1/simpleoptions/
+-rw-rw-rw-   0        0        0      217 2023-03-30 12:12:05.000000 simpleoptions-0.6.1/simpleoptions/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-06-21 14:46:48.000000 simpleoptions-0.6.1/simpleoptions/environment.py
+-rw-rw-rw-   0        0        0     1619 2023-04-14 17:42:51.000000 simpleoptions-0.6.1/simpleoptions/option.py
+-rw-rw-rw-   0        0        0    22676 2023-07-18 14:34:18.000000 simpleoptions-0.6.1/simpleoptions/options_agent.py
+-rw-rw-rw-   0        0        0     2069 2023-04-18 12:35:11.000000 simpleoptions-0.6.1/simpleoptions/primitive_option.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.280380 simpleoptions-0.6.1/simpleoptions.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.284381 simpleoptions-0.6.1/test/
+-rw-rw-rw-   0        0        0     1327 2023-04-14 17:42:51.000000 simpleoptions-0.6.1/test/test_discounted_sum.py
+-rw-rw-rw-   0        0        0     5007 2023-04-14 17:44:04.000000 simpleoptions-0.6.1/test/test_intra_option_update.py
+-rw-rw-rw-   0        0        0     8620 2023-04-15 00:31:22.000000 simpleoptions-0.6.1/test/test_macro_q_update.py
+-rw-rw-rw-   0        0        0    29384 2023-04-19 17:28:07.000000 simpleoptions-0.6.1/test/test_run_agent.py
```

### Comparing `simpleoptions-0.3.1/LICENSE` & `simpleoptions-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.3.1/PKG-INFO` & `simpleoptions-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleoptions
-Version: 0.3.1
+Version: 0.6.1
 Summary: A package which provides a simple framework for working with Options in Reinforcement Learning.
 Home-page: https://github.com/Ueva/BaRL-SimpleOptions
 Author: Joshua Evans
 Author-email: jbe25@bath.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleoptions-0.3.1/README.md` & `simpleoptions-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.3.1/setup.py` & `simpleoptions-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="simpleoptions",
-    version="0.3.1",
+    version="0.6.1",
     author="Joshua Evans",
     author_email="jbe25@bath.ac.uk",
     description="A package which provides a simple framework for working with Options in Reinforcement Learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ueva/BaRL-SimpleOptions",
     # packages=setuptools.find_packages(exclude=("example", "test")),
-    packages = ["simpleoptions"],
+    packages=["simpleoptions"],
     install_requires=["numpy", "networkx"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `simpleoptions-0.3.1/simpleoptions/environment.py` & `simpleoptions-0.6.1/simpleoptions/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import networkx as nx
 
-from typing import List
+from typing import List, Set
 from typing import Hashable, Tuple
 from abc import ABC, abstractmethod
 
 from simpleoptions.option import BaseOption
 
 
 class BaseEnvironment(ABC):
@@ -71,21 +71,31 @@
     def close(self):
         """
         Cleanly terminates all environment-related process (e.g. closing any renderers).
         """
         pass
 
     @abstractmethod
-    def get_action_space(self) -> List[Hashable]:
+    def get_state_space(self) -> Set[Hashable]:
         """
-        Returns a list containing the set of primitive actions available in this environment. A subset of
+        Returns a set containing all of the possible states in this environment.
+
+        Returns:
+            Set[Hashable]: All possible states in this environment.
+        """
+        pass
+
+    @abstractmethod
+    def get_action_space(self) -> Set[Hashable]:
+        """
+        Returns a set containing all of the primitive actions available in this environment. A subset of
         the actions in this list will be available in each individual state.
 
         Returns:
-            List[Hashable]: All possible primitive actions available in this environment.
+            Set[Hashable]: All possible primitive actions available in this environment.
 
         See Also:
             BaseEnvironment.get_available_actions
         """
         pass
 
     @abstractmethod
```

### Comparing `simpleoptions-0.3.1/simpleoptions/option.py` & `simpleoptions-0.6.1/simpleoptions/option.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 
             Returns:
                 bool -- [description]
         """
         pass
 
     @abstractmethod
-    def policy(self, state: Hashable) -> Hashable:
+    def policy(self, state: Hashable, test: bool = False) -> Hashable:
         """
         Returns the action specified by this option's policy for a given state.
 
         Arguments:
             state {Hashable} -- The environmental state in which the option chooses an action in.
+            test [bool] --  When True the option follows a greedy-policy, for evaluation. Defaults to False.
 
         Returns:
             action [Hashable] -- The action specified by the option's policy in this state.
         """
         pass
 
     @abstractmethod
```

### Comparing `simpleoptions-0.3.1/simpleoptions/options_agent.py` & `simpleoptions-0.6.1/simpleoptions/options_agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import gc
 import math
 import random
 import statistics
 import numpy as np
+from numpy.random import Generator as RNG
 
-from copy import copy, deepcopy
+from copy import copy
 from collections import defaultdict
-from typing import Hashable, List, Union
+from typing import Tuple, Hashable, List, Union, DefaultDict
 
 from simpleoptions.option import BaseOption
 from simpleoptions.environment import BaseEnvironment
 
 
 class OptionAgent:
     """
@@ -24,14 +25,15 @@
         test_env: "BaseEnvironment" = None,
         epsilon: float = 0.15,
         macro_alpha: float = 0.2,
         intra_option_alpha: float = 0.2,
         gamma: float = 1.0,
         default_action_value=0.0,
         n_step_updates=False,
+        rng: RNG = None,
     ):
         """
         Constructs a new OptionAgent object.
 
         Arguments:
             env {Environment} -- The environment for the agent to act in.
             epsilon {float} -- The chance of the agent taking a random action when following its base policy. Defaults to 0.15.
@@ -47,34 +49,38 @@
         self.gamma = gamma
         self.macro_q_alpha = macro_alpha
         self.intra_option_alpha = intra_option_alpha
         self.executing_options = []
         self.executing_options_states = []
         self.executing_options_rewards = []
         self.n_step_updates = n_step_updates
+        self.rng = rng if rng else random
 
         self.env = env
         self.test_env = test_env if test_env is not None else None
 
+        self.evaluation_log = defaultdict(lambda: defaultdict(lambda: defaultdict(list)))
+        self.training_log = defaultdict(list)
+
     def macro_q_learn(
-        self, state_trajectory: List[Hashable], rewards: List[float], option: "BaseOption", n_step=False
+        self,
+        state_trajectory: List[Hashable],
+        rewards: List[float],
+        option: "BaseOption",
+        n_step=False,
     ) -> None:
         """
         Performs Macro Q-Learning updates along the given trajectory for the given Option.
 
         Args:
             state_trajectory (List[Hashable]): The list of states visited each time-step while the option was executing.
             rewards (List[float]): The list of rewards earned each time-step while the Option was executing.
             option (Option): The option to perform an update for.
             n_step (bool): Whether or not to perform n-step updates. Defaults to False, performing one-step updates.
         """
-        state_trajectory = deepcopy(state_trajectory)
-        rewards = deepcopy(rewards)
-        option = option
-
         # For Debuging - saves info about long-running options to a file.
         if (len(state_trajectory) > 500) and hasattr(option, "hierarchy_level"):
             with open("long_running_options.txt", "a+") as f:
                 # Write the ID of the option and how long it executed for.
                 f.write(
                     f"Option {option.hierarchy_level}-{option.source_cluster}->{option.target_cluster} ran for {len(state_trajectory)} decision stages.\n"
                 )
@@ -85,41 +91,37 @@
                     for o in self.env.get_available_options(most_common_state)
                 }
                 f.write(f"State Stuck: {most_common_state}\tQ-Values: {q_values}\n\n")
                 quit()
 
         termination_state = state_trajectory[-1]
 
-        while len(state_trajectory) > 1:
-            num_rewards = len(rewards)
-            initiation_state = state_trajectory[0]
+        for i in range(len(state_trajectory) - 1):
+            initiation_state = state_trajectory[i]
 
             old_value = self.q_table[(hash(initiation_state), hash(option))]
 
             # Compute discounted sum of rewards.
-            discounted_sum_of_rewards = self._discounted_return(rewards, self.gamma)
+            discounted_sum_of_rewards = self._discounted_return(rewards[i:], self.gamma)
 
             # Get Q-Values for Next State.
             if not self.env.is_state_terminal(termination_state):
                 q_values = [
                     self.q_table[(hash(termination_state), hash(o))]
                     for o in self.env.get_available_options(termination_state)
                 ]
             # Cater for terminal states (Q-value is zero).
             else:
                 q_values = [0]
 
             # Perform Macro-Q Update
             self.q_table[(hash(initiation_state), hash(option))] = old_value + self.macro_q_alpha * (
-                discounted_sum_of_rewards + math.pow(self.gamma, len(rewards)) * max(q_values) - old_value
+                discounted_sum_of_rewards + math.pow(self.gamma, len(rewards) - i) * max(q_values) - old_value
             )
 
-            state_trajectory.pop(0)
-            rewards.pop(0)
-
             # If we're not performing n-step updates, exit after the first iteration.
             if not n_step:
                 break
 
     def intra_option_learn(
         self,
         state_trajectory: List[Hashable],
@@ -134,35 +136,31 @@
         Args:
             state_trajectory (List[Hashable]): The list of states visited each time-step while the option was executing.
             rewards (List[float]): The list of rewards earned each time-step while the option was executing.
             executed_option (Option): The option that was executed.
             higher_level_option (Union[None, optional): The option whose policy chose the executed_option. Defaults to None, indicating that the option was executed under the base policy.
             n_step (bool): Whether or not to perform n-step updates. Defaults to False, performing one-step updates.
         """
-        state_trajectory = deepcopy(state_trajectory)
-        rewards = deepcopy(rewards)
-        executed_option = executed_option
 
         termination_state = state_trajectory[-1]
 
-        while len(state_trajectory) > 1:
-            num_rewards = len(rewards)
-            initiation_state = state_trajectory[0]
+        for i in range(len(state_trajectory) - 1):
+            initiation_state = state_trajectory[i]
 
             # We perform an intra-option update for all other options which select executed_option in this state.
             for other_option in self.env.get_available_options(initiation_state):
                 if (
                     (hash(other_option) != hash(higher_level_option) or higher_level_option is None)
-                    and other_option.initiation(initiation_state)
                     and hash(other_option.policy(initiation_state)) == hash(executed_option)
+                    # and other_option.initiation(initiation_state) # This check is already handled in env.get_available_options!
                 ):
                     old_value = self.q_table[(hash(initiation_state), hash(other_option))]
 
                     # Compute discounted sum of rewards.
-                    discounted_sum_of_rewards = self._discounted_return(rewards, self.gamma)
+                    discounted_sum_of_rewards = self._discounted_return(rewards[i:], self.gamma)
 
                     if not self.env.is_state_terminal(termination_state):
                         # If the option terminates, we consider the value of the next best option.
                         next_q_terminates = other_option.termination(termination_state) * max(
                             [
                                 self.q_table[(hash(termination_state), hash(o))]
                                 for o in self.env.get_available_options(termination_state)
@@ -176,21 +174,18 @@
                     else:
                         next_q_terminates = 0
                         next_q_continues = 0
 
                     # Perform Intra-Option Update.
                     self.q_table[(hash(initiation_state), hash(other_option))] = old_value + self.intra_option_alpha * (
                         discounted_sum_of_rewards
-                        + math.pow(self.gamma, len(rewards)) * (next_q_continues + next_q_terminates)
+                        + math.pow(self.gamma, len(rewards) - i) * (next_q_continues + next_q_terminates)
                         - old_value
                     )
 
-            state_trajectory.pop(0)
-            rewards.pop(0)
-
             # If we're not performing n-step updates, exit after the first iteration.
             if not n_step:
                 break
 
     def select_action(
         self, state: Hashable, executing_options: List["BaseOption"], test: bool = False
     ) -> Union[BaseOption, Hashable, None]:
@@ -207,101 +202,121 @@
         # Select option from set of available options
         # Use epsilon greedy at lowest level, use option policy at higher levels.
 
         # If we do not currently have any options executing, we act according to the agent's
         # base epsilon-greedy policy over the set of currently available options.
         if len(executing_options) == 0:
             # Random Action.
-            if not test and random.random() < self.epsilon:
+            if not test and self.rng.random() < self.epsilon:
                 available_options = self.env.get_available_options(state, exploration=True)
-                return random.choice(available_options)
+                return self.rng.choice(available_options)
             # Best Action.
             else:
                 available_options = self.env.get_available_options(state, exploration=False)
                 # Find Q-values of available options.
                 q_values = [self.q_table[(hash(state), hash(o))] for o in available_options]
 
                 # Return the option with the highest Q-value, breaking ties randomly.
                 return available_options[
-                    random.choice([idx for idx, q_value in enumerate(q_values) if q_value == max(q_values)])
+                    self.rng.choice([idx for idx, q_value in enumerate(q_values) if q_value == max(q_values)])
                 ]
         # If we are currently following an option's policy, return what it selects.
         else:
-            return executing_options[-1].policy(state)
+            return executing_options[-1].policy(state, test)
 
     def run_agent(
-        self, num_epochs, epoch_length, render_interval: int = 0, test_interval: int = 0, test_length: int = 0
-    ) -> List[float]:
+        self,
+        num_epochs: int,
+        epoch_length: int,
+        render_interval: int = 0,
+        test_interval: int = 0,
+        test_length: int = 0,
+        test_runs: int = 10,
+        verbose_logging: bool = True,
+    ) -> Tuple[DefaultDict, DefaultDict | None]:
         """
         Trains the agent for a given number of episodes.
 
         Args:
             num_epochs (int): The number of epochs to train the agent for.
             epoch_length (int): How many time-steps each epoch should last for.
             render_interval (int, optional): How often (in time-steps) to call the environement's render function, in time-steps. Zero by default, disabling rendering.
             test_interval (int, optional): How often (in epochs) to evaluate the greedy policy learned by the agent. Zero by default, in which case training performance is returned.
             test_length (int, optional): How long (in time-steps) to test the agent for. Zero by default, in which case the agent is tested for one epoch.
+            test_runs (int, optional): How many test runs to perform each test_interval.
+            verbose_logging (bool, optional): Whether to log all information about each time-step, instead of just rewards. Defaults to True.
 
         Returns:
-            List[float]: A list containing floats representing the rewards earned by the agent each time-step.
+            Tuple[DefaultDict, DefaultDict | None]: A tuple of dictionaries, (training_logs, evaluation_logs), containing data logs of training and evaluation.
         """
 
         # Set the time-step limit.
         num_time_steps = num_epochs * epoch_length
 
         # If we are testing the greedy policy separately, make a separate copy of
         # the environment to use for those tests. Also initialise variables for
         # tracking test performance.
+        training_rewards = [None for _ in range(num_time_steps)]
+
         if test_interval > 0:
             test_interval_time_steps = test_interval * epoch_length
-            test_rewards = []
+            evaluation_rewards = [None for _ in range(num_time_steps // test_interval_time_steps)]
 
             # Check that a test environment has been provided - if not, raise an error.
             if self.test_env is None:
                 raise RuntimeError("No test_env has been provided specified.")
+        else:
+            evaluation_rewards = []
 
-        episode_rewards = []
-        # active_options = []
         episode = 0
         time_steps = 0
 
         while time_steps < num_time_steps:
-            episode_rewards.append([])
-
             # Initialise initial state variables.
             state = self.env.reset()
             terminal = False
 
             if render_interval > 0:
                 self.env.render()
 
             while not terminal:
                 selected_option = self.select_action(state, self.executing_options)
 
                 # Handle if the selected option is a higher-level option.
                 if isinstance(selected_option, BaseOption):
                     self.executing_options.append(copy(selected_option))
-                    self.executing_options_states.append([deepcopy(state)])
+                    self.executing_options_states.append([state])
                     self.executing_options_rewards.append([])
 
                 # Handle if the selected option is a primitive action.
                 else:
                     time_steps += 1
                     next_state, reward, terminal, __ = self.env.step(selected_option)
 
+                    # Logging
+                    training_rewards[time_steps - 1] = reward
+                    if verbose_logging:
+                        transition = {
+                            "state": state,
+                            "next_state": next_state,
+                            "reward": reward,
+                            "terminal": terminal,
+                            "active_options": [str(option) for option in self.executing_options],
+                        }
+                        for key, value in transition.items():
+                            self.training_log[key].append(value)
+
                     # Render, if we need to.
                     if render_interval > 0 and time_steps % render_interval == 0:
                         self.env.render()
 
-                    state = deepcopy(next_state)
-                    episode_rewards[episode].append(reward)
-                    # active_options.append(len(self.executing_options))
+                    state = next_state
 
                     for i in range(len(self.executing_options)):
-                        self.executing_options_states[i].append(deepcopy(next_state))
+                        self.executing_options_states[i].append(next_state)
                         self.executing_options_rewards[i].append(reward)
 
                     # Terminate any options which need terminating this time-step.
                     while self.executing_options and self._roll_termination(self.executing_options[-1], next_state):
                         if self.executing_options[-1] not in self.env.exploration_options:
                             # Perform a macro-q learning update for the terminating option.
                             self.macro_q_learn(
@@ -321,18 +336,24 @@
                         self.executing_options_states.pop()
                         self.executing_options_rewards.pop()
                         self.executing_options.pop()
 
                     # If we are testing the greedy policy learned by the agent separately,
                     # and it is time to test it, then test it.
                     if test_interval > 0 and time_steps % test_interval_time_steps == 0:
-                        test_rewards.append(self.test_policy(test_length))
+                        evaluation_rewards[(time_steps - 1) // test_interval_time_steps] = self.test_policy(
+                            test_length,
+                            test_runs,
+                            time_steps // test_interval_time_steps,
+                            allow_exploration=False,
+                            verbose_logging=verbose_logging,
+                        )
 
                 # If we have been training for more than the desired number of time-steps, terminate.
-                if time_steps > num_time_steps:
+                if time_steps >= num_time_steps:
                     terminal = True
 
                 # Handle if the current state is terminal.
                 if terminal:
                     while len(self.executing_options) > 0:
                         if self.executing_options[-1] not in self.env.exploration_options:
                             # Perform a macro-q learning update for the topmost option.
@@ -353,27 +374,29 @@
                         self.executing_options_states.pop()
                         self.executing_options_rewards.pop()
                         self.executing_options.pop()
 
             episode += 1
         gc.collect()
 
-        if test_interval == 0:
-            # return episode_rewards, active_options
-            return episode_rewards
+        if verbose_logging:
+            training_log = self.training_log
+            evaluation_log = self.evaluation_log if self.evaluation_log else None
+            return training_log, evaluation_log
         else:
-            # return test_rewards, active_options
-            return test_rewards
+            training_log = [sum(training_rewards[i * epoch_length : (i + 1) * epoch_length]) for i in range(num_epochs)]
+            evaluation_log = evaluation_rewards if evaluation_rewards else None
+            return training_log, evaluation_log
 
-    def test_policy(self, test_length, test_runs=10, allow_exploration=False):
-        test_returns = []
+    def test_policy(self, test_length, test_runs, eval_number, allow_exploration=False, verbose_logging=True):
+        test_returns = [None for _ in range(test_runs)]
 
         for test_run in range(test_runs):
             time_steps = 0
-            run_rewards = []
+            run_rewards = [None for _ in range(test_length)]
             while time_steps < test_length:
                 state = self.test_env.reset()
                 executing_options = []
                 terminal = False
 
                 while not terminal:
                     selected_option = self.select_action(state, executing_options, test=not allow_exploration)
@@ -383,31 +406,43 @@
                         executing_options.append(copy(selected_option))
 
                     # Handle if the selected option is a primitive action.
                     else:
                         time_steps += 1
                         next_state, reward, terminal, __ = self.test_env.step(selected_option)
 
-                        state = deepcopy(next_state)
-                        run_rewards.append(reward)
+                        # Logging
+                        run_rewards[time_steps - 1] = reward
+                        if verbose_logging:
+                            transition = {
+                                "state": state,
+                                "next_state": next_state,
+                                "reward": reward,
+                                "terminal": terminal,
+                                "active_options": [str(option) for option in executing_options],
+                            }
+                            for key, value in transition.items():
+                                self.evaluation_log[f"evaluation_{eval_number}"][f"run_{test_run+1}"][key].append(value)
+
+                        state = next_state
 
                         # Terminate any options which need terminating this time-step.
                         while executing_options and self._roll_termination(executing_options[-1], next_state):
                             executing_options.pop()
 
                     # If we have been testing for more than the desired number of time-steps, terminate.
-                    if time_steps > test_length:
+                    if time_steps >= test_length:
                         terminal = True
 
                     # Handle if the current state is terminal.
                     if terminal:
                         while len(executing_options) > 0:
                             executing_options.pop()
 
-            test_returns.append(sum(run_rewards))
+            test_returns[test_run] = sum(run_rewards)
         return statistics.mean(test_returns)
 
     def _discounted_return(self, rewards: List[float], gamma: float) -> float:
         # Computes the discounted reward given an ordered list of rewards, and a discount factor.
         num_rewards = len(rewards)
 
         # Fill an array with gamma^index for index = 0 to index = num_rewards - 1.
@@ -417,11 +452,11 @@
         discounted_sum_of_rewards = np.sum(np.multiply(rewards, gamma_exp))
 
         return discounted_sum_of_rewards
 
     def _roll_termination(self, option: "BaseOption", state: Hashable):
         # Rolls on whether or not the given option terminates in the given state.
         # Will work with stochastic and deterministic termination functions.
-        if random.random() > option.termination(state):
+        if self.rng.random() > option.termination(state):
             return False
         else:
             return True
```

### Comparing `simpleoptions-0.3.1/simpleoptions.egg-info/PKG-INFO` & `simpleoptions-0.6.1/simpleoptions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleoptions
-Version: 0.3.1
+Version: 0.6.1
 Summary: A package which provides a simple framework for working with Options in Reinforcement Learning.
 Home-page: https://github.com/Ueva/BaRL-SimpleOptions
 Author: Joshua Evans
 Author-email: jbe25@bath.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleoptions-0.3.1/test/test_intra_option_update.py` & `simpleoptions-0.6.1/test/test_intra_option_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,121 @@
-import pytest
-
-from simpleoptions import OptionAgent, BaseOption, PrimitiveOption, option, primitive_option
-
-
-class DummyOption(BaseOption):
-    """
-    A dummy option for testing.
-
-    Executes a dummy action (int 1) in every state, terminates with probability 1.0 in a
-    given state and probability 0.0 otherwise, and can be initiated in any state.
-    """
-
-    def __init__(self, name, action, termination_state):
-        self.name = name
-        self.action = action
-        self.termination_state = termination_state
-
-    def initiation(self, state):
-        return True
-
-    def policy(self, state):
-        return self.action
-
-    def termination(self, state):
-        if state == self.termination_state:
-            return 1.0
-        else:
-            return 0.0
-
-    def __str__(self):
-        return self.name
-
-    def __hash__(self):
-        return hash(str(self))
-
-
-class DummyEnv:
-    """
-    Dummy class to pass in as an environment - implements only what we need.
-    """
-
-    def __init__(self, options=[]):
-        self.options = options
-
-    def is_state_terminal(self, state):
-        return False
-
-    def get_available_actions(self, state):
-        return [1]
-
-    def get_available_options(self, state):
-        return self.options
-
-
-# Two options which execute the same primitive action, one time-step, intial q-values of zero.
-def test_one_step_intra_option_update_1():
-    # Set up dummy states, rewards, options, parameters etc. for the test.
-    state_trajectory = ["state_1", "state_2"]
-    reward_trajectory = [1]
-    initial_values = {"state_1, option": 0, "state_2, 1": 0}
-    alpha = 0.2
-    gamma = 0.9
-
-    # Define two dummy options which execute the SAME lower-level option.
-    # If we perform an intra-option update for one of them, the other should get updated.
-    lower_level_option = DummyOption("lower_level_option", 1, "state_2")
-    option_1 = DummyOption("test_option_1", lower_level_option, "state_2")
-    option_2 = DummyOption("test_option_2", lower_level_option, "state_2")
-
-    # Initialise an OptionAgent (note that initial q-values for all states are zero by default).
-    agent = OptionAgent(env=DummyEnv([option_1, option_2, lower_level_option]), macro_alpha=alpha, gamma=gamma)
-
-    # First, perform a macro-q update for option_1. Then, perform an intra-option update for
-    # option_1. This should result in both option_1 and option_2 having the same q-value in
-    # state_1, since they both execute the same primitive action, and should both get updated once.
-    agent.macro_q_learn(state_trajectory, reward_trajectory, option_1, n_step=True)
-    agent.intra_option_learn(state_trajectory, reward_trajectory, lower_level_option, option_1, n_step=True)
-
-    # Ensure that the q-values for executing option_1 in state_1 and executing option_2 in state_1 are the same.
-    assert agent.q_table[(hash("state_1"), hash(option_1))] == agent.q_table[(hash("state_1"), hash(option_2))]
-
-
-# Two options which execute the different primitive actions, one time-step, initial q-values of zero.
-def test_one_step_intra_option_update_2():
-    # Set up dummy states, rewards, options, parameters etc. for the test.
-    state_trajectory = ["state_1", "state_2"]
-    reward_trajectory = [1]
-    initial_values = {"state_1, option": 0, "state_2, 1": 0}
-    alpha = 0.2
-    gamma = 0.9
-
-    # Define two dummy options which execute DIFFERENT options. If we
-    # perform an intra-option update for one of them, the other should NOT get updated.
-    lower_level_option_1 = DummyOption("lower_level_option_1", 1, "state_2")
-    option_1 = DummyOption("test_option_1", lower_level_option_1, "state_2")
-    lower_level_option_2 = DummyOption("lower_level_option_2", 2, "state_2")
-    option_2 = DummyOption("test_option_2", lower_level_option_2, "state_2")
-
-    # Initialise an OptionAgent (note that initial q-values for all states are zero by default).
-    agent = OptionAgent(
-        env=DummyEnv([option_1, option_2, lower_level_option_1, lower_level_option_2]), macro_alpha=alpha, gamma=gamma
-    )
-
-    # First, perform a macro-q update for option_1. Then, perform an intra-option update for
-    # option_1. This should result in option_1 having its q-values updated once (during the
-    # macro-q update), but option_2 should not be updated during the intra-option update because
-    # its policy is different to option_1's.
-    agent.macro_q_learn(state_trajectory, reward_trajectory, option_1, n_step=True)
-    agent.intra_option_learn(state_trajectory, reward_trajectory, lower_level_option_1, option_1, n_step=True)
-
-    # Ensure that the q-value of executing option_1 in state_1 is updated, and that the
-    # q-value of executing option_2 in state_1 remains at 0.0.
-    assert agent.q_table.get((hash("state_1"), hash(option_1)), 0) == 0.2
-    assert agent.q_table.get((hash("state_1"), hash(option_2)), 0) == 0.0
+import pytest
+
+from simpleoptions import OptionAgent, BaseOption
+
+
+class DummyOption(BaseOption):
+    """
+    A dummy option for testing.
+
+    Executes a dummy action (int 1) in every state, terminates with probability 1.0 in a
+    given state and probability 0.0 otherwise, and can be initiated in any state.
+    """
+
+    def __init__(self, name, action, termination_state):
+        self.name = name
+        self.action = action
+        self.termination_state = termination_state
+
+    def initiation(self, state):
+        return True
+
+    def policy(self, state, test=False):
+        return self.action
+
+    def termination(self, state):
+        if state == self.termination_state:
+            return 1.0
+        else:
+            return 0.0
+
+    def __str__(self):
+        return self.name
+
+    def __hash__(self):
+        return hash(str(self))
+
+
+class DummyEnv:
+    """
+    Dummy class to pass in as an environment - implements only what we need.
+    """
+
+    def __init__(self, options=[]):
+        self.options = options
+
+    def is_state_terminal(self, state):
+        return False
+
+    def get_available_actions(self, state):
+        return [1]
+
+    def get_available_options(self, state):
+        return self.options
+
+
+# Two options which execute the same primitive action, one time-step, intial q-values of zero.
+def test_one_step_intra_option_update_1():
+    # Set up dummy states, rewards, options, parameters etc. for the test.
+    state_trajectory = ["state_1", "state_2"]
+    reward_trajectory = [1]
+    initial_values = {"state_1, option": 0, "state_2, 1": 0}
+    alpha = 0.2
+    gamma = 0.9
+
+    # Define two dummy options which execute the SAME lower-level option.
+    # If we perform an intra-option update for one of them, the other should get updated.
+    lower_level_option = DummyOption("lower_level_option", 1, "state_2")
+    option_1 = DummyOption("test_option_1", lower_level_option, "state_2")
+    option_2 = DummyOption("test_option_2", lower_level_option, "state_2")
+
+    # Initialise an OptionAgent (note that initial q-values for all states are zero by default).
+    agent = OptionAgent(
+        env=DummyEnv([option_1, option_2, lower_level_option]),
+        macro_alpha=alpha,
+        gamma=gamma,
+    )
+
+    # First, perform a macro-q update for option_1. Then, perform an intra-option update for
+    # option_1. This should result in both option_1 and option_2 having the same q-value in
+    # state_1, since they both execute the same primitive action, and should both get updated once.
+    agent.macro_q_learn(state_trajectory, reward_trajectory, option_1, n_step=True)
+    agent.intra_option_learn(state_trajectory, reward_trajectory, lower_level_option, option_1, n_step=True)
+
+    # Ensure that the q-values for executing option_1 in state_1 and executing option_2 in state_1 are the same.
+    assert agent.q_table[(hash("state_1"), hash(option_1))] == agent.q_table[(hash("state_1"), hash(option_2))]
+
+
+# Two options which execute the different primitive actions, one time-step, initial q-values of zero.
+def test_one_step_intra_option_update_2():
+    # Set up dummy states, rewards, options, parameters etc. for the test.
+    state_trajectory = ["state_1", "state_2"]
+    reward_trajectory = [1]
+    initial_values = {"state_1, option": 0, "state_2, 1": 0}
+    alpha = 0.2
+    gamma = 0.9
+
+    # Define two dummy options which execute DIFFERENT options. If we
+    # perform an intra-option update for one of them, the other should NOT get updated.
+    lower_level_option_1 = DummyOption("lower_level_option_1", 1, "state_2")
+    option_1 = DummyOption("test_option_1", lower_level_option_1, "state_2")
+    lower_level_option_2 = DummyOption("lower_level_option_2", 2, "state_2")
+    option_2 = DummyOption("test_option_2", lower_level_option_2, "state_2")
+
+    # Initialise an OptionAgent (note that initial q-values for all states are zero by default).
+    agent = OptionAgent(
+        env=DummyEnv([option_1, option_2, lower_level_option_1, lower_level_option_2]),
+        macro_alpha=alpha,
+        gamma=gamma,
+    )
+
+    # First, perform a macro-q update for option_1. Then, perform an intra-option update for
+    # option_1. This should result in option_1 having its q-values updated once (during the
+    # macro-q update), but option_2 should not be updated during the intra-option update because
+    # its policy is different to option_1's.
+    agent.macro_q_learn(state_trajectory, reward_trajectory, option_1, n_step=True)
+    agent.intra_option_learn(state_trajectory, reward_trajectory, lower_level_option_1, option_1, n_step=True)
+
+    # Ensure that the q-value of executing option_1 in state_1 is updated, and that the
+    # q-value of executing option_2 in state_1 remains at 0.0.
+    assert agent.q_table.get((hash("state_1"), hash(option_1)), 0) == 0.2
+    assert agent.q_table.get((hash("state_1"), hash(option_2)), 0) == 0.0
```

### Comparing `simpleoptions-0.3.1/test/test_macro_q_update.py` & `simpleoptions-0.6.1/test/test_macro_q_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,197 @@
-import pytest
-
-from copy import deepcopy
-
-from simpleoptions.option import BaseOption
-from simpleoptions.options_agent import OptionAgent
-
-
-class DummyOption(BaseOption):
-    """
-    A dummy option for testing.
-
-    Returns a dummy action, (int 1), terminates with probability 1.0 in
-    every state, and can be initiated in any state.
-    """
-
-    def __init__(self, name):
-        self.name = name
-
-    def initiation(self, state):
-        return True
-
-    def policy(self, state):
-        return 1
-
-    def termination(self, state):
-        return 1.0
-
-    def __str__(self):
-        return self.name
-
-    def __hash__(self):
-        return hash(str(self))
-
-
-class DummyEnv:
-    """
-    Dummy class to pass in as an environment - implements only what we need.
-    """
-
-    def __init__(self):
-        return
-
-    def is_state_terminal(self, state):
-        return False
-
-    def get_available_options(self, state):
-        return [1]
-
-
-# Test a macro_q_learning update over a single time-step, with initial q-values of zero.
-def test_one_step_macro_q_update_1():
-    # Set up dummy states, rewards, options, parameters etc. for the test.
-    state_trajectory = ["state_1", "state_2"]
-    reward_trajectory = [1]
-    option = DummyOption("test_option_1")
-    initial_values = {"state_1, option": 0, "state_2, 1": 0}
-    alpha = 0.2
-    gamma = 0.9
-
-    # Initialise an OptionAgent (note that initial q-values for all states are zero by default).
-    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
-
-    # Perform a macro-q learning update for our test option over a single time-step, where a reward of
-    # 1 was earned after transitioning from state_1 to state_2.
-    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
-
-    # Ensure that the new value of initating our test option in state_1 is correct after performing the update.
-    # Our dummy environment returns a list containing the primitive action 1 as the available action in state_2,
-    # and its value will be zero (we assume that this is the first update, and initial q-valaues are zero by default).
-    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
-        reward_trajectory[0] + gamma * initial_values["state_2, 1"] - initial_values["state_1, option"]
-    )
-
-
-# Test a macro_q_learning update over a single time-step, with non-zero initial q-values.
-def test_one_step_macro_q_update_2():
-    # Set up dummy states, rewards, options, parameters etc. for the test.
-    state_trajectory = ["state_1", "state_2"]
-    reward_trajectory = [1]
-    option = DummyOption("test_option_1")
-    initial_values = {"state_1, option": 2, "state_2, 1": 4}
-    alpha = 0.2
-    gamma = 0.9
-
-    # Initialise an OptionAgent..
-    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
-
-    # This time, our initial q_values are not zero. We set them to their test values here.
-    # Our dummy environment returns a list containing the primitive action 1 as the available action
-    # in state_2. This action's value is set to be greater than zero, so it will be the best-valued action.
-    agent.q_table[(hash("state_1"), hash(option))] = initial_values["state_1, option"]
-    agent.q_table[hash("state_2"), hash(1)] = initial_values["state_2, 1"]
-
-    # Perform a macro-q learning update for our test option over a single time-step, where a reward of
-    # 1 was earned after transitioning from state_1 to state_2.
-    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
-
-    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
-        reward_trajectory[0] + gamma * initial_values["state_2, 1"] - initial_values["state_1, option"]
-    )
-
-
-# Test a macro_q_learning update over three time-steps, with initial q-values of zero.
-def test_three_step_macro_q_update_1():
-    # Set up dummy states, rewards, options, parameters etc. for the test.
-    state_trajectory = ["state_1", "state_2", "state_3", "state_4"]
-    reward_trajectory = [2, 3, 4]
-    option = DummyOption("test_option_1")
-    initial_values = {"state_1, option": 0, "state_2, option": 0, "state_3, option": 0, "state_4, 1": 0}
-    alpha = 0.2
-    gamma = 0.9
-
-    # Initialise an OptionAgent..
-    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
-
-    # Perform a macro-q learning update for our test option over three time-steps, as the option
-    # executes and causes our agent to navigate between the states in state_trajectory and earn
-    # the rewards in reward_trajectory.
-    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
-
-    # Ensure that the value of executing our test option in state_1 has been updated correctly.
-    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
-        reward_trajectory[0]
-        + gamma**1 * reward_trajectory[1]
-        + gamma**2 * reward_trajectory[2]
-        + gamma**3 * initial_values["state_4, 1"]
-        - initial_values["state_1, option"]
-    )
-
-    # Ensure that the value of executing our test option in state_2 has been updated correctly.
-    assert agent.q_table[(hash("state_2"), hash(option))] == initial_values["state_1, option"] + alpha * (
-        reward_trajectory[1]
-        + gamma**1 * reward_trajectory[2]
-        + gamma**2 * initial_values["state_4, 1"]
-        - initial_values["state_2, option"]
-    )
-
-    # Ensure that the value of executing our test option in state_3 has been updated correctly.
-    assert agent.q_table[(hash("state_3"), hash(option))] == initial_values["state_1, option"] + alpha * (
-        reward_trajectory[2] + gamma**1 * initial_values["state_4, 1"] - initial_values["state_3, option"]
-    )
-
-
-# Test a macro_q_learning update over three time-steps, with non-zero initial q-values.
-def test_three_step_macro_q_update_2():
-    # Set up dummy states, rewards, options, parameters etc. for the test.
-    state_trajectory = ["state_1", "state_2", "state_3", "state_4"]
-    reward_trajectory = [2, 3, 4]
-    option = DummyOption("test_option_1")
-    initial_values = {"state_1, option": 4, "state_2, option": 5, "state_3, option": 6, "state_4, 1": 7}
-    alpha = 0.2
-    gamma = 0.9
-
-    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
-
-    # This time, our initial q_values are not zero. We set them to their test values here.
-    # Our dummy environment returns a list containing the primitive action 1 as the available action
-    # in state_4. This action's value is set to be greater than zero, so it will be the best-valued action.
-    agent.q_table[(hash("state_1"), hash(option))] = initial_values["state_1, option"]
-    agent.q_table[(hash("state_2"), hash(option))] = initial_values["state_2, option"]
-    agent.q_table[(hash("state_3"), hash(option))] = initial_values["state_3, option"]
-    agent.q_table[hash("state_4"), hash(1)] = initial_values["state_4, 1"]
-
-    # Perform a macro-q learning update for our test option over three time-steps, as the option
-    # executes and causes our agent to navigate between the states in state_trajectory and earn
-    # the rewards in reward_trajectory.
-    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
-
-    # Ensure that the value of executing our test option in state_1 has been updated correctly.
-    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
-        reward_trajectory[0]
-        + gamma**1 * reward_trajectory[1]
-        + gamma**2 * reward_trajectory[2]
-        + gamma**3 * initial_values["state_4, 1"]
-        - initial_values["state_1, option"]
-    )
-
-    # Ensure that the value of executing our test option in state_2 has been updated correctly.
-    assert agent.q_table[(hash("state_2"), hash(option))] == initial_values["state_2, option"] + alpha * (
-        reward_trajectory[1]
-        + gamma**1 * reward_trajectory[2]
-        + gamma**2 * initial_values["state_4, 1"]
-        - initial_values["state_2, option"]
-    )
-
-    # Ensure that the value of executing our test option in state_3 has been updated correctly.
-    assert agent.q_table[(hash("state_3"), hash(option))] == initial_values["state_3, option"] + alpha * (
-        reward_trajectory[2] + gamma**1 * initial_values["state_4, 1"] - initial_values["state_3, option"]
-    )
+import pytest
+
+from simpleoptions import BaseOption, OptionAgent
+
+
+class DummyOption(BaseOption):
+    """
+    A dummy option for testing.
+
+    Returns a dummy action, (int 1), terminates with probability 1.0 in
+    every state, and can be initiated in any state.
+    """
+
+    def __init__(self, name):
+        self.name = name
+
+    def initiation(self, state):
+        return True
+
+    def policy(self, state, test=False):
+        return 1
+
+    def termination(self, state):
+        return 1.0
+
+    def __str__(self):
+        return self.name
+
+    def __hash__(self):
+        return hash(str(self))
+
+
+class DummyEnv:
+    """
+    Dummy class to pass in as an environment - implements only what we need.
+    """
+
+    def __init__(self):
+        return
+
+    def is_state_terminal(self, state):
+        return False
+
+    def get_available_options(self, state):
+        return [1]
+
+
+# Test a macro_q_learning update over a single time-step, with initial q-values of zero.
+def test_one_step_macro_q_update_1():
+    # Set up dummy states, rewards, options, parameters etc. for the test.
+    state_trajectory = ["state_1", "state_2"]
+    reward_trajectory = [1]
+    option = DummyOption("test_option_1")
+    initial_values = {"state_1, option": 0, "state_2, 1": 0}
+    alpha = 0.2
+    gamma = 0.9
+
+    # Initialise an OptionAgent (note that initial q-values for all states are zero by default).
+    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
+
+    # Perform a macro-q learning update for our test option over a single time-step, where a reward of
+    # 1 was earned after transitioning from state_1 to state_2.
+    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
+
+    # Ensure that the new value of initating our test option in state_1 is correct after performing the update.
+    # Our dummy environment returns a list containing the primitive action 1 as the available action in state_2,
+    # and its value will be zero (we assume that this is the first update, and initial q-valaues are zero by default).
+    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
+        reward_trajectory[0] + gamma * initial_values["state_2, 1"] - initial_values["state_1, option"]
+    )
+
+
+# Test a macro_q_learning update over a single time-step, with non-zero initial q-values.
+def test_one_step_macro_q_update_2():
+    # Set up dummy states, rewards, options, parameters etc. for the test.
+    state_trajectory = ["state_1", "state_2"]
+    reward_trajectory = [1]
+    option = DummyOption("test_option_1")
+    initial_values = {"state_1, option": 2, "state_2, 1": 4}
+    alpha = 0.2
+    gamma = 0.9
+
+    # Initialise an OptionAgent..
+    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
+
+    # This time, our initial q_values are not zero. We set them to their test values here.
+    # Our dummy environment returns a list containing the primitive action 1 as the available action
+    # in state_2. This action's value is set to be greater than zero, so it will be the best-valued action.
+    agent.q_table[(hash("state_1"), hash(option))] = initial_values["state_1, option"]
+    agent.q_table[hash("state_2"), hash(1)] = initial_values["state_2, 1"]
+
+    # Perform a macro-q learning update for our test option over a single time-step, where a reward of
+    # 1 was earned after transitioning from state_1 to state_2.
+    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
+
+    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
+        reward_trajectory[0] + gamma * initial_values["state_2, 1"] - initial_values["state_1, option"]
+    )
+
+
+# Test a macro_q_learning update over three time-steps, with initial q-values of zero.
+def test_three_step_macro_q_update_1():
+    # Set up dummy states, rewards, options, parameters etc. for the test.
+    state_trajectory = ["state_1", "state_2", "state_3", "state_4"]
+    reward_trajectory = [2, 3, 4]
+    option = DummyOption("test_option_1")
+    initial_values = {
+        "state_1, option": 0,
+        "state_2, option": 0,
+        "state_3, option": 0,
+        "state_4, 1": 0,
+    }
+    alpha = 0.2
+    gamma = 0.9
+
+    # Initialise an OptionAgent..
+    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
+
+    # Perform a macro-q learning update for our test option over three time-steps, as the option
+    # executes and causes our agent to navigate between the states in state_trajectory and earn
+    # the rewards in reward_trajectory.
+    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
+
+    # Ensure that the value of executing our test option in state_1 has been updated correctly.
+    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
+        reward_trajectory[0]
+        + gamma**1 * reward_trajectory[1]
+        + gamma**2 * reward_trajectory[2]
+        + gamma**3 * initial_values["state_4, 1"]
+        - initial_values["state_1, option"]
+    )
+
+    # Ensure that the value of executing our test option in state_2 has been updated correctly.
+    assert agent.q_table[(hash("state_2"), hash(option))] == initial_values["state_1, option"] + alpha * (
+        reward_trajectory[1]
+        + gamma**1 * reward_trajectory[2]
+        + gamma**2 * initial_values["state_4, 1"]
+        - initial_values["state_2, option"]
+    )
+
+    # Ensure that the value of executing our test option in state_3 has been updated correctly.
+    assert agent.q_table[(hash("state_3"), hash(option))] == initial_values["state_1, option"] + alpha * (
+        reward_trajectory[2] + gamma**1 * initial_values["state_4, 1"] - initial_values["state_3, option"]
+    )
+
+
+# Test a macro_q_learning update over three time-steps, with non-zero initial q-values.
+def test_three_step_macro_q_update_2():
+    # Set up dummy states, rewards, options, parameters etc. for the test.
+    state_trajectory = ["state_1", "state_2", "state_3", "state_4"]
+    reward_trajectory = [2, 3, 4]
+    option = DummyOption("test_option_1")
+    initial_values = {
+        "state_1, option": 4,
+        "state_2, option": 5,
+        "state_3, option": 6,
+        "state_4, 1": 7,
+    }
+    alpha = 0.2
+    gamma = 0.9
+
+    agent = OptionAgent(DummyEnv(), macro_alpha=alpha, gamma=gamma)
+
+    # This time, our initial q_values are not zero. We set them to their test values here.
+    # Our dummy environment returns a list containing the primitive action 1 as the available action
+    # in state_4. This action's value is set to be greater than zero, so it will be the best-valued action.
+    agent.q_table[(hash("state_1"), hash(option))] = initial_values["state_1, option"]
+    agent.q_table[(hash("state_2"), hash(option))] = initial_values["state_2, option"]
+    agent.q_table[(hash("state_3"), hash(option))] = initial_values["state_3, option"]
+    agent.q_table[hash("state_4"), hash(1)] = initial_values["state_4, 1"]
+
+    # Perform a macro-q learning update for our test option over three time-steps, as the option
+    # executes and causes our agent to navigate between the states in state_trajectory and earn
+    # the rewards in reward_trajectory.
+    agent.macro_q_learn(state_trajectory, reward_trajectory, option, n_step=True)
+
+    # Ensure that the value of executing our test option in state_1 has been updated correctly.
+    assert agent.q_table[(hash("state_1"), hash(option))] == initial_values["state_1, option"] + alpha * (
+        reward_trajectory[0]
+        + gamma**1 * reward_trajectory[1]
+        + gamma**2 * reward_trajectory[2]
+        + gamma**3 * initial_values["state_4, 1"]
+        - initial_values["state_1, option"]
+    )
+
+    # Ensure that the value of executing our test option in state_2 has been updated correctly.
+    assert agent.q_table[(hash("state_2"), hash(option))] == initial_values["state_2, option"] + alpha * (
+        reward_trajectory[1]
+        + gamma**1 * reward_trajectory[2]
+        + gamma**2 * initial_values["state_4, 1"]
+        - initial_values["state_2, option"]
+    )
+
+    # Ensure that the value of executing our test option in state_3 has been updated correctly.
+    assert agent.q_table[(hash("state_3"), hash(option))] == initial_values["state_3, option"] + alpha * (
+        reward_trajectory[2] + gamma**1 * initial_values["state_4, 1"] - initial_values["state_3, option"]
+    )
```

