# Comparing `tmp/retro_games-0.1.1.tar.gz` & `tmp/retro_games-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retro_games-0.1.1.tar", max compression
+gzip compressed data, was "retro_games-0.1.2.tar", max compression
```

## Comparing `retro_games-0.1.1.tar` & `retro_games-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1593 2023-07-03 13:56:37.141970 retro_games-0.1.1/README.md
--rw-r--r--   0        0        0      375 2023-07-03 14:46:13.112524 retro_games-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      684 2023-07-03 11:52:59.620127 retro_games-0.1.1/retro/agent.py
--rw-r--r--   0        0        0     1264 2023-06-23 20:02:01.765416 retro_games-0.1.1/retro/errors.py
--rw-r--r--   0        0        0     3223 2023-07-03 14:40:26.118705 retro_games-0.1.1/retro/examples/snake/__main__.py
--rw-r--r--   0        0        0     3360 2023-07-03 14:39:39.969190 retro_games-0.1.1/retro/game.py
--rw-r--r--   0        0        0     5002 2023-06-23 20:15:55.974027 retro_games-0.1.1/retro/graph.py
--rw-r--r--   0        0        0      108 2023-06-23 19:55:22.313279 retro_games-0.1.1/retro/grid.py
--rw-r--r--   0        0        0     1444 2023-06-19 17:38:15.819682 retro_games-0.1.1/retro/validation.py
--rw-r--r--   0        0        0     4868 2023-07-03 14:42:42.259705 retro_games-0.1.1/retro/view.py
--rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 retro_games-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1593 2023-07-03 13:56:37.141970 retro_games-0.1.2/README.md
+-rw-r--r--   0        0        0      517 2023-07-06 15:07:14.610929 retro_games-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4328 2023-07-06 13:47:36.638402 retro_games-0.1.2/retro/agent.py
+-rw-r--r--   0        0        0     1499 2023-07-06 12:34:17.692538 retro_games-0.1.2/retro/errors.py
+-rw-r--r--   0        0        0      127 2023-07-04 16:02:45.226657 retro_games-0.1.2/retro/examples/debug.py
+-rw-r--r--   0        0        0     5219 2023-07-06 13:53:58.493663 retro_games-0.1.2/retro/examples/nav.py
+-rw-r--r--   0        0        0      142 2023-07-04 22:51:11.896137 retro_games-0.1.2/retro/examples/simple.py
+-rw-r--r--   0        0        0     8148 2023-07-04 00:19:49.688332 retro_games-0.1.2/retro/examples/snake.py
+-rw-r--r--   0        0        0     7291 2023-07-06 12:43:40.365129 retro_games-0.1.2/retro/game.py
+-rw-r--r--   0        0        0     5002 2023-06-23 20:15:55.974027 retro_games-0.1.2/retro/graph.py
+-rw-r--r--   0        0        0      108 2023-06-23 19:55:22.313279 retro_games-0.1.2/retro/grid.py
+-rw-r--r--   0        0        0     1438 2023-07-06 12:37:15.450356 retro_games-0.1.2/retro/validation.py
+-rw-r--r--   0        0        0     4868 2023-07-03 14:42:42.259705 retro_games-0.1.2/retro/view.py
+-rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 retro_games-0.1.2/PKG-INFO
```

### Comparing `retro_games-0.1.1/README.md` & `retro_games-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `retro_games-0.1.1/retro/errors.py` & `retro_games-0.1.2/retro/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 class GameError(Exception):
     pass
 
-class AgentAlreadyExists(GameError):
+class AgentWithNameAlreadyExists(GameError):
     def __init__(self, name):
         message = f"There is already an agent named {agent.name} in the game"
         super().__init__(message)
 
-class AgentNotFound(GameError):
+class AgentNotFoundByName(GameError):
     def __init__(self, name):
         message = f"There is no agent named {agent.name} in the game"
         super().__init__(message)
 
+class AgentNotInGame(GameError):
+    def __init__(self, agent):
+        name = agent.name or f"anonymous {agent.__class__.__name__}"
+        message = f"Agent {name} is not in the game"
+        super().__init__(message)
+
 class IllegalMove(GameError):
     def __init__(self, agent, position):
         message = f"Agent {agent.name} tried to move to {position}"
         super().__init__(message)
 
 class GraphError(GameError):
     pass
```

### Comparing `retro_games-0.1.1/retro/graph.py` & `retro_games-0.1.2/retro/graph.py`

 * *Files identical despite different names*

### Comparing `retro_games-0.1.1/retro/validation.py` & `retro_games-0.1.2/retro/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 def validate_agent(agent):
-    if not hasattr(agent, "name"):
-        raise ValueError(f"Agent {agent} must have a name")
-    if not hasattr(agent, "position"):
-        raise ValueError(f"Agent {agent.name} must have a position")
-    validate_agent_name(agent.name)
-    validate_position(agent.position)
+    if hasattr(agent, "name"):
+        validate_agent_name(agent.name)
+    if getattr(agent, 'display', True):
+        validate_position(agent.position)
+        if not hasattr(agent, "character"):
+            raise ValueError(f"Agent {agent.name} must have a character")
     return agent
 
 def validate_state(state):
     if not isinstance(state, dict):
         raise TypeError(f"State is {type(state)}, but must be a dict.")
     for key, value in state.items():
         if is_mutable(value):
```

### Comparing `retro_games-0.1.1/retro/view.py` & `retro_games-0.1.2/retro/view.py`

 * *Files identical despite different names*

### Comparing `retro_games-0.1.1/PKG-INFO` & `retro_games-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: retro-games
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple framework for Terminal-based games
+Home-page: https://makingwithcode.org
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: blessed (>=1.20.0,<2.0.0)
+Requires-Dist: furo (>=2023.5.20,<2024.0.0)
+Requires-Dist: sphinx (>=7.0.1,<8.0.0)
+Project-URL: Documentation, https://retro-games.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # Retro
 
 A simple framework for Terminal-based games.
 
 ```
```

