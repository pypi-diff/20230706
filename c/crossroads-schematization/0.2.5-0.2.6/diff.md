# Comparing `tmp/crossroads-schematization-0.2.5.tar.gz` & `tmp/crossroads-schematization-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.2.5.tar", last modified: Thu Jul  6 11:28:50 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.2.6.tar", last modified: Thu Jul  6 12:40:44 2023, max compression
```

## Comparing `crossroads-schematization-0.2.5.tar` & `crossroads-schematization-0.2.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 11:28:50.929334 crossroads-schematization-0.2.5/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.5/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-06 11:28:50.929334 crossroads-schematization-0.2.5/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.5/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 11:28:50.925334 crossroads-schematization-0.2.5/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-06 11:28:50.000000 crossroads-schematization-0.2.5/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     1188 2023-07-06 11:28:50.000000 crossroads-schematization-0.2.5/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-06 11:28:50.000000 crossroads-schematization-0.2.5/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-06 11:28:50.000000 crossroads-schematization-0.2.5/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-06 11:28:50.000000 crossroads-schematization-0.2.5/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 11:28:50.925334 crossroads-schematization-0.2.5/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-06 11:28:31.000000 crossroads-schematization-0.2.5/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     7911 2023-07-06 08:54:41.000000 crossroads-schematization-0.2.5/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    51273 2023-07-06 11:24:51.000000 crossroads-schematization-0.2.5/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    25845 2023-07-06 08:52:44.000000 crossroads-schematization-0.2.5/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.5/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 11:28:50.925334 crossroads-schematization-0.2.5/crschem/resources/
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 11:28:50.929334 crossroads-schematization-0.2.5/crschem/resources/400/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.5/crschem/resources/400/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.5/crschem/resources/400/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.5/crschem/resources/400/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.5/crschem/resources/400/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.5/crschem/resources/400/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.5/crschem/resources/400/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.5/crschem/resources/400/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.5/crschem/resources/400/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.5/crschem/resources/400/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.5/crschem/resources/400/style-96.xml
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 11:28:50.929334 crossroads-schematization-0.2.5/crschem/resources/500/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.5/crschem/resources/500/style-96.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.5/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.5/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-06 11:28:50.929334 crossroads-schematization-0.2.5/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.5/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 12:40:44.440175 crossroads-schematization-0.2.6/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.6/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-06 12:40:44.440175 crossroads-schematization-0.2.6/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.6/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 12:40:44.432175 crossroads-schematization-0.2.6/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-06 12:40:44.000000 crossroads-schematization-0.2.6/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1188 2023-07-06 12:40:44.000000 crossroads-schematization-0.2.6/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-06 12:40:44.000000 crossroads-schematization-0.2.6/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-06 12:40:44.000000 crossroads-schematization-0.2.6/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-06 12:40:44.000000 crossroads-schematization-0.2.6/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 12:40:44.436175 crossroads-schematization-0.2.6/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-06 12:40:23.000000 crossroads-schematization-0.2.6/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     8217 2023-07-06 12:33:37.000000 crossroads-schematization-0.2.6/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    52149 2023-07-06 12:32:56.000000 crossroads-schematization-0.2.6/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    26182 2023-07-06 12:12:58.000000 crossroads-schematization-0.2.6/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.6/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 12:40:44.432175 crossroads-schematization-0.2.6/crschem/resources/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 12:40:44.436175 crossroads-schematization-0.2.6/crschem/resources/400/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.6/crschem/resources/400/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.6/crschem/resources/400/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.6/crschem/resources/400/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.6/crschem/resources/400/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.6/crschem/resources/400/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.6/crschem/resources/400/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.6/crschem/resources/400/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.6/crschem/resources/400/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.6/crschem/resources/400/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.6/crschem/resources/400/style-96.xml
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-06 12:40:44.440175 crossroads-schematization-0.2.6/crschem/resources/500/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.6/crschem/resources/500/style-96.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.6/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.6/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-06 12:40:44.440175 crossroads-schematization-0.2.6/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.6/setup.py
```

### Comparing `crossroads-schematization-0.2.5/PKG-INFO` & `crossroads-schematization-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.5
+Version: 0.2.6
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.5/README.md` & `crossroads-schematization-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.2.6/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.5
+Version: 0.2.6
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.5/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.2.6/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/cmd.py` & `crossroads-schematization-0.2.6/crschem/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
     group_preprocess = parser.add_argument_group('Preprocessing', "Parameters of the preprocesses (crseg, crdesc)")
     group_preprocess.add_argument('--c0', help='Initial intersection size (distance between boundaries and middle of the initial intersection). Default: 2.', type=float, default=2)
     group_preprocess.add_argument('--c1', help='Intersection size (aggregation by adjacency). Default: 2.', type=float, default=2)
     group_preprocess.add_argument('--c2', help='Intersection size (aggregation by cycle detection). Default: 4.', type=float, default=4)
 
     group_process = parser.add_argument_group("Processing", "Parameters of the processing")
+    group_process.add_argument('--keep-doubled-crossings', help='In case of double crossings (current bad configuration in OSM data with traffic lights), keep both nodes.', action='store_true')
     group_process.add_argument('--ignore-crossings-for-sidewalks', help='Do not use crossings to shape the sidewalks', action='store_true')
     group_process.add_argument('--use-fixed-width-on-branches', help='Use a fixed width on each branch (do not evaluate the width adjustment)', action='store_true')
     group_process.add_argument('--turn-shape', help='Turn shape.', type=lambda s: c.TurningSidewalk.TurnShape[s], choices=list(c.TurningSidewalk.TurnShape))
 
     group_output = parser.add_argument_group("Output", "Display, log or save results")
     group_output.add_argument('-l', '--log-files', help='keep intermediate files and give their name in output', action='store_true')
     group_output.add_argument('-d', '--display-all', help='display all steps', action='store_true')
@@ -77,14 +78,15 @@
             longitude = args.by_coordinates[1]
             crschem = cs.CrossroadSchematization.build(latitude, longitude,
                                                     args.c0, args.c1, args.c2,
                                                     verbose = True,
                                                     ignore_crossings_for_sidewalks = args.ignore_crossings_for_sidewalks,
                                                     use_fixed_width_on_branches = args.use_fixed_width_on_branches,
                                                     turn_shape = args.turn_shape,
+                                                    remove_doubled_crossings = not args.keep_doubled_crossings,
                                                     ignore_cache = args.ignore_cache,
                                                     overpass = args.overpass,
                                                     log_files = args.log_files)
 
         '''if not crschem.is_valid_model():
             print("Error: the model is not valid")
             exit(1)'''
```

### Comparing `crossroads-schematization-0.2.5/crschem/crossroad.py` & `crossroads-schematization-0.2.6/crschem/crossroad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1015,19 +1015,39 @@
     def get_adjacent_footways_nodes(self):
         return [x for x in self.osm_input[self.node_id] if u.Utils.is_footway_edge(self.osm_input[self.node_id][x][0])]
 
 
     def build_vectors(self, nodes):
         return [u.Utils.normalized_vector(self.osm_input.nodes[self.node_id], self.osm_input.nodes[n]) for n in nodes]
 
+
+    def has_adjacent_crossing(osm_input, cr_input, node, radius = 5):
+        # check for all nodes near to the given node
+        for n in osm_input.nodes:
+            if n != node and Crossing.is_crossing(n, cr_input):
+                if u.Utils.edge_length(osm_input.nodes[n], osm_input.nodes[node]) < radius:
+                    return True
+
+        return False
+
     
-    def create_crossings(osm_input, cr_input, osm_input_oriented, distance_kerb_footway):
-        return dict([(n, Crossing(n, osm_input, cr_input, osm_input_oriented, distance_kerb_footway)) for n in osm_input.nodes if 
+    def create_crossings(osm_input, cr_input, osm_input_oriented, distance_kerb_footway, remove_doubled_crossings):
+        crossings = dict([(n, Crossing(n, osm_input, cr_input, osm_input_oriented, distance_kerb_footway)) for n in osm_input.nodes if 
                       osm_input.nodes[n]["type"] == "input" and Crossing.is_crossing(n, cr_input)])
 
+        if remove_doubled_crossings:
+            print("Removing double crossings")
+            # for each crossing
+            for n in list(crossings.keys()):
+                # if this crossing is on a traffic light node
+                if "highway" in osm_input.nodes[n] and osm_input.nodes[n]["highway"] == "traffic_signals":
+                    if Crossing.has_adjacent_crossing(osm_input, cr_input, n):
+                        del crossings[n]
+
+        return crossings
 
     def is_inside(self, region):
         return region.contains(Point(Point(self.osm_input.nodes[self.node_id]["x"], self.osm_input.nodes[self.node_id]["y"])))
 
     def is_crossing(node, cr_input):
         tags = u.Utils.get_initial_node_tags(cr_input, node)
         return tags and tags["type"] == "crosswalk"
```

### Comparing `crossroads-schematization-0.2.5/crschem/crossroad_schematization.py` & `crossroads-schematization-0.2.6/crschem/crossroad_schematization.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,38 +76,41 @@
     # If the OSM data has been previously loaded, do not load it again
     def __init__(self, cr_input, 
                  osm_oriented = None,
                  osm_unoriented = None,
                  ignore_crossings_for_sidewalks = False,
                  use_fixed_width_on_branches = False,
                  turn_shape = c.TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
+                 remove_doubled_crossings = True,
                  osm_buffer_size_meters = 200, 
                  distance_kerb_footway = 0.5,
                  white_space_meter = 1.5):
         self.osm_buffer_size_meters = osm_buffer_size_meters
         self.distance_kerb_footway = distance_kerb_footway
         self.white_space_meter = white_space_meter
         self.cr_input = cr_input
         self.ignore_crossings_for_sidewalks = ignore_crossings_for_sidewalks
         self.use_fixed_width_on_branches = use_fixed_width_on_branches
         self.turn_shape = turn_shape
+        self.remove_doubled_crossings = remove_doubled_crossings
 
         self.load_osm(osm_oriented, osm_unoriented)
 
         # get crossroad center
         is_n = cr_input["type"] == "crossroads"
         self.center = cr_input[is_n]["geometry"][0]
 
 
 
     def build(latitude, longitude,
               C0, C1, C2,
               ignore_crossings_for_sidewalks = False,
               use_fixed_width_on_branches = False,
               turn_shape = c.TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
+              remove_doubled_crossings = True,
               verbose = True,
               ignore_cache = False,
               overpass = False,
               log_files = False):
 
         import crseg.segmentation as cseg
         import crseg.utils as cru
@@ -161,15 +164,16 @@
             print("Model:", tmp2.name)
         else:
             os.unlink(tmp2.name)
 
         return CrossroadSchematization(cr_input, G_init, 
                                         ignore_crossings_for_sidewalks=ignore_crossings_for_sidewalks, 
                                         use_fixed_width_on_branches=use_fixed_width_on_branches,
-                                        turn_shape=turn_shape)
+                                        turn_shape=turn_shape,
+                                        remove_doubled_crossings=remove_doubled_crossings)
 
     def is_valid_model(self):
         for index, elem in self.cr_input.iterrows():
             if elem["type"] in ["branch", "way"]:                
                 for side in ["left", "right"]:
                     for obj in ["_island", "_sidewalk"]:
                         key = side + obj
@@ -193,15 +197,16 @@
         print("Creating sidewalks")
         self.build_sidewalks()
 
         # add pedestrian crossings
         print("Creating crossings")
         self.crossings = c.Crossing.create_crossings(self.osm_input, self.cr_input, 
                                                      self.osm_input_oriented,
-                                                     self.distance_kerb_footway)
+                                                     self.distance_kerb_footway,
+                                                     self.remove_doubled_crossings)
 
         # assemble sidewalks
         print("Assembling sidewalks")
         self.assemble_sidewalks()
 
         # compute inner region 
         print("Computing inner region")
```

### Comparing `crossroads-schematization-0.2.5/crschem/processing.py` & `crossroads-schematization-0.2.6/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/crossing-3-300.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/crossing-3-96.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/island-300-white.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/island-300.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/island-96-white.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/island-96.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/point-300.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/point-96.svg` & `crossroads-schematization-0.2.6/crschem/resources/400/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/style-300.xml` & `crossroads-schematization-0.2.6/crschem/resources/400/style-300.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/400/style-96.xml` & `crossroads-schematization-0.2.6/crschem/resources/400/style-96.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/crossing-3-300.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/crossing-3-96.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/island-300-white.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/island-300.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/island-96-white.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/island-96.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/point-300.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/point-96.svg` & `crossroads-schematization-0.2.6/crschem/resources/500/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/style-300.xml` & `crossroads-schematization-0.2.6/crschem/resources/500/style-300.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/resources/500/style-96.xml` & `crossroads-schematization-0.2.6/crschem/resources/500/style-96.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/crschem/utils.py` & `crossroads-schematization-0.2.6/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.5/setup.py` & `crossroads-schematization-0.2.6/setup.py`

 * *Files identical despite different names*

