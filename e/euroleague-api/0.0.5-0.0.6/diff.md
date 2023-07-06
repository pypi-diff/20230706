# Comparing `tmp/euroleague_api-0.0.5.tar.gz` & `tmp/euroleague_api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euroleague_api-0.0.5.tar", last modified: Sun Jun 25 21:14:15 2023, max compression
+gzip compressed data, was "euroleague_api-0.0.6.tar", last modified: Thu Jul  6 14:12:29 2023, max compression
```

## Comparing `euroleague_api-0.0.5.tar` & `euroleague_api-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 21:14:15.338489 euroleague_api-0.0.5/
--rw-rw-rw-   0        0        0     1097 2023-06-13 23:32:02.000000 euroleague_api-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2209 2023-06-25 21:14:15.338489 euroleague_api-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2023-06-25 20:38:17.000000 euroleague_api-0.0.5/README.md
--rw-rw-rw-   0        0        0       88 2023-06-13 23:33:55.000000 euroleague_api-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      711 2023-06-25 21:14:15.338489 euroleague_api-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 21:14:15.285797 euroleague_api-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:14:15.304996 euroleague_api-0.0.5/src/euroleague_api/
--rw-rw-rw-   0        0        0      336 2023-06-25 21:02:10.000000 euroleague_api-0.0.5/src/euroleague_api/__init__.py
--rw-rw-rw-   0        0        0     4413 2023-06-13 23:33:55.000000 euroleague_api-0.0.5/src/euroleague_api/game_stats.py
--rw-rw-rw-   0        0        0     2697 2023-06-25 20:29:49.000000 euroleague_api-0.0.5/src/euroleague_api/play_by_play_data.py
--rw-rw-rw-   0        0        0    10352 2023-06-13 23:33:55.000000 euroleague_api-0.0.5/src/euroleague_api/player_stats.py
--rw-rw-rw-   0        0        0     2470 2023-06-25 20:30:16.000000 euroleague_api-0.0.5/src/euroleague_api/shot_data.py
--rw-rw-rw-   0        0        0     1323 2023-06-13 23:33:55.000000 euroleague_api-0.0.5/src/euroleague_api/standings.py
--rw-rw-rw-   0        0        0     3804 2023-06-13 23:33:55.000000 euroleague_api-0.0.5/src/euroleague_api/team_stats.py
--rw-rw-rw-   0        0        0    17871 2023-06-13 23:33:55.000000 euroleague_api-0.0.5/src/euroleague_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:14:15.337483 euroleague_api-0.0.5/src/euroleague_api.egg-info/
--rw-rw-rw-   0        0        0     2209 2023-06-25 21:14:15.000000 euroleague_api-0.0.5/src/euroleague_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-25 21:14:15.000000 euroleague_api-0.0.5/src/euroleague_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 21:14:15.000000 euroleague_api-0.0.5/src/euroleague_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-25 21:14:15.000000 euroleague_api-0.0.5/src/euroleague_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 21:14:15.000000 euroleague_api-0.0.5/src/euroleague_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 14:12:29.014089 euroleague_api-0.0.6/
+-rw-rw-rw-   0        0        0     1097 2023-07-06 12:25:08.000000 euroleague_api-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2376 2023-07-06 14:12:29.014089 euroleague_api-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1923 2023-07-06 13:54:10.000000 euroleague_api-0.0.6/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-06 12:25:08.000000 euroleague_api-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      711 2023-07-06 14:12:29.022086 euroleague_api-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 14:12:28.902155 euroleague_api-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 14:12:28.958122 euroleague_api-0.0.6/src/euroleague_api/
+-rw-rw-rw-   0        0        0      387 2023-07-06 13:34:21.000000 euroleague_api-0.0.6/src/euroleague_api/__init__.py
+-rw-rw-rw-   0        0        0     4888 2023-07-06 13:53:31.000000 euroleague_api-0.0.6/src/euroleague_api/boxscore_data.py
+-rw-rw-rw-   0        0        0     4413 2023-07-06 12:25:08.000000 euroleague_api-0.0.6/src/euroleague_api/game_stats.py
+-rw-rw-rw-   0        0        0     2697 2023-07-06 13:21:24.000000 euroleague_api-0.0.6/src/euroleague_api/play_by_play_data.py
+-rw-rw-rw-   0        0        0    10352 2023-07-06 12:25:08.000000 euroleague_api-0.0.6/src/euroleague_api/player_stats.py
+-rw-rw-rw-   0        0        0     2470 2023-07-06 12:25:08.000000 euroleague_api-0.0.6/src/euroleague_api/shot_data.py
+-rw-rw-rw-   0        0        0     1323 2023-07-06 12:25:08.000000 euroleague_api-0.0.6/src/euroleague_api/standings.py
+-rw-rw-rw-   0        0        0     3804 2023-07-06 12:25:08.000000 euroleague_api-0.0.6/src/euroleague_api/team_stats.py
+-rw-rw-rw-   0        0        0    19311 2023-07-06 13:53:12.000000 euroleague_api-0.0.6/src/euroleague_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 14:12:29.012091 euroleague_api-0.0.6/src/euroleague_api.egg-info/
+-rw-rw-rw-   0        0        0     2376 2023-07-06 14:12:28.000000 euroleague_api-0.0.6/src/euroleague_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-06 14:12:28.000000 euroleague_api-0.0.6/src/euroleague_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 14:12:28.000000 euroleague_api-0.0.6/src/euroleague_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-06 14:12:28.000000 euroleague_api-0.0.6/src/euroleague_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 14:12:28.000000 euroleague_api-0.0.6/src/euroleague_api.egg-info/top_level.txt
```

### Comparing `euroleague_api-0.0.5/LICENSE` & `euroleague_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.5/PKG-INFO` & `euroleague_api-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: euroleague_api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python wrapper of the Euroleague API
 Home-page: https://github.com/giasemidis/euroleague_api
-Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.5.tar.gz
+Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.6.tar.gz
 Author: Georgios Giasemidis
 Author-email: g.giasemidis@gmail.com
 Keywords: euroleague,api,basketball
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -47,14 +47,17 @@
 
 ### Shot data
 [shot_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/shot_data.html)
 
 ### Play-by-play data
 [play_by_play_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/play_by_play_data.html)
 
+### Boxscore data
+[boxscore_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/boxscore_data.html)
+
 ### Auxiliary functions
 [utils.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_ap/utils.html)
 
 ## TODO
 - Add more endpoints from various sources
 - Add Eurocup API support
 - Add tests
```

### Comparing `euroleague_api-0.0.5/README.md` & `euroleague_api-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 ### Shot data
 [shot_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/shot_data.html)
 
 ### Play-by-play data
 [play_by_play_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/play_by_play_data.html)
 
+### Boxscore data
+[boxscore_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/boxscore_data.html)
+
 ### Auxiliary functions
 [utils.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_ap/utils.html)
 
 ## TODO
 - Add more endpoints from various sources
 - Add Eurocup API support
 - Add tests
```

### Comparing `euroleague_api-0.0.5/setup.cfg` & `euroleague_api-0.0.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7572 6f6c 6561 6775 655f 6170   = euroleague_ap
 00000020: 690d 0a76 6572 7369 6f6e 203d 2030 2e30  i..version = 0.0
-00000030: 2e35 0d0a 6175 7468 6f72 203d 2047 656f  .5..author = Geo
+00000030: 2e36 0d0a 6175 7468 6f72 203d 2047 656f  .6..author = Geo
 00000040: 7267 696f 7320 4769 6173 656d 6964 6973  rgios Giasemidis
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2067 2e67 6961 7365 6d69 6469 7340 676d   g.giasemidis@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2050 7974 686f 6e20  tion = A Python 
 00000090: 7772 6170 7065 7220 6f66 2074 6865 2045  wrapper of the E
 000000a0: 7572 6f6c 6561 6775 6520 4150 490d 0a64  uroleague API..d
@@ -22,15 +22,15 @@
 00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000160: 2f67 6961 7365 6d69 6469 732f 6575 726f  /giasemidis/euro
 00000170: 6c65 6167 7565 5f61 7069 0d0a 646f 776e  league_api..down
 00000180: 6c6f 6164 5f75 726c 203d 2068 7474 7073  load_url = https
 00000190: 3a2f 2f67 6974 6875 622e 636f 6d2f 6769  ://github.com/gi
 000001a0: 6173 656d 6964 6973 2f65 7572 6f6c 6561  asemidis/eurolea
 000001b0: 6775 655f 6170 692f 6172 6368 6976 652f  gue_api/archive/
-000001c0: 7265 6673 2f74 6167 732f 7630 2e30 2e35  refs/tags/v0.0.5
+000001c0: 7265 6673 2f74 6167 732f 7630 2e30 2e36  refs/tags/v0.0.6
 000001d0: 2e74 6172 2e67 7a0d 0a0d 0a5b 6f70 7469  .tar.gz....[opti
 000001e0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
 000001f0: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
 00000200: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
 00000210: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 00000220: 3d20 3e3d 332e 360d 0a69 6e73 7461 6c6c  = >=3.6..install
 00000230: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
```

### Comparing `euroleague_api-0.0.5/src/euroleague_api/game_stats.py` & `euroleague_api-0.0.6/src/euroleague_api/game_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.5/src/euroleague_api/play_by_play_data.py` & `euroleague_api-0.0.6/src/euroleague_api/play_by_play_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     play_by_play_df['CODETEAM'] = play_by_play_df['CODETEAM'].str.strip()
     play_by_play_df['PLAYER_ID'] = play_by_play_df['PLAYER_ID'].str.strip()
     play_by_play_df.insert(0, 'Season', season)
     play_by_play_df.insert(1, 'Gamecode', gamecode)
     return play_by_play_df
 
 
-def get_hame_shot_data_single_season(season: int) -> pd.DataFrame:
+def get_game_shot_data_single_season(season: int) -> pd.DataFrame:
     """
     A function that gets the play-by-play data of *all* games in a single
     season
 
     Args:
 
         season (int): The start year of the season
```

### Comparing `euroleague_api-0.0.5/src/euroleague_api/player_stats.py` & `euroleague_api-0.0.6/src/euroleague_api/player_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.5/src/euroleague_api/shot_data.py` & `euroleague_api-0.0.6/src/euroleague_api/shot_data.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.5/src/euroleague_api/standings.py` & `euroleague_api-0.0.6/src/euroleague_api/standings.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.5/src/euroleague_api/team_stats.py` & `euroleague_api-0.0.6/src/euroleague_api/team_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.5/src/euroleague_api/utils.py` & `euroleague_api-0.0.6/src/euroleague_api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Callable, Optional, List
 import logging
 import requests
+from json.decoder import JSONDecodeError
 import pandas as pd
 
 logging.basicConfig(encoding='utf-8', level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 BASE_URL = "https://api-live.euroleague.net"
@@ -149,14 +150,15 @@
             logger.debug(
                 "No more available game data for this season, break and exit"
             )
             break
 
     if data_list:
         data_df = pd.concat(data_list, axis=0)
+        data_df.reset_index(drop=True, inplace=True)
     else:
         data_df = pd.DataFrame([])
     return data_df
 
 
 def get_range_seasons_data(
     start_season: int,
@@ -183,14 +185,15 @@
         pd.DataFrame: A dataframe with the game data
     """
     data = []
     for season in range(start_season, end_season + 1):
         data_df = get_season_data_from_game_data(season, fun)
         data.append(data_df)
     df = pd.concat(data)
+    df.reset_index(drop=True, inplace=True)
     return df
 
 
 def get_player_stats(
     endpoint: str,
     params={},
     phase_type_code: Optional[str] = None,
@@ -618,7 +621,50 @@
 
     if var not in available_vals:
         raise ValueError(
             f"{descripitve_var}, {var}, is not applicable. "
             f"Available values: {available_vals}"
         )
     return
+
+
+def get_boxscore_data(
+    season: int,
+    gamecode: int,
+    boxscore_type: str = "ByQuarter"
+) -> List[dict]:
+    """A helper function that gets the boxscore data of a particular data.
+
+    Args:
+        season (int): The start year of the season
+        gamecode (int): The game-code of the game of interest.
+            It can be found on Euroleague's website.
+        boxscore_type (str, optional): The type of quarter boxscore data.
+            Available values:
+            - Stats
+            - ByQuarter
+            - EndOfQuarter
+            Defaults to "ByQuarter".
+
+    Raises:
+        ValueError: If boxscore_type value is not valid.
+
+    Returns:
+        List[dict]: A list of dictionaries with the data.
+    """
+    url = "https://live.euroleague.net/api/Boxscore"
+    params = {
+        "gamecode": gamecode,
+        "seasoncode": f"E{season}"
+    }
+    r = get_requests(url, params=params)
+
+    try:
+        data = r.json()
+    except JSONDecodeError:
+        raise ValueError(f"Game code, {gamecode}, did not return any data.")
+    boxscore_types = ["Stats", "ByQuarter", "EndOfQuarter"]
+
+    if boxscore_type not in boxscore_types:
+        raise_error(boxscore_type, "Boxscore", boxscore_types, False)
+
+    return data[boxscore_type]
```

### Comparing `euroleague_api-0.0.5/src/euroleague_api.egg-info/PKG-INFO` & `euroleague_api-0.0.6/src/euroleague_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: euroleague-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python wrapper of the Euroleague API
 Home-page: https://github.com/giasemidis/euroleague_api
-Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.5.tar.gz
+Download-URL: https://github.com/giasemidis/euroleague_api/archive/refs/tags/v0.0.6.tar.gz
 Author: Georgios Giasemidis
 Author-email: g.giasemidis@gmail.com
 Keywords: euroleague,api,basketball
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -47,14 +47,17 @@
 
 ### Shot data
 [shot_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/shot_data.html)
 
 ### Play-by-play data
 [play_by_play_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/play_by_play_data.html)
 
+### Boxscore data
+[boxscore_data.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_api/boxscore_data.html)
+
 ### Auxiliary functions
 [utils.py](https://htmlpreview.github.io/?https://github.com/giasemidis/euroleague_api/blob/main/site/euroleague_ap/utils.html)
 
 ## TODO
 - Add more endpoints from various sources
 - Add Eurocup API support
 - Add tests
```

### Comparing `euroleague_api-0.0.5/src/euroleague_api.egg-info/SOURCES.txt` & `euroleague_api-0.0.6/src/euroleague_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/euroleague_api/__init__.py
+src/euroleague_api/boxscore_data.py
 src/euroleague_api/game_stats.py
 src/euroleague_api/play_by_play_data.py
 src/euroleague_api/player_stats.py
 src/euroleague_api/shot_data.py
 src/euroleague_api/standings.py
 src/euroleague_api/team_stats.py
 src/euroleague_api/utils.py
```

