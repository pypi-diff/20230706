# Comparing `tmp/cdfs-0.1.0.tar.gz` & `tmp/cdfs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdfs-0.1.0.tar", max compression
+gzip compressed data, was "cdfs-0.1.1.tar", max compression
```

## Comparing `cdfs-0.1.0.tar` & `cdfs-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-01-05 21:55:12.930593 cdfs-0.1.0/LICENSE.rst
--rw-r--r--   0        0        0     2689 2023-01-05 21:59:57.824594 cdfs-0.1.0/README.rst
--rw-r--r--   0        0        0     1826 2023-06-13 19:06:46.427311 cdfs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      242 2023-06-13 18:49:59.544575 cdfs-0.1.0/src/cdfs/__init__.py
--rw-r--r--   0        0        0      424 2023-06-13 18:49:59.592575 cdfs-0.1.0/src/cdfs/contentsfile/__init__.py
--rw-r--r--   0        0        0      521 2023-06-13 18:49:59.528575 cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/__init__.py
--rw-r--r--   0        0        0    15241 2023-06-13 18:49:59.612575 cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/contentdatasetcomponent.py
--rw-r--r--   0        0        0    15890 2023-06-13 18:48:50.236871 cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/contentgroupcomponent.py
--rw-r--r--   0        0        0      503 2023-06-13 18:49:59.624575 cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/contentsfilecomponent.py
--rw-r--r--   0        0        0    16763 2023-06-13 18:49:59.632575 cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/timecontentdatasetcomponent.py
--rw-r--r--   0        0        0    41849 2023-06-13 18:49:59.640575 cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/timecontentgroupcomponent.py
--rw-r--r--   0        0        0      259 2023-06-13 18:49:59.476575 cdfs-0.1.0/src/cdfs/contentsfile/contentframes/__init__.py
--rw-r--r--   0        0        0    14226 2023-06-13 18:49:59.580575 cdfs-0.1.0/src/cdfs/contentsfile/contentframes/timecontentframe.py
--rw-r--r--   0        0        0      344 2023-06-13 18:49:59.588575 cdfs-0.1.0/src/cdfs/contentsfile/contentmaps/__init__.py
--rw-r--r--   0        0        0     2778 2023-06-13 18:49:59.516575 cdfs-0.1.0/src/cdfs/contentsfile/contentmaps/contentmaps.py
--rw-r--r--   0        0        0     2512 2023-06-13 18:49:59.600575 cdfs-0.1.0/src/cdfs/contentsfile/contentmaps/timecontentmaps.py
--rw-r--r--   0        0        0     1414 2023-06-13 18:49:59.552575 cdfs-0.1.0/src/cdfs/contentsfile/contentsfile.py
--rw-r--r--   0        0        0      994 2023-06-13 18:49:59.620575 cdfs-0.1.0/src/cdfs/contentsfile/timecontentsfile.py
--rw-r--r--   0        0        0      500 2023-06-13 19:06:11.343510 cdfs-0.1.0/src/cdfs/header.py
--rw-r--r--   0        0        0        0 2023-01-05 21:55:12.930593 cdfs-0.1.0/src/cdfs/py.typed
--rw-r--r--   0        0        0      234 2023-06-13 18:49:59.632575 cdfs-0.1.0/src/cdfs/structureobjects/__init__.py
--rw-r--r--   0        0        0     7075 2023-06-13 18:49:59.524575 cdfs-0.1.0/src/cdfs/structureobjects/cdfs.py
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cdfs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-01-05 21:55:12.930593 cdfs-0.1.1/LICENSE.rst
+-rw-r--r--   0        0        0     2689 2023-01-05 21:59:57.824594 cdfs-0.1.1/README.rst
+-rw-r--r--   0        0        0     1826 2023-07-05 22:34:20.393125 cdfs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      242 2023-06-13 18:49:59.544575 cdfs-0.1.1/src/cdfs/__init__.py
+-rw-r--r--   0        0        0      424 2023-06-13 18:49:59.592575 cdfs-0.1.1/src/cdfs/contentsfile/__init__.py
+-rw-r--r--   0        0        0      521 2023-06-13 18:49:59.528575 cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/__init__.py
+-rw-r--r--   0        0        0    15238 2023-06-29 20:55:34.806547 cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/contentdatasetcomponent.py
+-rw-r--r--   0        0        0    15890 2023-06-13 18:48:50.236871 cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/contentgroupcomponent.py
+-rw-r--r--   0        0        0      503 2023-06-13 18:49:59.624575 cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/contentsfilecomponent.py
+-rw-r--r--   0        0        0    16819 2023-06-29 20:52:36.386898 cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/timecontentdatasetcomponent.py
+-rw-r--r--   0        0        0    42604 2023-06-29 20:52:36.386898 cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/timecontentgroupcomponent.py
+-rw-r--r--   0        0        0      259 2023-06-13 18:49:59.476575 cdfs-0.1.1/src/cdfs/contentsfile/contentframes/__init__.py
+-rw-r--r--   0        0        0    14329 2023-06-29 23:53:21.228169 cdfs-0.1.1/src/cdfs/contentsfile/contentframes/timecontentframe.py
+-rw-r--r--   0        0        0      344 2023-06-13 18:49:59.588575 cdfs-0.1.1/src/cdfs/contentsfile/contentmaps/__init__.py
+-rw-r--r--   0        0        0     2778 2023-06-13 18:49:59.516575 cdfs-0.1.1/src/cdfs/contentsfile/contentmaps/contentmaps.py
+-rw-r--r--   0        0        0     2512 2023-06-13 18:49:59.600575 cdfs-0.1.1/src/cdfs/contentsfile/contentmaps/timecontentmaps.py
+-rw-r--r--   0        0        0     1414 2023-06-13 18:49:59.552575 cdfs-0.1.1/src/cdfs/contentsfile/contentsfile.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:52:36.558898 cdfs-0.1.1/src/cdfs/contentsfile/sqlite/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-29 20:52:36.582898 cdfs-0.1.1/src/cdfs/contentsfile/sqlite/basetable.py
+-rw-r--r--   0        0        0      714 2023-06-29 20:52:36.574898 cdfs-0.1.1/src/cdfs/contentsfile/sqlite/contenttable.py
+-rw-r--r--   0        0        0      994 2023-06-13 18:49:59.620575 cdfs-0.1.1/src/cdfs/contentsfile/timecontentsfile.py
+-rw-r--r--   0        0        0      500 2023-06-30 19:20:48.899381 cdfs-0.1.1/src/cdfs/header.py
+-rw-r--r--   0        0        0        0 2023-01-05 21:55:12.930593 cdfs-0.1.1/src/cdfs/py.typed
+-rw-r--r--   0        0        0      234 2023-06-13 18:49:59.632575 cdfs-0.1.1/src/cdfs/structureobjects/__init__.py
+-rw-r--r--   0        0        0     7073 2023-06-29 23:53:21.236169 cdfs-0.1.1/src/cdfs/structureobjects/cdfs.py
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cdfs-0.1.1/PKG-INFO
```

### Comparing `cdfs-0.1.0/LICENSE.rst` & `cdfs-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/README.rst` & `cdfs-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/pyproject.toml` & `cdfs-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdfs"
-version = "0.1.0"
+version = "0.1.1"
 description = "Continous Data File System"
 authors = ["Anthony Fong <FongAnthonyM@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/fongant/python-cdfs"
 repository = "https://github.com/fongant/python-cdfs"
 documentation = "https://python-cdfs.readthedocs.io"
@@ -18,17 +18,17 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/fongant/python-cdfs/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.0.3"
 dspobjects = "^0.2.0"
-framestructure = "^0.4.0"
+framestructure = "^0.4.1"
 h5py = "^3.8.0"
-hdf5objects = "^0.3.0"
+hdf5objects = "^0.3.1"
 numpy = "^1.24.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 coverage = {extras = ["toml"], version = "^6.3"}
 safety = "^1.10.3"
 mypy = "^0.910"
```

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/__init__.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/__init__.py`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/contentdatasetcomponent.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/contentdatasetcomponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,20 +190,19 @@
     def set_min_shapes_dataset(self, object_: HDF5Dataset | h5py.Dataset | h5py.Reference | None) -> None:
         self.region_references.set_object_reference(object_=object_, ref_name=self.mins_name)
 
     def set_max_shapes_dataset(self, object_: HDF5Dataset | h5py.Dataset | h5py.Reference | None) -> None:
         self.region_references.set_object_reference(object_=object_, ref_name=self.maxs_name)
 
     def get_lengths(self, ignore_zeros: bool = True) -> tuple[int, ...]:
+        min_shapes = self.min_shapes[...]
         if ignore_zeros:
-            return tuple(
-                self.min_shapes[i, a] for i, a in enumerate(self.composite["Axis"]) if self.min_shapes[i, a] > 0
-            )
+            return tuple(min_shapes[i, a] for i, a in enumerate(self.composite["Axis"]) if min_shapes[i, a] > 0)
         else:
-            return tuple(self.min_shapes[i, a] for i, a in enumerate(self.composite["Axis"]))
+            return tuple(min_shapes[i, a] for i, a in enumerate(self.composite["Axis"]))
 
     def get_length(self) -> int:
         return int(sum(self.get_lengths()))
 
     def get_min_shape(self) -> tuple[int, ...]:
         min_shape = list(self.min_shapes.components["shapes"].get_min_shape(ignore_zeros=True))
         min_shape[0] = self.get_length()  # Add a way to select main axis which the data is append along
```

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/contentgroupcomponent.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/contentgroupcomponent.py`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/timecontentdatasetcomponent.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/timecontentdatasetcomponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,14 +381,15 @@
                 start=start,
                 end=end,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 sample_rate=sample_rate,
                 id_=id_,
+                **kwargs,
             )
         else:
             index, dt = self.start_axis.components["axis"].find_time_index(start, approx=True, tails=True)
 
             if dt != start:
                 self.insert_entry(
                     index=index,
@@ -397,14 +398,15 @@
                     start=start,
                     end=end,
                     axis=axis,
                     min_shape=min_shape,
                     max_shape=max_shape,
                     sample_rate=sample_rate,
                     id_=id_,
+                    **kwargs,
                 )
             else:
                 raise ValueError("Entry already exists")
 
     def update_entry(self, index: int) -> None:
         """Updates an entry to the correct information of the child.
```

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentcomponents/timecontentgroupcomponent.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentcomponents/timecontentgroupcomponent.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,14 +166,15 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
 
         if map_ is None:
             return None
         else:
             start_tz = self.node_map.components["start_times"].time_axis.time_zone
             end_tz = self.node_map.components["end_times"].time_axis.time_zone
@@ -225,14 +226,15 @@
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 id_=id_,
+                **kwargs,
             )
 
     def require_child_start(
         self,
         path: str,
         start: datetime | float | int | np.dtype,
         end: datetime | float | int | np.dtype | None = None,
@@ -263,28 +265,33 @@
             index, dt = self.node_map.components["start_times"].find_time_index(start, approx=True, tails=True)
 
             if nanostamp(dt) == start:
                 if self.child_map_type is not None:
                     return index, self.node_map.components["object_reference"].get_object(index, ref_name="node")
                 else:
                     return index, None
+            elif start < self.node_map.components["start_times"].get_nanostamp(0):
+                index = 0
+            elif start < self.node_map.components["start_times"].get_nanostamp(-1):
+                index += 1
         else:
             index = 0
 
         return index, self.create_child(
             index=index,
             path=path,
             start=start,
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
 
     def require_child_start_date(
         self,
         path: str,
         start: datetime | date | float | int | np.dtype,
         end: datetime | float | int | np.dtype | None = None,
@@ -338,14 +345,15 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
 
     # Get Child
     def get_child_start(
         self,
         start: datetime | float | int | np.dtype,
         approx: bool = False,
@@ -398,15 +406,15 @@
         elif isinstance(start, date):
             start_date = start
         else:
             start_date = Timestamp(nanostamp(start)).date()
 
         start_date = Timestamp(start_date, tz=tz)
         try:
-            index, dt = self.node_map.components["start_times"].find_time_index(start_date, approx=True, tails=True)
+            index, dt = self.node_map.components["start_times"].find_day_index(start_date, approx=True, tails=True)
 
             if dt.date() == start_date.date():
                 return index, self.node_map.components["object_reference"].get_object(index, ref_name="node")
             else:
                 raise IndexError("Date outside of range.")
         except IndexError as e:
             if default is not SENTINEL:
@@ -537,14 +545,15 @@
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 min_shape=child_node_component.min_shape,
@@ -558,14 +567,15 @@
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
     def set_recursive_entry_start(
         self,
         paths: Iterable[str],
         start: datetime | float | int | np.dtype,
         end: datetime | float | int | np.dtype | None = None,
@@ -607,14 +617,15 @@
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 sample_rate=child_node_component.sample_rate,
@@ -628,14 +639,15 @@
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
     def set_recursive_entry_start_date(
         self,
         paths: Iterable[str],
         start: datetime | float | int | np.dtype,
         end: datetime | float | int | np.dtype | None = None,
@@ -677,14 +689,15 @@
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 sample_rate=child_node_component.sample_rate,
@@ -698,14 +711,15 @@
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
     # Entry Appending
     def append_recursive_entry_index(
         self,
         indices: Iterable[int],
         paths: Iterable[str],
@@ -752,28 +766,30 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
         if paths:
             child_node_component = child.components[self.child_component_name]
             child_node_component.append_recursive_entry(
                 indices=indices,
                 paths=paths,
                 start=start,
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 sample_rate=child_node_component.sample_rate,
@@ -821,27 +837,29 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
         if paths:
             child_node_component = child.components[self.child_component_name]
             child_node_component.append_recursive_entry(
                 paths=paths,
                 start=start,
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 sample_rate=child_node_component.sample_rate,
@@ -889,27 +907,29 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
         if paths:
             child_node_component = child.components[self.child_component_name]
             child_node_component.append_recursive_entry(
                 paths=paths,
                 start=start,
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 sample_rate=child_node_component.sample_rate,
@@ -965,27 +985,29 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
         if paths:
             child_node_component = child.components[self.child_component_name]
             child_node_component.insert_recursive_entry(
                 paths=paths,
                 start=start,
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 min_shape=child_node_component.min_shape,
@@ -1033,27 +1055,29 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
         if paths:
             child_node_component = child.components[self.child_component_name]
             child_node_component.insert_recursive_entry(
                 paths=paths,
                 start=start,
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 sample_rate=child_node_component.sample_rate,
@@ -1101,27 +1125,29 @@
             end=end,
             sample_rate=sample_rate,
             map_=map_,
             axis=axis,
             min_shape=min_shape,
             max_shape=max_shape,
             id_=id_,
+            **kwargs,
         )
         if paths:
             child_node_component = child.components[self.child_component_name]
             child_node_component.insert_recursive_entry(
                 paths=paths,
                 start=start,
                 end=end,
                 sample_rate=sample_rate,
                 map_=map_,
                 axis=axis,
                 min_shape=min_shape,
                 max_shape=max_shape,
                 ids=ids,
+                **kwargs,
             )
 
             self.node_map.components[self.node_component_name].set_entry(
                 index=index,
                 start=child_node_component.get_start_datetime(),
                 end=child_node_component.get_end_datetime(),
                 sample_rate=child_node_component.sample_rate,
```

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentframes/timecontentframe.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentframes/timecontentframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # Construction/Destruction
     def __init__(
         self,
         path: pathlib.Path | str | None = None,
         content_map: HDF5Group | None = None,
         frames: Iterable[DirectoryTimeFrameInterface] | None = None,
         mode: str = "r",
-        update: bool = False,
+        update: bool = True,
         open_: bool = False,
         build: bool = True,
         init: bool = True,
         **kwargs: Any,
     ) -> None:
         # New Attributes #
         self.content_map: HDF5Dataset | None = None
@@ -127,15 +127,15 @@
     # Constructors/Destructors
     def construct(
         self,
         path: pathlib.Path | str | None = None,
         content_map: HDF5Group | None = None,
         frames: Iterable[DirectoryTimeFrameInterface] | None = None,
         mode: str = "r",
-        update: bool = False,
+        update: bool = True,
         open_: bool = False,
         build: bool = False,
         **kwargs: Any,
     ) -> None:
         """Constructs this object.
 
         Args:
@@ -156,48 +156,42 @@
     def construct_leaf_frames(self, open_=False, **kwargs) -> None:
         """Constructs the frames for this object when they are leaves.
 
         Args:
             open_: Determines if the frames will remain open after construction.
             **kwargs: The keyword arguments to create contained frames.
         """
-        for i, frame_info in enumerate(self.content_map.components["tree_node"].node_map.get_item_dicts_iter()):
-            path = self.path / frame_info["Path"]
+        for i, frame_info in enumerate(self.content_map.components["tree_node"].node_map[...]):
+            path = self.path / frame_info["Path"].decode()
             if path not in self.frame_paths:
                 if path.is_file():
                     self.frame_paths.add(path)
                     self.valid_indices.append(i)
-                    self.frames.append(
-                        self.frame_type(
-                            path,
-                            open_=open_,
-                            **kwargs,
-                        )
-                    )
+                    self.frames.append(self.frame_type(path, open_=open_, **kwargs))
                 else:
                     warn(f"{path} is missing")
         self.clear_caches()
 
     def construct_node_frames(self, open_=False, **kwargs) -> None:
         """Constructs the frames for this object when they are nodes.
 
         Args:
             open_: Determines if the frames will remain open after construction.
             **kwargs: The keyword arguments to create contained frames.
         """
-        for i, frame_info in enumerate(self.content_map.components["tree_node"].node_map.get_item_dicts_iter()):
-            path = self.path / frame_info["Path"]
-            group = self.content_map.file[frame_info["Node"]]
-            if path.is_dir() or path.is_file():
-                if path not in self.frame_paths:
-                    self.frame_paths.add(path)
-                    self.valid_indices.append(i)
-                    self.frames.append(self.node_frame_type(path=path, content_map=group, open_=open_, **kwargs))
-                else:
-                    self.frames[i].update_frames()
+        for i, frame_info in enumerate(self.content_map.components["tree_node"].node_map[...]):
+            path = self.path / frame_info["Path"].decode()
+            if path in self.frame_paths:
+                self.frames[i].update_frames()
+            elif path.exists():
+                self.frame_paths.add(path)
+                self.valid_indices.append(i)
+                group = self.content_map.file[frame_info["Node"]]
+                self.frames.append(self.node_frame_type(path=path, content_map=group, open_=open_, **kwargs))
+
         self.clear_caches()
 
     def construct_frames(self, open_=False, **kwargs) -> None:
         """Constructs the frames for this object.
 
         Args:
             open_: Determines if the frames will remain open after construction.
@@ -207,155 +201,156 @@
         self.valid_indices.clear()
         self.frames.clear()
         if self.content_map.attributes["tree_type"] == "Node":
             self.construct_node_frames(open_=open_, **kwargs)
         else:
             self.construct_leaf_frames(open_=open_, **kwargs)
 
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def update_frames(self, open_=False, **kwargs) -> None:
         """Updates the frames for this object.
 
         Args:
             open_: Determines if the frames will remain open after the update.
             **kwargs: The keyword arguments to create contained frames.
         """
         if self.content_map.attributes["tree_type"] == "Node":
             self.construct_node_frames(open_=open_, **kwargs)
         else:
             self.construct_leaf_frames(open_=open_, **kwargs)
 
     # Getters and Setters
-    @timed_keyless_cache(lifetime=1.0, call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_min_shape(self, **kwargs) -> tuple[int]:
         """Get the minimum shapes from the contained frames/objects if they are different across axes.
 
         Returns:
             The minimum shapes of the contained frames/objects.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         return tuple(self.content_map.components["tree_node"].get_min_shape())
 
-    @timed_keyless_cache(lifetime=1.0, call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_max_shape(self, **kwargs) -> tuple[int]:
         """Get the maximum shapes from the contained frames/objects if they are different across axes.
 
         Returns:
             The maximum shapes of the contained frames/objects.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         return tuple(self.content_map.components["tree_node"].get_max_shape())
 
-    @timed_keyless_cache(lifetime=1.0, call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_lengths(self, **kwargs) -> tuple[int]:
         """Get the lengths of the contained frames/objects.
 
         Returns:
             All the lengths of the contained frames/objects.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         return self.content_map.components["tree_node"].get_lengths()
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_start_datetimes(self, **kwargs) -> tuple[Timestamp | None]:
         """Get the start_timestamp datetimes of all contained frames.
 
         Returns:
             All the start_timestamp datetimes.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         all_dt = self.content_map.components["tree_node"].node_map.components["start_times"].get_datetimes()
         return tuple(all_dt[i] for i in self.valid_indices)
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_start_nanostamps(self, **kwargs) -> np.ndarray:
         """Get the start_nanostamp nanostamps of all contained frames.
 
         Returns:
             All the start_nanostamp nanostamps.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         all_ns = self.content_map.components["tree_node"].node_map.components["start_times"].get_nanostamps()
         return tuple(all_ns[i] for i in self.valid_indices)
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_start_timestamps(self, **kwargs) -> np.ndarray:
         """Get the start_timestamp timestamps of all contained frames.
 
         Returns:
             All the start_timestamp timestamps.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         all_ts = self.content_map.components["tree_node"].node_map.components["start_times"].get_timestamps()
         return tuple(all_ts[i] for i in self.valid_indices)
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_end_datetimes(self, **kwargs) -> tuple[Timestamp | None]:
         """Get the end_timestamp datetimes of all contained frames.
 
         Returns:
             All the end_timestamp datetimes.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         all_dt = self.content_map.components["tree_node"].node_map.components["end_times"].get_datetimes()
         return tuple(all_dt[i] for i in self.valid_indices)
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_end_nanostamps(self, **kwargs) -> np.ndarray:
         """Get the end_nanostamp nanostamps of all contained frames.
 
         Returns:
             All the end_nanostamp nanostamps.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         all_ns = self.content_map.components["tree_node"].node_map.components["end_times"].get_nanostamps()
         return tuple(all_ns[i] for i in self.valid_indices)
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_end_timestamps(self, **kwargs) -> np.ndarray:
         """Get the end_timestamp timestamps of all contained frames.
 
         Returns:
             All the end_timestamp timestamps.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         all_ts = self.content_map.components["tree_node"].node_map.components["end_times"].get_timestamps()
         return tuple(all_ts[i] for i in self.valid_indices)
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_sample_rates(self, **kwargs) -> tuple[float]:
         """Get the sample rates of all contained frames.
 
         Returns:
             The sample rates of all contained frames.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         return tuple(
             float(self.content_map.components["tree_node"].node_map.get_field("Sample Rate")[i])
             for i in self.valid_indices
         )
 
-    @timed_keyless_cache(call_method="clearing_call", local=True)
+    @timed_keyless_cache(lifetime=0.5, call_method="clearing_call", local=True)
     def get_sample_rates_decimal(self, **kwargs) -> tuple[Decimal]:
         """Get the sample rates of all contained frames.
 
         Returns:
             The sample rates of all contained frames.
         """
         if self.content_map.file.swmr_mode:
-            self.update_frames(**kwargs)
+            self.update_frames.caching_call(**kwargs)
         return tuple(
             Decimal(self.content_map.components["tree_node"].node_map.get_field("Sample Rate")[i])
             for i in self.valid_indices
         )
 
 
 # Assign Cyclic Definitions
```

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentmaps/contentmaps.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentmaps/contentmaps.py`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentmaps/timecontentmaps.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentmaps/timecontentmaps.py`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/contentsfile.py` & `cdfs-0.1.1/src/cdfs/contentsfile/contentsfile.py`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/src/cdfs/contentsfile/timecontentsfile.py` & `cdfs-0.1.1/src/cdfs/contentsfile/timecontentsfile.py`

 * *Files identical despite different names*

### Comparing `cdfs-0.1.0/src/cdfs/structureobjects/cdfs.py` & `cdfs-0.1.1/src/cdfs/structureobjects/cdfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     # Magic Methods #
     # Construction/Destruction
     def __init__(
         self,
         path: pathlib.Path | str | None = None,
         mode: str = "r",
-        update: bool = False,
+        update: bool = True,
         open_: bool = True,
         load: bool = True,
         init: bool = True,
         **kwargs: Any,
     ) -> None:
         # New Attributes #
         self._path: pathlib.Path | None = None
@@ -138,15 +138,15 @@
 
     # Instance Methods
     # Constructors/Destructors
     def construct(
         self,
         path: pathlib.Path | str | None = None,
         mode: str = "r",
-        update: bool = False,
+        update: bool = True,
         open_: bool = False,
         load: bool = False,
         **kwargs: Any,
     ) -> None:
         """Constructs this object.
 
         Args:
```

### Comparing `cdfs-0.1.0/PKG-INFO` & `cdfs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cdfs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Continous Data File System
 Home-page: https://github.com/fongant/python-cdfs
 License: MIT
 Author: Anthony Fong
 Author-email: FongAnthonyM@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: dspobjects (>=0.2.0,<0.3.0)
-Requires-Dist: framestructure (>=0.4.0,<0.5.0)
+Requires-Dist: framestructure (>=0.4.1,<0.5.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
-Requires-Dist: hdf5objects (>=0.3.0,<0.4.0)
+Requires-Dist: hdf5objects (>=0.3.1,<0.4.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Project-URL: Changelog, https://github.com/fongant/python-cdfs/releases
 Project-URL: Documentation, https://python-cdfs.readthedocs.io
 Project-URL: Repository, https://github.com/fongant/python-cdfs
 Description-Content-Type: text/x-rst
 
 cdfs
```

