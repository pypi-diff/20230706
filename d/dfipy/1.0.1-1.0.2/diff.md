# Comparing `tmp/dfipy-1.0.1.tar.gz` & `tmp/dfipy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-1.0.1.tar", max compression
+gzip compressed data, was "dfipy-1.0.2.tar", max compression
```

## Comparing `dfipy-1.0.1.tar` & `dfipy-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      568 2023-06-17 20:34:31.360243 dfipy-1.0.1/LICENCE
--rw-r--r--   0        0        0     1713 2023-06-17 20:34:31.360243 dfipy-1.0.1/README.md
--rw-r--r--   0        0        0       27 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/__init__.py
--rw-r--r--   0        0        0    11774 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/analyse.py
--rw-r--r--   0        0        0     1537 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/client.py
--rw-r--r--   0        0        0     3648 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/connect.py
--rw-r--r--   0        0        0    20533 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/get.py
--rw-r--r--   0        0        0      351 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/models.py
--rw-r--r--   0        0        0     3064 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/polygons.py
--rw-r--r--   0        0        0     5325 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/show.py
--rw-r--r--   0        0        0     8731 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/validate.py
--rw-r--r--   0        0        0     1985 2023-06-17 20:34:40.048340 dfipy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 dfipy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      568 2023-07-06 09:33:03.982869 dfipy-1.0.2/LICENCE
+-rw-r--r--   0        0        0     1808 2023-07-06 09:33:03.982869 dfipy-1.0.2/README.md
+-rw-r--r--   0        0        0       99 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/__init__.py
+-rw-r--r--   0        0        0    14187 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/analyse.py
+-rw-r--r--   0        0        0     1418 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/client.py
+-rw-r--r--   0        0        0     3662 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/connect.py
+-rw-r--r--   0        0        0    20008 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/get.py
+-rw-r--r--   0        0        0     1320 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/models.py
+-rw-r--r--   0        0        0     2803 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/polygons.py
+-rw-r--r--   0        0        0     5196 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/show.py
+-rw-r--r--   0        0        0    11102 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/validate.py
+-rw-r--r--   0        0        0     2371 2023-07-06 09:33:05.506949 dfipy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 dfipy-1.0.2/PKG-INFO
```

### Comparing `dfipy-1.0.1/LICENCE` & `dfipy-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.1/README.md` & `dfipy-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-<img src="docs/gs_logo.png" width="40%" align="right">
+<img src="docs/source/_static/gs_logo.png" align="right">
 
 [![Python versions](https://img.shields.io/pypi/pyversions/dfipy.svg)](https://pypi.python.org/pypi/dfipy/)
 [![PyPI version](https://badge.fury.io/py/dfipy.svg)](https://badge.fury.io/py/dfipy)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
 
 # DFI API wrapper
 
 ## About
 
 - Python library created by [General System](https://www.generalsystem.com/) and publicly available on [github](https://github.com/thegeneralsystem) to query and experiment with the Data Flow Index (DFI) platform.
 - DFI provides the user with an unparalled foundation and scalable solution for processing high velocity, high volume spatiotemporal workloads for any geospatial data science need.
+- [Read the code documentation](https://dfipy.docs.generalsystem.com/)
 - [Read the whitepaper](https://assets.website-files.com/636ce900cf2e67aab6340642/643807134214aebc2b29849c_General%20System_The%20Data%20Flow%20Index%20Whitepaper%20_%20Nov%2022.pdf)
 
 ## Quickstart
 
+- Enroll at <https://eap.generalsystem.com> if you have not done so already.
+
 - Get the **key token** to access the demo DFI at  [https://tokens.dataflowindex.io/](https://tokens.dataflowindex.io/).
 
 - **Install** with:
     ```bash
     pip install dfipy
     ```
 
-- [Quickstart guide](https://github.com/thegeneralsystem/quickstart-guide)
-  
-- [DfiPyExamples](https://github.com/thegeneralsystem/dfipy-examples)
+- Start querying with [DfiPy Examples](https://github.com/thegeneralsystem/dfipy-examples)
 
 ## Licence
 
 - Copyright (c) 2023, General System Group Limited.
 
 - DFIPy is provided as it is and copyrighted under [Apache2 License](LICENCE).
```

### Comparing `dfipy-1.0.1/dfi/client.py` & `dfipy-1.0.2/dfi/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 """
 Class composition of all the other classes, to access the
 wrappers with syntactic sugar.
 """
-
-import logging
-
 from dfi.analyse import Analyse
 from dfi.connect import Connect
 from dfi.get import Get
 from dfi.polygons import Polygons
 from dfi.show import Show
 
-logger = logging.getLogger(__name__)
-
 
 class Client:
     """
     Client class gathering all the classes and method in a single one. Facade of dfi.Connect.
 
     See documentation of dfi.Connect for its input values.
 
-    Example
-    -------
-    >>> from dfi import Client
-    >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-    >>> dfi. <autocomplete + ? to access methods and documentations>
+    :example:
+    ```python
+    from dfi import Client
+
+    dfi = Client(dfi_token, instance_name, namespace, base_url)
+    ```
     """
 
     def __init__(
         self,
         api_token: str,
         instance_name: str,
         namespace: str = None,
```

### Comparing `dfipy-1.0.1/dfi/connect.py` & `dfipy-1.0.2/dfi/connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,40 +4,34 @@
 import logging
 from typing import Optional
 
 import requests
 
 from dfi import validate
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class Connect:
     """
     Class instantiating the connectors to the DFI API.
 
-    Parameters
-    ----------
-    api_token: str
-        token provided by generalsystem.com to access the running DFI environments.
-    instance_name: str
-        Name of a DFI API engine instance, living in the specified namespace.
-    namespace: str
-        Name for the collection of instances of DFI engines where to find the specific instance to connect to.
-    base_url : str
-        Base url where the service is located
-    query_timeout: int = 60
-        Time after an unresponsive query will be dropped.
-    progress_bar: bool = False
-        Visualise a progress bar if True (slows down the execution, typically used for demos and tests).
-
-    Examples
-    --------
-    >>> dfi_conn = dfi.Connect(api_token, instance_name, namespace, base_url)
-    >>> dfi_conn.streaming_headers
+    :param api_token: token provided by generalsystem.com to access the running DFI environments.
+    :param instance_name: Name of a DFI API engine instance, living in the specified namespace.
+    :param namespace: Name for the collection of instances of DFI engines where to find the specific instance to connect to.
+    :param base_url: Base url where the service is located
+    :param query_timeout: Time after an unresponsive query will be dropped.
+    :param progress_bar: Visualise a progress bar if True (slows down the execution, typically used for demos and tests).
+
+    :example:
+    ````python
+    dfi_conn = dfi.Connect(api_token, instance_name, namespace, base_url)
+
+    dfi_conn.streaming_headers
+    ````
     """
 
     def __init__(
         self,
         api_token: str,
         instance_name: str,
         namespace: str = None,
@@ -66,30 +60,32 @@
             self.qualified_instance_name = f"{namespace}.{instance_name}"
 
     # The representation will expose the secret token
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} {self.base_url}"
 
     def __str__(self) -> str:
-        return f"""API connection instance
-base_url={self.base_url},
-namespace={self.namespace},
-instance_name={self.instance_name}"""
+        return f"""
+                API connection instance
+                base_url={self.base_url},
+                namespace={self.namespace},
+                instance_name={self.instance_name}
+                """
 
     # get and post API wrappers
     def api_get(
         self,
         endpoint: str,
         stream: bool = True,
         params: Optional[dict] = None,
     ) -> requests.models.Response:
         """Helper wrapping requests.get method"""
         headers = self.streaming_headers
         url = f"{self.base_url}/{endpoint}"
-        logger.debug(dict(url=url, headers=headers, stream=stream, params=params, timeout=self.query_timeout))
+        _logger.debug(dict(url=url, headers=headers, stream=stream, params=params, timeout=self.query_timeout))
         response = requests.get(
             url,
             headers=headers,
             stream=stream,
             params=params,
             timeout=self.query_timeout,
         )
```

### Comparing `dfipy-1.0.1/dfi/get.py` & `dfipy-1.0.2/dfi/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,47 +13,47 @@
 import requests
 import sseclient
 from tqdm import tqdm
 
 from dfi import models, validate
 from dfi.connect import Connect
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 NUM_ATTEMPTS = 3
 
 
 class Get:
     """
     Class responsible to call the HTTP API and submit queries.
 
     It can be accessed via the a dfi.Client class instance or it must be instantiated
     with a dfi.Connect instance as argument.
 
-    Parameters
-    ----------
-    conn : Connect
-        Instance of a Connect with the credentials and namespace of the DFI connection.
-
-    Examples
-    --------
+    :param conn: Instance of a Connect with the credentials and namespace of the DFI connection.
+    :example:
     Access via the Client class:
 
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> dfi.get.entities(time_interval=[start_time, end_time])
+    ```python
+    from dfi import Client
 
-    Or access only the Get class directly:
+    dfi = Client(dfi_token, instance_name, namespace, base_url)
+    dfi.get.entities(time_interval=[start_time, end_time])
+    ```
 
-        >>> from dfi.connect import Connect
-        >>> from dfi.get import Get
-        >>> conn = dfi.Connect(api_token, instance_name, namespace, base_url)
-        >>> dfi_get = dfi.Get(conn)
-        >>> dfi_get.entities(time_interval=[start_time, end_time])
+    Or access only the Get class directly:
 
+    ```python
+    from dfi.connect import Connect
+    from dfi.get import Get
+
+    conn = dfi.Connect(api_token, instance_name, namespace, base_url)
+    dfi_get = dfi.Get(conn)
+    dfi_get.entities(time_interval=[start_time, end_time])
+    ```
     """
 
     def __init__(self, conn: Connect) -> None:
         self.conn = conn
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.conn!r})"
@@ -66,54 +66,47 @@
         Returns the version of the Data Flow Index API.
         """
         with self.conn.api_get("version", stream=False, params=None) as response:
             return response.text
 
     def records_count(
         self,
-        time_interval: Optional[models.TimeInterval] = None,
-        polygon: Optional[models.Polygon] = None,
         entities: Optional[List[str]] = None,
+        polygon: Optional[models.Polygon] = None,
+        time_interval: Optional[models.TimeInterval] = None,
     ) -> int:
         """
-        Returns the number of records stored in the DFI engine after optional
-        time, space and entity ids constraints.
+        Queries for the number of records within the bounds.
 
         If all the variables are None it returns the total number of records in the
         database. Start_time and end_time must be both valid datetime, with
         start_time < end_time or both None.
 
-        Parameters
-        ----------
-        time_interval: Optional[models.TimeInterval] = None
-            Tuple with the Lower bound and the upper bound time constraints.
-        polygon: Optional[models.Polygon] = None
-            List of vertices [[lon1, lat1], [lon2, lat2], ...] or a list of four
-            floats representing the bounding box extremes as [lon_min, lat_min, lon_max, lat_max].
+        :param time_interval: Tuple with the lower bound and the upper bound time constraints.
+        :param polyogn: List of vertices `[[lon1, lat1], [lon2, lat2], [lon3, lat3], [lon1, lat1]]` or a list of four
+            floats representing the bounding box extremes as `[lon_min, lat_min, lon_max, lat_max]`.
             Non-valid input will raise an error.
-        entities: Optional[List[str]] = None
-            List of entity ids. It must be passed as list also for a single element.
-
-        Returns
-        -------
-        The number of records stored in the DFI engine.
-
-        Example
-        -------
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> start_time = datetime.strptime("2022-01-01T08:00:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
-        >>> end_time = datetime.strptime("2022-01-01T08:30:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
-        >>> entities = ["299eb59a-e47e-48c0-9ad5-89a9ce1303f4"]
-        >>> dfi.get.records_count(
-        ...     time_interval = (start_time, end_time),
-        ...     polygon = None,
-        ...     entities = entities,
-        ... )
-
+        :returns: The number of records stored in the DFI engine.
+        :raises `DFIInputValueError`: If `time_interval` or `polygon` are ill-formed.
+        :example:
+        ```python
+        from dfi import Client
+
+        dfi = Client(dfi_token, instance_name, namespace, base_url)
+
+        start_time = datetime.strptime("2022-01-01T08:00:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
+        end_time = datetime.strptime("2022-01-01T08:30:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
+        entities = ["299eb59a-e47e-48c0-9ad5-89a9ce1303f4"]
+
+        dfi.get.records_count(
+            time_interval = (start_time, end_time),
+            polygon = None,
+            entities = entities,
+        )
+        ```
         """
         validate.time_interval(time_interval)
         validate.polygon(polygon)
         validate.entities(entities)
 
         params = {"instance": self.conn.qualified_instance_name}
 
@@ -152,58 +145,56 @@
             with self.conn.api_get(
                 f"bounding-box/{min_lng}/{min_lat}/{max_lng}/{max_lat}/count", params=params
             ) as response:
                 return self._receive_count(response)
 
     def records(
         self,
-        time_interval: Optional[models.TimeInterval] = None,
-        polygon: Optional[models.Polygon] = None,
         entities: Optional[List[str]] = None,
+        polygon: Optional[models.Polygon] = None,
+        time_interval: Optional[models.TimeInterval] = None,
         add_payload_as_json: bool = False,
     ) -> pd.DataFrame:
         """
         Get the records of the entities appearing within the given time, space and entity ids constraints.
 
         List of entities and polygon can not be left both to None.
 
         Start time and end time passed in the time_interval must be both valid datetime,
         with start_time < end_time or both None.
 
-        Parameters
-        ----------
-        time_interval: Optional[models.TimeInterval] = None
-            Tuple with the Lower bound and the upper bound time constraints.
-        polygon: Optional[models.Polygon]
-            List of vertices [[lon1, lat1], [lon2, lat2], ...] or a list of four
+        :param time_interval: Tuple with the Lower bound and the upper bound time constraints.
+        :param polygon: List of vertices [[lon1, lat1], [lon2, lat2], ...] or a list of four
             floats representing the bounding box extremes as [lon_min, lat_min, lon_max, lat_max].
             Non-valid input will raise an error.
-        entities: Optional[List[str]] = None
-            List of entity ids. It must be passed as list also for a single element.
-        add_payload_as_json: bool = False
-            If True it parses the payload as a JSON string into the column payload.
-
-        Returns
-        -------
-        Dataframe with the records of the entities found in polygon, given the input constraints.
-
-        Example
-        -------
-            >>> from dfi import Client
-            >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-            >>> start_time = datetime.strptime("2022-01-01T08:00:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
-            >>> end_time = datetime.strptime("2022-01-01T08:30:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
-            >>> entities=["299eb59a-e47e-48c0-9ad5-89a9ce1303f4"]
-            >>> dfi.get.records(
-            ...     time_interval = (start_time, end_time),
-            ...     polygon = None,
-            ...     entities = entities,
-            ...     add_payload_as_json=True
-            ... )
+        :param entities: List of entity ids. It must be passed as list also for a single element.
+        :param add_payload_as_json: If True it parses the payload as a JSON string into the column payload.
+        :returns: Dataframe with the records of the entities found in polygon, given the input constraints.
+        :raises `DFIInputValueError`: If `time_interval` or `polygon` are ill-formed.
+        :raises `ValueError`: If no filter bound is specified.
+        :example:
+        ```python
+        from dfi import Client
+
+        dfi = Client(dfi_token, instance_name, namespace, base_url)
+
+        start_time = datetime.strptime("2022-01-01T08:00:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
+        end_time = datetime.strptime("2022-01-01T08:30:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
+        entities = ["299eb59a-e47e-48c0-9ad5-89a9ce1303f4"]
+
+        dfi.get.records(
+            time_interval = (start_time, end_time),
+            polygon = None,
+            entities = entities,
+            add_payload_as_json=True
+        )
+
+        ```
         """
+
         validate.time_interval(time_interval)
         validate.polygon(polygon)
         validate.entities(entities)
 
         params = {"instance": self.conn.qualified_instance_name}
 
         if polygon is None:
@@ -212,24 +203,24 @@
             if time_interval is not None:
                 params["startTime"], params["endTime"] = unpack_and_convert_time_interval(time_interval)
 
             df_entities = pd.DataFrame(columns=["entity_id", "timestamp", "longitude", "latitude", "payload"])
             for uid in entities:
                 with self.conn.api_get(f"entities/{uid}/history", params=params) as response:
                     data = self._receive_history(response)
-                    logger.debug("Uid: %s \nHistory length: %i", uid, len(data))
+                    _logger.debug("Uid: %s \nHistory length: %i", uid, len(data))
                     data_formatted = []
 
                     for item in data:
                         if add_payload_as_json:
                             try:
                                 payload = json.loads(item["payload"])
                             except Exception as err:
                                 payload = {}
-                                logger.debug("Failed to parse payload to JSON: %s for item %s", err, str(item))
+                                _logger.debug("Failed to parse payload to JSON: %s for item %s", err, str(item))
                         else:
                             payload = item["payload"]
                         data_formatted.append(
                             [
                                 item["id"],
                                 datetime.strptime(item["time"], "%Y-%m-%dT%H:%M:%S.%fZ"),
                                 item["coordinate"][0],
@@ -269,15 +260,15 @@
         data_formatted = []
         for item in streamed_data:
             if add_payload_as_json:
                 try:
                     payload = json.loads(item.get("payload"))
                 except Exception as err:
                     payload = {}
-                    logger.error("Failed to parse payload to JSON: %s", err)
+                    _logger.error("Failed to parse payload to JSON: %s", err)
             else:
                 payload = item.get("payload")
             data_formatted.append(
                 [
                     item["id"],
                     datetime.strptime(item["time"], "%Y-%m-%dT%H:%M:%S.%fZ"),
                     item["coordinate"][0],
@@ -285,59 +276,57 @@
                     payload,
                 ]
             )
         return pd.DataFrame(data_formatted, columns=["entity_id", "timestamp", "longitude", "latitude", "payload"])
 
     def entities(
         self,
-        time_interval: Optional[models.TimeInterval] = None,
         polygon: Optional[models.Polygon] = None,
+        time_interval: Optional[models.TimeInterval] = None,
     ) -> List[Union[str, int]]:
         """
         Get the list of entity ids within a space and optional time constraint.
 
         If time constraints are not passed, the whole dataset is returned.
         Start time and end time passed in the time_interval must be both valid datetime, with
         start_time < end_time or both None.
 
-        Parameters
-        ----------
-        time_interval: Optional[models.TimeInterval] = None
-            Tuple with the Lower bound and the upper bound time constraints.
-        polygon: Optional[models.Polygon] = None
-            List of vertices [[lon1, lat1], [lon2, lat2], ...] or a list of four
+        :param time_interval: Tuple with the Lower bound and the upper bound time constraints.
+        :param polygon: List of vertices [[lon1, lat1], [lon2, lat2], ...] or a list of four
             floats representing the bounding box extremes as [lon_min, lat_min, lon_max, lat_max].
             Non valid input will raise an error.
+        :returns: List of unique entities in time interval and polygon.
+        :raises `DFIInputValueError`: If `time_interval` or `polygon` are ill-formed.
+        :example:
+        ```python
+        from dfi import Client
+
+        dfi = Client(dfi_token, instance_name, namespace, base_url)
+
+        start_time = datetime.strptime("2022-01-01T08:00:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
+        end_time = datetime.strptime("2022-01-01T08:30:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
+        pimlico_tube_station =  [
+            [-0.13410870522207574, 51.48932327401289],
+            [-0.1355577905032419, 51.48887697878598],
+            [-0.1339996342869938, 51.487266398812636],
+            [-0.13279985400049554, 51.487508959676234],
+            [-0.13230124401115972, 51.4875768764868],
+            [-0.1319428680814667, 51.487955268294115],
+            [-0.1322389177630896, 51.4883918703234],
+            [-0.1322389177630896, 51.48887697878598],
+            [-0.13301799587057417, 51.48930386996324],
+            [-0.13410870522207574, 51.48932327401289],
+        ]
+
+        dfi.get.entities(
+            time_intervals = (start_time, end_time),
+            polygon = pimlico_tube_station,
+        )
 
-        Returns
-        -------
-        List of unique entities in time interval and polygon.
-
-        Example
-        -------
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> start_time = datetime.strptime("2022-01-01T08:00:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
-        >>> end_time = datetime.strptime("2022-01-01T08:30:00.000Z", "%Y-%m-%dT%H:%M:%S.%fZ")
-        >>> pimlico_tube_station =  [
-        ...     [-0.13410870522207574, 51.48932327401289],
-        ...     [-0.1355577905032419, 51.48887697878598],
-        ...     [-0.1339996342869938, 51.487266398812636],
-        ...     [-0.13279985400049554, 51.487508959676234],
-        ...     [-0.13230124401115972, 51.4875768764868],
-        ...     [-0.1319428680814667, 51.487955268294115],
-        ...     [-0.1322389177630896, 51.4883918703234],
-        ...     [-0.1322389177630896, 51.48887697878598],
-        ...     [-0.13301799587057417, 51.48930386996324],
-        ...     [-0.13410870522207574, 51.48932327401289],
-        ... ]
-        >>> dfi.get.entities(
-        ...     time_intervals = (start_time, end_time),
-        ...     polygon = pimlico_tube_station,
-        ... )
+        ```
         """
 
         validate.time_interval(time_interval)
         validate.polygon(polygon)
 
         params = {"instance": self.conn.qualified_instance_name}
         payload = {}
@@ -481,24 +470,24 @@
         end_time = end_time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
     return start_time, end_time
 
 
 def _raise_query_error_event(event: sseclient.Event) -> None:
     """helper to raise a QueryError response error"""
     msg = f"event returned QueryError: {event.data}"
-    logger.error(msg)
+    _logger.error(msg)
     raise validate.DFIResponseError(msg)
 
 
 def _raise_unexpected_event_found(event: sseclient.Event) -> None:
     """helper to raise a an unexpected event was found"""
     msg = f"Unexpected event in bagging area: {event}"
-    logger.error(msg)
+    _logger.error(msg)
     raise validate.DFIResponseError(msg)
 
 
 def _raise_message_event_not_reached() -> None:
     """helper to raise a warning if the "message" event was not reached."""
     # see DFIS-694
     msg = "DFI provided no 'message' events."
-    logger.warning(msg)
+    _logger.warning(msg)
     warnings.warn(msg)
```

### Comparing `dfipy-1.0.1/dfi/polygons.py` & `dfipy-1.0.2/dfi/polygons.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 """
-Class with DFI polygon DB, wrappers of the DFI python API.
-Composition of the class Connection, aimed at accessing the
-polygon DB, where a dataset of named polygons is made available to the user.
+Storage and retrieval of named polygons in the DFI Web API.
 """
 
 import logging
 from typing import List
 
 from dfi import validate
 from dfi.connect import Connect
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class Polygons:
     """
     Class responsible to call the DFI API and access the polygons DB.
 
     The polygon DB is a dataset of named polygons. It is made available to the user within the same
     namespace of where the DFI instances lives.
 
     It can be accessed via the a dfi.Client class instance or it must be instantiated
     with a dfi.Connect instance as argument.
 
-    Parameters
-    ----------
-    dfi_conn : Connect
-        Instance of a Connect with the credentials and namespace of the DFI connection.
+    :param dfi_conn: Instance of a Connect with the credentials and namespace of the DFI connection.
 
-    Examples
-    --------
+    :example:
     Access via the Client class:
 
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> dfi_polygons.get_vertices("my polygon name")
+    ```python
+    from dfi import Client
 
-    Or access only the Polygons class directly:
+    dfi = Client(dfi_token, instance_name, namespace, base_url)
 
-        >>> from dfi.connect import Connect
-        >>> from dfi.get import Polygons
-        >>> conn = dfi.Connect(api_token, instance_name, namespace, base_url)
-        >>> dfi_polygons = dfi.Polygons(conn)
-        >>> dfi_polygons.get_vertices("my polygon name")
+    dfi_polygons.get_vertices("my polygon name")
+    ```
 
+    Or access only the Polygons class directly:
+    ```python
+    from dfi.connect import Connect
+    from dfi.polygons import Polygons
+
+    conn = dfi.Connect(api_token, instance_name, namespace, base_url)
+
+    dfi_polygons = dfi.Polygons(conn)
+    dfi_polygons.get_vertices("my polygon name")
+    ```
     """
 
     def __init__(self, dfi_conn: Connect) -> None:
         self.conn: Connect = dfi_conn
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.conn!r})"
@@ -55,46 +55,43 @@
     def __str__(self) -> str:
         return f"""Instance of dfi.{self.__class__.__name__} composed with: {self.conn!s}"""
 
     def get_names(self) -> List[dict]:
         """
         Retrieves a list of saved polygons.
 
-        Example
-        -------
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> dfi.polygon.get_names()
+        :example:
+        ```python
+        from dfi import Client
 
+        dfi = Client(dfi_token, instance_name, namespace, base_url)
+
+        dfi.polygons.get_names()
+        ```
         """
 
         with self.conn.api_get("polygons") as response:
             list_polygons = response.json().get("polygons")
             validate.list_polygons_response(list_polygons, response)
             return list_polygons
 
     def get_vertices(self, polygon_name: str) -> List[List[float]]:
         """
         Get the list of a polygon saved in the polygon database from its name.
 
-        Parameters
-        ----------
-        polygon_name: str
-            Name of the polygon the user wants to retrieve from the polygons database.
-
-        Return
-        -------
-        List of the polygon coordinates.
-
-        Example
-        -------
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> dfi.polygon.get_names()
-        >>> dfi.polygon.get_vertices('my-first-polygon')
-
+        :param polygon_name: Name of the polygon the user wants to retrieve from the polygons database.
+        :returns: List of the polygon coordinates.
+        :example:
+        ```python
+        from dfi import Client
+
+        dfi = Client(dfi_token, instance_name, namespace, base_url)
+
+        dfi.polygons.get_names()
+        dfi.polygons.get_vertices('my-first-polygon')
+        ```
         """
 
         with self.conn.api_get("polygons/" + polygon_name) as response:
             vertices = response.json().get("vertices")
             validate.vertices_response(vertices, response)
             return vertices
```

### Comparing `dfipy-1.0.1/dfi/show.py` & `dfipy-1.0.2/dfi/show.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
-Class with methods to show DFI results.
-Composition of the class Connection.
+Provides a simple way to visualize query results on a map.  For instructions see [Kepler.GL](https://kepler.gl/) user guide.
+
+:::{attention}
+This module should be considered experimental and subject to change.
+:::
 """
 
 import logging
 from copy import deepcopy
 from typing import List, Optional, Tuple, Union
 
 import geopandas as gpd
@@ -13,45 +16,36 @@
 from shapely.geometry import Polygon
 
 from dfi import validate
 from dfi.connect import Connect
 from dfi.models import Polygon as ModelPolygons
 from dfi.polygons import Polygons
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class Show:
     """
     Visualisation methods to build use case on top of the queries from DFI.
 
     It can be accessed via the a dfi.Client class instance or it must be instantiated
     with a dfi.Connect instance as argument.
 
-    Parameters
-    ----------
-    dfi_conn : Connect
-        Instance of a Connect with the credentials and namespace of the DFI connection.
+    :param dfi_conn: Instance of a Connect with the credentials and namespace of the DFI connection.
 
-    Examples
-    --------
+    :exmaple:
     Access via the Client class:
 
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> dfi_polygons.get_vertices("my polygon name")
-
-    Or access only the Polygons class directly:
-
-        >>> from dfi.connect import Connect
-        >>> from dfi.get import Polygons
-        >>> conn = dfi.Connect(api_token, instance_name, namespace, base_url)
-        >>> dfi_polygons = dfi.Polygons(conn)
-        >>> dfi_polygons.get_vertices("my polygon name")
+    ```python
+    from dfi import Client
+
+    dfi = Client(dfi_token, instance_name, namespace, base_url)
 
+    dfi.show.map() # creates an empty Kepler map
+    ```
     """
 
     def __init__(self, dfi_conn: Connect) -> None:
         self.conn: Connect = dfi_conn
         self.polygons = Polygons(self.conn)
 
     def __repr__(self) -> str:
@@ -69,38 +63,39 @@
         map_height: int = 1200,
         config: Optional[dict] = None,
     ) -> KeplerGl:
         """
         Helper method to crete a kepler map with the given input layers, to reproduce proposed
         examples in the example notebooks.
 
-        Parameters
-        ----------
-        list_polygons: Optional[List[str]]
-            List of polygons, as list of vertices [[lon1, lat1], [lon2, lat2], ...].
-        list_polygons_by_names: Optional[List[str]]
-            List of polygon names as they are named in the auxiliary Polygon DB.
-        df_records: Optional[pd.DataFrame]
-            Dataframe of records with record_id, timestamp, latitude, longitude as its columns.
-        list_dfs: Optional[Union[gpd.GeoDataFrame, pd.DataFrame]] = None,
-            Generic list of any dataframe or geodataframe to be visualised on the map.
-        map_height: int = 1200
-            Parameter passed to the KeplerGl instance as it is, overriding the default.
-        config: Optional[dict] = None
-            Parameter passed to the KeplerGl instance as it is.
-
-        Return
-        -------
-        Instance of a kepler map with the given data to visualise.
-
-        Example
-        -------
-        >>> from dfi import Client
-        >>> dfi = Client(dfi_token, instance_name, namespace, base_url)
-        >>> dfi.show.map()  # creates an empty Kepler map
+        :param list_polygons: List of polygons, as list of vertices [[lon1, lat1], [lon2, lat2], ...].
+        :param list_polygons_by_names: List of polygon names as they are named in the auxiliary Polygon DB.
+        :param df_records: Dataframe of records with record_id, timestamp, latitude, longitude as its columns.
+        :param list_dfs: Generic list of any dataframe or geodataframe to be visualised on the map.
+        :param map_height: Parameter passed to the KeplerGl instance as it is, overriding the default.
+        :param config: A KeplerGL map config.  See [KeplerGL docs](https://github.com/keplergl/kepler.gl/tree/master/bindings/kepler.gl-jupyter#for-jupyter-notebook-and-jupyterlab) for more info.
+        :returns: Instance of a KeplerGL map with the given data to visualise.
+        :example:
+        ```python
+        from dfi import Client
+
+        dfi = Client(dfi_token, instance_name, namespace, base_url)
+
+        df = dfi.get.records(
+            entities = ["a1a2a3a4-b1b2-c1c2-d1d2-d3d4d5d6d7d8"]
+        )
+
+        dfi.show.map(
+            df_records=df
+        )
+        ```
+
+        :::{note}
+        For instructions see [Kepler.GL](https://kepler.gl/) user guide.
+        :::
         """
         if list_polygons is None:
             list_polygons = []
 
         list_polygons_as_vertices = []
         for poly in list_polygons:
             # from bounding boxes to vertices
@@ -139,11 +134,11 @@
 
         if config is None:
             return KeplerGl(data=deepcopy(kepler_data), height=map_height)
         return KeplerGl(data=deepcopy(kepler_data), height=map_height, config=config)
 
 
 def from_bbox_to_polygon_list(bounding_box: List[float]) -> Tuple[Tuple[float, float]]:
-    """Convert a bounding box, passed as a list [min_lon, min_lat, max_lon, max_lat] into a tuple of vertices"""
+    """Convert a bounding box, passed as a list `[min_lon, min_lat, max_lon, max_lat]` into a tuple of vertices."""
     validate.bounding_box(bounding_box)
     min_lon, min_lat, max_lon, max_lat = bounding_box
     return ((max_lon, max_lat), (max_lon, min_lat), (min_lon, min_lat), (min_lon, max_lat), (max_lon, max_lat))
```

### Comparing `dfipy-1.0.1/dfi/validate.py` & `dfipy-1.0.2/dfi/validate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 Module with private validator methods used across classes.
 
 Some will be improved and delegated to the DFI API.
 
-Example
--------
->>> from dfi import validate
->>> validate.df_records(df_records)
+:example:
+```python
+from dfi import validate
+
+validate.df_records(df_records)
+```
+
 """
 import json
 import logging
 from datetime import datetime
 from typing import List, Optional
 
 import pandas as pd
 import requests
 
 from dfi import models
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class DFIResponseError(Exception):
     """Raised when an error propagated back from the HTTP API"""
 
 
 class DFIResponseWarning(Warning):
@@ -40,51 +43,94 @@
 class DFIInputValueOutOfBoundError(Exception):
     """Raised when the user passes a wrong input value to the DFI query"""
 
 
 def df_records(df_rec: pd.DataFrame) -> None:
     """
     Check the column names are correct.
+
+    :param h3_res: A dataframe of records
+    :returns `None`:
+    :raises `DFIDataFrameColumnsNameError`: If a column name is not in
+        `["entity_id", "latitude", "longitude", "timestamp"]`
     """
     for col_name in ["entity_id", "latitude", "longitude", "timestamp"]:
         if col_name not in df_rec.columns:
             raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
 
 
 def h3_resolution(h3_res: int) -> None:
-    """check the input is within an acceptable range."""
+    """
+    check the input is within an acceptable range.
+
+    :param `h3_res`: An H3 resolution
+    :returns: `None`
+    :raises `DFIInputValueOutOfBoundError`:  If not 1<= h3_res <= 15
+    """
     if (h3_res < 1) or (h3_res > 15):
         raise DFIInputValueOutOfBoundError(
             f"Resolution is incorrect. It must be between 1 and 15. User passed {h3_res}"
         )
 
 
 def vertices_response(vert: Optional[models.Polygon], resp: requests.models.Response) -> None:
+    """
+    :param vert:
+    :returns: `None`
+    :raises `DFIResponseError`: If there was an error querying the DFI API.
+
+    :::{TODO}
+    Display error from API.
+    :::
+    """
     if vert is None:
         msg = f"Polygon vertices can not be retrieved from the json response: {resp.json()}"
-        logger.error(msg)
+        _logger.error(msg)
         raise DFIResponseError(msg)
 
 
 def list_polygons_response(vert: Optional[models.Polygon], resp: requests.models.Response) -> None:
+    """
+    :param vert:
+    :returns: `None`
+    :raises `DFIResponseError`: If there was an error querying the DFI API.
+
+    :::{TODO}
+    Display error from API.
+    :::
+    """
     if vert is None:
         msg = f"Polygon list can not be retrieved from the json response: {resp.json()}"
-        logger.error(msg)
+        _logger.error(msg)
         raise DFIResponseError(msg)
 
 
 def response(
     resp: requests.models.Response,
     url: str,
     headers: dict,
     params: dict,
     payload: Optional[dict] = None,
 ) -> None:
     """
     Log the response of a request with the given parameters. Raise an error if status code is not 20x.
+
+    :param resp: a response object
+    :param url: the queried url
+    :param headers: request headers
+    :param params: request params
+    :param payload: request payload
+
+    :returns: `None`
+
+    :raises `DFIResponseError`: If there was an error querying the DFI API.
+
+    :::{TODO}
+    Display error from API.
+    :::
     """
     # prevent from showing the user token to terminal and logs
     headers = headers.copy()
     headers["X-API-TOKEN"] = "Bearer XXX"
 
     msg = f"""Response status code {resp.status_code}.
 Query URL: {url},
@@ -93,23 +139,27 @@
 """
     if payload is not None:
         msg += f"PAYLOAD: {json.dumps(payload, sort_keys=True, indent=4)}"
 
     if int(resp.status_code / 10) != 20:
         msg += f" Status Code {resp.status_code}. "
         msg += resp.text
-        logger.error(msg)
+        _logger.error(msg)
         raise DFIResponseError(msg)
 
-    logger.debug(msg)
+    _logger.debug(msg)
 
 
 def time_interval(time_interv: Optional[models.TimeInterval] = None) -> None:
     """
     Validate input datetimes are both given and compatible.
+
+    :param time_interv: - a tuple of start time and end time bounds e.g. `(start_time, end_time)`
+    :returns: `None`
+    :raises `DFIInputValueError`: If `time_interv` is ill-formed.
     """
     if time_interv is None:
         return
     if len(time_interv) != 2:
         msg = f"Time interval is not an interval with two dates. User passed {time_interv}"
         raise DFIInputValueError(msg)
 
@@ -136,14 +186,18 @@
         msg = f"Start time {start_time} happened after than end time {end_time}."
         raise DFIInputValueError(msg)
 
 
 def entities(input_entities: Optional[List[str]]) -> None:
     """
     Validate a given list of entities is a list of strings.
+
+    :param `input_entities`: a list of entity ids
+    :returns: `None`
+    :raises `DFIInputValueError`: If `input_entities` is not a list of string or is empty or has duplicates.
     """
     if input_entities is None:
         return
     if not isinstance(input_entities, list):
         raise DFIInputValueError(f"Entities must be a list of strings. Received {input_entities}")
     if len(input_entities) == 0:
         raise DFIInputValueError("Entities must be a list of strings. Received an empty list")
@@ -152,22 +206,26 @@
         raise DFIInputValueError(f"Entities list must not contain duplicates. Duplicates found {duplicates_found}")
 
 
 def vertices(input_vertices: Optional[List[List[float]]]) -> None:
     """
     Check input list of vertices correspond to a polygon.
     It does not check if the polygon is simple.
+
+    :param input_vertices: a list of polygon vertices
+    :returns: `None`
+    :raises `DFIInputValueError`: If `input_vertices` is ill-formed.
     """
     if input_vertices is None:
         return
     if len(input_vertices) < 3:
-        raise DFIInputValueError("A polygon can not have less than 3 vertices. User passed {vertices}.")
+        raise DFIInputValueError(f"A polygon can not have less than 3 vertices. User passed {input_vertices}.")
     for vertex in input_vertices:
         if not len(vertex) == 2:
-            raise DFIInputValueError("Length of each vertex must be 2. User passed {vertex}")
+            raise DFIInputValueError(f"Length of each vertex must be 2. User passed {vertex}")
         if not isinstance(vertex[0], float) or not isinstance(vertex[1], float):
             raise DFIInputValueError(
                 f"Coordinates must be of type float."
                 f" User passed {vertex} of types ({type(vertex[0])}, {type(vertex[1])})"
             )
         lng, lat = vertex
         if not -180 < lng <= 180:
@@ -178,14 +236,19 @@
     if not input_vertices[0] == input_vertices[-1]:
         raise DFIInputValueError("First and last vertices are expected to be identical points.")
 
 
 def bounding_box(list_bbox: Optional[List[float]]) -> None:
     """
     Check input list of coordinates correspond to a bounding box, with lon, lat within the range.
+
+    :param list_bbox: a bbox
+    :returns: `None`
+    :raises `DFIInputValueError`: If `polygon` is ill-formed.
+    :raises `DFIInputValueOutOfBoundError`: If not -180.0 < longitude <= 180.0 or not -90 < latitude <= 90.0.
     """
     if list_bbox is None:
         return
     if len(list_bbox) != 4:
         raise DFIInputValueError(f"Input bounding box parameters must be a list of 4 floats. User passed {list_bbox}")
     for value in list_bbox:
         if not isinstance(value, float):
@@ -202,38 +265,52 @@
     if not -90 < max_lat < 90:
         raise DFIInputValueOutOfBoundError(f"Input max latitude {max_lat} is out of range.")
 
 
 def polygon(poly: Optional[models.Polygon]) -> None:
     """
     Check input list of coordinates correspond to a list of vertices, or a bounding box.
+
+    :param poly: A list of vertices or bbox.
+    :returns `None`:
+    :raises `DFIInputValueError`: If `polygon` is ill-formed.
     """
     if poly is None:
         return
     if not isinstance(poly, (list, tuple)):
-        return DFIInputValueError(f"Polygon {poly} must be of type list or tuple.")
+        raise DFIInputValueError(f"Polygon {poly} must be of type list or tuple.")
     if len(poly) == 0:
         raise DFIInputValueError(f"Given polygon {poly} is empty.")
     if not isinstance(poly[0], (list, tuple, float)):
-        return DFIInputValueError(f"Polygon {poly} must be a list of tuples or floats.")
+        raise DFIInputValueError(f"Polygon {poly} must be a list of tuples or floats.")
     if isinstance(poly[0], float):
         bounding_box(poly)
     if isinstance(poly[0], (list, tuple)):
         vertices(poly)
 
 
 def df_hexes_heatmap(df_h3: pd.DataFrame) -> None:
     """
     Check the column names are correct.
+
+    :param df_h3: A dataframe with a `"hex_id"` column.
+    :returns: `None`
+    :raises `DFIDataFrameColumnsNameError`: If a column name is not in
+        `["entity_id", "latitude", "longitude", "timestamp", "hex_id", "period_start", "period end"]`
     """
     for col_name in ["entity_id", "latitude", "longitude", "timestamp", "hex_id", "period_start", "period end"]:
         if col_name not in df_h3.columns:
             raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
 
 
 def df_hexes(df_h3: pd.DataFrame) -> None:
     """
     Check the column names are correct.
+
+    :param df_h3: A dataframe with a `"hex_id"` column.
+    :returns: `None`
+    :raises `DFIDataFrameColumnsNameError`: If a column name is not in
+        `["entity_id", "latitude", "longitude", "timestamp", "hex_id"]`
     """
     for col_name in ["entity_id", "latitude", "longitude", "timestamp", "hex_id"]:
         if col_name not in df_h3.columns:
             raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
```

### Comparing `dfipy-1.0.1/pyproject.toml` & `dfipy-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -60,21 +60,24 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "1.0.1"
+version = "1.0.2"
 description = "DFI api python wrapper"
 authors = [
   "Maurizio Morriello <maurizio.morriello@generalsystem.com>",
   "Sebastiano Ferraris <sebastiano.ferraris@generalsystem.com>",
 ]
 readme = "README.md"
+homepage = "https://www.generalsystem.com/"
+repository = "https://github.com/thegeneralsystem/dfipy"
+documentation = "https://dfipy.docs.generalsystem.com/"
 include = ["LICENCE"]
 packages = [{ include = "dfi" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 h3 = "^3.7.6"
 pandas = "^2.0.1"
@@ -84,19 +87,31 @@
 sseclient-py = "^1.7.2"
 tqdm = "^4.65.0"
 numpy = "^1.24.3"
 geopandas = "^0.13.0"
 keplergl = "^0.3.2"
 setuptools = "^67.8.0"
 
+
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pylint = "^2.17.4"
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 pylance = "^0.4.19"
 
+[tool.poetry.group.docs.dependencies]
+myst_parser = "^2.0.0"
+pydata-sphinx-theme = "^0.13.3"
+sphinx = "^7.0.1"
+sphinx-autodoc2 = "^0.4.2"
+sphinx-favicon = "^1.0.1"
+sphinxcontrib-napoleon = "^0.7"
+sphinx-copybutton = "^0.5.2"
+
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dfipy-1.0.1/PKG-INFO` & `dfipy-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: DFI api python wrapper
+Home-page: https://www.generalsystem.com/
 Author: Maurizio Morriello
 Author-email: maurizio.morriello@generalsystem.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,43 +17,46 @@
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Documentation, https://dfipy.docs.generalsystem.com/
+Project-URL: Repository, https://github.com/thegeneralsystem/dfipy
 Description-Content-Type: text/markdown
 
-<img src="docs/gs_logo.png" width="40%" align="right">
+<img src="docs/source/_static/gs_logo.png" align="right">
 
 [![Python versions](https://img.shields.io/pypi/pyversions/dfipy.svg)](https://pypi.python.org/pypi/dfipy/)
 [![PyPI version](https://badge.fury.io/py/dfipy.svg)](https://badge.fury.io/py/dfipy)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)
 
 # DFI API wrapper
 
 ## About
 
 - Python library created by [General System](https://www.generalsystem.com/) and publicly available on [github](https://github.com/thegeneralsystem) to query and experiment with the Data Flow Index (DFI) platform.
 - DFI provides the user with an unparalled foundation and scalable solution for processing high velocity, high volume spatiotemporal workloads for any geospatial data science need.
+- [Read the code documentation](https://dfipy.docs.generalsystem.com/)
 - [Read the whitepaper](https://assets.website-files.com/636ce900cf2e67aab6340642/643807134214aebc2b29849c_General%20System_The%20Data%20Flow%20Index%20Whitepaper%20_%20Nov%2022.pdf)
 
 ## Quickstart
 
+- Enroll at <https://eap.generalsystem.com> if you have not done so already.
+
 - Get the **key token** to access the demo DFI at  [https://tokens.dataflowindex.io/](https://tokens.dataflowindex.io/).
 
 - **Install** with:
     ```bash
     pip install dfipy
     ```
 
-- [Quickstart guide](https://github.com/thegeneralsystem/quickstart-guide)
-  
-- [DfiPyExamples](https://github.com/thegeneralsystem/dfipy-examples)
+- Start querying with [DfiPy Examples](https://github.com/thegeneralsystem/dfipy-examples)
 
 ## Licence
 
 - Copyright (c) 2023, General System Group Limited.
 
 - DFIPy is provided as it is and copyrighted under [Apache2 License](LICENCE).
```

