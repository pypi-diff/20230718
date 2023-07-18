# Comparing `tmp/playgroundrl_envs-0.0.6.tar.gz` & `tmp/playgroundrl_envs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl_envs-0.0.6.tar", last modified: Wed Jun 28 19:03:07 2023, max compression
+gzip compressed data, was "playgroundrl_envs-0.0.7.tar", last modified: Sat Jul  8 16:38:22 2023, max compression
```

## Comparing `playgroundrl_envs-0.0.6.tar` & `playgroundrl_envs-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.825520 playgroundrl_envs-0.0.6/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-28 19:03:07.825604 playgroundrl_envs-0.0.6/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      201 2023-06-04 00:27:10.000000 playgroundrl_envs-0.0.6/README.md
--rw-r--r--   0 rayan      (501) staff       (20)       38 2023-06-28 19:03:07.825852 playgroundrl_envs-0.0.6/setup.cfg
--rw-r--r--   0 rayan      (501) staff       (20)      664 2023-06-28 19:03:01.000000 playgroundrl_envs-0.0.6/setup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.820616 playgroundrl_envs-0.0.6/src/
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.822073 playgroundrl_envs-0.0.6/src/playgroundrl_envs/
--rw-r--r--   0 rayan      (501) staff       (20)     2939 2023-05-22 16:32:00.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/game_interface.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.823942 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-28 19:01:37.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/__init__.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.824337 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/catan/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-28 19:01:42.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/catan/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     5442 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/catan/catan.py
--rw-r--r--   0 rayan      (501) staff       (20)     9605 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/catan/encoder.py
--rw-r--r--   0 rayan      (501) staff       (20)     3857 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/chess.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.824598 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/codenames/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-28 19:01:47.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/codenames/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     7799 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/codenames/codenames.py
--rw-r--r--   0 rayan      (501) staff       (20)      517 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/coup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.824853 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-28 19:01:53.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/__init__.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.825387 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/engine/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-06-28 19:01:58.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/engine/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)    14656 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/engine/gogame.py
--rw-r--r--   0 rayan      (501) staff       (20)      117 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/engine/govars.py
--rw-r--r--   0 rayan      (501) staff       (20)    10833 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/engine/state_utils.py
--rw-r--r--   0 rayan      (501) staff       (20)     3656 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/go.py
--rw-r--r--   0 rayan      (501) staff       (20)     4934 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/mining_decarbonization.py
--rw-r--r--   0 rayan      (501) staff       (20)     3201 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/petting_zoo.py
--rw-r--r--   0 rayan      (501) staff       (20)     9059 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/poker.py
--rw-r--r--   0 rayan      (501) staff       (20)     3176 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/snake.py
--rw-r--r--   0 rayan      (501) staff       (20)     3707 2023-06-28 17:36:32.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/tic_tac_toe.py
--rw-r--r--   0 rayan      (501) staff       (20)      832 2023-06-04 23:55:41.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs/sid_util.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-06-28 19:03:07.822793 playgroundrl_envs-0.0.6/src/playgroundrl_envs.egg-info/
--rw-r--r--   0 rayan      (501) staff       (20)      192 2023-06-28 19:03:07.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs.egg-info/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)     1167 2023-06-28 19:03:07.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs.egg-info/SOURCES.txt
--rw-r--r--   0 rayan      (501) staff       (20)        1 2023-06-28 19:03:07.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs.egg-info/dependency_links.txt
--rw-r--r--   0 rayan      (501) staff       (20)       29 2023-06-28 19:03:07.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs.egg-info/requires.txt
--rw-r--r--   0 rayan      (501) staff       (20)       18 2023-06-28 19:03:07.000000 playgroundrl_envs-0.0.6/src/playgroundrl_envs.egg-info/top_level.txt
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:38:22.791471 playgroundrl_envs-0.0.7/
+-rw-r--r--   0 langston   (501) staff       (20)      192 2023-07-08 16:38:22.796744 playgroundrl_envs-0.0.7/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      201 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/README.md
+-rw-r--r--   0 langston   (501) staff       (20)       38 2023-07-08 16:38:22.797340 playgroundrl_envs-0.0.7/setup.cfg
+-rw-r--r--   0 langston   (501) staff       (20)     1096 2023-07-08 16:37:50.000000 playgroundrl_envs-0.0.7/setup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:34:55.959957 playgroundrl_envs-0.0.7/src/
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:34:55.963018 playgroundrl_envs-0.0.7/src/playgroundrl_envs/
+-rw-r--r--   0 langston   (501) staff       (20)     2939 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/game_interface.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:34:55.967574 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/__init__.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:34:55.968482 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/catan/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/catan/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     5442 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/catan/catan.py
+-rw-r--r--   0 langston   (501) staff       (20)     9605 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/catan/encoder.py
+-rw-r--r--   0 langston   (501) staff       (20)     3857 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/chess.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:38:22.795567 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/codenames/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/codenames/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     8081 2023-07-08 04:07:48.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/codenames/codenames.py
+-rw-r--r--   0 langston   (501) staff       (20)     2481 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/codenames/wordlist.txt
+-rw-r--r--   0 langston   (501) staff       (20)      517 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/coup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:34:55.969951 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/__init__.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:34:55.971279 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/engine/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/engine/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)    14656 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/engine/gogame.py
+-rw-r--r--   0 langston   (501) staff       (20)      117 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/engine/govars.py
+-rw-r--r--   0 langston   (501) staff       (20)    10833 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/engine/state_utils.py
+-rw-r--r--   0 langston   (501) staff       (20)     3656 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/go.py
+-rw-r--r--   0 langston   (501) staff       (20)     4934 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/mining_decarbonization.py
+-rw-r--r--   0 langston   (501) staff       (20)     3201 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/petting_zoo.py
+-rw-r--r--   0 langston   (501) staff       (20)     9059 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/poker.py
+-rw-r--r--   0 langston   (501) staff       (20)     3176 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/snake.py
+-rw-r--r--   0 langston   (501) staff       (20)     3707 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/tic_tac_toe.py
+-rw-r--r--   0 langston   (501) staff       (20)      832 2023-06-29 00:59:53.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs/sid_util.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-07-08 16:38:22.794292 playgroundrl_envs-0.0.7/src/playgroundrl_envs.egg-info/
+-rw-r--r--   0 langston   (501) staff       (20)      192 2023-07-08 16:38:22.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs.egg-info/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)     1218 2023-07-08 16:38:22.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs.egg-info/SOURCES.txt
+-rw-r--r--   0 langston   (501) staff       (20)        1 2023-07-08 16:38:22.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs.egg-info/dependency_links.txt
+-rw-r--r--   0 langston   (501) staff       (20)      207 2023-07-08 16:38:22.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs.egg-info/requires.txt
+-rw-r--r--   0 langston   (501) staff       (20)       18 2023-07-08 16:38:22.000000 playgroundrl_envs-0.0.7/src/playgroundrl_envs.egg-info/top_level.txt
```

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/game_interface.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/game_interface.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/catan/catan.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/catan/catan.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/catan/encoder.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/catan/encoder.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/chess.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/chess.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/codenames/codenames.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/codenames/codenames.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,47 +148,52 @@
 
     def submit_action(self, action, player_sid=""):
         if self.player_moving.sid != player_sid:
             return False
 
         # TODO: This isn't necessary
         action = json.loads(action)
+        print("ACTION", action)
         player_color = self.player_moving.color
 
         if self.player_moving.type == PlayerType.GIVER:
             word = action["word"].lower()
             # if not DICTIONARY.check(word):
             #     print("RECEIVED INVALID WORD -- words must be english")
             #     return False
-
+            print("WORD", word)
             # Can't use same word as on board
             for row in self.words:
                 for board_word in row:
                     if word == board_word:
+                        print("WORD ON BOARD")
                         return False
 
             count = int(action["count"])
 
             if count < 0 or count > 9:
+                print("BAD COUNT")
                 return False
 
             self.last_clue = word
             self.last_count = count
 
             self.increment_turn()
         else:
             row, col = action["guess"]
             if row == col == -1:
                 # -1, -1 represents finishing your turn
                 self.increment_turn()
             else:
                 if not 0 <= row < BOARD_SIZE or not 0 <= col < BOARD_SIZE:
+                    print("GUESSED BAD ROW  OR COL")
                     return False
 
                 if self.guessed_colors[row][col] != Color.UNKNOWN:
+                    print("GUESSED ALREADY GUESSED COLOR")
                     return False
 
                 color = self.actual_colors[row][col]
                 self.guessed_colors[row][col] = color
 
                 if color == Color.ASSASSIN:
                     self.is_game_over = True
@@ -215,15 +220,15 @@
 
                     if self.scores[Color.BLUE] == BLUE_CARDS:
                         self.is_game_over = True
                         self.winning_team = Color.BLUE
                     elif self.scores[Color.RED] == RED_CARDS:
                         self.is_game_over = True
                         self.winning_team = Color.RED
-
+        print("SUCCESSS")
         return True  # Success
 
     def get_state(self, player_sid="", player_id=-1):
         # TODO: Smarter
         if player_id == -1:
             player_id = 0
```

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/coup.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/coup.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/engine/gogame.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/engine/gogame.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/engine/state_utils.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/engine/state_utils.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/go/go.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/go/go.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/mining_decarbonization.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/mining_decarbonization.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/petting_zoo.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/petting_zoo.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/poker.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/poker.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/snake.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/snake.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/games/tic_tac_toe.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/games/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs/sid_util.py` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs/sid_util.py`

 * *Files identical despite different names*

### Comparing `playgroundrl_envs-0.0.6/src/playgroundrl_envs.egg-info/SOURCES.txt` & `playgroundrl_envs-0.0.7/src/playgroundrl_envs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 src/playgroundrl_envs/games/snake.py
 src/playgroundrl_envs/games/tic_tac_toe.py
 src/playgroundrl_envs/games/catan/__init__.py
 src/playgroundrl_envs/games/catan/catan.py
 src/playgroundrl_envs/games/catan/encoder.py
 src/playgroundrl_envs/games/codenames/__init__.py
 src/playgroundrl_envs/games/codenames/codenames.py
+src/playgroundrl_envs/games/codenames/wordlist.txt
 src/playgroundrl_envs/games/go/__init__.py
 src/playgroundrl_envs/games/go/go.py
 src/playgroundrl_envs/games/go/engine/__init__.py
 src/playgroundrl_envs/games/go/engine/gogame.py
 src/playgroundrl_envs/games/go/engine/govars.py
 src/playgroundrl_envs/games/go/engine/state_utils.py
```

