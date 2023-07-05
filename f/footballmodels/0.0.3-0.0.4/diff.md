# Comparing `tmp/footballmodels-0.0.3.tar.gz` & `tmp/footballmodels-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footballmodels-0.0.3.tar", last modified: Tue Jul  4 20:48:29 2023, max compression
+gzip compressed data, was "footballmodels-0.0.4.tar", last modified: Wed Jul  5 23:52:54 2023, max compression
```

## Comparing `footballmodels-0.0.3.tar` & `footballmodels-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.528609 footballmodels-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 20:48:21.000000 footballmodels-0.0.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 20:48:21.000000 footballmodels-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-04 20:48:29.528609 footballmodels-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 20:48:21.000000 footballmodels-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 20:48:21.000000 footballmodels-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 20:48:21.000000 footballmodels-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-04 20:48:29.528609 footballmodels-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-04 20:48:21.000000 footballmodels-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/footballmodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/footballmodels/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/definitions/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.528609 footballmodels-0.0.3/src/footballmodels/player_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/player_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/player_similarity/column_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/player_similarity/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.528609 footballmodels-0.0.3/src/footballmodels/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-04 20:48:21.000000 footballmodels-0.0.3/src/footballmodels/utils/possession_adjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:48:29.524609 footballmodels-0.0.3/src/footballmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 20:48:29.000000 footballmodels-0.0.3/src/footballmodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.698256 footballmodels-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.694256 footballmodels-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.694256 footballmodels-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-05 23:52:45.000000 footballmodels-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-05 23:52:45.000000 footballmodels-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 23:52:45.000000 footballmodels-0.0.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.694256 footballmodels-0.0.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-05 23:52:45.000000 footballmodels-0.0.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 23:52:45.000000 footballmodels-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 23:52:54.698256 footballmodels-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 23:52:45.000000 footballmodels-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 23:52:45.000000 footballmodels-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 23:52:45.000000 footballmodels-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-05 23:52:54.698256 footballmodels-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-05 23:52:45.000000 footballmodels-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.694256 footballmodels-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.694256 footballmodels-0.0.4/src/footballmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.698256 footballmodels-0.0.4/src/footballmodels/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/definitions/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.698256 footballmodels-0.0.4/src/footballmodels/player_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/player_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/player_similarity/column_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/player_similarity/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.698256 footballmodels-0.0.4/src/footballmodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-05 23:52:45.000000 footballmodels-0.0.4/src/footballmodels/utils/possession_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:52:54.698256 footballmodels-0.0.4/src/footballmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 23:52:54.000000 footballmodels-0.0.4/src/footballmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-05 23:52:54.000000 footballmodels-0.0.4/src/footballmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:52:54.000000 footballmodels-0.0.4/src/footballmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 23:52:54.000000 footballmodels-0.0.4/src/footballmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 23:52:54.000000 footballmodels-0.0.4/src/footballmodels.egg-info/top_level.txt
```

### Comparing `footballmodels-0.0.3/.gitignore` & `footballmodels-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/.vscode/settings.json` & `footballmodels-0.0.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/LICENSE` & `footballmodels-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/PKG-INFO` & `footballmodels-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.3
+Version: 0.0.4
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.3/setup.cfg` & `footballmodels-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/setup.py` & `footballmodels-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/src/footballmodels/definitions/templates.py` & `footballmodels-0.0.4/src/footballmodels/definitions/templates.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/src/footballmodels/player_similarity/column_defs.py` & `footballmodels-0.0.4/src/footballmodels/player_similarity/column_defs.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/src/footballmodels/player_similarity/models.py` & `footballmodels-0.0.4/src/footballmodels/player_similarity/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from abc import ABC, abstractmethod
 from typing import List
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 import pandas as pd
 from footballmodels.definitions.templates import TemplateAttribute
 from footballmodels.utils.distance import (
-    cartesian_distance,
     weighted_cartesian_distance,
+    weighted_l1_distance
 )
+import numpy as np
 
 
 class SimilarityAlgorith(ABC):
     MINIMUM_MINUTES = 300
     def __init__(self, data: pd.DataFrame):
         self._data = data
         
@@ -56,17 +57,24 @@
 
 class TemplateSimilarityAlgorithm(SimilarityAlgorith):
     """
     Finds similar players based on features specified by
     positional tempate
     """
 
-    def __init__(self, data: pd.DataFrame, template: List[TemplateAttribute]):
+    def __init__(self, data: pd.DataFrame, template: List[TemplateAttribute], distance_metric:str='cartesian'):
         super().__init__(data)
         self._template = template
+        if distance_metric == 'cartesian':
+            self._distance = weighted_cartesian_distance
+        elif distance_metric == 'l1':
+            self._distance = weighted_l1_distance
+        else:
+            raise ValueError(f"Distance metric {distance_metric} not supported")
+
 
     def transform(self, orig_data:pd.DataFrame)->pd.DataFrame:
         data = pd.DataFrame(
             {
                 "player": orig_data["player"],
                 "squad": orig_data["squad"],
                 "season":orig_data["season"],
@@ -92,31 +100,32 @@
         player_data =data[
             (data["player"] == player)
             & (data["squad"] == squad)
             & (data["season"] == season)
             & (data["comp"] == comp)
         ]
         player_data = player_data.drop(["player", "squad", "season", "comp", "age", "gender",'minutes'], axis=1)
-        distances = cartesian_distance(
+        distances = self._distance(
             player_data.values,
             data[[attr.name for attr in self._template]].values,
+            np.ones(player_data.shape),
         )
         data["distance"] = MinMaxScaler().fit_transform(distances.reshape(-1, 1))
         return data
 
 class WeightedTemplateSimilarityAlgorithm(TemplateSimilarityAlgorithm):
     def _find(self, data:pd.DataFrame, player: str, squad: str, season: int, comp: str, n: int = 10):
         
         player_data = data[
             (data["player"] == player)
             & (data["squad"] == squad)
             & (data["season"] == season)
             & (data["comp"] == comp)
         ]
         player_data = player_data.drop(["player", "squad", "season", "comp", "age", "gender",'minutes'], axis=1)
-        distances = weighted_cartesian_distance(
+        distances = self._distance(
             player_data.values,
             data[[attr.name for attr in self._template]].values,
             player_data.values,
         )
         data["distance"] = MinMaxScaler().fit_transform(distances.reshape(-1, 1))
         return data
```

### Comparing `footballmodels-0.0.3/src/footballmodels/utils/distance.py` & `footballmodels-0.0.4/src/footballmodels/utils/distance.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,7 +22,20 @@
         all_points (np.ndarray): The set of points to calculate the distance to.
         weights (np.ndarray): The weights to apply to each dimension of the points.
 
     Returns:
         np.ndarray: The weighted cartesian distance between the point and all other points in the set.
     """
     return np.linalg.norm((point - all_points) * weights, axis=1)
+
+def weighted_l1_distance(point: np.ndarray, all_points: np.ndarray, weights: np.ndarray) -> np.ndarray:
+    """Calculate the weighted L1 distance between a point and all other points in a set.
+
+    Args:
+        point (np.ndarray): The point to calculate the distance from.
+        all_points (np.ndarray): The set of points to calculate the distance to.
+        weights (np.ndarray): The weights to apply to each dimension of the points.
+
+    Returns:
+        np.ndarray: The weighted L1 distance between the point and all other points in the set.
+    """
+    return np.sum(np.abs((point - all_points) * weights), axis=1 )
```

### Comparing `footballmodels-0.0.3/src/footballmodels/utils/possession_adjustment.py` & `footballmodels-0.0.4/src/footballmodels/utils/possession_adjustment.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.3/src/footballmodels.egg-info/PKG-INFO` & `footballmodels-0.0.4/src/footballmodels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.3
+Version: 0.0.4
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.3/src/footballmodels.egg-info/SOURCES.txt` & `footballmodels-0.0.4/src/footballmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

