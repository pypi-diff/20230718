# Comparing `tmp/une_ai-1.1.2.tar.gz` & `tmp/une_ai-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "une_ai-1.1.2.tar", last modified: Thu Jul  6 02:32:11 2023, max compression
+gzip compressed data, was "une_ai-1.1.3.tar", last modified: Tue Jul 18 05:48:57 2023, max compression
```

## Comparing `une_ai-1.1.2.tar` & `une_ai-1.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.318954 une_ai-1.1.2/
--rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.1.2/LICENSE
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-07-06 02:32:11.318806 une_ai-1.1.2/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.1.2/README.md
--rw-r--r--   0 jonathan   (501) staff       (20)      481 2023-07-06 02:31:19.000000 une_ai-1.1.2/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-07-06 02:32:11.318999 une_ai-1.1.2/setup.cfg
--rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.1.2/setup.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.310082 une_ai-1.1.2/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.311252 une_ai-1.1.2/src/une_ai/
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.1.2/src/une_ai/__init__.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.313753 une_ai-1.1.2/src/une_ai/assignments/
--rw-r--r--   0 jonathan   (501) staff       (20)      198 2023-06-17 05:23:26.000000 une_ai-1.1.2/src/une_ai/assignments/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)    12875 2023-06-25 01:46:33.000000 une_ai-1.1.2/src/une_ai/assignments/connect_four_base_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     9726 2023-07-03 03:32:39.000000 une_ai-1.1.2/src/une_ai/assignments/connect_four_game.py
--rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.1.2/src/une_ai/assignments/snake_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     6359 2023-07-05 01:56:22.000000 une_ai-1.1.2/src/une_ai/assignments/snake_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.316305 une_ai-1.1.2/src/une_ai/models/
--rw-r--r--   0 jonathan   (501) staff       (20)     1323 2023-06-25 00:13:50.000000 une_ai-1.1.2/src/une_ai/models/MCTS_graph_node.py
--rw-r--r--   0 jonathan   (501) staff       (20)      254 2023-06-24 12:38:18.000000 une_ai-1.1.2/src/une_ai/models/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.1.2/src/une_ai/models/agent.py
--rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.1.2/src/une_ai/models/environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1083 2023-06-22 07:56:49.000000 une_ai-1.1.2/src/une_ai/models/game_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1312 2023-06-12 07:15:34.000000 une_ai-1.1.2/src/une_ai/models/graph_node.py
--rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.1.2/src/une_ai/models/grid_map.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5827 2023-06-24 06:33:53.000000 une_ai-1.1.2/src/une_ai/models/transposition_table.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.317226 une_ai-1.1.2/src/une_ai/tictactoe/
--rw-r--r--   0 jonathan   (501) staff       (20)       87 2023-06-25 01:53:59.000000 une_ai-1.1.2/src/une_ai/tictactoe/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1313 2023-07-04 01:51:27.000000 une_ai-1.1.2/src/une_ai/tictactoe/tictactoc_player.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5517 2023-07-04 04:24:19.000000 une_ai-1.1.2/src/une_ai/tictactoe/tictactoe_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.318446 une_ai-1.1.2/src/une_ai/vacuum/
--rw-r--r--   0 jonathan   (501) staff       (20)      186 2023-06-12 02:00:34.000000 une_ai-1.1.2/src/une_ai/vacuum/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)      910 2023-06-12 07:14:58.000000 une_ai-1.1.2/src/une_ai/vacuum/vacuum_dock_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.1.2/src/une_ai/vacuum/vacuum_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     6332 2023-07-05 01:33:24.000000 une_ai-1.1.2/src/une_ai/vacuum/vacuum_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.312136 une_ai-1.1.2/src/une_ai.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      978 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       19 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.953352 une_ai-1.1.3/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.1.3/LICENSE
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-07-18 05:48:57.953197 une_ai-1.1.3/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.1.3/README.md
+-rw-r--r--   0 jonathan   (501) staff       (20)      498 2023-07-18 05:48:08.000000 une_ai-1.1.3/pyproject.toml
+-rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-07-18 05:48:57.953397 une_ai-1.1.3/setup.cfg
+-rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.1.3/setup.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.945219 une_ai-1.1.3/src/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.946682 une_ai-1.1.3/src/une_ai/
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.1.3/src/une_ai/__init__.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.948998 une_ai-1.1.3/src/une_ai/assignments/
+-rw-r--r--   0 jonathan   (501) staff       (20)      198 2023-06-17 05:23:26.000000 une_ai-1.1.3/src/une_ai/assignments/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)    12875 2023-06-25 01:46:33.000000 une_ai-1.1.3/src/une_ai/assignments/connect_four_base_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     9726 2023-07-03 03:32:39.000000 une_ai-1.1.3/src/une_ai/assignments/connect_four_game.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.1.3/src/une_ai/assignments/snake_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     6359 2023-07-05 01:56:22.000000 une_ai-1.1.3/src/une_ai/assignments/snake_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.951011 une_ai-1.1.3/src/une_ai/models/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1323 2023-06-25 00:13:50.000000 une_ai-1.1.3/src/une_ai/models/MCTS_graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      254 2023-07-18 05:47:22.000000 une_ai-1.1.3/src/une_ai/models/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.1.3/src/une_ai/models/agent.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.1.3/src/une_ai/models/environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1083 2023-06-22 07:56:49.000000 une_ai-1.1.3/src/une_ai/models/game_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1312 2023-06-12 07:15:34.000000 une_ai-1.1.3/src/une_ai/models/graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.1.3/src/une_ai/models/grid_map.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5827 2023-06-24 06:33:53.000000 une_ai-1.1.3/src/une_ai/models/transposition_table.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.951768 une_ai-1.1.3/src/une_ai/tictactoe/
+-rw-r--r--   0 jonathan   (501) staff       (20)       87 2023-06-25 01:53:59.000000 une_ai-1.1.3/src/une_ai/tictactoe/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1313 2023-07-04 01:51:27.000000 une_ai-1.1.3/src/une_ai/tictactoe/tictactoc_player.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5517 2023-07-04 04:24:19.000000 une_ai-1.1.3/src/une_ai/tictactoe/tictactoe_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.952845 une_ai-1.1.3/src/une_ai/vacuum/
+-rw-r--r--   0 jonathan   (501) staff       (20)      186 2023-06-12 02:00:34.000000 une_ai-1.1.3/src/une_ai/vacuum/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      910 2023-06-12 07:14:58.000000 une_ai-1.1.3/src/une_ai/vacuum/vacuum_dock_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.1.3/src/une_ai/vacuum/vacuum_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     6332 2023-07-05 01:33:24.000000 une_ai-1.1.3/src/une_ai/vacuum/vacuum_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-18 05:48:57.947621 une_ai-1.1.3/src/une_ai.egg-info/
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-07-18 05:48:57.000000 une_ai-1.1.3/src/une_ai.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)      978 2023-07-18 05:48:57.000000 une_ai-1.1.3/src/une_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-07-18 05:48:57.000000 une_ai-1.1.3/src/une_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)       29 2023-07-18 05:48:57.000000 une_ai-1.1.3/src/une_ai.egg-info/requires.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-07-18 05:48:57.000000 une_ai-1.1.3/src/une_ai.egg-info/top_level.txt
```

### Comparing `une_ai-1.1.2/LICENSE` & `une_ai-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/PKG-INFO` & `une_ai-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une_ai
-Version: 1.1.2
+Version: 1.1.3
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.1.2/README.md` & `une_ai-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/assignments/connect_four_base_environment.py` & `une_ai-1.1.3/src/une_ai/assignments/connect_four_base_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/assignments/connect_four_game.py` & `une_ai-1.1.3/src/une_ai/assignments/connect_four_game.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/assignments/snake_environment.py` & `une_ai-1.1.3/src/une_ai/assignments/snake_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/assignments/snake_game.py` & `une_ai-1.1.3/src/une_ai/assignments/snake_game.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/models/MCTS_graph_node.py` & `une_ai-1.1.3/src/une_ai/models/MCTS_graph_node.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/models/agent.py` & `une_ai-1.1.3/src/une_ai/models/agent.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/models/game_environment.py` & `une_ai-1.1.3/src/une_ai/models/game_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/models/graph_node.py` & `une_ai-1.1.3/src/une_ai/models/graph_node.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/models/grid_map.py` & `une_ai-1.1.3/src/une_ai/models/grid_map.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/models/transposition_table.py` & `une_ai-1.1.3/src/une_ai/models/transposition_table.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/tictactoe/tictactoc_player.py` & `une_ai-1.1.3/src/une_ai/tictactoe/tictactoc_player.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/tictactoe/tictactoe_game.py` & `une_ai-1.1.3/src/une_ai/tictactoe/tictactoe_game.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/vacuum/vacuum_dock_environment.py` & `une_ai-1.1.3/src/une_ai/vacuum/vacuum_dock_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/vacuum/vacuum_environment.py` & `une_ai-1.1.3/src/une_ai/vacuum/vacuum_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai/vacuum/vacuum_game.py` & `une_ai-1.1.3/src/une_ai/vacuum/vacuum_game.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.2/src/une_ai.egg-info/PKG-INFO` & `une_ai-1.1.3/src/une_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une-ai
-Version: 1.1.2
+Version: 1.1.3
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.1.2/src/une_ai.egg-info/SOURCES.txt` & `une_ai-1.1.3/src/une_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

