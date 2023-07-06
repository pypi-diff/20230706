# Comparing `tmp/fa-models-1.0.72.tar.gz` & `tmp/fa-models-1.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.72.tar", last modified: Sun Jul  2 13:12:21 2023, max compression
+gzip compressed data, was "fa-models-1.0.73.tar", last modified: Thu Jul  6 05:03:07 2023, max compression
```

## Comparing `fa-models-1.0.72.tar` & `fa-models-1.0.73.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.624729 fa-models-1.0.72/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 13:12:21.624729 fa-models-1.0.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 13:11:51.000000 fa-models-1.0.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.620729 fa-models-1.0.72/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.620729 fa-models-1.0.72/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.624729 fa-models-1.0.72/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/signal_supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/state_of_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/state_of_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/state_of_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-02 13:12:13.000000 fa-models-1.0.72/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:12:21.624729 fa-models-1.0.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-02 13:11:51.000000 fa-models-1.0.72/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.624729 fa-models-1.0.72/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-02 13:11:51.000000 fa-models-1.0.72/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-02 13:11:51.000000 fa-models-1.0.72/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.464277 fa-models-1.0.73/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 05:03:07.460277 fa-models-1.0.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-06 05:02:32.000000 fa-models-1.0.73/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 05:03:07.000000 fa-models-1.0.73/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-06 05:02:32.000000 fa-models-1.0.73/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-06 05:02:57.000000 fa-models-1.0.73/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:03:07.464277 fa-models-1.0.73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-06 05:02:32.000000 fa-models-1.0.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:03:07.460277 fa-models-1.0.73/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-06 05:02:32.000000 fa-models-1.0.73/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 05:02:32.000000 fa-models-1.0.73/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.72/PKG-INFO` & `fa-models-1.0.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.72
+Version: 1.0.73
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.72/README.md` & `fa-models-1.0.73/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.72/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.73/fa_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.72
+Version: 1.0.73
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.72/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.73/fa_models.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 fa_models.egg-info/requires.txt
 fa_models.egg-info/top_level.txt
 famodels/__init__.py
 famodels/models/__init__.py
 famodels/models/algorithm.py
 famodels/models/direction.py
 famodels/models/investor.py
+famodels/models/investor_statement.py
 famodels/models/order.py
 famodels/models/order_type.py
 famodels/models/person.py
 famodels/models/processed_signal.py
 famodels/models/side.py
-famodels/models/signal_supplier.py
-famodels/models/state_of_investor.py
-famodels/models/state_of_signal.py
-famodels/models/state_of_trade.py
+famodels/models/signal_provider.py
 famodels/models/trade.py
 famodels/models/trading_signal.py
 famodels/models/virtual_order.py
+famodels/models/market/__init__.py
+famodels/models/market/public_trade.py
 tests/test_investor.py
 tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.72/famodels/models/algorithm.py` & `fa-models-1.0.73/famodels/models/market/public_trade.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 import os
 from redis_om import (Field, JsonModel)
 from redis_om.connections import get_redis_connection
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
-class Algorithm(JsonModel):
-    algo_id: str = Field(index=True)   
-    provider_id: str = Field(index=True) 
-    
+class PublicTrade(JsonModel):
+    market: str = Field(index=True)
+    exchange: str = Field(index = True)
+    price: float = Field(index=True)
+    quantity: float = Field(index=True)
+    side: str = Field(index=True)
+    timestamp: int = Field(index=True)
+
     class Meta:
         # global_key_prefix="fa-investor-processing"
-        model_key_prefix="algorithm"
-        database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
+        model_key_prefix="public-trade"
+        database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
```

### Comparing `fa-models-1.0.72/famodels/models/investor.py` & `fa-models-1.0.73/famodels/models/investor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 import os
 from typing import List, Optional
 from pydantic import EmailStr
 from redis_om import Field, JsonModel, EmbeddedJsonModel
 from redis_om.connections import get_redis_connection
-from famodels.models.state_of_investor import StateOfInvestor
 from famodels.models.person import Person
 from cryptography.fernet import Fernet
 from hashlib import sha256
 import bcrypt
-from base64 import urlsafe_b64encode, urlsafe_b64decode
+from base64 import urlsafe_b64encode
+
+from enum import Enum
+
+class StateOfInvestor(str, Enum):    
+    """Describing the possible states of an Investor. Keep it simple. Also, we added the str to inherit from, so that the ENUM is serializable.         """
+    REGISTERED = "registered"
+    """When an investor is merely registered, but NOT authenticated with an official document. Registered allows cold trading."""
+    QUALIFIED = "qualified"
+    """When an investor is identified and authenticated by an offical document and qualified for hot trades. This is the highest state."""
+    BANNED = "banned"
+    """The investor was deliberatly banned from the system."""
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 key = os.environ.get("ENCRYPTION_KEY").encode()
 ENCRYPTION_KEY = urlsafe_b64encode(sha256(key).digest())
 
 class Subscription(EmbeddedJsonModel):
-    subscription_id: str = Field(index=False)
+    id: str = Field(index=False)
     algo_id:str = Field(index=True)
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="subscription"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 class Fund(EmbeddedJsonModel):
-    fund_id:str = Field(index=True)
+    id:str = Field(index=True)
     name:str = Field(index=True)    
     compounding: str = Field(index=True, default="true")
     """Marks the investment as to be compounded with every trade. CAUTION: Due to redis-om model restrictions this could not be a boolean as it's value suggests. The workaround is a str with values 'true' and 'false'. Default is 'true'. Will bechanged as soon the redis-om library has enhanced."""
     subscriptions: Optional[List[Subscription]]  
-    absolute_max_amount: Optional[float]
+    number_of_positions: int = Field(index=False, default=5)
+    max_amount: Optional[float]
+    """The max amount in quote currency to invest. e.g. 10'000 (USDT)."""
     
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="fund"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
     def add_subscription(self, subscription):
@@ -51,15 +63,15 @@
         return f.encrypt(value.encode()).decode()
 
     def decrypt(self, encrypted_value: str) -> str:
         f = Fernet(self.key)
         return f.decrypt(encrypted_value.encode()).decode()
 
 class ExchangeKey(EmbeddedJsonModel):
-    exchange: str = Field(index=True)
+    exchange: str = Field(index=True,)
     key_id: str = Field(index=True)
     _key_secret: str = Field(index=False)
 
     def set_key_secret(self, value: str, encryption_service: EncryptionService):
         self._key_secret = encryption_service.encrypt(value)
 
     def get_key_secret(self, encryption_service: EncryptionService) -> str:
@@ -67,15 +79,15 @@
 
     class Meta:
         model_key_prefix = "exchange-key"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 
 class Investor(JsonModel):
-    investor_id: str = Field(index=True)
+    id: str = Field(index=True)
     email: EmailStr = Field(index=True)
     accountable: Person = Field(index=True)        
     state: StateOfInvestor = Field(index=True, default=StateOfInvestor.REGISTERED.value)
     _passphrase: Optional[str]
     #library constraint: "redis_om.model.model.RedisModelError: In this Preview release, list and tuple fields can only contain strings. Problem field: compounding"
     funds: Optional[List[Fund]]
     exchange_keys: Optional[List[ExchangeKey]]
@@ -93,11 +105,14 @@
         # DO NOT USE A STATIC SALT!
         salt = bcrypt.gensalt()
         self._passphrase = bcrypt.hashpw(encoded_pw, salt)
 
     def verify_passphrase(self, passphrase: str):
         return bcrypt.checkpw(passphrase.encode(), self._passphrase)    
     
+    def is_qualified(self):
+        return self.state == StateOfInvestor.QUALIFIED
+    
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="investor"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
```

### Comparing `fa-models-1.0.72/famodels/models/order.py` & `fa-models-1.0.73/famodels/models/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.72/famodels/models/person.py` & `fa-models-1.0.73/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.72/famodels/models/processed_signal.py` & `fa-models-1.0.73/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.72/famodels/models/trade.py` & `fa-models-1.0.73/famodels/models/trade.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 from datetime import datetime
-import os
-from famodels.models.state_of_trade import StateOfTrade
+import os, time, uuid
 from famodels.models.direction import Direction
 from typing import Optional
-import uuid
 from redis_om import Migrator
 from redis_om import (Field, JsonModel)
 from redis_om.connections import get_redis_connection
+from enum import Enum
+
+class StateOfTrade(str, Enum):    
+    """Describing the possible states of a Trade. Keep it simple. Also, we added the str to inherit from, so that the ENUM is serializable.         """
+    NEW = "new"
+    BUYING = "buying"    
+    """BUYING means that we have at least submitted an order to buy."""
+    WAITING_FOR_SELL_DECISION = "waiting_for_sell_decision"
+    """Indicates, the the buy has been completed and we are waiting for a sell order to be sent."""
+    SELLING = "selling"
+    """SELLING means that a sell-order (close position) has been sent to the CEX. """
+    CANCELED = "canceled"
+    """Cancelled is the state where a trade was canceled but cleaned up (i.e. sold what was previously bought. Or bought-back what was previously sold)."""
+    CLOSED = "closed"
+    """Closed means the trade did buy completely and sold completely."""
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"the env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
-
 class Trade(JsonModel):
     """A trade in our system is composed of a buy and a sell order. Do not mistaken it for a trade from the CEX.
         Create a new Trade record for every update and correlate them with trade_id. See attribute #trade_id"""   
-    id: Optional[int] = Field(default=None, primary_key=True)    
-    trade_id: Optional[str] = Field(default=str(uuid.uuid4()), nullable=False)
+    # id: Optional[int] = Field(default=None, primary_key=True)    
+    id: str = Field(default=str(uuid.uuid4().hex), nullable=False, primary_key=True)
     # sort_index:int = field(init=False, repr=False)
     #trade_id: Optional[str] = Field(default=uuid.uuid4(), primary_key=True)
     """The trade id is the reference that keeps the state updates correlated. It will generate a UUID by default.
         Use this for the first record you insert. Inserting updated records (new records should then have the trade_id
         provided to create the correlation.)"""
+    investor_id: str = Field(index=True)
+    fund_id: str = Field(index=True)
     pos_idx:int
-    market:str
-    status:StateOfTrade
+    market:str = Field(index=True)    
+    status:StateOfTrade = Field(index=True)
     direction:Direction
-    time_of_initiation:datetime
+    amount: float
+    time_of_initiation:datetime = Field(index=True, default=int(time.time() * 1000))
     """When we decided to start this trade."""
-    buy_order_id:str
+    buy_order_id: Optional[str] = None
     sell_order_id:Optional[str] = None
-    take_profit:Optional[int] = None
-    stop_loss:Optional[int] = None
+    take_profit:Optional[float] = None
+    stop_loss:Optional[float] = None
     """This is usually the receiving timestamp."""        
     profit_and_loss_percentage: Optional[float] = None
     profit_and_loss_amount: Optional[float] = None
 
     class Meta:
         # global_key_prefix="order-and-trade-processing"
         model_key_prefix="trade"
```

### Comparing `fa-models-1.0.72/famodels/models/trading_signal.py` & `fa-models-1.0.73/famodels/models/trading_signal.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 from typing import Optional
 from uuid import UUID
 from famodels.models.direction import Direction
 from famodels.models.side import Side
 from redis_om import Migrator
 from redis_om import (Field, JsonModel)
 from redis_om.connections import get_redis_connection
+from enum import Enum
+
+class StateOfSignal(str, Enum):    
+    """Describing the possible states of a Signal (not a Trade). """
+    SUBMITTED = "submitted"
+    ERRONEOUS = "erroneous"   
+    REJECTED = "rejected"
+    QUALIFIED = "qualified"
+    EXECUTED = "executed"
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 class TradingSignal(JsonModel):
     """A trading signal represents a suggestion to buy or sell. It is issued by a signal supplier (manually or algorithmically). It must have a correlating id to a trade."""    
     provider_id: str = Field(index=True)
```

### Comparing `fa-models-1.0.72/famodels/models/virtual_order.py` & `fa-models-1.0.73/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.72/pyproject.toml` & `fa-models-1.0.73/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.72"
+version = "1.0.73"
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
-current_version = "1.0.72"
+current_version = "1.0.73"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.72/setup.py` & `fa-models-1.0.73/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #                 #     if obj.__module__ == module_name:
 #                 #         print(name)
 
 #         build.run(self)
 
 setup(
     name='fa-models',
-    packages=find_packages(include=['famodels', 'famodels.models', 'famodels.generators', 'schemas'], exclude=['tests*']),
+    packages=find_packages(include=['famodels', 'famodels.models', 'famodels.models.market'], exclude=['tests*']),
     # packages=['famodels'],
     # package_dir={'famodels':'src'}
     #packages=find_packages(),
     #version='0.1.0',
     # description='The library describes the most common models used in trading systems.',
     # author='Brayan Svan',
     # license='MIT',
```

### Comparing `fa-models-1.0.72/tests/test_investor.py` & `fa-models-1.0.73/tests/test_investor.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system('docker stop redis-unit-test')
         os.system('docker rm redis-unit-test')
 
 
 def test_investor_model():
     # Now we can create an instance of `Investor` without connecting to a real Redis server
     person = Person(given_name="john", family_name="Doe", email="john@doe.com", sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
-    investor = Investor(investor_id='123', email='test@example.com', accountable=person)    
+    investor = Investor(id='123', email='test@example.com', accountable=person)    
 
 
 @pytest.mark.parametrize(
     "email, nationality_iso3, country_of_residence_iso3",
     [
         ("invalidemail", "GBR", "IRE"),  # invalid email
         ("john@doe.com", "GB", "IRE"),  # invalid nationality_iso3
@@ -99,44 +99,44 @@
     assert exchange_key.exchange == exchange
     assert exchange_key.key_id == key_id
     assert exchange_key.get_key_secret(encryption_service) == key_secret
 
 @pytest.mark.parametrize(
     "investor_id, email, funds",
     [
-        ("1", "investor1@example.com", [{"fund_id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"subscription_id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"fund_id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"subscription_id": "s2", "algo_id": "a2"}, {"subscription_id": "s3", "algo_id": "a3"}], "compounding": "false", "absolute_max_amount": 500.0}]),
-        ("2", "investor2@example.com", [{"fund_id": "f3", "name": "fund3", "investor_id": "2", "subscriptions": [{"subscription_id": "s4", "algo_id": "a4"}, {"subscription_id": "s5", "algo_id": "a5"}, {"subscription_id": "s6", "algo_id": "a6"}], "compounding": 1}]),
-        ("3", "investor3@example.com", [{"fund_id": "f4", "name": "fund4", "investor_id": "3", "subscriptions": [{"subscription_id": "s7", "algo_id": "a7"}], "compounding": 0, "absolute_max_amount": 10000.0}, {"fund_id": "f5", "name": "fund5", "investor_id": "3", "subscriptions": [{"subscription_id": "s8", "algo_id": "a8"}, {"subscription_id": "s9", "algo_id": "a9"}, {"subscription_id": "s10", "algo_id": "a10"}]}])
+        ("1", "investor1@example.com", [{"id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"id": "s2", "algo_id": "a2"}, {"id": "s3", "algo_id": "a3"}], "compounding": "false", "absolute_max_amount": 500.0}]),
+        ("2", "investor2@example.com", [{"id": "f3", "name": "fund3", "investor_id": "2", "subscriptions": [{"id": "s4", "algo_id": "a4"}, {"id": "s5", "algo_id": "a5"}, {"id": "s6", "algo_id": "a6"}], "compounding": 1}]),
+        ("3", "investor3@example.com", [{"id": "f4", "name": "fund4", "investor_id": "3", "subscriptions": [{"id": "s7", "algo_id": "a7"}], "compounding": 0, "absolute_max_amount": 10000.0}, {"id": "f5", "name": "fund5", "investor_id": "3", "subscriptions": [{"id": "s8", "algo_id": "a8"}, {"id": "s9", "algo_id": "a9"}, {"id": "s10", "algo_id": "a10"}]}])
     ]
 )
 def test_investor_funds(investor_id, email, funds):
     person = Person(given_name="john", family_name="Doe", email=email, sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
 
     funds_objects = []
     for fund in funds:
         subscriptions = [Subscription(**subscription) for subscription in fund.pop('subscriptions')]
         fund_obj = Fund(subscriptions=subscriptions, **fund)
         funds_objects.append(fund_obj)
 
-    investor = Investor(investor_id=investor_id, email=email, accountable=person, funds=funds_objects)
+    investor = Investor(id=investor_id, email=email, accountable=person, funds=funds_objects)
 
-    assert investor.investor_id == investor_id
+    assert investor.id == investor_id
     assert investor.email == email
     assert len(investor.funds) == len(funds_objects)
     for i in range(len(funds_objects)):
-        assert investor.funds[i].fund_id == funds_objects[i].fund_id
+        assert investor.funds[i].id == funds_objects[i].id
         assert investor.funds[i].name == funds_objects[i].name
         assert investor.funds[i].compounding == funds_objects[i].compounding
         assert len(investor.funds[i].subscriptions) == len(funds_objects[i].subscriptions)
 
 
 def test_passphrase():
     # Create an Investor instance
     person = Person(given_name="john", family_name="Doe", email="john@doe.com", sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
-    investor = Investor(investor_id='123', email='test@example.com', accountable=person)
+    investor = Investor(id='123', email='test@example.com', accountable=person)
     investor.setPassphrase("testpass")
     # Check that passphrase can't be retrieved directly
     with pytest.raises(Exception) as e:
         print(f"INVOKING IS FORBIDDEN --> {investor.passphrase}")
     assert str(e.value) == "Cannot retrieve passphrase."
 
     # Check the passphrase
```

### Comparing `fa-models-1.0.72/tests/test_processed_trading_signal.py` & `fa-models-1.0.73/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

