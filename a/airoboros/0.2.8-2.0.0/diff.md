# Comparing `tmp/airoboros-0.2.8.tar.gz` & `tmp/airoboros-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-0.2.8.tar", last modified: Sun Jun 25 10:36:09 2023, max compression
+gzip compressed data, was "airoboros-2.0.0.tar", last modified: Tue Jul 18 18:05:42 2023, max compression
```

## Comparing `airoboros-0.2.8.tar` & `airoboros-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:36:09.951199 airoboros-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 10:35:56.000000 airoboros-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-25 10:36:09.951199 airoboros-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-25 10:35:56.000000 airoboros-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:36:09.947199 airoboros-0.2.8/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 10:35:56.000000 airoboros-0.2.8/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-25 10:35:56.000000 airoboros-0.2.8/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-25 10:35:56.000000 airoboros-0.2.8/airoboros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    43192 2023-06-25 10:35:56.000000 airoboros-0.2.8/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:36:09.951199 airoboros-0.2.8/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-25 10:36:09.000000 airoboros-0.2.8/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 10:36:09.000000 airoboros-0.2.8/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:36:09.000000 airoboros-0.2.8/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-25 10:36:09.000000 airoboros-0.2.8/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-25 10:36:09.000000 airoboros-0.2.8/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-25 10:36:09.000000 airoboros-0.2.8/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 10:36:09.951199 airoboros-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-25 10:35:56.000000 airoboros-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:05:42.436813 airoboros-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 18:05:30.000000 airoboros-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-18 18:05:42.436813 airoboros-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-18 18:05:30.000000 airoboros-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:05:42.428813 airoboros-2.0.0/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:05:42.432813 airoboros-2.0.0/airoboros/instructors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/counterfactual_contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/experiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/inline_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/orca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:05:42.436813 airoboros-2.0.0/airoboros/instructors/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/agent.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/coding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/cot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/counterfactual_contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/counterfactual_contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/experience.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/general.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/orca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/riddle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/roleplay.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/trivia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/prompts/wordgame.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/riddles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/roleplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/simple_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/trivia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/instructors/wordgames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-07-18 18:05:30.000000 airoboros-2.0.0/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:05:42.428813 airoboros-2.0.0/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-18 18:05:42.000000 airoboros-2.0.0/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-18 18:05:42.000000 airoboros-2.0.0/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:05:42.000000 airoboros-2.0.0/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 18:05:42.000000 airoboros-2.0.0/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-18 18:05:42.000000 airoboros-2.0.0/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:05:42.000000 airoboros-2.0.0/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:05:42.436813 airoboros-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-18 18:05:30.000000 airoboros-2.0.0/setup.py
```

### Comparing `airoboros-0.2.8/LICENSE` & `airoboros-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-0.2.8/airoboros/entrypoint.py` & `airoboros-2.0.0/airoboros/entrypoint.py`

 * *Files identical despite different names*

