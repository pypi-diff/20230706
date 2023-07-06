# Comparing `tmp/regcensus-1.0.0.tar.gz` & `tmp/regcensus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regcensus-1.0.0.tar", last modified: Mon Jul  3 13:39:36 2023, max compression
+gzip compressed data, was "regcensus-1.0.1.tar", last modified: Thu Jul  6 17:03:21 2023, max compression
```

## Comparing `regcensus-1.0.0.tar` & `regcensus-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.749439 regcensus-1.0.0/
--rw-r--r--   0 jnelson    (501) staff       (20)       78 2023-04-26 13:32:43.000000 regcensus-1.0.0/.gitignore
--rw-r--r--   0 jnelson    (501) staff       (20)     1098 2023-04-26 13:32:43.000000 regcensus-1.0.0/LICENSE
--rw-r--r--   0 jnelson    (501) staff       (20)      401 2023-07-03 13:39:36.749516 regcensus-1.0.0/PKG-INFO
--rw-r--r--   0 jnelson    (501) staff       (20)    14364 2023-04-26 13:32:43.000000 regcensus-1.0.0/README.md
-drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.747865 regcensus-1.0.0/regcensus/
--rw-r--r--   0 jnelson    (501) staff       (20)      793 2023-06-30 17:20:28.000000 regcensus-1.0.0/regcensus/__init__.py
--rw-r--r--   0 jnelson    (501) staff       (20)    25044 2023-06-30 18:07:03.000000 regcensus-1.0.0/regcensus/api.py
--rw-r--r--   0 jnelson    (501) staff       (20)     1047 2023-06-30 17:20:28.000000 regcensus-1.0.0/regcensus/cache.py
-drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.748910 regcensus-1.0.0/regcensus.egg-info/
--rw-r--r--   0 jnelson    (501) staff       (20)      401 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/PKG-INFO
--rw-r--r--   0 jnelson    (501) staff       (20)      304 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/SOURCES.txt
--rw-r--r--   0 jnelson    (501) staff       (20)        1 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/dependency_links.txt
--rw-r--r--   0 jnelson    (501) staff       (20)       16 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/requires.txt
--rw-r--r--   0 jnelson    (501) staff       (20)       10 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/top_level.txt
--rw-r--r--   0 jnelson    (501) staff       (20)       15 2023-04-26 13:32:44.000000 regcensus-1.0.0/requirements.txt
--rw-r--r--   0 jnelson    (501) staff       (20)      130 2023-07-03 13:39:36.749830 regcensus-1.0.0/setup.cfg
--rw-r--r--   0 jnelson    (501) staff       (20)      583 2023-06-30 17:20:34.000000 regcensus-1.0.0/setup.py
-drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.749104 regcensus-1.0.0/tests/
--rw-r--r--   0 jnelson    (501) staff       (20)    10074 2023-06-30 17:20:28.000000 regcensus-1.0.0/tests/test_api.py
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-06 17:03:21.825513 regcensus-1.0.1/
+-rw-r--r--   0 jnelson    (501) staff       (20)       78 2023-04-26 13:32:43.000000 regcensus-1.0.1/.gitignore
+-rw-r--r--   0 jnelson    (501) staff       (20)     1098 2023-04-26 13:32:43.000000 regcensus-1.0.1/LICENSE
+-rw-r--r--   0 jnelson    (501) staff       (20)      401 2023-07-06 17:03:21.825562 regcensus-1.0.1/PKG-INFO
+-rw-r--r--   0 jnelson    (501) staff       (20)    14233 2023-07-06 16:59:43.000000 regcensus-1.0.1/README.md
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-06 17:03:21.824461 regcensus-1.0.1/regcensus/
+-rw-r--r--   0 jnelson    (501) staff       (20)      793 2023-06-30 17:20:28.000000 regcensus-1.0.1/regcensus/__init__.py
+-rw-r--r--   0 jnelson    (501) staff       (20)    25370 2023-07-06 16:59:43.000000 regcensus-1.0.1/regcensus/api.py
+-rw-r--r--   0 jnelson    (501) staff       (20)     1047 2023-06-30 17:20:28.000000 regcensus-1.0.1/regcensus/cache.py
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-06 17:03:21.825136 regcensus-1.0.1/regcensus.egg-info/
+-rw-r--r--   0 jnelson    (501) staff       (20)      401 2023-07-06 17:03:21.000000 regcensus-1.0.1/regcensus.egg-info/PKG-INFO
+-rw-r--r--   0 jnelson    (501) staff       (20)      304 2023-07-06 17:03:21.000000 regcensus-1.0.1/regcensus.egg-info/SOURCES.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)        1 2023-07-06 17:03:21.000000 regcensus-1.0.1/regcensus.egg-info/dependency_links.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)       16 2023-07-06 17:03:21.000000 regcensus-1.0.1/regcensus.egg-info/requires.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)       10 2023-07-06 17:03:21.000000 regcensus-1.0.1/regcensus.egg-info/top_level.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)       15 2023-04-26 13:32:44.000000 regcensus-1.0.1/requirements.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)      130 2023-07-06 17:03:21.825932 regcensus-1.0.1/setup.cfg
+-rw-r--r--   0 jnelson    (501) staff       (20)      583 2023-07-05 21:53:30.000000 regcensus-1.0.1/setup.py
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-06 17:03:21.825262 regcensus-1.0.1/tests/
+-rw-r--r--   0 jnelson    (501) staff       (20)    10074 2023-06-30 17:20:28.000000 regcensus-1.0.1/tests/test_api.py
```

### Comparing `regcensus-1.0.0/LICENSE` & `regcensus-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `regcensus-1.0.0/README.md` & `regcensus-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
 In requesting data through the API, you must specify the document type and the indicate a preference for *summary* or *document-level*. By default, RegCensus API returns summarized data for the date of interest. This means that if you do not specify the *summary* preference, you will receive the summarized data for a date. The __get_series__ helper function (described below) returns the dates available for each series.
 
 RegCensus API defines a number of dates depending on the series. For example, the total restrictions series of Federal regulations uses two main dates: daily and annual. The daily data produces the number of regulatory restrictions issued on a particular date by the US Federal government. The same data are available on an annual basis.
 
 There are five helper functions to retrieve information about these key components of regdata. These functions provider the following information: document types, jurisdictions, series, agencies, and dates with data. The list functions begin with __list__.
 
-Each document type comprises one or more *series*. The __list_series__ function returns the list of all series when no series id is provided. 
+Each document type comprises one or more *series*. The __list_series__ function returns the list of all series.
 
 ```
-rc.list_series(jurisdictionID = 38)
+rc.list_series()
 ```
 
 Listing the jurisdictions is another great place to start. If you are looking for data for a specifc jurisdiction(s), this function
 will return the jurisdiction_id for all jurisdiction, which is key for retrieving data on any individual jurisdiction.
 
 The __get_series__ function returns a list of all series and the years with data available for each jurisdiction. 
 
@@ -55,22 +55,30 @@
 
 Use the __get_jurisdiction__ function to return a data frame with all the jurisdictions. When you supply the jurisdiction ID parameter, the function returns the details of just that jurisdiction. Use the output from the __get_jurisdiction__ function to merge with data from the __get_values__ function.
 
 ```
 rc.get_jurisdictions()
 ```
 
+### DataFinder
+
+Use the __get_datafinder__ function to return a data frame for a specific jurisdiction. It returns the following attributes in the data - `['jurisdiction', 'documentType', 'year', 'series', 'document_endpoints', 'summary_endpoints', 'label_endpoints']`
+
+```
+get_datafinder(jurisdiction = 38)
+```
+
 ### Agencies
 
 The __get_agencies__ function returns a data frame of agencies with data in RegData. Either the `jurisdictionID` or `keyword` arguments must be supplied. If `jurisdictionID` is passed, the data frame will include information for all agencies in that jurisdiction. If `keyword` is supplied, the data frame will include information for all agencies whose name contains the keyword.
 
 The following code snippet will return data for all agencies in the Federal United States:
 
 ```
-rc.get_agencies(jurisdiction = 38)
+rc.get_agencies(jurisdictionID = 38)
 ```
 
 Likewise, this code snippet will return data for all agencies (in any jurisdiction) containing the word "education" (not case sensitive):
 
 ```
 rc.get_agencies(keyword = 'education')
 ```
@@ -80,156 +88,146 @@
 ### Industries
 
 The __get_industries__ function returns a data frame of industries with data in the API. The available standards include the North American Industry Classification System (NAICS), the Bereau of Economic Analysis system (BEA), and the Standard Occupational Classification System (SOC). By default, the function only returns a data frame with 3-digit NAICS industries. The `codeLevel` and `standard` arguments can be used to select from other classifications.
 
 The following line will get you industry information for all 4-digit NAICS industries:
 
 ```
-rc.get_industries(codeLevel = 4)
+rc.get_industries(labellevel = 4)
 ```
 
-This line will get you information for the BEA industries:
+This line will get you information for the NAICS industries (this function is temporarily disabled as of 1.0.0):
 
 ```
-rc.get_industries(standard = 'BEA')
+rc.get_industries(labelsource = 'NAICS')
 ```
 
-Like the __get_agencies__ function, the `keyword` argument may also be used. The following code snippet will return information for all 6-digit NAICS industries with the word "fishing" in the name:
-
-```
-rc.get_industries(keyword = 'fishing', codeLevel = 6)
-```
-
-### Documents
-
-The __get_documents__ function returns a data frame with metadata for document-level data. The fucntion takes two parameters, jurisdictionID (required) and documentType (default value of 1, which is "all regulations").
-
-The following line will get metadata for documents associated with U.S. Federal healthcare regulations.
+Like the __get_agencies__ function, the `keyword` argument may also be used. The following code snippet will return information for all 6-digit NAICS industries with the word "fishing" in the name (this function is temporarily disabled as of 1.0.0):
 
 ```
-rc.get_documents(jurisdictionID = 38, documentType = 3)
+rc.get_industries(keyword = 'fishing', labellevel = 6)
 ```
 
 ## Values
 
 The __get_values__ function is the primary function for obtaining RegData from the RegCensus API. The function takes the following parameters:
 
 * jurisdiction (required) - value or list of jurisdiction IDs
 * series (required) - value or list of series IDs
-* date (required) - value or list of years
+* year (required) - value or list of years
 * agency (optional) - value or list of agencies
 * industry (optional) - value of list of agencies
 * dateIsRange (optional) - specify if the list of years provided for the parameter years is a range. Default is True.
 * filtered (optional) - specify if poorly-performing industry results should be excluded. Default is True.
 * summary (optional) - specify if summary results should be returned, instead of document-level results. Default is True.
 * country (optional) - specify if all values for a country's jurisdiction ID should be returned. Default is False.
 * industryLevel (optional): level of NAICS industries to include. Default is 3.
 * version (optional): Version ID for datasets with multiple versions, if no ID is given, API returns most recent version
 * download (optional): if not False, a path location for a downloaded csv of the results.
 * verbose (optional) - value specifying how much debugging information should be printed for each function call. Higher number specifies more information, default is 0.
 
 In the example below, we are interested in the total number of restrictions and total number of words for the US (get_jurisdictions(38)) for the dates 2010 to 2019.
 
 ```
-rc.get_values(series = [1,2], jurisdiction = 38, date = [2010, 2019])
+rc.get_values(series = [1,2], jurisdiction = 38, year = [2010, 2019])
 ```
 
 ### Get all Values for a Country
 
-The `country` argument can be used to get all values for one or multiple series for a specific national jurisdiction. The following line will get you a summary of the national and state-level restriction counts for the United States from 2016 to 2019:
+The `country` argument can be used to get all values for one or multiple series for a specific national jurisdiction. The following line will get you a summary of the national and state-level restriction counts for the United States from 2016 to 2019 (this function is temporarily disabled as of 1.0.0):
 
 ```
-rc.get_values(series = 1, jurisdiction = 38, date = [2016, 2019], country=True)
+rc.get_values(series = 1, jurisdiction = 38, year = [2016, 2019], country=True)
 ```
 
 ### Values by Subgroup
 
 You can obtain data for any of the three subgroups for each series - agencies, industries, and occupations (when they become available).
 
 #### Values by Agencies
 
 To obtain the restrictions for a specific agency (or agencies), the series id supplied must be in the list of available series by agency. To recap, the list of available series for an agency is available via the __list_series__ function, and the list of agencies with data is available via __get_agencies__ function.
 
 ```
 # Identify all agencies
-rc.list_agencies(jurisdictionID)
+rc.list_agencies(jurisdictionID = 38)
 
-# Call the get_values() for this agency and series 91
-rc.get_values(series = 91, jurisdiction = 38, date = [1990, 2018], agency = [81, 84])
+# Call the get_values() for two agencies and series 13
+rc.get_values(series = 13, jurisdiction = 38, year = [2000, 2018], agency = [15918, 15921])
 ```
 
 #### Values by Agency and Industry
 
 Some agency series may also have data by industry. For example, under the Total Restrictions topic, RegData includes the industry-relevant restrictions, which estimates the number of restrictions that apply to a given industry. These are available in both the main series - Total Restrictions, and the sub-group Restrictions by Agency. 
 
 Valid values for industries include the industry codes specified in the classification system obtained by calling the __get_industries(jurisdiction)__ function.
 
-In the example below, the series 92 (Restrictions by Agency and Industry), we can request data for the two industries 111 and 33 by the following code snippet.
+In the example below, for the below series, we can request data for the two industries 111 and 33 by the following code snippet.
 
 ```
-rc.get_values(series = 92, jurisdiction = 38, time = [1990, 2000], industry = [111, 33], agency = 66)
+rc.get_values(series = [1,28,33,36], jurisdiction = 38, year = [1990, 2000], label = 111, agency = 0)
 ```
 
 ### Document-Level Values
 
 For most use-cases, our summary-level data will be enough. However, document-level data is also available, though most of these queries take much longer to return results. Multi-year and industry results for jurisdiction 38 will especially take a long time. If you want the full dataset for United States Federal, consider using our bulk downloads, available at the [QuantGov website][2].
 
 We can request the same data from above, but at the document level, using the following code snippet.
 
 ```
-rc.get_values(series = [1,2], jurisdiction = 38, date = ['2010-01-01', '2019-01-01'], summary=False)
+rc.get_values(series = [1,2], jurisdiction = 38, year = 2020, summary=False)
 ```
 
 Alternatively, we can use the  __get_document_values__ function as in the following code snippet.
 
 ```
-rc.get_document_values(series = [1,2], jurisdiction = 38, date = ['2010-01-01', '2019-01-01'])
+rc.get_document_values(series = [1,2], jurisdiction = 38, year = 2019)
 ```
 
-Note that for document-level queries, a full date (not just the year) is often required. See the __get_series__ function for specifics by jurisdiction.
+See the __get_series__ function for specifics by jurisdiction.
 
 ### Version
 
 _This currently applies to the RegData U.S. Annual project only._
 
 As of version 0.2.4, a version parameter can be passed to the __get_values__ function to obtained data from past versions of data (currently only for the RegData U.S. Annual project). Available versions and their associated versionIDs can be obtained by using the __get_version__ function. If no version parameter is given, the most recent version will be returned. The following code snippet will return restrictions data for the 3.2 version of RegData U.S. Annual for the years 2010 to 2019.
 
 ```
-rc.get_values(series = 1, jurisdiction = 38, date = [2010, 2019], version = 1)
+rc.get_values(series = 1, jurisdiction = 38, year = [2010, 2019], version = 1)
 ```
 
 ### Merging with Metadata
 
 To minimize the network bandwidth requirements to use RegCensusAPI, the data returned by __get_values__ function contain very minimal metadata. Once you pull the values by __get_values__, you can use the Pandas library to include the metadata.
 
 Suppose we want to attach the agency names and other agency characteristics to the data from the last code snippet. First be sure to pull the list of agencies into a separate data frame. Then merge with the values data frame. The key for matching the data will be the *agency_id* column.
 
 We can merge the agency data with the values data as in the code snippet below.
 
 ```
 agencies = rc.get_agencies(jurisdictionID = 38)
 agency_by_industry = rc.get_values(
-    series = 92,
+    series = [1,28,33,36],
     jurisdiction = 38,
-    time = [1990, 2000],
-    industry = [111, 33],
-    agency = [66, 111])
+    year = [1990, 2000],
+    label = 111,
+    agency = 0)
 agency_restrictions_ind = agency_by_industry.merge(
-    agencies, by='agency_id')
+    agencies, on='agency_id')
 ```
 
 ## Downloading Data
 
 There are two different ways to download data retrieved from RegCensusAPI:
 
 1. Use the pandas `df.to_csv(outpath)` function, which allows the user to download a csv of the data, with the given outpath. See the pandas [documentation][3] for more features.
 
 2. As of version 0.2.0, the __get_values__ function includes a `download` argument, which allows the user to simply download a csv of the data in the same line as the API call. See below for an example of this call.
 
 ```
-rc.get_values(series = [1,2], jurisdiction = 38, date = [2010, 2019], download='regdata2010to2019.csv')
+rc.get_values(series = [1,28,33,36], jurisdiction = 38, year = [2010, 2019], download='regdata2010to2019.csv')
 ```
 
 [1]:https://api.quantgov.org/swagger-ui.html
 [2]:https://www.quantgov.org/download-interactively
 [3]:https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html
 [4]:https://mercatus.wistia.com/medias/1hxnkfjnxa
```

### Comparing `regcensus-1.0.0/regcensus/__init__.py` & `regcensus-1.0.1/regcensus/__init__.py`

 * *Files identical despite different names*

### Comparing `regcensus-1.0.0/regcensus/api.py` & `regcensus-1.0.1/regcensus/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from regcensus.cache import Memoized
 
 pp = pprint.PrettyPrinter()
 
 date_format = re.compile(r'\d{4}(?:-\d{2}-\d{2})?')
 
-URL = 'https://64gzqlrrd2.execute-api.us-east-1.amazonaws.com/dev'
+URL = 'https://api.quantgov.org'
 
 
 def get_values(series, jurisdiction, year, documentType=1, summary=True,
                dateIsRange=True, country=False, agency=None, cluster=None,
                label=None, industry=None, filtered=True,
                labellevel=3, industryLevel=None,
                labelsource='NAICS', version=None,
@@ -153,14 +153,20 @@
                                     onlyID=True)[str(label)]
         url_call += f'&label={label}'
     # Specify level of industry (NAICS only)
     if labellevel:
         url_call += f'&labelLevel={labellevel}'
 
     # If multiple years are given, parses the list into a string
+    if not summary and type(year) == list:
+        print(
+            'WARNING: document-level data is only returnable for a single '
+            'year at a time. Returning the first year requested.'
+        )
+        year = year[0]
     if type(year) == list:
         # If dateIsRange, parses the list to include all years
         if dateIsRange and len(year) == 2:
             year = range(int(year[0]), int(year[1]) + 1)
         url_call += f'&year={",".join(str(i) for i in year)}'
     # Checks to see if date is in correct format
     elif date_format.match(str(year)):
@@ -227,15 +233,15 @@
         page = 1
         while len(output) == 5000:
             if verbose:
                 print(f'Output truncated, found page {page}')
             page += 1
             output = json_normalize(json.loads(requests.get(
                 url_call + f'&page={page}').json()))
-            full_output = full_output.append(output)
+            full_output = pd.concat([full_output, output])
         output = full_output
 
     # If download path is given, write csv instead of returning dataframe
     if download:
         if type(download) == str:
             clean_columns(output).to_csv(download, index=False)
         else:
@@ -247,14 +253,17 @@
 
 def get_document_values(*args, **kwargs):
     """
     Get values for a specific jurisdition and series at the document level
 
     Simply returns get_values() with summary=False
     """
+    if type(kwargs["year"]) == list:
+        print_error({"message" : "Only single year can be passed."})
+        return
     return get_values(*args, **kwargs, summary=False)
 
 
 def get_reading_time(*args, **kwargs):
     """
     Convert word counts to total reading time
     """
```

### Comparing `regcensus-1.0.0/regcensus/cache.py` & `regcensus-1.0.1/regcensus/cache.py`

 * *Files identical despite different names*

### Comparing `regcensus-1.0.0/setup.py` & `regcensus-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 import setuptools
 
 
 setup(
     name='regcensus',
-    version='1.0.0',
+    version='1.0.1',
     description='Python package for accessing data from the QuantGov API',
     url='https://github.com/QuantGov/regcensus-api-python',
     author='QuantGov',
     author_email='quantgov.info@gmail.com',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `regcensus-1.0.0/tests/test_api.py` & `regcensus-1.0.1/tests/test_api.py`

 * *Files identical despite different names*

