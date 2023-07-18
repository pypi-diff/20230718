# Comparing `tmp/letterenv-0.1.3.tar.gz` & `tmp/letterenv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterenv-0.1.3.tar", max compression
+gzip compressed data, was "letterenv-0.1.4.tar", max compression
```

## Comparing `letterenv-0.1.3.tar` & `letterenv-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       13 2023-07-17 12:55:47.855819 letterenv-0.1.3/README.md
--rw-r--r--   0        0        0       42 2023-07-09 13:43:03.544543 letterenv-0.1.3/letterenv/__init__.py
--rw-r--r--   0        0        0     5899 2023-07-17 13:07:17.581799 letterenv-0.1.3/letterenv/letterenv.py
--rw-r--r--   0        0        0      506 2023-07-17 13:08:45.237161 letterenv-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 letterenv-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-07-17 12:55:47.855819 letterenv-0.1.4/README.md
+-rw-r--r--   0        0        0       42 2023-07-09 13:43:03.544543 letterenv-0.1.4/letterenv/__init__.py
+-rw-r--r--   0        0        0     6104 2023-07-18 19:17:28.289088 letterenv-0.1.4/letterenv/letterenv.py
+-rw-r--r--   0        0        0      506 2023-07-18 19:18:12.263342 letterenv-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 letterenv-0.1.4/PKG-INFO
```

### Comparing `letterenv-0.1.3/letterenv/letterenv.py` & `letterenv-0.1.4/letterenv/letterenv.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         self.active_propositions = {pos: p for p, pos in self.locations.items()}
 
         # Set agent initial position
         self.agent_position = self.agent_start_location
         return self._construct_observation(), {}
 
     def step(self, action: int):
+        self.n_steps += 1
         # Move agent in environment
         self._update_agent_position(action)
 
         # Calculate which propositions are true in the environment
         if self.agent_position in self.active_propositions:
             obs_prop = self.active_propositions[self.agent_position]
 
@@ -92,38 +93,45 @@
 
             if self.prop_obs_counts[prop_idx] == self.max_observation_counts[obs_prop]:
                 # Replace proposition with next proposition in replacement mapping
                 self.active_propositions[
                     self.agent_position
                 ] = self.replacement_mapping[obs_prop]
 
-            if obs_prop == self.task_string[self.task_string_idx]:
-                if self.task_string_idx < len(self.task_string):
+            try:
+                if obs_prop == self.task_string[self.task_string_idx]:
                     self.task_string_idx += 1
-            else:
-                self.task_failed = True
-                print("Failed task")
-
+                else:
+                    self.task_failed = True
+            except IndexError:
+                pass
         else:
             obs_prop = "_"
 
         obs = self._construct_observation()
 
         # Determine if episode is terminated due to max number of steps
         if self.spec is not None and self.spec.max_episode_steps == self.n_steps:
             terminated = True
             # Episode ended based on condition outside MDP (interface for more details)
             truncated = True
             reward = 0
         else:
-            terminated = not self.task_failed and self.task_string_idx == len(
-                self.task_string
-            )
-            truncated = False
-            reward = 1 if terminated else 0
+            if self.task_failed:
+                terminated = True
+                truncated = False
+                reward = 0
+            elif self.task_string_idx == len(self.task_string):
+                terminated = True
+                truncated = False
+                reward = 1
+            else:
+                terminated = False
+                truncated = False
+                reward = 0
 
         return (
             obs,
             reward,
             terminated,
             truncated,
             {},
```

