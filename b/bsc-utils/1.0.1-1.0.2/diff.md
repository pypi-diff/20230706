# Comparing `tmp/bsc_utils-1.0.1.tar.gz` & `tmp/bsc_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsc_utils-1.0.1.tar", last modified: Mon Jun  5 06:44:39 2023, max compression
+gzip compressed data, was "bsc_utils-1.0.2.tar", last modified: Thu Jul  6 08:54:12 2023, max compression
```

## Comparing `bsc_utils-1.0.1.tar` & `bsc_utils-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 06:44:39.296527 bsc_utils-1.0.1/
--rw-rw-rw-   0        0        0       26 2023-05-15 03:09:29.000000 bsc_utils-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      547 2023-06-05 06:44:39.291513 bsc_utils-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-15 02:48:57.000000 bsc_utils-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 06:44:39.202776 bsc_utils-1.0.1/bsc_utils/
--rw-rw-rw-   0        0        0       21 2023-06-05 06:41:30.000000 bsc_utils-1.0.1/bsc_utils/__init__.py
--rw-rw-rw-   0        0        0      402 2023-05-12 03:53:41.000000 bsc_utils-1.0.1/bsc_utils/config.py
--rw-rw-rw-   0        0        0     2240 2023-06-01 09:15:36.000000 bsc_utils-1.0.1/bsc_utils/database.py
--rw-rw-rw-   0        0        0       44 2023-05-12 08:32:56.000000 bsc_utils-1.0.1/bsc_utils/exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-05 06:40:42.000000 bsc_utils-1.0.1/bsc_utils/helpers.py
--rw-rw-rw-   0        0        0     2171 2023-06-05 06:40:42.000000 bsc_utils-1.0.1/bsc_utils/visual.py
-drwxrwxrwx   0        0        0        0 2023-06-05 06:44:39.281988 bsc_utils-1.0.1/bsc_utils.egg-info/
--rw-rw-rw-   0        0        0      547 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 06:44:38.000000 bsc_utils-1.0.1/bsc_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-06-05 06:40:42.000000 bsc_utils-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 06:44:39.297029 bsc_utils-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-05-15 03:04:43.000000 bsc_utils-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:54:12.517596 bsc_utils-1.0.2/
+-rw-rw-rw-   0        0        0       26 2023-05-15 03:09:29.000000 bsc_utils-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      547 2023-07-06 08:54:12.516593 bsc_utils-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-15 02:48:57.000000 bsc_utils-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 08:54:12.503723 bsc_utils-1.0.2/bsc_utils/
+-rw-rw-rw-   0        0        0       21 2023-07-06 08:51:57.000000 bsc_utils-1.0.2/bsc_utils/__init__.py
+-rw-rw-rw-   0        0        0      544 2023-07-06 08:42:23.000000 bsc_utils-1.0.2/bsc_utils/_config.py
+-rw-rw-rw-   0        0        0      505 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/_helpers.py
+-rw-rw-rw-   0        0        0      788 2023-06-21 09:27:42.000000 bsc_utils-1.0.2/bsc_utils/chat.py
+-rw-rw-rw-   0        0        0     1097 2023-07-06 08:42:23.000000 bsc_utils-1.0.2/bsc_utils/crawl.py
+-rw-rw-rw-   0        0        0     2688 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/database.py
+-rw-rw-rw-   0        0        0      231 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/exceptions.py
+-rw-rw-rw-   0        0        0     2073 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/time.py
+-rw-rw-rw-   0        0        0     2700 2023-06-08 01:45:46.000000 bsc_utils-1.0.2/bsc_utils/visual.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:54:12.513586 bsc_utils-1.0.2/bsc_utils.egg-info/
+-rw-rw-rw-   0        0        0      547 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      160 2023-06-21 09:27:42.000000 bsc_utils-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 08:54:12.519602 bsc_utils-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2023-05-15 03:04:43.000000 bsc_utils-1.0.2/setup.py
```

### Comparing `bsc_utils-1.0.1/PKG-INFO` & `bsc_utils-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsc_utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Util Functions for BSC Quants
 Home-page: https://github.com/dang-trung/bsc-utils
 Author: Trung Dang
 Author-email: trungd@bsc.com.vn
 Maintainer: Trung Dang
 Maintainer-email: trungd@bsc.com.vn
 License: MIT
```

### Comparing `bsc_utils-1.0.1/bsc_utils/database.py` & `bsc_utils-1.0.2/bsc_utils/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from enum import Enum
 from typing import Union
 
 import sqlite3
 import oracledb
 import pandas as pd
 import pymssql
+import pyodbc
 
-import bsc_utils.config as config
-from bsc_utils.helpers import dict_factory
-from bsc_utils.exceptions import NotDatabaseError
+from . import _config as config
+from ._helpers import dict_factory
+from .exceptions import NotDatabaseError
 
 
 class Database(Enum):
     MSSQL = 'mssql'
     ORACLE = 'oracle'
     SQLITE = 'sqlite'
+    ACCESS = 'access'
 
 
 def connect(database: Database):
     if not isinstance(database, Database):
         raise NotDatabaseError('Must be a database.Database instance.')
 
     if database == Database.MSSQL:
@@ -33,49 +35,64 @@
             user=config.oracle_user,
             password=config.oracle_password,
             dsn=config.oracle_dsn
         )
     elif database == Database.SQLITE:
         return sqlite3.connect(database=config.sqlite_path)
 
+    elif database == Database.ACCESS:
+        return pyodbc.connect(
+            f'''
+            Driver={{Microsoft Access Driver (*.mdb, *.accdb)}};
+            DBQ={config.access_path};
+            '''
+        )
+
 
 def query(
     database: Database,
     query: str,
     params: Union[list, tuple] = None,
     fetch: bool = True,
     as_df: bool = True,
     index_col: str = None
 ) -> Union[list, pd.DataFrame]:
     con = connect(database)
     if database == Database.MSSQL:
         cur = con.cursor(as_dict=True)
 
-    if database == Database.SQLITE:
+    elif database == Database.SQLITE:
         con.row_factory = dict_factory
         cur = con.cursor()
 
-    if database == Database.ORACLE:
+    elif database == Database.ORACLE or database == Database.ACCESS:
         cur = con.cursor()
 
     cur.execute(query) if params is None else (
         cur.executemany(query, params)
         if isinstance(params, list) else cur.execute(query, params)
     )
 
     if database == Database.ORACLE:
         cols = [col[0] for col in cur.description]
         cur.rowfactory = lambda *args: dict(zip(cols, args))
 
     obj = None
     if fetch:
         obj = cur.fetchall()
+
+        if database == Database.ACCESS:
+            obj = [
+                dict(zip([col[0] for col in cur.description], row))
+                for row in obj
+            ]
+
         if as_df:
             obj = make_tabular(obj, index_col)
-            
+
     con.commit()
     con.close()
 
     return obj
 
 
 def make_tabular(obj: list[dict], index_col: str) -> pd.DataFrame:
```

### Comparing `bsc_utils-1.0.1/bsc_utils/visual.py` & `bsc_utils-1.0.2/bsc_utils/visual.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-import numpy as np
+import pandas as pd
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from bsc_utils.helpers import row_ratio
+from ._helpers import row_ratio
 
 
-def plotly(subplots: dict, **layout_kwargs) -> go.Figure:
+def plotly(
+    subplots: dict,
+    shared_xaxis: bool = True,
+    fill_gap: bool = True,
+    **layout_kwargs
+) -> go.Figure:
 
     no_subplots = len(subplots)
 
     fig = make_subplots(
         rows=no_subplots,
         cols=1,
-        shared_xaxes=True,
+        shared_xaxes=shared_xaxis,
         row_heights=row_ratio(no_subplots),
         vertical_spacing=0.25 / no_subplots,
         subplot_titles=list(subplots.keys()),
         specs=[[{
             'secondary_y': True
         }] for _ in subplots]
     )
@@ -29,25 +34,25 @@
                     for k, v in trace.items()
                     if k not in ['secondary_y', 'range', 'showticklabels']
                 },
                 secondary_y=trace.get('secondary_y', False),
                 row=(row_id + 1),
                 col=1,
             )
-            if trace.get('range'):
-                if not trace.get('secondary_y'):
-                    fig['layout'][f'yaxis{row_id * 2 + 1}'].update(
-                        range=trace.get('range'), side='right'
-                    )
-                else:
-                    fig['layout'][f'yaxis{row_id * 2 + 2}'].update(
-                        range=trace.get('range'),
-                        showticklabels=trace.get('showticklabels'),
-                        side='right'
-                    )
+
+            if not trace.get('secondary_y'):
+                fig['layout'][f'yaxis{row_id * 2 + 1}'].update(
+                    range=trace.get('range'), side='right'
+                )
+            else:
+                fig['layout'][f'yaxis{row_id * 2 + 2}'].update(
+                    range=trace.get('range'),
+                    showticklabels=trace.get('showticklabels'),
+                    side='right'
+                )
 
     fig.update_traces(
         xaxis=f'x{no_subplots}',
         xhoverformat='%a %d %b %Y',
     )
     fig.update_xaxes(
         showgrid=False,
@@ -67,8 +72,20 @@
     fig.update_layout(
         showlegend=True,
         autosize=True,
         font_family='Rockwell',
         hovermode='x unified',
         **layout_kwargs
     )
+    if shared_xaxis and fill_gap:
+        shared_x = trace.get('x')
+        if shared_x.dtype.kind == 'M':  # datetime type
+            avb_days = [d.to_pydatetime() for d in shared_x]
+            all_days = [
+                d.to_pydatetime() for d in pd.date_range(
+                    start=avb_days[0], end=avb_days[-1], freq=shared_x.freq
+                )
+            ]
+            non_avb_days = [d for d in all_days if d not in avb_days]
+            fig.update_xaxes(rangebreaks=[dict(values=non_avb_days)])
+
     return fig
```

### Comparing `bsc_utils-1.0.1/bsc_utils.egg-info/PKG-INFO` & `bsc_utils-1.0.2/bsc_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsc-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Util Functions for BSC Quants
 Home-page: https://github.com/dang-trung/bsc-utils
 Author: Trung Dang
 Author-email: trungd@bsc.com.vn
 Maintainer: Trung Dang
 Maintainer-email: trungd@bsc.com.vn
 License: MIT
```

### Comparing `bsc_utils-1.0.1/setup.py` & `bsc_utils-1.0.2/setup.py`

 * *Files identical despite different names*

