# Comparing `tmp/brfunds-0.2.0.tar.gz` & `tmp/brfunds-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brfunds-0.2.0.tar", last modified: Mon Jul 25 00:26:48 2022, max compression
+gzip compressed data, was "brfunds-0.2.1.tar", last modified: Wed Jul  5 23:30:07 2023, max compression
```

## Comparing `brfunds-0.2.0.tar` & `brfunds-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-25 00:26:48.694576 brfunds-0.2.0/
--rw-rw-rw-   0        0        0     1076 2021-06-06 22:40:21.000000 brfunds-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3132 2022-07-25 00:26:48.692582 brfunds-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2343 2022-07-25 00:11:31.000000 brfunds-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-07-25 00:26:48.674630 brfunds-0.2.0/brfunds/
--rw-rw-rw-   0        0        0      127 2022-07-24 23:53:50.000000 brfunds-0.2.0/brfunds/__init__.py
--rw-rw-rw-   0        0        0     4468 2022-07-24 17:19:43.000000 brfunds-0.2.0/brfunds/api.py
--rw-rw-rw-   0        0        0    10910 2022-07-25 00:17:56.000000 brfunds-0.2.0/brfunds/brfunds.py
-drwxrwxrwx   0        0        0        0 2022-07-25 00:26:48.690589 brfunds-0.2.0/brfunds.egg-info/
--rw-rw-rw-   0        0        0     3132 2022-07-25 00:26:47.000000 brfunds-0.2.0/brfunds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2022-07-25 00:26:48.000000 brfunds-0.2.0/brfunds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-25 00:26:47.000000 brfunds-0.2.0/brfunds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-07-25 00:26:48.000000 brfunds-0.2.0/brfunds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-25 00:26:48.000000 brfunds-0.2.0/brfunds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-06-06 22:21:28.000000 brfunds-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-25 00:26:48.694576 brfunds-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1081 2022-07-24 23:43:31.000000 brfunds-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 23:30:07.362736 brfunds-0.2.1/
+-rw-rw-rw-   0        0        0     1076 2021-06-06 22:40:21.000000 brfunds-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4666 2023-07-05 23:30:07.360448 brfunds-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3877 2023-07-05 23:13:52.000000 brfunds-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 23:30:07.344096 brfunds-0.2.1/brfunds/
+-rw-rw-rw-   0        0        0      127 2023-07-05 21:07:13.000000 brfunds-0.2.1/brfunds/__init__.py
+-rw-rw-rw-   0        0        0     6093 2023-07-05 21:11:54.000000 brfunds-0.2.1/brfunds/api.py
+-rw-rw-rw-   0        0        0    10574 2023-07-05 22:48:37.000000 brfunds-0.2.1/brfunds/brfunds.py
+drwxrwxrwx   0        0        0        0 2023-07-05 23:30:07.357928 brfunds-0.2.1/brfunds.egg-info/
+-rw-rw-rw-   0        0        0     4666 2023-07-05 23:30:07.000000 brfunds-0.2.1/brfunds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-05 23:30:07.000000 brfunds-0.2.1/brfunds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 23:30:07.000000 brfunds-0.2.1/brfunds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-05 23:30:07.000000 brfunds-0.2.1/brfunds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 23:30:07.000000 brfunds-0.2.1/brfunds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-06-06 22:21:28.000000 brfunds-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 23:30:07.363762 brfunds-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-05 22:49:53.000000 brfunds-0.2.1/setup.py
```

### Comparing `brfunds-0.2.0/LICENSE` & `brfunds-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brfunds-0.2.0/README.md` & `brfunds-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -40,8 +40,35 @@
 |2016-02-07	| -0.009009      |
 |2016-02-08	| -0.007612      |
 | ...       |  ...           |
 |2021-06-02	| 0.910064       |
 |2021-06-04	| 0.914201       |
 |2021-06-07	| 0.917008       |
 |2021-06-08	| 0.911554       |
-|2021-06-09	| 0.911601       |
+|2021-06-09	| 0.911601       |
+
+```python
+#It can also be used to multiple funds and benchmarks
+getFundsEarnings('00.000.000/0000-00','00.000.000/0000-00', benchmarks = ['cdi','ibovespa'], start = '31/01/16', end = '09/06/21')
+```
+
+|   Date    | Example Fund 1 | Example Fund 2 | CDI     | IBOV       |
+|-----------|----------------|----------------|---------|------------|
+|2016-01-31 | 0.000000       |  0.00000       | 0.00000 |  0.00000   |
+|2016-02-01 | -0.000715      |  0.001136      | 0.000525| -0.048653  |
+|2016-02-06	| -0.009902      | -0.005026      | 0.001049| -0.024186  |
+|2016-02-07	| -0.009009      | -0.006855      | 0.001575|  0.006204  |
+|2016-02-08	| -0.007612      | -0.009379      | 0.002100|  0.000544  |
+| ...       |  ...           |  ...           | ...     |  ...       |
+|2021-06-02	| 0.910064       | 1.324291       | 0.450420|  2.194512  |
+|2021-06-04	| 0.914201       | 1.323814       | 0.450612|  2.207436  |
+|2021-06-07	| 0.917008       | 1.323690       | 0.450805|  2.22347   |
+|2021-06-08	| 0.911554       | 1.327529       | 0.450997|  2.199088  |
+|2021-06-09	| 0.911601       | 1.329402       | 0.451190|  2.202039  |
+
+```python
+#The package also includes functions for drawdown, 30d Volatility, Number of Shareholders and Net Worth. 
+getFundsDrawdown('00.000.000/0000-00','00.000.000/0000-00', start = '08/01/20')
+getFundsVolatility('00.000.000/0000-00', start = '13/10/20')
+getFundsShareholders('00.000.000/0000-00','00.000.000/0000-00')
+getFundsNetWorth('00.000.000/0000-00', end = '31/12/18')
+```
```

### Comparing `brfunds-0.2.0/brfunds/brfunds.py` & `brfunds-0.2.1/brfunds/brfunds.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,14 @@
             - Accept Values: datetime.date or string with format 'dd/mm/yy'
     """
     return _baseGetData(cnpjs, scrapType='drawdown', period=period, start=start, end=end,
                         multiplier=1/100)
 
 
 def __nameTreatment(name: str, search: bool = False) -> str:
-    name = name.lower()
     replace_map = {
         'a': 'ãáâ',
         'e': 'éê',
         'i': 'í',
         'o': 'õóô',
         'u': 'ú',
         'c': 'ç',
@@ -245,21 +244,10 @@
                      '4y': reference - signal * 31556926*4000,
                      '5y': reference - signal * 31556926*5000}
     return periodOptions[period]
 
 
 def searchFund(name: str, max_size: int = 20) -> pd.DataFrame:
     """Return a list with funds with similar names, can control the size of the list with the max_size parameter, default 20"""
-    name = __nameTreatment(name, search=True)
-    fundData = api.search(name, max_size)
-    fundList = __getFundNames(fundData)
-    return fundList
-
-
-def __getFundNames(data: List) -> pd.DataFrame:
-    fundList = []
-    cnpjList = []
-    for fund in data:
-        fundList.append(fund[NAME])
-        cnpjList.append(fund[CNPJ])
-    data = pd.DataFrame({'Name': fundList, 'CNPJ': cnpjList})
-    return data
+    fundData : pd.DataFrame = api.search(name)
+    fundData = fundData.head(max_size)
+    return fundData
```

### Comparing `brfunds-0.2.0/setup.py` & `brfunds-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="brfunds",
-    version="0.2.0",
+    version="0.2.1",
     author="Phactos",
     description="Package to scrap data from brazilian funds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phactos/brfunds",
     project_urls={
         "Bug Tracker": "https://github.com/Phactos/brfunds/issues",
```

