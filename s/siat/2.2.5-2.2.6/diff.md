# Comparing `tmp/siat-2.2.5-py3-none-any.whl.zip` & `tmp/siat-2.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1696578 bytes, number of entries: 120
+Zip file size: 1696631 bytes, number of entries: 120
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Apr-10 11:29 siat/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-Apr-10 11:29 siat/allin.py
 -rw-rw-rw-  2.0 fat      747 b- defN 23-Apr-10 11:29 siat/alpha_vantage_test.py
 -rw-rw-rw-  2.0 fat    28555 b- defN 23-Apr-10 11:29 siat/assets_liquidity.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-10 11:29 siat/assets_liquidity_test.py
 -rw-rw-rw-  2.0 fat    10110 b- defN 23-Apr-10 11:29 siat/barrons_scraping_test.py
 -rw-rw-rw-  2.0 fat    36597 b- defN 23-Apr-10 11:29 siat/beta_adjustment.py
@@ -85,15 +85,15 @@
 -rw-rw-rw-  2.0 fat   101523 b- defN 23-May-27 06:22 siat/sector_china.py
 -rw-rw-rw-  2.0 fat     5843 b- defN 23-Apr-11 14:17 siat/sector_china_test.py
 -rw-rw-rw-  2.0 fat    29185 b- defN 23-May-25 02:36 siat/security_price.py
 -rw-rw-rw-  2.0 fat    74058 b- defN 23-Jul-05 13:33 siat/security_prices.py
 -rw-rw-rw-  2.0 fat    10779 b- defN 23-Apr-10 11:29 siat/security_prices_test.py
 -rw-rw-rw-  2.0 fat     1335 b- defN 23-Apr-10 11:29 siat/setup.py
 -rw-rw-rw-  2.0 fat     1418 b- defN 23-Apr-10 11:29 siat/shenwan index history test.py
--rw-rw-rw-  2.0 fat   129369 b- defN 23-Jul-04 09:02 siat/stock.py
+-rw-rw-rw-  2.0 fat   129603 b- defN 23-Jul-06 11:34 siat/stock.py
 -rw-rw-rw-  2.0 fat    31655 b- defN 23-Apr-10 11:29 siat/stock_advice_linear.py
 -rw-rw-rw-  2.0 fat     1312 b- defN 23-Apr-10 11:29 siat/stock_base.py
 -rw-rw-rw-  2.0 fat    82785 b- defN 23-Jun-17 02:52 siat/stock_china.py
 -rw-rw-rw-  2.0 fat     1294 b- defN 23-Jun-14 07:32 siat/stock_china_test.py
 -rw-rw-rw-  2.0 fat  1266744 b- defN 23-Jun-05 00:13 siat/stock_info.pickle
 -rw-rw-rw-  2.0 fat     6122 b- defN 23-Apr-10 11:29 siat/stock_info_test.py
 -rw-rw-rw-  2.0 fat     1014 b- defN 23-Apr-10 11:29 siat/stock_list_china_test.py
@@ -111,12 +111,12 @@
 -rw-rw-rw-  2.0 fat   118133 b- defN 23-Apr-10 11:29 siat/translate-20230206.py
 -rw-rw-rw-  2.0 fat   121657 b- defN 23-Apr-10 11:29 siat/translate-20230215.py
 -rw-rw-rw-  2.0 fat   134050 b- defN 23-Jul-04 11:47 siat/translate.py
 -rw-rw-rw-  2.0 fat     3936 b- defN 23-Apr-10 11:29 siat/universal_test.py
 -rw-rw-rw-  2.0 fat    51342 b- defN 23-May-11 00:30 siat/valuation_china.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-10 11:29 siat/valuation_market_china_test.py
 -rw-rw-rw-  2.0 fat    14859 b- defN 23-Apr-10 11:29 siat/var_model_validation.py
--rw-rw-rw-  2.0 fat     1410 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     9602 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/RECORD
-120 files, 7751530 bytes uncompressed, 1681938 bytes compressed:  78.3%
+-rw-rw-rw-  2.0 fat     1429 b- defN 23-Jul-06 13:58 siat-2.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 13:58 siat-2.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-06 13:58 siat-2.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     9602 b- defN 23-Jul-06 13:58 siat-2.2.6.dist-info/RECORD
+120 files, 7751783 bytes uncompressed, 1681991 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -342,20 +342,20 @@
 
 Filename: siat/valuation_market_china_test.py
 Comment: 
 
 Filename: siat/var_model_validation.py
 Comment: 
 
-Filename: siat-2.2.5.dist-info/METADATA
+Filename: siat-2.2.6.dist-info/METADATA
 Comment: 
 
-Filename: siat-2.2.5.dist-info/WHEEL
+Filename: siat-2.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: siat-2.2.5.dist-info/top_level.txt
+Filename: siat-2.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: siat-2.2.5.dist-info/RECORD
+Filename: siat-2.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siat/stock.py

```diff
@@ -532,25 +532,25 @@
     result2=result1.drop_duplicates(subset=None,keep='first',ignore_index=False)
     result3=result2.T
 
     return result3
 
 
 if __name__ =="__main__":
-    ticker1='NVDA'
+    ticker='NVDA'
     fromdate='2023-5-1'
     todate='2023-6-16'
-    rtype="Exp Ret%"
-    rtype="Annual Ret Volatility%"
+    indicator="Exp Ret%"
+    indicator="Annual Ret Volatility%"
     
     datatag=False
     power=0
     graph=True
 
-def security_indicator(ticker,fromdate,todate,rtype="Daily Ret%",datatag=False,power=0,graph=True):
+def security_indicator(ticker,indicator,fromdate,todate,datatag=False,power=0,graph=True):
     """
     功能：单只证券的全部指标
     """
     fromdate1=date_adjust(fromdate,adjust=-365*3)
     
     pricedf=get_price(ticker,fromdate1,todate)
     if pricedf is None:
@@ -559,40 +559,40 @@
     
     erdf=all_calculate(pricedf,ticker,fromdate,todate)
     
     import pandas as pd
     fromdate_pd=pd.to_datetime(fromdate)
     erdf2=erdf[erdf.index >= fromdate_pd]
     
-    # 若rtype为Exp Ret%类指标，此处需要首行置零
+    # 若indicator为Exp Ret%类指标，此处需要首行置零
     colList=list(erdf2)
     index1=erdf2.head(1).index.values[0]
     for c in colList:
         if 'Exp Ret%' in c:
             erdf2.loc[erdf2[erdf2.index==index1].index.tolist(),c]=0
     
-    #erdf3=pd.DataFrame(erdf2[rtype])
+    #erdf3=pd.DataFrame(erdf2[indicator])
     erdf3=erdf2
 
     # 绘图
     if not graph:
         return erdf3
     
     titletxt=texttranslate("证券指标运动趋势：")+codetranslate(ticker)
     import datetime; today = datetime.date.today()
     footnote=texttranslate("数据来源：新浪/东方财富/stooq/雅虎财经，")+str(today)
-    collabel=ectranslate(rtype)
-    ylabeltxt=ectranslate(rtype)
+    collabel=ectranslate(indicator)
+    ylabeltxt=ectranslate(indicator)
     
-    if 'Ret%' in rtype:
+    if 'Ret%' in indicator:
         zeroline=True
     else:
         zeroline=False
         
-    plot_line(erdf3,rtype,collabel,ylabeltxt,titletxt,footnote,datatag=datatag, \
+    plot_line(erdf3,indicator,collabel,ylabeltxt,titletxt,footnote,datatag=datatag, \
               power=power,zeroline=zeroline)
     
     return erdf3
     
     
 def stock_ret(ticker,fromdate,todate,rtype="Daily Ret%",datatag=False,power=0,graph=True):
     """
@@ -683,14 +683,21 @@
     功能：单个证券，多个指标对比
     date_range=False：指定开始结束日期绘图
     date_freq=False：指定横轴日期间隔，例如'D'、'2D'、'W'、'M'等，横轴一般不超过25个标注，否则会重叠
     """
     # 提前开始日期
     fromdate1=date_adjust(fromdate,adjust=-365*3)
     
+    if isinstance(ticker,list):
+        if len(ticker) == 1:
+            ticker=ticker[0]
+        else:
+            print("  #Error(security_mindicators): need 1 ticker only in",ticker)
+            return None
+
     if isinstance(measures,str):
         measures=[measures]
     
     try:
         pricedf=get_price(ticker,fromdate1,todate)
     except:
         print("  #Error(security_mindicators): price info not found for",ticker)
@@ -1508,15 +1515,15 @@
     import pandas as pd
     from functools import reduce
 
     dfs=pd.DataFrame()
     for t in tickers:
         print("  Looking security info for",t,'...')
         with HiddenPrints():
-            df_tmp=security_indicator(t,start,end,rtype=measure,graph=False)
+            df_tmp=security_indicator(t,measure,start,end,graph=False)
         if df_tmp is None:
             print("  #Warning(compare_msecurity): security info not found for",t)
             continue
         if len(df_tmp)==0:
             print("  #Warning(compare_msecurity): security info not found for",t,'between',start,'and',end)
             continue
```

## Comparing `siat-2.2.5.dist-info/RECORD` & `siat-2.2.6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 siat/sector_china.py,sha256=sHd7nlYWCK0SWAZbu-BLn-3vNPe2E8OFaDFYF67Hoho,101523
 siat/sector_china_test.py,sha256=1wq7ef8Bb_L8F0h0W6FvyBrIcBTEbrTV7hljtpj49U4,5843
 siat/security_price.py,sha256=2oHskgiw41KMGfqtnA0i2YjNNV6cYgtlUK0j3YeuXWs,29185
 siat/security_prices.py,sha256=1J4SA5tZB4iFrQ91ijUA7jn0kkbAF8Jgc0J__IHq_ow,74058
 siat/security_prices_test.py,sha256=OEphoJ87NPKoNow1QA8EU_5MUYrJF-qKoWKNapVfZNI,10779
 siat/setup.py,sha256=up65rQGLmTBkhtaMLowjoQXYmIsnycnm4g1SYmeQS6o,1335
 siat/shenwan index history test.py,sha256=JCVAzOSEldHalhSFa3pqD8JI_8_djPMQOxpkuYU-Esg,1418
-siat/stock.py,sha256=WaRjLIXpjPl3VoUQ0AWvdtCCHKVP8RNm0ZPtUqOWaYo,129369
+siat/stock.py,sha256=esJe4A-O6A1RX4KMZQpDuMV1B3eah2D_dTBn6Pb3DoA,129603
 siat/stock_advice_linear.py,sha256=-twT7IGP-NEplkL1WPSACcNJjggRB2j4mlAQCkzOAuo,31655
 siat/stock_base.py,sha256=uISvbRyOGy8p9QREA96CVydgflBkn5L3OXOGKl8oanc,1312
 siat/stock_china.py,sha256=jVSuCWr6TaTx0Y0sgqN-dU9ZL72uKiI_MzvugvH9NaI,82785
 siat/stock_china_test.py,sha256=eO4HWsSvc6qezl0LndjtL24lViEyrBjH_sx2c2Y2Q2M,1294
 siat/stock_info.pickle,sha256=o4M-pcN8Sh8QiwZQAZWY1aelI4xgIGIxors7n2uHSJI,1266744
 siat/stock_info_test.py,sha256=gfG3DbhDACbtD8wnv_R6zhj0t11XaC8NX8uLD9Qv3Fo,6122
 siat/stock_list_china_test.py,sha256=gv14UwMMvkZqtb6G7DCTSuehIwVHuVwu7w60p6gyHoo,1014
@@ -110,11 +110,11 @@
 siat/translate-20230206.py,sha256=-vtI125WyaJhmPotOpDAmclt_XnYVaWU9ByLWZ6FyYE,118133
 siat/translate-20230215.py,sha256=TJgtPE3n8IjljmZ4Pefy8dmHoNdFF-1zpML6BhA9FKE,121657
 siat/translate.py,sha256=pFi_U1_LLzcq6rE9ns0Hr0fLYjzB_n2sGLapdbLlVxw,134050
 siat/universal_test.py,sha256=CDAOffW1Rvs-TcNN5giWVvHMlch1w4dp-w5SIV9jXL0,3936
 siat/valuation_china.py,sha256=gYYXeT9bBPyQ251TCsYlibWcu6JA8x-YOKqLUEeLE7U,51342
 siat/valuation_market_china_test.py,sha256=gbJ0ioauuo4koTPH6WKUkqcXiQPafnbhU5eKJ6lpdLA,1571
 siat/var_model_validation.py,sha256=zB_Skk_tmzIR15l6oAW3am4HBGVIG-eZ8gJhCdXZ8Qw,14859
-siat-2.2.5.dist-info/METADATA,sha256=qwkcyHwE6Y30y-PJGL0IyaXLyQ_lNcAI-HRncXH6MNw,1410
-siat-2.2.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-siat-2.2.5.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
-siat-2.2.5.dist-info/RECORD,,
+siat-2.2.6.dist-info/METADATA,sha256=s54STTkPj_7ck-vRQUieP0x0lLRZ2CADofJygWpdRYI,1429
+siat-2.2.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+siat-2.2.6.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
+siat-2.2.6.dist-info/RECORD,,
```

