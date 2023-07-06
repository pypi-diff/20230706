# Comparing `tmp/fast-checkers-0.0.7.tar.gz` & `tmp/fast-checkers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.0.7.tar", last modified: Thu Jul  6 15:43:14 2023, max compression
+gzip compressed data, was "fast-checkers-0.2.0.tar", last modified: Thu Jul  6 20:06:16 2023, max compression
```

## Comparing `fast-checkers-0.0.7.tar` & `fast-checkers-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.188968 fast-checkers-0.0.7/
--rw-rw-rw-   0        0        0       17 2023-07-06 12:35:59.000000 fast-checkers-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5471 2023-07-06 15:43:14.187967 fast-checkers-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4093 2023-07-06 15:31:55.000000 fast-checkers-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.174971 fast-checkers-0.0.7/checkers/
--rw-rw-rw-   0        0        0      947 2023-07-06 15:43:02.000000 fast-checkers-0.0.7/checkers/__init__.py
--rw-rw-rw-   0        0        0     4053 2023-07-06 15:42:07.000000 fast-checkers-0.0.7/checkers/american.py
--rw-rw-rw-   0        0        0     5749 2023-07-06 15:17:12.000000 fast-checkers-0.0.7/checkers/base.py
--rw-rw-rw-   0        0        0     1149 2023-07-06 15:09:38.000000 fast-checkers-0.0.7/checkers/main.py
--rw-rw-rw-   0        0        0      576 2023-07-06 15:09:38.000000 fast-checkers-0.0.7/checkers/models.py
--rw-rw-rw-   0        0        0     3999 2023-07-06 15:33:13.000000 fast-checkers-0.0.7/checkers/move.py
--rw-rw-rw-   0        0        0       65 2023-06-18 11:52:25.000000 fast-checkers-0.0.7/checkers/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.183967 fast-checkers-0.0.7/fast_checkers.egg-info/
--rw-rw-rw-   0        0        0     5471 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 15:43:14.188968 fast-checkers-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1714 2023-07-06 15:40:27.000000 fast-checkers-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.185972 fast-checkers-0.0.7/test/
--rw-rw-rw-   0        0        0     2375 2023-07-06 15:09:38.000000 fast-checkers-0.0.7/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.818050 fast-checkers-0.2.0/
+-rw-rw-rw-   0        0        0       18 2023-07-06 19:57:20.000000 fast-checkers-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5211 2023-07-06 20:06:16.817050 fast-checkers-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3834 2023-07-06 20:05:16.000000 fast-checkers-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.803058 fast-checkers-0.2.0/checkers/
+-rw-rw-rw-   0        0        0      947 2023-07-06 19:56:06.000000 fast-checkers-0.2.0/checkers/__init__.py
+-rw-rw-rw-   0        0        0     3780 2023-07-06 19:54:23.000000 fast-checkers-0.2.0/checkers/american.py
+-rw-rw-rw-   0        0        0     6038 2023-07-06 19:55:03.000000 fast-checkers-0.2.0/checkers/base.py
+-rw-rw-rw-   0        0        0     1441 2023-07-06 19:40:43.000000 fast-checkers-0.2.0/checkers/main.py
+-rw-rw-rw-   0        0        0      674 2023-07-06 19:46:12.000000 fast-checkers-0.2.0/checkers/models.py
+-rw-rw-rw-   0        0        0     4120 2023-07-06 18:18:47.000000 fast-checkers-0.2.0/checkers/move.py
+-rw-rw-rw-   0        0        0       65 2023-06-18 11:52:25.000000 fast-checkers-0.2.0/checkers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.812048 fast-checkers-0.2.0/fast_checkers.egg-info/
+-rw-rw-rw-   0        0        0     5211 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 20:06:16.818050 fast-checkers-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1723 2023-07-06 15:59:26.000000 fast-checkers-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.816048 fast-checkers-0.2.0/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-06 16:45:41.000000 fast-checkers-0.2.0/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2375 2023-07-06 15:09:38.000000 fast-checkers-0.2.0/test/test_board.py
```

### Comparing `fast-checkers-0.0.7/PKG-INFO` & `fast-checkers-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.0.7
+Version: 0.2.0
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/checkers/index.html
 Keywords: checkers AI mini-max droughts,game,board
@@ -20,147 +20,133 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 
-![example workflow](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)
-[![PyPI version](https://badge.fury.io/py/fast_checkers.svg)](https://badge.fury.io/py/fast_checkers)
+Fast Checkers
+=============
 
-# Checkers 
+.. image:: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg
+   :target: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml
 
-__Project still under active development. Usage may be different in futurue versions__
+.. image:: https://badge.fury.io/py/fast_checkers.svg
+   :target: https://badge.fury.io/py/fast_checkers
 
-Efficient Modern and flexible implementation of checkers game with beautiful web interface.
-Supports multiple variants of the game and allows to play against AI.
-
-## [Documentation](https://michalskibinski109.github.io/checkers/)
-
-# Installation
-
-```bash
-python -m pip install fast-checkers 
-```
-
-## Usage:
-
-### simple
-
-```python
-import checkers.american as checkers
-
-board = checkers.Board()
-
-
-board.push_from_str("24-19")
-board.push_from_str("12-16")
-board.push_from_str("23-18")
-board.push_from_str("16x23")
-board.push_from_str("26x19")
-print(board)
-```
-```bash
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   |   |
----------------------------------
-|   |   |   |   |   |   |   |   |
----------------------------------
-|   |   |   | o |   | o |   |   |
----------------------------------
-| o |   | o |   |   |   |   |   |
----------------------------------
-|   | o |   |   |   | o |   | o |
----------------------------------
-| o |   | o |   | o |   | o |   |
-```
-```python
-board.pop()
-print(board)
-```
-```bash
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   |   |
----------------------------------
-|   |   |   |   |   |   |   |   |
----------------------------------
-|   |   |   | o |   |   |   |   |
----------------------------------
-| o |   | o |   | x |   |   |   |
----------------------------------
-|   | o |   | o |   | o |   | o |
----------------------------------
-| o |   | o |   | o |   | o |   |
-```
-```python
-print(list(board.legal_moves))
-```
-```bash
-[Move through squares: [8, 12], Move through squares: [9, 13],
- Move through squares: [9, 14], Move through squares: [10, 14],
- Move through squares: [10, 15], Move through squares: [11, 15],
- Move through squares: [11, 16]]
-```
-
-### advenced:
-
-```python
-import checkers.base as checkers
-import numpy as np
-CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
-board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
-board.legal_moves = ... # create your own custom legal_moves method (property)
-print(board)
-print(board.legal_moves)
-```
-
-```bash
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| o |   | o |   | o |   | o |   |
----------------------------------
-|   | o |   | o |   | o |   | o |
----------------------------------
-| o |   | o |   | o |   | o |   |
-
-Ellipsis
-```
-
-
-## Bibliography
-1. [notatin](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
-2. [rules and variants](https://en.wikipedia.org/wiki/Checkers)
-3. [list of pdns](https://github.com/mig0/Games-Checkers/)
-4. [additional 1 (checkers online)](https://checkers.online/play)
-5. [additional 2 (chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
+Checkers
+--------
 
-## UI
-__for now UI is mostly used for debugging pruposes__
+**Project still under active development. Usage may be different in future versions**
 
+Efficient Modern and flexible implementation of checkers game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
-<img src="https://github.com/michalskibinski109/checkers/assets/77834536/acae0786-9cf3-4e30-9a04-abd7c018202b" width="400">
+Documentation
+-------------
 
-## Contributing
+`Documentation <https://michalskibinski109.github.io/checkers/>`_
+
+Installation
+------------
+
+.. code-block:: bash
+
+    python -m pip install fast-checkers
+
+Usage
+-----
+
+simple
+*******
+
+.. code-block:: python
+
+    >>> import checkers.american as checkers
+
+    >>> board = checkers.Board()
+    ---------------------------------
+    |   | x |   | x |   | x |   | x |
+    ---------------------------------
+    | x |   | x |   | x |   | x |   |
+    ---------------------------------
+    |   | x |   | x |   | x |   | x |
+    ---------------------------------
+    |   |   |   |   |   |   |   |   |
+    ---------------------------------
+    |   |   |   |   |   |   |   |   |
+    ---------------------------------
+    | o |   | o |   | o |   | o |   |
+    ---------------------------------
+    |   | o |   | o |   | o |   | o |
+    ---------------------------------
+    | o |   | o |   | o |   | o |   |
+
+
+Moving pieces
+*************
+
+.. code-block:: python
+
+    >>> board.push_from_str("24-19")
+    >>> board.push_from_str("12-16")
+    >>> board.push_from_str("23-18")
+    >>> board.push_from_str("16x23")
+    >>> board.push_from_str("26x19")
+    >>> board.pop()
+    >>> print(board)
+    ---------------------------------
+    |   | x |   | x |   | x |   | x |
+    ---------------------------------
+    | x |   | x |   | x |   | x |   |
+    ---------------------------------
+    |   | x |   | x |   | x |   |   |
+    ---------------------------------
+    |   |   |   |   |   |   |   |   |
+    ---------------------------------
+    |   |   |   | o |   |   |   |   |
+    ---------------------------------
+    | o |   | o |   | x |   |   |   |
+    ---------------------------------
+    |   | o |   | o |   | o |   | o |
+    ---------------------------------
+    | o |   | o |   | o |   | o |   |
+
+
+.. code-block:: python
+
+    >>> print(list(board.legal_moves))
+    [Move: 21->17, Move: 22->18, Move: 22->17, Move: 23->19, Move: 23->18, Move: 24->20, Move: 24->19]
+
+Creating custom board
+*********************
+
+.. code-block:: python
+
+    import checkers.base as checkers
+    import numpy as np
+    CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
+    board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
+    board.legal_moves = ... # create your own custom legal_moves method (property)
+
+UI
+--
+
+**for now UI is mostly used for debugging purpose**
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/acae0786-9cf3-4e30-9a04-abd7c018202b
+   :width: 400
+
+Contributing
+------------
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
----
+Bibliography
+------------
 
+1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
+2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
+3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
+4. `additional 1 (checkers online) <https://checkers.online/play>`_
+5. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
```

### Comparing `fast-checkers-0.0.7/checkers/__init__.py` & `fast-checkers-0.2.0/checkers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A checkers library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
-__version__ = "0.0.7"
+__version__ = "0.2.0"
 __author__ = "Michał Skibiński"
```

### Comparing `fast-checkers-0.0.7/checkers/american.py` & `fast-checkers-0.2.0/checkers/american.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from __future__ import annotations
 
 from typing import Generator
 
 import numpy as np
 
 from checkers.base import BaseBoard
-from checkers.models import Color
+from checkers.models import Color, Entity
 from checkers.move import Move
 from checkers.utils import logger
 
-"""
- board 8x8
- Short moves only 
- Cannot capture backwards
- Capture - choose any
-"""
 
 # fmt: off
-SQUARES = [_, B8, D8, F8, H8,
+SQUARES = [B8, D8, F8, H8,
         A7, C7, E7, G7,
         B6, D6, F6, H6,
         A5, C5, E5, G5,
         B4, D4, F4, H4,
         A3, C3, E3, G3,
         B2, D2, F2, H2,
-        A1, C1, E1, G1] = range(33)
+        A1, C1, E1, G1] = range(32)
 # fmt: on
 
 
 class Board(BaseBoard):
     """
     **Board for American checkers.**
      Game rules:
@@ -40,80 +34,82 @@
     """
 
     STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
     size = int(np.sqrt(len(STARTING_POSITION) * 2))
     row_idx = {val: val // 4 for val in range(len(STARTING_POSITION))}
     col_idx = {val: val % 8 for val in range(len(STARTING_POSITION))}
 
-    def __init__(self) -> None:
-        super().__init__(Board.STARTING_POSITION)
+    def __init__(self, starting_position=STARTING_POSITION) -> None:
+        super().__init__(starting_position)
 
     @property
     def legal_moves(self) -> Generator[Move, None, None]:
         if self.turn == Color.BLACK:
             squares_list = np.transpose(np.nonzero(self._pos > 0))
         else:
             squares_list = np.transpose(np.nonzero(self._pos < 0))
-
         for square in squares_list.flatten():
             moves = self._legal_moves_from(square)
             for move in moves:
                 yield move
 
-    def _legal_moves_from(self, square: int) -> Generator[Move, None, None]:
+    def _legal_moves_from(
+        self, square: int, is_after_capture=False
+    ) -> Generator[Move, None, None]:
         row = self.row_idx[square]
         moves = []
-        odd = (row % 2 != 0 and self.turn == Color.BLACK) or (
+        odd = bool(row % 2 != 0 and self.turn == Color.BLACK) or (
             row % 2 == 0 and self.turn == Color.WHITE
         )
-        for move_offset, capture_offset in [(4 - odd, 7), (5 - odd, 9)]:
-            move_square = square + move_offset * (self.turn.value)
-            capture_square = square + capture_offset * (self.turn.value)
+        is_king = bool(self[square] == self.turn.value * Entity.KING)
+        # is_king = False  # DEBUF
+        for mv_offset, cap_offset, dir in [
+            (4 - odd, 7, self.turn.value),
+            (5 - odd, 9, self.turn.value),
+        ] + is_king * [
+            (4 - (not odd), 7, -self.turn.value),
+            (5 - (not odd), 9, -self.turn.value),
+        ]:
+            move_sq = square + mv_offset * (dir)
+            capture_sq = square + cap_offset * (dir)
 
             if (
-                0 <= move_square < len(self._pos)
-                and row + 1 * (self.turn.value) == self.row_idx[move_square]
-                and self[move_square] == 0
+                0 <= move_sq < len(self._pos)
+                and row + 1 * (dir) == self.row_idx[move_sq]
+                and self[move_sq] == 0
+                and not is_after_capture
             ):
-                moves.append(Move([square, move_square]))
+                moves.append(Move([square, move_sq]))
             elif (
-                0 <= capture_square < len(self._pos)
-                and row + 2 * (self.turn.value) == self.row_idx[capture_square]
-                and self[capture_square] == 0
-                and self[move_square] * self.turn.value < 0
+                0 <= capture_sq < len(self._pos)
+                and row + 2 * (dir) == self.row_idx[capture_sq]
+                and self[capture_sq] == 0
+                and self[move_sq] * self.turn.value < 0
             ):
                 move = Move(
-                    [square, capture_square],
-                    captured_list=[move_square],
-                    captured_entities=[self[move_square]],
+                    [square, capture_sq],
+                    captured_list=[move_sq],
+                    captured_entities=[self[move_sq]],
                 )
                 moves.append(move)
                 self.push(move, False)
-                moves += [move + m for m in self._legal_moves_from(capture_square)]
+                moves += [move + m for m in self._legal_moves_from(capture_sq, True)]
                 self.pop(False)
 
         return moves
 
 
 if __name__ == "__main__":
     board = Board()
-    board.push_from_str("24-19")
-    board.push_from_str("12-16")
-    board.push_from_str("23-18")
-    # from copy import deepcopy
-
-    # logger.info(
-    #     f"stack: {len(board._moves_stack)} turn: {board.turn}, num_moves: {len(list(board.legal_moves))}, num_of_white: {len(np.where(board._pos == -1)[0])}, num_of_black: {len(np.where(board._pos == 1)[0])}"
-    # )
-    # logger.info(
-    #     f"stack: {len(board._moves_stack)} turn: {board.turn}, num_moves: {len(list(board.legal_moves))}, num_of_white: {len(np.where(board._pos == -1)[0])}, num_of_black: {len(np.where(board._pos == 1)[0])}"
-    # )
-    # print(b2.__dict__)
-    # print(board.__dict__)
-    board.push_from_str("16-23")
+    print(list(board.legal_moves))
+    # board.push_from_str("12-16")
+    # board.push_from_str("12-16")
+    # board.push_from_str("23-18")
+    # board.push_from_str("16-23")
+    # print(board.pop())
     print(board)
     # while True:
     #     moves = board.legal_moves
     #     move = np.random.choice(list(moves))
     #     board.push(move)
     #     print(move)
     #     print(board)
```

### Comparing `fast-checkers-0.0.7/checkers/base.py` & `fast-checkers-0.2.0/checkers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,26 +74,32 @@
     @property
     def position(self) -> np.ndarray:
         """Returns board position."""
         return self._pos
 
     def push(self, move: Move, is_finished: bool = True) -> None:
         """Pushes a move to the board.
+        Automatically promotes a piece if it reaches the last row.
 
         If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
         for generating legal moves.
+
         """
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
-        logger.debug(
-            f"({is_finished}) PUSH METHOD: Moved entity: {Entity(self._pos[tg])} to {tg}"
-        )
+        # is promotion
+        if (tg // (self.shape[0] // 2)) in (0, self.shape[0] - 1) and abs(
+            self._pos[tg]
+        ) == 1:
+            self._pos[tg] *= Entity.KING.value
+            move.is_promotion = True
+            logger.warning(f"Kinged: {tg} on row {tg // self.shape[0]}")
         if move.captured_list:
             self._pos[np.array([sq for sq in move.captured_list])] = Entity.EMPTY
         self._moves_stack.append(move)
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
 
     def pop(self, is_finished=True) -> None:
@@ -103,25 +109,29 @@
         for generating legal moves.
         """
         move = self._moves_stack.pop()
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
-        logger.debug(f"({is_finished}): Reversing: {Entity(self._pos[tg])} to {tg}")
+        if move.is_promotion:
+            self._pos[tg] //= Entity.KING.value
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         for sq, entity in zip(move.captured_list, move.captured_entities):
             self._pos[sq] = entity  # Dangerous line
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
         return move
 
     def push_from_str(self, str_move: str) -> None:
         """
         Allows to push a move from a string.
+
+        * Converts string to ``Move`` object
+        * calls ``BaseBoard.push`` method
         """
         try:
             move = Move.from_string(str_move, self.legal_moves)
         except ValueError as e:
             logger.error(f"{e} \n {str(self)}")
             raise e
         self.push(move)
@@ -170,9 +180,7 @@
     m3 = Move([G3, H4])
     board.push(m3)
     print(board)
 
     m4 = Move([A5, C3], captured_list=[B4])
     board.push(m4)
     print(board)
-    SQUARES = range(51)
-    print(SQUARES)
```

### Comparing `fast-checkers-0.0.7/checkers/models.py` & `fast-checkers-0.2.0/checkers/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 
 class Color(Enum):
     WHITE = -1
     BLACK = 1
 
 
 class Entity(IntEnum):
-    BLACK_KING = 10
-    BLACK_MAN = 1
-    WHITE_KING = -10
-    WHITE_MAN = -1
+    BLACK_KING = Color.BLACK.value * 10
+    BLACK_MAN = Color.BLACK.value
+    WHITE_KING = Color.WHITE.value * 10
+    WHITE_MAN = Color.WHITE.value
+    KING = 10
+    MAN = 1
     EMPTY = 0
 
 
 ENTITY_REPR = {
     Entity.BLACK_MAN: "x",
     Entity.WHITE_MAN: "o",
     Entity.EMPTY: " ",
```

### Comparing `fast-checkers-0.0.7/checkers/move.py` & `fast-checkers-0.2.0/checkers/move.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,24 @@
     """
 
     def __init__(
         self,
         visited_squares: list[int],
         captured_list: list[int] = [],
         captured_entities: list[Entity.value] = [],
+        is_promotion: bool = False,
     ) -> None:
         self.square_list = visited_squares
         self.captured_list = captured_list
         self.captured_entities = captured_entities
+        self.is_promotion = is_promotion
 
     def __repr__(self) -> str:
-        return f"Move through squares: {[s + 1 for s in self.square_list ]}"
+        visited_squares = [str(s + 1) for s in self.square_list]
+        return f"Move: {'->'.join(visited_squares)}"
 
     def __eq__(self, other: object) -> bool:
         """Check if two moves are equal. move created from string will have only visited squares definied."""
         if not isinstance(other, Move):
             return False
 
         if (
```

### Comparing `fast-checkers-0.0.7/fast_checkers.egg-info/PKG-INFO` & `fast-checkers-0.2.0/fast_checkers.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.0.7
+Version: 0.2.0
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/checkers/index.html
 Keywords: checkers AI mini-max droughts,game,board
@@ -20,147 +20,133 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 
-![example workflow](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)
-[![PyPI version](https://badge.fury.io/py/fast_checkers.svg)](https://badge.fury.io/py/fast_checkers)
+Fast Checkers
+=============
 
-# Checkers 
+.. image:: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg
+   :target: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml
 
-__Project still under active development. Usage may be different in futurue versions__
+.. image:: https://badge.fury.io/py/fast_checkers.svg
+   :target: https://badge.fury.io/py/fast_checkers
 
-Efficient Modern and flexible implementation of checkers game with beautiful web interface.
-Supports multiple variants of the game and allows to play against AI.
-
-## [Documentation](https://michalskibinski109.github.io/checkers/)
-
-# Installation
-
-```bash
-python -m pip install fast-checkers 
-```
-
-## Usage:
-
-### simple
-
-```python
-import checkers.american as checkers
-
-board = checkers.Board()
-
-
-board.push_from_str("24-19")
-board.push_from_str("12-16")
-board.push_from_str("23-18")
-board.push_from_str("16x23")
-board.push_from_str("26x19")
-print(board)
-```
-```bash
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   |   |
----------------------------------
-|   |   |   |   |   |   |   |   |
----------------------------------
-|   |   |   | o |   | o |   |   |
----------------------------------
-| o |   | o |   |   |   |   |   |
----------------------------------
-|   | o |   |   |   | o |   | o |
----------------------------------
-| o |   | o |   | o |   | o |   |
-```
-```python
-board.pop()
-print(board)
-```
-```bash
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   |   |
----------------------------------
-|   |   |   |   |   |   |   |   |
----------------------------------
-|   |   |   | o |   |   |   |   |
----------------------------------
-| o |   | o |   | x |   |   |   |
----------------------------------
-|   | o |   | o |   | o |   | o |
----------------------------------
-| o |   | o |   | o |   | o |   |
-```
-```python
-print(list(board.legal_moves))
-```
-```bash
-[Move through squares: [8, 12], Move through squares: [9, 13],
- Move through squares: [9, 14], Move through squares: [10, 14],
- Move through squares: [10, 15], Move through squares: [11, 15],
- Move through squares: [11, 16]]
-```
-
-### advenced:
-
-```python
-import checkers.base as checkers
-import numpy as np
-CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
-board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
-board.legal_moves = ... # create your own custom legal_moves method (property)
-print(board)
-print(board.legal_moves)
-```
-
-```bash
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| x |   | x |   | x |   | x |   |
----------------------------------
-|   | x |   | x |   | x |   | x |
----------------------------------
-| o |   | o |   | o |   | o |   |
----------------------------------
-|   | o |   | o |   | o |   | o |
----------------------------------
-| o |   | o |   | o |   | o |   |
-
-Ellipsis
-```
-
-
-## Bibliography
-1. [notatin](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
-2. [rules and variants](https://en.wikipedia.org/wiki/Checkers)
-3. [list of pdns](https://github.com/mig0/Games-Checkers/)
-4. [additional 1 (checkers online)](https://checkers.online/play)
-5. [additional 2 (chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
+Checkers
+--------
 
-## UI
-__for now UI is mostly used for debugging pruposes__
+**Project still under active development. Usage may be different in future versions**
 
+Efficient Modern and flexible implementation of checkers game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
-<img src="https://github.com/michalskibinski109/checkers/assets/77834536/acae0786-9cf3-4e30-9a04-abd7c018202b" width="400">
+Documentation
+-------------
 
-## Contributing
+`Documentation <https://michalskibinski109.github.io/checkers/>`_
+
+Installation
+------------
+
+.. code-block:: bash
+
+    python -m pip install fast-checkers
+
+Usage
+-----
+
+simple
+*******
+
+.. code-block:: python
+
+    >>> import checkers.american as checkers
+
+    >>> board = checkers.Board()
+    ---------------------------------
+    |   | x |   | x |   | x |   | x |
+    ---------------------------------
+    | x |   | x |   | x |   | x |   |
+    ---------------------------------
+    |   | x |   | x |   | x |   | x |
+    ---------------------------------
+    |   |   |   |   |   |   |   |   |
+    ---------------------------------
+    |   |   |   |   |   |   |   |   |
+    ---------------------------------
+    | o |   | o |   | o |   | o |   |
+    ---------------------------------
+    |   | o |   | o |   | o |   | o |
+    ---------------------------------
+    | o |   | o |   | o |   | o |   |
+
+
+Moving pieces
+*************
+
+.. code-block:: python
+
+    >>> board.push_from_str("24-19")
+    >>> board.push_from_str("12-16")
+    >>> board.push_from_str("23-18")
+    >>> board.push_from_str("16x23")
+    >>> board.push_from_str("26x19")
+    >>> board.pop()
+    >>> print(board)
+    ---------------------------------
+    |   | x |   | x |   | x |   | x |
+    ---------------------------------
+    | x |   | x |   | x |   | x |   |
+    ---------------------------------
+    |   | x |   | x |   | x |   |   |
+    ---------------------------------
+    |   |   |   |   |   |   |   |   |
+    ---------------------------------
+    |   |   |   | o |   |   |   |   |
+    ---------------------------------
+    | o |   | o |   | x |   |   |   |
+    ---------------------------------
+    |   | o |   | o |   | o |   | o |
+    ---------------------------------
+    | o |   | o |   | o |   | o |   |
+
+
+.. code-block:: python
+
+    >>> print(list(board.legal_moves))
+    [Move: 21->17, Move: 22->18, Move: 22->17, Move: 23->19, Move: 23->18, Move: 24->20, Move: 24->19]
+
+Creating custom board
+*********************
+
+.. code-block:: python
+
+    import checkers.base as checkers
+    import numpy as np
+    CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
+    board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
+    board.legal_moves = ... # create your own custom legal_moves method (property)
+
+UI
+--
+
+**for now UI is mostly used for debugging purpose**
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/acae0786-9cf3-4e30-9a04-abd7c018202b
+   :width: 400
+
+Contributing
+------------
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
----
+Bibliography
+------------
 
+1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
+2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
+3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
+4. `additional 1 (checkers online) <https://checkers.online/play>`_
+5. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
```

### Comparing `fast-checkers-0.0.7/setup.py` & `fast-checkers-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from pathlib import Path
 
 import setuptools
 
 from checkers.__init__ import __doc__, __version__
 
 this_directory = Path(__file__).parent
-long_description = (this_directory / "readme.md").read_text()
+long_description = (this_directory / "readme.rst").read_text()
 
 setuptools.setup(
     name="fast-checkers",
     version=__version__,
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     files_to_include=["checkers"],
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    # rst
+    long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(),
     license="GPL-3.0+",
     keywords="checkers AI mini-max droughts, game, board",
     url="https://github.com/michalskibinski109/checkers",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `fast-checkers-0.0.7/test/test_board.py` & `fast-checkers-0.2.0/test/test_board.py`

 * *Files identical despite different names*

