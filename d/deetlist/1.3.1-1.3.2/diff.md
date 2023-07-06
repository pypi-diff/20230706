# Comparing `tmp/deetlist-1.3.1.tar.gz` & `tmp/deetlist-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deetlist-1.3.1.tar", last modified: Thu Jul  6 13:00:10 2023, max compression
+gzip compressed data, was "deetlist-1.3.2.tar", last modified: Thu Jul  6 13:01:55 2023, max compression
```

## Comparing `deetlist-1.3.1.tar` & `deetlist-1.3.2.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:10.119289 deetlist-1.3.1/
--rw-rw-rw-   0        0        0     1039 2023-07-06 13:00:10.118291 deetlist-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-04-09 17:25:37.000000 deetlist-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.771294 deetlist-1.3.1/deetlist/
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.877291 deetlist-1.3.1/deetlist/crawler/
--rw-rw-rw-   0        0        0     1296 2023-04-17 19:05:56.000000 deetlist-1.3.1/deetlist/crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.882290 deetlist-1.3.1/deetlist/fetcher/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:27:44.000000 deetlist-1.3.1/deetlist/fetcher/__init__.py
--rw-rw-rw-   0        0        0     1280 2023-04-09 15:33:04.000000 deetlist-1.3.1/deetlist/fetcher/base.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.891295 deetlist-1.3.1/deetlist/fetcher/dragons/
--rw-rw-rw-   0        0        0      316 2023-04-17 18:28:50.000000 deetlist-1.3.1/deetlist/fetcher/dragons/__init__.py
--rw-rw-rw-   0        0        0      241 2023-04-09 15:32:01.000000 deetlist-1.3.1/deetlist/fetcher/dragons/all.py
--rw-rw-rw-   0        0        0      241 2023-04-09 15:32:10.000000 deetlist-1.3.1/deetlist/fetcher/dragons/new.py
--rw-rw-rw-   0        0        0     1696 2023-04-17 18:28:12.000000 deetlist-1.3.1/deetlist/fetcher/dragons/page.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.917292 deetlist-1.3.1/deetlist/fetcher/islands/
--rw-rw-rw-   0        0        0      538 2023-04-09 15:32:33.000000 deetlist-1.3.1/deetlist/fetcher/islands/__init__.py
--rw-rw-rw-   0        0        0      240 2023-04-09 15:32:36.000000 deetlist-1.3.1/deetlist/fetcher/islands/fog_islands.py
--rw-rw-rw-   0        0        0      243 2023-04-09 15:32:41.000000 deetlist-1.3.1/deetlist/fetcher/islands/grid_islands.py
--rw-rw-rw-   0        0        0      243 2023-04-09 15:32:45.000000 deetlist-1.3.1/deetlist/fetcher/islands/heroic_races.py
--rw-rw-rw-   0        0        0      243 2023-04-09 15:32:48.000000 deetlist-1.3.1/deetlist/fetcher/islands/maze_islands.py
--rw-rw-rw-   0        0        0      249 2023-04-09 15:32:50.000000 deetlist-1.3.1/deetlist/fetcher/islands/puzzle_islands.py
--rw-rw-rw-   0        0        0      249 2023-04-09 15:32:54.000000 deetlist-1.3.1/deetlist/fetcher/islands/runner_islands.py
--rw-rw-rw-   0        0        0      246 2023-04-09 15:32:58.000000 deetlist-1.3.1/deetlist/fetcher/islands/tower_islands.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.919293 deetlist-1.3.1/deetlist/parser/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:27:54.000000 deetlist-1.3.1/deetlist/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.936292 deetlist-1.3.1/deetlist/parser/dragons/
--rw-rw-rw-   0        0        0      198 2023-04-09 15:31:13.000000 deetlist-1.3.1/deetlist/parser/dragons/__init__.py
--rw-rw-rw-   0        0        0     1617 2023-04-09 15:31:18.000000 deetlist-1.3.1/deetlist/parser/dragons/all.py
--rw-rw-rw-   0        0        0     1924 2023-04-09 15:31:22.000000 deetlist-1.3.1/deetlist/parser/dragons/new.py
--rw-rw-rw-   0        0        0     8236 2023-05-14 21:00:34.000000 deetlist-1.3.1/deetlist/parser/dragons/page.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.950293 deetlist-1.3.1/deetlist/parser/islands/
--rw-rw-rw-   0        0        0      524 2023-04-09 15:29:55.000000 deetlist-1.3.1/deetlist/parser/islands/__init__.py
--rw-rw-rw-   0        0        0     2850 2023-04-09 15:29:28.000000 deetlist-1.3.1/deetlist/parser/islands/fog_islands.py
--rw-rw-rw-   0        0        0     2849 2023-04-09 15:29:23.000000 deetlist-1.3.1/deetlist/parser/islands/grid_islands.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.963290 deetlist-1.3.1/deetlist/parser/islands/heroic_races/
--rw-rw-rw-   0        0        0     2850 2023-04-09 15:30:48.000000 deetlist-1.3.1/deetlist/parser/islands/heroic_races/__init__.py
--rw-rw-rw-   0        0        0      900 2023-04-09 15:30:51.000000 deetlist-1.3.1/deetlist/parser/islands/heroic_races/lap.py
--rw-rw-rw-   0        0        0     1460 2023-04-09 15:30:54.000000 deetlist-1.3.1/deetlist/parser/islands/heroic_races/mission.py
--rw-rw-rw-   0        0        0      939 2023-04-09 15:31:01.000000 deetlist-1.3.1/deetlist/parser/islands/heroic_races/node.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.975293 deetlist-1.3.1/deetlist/parser/islands/maze_islands/
--rw-rw-rw-   0        0        0     1488 2023-04-09 15:30:44.000000 deetlist-1.3.1/deetlist/parser/islands/maze_islands/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-04-09 15:30:40.000000 deetlist-1.3.1/deetlist/parser/islands/maze_islands/dragon.py
--rw-rw-rw-   0        0        0     1379 2023-04-09 15:30:35.000000 deetlist-1.3.1/deetlist/parser/islands/maze_islands/node.py
--rw-rw-rw-   0        0        0     1119 2023-04-09 15:30:31.000000 deetlist-1.3.1/deetlist/parser/islands/maze_islands/path.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.981290 deetlist-1.3.1/deetlist/parser/islands/puzzle_islands/
--rw-rw-rw-   0        0        0     2908 2023-04-09 15:30:23.000000 deetlist-1.3.1/deetlist/parser/islands/puzzle_islands/__init__.py
--rw-rw-rw-   0        0        0      883 2023-04-09 15:30:19.000000 deetlist-1.3.1/deetlist/parser/islands/puzzle_islands/mission.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:10.006288 deetlist-1.3.1/deetlist/parser/islands/runner_islands/
--rw-rw-rw-   0        0        0     2961 2023-04-09 15:30:11.000000 deetlist-1.3.1/deetlist/parser/islands/runner_islands/__init__.py
--rw-rw-rw-   0        0        0     1362 2023-04-09 15:30:01.000000 deetlist-1.3.1/deetlist/parser/islands/runner_islands/mission.py
--rw-rw-rw-   0        0        0      682 2023-05-14 17:33:49.000000 deetlist-1.3.1/deetlist/parser/islands/runner_islands/mission_set.py
--rw-rw-rw-   0        0        0     2856 2023-04-09 15:29:20.000000 deetlist-1.3.1/deetlist/parser/islands/tower_islands.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:10.030290 deetlist-1.3.1/deetlist/scraper/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:28:14.000000 deetlist-1.3.1/deetlist/scraper/__init__.py
--rw-rw-rw-   0        0        0      293 2023-04-09 15:18:43.000000 deetlist-1.3.1/deetlist/scraper/base.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:10.040291 deetlist-1.3.1/deetlist/scraper/dragons/
--rw-rw-rw-   0        0        0      550 2023-04-17 19:03:32.000000 deetlist-1.3.1/deetlist/scraper/dragons/__init__.py
--rw-rw-rw-   0        0        0      517 2023-04-17 18:33:53.000000 deetlist-1.3.1/deetlist/scraper/dragons/all.py
--rw-rw-rw-   0        0        0      517 2023-04-17 18:33:55.000000 deetlist-1.3.1/deetlist/scraper/dragons/new.py
--rw-rw-rw-   0        0        0     1856 2023-04-17 18:34:02.000000 deetlist-1.3.1/deetlist/scraper/dragons/page.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:10.067288 deetlist-1.3.1/deetlist/scraper/islands/
--rw-rw-rw-   0        0        0      890 2023-04-09 15:21:26.000000 deetlist-1.3.1/deetlist/scraper/islands/__init__.py
--rw-rw-rw-   0        0        0      455 2023-04-09 15:15:05.000000 deetlist-1.3.1/deetlist/scraper/islands/fog_islands.py
--rw-rw-rw-   0        0        0      465 2023-04-09 15:15:41.000000 deetlist-1.3.1/deetlist/scraper/islands/grid_islands.py
--rw-rw-rw-   0        0        0      465 2023-04-09 15:16:16.000000 deetlist-1.3.1/deetlist/scraper/islands/heroic_races.py
--rw-rw-rw-   0        0        0      465 2023-04-09 15:16:55.000000 deetlist-1.3.1/deetlist/scraper/islands/maze_islands.py
--rw-rw-rw-   0        0        0      485 2023-04-09 15:17:21.000000 deetlist-1.3.1/deetlist/scraper/islands/puzzle_islands.py
--rw-rw-rw-   0        0        0      485 2023-04-09 15:18:00.000000 deetlist-1.3.1/deetlist/scraper/islands/runner_islands.py
--rw-rw-rw-   0        0        0      475 2023-04-09 15:18:37.000000 deetlist-1.3.1/deetlist/scraper/islands/tower_islands.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:10.072294 deetlist-1.3.1/deetlist/utils/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:28:25.000000 deetlist-1.3.1/deetlist/utils/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-05-14 20:25:23.000000 deetlist-1.3.1/deetlist/utils/time_parser.py
-drwxrwxrwx   0        0        0        0 2023-07-06 13:00:09.875290 deetlist-1.3.1/deetlist.egg-info/
--rw-rw-rw-   0        0        0     1039 2023-07-06 13:00:09.000000 deetlist-1.3.1/deetlist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4266 2023-07-06 13:00:09.000000 deetlist-1.3.1/deetlist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 13:00:09.000000 deetlist-1.3.1/deetlist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-06 13:00:09.000000 deetlist-1.3.1/deetlist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 13:00:10.119289 deetlist-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-07-06 13:00:02.000000 deetlist-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.300272 deetlist-1.3.2/
+-rw-rw-rw-   0        0        0     1039 2023-07-06 13:01:55.299276 deetlist-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-04-09 17:25:37.000000 deetlist-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.071276 deetlist-1.3.2/deetlist/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:59:56.000000 deetlist-1.3.2/deetlist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.111276 deetlist-1.3.2/deetlist/crawler/
+-rw-rw-rw-   0        0        0     1296 2023-04-17 19:05:56.000000 deetlist-1.3.2/deetlist/crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.126273 deetlist-1.3.2/deetlist/fetcher/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:27:44.000000 deetlist-1.3.2/deetlist/fetcher/__init__.py
+-rw-rw-rw-   0        0        0     1280 2023-04-09 15:33:04.000000 deetlist-1.3.2/deetlist/fetcher/base.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.142277 deetlist-1.3.2/deetlist/fetcher/dragons/
+-rw-rw-rw-   0        0        0      316 2023-04-17 18:28:50.000000 deetlist-1.3.2/deetlist/fetcher/dragons/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-04-09 15:32:01.000000 deetlist-1.3.2/deetlist/fetcher/dragons/all.py
+-rw-rw-rw-   0        0        0      241 2023-04-09 15:32:10.000000 deetlist-1.3.2/deetlist/fetcher/dragons/new.py
+-rw-rw-rw-   0        0        0     1696 2023-04-17 18:28:12.000000 deetlist-1.3.2/deetlist/fetcher/dragons/page.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.172276 deetlist-1.3.2/deetlist/fetcher/islands/
+-rw-rw-rw-   0        0        0      538 2023-04-09 15:32:33.000000 deetlist-1.3.2/deetlist/fetcher/islands/__init__.py
+-rw-rw-rw-   0        0        0      240 2023-04-09 15:32:36.000000 deetlist-1.3.2/deetlist/fetcher/islands/fog_islands.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 15:32:41.000000 deetlist-1.3.2/deetlist/fetcher/islands/grid_islands.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 15:32:45.000000 deetlist-1.3.2/deetlist/fetcher/islands/heroic_races.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 15:32:48.000000 deetlist-1.3.2/deetlist/fetcher/islands/maze_islands.py
+-rw-rw-rw-   0        0        0      249 2023-04-09 15:32:50.000000 deetlist-1.3.2/deetlist/fetcher/islands/puzzle_islands.py
+-rw-rw-rw-   0        0        0      249 2023-04-09 15:32:54.000000 deetlist-1.3.2/deetlist/fetcher/islands/runner_islands.py
+-rw-rw-rw-   0        0        0      246 2023-04-09 15:32:58.000000 deetlist-1.3.2/deetlist/fetcher/islands/tower_islands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.175276 deetlist-1.3.2/deetlist/parser/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:27:54.000000 deetlist-1.3.2/deetlist/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.187274 deetlist-1.3.2/deetlist/parser/dragons/
+-rw-rw-rw-   0        0        0      198 2023-04-09 15:31:13.000000 deetlist-1.3.2/deetlist/parser/dragons/__init__.py
+-rw-rw-rw-   0        0        0     1617 2023-04-09 15:31:18.000000 deetlist-1.3.2/deetlist/parser/dragons/all.py
+-rw-rw-rw-   0        0        0     1924 2023-04-09 15:31:22.000000 deetlist-1.3.2/deetlist/parser/dragons/new.py
+-rw-rw-rw-   0        0        0     8236 2023-05-14 21:00:34.000000 deetlist-1.3.2/deetlist/parser/dragons/page.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.201276 deetlist-1.3.2/deetlist/parser/islands/
+-rw-rw-rw-   0        0        0      524 2023-04-09 15:29:55.000000 deetlist-1.3.2/deetlist/parser/islands/__init__.py
+-rw-rw-rw-   0        0        0     2850 2023-04-09 15:29:28.000000 deetlist-1.3.2/deetlist/parser/islands/fog_islands.py
+-rw-rw-rw-   0        0        0     2849 2023-04-09 15:29:23.000000 deetlist-1.3.2/deetlist/parser/islands/grid_islands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.214277 deetlist-1.3.2/deetlist/parser/islands/heroic_races/
+-rw-rw-rw-   0        0        0     2850 2023-04-09 15:30:48.000000 deetlist-1.3.2/deetlist/parser/islands/heroic_races/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-04-09 15:30:51.000000 deetlist-1.3.2/deetlist/parser/islands/heroic_races/lap.py
+-rw-rw-rw-   0        0        0     1460 2023-04-09 15:30:54.000000 deetlist-1.3.2/deetlist/parser/islands/heroic_races/mission.py
+-rw-rw-rw-   0        0        0      939 2023-04-09 15:31:01.000000 deetlist-1.3.2/deetlist/parser/islands/heroic_races/node.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.227276 deetlist-1.3.2/deetlist/parser/islands/maze_islands/
+-rw-rw-rw-   0        0        0     1488 2023-04-09 15:30:44.000000 deetlist-1.3.2/deetlist/parser/islands/maze_islands/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-04-09 15:30:40.000000 deetlist-1.3.2/deetlist/parser/islands/maze_islands/dragon.py
+-rw-rw-rw-   0        0        0     1379 2023-04-09 15:30:35.000000 deetlist-1.3.2/deetlist/parser/islands/maze_islands/node.py
+-rw-rw-rw-   0        0        0     1119 2023-04-09 15:30:31.000000 deetlist-1.3.2/deetlist/parser/islands/maze_islands/path.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.237280 deetlist-1.3.2/deetlist/parser/islands/puzzle_islands/
+-rw-rw-rw-   0        0        0     2908 2023-04-09 15:30:23.000000 deetlist-1.3.2/deetlist/parser/islands/puzzle_islands/__init__.py
+-rw-rw-rw-   0        0        0      883 2023-04-09 15:30:19.000000 deetlist-1.3.2/deetlist/parser/islands/puzzle_islands/mission.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.247274 deetlist-1.3.2/deetlist/parser/islands/runner_islands/
+-rw-rw-rw-   0        0        0     2961 2023-04-09 15:30:11.000000 deetlist-1.3.2/deetlist/parser/islands/runner_islands/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-04-09 15:30:01.000000 deetlist-1.3.2/deetlist/parser/islands/runner_islands/mission.py
+-rw-rw-rw-   0        0        0      682 2023-05-14 17:33:49.000000 deetlist-1.3.2/deetlist/parser/islands/runner_islands/mission_set.py
+-rw-rw-rw-   0        0        0     2856 2023-04-09 15:29:20.000000 deetlist-1.3.2/deetlist/parser/islands/tower_islands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.253278 deetlist-1.3.2/deetlist/scraper/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:28:14.000000 deetlist-1.3.2/deetlist/scraper/__init__.py
+-rw-rw-rw-   0        0        0      293 2023-04-09 15:18:43.000000 deetlist-1.3.2/deetlist/scraper/base.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.267275 deetlist-1.3.2/deetlist/scraper/dragons/
+-rw-rw-rw-   0        0        0      550 2023-04-17 19:03:32.000000 deetlist-1.3.2/deetlist/scraper/dragons/__init__.py
+-rw-rw-rw-   0        0        0      517 2023-04-17 18:33:53.000000 deetlist-1.3.2/deetlist/scraper/dragons/all.py
+-rw-rw-rw-   0        0        0      517 2023-04-17 18:33:55.000000 deetlist-1.3.2/deetlist/scraper/dragons/new.py
+-rw-rw-rw-   0        0        0     1856 2023-04-17 18:34:02.000000 deetlist-1.3.2/deetlist/scraper/dragons/page.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.290277 deetlist-1.3.2/deetlist/scraper/islands/
+-rw-rw-rw-   0        0        0      890 2023-04-09 15:21:26.000000 deetlist-1.3.2/deetlist/scraper/islands/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-04-09 15:15:05.000000 deetlist-1.3.2/deetlist/scraper/islands/fog_islands.py
+-rw-rw-rw-   0        0        0      465 2023-04-09 15:15:41.000000 deetlist-1.3.2/deetlist/scraper/islands/grid_islands.py
+-rw-rw-rw-   0        0        0      465 2023-04-09 15:16:16.000000 deetlist-1.3.2/deetlist/scraper/islands/heroic_races.py
+-rw-rw-rw-   0        0        0      465 2023-04-09 15:16:55.000000 deetlist-1.3.2/deetlist/scraper/islands/maze_islands.py
+-rw-rw-rw-   0        0        0      485 2023-04-09 15:17:21.000000 deetlist-1.3.2/deetlist/scraper/islands/puzzle_islands.py
+-rw-rw-rw-   0        0        0      485 2023-04-09 15:18:00.000000 deetlist-1.3.2/deetlist/scraper/islands/runner_islands.py
+-rw-rw-rw-   0        0        0      475 2023-04-09 15:18:37.000000 deetlist-1.3.2/deetlist/scraper/islands/tower_islands.py
+-rw-rw-rw-   0        0        0      941 2023-04-09 15:34:11.000000 deetlist-1.3.2/deetlist/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.297281 deetlist-1.3.2/deetlist/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:28:25.000000 deetlist-1.3.2/deetlist/utils/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-05-14 20:25:23.000000 deetlist-1.3.2/deetlist/utils/time_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:01:55.107276 deetlist-1.3.2/deetlist.egg-info/
+-rw-rw-rw-   0        0        0     1039 2023-07-06 13:01:54.000000 deetlist-1.3.2/deetlist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2248 2023-07-06 13:01:54.000000 deetlist-1.3.2/deetlist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:01:54.000000 deetlist-1.3.2/deetlist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 13:01:54.000000 deetlist-1.3.2/deetlist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:01:55.300272 deetlist-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-07-06 13:01:51.000000 deetlist-1.3.2/setup.py
```

### Comparing `deetlist-1.3.1/PKG-INFO` & `deetlist-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deetlist
-Version: 1.3.1
+Version: 1.3.2
 Summary: Fetcher/scraper of https://deetlist.com/dragoncity/
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
 Keywords: dragoncity dcutils tools
 Description-Content-Type: text/markdown
```

### Comparing `deetlist-1.3.1/README.md` & `deetlist-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/crawler/__init__.py` & `deetlist-1.3.2/deetlist/crawler/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/fetcher/base.py` & `deetlist-1.3.2/deetlist/fetcher/base.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/fetcher/dragons/page.py` & `deetlist-1.3.2/deetlist/fetcher/dragons/page.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/fetcher/islands/__init__.py` & `deetlist-1.3.2/deetlist/fetcher/islands/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/dragons/all.py` & `deetlist-1.3.2/deetlist/parser/dragons/all.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/dragons/new.py` & `deetlist-1.3.2/deetlist/parser/dragons/new.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/dragons/page.py` & `deetlist-1.3.2/deetlist/parser/dragons/page.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/__init__.py` & `deetlist-1.3.2/deetlist/parser/islands/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/fog_islands.py` & `deetlist-1.3.2/deetlist/parser/islands/fog_islands.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/grid_islands.py` & `deetlist-1.3.2/deetlist/parser/islands/grid_islands.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/heroic_races/__init__.py` & `deetlist-1.3.2/deetlist/parser/islands/heroic_races/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/heroic_races/lap.py` & `deetlist-1.3.2/deetlist/parser/islands/heroic_races/lap.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/heroic_races/mission.py` & `deetlist-1.3.2/deetlist/parser/islands/heroic_races/mission.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/heroic_races/node.py` & `deetlist-1.3.2/deetlist/parser/islands/heroic_races/node.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/maze_islands/__init__.py` & `deetlist-1.3.2/deetlist/parser/islands/maze_islands/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/maze_islands/dragon.py` & `deetlist-1.3.2/deetlist/parser/islands/maze_islands/dragon.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/maze_islands/node.py` & `deetlist-1.3.2/deetlist/parser/islands/maze_islands/node.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/maze_islands/path.py` & `deetlist-1.3.2/deetlist/parser/islands/maze_islands/path.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/puzzle_islands/__init__.py` & `deetlist-1.3.2/deetlist/parser/islands/puzzle_islands/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/puzzle_islands/mission.py` & `deetlist-1.3.2/deetlist/parser/islands/puzzle_islands/mission.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/runner_islands/__init__.py` & `deetlist-1.3.2/deetlist/parser/islands/runner_islands/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/runner_islands/mission.py` & `deetlist-1.3.2/deetlist/parser/islands/runner_islands/mission.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/runner_islands/mission_set.py` & `deetlist-1.3.2/deetlist/parser/islands/runner_islands/mission_set.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/parser/islands/tower_islands.py` & `deetlist-1.3.2/deetlist/parser/islands/tower_islands.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/scraper/dragons/__init__.py` & `deetlist-1.3.2/deetlist/scraper/dragons/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/scraper/dragons/all.py` & `deetlist-1.3.2/deetlist/scraper/dragons/all.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/scraper/dragons/new.py` & `deetlist-1.3.2/deetlist/scraper/dragons/new.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/scraper/dragons/page.py` & `deetlist-1.3.2/deetlist/scraper/dragons/page.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/scraper/islands/__init__.py` & `deetlist-1.3.2/deetlist/scraper/islands/__init__.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist/utils/time_parser.py` & `deetlist-1.3.2/deetlist/utils/time_parser.py`

 * *Files identical despite different names*

### Comparing `deetlist-1.3.1/deetlist.egg-info/PKG-INFO` & `deetlist-1.3.2/deetlist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deetlist
-Version: 1.3.1
+Version: 1.3.2
 Summary: Fetcher/scraper of https://deetlist.com/dragoncity/
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
 Keywords: dragoncity dcutils tools
 Description-Content-Type: text/markdown
```

### Comparing `deetlist-1.3.1/deetlist.egg-info/SOURCES.txt` & `deetlist-1.3.2/deetlist.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,22 @@
 README.md
 setup.py
+deetlist/__init__.py
+deetlist/settings.py
 deetlist.egg-info/PKG-INFO
 deetlist.egg-info/SOURCES.txt
 deetlist.egg-info/dependency_links.txt
 deetlist.egg-info/top_level.txt
 deetlist/crawler/__init__.py
 deetlist/fetcher/__init__.py
 deetlist/fetcher/base.py
 deetlist/fetcher/dragons/__init__.py
 deetlist/fetcher/dragons/all.py
 deetlist/fetcher/dragons/new.py
 deetlist/fetcher/dragons/page.py
-deetlist/fetcher/islands/__init__.py
-deetlist/fetcher/islands/fog_islands.py
-deetlist/fetcher/islands/grid_islands.py
-deetlist/fetcher/islands/heroic_races.py
-deetlist/fetcher/islands/maze_islands.py
-deetlist/fetcher/islands/puzzle_islands.py
-deetlist/fetcher/islands/runner_islands.py
-deetlist/fetcher/islands/tower_islands.py
-deetlist/parser/__init__.py
-deetlist/parser/dragons/__init__.py
-deetlist/parser/dragons/all.py
-deetlist/parser/dragons/new.py
-deetlist/parser/dragons/page.py
-deetlist/parser/islands/__init__.py
-deetlist/parser/islands/fog_islands.py
-deetlist/parser/islands/grid_islands.py
-deetlist/parser/islands/tower_islands.py
-deetlist/parser/islands/heroic_races/__init__.py
-deetlist/parser/islands/heroic_races/lap.py
-deetlist/parser/islands/heroic_races/mission.py
-deetlist/parser/islands/heroic_races/node.py
-deetlist/parser/islands/maze_islands/__init__.py
-deetlist/parser/islands/maze_islands/dragon.py
-deetlist/parser/islands/maze_islands/node.py
-deetlist/parser/islands/maze_islands/path.py
-deetlist/parser/islands/puzzle_islands/__init__.py
-deetlist/parser/islands/puzzle_islands/mission.py
-deetlist/parser/islands/runner_islands/__init__.py
-deetlist/parser/islands/runner_islands/mission.py
-deetlist/parser/islands/runner_islands/mission_set.py
-deetlist/scraper/__init__.py
-deetlist/scraper/base.py
-deetlist/scraper/dragons/__init__.py
-deetlist/scraper/dragons/all.py
-deetlist/scraper/dragons/new.py
-deetlist/scraper/dragons/page.py
-deetlist/scraper/islands/__init__.py
-deetlist/scraper/islands/fog_islands.py
-deetlist/scraper/islands/grid_islands.py
-deetlist/scraper/islands/heroic_races.py
-deetlist/scraper/islands/maze_islands.py
-deetlist/scraper/islands/puzzle_islands.py
-deetlist/scraper/islands/runner_islands.py
-deetlist/scraper/islands/tower_islands.py
-deetlist/utils/__init__.py
-deetlist/utils/time_parser.py
-deetlist/crawler/__init__.py
-deetlist/fetcher/__init__.py
-deetlist/fetcher/base.py
-deetlist/fetcher/dragons/__init__.py
-deetlist/fetcher/dragons/all.py
-deetlist/fetcher/dragons/new.py
-deetlist/fetcher/dragons/page.py
 deetlist/fetcher/islands/__init__.py
 deetlist/fetcher/islands/fog_islands.py
 deetlist/fetcher/islands/grid_islands.py
 deetlist/fetcher/islands/heroic_races.py
 deetlist/fetcher/islands/maze_islands.py
 deetlist/fetcher/islands/puzzle_islands.py
 deetlist/fetcher/islands/runner_islands.py
```

### Comparing `deetlist-1.3.1/setup.py` & `deetlist-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name="deetlist",
-    version="1.3.1",
+    version="1.3.2",
     license="MIT License",
     author="Marcuth",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author_email="marcuth2006@gmail.com",
     keywords="dragoncity dcutils tools",
     description=f"Fetcher/scraper of https://deetlist.com/dragoncity/",
-    packages=[ "deetlist/" + x for x in find_packages("deetlist") ]
+    packages=[ "deetlist/" + x for x in find_packages("deetlist") ].append("settings")
 )
```

