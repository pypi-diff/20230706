# Comparing `tmp/fa-models-1.0.73.tar.gz` & `tmp/fa-models-1.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.73.tar", last modified: Thu Jul  6 05:03:07 2023, max compression
+gzip compressed data, was "fa-models-1.0.74.tar", last modified: Thu Jul  6 07:39:48 2023, max compression
```

## Comparing `fa-models-1.0.73.tar` & `fa-models-1.0.74.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.464277 fa-models-1.0.73/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 05:03:07.460277 fa-models-1.0.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-06 05:02:32.000000 fa-models-1.0.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/famodels/models/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-06 05:02:57.000000 fa-models-1.0.73/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:03:07.464277 fa-models-1.0.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-06 05:02:32.000000 fa-models-1.0.73/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-06 05:02:32.000000 fa-models-1.0.73/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 05:02:32.000000 fa-models-1.0.73/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.154089 fa-models-1.0.74/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 07:39:48.154089 fa-models-1.0.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-06 07:39:17.000000 fa-models-1.0.74/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.146089 fa-models-1.0.74/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 07:39:48.000000 fa-models-1.0.74/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.146089 fa-models-1.0.74/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.150089 fa-models-1.0.74/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.154089 fa-models-1.0.74/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-06 07:39:17.000000 fa-models-1.0.74/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-06 07:39:40.000000 fa-models-1.0.74/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:39:48.154089 fa-models-1.0.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-06 07:39:17.000000 fa-models-1.0.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:39:48.154089 fa-models-1.0.74/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-06 07:39:17.000000 fa-models-1.0.74/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 07:39:17.000000 fa-models-1.0.74/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.73/PKG-INFO` & `fa-models-1.0.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.73
+Version: 1.0.74
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.73/README.md` & `fa-models-1.0.74/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.74/fa_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.73
+Version: 1.0.74
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.73/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.74/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/famodels/models/algorithm.py` & `fa-models-1.0.74/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/famodels/models/investor.py` & `fa-models-1.0.74/famodels/models/investor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 from typing import List, Optional
 from pydantic import EmailStr
 from redis_om import Field, JsonModel, EmbeddedJsonModel
 from redis_om.connections import get_redis_connection
 from famodels.models.person import Person
 from cryptography.fernet import Fernet
 from hashlib import sha256
@@ -25,14 +26,18 @@
 
 key = os.environ.get("ENCRYPTION_KEY").encode()
 ENCRYPTION_KEY = urlsafe_b64encode(sha256(key).digest())
 
 class Subscription(EmbeddedJsonModel):
     id: str = Field(index=False)
     algo_id:str = Field(index=True)
+    # redis model can only store these fields of the embedded json model as string
+    start_timestamp:str = Field(index=True, default=int(time.time() * 1000))
+    stop_timestamp: Optional[str]
+
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="subscription"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 class Fund(EmbeddedJsonModel):
     id:str = Field(index=True)
@@ -80,14 +85,16 @@
     class Meta:
         model_key_prefix = "exchange-key"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 
 class Investor(JsonModel):
     id: str = Field(index=True)
+    name: str = Field(index=True, full_text_search=True)
+    """company name or givenname & family name"""
     email: EmailStr = Field(index=True)
     accountable: Person = Field(index=True)        
     state: StateOfInvestor = Field(index=True, default=StateOfInvestor.REGISTERED.value)
     _passphrase: Optional[str]
     #library constraint: "redis_om.model.model.RedisModelError: In this Preview release, list and tuple fields can only contain strings. Problem field: compounding"
     funds: Optional[List[Fund]]
     exchange_keys: Optional[List[ExchangeKey]]
```

### Comparing `fa-models-1.0.73/famodels/models/market/public_trade.py` & `fa-models-1.0.74/famodels/models/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/famodels/models/order.py` & `fa-models-1.0.74/famodels/models/order.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List, Set, Optional
-from famodels.models.state_of_trade import StateOfTrade
 from famodels.models.direction import Direction
 from famodels.models.order_type import OrderType
 from famodels.models.side import Side
 from redis_om import (Field, JsonModel)
 from redis_om.connections import get_redis_connection
 import os
```

### Comparing `fa-models-1.0.73/famodels/models/person.py` & `fa-models-1.0.74/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/famodels/models/processed_signal.py` & `fa-models-1.0.74/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/famodels/models/signal_provider.py` & `fa-models-1.0.74/famodels/models/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/famodels/models/trade.py` & `fa-models-1.0.74/famodels/models/trade.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"the env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 class Trade(JsonModel):
     """A trade in our system is composed of a buy and a sell order. Do not mistaken it for a trade from the CEX.
         Create a new Trade record for every update and correlate them with trade_id. See attribute #trade_id"""   
     # id: Optional[int] = Field(default=None, primary_key=True)    
-    id: str = Field(default=str(uuid.uuid4().hex), nullable=False, primary_key=True)
+    id: str = Field(primary_key=True)
     # sort_index:int = field(init=False, repr=False)
     #trade_id: Optional[str] = Field(default=uuid.uuid4(), primary_key=True)
     """The trade id is the reference that keeps the state updates correlated. It will generate a UUID by default.
         Use this for the first record you insert. Inserting updated records (new records should then have the trade_id
         provided to create the correlation.)"""
     investor_id: str = Field(index=True)
     fund_id: str = Field(index=True)
     pos_idx:int
     market:str = Field(index=True)    
-    status:StateOfTrade = Field(index=True)
+    status:StateOfTrade = Field(index=True, default=StateOfTrade.NEW)
     direction:Direction
     amount: float
     time_of_initiation:datetime = Field(index=True, default=int(time.time() * 1000))
     """When we decided to start this trade."""
     buy_order_id: Optional[str] = None
     sell_order_id:Optional[str] = None
     take_profit:Optional[float] = None
```

### Comparing `fa-models-1.0.73/famodels/models/trading_signal.py` & `fa-models-1.0.74/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/famodels/models/virtual_order.py` & `fa-models-1.0.74/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/pyproject.toml` & `fa-models-1.0.74/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.73"
+version = "1.0.74"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.73"
+current_version = "1.0.74"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.73/setup.py` & `fa-models-1.0.74/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.73/tests/test_investor.py` & `fa-models-1.0.74/tests/test_investor.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system('docker stop redis-unit-test')
         os.system('docker rm redis-unit-test')
 
 
 def test_investor_model():
     # Now we can create an instance of `Investor` without connecting to a real Redis server
     person = Person(given_name="john", family_name="Doe", email="john@doe.com", sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
-    investor = Investor(id='123', email='test@example.com', accountable=person)    
+    investor = Investor(id='123', name="Jonathans Investements Ltd", email='test@example.com', accountable=person)    
 
 
 @pytest.mark.parametrize(
     "email, nationality_iso3, country_of_residence_iso3",
     [
         ("invalidemail", "GBR", "IRE"),  # invalid email
         ("john@doe.com", "GB", "IRE"),  # invalid nationality_iso3
@@ -97,46 +97,47 @@
 
     # Assert the attributes of the ExchangeKey
     assert exchange_key.exchange == exchange
     assert exchange_key.key_id == key_id
     assert exchange_key.get_key_secret(encryption_service) == key_secret
 
 @pytest.mark.parametrize(
-    "investor_id, email, funds",
+    "investor_id, name, email, funds",
     [
-        ("1", "investor1@example.com", [{"id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"id": "s2", "algo_id": "a2"}, {"id": "s3", "algo_id": "a3"}], "compounding": "false", "absolute_max_amount": 500.0}]),
-        ("2", "investor2@example.com", [{"id": "f3", "name": "fund3", "investor_id": "2", "subscriptions": [{"id": "s4", "algo_id": "a4"}, {"id": "s5", "algo_id": "a5"}, {"id": "s6", "algo_id": "a6"}], "compounding": 1}]),
-        ("3", "investor3@example.com", [{"id": "f4", "name": "fund4", "investor_id": "3", "subscriptions": [{"id": "s7", "algo_id": "a7"}], "compounding": 0, "absolute_max_amount": 10000.0}, {"id": "f5", "name": "fund5", "investor_id": "3", "subscriptions": [{"id": "s8", "algo_id": "a8"}, {"id": "s9", "algo_id": "a9"}, {"id": "s10", "algo_id": "a10"}]}])
+        ("1", "Superion Corp.", "investor1@example.com", [{"id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"id": "s2", "algo_id": "a2"}, {"id": "s3", "algo_id": "a3"}], "compounding": "false", "absolute_max_amount": 500.0}]),
+        ("2", "Super Investment Ltd", "investor2@example.com", [{"id": "f3", "name": "fund3", "investor_id": "2", "subscriptions": [{"id": "s4", "algo_id": "a4"}, {"id": "s5", "algo_id": "a5"}, {"id": "s6", "algo_id": "a6"}], "compounding": 1}]),
+        ("3", "XY Funds", "investor3@example.com", [{"id": "f4", "name": "fund4", "investor_id": "3", "subscriptions": [{"id": "s7", "algo_id": "a7"}], "compounding": 0, "absolute_max_amount": 10000.0}, {"id": "f5", "name": "fund5", "investor_id": "3", "subscriptions": [{"id": "s8", "algo_id": "a8"}, {"id": "s9", "algo_id": "a9"}, {"id": "s10", "algo_id": "a10"}]}])
     ]
 )
-def test_investor_funds(investor_id, email, funds):
+def test_investor_funds(investor_id, name, email, funds):
     person = Person(given_name="john", family_name="Doe", email=email, sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
 
     funds_objects = []
     for fund in funds:
         subscriptions = [Subscription(**subscription) for subscription in fund.pop('subscriptions')]
         fund_obj = Fund(subscriptions=subscriptions, **fund)
         funds_objects.append(fund_obj)
 
-    investor = Investor(id=investor_id, email=email, accountable=person, funds=funds_objects)
+    investor = Investor(id=investor_id, name=name, email=email, accountable=person, funds=funds_objects)
 
     assert investor.id == investor_id
-    assert investor.email == email
+    assert investor.name == name
+    assert investor.email == email    
     assert len(investor.funds) == len(funds_objects)
     for i in range(len(funds_objects)):
         assert investor.funds[i].id == funds_objects[i].id
         assert investor.funds[i].name == funds_objects[i].name
         assert investor.funds[i].compounding == funds_objects[i].compounding
         assert len(investor.funds[i].subscriptions) == len(funds_objects[i].subscriptions)
 
 
 def test_passphrase():
     # Create an Investor instance
     person = Person(given_name="john", family_name="Doe", email="john@doe.com", sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
-    investor = Investor(id='123', email='test@example.com', accountable=person)
+    investor = Investor(id='123', name="Johnny's Investments", email='test@example.com', accountable=person)
     investor.setPassphrase("testpass")
     # Check that passphrase can't be retrieved directly
     with pytest.raises(Exception) as e:
         print(f"INVOKING IS FORBIDDEN --> {investor.passphrase}")
     assert str(e.value) == "Cannot retrieve passphrase."
 
     # Check the passphrase
```

### Comparing `fa-models-1.0.73/tests/test_processed_trading_signal.py` & `fa-models-1.0.74/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

