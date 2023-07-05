# Comparing `tmp/microviewer-1.6.2.tar.gz` & `tmp/microviewer-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.6.2.tar", last modified: Tue Jul  4 05:44:26 2023, max compression
+gzip compressed data, was "microviewer-1.6.3.tar", last modified: Wed Jul  5 23:25:21 2023, max compression
```

## Comparing `microviewer-1.6.2.tar` & `microviewer-1.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.531185 microviewer-1.6.2/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-04 05:44:26.000000 microviewer-1.6.2/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     3615 2023-07-04 05:44:26.000000 microviewer-1.6.2/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.6.2/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.6.2/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:44:26.531589 microviewer-1.6.2/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1987 2023-07-03 23:31:40.000000 microviewer-1.6.2/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.522198 microviewer-1.6.2/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.6.2/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.6.2/microviewer/crackle.js
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.529319 microviewer-1.6.2/microviewer/cursors/
--rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/exact-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/exact.png
--rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/large-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/large.png
--rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/medium-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/medium.png
--rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/small-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/small.png
--rw-r--r--   0 wms        (501) staff       (20)    42865 2023-07-04 05:42:09.000000 microviewer-1.6.2/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.6.2/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    36691 2023-07-04 05:42:24.000000 microviewer-1.6.2/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.6.2/microviewer/jquery-3.7.0.min.js
--rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.6.2/microviewer/libcrackle.wasm
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.525299 microviewer-1.6.2/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.6.2/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.530638 microviewer-1.6.2/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.6.2/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.6.2/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.6.2/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)  1240284 2023-07-03 23:07:14.000000 microviewer-1.6.2/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-04 05:44:26.532683 microviewer-1.6.2/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.6.2/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-05 23:25:21.033020 microviewer-1.6.3/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-05 23:25:20.000000 microviewer-1.6.3/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     3696 2023-07-05 23:25:20.000000 microviewer-1.6.3/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.6.3/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.6.3/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-05 23:25:21.033196 microviewer-1.6.3/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1987 2023-07-03 23:31:40.000000 microviewer-1.6.3/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-05 23:25:21.027329 microviewer-1.6.3/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.6.3/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.6.3/microviewer/crackle.js
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-05 23:25:21.032148 microviewer-1.6.3/microviewer/cursors/
+-rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/exact-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/exact.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/large-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/large.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/medium-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/medium.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/small-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.6.3/microviewer/cursors/small.png
+-rw-r--r--   0 wms        (501) staff       (20)    43024 2023-07-05 23:22:37.000000 microviewer-1.6.3/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.6.3/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    36691 2023-07-04 05:42:24.000000 microviewer-1.6.3/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.6.3/microviewer/jquery-3.7.0.min.js
+-rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.6.3/microviewer/libcrackle.wasm
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-05 23:25:21.030370 microviewer-1.6.3/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-05 23:25:20.000000 microviewer-1.6.3/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-05 23:25:21.000000 microviewer-1.6.3/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-05 23:25:20.000000 microviewer-1.6.3/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-05 23:25:20.000000 microviewer-1.6.3/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.6.3/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-05 23:25:20.000000 microviewer-1.6.3/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-05 23:25:20.000000 microviewer-1.6.3/microviewer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-05 23:25:20.000000 microviewer-1.6.3/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-05 23:25:21.032670 microviewer-1.6.3/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.6.3/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.6.3/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.6.3/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)  1240284 2023-07-03 23:07:14.000000 microviewer-1.6.3/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-05 23:25:21.033849 microviewer-1.6.3/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.6.3/setup.py
```

### Comparing `microviewer-1.6.2/ChangeLog` & `microviewer-1.6.3/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+1.6.3
+-----
+
+* fix: paint uint64 arrays
+* fix: select segments on uint64 arrays
+
 1.6.2
 -----
 
 * fix: brushes are circular on rectangular images
 * fix: use pixelated image rendering in chrome
 
 1.6.1
```

### Comparing `microviewer-1.6.2/LICENSE` & `microviewer-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/PKG-INFO` & `microviewer-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.6.2
+Version: 1.6.3
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.6.2/README.md` & `microviewer-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/__init__.py` & `microviewer-1.6.3/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/crackle.js` & `microviewer-1.6.3/microviewer/crackle.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/cursors/exact-active.png` & `microviewer-1.6.3/microviewer/cursors/exact-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/cursors/exact.png` & `microviewer-1.6.3/microviewer/cursors/exact.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/cursors/large-active.png` & `microviewer-1.6.3/microviewer/cursors/large-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/cursors/large.png` & `microviewer-1.6.3/microviewer/cursors/large.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/cursors/medium-active.png` & `microviewer-1.6.3/microviewer/cursors/medium-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/cursors/medium.png` & `microviewer-1.6.3/microviewer/cursors/medium.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/datacube.js` & `microviewer-1.6.3/microviewer/datacube.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -411,29 +411,32 @@
             ry2 = dy * dy / 4;
 
         let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
             xf = Math.min(width, Math.trunc(cx + rx) + 0.5),
             y0 = Math.max(0, Math.trunc(cy - ry) + 0.5),
             yf = Math.min(width, Math.trunc(cy + ry) + 0.5);
 
-        let segid = 0,
+        const ZERO = _this.getSegmentation().cast(0);
+        let segid = ZERO,
             bounds_test = 0.0;
 
         let segids = {};
 
         // For anisotropic data, we need to distort our circle (UI) into an ellipse 
         // since we've distorted the data to be square.
         // eqn of an ellipse: ((x - h)^2 / rx^2) + ((y - k)^2 / ry^2) <= 1
         // We'll use < instead of <= though to exclude the boundary
 
         for (var x = x0; x <= xf; x++) {
             for (var y = y0; y <= yf; y++) {
                 bounds_test = ((x - cx) * (x - cx) / rx2) + ((y - cy) * (y - cy) / ry2);
-                segid = ((bounds_test < 1) && buffer[(x | 0) + width * (y | 0)]) | 0;
-                segids[segid] = true;
+                if (bounds_test < 1) {
+                    segid = buffer[(x | 0) + width * (y | 0)] | ZERO;
+                    segids[segid] = true;
+                }
             }
         }
 
         delete segids[0];
 
         return Object.keys(segids).map((segid) => parseInt(segid, 10));
     }
@@ -454,14 +457,16 @@
         });
     }
 
     paintCircle(axis, slice, dx, dy, cx, cy, label) {
         let _this = this;
         let [width, height] = _this.getSegmentation().faceDimensions(axis);
 
+        label = _this.getSegmentation().cast(label);
+
         if (_this.inverse_renumbering[label] === undefined) {
             _this.renumbering[_this.max_label] = label;
             _this.inverse_renumbering[label] = _this.max_label;
             _this.assigned_colors[_this.max_label] = _this.colorToUint32({
                 r: 0,
                 g: 230,
                 b: 0
@@ -483,15 +488,15 @@
             ry2 = dy * dy / 4;
 
         let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
             xf = Math.min(width, Math.trunc(cx + rx) + 0.5),
             y0 = Math.max(0, Math.trunc(cy - ry) + 0.5),
             yf = Math.min(height, Math.trunc(cy + ry) + 0.5);
 
-        let segid = 0,
+        let segid = _this.getSegmentation().cast(0),
             bounds_test = 0.0;
 
         // For anisotropic data, we need to distort our circle (UI) into an ellipse 
         // since we've distorted the data to be square.
         // eqn of an ellipse: ((x - h)^2 / rx^2) + ((y - k)^2 / ry^2) <= 1
         // We'll use < instead of <= though to exclude the boundary
         let cube = _this.getSegmentation().cube;
```

### Comparing `microviewer-1.6.2/microviewer/favicon.ico` & `microviewer-1.6.3/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/index.html` & `microviewer-1.6.3/microviewer/index.html`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/jquery-3.7.0.min.js` & `microviewer-1.6.3/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer/libcrackle.wasm` & `microviewer-1.6.3/microviewer/libcrackle.wasm`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer.egg-info/PKG-INFO` & `microviewer-1.6.3/microviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.6.2
+Version: 1.6.3
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.6.2/microviewer.egg-info/SOURCES.txt` & `microviewer-1.6.3/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/microviewer_cli/cli.py` & `microviewer-1.6.3/microviewer_cli/cli.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/seg-demo.png` & `microviewer-1.6.3/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.2/setup.cfg` & `microviewer-1.6.3/setup.cfg`

 * *Files identical despite different names*

