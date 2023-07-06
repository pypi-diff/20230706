# Comparing `tmp/basin3d-0.4.0.tar.gz` & `tmp/basin3d-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basin3d-0.4.0.tar", last modified: Tue Feb 14 19:57:25 2023, max compression
+gzip compressed data, was "basin3d-0.4.1.tar", last modified: Thu Jul  6 14:34:59 2023, max compression
```

## Comparing `basin3d-0.4.0.tar` & `basin3d-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.653462 basin3d-0.4.0/
--rw-r--r--   0 val        (501) staff       (20)     2500 2022-11-11 15:42:57.000000 basin3d-0.4.0/LICENSE
--rw-r--r--   0 val        (501) staff       (20)      174 2023-02-14 19:50:25.000000 basin3d-0.4.0/MANIFEST.in
--rw-r--r--   0 val        (501) staff       (20)     7682 2023-02-14 19:57:25.652909 basin3d-0.4.0/PKG-INFO
--rw-r--r--   0 val        (501) staff       (20)     3573 2023-02-14 19:50:25.000000 basin3d-0.4.0/README.md
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.624559 basin3d-0.4.0/basin3d/
--rw-r--r--   0 val        (501) staff       (20)      246 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/__init__.py
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.642137 basin3d-0.4.0/basin3d/core/
--rw-r--r--   0 val        (501) staff       (20)        0 2022-11-11 15:42:57.000000 basin3d-0.4.0/basin3d/core/__init__.py
--rw-r--r--   0 val        (501) staff       (20)     1321 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/access.py
--rw-r--r--   0 val        (501) staff       (20)    29927 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/catalog.py
--rw-r--r--   0 val        (501) staff       (20)    13765 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/connection.py
--rw-r--r--   0 val        (501) staff       (20)      411 2022-11-11 15:42:57.000000 basin3d-0.4.0/basin3d/core/logging.yaml
--rw-r--r--   0 val        (501) staff       (20)    54076 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/models.py
--rw-r--r--   0 val        (501) staff       (20)     6435 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/monitor.py
--rw-r--r--   0 val        (501) staff       (20)     6994 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/plugin.py
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.644970 basin3d-0.4.0/basin3d/core/schema/
--rw-r--r--   0 val        (501) staff       (20)        0 2022-11-11 15:42:57.000000 basin3d-0.4.0/basin3d/core/schema/__init__.py
--rw-r--r--   0 val        (501) staff       (20)     5039 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/schema/enum.py
--rw-r--r--   0 val        (501) staff       (20)     9591 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/schema/query.py
--rw-r--r--   0 val        (501) staff       (20)    16609 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/synthesis.py
--rw-r--r--   0 val        (501) staff       (20)    17603 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/translate.py
--rw-r--r--   0 val        (501) staff       (20)     1013 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/core/types.py
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.647223 basin3d-0.4.0/basin3d/data/
--rw-r--r--   0 val        (501) staff       (20)        0 2022-11-11 15:42:57.000000 basin3d-0.4.0/basin3d/data/__init__.py
--rw-r--r--   0 val        (501) staff       (20)    10064 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/data/basin3d_observed_property_vocabulary.csv
--rw-r--r--   0 val        (501) staff       (20)      522 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/monitor.py
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.651300 basin3d-0.4.0/basin3d/plugins/
--rw-r--r--   0 val        (501) staff       (20)        0 2022-11-11 15:42:57.000000 basin3d-0.4.0/basin3d/plugins/__init__.py
--rw-r--r--   0 val        (501) staff       (20)    34440 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/plugins/usgs.py
--rw-r--r--   0 val        (501) staff       (20)    66040 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/plugins/usgs_huc_codes.py
--rw-r--r--   0 val        (501) staff       (20)     5027 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/plugins/usgs_mapping.csv
--rw-r--r--   0 val        (501) staff       (20)    13934 2023-02-14 19:50:25.000000 basin3d-0.4.0/basin3d/synthesis.py
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.631213 basin3d-0.4.0/basin3d.egg-info/
--rw-r--r--   0 val        (501) staff       (20)     7682 2023-02-14 19:57:25.000000 basin3d-0.4.0/basin3d.egg-info/PKG-INFO
--rw-r--r--   0 val        (501) staff       (20)      827 2023-02-14 19:57:25.000000 basin3d-0.4.0/basin3d.egg-info/SOURCES.txt
--rw-r--r--   0 val        (501) staff       (20)        1 2023-02-14 19:57:25.000000 basin3d-0.4.0/basin3d.egg-info/dependency_links.txt
--rw-r--r--   0 val        (501) staff       (20)      226 2023-02-14 19:57:25.000000 basin3d-0.4.0/basin3d.egg-info/requires.txt
--rw-r--r--   0 val        (501) staff       (20)        8 2023-02-14 19:57:25.000000 basin3d-0.4.0/basin3d.egg-info/top_level.txt
-drwxr-xr-x   0 val        (501) staff       (20)        0 2023-02-14 19:57:25.652093 basin3d-0.4.0/docs/
--rw-r--r--   0 val        (501) staff       (20)    10554 2023-02-14 19:50:25.000000 basin3d-0.4.0/docs/conf.py
--rw-r--r--   0 val        (501) staff       (20)     2386 2023-02-14 19:50:25.000000 basin3d-0.4.0/pyproject.toml
--rw-r--r--   0 val        (501) staff       (20)       38 2023-02-14 19:57:25.653630 basin3d-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.179538 basin3d-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-06 14:34:44.000000 basin3d-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 14:34:44.000000 basin3d-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-06 14:34:59.179538 basin3d-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-06 14:34:44.000000 basin3d-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29927 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    54076 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/core/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/schema/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/schema/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16687 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/data/basin3d_observed_property_vocabulary.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34440 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66040 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/usgs_huc_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/plugins/usgs_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-07-06 14:34:44.000000 basin3d-0.4.1/basin3d/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:34:59.175538 basin3d-0.4.1/basin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 14:34:59.000000 basin3d-0.4.1/basin3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-06 14:34:44.000000 basin3d-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:34:59.179538 basin3d-0.4.1/setup.cfg
```

### Comparing `basin3d-0.4.0/LICENSE` & `basin3d-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/PKG-INFO` & `basin3d-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basin3d
-Version: 0.4.0
+Version: 0.4.1
 Summary: BASIN-3D Core Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>, Catherine Wong <catwong@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
@@ -64,14 +64,17 @@
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
+[![Python package](https://github.com/BASIN-3D/basin3d/actions/workflows/main.yml/badge.svg)](https://github.com/BASIN-3D/basin3d/actions/workflows/main.yml)
+[![Pypi](https://img.shields.io/pypi/v/basin3d)](https://pypi.org/project/basin3d/)
+
 # basin3d
 Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets. 
 
 ![basin3d](https://user-images.githubusercontent.com/20212666/112556236-ff1a9b80-8d86-11eb-9009-25b658ce41e0.png)
 
 BASIN-3D is a software ecosystem that synthesizes diverse earth science data from a variety of remote data sources on-demand, without the need for storing data in a single database. It is designed to parse, translate, and synthesize diverse observations from well-curated repositories into standardized formats for scientific uses such as analysis and visualization.
```

### Comparing `basin3d-0.4.0/README.md` & `basin3d-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![Python package](https://github.com/BASIN-3D/basin3d/actions/workflows/main.yml/badge.svg)](https://github.com/BASIN-3D/basin3d/actions/workflows/main.yml)
+[![Pypi](https://img.shields.io/pypi/v/basin3d)](https://pypi.org/project/basin3d/)
+
 # basin3d
 Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets. 
 
 ![basin3d](https://user-images.githubusercontent.com/20212666/112556236-ff1a9b80-8d86-11eb-9009-25b658ce41e0.png)
 
 BASIN-3D is a software ecosystem that synthesizes diverse earth science data from a variety of remote data sources on-demand, without the need for storing data in a single database. It is designed to parse, translate, and synthesize diverse observations from well-curated repositories into standardized formats for scientific uses such as analysis and visualization.
```

### Comparing `basin3d-0.4.0/basin3d/core/access.py` & `basin3d-0.4.1/basin3d/core/access.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/catalog.py` & `basin3d-0.4.1/basin3d/core/catalog.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/connection.py` & `basin3d-0.4.1/basin3d/core/connection.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/models.py` & `basin3d-0.4.1/basin3d/core/models.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/monitor.py` & `basin3d-0.4.1/basin3d/core/monitor.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/plugin.py` & `basin3d-0.4.1/basin3d/core/plugin.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/schema/enum.py` & `basin3d-0.4.1/basin3d/core/schema/enum.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/schema/query.py` & `basin3d-0.4.1/basin3d/core/schema/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,16 +184,16 @@
 class SynthesisResponse(BaseModel):
     """BASIN-3D Synthesis Response """
 
     query: QueryBase = Field(title="Query", description="The original query for the current response")
     data: Optional[Union[object, List[object]]] = Field(title="Data",
                                                         description="The data for the current response. Empty if provided "
                                                                     "via Iterator.")
-    messages: List[SynthesisMessage] = Field([], title="Messages",
-                                             description="The synthesis messages for this response")
+    messages: List[Optional[SynthesisMessage]] = Field([], title="Messages",
+                                                       description="The synthesis messages for this response")
 
     class Config:
         # output fields to camelcase
         alias_generator = _to_camelcase
         # whether an aliased field may be populated by its name as given by the model attribute
         #  (allows bot camelcase and underscore fields)
         allow_population_by_field_name = True
```

### Comparing `basin3d-0.4.0/basin3d/core/synthesis.py` & `basin3d-0.4.1/basin3d/core/synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """
         Initialize the generator with the query and the model access
 
         :param query: the unsynthesized query
         :param model_access: Model access
         """
 
-        self._synthesis_response = SynthesisResponse(query=query)
+        self._synthesis_response = SynthesisResponse(query=query)  # type: ignore[call-arg]
         self._model_access: 'DataSourceModelAccess' = model_access
 
         # Filter the plugins, if specified
         if not self._synthesis_response.query.datasource:
             self._plugins = list(self._model_access.plugins.values())
         elif self._synthesis_response.query.datasource:
             self._plugins = [self._model_access.plugins[d] for d in self._synthesis_response.query.datasource if
@@ -262,26 +262,26 @@
                 plugin_views = plugin.get_plugin_access()
                 monitor.set_ctx_basin3d_where([plugin.get_datasource().id, self.synthesis_model.__name__])
                 if self.synthesis_model in plugin_views:
                     synthesized_query: QueryById = query.copy()
                     synthesized_query.id = datasource_pk
                     synthesized_query.datasource = [datasource.id]
                     obj: Base = plugin_views[self.synthesis_model].get(query=synthesized_query)
-                    return SynthesisResponse(query=query, data=obj)
+                    return SynthesisResponse(query=query, data=obj)  # type: ignore[call-arg]
                 else:
                     messages.append(self.log("Plugin view does not exist",
                                              MessageLevelEnum.WARN,
                                              [plugin.get_datasource().id, self.synthesis_model.__name__],
                                              ))
 
             else:
                 messages.append(self.log(f"DataSource not not found for id {query.id}",
                                 MessageLevelEnum.ERROR))
 
-        return SynthesisResponse(query=query, messages=messages)
+        return SynthesisResponse(query=query, messages=messages)  # type: ignore[call-arg]
 
 
 class MonitoringFeatureAccess(DataSourceModelAccess):
     """
     MonitoringFeature: A feature upon which monitoring is made. OGC Timeseries Profile OM_MonitoringFeature.
 
     **Properties**
```

### Comparing `basin3d-0.4.0/basin3d/core/translate.py` & `basin3d-0.4.1/basin3d/core/translate.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/core/types.py` & `basin3d-0.4.1/basin3d/core/types.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/data/basin3d_observed_property_vocabulary.csv` & `basin3d-0.4.1/basin3d/data/basin3d_observed_property_vocabulary.csv`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/monitor.py` & `basin3d-0.4.1/basin3d/monitor.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/plugins/usgs.py` & `basin3d-0.4.1/basin3d/plugins/usgs.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/plugins/usgs_huc_codes.py` & `basin3d-0.4.1/basin3d/plugins/usgs_huc_codes.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/plugins/usgs_mapping.csv` & `basin3d-0.4.1/basin3d/plugins/usgs_mapping.csv`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d/synthesis.py` & `basin3d-0.4.1/basin3d/synthesis.py`

 * *Files identical despite different names*

### Comparing `basin3d-0.4.0/basin3d.egg-info/PKG-INFO` & `basin3d-0.4.1/basin3d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basin3d
-Version: 0.4.0
+Version: 0.4.1
 Summary: BASIN-3D Core Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>, Catherine Wong <catwong@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
@@ -64,14 +64,17 @@
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
+[![Python package](https://github.com/BASIN-3D/basin3d/actions/workflows/main.yml/badge.svg)](https://github.com/BASIN-3D/basin3d/actions/workflows/main.yml)
+[![Pypi](https://img.shields.io/pypi/v/basin3d)](https://pypi.org/project/basin3d/)
+
 # basin3d
 Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets. 
 
 ![basin3d](https://user-images.githubusercontent.com/20212666/112556236-ff1a9b80-8d86-11eb-9009-25b658ce41e0.png)
 
 BASIN-3D is a software ecosystem that synthesizes diverse earth science data from a variety of remote data sources on-demand, without the need for storing data in a single database. It is designed to parse, translate, and synthesize diverse observations from well-curated repositories into standardized formats for scientific uses such as analysis and visualization.
```

### Comparing `basin3d-0.4.0/basin3d.egg-info/SOURCES.txt` & `basin3d-0.4.1/basin3d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,8 @@
 basin3d/core/schema/enum.py
 basin3d/core/schema/query.py
 basin3d/data/__init__.py
 basin3d/data/basin3d_observed_property_vocabulary.csv
 basin3d/plugins/__init__.py
 basin3d/plugins/usgs.py
 basin3d/plugins/usgs_huc_codes.py
-basin3d/plugins/usgs_mapping.csv
-docs/conf.py
+basin3d/plugins/usgs_mapping.csv
```

### Comparing `basin3d-0.4.0/pyproject.toml` & `basin3d-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 description = "BASIN-3D Core Framework"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = '>=3.8,<3.11'
 dependencies = [
     "pyyaml>=6.0",
     "requests",
-    "pydantic",
+    "pydantic<2",
     "tinydb",
 ]
 
 
 [project.optional-dependencies]
 dev = ['pytest', 'pytest-mypy', 'pytest-cov', 'flake8',
     'types-PyYAML', 'types-chardet', 'types-cryptography', 'types-requests']
-docs = ["sphinx",
-    "sphinx-autodoc-typehints",
+docs = ["sphinx<=6.2.1",
+    "sphinx-autodoc-typehints<=1.23.0",
     "graphviz",
     "sphinx_rtd_theme",
     "tomli",
     "myst-parser"]
 
 [project.urls]
 homepage = "https://github.com/BASIN-3D/basin3d"
```

