# Comparing `tmp/KwoksTool-0.0.5.tar.gz` & `tmp/KwoksTool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksTool-0.0.5.tar", last modified: Wed Jul  5 12:57:40 2023, max compression
+gzip compressed data, was "KwoksTool-0.0.6.tar", last modified: Wed Jul  5 13:07:31 2023, max compression
```

## Comparing `KwoksTool-0.0.5.tar` & `KwoksTool-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.988531 KwoksTool-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/KwoksTool/
--rw-rw-rw-   0        0        0      807 2023-07-05 12:56:26.000000 KwoksTool-0.0.5/KwoksTool/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-05 12:57:17.000000 KwoksTool-0.0.5/KwoksTool/_version.py
--rw-rw-rw-   0        0        0    15701 2023-07-05 12:56:58.000000 KwoksTool-0.0.5/KwoksTool/function.py
--rw-rw-rw-   0        0        0      122 2023-07-05 12:54:44.000000 KwoksTool-0.0.5/KwoksTool/info.py
--rw-rw-rw-   0        0        0     1806 2023-07-05 12:54:44.000000 KwoksTool-0.0.5/KwoksTool/model.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/KwoksTool/source/
--rw-rw-rw-   0        0        0   199365 2023-07-05 10:25:10.000000 KwoksTool-0.0.5/KwoksTool/source/IpPool.py
--rw-rw-rw-   0        0        0     3750 2023-07-05 12:54:44.000000 KwoksTool-0.0.5/KwoksTool/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/KwoksTool.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 12:57:40.000000 KwoksTool-0.0.5/KwoksTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-05 12:57:40.972932 KwoksTool-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-07-05 12:53:12.000000 KwoksTool-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 12:57:40.988531 KwoksTool-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 13:07:31.045099 KwoksTool-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:07:31.029474 KwoksTool-0.0.6/KwoksTool/
+-rw-rw-rw-   0        0        0      763 2023-07-05 13:04:37.000000 KwoksTool-0.0.6/KwoksTool/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-05 13:04:24.000000 KwoksTool-0.0.6/KwoksTool/_version.py
+-rw-rw-rw-   0        0        0    14458 2023-07-05 13:06:08.000000 KwoksTool-0.0.6/KwoksTool/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-05 12:54:44.000000 KwoksTool-0.0.6/KwoksTool/info.py
+-rw-rw-rw-   0        0        0     1095 2023-07-05 13:06:29.000000 KwoksTool-0.0.6/KwoksTool/model.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:07:31.029474 KwoksTool-0.0.6/KwoksTool/source/
+-rw-rw-rw-   0        0        0   199365 2023-07-05 10:25:10.000000 KwoksTool-0.0.6/KwoksTool/source/IpPool.py
+-rw-rw-rw-   0        0        0     3737 2023-07-05 13:06:51.000000 KwoksTool-0.0.6/KwoksTool/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:07:31.029474 KwoksTool-0.0.6/KwoksTool.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-05 13:07:31.000000 KwoksTool-0.0.6/KwoksTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-05 13:07:31.000000 KwoksTool-0.0.6/KwoksTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:07:31.000000 KwoksTool-0.0.6/KwoksTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 13:07:31.000000 KwoksTool-0.0.6/KwoksTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-05 13:07:31.045099 KwoksTool-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-05 13:04:17.000000 KwoksTool-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 13:07:31.045099 KwoksTool-0.0.6/setup.cfg
```

### Comparing `KwoksTool-0.0.5/KwoksTool/__init__.py` & `KwoksTool-0.0.6/KwoksTool/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from KwoksTool.info import (welcome,how)
 from KwoksTool.spider import (Browser,PlateComponentStocks)
 from KwoksTool.function import (GetCityNumFromLiepin,
-                                GetIpPool,
                                 GetCityNumFromBossZhiPing,
                                 GetCityNameFromLiepin,
                                 YesOrNot,
                                 CheckIp,
                                 IntoZip,
                                 ZipOut,
                                 SendEmail,
```

### Comparing `KwoksTool-0.0.5/KwoksTool/function.py` & `KwoksTool-0.0.6/KwoksTool/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -291,41 +291,14 @@
         # print("title:", title)
         get_att(msg, dir)
 def ProgressBar(i, sum, printvalue):
     sys.stdout.write('\r')
     sys.stdout.write('{}%|{}{}|{}'.format(int(i / sum * 100), ((int(i / sum * 100))) * '■',
                                           (100 - int(i / sum * 100 + 1)) * '_', '当前打印：' + str(printvalue)))
     sys.stdout.flush()
-def GetPlateSon1(num):
-    if num == '':
-        res = requests.get(r'https://hq.stock.sohu.com/pl/pl-1631.html?uid=1681655630543283qgz&548285357286').text
-        res = json.loads(
-            res.split('PEAK_ODIA(')[1].split(')</script>')[0].replace('\'pllist\',', '').replace('\'', '"'))
-        info = ''
-        for son in res:
-            info = info + son[1] + ':' + son[0] + '、'
-        print('请将所需板块的编号作为参数传入进来，具体信息如下：\n', info)
-        input('')
-    else:
-        res = requests.get(r'https://q.stock.sohu.com/cn/bk_' + num + '.shtml').text
-        res = res.split('</tbody>')[0].split('<tbody>')[1]
-        res1 = res
-        name = re.compile(r'>\d{6}<').findall(res1)
-        res = re.compile(r'>[\u4e00-\u9fa5]+<').findall(res)
-        '''>[\u4e00-\u9fa5]+<'''  # 匹配名称
-        result1 = []
-        for son in res:
-            result1.append(son.replace('\'', '').replace('>', '').replace('<', ''))
-        result2 = []
-        for son1 in name:
-            result2.append(son1.replace('\'', '').replace('>', '').replace('<', ''))
-        result = {}
-        result['代码'] = result2
-        result['名称'] = result1
-        return result
 def MergeTable(data1, data2, on, data1name, data2name):
     data1 = pd.merge(data1, data2, on=on, how='outer')
     for i in range(0, len(list(data1))):
         data1 = data1.rename(
             columns={list(data1)[i]: list(data1)[i].replace('_x', data1name).replace('_y', data2name)})
     return data1
 def ChoiceColumn(date,name):
```

### Comparing `KwoksTool-0.0.5/KwoksTool/source/IpPool.py` & `KwoksTool-0.0.6/KwoksTool/source/IpPool.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.5/KwoksTool/spider.py` & `KwoksTool-0.0.6/KwoksTool/spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 import tushare as ts
 import re
 from KwoksTool.function import ProgressBar
 def Browser(url, show=False):
     options = webdriver.ChromeOptions()
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-import time from selenium import webdriver from
-selenium.webdriver.chrome.service import Service import tushare as ts import re
-from KwoksTool.function import ProgressBar def Browser(url, show=False):
-options = webdriver.ChromeOptions() options.add_experimental_option
-("excludeSwitches", ["enable-automation"]) options.add_experimental_option
-('useAutomationExtension', False) if show is False: options.add_argument('--
-headless') driver = webdriver.Chrome(options=options, service=Service
-("chromedriver.exe")) driver.execute_cdp_cmd
+from selenium import webdriver from selenium.webdriver.chrome.service import
+Service import tushare as ts import re from KwoksTool.function import
+ProgressBar def Browser(url, show=False): options = webdriver.ChromeOptions()
+options.add_experimental_option("excludeSwitches", ["enable-automation"])
+options.add_experimental_option('useAutomationExtension', False) if show is
+False: options.add_argument('--headless') driver = webdriver.Chrome
+(options=options, service=Service("chromedriver.exe")) driver.execute_cdp_cmd
 ("Page.addScriptToEvaluateOnNewDocument", { "source": """ Object.defineProperty
 (navigator, 'webdriver', { get: () => undefined }) """ }) #
 driver.maximize_window() driver.minimize_window() driver.get(url) return driver
 def PlateComponentStocks(PlateInfoName, url,code): # code:tushureçç§é¥ #
 url:æä»¶ä¿å­çè·¯å¾ # plateinfoname:è¡ç¥¨çæ¿åä»£ç  def GetPlateSon
 (stock_num): def get_stock_name(date, num): def get_re_name(date): date = '
 \D*_return_date_a_=_(re.findall(re.compile(str(get_re_name(str(num)))),_date))
```

