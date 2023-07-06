# Comparing `tmp/a_pandas_ex_excel_edit-0.1.tar.gz` & `tmp/a_pandas_ex_excel_edit-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_excel_edit-0.1.tar", last modified: Thu Oct  6 22:33:19 2022, max compression
+gzip compressed data, was "a_pandas_ex_excel_edit-0.11.tar", last modified: Thu Jul  6 00:06:36 2023, max compression
```

## Comparing `a_pandas_ex_excel_edit-0.1.tar` & `a_pandas_ex_excel_edit-0.11.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-10-06 22:33:19.764662 a_pandas_ex_excel_edit-0.1/
--rw-rw-rw-   0        0        0     1148 2022-10-06 22:33:14.000000 a_pandas_ex_excel_edit-0.1/LICENSE.rst
--rw-rw-rw-   0        0        0      177 2022-10-06 22:33:13.000000 a_pandas_ex_excel_edit-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5593 2022-10-06 22:33:19.764662 a_pandas_ex_excel_edit-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4518 2022-10-06 22:30:48.000000 a_pandas_ex_excel_edit-0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-10-06 22:33:19.760691 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/LICENSE
--rw-rw-rw-   0        0        0     4518 2022-10-06 22:30:48.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/README.MD
--rw-rw-rw-   0        0        0     6343 2022-10-06 22:25:42.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/__init__.py
--rw-rw-rw-   0        0        0        6 2022-10-06 22:33:18.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/requirements.txt
--rw-rw-rw-   0        0        0        2 2022-10-06 22:33:18.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/thirdparty.json
-drwxrwxrwx   0        0        0        0 2022-10-06 22:33:19.764662 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit.egg-info/
--rw-rw-rw-   0        0        0     5593 2022-10-06 22:33:19.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2022-10-06 22:33:19.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-06 22:33:19.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-10-06 22:33:19.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2022-10-06 22:33:19.000000 a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-10-06 22:33:19.764662 a_pandas_ex_excel_edit-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1467 2022-10-06 22:33:18.000000 a_pandas_ex_excel_edit-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:06:36.364638 a_pandas_ex_excel_edit-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-06 00:06:30.000000 a_pandas_ex_excel_edit-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      137 2023-07-06 00:06:28.000000 a_pandas_ex_excel_edit-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     5223 2023-07-06 00:06:36.364638 a_pandas_ex_excel_edit-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     4518 2023-04-15 00:18:30.000000 a_pandas_ex_excel_edit-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 00:06:36.360629 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit/
+-rw-rw-rw-   0        0        0     4518 2023-04-15 00:18:30.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit/README.MD
+-rw-rw-rw-   0        0        0     6704 2023-07-06 00:05:09.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-07-06 00:06:35.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit/requirements.txt
+-rw-rw-rw-   0        0        0     1746 2023-07-06 00:06:35.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-06 00:06:36.363651 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit.egg-info/
+-rw-rw-rw-   0        0        0     5223 2023-07-06 00:06:36.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-07-06 00:06:36.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 00:06:36.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 00:06:36.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-06 00:06:36.000000 a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-06 00:06:36.364638 a_pandas_ex_excel_edit-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1368 2023-07-06 00:06:35.000000 a_pandas_ex_excel_edit-0.11/setup.py
```

### Comparing `a_pandas_ex_excel_edit-0.1/LICENSE.rst` & `a_pandas_ex_excel_edit-0.11/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2022 Johannes Fischer
+ Copyright (c) 2023 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `a_pandas_ex_excel_edit-0.1/PKG-INFO` & `a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,124 @@
 Metadata-Version: 2.1
-Name: a_pandas_ex_excel_edit
-Version: 0.1
+Name: a-pandas-ex-excel-edit
+Version: 0.11
 Summary: If you have to change a lot of arbitrary values which don't have a clear pattern, use Excel!
 Home-page: https://github.com/hansalemaos/a_pandas_ex_excel_edit
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,excel,MS Excel,quick,edit
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
-## Quickly edit Pandas DataFrames and Series in Excel
-
-Use this methods to quickly edit your DataFrame with MS Excel.  
-Of course, Pandas is a lot better than Excel, but if you have to change a lot of  arbitrary values which don't have a clear pattern,  a GUI is imho the best choice.
-
-```python
-pip install a-pandas-ex-excel-edit 
-```
-
-```python
-    #Here is an example:
-
-    import pandas as pd
-    from a_pandas_ex_excel_edit import pd_add_excel_editor    
-
-    #pd_add_excel_editor will add 2 new methods:  
-    #pandas.Series.s_edit_in_excel
-    #pandas.DataFrame.d_edit_in_excel
-    pd_add_excel_editor()   
-
-    dframe = pd.read_csv("https://raw.githubusercontent.com/pandas-dev/pandas/main/doc/data/titanic.csv")
-    #Let's add a row with lists, a tough data type to handle
-    dframe['list_in_columns'] = [[[1]*10]] * len(dframe)   
-
-         PassengerId  Survived  ...  Embarked                   list_in_columns
-0              1         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-1              2         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-2              3         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-3              4         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-4              5         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-..           ...       ...  ...       ...                               ...
-886          887         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-887          888         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-888          889         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-889          890         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-890          891         0  ...         Q  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-[891 rows x 13 columns]   
-
-dframe.dtypes
-Out[6]: 
-PassengerId          int64
-Survived             int64
-Pclass               int64
-Name                object
-Sex                 object
-Age                float64
-SibSp                int64
-Parch                int64
-Ticket              object
-Fare               float64
-Cabin               object
-Embarked            object
-list_in_columns     object
-dtype: object    
-
-df = dframe.d_edit_in_excel() #DataFrames   
-
-Out[7]: 
-     PassengerId  Survived  ...  Embarked                       list_in_columns
-0          10001      9999  ...   NOT YET  [[1, 99999, 1, 1, 1, 1, 1, 1, 1, 1]]
-1          10000         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-2           9999         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-3           9998         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-4           9997         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-..           ...       ...  ...       ...                                   ...
-886          887         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-887          888         1  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-888          889         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-889          890         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-890          891         0  ...         Q      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-[891 rows x 13 columns]
-
-   df.dtypes
-Out[9]: 
-PassengerId          uint16
-Survived             uint16
-Pclass                uint8
-Name                 string
-Sex                category
-Age                  object
-SibSp                 uint8
-Parch                 uint8
-Ticket               object
-Fare                float64
-Cabin              category
-Embarked           category
-list_in_columns      object #you can even edit lists, dicts and tuples with Excel!
-dtype: object    
-
-df2 = dframe.Name.s_edit_in_excel() #Series
-
-df2
-Out[8]: 
-0                                        HANNIBAL LECTOR
-1      Cumings, Mrs. John Bradley (Florence Briggs Th...
-2                                 Heikkinen, Miss. Laina
-3           Futrelle, Mrs. Jacques Heath (Lily May Peel)
-4                               Allen, Mr. William Henry
-                             ...                        
-886                                Montvila, Rev. Juozas
-887                         Graham, Miss. Margaret Edith
-888             Johnston, Miss. Catherine Helen "Carrie"
-889                                Behr, Mr. Karl Howell
-890                                  Dooley, Mr. Patrick
-Name: Name, Length: 891, dtype: string    
-```
+## Quickly edit Pandas DataFrames and Series in Excel
+
+Use this methods to quickly edit your DataFrame with MS Excel.  
+Of course, Pandas is a lot better than Excel, but if you have to change a lot of  arbitrary values which don't have a clear pattern,  a GUI is imho the best choice.
+
+```python
+pip install a-pandas-ex-excel-edit 
+```
+
+```python
+    #Here is an example:
+
+    import pandas as pd
+    from a_pandas_ex_excel_edit import pd_add_excel_editor    
+
+    #pd_add_excel_editor will add 2 new methods:  
+    #pandas.Series.s_edit_in_excel
+    #pandas.DataFrame.d_edit_in_excel
+    pd_add_excel_editor()   
+
+    dframe = pd.read_csv("https://raw.githubusercontent.com/pandas-dev/pandas/main/doc/data/titanic.csv")
+    #Let's add a row with lists, a tough data type to handle
+    dframe['list_in_columns'] = [[[1]*10]] * len(dframe)   
+
+         PassengerId  Survived  ...  Embarked                   list_in_columns
+0              1         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+1              2         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+2              3         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+3              4         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+4              5         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+..           ...       ...  ...       ...                               ...
+886          887         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+887          888         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+888          889         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+889          890         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+890          891         0  ...         Q  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+[891 rows x 13 columns]   
+
+dframe.dtypes
+Out[6]: 
+PassengerId          int64
+Survived             int64
+Pclass               int64
+Name                object
+Sex                 object
+Age                float64
+SibSp                int64
+Parch                int64
+Ticket              object
+Fare               float64
+Cabin               object
+Embarked            object
+list_in_columns     object
+dtype: object    
+
+df = dframe.d_edit_in_excel() #DataFrames   
+
+Out[7]: 
+     PassengerId  Survived  ...  Embarked                       list_in_columns
+0          10001      9999  ...   NOT YET  [[1, 99999, 1, 1, 1, 1, 1, 1, 1, 1]]
+1          10000         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+2           9999         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+3           9998         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+4           9997         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+..           ...       ...  ...       ...                                   ...
+886          887         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+887          888         1  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+888          889         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+889          890         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+890          891         0  ...         Q      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+[891 rows x 13 columns]
+
+   df.dtypes
+Out[9]: 
+PassengerId          uint16
+Survived             uint16
+Pclass                uint8
+Name                 string
+Sex                category
+Age                  object
+SibSp                 uint8
+Parch                 uint8
+Ticket               object
+Fare                float64
+Cabin              category
+Embarked           category
+list_in_columns      object #you can even edit lists, dicts and tuples with Excel!
+dtype: object    
+
+df2 = dframe.Name.s_edit_in_excel() #Series
+
+df2
+Out[8]: 
+0                                        HANNIBAL LECTOR
+1      Cumings, Mrs. John Bradley (Florence Briggs Th...
+2                                 Heikkinen, Miss. Laina
+3           Futrelle, Mrs. Jacques Heath (Lily May Peel)
+4                               Allen, Mr. William Henry
+                             ...                        
+886                                Montvila, Rev. Juozas
+887                         Graham, Miss. Margaret Edith
+888             Johnston, Miss. Catherine Helen "Carrie"
+889                                Behr, Mr. Karl Howell
+890                                  Dooley, Mr. Patrick
+Name: Name, Length: 891, dtype: string    
+```
```

### Comparing `a_pandas_ex_excel_edit-0.1/README.md` & `a_pandas_ex_excel_edit-0.11/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/README.MD` & `a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit/README.MD`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit/__init__.py` & `a_pandas_ex_excel_edit-0.11/a_pandas_ex_excel_edit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
+from time import sleep
 from typing import Union
-from pandas.core.frame import DataFrame, Series
 
-from a_stringdf_2_types import convert_stringdf_to_df
-from tempfile import TemporaryDirectory
 import pandas as pd
+from pandas.core.frame import DataFrame, Series
+from tempfile import NamedTemporaryFile
 
 
 def series_to_dataframe(
-    df: Union[pd.Series, pd.DataFrame]
+        df: Union[pd.Series, pd.DataFrame]
 ) -> (Union[pd.Series, pd.DataFrame], bool):
     dataf = df.copy()
     isseries = False
     if isinstance(dataf, pd.Series):
         columnname = dataf.name
         dataf = dataf.to_frame()
 
@@ -22,17 +22,22 @@
             dataf.index = [columnname]
             dataf = dataf.T
         isseries = True
 
     return dataf, isseries
 
 
-def edit_pandas_with_excel(
-    dframe: Union[pd.Series, pd.DataFrame]
-) -> Union[pd.Series, pd.DataFrame]:
+def get_tmpfile(suffix=".xlsx"):
+    tfp = NamedTemporaryFile(delete=False, suffix=suffix)
+    filename = tfp.name
+    tfp.close()
+    return filename
+
+
+def edit_pandas_with_excel(dframe, sleeptime=3):
     """
     Use this function to quick edit your DataFrame with MS Excel.
     Of course, Pandas is a lot better than Excel, but if you have to change arbitrary values which don't have a clear pattern,
     a GUI is imho the best choice.
 
     #Here is an example:
 
@@ -133,26 +138,40 @@
         Parameters:
             dframe: Union[pd.Series, pd.DataFrame]
         Returns:
             Union[pd.Series, pd.DataFrame]
 
     """
     df, isseries = series_to_dataframe(dframe)
-    tmp = TemporaryDirectory()
-    exceltemp = os.path.join(tmp.name, "tmpexcel.xlsx")
-    dfcolumns = df.columns.to_list()
-    df.to_excel(exceltemp)
-    os.system(f"CALL {exceltemp}")
-    dfnew = pd.read_excel(exceltemp)
-    indexcol = [x for x in dfnew.columns if x not in dfcolumns and ": " in x]
-    dfnewoldindex = dfnew[indexcol[0]].__array__().copy()
-    dfnew = dfnew.drop(columns=indexcol[0])
-    dfnew.index = dfnewoldindex.copy()
-    dfnew = convert_stringdf_to_df(dfnew)
+    tmpfile = get_tmpfile(suffix=".xlsx")
+    df.to_excel(tmpfile, index=True, index_label=df.index.to_list(), na_rep='<NA>')
+    os.startfile(tmpfile)
+    sleep(sleeptime)
+    while True:
+        try:
+            os.rename(tmpfile, tmpfile)
+            sleep(sleeptime)
+            break
+        except OSError:
+            sleep(sleeptime)
+            continue
+    try:
+        df2 = pd.read_excel(tmpfile, index_col=0, dtype=df.dtypes.to_dict())
+    except Exception:
+        df2 = pd.read_excel(tmpfile, index_col=0)
+        for key, item in df.dtypes.to_dict().items():
+            try:
+                df2[key] = df2[key].astype(item)
+            except Exception:
+                continue
     if isseries:
-        dfnew = dfnew[dfnew.columns[0]]
-    return dfnew
+        df2 = df2[df2.columns[0]]
+    try:
+        os.remove(tmpfile)
+    except Exception:
+        pass
+    return df2
 
 
 def pd_add_excel_editor():
     DataFrame.d_edit_in_excel = edit_pandas_with_excel
     Series.s_edit_in_excel = edit_pandas_with_excel
```

### Comparing `a_pandas_ex_excel_edit-0.1/a_pandas_ex_excel_edit.egg-info/PKG-INFO` & `a_pandas_ex_excel_edit-0.11/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,124 @@
 Metadata-Version: 2.1
-Name: a-pandas-ex-excel-edit
-Version: 0.1
+Name: a_pandas_ex_excel_edit
+Version: 0.11
 Summary: If you have to change a lot of arbitrary values which don't have a clear pattern, use Excel!
 Home-page: https://github.com/hansalemaos/a_pandas_ex_excel_edit
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,excel,MS Excel,quick,edit
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
-## Quickly edit Pandas DataFrames and Series in Excel
-
-Use this methods to quickly edit your DataFrame with MS Excel.  
-Of course, Pandas is a lot better than Excel, but if you have to change a lot of  arbitrary values which don't have a clear pattern,  a GUI is imho the best choice.
-
-```python
-pip install a-pandas-ex-excel-edit 
-```
-
-```python
-    #Here is an example:
-
-    import pandas as pd
-    from a_pandas_ex_excel_edit import pd_add_excel_editor    
-
-    #pd_add_excel_editor will add 2 new methods:  
-    #pandas.Series.s_edit_in_excel
-    #pandas.DataFrame.d_edit_in_excel
-    pd_add_excel_editor()   
-
-    dframe = pd.read_csv("https://raw.githubusercontent.com/pandas-dev/pandas/main/doc/data/titanic.csv")
-    #Let's add a row with lists, a tough data type to handle
-    dframe['list_in_columns'] = [[[1]*10]] * len(dframe)   
-
-         PassengerId  Survived  ...  Embarked                   list_in_columns
-0              1         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-1              2         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-2              3         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-3              4         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-4              5         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-..           ...       ...  ...       ...                               ...
-886          887         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-887          888         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-888          889         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-889          890         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-890          891         0  ...         Q  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-[891 rows x 13 columns]   
-
-dframe.dtypes
-Out[6]: 
-PassengerId          int64
-Survived             int64
-Pclass               int64
-Name                object
-Sex                 object
-Age                float64
-SibSp                int64
-Parch                int64
-Ticket              object
-Fare               float64
-Cabin               object
-Embarked            object
-list_in_columns     object
-dtype: object    
-
-df = dframe.d_edit_in_excel() #DataFrames   
-
-Out[7]: 
-     PassengerId  Survived  ...  Embarked                       list_in_columns
-0          10001      9999  ...   NOT YET  [[1, 99999, 1, 1, 1, 1, 1, 1, 1, 1]]
-1          10000         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-2           9999         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-3           9998         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-4           9997         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-..           ...       ...  ...       ...                                   ...
-886          887         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-887          888         1  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-888          889         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-889          890         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-890          891         0  ...         Q      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
-[891 rows x 13 columns]
-
-   df.dtypes
-Out[9]: 
-PassengerId          uint16
-Survived             uint16
-Pclass                uint8
-Name                 string
-Sex                category
-Age                  object
-SibSp                 uint8
-Parch                 uint8
-Ticket               object
-Fare                float64
-Cabin              category
-Embarked           category
-list_in_columns      object #you can even edit lists, dicts and tuples with Excel!
-dtype: object    
-
-df2 = dframe.Name.s_edit_in_excel() #Series
-
-df2
-Out[8]: 
-0                                        HANNIBAL LECTOR
-1      Cumings, Mrs. John Bradley (Florence Briggs Th...
-2                                 Heikkinen, Miss. Laina
-3           Futrelle, Mrs. Jacques Heath (Lily May Peel)
-4                               Allen, Mr. William Henry
-                             ...                        
-886                                Montvila, Rev. Juozas
-887                         Graham, Miss. Margaret Edith
-888             Johnston, Miss. Catherine Helen "Carrie"
-889                                Behr, Mr. Karl Howell
-890                                  Dooley, Mr. Patrick
-Name: Name, Length: 891, dtype: string    
-```
+## Quickly edit Pandas DataFrames and Series in Excel
+
+Use this methods to quickly edit your DataFrame with MS Excel.  
+Of course, Pandas is a lot better than Excel, but if you have to change a lot of  arbitrary values which don't have a clear pattern,  a GUI is imho the best choice.
+
+```python
+pip install a-pandas-ex-excel-edit 
+```
+
+```python
+    #Here is an example:
+
+    import pandas as pd
+    from a_pandas_ex_excel_edit import pd_add_excel_editor    
+
+    #pd_add_excel_editor will add 2 new methods:  
+    #pandas.Series.s_edit_in_excel
+    #pandas.DataFrame.d_edit_in_excel
+    pd_add_excel_editor()   
+
+    dframe = pd.read_csv("https://raw.githubusercontent.com/pandas-dev/pandas/main/doc/data/titanic.csv")
+    #Let's add a row with lists, a tough data type to handle
+    dframe['list_in_columns'] = [[[1]*10]] * len(dframe)   
+
+         PassengerId  Survived  ...  Embarked                   list_in_columns
+0              1         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+1              2         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+2              3         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+3              4         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+4              5         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+..           ...       ...  ...       ...                               ...
+886          887         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+887          888         1  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+888          889         0  ...         S  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+889          890         1  ...         C  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+890          891         0  ...         Q  [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+[891 rows x 13 columns]   
+
+dframe.dtypes
+Out[6]: 
+PassengerId          int64
+Survived             int64
+Pclass               int64
+Name                object
+Sex                 object
+Age                float64
+SibSp                int64
+Parch                int64
+Ticket              object
+Fare               float64
+Cabin               object
+Embarked            object
+list_in_columns     object
+dtype: object    
+
+df = dframe.d_edit_in_excel() #DataFrames   
+
+Out[7]: 
+     PassengerId  Survived  ...  Embarked                       list_in_columns
+0          10001      9999  ...   NOT YET  [[1, 99999, 1, 1, 1, 1, 1, 1, 1, 1]]
+1          10000         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+2           9999         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+3           9998         1  ...   NOT YET      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+4           9997         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+..           ...       ...  ...       ...                                   ...
+886          887         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+887          888         1  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+888          889         0  ...         S      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+889          890         1  ...         C      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+890          891         0  ...         Q      [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
+[891 rows x 13 columns]
+
+   df.dtypes
+Out[9]: 
+PassengerId          uint16
+Survived             uint16
+Pclass                uint8
+Name                 string
+Sex                category
+Age                  object
+SibSp                 uint8
+Parch                 uint8
+Ticket               object
+Fare                float64
+Cabin              category
+Embarked           category
+list_in_columns      object #you can even edit lists, dicts and tuples with Excel!
+dtype: object    
+
+df2 = dframe.Name.s_edit_in_excel() #Series
+
+df2
+Out[8]: 
+0                                        HANNIBAL LECTOR
+1      Cumings, Mrs. John Bradley (Florence Briggs Th...
+2                                 Heikkinen, Miss. Laina
+3           Futrelle, Mrs. Jacques Heath (Lily May Peel)
+4                               Allen, Mr. William Henry
+                             ...                        
+886                                Montvila, Rev. Juozas
+887                         Graham, Miss. Margaret Edith
+888             Johnston, Miss. Catherine Helen "Carrie"
+889                                Behr, Mr. Karl Howell
+890                                  Dooley, Mr. Patrick
+Name: Name, Length: 891, dtype: string    
+```
```

