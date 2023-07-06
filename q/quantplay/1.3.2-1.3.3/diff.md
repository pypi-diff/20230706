# Comparing `tmp/quantplay-1.3.2.tar.gz` & `tmp/quantplay-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.3.2.tar", last modified: Thu Jul  6 16:08:21 2023, max compression
+gzip compressed data, was "quantplay-1.3.3.tar", last modified: Thu Jul  6 16:09:45 2023, max compression
```

## Comparing `quantplay-1.3.2.tar` & `quantplay-1.3.3.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.120916 quantplay-1.3.2/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-06 16:08:21.120972 quantplay-1.3.2/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.3.2/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.105084 quantplay-1.3.2/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.106038 quantplay-1.3.2/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.3.2/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.108727 quantplay-1.3.2/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.108955 quantplay-1.3.2/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.3.2/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.109318 quantplay-1.3.2/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.3.2/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.3.2/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.3.2/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.3.2/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.3.2/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.3.2/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.110903 quantplay-1.3.2/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.3.2/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.3.2/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17259 2023-07-06 16:08:04.000000 quantplay-1.3.2/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.111020 quantplay-1.3.2/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.111203 quantplay-1.3.2/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.111655 quantplay-1.3.2/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.3.2/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.112315 quantplay-1.3.2/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.3.2/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.112507 quantplay-1.3.2/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.3.2/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.3.2/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.112725 quantplay-1.3.2/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.112994 quantplay-1.3.2/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.113685 quantplay-1.3.2/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.113849 quantplay-1.3.2/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.114464 quantplay-1.3.2/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.3.2/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.114740 quantplay-1.3.2/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.114892 quantplay-1.3.2/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.115249 quantplay-1.3.2/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.115716 quantplay-1.3.2/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.3.2/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.3.2/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.3.2/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.116337 quantplay-1.3.2/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.3.2/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.3.2/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.116554 quantplay-1.3.2/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.3.2/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.116646 quantplay-1.3.2/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.3.2/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.116735 quantplay-1.3.2/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.3.2/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.116823 quantplay-1.3.2/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.3.2/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.116910 quantplay-1.3.2/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.3.2/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.117006 quantplay-1.3.2/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.3.2/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.117096 quantplay-1.3.2/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.3.2/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.117821 quantplay-1.3.2/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.3.2/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.3.2/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.3.2/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.3.2/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.118109 quantplay-1.3.2/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.3.2/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.3.2/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.119674 quantplay-1.3.2/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.3.2/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.3.2/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.3.2/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.105835 quantplay-1.3.2/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-06 16:08:21.000000 quantplay-1.3.2/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-07-06 16:08:21.000000 quantplay-1.3.2/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-07-06 16:08:21.000000 quantplay-1.3.2/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-07-06 16:08:21.000000 quantplay-1.3.2/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-07-06 16:08:21.000000 quantplay-1.3.2/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-07-06 16:08:21.121169 quantplay-1.3.2/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      875 2023-07-06 16:08:04.000000 quantplay-1.3.2/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.119928 quantplay-1.3.2/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.3.2/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.120165 quantplay-1.3.2/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.120403 quantplay-1.3.2/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:08:21.120794 quantplay-1.3.2/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.3.2/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.379791 quantplay-1.3.3/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-06 16:09:45.379876 quantplay-1.3.3/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.3.3/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.363677 quantplay-1.3.3/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.364829 quantplay-1.3.3/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.3.3/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.368275 quantplay-1.3.3/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.368500 quantplay-1.3.3/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.3.3/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.368824 quantplay-1.3.3/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.3.3/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.3.3/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.3.3/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.3.3/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.3.3/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.3.3/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.370365 quantplay-1.3.3/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.3.3/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.3.3/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17259 2023-07-06 16:08:51.000000 quantplay-1.3.3/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.370455 quantplay-1.3.3/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.370630 quantplay-1.3.3/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.371039 quantplay-1.3.3/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28260 2023-07-06 16:08:51.000000 quantplay-1.3.3/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.371466 quantplay-1.3.3/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.3.3/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.371647 quantplay-1.3.3/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.3.3/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.3.3/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.371873 quantplay-1.3.3/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.372122 quantplay-1.3.3/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.372712 quantplay-1.3.3/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.372846 quantplay-1.3.3/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.373451 quantplay-1.3.3/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.3.3/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.373677 quantplay-1.3.3/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.373809 quantplay-1.3.3/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.374138 quantplay-1.3.3/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.374624 quantplay-1.3.3/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.3.3/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.3.3/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.3.3/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.375299 quantplay-1.3.3/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.3.3/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.3.3/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.375529 quantplay-1.3.3/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.3.3/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.375630 quantplay-1.3.3/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.3.3/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.375741 quantplay-1.3.3/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.3.3/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.375844 quantplay-1.3.3/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.3.3/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.375966 quantplay-1.3.3/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.3.3/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.376069 quantplay-1.3.3/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.3.3/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.376180 quantplay-1.3.3/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.3.3/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.376906 quantplay-1.3.3/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.3.3/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.3.3/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.3.3/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.3.3/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.377190 quantplay-1.3.3/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.3.3/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.3.3/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.378573 quantplay-1.3.3/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.3.3/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.3.3/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.3.3/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.364564 quantplay-1.3.3/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-06 16:09:45.000000 quantplay-1.3.3/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-07-06 16:09:45.000000 quantplay-1.3.3/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-07-06 16:09:45.000000 quantplay-1.3.3/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      221 2023-07-06 16:09:45.000000 quantplay-1.3.3/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-07-06 16:09:45.000000 quantplay-1.3.3/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-07-06 16:09:45.380142 quantplay-1.3.3/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      875 2023-07-06 16:09:17.000000 quantplay-1.3.3/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.378816 quantplay-1.3.3/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.3.3/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.379050 quantplay-1.3.3/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.379287 quantplay-1.3.3/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-06 16:09:45.379643 quantplay-1.3.3/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.3.3/test/test_motilal.py
```

### Comparing `quantplay-1.3.2/PKG-INFO` & `quantplay-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.3.2
+Version: 1.3.3
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.3.2/quantplay/backtest/backtest_trades.py` & `quantplay-1.3.3/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/angelone.py` & `quantplay-1.3.3/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/broker_client.py` & `quantplay-1.3.3/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.3.3/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/generics/broker.py` & `quantplay-1.3.3/quantplay/broker/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/iifl.py` & `quantplay-1.3.3/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/iifl_xts.py` & `quantplay-1.3.3/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/kite_utils.py` & `quantplay-1.3.3/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/motilal.py` & `quantplay-1.3.3/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/shoonya.py` & `quantplay-1.3.3/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/symphony.py` & `quantplay-1.3.3/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/xts.py` & `quantplay-1.3.3/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.3.3/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.3.3/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.3.3/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.3.3/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/broker/zerodha.py` & `quantplay-1.3.3/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.3.3/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/brokerage/generics/broker.py` & `quantplay-1.3.3/quantplay/brokerage/generics/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,21 @@
 
             end_date = datetime.now()
             end_date = end_date.replace(second=0, microsecond=0)
 
             start_date = end_date - timedelta(days=20)
             start_date = start_date.replace(minute=0, hour=0)
 
-            response = self.get_historical_data(
-                instrument_id, start_date=start_date, end_date=end_date, interval_max_days=interval_max_days
-            )
+            try:
+                response = self.get_historical_data(
+                    instrument_id, start_date=start_date, end_date=end_date, interval_max_days=interval_max_days
+                )
+            except Exception as e:
+                Constants.logger.error(f"[HISTORICAL_DATA_FETCH_FAILED] {instrument_id}")
+                continue
             for interval, data in response.items():
                 if len(data) > 0:
                     data = self.add_today_candles(data, symbol)
                     data.loc[:, "security_type"] = security_type
                     instrument_data_by_interval[interval].append(data)
                 else:
                     Constants.logger.info(
```

### Comparing `quantplay-1.3.2/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.3.3/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/config/qplay_config.py` & `quantplay-1.3.3/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/create_sample_data.py` & `quantplay-1.3.3/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/data_modify_script.py` & `quantplay-1.3.3/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/date_fix.py` & `quantplay-1.3.3/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/exception/exceptions.py` & `quantplay-1.3.3/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/executor/strategy_executor.py` & `quantplay-1.3.3/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/indicators/Indicator.py` & `quantplay-1.3.3/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/model/exchange/instrument.py` & `quantplay-1.3.3/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/model/exchange/order.py` & `quantplay-1.3.3/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/model/exchange/tick.py` & `quantplay-1.3.3/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.3.3/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/order_execution/mean_price.py` & `quantplay-1.3.3/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/reporting/strategy_report.py` & `quantplay-1.3.3/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/reporting/visuals.py` & `quantplay-1.3.3/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/services/market.py` & `quantplay-1.3.3/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/services/tradelens.py` & `quantplay-1.3.3/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.3.3/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.3.3/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/strategy/base.py` & `quantplay-1.3.3/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/utils/config_util.py` & `quantplay-1.3.3/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/utils/constant.py` & `quantplay-1.3.3/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/utils/data_utils.py` & `quantplay-1.3.3/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/utils/exchange.py` & `quantplay-1.3.3/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/utils/number_utils.py` & `quantplay-1.3.3/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/utils/selenium_utils.py` & `quantplay-1.3.3/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay/utils/transaction_utils.py` & `quantplay-1.3.3/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/quantplay.egg-info/PKG-INFO` & `quantplay-1.3.3/quantplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.3.2
+Version: 1.3.3
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.3.2/quantplay.egg-info/SOURCES.txt` & `quantplay-1.3.3/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/setup.py` & `quantplay-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.3.2",
+    version="1.3.3",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.3.2/test/strategy/sample_strategy.py` & `quantplay-1.3.3/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.2/test/test_motilal.py` & `quantplay-1.3.3/test/test_motilal.py`

 * *Files identical despite different names*

