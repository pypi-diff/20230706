# Comparing `tmp/fast-checkers-0.0.3.tar.gz` & `tmp/fast-checkers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.0.3.tar", last modified: Wed Jul  5 11:56:40 2023, max compression
+gzip compressed data, was "fast-checkers-0.0.4.tar", last modified: Thu Jul  6 09:14:06 2023, max compression
```

## Comparing `fast-checkers-0.0.3.tar` & `fast-checkers-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.357052 fast-checkers-0.0.3/
--rw-rw-rw-   0        0        0     2711 2023-07-05 11:56:40.355051 fast-checkers-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2169 2023-07-05 07:52:18.000000 fast-checkers-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.316189 fast-checkers-0.0.3/checkers/
--rw-rw-rw-   0        0        0     1516 2023-07-05 07:52:01.000000 fast-checkers-0.0.3/checkers/__init__.py
--rw-rw-rw-   0        0        0     3552 2023-07-05 07:48:08.000000 fast-checkers-0.0.3/checkers/american_board.py
--rw-rw-rw-   0        0        0     4276 2023-07-05 07:48:34.000000 fast-checkers-0.0.3/checkers/base_board.py
--rw-rw-rw-   0        0        0     1161 2023-07-05 07:25:47.000000 fast-checkers-0.0.3/checkers/main.py
--rw-rw-rw-   0        0        0     3357 2023-07-05 07:36:27.000000 fast-checkers-0.0.3/checkers/models.py
--rw-rw-rw-   0        0        0       65 2023-07-04 07:53:40.000000 fast-checkers-0.0.3/checkers/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.342033 fast-checkers-0.0.3/fast_checkers.egg-info/
--rw-rw-rw-   0        0        0     2711 2023-07-05 11:56:36.000000 fast-checkers-0.0.3/fast_checkers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-05 11:56:39.000000 fast-checkers-0.0.3/fast_checkers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 11:56:36.000000 fast-checkers-0.0.3/fast_checkers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 11:56:36.000000 fast-checkers-0.0.3/fast_checkers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 11:56:40.358055 fast-checkers-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      829 2023-07-05 11:52:26.000000 fast-checkers-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.350051 fast-checkers-0.0.3/test/
--rw-rw-rw-   0        0        0     2376 2023-07-05 07:24:56.000000 fast-checkers-0.0.3/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:14:06.773697 fast-checkers-0.0.4/
+-rw-rw-rw-   0        0        0     3913 2023-07-06 09:14:06.771706 fast-checkers-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3371 2023-07-06 09:13:01.000000 fast-checkers-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 09:14:06.726704 fast-checkers-0.0.4/checkers/
+-rw-rw-rw-   0        0        0      889 2023-07-06 08:57:48.000000 fast-checkers-0.0.4/checkers/__init__.py
+-rw-rw-rw-   0        0        0     3728 2023-07-06 09:03:05.000000 fast-checkers-0.0.4/checkers/american.py
+-rw-rw-rw-   0        0        0     4634 2023-07-06 09:10:07.000000 fast-checkers-0.0.4/checkers/base.py
+-rw-rw-rw-   0        0        0     1147 2023-07-06 09:03:05.000000 fast-checkers-0.0.4/checkers/main.py
+-rw-rw-rw-   0        0        0     3229 2023-07-06 09:06:15.000000 fast-checkers-0.0.4/checkers/models.py
+-rw-rw-rw-   0        0        0       65 2023-07-04 07:53:40.000000 fast-checkers-0.0.4/checkers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:14:06.755700 fast-checkers-0.0.4/fast_checkers.egg-info/
+-rw-rw-rw-   0        0        0     3913 2023-07-06 09:14:01.000000 fast-checkers-0.0.4/fast_checkers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-07-06 09:14:05.000000 fast-checkers-0.0.4/fast_checkers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 09:14:01.000000 fast-checkers-0.0.4/fast_checkers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 09:14:01.000000 fast-checkers-0.0.4/fast_checkers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 09:14:06.774701 fast-checkers-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-07-06 09:13:28.000000 fast-checkers-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:14:06.765702 fast-checkers-0.0.4/test/
+-rw-rw-rw-   0        0        0     2370 2023-07-06 08:57:48.000000 fast-checkers-0.0.4/test/test_board.py
```

### Comparing `fast-checkers-0.0.3/PKG-INFO` & `fast-checkers-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.0.3
+Version: 0.0.4
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,24 +25,28 @@
 
 ```bash
 python -m pip install fast-checkers 
 ```
 
 ## Usage:
 
+### simple
+
 ```python
-import checkers
-from checkers.american_board import AmericanBoard, Move 
-board = AmericanBoard()
-move = Move([A3, B4])
+import checkers.american as checkers
+board = checkers.Board()
+move = checkers.Move([checkers.A3, checkers.B4])
 board.push(move)
+
+print(list(board.legal_moves))
 print(board)
 ```
 
 ```bash
+['Move through squares: [8, 12]', 'Move through squares: [8, 13]', 'Move through squares: [9, 13]', 'Move through squares: [9, 14]', 'Move through squares: [10, 14]', 'Move through squares: [10, 15]', 'Move through squares: [11, 15]']
 ---------------------------------
 |   | x |   | x |   | x |   | x |
 ---------------------------------
 | x |   | x |   | x |   | x |   |
 ---------------------------------
 |   | x |   | x |   | x |   | x |
 ---------------------------------
@@ -53,14 +57,48 @@
 | o |   |   |   | o |   | o |   |
 ---------------------------------
 |   | o |   | o |   | o |   | o |
 ---------------------------------
 | o |   | o |   | o |   | o |   |
 ```
 
+### advenced:
+
+```python
+import checkers.base as checkers
+import numpy as np
+CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
+board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
+board.legal_moves = ... # create your own custom legal_moves method (property)
+print(board)
+print(board.legal_moves)
+```
+
+```bash
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| x |   | x |   | x |   | x |   |
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| x |   | x |   | x |   | x |   |
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| o |   | o |   | o |   | o |   |
+---------------------------------
+|   | o |   | o |   | o |   | o |
+---------------------------------
+| o |   | o |   | o |   | o |   |
+
+Ellipsis
+```
+
+
 ## Bibliography
 1. [notatin](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
 2. [rules and variants](https://en.wikipedia.org/wiki/Checkers)
 3. [additional 1 (checkers online)](https://checkers.online/play)
 4. [additional 2 (chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
 
 ## Contributing
```

### Comparing `fast-checkers-0.0.3/README.md` & `fast-checkers-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 
 ```bash
 python -m pip install fast-checkers 
 ```
 
 ## Usage:
 
+### simple
+
 ```python
-import checkers
-from checkers.american_board import AmericanBoard, Move 
-board = AmericanBoard()
-move = Move([A3, B4])
+import checkers.american as checkers
+board = checkers.Board()
+move = checkers.Move([checkers.A3, checkers.B4])
 board.push(move)
+
+print(list(board.legal_moves))
 print(board)
 ```
 
 ```bash
+['Move through squares: [8, 12]', 'Move through squares: [8, 13]', 'Move through squares: [9, 13]', 'Move through squares: [9, 14]', 'Move through squares: [10, 14]', 'Move through squares: [10, 15]', 'Move through squares: [11, 15]']
 ---------------------------------
 |   | x |   | x |   | x |   | x |
 ---------------------------------
 | x |   | x |   | x |   | x |   |
 ---------------------------------
 |   | x |   | x |   | x |   | x |
 ---------------------------------
@@ -40,14 +44,48 @@
 | o |   |   |   | o |   | o |   |
 ---------------------------------
 |   | o |   | o |   | o |   | o |
 ---------------------------------
 | o |   | o |   | o |   | o |   |
 ```
 
+### advenced:
+
+```python
+import checkers.base as checkers
+import numpy as np
+CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
+board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
+board.legal_moves = ... # create your own custom legal_moves method (property)
+print(board)
+print(board.legal_moves)
+```
+
+```bash
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| x |   | x |   | x |   | x |   |
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| x |   | x |   | x |   | x |   |
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| o |   | o |   | o |   | o |   |
+---------------------------------
+|   | o |   | o |   | o |   | o |
+---------------------------------
+| o |   | o |   | o |   | o |   |
+
+Ellipsis
+```
+
+
 ## Bibliography
 1. [notatin](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
 2. [rules and variants](https://en.wikipedia.org/wiki/Checkers)
 3. [additional 1 (checkers online)](https://checkers.online/play)
 4. [additional 2 (chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
 
 ## Contributing
```

### Comparing `fast-checkers-0.0.3/checkers/base_board.py` & `fast-checkers-0.0.4/checkers/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,35 +6,56 @@
     STARTING_POSITION,
     ENTITY_MAP,
     Color,
     Move,
     SquareT,
 )
 import checkers
-from typing import Generator, Literal
-from abc import ABC, abstractmethod
-import warnings
+from typing import Generator
+from abc import ABC
 import numpy as np
 
+# SQUARES = [
+#     _, B10, D10, F10, H10, J10,
+#     A9, C9, E9, G9, I9,
+#     B8, D8, F8, H8, J8,
+#     A7, C7, E7, G7, I7,
+#     B6, D6, F6, H6, J6,
+#     A5, C5, E5, G5, I5,
+#     B4, D4, F4, H4, J4,
+#     A3, C3, E3, G3, I3,
+#     B2, D2, F2, H2, J2,
+#     A1, C1, E1, G1, I1
+#     ] = range(51)
+# fmt: off
+SQUARES = [_, B8, D8, F8, H8,
+        A7, C7, E7, G7,
+        B6, D6, F6, H6,
+        A5, C5, E5, G5,
+        B4, D4, F4, H4,
+        A3, C3, E3, G3,
+        B2, D2, F2, H2,
+        A1, C1, E1, G1] = range(33)
+# fmt: on
+
 
 class BaseBoard(ABC):
     """
     The class is designed to support checkers boards of any size.
     The shape attribute, represented as a tuple (rows, columns),
     enables dynamic configuration of the board's dimensions.
     """
 
-    SQUARES_MAP: checkers.T10X10 | checkers.T8X8 = checkers.T8X8
 
-    def __init__(self, position: np.ndarray = STARTING_POSITION) -> None:
+    def __init__(self, starting_position: np.ndarray = STARTING_POSITION) -> None:
         super().__init__()
-        self._pos = position.copy()
+        self._pos = starting_position.copy()
         size = int(np.sqrt(len(self.position) * 2))
         if size**2 != len(self.position) * 2:
-            msg = f"Invalid board with shape {position.shape} provided.\
+            msg = f"Invalid board with shape {starting_position.shape} provided.\
                 Please use an array with lenght = (n * n/2). \
                 Where n is an size of the board."
             logger.error(msg)
             raise ValueError(msg)
         self.shape = (size, size)
         self.turn = Color.WHITE
         self._moves_stack: list[Move] = []
@@ -54,15 +75,15 @@
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         if move.captured_list:
             self._pos[
-                np.array([self.SQUARES_MAP[sq] for sq in move.captured_list])
+                np.array([sq for sq in move.captured_list])
             ] = Entity.EMPTY
         self._moves_stack.append(move)
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
 
     def pop(self, is_finished=True) -> None:
         """Pops a move from the board."""
@@ -109,22 +130,22 @@
     def __getitem__(self, key: SquareT) -> Entity:
         return self.position[key]
 
 
 if __name__ == "__main__":
     board = BaseBoard(STARTING_POSITION)
 
-    m1 = Move([checkers.C3, checkers.B4])
+    m1 = Move([C3, B4])
     board.push(m1)
 
-    m2 = Move([checkers.B6, checkers.A5])
+    m2 = Move([B6, A5])
     board.push(m2)
 
-    m3 = Move([checkers.G3, checkers.H4])
+    m3 = Move([G3, H4])
     board.push(m3)
     print(board)
 
-    m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
+    m4 = Move([A5, C3], captured_list=[B4])
     board.push(m4)
     print(board)
-    checkers.SQUARES = range(51)
-    print(checkers.SQUARES)
+    SQUARES = range(51)
+    print(SQUARES)
```

### Comparing `fast-checkers-0.0.3/checkers/main.py` & `fast-checkers-0.0.4/checkers/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from fastapi import FastAPI, Request
 import uvicorn
 from fastapi.responses import JSONResponse, HTMLResponse
 from fastapi.templating import Jinja2Templates
 from fastapi.staticfiles import StaticFiles
-from checkers.american_board import AmericanBoard as Board
+from checkers.american import Board as Board
 
 templates = Jinja2Templates(directory="checkers/templates/")
 
 app = FastAPI()
 board = Board()
 app.mount("/static", StaticFiles(directory="checkers/static"), name="static")
```

### Comparing `fast-checkers-0.0.3/checkers/models.py` & `fast-checkers-0.0.4/checkers/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from __future__ import annotations
 
 from typing import NewType, Generator
 import numpy as np
 from enum import Enum, IntEnum
 from checkers.utils import logger
-from dataclasses import dataclass, field
-
-# import cached_property
-from functools import cached_property
 
 STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
 SquareT = NewType("SquareT", int)
 
 
 class Move:
     """Move representation.
@@ -37,15 +33,15 @@
         captured_entities: list[bool] = [],
     ) -> None:
         self.square_list = visited_squares
         self.captured_list = captured_list
         self.captured_entities = captured_entities
 
     def __str__(self) -> str:
-        return f"Squares: {self.square_list}, Captured: {self.captured_list}"
+        return f"Move through squares: {self.square_list}"
 
     def __add__(self, other: Move) -> Move:
         """Append moves"""
         if self.square_list[-1] != other.square_list[0]:
             raise ValueError(
                 f"Cannot append moves {self} and {other}. Last square of first move should be equal to first square of second move."
             )
```

### Comparing `fast-checkers-0.0.3/fast_checkers.egg-info/PKG-INFO` & `fast-checkers-0.0.4/fast_checkers.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.0.3
+Version: 0.0.4
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,24 +25,28 @@
 
 ```bash
 python -m pip install fast-checkers 
 ```
 
 ## Usage:
 
+### simple
+
 ```python
-import checkers
-from checkers.american_board import AmericanBoard, Move 
-board = AmericanBoard()
-move = Move([A3, B4])
+import checkers.american as checkers
+board = checkers.Board()
+move = checkers.Move([checkers.A3, checkers.B4])
 board.push(move)
+
+print(list(board.legal_moves))
 print(board)
 ```
 
 ```bash
+['Move through squares: [8, 12]', 'Move through squares: [8, 13]', 'Move through squares: [9, 13]', 'Move through squares: [9, 14]', 'Move through squares: [10, 14]', 'Move through squares: [10, 15]', 'Move through squares: [11, 15]']
 ---------------------------------
 |   | x |   | x |   | x |   | x |
 ---------------------------------
 | x |   | x |   | x |   | x |   |
 ---------------------------------
 |   | x |   | x |   | x |   | x |
 ---------------------------------
@@ -53,14 +57,48 @@
 | o |   |   |   | o |   | o |   |
 ---------------------------------
 |   | o |   | o |   | o |   | o |
 ---------------------------------
 | o |   | o |   | o |   | o |   |
 ```
 
+### advenced:
+
+```python
+import checkers.base as checkers
+import numpy as np
+CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
+board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
+board.legal_moves = ... # create your own custom legal_moves method (property)
+print(board)
+print(board.legal_moves)
+```
+
+```bash
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| x |   | x |   | x |   | x |   |
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| x |   | x |   | x |   | x |   |
+---------------------------------
+|   | x |   | x |   | x |   | x |
+---------------------------------
+| o |   | o |   | o |   | o |   |
+---------------------------------
+|   | o |   | o |   | o |   | o |
+---------------------------------
+| o |   | o |   | o |   | o |   |
+
+Ellipsis
+```
+
+
 ## Bibliography
 1. [notatin](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
 2. [rules and variants](https://en.wikipedia.org/wiki/Checkers)
 3. [additional 1 (checkers online)](https://checkers.online/play)
 4. [additional 2 (chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
 
 ## Contributing
```

### Comparing `fast-checkers-0.0.3/setup.py` & `fast-checkers-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="fast-checkers",
-    version="0.0.3",
+    version="0.0.4",
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     files_to_include=["checkers"],
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

### Comparing `fast-checkers-0.0.3/test/test_board.py` & `fast-checkers-0.0.4/test/test_board.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from checkers.base_board import (
+from checkers.base import (
     BaseBoard,
     Color,
     Move,
     STARTING_POSITION,
     Entity,
 )
 import checkers
```

