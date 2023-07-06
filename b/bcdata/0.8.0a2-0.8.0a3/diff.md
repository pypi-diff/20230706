# Comparing `tmp/bcdata-0.8.0a2.tar.gz` & `tmp/bcdata-0.8.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdata-0.8.0a2.tar", last modified: Mon Jul  3 22:37:14 2023, max compression
+gzip compressed data, was "bcdata-0.8.0a3.tar", last modified: Thu Jul  6 00:10:05 2023, max compression
```

## Comparing `bcdata-0.8.0a2.tar` & `bcdata-0.8.0a3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.847999 bcdata-0.8.0a2/
--rw-r--r--   0 snorris    (501) staff       (20)     7313 2023-07-03 22:32:31.000000 bcdata-0.8.0a2/CHANGES.txt
--rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.8.0a2/LICENSE.txt
--rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-03 22:37:14.847743 bcdata-0.8.0a2/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)    15657 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/README.md
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.846099 bcdata-0.8.0a2/bcdata/
--rw-r--r--   0 snorris    (501) staff       (20)      351 2023-07-03 21:55:43.000000 bcdata-0.8.0a2/bcdata/__init__.py
--rw-r--r--   0 snorris    (501) staff       (20)     6196 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     4936 2023-07-03 22:27:54.000000 bcdata-0.8.0a2/bcdata/bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     9940 2023-06-29 22:02:05.000000 bcdata-0.8.0a2/bcdata/cli.py
--rw-r--r--   0 snorris    (501) staff       (20)     6337 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/database.py
--rw-r--r--   0 snorris    (501) staff       (20)     3654 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/wcs.py
--rw-r--r--   0 snorris    (501) staff       (20)    11261 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/wfs.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.846991 bcdata-0.8.0a2/bcdata.egg-info/
--rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)      474 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/SOURCES.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/dependency_links.txt
--rw-r--r--   0 snorris    (501) staff       (20)       42 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/entry_points.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.8.0a2/bcdata.egg-info/not-zip-safe
--rw-r--r--   0 snorris    (501) staff       (20)      134 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/requires.txt
--rw-r--r--   0 snorris    (501) staff       (20)        7 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/top_level.txt
--rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.8.0a2/pyproject.toml
--rw-r--r--   0 snorris    (501) staff       (20)      115 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/requirements.txt
--rw-r--r--   0 snorris    (501) staff       (20)       38 2023-07-03 22:37:14.848051 bcdata-0.8.0a2/setup.cfg
--rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.8.0a2/setup.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.847435 bcdata-0.8.0a2/tests/
--rw-r--r--   0 snorris    (501) staff       (20)     5033 2023-06-28 23:17:04.000000 bcdata-0.8.0a2/tests/test_bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     6088 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/tests/test_bcdata.py
--rw-r--r--   0 snorris    (501) staff       (20)    11744 2023-07-03 22:28:46.000000 bcdata-0.8.0a2/tests/test_bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.8.0a2/tests/test_cli.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.782237 bcdata-0.8.0a3/
+-rw-r--r--   0 snorris    (501) staff       (20)     7455 2023-07-06 00:08:01.000000 bcdata-0.8.0a3/CHANGES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.8.0a3/LICENSE.txt
+-rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-06 00:10:05.782093 bcdata-0.8.0a3/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)    15657 2023-06-29 21:33:29.000000 bcdata-0.8.0a3/README.md
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.780479 bcdata-0.8.0a3/bcdata/
+-rw-r--r--   0 snorris    (501) staff       (20)      351 2023-07-06 00:07:45.000000 bcdata-0.8.0a3/bcdata/__init__.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6513 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     4483 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)    10042 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6342 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/database.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3654 2023-07-04 20:29:20.000000 bcdata-0.8.0a3/bcdata/wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)    12144 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/wfs.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.781461 bcdata-0.8.0a3/bcdata.egg-info/
+-rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)      474 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       42 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/entry_points.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.8.0a3/bcdata.egg-info/not-zip-safe
+-rw-r--r--   0 snorris    (501) staff       (20)      134 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/requires.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        7 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/top_level.txt
+-rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.8.0a3/pyproject.toml
+-rw-r--r--   0 snorris    (501) staff       (20)      115 2023-06-29 21:33:29.000000 bcdata-0.8.0a3/requirements.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       38 2023-07-06 00:10:05.782273 bcdata-0.8.0a3/setup.cfg
+-rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.8.0a3/setup.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.781938 bcdata-0.8.0a3/tests/
+-rw-r--r--   0 snorris    (501) staff       (20)     5273 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/tests/test_bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6088 2023-06-29 21:33:29.000000 bcdata-0.8.0a3/tests/test_bcdata.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11744 2023-07-03 22:28:46.000000 bcdata-0.8.0a3/tests/test_bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.8.0a3/tests/test_cli.py
```

### Comparing `bcdata-0.8.0a2/CHANGES.txt` & `bcdata-0.8.0a3/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 =======
 
+0.8.0a3 (2023-07-05)
+------------------
+- improve retry logic on download error, further request minimization, fix bcdc regression from #135
+
 0.8.0a2 (2023-07-03)
 ------------------
 - handle tables with schema stored in bcdc resource with format='multiple' (#135)
 
 0.8.0a1 (2023-06-29)
 ------------------
 - cache WFS GetCapabilities response for faster requests and fewer http errors
```

### Comparing `bcdata-0.8.0a2/LICENSE.txt` & `bcdata-0.8.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a2/PKG-INFO` & `bcdata-0.8.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.8.0a2
+Version: 0.8.0a3
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bcdata-0.8.0a2/README.md` & `bcdata-0.8.0a3/README.md`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a2/bcdata/bc2pg.py` & `bcdata-0.8.0a3/bcdata/bc2pg.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,22 @@
     "MULTILINESTRING",
     "MULTILINESTRINGZ",
     "POLYGON",
     "MULTIPOLYGON",
 ]
 
 
-@retry(stop=stop_after_delay(10), wait=wait_random_exponential(multiplier=1, max=60))
+@retry(stop=stop_after_delay(120), wait=wait_random_exponential(multiplier=1, max=60))
 def _download(url):
     """offload download requests to geopandas, using tenacity to handle unsuccessful requests"""
-    return gpd.read_file(url)
+    try:
+        data = gpd.read_file(url)
+    except Exception:
+        log.error("Data transfer error")
+    return data
 
 
 def bc2pg(
     dataset,
     db_url,
     table=None,
     schema=None,
@@ -73,14 +77,19 @@
         column_names = db.get_columns(schema_name, table_name)
 
     # if not appending, define and create table
     else:
         # get info about the table from catalouge
         table_comments, table_details = bcdata.get_table_definition(dataset)
 
+        if not table_details:
+            raise ValueError(
+                "Cannot create table, schema details not found via bcdc api"
+            )
+
         # clean provided geometry type and ensure it is valid
         if geometry_type:
             geometry_type = geometry_type.upper()
             if geometry_type not in SUPPORTED_TYPES:
                 raise ValueError("Geometry type {geometry_type} is not supported")
 
         # if geometry type is not provided, infer from first 10 records in dataset
@@ -88,16 +97,16 @@
             geometry_type = bcdata.get_types(dataset, 10)[0]
 
         # build the table definition and create table
         table = db.define_table(
             schema_name,
             table_name,
             table_details,
-            table_comments,
             geometry_type,
+            table_comments,
             primary_key,
             append,
         )
         column_names = [c.name for c in table.columns]
 
     # check if column provided in sortby option is present in dataset
     if sortby and sortby.lower() not in column_names:
@@ -116,14 +125,15 @@
             pagesize=pagesize,
             crs="epsg:3005",
         )
         # loop through the requests
         for n, url in enumerate(urls):
             log.info(url)
             df = _download(url)
+            log.info(_download.retry.statistics)  # log the retry stats
             # tidy the resulting dataframe
             df = df.rename_geometry("geom")
             # lowercasify
             df.columns = df.columns.str.lower()
             # retain only columns matched in table definition
             df = df[column_names]
             # extract features with no geometry
```

### Comparing `bcdata-0.8.0a2/bcdata/bcdc.py` & `bcdata-0.8.0a3/bcdata/bcdc.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,49 +60,43 @@
         return []
     else:
         matches = []
         # iterate through results of search (packages)
         for result in r.json()["result"]["results"]:
             # iterate through resources associated with each package
             for resource in result["resources"]:
-                log.debug(resource)
-                # if resource is wms and url matches provided table name,
-                # extract the metadata
+                # wms format resource
                 if resource["format"] == "wms":
+                    # if wms, check for table name match in this location
                     if urlparse(resource["url"]).path.split("/")[3] == table_name:
                         if "object_table_comments" in resource.keys():
                             table_comments = resource["object_table_comments"]
                         else:
-                            log.info(f"No table comments found for {table_name}")
                             table_comments = None
+                        # only add to matches if schema details found
                         if "details" in resource.keys() and resource["details"] != "":
                             table_details = resource["details"]
-                        else:
-                            log.info(f"No details found for {table_name}")
-                            table_details = None
-                        if table_details and table_comments:
                             matches.append((table_comments, table_details))
-                # some datasets are documented in the resource with format="multiple", not format="wms"
-                # (for example, WHSE_FOREST_VEGETATION.OGSR_PRIORITY_DEF_AREA_CUR_SP)
+                            log.debug(resource)
+
+                # multiple format resource
                 elif resource["format"] == "multiple":
+                    # if multiple format, check for table name match in this location
                     if json.loads(resource["preview_info"])["layer_name"] == table_name:
                         if "object_table_comments" in resource.keys():
                             table_comments = resource["object_table_comments"]
                         else:
-                            log.info(f"No table comments found for {table_name}")
                             table_comments = None
-                        if "details" in resource.keys():
+                        # only add to matches if schema details found
+                        if "details" in resource.keys() and resource["details"] != "":
                             table_details = resource["details"]
-                        else:
-                            log.info(f"No details found for {table_name}")
-                            table_details = None
-                        if table_details and table_comments:
                             matches.append((table_comments, table_details))
+                            log.debug(resource)
+
         # uniquify the result
         if len(matches) > 0:
             matched = list(set(matches))[0]
             return (matched[0], json.loads(matched[1]))
         else:
-            log.warning(
-                f"BCDC search for {table_name} does not return expected details"
+            raise ValueError(
+                f"BCDC search for {table_name} does not return a table schema"
             )
-            return (None, None)
```

### Comparing `bcdata-0.8.0a2/bcdata/cli.py` & `bcdata-0.8.0a3/bcdata/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 import click
 from cligj import indent_opt
 from cligj import compact_opt
 from cligj import verbose_opt, quiet_opt
 
 import bcdata
 
+LOG_FORMAT = "%(asctime)s:%(levelname)s:%(name)s: %(message)s"
+
 
 def configure_logging(verbosity):
     log_level = max(10, 30 - 10 * verbosity)
-    logging.basicConfig(stream=sys.stderr, level=log_level)
+    logging.basicConfig(stream=sys.stderr, level=log_level, format=LOG_FORMAT)
 
 
 def complete_dataset_names(ctx, param, incomplete):
     return [k for k in bcdata.list_tables() if k.startswith(incomplete)]
 
 
 # bounds handling direct from rasterio
@@ -356,15 +358,15 @@
 
     \b
      $ bcdata bc2pg bc-airports --db_url postgresql://postgres:postgres@localhost:5432/postgis
     """
     # for this command, default to INFO level logging
     verbosity = verbose - quiet
     log_level = max(10, 20 - 10 * verbosity)
-    logging.basicConfig(stream=sys.stderr, level=log_level)
+    logging.basicConfig(stream=sys.stderr, level=log_level, format=LOG_FORMAT)
     log = logging.getLogger(__name__)
     if no_timestamp:
         timestamp = False
     else:
         timestamp = True
     out_table = bcdata.bc2pg(
         dataset,
```

### Comparing `bcdata-0.8.0a2/bcdata/database.py` & `bcdata-0.8.0a3/bcdata/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             self.execute(dbq)
 
     def define_table(
         self,
         schema_name,
         table_name,
         table_details,
-        table_comments,
         geom_type,
+        table_comments=None,
         primary_key=None,
         append=False,
     ):
         """build sqlalchemy table definition from bcdc provided json definitions"""
         # remove columns of unsupported types, redundant columns
         table_details = [
             c for c in table_details if c["data_type"] in self.supported_types.keys()
```

### Comparing `bcdata-0.8.0a2/bcdata/wcs.py` & `bcdata-0.8.0a3/bcdata/wcs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a2/bcdata/wfs.py` & `bcdata-0.8.0a3/bcdata/wfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import bcdata
 
 if not sys.warnoptions:
     warnings.simplefilter("ignore")
 
 log = logging.getLogger(__name__)
 
+
 WFS_URL = "https://openmaps.gov.bc.ca/geo/pub/wfs"
 OWS_URL = "http://openmaps.gov.bc.ca/geo/ows"
 
 
 def check_cache(path):
     """Return true if the getcapabilities cache does not exist or is more than a day old"""
     if not os.path.exists(path):
@@ -101,15 +102,15 @@
     """Return a list of all tables available via WFS"""
     capabilites = get_capabilities(cache_file)
     return [i.strip("pub:") for i in list(capabilites.contents)]
 
 
 @retry(
     retry=retry_if_exception_type(requests.exceptions.HTTPError),
-    stop=stop_after_delay(10),
+    stop=stop_after_delay(120),
     wait=wait_random_exponential(multiplier=1, max=60),
 )
 def get_count(dataset, query=None):
     """Ask DataBC WFS how many features there are in a table/query"""
     # https://gis.stackexchange.com/questions/45101/only-return-the-numberoffeatures-in-a-wfs-query
     table = validate_name(dataset)
     payload = {
@@ -118,46 +119,63 @@
         "request": "GetFeature",
         "typeName": table,
         "resultType": "hits",
         "outputFormat": "json",
     }
     if query:
         payload["CQL_FILTER"] = query
-
-    r = requests.get(WFS_URL, params=payload)
-    log.debug(r.url)
-    r.raise_for_status()  # check status code is 200
-    return int(ET.fromstring(r.text).attrib["numberMatched"])
+    try:
+        r = requests.get(WFS_URL, params=payload)
+        log.debug(r.url)
+        log.debug(r.headers)
+        r.raise_for_status()  # check status code is 200
+        return int(ET.fromstring(r.text).attrib["numberMatched"])
+    except Exception:
+        log.debug("Network error")
 
 
 def define_requests(
     dataset,
     query=None,
     crs="epsg:4326",
     bounds=None,
     bounds_crs="EPSG:3005",
     count=None,
     sortby=None,
     pagesize=10000,
+    check_count=True,
 ):
     """Translate provided parameters into a list of WFS request URLs required
     to download the dataset as specified
 
     References:
     - http://www.opengeospatial.org/standards/wfs
     - http://docs.geoserver.org/stable/en/user/services/wfs/vendor.html
     - http://docs.geoserver.org/latest/en/user/tutorials/cql/cql_tutorial.html
     """
-    # validate the table name and find out how many features it holds
+    # validate the table name
     table = validate_name(dataset)
-    n = bcdata.get_count(table, query=query)
-    # if count not provided or if it is greater than n of total features,
-    # set count to number of features
-    if not count or count > n:
-        count = n
+    # find out how many records are in the table
+    if not count and check_count is False:
+        raise ValueError(
+            "{count: Null, check_count=False} is invalid, either provide record count or let bcdata request it"
+        )
+    elif (
+        not count and check_count is True
+    ):  # if not provided a count, get one if not told otherwise
+        count = get_count(table, query=query)
+        log.info(get_count.retry.statistics)
+    elif (
+        count and check_count is True
+    ):  # if provided a count that is bigger than actual number of records, automatically correct count
+        n = get_count(table, query=query)
+        log.info(get_count.retry.statistics)
+        if count > n:
+            count = n
+
     log.info(f"Total features requested: {count}")
     wfs = get_capabilities()
     schema = wfs.get_schema("pub:" + table)
     geom_column = schema["geometry_column"]
 
     # for datasets with >10k records, generate a list of urls based on number of features in the dataset.
     chunks = math.ceil(count / pagesize)
@@ -200,15 +218,15 @@
                 request["count"] = pagesize
         urls.append(WFS_URL + "?" + urlencode(request, doseq=True))
     return urls
 
 
 @retry(
     retry=retry_if_exception_type(requests.exceptions.HTTPError),
-    stop=stop_after_delay(10),
+    stop=stop_after_delay(120),
     wait=wait_random_exponential(multiplier=1, max=60),
 )
 def make_request(url):
     """Submit a getfeature request to DataBC WFS and return features"""
     r = requests.get(url)
     log.info(r.url)
     log.debug(r.headers)
@@ -239,14 +257,15 @@
         sortby=sortby,
         pagesize=pagesize,
     )
     # loop through requests
     results = []
     for url in urls:
         results.append(make_request(url))
+        log.info(make_request.retry.statistics)
 
     outjson = dict(type="FeatureCollection", features=[])
     for result in results:
         outjson["features"] += result
     # if specified, lowercasify all properties
     if lowercase:
         for feature in outjson["features"]:
@@ -277,43 +296,48 @@
     crs="epsg:4326",
     bounds=None,
     bounds_crs="epsg:3005",
     count=None,
     sortby=None,
     pagesize=10000,
     lowercase=False,
+    check_count=True,
 ):
     """Yield features from DataBC WFS"""
     urls = define_requests(
         dataset,
         query=query,
         crs=crs,
         bounds=bounds,
         bounds_crs=bounds_crs,
         count=count,
         sortby=sortby,
         pagesize=pagesize,
+        check_count=check_count,
     )
     for url in urls:
         for feature in make_request(url):
             if lowercase:
                 feature["properties"] = {
                     k.lower(): v for k, v in feature["properties"].items()
                 }
             yield feature
+        log.info(make_request.retry.statistics)
 
 
 def get_types(dataset, count=10):
     """Return distinct types within the first n features"""
     # validate the table name
     table = validate_name(dataset)
     log.info("Getting feature geometry type")
     # get first n features, examine the feature geometry type (where geometry is not empty)
     geom_types = []
-    for f in get_features(table, count=count):
+    for f in get_features(
+        table, count=count, check_count=False
+    ):  # to minimize network traffic, do not check record count for this requests
         if f["geometry"]:
             geom_type = f["geometry"]["type"].upper()
             # only these geometry types are expected/supported
             if geom_type not in (
                 "POINT",
                 "LINESTRING",
                 "POLYGON",
```

### Comparing `bcdata-0.8.0a2/bcdata.egg-info/PKG-INFO` & `bcdata-0.8.0a3/bcdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.8.0a2
+Version: 0.8.0a3
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bcdata-0.8.0a2/setup.py` & `bcdata-0.8.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a2/tests/test_bc2pg.py` & `bcdata-0.8.0a3/tests/test_bc2pg.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 def test_bc2pg():
     bcdata.bc2pg(AIRPORTS_TABLE, DB_URL)
     assert AIRPORTS_TABLE in DB_CONNECTION.tables
     DB_CONNECTION.execute("drop table " + AIRPORTS_TABLE)
 
 
+def test_bc2pg_50kgrid():
+    bcdata.bc2pg("whse_basemapping.dbm_mof_50k_grid", DB_URL)
+    assert "whse_basemapping.dbm_mof_50k_grid" in DB_CONNECTION.tables
+    DB_CONNECTION.execute("drop table " + "whse_basemapping.dbm_mof_50k_grid")
+
+
 def test_bc2pg_count():
     bcdata.bc2pg(AIRPORTS_TABLE, DB_URL, count=10)
     assert AIRPORTS_TABLE in DB_CONNECTION.tables
     r = DB_CONNECTION.query(
         "select airport_name from whse_imagery_and_base_maps.gsr_airports_svw"
     )
     assert len(r) == 10
```

### Comparing `bcdata-0.8.0a2/tests/test_bcdata.py` & `bcdata-0.8.0a3/tests/test_bcdata.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a2/tests/test_bcdc.py` & `bcdata-0.8.0a3/tests/test_bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a2/tests/test_cli.py` & `bcdata-0.8.0a3/tests/test_cli.py`

 * *Files identical despite different names*

