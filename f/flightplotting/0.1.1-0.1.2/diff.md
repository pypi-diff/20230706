# Comparing `tmp/flightplotting-0.1.1.tar.gz` & `tmp/flightplotting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightplotting-0.1.1.tar", last modified: Wed Jun 14 09:42:33 2023, max compression
+gzip compressed data, was "flightplotting-0.1.2.tar", last modified: Thu Jul  6 10:41:36 2023, max compression
```

## Comparing `flightplotting-0.1.1.tar` & `flightplotting-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    35129 2023-03-28 15:54:20.000000 flightplotting-0.1.1/COPYING
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-03-28 15:54:20.000000 flightplotting-0.1.1/MANIFEST.in
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      376 2023-06-14 09:42:33.808484 flightplotting-0.1.1/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       88 2023-03-28 15:54:20.000000 flightplotting-0.1.1/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.800484 flightplotting-0.1.1/flightplotting/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       66 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/flightplotting/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)   142015 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/data/ColdDraftF3APlane.obj
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/data/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2976 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/model.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7217 2023-06-05 19:30:36.000000 flightplotting-0.1.1/flightplotting/plots.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      741 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/templates.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1298 2023-05-20 13:06:57.000000 flightplotting-0.1.1/flightplotting/titlerenderer.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7118 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/traces.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/flightplotting.egg-info/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      376 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      492 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       57 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      459 2023-06-14 09:42:33.808484 flightplotting-0.1.1/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      668 2023-03-28 15:54:20.000000 flightplotting-0.1.1/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      256 2023-03-28 15:54:20.000000 flightplotting-0.1.1/tests/test_traces.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:41:36.290369 flightplotting-0.1.2/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    35129 2023-03-28 15:54:20.000000 flightplotting-0.1.2/COPYING
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-03-28 15:54:20.000000 flightplotting-0.1.2/MANIFEST.in
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      413 2023-07-06 10:41:36.294369 flightplotting-0.1.2/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       88 2023-03-28 15:54:20.000000 flightplotting-0.1.2/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:41:36.290369 flightplotting-0.1.2/flightplotting/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       66 2023-03-28 15:54:20.000000 flightplotting-0.1.2/flightplotting/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:41:36.290369 flightplotting-0.1.2/flightplotting/data/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)   142015 2023-03-28 15:54:20.000000 flightplotting-0.1.2/flightplotting/data/ColdDraftF3APlane.obj
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-03-28 15:54:20.000000 flightplotting-0.1.2/flightplotting/data/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2976 2023-03-28 15:54:20.000000 flightplotting-0.1.2/flightplotting/model.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7217 2023-07-04 20:36:21.000000 flightplotting-0.1.2/flightplotting/plots.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      741 2023-03-28 15:54:20.000000 flightplotting-0.1.2/flightplotting/templates.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1298 2023-05-20 13:06:57.000000 flightplotting-0.1.2/flightplotting/titlerenderer.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7146 2023-07-04 20:38:00.000000 flightplotting-0.1.2/flightplotting/traces.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:41:36.290369 flightplotting-0.1.2/flightplotting.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      413 2023-07-06 10:41:36.000000 flightplotting-0.1.2/flightplotting.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      492 2023-07-06 10:41:36.000000 flightplotting-0.1.2/flightplotting.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-07-06 10:41:36.000000 flightplotting-0.1.2/flightplotting.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       57 2023-07-06 10:41:36.000000 flightplotting-0.1.2/flightplotting.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-07-06 10:41:36.000000 flightplotting-0.1.2/flightplotting.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      459 2023-07-06 10:41:36.294369 flightplotting-0.1.2/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      668 2023-03-28 15:54:20.000000 flightplotting-0.1.2/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-06 10:41:36.290369 flightplotting-0.1.2/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      256 2023-03-28 15:54:20.000000 flightplotting-0.1.2/tests/test_traces.py
```

### Comparing `flightplotting-0.1.1/COPYING` & `flightplotting-0.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.1/flightplotting/data/ColdDraftF3APlane.obj` & `flightplotting-0.1.2/flightplotting/data/ColdDraftF3APlane.obj`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.1/flightplotting/model.py` & `flightplotting-0.1.2/flightplotting/model.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.1/flightplotting/plots.py` & `flightplotting-0.1.2/flightplotting/plots.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.1/flightplotting/templates.py` & `flightplotting-0.1.2/flightplotting/templates.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.1/flightplotting/titlerenderer.py` & `flightplotting-0.1.2/flightplotting/titlerenderer.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.1/flightplotting/traces.py` & `flightplotting-0.1.2/flightplotting/traces.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,24 @@
         i=[0, 0, 0, 0, 0], 
         j=[1, 2, 1, 3, 4], 
         k=[2, 3, 4, 6, 6],
         opacity=0.4
     )]
 
 
-def meshes(npoints, seq, colour, obj: OBJ=obj):
-    step = int(len(seq.data) / (npoints+1))
+def meshes(npoints, seq: State, colour, obj: OBJ=obj):
+    step = int(len(seq.data) / max(npoints, 1))
     
-    return [obj.transform(Transformation(st.pos, st.att)).create_mesh(colour,f"{st.time.t[0]:.1f}") for st in seq[::step]]
+    ms = []
+
+    sts = [seq[0]] + [ st for st in seq[::step]] + [seq[-1]]
+    for st in sts:
+        ms.append(obj.transform(Transformation(st.pos, st.att)).create_mesh(colour,f"{st.time.t[0]:.1f}"))
+    return ms
+#    return [obj.transform(Transformation(st.pos, st.att)).create_mesh(colour,f"{st.time.t[0]:.1f}") for st in seq[::step]]
 
 
 def vectors(npoints: int, seq: State, vectors: Point, **kwargs):
     trs = []
     step = int(len(seq.data) / (npoints+1))
     for pos, wind in zip(seq.pos[::step], vectors[::step]):
         pdata = Point.concatenate([pos, pos+wind])
@@ -157,47 +163,39 @@
 
 
 def axis_rate_trace(sec, dash="solid", colours = px.colors.qualitative.Plotly):
     return sec_col_trace(sec, sec.constructs.rvel.keys, dash, colours, np.degrees) 
 
 
 
-
-
-
 control_inputs =  ["aileron_1", "aileron_2", "elevator", "rudder", "throttle"]
 
 def control_input_trace(sec, dash="solid", colours = px.colors.qualitative.Plotly, control_inputs = None):
     if control_inputs is None:
         control_inputs =  ["aileron", "elevator", "rudder", "throttle"]
     return sec_col_trace(sec,control_inputs, dash, colours)
 
 
 def aoa_trace(sec, dash="dash", colours = px.colors.qualitative.Plotly):
     #sec = sec.append_columns(sec.aoa())
     return sec_col_trace(sec, ["alpha", "beta"], dash, colours, np.degrees)
 
-def _axistrace(cid: Coord, length:float=20.0):
+def axestrace(cid: Coord, length:float=20.0):
     ntraces = []
     colours = {"x":"red", "y":"blue", "z":"green"}
     for ax, col in zip([cid.x_axis, cid.y_axis, cid.z_axis], list("xyz")):
         axis = Point.concatenate([cid.origin, cid.origin + ax * length])
         ntraces.append(go.Scatter3d(
             x=axis.x, y=axis.y, z=axis.z, mode="lines", 
             line=dict(color=colours[col]),
             name=col
         ))
         
     return ntraces
 
-def axestrace(cids: Union[Coord, List[Coord]]):
-    if isinstance(cids, List):
-        return [_axistrace(cid) for cid in cids]
-    elif isinstance(cids, Coord):
-        return _axistrace(cids)
 
 
 
 def _npinterzip(a, b):
     """
     takes two numpy arrays and zips them.
     Args:
```

### Comparing `flightplotting-0.1.1/setup.py` & `flightplotting-0.1.2/setup.py`

 * *Files identical despite different names*

