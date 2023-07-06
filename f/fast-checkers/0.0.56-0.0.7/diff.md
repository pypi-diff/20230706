# Comparing `tmp/fast-checkers-0.0.56.tar.gz` & `tmp/fast-checkers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.0.56.tar", last modified: Thu Jul  6 13:09:36 2023, max compression
+gzip compressed data, was "fast-checkers-0.0.7.tar", last modified: Thu Jul  6 15:43:14 2023, max compression
```

## Comparing `fast-checkers-0.0.56.tar` & `fast-checkers-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.340021 fast-checkers-0.0.56/
--rw-rw-rw-   0        0        0       17 2023-07-06 12:35:59.000000 fast-checkers-0.0.56/MANIFEST.in
--rw-rw-rw-   0        0        0     4570 2023-07-06 13:09:36.340021 fast-checkers-0.0.56/PKG-INFO
--rw-rw-rw-   0        0        0     4027 2023-07-06 13:00:06.000000 fast-checkers-0.0.56/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.326023 fast-checkers-0.0.56/checkers/
--rw-rw-rw-   0        0        0      889 2023-07-06 11:33:52.000000 fast-checkers-0.0.56/checkers/__init__.py
--rw-rw-rw-   0        0        0     3735 2023-07-06 12:28:19.000000 fast-checkers-0.0.56/checkers/american.py
--rw-rw-rw-   0        0        0     5062 2023-07-06 12:21:56.000000 fast-checkers-0.0.56/checkers/base.py
--rw-rw-rw-   0        0        0     1147 2023-07-06 11:33:52.000000 fast-checkers-0.0.56/checkers/main.py
--rw-rw-rw-   0        0        0     3838 2023-07-06 12:21:42.000000 fast-checkers-0.0.56/checkers/models.py
--rw-rw-rw-   0        0        0       65 2023-06-18 11:52:25.000000 fast-checkers-0.0.56/checkers/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.335021 fast-checkers-0.0.56/fast_checkers.egg-info/
--rw-rw-rw-   0        0        0     4570 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 13:09:36.000000 fast-checkers-0.0.56/fast_checkers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 13:09:36.341022 fast-checkers-0.0.56/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-07-06 13:09:27.000000 fast-checkers-0.0.56/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:09:36.338022 fast-checkers-0.0.56/test/
--rw-rw-rw-   0        0        0     2387 2023-07-06 11:33:52.000000 fast-checkers-0.0.56/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.188968 fast-checkers-0.0.7/
+-rw-rw-rw-   0        0        0       17 2023-07-06 12:35:59.000000 fast-checkers-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5471 2023-07-06 15:43:14.187967 fast-checkers-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4093 2023-07-06 15:31:55.000000 fast-checkers-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.174971 fast-checkers-0.0.7/checkers/
+-rw-rw-rw-   0        0        0      947 2023-07-06 15:43:02.000000 fast-checkers-0.0.7/checkers/__init__.py
+-rw-rw-rw-   0        0        0     4053 2023-07-06 15:42:07.000000 fast-checkers-0.0.7/checkers/american.py
+-rw-rw-rw-   0        0        0     5749 2023-07-06 15:17:12.000000 fast-checkers-0.0.7/checkers/base.py
+-rw-rw-rw-   0        0        0     1149 2023-07-06 15:09:38.000000 fast-checkers-0.0.7/checkers/main.py
+-rw-rw-rw-   0        0        0      576 2023-07-06 15:09:38.000000 fast-checkers-0.0.7/checkers/models.py
+-rw-rw-rw-   0        0        0     3999 2023-07-06 15:33:13.000000 fast-checkers-0.0.7/checkers/move.py
+-rw-rw-rw-   0        0        0       65 2023-06-18 11:52:25.000000 fast-checkers-0.0.7/checkers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.183967 fast-checkers-0.0.7/fast_checkers.egg-info/
+-rw-rw-rw-   0        0        0     5471 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 15:43:14.000000 fast-checkers-0.0.7/fast_checkers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:43:14.188968 fast-checkers-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2023-07-06 15:40:27.000000 fast-checkers-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:43:14.185972 fast-checkers-0.0.7/test/
+-rw-rw-rw-   0        0        0     2375 2023-07-06 15:09:38.000000 fast-checkers-0.0.7/test/test_board.py
```

### Comparing `fast-checkers-0.0.56/README.md` & `fast-checkers-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Checkers 
 
 __Project still under active development. Usage may be different in futurue versions__
 
 Efficient Modern and flexible implementation of checkers game with beautiful web interface.
 Supports multiple variants of the game and allows to play against AI.
 
-
+## [Documentation](https://michalskibinski109.github.io/checkers/)
 
 # Installation
 
 ```bash
 python -m pip install fast-checkers 
 ```
```

### Comparing `fast-checkers-0.0.56/checkers/__init__.py` & `fast-checkers-0.0.7/checkers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A checkers library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
+__version__ = "0.0.7"
+__author__ = "Michał Skibiński"
```

### Comparing `fast-checkers-0.0.56/checkers/american.py` & `fast-checkers-0.0.7/checkers/american.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
+
 from typing import Generator
+
+import numpy as np
+
 from checkers.base import BaseBoard
-from checkers.models import Move, Color
+from checkers.models import Color
+from checkers.move import Move
 from checkers.utils import logger
-import numpy as np
 
 """
  board 8x8
  Short moves only 
  Cannot capture backwards
  Capture - choose any
 """
@@ -21,19 +25,32 @@
         A3, C3, E3, G3,
         B2, D2, F2, H2,
         A1, C1, E1, G1] = range(33)
 # fmt: on
 
 
 class Board(BaseBoard):
+    """
+    **Board for American checkers.**
+     Game rules:
+
+     - Board size: 8x8
+     - Short moves only
+     - Only the king can capture backwards
+     - Capture - choose any
+    """
+
     STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
     size = int(np.sqrt(len(STARTING_POSITION) * 2))
     row_idx = {val: val // 4 for val in range(len(STARTING_POSITION))}
     col_idx = {val: val % 8 for val in range(len(STARTING_POSITION))}
 
+    def __init__(self) -> None:
+        super().__init__(Board.STARTING_POSITION)
+
     @property
     def legal_moves(self) -> Generator[Move, None, None]:
         if self.turn == Color.BLACK:
             squares_list = np.transpose(np.nonzero(self._pos > 0))
         else:
             squares_list = np.transpose(np.nonzero(self._pos < 0))
```

### Comparing `fast-checkers-0.0.56/checkers/base.py` & `fast-checkers-0.0.7/checkers/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,23 @@
+# documentation in rst format
+"""
+
+"""
+
 from __future__ import annotations
-from checkers.utils import logger
-from checkers.models import (
-    Entity,
-    ENTITY_REPR,
-    STARTING_POSITION,
-    Color,
-    Move,
-    SquareT,
-)
-import checkers
-from typing import Generator
+
 from abc import ABC
+from typing import Generator
+
 import numpy as np
 
-# SQUARES = [
-#     _, B10, D10, F10, H10, J10,
-#     A9, C9, E9, G9, I9,
-#     B8, D8, F8, H8, J8,
-#     A7, C7, E7, G7, I7,
-#     B6, D6, F6, H6, J6,
-#     A5, C5, E5, G5, I5,
-#     B4, D4, F4, H4, J4,
-#     A3, C3, E3, G3, I3,
-#     B2, D2, F2, H2, J2,
-#     A1, C1, E1, G1, I1
-#     ] = range(51)
+from checkers.models import ENTITY_REPR, STARTING_POSITION, Color, Entity, SquareT
+from checkers.move import Move
+from checkers.utils import logger
+
 # fmt: off
 SQUARES = [_, B8, D8, F8, H8,
         A7, C7, E7, G7,
         B6, D6, F6, H6,
         A5, C5, E5, G5,
         B4, D4, F4, H4,
         A3, C3, E3, G3,
@@ -36,19 +25,37 @@
         A1, C1, E1, G1] = range(33)
 # fmt: on
 
 
 class BaseBoard(ABC):
     """
     The class is designed to support checkers boards of any size.
-    The shape attribute, represented as a tuple (rows, columns),
-    enables dynamic configuration of the board's dimensions.
+    By specifying the starting position, the user can create a board of any size.
+
+
+
+    To create new variants of checkers, inherit from this class and:
+
+    - override the ``legal_moves`` property
+    - override the ``SQUARES`` list to match the new board size
+    - override the ``STARTING_POSITION`` to specify the starting position
+
+    Constraints:
+    - There are only two colors: ``Color.WHITE`` and ``Color.BLACK``
+    - There are only two types of pieces: ``PieceType.MAN`` and ``PieceType.KING``
+    - Board should always be square.
     """
 
-    def __init__(self, starting_position: np.ndarray = STARTING_POSITION) -> None:
+    def __init__(self, starting_position: np.ndarray) -> None:
+        """
+        Initializes the board with a starting position.
+        The starting position must be a numpy array of length n * n/2,
+        where n is the size of the board.
+
+        """
         super().__init__()
         self._pos = starting_position.copy()
         size = int(np.sqrt(len(self.position) * 2))
         if size**2 != len(self.position) * 2:
             msg = f"Invalid board with shape {starting_position.shape} provided.\
                 Please use an array with lenght = (n * n/2). \
                 Where n is an size of the board."
@@ -66,15 +73,19 @@
 
     @property
     def position(self) -> np.ndarray:
         """Returns board position."""
         return self._pos
 
     def push(self, move: Move, is_finished: bool = True) -> None:
-        """Pushes a move to the board."""
+        """Pushes a move to the board.
+
+        If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
+        for generating legal moves.
+        """
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         logger.debug(
             f"({is_finished}) PUSH METHOD: Moved entity: {Entity(self._pos[tg])} to {tg}"
@@ -82,29 +93,36 @@
         if move.captured_list:
             self._pos[np.array([sq for sq in move.captured_list])] = Entity.EMPTY
         self._moves_stack.append(move)
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
 
     def pop(self, is_finished=True) -> None:
-        """Pops a move from the board."""
+        """Pops a move from the board.
+
+        If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
+        for generating legal moves.
+        """
         move = self._moves_stack.pop()
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
         logger.debug(f"({is_finished}): Reversing: {Entity(self._pos[tg])} to {tg}")
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         for sq, entity in zip(move.captured_list, move.captured_entities):
             self._pos[sq] = entity  # Dangerous line
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
         return move
 
     def push_from_str(self, str_move: str) -> None:
+        """
+        Allows to push a move from a string.
+        """
         try:
             move = Move.from_string(str_move, self.legal_moves)
         except ValueError as e:
             logger.error(f"{e} \n {str(self)}")
             raise e
         self.push(move)
```

### Comparing `fast-checkers-0.0.56/checkers/main.py` & `fast-checkers-0.0.7/checkers/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
-from fastapi import FastAPI, Request
 import uvicorn
-from fastapi.responses import JSONResponse, HTMLResponse
-from fastapi.templating import Jinja2Templates
+from fastapi import FastAPI, Request
+from fastapi.responses import HTMLResponse, JSONResponse
 from fastapi.staticfiles import StaticFiles
+from fastapi.templating import Jinja2Templates
+
 from checkers.american import Board as Board
 
 templates = Jinja2Templates(directory="checkers/templates/")
 
 app = FastAPI()
 board = Board()
 app.mount("/static", StaticFiles(directory="checkers/static"), name="static")
```

### Comparing `fast-checkers-0.0.56/checkers/models.py` & `fast-checkers-0.0.7/checkers/move.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
-from typing import NewType, Generator
+from typing import Generator, NewType
+
 import numpy as np
-from enum import Enum, IntEnum
-from checkers.utils import logger
 
-STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
-SquareT = NewType("SquareT", int)
+from checkers.models import Color, Entity, SquareT
 
 
 class Move:
     """Move representation.
-    Since
-    ```
-    Multiple jumps, such as a double or triple jump,
+    End user should never interact with this class directly.
+
+    As we can read on wikipedia:
+
+    *Multiple jumps, such as a double or triple jump,
     require you to pay attention, as the convention is
     to just show the start and end squares and not the
     in-between or intermediate squares. So the notation
     1-3 would mean a King does a double jump from 1 to 10 to 3.
     The intermediate square is only shown if there are two ways
-    to jump and it would not be clear otherwise.
-    ```
-    Note that:
+    to jump and it would not be clear otherwise.*
+
+    Note that always:
     n - number of visited squares (include source square)
     n - 2 - number of captured pieces
     """
 
     def __init__(
         self,
         visited_squares: list[int],
@@ -73,50 +73,42 @@
             self.square_list + other.square_list[1:],
             self.captured_list + other.captured_list,
             self.captured_entities + other.captured_entities,
         )
 
     @classmethod
     def from_string(cls, move: str, legal_moves: Generator) -> Move:
-        """Converts string representation of move to MovesChain
-        Accepted types:
-        with `-` separator: eg 1-5
-        with `x` separator: eg 1x5
-        multiple jumps: eg 1-5-9
+        """
+
+        Converts string representation of move to ``Move`` object.
+        This is generic method, so it can be used for any board size. Therefore,
+        For different context different move object will be generated.
+        Also we need to pass legal moves, to understand given move and check if it is legal.
+
+
+        input format:
+
+        * ``<square_number>-<square_number>`` for simple move
+        * ``<square_number>x<square_number>`` for capture
+
+        Examples:
+
+        * ``24-19`` - means from 24 to 19
+        * ``24x19`` - means from 24 to 16 means capture of piece between 24 and 16
+        * ``1x10x19`` - means capture of two pieces between 1 and 19
+
         """
         move = move.lower()
-        if "-" in move:
+        if "-" in move:  # classic move
             steps = move.split("-")
-        elif "x" in move:
+        elif "x" in move:  # this means capture
             steps = move.split("x")
         else:
             raise ValueError(f"Invalid move {move}.")
 
         move = Move([int(step) - 1 for step in steps])
         for legal_move in legal_moves:
             if legal_move == move:
                 return legal_move
         raise ValueError(
             f"{move} is correct, but not legal in given position.\n Legal moves are: {list(legal_moves)}"
         )
-
-
-class Color(Enum):
-    WHITE = -1
-    BLACK = 1
-
-
-class Entity(IntEnum):
-    BLACK_KING = 10
-    BLACK_MAN = 1
-    WHITE_KING = -10
-    WHITE_MAN = -1
-    EMPTY = 0
-
-
-ENTITY_REPR = {
-    Entity.BLACK_MAN: "x",
-    Entity.WHITE_MAN: "o",
-    Entity.EMPTY: " ",
-    Entity.BLACK_KING: "X",
-    Entity.WHITE_KING: "O",
-}
```

### Comparing `fast-checkers-0.0.56/test/test_board.py` & `fast-checkers-0.0.7/test/test_board.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-from checkers.base import (
-    BaseBoard,
-    Color,
-    Move,
-    STARTING_POSITION,
-    Entity,
-)
-import checkers.base as checkers
-import pytest
 import numpy as np
+import pytest
+
+import checkers.base as checkers
+from checkers.base import STARTING_POSITION, BaseBoard, Color, Entity, Move
 
 
 class TestBoard:
     @pytest.fixture(autouse=True)
     def setup(self):
-        self.board = BaseBoard()
+        self.board = BaseBoard(STARTING_POSITION)
         yield
         del self.board
 
     def test_init(self):
         assert self.board.turn == Color.WHITE
         assert np.array_equal(self.board.position, STARTING_POSITION)
```

