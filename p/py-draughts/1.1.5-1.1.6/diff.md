# Comparing `tmp/py-draughts-1.1.5.tar.gz` & `tmp/py-draughts-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.1.5.tar", last modified: Sun Jul 16 20:29:20 2023, max compression
+gzip compressed data, was "py-draughts-1.1.6.tar", last modified: Tue Jul 18 21:33:10 2023, max compression
```

## Comparing `py-draughts-1.1.5.tar` & `py-draughts-1.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.352927 py-draughts-1.1.5/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.5/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5226 2023-07-16 20:29:20.351925 py-draughts-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3806 2023-07-16 18:55:32.000000 py-draughts-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.323356 py-draughts-1.1.5/draughts/
--rw-rw-rw-   0        0        0     1585 2023-07-16 20:29:03.000000 py-draughts-1.1.5/draughts/__init__.py
--rw-rw-rw-   0        0        0     3666 2023-07-16 18:41:37.000000 py-draughts-1.1.5/draughts/american.py
--rw-rw-rw-   0        0        0    12410 2023-07-16 18:41:54.000000 py-draughts-1.1.5/draughts/base.py
--rw-rw-rw-   0        0        0     3663 2023-07-16 18:55:10.000000 py-draughts-1.1.5/draughts/engine.py
--rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.1.5/draughts/models.py
--rw-rw-rw-   0        0        0     4147 2023-07-16 18:11:26.000000 py-draughts-1.1.5/draughts/move.py
--rw-rw-rw-   0        0        0     5300 2023-07-16 18:11:04.000000 py-draughts-1.1.5/draughts/server.py
--rw-rw-rw-   0        0        0     8033 2023-07-16 20:18:47.000000 py-draughts-1.1.5/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.288272 py-draughts-1.1.5/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.324356 py-draughts-1.1.5/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.5/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.326356 py-draughts-1.1.5/draughts/static/js/
--rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.5/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.331877 py-draughts-1.1.5/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.5/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.5/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.5/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.346408 py-draughts-1.1.5/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5226 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 19:28:37.000000 py-draughts-1.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 20:29:20.352927 py-draughts-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1908 2023-07-16 09:45:04.000000 py-draughts-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.349926 py-draughts-1.1.5/test/
--rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.1.5/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.5/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:10.063147 py-draughts-1.1.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5199 2023-07-18 21:33:10.062147 py-draughts-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3779 2023-07-17 12:17:15.000000 py-draughts-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:10.009534 py-draughts-1.1.6/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-18 21:32:53.000000 py-draughts-1.1.6/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3666 2023-07-16 18:41:37.000000 py-draughts-1.1.6/draughts/american.py
+-rw-rw-rw-   0        0        0    12412 2023-07-18 21:25:14.000000 py-draughts-1.1.6/draughts/base.py
+-rw-rw-rw-   0        0        0     3663 2023-07-16 18:55:10.000000 py-draughts-1.1.6/draughts/engine.py
+-rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.1.6/draughts/models.py
+-rw-rw-rw-   0        0        0     4147 2023-07-16 18:11:26.000000 py-draughts-1.1.6/draughts/move.py
+-rw-rw-rw-   0        0        0     5607 2023-07-18 21:31:16.000000 py-draughts-1.1.6/draughts/server.py
+-rw-rw-rw-   0        0        0     8454 2023-07-18 21:30:46.000000 py-draughts-1.1.6/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:09.965992 py-draughts-1.1.6/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:10.017554 py-draughts-1.1.6/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.6/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:10.031148 py-draughts-1.1.6/draughts/static/js/
+-rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.6/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:10.034182 py-draughts-1.1.6/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.6/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.6/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.6/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:10.047147 py-draughts-1.1.6/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5199 2023-07-18 21:33:09.000000 py-draughts-1.1.6/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-18 21:33:09.000000 py-draughts-1.1.6/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:33:09.000000 py-draughts-1.1.6/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-18 21:33:09.000000 py-draughts-1.1.6/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 21:33:09.000000 py-draughts-1.1.6/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 19:28:37.000000 py-draughts-1.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 21:33:10.063147 py-draughts-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-16 09:45:04.000000 py-draughts-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:33:10.061148 py-draughts-1.1.6/test/
+-rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.1.6/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.6/test/test_board.py
```

### Comparing `py-draughts-1.1.5/LICENSE` & `py-draughts-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/PKG-INFO` & `py-draughts-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.5
+Version: 1.1.6
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -27,20 +27,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
-[![Downloads](https://static.pepy.tech/personalized-badge/py-draughts?period=month&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/py-draughts)
-
+[![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
+_inspired by [python-chess](https://pypi.org/project/chess/)_
+
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
```

### Comparing `py-draughts-1.1.5/README.md` & `py-draughts-1.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
-[![Downloads](https://static.pepy.tech/personalized-badge/py-draughts?period=month&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/py-draughts)
-
+[![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
+_inspired by [python-chess](https://pypi.org/project/chess/)_
+
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
```

### Comparing `py-draughts-1.1.5/draughts/__init__.py` & `py-draughts-1.1.6/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
 from typing import Literal
 
-__version__ = "1.1.5"
+__version__ = "1.1.6"
 __author__ = "Michał Skibiński"
 
 
 def get_board(variant: Literal["standard", "american"], fen: str = None):
     """
     Board factory method.
     - ``standard`` - standard draughts board
```

### Comparing `py-draughts-1.1.5/draughts/american.py` & `py-draughts-1.1.6/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/base.py` & `py-draughts-1.1.6/draughts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         Fen examples:
 
         - ``[FEN "B:W18,24,27,28,K10,K15:B12,16,20,K22,K25,K29"]``
         - ``[FEN "B:W18,19,21,23,24,26,29,30,31,32:B1,2,3,4,6,7,9,10,11,12"]``
         """
         COLORS_REPR = {Color.WHITE: "W", Color.BLACK: "B"}
         fen_components = [
-            f'[FEN "{COLORS_REPR[self.turn]}:W',
+            f'[FEN "W:{COLORS_REPR[self.turn]}:W',
             ",".join(
                 "K" * bool(self._pos[sq] < -1) + str(sq + 1)
                 for sq in np.where(self.position < 0)[0]
             ),
             ":B",
             ",".join(
                 "K" * bool(self._pos[sq] > 1) + str(sq + 1)
```

### Comparing `py-draughts-1.1.5/draughts/engine.py` & `py-draughts-1.1.6/draughts/engine.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/models.py` & `py-draughts-1.1.6/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/move.py` & `py-draughts-1.1.6/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/server.py` & `py-draughts-1.1.6/draughts/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,14 +110,17 @@
         )
         self.board._moves_stack = []
         self.board._pos = STARTING_POSITION
         return self.position_json
 
     def get_best_move(self, request: Request) -> PositionResponse:
         move = self.get_best_move_method(self.board)
+        if self.board.game_over:
+            print("Game over")
+            return self.position_json
         self.board.push(move)
         return self.position_json
 
     def move(self, request: Request, source: str, target: str) -> PositionResponse:
         move_str = f"{source}-{target}"
         self.board.push_uci(move_str)
         return self.position_json
@@ -137,11 +140,16 @@
 
     def run(self, **kwargs):
         uvicorn.run(self.APP, **kwargs)
 
 
 if __name__ == "__main__":
     from draughts.engine import AlphaBetaEngine
+    from draughts import get_board
 
-    engine = AlphaBetaEngine(depth=5)
+    engine = AlphaBetaEngine(depth=2)
+    # board = get_board(
+    #     "standard",
+    #     '[FEN "B:W18,26,28,29,32,33,38,39,41,45,46,47,48,49,50:B4,5,7,8,9,10,11,12,13,15,16,17,19,20"]',
+    # )
     server = Server(get_best_move_method=engine.get_best_move)
     server.run()
```

### Comparing `py-draughts-1.1.5/draughts/standard.py` & `py-draughts-1.1.6/draughts/standard.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     - Any piece can capture backwards and forwards
     - Capture is mandatory
     - King can move along the diagonal any number of squares
 
     **Winning and drawing**
 
     - A player wins the game when the opponent no longer has any valid moves.
-    This can be either because all of the player's pieces have been captured,
-    or because they are all blocked and thus have no more squares available.
+      This can be either because all of the player's pieces have been captured,
+      or because they are all blocked and thus have no more squares available.
     - If the same position appears on the board for the third time,
-    with the same side to move, the game is considered drawn by threefold repetition.
+      with the same side to move, the game is considered drawn by threefold repetition.
     - The game is drawn when both players make 25 consecutive king moves without capturing.
-    When one player has only a king left, and the other player three pieces including at least
-    one king (three kings, two kings and a man, or one king and two men),
-    the game is drawn after both players made 16 moves.
+      When one player has only a king left, and the other player three pieces including at least
+      one king (three kings, two kings and a man, or one king and two men),
+      the game is drawn after both players made 16 moves.
     - When one player has only a king left, and the other player two pieces
-    or less including at least one king (one king, two kings, or one king and a man),
-    the game is drawn after both players made 5 moves.
+      or less including at least one king (one king, two kings, or one king and a man),
+      the game is drawn after both players made 5 moves.
 
     """
 
     GAME_TYPE = 20
     STARTING_POSITION = np.array([1] * 15 + [0] * 20 + [-1] * 15, dtype=np.int8)
     PSEUDO_LEGAL_KING_MOVES = get_king_pseudo_legal_moves(len(STARTING_POSITION))
     PSEUDO_LEGAL_MAN_MOVES = get_man_pseudo_legal_moves(len(STARTING_POSITION))
@@ -70,40 +70,43 @@
             or self.is_5_moves_rule
             or self.is_16_moves_rule
             or self.is_25_moves_rule
         )
 
     @property
     def is_25_moves_rule(self) -> bool:
-        if len(self._moves_stack) < 25:
+        if len(self._moves_stack) < 50:
             return False
-        for move in self._moves_stack[-25:]:
-            if move.captured_list:
+        for move in self._moves_stack[-50:]:
+            src = move.square_list[-1]
+            if move.captured_list or self._pos[src] != Figure.KING.value:
                 return False
         logger.debug("25 moves rule")
         return True
 
     @property
     def is_16_moves_rule(self) -> bool:
-        if len(self._moves_stack) < 16:
+        if len(self._moves_stack) < 32 or len(self._pos[self._pos != Figure.EMPTY]) > 4:
             return False
-        for move in self._moves_stack[-16:]:
+        if np.abs(self._pos).sum() < Figure.KING.value * 2 + Figure.MAN.value * 2:
+            return False
+        for move in self._moves_stack[-32:]:
             if move.captured_list or move.is_promotion:
                 return False
         logger.debug("16 moves rule")
         return True
 
     @property
     def is_5_moves_rule(self) -> bool:
         # if count of pieces is not 3 or 4
-        if len(self._pos[self._pos != Figure.EMPTY]) > 4:
+        if len(self._pos[self._pos != Figure.EMPTY]) > 3:
             return False
-        if len(self._moves_stack) < 5:
+        if np.abs(self._pos).sum() < Figure.KING.value * 2 + Figure.MAN.value:
             return False
-        for move in self._moves_stack[-5:]:
+        for move in self._moves_stack[-10:]:
             if move.captured_list or move.is_promotion:
                 return False
         logger.debug("5 moves rule")
         return True
 
     @property
     def legal_moves(self) -> list[Move]:
@@ -113,16 +116,16 @@
         for square in squares_list.flatten():
             moves = self._legal_moves_from(square, is_capture_mandatory)
             # if not is_capture_mandatory and any( # TODO this should optimize the search
             #     [len(move.square_list) > 0 for move in moves]
             # ):
             #     is_capture_mandatory = True
             all_moves.extend(moves)
-        if any([len(move.captured_list) > 0 for move in all_moves]):
-            all_moves = [move for move in all_moves if len(move.captured_list) > 0]
+        if any([len(move) > 1 for move in all_moves]):
+            all_moves = [move for move in all_moves if len(move) > 1]
         return all_moves
 
     def _get_man_legal_moves_from(
         self, square: int, is_capture_mandatory: bool
     ) -> list:
         moves = []
         # white can move only on even directions
@@ -139,17 +142,20 @@
                 len(direction) > 1
                 and self._pos[direction[0]] * self.turn.value < 0
                 and self._pos[direction[1]] == Figure.EMPTY
             ):
                 move = Move(
                     [square, direction[1]], [direction[0]], [self._pos[direction[0]]]
                 )
-                moves.append(move)
+                # moves.append(move)
                 self.push(move, False)
-                moves += [move + m for m in self._legal_moves_from(direction[1], True)]
+                new_moves = [
+                    move + m for m in self._legal_moves_from(direction[1], True)
+                ]
+                moves += [move] if len(new_moves) == 0 else new_moves
                 self.pop(False)
         return moves
 
     def _get_king_legal_moves_from(
         self, square: int, is_capture_mandatory: bool
     ) -> list[Move]:
         moves = []
@@ -166,15 +172,16 @@
                     ):
                         move = Move(
                             [square, direction[i]], [target], [self._pos[target]]
                         )
                         moves.append(move)
                         self.push(move, False)
                         moves += [
-                            move + m for m in self._legal_moves_from(direction[i], True)
+                            move + m
+                            for m in self._get_king_legal_moves_from(direction[i], True)
                         ]
                         # if one move is longer then others return only this one
                         self.pop(False)
                         max_len = max([len(m) for m in moves])
                         moves = [m for m in moves if len(m) == max_len]
                         i += 1
                     break
```

### Comparing `py-draughts-1.1.5/draughts/static/css/style.css` & `py-draughts-1.1.6/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/static/js/script.js` & `py-draughts-1.1.6/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/templates/base.html` & `py-draughts-1.1.6/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/templates/index.html` & `py-draughts-1.1.6/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/draughts/utils.py` & `py-draughts-1.1.6/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.1.6/py_draughts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.5
+Version: 1.1.6
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -27,20 +27,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
-[![Downloads](https://static.pepy.tech/personalized-badge/py-draughts?period=month&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/py-draughts)
-
+[![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
+_inspired by [python-chess](https://pypi.org/project/chess/)_
+
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
```

### Comparing `py-draughts-1.1.5/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.1.6/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/setup.py` & `py-draughts-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/test/test_american_board.py` & `py-draughts-1.1.6/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.5/test/test_board.py` & `py-draughts-1.1.6/test/test_board.py`

 * *Files identical despite different names*

