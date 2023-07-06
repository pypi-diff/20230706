# Comparing `tmp/une_ai-1.1.1.tar.gz` & `tmp/une_ai-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "une_ai-1.1.1.tar", last modified: Mon Jun 26 09:12:31 2023, max compression
+gzip compressed data, was "une_ai-1.1.2.tar", last modified: Thu Jul  6 02:32:11 2023, max compression
```

## Comparing `une_ai-1.1.1.tar` & `une_ai-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.260414 une_ai-1.1.1/
--rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.1.1/LICENSE
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-26 09:12:31.260253 une_ai-1.1.1/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.1.1/README.md
--rw-r--r--   0 jonathan   (501) staff       (20)      481 2023-06-26 09:11:57.000000 une_ai-1.1.1/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-06-26 09:12:31.260479 une_ai-1.1.1/setup.cfg
--rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.1.1/setup.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.253924 une_ai-1.1.1/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.254947 une_ai-1.1.1/src/une_ai/
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.1.1/src/une_ai/__init__.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.256622 une_ai-1.1.1/src/une_ai/assignments/
--rw-r--r--   0 jonathan   (501) staff       (20)      198 2023-06-17 05:23:26.000000 une_ai-1.1.1/src/une_ai/assignments/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)    12875 2023-06-25 01:46:33.000000 une_ai-1.1.1/src/une_ai/assignments/connect_four_base_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     9692 2023-06-26 09:10:11.000000 une_ai-1.1.1/src/une_ai/assignments/connect_four_game.py
--rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.1.1/src/une_ai/assignments/snake_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5992 2023-06-26 09:09:49.000000 une_ai-1.1.1/src/une_ai/assignments/snake_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.258732 une_ai-1.1.1/src/une_ai/models/
--rw-r--r--   0 jonathan   (501) staff       (20)     1323 2023-06-25 00:13:50.000000 une_ai-1.1.1/src/une_ai/models/MCTS_graph_node.py
--rw-r--r--   0 jonathan   (501) staff       (20)      254 2023-06-24 12:38:18.000000 une_ai-1.1.1/src/une_ai/models/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.1.1/src/une_ai/models/agent.py
--rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.1.1/src/une_ai/models/environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1083 2023-06-22 07:56:49.000000 une_ai-1.1.1/src/une_ai/models/game_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1312 2023-06-12 07:15:34.000000 une_ai-1.1.1/src/une_ai/models/graph_node.py
--rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.1.1/src/une_ai/models/grid_map.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5827 2023-06-24 06:33:53.000000 une_ai-1.1.1/src/une_ai/models/transposition_table.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.259554 une_ai-1.1.1/src/une_ai/tictactoe/
--rw-r--r--   0 jonathan   (501) staff       (20)       87 2023-06-25 01:53:59.000000 une_ai-1.1.1/src/une_ai/tictactoe/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)     1332 2023-06-25 02:53:44.000000 une_ai-1.1.1/src/une_ai/tictactoe/tictactoc_player.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5011 2023-06-26 09:10:25.000000 une_ai-1.1.1/src/une_ai/tictactoe/tictactoe_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.260044 une_ai-1.1.1/src/une_ai/vacuum/
--rw-r--r--   0 jonathan   (501) staff       (20)      186 2023-06-12 02:00:34.000000 une_ai-1.1.1/src/une_ai/vacuum/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)      910 2023-06-12 07:14:58.000000 une_ai-1.1.1/src/une_ai/vacuum/vacuum_dock_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.1.1/src/une_ai/vacuum/vacuum_environment.py
--rw-r--r--   0 jonathan   (501) staff       (20)     5948 2023-06-26 09:10:38.000000 une_ai-1.1.1/src/une_ai/vacuum/vacuum_game.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-06-26 09:12:31.255702 une_ai-1.1.1/src/une_ai.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-06-26 09:12:30.000000 une_ai-1.1.1/src/une_ai.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      978 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       19 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-06-26 09:12:31.000000 une_ai-1.1.1/src/une_ai.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.318954 une_ai-1.1.2/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1088 2023-04-26 02:42:42.000000 une_ai-1.1.2/LICENSE
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-07-06 02:32:11.318806 une_ai-1.1.2/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)     4475 2023-06-12 00:05:49.000000 une_ai-1.1.2/README.md
+-rw-r--r--   0 jonathan   (501) staff       (20)      481 2023-07-06 02:31:19.000000 une_ai-1.1.2/pyproject.toml
+-rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-07-06 02:32:11.318999 une_ai-1.1.2/setup.cfg
+-rw-r--r--   0 jonathan   (501) staff       (20)       91 2023-04-26 01:50:26.000000 une_ai-1.1.2/setup.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.310082 une_ai-1.1.2/src/
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.311252 une_ai-1.1.2/src/une_ai/
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-16 02:02:27.000000 une_ai-1.1.2/src/une_ai/__init__.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.313753 une_ai-1.1.2/src/une_ai/assignments/
+-rw-r--r--   0 jonathan   (501) staff       (20)      198 2023-06-17 05:23:26.000000 une_ai-1.1.2/src/une_ai/assignments/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)    12875 2023-06-25 01:46:33.000000 une_ai-1.1.2/src/une_ai/assignments/connect_four_base_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     9726 2023-07-03 03:32:39.000000 une_ai-1.1.2/src/une_ai/assignments/connect_four_game.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     7263 2023-06-04 07:45:17.000000 une_ai-1.1.2/src/une_ai/assignments/snake_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     6359 2023-07-05 01:56:22.000000 une_ai-1.1.2/src/une_ai/assignments/snake_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.316305 une_ai-1.1.2/src/une_ai/models/
+-rw-r--r--   0 jonathan   (501) staff       (20)     1323 2023-06-25 00:13:50.000000 une_ai-1.1.2/src/une_ai/models/MCTS_graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      254 2023-06-24 12:38:18.000000 une_ai-1.1.2/src/une_ai/models/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5409 2023-06-04 07:46:40.000000 une_ai-1.1.2/src/une_ai/models/agent.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      357 2023-06-04 03:18:52.000000 une_ai-1.1.2/src/une_ai/models/environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1083 2023-06-22 07:56:49.000000 une_ai-1.1.2/src/une_ai/models/game_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1312 2023-06-12 07:15:34.000000 une_ai-1.1.2/src/une_ai/models/graph_node.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     2198 2023-05-26 04:05:50.000000 une_ai-1.1.2/src/une_ai/models/grid_map.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5827 2023-06-24 06:33:53.000000 une_ai-1.1.2/src/une_ai/models/transposition_table.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.317226 une_ai-1.1.2/src/une_ai/tictactoe/
+-rw-r--r--   0 jonathan   (501) staff       (20)       87 2023-06-25 01:53:59.000000 une_ai-1.1.2/src/une_ai/tictactoe/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     1313 2023-07-04 01:51:27.000000 une_ai-1.1.2/src/une_ai/tictactoe/tictactoc_player.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     5517 2023-07-04 04:24:19.000000 une_ai-1.1.2/src/une_ai/tictactoe/tictactoe_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.318446 une_ai-1.1.2/src/une_ai/vacuum/
+-rw-r--r--   0 jonathan   (501) staff       (20)      186 2023-06-12 02:00:34.000000 une_ai-1.1.2/src/une_ai/vacuum/__init__.py
+-rw-r--r--   0 jonathan   (501) staff       (20)      910 2023-06-12 07:14:58.000000 une_ai-1.1.2/src/une_ai/vacuum/vacuum_dock_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     8119 2023-06-06 11:02:22.000000 une_ai-1.1.2/src/une_ai/vacuum/vacuum_environment.py
+-rw-r--r--   0 jonathan   (501) staff       (20)     6332 2023-07-05 01:33:24.000000 une_ai-1.1.2/src/une_ai/vacuum/vacuum_game.py
+drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-07-06 02:32:11.312136 une_ai-1.1.2/src/une_ai.egg-info/
+-rw-r--r--   0 jonathan   (501) staff       (20)     6030 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan   (501) staff       (20)      978 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)       19 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/requires.txt
+-rw-r--r--   0 jonathan   (501) staff       (20)        7 2023-07-06 02:32:11.000000 une_ai-1.1.2/src/une_ai.egg-info/top_level.txt
```

### Comparing `une_ai-1.1.1/LICENSE` & `une_ai-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/PKG-INFO` & `une_ai-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une_ai
-Version: 1.1.1
+Version: 1.1.2
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.1.1/README.md` & `une_ai-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/assignments/connect_four_base_environment.py` & `une_ai-1.1.2/src/une_ai/assignments/connect_four_base_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/assignments/connect_four_game.py` & `une_ai-1.1.2/src/une_ai/assignments/connect_four_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         cur_colour = type(self._environment).turn(game_state)
         
         # SENSE
         self._agents[cur_colour].sense(self._environment)
         # THINK
         actions = self._agents[cur_colour].think()
         player = 'Yellow' if cur_colour == 'Y' else 'Red'
-        self._last_action = "{0} player played the move '{1}'".format(player, actions[0])
+        if len(actions) != 0:
+            self._last_action = "{0} player played the move '{1}'".format(player, actions[0])
         # ACT
         self._agents[cur_colour].act(actions, self._environment)
     
     def _reset_bg(self):
         self._display.fill(BLACK)
     
     def _draw_box(self, x, y, color, alpha = 255):
```

### Comparing `une_ai-1.1.1/src/une_ai/assignments/snake_environment.py` & `une_ai-1.1.2/src/une_ai/assignments/snake_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/assignments/snake_game.py` & `une_ai-1.1.2/src/une_ai/assignments/snake_game.py`

 * *Files 13% similar despite different names*

```diff
@@ -99,23 +99,30 @@
             pygame.draw.rect(self._display, WHITE, pygame.Rect(x_coord, y_coord, self._display_size[0], self._display_size[1] - y_coord))
     
     def _draw_score_bar(self):
         surface = pygame.Surface((DISPLAY_WIDTH,SCORE_BAR_HEIGHT))
         pygame.draw.rect(surface, WHITE, surface.get_rect())
         self._display.blit(surface, (0, DISPLAY_HEIGHT,DISPLAY_WIDTH,SCORE_BAR_HEIGHT) )
         font = pygame.font.SysFont(self._font, 15)
-        score_text = font.render("Score: {0}".format(self._environment.get_score()), True, BLACK)
+        score_text_str = "Score: {0}".format(self._environment.get_score())
+        score_text_size = font.size(score_text_str)
+        score_text = font.render(score_text_str, True, BLACK)
         if self._environment.is_game_over():
             time = 0
         else:
             time = int(self._environment.get_time())
-        time_text = font.render("Time: {0}".format(time), True, BLACK)
-        padding = 15
-        self._display.blit(score_text, (padding, DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2)-padding, SCORE_BAR_HEIGHT))
-        self._display.blit(time_text, (int(DISPLAY_WIDTH/2), DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2), SCORE_BAR_HEIGHT))
+        time_text_str = "Time: {0}".format(time)
+        time_text_size = font.size(time_text_str)
+        time_text = font.render(time_text_str, True, BLACK)
+        padding_top = int((SCORE_BAR_HEIGHT - score_text_size[1]) / 2)
+        white_space = DISPLAY_WIDTH - score_text_size[0] - time_text_size[0]
+        padding_side = int(white_space * 0.25)
+        padding_central = white_space - 2 * padding_side
+        self._display.blit(score_text, (padding_side, DISPLAY_HEIGHT+padding_top))
+        self._display.blit(time_text, (padding_side + score_text_size[0] + padding_central, DISPLAY_HEIGHT+padding_top))
     
     def _draw_game_over(self):
         surface = pygame.Surface((DISPLAY_WIDTH,DISPLAY_HEIGHT))
         surface.set_alpha(60)
         pygame.draw.rect(surface, WHITE, surface.get_rect())
         y_pos = int((DISPLAY_HEIGHT-GAME_OVER_HEIGHT)/2)
         self._display.blit(surface, (0, 0, DISPLAY_WIDTH,DISPLAY_HEIGHT) )
```

### Comparing `une_ai-1.1.1/src/une_ai/models/MCTS_graph_node.py` & `une_ai-1.1.2/src/une_ai/models/MCTS_graph_node.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/models/agent.py` & `une_ai-1.1.2/src/une_ai/models/agent.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/models/game_environment.py` & `une_ai-1.1.2/src/une_ai/models/game_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/models/graph_node.py` & `une_ai-1.1.2/src/une_ai/models/graph_node.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/models/grid_map.py` & `une_ai-1.1.2/src/une_ai/models/grid_map.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/models/transposition_table.py` & `une_ai-1.1.2/src/une_ai/models/transposition_table.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/tictactoe/tictactoc_player.py` & `une_ai-1.1.2/src/une_ai/tictactoe/tictactoc_player.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from une_ai.models import Agent, GridMap
 
 class TicTacToePlayer(Agent):
 
     def __init__(self, agent_name, agent_program, board_size=3):
         self._board_size = board_size
         super().__init__(agent_name, agent_program)
```

### Comparing `une_ai-1.1.1/src/une_ai/tictactoe/tictactoe_game.py` & `une_ai-1.1.2/src/une_ai/tictactoe/tictactoe_game.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import pygame
 
+from une_ai.models import GridMap
+
 BLACK = (0, 0, 0)
 WHITE = (255, 255, 255)
 RED = (255, 0, 0)
 BLUE = (0, 0, 255)
 
 DISPLAY_WIDTH = 320
 DISPLAY_HEIGHT = 240
 SCORE_BAR_HEIGHT = 40
 BOX_SIZE = 50
 
 class TicTacToeGame:
 
-    def __init__(self, agent_X, agent_O, environment, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, box_size=BOX_SIZE):
+    def __init__(self, agent_X, agent_O, environment, board_size=3, display_w=DISPLAY_WIDTH, display_h=DISPLAY_HEIGHT, box_size=BOX_SIZE):
         assert type(agent_X).__name__ == 'TicTacToePlayer', "agent_X must be an instance of a the class TicTacToePlayer"
         assert type(agent_O).__name__ == 'TicTacToePlayer', "agent_O must be an instance of the class TicTacToePlayer"
         assert type(environment).__name__ == 'TicTacToeGameEnvironment', "The parameter environment must be an instance of the class TicTacToeGameEnvironment"
         
         pygame.init()
         window = pygame.display.set_mode((DISPLAY_WIDTH, DISPLAY_HEIGHT+SCORE_BAR_HEIGHT))
         pygame.display.set_caption('Tic Tac Toe')
@@ -25,14 +27,15 @@
         self._box_size = box_size
         self._display = window
         self._display_size = (display_w, display_h)
         self._agents = {}
         self._agents['X'] = agent_X
         self._agents['O'] = agent_O
         self._environment = environment
+        self._board_size = board_size
         
         fonts = pygame.font.get_fonts()
         self._font = fonts[0] # default to a random font
         # try to look among the most common fonts
         test_fonts = ['arial', 'couriernew', 'verdana', 'helvetica', 'roboto']
         for font in test_fonts:
             if font in fonts:
@@ -42,65 +45,74 @@
         self.main()
         
     def _play_step(self):
         game_state = self._environment.get_game_state()
         if type(self._environment).is_terminal(game_state):
             return
         
-        cur_marker = type(self._environment).turn(game_state)
+        try:
+            cur_marker = type(self._environment).turn(game_state)
+        except:
+            print("Error. The game environment class does not return a correct game state. Skipping updating the game state")
+            return
         
         # SENSE
         self._agents[cur_marker].sense(self._environment)
         # THINK
         actions = self._agents[cur_marker].think()
         # ACT
         self._agents[cur_marker].act(actions, self._environment)
     
     def _reset_bg(self):
         self._display.fill(BLACK)
     
     def _draw_box(self, x, y, color, alpha = 255):
         font = pygame.font.SysFont(self._font, 30)
         game_state = self._environment.get_game_state()
-        n_cells = self._environment.get_board_size()
+        n_cells = self._board_size
         padding_left = int((self._display_size[0] - n_cells*self._box_size)/2)
         padding_top = int((self._display_size[1] - n_cells*self._box_size)/2)
         x_coord = padding_left + x*self._box_size
         y_coord = padding_top + y*self._box_size
 
         surface = pygame.Surface((self._box_size-2,self._box_size-2))
         surface.set_alpha(alpha) # alpha level
         pygame.draw.rect(surface, color, surface.get_rect())
         self._display.blit(surface, (x_coord, y_coord) )
 
-        game_board = game_state['game-board']
+        if isinstance(game_state, dict) and 'game-board' in game_state.keys():
+            game_board = game_state['game-board']
+        else:
+            print("Error. The game environment class does not return a correct game state. Drawing an empty game board.")
+            game_board = GridMap(self._board_size, self._board_size, None)
+
         cur_mark = game_board.get_item_value(x, y)
         if cur_mark != None:
             color = RED if cur_mark == 'X' else BLUE
             text_size = font.size(cur_mark)
             mark_text = font.render(cur_mark, True, color)
             top = y_coord + int((BOX_SIZE - text_size[1])/2)
             left = x_coord + int((BOX_SIZE - text_size[0])/2)
             self._display.blit(mark_text, (left, top))
     
     def _draw_board(self):
-        n_cells = self._environment.get_board_size()
+        n_cells = self._board_size
         for i in range(0, n_cells):
             for j in range(0, n_cells):
                 self._draw_box(j, i, WHITE)
     
     def _draw_game_over(self):
         winner = type(self._environment).get_winner(self._environment.get_game_state())
         
         if winner is not None:
             text = "Player {0} won!".format(winner)
         else:
             text = "Tie!"
         
-        n_cells = self._environment.get_board_size()
+        n_cells = self._board_size
         font = pygame.font.SysFont(self._font, 20)
         text_size = font.size(text)
         game_over_text = font.render(text, True, WHITE)
         padding_top = int((self._display_size[1] - n_cells*self._box_size)/2)
         x_coord = int((self._display_size[0] - text_size[0])/2)
         y_coord = padding_top + n_cells*self._box_size + 30
         self._display.blit(game_over_text, (x_coord, y_coord))
```

### Comparing `une_ai-1.1.1/src/une_ai/vacuum/vacuum_dock_environment.py` & `une_ai-1.1.2/src/une_ai/vacuum/vacuum_dock_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/vacuum/vacuum_environment.py` & `une_ai-1.1.2/src/une_ai/vacuum/vacuum_environment.py`

 * *Files identical despite different names*

### Comparing `une_ai-1.1.1/src/une_ai/vacuum/vacuum_game.py` & `une_ai-1.1.2/src/une_ai/vacuum/vacuum_game.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,19 +118,26 @@
             self._draw_tile(coord[0], coord[1], BLUE, 80)
     
     def _draw_score_bar(self):
         surface = pygame.Surface((DISPLAY_WIDTH,SCORE_BAR_HEIGHT))
         pygame.draw.rect(surface, WHITE, surface.get_rect())
         self._display.blit(surface, (0, DISPLAY_HEIGHT,DISPLAY_WIDTH,SCORE_BAR_HEIGHT) )
         font = pygame.font.SysFont(self._font, 15)
-        score_text = font.render("Score: {0}".format(self._environment.get_score()), True, BLACK)
-        battery_text = font.render("Battery level: {0}%".format(self._agent.get_battery_level()), True, BLACK)
-        padding = 15
-        self._display.blit(score_text, (padding, DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2)-padding, SCORE_BAR_HEIGHT))
-        self._display.blit(battery_text, (int(DISPLAY_WIDTH/2), DISPLAY_HEIGHT+padding, int(DISPLAY_WIDTH/2), SCORE_BAR_HEIGHT))
+        score_text_str = "Score: {0}".format(self._environment.get_score())
+        score_text_size = font.size(score_text_str)
+        score_text = font.render(score_text_str, True, BLACK)
+        battery_text_str = "Battery level: {0}%".format(self._agent.get_battery_level())
+        battery_text_size = font.size(battery_text_str)
+        battery_text = font.render(battery_text_str, True, BLACK)
+        white_space = DISPLAY_WIDTH - score_text_size[0] - battery_text_size[0]
+        padding_top = int((SCORE_BAR_HEIGHT - score_text_size[1]) / 2)
+        padding_side = int(white_space * 0.25)
+        central_padding = white_space - (padding_side * 2)
+        self._display.blit(score_text, (padding_side, DISPLAY_HEIGHT+padding_top))
+        self._display.blit(battery_text, (padding_side + score_text_size[0] + central_padding, DISPLAY_HEIGHT+padding_top))
 
     def _draw_frame(self):
         self._reset_bg()
         self._draw_walls()
         self._draw_explored()
         self._draw_dirt()
         self._draw_charging_dock()
```

### Comparing `une_ai-1.1.1/src/une_ai.egg-info/PKG-INFO` & `une_ai-1.1.2/src/une_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: une-ai
-Version: 1.1.1
+Version: 1.1.2
 Summary: Modules used to facilitate the tutorial sessions for UNE unit COSC350/550
 Author-email: Jonathan Vitale <jvitale@une.edu.au>
 License: MIT License
         
         Copyright (c) 2023, University of New England (UNE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `une_ai-1.1.1/src/une_ai.egg-info/SOURCES.txt` & `une_ai-1.1.2/src/une_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

