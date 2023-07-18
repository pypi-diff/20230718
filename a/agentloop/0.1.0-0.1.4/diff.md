# Comparing `tmp/agentloop-0.1.0.tar.gz` & `tmp/agentloop-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentloop-0.1.0.tar", last modified: Sun Jul 16 00:05:33 2023, max compression
+gzip compressed data, was "agentloop-0.1.4.tar", last modified: Tue Jul 18 14:03:58 2023, max compression
```

## Comparing `agentloop-0.1.0.tar` & `agentloop-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:05:33.924559 agentloop-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 00:05:19.000000 agentloop-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-16 00:05:33.924559 agentloop-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-16 00:05:19.000000 agentloop-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:05:33.924559 agentloop-0.1.0/agentloop/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-16 00:05:19.000000 agentloop-0.1.0/agentloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-16 00:05:19.000000 agentloop-0.1.0/agentloop/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:05:33.924559 agentloop-0.1.0/agentloop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-16 00:05:33.000000 agentloop-0.1.0/agentloop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-16 00:05:33.000000 agentloop-0.1.0/agentloop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 00:05:33.000000 agentloop-0.1.0/agentloop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 00:05:33.000000 agentloop-0.1.0/agentloop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 00:05:33.000000 agentloop-0.1.0/agentloop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 00:05:33.924559 agentloop-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-16 00:05:19.000000 agentloop-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:58.948129 agentloop-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-18 14:03:46.000000 agentloop-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-18 14:03:58.948129 agentloop-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-18 14:03:46.000000 agentloop-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:58.948129 agentloop-0.1.4/agentloop/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:58.948129 agentloop-0.1.4/agentloop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:03:58.948129 agentloop-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-18 14:03:46.000000 agentloop-0.1.4/setup.py
```

### Comparing `agentloop-0.1.0/LICENSE` & `agentloop-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentloop-0.1.0/PKG-INFO` & `agentloop-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.1.0
+Version: 0.1.4
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentloop-0.1.0/README.md` & `agentloop-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `agentloop-0.1.0/agentloop/main.py` & `agentloop-0.1.4/agentloop/loop.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,9 @@
 import threading
 
-from pynput import keyboard
-
-
-def stop(loop_data):
-    """
-    Function to handle stopping of the loop
-        loop_data: a dictionary containing threading events related to the loop
-            (You should pass in the object created by the start function)
-    """
-
-    listener = loop_data.get("listener", None)
-    stop_event = loop_data["stop_event"]
-    stop_event.set()
-    if listener is not None and listener.running:
-        listener.stop()
-    loop_data["thread"].join(timeout=10)
-
-
-def step(loop_data):
-    """
-    Function to perform a single step in the loop
-
-    Args:
-        loop_data: loop data object, created by the start function
-
-    This function does not return any value.
-    """
-    loop_data["step_event"].set()
-
 
 def start(steps, stepped=False):
     """
     Function to start the main loop
 
     Args:
         stepped: boolean - whether the loop should run one-step-at-a-time.
@@ -53,14 +24,44 @@
 
     thread.start()
     loop_data["started_event"].wait()  # Wait here until loop is started
 
     return loop_data
 
 
+def stop(loop_data):
+    """
+    Function to handle stopping of the loop
+        loop_data: a dictionary containing threading events related to the loop
+            (You should pass in the object created by the start function)
+    """
+
+    listener = loop_data.get("listener", None)
+    stop_event = loop_data["stop_event"]
+    stop_event.set()
+    if listener is not None and listener.running:
+        listener.stop()
+    try:
+        loop_data["thread"].join(timeout=10)
+    except RuntimeError:
+        pass
+
+
+def step(loop_data):
+    """
+    Function to perform a single step in the loop
+
+    Args:
+        loop_data: loop data object, created by the start function
+
+    This function does not return any value.
+    """
+    loop_data["step_event"].set()
+
+
 def loop(steps, stepped=False, loop_data=None):
     """
     Run the step array in a loop until stopped
 
     Args:
         steps: array of functions to be run in the loop
         stepped: boolean - whether the loop should run in stepped mode or not
@@ -99,29 +100,7 @@
                 if loop_data["stop_event"].is_set():
                     break
                 loop_data["step_event"].clear()
         if loop_data["stop_event"].is_set():
             break
 
 
-def use_keyboard(loop_data, input_key=keyboard.Key.space):
-    """
-    Listen for a specified key press, and when detected, step the loop
-
-    Args:
-        loop_data: loop data object, created by the start function
-        input_key: The keyboard key which the listener will react to
-            Defaults to keyboard.Key.space
-
-    Returns:
-        loop_data: The updated loop dictionary with the newly created listener
-    """
-
-    def on_press(key):
-        if key == input_key:
-            loop_data["step_event"].set()
-
-    listener = None
-    listener = keyboard.Listener(on_press=on_press)
-    listener.start()
-    loop_data["listener"] = listener
-    return loop_data
```

### Comparing `agentloop-0.1.0/agentloop.egg-info/PKG-INFO` & `agentloop-0.1.4/agentloop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.1.0
+Version: 0.1.4
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentloop-0.1.0/setup.py` & `agentloop-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentloop",
-    version="0.1.0",
+    version="0.1.4",
     description="A simple, lightweight loop for your agent.",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentloop",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

