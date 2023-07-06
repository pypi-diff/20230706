# Comparing `tmp/mypy-boto3-quicksight-1.27.0.tar.gz` & `tmp/mypy-boto3-quicksight-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-quicksight-1.27.0.tar", last modified: Mon Jul  3 19:51:17 2023, max compression
+gzip compressed data, was "mypy-boto3-quicksight-1.28.0.tar", last modified: Thu Jul  6 21:00:22 2023, max compression
```

## Comparing `mypy-boto3-quicksight-1.27.0.tar` & `mypy-boto3-quicksight-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.687844 mypy-boto3-quicksight-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    60442 2023-07-03 19:51:17.683843 mypy-boto3-quicksight-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    58945 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.679844 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   118036 2023-07-03 19:45:30.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   117853 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34638 2023-07-03 19:45:31.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    34636 2023-07-03 19:45:30.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21024 2023-07-03 19:45:30.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21004 2023-07-03 19:45:30.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   400038 2023-07-03 19:45:41.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   399520 2023-07-03 19:45:35.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:45:26.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:17.683843 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    60442 2023-07-03 19:51:17.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:51:17.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:17.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:17.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:17.000000 mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:17.687844 mypy-boto3-quicksight-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:45:25.000000 mypy-boto3-quicksight-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.750401 mypy-boto3-quicksight-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    60631 2023-07-06 21:00:22.750401 mypy-boto3-quicksight-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    59134 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.750401 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118036 2023-07-06 20:52:00.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117853 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-07-06 20:52:01.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34913 2023-07-06 20:52:01.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21024 2023-07-06 20:52:00.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21004 2023-07-06 20:52:00.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   401486 2023-07-06 20:52:21.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400964 2023-07-06 20:52:12.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.750401 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    60631 2023-07-06 21:00:22.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 21:00:22.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:22.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:22.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:22.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:22.000000 mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:22.750401 mypy-boto3-quicksight-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:51:59.000000 mypy-boto3-quicksight-1.28.0/setup.py
```

### Comparing `mypy-boto3-quicksight-1.27.0/LICENSE` & `mypy-boto3-quicksight-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/PKG-INFO` & `mypy-boto3-quicksight-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.27.0
-Summary: Type annotations for boto3.QuickSight 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.QuickSight 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-quicksight?color=blue)](https://pypistats.org/packages/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -510,15 +510,18 @@
     SelectedFieldOptionsType,
     SelectedTooltipTypeType,
     SheetContentTypeType,
     SheetControlDateTimePickerTypeType,
     SheetControlListTypeType,
     SheetControlSliderTypeType,
     SimpleNumericalAggregationFunctionType,
+    SmallMultiplesAxisPlacementType,
+    SmallMultiplesAxisScaleType,
     SortDirectionType,
+    SpecialValueType,
     StatusType,
     TableBorderStyleType,
     TableCellImageScalingConfigurationType,
     TableFieldIconSetTypeType,
     TableOrientationType,
     TableTotalsPlacementType,
     TableTotalsScrollStatusType,
@@ -642,14 +645,15 @@
     CustomFilterConfigurationTypeDef,
     CustomFilterListConfigurationTypeDef,
     FilterListConfigurationTypeDef,
     CellValueSynonymTypeDef,
     SimpleClusterMarkerTypeDef,
     CollectiveConstantTypeDef,
     DataColorTypeDef,
+    CustomColorTypeDef,
     ColumnDescriptionTypeDef,
     ColumnGroupColumnSchemaTypeDef,
     GeoSpatialColumnGroupTypeDef,
     ColumnLevelPermissionRuleTypeDef,
     ColumnSchemaTypeDef,
     ComparativeOrderTypeDef,
     ConditionalFormattingSolidColorTypeDef,
@@ -980,14 +984,15 @@
     SpacingTypeDef,
     SheetVisualScopingConfigurationTypeDef,
     SemanticEntityTypeTypeDef,
     SemanticTypeTypeDef,
     SheetTextBoxTypeDef,
     SheetElementConfigurationOverridesTypeDef,
     ShortFormatTextTypeDef,
+    SmallMultiplesAxisPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StringDatasetParameterDefaultValuesTypeDef,
     StringValueWhenUnsetConfigurationTypeDef,
     TableCellImageSizingConfigurationTypeDef,
     TablePaginatedReportOptionsTypeDef,
     TableFieldCustomIconContentTypeDef,
@@ -1071,14 +1076,15 @@
     TileStyleTypeDef,
     BoxPlotOptionsTypeDef,
     CreateColumnsOperationTypeDef,
     CategoryFilterConfigurationTypeDef,
     ClusterMarkerTypeDef,
     TopicCategoryFilterConstantTypeDef,
     ColorScaleTypeDef,
+    ColorsConfigurationTypeDef,
     ColumnTagTypeDef,
     ColumnGroupSchemaTypeDef,
     ColumnGroupTypeDef,
     DataSetSchemaTypeDef,
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.27.0/README.md` & `mypy-boto3-quicksight-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-quicksight?color=blue)](https://pypistats.org/packages/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -478,15 +478,18 @@
     SelectedFieldOptionsType,
     SelectedTooltipTypeType,
     SheetContentTypeType,
     SheetControlDateTimePickerTypeType,
     SheetControlListTypeType,
     SheetControlSliderTypeType,
     SimpleNumericalAggregationFunctionType,
+    SmallMultiplesAxisPlacementType,
+    SmallMultiplesAxisScaleType,
     SortDirectionType,
+    SpecialValueType,
     StatusType,
     TableBorderStyleType,
     TableCellImageScalingConfigurationType,
     TableFieldIconSetTypeType,
     TableOrientationType,
     TableTotalsPlacementType,
     TableTotalsScrollStatusType,
@@ -610,14 +613,15 @@
     CustomFilterConfigurationTypeDef,
     CustomFilterListConfigurationTypeDef,
     FilterListConfigurationTypeDef,
     CellValueSynonymTypeDef,
     SimpleClusterMarkerTypeDef,
     CollectiveConstantTypeDef,
     DataColorTypeDef,
+    CustomColorTypeDef,
     ColumnDescriptionTypeDef,
     ColumnGroupColumnSchemaTypeDef,
     GeoSpatialColumnGroupTypeDef,
     ColumnLevelPermissionRuleTypeDef,
     ColumnSchemaTypeDef,
     ComparativeOrderTypeDef,
     ConditionalFormattingSolidColorTypeDef,
@@ -948,14 +952,15 @@
     SpacingTypeDef,
     SheetVisualScopingConfigurationTypeDef,
     SemanticEntityTypeTypeDef,
     SemanticTypeTypeDef,
     SheetTextBoxTypeDef,
     SheetElementConfigurationOverridesTypeDef,
     ShortFormatTextTypeDef,
+    SmallMultiplesAxisPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StringDatasetParameterDefaultValuesTypeDef,
     StringValueWhenUnsetConfigurationTypeDef,
     TableCellImageSizingConfigurationTypeDef,
     TablePaginatedReportOptionsTypeDef,
     TableFieldCustomIconContentTypeDef,
@@ -1039,14 +1044,15 @@
     TileStyleTypeDef,
     BoxPlotOptionsTypeDef,
     CreateColumnsOperationTypeDef,
     CategoryFilterConfigurationTypeDef,
     ClusterMarkerTypeDef,
     TopicCategoryFilterConstantTypeDef,
     ColorScaleTypeDef,
+    ColorsConfigurationTypeDef,
     ColumnTagTypeDef,
     ColumnGroupSchemaTypeDef,
     ColumnGroupTypeDef,
     DataSetSchemaTypeDef,
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/__init__.py` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/__init__.pyi` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/__main__.py` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QuickSight 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.QuickSight 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.27.0")
+    print("1.28.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/client.py` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/client.pyi` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/literals.py` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnalysisErrorTypeType",
     "AnalysisFilterAttributeType",
     "AnchorOptionType",
     "ArcThicknessOptionsType",
     "ArcThicknessType",
     "AssetBundleExportFormatType",
@@ -180,15 +179,18 @@
     "SelectedFieldOptionsType",
     "SelectedTooltipTypeType",
     "SheetContentTypeType",
     "SheetControlDateTimePickerTypeType",
     "SheetControlListTypeType",
     "SheetControlSliderTypeType",
     "SimpleNumericalAggregationFunctionType",
+    "SmallMultiplesAxisPlacementType",
+    "SmallMultiplesAxisScaleType",
     "SortDirectionType",
+    "SpecialValueType",
     "StatusType",
     "TableBorderStyleType",
     "TableCellImageScalingConfigurationType",
     "TableFieldIconSetTypeType",
     "TableOrientationType",
     "TableTotalsPlacementType",
     "TableTotalsScrollStatusType",
@@ -225,15 +227,14 @@
     "QuickSightServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnalysisErrorTypeType = Literal[
     "ACCESS_DENIED",
     "COLUMN_GEOGRAPHIC_ROLE_MISMATCH",
     "COLUMN_REPLACEMENT_MISSING",
     "COLUMN_TYPE_MISMATCH",
     "DATA_SET_NOT_FOUND",
     "INTERNAL_FAILURE",
@@ -708,15 +709,18 @@
     "MIN",
     "STDEV",
     "STDEVP",
     "SUM",
     "VAR",
     "VARP",
 ]
+SmallMultiplesAxisPlacementType = Literal["INSIDE", "OUTSIDE"]
+SmallMultiplesAxisScaleType = Literal["INDEPENDENT", "SHARED"]
 SortDirectionType = Literal["ASC", "DESC"]
+SpecialValueType = Literal["EMPTY", "NULL", "OTHER"]
 StatusType = Literal["DISABLED", "ENABLED"]
 TableBorderStyleType = Literal["NONE", "SOLID"]
 TableCellImageScalingConfigurationType = Literal[
     "DO_NOT_SCALE", "FIT_TO_CELL_HEIGHT", "FIT_TO_CELL_WIDTH"
 ]
 TableFieldIconSetTypeType = Literal["LINK"]
 TableOrientationType = Literal["HORIZONTAL", "VERTICAL"]
```

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/literals.pyi` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AnalysisErrorTypeType",
     "AnalysisFilterAttributeType",
     "AnchorOptionType",
     "ArcThicknessOptionsType",
     "ArcThicknessType",
     "AssetBundleExportFormatType",
@@ -179,15 +180,18 @@
     "SelectedFieldOptionsType",
     "SelectedTooltipTypeType",
     "SheetContentTypeType",
     "SheetControlDateTimePickerTypeType",
     "SheetControlListTypeType",
     "SheetControlSliderTypeType",
     "SimpleNumericalAggregationFunctionType",
+    "SmallMultiplesAxisPlacementType",
+    "SmallMultiplesAxisScaleType",
     "SortDirectionType",
+    "SpecialValueType",
     "StatusType",
     "TableBorderStyleType",
     "TableCellImageScalingConfigurationType",
     "TableFieldIconSetTypeType",
     "TableOrientationType",
     "TableTotalsPlacementType",
     "TableTotalsScrollStatusType",
@@ -224,14 +228,15 @@
     "QuickSightServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AnalysisErrorTypeType = Literal[
     "ACCESS_DENIED",
     "COLUMN_GEOGRAPHIC_ROLE_MISMATCH",
     "COLUMN_REPLACEMENT_MISSING",
     "COLUMN_TYPE_MISMATCH",
     "DATA_SET_NOT_FOUND",
     "INTERNAL_FAILURE",
@@ -706,15 +711,18 @@
     "MIN",
     "STDEV",
     "STDEVP",
     "SUM",
     "VAR",
     "VARP",
 ]
+SmallMultiplesAxisPlacementType = Literal["INSIDE", "OUTSIDE"]
+SmallMultiplesAxisScaleType = Literal["INDEPENDENT", "SHARED"]
 SortDirectionType = Literal["ASC", "DESC"]
+SpecialValueType = Literal["EMPTY", "NULL", "OTHER"]
 StatusType = Literal["DISABLED", "ENABLED"]
 TableBorderStyleType = Literal["NONE", "SOLID"]
 TableCellImageScalingConfigurationType = Literal[
     "DO_NOT_SCALE", "FIT_TO_CELL_HEIGHT", "FIT_TO_CELL_WIDTH"
 ]
 TableFieldIconSetTypeType = Literal["LINK"]
 TableOrientationType = Literal["HORIZONTAL", "VERTICAL"]
```

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/paginator.py` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/paginator.pyi` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/type_defs.py` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,18 @@
     SectionPageBreakStatusType,
     SelectedTooltipTypeType,
     SheetContentTypeType,
     SheetControlDateTimePickerTypeType,
     SheetControlListTypeType,
     SheetControlSliderTypeType,
     SimpleNumericalAggregationFunctionType,
+    SmallMultiplesAxisPlacementType,
+    SmallMultiplesAxisScaleType,
     SortDirectionType,
+    SpecialValueType,
     StatusType,
     TableBorderStyleType,
     TableCellImageScalingConfigurationType,
     TableOrientationType,
     TableTotalsPlacementType,
     TableTotalsScrollStatusType,
     TemplateErrorTypeType,
@@ -265,14 +268,15 @@
     "CustomFilterConfigurationTypeDef",
     "CustomFilterListConfigurationTypeDef",
     "FilterListConfigurationTypeDef",
     "CellValueSynonymTypeDef",
     "SimpleClusterMarkerTypeDef",
     "CollectiveConstantTypeDef",
     "DataColorTypeDef",
+    "CustomColorTypeDef",
     "ColumnDescriptionTypeDef",
     "ColumnGroupColumnSchemaTypeDef",
     "GeoSpatialColumnGroupTypeDef",
     "ColumnLevelPermissionRuleTypeDef",
     "ColumnSchemaTypeDef",
     "ComparativeOrderTypeDef",
     "ConditionalFormattingSolidColorTypeDef",
@@ -603,14 +607,15 @@
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
     "SemanticEntityTypeTypeDef",
     "SemanticTypeTypeDef",
     "SheetTextBoxTypeDef",
     "SheetElementConfigurationOverridesTypeDef",
     "ShortFormatTextTypeDef",
+    "SmallMultiplesAxisPropertiesTypeDef",
     "StartAssetBundleExportJobResponseTypeDef",
     "StartAssetBundleImportJobResponseTypeDef",
     "StringDatasetParameterDefaultValuesTypeDef",
     "StringValueWhenUnsetConfigurationTypeDef",
     "TableCellImageSizingConfigurationTypeDef",
     "TablePaginatedReportOptionsTypeDef",
     "TableFieldCustomIconContentTypeDef",
@@ -694,14 +699,15 @@
     "TileStyleTypeDef",
     "BoxPlotOptionsTypeDef",
     "CreateColumnsOperationTypeDef",
     "CategoryFilterConfigurationTypeDef",
     "ClusterMarkerTypeDef",
     "TopicCategoryFilterConstantTypeDef",
     "ColorScaleTypeDef",
+    "ColorsConfigurationTypeDef",
     "ColumnTagTypeDef",
     "ColumnGroupSchemaTypeDef",
     "ColumnGroupTypeDef",
     "DataSetSchemaTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
@@ -2098,14 +2104,34 @@
     {
         "Color": str,
         "DataValue": float,
     },
     total=False,
 )
 
+_RequiredCustomColorTypeDef = TypedDict(
+    "_RequiredCustomColorTypeDef",
+    {
+        "Color": str,
+    },
+)
+_OptionalCustomColorTypeDef = TypedDict(
+    "_OptionalCustomColorTypeDef",
+    {
+        "FieldValue": str,
+        "SpecialValue": SpecialValueType,
+    },
+    total=False,
+)
+
+
+class CustomColorTypeDef(_RequiredCustomColorTypeDef, _OptionalCustomColorTypeDef):
+    pass
+
+
 ColumnDescriptionTypeDef = TypedDict(
     "ColumnDescriptionTypeDef",
     {
         "Text": str,
     },
     total=False,
 )
@@ -6258,14 +6284,23 @@
     {
         "PlainText": str,
         "RichText": str,
     },
     total=False,
 )
 
+SmallMultiplesAxisPropertiesTypeDef = TypedDict(
+    "SmallMultiplesAxisPropertiesTypeDef",
+    {
+        "Scale": SmallMultiplesAxisScaleType,
+        "Placement": SmallMultiplesAxisPlacementType,
+    },
+    total=False,
+)
+
 StartAssetBundleExportJobResponseTypeDef = TypedDict(
     "StartAssetBundleExportJobResponseTypeDef",
     {
         "Arn": str,
         "AssetBundleExportJobId": str,
         "RequestId": str,
         "Status": int,
@@ -7359,14 +7394,22 @@
 )
 
 
 class ColorScaleTypeDef(_RequiredColorScaleTypeDef, _OptionalColorScaleTypeDef):
     pass
 
 
+ColorsConfigurationTypeDef = TypedDict(
+    "ColorsConfigurationTypeDef",
+    {
+        "CustomColors": Sequence[CustomColorTypeDef],
+    },
+    total=False,
+)
+
 ColumnTagTypeDef = TypedDict(
     "ColumnTagTypeDef",
     {
         "ColumnGeographicRole": GeoSpatialDataRoleType,
         "ColumnDescription": ColumnDescriptionTypeDef,
     },
     total=False,
@@ -10946,23 +10989,36 @@
         "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationTypeDef,
         "CurrencyDisplayFormatConfiguration": CurrencyDisplayFormatConfigurationTypeDef,
         "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-AggregationSortConfigurationTypeDef = TypedDict(
-    "AggregationSortConfigurationTypeDef",
+_RequiredAggregationSortConfigurationTypeDef = TypedDict(
+    "_RequiredAggregationSortConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "SortDirection": SortDirectionType,
+    },
+)
+_OptionalAggregationSortConfigurationTypeDef = TypedDict(
+    "_OptionalAggregationSortConfigurationTypeDef",
+    {
         "AggregationFunction": AggregationFunctionTypeDef,
     },
+    total=False,
 )
 
+
+class AggregationSortConfigurationTypeDef(
+    _RequiredAggregationSortConfigurationTypeDef, _OptionalAggregationSortConfigurationTypeDef
+):
+    pass
+
+
 _RequiredColumnSortTypeDef = TypedDict(
     "_RequiredColumnSortTypeDef",
     {
         "SortBy": ColumnIdentifierTypeDef,
         "Direction": SortDirectionType,
     },
 )
@@ -11600,14 +11656,16 @@
 
 SmallMultiplesOptionsTypeDef = TypedDict(
     "SmallMultiplesOptionsTypeDef",
     {
         "MaxVisibleRows": int,
         "MaxVisibleColumns": int,
         "PanelConfiguration": PanelConfigurationTypeDef,
+        "XAxis": SmallMultiplesAxisPropertiesTypeDef,
+        "YAxis": SmallMultiplesAxisPropertiesTypeDef,
     },
     total=False,
 )
 
 TableFieldLinkConfigurationTypeDef = TypedDict(
     "TableFieldLinkConfigurationTypeDef",
     {
@@ -12994,14 +13052,15 @@
     },
 )
 _OptionalColumnConfigurationTypeDef = TypedDict(
     "_OptionalColumnConfigurationTypeDef",
     {
         "FormatConfiguration": FormatConfigurationTypeDef,
         "Role": ColumnRoleType,
+        "ColorsConfiguration": ColorsConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class ColumnConfigurationTypeDef(
     _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
```

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight/type_defs.pyi` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,18 @@
     SectionPageBreakStatusType,
     SelectedTooltipTypeType,
     SheetContentTypeType,
     SheetControlDateTimePickerTypeType,
     SheetControlListTypeType,
     SheetControlSliderTypeType,
     SimpleNumericalAggregationFunctionType,
+    SmallMultiplesAxisPlacementType,
+    SmallMultiplesAxisScaleType,
     SortDirectionType,
+    SpecialValueType,
     StatusType,
     TableBorderStyleType,
     TableCellImageScalingConfigurationType,
     TableOrientationType,
     TableTotalsPlacementType,
     TableTotalsScrollStatusType,
     TemplateErrorTypeType,
@@ -264,14 +267,15 @@
     "CustomFilterConfigurationTypeDef",
     "CustomFilterListConfigurationTypeDef",
     "FilterListConfigurationTypeDef",
     "CellValueSynonymTypeDef",
     "SimpleClusterMarkerTypeDef",
     "CollectiveConstantTypeDef",
     "DataColorTypeDef",
+    "CustomColorTypeDef",
     "ColumnDescriptionTypeDef",
     "ColumnGroupColumnSchemaTypeDef",
     "GeoSpatialColumnGroupTypeDef",
     "ColumnLevelPermissionRuleTypeDef",
     "ColumnSchemaTypeDef",
     "ComparativeOrderTypeDef",
     "ConditionalFormattingSolidColorTypeDef",
@@ -602,14 +606,15 @@
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
     "SemanticEntityTypeTypeDef",
     "SemanticTypeTypeDef",
     "SheetTextBoxTypeDef",
     "SheetElementConfigurationOverridesTypeDef",
     "ShortFormatTextTypeDef",
+    "SmallMultiplesAxisPropertiesTypeDef",
     "StartAssetBundleExportJobResponseTypeDef",
     "StartAssetBundleImportJobResponseTypeDef",
     "StringDatasetParameterDefaultValuesTypeDef",
     "StringValueWhenUnsetConfigurationTypeDef",
     "TableCellImageSizingConfigurationTypeDef",
     "TablePaginatedReportOptionsTypeDef",
     "TableFieldCustomIconContentTypeDef",
@@ -693,14 +698,15 @@
     "TileStyleTypeDef",
     "BoxPlotOptionsTypeDef",
     "CreateColumnsOperationTypeDef",
     "CategoryFilterConfigurationTypeDef",
     "ClusterMarkerTypeDef",
     "TopicCategoryFilterConstantTypeDef",
     "ColorScaleTypeDef",
+    "ColorsConfigurationTypeDef",
     "ColumnTagTypeDef",
     "ColumnGroupSchemaTypeDef",
     "ColumnGroupTypeDef",
     "DataSetSchemaTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
@@ -2063,14 +2069,32 @@
     {
         "Color": str,
         "DataValue": float,
     },
     total=False,
 )
 
+_RequiredCustomColorTypeDef = TypedDict(
+    "_RequiredCustomColorTypeDef",
+    {
+        "Color": str,
+    },
+)
+_OptionalCustomColorTypeDef = TypedDict(
+    "_OptionalCustomColorTypeDef",
+    {
+        "FieldValue": str,
+        "SpecialValue": SpecialValueType,
+    },
+    total=False,
+)
+
+class CustomColorTypeDef(_RequiredCustomColorTypeDef, _OptionalCustomColorTypeDef):
+    pass
+
 ColumnDescriptionTypeDef = TypedDict(
     "ColumnDescriptionTypeDef",
     {
         "Text": str,
     },
     total=False,
 )
@@ -6073,14 +6097,23 @@
     {
         "PlainText": str,
         "RichText": str,
     },
     total=False,
 )
 
+SmallMultiplesAxisPropertiesTypeDef = TypedDict(
+    "SmallMultiplesAxisPropertiesTypeDef",
+    {
+        "Scale": SmallMultiplesAxisScaleType,
+        "Placement": SmallMultiplesAxisPlacementType,
+    },
+    total=False,
+)
+
 StartAssetBundleExportJobResponseTypeDef = TypedDict(
     "StartAssetBundleExportJobResponseTypeDef",
     {
         "Arn": str,
         "AssetBundleExportJobId": str,
         "RequestId": str,
         "Status": int,
@@ -7148,14 +7181,22 @@
     },
     total=False,
 )
 
 class ColorScaleTypeDef(_RequiredColorScaleTypeDef, _OptionalColorScaleTypeDef):
     pass
 
+ColorsConfigurationTypeDef = TypedDict(
+    "ColorsConfigurationTypeDef",
+    {
+        "CustomColors": Sequence[CustomColorTypeDef],
+    },
+    total=False,
+)
+
 ColumnTagTypeDef = TypedDict(
     "ColumnTagTypeDef",
     {
         "ColumnGeographicRole": GeoSpatialDataRoleType,
         "ColumnDescription": ColumnDescriptionTypeDef,
     },
     total=False,
@@ -10611,23 +10652,34 @@
         "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationTypeDef,
         "CurrencyDisplayFormatConfiguration": CurrencyDisplayFormatConfigurationTypeDef,
         "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-AggregationSortConfigurationTypeDef = TypedDict(
-    "AggregationSortConfigurationTypeDef",
+_RequiredAggregationSortConfigurationTypeDef = TypedDict(
+    "_RequiredAggregationSortConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "SortDirection": SortDirectionType,
+    },
+)
+_OptionalAggregationSortConfigurationTypeDef = TypedDict(
+    "_OptionalAggregationSortConfigurationTypeDef",
+    {
         "AggregationFunction": AggregationFunctionTypeDef,
     },
+    total=False,
 )
 
+class AggregationSortConfigurationTypeDef(
+    _RequiredAggregationSortConfigurationTypeDef, _OptionalAggregationSortConfigurationTypeDef
+):
+    pass
+
 _RequiredColumnSortTypeDef = TypedDict(
     "_RequiredColumnSortTypeDef",
     {
         "SortBy": ColumnIdentifierTypeDef,
         "Direction": SortDirectionType,
     },
 )
@@ -11223,14 +11275,16 @@
 
 SmallMultiplesOptionsTypeDef = TypedDict(
     "SmallMultiplesOptionsTypeDef",
     {
         "MaxVisibleRows": int,
         "MaxVisibleColumns": int,
         "PanelConfiguration": PanelConfigurationTypeDef,
+        "XAxis": SmallMultiplesAxisPropertiesTypeDef,
+        "YAxis": SmallMultiplesAxisPropertiesTypeDef,
     },
     total=False,
 )
 
 TableFieldLinkConfigurationTypeDef = TypedDict(
     "TableFieldLinkConfigurationTypeDef",
     {
@@ -12571,14 +12625,15 @@
     },
 )
 _OptionalColumnConfigurationTypeDef = TypedDict(
     "_OptionalColumnConfigurationTypeDef",
     {
         "FormatConfiguration": FormatConfigurationTypeDef,
         "Role": ColumnRoleType,
+        "ColorsConfiguration": ColorsConfigurationTypeDef,
     },
     total=False,
 )
 
 class ColumnConfigurationTypeDef(
     _RequiredColumnConfigurationTypeDef, _OptionalColumnConfigurationTypeDef
 ):
```

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/PKG-INFO` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.27.0
-Summary: Type annotations for boto3.QuickSight 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.QuickSight 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-quicksight?color=blue)](https://pypistats.org/packages/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -510,15 +510,18 @@
     SelectedFieldOptionsType,
     SelectedTooltipTypeType,
     SheetContentTypeType,
     SheetControlDateTimePickerTypeType,
     SheetControlListTypeType,
     SheetControlSliderTypeType,
     SimpleNumericalAggregationFunctionType,
+    SmallMultiplesAxisPlacementType,
+    SmallMultiplesAxisScaleType,
     SortDirectionType,
+    SpecialValueType,
     StatusType,
     TableBorderStyleType,
     TableCellImageScalingConfigurationType,
     TableFieldIconSetTypeType,
     TableOrientationType,
     TableTotalsPlacementType,
     TableTotalsScrollStatusType,
@@ -642,14 +645,15 @@
     CustomFilterConfigurationTypeDef,
     CustomFilterListConfigurationTypeDef,
     FilterListConfigurationTypeDef,
     CellValueSynonymTypeDef,
     SimpleClusterMarkerTypeDef,
     CollectiveConstantTypeDef,
     DataColorTypeDef,
+    CustomColorTypeDef,
     ColumnDescriptionTypeDef,
     ColumnGroupColumnSchemaTypeDef,
     GeoSpatialColumnGroupTypeDef,
     ColumnLevelPermissionRuleTypeDef,
     ColumnSchemaTypeDef,
     ComparativeOrderTypeDef,
     ConditionalFormattingSolidColorTypeDef,
@@ -980,14 +984,15 @@
     SpacingTypeDef,
     SheetVisualScopingConfigurationTypeDef,
     SemanticEntityTypeTypeDef,
     SemanticTypeTypeDef,
     SheetTextBoxTypeDef,
     SheetElementConfigurationOverridesTypeDef,
     ShortFormatTextTypeDef,
+    SmallMultiplesAxisPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StringDatasetParameterDefaultValuesTypeDef,
     StringValueWhenUnsetConfigurationTypeDef,
     TableCellImageSizingConfigurationTypeDef,
     TablePaginatedReportOptionsTypeDef,
     TableFieldCustomIconContentTypeDef,
@@ -1071,14 +1076,15 @@
     TileStyleTypeDef,
     BoxPlotOptionsTypeDef,
     CreateColumnsOperationTypeDef,
     CategoryFilterConfigurationTypeDef,
     ClusterMarkerTypeDef,
     TopicCategoryFilterConstantTypeDef,
     ColorScaleTypeDef,
+    ColorsConfigurationTypeDef,
     ColumnTagTypeDef,
     ColumnGroupSchemaTypeDef,
     ColumnGroupTypeDef,
     DataSetSchemaTypeDef,
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-quicksight-1.27.0/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy-boto3-quicksight-1.28.0/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.27.0/setup.py` & `mypy-boto3-quicksight-1.28.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QuickSight 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.QuickSight 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

