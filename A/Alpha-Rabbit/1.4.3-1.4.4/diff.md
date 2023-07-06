# Comparing `tmp/Alpha_Rabbit-1.4.3.tar.gz` & `tmp/Alpha_Rabbit-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.4.3.tar", last modified: Mon Jul  3 02:14:49 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.4.4.tar", last modified: Thu Jul  6 05:54:21 2023, max compression
```

## Comparing `Alpha_Rabbit-1.4.3.tar` & `Alpha_Rabbit-1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 02:14:49.067777 Alpha_Rabbit-1.4.3/
-drwxrwxrwx   0        0        0        0 2023-07-03 02:14:49.061931 Alpha_Rabbit-1.4.3/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    42315 2023-07-03 02:14:23.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-07-03 02:14:49.067777 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-07-03 02:14:49.068778 Alpha_Rabbit-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/README.md
--rw-rw-rw-   0        0        0       85 2023-07-03 02:14:49.068778 Alpha_Rabbit-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-07-03 02:14:32.000000 Alpha_Rabbit-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 05:54:21.449684 Alpha_Rabbit-1.4.4/
+drwxrwxrwx   0        0        0        0 2023-07-06 05:54:21.443700 Alpha_Rabbit-1.4.4/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    42315 2023-07-06 05:48:25.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13937 2023-07-06 05:48:27.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-07-06 05:54:21.448686 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 05:54:21.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-07-06 05:54:21.449684 Alpha_Rabbit-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.4/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-06 05:54:21.450686 Alpha_Rabbit-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-07-06 05:54:01.000000 Alpha_Rabbit-1.4.4/setup.py
```

### Comparing `Alpha_Rabbit-1.4.3/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.4.4/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         # 收益率与换手率变动的相关性因子
         timerange = sorted(list(pricebyday.index.get_level_values('date').drop_duplicates()))[-21:]
         uploadfactordict['corr_ret_turnd_1M'] = corr_ret_turnd(timerange,pricebyday,'1M')
     ######################################## 日内数据计算因子 ####################################
 
     # #单笔成交金额相关因子
     sing_trade_amt = pd.DataFrame(minbar['total_turnover']/minbar['num_trades'],columns= ['single_trade_amt'])
-    sing_trade_amt = sing_trade_amt[sing_trade_amt['single_trade_amt']>=0]
+    sing_trade_amt = sing_trade_amt[sing_trade_amt['single_trade_amt']>0]
     sing_trade_amt['trading_date'] = todaydate
     sta_del_extrm = sing_trade_amt.groupby(level = 0).apply(lambda x: x.sort_values('single_trade_amt').iloc[:-10]).droplevel(0)# 剔除极大值
     sta_50pct = sing_trade_amt.groupby(level = 0).\
         apply(lambda x: x[x['single_trade_amt']<x['single_trade_amt'].quantile(0.5)]).droplevel(0)# 后百分之五十
 
 
     if 'mts' in factors_to_cal or factors_to_cal == 'all':
```

### Comparing `Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.4.4/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.3/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.4.4/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.4.4/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha-Rabbit
-Version: 1.4.3
+Version: 1.4.4
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.3/LICENSE.txt` & `Alpha_Rabbit-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.3/PKG-INFO` & `Alpha_Rabbit-1.4.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha_Rabbit
-Version: 1.4.3
+Version: 1.4.4
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.3/setup.py` & `Alpha_Rabbit-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.4.3",
+    version="1.4.4",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```

