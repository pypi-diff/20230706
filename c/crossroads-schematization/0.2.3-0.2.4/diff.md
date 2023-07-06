# Comparing `tmp/crossroads-schematization-0.2.3.tar.gz` & `tmp/crossroads-schematization-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.2.3.tar", last modified: Mon Jul  3 14:59:08 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.2.4.tar", last modified: Tue Jul  4 15:19:05 2023, max compression
```

## Comparing `crossroads-schematization-0.2.3.tar` & `crossroads-schematization-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.3/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.3/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.469362 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     1104 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-03 14:59:08.000000 crossroads-schematization-0.2.3/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.469362 crossroads-schematization-0.2.3/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-03 14:58:46.000000 crossroads-schematization-0.2.3/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     7465 2023-07-03 14:58:16.000000 crossroads-schematization-0.2.3/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-28 14:41:35.000000 crossroads-schematization-0.2.3/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    29411 2023-07-03 14:56:56.000000 crossroads-schematization-0.2.3/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.3/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.3/crschem/resources/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.3/crschem/resources/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.3/crschem/resources/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.3/crschem/resources/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.3/crschem/resources/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.3/crschem/resources/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.3/crschem/resources/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.3/crschem/resources/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-crossings.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-islands.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-polylines-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.2.3/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.3/crschem/resources/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.3/crschem/resources/style-96.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.2.3/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.3/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.3/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-03 14:59:08.477362 crossroads-schematization-0.2.3/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.3/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-04 15:19:05.611098 crossroads-schematization-0.2.4/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.4/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-04 15:19:05.611098 crossroads-schematization-0.2.4/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.4/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-04 15:19:05.607098 crossroads-schematization-0.2.4/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-04 15:19:05.000000 crossroads-schematization-0.2.4/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1188 2023-07-04 15:19:05.000000 crossroads-schematization-0.2.4/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-04 15:19:05.000000 crossroads-schematization-0.2.4/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-04 15:19:05.000000 crossroads-schematization-0.2.4/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-04 15:19:05.000000 crossroads-schematization-0.2.4/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-04 15:19:05.611098 crossroads-schematization-0.2.4/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-04 11:45:06.000000 crossroads-schematization-0.2.4/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     7618 2023-07-04 11:43:01.000000 crossroads-schematization-0.2.4/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-28 14:41:35.000000 crossroads-schematization-0.2.4/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    29389 2023-07-04 11:39:44.000000 crossroads-schematization-0.2.4/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.4/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-04 15:19:05.607098 crossroads-schematization-0.2.4/crschem/resources/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-04 15:19:05.611098 crossroads-schematization-0.2.4/crschem/resources/400/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.4/crschem/resources/400/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.4/crschem/resources/400/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.4/crschem/resources/400/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.4/crschem/resources/400/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.4/crschem/resources/400/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.4/crschem/resources/400/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.4/crschem/resources/400/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.4/crschem/resources/400/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.4/crschem/resources/400/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.4/crschem/resources/400/style-96.xml
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-04 15:19:05.611098 crossroads-schematization-0.2.4/crschem/resources/500/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.4/crschem/resources/500/style-96.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.4/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.4/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-04 15:19:05.611098 crossroads-schematization-0.2.4/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.4/setup.py
```

### Comparing `crossroads-schematization-0.2.3/PKG-INFO` & `crossroads-schematization-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.3
+Version: 0.2.4
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.3/README.md` & `crossroads-schematization-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.2.4/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.3
+Version: 0.2.4
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.3/crschem/cmd.py` & `crossroads-schematization-0.2.4/crschem/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     group_process.add_argument('--turn-shape', help='Turn shape.', type=lambda s: c.TurningSidewalk.TurnShape[s], choices=list(c.TurningSidewalk.TurnShape))
 
     group_output = parser.add_argument_group("Output", "Display, log or save results")
     group_output.add_argument('-l', '--log-files', help='keep intermediate files and give their name in output', action='store_true')
     group_output.add_argument('-d', '--display-all', help='display all steps', action='store_true')
     group_output.add_argument('--display-preview', help='display a preview of the crossroad schematization', action='store_true')
     group_output.add_argument('-o', '--output', help='output file (supported format: geojson, pdf, tif, shp)', type=FileOpener('w'))
+    group_output.add_argument('--scale', help='Scale of the map. Default: 400 (for 1:400)', type=int, default=400, choices=[400, 500])
     group_output.add_argument('--dpi', help='dpi for tif export', type=int, choices=[96, 300], default=300)
     group_output.add_argument('--layout', help='Map layout.', type=lambda s: cs.CrossroadSchematization.Layout[s], choices=list(cs.CrossroadSchematization.Layout))
     group_output.add_argument('--margin', help='Margin in cm. Default: 1.0cm', type=float, default=1)
 
     group_preview = parser.add_argument_group("Preview options", "Parameters used by the preview display")
     group_preview.add_argument('--osm', help='display OpenStreetMap network', action='store_true')
     group_preview.add_argument('--branches', help='display branches', action='store_true')
@@ -104,15 +105,15 @@
 
             if args.output.filename.endswith(".pdf"):
                 print("Exporting as pdf:", args.output.filename)
                 print("!! Legacy export")
                 crschem.toPdf(args.output.filename, args.log_files)
             elif args.output.filename.endswith(".tif"):
                 print("Exporting as tif:", args.output.filename)
-                crschem.toTif(args.output.filename, args.log_files, resolution=args.dpi, layout=args.layout, margin=args.margin)
+                crschem.toTif(args.output.filename, args.log_files, resolution=args.dpi, layout=args.layout, margin=args.margin, scale=args.scale)
             elif args.output.filename.endswith(".svg"):
                 print("Exporting as svg:", args.output.filename)
                 print("!! Legacy export")
                 crschem.toSvg(args.output.filename, args.non_reachable_islands)
             elif args.output.filename.endswith(".geojson"):
                 print("Exporting as geojson:", args.output.filename)
                 crschem.toGeojson(args.output.filename, args.non_reachable_islands)
```

### Comparing `crossroads-schematization-0.2.3/crschem/crossroad.py` & `crossroads-schematization-0.2.4/crschem/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/crossroad_schematization.py` & `crossroads-schematization-0.2.4/crschem/crossroad_schematization.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,17 +506,14 @@
         self.to_printable_internal(filename, log_files)
 
 
     def toTifInternal(self, dirName, filename, log_files, resolution, scale, layout, marginCM):
         widthMeter = layout.width(marginCM / 100)
         heightMeter = layout.height(marginCM / 100)
 
-        # scale (ie 1cm in the map is scale "scale" * 1 cm in reality)
-        scale = 400
-
         width = int(m2px(widthMeter, resolution))
         height = int(m2px(heightMeter, resolution))
 
         mapfile = dirName + "/style-" + str(resolution) + ".xml"
         output = filename
 
         pseudo_mercator = mapnik.Projection('+proj=merc +a=6378137 +b=6378137 +lat_ts=0.0 +lon_0=0.0 +x_0=0.0 +y_0=0 +k=1.0 +units=m +nadgrids=@null +no_defs +over')
@@ -580,21 +577,22 @@
         # first export to shapefiles in a temporary directory
         dirName = tempfile.mkdtemp()
         if log_files:
             print('Temporary directory (styling):', dirName)
         self.toShapefiles(dirName + "/crossroad.shp")
 
         # then move style file (xml) in this directory
+        os.mkdir(dirName + "/" + str(scale))
         if resolution in [96, 300]:
             for f in ["style-" + str(resolution) + ".xml",
                         "crossing-3-" + str(resolution) + ".svg", 
                         "point-" + str(resolution) + ".svg",
                         "island-" + str(resolution) + ".svg",
                         "island-" + str(resolution) + "-white.svg"]:
-                shutil.copy(os.path.dirname(__file__) + "/resources/" + f, dirName)
+                shutil.copy(os.path.dirname(__file__) + "/resources/" + str(scale) + "/" + f, dirName + "/")
         else:
             print("not supported DPI")
             return
 
         # finally render the image
         self.toTifInternal(dirName, filename, log_files, resolution, scale, layout, margin)
```

### Comparing `crossroads-schematization-0.2.3/crschem/processing.py` & `crossroads-schematization-0.2.4/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/crossing-3-300.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/crossing-3-96.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/island-300-white.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/island-300.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/island-96-white.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/island-96.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/point-300.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/point-96.svg` & `crossroads-schematization-0.2.4/crschem/resources/400/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/style-300.xml` & `crossroads-schematization-0.2.4/crschem/resources/400/style-300.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/resources/style-96.xml` & `crossroads-schematization-0.2.4/crschem/resources/400/style-96.xml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/crschem/utils.py` & `crossroads-schematization-0.2.4/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.3/setup.py` & `crossroads-schematization-0.2.4/setup.py`

 * *Files identical despite different names*

