# Comparing `tmp/piso-0.9.0.tar.gz` & `tmp/piso-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piso-0.9.0.tar", max compression
+gzip compressed data, was "piso-1.0.0.tar", max compression
```

## Comparing `piso-0.9.0.tar` & `piso-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1069 2022-05-04 13:48:42.664434 piso-0.9.0/LICENSE
--rw-r--r--   0        0        0     4229 2022-05-04 13:48:42.668434 piso-0.9.0/README.md
--rw-r--r--   0        0        0     1641 2022-05-04 13:48:42.672434 piso-0.9.0/piso/__init__.py
--rw-r--r--   0        0        0     1680 2022-05-04 13:48:42.672434 piso-0.9.0/piso/_decorators.py
--rw-r--r--   0        0        0      863 2022-05-04 13:48:42.672434 piso-0.9.0/piso/_exceptions.py
--rw-r--r--   0        0        0     6178 2022-05-04 13:48:42.672434 piso-0.9.0/piso/accessor.py
--rw-r--r--   0        0        0    28657 2022-05-04 13:48:42.672434 piso-0.9.0/piso/docstrings/accessor.py
--rw-r--r--   0        0        0     5798 2022-05-04 13:48:42.672434 piso-0.9.0/piso/docstrings/interval.py
--rw-r--r--   0        0        0    27007 2022-05-04 13:48:42.672434 piso-0.9.0/piso/docstrings/intervalarray.py
--rw-r--r--   0        0        0     4368 2022-05-04 13:48:42.672434 piso-0.9.0/piso/docstrings/ndframe.py
--rw-r--r--   0        0        0     6419 2022-05-04 13:48:42.672434 piso-0.9.0/piso/graph.py
--rw-r--r--   0        0        0     4884 2022-05-04 13:48:42.672434 piso-0.9.0/piso/interval.py
--rw-r--r--   0        0        0    10344 2022-05-04 13:48:42.672434 piso-0.9.0/piso/intervalarray.py
--rw-r--r--   0        0        0     4502 2022-05-04 13:48:42.672434 piso-0.9.0/piso/ndframe.py
--rw-r--r--   0        0        0      943 2022-05-04 13:48:42.672434 piso-0.9.0/piso/util.py
--rw-r--r--   0        0        0     2067 2022-05-04 13:48:42.672434 piso-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5161 2022-05-04 13:49:55.610983 piso-0.9.0/setup.py
--rw-r--r--   0        0        0     5579 2022-05-04 13:49:55.611535 piso-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-06 11:09:44.246183 piso-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4229 2023-07-06 11:09:44.246183 piso-1.0.0/README.md
+-rw-r--r--   0        0        0     1641 2023-07-06 11:09:44.254183 piso-1.0.0/piso/__init__.py
+-rw-r--r--   0        0        0     1680 2023-07-06 11:09:44.254183 piso-1.0.0/piso/_decorators.py
+-rw-r--r--   0        0        0      863 2023-07-06 11:09:44.254183 piso-1.0.0/piso/_exceptions.py
+-rw-r--r--   0        0        0     6178 2023-07-06 11:09:44.254183 piso-1.0.0/piso/accessor.py
+-rw-r--r--   0        0        0    28590 2023-07-06 11:09:44.254183 piso-1.0.0/piso/docstrings/accessor.py
+-rw-r--r--   0        0        0     5774 2023-07-06 11:09:44.254183 piso-1.0.0/piso/docstrings/interval.py
+-rw-r--r--   0        0        0    26941 2023-07-06 11:09:44.254183 piso-1.0.0/piso/docstrings/intervalarray.py
+-rw-r--r--   0        0        0     4357 2023-07-06 11:09:44.254183 piso-1.0.0/piso/docstrings/ndframe.py
+-rw-r--r--   0        0        0     6418 2023-07-06 11:09:44.254183 piso-1.0.0/piso/graph.py
+-rw-r--r--   0        0        0     4884 2023-07-06 11:09:44.254183 piso-1.0.0/piso/interval.py
+-rw-r--r--   0        0        0    10523 2023-07-06 11:09:44.254183 piso-1.0.0/piso/intervalarray.py
+-rw-r--r--   0        0        0     4502 2023-07-06 11:09:44.254183 piso-1.0.0/piso/ndframe.py
+-rw-r--r--   0        0        0      943 2023-07-06 11:09:44.254183 piso-1.0.0/piso/util.py
+-rw-r--r--   0        0        0     2344 2023-07-06 11:09:44.258183 piso-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5901 1970-01-01 00:00:00.000000 piso-1.0.0/PKG-INFO
```

### Comparing `piso-0.9.0/LICENSE` & `piso-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/README.md` & `piso-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/piso/__init__.py` & `piso-1.0.0/piso/__init__.py`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/piso/_decorators.py` & `piso-1.0.0/piso/_decorators.py`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/piso/_exceptions.py` & `piso-1.0.0/piso/_exceptions.py`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/piso/accessor.py` & `piso-1.0.0/piso/accessor.py`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/piso/docstrings/accessor.py` & `piso-1.0.0/piso/docstrings/accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from piso.graph import adjacency_matrix
 
 union_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 
 Examples with *interval_arrays* empty:
@@ -65,15 +65,15 @@
 
 >>> arr1.piso.union(arr2, arr3, squeeze=True)
 Interval(0.0, 12.0, closed='right')
 """
 
 intersection_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 
 Examples with *interval_arrays* empty:
@@ -145,15 +145,15 @@
 <IntervalArray>
 [(3.0, 4.0], (10.0, 11.0]]
 Length: 2, closed: right, dtype: interval[float64]
 """
 
 difference_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
@@ -188,15 +188,15 @@
 
 >>> arr1.piso.difference(arr2, arr3, squeeze=True)
 Interval(0.0, 2.0, closed='right')
 """
 
 symmetric_difference_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 
 Examples with *interval_arrays* empty:
@@ -257,15 +257,15 @@
 [(0.0, 12.0]]
 Length: 1, closed: right, dtype: interval[float64]
 """
 
 
 isdisjoint_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 3), (2, 4)],
@@ -288,15 +288,15 @@
 
 >>> arr1.piso.isdisjoint(arr3)
 False
 """
 
 issuperset_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 6), (7, 8), (10, 12)],
@@ -320,15 +320,15 @@
 >>> arr2.piso.issuperset(arr3)
 False
 """
 
 
 issubset_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(2, 5), (7, 8)],
@@ -402,15 +402,15 @@
 
 {extra_desc}
 Parameters
 ----------
 {params}
 
 Returns
-----------
+-------
 {return_type}
 
 {examples}
 """
 
 operation_template_doc = (
     """
@@ -435,15 +435,15 @@
 
 {extra_desc}
 Parameters
 ----------
 {params}
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
 
 {examples}
 """
 
 is_super_sub_set_template = """
 Indicates whether a set is a {operation} of one, or more, other sets.
@@ -459,15 +459,15 @@
 a single boolean using the *squeeze* parameter.
 
 Parameters
 ----------
 {params}
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
 
 {examples}
 """
 
 array_return_type = (
     ":class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`"
@@ -613,19 +613,19 @@
 how : {"fraction", "sum"}, default "fraction"
     If *how* = "fraction" then the result is a fraction of the size of the domain.
     If *how* = "sum" then the result is the length of the domain covered.
 
     .. versionadded:: 0.8.0
 
 Returns
-----------
+-------
 float or :class:`pandas.Series`
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 5), (7, 8)],
@@ -672,20 +672,20 @@
     Specifies the domain over which to calculate the "complement".  If *domain* is `None`,
     then the domain is considered to be the extremities of the intervals contained in the interval array
     that the accessor belongs to. If *domain* is a tuple then it should specify lower and upper bounds, and be equivalent to a
     :class:`pandas.Interval`.  If *domain* is a :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     then the intervals it contains define a possibly disconnected domain.
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     The return type will be the same as the interval array object the accessor belongs to.
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 5), (7, 8)],
 ... )
@@ -724,21 +724,21 @@
 Parameters
 ----------
 x : scalar, or array-like of scalars
     Values in *x* should belong to the same domain as the intervals contained in the interval array
     that the accessor belongs to.
 
 Returns
-----------
+-------
 :class:`numpy.ndarray`
     Values will be integer.  If a point is not contained in any interval then the corresponding
     value is -1.
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (6, 8), (10, 12)],
@@ -785,20 +785,20 @@
 how : {"any", "all"}, default "any"
     Only relevant if *result* is not "cartesian".  This parameter indicates either:
     - a True value means any or all points are contained within an interval, or
     - a True value means any or all intervals contained a point.
     Which of these interpretations is dependent on the *result* parameter.
 
 Returns
-----------
+-------
 :class:`numpy.ndarray`, :class:`pandas.DataFrame` or :class:`pandas.Series`
     One, or two, dimensional and boolean valued.  Return type dependent on *include_index* and *result*.
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (2, 5)],
@@ -852,20 +852,20 @@
 Parameters
 ----------
 x : scalar, or array-like of scalars
     Values in *x* should belong to the same domain as the intervals in *interval_array*.
     May contain duplicates and be unsorted.
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     Return type will be the same type as the object the accessor belongs to.
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (2, 5)],
@@ -910,15 +910,15 @@
 
 Returns
 -------
 :class:`pandas.DataFrame` or :class:`numpy.ndarray`
     Boolean valued, symmetrical, with False along diagonal.
 
 Examples
----------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...    [(0,4), (3,6), (5, 7), (8,9), (9,10)],
@@ -960,21 +960,21 @@
 Parameters
 ----------
 threshold : scalar
     The value should belong to the domain that arises from a subtraction over the domain of the intervals.
     For instance, if intervals are timestamp data, then *threshold* should be timedelta.
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     Return type will be the same type as the object the accessor belongs to.
 
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 >>> piso.register_accessors()
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 5), (7, 8), (11, 12)],
```

### Comparing `piso-0.9.0/piso/docstrings/interval.py` & `piso-1.0.0/piso/docstrings/interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 union_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso.interval
 
 >>> piso.interval.union(
 ...    pd.Interval(0, 3),
 ...    pd.Interval(2, 4),
@@ -33,15 +33,15 @@
 <IntervalArray>
 [(0.0, 1.0], (3.0, 4.0]]
 Length: 2, closed: right, dtype: interval[float64]
 """
 
 intersection_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso.interval
 
 >>> piso.interval.intersection(
 ...    pd.Interval(0, 3),
 ...    pd.Interval(2, 4),
@@ -70,15 +70,15 @@
 <IntervalArray>
 []
 Length: 0, closed: right, dtype: interval[int64]
 """
 
 difference_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso.interval
 
 >>> piso.interval.difference(
 ...    pd.Interval(0, 3),
 ...    pd.Interval(2, 4),
@@ -110,15 +110,15 @@
 []
 Length: 0, closed: right, dtype: interval[int64]
 """
 
 
 symmetric_difference_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso.interval
 
 >>> piso.interval.symmetric_difference(
 ...    pd.Interval(0, 3),
 ...    pd.Interval(2, 4),
@@ -148,15 +148,15 @@
 <IntervalArray>
 [(0.0, 2.0], (3.0, 4.0]]
 Length: 2, closed: right, dtype: interval[float64]
 """
 
 issuperset_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso.interval
 
 >>> piso.interval.issuperset(
 ...    pd.Interval(1, 4),
 ...    pd.Interval(2, 4),
@@ -183,15 +183,15 @@
 ... )
 array([ True])
 """
 
 
 issubset_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso.interval
 
 >>> piso.interval.issubset(
 ...    pd.Interval(2, 4),
 ...    pd.Interval(1, 4),
@@ -228,15 +228,15 @@
     the first operand
 interval2 : pandas.Interval
     the second operand
 squeeze : boolean, default True
     If True, will try to coerce the return value to a :class:`pandas.Interval`
 
 Returns
-----------
+-------
 :class:`pandas.Interval` or :class:`pandas.arrays.IntervalArray`
 
 {examples}
 """
 
 
 union_docstring = template_doc.format(operation="union", examples=union_examples)
@@ -260,15 +260,15 @@
     An interval, against which all other intervals belonging to *intervals* are compared.
 *intervals : argument list of :class:`pandas.Interval`
     Must contain at least one argument.
 squeeze : boolean, default True
     If True, will try to coerce the return value to a single boolean
 
 Returns
-----------
+-------
 boolean, or :class:`numpy.ndarray` of booleans
 
 {examples}
 """
 
 issuperset_docstring = is_sub_super_doc.format(
     operation="superset",
```

### Comparing `piso-0.9.0/piso/docstrings/intervalarray.py` & `piso-1.0.0/piso/docstrings/intervalarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 union_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 
 Examples with *interval_arrays* empty:
 
@@ -62,15 +62,15 @@
 
 >>> piso.union(arr1, arr2, arr3, squeeze=True)
 Interval(0.0, 12.0, closed='right')
 """
 
 intersection_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 Examples with *interval_arrays* empty:
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
@@ -131,15 +131,15 @@
 <IntervalArray>
 [(3.0, 4.0], (10.0, 11.0]]
 Length: 2, closed: right, dtype: interval[float64]
 """
 
 difference_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (2, 5), (3, 6), (7, 8), (8, 9), (10, 12)],
 ... )
@@ -172,15 +172,15 @@
 
 >>> piso.difference(arr1, arr2, arr3, squeeze=True)
 Interval(0.0, 2.0, closed='right')
 """
 
 symmetric_difference_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 Examples with *interval_arrays* empty:
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
@@ -239,15 +239,15 @@
 [(0.0, 12.0]]
 Length: 1, closed: right, dtype: interval[float64]
 """
 
 
 isdisjoint_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 3), (2, 4)],
 ... )
@@ -270,15 +270,15 @@
 >>> piso.isdisjoint(arr1, arr3)
 False
 """
 
 
 issuperset_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 6), (7, 8), (10, 12)],
 ... )
@@ -301,15 +301,15 @@
 >>> piso.issuperset(arr2, arr3)
 False
 """
 
 
 issubset_examples = """
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(2, 5), (7, 8)],
 ... )
@@ -396,15 +396,15 @@
 
 {extra_desc}
 Parameters
 ----------
 {params}
 
 Returns
-----------
+-------
 {return_type}
 
 {examples}
 """
 
 
 operation_template_doc = (
@@ -429,15 +429,15 @@
 
 {extra_desc}
 Parameters
 ----------
 {params}
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
 
 {examples}
 """
 
 doc_is_sub_super_set_template = """
 Indicates whether a set is a {operation} of one, or more, other sets.
@@ -453,15 +453,15 @@
 
 {extra_desc}
 Parameters
 ----------
 {params}
 
 Returns
-----------
+-------
 boolean, or :class:`numpy.ndarray` of boolean
 
 {examples}
 """
 
 
 array_return_type = (
@@ -618,19 +618,19 @@
 how : {"fraction", "sum"}, default "fraction"
     If *how* = "fraction" then the result is a fraction of the size of the domain.
     If *how* = "sum" then the result is the length of the domain covered.
 
     .. versionadded:: 0.8.0
 
 Returns
-----------
+-------
 float or :class:`pandas.Series`
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 5), (7, 8)],
 ... )
@@ -678,20 +678,20 @@
     Specifies the domain over which to calculate the "complement".  If *domain* is `None`,
     then the domain is considered to be the extremities of the intervals contained in *interval_array*
     If *domain* is a tuple then it should specify lower and upper bounds, and be equivalent to a
     :class:`pandas.Interval`.  If *domain* is a :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     then the intervals it contains define a possibly disconnected domain.
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     The return type will be the same as *interval_array*.
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr1 = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 5), (7, 8)],
 ... )
@@ -732,21 +732,21 @@
 ----------
 interval_array : :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     Contains the disjoint intervals.
 x : scalar, or array-like of scalars
     Values in *x* should belong to the same domain as the intervals in *interval_array*.
 
 Returns
-----------
+-------
 :class:`numpy.ndarray`
     Values will be integer.  If a point is not contained in any interval then the corresponding
     value is -1.
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (6, 8), (10, 12)],
 ... )
@@ -792,20 +792,20 @@
     Only relevant if *result* is not "cartesian".  This parameter indicates either:
     - a True value means any or all points are contained within an interval, or
     - a True value means any or all intervals contained a point.
     Which of these interpretations is dependent on the *result* parameter.
 
 
 Returns
-----------
+-------
 :class:`numpy.ndarray`, :class:`pandas.DataFrame` or :class:`pandas.Series`
     One, or two, dimensional and boolean valued.  Return type dependent on *include_index* and *result*.
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (2, 5)],
 ... )
@@ -856,20 +856,20 @@
 interval_array : :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     Contains the (possibly overlapping) intervals.  May be left-closed, right-closed, both, or neither.
 x : scalar, or array-like of scalars
     Values in *x* should belong to the same domain as the intervals in *interval_array*.
     May contain duplicates and be unsorted.
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     Return type will be the same type as *interval_array*
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (2, 5)],
 ... )
@@ -907,21 +907,21 @@
 interval_array : :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     Contains the (possibly overlapping) intervals.  May be left-closed or right-closed.
 threshold : scalar
     The value should belong to the domain that arises from a subtraction over the domain of the intervals.
     For instance, if intervals are timestamp data, then *threshold* should be timedelta.
 
 Returns
-----------
+-------
 :class:`pandas.IntervalIndex` or :class:`pandas.arrays.IntervalArray`
     Return type will be the same type as the object the accessor belongs to.
 
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (3, 5), (7, 8), (11, 12)],
 ... )
```

### Comparing `piso-0.9.0/piso/docstrings/ndframe.py` & `piso-1.0.0/piso/docstrings/ndframe.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 ----------
 frame_or_series : :class:`pandas.DataFrame` or :class:`pandas.Series`
     Must be indexed by a :class:`pandas.IntervalIndex` containing disjoint intervals
 x : scalar, or array-like of scalars
     Values in *x* should belong to the same domain as the intervals in the interval index.
 
 Returns
-----------
+-------
 :class:`pandas.DataFrame` or :class:`pandas.Series`
     Will be the same type as *frame_or_series*
 
 Examples
------------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> arr = pd.arrays.IntervalArray.from_tuples(
 ...     [(0, 4), (6, 8), (10, 12)],
 ... )
@@ -73,20 +73,20 @@
     What sort of join to perform.
 suffixes : list of str or None, default None
     Suffixes to use for overlapping columns.  If used then should be same length as *frames_or_series*.
 sort : bool, default False
     Order result DataFrame lexicographically by the join key. If False, the order of the join key depends on the join type.
 
 Returns
-----------
+-------
 :class:`pandas.DataFrame`
     A dataframe containing columns from elements of *frames_or_series*
 
 Examples
-----------
+--------
 
 >>> import pandas as pd
 >>> import piso
 
 >>> df = pd.DataFrame(
 ...     {"A":[4,3], "B":["x","y"]},
 ...     index=pd.IntervalIndex.from_tuples([(1,3), (5,7)]),
```

### Comparing `piso-0.9.0/piso/graph.py` & `piso-1.0.0/piso/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     Returns
     -------
     :class:`pandas.DataFrame` or :class:`numpy.ndarray`
         Boolean valued, symmetrical, with False along diagonal.
 
     Examples
-    ---------
+    --------
 
     >>> import pandas as pd
     >>> import piso
 
     >>> arr = pd.arrays.IntervalArray.from_tuples(
     ...    [(0,4), (3,6), (5, 7), (8,9), (9,10)],
     ...    closed="both",
```

### Comparing `piso-0.9.0/piso/interval.py` & `piso-1.0.0/piso/interval.py`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/piso/intervalarray.py` & `piso-1.0.0/piso/intervalarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,17 @@
     _boolean_stairs_to_interval_array,
     _interval_x_to_stairs,
     _validate_intervals,
 )
 
 
 def _check_matched_closed(interval_arrays):
-    closed_values = [arr.closed for arr in interval_arrays]
-    assert closed_values.count(closed_values[0]) == len(closed_values)
+    closed_values = [arr.closed for arr in interval_arrays if len(arr) > 0]
+    if len(closed_values):
+        assert closed_values.count(closed_values[0]) == len(closed_values)
 
 
 def _validate_array_of_intervals_arrays(*interval_arrays, validate_intervals=True):
     assert len(interval_arrays) > 0
     _check_matched_closed(interval_arrays)
     if validate_intervals:
         for arr in interval_arrays:
@@ -242,21 +243,27 @@
             index = x if result == "points" else interval_array
             calc = pd.Series(calc, index=index)
     return calc
 
 
 @Appender(docstrings.split_docstring, join="\n", indents=1)
 def split(interval_array, x):
-    # x = pd.Series(x).values
     x = pd.Series(sorted(set(x))).values  # converting to numpy array will not work
     contained = contains(interval_array.set_closed("neither"), x, include_index=False)
+
+    none = np.nan
+    if pd.api.types.is_datetime64_any_dtype(x) or pd.api.types.is_timedelta64_dtype(x):
+        none = pd.NaT
+
     breakpoints = np.concatenate(
         (
             np.expand_dims(interval_array.left.values, 1),
-            pd.DataFrame(np.broadcast_to(x, contained.shape)).where(contained).values,
+            pd.DataFrame(np.broadcast_to(x, contained.shape))
+            .where(contained, none)
+            .values,
             np.expand_dims(interval_array.right.values, 1),
         ),
         axis=1,
     )
     lefts = breakpoints[:, :-1]
     rights = breakpoints[:, 1:]
     return interval_array.from_arrays(
```

### Comparing `piso-0.9.0/piso/ndframe.py` & `piso-1.0.0/piso/ndframe.py`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/piso/util.py` & `piso-1.0.0/piso/util.py`

 * *Files identical despite different names*

### Comparing `piso-0.9.0/pyproject.toml` & `piso-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "piso"
-version = "0.9.0"
+version = "1.0.0"
 description = "Pandas Interval Set Operations: methods for set operations, analytics, lookups and joins on pandas' Interval, IntervalArray and IntervalIndex"
 readme = "README.md"
 authors = ["Riley Clement <venaturum@gmail.com>"]
 maintainers = ["Riley Clement <venaturum@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/staircase-dev/piso"
 homepage = "https://github.com/staircase-dev/piso"
@@ -28,44 +28,59 @@
 	'Analysis',
 	'Data Structures',
 ]
 
 classifiers=[
 	'Operating System :: OS Independent',
 	'Intended Audience :: Science/Research',
-	'Programming Language :: Python :: 3.6',
 	'Programming Language :: Python :: 3.7',
 	'Programming Language :: Python :: 3.8',
 	'Programming Language :: Python :: 3.9',
+	'Programming Language :: Python :: 3.10',
+	'Programming Language :: Python :: 3.11',
 	'Topic :: Scientific/Engineering',
 ]
 
+
 [tool.poetry.dependencies]
-python = "^3.6.1"
+python = "^3.7"
 staircase = "^2.1.0"
-pandas = "^1"
 
+[[tool.poetry.dependencies.pandas]]
+python = ">=3.7,<3.10"
+version = "^1"
+
+[[tool.poetry.dependencies.pandas]]
+python = "^3.10"
+version = ">=1.3.4,<3"
+
+[[tool.poetry.dependencies.numpy]]
+python = ">=3.7,<3.10"
+version = "^1.15"
+
+[[tool.poetry.dependencies.numpy]]
+python = "^3.10"
+version = "^1.21.2"
 
 
 [tool.poetry.dev-dependencies]
-ipykernel = "^5"
+ipykernel = "^6"
 pytest = "^6"
 pytest-cov = "*"
 sphinx = "*"
 nbsphinx = ">=0.8.5"
 sphinx-autobuild = "*"
 numpydoc = "*"
 notebook = ">= 6.0"
-isort = ">=5.8"
-black = {version = "*", python = "^3.6.2"}
-flake8 = ">=3.9"
-pre-commit = {version = ">=2.13", python = "^3.6.1"}
+isort = ">=5.8,<5.12"
+black = ">=22.10"
+flake8 = ">=5"
+pre-commit = ">=2.20"
 tox=">=3.15"
 
-
 [tool.poetry.extras]
 codecov = ["codecov"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/staircase-dev/piso/issues"
 
 [tool.isort]
```

### Comparing `piso-0.9.0/setup.py` & `piso-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: piso
+Version: 1.0.0
+Summary: Pandas Interval Set Operations: methods for set operations, analytics, lookups and joins on pandas' Interval, IntervalArray and IntervalIndex
+Home-page: https://github.com/staircase-dev/piso
+License: MIT
+Keywords: piso,pandas,set,set operations,interval,IntervalArray,IntervalIndex,Data Analysis,Analysis,Data Structures
+Author: Riley Clement
+Author-email: venaturum@gmail.com
+Maintainer: Riley Clement
+Maintainer-email: venaturum@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Provides-Extra: codecov
+Requires-Dist: numpy (>=1.15,<2.0) ; python_version >= "3.7" and python_version < "3.10"
+Requires-Dist: numpy (>=1.21.2,<2.0.0) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: pandas (>=1,<2) ; python_version >= "3.7" and python_version < "3.10"
+Requires-Dist: pandas (>=1.3.4,<3) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: staircase (>=2.1.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/staircase-dev/piso/issues
+Project-URL: Documentation, https://piso.readthedocs.io
+Project-URL: Repository, https://github.com/staircase-dev/piso
+Description-Content-Type: text/markdown
+
+<p align="center"><a href="https://github.com/staircase-dev/piso"><img src="https://github.com/staircase-dev/piso/blob/master/docs/img/piso_social_transparent.svg" title="piso logo" alt="piso logo"></a></p>
+
+<p align="center">
+    <a href="https://www.python.org/" alt="Python version">
+        <img src="https://img.shields.io/pypi/pyversions/piso" /></a>
+    <a href="https://pypi.org/project/piso/" alt="PyPI version">
+        <img src="https://img.shields.io/pypi/v/piso" /></a>
+    <a href="https://anaconda.org/conda-forge/piso" alt="Conda Forge version">
+        <img src="https://anaconda.org/conda-forge/piso/badges/version.svg?branch=master&kill_cache=1" /></a>
+	<a href="https://github.com/staircase-dev/piso/actions/workflows/ci.yml" alt="Github CI">
+		<img src="https://github.com/staircase-dev/piso/actions/workflows/ci.yml/badge.svg"/></a>
+    <a href="https://piso.readthedocs.io" alt="Documentation">
+        <img src="https://readthedocs.org/projects/piso/badge/?version=latest" /></a>
+</p>
+
+# piso - pandas interval set operations
+
+**piso** exists to bring set operations (union, intersection, difference + more), analytical methods, and lookup and join functionality to [pandas'](https://pandas.pydata.org/) interval classes, specifically
+
+    - pandas.Interval
+    - pandas.arrays.IntervalArray
+    - pandas.IntervalIndex
+
+Currently, there is a lack of such functionality in pandas, although it has been earmarked for development.  Until this eventuates, piso aims to fill the void.  Many of the methods can be used via accessors, which can be registered to `pandas.arrays.IntervalArray` and `pandas.IntervalIndex` classes, for example:
+
+```python
+>>> import pandas as pd
+>>> import piso
+>>> piso.register_accessors()
+
+>>> arr = pd.arrays.IntervalArray.from_tuples(
+...        [(1,5), (3,6), (2,4)]
+...    )
+
+>>> arr.piso.intersection()
+<IntervalArray>
+[(3, 4]]
+Length: 1, closed: right, dtype: interval[int64]
+
+>>> arr.piso.contains([2, 3, 5])
+            2      3      5
+(1, 5]   True   True   True
+(3, 6]  False  False   True
+(2, 4]  False   True  False
+
+>>> df = pd.DataFrame(
+...     {"A":[4,3], "B":["x","y"]},
+...     index=pd.IntervalIndex.from_tuples([(1,3), (5,7)]),
+... )
+
+>>> s = pd.Series(
+...     [True, False],
+...     index=pd.IntervalIndex.from_tuples([(2,4), (5,6)]),
+...     name="C",
+... )
+
+>>> piso.join(df, s)
+        A  B      C
+(1, 2]  4  x    NaN
+(2, 3]  4  x   True
+(5, 6]  3  y  False
+(6, 7]  3  y    NaN
+
+>>> piso.join(df, s, how="inner")
+        A  B      C
+(2, 3]  4  x   True
+(5, 6]  3  y  False
+```
+
+The domain of the intervals can be either numerical, `pandas.Timestamp` or `pandas.Timedelta`.
+
+Several [case studies](https://piso.readthedocs.io/en/latest/user_guide/case_studies/index.html) using piso can be found in the [user guide](https://piso.readthedocs.io/en/latest/user_guide/index.html).  Further examples, and a detailed explanation of functionality, are provided in the [API reference](https://piso.readthedocs.io/en/latest/reference/index.html).
+
+Visit [https://piso.readthedocs.io](https://piso.readthedocs.io/) for the documentation.
+
+## Installation
+
+`piso` can be installed from PyPI or Anaconda.
+
+To install the latest version from PyPI::
+
+```sh
+python -m pip install piso
+```
+
+To install the latest version through conda-forge::
+
+```sh
+conda install -c conda-forge piso
+```
+
+## Versioning
+
+[SemVer](http://semver.org/) is used by piso for versioning releases.  For versions available, see the [tags on this repository](https://github.com/staircase-dev/piso/tags).
+
+## License
+
+This project is licensed under the [MIT License](https://github.com/staircase-dev/piso/blob/master/LICENSE)
 
-packages = \
-['piso', 'piso.docstrings']
+## Acknowledgments
 
-package_data = \
-{'': ['*']}
+Currently, piso is a pure-python implentation which relies heavily on [staircase](https://www.staircase.dev) and [pandas](https://pandas.pydata.org/).  It is designed to operate as part of the *pandas ecosystem*.  The colours for the piso logo have been assimilated from pandas as a homage, and is not to intended to imply and affiliation with, or endorsement by, pandas.
 
-install_requires = \
-['pandas>=1,<2', 'staircase>=2.1.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'piso',
-    'version': '0.9.0',
-    'description': "Pandas Interval Set Operations: methods for set operations, analytics, lookups and joins on pandas' Interval, IntervalArray and IntervalIndex",
-    'long_description': '<p align="center"><a href="https://github.com/staircase-dev/piso"><img src="https://github.com/staircase-dev/piso/blob/master/docs/img/piso_social_transparent.svg" title="piso logo" alt="piso logo"></a></p>\n\n<p align="center">\n    <a href="https://www.python.org/" alt="Python version">\n        <img src="https://img.shields.io/pypi/pyversions/piso" /></a>\n    <a href="https://pypi.org/project/piso/" alt="PyPI version">\n        <img src="https://img.shields.io/pypi/v/piso" /></a>\n    <a href="https://anaconda.org/conda-forge/piso" alt="Conda Forge version">\n        <img src="https://anaconda.org/conda-forge/piso/badges/version.svg?branch=master&kill_cache=1" /></a>\n\t<a href="https://github.com/staircase-dev/piso/actions/workflows/ci.yml" alt="Github CI">\n\t\t<img src="https://github.com/staircase-dev/piso/actions/workflows/ci.yml/badge.svg"/></a>\n    <a href="https://piso.readthedocs.io" alt="Documentation">\n        <img src="https://readthedocs.org/projects/piso/badge/?version=latest" /></a>\n</p>\n\n# piso - pandas interval set operations\n\n**piso** exists to bring set operations (union, intersection, difference + more), analytical methods, and lookup and join functionality to [pandas\'](https://pandas.pydata.org/) interval classes, specifically\n\n    - pandas.Interval\n    - pandas.arrays.IntervalArray\n    - pandas.IntervalIndex\n\nCurrently, there is a lack of such functionality in pandas, although it has been earmarked for development.  Until this eventuates, piso aims to fill the void.  Many of the methods can be used via accessors, which can be registered to `pandas.arrays.IntervalArray` and `pandas.IntervalIndex` classes, for example:\n\n```python\n>>> import pandas as pd\n>>> import piso\n>>> piso.register_accessors()\n\n>>> arr = pd.arrays.IntervalArray.from_tuples(\n...        [(1,5), (3,6), (2,4)]\n...    )\n\n>>> arr.piso.intersection()\n<IntervalArray>\n[(3, 4]]\nLength: 1, closed: right, dtype: interval[int64]\n\n>>> arr.piso.contains([2, 3, 5])\n            2      3      5\n(1, 5]   True   True   True\n(3, 6]  False  False   True\n(2, 4]  False   True  False\n\n>>> df = pd.DataFrame(\n...     {"A":[4,3], "B":["x","y"]},\n...     index=pd.IntervalIndex.from_tuples([(1,3), (5,7)]),\n... )\n\n>>> s = pd.Series(\n...     [True, False],\n...     index=pd.IntervalIndex.from_tuples([(2,4), (5,6)]),\n...     name="C",\n... )\n\n>>> piso.join(df, s)\n        A  B      C\n(1, 2]  4  x    NaN\n(2, 3]  4  x   True\n(5, 6]  3  y  False\n(6, 7]  3  y    NaN\n\n>>> piso.join(df, s, how="inner")\n        A  B      C\n(2, 3]  4  x   True\n(5, 6]  3  y  False\n```\n\nThe domain of the intervals can be either numerical, `pandas.Timestamp` or `pandas.Timedelta`.\n\nSeveral [case studies](https://piso.readthedocs.io/en/latest/user_guide/case_studies/index.html) using piso can be found in the [user guide](https://piso.readthedocs.io/en/latest/user_guide/index.html).  Further examples, and a detailed explanation of functionality, are provided in the [API reference](https://piso.readthedocs.io/en/latest/reference/index.html).\n\nVisit [https://piso.readthedocs.io](https://piso.readthedocs.io/) for the documentation.\n\n## Installation\n\n`piso` can be installed from PyPI or Anaconda.\n\nTo install the latest version from PyPI::\n\n```sh\npython -m pip install piso\n```\n\nTo install the latest version through conda-forge::\n\n```sh\nconda install -c conda-forge piso\n```\n\n## Versioning\n\n[SemVer](http://semver.org/) is used by piso for versioning releases.  For versions available, see the [tags on this repository](https://github.com/staircase-dev/piso/tags).\n\n## License\n\nThis project is licensed under the [MIT License](https://github.com/staircase-dev/piso/blob/master/LICENSE)\n\n## Acknowledgments\n\nCurrently, piso is a pure-python implentation which relies heavily on [staircase](https://www.staircase.dev) and [pandas](https://pandas.pydata.org/).  It is designed to operate as part of the *pandas ecosystem*.  The colours for the piso logo have been assimilated from pandas as a homage, and is not to intended to imply and affiliation with, or endorsement by, pandas.\n\nAdditionally, two classes have been borrowed, almost verbatim, from the pandas source code:\n\n    - `pandas.util._decorators.Appender`\n    - `pandas.core.accessor.CachedAccessor`',
-    'author': 'Riley Clement',
-    'author_email': 'venaturum@gmail.com',
-    'maintainer': 'Riley Clement',
-    'maintainer_email': 'venaturum@gmail.com',
-    'url': 'https://github.com/staircase-dev/piso',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.1,<4.0.0',
-}
+Additionally, two classes have been borrowed, almost verbatim, from the pandas source code:
 
-
-setup(**setup_kwargs)
+    - `pandas.util._decorators.Appender`
+    - `pandas.core.accessor.CachedAccessor`
```

#### html2text {}

```diff
@@ -1,61 +1,69 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['piso',
-'piso.docstrings'] package_data = \ {'': ['*']} install_requires = \
-['pandas>=1,<2', 'staircase>=2.1.0,<3.0.0'] setup_kwargs = { 'name': 'piso',
-'version': '0.9.0', 'description': "Pandas Interval Set Operations: methods for
-set operations, analytics, lookups and joins on pandas' Interval, IntervalArray
-and IntervalIndex", 'long_description': '
+Metadata-Version: 2.1 Name: piso Version: 1.0.0 Summary: Pandas Interval Set
+Operations: methods for set operations, analytics, lookups and joins on pandas'
+Interval, IntervalArray and IntervalIndex Home-page: https://github.com/
+staircase-dev/piso License: MIT Keywords: piso,pandas,set,set
+operations,interval,IntervalArray,IntervalIndex,Data Analysis,Analysis,Data
+Structures Author: Riley Clement Author-email: venaturum@gmail.com Maintainer:
+Riley Clement Maintainer-email: venaturum@gmail.com Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering Provides-Extra: codecov Requires-
+Dist: numpy (>=1.15,<2.0) ; python_version >= "3.7" and python_version < "3.10"
+Requires-Dist: numpy (>=1.21.2,<2.0.0) ; python_version >= "3.10" and
+python_version < "4.0" Requires-Dist: pandas (>=1,<2) ; python_version >= "3.7"
+and python_version < "3.10" Requires-Dist: pandas (>=1.3.4,<3) ; python_version
+>= "3.10" and python_version < "4.0" Requires-Dist: staircase (>=2.1.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/staircase-dev/piso/issues Project-
+URL: Documentation, https://piso.readthedocs.io Project-URL: Repository, https:
+//github.com/staircase-dev/piso Description-Content-Type: text/markdown
                                   [piso_logo]
-\n\n
-      \n \n_[https://img.shields.io/pypi/pyversions/piso]\n \n_[https://
-img.shields.io/pypi/v/piso]\n \n_[https://anaconda.org/conda-forge/piso/badges/
-version.svg?branch=master&kill_cache=1]\n\t\n\t\t[https://github.com/staircase-
-  dev/piso/actions/workflows/ci.yml/badge.svg]\n \n_[https://readthedocs.org/
-                    projects/piso/badge/?version=latest]\n
-\n\n# piso - pandas interval set operations\n\n**piso** exists to bring set
-operations (union, intersection, difference + more), analytical methods, and
-lookup and join functionality to [pandas\'](https://pandas.pydata.org/
-) interval classes, specifically\n\n - pandas.Interval\n -
-pandas.arrays.IntervalArray\n - pandas.IntervalIndex\n\nCurrently, there is a
-lack of such functionality in pandas, although it has been earmarked for
-development. Until this eventuates, piso aims to fill the void. Many of the
-methods can be used via accessors, which can be registered to
-`pandas.arrays.IntervalArray` and `pandas.IntervalIndex` classes, for example:
-\n\n```python\n>>> import pandas as pd\n>>> import piso\n>>>
-piso.register_accessors()\n\n>>> arr = pd.arrays.IntervalArray.from_tuples
-(\n... [(1,5), (3,6), (2,4)]\n... )\n\n>>> arr.piso.intersection()\n\n[(3,
-4]]\nLength: 1, closed: right, dtype: interval[int64]\n\n>>> arr.piso.contains(
-[2, 3, 5])\n 2 3 5\n(1, 5] True True True\n(3, 6] False False True\n(2, 4]
-False True False\n\n>>> df = pd.DataFrame(\n... {"A":[4,3], "B":
-["x","y"]},\n... index=pd.IntervalIndex.from_tuples([(1,3), (5,7)]),\n...
-)\n\n>>> s = pd.Series(\n... [True, False],\n...
-index=pd.IntervalIndex.from_tuples([(2,4), (5,6)]),\n... name="C",\n...
-)\n\n>>> piso.join(df, s)\n A B C\n(1, 2] 4 x NaN\n(2, 3] 4 x True\n(5, 6] 3 y
-False\n(6, 7] 3 y NaN\n\n>>> piso.join(df, s, how="inner")\n A B C\n(2, 3] 4 x
-True\n(5, 6] 3 y False\n```\n\nThe domain of the intervals can be either
-numerical, `pandas.Timestamp` or `pandas.Timedelta`.\n\nSeveral [case studies]
-(https://piso.readthedocs.io/en/latest/user_guide/case_studies/index.html)
-using piso can be found in the [user guide](https://piso.readthedocs.io/en/
-latest/user_guide/index.html). Further examples, and a detailed explanation of
-functionality, are provided in the [API reference](https://piso.readthedocs.io/
-en/latest/reference/index.html).\n\nVisit [https://piso.readthedocs.io](https:/
-/piso.readthedocs.io/) for the documentation.\n\n## Installation\n\n`piso` can
-be installed from PyPI or Anaconda.\n\nTo install the latest version from
-PyPI::\n\n```sh\npython -m pip install piso\n```\n\nTo install the latest
-version through conda-forge::\n\n```sh\nconda install -c conda-forge
-piso\n```\n\n## Versioning\n\n[SemVer](http://semver.org/) is used by piso for
-versioning releases. For versions available, see the [tags on this repository]
-(https://github.com/staircase-dev/piso/tags).\n\n## License\n\nThis project is
-licensed under the [MIT License](https://github.com/staircase-dev/piso/blob/
-master/LICENSE)\n\n## Acknowledgments\n\nCurrently, piso is a pure-python
-implentation which relies heavily on [staircase](https://www.staircase.dev) and
-[pandas](https://pandas.pydata.org/). It is designed to operate as part of the
-*pandas ecosystem*. The colours for the piso logo have been assimilated from
-pandas as a homage, and is not to intended to imply and affiliation with, or
-endorsement by, pandas.\n\nAdditionally, two classes have been borrowed, almost
-verbatim, from the pandas source code:\n\n -
-`pandas.util._decorators.Appender`\n - `pandas.core.accessor.CachedAccessor`',
-'author': 'Riley Clement', 'author_email': 'venaturum@gmail.com', 'maintainer':
-'Riley Clement', 'maintainer_email': 'venaturum@gmail.com', 'url': 'https://
-github.com/staircase-dev/piso', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.6.1,<4.0.0', } setup(**setup_kwargs)
+ [https://img.shields.io/pypi/pyversions/piso] [https://img.shields.io/pypi/v/
+             piso] [https://anaconda.org/conda-forge/piso/badges/
+version.svg?branch=master&kill_cache=1] [https://github.com/staircase-dev/piso/
+  actions/workflows/ci.yml/badge.svg] [https://readthedocs.org/projects/piso/
+                            badge/?version=latest]
+# piso - pandas interval set operations **piso** exists to bring set operations
+(union, intersection, difference + more), analytical methods, and lookup and
+join functionality to [pandas'](https://pandas.pydata.org/) interval classes,
+specifically - pandas.Interval - pandas.arrays.IntervalArray -
+pandas.IntervalIndex Currently, there is a lack of such functionality in
+pandas, although it has been earmarked for development. Until this eventuates,
+piso aims to fill the void. Many of the methods can be used via accessors,
+which can be registered to `pandas.arrays.IntervalArray` and
+`pandas.IntervalIndex` classes, for example: ```python >>> import pandas as pd
+>>> import piso >>> piso.register_accessors() >>> arr =
+pd.arrays.IntervalArray.from_tuples( ... [(1,5), (3,6), (2,4)] ... ) >>>
+arr.piso.intersection()  [(3, 4]] Length: 1, closed: right, dtype: interval
+[int64] >>> arr.piso.contains([2, 3, 5]) 2 3 5 (1, 5] True True True (3, 6]
+False False True (2, 4] False True False >>> df = pd.DataFrame( ... {"A":[4,3],
+"B":["x","y"]}, ... index=pd.IntervalIndex.from_tuples([(1,3), (5,7)]), ... )
+>>> s = pd.Series( ... [True, False], ... index=pd.IntervalIndex.from_tuples([
+(2,4), (5,6)]), ... name="C", ... ) >>> piso.join(df, s) A B C (1, 2] 4 x NaN
+(2, 3] 4 x True (5, 6] 3 y False (6, 7] 3 y NaN >>> piso.join(df, s,
+how="inner") A B C (2, 3] 4 x True (5, 6] 3 y False ``` The domain of the
+intervals can be either numerical, `pandas.Timestamp` or `pandas.Timedelta`.
+Several [case studies](https://piso.readthedocs.io/en/latest/user_guide/
+case_studies/index.html) using piso can be found in the [user guide](https://
+piso.readthedocs.io/en/latest/user_guide/index.html). Further examples, and a
+detailed explanation of functionality, are provided in the [API reference]
+(https://piso.readthedocs.io/en/latest/reference/index.html). Visit [https://
+piso.readthedocs.io](https://piso.readthedocs.io/) for the documentation. ##
+Installation `piso` can be installed from PyPI or Anaconda. To install the
+latest version from PyPI:: ```sh python -m pip install piso ``` To install the
+latest version through conda-forge:: ```sh conda install -c conda-forge piso
+``` ## Versioning [SemVer](http://semver.org/) is used by piso for versioning
+releases. For versions available, see the [tags on this repository](https://
+github.com/staircase-dev/piso/tags). ## License This project is licensed under
+the [MIT License](https://github.com/staircase-dev/piso/blob/master/LICENSE) ##
+Acknowledgments Currently, piso is a pure-python implentation which relies
+heavily on [staircase](https://www.staircase.dev) and [pandas](https://
+pandas.pydata.org/). It is designed to operate as part of the *pandas
+ecosystem*. The colours for the piso logo have been assimilated from pandas as
+a homage, and is not to intended to imply and affiliation with, or endorsement
+by, pandas. Additionally, two classes have been borrowed, almost verbatim, from
+the pandas source code: - `pandas.util._decorators.Appender` -
+`pandas.core.accessor.CachedAccessor`
```

