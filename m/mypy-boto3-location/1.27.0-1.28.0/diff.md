# Comparing `tmp/mypy-boto3-location-1.27.0.tar.gz` & `tmp/mypy-boto3-location-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-location-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
+gzip compressed data, was "mypy-boto3-location-1.28.0.tar", last modified: Thu Jul  6 21:00:01 2023, max compression
```

## Comparing `mypy-boto3-location-1.27.0.tar` & `mypy-boto3-location-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/mypy_boto3_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45353 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45278 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64854 2023-07-03 19:41:16.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64743 2023-07-03 19:41:14.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/mypy_boto3_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45468 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-06 20:46:02.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65082 2023-07-06 20:46:04.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64971 2023-07-06 20:46:03.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/mypy_boto3_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:00.000000 mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:01.026357 mypy-boto3-location-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:46:01.000000 mypy-boto3-location-1.28.0/setup.py
```

### Comparing `mypy-boto3-location-1.27.0/LICENSE` & `mypy-boto3-location-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/PKG-INFO` & `mypy-boto3-location-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.27.0
-Summary: Type annotations for boto3.LocationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.LocationService 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-location-1.27.0/README.md` & `mypy-boto3-location-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.py` & `mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.pyi` & `mypy-boto3-location-1.28.0/mypy_boto3_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/__main__.py` & `mypy-boto3-location-1.28.0/mypy_boto3_location/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LocationService 1.27.0\nVersion:         1.27.0\nBuilder"
+        "Type annotations for boto3.LocationService 1.28.0\nVersion:         1.28.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/client.py` & `mypy-boto3-location-1.28.0/mypy_boto3_location/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,15 @@
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: Union[datetime, str] = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
         """
         [Calculates a
         route](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
@@ -241,14 +242,15 @@
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: Union[datetime, str] = ...,
         DistanceUnit: DistanceUnitType = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
         route-matrix.html)_ given the following required parameters:
@@ -299,16 +301,15 @@
         Description: str = ...,
         ExpireTime: Union[datetime, str] = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
-        grant `geo:GetMap*` actions for Amazon Location Map resources to the API key
-        bearer.
+        grant actions for Amazon Location resources to the API key bearer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#create_key)
         """
 
     def create_map(
         self,
@@ -361,14 +362,15 @@
         """
 
     def create_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         KmsKeyId: str = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateTrackerResponseTypeDef:
         """
@@ -576,15 +578,15 @@
         Retrieves a vector data tile from the map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_tile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#get_map_tile)
         """
 
     def get_place(
-        self, *, IndexName: str, PlaceId: str, Language: str = ...
+        self, *, IndexName: str, PlaceId: str, Key: str = ..., Language: str = ...
     ) -> GetPlaceResponseTypeDef:
         """
         Finds a place by its unique ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_place)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#get_place)
         """
@@ -703,14 +705,15 @@
         """
 
     def search_place_index_for_position(
         self,
         *,
         IndexName: str,
         Position: Sequence[float],
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForPositionResponseTypeDef:
         """
         Reverse geocodes a given coordinate and returns a legible address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_position)
@@ -722,14 +725,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form text.
 
@@ -742,14 +746,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of interest.
 
@@ -847,14 +852,15 @@
         """
 
     def update_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...
     ) -> UpdateTrackerResponseTypeDef:
         """
         Updates the specified properties of a given tracker resource.
```

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/client.pyi` & `mypy-boto3-location-1.28.0/mypy_boto3_location/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,15 @@
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: Union[datetime, str] = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
         """
         [Calculates a
         route](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
@@ -228,14 +229,15 @@
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: Union[datetime, str] = ...,
         DistanceUnit: DistanceUnitType = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
         route-matrix.html)_ given the following required parameters:
@@ -282,16 +284,15 @@
         Description: str = ...,
         ExpireTime: Union[datetime, str] = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
-        grant `geo:GetMap*` actions for Amazon Location Map resources to the API key
-        bearer.
+        grant actions for Amazon Location resources to the API key bearer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#create_key)
         """
     def create_map(
         self,
         *,
@@ -340,14 +341,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#create_route_calculator)
         """
     def create_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         KmsKeyId: str = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateTrackerResponseTypeDef:
         """
@@ -533,15 +535,15 @@
         """
         Retrieves a vector data tile from the map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_tile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#get_map_tile)
         """
     def get_place(
-        self, *, IndexName: str, PlaceId: str, Language: str = ...
+        self, *, IndexName: str, PlaceId: str, Key: str = ..., Language: str = ...
     ) -> GetPlaceResponseTypeDef:
         """
         Finds a place by its unique ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_place)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#get_place)
         """
@@ -648,14 +650,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#put_geofence)
         """
     def search_place_index_for_position(
         self,
         *,
         IndexName: str,
         Position: Sequence[float],
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForPositionResponseTypeDef:
         """
         Reverse geocodes a given coordinate and returns a legible address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_position)
@@ -666,14 +669,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form text.
 
@@ -685,14 +689,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of interest.
 
@@ -782,14 +787,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_route_calculator)
         """
     def update_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...
     ) -> UpdateTrackerResponseTypeDef:
         """
         Updates the specified properties of a given tracker resource.
```

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/literals.py` & `mypy-boto3-location-1.28.0/mypy_boto3_location/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/literals.pyi` & `mypy-boto3-location-1.28.0/mypy_boto3_location/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.py` & `mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.pyi` & `mypy-boto3-location-1.28.0/mypy_boto3_location/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.py` & `mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,14 +477,15 @@
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Mapping[str, str],
     },
     total=False,
@@ -623,14 +624,15 @@
 )
 
 DescribeTrackerResponseTypeDef = TypedDict(
     "DescribeTrackerResponseTypeDef",
     {
         "CreateTime": datetime,
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Dict[str, str],
         "TrackerArn": str,
         "TrackerName": str,
@@ -858,14 +860,15 @@
         "IndexName": str,
         "PlaceId": str,
     },
 )
 _OptionalGetPlaceRequestRequestTypeDef = TypedDict(
     "_OptionalGetPlaceRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
     },
     total=False,
 )
 
 
 class GetPlaceRequestRequestTypeDef(
@@ -1390,14 +1393,15 @@
         "IndexName": str,
         "Position": Sequence[float],
     },
 )
 _OptionalSearchPlaceIndexForPositionRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForPositionRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 
@@ -1442,14 +1446,15 @@
 _OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 
@@ -1498,14 +1503,15 @@
 _OptionalSearchPlaceIndexForTextRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 
@@ -1663,14 +1669,15 @@
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
     },
     total=False,
 )
 
@@ -2264,14 +2271,15 @@
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": Union[datetime, str],
         "DistanceUnit": DistanceUnitType,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
 
 
@@ -2294,14 +2302,15 @@
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": Union[datetime, str],
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.pyi` & `mypy-boto3-location-1.28.0/mypy_boto3_location/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -468,14 +468,15 @@
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Mapping[str, str],
     },
     total=False,
@@ -612,14 +613,15 @@
 )
 
 DescribeTrackerResponseTypeDef = TypedDict(
     "DescribeTrackerResponseTypeDef",
     {
         "CreateTime": datetime,
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Dict[str, str],
         "TrackerArn": str,
         "TrackerName": str,
@@ -835,14 +837,15 @@
         "IndexName": str,
         "PlaceId": str,
     },
 )
 _OptionalGetPlaceRequestRequestTypeDef = TypedDict(
     "_OptionalGetPlaceRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
     },
     total=False,
 )
 
 class GetPlaceRequestRequestTypeDef(
     _RequiredGetPlaceRequestRequestTypeDef, _OptionalGetPlaceRequestRequestTypeDef
@@ -1335,14 +1338,15 @@
         "IndexName": str,
         "Position": Sequence[float],
     },
 )
 _OptionalSearchPlaceIndexForPositionRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForPositionRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class SearchPlaceIndexForPositionRequestRequestTypeDef(
@@ -1383,14 +1387,15 @@
 _OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class SearchPlaceIndexForSuggestionsRequestRequestTypeDef(
@@ -1435,14 +1440,15 @@
 _OptionalSearchPlaceIndexForTextRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class SearchPlaceIndexForTextRequestRequestTypeDef(
@@ -1592,14 +1598,15 @@
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
     },
     total=False,
 )
 
@@ -2167,14 +2174,15 @@
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": Union[datetime, str],
         "DistanceUnit": DistanceUnitType,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
 
 class CalculateRouteMatrixRequestRequestTypeDef(
@@ -2195,14 +2203,15 @@
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": Union[datetime, str],
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/PKG-INFO` & `mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.27.0
-Summary: Type annotations for boto3.LocationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.LocationService 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/SOURCES.txt` & `mypy-boto3-location-1.28.0/mypy_boto3_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.27.0/setup.py` & `mypy-boto3-location-1.28.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-location",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LocationService 1.27.0 service generated with"
+        "Type annotations for boto3.LocationService 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

