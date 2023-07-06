# Comparing `tmp/dndfog-0.6.2.tar.gz` & `tmp/dndfog-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dndfog-0.6.2.tar", max compression
+gzip compressed data, was "dndfog-0.6.3.tar", max compression
```

## Comparing `dndfog-0.6.2.tar` & `dndfog-0.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2022-07-16 18:14:13.435341 dndfog-0.6.2/dndfog/__init__.py
--rw-r--r--   0        0        0     3221 2023-03-03 21:08:09.362534 dndfog-0.6.2/dndfog/_aoe.py
--rw-r--r--   0        0        0     1663 2023-03-03 21:45:04.825940 dndfog-0.6.2/dndfog/camera.py
--rw-r--r--   0        0        0      673 2023-04-30 05:40:21.761087 dndfog-0.6.2/dndfog/draw/__init__.py
--rw-r--r--   0        0        0     1615 2023-03-05 11:50:47.883429 dndfog-0.6.2/dndfog/draw/generic.py
--rw-r--r--   0        0        0     2793 2023-03-05 13:04:18.410213 dndfog-0.6.2/dndfog/draw/map.py
--rw-r--r--   0        0        0     7133 2023-03-05 12:04:24.440504 dndfog-0.6.2/dndfog/draw/toolbar.py
--rw-r--r--   0        0        0     8638 2023-04-30 05:39:32.017856 dndfog-0.6.2/dndfog/event_handlers.py
--rw-r--r--   0        0        0     1188 2023-03-04 10:13:55.536095 dndfog-0.6.2/dndfog/fog.py
--rw-r--r--   0        0        0     1251 2023-03-04 09:41:04.665316 dndfog-0.6.2/dndfog/gameloop.py
--rw-r--r--   0        0        0      623 2023-03-03 21:45:05.195611 dndfog-0.6.2/dndfog/grid.py
--rw-r--r--   0        0        0      641 2023-04-30 06:01:12.709340 dndfog-0.6.2/dndfog/main.py
--rw-r--r--   0        0        0      746 2023-03-03 21:45:04.701005 dndfog-0.6.2/dndfog/map.py
--rw-r--r--   0        0        0     3097 2023-03-05 13:09:35.096950 dndfog-0.6.2/dndfog/markings.py
--rw-r--r--   0        0        0      477 2023-03-05 10:01:20.693142 dndfog-0.6.2/dndfog/math.py
--rw-r--r--   0        0        0     3283 2023-03-05 11:16:15.289422 dndfog-0.6.2/dndfog/piece.py
--rw-r--r--   0        0        0     6606 2023-04-30 05:39:50.391106 dndfog-0.6.2/dndfog/saving.py
--rw-r--r--   0        0        0     3631 2023-03-05 12:02:43.899586 dndfog-0.6.2/dndfog/toolbar.py
--rw-r--r--   0        0        0     7992 2023-03-05 13:23:14.983423 dndfog-0.6.2/dndfog/types.py
--rw-r--r--   0        0        0     1090 2022-01-21 22:49:34.887128 dndfog-0.6.2/LICENSE
--rw-r--r--   0        0        0     2682 2023-04-30 05:40:37.925296 dndfog-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5461 2023-03-06 18:21:44.672857 dndfog-0.6.2/README.md
--rw-r--r--   0        0        0     6465 1970-01-01 00:00:00.000000 dndfog-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-16 18:14:13.435341 dndfog-0.6.3/dndfog/__init__.py
+-rw-r--r--   0        0        0     3221 2023-03-03 21:08:09.362534 dndfog-0.6.3/dndfog/_aoe.py
+-rw-r--r--   0        0        0     1663 2023-03-03 21:45:04.825940 dndfog-0.6.3/dndfog/camera.py
+-rw-r--r--   0        0        0      673 2023-04-30 05:40:21.761087 dndfog-0.6.3/dndfog/draw/__init__.py
+-rw-r--r--   0        0        0     1615 2023-03-05 11:50:47.883429 dndfog-0.6.3/dndfog/draw/generic.py
+-rw-r--r--   0        0        0     2793 2023-03-05 13:04:18.410213 dndfog-0.6.3/dndfog/draw/map.py
+-rw-r--r--   0        0        0     7133 2023-03-05 12:04:24.440504 dndfog-0.6.3/dndfog/draw/toolbar.py
+-rw-r--r--   0        0        0     9044 2023-07-06 07:11:49.278602 dndfog-0.6.3/dndfog/event_handlers.py
+-rw-r--r--   0        0        0     1188 2023-03-04 10:13:55.536095 dndfog-0.6.3/dndfog/fog.py
+-rw-r--r--   0        0        0     1251 2023-03-04 09:41:04.665316 dndfog-0.6.3/dndfog/gameloop.py
+-rw-r--r--   0        0        0      623 2023-03-03 21:45:05.195611 dndfog-0.6.3/dndfog/grid.py
+-rw-r--r--   0        0        0      696 2023-07-06 07:11:49.278602 dndfog-0.6.3/dndfog/main.py
+-rw-r--r--   0        0        0      746 2023-03-03 21:45:04.701005 dndfog-0.6.3/dndfog/map.py
+-rw-r--r--   0        0        0     3097 2023-03-05 13:09:35.096950 dndfog-0.6.3/dndfog/markings.py
+-rw-r--r--   0        0        0      477 2023-03-05 10:01:20.693142 dndfog-0.6.3/dndfog/math.py
+-rw-r--r--   0        0        0     3283 2023-03-05 11:16:15.289422 dndfog-0.6.3/dndfog/piece.py
+-rw-r--r--   0        0        0     6842 2023-07-06 07:11:49.279600 dndfog-0.6.3/dndfog/saving.py
+-rw-r--r--   0        0        0     3631 2023-03-05 12:02:43.899586 dndfog-0.6.3/dndfog/toolbar.py
+-rw-r--r--   0        0        0     7992 2023-03-05 13:23:14.983423 dndfog-0.6.3/dndfog/types.py
+-rw-r--r--   0        0        0     1090 2022-01-21 22:49:34.887128 dndfog-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2682 2023-07-06 07:17:36.088194 dndfog-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5476 2023-07-06 07:11:49.252589 dndfog-0.6.3/README.md
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 dndfog-0.6.3/PKG-INFO
```

### Comparing `dndfog-0.6.2/dndfog/_aoe.py` & `dndfog-0.6.3/dndfog/_aoe.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/camera.py` & `dndfog-0.6.3/dndfog/camera.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/draw/__init__.py` & `dndfog-0.6.3/dndfog/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/draw/generic.py` & `dndfog-0.6.3/dndfog/draw/generic.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/draw/map.py` & `dndfog-0.6.3/dndfog/draw/map.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/draw/toolbar.py` & `dndfog-0.6.3/dndfog/draw/toolbar.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/event_handlers.py` & `dndfog-0.6.3/dndfog/event_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dndfog.camera import move_camera, zoom_camera
 from dndfog.fog import add_fog, remove_fog
 from dndfog.grid import grid_position
 from dndfog.map import move_map, zoom_map
 from dndfog.markings import add_markings, move_markings, remove_markings
 from dndfog.piece import add_piece, move_piece, remove_piece
-from dndfog.saving import open_data_file, open_file_dialog, save_data_file, save_file_dialog
+from dndfog.saving import get_default_filename, open_data_file, open_file_dialog, save_data_file, save_file_dialog
 from dndfog.toolbar import (
     TOOLBAR_HEIGHT,
     select_button,
     select_checkbox,
     select_indicator,
     select_size_tool,
     set_indicator,
@@ -63,24 +63,41 @@
         handle_right_mouse_button_held(event, loop, state)
 
 
 def handle_key_down(event: KeyEvent, loop: LoopData, state: ProgramState) -> None:
     # Save data
     if event.mod & pygame.KMOD_CTRL and event.key == pygame.K_s:
         if event.mod & pygame.KMOD_SHIFT or state.file is None:
-            file = save_file_dialog(title="Save Map", ext=[("Json file", "json")], default_ext="json")
+            filename = get_default_filename(state)
+
+            file = save_file_dialog(
+                title="Save Map",
+                ext=[
+                    ("DND fog file", "dndfog"),
+                    ("Json file", "json"),
+                ],
+                default_name=filename,
+                default_ext="dndfog",
+            )
             if file:
                 state.file = file
                 save_data_file(state)
         else:
             save_data_file(state)
 
     # Load data
     elif event.mod & pygame.KMOD_CTRL and event.key == pygame.K_o:
-        path = open_file_dialog(title="Open Map", ext=[("Json file", "json")], default_ext="json")
+        path = open_file_dialog(
+            title="Open Map",
+            ext=[
+                ("DND fog file", "dndfog"),
+                ("Json file", "json"),
+            ],
+            default_ext="dndfog",
+        )
         if path:
             state.file = path
             open_data_file(state)
 
     # Hide/Show toolbar
     elif event.key == pygame.K_TAB:
         state.show.toolbar = not state.show.toolbar
```

### Comparing `dndfog-0.6.2/dndfog/fog.py` & `dndfog-0.6.3/dndfog/fog.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/gameloop.py` & `dndfog-0.6.3/dndfog/gameloop.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/grid.py` & `dndfog-0.6.3/dndfog/grid.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/main.py` & `dndfog-0.6.3/dndfog/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from argparse import ArgumentParser
-
-from dndfog.gameloop import run
-from dndfog.saving import open_file_dialog
-
-
-def start() -> None:
-    parser = ArgumentParser()
-    parser.add_argument("file", default=None)
-    args = parser.parse_args()
-
-    if args.file is not None:
-        map_file = str(args.file)
-    else:
-        map_file = open_file_dialog(
-            title="Select a background map, or a json data file",
-            ext=[("PNG file", "png"), ("JPG file", "jpg"), ("JSON file", "json")],
-        )
-
-    if not map_file:
-        raise SystemExit("No file selected.")
-
-    run(map_file)
-
-
-if __name__ == "__main__":
-    start()
+from argparse import ArgumentParser
+
+from dndfog.gameloop import run
+from dndfog.saving import open_file_dialog
+
+
+def start() -> None:
+    parser = ArgumentParser()
+    parser.add_argument("file", default=None)
+    args = parser.parse_args()
+
+    if args.file is not None:
+        map_file = str(args.file)
+    else:
+        map_file = open_file_dialog(
+            title="Select a background map, or a json data file",
+            ext=[("PNG file", "png"), ("JPG file", "jpg"), ("JSON file", "json"), ("DND fog file", "dndfog")],
+        )
+
+    if not map_file:
+        raise SystemExit("No file selected.")
+
+    run(map_file)
+
+
+if __name__ == "__main__":
+    start()
```

### Comparing `dndfog-0.6.2/dndfog/map.py` & `dndfog-0.6.3/dndfog/map.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/markings.py` & `dndfog-0.6.3/dndfog/markings.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/piece.py` & `dndfog-0.6.3/dndfog/piece.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/saving.py` & `dndfog-0.6.3/dndfog/saving.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,7 +213,16 @@
 
 def deserialize_map(data: BackgroundImage) -> pygame.Surface:
     return pygame.image.fromstring(
         gzip.decompress(base64.b64decode(data["img"])),
         data["size"],
         data["mode"],
     ).convert_alpha()
+
+
+def get_default_filename(state: ProgramState) -> str:
+    if state.file is None:
+        return ""
+
+    filename = state.file.rsplit("/", maxsplit=1)[-1]
+    filename = filename.rsplit(".", maxsplit=1)[0]
+    return filename
```

### Comparing `dndfog-0.6.2/dndfog/toolbar.py` & `dndfog-0.6.3/dndfog/toolbar.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/dndfog/types.py` & `dndfog-0.6.3/dndfog/types.py`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/LICENSE` & `dndfog-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dndfog-0.6.2/pyproject.toml` & `dndfog-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dndfog"
-version = "0.6.2"
+version = "0.6.3"
 description = "DND battle map with fog of war"
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "dndfog" },
 ]
@@ -39,32 +39,32 @@
 exclude = [
     "tests",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 pywin32 = "306"
-pygame-ce = ">=2.2.1"
+pygame-ce = "2.3.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.3.1"
+pytest = "7.4.0"
 coverage = "6.5.0"
-pre-commit = "3.2.2"
-tox = "4.5.1"
-tox-gh-actions = "3.1.0"
+pre-commit = "3.3.3"
+tox = "4.6.3"
+tox-gh-actions = "3.1.1"
 coveralls = "3.3.1"
-pyinstaller = "5.10.1"
+pyinstaller = "5.13.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.2"
-pymdown-extensions = "9.11"
+mkdocs = "1.4.3"
+pymdown-extensions = "10.0.1"
 mkdocs-mermaid2-plugin = "0.6.0"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "1.2.0"
+mypy = "1.4.1"
 
 [tool.poetry.scripts]
 dndfog = "dndfog.main:start"
 
 [tool.black]
 line-length = 120
 
@@ -127,9 +127,9 @@
     PYTHONPATH = {toxinidir}
 commands =
     poetry install
     poetry run coverage run -m pytest -vv -s --log-cli-level=INFO
 """
 
 [build-system]
-requires = ["poetry-core>=1.4.0"]
+requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dndfog-0.6.2/README.md` & `dndfog-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 When installing from [pypi](https://pypi.org/), the library should come with a script
 named `dndfog` that you can run. It should be available in your environment if
 the `Python\Scripts` folder is set in PATH. You can also download an EXE from
 the [GitHub releases](https://github.com/MrThearMan/dndfog/releases).
 
 When the program opens, you need to select an image file to use as a background,
 or a JSON data file to load a map from. You can also lauch the program with
-`--file=<filepath>` to add an initial file.
+a positional argument `<filepath>` to add an initial file.
 
 > The program does not autosave! You have to save (and override) the file yourself!
 
 ### Keyboard shortcuts
 
 Toolbar:
 - Open/close the toolbar: `TAB`
```

### Comparing `dndfog-0.6.2/PKG-INFO` & `dndfog-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dndfog
-Version: 0.6.2
+Version: 0.6.3
 Summary: DND battle map with fog of war
 Home-page: https://mrthearman.github.io/dndfog/
 License: MIT
 Keywords: dnd,fog,war,map,combat,infinite,gird
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.10,<3.12
@@ -13,19 +13,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pygame-ce (>=2.2.1)
+Requires-Dist: pygame-ce (==2.3.0)
 Requires-Dist: pywin32 (==306)
 Project-URL: Repository, https://github.com/MrThearMan/dndfog
 Description-Content-Type: text/markdown
 
 # DnD Fog
 
 [![GitHub Workflow Status][status-badge]][status]
@@ -71,15 +68,15 @@
 When installing from [pypi](https://pypi.org/), the library should come with a script
 named `dndfog` that you can run. It should be available in your environment if
 the `Python\Scripts` folder is set in PATH. You can also download an EXE from
 the [GitHub releases](https://github.com/MrThearMan/dndfog/releases).
 
 When the program opens, you need to select an image file to use as a background,
 or a JSON data file to load a map from. You can also lauch the program with
-`--file=<filepath>` to add an initial file.
+a positional argument `<filepath>` to add an initial file.
 
 > The program does not autosave! You have to save (and override) the file yourself!
 
 ### Keyboard shortcuts
 
 Toolbar:
 - Open/close the toolbar: `TAB`
```

