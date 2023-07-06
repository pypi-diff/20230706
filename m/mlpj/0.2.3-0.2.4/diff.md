# Comparing `tmp/mlpj-0.2.3.tar.gz` & `tmp/mlpj-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpj-0.2.3.tar", last modified: Thu Apr 27 19:31:48 2023, max compression
+gzip compressed data, was "mlpj-0.2.4.tar", last modified: Thu Jul  6 21:32:33 2023, max compression
```

## Comparing `mlpj-0.2.3.tar` & `mlpj-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 19:31:48.203901 mlpj-0.2.3/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.2.3/LICENSE
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-27 19:31:48.203901 mlpj-0.2.3/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      965 2023-04-24 11:56:12.000000 mlpj-0.2.3/README.md
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 19:31:48.203901 mlpj-0.2.3/mlpj/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       72 2023-04-27 19:19:00.000000 mlpj-0.2.3/mlpj/__init__.py
--rw-------   0 bruno     (1000) bruno     (1000)    31419 2023-04-26 13:32:13.000000 mlpj-0.2.3/mlpj/actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    12473 2023-04-27 19:17:38.000000 mlpj-0.2.3/mlpj/ml_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1280 2023-04-26 12:56:20.000000 mlpj-0.2.3/mlpj/numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    24925 2023-04-26 13:58:50.000000 mlpj-0.2.3/mlpj/pandas_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    29704 2023-04-26 12:54:56.000000 mlpj-0.2.3/mlpj/plot_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)     7792 2023-04-26 13:31:12.000000 mlpj-0.2.3/mlpj/project_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8449 2023-04-26 13:42:35.000000 mlpj-0.2.3/mlpj/python_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    18778 2023-04-26 13:30:54.000000 mlpj-0.2.3/mlpj/result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.2.3/mlpj/result_template.html
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1882 2023-04-26 14:13:05.000000 mlpj-0.2.3/mlpj/timeseries_utils.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 19:31:48.203901 mlpj-0.2.3/mlpj.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-27 19:31:48.000000 mlpj-0.2.3/mlpj.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      584 2023-04-27 19:31:48.000000 mlpj-0.2.3/mlpj.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-04-27 19:31:48.000000 mlpj-0.2.3/mlpj.egg-info/dependency_links.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-04-27 19:31:48.000000 mlpj-0.2.3/mlpj.egg-info/requires.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-04-27 19:31:48.000000 mlpj-0.2.3/mlpj.egg-info/top_level.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-04-27 19:31:48.203901 mlpj-0.2.3/setup.cfg
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1223 2023-04-27 19:18:54.000000 mlpj-0.2.3/setup.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-27 19:31:48.203901 mlpj-0.2.3/test/
--rw-r--r--   0 bruno     (1000) bruno     (1000)    11486 2023-04-26 14:07:56.000000 mlpj-0.2.3/test/test_actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5570 2023-04-27 19:09:34.000000 mlpj-0.2.3/test/test_ml_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      499 2023-04-26 12:33:47.000000 mlpj-0.2.3/test/test_numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    13724 2023-04-26 12:35:55.000000 mlpj-0.2.3/test/test_pandas_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3807 2023-04-26 12:55:06.000000 mlpj-0.2.3/test/test_python_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3102 2023-04-26 14:00:27.000000 mlpj-0.2.3/test/test_result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1531 2023-04-26 14:00:51.000000 mlpj-0.2.3/test/test_timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.444157 mlpj-0.2.4/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.2.4/LICENSE
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-07-06 21:32:33.444157 mlpj-0.2.4/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      965 2023-04-24 11:56:12.000000 mlpj-0.2.4/README.md
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.440823 mlpj-0.2.4/mlpj/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       72 2023-07-06 21:29:27.000000 mlpj-0.2.4/mlpj/__init__.py
+-rw-------   0 bruno     (1000) bruno     (1000)    31419 2023-04-28 07:04:13.000000 mlpj-0.2.4/mlpj/actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    12367 2023-04-27 19:54:42.000000 mlpj-0.2.4/mlpj/ml_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1276 2023-05-19 10:51:10.000000 mlpj-0.2.4/mlpj/numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    28584 2023-07-06 20:37:39.000000 mlpj-0.2.4/mlpj/pandas_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    29704 2023-04-26 12:54:56.000000 mlpj-0.2.4/mlpj/plot_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)     7792 2023-04-28 06:51:00.000000 mlpj-0.2.4/mlpj/project_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     9444 2023-07-06 21:19:33.000000 mlpj-0.2.4/mlpj/python_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    18778 2023-04-26 13:30:54.000000 mlpj-0.2.4/mlpj/result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.2.4/mlpj/result_template.html
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1882 2023-04-26 14:13:05.000000 mlpj-0.2.4/mlpj/timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.440823 mlpj-0.2.4/mlpj.egg-info/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      584 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/requires.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/top_level.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-07-06 21:32:33.444157 mlpj-0.2.4/setup.cfg
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1221 2023-07-06 21:29:38.000000 mlpj-0.2.4/setup.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.444157 mlpj-0.2.4/test/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    11486 2023-04-26 14:07:56.000000 mlpj-0.2.4/test/test_actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     5570 2023-04-27 19:09:34.000000 mlpj-0.2.4/test/test_ml_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      499 2023-04-26 12:33:47.000000 mlpj-0.2.4/test/test_numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    17383 2023-07-06 21:05:17.000000 mlpj-0.2.4/test/test_pandas_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     4489 2023-07-06 21:25:45.000000 mlpj-0.2.4/test/test_python_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     3102 2023-04-26 14:00:27.000000 mlpj-0.2.4/test/test_result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1564 2023-07-06 21:28:41.000000 mlpj-0.2.4/test/test_timeseries_utils.py
```

### Comparing `mlpj-0.2.3/LICENSE` & `mlpj-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/PKG-INFO` & `mlpj-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpj
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tools for machine learning projects
 Home-page: https://github.com/bdanielby/mlpj
 Author: Bruno Daniel
 License: MIT
 Project-URL: Homepage, https://github.com/bdanielby/mlpj
 Project-URL: Source, https://github.com/bdanielby/mlpj
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlpj-0.2.3/README.md` & `mlpj-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/mlpj/actions_looper.py` & `mlpj-0.2.4/mlpj/actions_looper.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/mlpj/ml_utils.py` & `mlpj-0.2.4/mlpj/ml_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,17 +259,14 @@
 class OnColsTrans(sklearn.base.BaseEstimator, sklearn.base.TransformerMixin,
               auto_wrap_output_keys=None):
     """Scikit-learn-style meta-transformer restricting a given transformer to
     a given subset of the columns of the feature matrix.
 
     The feature matrix is expected to be a `pd.DataFrame`.
 
-    In the methods `get_params`, `set_params`, `OnColsTrans` just delegates
-    to the base transformer.
-
     Args:
         est: base transformer to be wrapped
         used_features: column names to restrict to
         output_features: column names for the result of the base transformer,
             defaulting to `used_features`
 
             If the base transformer transforms a `pd.DataFrame` into a
```

### Comparing `mlpj-0.2.3/mlpj/numpy_utils.py` & `mlpj-0.2.4/mlpj/numpy_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     would result in an IndexError.
 
     Args:
         x (array-like, 1dim): input array to be binned
         bins (array-like, 1dim): array of bins, must be monotonic
     Returns:
         `np.ndarray`: array of indices; it has the same shape as `x`.
-    
+
     Raises:
         ValueError: If the input is not 1-dimensional, or if `bins` is not monotonic.
         TypeError: If the type of the input is complex.
     """
     bin_numbers = np.digitize(x, bins)
     is_max = x >= bins.max()
     bin_numbers[is_max] -= 1
```

### Comparing `mlpj-0.2.3/mlpj/pandas_utils.py` & `mlpj-0.2.4/mlpj/pandas_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 Utilities and convenience functions for using `pandas`.
 """
 import re
 import contextlib
 import collections
+import datetime
+import dateutil.tz
+import pytz
 from typing import Optional, Union, List, Tuple, Any, Dict
 from collections.abc import Sequence, Generator
 import types
 
 import numpy as np
 from numpy.typing import ArrayLike
 import pandas as pd
@@ -72,15 +75,15 @@
       bool: whether the series can be used for numerical purposes
     """
     return ser.dtype.kind in "bif"
 
 
 def get_colnames(X_or_names: Any) -> List[str]:
     """Get columns from an object carrying column names
-    
+
     Args:
         X_or_names (`pd.DataFrame` or `DataFrameGroupBy` or seq of str):
             input carrying column names
     Returns:
         list of str: list of column names
     """
     if isinstance(X_or_names, pd.DataFrame):
@@ -124,15 +127,15 @@
             selected.append(colname)
     if feature_list is not None:
         selected = set(selected)
         return [feature for feature in feature_list if feature in selected]
     else:
         return selected
 
-    
+
 def rename_column(X: pd.DataFrame, old_name: str, new_name: str) -> None:
     """Rename a column in the passed dataframe (in place).
 
     Args:
         X (`pd.DataFrame): input dataframe
         old_name (str): old column name
         new_name (str): new column name
@@ -140,15 +143,15 @@
     Raises:
         `ValueError` if the `old_name` isn't found among the columns.
     """
     if old_name not in X.columns:
         raise KeyError('column {} not found'.format(old_name))
     X.rename(columns={old_name: new_name}, inplace=True)
 
-    
+
 def drop_index(X: pd.DataFrame) -> pd.DataFrame:
     """Drop the index from a dataframe in place.
 
     Args:
         X (`pd.DataFrame`): input dataframe
     Returns:
         X: changed in place
@@ -196,15 +199,15 @@
 
     Args:
         df (`pd.DataFrame`): input dataframe
     Returns:
         `pd.DataFrame`: new dataframe
     """
     import sklearn.utils
-    
+
     df = sklearn.utils.shuffle(df)
     drop_index(df)
     return df
 
 
 def assert_frame_contents_equal(
         df1: pd.DataFrame, df2: pd.DataFrame, **kwargs
@@ -218,15 +221,15 @@
         df1 (`pd.DataFrame`): first input dataframe
         df2 (`pd.DataFrame`): second input dataframe
         kwargs: See `pd.testing.assert_frame_equal`.
     """
     pd_testing.assert_frame_equal(
         df1.reset_index(drop=True), df2.reset_index(drop=True), **kwargs)
 
-        
+
 def ser_where_defined(ser: pd.Series) -> pd.Series:
     """Select non-null entries of a series.
 
     Args:
         ser (`pd.Series`): input series
     Returns:
         `pd.Series`: a new series containing the non-null entries.
@@ -242,27 +245,60 @@
     Returns:
        n, perc: the number of undefined values in the series and their
            percentage (scaled to 100)
     """
     return pu.wi_perc(ser.isnull().sum(), len(ser))
 
 
+def n_undefined(ser: pd.Series) -> int:
+    """number of undefined entries in a series
+
+    Args:
+        ser: Series
+    Returns:
+        number of undefined entries
+    """
+    return ser.isnull().sum()
+
+
+def defined_everywhere(ser: pd.Series) -> bool:
+    """Are all entries of a series defined?
+
+    Args:
+        ser: Series
+    Returns:
+        whether there are no missing/undefined values
+    """
+    return n_undefined(ser) == 0
+
+
+def fill_forward_then_backward(ser: pd.Series) -> pd.Series:
+    """Fill missing values in a series first forward, then backward.
+
+    Args:
+        ser: input Series
+    Returns:
+        output Series
+    """
+    return ser.ffill().bfill()
+
+
 def colname_list(colnames: Union[str, Sequence[str]]) -> Sequence[str]:
     """If the input is a string, turn it into a one-element list, otherwise just
     return the input.
 
     Args:
         colnames (str or list of str): input column names
     Returns:
         list of str: list of oclumn names
     """
     if pu.isstring(colnames):
         return [colnames]
     return colnames
-    
+
 
 def sort(
         X: pd.DataFrame, colnames: Union[str, Sequence[str]] = None,
         inplace: bool = False, kind: str = 'stable', ascending: bool = True
 ) -> pd.DataFrame:
     """Convenience function to sort a dataframe with a stable sort and ignoring
     the index.
@@ -301,15 +337,15 @@
     """
     arr = np.unique(ser.values)
     return pd.Series(arr, name=ser.name)
 
 
 def left_merge(left: pd.DataFrame, right: pd.DataFrame, **kwargs) -> pd.DataFrame:
     """Convience function for a left merge in Pandas.
-    
+
     `pd.DataFrame.merge` may produce result columns to in a different order
     if the left dataframe is empty. The (empty) index is also of a different
     type than for nonempty dataframes. This causes problems in `dask`. This
     wrapper function fixes the bug.
 
     Duplicated rows are not tolerated, i.e. the merge must be unique and the
     result must have rows in one-to-one correspondence with `left`. The
@@ -324,15 +360,15 @@
         length as `left`. No arrays are shared with `left` or `right`.
     Raises:
         `ValueError` if the result length is different from the length of
         `left`.
     """
     assert 'how' not in kwargs
     df = left.merge(right, how='left', **kwargs)
-    
+
     left_colnames = left.columns.tolist()
     if (len(df) == 0 and
             df.columns.tolist()[:len(left_colnames)] != left_colnames):
         rest_colnames = all_colnames_except(df, left_colnames)
         df = df.loc[:, left_colnames + rest_colnames]
     if len(df) != len(left):
         raise ValueError("The left merge has a different number of rows ({}) "
@@ -366,15 +402,15 @@
             row_of_group_end += 1
 
         work_columns_slice = (
             work_columns[row_of_group_start:row_of_group_end, :])
 
         f(work_columns_slice)
         row_of_group_start = row_of_group_end
-        
+
 
 _fast_groupby_multi_transform1_jit = numba.njit(_fast_groupby_multi_transform1)
 
 
 def fast_groupby_multi_transform(
         df: pd.DataFrame, group_colnames: Union[str, Sequence[str]],
         work_colnames: Union[str, Sequence[str]],
@@ -419,15 +455,15 @@
     group_colnames = colname_list(group_colnames)
     work_colnames = colname_list(work_colnames)
     result_colnames = colname_list(result_colnames)
     if not set(result_colnames) <= set(work_colnames):
         raise ValueError(
             f"result_colnames {result_colnames} is not a subset of work_colnames "
             f"{work_colnames}")
-        
+
     further_sort_colnames = colname_list(further_sort_colnames)
     if not already_sorted:
         df.sort_values(group_colnames + further_sort_colnames, inplace=True,
                        kind='stable')
 
     igroup = df.groupby(group_colnames).ngroup().values
 
@@ -458,15 +494,15 @@
 def rename_groupby_colnames(
         df: pd.DataFrame, name_for_count: Optional[str] = None,
         renamings: Union[Sequence[Tuple[str, str]], Dict[str, str]] = ()
 ) -> None:
     """Rename column names as they arise from groupby-calls.
 
     The dataframe is changed in place.
-    
+
     If a column has multiple aggregations, the tuple column names are combined
     with underscores. Otherwise just the column is used.
 
     Args:
         df (`pd.DataFrame`): input dataframe
         name_for_count (str, optional): If given, this aggregation is treated
             separately because such an aggregation is often not specific to
@@ -474,35 +510,35 @@
         renamings (seq of key-value pairs or dict):
             These renamings are applied after all the other steps. They are
             applied to the name of the index (or its levels for a multiindex).
     """
     assert name_for_count is None or pu.isstring(name_for_count)
     if not isinstance(renamings, dict):
         renamings = dict(renamings)
-        
+
     aggs_for_colname = collections.defaultdict(list)
     for colname, agg_name in df.columns:
         if name_for_count is not None and agg_name == 'count':
             continue
         aggs_for_colname[colname].append(agg_name)
-        
+
     new_colnames = []
     for colname, agg_name in df.columns:
         if name_for_count is not None and agg_name == 'count':
             new_colname = name_for_count
         else:
             aggs = aggs_for_colname[colname]
             if len(aggs) == 1:
                 new_colname = colname
             else:
                 new_colname = '{}__{}'.format(colname, agg_name)
         new_colname = renamings.get(new_colname, new_colname)
         new_colnames.append(new_colname)
     df.columns = new_colnames
-    
+
     if len(renamings) > 0:
         if isinstance(df.index, pd.MultiIndex):
             for i_level in range(len(df.index.levels)):
                 name = df.index.levels[i_level].name
                 if name in renamings:
                     df.index.levels[i_level].name = renamings[name]
         else:
@@ -511,15 +547,15 @@
 
 
 def print_column_info(
         col: pd.Series, table_name: str = None,
         ignored_columns: Sequence[str] = (), n_value_counts: int = 50
 ) -> None:
     """Print information about a column
-    
+
     For a column, print its `dtype`, call `describe`, count the missing
     values, count the distinct values and print the `value_counts` of up to
     `n_value_counts` most frequent values.
 
     Args:
         col (`pd.Series`): the input column
         table_name (str): table name of the dataframe for context
@@ -534,15 +570,15 @@
         full_colname = f"{table_name}.{colname}"
     internal_link = re.sub(r'\.', '_', full_colname) + '_colinfo'
     print(f'<a name="{internal_link}"><h3><a href="#{internal_link}">'
           f'column: {full_colname}</a></h3>')
     print(f"column dtype: {col.dtype}, length {len(col)}")
     if colname in ignored_columns:
         return
-    
+
     print()
     print("describe:")
     print(col.describe())
     print()
     n_undefined, perc_undefined = n_undefined_and_percentage(col)
     print(f"{n_undefined} missing values ({perc_undefined:.1f} %)")
     value_counts = col.value_counts()
@@ -552,21 +588,21 @@
     if n_value_counts < 50:
         print(f"value counts")
         print(value_counts)
     else:
         print("value counts of the 50 most frequent values:")
         print(value_counts.iloc[:50])
 
-        
+
 def print_table_info(
         df: pd.DataFrame, table_name: str,
         ignored_columns: Sequence[str] = (), n_value_counts: int = 50
 ) -> None:
     """Print information about a dataframe's columns.
-    
+
     For a dataframe, print its shape, column dtypes and call
     `print_column_info` for each column (except the ones in `ignored_columns`).
 
     Args:
         df (`pd.DataFrame`): the input dataframe
         table_name (str): table name of the dataframe for context
         ignored_columns (seq of str): sequence of columns to ignore
@@ -594,15 +630,15 @@
         colname_b (str): second column name to compare
         n_examples (int): number of inconsistency examples to show
         extra_colnames (list of str): extra columns to show for context in the
             inconsistency results
     """
     ser_a = df[colname_a]
     ser_b = df[colname_b]
-    
+
     print(f"consistency check of {ser_a.name} and {ser_b.name}")
     a_isnull = ser_a.isnull()
     is_same = (ser_a == ser_b) | (a_isnull & (a_isnull == ser_b.isnull()))
     if is_same.all():
         print("always the same")
     else:
         print("not always the same; value counts of equality:")
@@ -615,15 +651,15 @@
         if len(examples) <= n_examples:
             print("all inconsistencies:")
         else:
             examples = examples.iloc[-n_examples:]
             print(f"the last {len(examples)} inconsistencies:")
         print(examples)
 
-        
+
 def keys_of_dict_column(ser: pd.Series) -> pd.Series:
     """Transform a series with dict values into a series with the lists of their
     keys.
 
     Args:
         ser (`pd.Series`): input series with `dict` entries
     Returns:
@@ -640,14 +676,25 @@
         ser (`pd.Series`): input series with `dict` entries
     Returns:
         `np.ndarray`: array of distinct lists of keys
     """
     return np.unique(keys_of_dict_column(ser))
 
 
+def to_datetime_ser(entries: ArrayLike) -> pd.Series:
+    """Convert an array of date strings into a datetimens series.
+
+    Args:
+        entries: date strings to be converted
+    Returns:
+        series of type datetimens
+    """
+    return pd.Series(pd.to_datetime(entries))
+
+
 def truncate_datetime_to_freq(ser: pd.Series, freq: str) -> pd.Series:
     """Truncate datetime values to the specified period.
 
     Args:
         ser (`pd.Series`): input series
         freq (str): Pandas frequency or frequency alias
     Returns:
@@ -656,29 +703,29 @@
     return ser.dt.to_period(freq).dt.start_time
 
 
 def truncate_datetime_to_month(ser: pd.Series) -> pd.Series:
     """Truncate datetime values to the beginning of the month.
 
     Special case of `truncate_datetime_to_freq` with frequency 'M'.
-    
+
     Args:
         ser (`pd.Series`): input series
     Returns:
         `pd.Series` with datetime values truncated to the beginning of the
         respective month
     """
     return truncate_datetime_to_freq(ser, 'M')
 
 
 def truncate_datetime_to_week(ser: pd.Series, sunday_first: bool = False) -> pd.Series:
     """Truncate datetime values to the beginning of the week.
 
     Special case of `truncate_datetime_to_freq`.
-    
+
     Args:
         ser (`pd.Series`): input series
         sunday_first (bool): whether to consider Sunday the beginning of the week;
             by default the week starts with Monday
     Returns:
         `pd.Series` with datetime values truncated to the beginning of the
         respective week
@@ -692,25 +739,99 @@
 
 MIN_DATETIME = pd.to_datetime("1970-01-01")
 
 
 def datetime_to_epoch(ser: pd.Series) -> pd.Series:
     """Convert a Pandas datetime series to a float epoch, including the
     nanoseconds.
-    
+
     NaT values are converted to NaT values.
 
     Args:
         ser (`pd.Series`): input deries
     Returns:
         `pd.Series`: output series containing float epochs
     """
     return (ser - MIN_DATETIME).dt.total_seconds()
 
 
+def convert_to_timezone(
+        ser: pd.Series,
+        tz: Union[str, pytz.timezone, dateutil.tz.tzfile, datetime.tzinfo]
+) -> pd.Series:
+    """Convert a timezone-naive datetime column in UTC to the given timezone
+
+    Args:
+        ser: input series (datetime)
+        tz: time zone to convert to
+    Returns:
+        output series
+    """
+    return ser.dt.tz_localize(pytz.utc).dt.tz_convert(tz)
+
+
+def add_missing_days(dfg: pd.DataFrame, end_datetime: Optional[Any] = None,
+                   freq: str = 'D', reset_index: bool = True
+                   ) -> pd.DataFrame:
+    """For the groupby-result of a daily aggregation, add the missing days by
+    reindexing the dataframe.
+
+    A MultiIndex is used to create the Cartesian product of all three
+    levels. For the datetime level among them (which must exist), add
+    entries up to `end_datetime`.
+
+    Args:
+        dfg: input dataframe; it must have a `MultiIndex` with one of the
+            index levels being the date.
+        end_datetime (must be convertible with `pd.to_datetime`): The final
+            datetime to reconstruct in the reindexing.
+            This way, further datetimes can be added at the end. By
+            default the maximum datetime is taken.
+        freq: frequency alias to use within `pd.date_range`
+        reset_index: whether to call `reset_index` in the end, which is often
+            useful after a groupby operation
+    Returns:
+        reindexed dataframe; the former index levels are also turned into
+            columns. Please fill the resulting NaN entries where appropriate,
+            e.g. by setting them to 0 (for sales) or forward filling them
+            (for features)
+    """
+    n_levels_found = dfg.index.nlevels
+
+    new_index_levels = []
+    datetime_level_found = False
+    for i_level in range(n_levels_found):
+        level_vals = dfg.index.get_level_values(i_level)
+        if level_vals.dtype.name.startswith('datetime'):
+            if end_datetime == None:
+                date_end = level_vals.max()
+            else:
+                date_end = pd.to_datetime(end_datetime)
+            new_level_vals = pd.Series(
+                pd.date_range(level_vals.min(), date_end, freq=freq),
+                name=dfg.index.names[i_level])
+            datetime_level_found = True
+        else:
+            new_level_vals = sorted_unique_1dim(level_vals)
+        new_index_levels.append(new_level_vals)
+
+    if not datetime_level_found:
+        raise ValueError("No datetime index level found")
+    if n_levels_found == 1:
+        new_index = new_index_levels[0]
+    else:
+        new_index = pd.MultiIndex.from_product(new_index_levels)
+    dfg = dfg.reindex(new_index)
+
+    if reset_index:
+        dfg.reset_index(inplace=True)
+
+    return dfg
+
+
 def to_csv(df: pd.DataFrame, filepath: str, **kwargs) -> None:
     """Convenience function to call `pd.DataFrame.to_csv` with common
     defaults.
 
     Args:
         df (`pd.DataFrame`): input dataframe
         file (str or stream): CSV filepath to create or stream to write to
```

### Comparing `mlpj-0.2.3/mlpj/plot_utils.py` & `mlpj-0.2.4/mlpj/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/mlpj/project_utils.py` & `mlpj-0.2.4/mlpj/project_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/mlpj/python_utils.py` & `mlpj-0.2.4/mlpj/python_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utilities and convenience functions for using the Python standard library.
 """
+import re
 import os
 import sys
 import sqlite3
 import datetime
 import contextlib
 import tempfile
 import logging
@@ -46,15 +47,15 @@
     Returns:
         the chosen value as specified above
     """
     if flag:
         return value
     else:
         return default
-    
+
 
 def wi_perc(value: float, reference: float) -> Tuple[float, float]:
     """Return the value and the percentage of the value in the reference.
 
     Args:
         value (number): value to compare
         reference (number): total amount
@@ -116,25 +117,38 @@
     i = 0
     for i, part in enumerate(parts):
         if i >= n_ref or part != parts_ref[i]:
             break
     return os.path.join(*(['..'] * (n_ref - i) + parts[i:]))
 
 
+def filepath_in_dir_of(filename: str, filepath_in_same_dir: str) -> str:
+    """Take the directory of the given filepath and add the given filename to
+    it.
+
+    Args:
+        filename: a filename for the directory
+        filepath_in_same_dir: a filepath defining the directory
+    Returns:
+        composed filepath
+    """
+    return os.path.join(os.path.dirname(filepath_in_same_dir), filename)
+
+
 @contextlib.contextmanager
 def redirect_stdouterr(outfp: TextIO, errfp: TextIO) -> Generator[None]:
     """Context manager for temporary redirection of `sys.stdout` and
     `sys.stderr`.
-    
+
     Args:
         outfp (output stream): output stream to redirect the standard output
             stream to (default=`os.devnull`)
         errfp (output stream): path or output stream to redirect
             the standard error stream to (default=`os.devnull`)
-    
+
     If you want to keep one of the two unchanged, just pass `sys.stdout` or
     `sys.stderr`, respectively.
     """
     old_stdout = sys.stdout
     old_stderr = sys.stderr
     try:
         sys.stdout.flush()
@@ -142,15 +156,15 @@
         sys.stdout = outfp
         sys.stderr = errfp
         yield
     finally:
         sys.stdout = old_stdout
         sys.stderr = old_stderr
 
-        
+
 class BranchedOutputStreams:
     """Output stream that delegates to multiple other output streams
 
     Args:
         streams (seq of output streams): output streams to delegate to
     """
     def __init__(self, streams: Sequence[TextIO]):
@@ -171,15 +185,15 @@
             stream.flush()
 
     def close(self) -> None:
         """Close all output streams."""
         for stream in self.streams:
             stream.close()
 
-        
+
 @contextlib.contextmanager
 def open_overwriting_safely(
         filepath: str, mode: int
 ) -> Generator[Union[TextIO, BinaryIO]]:
     """Open a temporary file and rename it in the end.
 
     Instead of overwriting the given file directly, open a temporary file
@@ -217,15 +231,15 @@
         ANSII escape code
     """
     if is_bright:
         bright_part = ';1'
     else:
         bright_part = ''
     return f"\x1b[{color_num}{bright_part}m"
-    
+
 
 TERMSEQ = {
     'red[': ansiicol(31),
     'br_red[': ansiicol(31, True),
     'green[': ansiicol(32),
     'br_green[': ansiicol(32, True),
     'yellow[': ansiicol(33),
@@ -261,26 +275,37 @@
             db.close()
 
 
 SECONDS_IN_HOUR = 3600
 
 SECONDS_IN_DAY = 24 * SECONDS_IN_HOUR
 
-    
+
 def n_days_ago(n_days: int) -> datetime.datetime:
     """The datetime object for the day n_days days ago
 
     Args:
         n_days (int): number of days to go into the past
     Returns:
         `datetime.datetime`: datetime object for that day in the past
     """
     return datetime.date.today() - datetime.timedelta(n_days)
 
 
+def n_days_from_today(n_days: int) -> datetime.datetime:
+    """The datetime object for the day n_days from today
+
+    Args:
+        n_days (int): number of days to go into the future
+    Returns:
+        `datetime.datetime`: datetime object for that day in the future
+    """
+    return datetime.date.today() + datetime.timedelta(n_days)
+
+
 def today_isoformat() -> str:
     """Today in ISO date format
 
     Returns:
         str: in ISO date format
     """
     return datetime.date.today().isoformat()
@@ -299,7 +324,19 @@
     logger.setLevel(level)
     handler = logging.StreamHandler()
     handler.setFormatter(
         logging.Formatter("%(asctime)s %(name)s %(levelname)s: %(message)s"))
     logger.addHandler(handler)
 
     return logger
+
+
+def strip_margin(text: str) -> str:
+    """After each newline in the string, strip the whitespace part before a
+    vertical bar just like in Scala.
+
+    Args:
+        text: input string
+    Returns:
+        output string
+    """
+    return re.sub('\n[ \t]*[|]', '\n', text)
```

### Comparing `mlpj-0.2.3/mlpj/result_display.py` & `mlpj-0.2.4/mlpj/result_display.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/mlpj/result_template.html` & `mlpj-0.2.4/mlpj/result_template.html`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/mlpj/timeseries_utils.py` & `mlpj-0.2.4/mlpj/timeseries_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/mlpj.egg-info/PKG-INFO` & `mlpj-0.2.4/mlpj.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpj
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tools for machine learning projects
 Home-page: https://github.com/bdanielby/mlpj
 Author: Bruno Daniel
 License: MIT
 Project-URL: Homepage, https://github.com/bdanielby/mlpj
 Project-URL: Source, https://github.com/bdanielby/mlpj
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlpj-0.2.3/mlpj.egg-info/SOURCES.txt` & `mlpj-0.2.4/mlpj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/setup.py` & `mlpj-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 github_url = 'https://github.com/bdanielby/mlpj'
 
 setup(
     name='mlpj',
-    version='0.2.3',
+    version='0.2.4',
     description='Tools for machine learning projects',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url=github_url,
     author='Bruno Daniel',
     license='MIT',
     packages=['mlpj'],
@@ -29,14 +29,14 @@
         'Source': github_url,
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Manufacturing',
-        'License :: OSI Approved :: MIT License',  
+        'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python :: 3',
     ],
 )
```

### Comparing `mlpj-0.2.3/test/test_actions_looper.py` & `mlpj-0.2.4/test/test_actions_looper.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/test/test_ml_utils.py` & `mlpj-0.2.4/test/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/test/test_pandas_utils.py` & `mlpj-0.2.4/test/test_pandas_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Unit tests for `mlpj.pandas_utils`.
 """
 import datetime
 import collections
 import io
+from typing import List
 
 import numpy as np
 import pandas as pd
 import numba
 import pandas.testing as pd_testing
 import pytest
 
@@ -81,36 +82,36 @@
     X = pd.DataFrame(np.eye(4), columns=['x', 'a', 'ba', 'c'])
     assert pdu.all_colnames_except(X, ['a', 'c']) == ['x', 'ba']
 
     X = pd.DataFrame(np.eye(4), columns=list('abcd'))
     assert pdu.all_colnames_except(X, ['c', 'a']) == ['b', 'd']
     assert pdu.all_colnames_except(X, ['c', 'a', 'b', 'd']) == []
 
-    
+
 def test_category_colnames() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
         ('c', ['x', 'y', 'z', 'x'])
     ])
-        
+
     assert pdu.category_colnames(df) == []
     for colname in ['a', 'b']:
         df[colname] = df[colname].astype('category')
     assert pdu.category_colnames(df) == ['a', 'b']
 
     assert pdu.category_colnames(df, feature_list=('b', 'c')) == ['b']
 
 
 def test_rename_column() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
     ])
-    
+
     pdu.rename_column(df, 'b', 'b1')
     pd_testing.assert_frame_equal(
         df,
         pdu.from_items([
             ('a', [3, 4, 3, 2]),
             ('b1', ['a', 'b', 'b', 'a']),
         ]))
@@ -130,22 +131,22 @@
     pd_testing.assert_frame_equal(
         df,
         pdu.from_items([
             ('b', np.array([3, 8])),
             ('a', ['first', 'second'])
         ]))
 
-    
+
 def test_drop_columns() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'b', 'a']),
         ('c', ['x', 'y', 'z', 'x'])
     ], index=[3, 4, 5, 8])
-    
+
     df1 = df.copy()
     pdu.drop_columns(df1, 'a')
 
     pd_testing.assert_frame_equal(
         df1,
         pdu.from_items([
             ('b', ['a', 'b', 'b', 'a']),
@@ -155,15 +156,15 @@
     df2 = df.copy()
     pdu.drop_columns(df2, ['a', 'c'])
     pd_testing.assert_frame_equal(
         df2,
         pdu.from_items([
             ('b', ['a', 'b', 'b', 'a']),
         ], index=[3, 4, 5, 8]))
-        
+
     with pytest.raises(KeyError):
         pdu.drop_columns(df, 'x')
 
 
 def test_columns_to_right() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
@@ -189,15 +190,15 @@
 
 
 def test_assert_frame_contents_equal() -> None:
     df1 = pdu.from_items([
         ('b', np.array([3, 8])),
         ('a', ['first', 'second']),
     ], index=[3, 4])
-    
+
     df2 = pd.DataFrame([[3, 'first'], [8, 'second']],
                        columns=['b', 'a'])
 
     with pytest.raises(AssertionError):
         pd_testing.assert_frame_equal(df1, df2)
 
     pdu.assert_frame_contents_equal(df1, df2)
@@ -206,46 +207,80 @@
 def test_ser_where_defined() -> None:
     x = pd.Series([4, 5, nan, 2, nan])
 
     pd_testing.assert_series_equal(
         pdu.ser_where_defined(x),
         pd.Series([4., 5, 2], index=[0, 1, 3]))
 
-    
+
 def test_n_undefined_and_percentage() -> None:
     x = pd.Series([4, 5, nan, 2, nan])
-    
+
     n, perc = pdu.n_undefined_and_percentage(x)
     assert n == 2
     assert perc == 2 / 5 * 100
 
 
+@pytest.mark.parametrize('ser, expected', [
+    (pd.Series([3., nan, 4, nan]), 2),
+    (pd.Series([3., 4]), 0),
+    (pd.Series([None, "a", ""]), 1),
+    (pd.Series(["a", ""]), 0),
+    (pd.Series([]), 0),
+])
+def test_n_undefined(ser: pd.Series, expected: int) -> None:
+    assert pdu.n_undefined(ser) == expected
+
+
+
+@pytest.mark.parametrize('ser, expected', [
+    (pd.Series([3., nan, 4, nan]), False),
+    (pd.Series([3., 4]), True),
+    (pd.Series([None, "a", ""]), False),
+    (pd.Series(["a", ""]), True),
+    (pd.Series([]), True),
+])
+def test_defined_everywhere(ser: pd.Series, expected: int) -> None:
+    assert pdu.defined_everywhere(ser) == expected
+
+
+@pytest.mark.parametrize('ser, expected', [
+    (pd.Series([nan, 3., nan, 4, nan]), pd.Series([3., 3, 3, 4, 4])),
+    (pd.Series([3., 4]), pd.Series([3., 4])),
+    (pd.Series([None, "a", "", None]), pd.Series(["a", "a", "", ""])),
+    (pd.Series(["a", ""]), pd.Series(["a", ""])),
+    (pd.Series([]), pd.Series([])),
+])
+def test_fill_forward_then_backward(ser: pd.Series, expected: pd.Series) -> None:
+    pd_testing.assert_series_equal(pdu.fill_forward_then_backward(ser), expected)
+
+
 def test_colname_list() -> None:
     assert pdu.colname_list('foo') == ['foo']
     assert pdu.colname_list(['foo', 'bar']) == ['foo', 'bar']
 
 
 def test_sort() -> None:
     df = pdu.from_items([
         ('a', [3, 4, 3, 2]),
         ('b', ['a', 'b', 'c', 'd']),
         ('c', ['x', 'y', 'z', 'w'])
     ], index=[3, 4, 5, 8])
 
     df1 = pdu.sort(df, colnames='a', inplace=True)
     assert df1 is df
-    
+
     pd_testing.assert_frame_equal(
         df,
         pdu.from_items([
             ('a', [2, 3, 3, 4]),
             ('b', ['d', 'a', 'c', 'b']),
             ('c', ['w', 'x', 'z', 'y'])
         ], index=[0, 1, 2, 3]))
-        
+
 
 def test_sorted_unique_1dim() -> None:
     x = pd.Series([4, 3, nan, 8, 4, 3, nan, 2])
     pd_testing.assert_series_equal(
         pdu.sorted_unique_1dim(x),
         pd.Series([2, 3, 4, 8, nan]))
 
@@ -256,15 +291,15 @@
     dfb = pdu.from_items([('ITEM', [10, 20, 90]),
                           ('Quantity_nrm', [8, 9, 7])])
     dfr = pdu.left_merge(df, dfb, on=['ITEM'])
     pd_testing.assert_frame_equal(
         dfr, pdu.from_items([('ITEM', [10, 20, 70, 30]),
                              ('Quantity', [3, 4, 8, 9]),
                              ('Quantity_nrm', [8, 9, nan, nan])]))
-    
+
     df = pdu.from_items([('ITEM', np.zeros(0)),
                          ('Quantity', np.zeros(0))])
     dfb = pdu.from_items([('ITEM', np.zeros(0)),
                           ('Quantity_nrm', np.zeros(0))])
     dfr = pdu.left_merge(df, dfb, on=['ITEM'])
     pd_testing.assert_frame_equal(
         dfr, pdu.from_items([('ITEM', np.zeros(0)),
@@ -281,54 +316,54 @@
     # to test whether overwriting a non-result column has any consequence:
     a[:] = 0.
 
 
 @numba.njit
 def double_a(X: pd.DataFrame) -> None:
     X[:, 0] *= 2
-    
+
 
 def test_fast_groupby_multi_transform() -> None:
     df = pdu.shuffle_df_drop_index(
         pdu.from_items([
             ('g', [0,   0, 0, 0, 1, 1, 1, 1]),
             ('a', [1,   2, 4, 8, 3, 9, 27, 81]),
             ('b', [nan, 2, 5, 4, 4, 0, 3, -1])
         ]))
-    
+
     pdu.fast_groupby_multi_transform(
         df, 'g', ['a', 'b'], 'b', add_cumsum_a_to_b, further_sort_colnames='a')
 
     pdu.assert_frame_contents_equal(
         df,
         pdu.from_items([
             ('g', [0,   0, 0, 0,   1, 1, 1, 1]),
             ('a', [1,   2, 4, 8,   3, 9,  27, 81]),
             ('b', [nan, 5, 12, 19, 7, 12, 42, 119])
         ]))
 
     pdu.fast_groupby_multi_transform(
         df, 'g', 'a', 'a', double_a, already_sorted=True)
-    
+
     pdu.assert_frame_contents_equal(
         df,
         pdu.from_items([
             ('g', [0,   0, 0, 0,   1, 1, 1, 1]),
             ('a', [2,   4, 8, 16,  6, 18, 54, 162]),
             ('b', [nan, 5, 12, 19, 7, 12, 42, 119])
         ]))
-    
+
 
 def test_flatten_multi_columns() -> None:
     df = pdu.from_items([
         (('a', '1'), [3, 4, 3, 2]),
         (('b', '2'), ['a', 'b', 'b', 'a']),
         (('c', '1'), ['x', 'y', 'z', 'x'])
     ], index=[3, 4, 5, 8])
-    
+
     pdu.flatten_multi_columns(df)
     pd_testing.assert_frame_equal(
         df,
         pdu.from_items([
             ('a_1', [3, 4, 3, 2]),
             ('b_2', ['a', 'b', 'b', 'a']),
             ('c_1', ['x', 'y', 'z', 'x'])
@@ -338,15 +373,15 @@
 def test_rename_groupby_colnames() -> None:
     df = pdu.from_items([
         ('g', [0, 0, 0, 0, 1, 1, 1]),
         ('a', [2, 3, 0, 1, 4, 2, 1]),
         ('b', [-1, 1, 2, 0, -2, 1, 0]),
         ('c', [8, 2, 5, 1, -2, -1, 4]),
     ])
-    
+
     dfg = df.groupby('g').agg(collections.OrderedDict([
         ('a', ['sum', 'max']),
         ('b', ['sum', 'count']),
         ('c', 'max'),
     ]))
 
     dfg1 = dfg.copy()
@@ -356,15 +391,15 @@
         pdu.from_items([
             ('a__sum', [6, 7]),
             ('a__max', [3, 4]),
             ('b', [2, -1]),
             ('group_count', [4, 3]),
             ('c', [8, 4])
         ], index=pd.Index([0, 1], name='g')))
-    
+
     dfg2 = dfg.copy()
     pdu.rename_groupby_colnames(
         dfg2, name_for_count='group_count',
         renamings={'a__sum': 'summed_a', 'g': 'group', 'group_count': 'count'}
     )
     pd_testing.assert_frame_equal(
         dfg2,
@@ -375,100 +410,179 @@
             ('count', [4, 3]),
             ('c', [8, 4])
         ], index=pd.Index([0, 1], name='group')))
 
 
 def test_print_column_info() -> None:
     ser = pd.Series([3, 4, nan, 2])
-    
+
     out = io.StringIO()
     with pu.redirect_stdouterr(out, out):
         pdu.print_column_info(ser, table_name='X')
 
 
 def test_print_table_info() -> None:
     df = pdu.from_items([
         ('a', [2, 3, 0, 1, 4, 2, 1]),
         ('c', [8, 2, 5, 1, -2, -1, 4]),
     ])
-    
+
     out = io.StringIO()
     with pu.redirect_stdouterr(out, out):
         pdu.print_table_info(df, table_name='X')
 
 
 def test_consistency_check() -> None:
     df = pdu.from_items([
         ('a', [2, 3,    0, 1, 4.1, 2, 1]),
         ('a1', [2, 3.1, 0, 1, 4,   2, 1]),
         ('c', [8, 2, 5, 1, -2, -1, 4]),
     ])
-    
+
     out = io.StringIO()
     with pu.redirect_stdouterr(out, out):
         pdu.consistency_check(df, 'a', 'a1')
 
 
+@pytest.mark.parametrize('entries', [
+    ['2023-04-22 10:40:22', '2023-03-01 00:00:00'],
+    ['2023-04-22', '2023-03-01', "NaT"],
+])
+def test_to_datetime_ser(entries: List[str]) -> None:
+    pd_testing.assert_series_equal(
+        pdu.to_datetime_ser(entries), pd.Series(pd.to_datetime(entries)))
+
+
 def test_truncate_datetime_to_freq() -> None:
-    x = pd.Series(pd.to_datetime(['2023-04-22 10:40:22', '2023-03-01']))
-    
+    x = pdu.to_datetime_ser(['2023-04-22 10:40:22', '2023-03-01 00:00:00'])
+
     pd_testing.assert_series_equal(
         pdu.truncate_datetime_to_freq(x, 'D'),
-        pd.Series(pd.to_datetime(['2023-04-22', '2023-03-01'])))
-    
+        pdu.to_datetime_ser(['2023-04-22', '2023-03-01']))
+
     pd_testing.assert_series_equal(
         pdu.truncate_datetime_to_freq(x, 'M'),
-        pd.Series(pd.to_datetime(['2023-04-01', '2023-03-01'])))
-    
+        pdu.to_datetime_ser(['2023-04-01', '2023-03-01']))
+
     pd_testing.assert_series_equal(
         pdu.truncate_datetime_to_freq(x, 'W'),
-        pd.Series(pd.to_datetime(['2023-04-17', '2023-02-27'])))
+        pdu.to_datetime_ser(['2023-04-17', '2023-02-27']))
 
 
 def test_truncate_datetime_to_month() -> None:
     df = pd.DataFrame({'dt': pd.to_datetime(['2017-09-12', '2017-10-20'])})
-    
+
     df['dtm'] = pdu.truncate_datetime_to_month(df['dt'])
-    
+
     pd_testing.assert_frame_equal(
         df, pdu.from_items([
         ('dt', pd.to_datetime(['2017-09-12', '2017-10-20'])),
         ('dtm', pd.to_datetime(['2017-09-01', '2017-10-01']))]))
 
 
 def test_truncate_datetime_to_week() -> None:
     df = pd.DataFrame({'dt': pd.to_datetime(['2017-09-11', '2017-09-24'])})
-    
+
     df['dtm'] = pdu.truncate_datetime_to_week(df['dt'])
     df['dtm_sun'] = pdu.truncate_datetime_to_week(df['dt'], sunday_first=True)
-    
+
     pd_testing.assert_frame_equal(
         df, pdu.from_items([
             ('dt', pd.to_datetime(['2017-09-11', '2017-09-24'])),
             ('dtm', pd.to_datetime(['2017-09-11', '2017-09-18'])),
             ('dtm_sun', pd.to_datetime(['2017-09-10', '2017-09-24']))
         ]))
 
 
 def test_datetime_to_epoch() -> None:
     pd_testing.assert_series_equal(
         pdu.datetime_to_epoch(
-            pd.Series(pd.to_datetime(["1970-01-01", "1970-01-01 0:01:02.345",
-                                      "NaT"]))),
+            pdu.to_datetime_ser(
+                ["1970-01-01 00:00:00.0", "1970-01-01 0:01:02.345", "NaT"])),
         pd.Series([0., 62.345, nan]), check_exact=True)
-    
+
     pd_testing.assert_series_equal(
         pdu.datetime_to_epoch(
-            pd.Series([pd.to_datetime("1970-01-01 1:00:00")])),
+            pdu.to_datetime_ser(["1970-01-01 1:00:00"])),
         pd.Series([3600.]))
 
 
+def test_convert_to_timezone() -> None:
+    ser = pdu.to_datetime_ser(
+        ['2022-02-01 23:05:00', '2022-06-05 10:20:00'])
+    ser_berlin = pdu.convert_to_timezone(ser, 'Europe/Helsinki')
+    pd_testing.assert_series_equal(
+        ser_berlin.dt.day, pd.Series([2, 5], dtype=np.int32))
+    pd_testing.assert_series_equal(
+        ser_berlin.dt.hour, pd.Series([1, 13], dtype=np.int32))
+    pd_testing.assert_series_equal(
+        ser_berlin.dt.minute, pd.Series([5, 20], dtype=np.int32))
+
+
+def test_add_missing_days_one_level() -> None:
+    df = pdu.from_items([
+        ('date', pd.to_datetime(['2020-02-01', '2020-02-03'])),
+        ('a', [2, 3])
+    ]).set_index('date')
+
+    expd = pdu.from_items([
+        ('date',
+         pd.to_datetime(['2020-02-01', '2020-02-02', '2020-02-03',
+                         '2020-02-04', '2020-02-05'])),
+        ('a', [2, nan, 3, nan, nan])])
+
+    pd_testing.assert_frame_equal(
+        pdu.add_missing_days(df, end_datetime='2020-02-05'),
+        expd)
+
+    pd_testing.assert_frame_equal(
+        pdu.add_missing_days(df, end_datetime='2020-02-05', reset_index=False),
+        expd.set_index('date'))
+
+    pd_testing.assert_frame_equal(
+        pdu.add_missing_days(df),
+        pdu.from_items([
+            ('date',
+             pd.to_datetime(['2020-02-01', '2020-02-02', '2020-02-03'])),
+            ('a', [2, nan, 3])]))
+
+
+def test_add_missing_days_multiple_levels() -> None:
+    df = pdu.from_items([
+        ('a', [0, 0, 0, 1, 1]),
+        ('date',
+         pd.to_datetime([
+             '2023-07-03', '2023-07-03', '2023-07-17',
+             '2023-07-03', '2023-07-17'])),
+        ('c', [5, 6, 5, 5, 6]),
+        ('d', [10, 11, 12, 13, 14])
+    ]).set_index(['a', 'date', 'c'])
+
+    print(
+        pdu.add_missing_days(df, '2023-07-31', freq='W-MON'))
+    pd_testing.assert_frame_equal(
+        pdu.add_missing_days(df, '2023-07-31', freq='W-MON'),
+        pdu.from_items([
+            ('a', [0] * 10 + [1] * 10),
+            ('date',
+             pd.to_datetime((
+                 ['2023-07-03'] * 2 + ['2023-07-10'] * 2 + ['2023-07-17'] * 2
+                 + ['2023-07-24'] * 2 + ['2023-07-31'] * 2
+             ) * 2)),
+            ('c', [5, 6] * 10),
+            ('d', [10, 11, nan, nan, 12, nan, nan, nan, nan, nan,
+                   13, nan, nan, nan, nan, 14, nan, nan, nan, nan]),
+        ]))
+
+
 def test_to_csv() -> None:
     df = pdu.from_items([
         ('b', np.array([3, 8])),
         ('a', ['first', 'second']),
     ], index=[3, 4])
 
     out = io.StringIO()
     pdu.to_csv(df, out)
 
     assert out.getvalue() == "b;a\n3;first\n8;second\n"
+
+
```

### Comparing `mlpj-0.2.3/test/test_python_utils.py` & `mlpj-0.2.4/test/test_python_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import sys
 import collections
 import io
 import tempfile
 import datetime
 
+import pytest
+
 from mlpj import python_utils as pu
 
 
 def test_all_except() -> None:
     lst = ['x', 'a', 'ba', 'a', 'c']
     assert pu.all_except(lst, ['a', 'c']) == ['x', 'ba']
 
@@ -37,15 +39,15 @@
 def test_perc_str() -> None:
     assert pu.perc_str(6, 10) == "6 (60.00 %)"
 
 
 def test_first_of_each_item() -> None:
     assert pu.first_of_each_item([('a', 3, 9), ('b', 4), ('c',)]) == [
         'a', 'b', 'c']
-    
+
     assert (
         pu.first_of_each_item(collections.OrderedDict([('A', 3), ('B', 4)])
                               .items())
         == ['A', 'B'])
 
 
 def test_mkdir_unless_exists() -> None:
@@ -61,15 +63,24 @@
     assert pu.make_path_relative_to('/ab/cd/d/e', '/ab/cd') == 'd/e'
     assert pu.make_path_relative_to('/ab/cd/d/e', '/ab/cd/d2') == '../d/e'
     assert pu.make_path_relative_to('/abd/cd/d/e', '/ab/cd/d2') == (
         '../../../abd/cd/d/e')
 
     assert pu.make_path_relative_to('/ab//cd//d/e/', '/ab//cd/') == 'd/e'
     assert pu.make_path_relative_to('/ab//cd//d/e/', '/ab//cd//d2') == '../d/e'
-    
+
+
+@pytest.mark.parametrize('filename, filepath, xpd', [
+    ('bar.txt', 'foo/xx', 'foo/bar.txt'),
+    ('bar.txt', '/foo/xx', '/foo/bar.txt'),
+    ('bar.txt', '/', '/bar.txt'),
+])
+def test_filepath_in_dir_of(filename: str, filepath: str, xpd: str) -> None:
+    assert pu.filepath_in_dir_of(filename, filepath) == xpd
+
 
 def test_redirect_stdouterr() -> None:
     out = io.StringIO()
     err = io.StringIO()
     with pu.redirect_stdouterr(out, err):
         print("foo")
         print("bar", file=sys.stderr)
@@ -91,33 +102,33 @@
 
     stream.close()
 
 
 def test_open_overwriting_safely() -> None:
     with tempfile.TemporaryDirectory() as tmpdir:
         filepath = os.path.join(tmpdir, 'foo.txt')
-        
+
         original_output = "foo\nbar\n"
         with open(filepath, 'w') as fout:
             fout.write(original_output)
 
         def contents(filepath):
             with open(filepath) as fin:
                 return fin.read()
-            
+
         new_output = "new output\n"
         try:
             with pu.open_overwriting_safely(filepath, 'w') as fout:
                 fout.write(new_output)
                 raise ValueError()
         except ValueError:
             pass
 
         assert contents(filepath) == original_output
-        
+
         with pu.open_overwriting_safely(filepath, 'w') as fout:
             fout.write(new_output)
         assert contents(filepath) == new_output
 
 
 def test_ansiicol() -> None:
     assert pu.ansiicol(31) == "\x1b[31m"
@@ -131,10 +142,24 @@
 
 
 def test_n_days_ago() -> None:
     today = datetime.date.today()
     assert (today - pu.n_days_ago(5)) == datetime.timedelta(days=5)
 
 
+def test_n_days_from_today() -> None:
+    today = datetime.date.today()
+    assert (pu.n_days_from_today(5) - today) == datetime.timedelta(days=5)
+
+
 def test_today_isoformat() -> None:
     today = datetime.date.today()
     assert pu.today_isoformat() == today.strftime("%Y-%m-%d")
+
+
+@pytest.mark.parametrize('input, xpd', [
+    ('line1\n   |line2\n\t  |line3\n  line4',
+     'line1\nline2\nline3\n  line4'),
+    ('', ''),
+])
+def test_strip_margin(input: str, xpd: str) -> None:
+    assert pu.strip_margin(input) == xpd
```

### Comparing `mlpj-0.2.3/test/test_result_display.py` & `mlpj-0.2.4/test/test_result_display.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.3/test/test_timeseries_utils.py` & `mlpj-0.2.4/test/test_timeseries_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 from mlpj import pandas_utils as pdu
 from mlpj import timeseries_utils as tsu
 
 
 def test_remove_last_n_days() -> None:
     df = pdu.from_items([
         ('date', pd.to_datetime(
-            [pu.n_days_ago(20), pu.n_days_ago(5), pu.n_days_ago(10)])),
-        ('a', [2, 3, 1])
+            [pu.n_days_ago(20), pu.n_days_ago(5), pu.n_days_ago(10),
+             pu.n_days_from_today(5)])),
+        ('a', [2, 3, 1, 8])
     ])
-    
+
     df1 = tsu.remove_last_n_days(df, 'date', 10)
     pdu.assert_frame_contents_equal(
         df1,
         pdu.from_items([
             ('date', pd.to_datetime([pu.n_days_ago(20), pu.n_days_ago(10)])),
             ('a', [2, 1])
         ]))
 
-    
+
 def test_ts_train_test_split() -> None:
     df = pdu.from_items([
         ('date', pd.to_datetime(['2023-03-05', '2023-01-15', '2023-02-01'])),
         ('a', [2, 3, 1]),
         ('y', [0, 1, -1]),
     ])
```

