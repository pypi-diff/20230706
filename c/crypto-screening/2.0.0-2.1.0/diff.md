# Comparing `tmp/crypto-screening-2.0.0.tar.gz` & `tmp/crypto-screening-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.0.0.tar", last modified: Wed Jul  5 16:38:00 2023, max compression
+gzip compressed data, was "crypto-screening-2.1.0.tar", last modified: Thu Jul  6 12:51:55 2023, max compression
```

## Comparing `crypto-screening-2.0.0.tar` & `crypto-screening-2.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.771188 crypto-screening-2.0.0/
--rw-rw-rw-   0        0        0       98 2023-07-05 16:37:58.000000 crypto-screening-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-05 16:38:00.771188 crypto-screening-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.664308 crypto-screening-2.0.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.701373 crypto-screening-2.0.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.0.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.0.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    32354 2023-07-05 16:37:05.000000 crypto-screening-2.0.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11846 2023-07-04 23:21:46.000000 crypto-screening-2.0.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18998 2023-07-04 23:21:46.000000 crypto-screening-2.0.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.0.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.0.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-2.0.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.706374 crypto-screening-2.0.0/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.730043 crypto-screening-2.0.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.0.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.770218 crypto-screening-2.0.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.0.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.0.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.0.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-2.0.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.0.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-05 16:38:00.678851 crypto-screening-2.0.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-05 16:38:00.000000 crypto-screening-2.0.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-05 16:37:58.000000 crypto-screening-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-2.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-2.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 16:38:00.771188 crypto-screening-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-05 16:37:53.000000 crypto-screening-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:51:55.528597 crypto-screening-2.1.0/
+-rw-rw-rw-   0        0        0       98 2023-07-06 12:51:53.000000 crypto-screening-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-06 12:51:55.527596 crypto-screening-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:51:55.501597 crypto-screening-2.1.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:51:55.519597 crypto-screening-2.1.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.1.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.1.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    32257 2023-07-06 12:48:49.000000 crypto-screening-2.1.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.1.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.1.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.1.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.1.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.1.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:51:55.520597 crypto-screening-2.1.0/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:51:55.522597 crypto-screening-2.1.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.1.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.1.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.1.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.1.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:51:55.526597 crypto-screening-2.1.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.1.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.1.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.1.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.1.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.1.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.1.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.1.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.1.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.1.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.1.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:51:55.516597 crypto-screening-2.1.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-06 12:51:55.000000 crypto-screening-2.1.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-07-06 12:51:55.000000 crypto-screening-2.1.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:51:55.000000 crypto-screening-2.1.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-06 12:51:55.000000 crypto-screening-2.1.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-06 12:51:55.000000 crypto-screening-2.1.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-06 12:51:53.000000 crypto-screening-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 12:51:55.528597 crypto-screening-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-06 12:51:37.000000 crypto-screening-2.1.0/setup.py
```

### Comparing `crypto-screening-2.0.0/PKG-INFO` & `crypto-screening-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.0.0
+Version: 2.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.0.0/README.md` & `crypto-screening-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/build.py` & `crypto-screening-2.1.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/collect/assets.py` & `crypto-screening-2.1.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/collect/exchanges.py` & `crypto-screening-2.1.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/collect/market.py` & `crypto-screening-2.1.0/crypto_screening/collect/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # market.py
 
-from dataclasses import dataclass
 from abc import ABCMeta
 from typing import (
     Iterable, Dict, Optional, Union,
     Any, ClassVar, List
 )
 
+from attrs import define
+
 from represent import represent, Modifiers
 
 import numpy as np
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.dataset import BIDS, ASKS
 from crypto_screening.symbols import symbol_to_parts
@@ -256,15 +257,15 @@
         exchange=exchange, symbol=symbol,
         prices=prices, provider=provider
     )
 
     return float(prices[exchange][symbol])
 # end symbols_market_price
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class AssetsMarketBase(metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
@@ -359,15 +360,15 @@
                 exchange=exchange, symbol=symbol,
                 separator=separator
             )
         )
     # end in_prices
 # end AssetsMarketBase
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class AssetsMarketState(AssetsMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
@@ -483,15 +484,15 @@
     # end for
 
     return AssetsMarketState(
         screeners=screeners, bids=bids, asks=asks
     )
 # end assets_market_state
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class SymbolsMarketBase(metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
@@ -568,15 +569,15 @@
 
         return (
             self.in_bids_prices(exchange=exchange, symbol=symbol) and
             self.in_asks_prices(exchange=exchange, symbol=symbol)
         )
     # end in_prices
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class SymbolsMarketState(SymbolsMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
@@ -710,15 +711,15 @@
         exchange=exchange, symbol=symbol,
         prices=prices, provider=provider
     )
 
     return [float(value) for value in prices[exchange][symbol]]
 # end symbols_market_price_sequence
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class AssetsMarketStates(AssetsMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
@@ -873,15 +874,15 @@
     # end for
 
     return AssetsMarketStates(
         screeners=screeners, bids=bids, asks=asks
     )
 # end assets_market_state
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class SymbolsMarketStates(SymbolsMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
     bids and asks prices of specific assets, gathered from the network.
```

### Comparing `crypto-screening-2.0.0/crypto_screening/collect/screeners.py` & `crypto-screening-2.1.0/crypto_screening/collect/screeners.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # screeners.py
 
-from dataclasses import dataclass
 from typing import (
     Optional, Dict, Iterable,
     Set, Union, Tuple, List
 )
 
+from attrs import define
+
 from crypto_screening.symbols import symbol_to_pair
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature,
     exchanges_symbols
 )
 from crypto_screening.market.screeners.base import (
     BaseScreener, BaseMultiScreener
@@ -104,15 +105,15 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_screener_pairs
 
-@dataclass(repr=False, slots=True, unsafe_hash=True)
+@define(repr=False, unsafe_hash=True)
 class MarketScreenerSignature(MarketSymbolSignature):
     """A class to represent the data for the execution of a trade."""
 
     screener: Optional[BaseScreener] = None
 # end MarketScreenerSignature
 
 def matching_screener_signatures(
```

### Comparing `crypto-screening-2.0.0/crypto_screening/collect/symbols.py` & `crypto-screening-2.1.0/crypto_screening/collect/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # symbols.py
 
-from dataclasses import dataclass
 from typing import (
     Optional, Dict, Iterable,
     Set, Union, Tuple
 )
 
-from represent import represent
+from attrs import define
 
+from represent import represent
 
 from crypto_screening.process import (
     find_string_value, upper_string_values,
     mutual_string_values
 )
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import (
@@ -553,15 +553,15 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_symbol_pairs
 
-@dataclass(repr=False, slots=True, unsafe_hash=True)
+@define(repr=False, unsafe_hash=True)
 @represent
 class MarketSymbolSignature:
     """A class to represent the data for the execution of a trade."""
 
     asset: str
     currency: str
     exchange: str
```

### Comparing `crypto-screening-2.0.0/crypto_screening/dataset.py` & `crypto-screening-2.1.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/interval.py` & `crypto-screening-2.1.0/crypto_screening/interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # interval.py
 
 from typing import Tuple, Union, Iterable
-from dataclasses import dataclass
 import datetime as dt
 
+from attrs import define
+
 from represent import represent, Modifiers
 
 
 __all__ = [
     "interval_to_duration",
     "interval_to_time",
     "interval_to_total_time",
@@ -34,15 +35,15 @@
     HOURS: dt.timedelta(hours=1),
     DAYS: dt.timedelta(days=1),
     WEEKS: dt.timedelta(days=7),
     MONTHS: dt.timedelta(days=30),
     YEARS: dt.timedelta(days=365)
 }
 
-@dataclass(init=False, repr=False)
+@define(slots=False, init=False, repr=False)
 @represent
 class Interval:
     """
     A class to represent a trading pair.
 
     This object represents a pair of assets that can be traded.
```

### Comparing `crypto-screening-2.0.0/crypto_screening/market/foundation/data.py` & `crypto-screening-2.1.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.1.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/foundation/state.py` & `crypto-screening-2.1.0/crypto_screening/market/foundation/state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # state.py
 
 import datetime as dt
-from dataclasses import dataclass
 from typing import (
     Optional, Union, Iterable, ClassVar, TypeVar, Generic
 )
 
+from attrs import define
+
 from represent import represent, Modifiers
 
 from crypto_screening.market.foundation.protocols import (
     BaseScreenerProtocol, BaseMultiScreenerProtocol, DataCollectorProtocol
 )
 
 __all__ = [
     "WaitingState"
 ]
 
 
 _BS = TypeVar("_BS")
 
-@dataclass(repr=False, slots=True)
+@define(repr=False)
 @represent
 class WaitingState(Generic[_BS]):
     """A class to represent the waiting state of screener objects."""
 
     screeners: Iterable[
         Union[
             _BS,
```

### Comparing `crypto-screening-2.0.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.1.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/screeners/base.py` & `crypto-screening-2.1.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/screeners/container.py` & `crypto-screening-2.1.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.1.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.1.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.1.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/market/waiting.py` & `crypto-screening-2.1.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/process.py` & `crypto-screening-2.1.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening/symbols.py` & `crypto-screening-2.1.0/crypto_screening/symbols.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # symbols.py
 
-from dataclasses import dataclass
 from typing import (
     Optional, Tuple, Dict, Any, List, Iterable, Union
 )
 
+from attrs import define
+
 from represent import represent, Modifiers
 
 __all__ = [
     "Pair",
     "symbol_to_pair",
     "symbol_to_parts",
     "pair_to_symbol",
@@ -28,15 +29,15 @@
 
 class Separator:
     """A class to contain the separator value."""
 
     value = "/"
 # end Separator
 
-@dataclass(init=False, repr=False)
+@define(slots=False, init=False, repr=False)
 @represent
 class Pair:
     """
     A class to represent a trading pair.
 
     This object represents a pair of assets that can be traded.
```

### Comparing `crypto-screening-2.0.0/crypto_screening/validate.py` & `crypto-screening-2.1.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.1.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.0.0
+Version: 2.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.0.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.1.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.0.0/pyproject.toml` & `crypto-screening-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.0.0'
+version = '2.1.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.0.0/setup.py` & `crypto-screening-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.0.0',
+        version='2.1.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

