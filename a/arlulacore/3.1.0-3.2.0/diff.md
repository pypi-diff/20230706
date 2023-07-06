# Comparing `tmp/arlulacore-3.1.0.tar.gz` & `tmp/arlulacore-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlulacore-3.1.0.tar", last modified: Tue Jan 17 03:16:02 2023, max compression
+gzip compressed data, was "arlulacore-3.2.0.tar", last modified: Thu Jul  6 00:00:58 2023, max compression
```

## Comparing `arlulacore-3.1.0.tar` & `arlulacore-3.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 03:16:02.496733 arlulacore-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-17 03:15:53.000000 arlulacore-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-01-17 03:16:02.496733 arlulacore-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-01-17 03:15:53.000000 arlulacore-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 03:16:02.492732 arlulacore-3.1.0/arlulacore/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/arlula.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-01-17 03:15:53.000000 arlulacore-3.1.0/arlulacore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 03:16:02.496733 arlulacore-3.1.0/arlulacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-01-17 03:16:02.000000 arlulacore-3.1.0/arlulacore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-17 03:16:02.000000 arlulacore-3.1.0/arlulacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 03:16:02.000000 arlulacore-3.1.0/arlulacore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-17 03:16:02.000000 arlulacore-3.1.0/arlulacore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-17 03:16:02.000000 arlulacore-3.1.0/arlulacore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 03:16:02.496733 arlulacore-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-17 03:15:53.000000 arlulacore-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:00:58.918454 arlulacore-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 00:00:46.000000 arlulacore-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-06 00:00:58.918454 arlulacore-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-06 00:00:46.000000 arlulacore-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:00:58.918454 arlulacore-3.2.0/arlulacore/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/arlula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-06 00:00:46.000000 arlulacore-3.2.0/arlulacore/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:00:58.918454 arlulacore-3.2.0/arlulacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-06 00:00:58.000000 arlulacore-3.2.0/arlulacore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 00:00:58.000000 arlulacore-3.2.0/arlulacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:00:58.000000 arlulacore-3.2.0/arlulacore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 00:00:58.000000 arlulacore-3.2.0/arlulacore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 00:00:58.000000 arlulacore-3.2.0/arlulacore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 00:00:58.918454 arlulacore-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 00:00:46.000000 arlulacore-3.2.0/setup.py
```

### Comparing `arlulacore-3.1.0/LICENSE` & `arlulacore-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arlulacore-3.1.0/PKG-INFO` & `arlulacore-3.2.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlulacore
-Version: 3.1.0
+Version: 3.2.0
 Summary: A package to facilitate access to the Arlula Imagery Marketplace API
 Home-page: https://github.com/Arlula/python-core-sdk.git
 Author: Arlula
 Author-email: tech@arlula.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arlulacore-3.1.0/README.md` & `arlulacore-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arlulacore-3.1.0/arlulacore/__init__.py` & `arlulacore-3.2.0/arlulacore/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     License,
     Band,
     Bundle,
     SearchResult,
     SearchResponse,
     SearchRequest,
     OrderRequest,
+    BatchOrderRequest,
     ArchiveAPI,
     Polygon,
 )
 from .orders import (
     OrderResult,
     OrdersAPI,
     DetailedOrderResult,
```

### Comparing `arlulacore-3.1.0/arlulacore/archive.py` & `arlulacore-3.2.0/arlulacore/archive.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from datetime import date, datetime
 from .common import ArlulaObject
 from .auth import Session
 from .exception import ArlulaAPIException
 from .orders import DetailedOrderResult
 from .util import parse_rfc3339, calculate_price, remove_none, simple_indent
 
-Polygon = typing.Union[typing.List[typing.List[typing.List[float]]], str]
+Polygon = typing.List[typing.List[typing.List[float]]]
 
 class CenterPoint(ArlulaObject):
     data: dict
     long: float
     lat: float
 
     def __init__(self, data):
@@ -166,15 +166,15 @@
     area: float
     center: CenterPoint
     bounding: typing.List[typing.List[typing.List[float]]]
     overlap: Overlap
     fulfillment_time: float
     ordering_id: str
     bundles: typing.List[Bundle]
-    license: typing.List[License]
+    licenses: typing.List[License]
     annotations: typing.List[str]
 
     def __init__(self, data):
         self.data = data
         self.scene_id = data["sceneID"]
         self.supplier = data["supplier"]
         self.platform = data["platform"]
@@ -194,35 +194,35 @@
         self.overlap = Overlap(data["overlap"])
         self.fulfillment_time = data["fulfillmentTime"]
 
         self.ordering_id = data["orderingID"]
             
         self.bundles = []
         self.bundles += [Bundle(b) for b in data["bundles"]]
-        self.license = []
-        self.license += [License(l) for l in data["license"]]
+        self.licenses = []
+        self.licenses += [License(l) for l in data["licenses"]]
 
         self.annotations = []
         if "annotations" in data:
             self.annotations = data["annotations"]
 
     def calculate_price(self, license_href: string, bundle_key: string) -> int:
         '''
             Wrapper for util.calculate_price, returns price in US Cents. Raises error in the case of invalid license_name or bundle_key
         '''
         
         bundle = None
         license = None
         
         for b in self.bundles:
-            if bundle.key == bundle_key:
+            if b.key == bundle_key:
                 bundle = b
         
-        for l in self.license:
-            if license.href == license_href:
+        for l in self.licenses:
+            if l.href == license_href:
                 license = l
 
         if bundle == None:
             raise ValueError("Invalid bundle_key")
 
         if license == None:
             raise ValueError("Invalid license_href")
@@ -232,15 +232,15 @@
     def dict(self) -> dict:
         return self.data
 
     def __str__(self) -> str:
 
         bundles = simple_indent(''.join([str(b) for b in self.bundles]), 2, 2)
         bands = simple_indent(''.join([str(b) for b in self.bands]), 2, 2)
-        license = simple_indent(''.join([str(l) for l in self.license]), 2, 2)
+        licenses = simple_indent(''.join([str(l) for l in self.licenses]), 2, 2)
         return simple_indent(
             f"Result ({self.ordering_id}):\n"\
             f"Scene ID: {self.scene_id}\n"\
             f"Supplier: {self.supplier}\n"\
             f"Platform: {self.platform}\n"\
             f"Capture Date: {self.date.strftime('%Y-%m-%d')}\n"\
             f"Thumbnail URL: {self.thumbnail}\n"\
@@ -252,16 +252,16 @@
             f"{str(self.center)}\n"\
             f"Bounding: {self.bounding}\n"\
             f"{str(self.overlap)}"\
             f"Bands:\n"\
             f"{bands}"
             f"Bundles: \n"\
             f"{bundles}"
-            f"License: \n"\
-            f"{license}"
+            f"Licenses: \n"\
+            f"{licenses}"
             f"Annotations: {', '.join(self.annotations)}\n", 0, 2)
 
 class SearchResponse(ArlulaObject):
     data: dict
     state: string
     errors: typing.List[str]
     warnings: typing.List[str]
@@ -386,49 +386,68 @@
     def valid_area_of_interest(self) -> bool:
         return self.north != None and self.south != None and self.east != None and self.west != None
     
     def valid(self) -> bool:
         return (self.valid_area_of_interest() or self.valid_point_of_interest) and self.start != None and self.gsd != None
     
     def dict(self):
-        param_dict = {
+        d = {
             "start": str(self.start) if self.start != None else None, 
             "end": str(self.end) if self.end != None else None,
-            "gsd": self.gsd, "cloud": self.cloud,
-            "lat": self.lat, "long": self.long,
-            "north": self.north, "south": self.south, "east": self.east, 
-            "west": self.west, "supplier": self.supplier, "off-nadir": self.off_nadir,
-            "polygon": json.dumps(self.polygon) if isinstance(self.polygon, list) else self.polygon}
+            "gsd": self.gsd, 
+            "cloud": self.cloud,
+            "offNadir": self.off_nadir,
+            "supplier": self.supplier,
+        }
+
+        # Add the polygon if not None
+        if self.polygon != None:
+            d["polygon"] = self.polygon if isinstance(self.polygon, list) else self.polygon
+        # Add boundingBox if all related not None
+        elif self.north != None and self.east != None and self.west != None and self.south != None:
+            d["boundingBox"] = {
+                "north": self.north,
+                "east": self.east,
+                "west": self.west,
+                "south": self.south,
+            }
+        # Add latLong if all related not None
+        elif self.lat != None and self.long != None:
+            d["latLong"] = {
+                "latitude": self.lat,
+                "longitude": self.long,
+            }
 
-        query_params = {k: v for k, v in param_dict.items()
-            if v is not None}
-
-        return remove_none(query_params)
+        return remove_none(d)
 
 class OrderRequest(ArlulaObject):
 
     id: str
     eula: str
     bundle_key: str
     webhooks: typing.List[str]
     emails: typing.List[str]
+    team: str
+    payment: str
 
     def __init__(self,
             id: str,
             eula: str,
             bundle_key: str,
             webhooks: typing.Optional[typing.List[str]] = [],
             emails: typing.Optional[typing.List[str]] = [],
-            team: typing.Optional[str] = None):
+            team: typing.Optional[str] = None,
+            payment: typing.Optional[str] = None):
         self.id = id
         self.eula = eula
         self.bundle_key = bundle_key
         self.webhooks = webhooks
         self.emails = emails
         self.team = team
+        self.payment = payment
     
     def add_webhook(self, webhook: str) -> "OrderRequest":
         self.webhooks.append(webhook)
         return self
     
     def set_webhooks(self, webhooks: typing.List[str]) -> "OrderRequest":
         self.webhooks = webhooks
@@ -441,28 +460,99 @@
     def set_emails(self, emails: typing.List[str]) -> "OrderRequest":
         self.emails = emails
         return self
 
     def set_team(self, team: str) -> "OrderRequest":
         self.team = team
         return self
+    
+    def set_payment(self, payment: str) -> "OrderRequest":
+        self.payment = payment
+        return payment
 
     def valid(self) -> bool:
         return self.id != None and self.eula != None and self.bundle_key != None
 
     def dict(self):
         return remove_none({
             "id": self.id,
             "eula": self.eula,
             "bundleKey": self.bundle_key,
             "webhooks": self.webhooks,
             "emails": self.emails,
             "team": None if self.team == "" else self.team,
+            "payment": None if self.payment == "" else self.payment,
         })
 
+class BatchOrderRequest():
+
+    orders: typing.List[OrderRequest]
+    webhooks: typing.List[str]
+    emails: typing.List[str]
+    team: str
+    payment: str
+
+    def __init__(
+        self, 
+        orders: typing.Optional[typing.List[OrderRequest]] = [],
+        webhooks: typing.Optional[typing.List[str]] = [],
+        emails: typing.Optional[typing.List[str]] = [],
+        team: typing.Optional[str] = None,
+        payment: typing.Optional[str] = None):
+
+        self.orders = orders
+        self.webhooks = webhooks
+        self.emails = emails
+        self.team = team
+        self.payment = payment
+
+    def add_order(self, order: OrderRequest) -> "BatchOrderRequest":
+        self.orders.append(order)
+        return self
+    
+    def set_orders(self, orders: typing.List[OrderRequest]) -> "BatchOrderRequest":
+        self.orders = orders
+        return self
+
+    def add_webhook(self, webhook: str) -> "BatchOrderRequest":
+        self.webhooks.append(webhook)
+        return self
+    
+    def set_webhooks(self, webhooks: typing.List[str]) -> "BatchOrderRequest":
+        self.webhooks = webhooks
+        return self
+
+    def add_email(self, email: str) -> "BatchOrderRequest":
+        self.emails.append(email)
+        return self
+    
+    def set_emails(self, emails: typing.List[str]) -> "BatchOrderRequest":
+        self.emails = emails
+        return self
+
+    def set_team(self, team: str) -> "BatchOrderRequest":
+        self.team = team
+        return self
+    
+    def set_payment(self, payment: str) -> "BatchOrderRequest":
+        self.payment = payment
+        return self
+
+    def dict(self):
+        d = {
+            "orders": [o.dict() for o in self.orders],
+            "webhooks": self.webhooks,
+            "emails": self.emails,
+            "team": None if self.team == "" else self.team,
+            "payment": None if self.payment == "" else self.payment,
+        }
+
+        return remove_none(d)
+
+
 
 class ArchiveAPI:
     '''
         Archive is used to interface with the Arlula Archive API
     '''
 
     def __init__(self,
@@ -476,17 +566,17 @@
             Requires one of (lat, long) or (north, south, east, west).
         '''
 
         url = self.url+"/search"
 
         # Send request and handle responses
         response = requests.request(
-            "GET", url,
+            "POST", url,
             headers=self.session.header,
-            params=request.dict())
+            data=json.dumps(request.dict()))
         if response.status_code != 200:
             raise ArlulaAPIException(response)
         else:
             resp_data = json.loads(response.text)
             # Construct an instance of `SearchResponse`
             return SearchResponse(resp_data)
 
@@ -503,7 +593,26 @@
             data=json.dumps(request.dict()),
             headers=self.session.header)
 
         if response.status_code != 200:
             raise ArlulaAPIException(response)
         else:
             return DetailedOrderResult(json.loads(response.text))
+        
+    def batch_order(self, request: BatchOrderRequest) -> typing.List[DetailedOrderResult]:
+        '''
+            Order multiple scenes from the Arlula imagery archive
+        '''
+
+        url = self.url + "/order/batch"
+
+        response = requests.request(
+            "POST",
+            url,
+            data=json.dumps(request.dict()),
+            headers=self.session.header,
+        )
+
+        if response.status_code != 200:
+            raise ArlulaAPIException(response)
+        else:
+            return [DetailedOrderResult(r) for r in json.loads(response.text)]
```

### Comparing `arlulacore-3.1.0/arlulacore/arlula.py` & `arlulacore-3.2.0/arlulacore/arlula.py`

 * *Files identical despite different names*

### Comparing `arlulacore-3.1.0/arlulacore/auth.py` & `arlulacore-3.2.0/arlulacore/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .exception import ArlulaSessionError
 
 # Package Name
 name = "arlulacore"
 
 # User agent setting
-sdk_version = "3.1.0"
+sdk_version = "3.2.0"
 py_version = sys.version.split(' ')[0]
 os_version = platform.platform()
 def_ua = "core-sdk " + \
     sdk_version + " python " + py_version + " OS " + os_version
 
 # Expected API version
 x_api_version = '2023-01'
```

### Comparing `arlulacore-3.1.0/arlulacore/common.py` & `arlulacore-3.2.0/arlulacore/common.py`

 * *Files identical despite different names*

### Comparing `arlulacore-3.1.0/arlulacore/orders.py` & `arlulacore-3.2.0/arlulacore/orders.py`

 * *Files identical despite different names*

### Comparing `arlulacore-3.1.0/arlulacore/util.py` & `arlulacore-3.2.0/arlulacore/util.py`

 * *Files identical despite different names*

### Comparing `arlulacore-3.1.0/arlulacore.egg-info/PKG-INFO` & `arlulacore-3.2.0/arlulacore.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlulacore
-Version: 3.1.0
+Version: 3.2.0
 Summary: A package to facilitate access to the Arlula Imagery Marketplace API
 Home-page: https://github.com/Arlula/python-core-sdk.git
 Author: Arlula
 Author-email: tech@arlula.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arlulacore-3.1.0/setup.py` & `arlulacore-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='arlulacore',
-    version='3.1.0',
+    version='3.2.0',
     author="Arlula",
     author_email="tech@arlula.com",
     description="A package to facilitate access to the Arlula Imagery Marketplace API",
 
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Arlula/python-core-sdk.git",
```

