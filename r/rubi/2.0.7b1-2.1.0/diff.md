# Comparing `tmp/rubi-2.0.7b1.tar.gz` & `tmp/rubi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.7b1.tar", max compression
+gzip compressed data, was "rubi-2.1.0.tar", max compression
```

## Comparing `rubi-2.0.7b1.tar` & `rubi-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.7b1/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.7b1/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.7b1/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.7b1/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.7b1/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.7b1/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-04 04:06:44.820395 rubi-2.0.7b1/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.7b1/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.7b1/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      745 2023-07-04 04:06:44.820830 rubi-2.0.7b1/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.7b1/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.7b1/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      648 2023-07-04 04:07:12.026104 rubi-2.0.7b1/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.7b1/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.7b1/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-04 04:06:44.821665 rubi-2.0.7b1/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0      900 2023-07-04 04:09:57.055232 rubi-2.0.7b1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-04 04:06:44.824417 rubi-2.0.7b1/rubi/__init__.py
--rw-r--r--   0        0        0    27431 2023-07-04 04:06:47.229455 rubi-2.0.7b1/rubi/client.py
--rw-r--r--   0        0        0      163 2023-06-30 02:50:06.554484 rubi-2.0.7b1/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.7b1/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11860 2023-07-04 04:06:47.229669 rubi-2.0.7b1/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-04 04:06:47.229802 rubi-2.0.7b1/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15968 2023-06-30 02:50:06.555210 rubi-2.0.7b1/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2708 2023-07-04 04:06:47.229945 rubi-2.0.7b1/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18474 2023-07-04 04:06:47.230142 rubi-2.0.7b1/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24668 2023-07-04 04:06:47.230369 rubi-2.0.7b1/rubi/contracts/market.py
--rw-r--r--   0        0        0    14847 2023-06-30 02:50:06.556060 rubi-2.0.7b1/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-04 04:06:44.826720 rubi-2.0.7b1/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-04 04:06:44.827064 rubi-2.0.7b1/rubi/data/__init__.py
--rw-r--r--   0        0        0    19848 2023-07-04 04:06:44.827426 rubi-2.0.7b1/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.7b1/rubi/network/__init__.py
--rw-r--r--   0        0        0     8052 2023-07-04 04:06:44.827822 rubi-2.0.7b1/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-30 02:50:06.556396 rubi-2.0.7b1/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15554 2023-07-04 04:06:47.230559 rubi-2.0.7b1/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0     6305 2023-07-04 04:06:47.230678 rubi-2.0.7b1/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2776 2023-06-30 02:50:06.556913 rubi-2.0.7b1/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 rubi-2.0.7b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 01:41:13.434500 rubi-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-06 01:41:13.434500 rubi-2.1.0/README.md
+-rw-r--r--   0        0        0     6735 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      745 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      648 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-06 01:41:13.438500 rubi-2.1.0/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1729 2023-07-06 01:41:53.450427 rubi-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-06 01:41:13.438500 rubi-2.1.0/rubi/__init__.py
+-rw-r--r--   0        0        0    28087 2023-07-06 01:41:13.438500 rubi-2.1.0/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-06 01:41:13.438500 rubi-2.1.0/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11860 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15968 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2708 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18474 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24668 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14847 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/data/__init__.py
+-rw-r--r--   0        0        0     9355 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8181 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/network/network.py
+-rw-r--r--   0        0        0       93 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15638 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    10670 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6410 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2776 2023-07-06 01:41:13.442500 rubi-2.1.0/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 rubi-2.1.0/PKG-INFO
```

### Comparing `rubi-2.0.7b1/LICENSE` & `rubi-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/README.md` & `rubi-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/ERC20.json` & `rubi-2.1.0/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/README.md` & `rubi-2.1.0/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/abitrum_goerli/abis/market.json` & `rubi-2.1.0/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/abitrum_goerli/abis/router.json` & `rubi-2.1.0/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/abitrum_goerli/network.yaml` & `rubi-2.1.0/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/optimism/abis/market.json` & `rubi-2.1.0/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/optimism/abis/router.json` & `rubi-2.1.0/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/optimism/network.yaml` & `rubi-2.1.0/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/optimism_goerli/abis/market.json` & `rubi-2.1.0/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/optimism_goerli/abis/router.json` & `rubi-2.1.0/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/optimism_goerli/network.yaml` & `rubi-2.1.0/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/polygon_mumbai/abis/market.json` & `rubi-2.1.0/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/polygon_mumbai/abis/router.json` & `rubi-2.1.0/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/network_config/polygon_mumbai/network.yaml` & `rubi-2.1.0/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/client.py` & `rubi-2.1.0/rubi/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging as log
 from _decimal import Decimal
 from multiprocessing import Queue
 from threading import Thread
 from time import sleep
 from typing import Union, List, Optional, Dict, Type, Any, Callable
 
+import pandas as pd
 from eth_typing import ChecksumAddress
 from web3.types import EventData, Nonce
 
 from rubi.contracts import (
     RubiconMarket,
     RubiconRouter,
     ERC20,
@@ -66,19 +67,20 @@
 
         self.wallet = self.network.w3.to_checksum_address(wallet) if wallet else wallet  # type: ChecksumAddress |  None
         self.key = key  # type: str |  None
 
         self.market = RubiconMarket.from_network(network=self.network, wallet=self.wallet, key=self.key)
         self.router = RubiconRouter.from_network(network=self.network, wallet=self.wallet, key=self.key)
 
+        self.tokens = self.get_network_tokens()
         self._pairs: Dict[str, Pair] = {}
 
         self.message_queue = message_queue  # type: Queue | None
 
-        self.market_data = MarketData.from_network(network=self.network)
+        self.market_data = MarketData.from_network_with_tokens(network=self.network, network_tokens=self.tokens)
 
     @classmethod
     def from_http_node_url(
         cls,
         http_node_url: str,
         custom_token_addresses_file: Optional[str] = None,
         message_queue: Optional[Queue] = None,
@@ -619,23 +621,40 @@
         open: Optional[bool] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
         first: Optional[int] = 1000,
         order_by: Optional[str] = 'timestamp',
         order_direction: Optional[str] = 'desc',
         formatted: Optional[bool] = True
-    ):
+    ) -> pd.DataFrame:
         
         df = self.market_data.get_offers(maker, from_address, pair_name, book_side, pay_gem, buy_gem, open, start_time, end_time, first, order_by, order_direction, formatted)
         return df
 
     ######################################################################
     # helper methods
     ######################################################################
 
+    def get_network_tokens(
+            self, 
+    ) -> Dict[ChecksumAddress, ERC20]: 
+        """Returns a Dict of addresses to ERC20 objects for all tokens on the network."""
+
+        network_tokens = {}
+
+        for address in self.network.token_addresses: 
+
+            try: 
+                network_tokens[address] = ERC20.from_network(name=address, network=self.network)
+
+            except Exception as e:
+                raise Exception(f"Token address: {address} invalid from network: {e}")
+
+        return network_tokens
+
     # TODO: revisit as the safer thing is to set approval to 0 and then set approval to new_allowance
     #  or use increaseAllowance and decreaseAllowance but the current abi does not support these methods
     #  See: https://github.com/ethereum/EIPs/issues/20#issuecomment-263524729
     @staticmethod
     def _update_asset_allowance(
         asset: ERC20,
         spender: ChecksumAddress,
```

### Comparing `rubi-2.0.7b1/rubi/contracts/aid.py` & `rubi-2.1.0/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/contracts/base_contract.py` & `rubi-2.1.0/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/contracts/contract_types/events.py` & `rubi-2.1.0/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.1.0/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/contracts/erc20.py` & `rubi-2.1.0/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/contracts/market.py` & `rubi-2.1.0/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/contracts/router.py` & `rubi-2.1.0/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/rubi/network/network.py` & `rubi-2.1.0/rubi/network/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 from enum import Enum
 from typing import Optional
 
 import yaml
 from eth_typing import ChecksumAddress
-from web3 import Web3
 from subgrounds import Subgrounds
+from web3 import Web3
 
 
 class NetworkId(Enum):
     # MAINNET
     OPTIMISM = 10
 
     # TESTNET
@@ -24,15 +24,15 @@
     provides and easy way to configure a client or contracts.
     """
 
     def __init__(
         self,
         path: str,
         w3: Web3,
-        subgrounds: Subgrounds, 
+        subgrounds: Subgrounds,
         # The below all come from network_config/{network_name}/network.yaml
         name: str,
         chain_id: int,
         currency: str,
         rpc_url: str,
         explorer_url: str,
         market_data_url: str,
@@ -71,15 +71,16 @@
         self.chain_id = chain_id
         self.w3 = w3
         self.subgrounds = subgrounds
 
         self.currency = currency
         self.rpc_url = rpc_url
         self.explorer_url = explorer_url
-        # TODO: currently we are utilizing just a single url, we should switch to a dictionary as the number of subgraphs we support grows
+        # TODO: currently we are utilizing just a single url, we should switch to a dictionary as the number of
+        #  subgraphs we support grows
         self.market_data_url = market_data_url
         self.rubicon = RubiconContracts(path=path, w3=self.w3, **rubicon)
 
         checksummed_token_addresses: dict[str, ChecksumAddress] = {}
         for k, v in token_addresses.items():
             checksummed_token_addresses[k] = self.w3.to_checksum_address(v)
 
@@ -124,15 +125,21 @@
         network_name = NetworkId(w3.eth.chain_id).name.lower()
 
         try:
             path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/{network_name}"
 
             with open(f"{path}/network.yaml") as f:
                 network_data = yaml.safe_load(f)
-                return cls(path=path, w3=w3, subgrounds=subgrounds,custom_token_addresses_file=custom_token_addresses_file, **network_data)
+                return cls(
+                    path=path,
+                    w3=w3,
+                    subgrounds=subgrounds,
+                    custom_token_addresses_file=custom_token_addresses_file,
+                    **network_data
+                )
         except FileNotFoundError:
             raise Exception(f"no network config found for {network_name}, there should be a corresponding folder in "
                             f"the network_config directory")
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.0.7b1/rubi/rubicon_types/order.py` & `rubi-2.1.0/rubi/rubicon_types/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
             pair_name=pair_name,
             order_type=OrderType.LIMIT,
             order_side=OrderSide.NEUTRAL,
         )
 
         self.order_id = order_id
 
+# TODO: add a new class for a limit order object that is returned from the subgraph
 
 class Transaction:
     """
     Class representing a transaction to be executed on chain
 
     :param orders: The list of orders to include in the transaction.
     :type orders: List[BaseNewOrder]
```

### Comparing `rubi-2.0.7b1/rubi/rubicon_types/orderbook.py` & `rubi-2.1.0/rubi/rubicon_types/orderbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,7 +195,9 @@
         """
 
         return self.best_ask() - self.best_bid()
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
+
+# TODO: add a DetailedORderBook class that contains the full order book composed of LimitOrder instances
```

### Comparing `rubi-2.0.7b1/rubi/rubicon_types/pair.py` & `rubi-2.1.0/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.7b1/PKG-INFO` & `rubi-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.7b1
+Version: 2.1.0
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,14 +12,15 @@
 Requires-Dist: attributedict (==0.3.0)
 Requires-Dist: eth-abi (==4.0.0)
 Requires-Dist: eth-tester (==0.9.0b1)
 Requires-Dist: eth-utils (==2.1.0)
 Requires-Dist: hexbytes (==0.3.0)
 Requires-Dist: py-evm (==0.7.0a2)
 Requires-Dist: pytest (==7.3.1)
+Requires-Dist: python-semantic-release (==7.34.3)
 Requires-Dist: pyyaml (==6.0.0)
 Requires-Dist: sphinx (==7.0.1) ; extra == "docs"
 Requires-Dist: subgrounds[dash] (==1.6.0)
 Requires-Dist: web3 (==6.5.0)
 Description-Content-Type: text/markdown
 
 # rubi
```

