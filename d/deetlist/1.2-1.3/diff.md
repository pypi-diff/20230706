# Comparing `tmp/deetlist-1.2.tar.gz` & `tmp/deetlist-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deetlist-1.2.tar", last modified: Mon Apr 17 15:45:16 2023, max compression
+gzip compressed data, was "deetlist-1.3.tar", last modified: Thu Jul  6 12:28:30 2023, max compression
```

## Comparing `deetlist-1.2.tar` & `deetlist-1.3.tar`

### file list

```diff
@@ -1,11 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:45:16.546502 deetlist-1.2/
--rw-rw-rw-   0        0        0     1037 2023-04-17 15:45:16.543497 deetlist-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-04-09 17:25:37.000000 deetlist-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 15:45:16.541494 deetlist-1.2/deetlist.egg-info/
--rw-rw-rw-   0        0        0     1037 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      279 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:45:16.546502 deetlist-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-04-17 15:45:15.000000 deetlist-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:30.004949 deetlist-1.3/
+-rw-rw-rw-   0        0        0     1037 2023-07-06 12:28:30.002948 deetlist-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-04-09 17:25:37.000000 deetlist-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.307952 deetlist-1.3/deetlist/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.357950 deetlist-1.3/deetlist/crawler/
+-rw-rw-rw-   0        0        0     1296 2023-04-17 19:05:56.000000 deetlist-1.3/deetlist/crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.368949 deetlist-1.3/deetlist/fetcher/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:27:44.000000 deetlist-1.3/deetlist/fetcher/__init__.py
+-rw-rw-rw-   0        0        0     1280 2023-04-09 15:33:04.000000 deetlist-1.3/deetlist/fetcher/base.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.425950 deetlist-1.3/deetlist/fetcher/dragons/
+-rw-rw-rw-   0        0        0      316 2023-04-17 18:28:50.000000 deetlist-1.3/deetlist/fetcher/dragons/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-04-09 15:32:01.000000 deetlist-1.3/deetlist/fetcher/dragons/all.py
+-rw-rw-rw-   0        0        0      241 2023-04-09 15:32:10.000000 deetlist-1.3/deetlist/fetcher/dragons/new.py
+-rw-rw-rw-   0        0        0     1696 2023-04-17 18:28:12.000000 deetlist-1.3/deetlist/fetcher/dragons/page.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.549954 deetlist-1.3/deetlist/fetcher/islands/
+-rw-rw-rw-   0        0        0      538 2023-04-09 15:32:33.000000 deetlist-1.3/deetlist/fetcher/islands/__init__.py
+-rw-rw-rw-   0        0        0      240 2023-04-09 15:32:36.000000 deetlist-1.3/deetlist/fetcher/islands/fog_islands.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 15:32:41.000000 deetlist-1.3/deetlist/fetcher/islands/grid_islands.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 15:32:45.000000 deetlist-1.3/deetlist/fetcher/islands/heroic_races.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 15:32:48.000000 deetlist-1.3/deetlist/fetcher/islands/maze_islands.py
+-rw-rw-rw-   0        0        0      249 2023-04-09 15:32:50.000000 deetlist-1.3/deetlist/fetcher/islands/puzzle_islands.py
+-rw-rw-rw-   0        0        0      249 2023-04-09 15:32:54.000000 deetlist-1.3/deetlist/fetcher/islands/runner_islands.py
+-rw-rw-rw-   0        0        0      246 2023-04-09 15:32:58.000000 deetlist-1.3/deetlist/fetcher/islands/tower_islands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.552949 deetlist-1.3/deetlist/parser/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:27:54.000000 deetlist-1.3/deetlist/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.593950 deetlist-1.3/deetlist/parser/dragons/
+-rw-rw-rw-   0        0        0      198 2023-04-09 15:31:13.000000 deetlist-1.3/deetlist/parser/dragons/__init__.py
+-rw-rw-rw-   0        0        0     1617 2023-04-09 15:31:18.000000 deetlist-1.3/deetlist/parser/dragons/all.py
+-rw-rw-rw-   0        0        0     1924 2023-04-09 15:31:22.000000 deetlist-1.3/deetlist/parser/dragons/new.py
+-rw-rw-rw-   0        0        0     8236 2023-05-14 21:00:34.000000 deetlist-1.3/deetlist/parser/dragons/page.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.644950 deetlist-1.3/deetlist/parser/islands/
+-rw-rw-rw-   0        0        0      524 2023-04-09 15:29:55.000000 deetlist-1.3/deetlist/parser/islands/__init__.py
+-rw-rw-rw-   0        0        0     2850 2023-04-09 15:29:28.000000 deetlist-1.3/deetlist/parser/islands/fog_islands.py
+-rw-rw-rw-   0        0        0     2849 2023-04-09 15:29:23.000000 deetlist-1.3/deetlist/parser/islands/grid_islands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.695956 deetlist-1.3/deetlist/parser/islands/heroic_races/
+-rw-rw-rw-   0        0        0     2850 2023-04-09 15:30:48.000000 deetlist-1.3/deetlist/parser/islands/heroic_races/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-04-09 15:30:51.000000 deetlist-1.3/deetlist/parser/islands/heroic_races/lap.py
+-rw-rw-rw-   0        0        0     1460 2023-04-09 15:30:54.000000 deetlist-1.3/deetlist/parser/islands/heroic_races/mission.py
+-rw-rw-rw-   0        0        0      939 2023-04-09 15:31:01.000000 deetlist-1.3/deetlist/parser/islands/heroic_races/node.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.749947 deetlist-1.3/deetlist/parser/islands/maze_islands/
+-rw-rw-rw-   0        0        0     1488 2023-04-09 15:30:44.000000 deetlist-1.3/deetlist/parser/islands/maze_islands/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-04-09 15:30:40.000000 deetlist-1.3/deetlist/parser/islands/maze_islands/dragon.py
+-rw-rw-rw-   0        0        0     1379 2023-04-09 15:30:35.000000 deetlist-1.3/deetlist/parser/islands/maze_islands/node.py
+-rw-rw-rw-   0        0        0     1119 2023-04-09 15:30:31.000000 deetlist-1.3/deetlist/parser/islands/maze_islands/path.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.777953 deetlist-1.3/deetlist/parser/islands/puzzle_islands/
+-rw-rw-rw-   0        0        0     2908 2023-04-09 15:30:23.000000 deetlist-1.3/deetlist/parser/islands/puzzle_islands/__init__.py
+-rw-rw-rw-   0        0        0      883 2023-04-09 15:30:19.000000 deetlist-1.3/deetlist/parser/islands/puzzle_islands/mission.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.817953 deetlist-1.3/deetlist/parser/islands/runner_islands/
+-rw-rw-rw-   0        0        0     2961 2023-04-09 15:30:11.000000 deetlist-1.3/deetlist/parser/islands/runner_islands/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-04-09 15:30:01.000000 deetlist-1.3/deetlist/parser/islands/runner_islands/mission.py
+-rw-rw-rw-   0        0        0      682 2023-05-14 17:33:49.000000 deetlist-1.3/deetlist/parser/islands/runner_islands/mission_set.py
+-rw-rw-rw-   0        0        0     2856 2023-04-09 15:29:20.000000 deetlist-1.3/deetlist/parser/islands/tower_islands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.830951 deetlist-1.3/deetlist/scraper/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:28:14.000000 deetlist-1.3/deetlist/scraper/__init__.py
+-rw-rw-rw-   0        0        0      293 2023-04-09 15:18:43.000000 deetlist-1.3/deetlist/scraper/base.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.885952 deetlist-1.3/deetlist/scraper/dragons/
+-rw-rw-rw-   0        0        0      550 2023-04-17 19:03:32.000000 deetlist-1.3/deetlist/scraper/dragons/__init__.py
+-rw-rw-rw-   0        0        0      517 2023-04-17 18:33:53.000000 deetlist-1.3/deetlist/scraper/dragons/all.py
+-rw-rw-rw-   0        0        0      517 2023-04-17 18:33:55.000000 deetlist-1.3/deetlist/scraper/dragons/new.py
+-rw-rw-rw-   0        0        0     1856 2023-04-17 18:34:02.000000 deetlist-1.3/deetlist/scraper/dragons/page.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.989949 deetlist-1.3/deetlist/scraper/islands/
+-rw-rw-rw-   0        0        0      890 2023-04-09 15:21:26.000000 deetlist-1.3/deetlist/scraper/islands/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-04-09 15:15:05.000000 deetlist-1.3/deetlist/scraper/islands/fog_islands.py
+-rw-rw-rw-   0        0        0      465 2023-04-09 15:15:41.000000 deetlist-1.3/deetlist/scraper/islands/grid_islands.py
+-rw-rw-rw-   0        0        0      465 2023-04-09 15:16:16.000000 deetlist-1.3/deetlist/scraper/islands/heroic_races.py
+-rw-rw-rw-   0        0        0      465 2023-04-09 15:16:55.000000 deetlist-1.3/deetlist/scraper/islands/maze_islands.py
+-rw-rw-rw-   0        0        0      485 2023-04-09 15:17:21.000000 deetlist-1.3/deetlist/scraper/islands/puzzle_islands.py
+-rw-rw-rw-   0        0        0      485 2023-04-09 15:18:00.000000 deetlist-1.3/deetlist/scraper/islands/runner_islands.py
+-rw-rw-rw-   0        0        0      475 2023-04-09 15:18:37.000000 deetlist-1.3/deetlist/scraper/islands/tower_islands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.994951 deetlist-1.3/deetlist/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:28:25.000000 deetlist-1.3/deetlist/utils/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-05-14 20:25:23.000000 deetlist-1.3/deetlist/utils/time_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:28:29.353952 deetlist-1.3/deetlist.egg-info/
+-rw-rw-rw-   0        0        0     1037 2023-07-06 12:28:29.000000 deetlist-1.3/deetlist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2235 2023-07-06 12:28:29.000000 deetlist-1.3/deetlist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:28:29.000000 deetlist-1.3/deetlist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-06 12:28:29.000000 deetlist-1.3/deetlist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 12:28:30.004949 deetlist-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      540 2023-07-06 12:27:10.000000 deetlist-1.3/setup.py
```

### Comparing `deetlist-1.2/PKG-INFO` & `deetlist-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deetlist
-Version: 1.2
+Version: 1.3
 Summary: Fetcher/scraper of https://deetlist.com/dragoncity/
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
 Keywords: dragoncity dcutils tools
 Description-Content-Type: text/markdown
```

### Comparing `deetlist-1.2/README.md` & `deetlist-1.3/README.md`

 * *Files identical despite different names*

### Comparing `deetlist-1.2/deetlist.egg-info/PKG-INFO` & `deetlist-1.3/deetlist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deetlist
-Version: 1.2
+Version: 1.3
 Summary: Fetcher/scraper of https://deetlist.com/dragoncity/
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
 Keywords: dragoncity dcutils tools
 Description-Content-Type: text/markdown
```

