# Comparing `tmp/pynuml-23.6.1.tar.gz` & `tmp/pynuml-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynuml-23.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynuml-23.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynuml-23.6.1.tar` & `pynuml-23.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       17 2022-08-22 18:47:46.562567 pynuml-23.6.1/.gitignore
--rw-r--r--   0        0        0      824 2023-06-15 20:05:13.774670 pynuml-23.6.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1074 2023-05-23 17:23:11.333385 pynuml-23.6.1/LICENSE
--rw-r--r--   0        0        0     5647 2023-05-11 17:09:33.660248 pynuml-23.6.1/README.md
--rw-r--r--   0        0        0      170 2022-08-22 18:47:46.563031 pynuml-23.6.1/doc/README.md
--rw-r--r--   0        0        0     9267 2022-08-22 18:47:46.563254 pynuml-23.6.1/doc/graph_create.md
--rw-r--r--   0        0        0     2903 2022-08-22 18:47:46.563416 pynuml-23.6.1/doc/python_env.md
--rw-r--r--   0        0        0      638 2023-05-23 17:23:11.333546 pynuml-23.6.1/docs/Makefile
--rw-r--r--   0        0        0      924 2023-06-26 16:24:16.942644 pynuml-23.6.1/docs/conf.py
--rw-r--r--   0        0        0      673 2023-06-15 20:05:13.775100 pynuml-23.6.1/docs/index.rst
--rw-r--r--   0        0        0     1413 2023-06-15 20:05:13.775357 pynuml-23.6.1/docs/install/installation.rst
--rw-r--r--   0        0        0      804 2023-05-23 17:23:11.333683 pynuml-23.6.1/docs/make.bat
--rw-r--r--   0        0        0      581 2022-08-22 18:47:46.563608 pynuml-23.6.1/example/plot.py
--rwxr-xr-x   0        0        0     2089 2022-11-30 18:31:20.903706 pynuml-23.6.1/example/process.py
--rw-r--r--   0        0        0     1169 2022-08-22 18:47:46.563858 pynuml-23.6.1/h5merge.py
--rw-r--r--   0        0        0       38 2022-10-01 15:34:05.362452 pynuml-23.6.1/pynuml/.gitignore
--rw-r--r--   0        0        0      164 2023-06-26 16:24:16.942849 pynuml-23.6.1/pynuml/__init__.py
--rw-r--r--   0        0        0       97 2023-02-27 22:44:16.230810 pynuml-23.6.1/pynuml/io/__init__.py
--rw-r--r--   0        0        0    33647 2023-05-23 17:23:11.334552 pynuml-23.6.1/pynuml/io/file.py
--rw-r--r--   0        0        0     3224 2023-06-26 16:24:16.943048 pynuml-23.6.1/pynuml/io/h5interface.py
--rw-r--r--   0        0        0     4089 2023-05-23 17:23:11.334967 pynuml-23.6.1/pynuml/io/out.py
--rw-r--r--   0        0        0      102 2023-06-15 20:05:13.776689 pynuml-23.6.1/pynuml/labels/__init__.py
--rw-r--r--   0        0        0     1476 2022-10-01 15:34:05.363366 pynuml-23.6.1/pynuml/labels/ccqe.py
--rw-r--r--   0        0        0     1156 2023-06-15 20:05:13.776860 pynuml-23.6.1/pynuml/labels/flavor.py
--rw-r--r--   0        0        0      779 2023-05-23 17:23:11.335229 pynuml-23.6.1/pynuml/labels/simple.py
--rw-r--r--   0        0        0    10593 2023-06-15 15:41:12.568618 pynuml-23.6.1/pynuml/labels/standard.py
--rw-r--r--   0        0        0       28 2023-05-23 17:23:11.335591 pynuml-23.6.1/pynuml/plot/__init__.py
--rw-r--r--   0        0        0     5246 2023-05-23 17:23:11.335785 pynuml-23.6.1/pynuml/plot/graph.py
--rw-r--r--   0        0        0       39 2023-02-27 22:44:16.231786 pynuml-23.6.1/pynuml/process/__init__.py
--rw-r--r--   0        0        0      463 2023-02-27 22:44:16.231898 pynuml-23.6.1/pynuml/process/base.py
--rw-r--r--   0        0        0     6703 2023-06-23 18:03:06.407000 pynuml-23.6.1/pynuml/process/hitgraph.py
--rw-r--r--   0        0        0     3780 2022-10-01 15:34:05.363995 pynuml-23.6.1/pynuml/process/spmap.py
--rw-r--r--   0        0        0      599 2023-06-15 15:15:22.011325 pynuml-23.6.1/pyproject.toml
--rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 pynuml-23.6.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2022-08-22 18:47:46.562567 pynuml-23.7.0/.gitignore
+-rw-r--r--   0        0        0      824 2023-06-15 20:05:13.774670 pynuml-23.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1074 2023-05-23 17:23:11.333385 pynuml-23.7.0/LICENSE
+-rw-r--r--   0        0        0     5647 2023-05-11 17:09:33.660248 pynuml-23.7.0/README.md
+-rw-r--r--   0        0        0      170 2022-08-22 18:47:46.563031 pynuml-23.7.0/doc/README.md
+-rw-r--r--   0        0        0     9267 2022-08-22 18:47:46.563254 pynuml-23.7.0/doc/graph_create.md
+-rw-r--r--   0        0        0     2903 2022-08-22 18:47:46.563416 pynuml-23.7.0/doc/python_env.md
+-rw-r--r--   0        0        0      638 2023-05-23 17:23:11.333546 pynuml-23.7.0/docs/Makefile
+-rw-r--r--   0        0        0      905 2023-07-06 19:11:22.405702 pynuml-23.7.0/docs/conf.py
+-rw-r--r--   0        0        0      673 2023-06-15 20:05:13.775100 pynuml-23.7.0/docs/index.rst
+-rw-r--r--   0        0        0     1413 2023-06-15 20:05:13.775357 pynuml-23.7.0/docs/install/installation.rst
+-rw-r--r--   0        0        0      804 2023-05-23 17:23:11.333683 pynuml-23.7.0/docs/make.bat
+-rw-r--r--   0        0        0      581 2022-08-22 18:47:46.563608 pynuml-23.7.0/example/plot.py
+-rwxr-xr-x   0        0        0     2089 2022-11-30 18:31:20.903706 pynuml-23.7.0/example/process.py
+-rw-r--r--   0        0        0     1169 2022-08-22 18:47:46.563858 pynuml-23.7.0/h5merge.py
+-rw-r--r--   0        0        0       38 2022-10-01 15:34:05.362452 pynuml-23.7.0/pynuml/.gitignore
+-rw-r--r--   0        0        0      164 2023-07-06 19:11:22.405964 pynuml-23.7.0/pynuml/__init__.py
+-rw-r--r--   0        0        0       97 2023-02-27 22:44:16.230810 pynuml-23.7.0/pynuml/io/__init__.py
+-rw-r--r--   0        0        0    33647 2023-05-23 17:23:11.334552 pynuml-23.7.0/pynuml/io/file.py
+-rw-r--r--   0        0        0     3224 2023-06-26 16:24:16.943048 pynuml-23.7.0/pynuml/io/h5interface.py
+-rw-r--r--   0        0        0     4089 2023-05-23 17:23:11.334967 pynuml-23.7.0/pynuml/io/out.py
+-rw-r--r--   0        0        0      102 2023-06-15 20:05:13.776689 pynuml-23.7.0/pynuml/labels/__init__.py
+-rw-r--r--   0        0        0     1476 2022-10-01 15:34:05.363366 pynuml-23.7.0/pynuml/labels/ccqe.py
+-rw-r--r--   0        0        0     1119 2023-07-06 19:07:10.376650 pynuml-23.7.0/pynuml/labels/flavor.py
+-rw-r--r--   0        0        0      779 2023-05-23 17:23:11.335229 pynuml-23.7.0/pynuml/labels/simple.py
+-rw-r--r--   0        0        0    10593 2023-06-28 17:21:51.440062 pynuml-23.7.0/pynuml/labels/standard.py
+-rw-r--r--   0        0        0       28 2023-05-23 17:23:11.335591 pynuml-23.7.0/pynuml/plot/__init__.py
+-rw-r--r--   0        0        0     5245 2023-07-06 19:07:10.377450 pynuml-23.7.0/pynuml/plot/graph.py
+-rw-r--r--   0        0        0       39 2023-02-27 22:44:16.231786 pynuml-23.7.0/pynuml/process/__init__.py
+-rw-r--r--   0        0        0      463 2023-02-27 22:44:16.231898 pynuml-23.7.0/pynuml/process/base.py
+-rw-r--r--   0        0        0     7479 2023-07-06 19:07:10.377725 pynuml-23.7.0/pynuml/process/hitgraph.py
+-rw-r--r--   0        0        0     3780 2022-10-01 15:34:05.363995 pynuml-23.7.0/pynuml/process/spmap.py
+-rw-r--r--   0        0        0      599 2023-06-15 15:15:22.011325 pynuml-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 pynuml-23.7.0/PKG-INFO
```

### Comparing `pynuml-23.6.1/.readthedocs.yaml` & `pynuml-23.7.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/LICENSE` & `pynuml-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/README.md` & `pynuml-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/doc/graph_create.md` & `pynuml-23.7.0/doc/graph_create.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/doc/python_env.md` & `pynuml-23.7.0/doc/python_env.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/docs/Makefile` & `pynuml-23.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/docs/conf.py` & `pynuml-23.7.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'pynuml'
 copyright = '2023, v hewes'
 author = 'v hewes'
-release = '23.6.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ['_templates']
```

### Comparing `pynuml-23.6.1/docs/index.rst` & `pynuml-23.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/docs/install/installation.rst` & `pynuml-23.7.0/docs/install/installation.rst`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/docs/make.bat` & `pynuml-23.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/example/plot.py` & `pynuml-23.7.0/example/plot.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/example/process.py` & `pynuml-23.7.0/example/process.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/h5merge.py` & `pynuml-23.7.0/h5merge.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pynuml/io/file.py` & `pynuml-23.7.0/pynuml/io/file.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pynuml/io/h5interface.py` & `pynuml-23.7.0/pynuml/io/h5interface.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pynuml/io/out.py` & `pynuml-23.7.0/pynuml/io/out.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pynuml/labels/ccqe.py` & `pynuml-23.7.0/pynuml/labels/ccqe.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pynuml/labels/flavor.py` & `pynuml-23.7.0/pynuml/labels/flavor.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,15 @@
     def cc_numu(self):
         return self.index('cc_numu')
 
     @property
     def nc(self):
         return self.index('nc')
 
-    def __call__(self, events: pd.DataFrame):
-        event = events.squeeze()
+    def __call__(self, event: pd.Series):
         if not event.is_cc:
             return self.nc
         pdg = abs(event.nu_pdg)
         if pdg == 12:
             return self.cc_nue
         if pdg == 14:
             return self.cc_numu
```

### Comparing `pynuml-23.6.1/pynuml/labels/simple.py` & `pynuml-23.7.0/pynuml/labels/simple.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pynuml/labels/standard.py` & `pynuml-23.7.0/pynuml/labels/standard.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pynuml/plot/graph.py` & `pynuml-23.7.0/pynuml/plot/graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import List
-
 import pandas as pd
 from torch_geometric.data import HeteroData
 import plotly.express as px
+from plotly.graph_objects import FigureWidget
 
 class GraphPlot:
     def __init__(self,
-                 planes: List[str],
-                 classes: List[str]):
+                 planes: list[str],
+                 classes: list[str]):
         self._planes = planes
         self._classes = classes
         self._labels = pd.CategoricalDtype(classes, ordered=True)
         self._cmap = { c: px.colors.qualitative.Plotly[i] for i, c in enumerate(self._classes) }
         self._data = None
         self._df = None
 
@@ -20,34 +19,31 @@
             return pd.Categorical.from_codes(codes=arr, dtype=self._labels)
         dfs = []
         for p in self._planes:
             plane = data[p].to_dict()
             df = pd.DataFrame(plane['id'], columns=['id'])
             df['plane'] = p
             df[['wire','time']] = plane['pos']
-            df['y_f'] = plane['y_f']
-            mask = df.y_f.values
-            df.loc[mask, 'y_s'] = to_categorical(plane['y_s'])
-            df.loc[mask, 'y_i'] = plane['y_i'].numpy()
-            if 'x_s' in plane.keys():
-                df['x_s'] = to_categorical(plane['x_s'].argmax(dim=-1).detach())
-                df[self._classes] = plane['x_s'].detach()
-            if 'x_f' in plane.keys():
-                df['x_f'] = plane['x_f'].detach()
+            df['y_filter'] = plane['y_semantic'] != -1
+            mask = df.y_filter.values
+            df['y_semantic'] = to_categorical(plane['y_semantic'])
+            df['y_instance'] = plane['y_instance'].numpy()
+            if 'x_semantic' in plane.keys():
+                df['x_semantic'] = to_categorical(plane['x_semantic'].argmax(dim=-1).detach())
+                df[self._classes] = plane['x_semantic'].detach()
+            if 'x_filter' in plane.keys():
+                df['x_filter'] = plane['x_filter'].detach()
             dfs.append(df)
         return pd.concat(dfs)
 
     def plot(self,
              data: HeteroData,
-             name: str,
              target: str = 'hits',
              how: str = 'none',
-             filter: str = 'none',
-             write_png: bool = True,
-             write_html: bool = False):
+             filter: str = 'none') -> FigureWidget:
 
         if data is not self._data:
             self._data = data
             self._df = self.to_dataframe(data)
 
         # no colour
         if target == 'hits':
@@ -56,23 +52,23 @@
             }
 
         # semantic labels
         elif target == 'semantic':
             if how == 'true':
                 opts = {
                     'title': 'True semantic labels',
-                    'labels': { 'y_s': 'Semantic label' },
-                    'color': 'y_s',
+                    'labels': { 'y_semantic': 'Semantic label' },
+                    'color': 'y_semantic',
                     'color_discrete_map': self._cmap
                 }
             elif how == 'pred':
                 opts = {
                     'title': 'Predicted semantic labels',
-                    'labels': { 'x_s': 'Semantic label' },
-                    'color': 'x_s',
+                    'labels': { 'x_semantic': 'Semantic label' },
+                    'color': 'x_semantic',
                     'color_discrete_map': self._cmap
                 }
             elif how in self._classes:
                 opts = {
                     'title': f'Predicted semantic label strength for {how} class',
                     'labels': { how: f'{how} probability' },
                     'color': how,
@@ -82,61 +78,58 @@
                 raise Exception('for semantic labels, "how" must be one of "true", "pred" or the name of a class.')
 
         # instance labels
         elif target == 'instance':
             if how == 'true':
                 opts = {
                     'title': 'True instance labels',
-                    'labels': { 'y_i': 'Instance label' },
-                    'color': 'y_i'
+                    'labels': { 'y_instance': 'Instance label' },
+                    'color': 'y_instance'
                 }
             elif how == 'pred':
                 opts = {
                     'title': 'Predicted instance labels',
-                    'labels': { 'x_i': 'Instance label' },
-                    'color': 'x_i'
+                    'labels': { 'x_instance': 'Instance label' },
+                    'color': 'x_instance'
                 }
             else:
                 raise Exception('for instance labels, "how" must be one of "true" or "pred".')
 
         # filter labels
         elif target == 'filter':
             if how == 'true':
                 opts = {
                     'title': 'True filter labels',
-                    'labels': { 'y_f': 'Filter label' },
-                    'color': 'y_f',
+                    'labels': { 'y_filter': 'Filter label' },
+                    'color': 'y_filter',
                     'color_continuous_scale': px.colors.sequential.Reds
                 }
             elif how == 'pred':
                 opts = {
                     'title': 'Predicted filter labels',
-                    'labels': { 'x_f': 'Filter label' },
-                    'color': 'x_f',
+                    'labels': { 'x_filter': 'Filter label' },
+                    'color': 'x_filter',
                     'color_continuous_scale': px.colors.sequential.Reds
                 }
             else:
                 raise Exception('for filter labels, "how" must be one of "true" or "pred".')
 
         else:
             raise Exception('"target" must be one of "hits", "semantic", "instance" or "filter".')
 
         if filter == 'none':
             df = self._df
         elif filter == 'true':
-            df = self._df[self._df.y_f.values]
+            df = self._df[self._df.y_filter.values]
             opts['title'] += ' (filtered by truth)'
         elif filter == 'pred':
-            df = self._df[self._df.x_f > 0.5]
+            df = self._df[self._df.x_filter > 0.5]
             opts['title'] += ' (filtered by prediction)'
         else:
             raise Exception('"filter" must be one of "none", "true" or "pred.')
 
         fig = px.scatter(df, x='wire', y='time', facet_col='plane', **opts)
         fig.update_yaxes(matches=None)
         fig.update_xaxes(matches=None)
         for a in fig.layout.annotations:
             a.text = a.text.replace('plane=', '')
-        if write_html:
-            fig.write_html(f'{name}.html')
-        if write_png:
-            fig.write_image(f'{name}.png')
+        return FigureWidget(fig)
```

### Comparing `pynuml-23.6.1/pynuml/process/hitgraph.py` & `pynuml-23.7.0/pynuml/process/hitgraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 class HitGraphProducer(ProcessorBase):
     '''Process event into graphs'''
 
     def __init__(self,
                  file: 'pynuml.io.File',
                  semantic_labeller: Callable = None,
                  event_labeller: Callable = None,
+                 label_vertex: bool = False,
                  planes: list[str] = ['u','v','y'],
                  node_pos: list[str] = ['local_wire','local_time'],
                  pos_norm: list[float] = [0.3,0.055],
                  node_feats: list[str] = ['integral','rms'],
                  lower_bound: int = 20,
                  filter_hits: bool = False):
 
         self.semantic_labeller = semantic_labeller
         self.event_labeller = event_labeller
+        self.label_vertex = label_vertex
         self.planes = planes
         self.node_pos = node_pos
         self.pos_norm = torch.tensor(pos_norm).float()
         self.node_feats = node_feats
         self.lower_bound = lower_bound
         self.filter_hits = filter_hits
 
@@ -43,14 +45,20 @@
             'spacepoint_table': ['spacepoint_id','hit_id']
         }
         if self.semantic_labeller:
             groups['particle_table'] = ['g4_id','parent_id','type','momentum','start_process','end_process']
             groups['edep_table'] = []
         if self.event_labeller:
             groups['event_table'] = ['is_cc', 'nu_pdg']
+        if self.label_vertex:
+            keys = ['nu_vtx','nu_vtx_wire_pos','nu_vtx_wire_time']
+            if 'event_table' in groups:
+                groups['event_table'].extend(keys)
+            else:
+                groups['event_table'] = keys
         return groups
 
     @property
     def metadata(self):
         metadata = { 'planes': self.planes }
         if self.semantic_labeller is not None:
             metadata['semantic_classes'] = self.semantic_labeller.labels[:-1]
@@ -59,14 +67,16 @@
         return metadata
 
     def __call__(self, evt: 'pynuml.io.Event') -> tuple[str, Any]:
 
         event_id = evt.event_id
         name = f'r{event_id[0]}_sr{event_id[1]}_evt{event_id[2]}'
 
+        event = evt['event_table'].squeeze()
+
         hits = evt['hit_table']
         spacepoints = evt['spacepoint_table'].reset_index(drop=True)
 
         # handle energy depositions
         if self.filter_hits or self.semantic_labeller:
             edeps = evt['edep_table']
             energy_col = 'energy' if 'energy' in edeps.columns else 'energy_fraction' # for backwards compatibility
@@ -156,11 +166,21 @@
             edge3d = torch.tensor(edge3d) if edge3d.size else torch.empty((2,0))
             data[p, 'nexus', 'sp'].edge_index = edge3d.long()
 
             # truth information
             if self.semantic_labeller:
                 data[p].y_semantic = torch.tensor(plane_hits['semantic_label'].fillna(-1).values).long()
                 data[p].y_instance = torch.tensor(plane_hits['instance_label'].fillna(-1).values).long()
-            if self.event_labeller:
-                data['evt'].y = torch.tensor(self.event_labeller(evt['event_table'])).long()
+            if self.label_vertex:
+                vtx_2d = torch.tensor([ event[f'nu_vtx_wire_pos_{i}'], event.nu_vtx_wire_time ]).float()
+                data[p].y_vtx = vtx_2d * self.pos_norm[None,:]
+
+        # event label
+        if self.event_labeller:
+            data['evt'].y = torch.tensor(self.event_labeller(event)).long()
+
+        # 3D vertex truth
+        if self.label_vertex:
+            vtx_3d = [ event.nu_vtx_x, event.nu_vtx_y, event.nu_vtx_z ]
+            data['evt'].y_vtx = torch.tensor(vtx_3d).float()
 
-        return evt.name, data
+        return evt.name, data
```

### Comparing `pynuml-23.6.1/pynuml/process/spmap.py` & `pynuml-23.7.0/pynuml/process/spmap.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/pyproject.toml` & `pynuml-23.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynuml-23.6.1/PKG-INFO` & `pynuml-23.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynuml
-Version: 23.6.1
+Version: 23.7.0
 Summary: Standardised ML input processing for particle physics
 Author-email: v hewes <vhewes@fnal.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: h5py>=3.7.0
```

