# Comparing `tmp/shortzy-0.0.7.tar.gz` & `tmp/shortzy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortzy-0.0.7.tar", last modified: Thu May  4 17:39:23 2023, max compression
+gzip compressed data, was "shortzy-0.0.8.tar", last modified: Thu Jul  6 16:36:58 2023, max compression
```

## Comparing `shortzy-0.0.7.tar` & `shortzy-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-04 17:39:22.980000 shortzy-0.0.7/
--rwx------   0 kevinnadar   (501) staff       (20)    34523 2023-05-04 17:39:23.010000 shortzy-0.0.7/LICENSE
--rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-04 17:39:23.140000 shortzy-0.0.7/PKG-INFO
--rwx------   0 kevinnadar   (501) staff       (20)     5442 2023-05-04 17:39:23.030000 shortzy-0.0.7/README.md
--rwx------   0 kevinnadar   (501) staff       (20)       38 2023-05-04 17:39:23.140000 shortzy-0.0.7/setup.cfg
--rwx------   0 kevinnadar   (501) staff       (20)     1146 2023-05-04 17:39:23.040000 shortzy-0.0.7/setup.py
-drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-04 17:39:22.980000 shortzy-0.0.7/shortzy/
--rwx------   0 kevinnadar   (501) staff       (20)       25 2023-05-04 17:39:23.080000 shortzy-0.0.7/shortzy/__init__.py
--rwx------   0 kevinnadar   (501) staff       (20)     5227 2023-05-04 17:39:23.100000 shortzy-0.0.7/shortzy/adlinkfly.py
--rwx------   0 kevinnadar   (501) staff       (20)     4594 2023-05-04 17:39:23.100000 shortzy-0.0.7/shortzy/main.py
--rwx------   0 kevinnadar   (501) staff       (20)     5105 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy/shareus.py
-drwx------   0 kevinnadar   (501) staff       (20)        0 2023-05-04 17:39:22.980000 shortzy-0.0.7/shortzy.egg-info/
--rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/PKG-INFO
--rwx------   0 kevinnadar   (501) staff       (20)      256 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/SOURCES.txt
--rwx------   0 kevinnadar   (501) staff       (20)        1 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/dependency_links.txt
--rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-04 17:39:23.110000 shortzy-0.0.7/shortzy.egg-info/requires.txt
--rwx------   0 kevinnadar   (501) staff       (20)        8 2023-05-04 17:39:23.140000 shortzy-0.0.7/shortzy.egg-info/top_level.txt
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-07-06 16:36:58.430000 shortzy-0.0.8/
+-rwx------   0 kevinnadar   (501) staff       (20)    34523 2023-07-06 16:36:58.440000 shortzy-0.0.8/LICENSE
+-rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-07-06 16:36:58.470000 shortzy-0.0.8/PKG-INFO
+-rwx------   0 kevinnadar   (501) staff       (20)     5442 2023-07-06 16:36:58.440000 shortzy-0.0.8/README.md
+-rwx------   0 kevinnadar   (501) staff       (20)       38 2023-07-06 16:36:58.470000 shortzy-0.0.8/setup.cfg
+-rwx------   0 kevinnadar   (501) staff       (20)     1145 2023-07-06 16:36:58.450000 shortzy-0.0.8/setup.py
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-07-06 16:36:58.430000 shortzy-0.0.8/shortzy/
+-rwx------   0 kevinnadar   (501) staff       (20)       25 2023-07-06 16:36:58.450000 shortzy-0.0.8/shortzy/__init__.py
+-rwx------   0 kevinnadar   (501) staff       (20)     5227 2023-07-06 16:36:58.450000 shortzy-0.0.8/shortzy/adlinkfly.py
+-rwx------   0 kevinnadar   (501) staff       (20)     4848 2023-07-06 16:36:58.450000 shortzy-0.0.8/shortzy/main.py
+-rwx------   0 kevinnadar   (501) staff       (20)     5084 2023-07-06 16:36:58.460000 shortzy-0.0.8/shortzy/shareus.py
+-rwx------   0 kevinnadar   (501) staff       (20)     5042 2023-07-06 16:36:58.460000 shortzy-0.0.8/shortzy/shareusio.py
+drwx------   0 kevinnadar   (501) staff       (20)        0 2023-07-06 16:36:58.440000 shortzy-0.0.8/shortzy.egg-info/
+-rwx------   0 kevinnadar   (501) staff       (20)     6152 2023-07-06 16:36:58.460000 shortzy-0.0.8/shortzy.egg-info/PKG-INFO
+-rwx------   0 kevinnadar   (501) staff       (20)      277 2023-07-06 16:36:58.460000 shortzy-0.0.8/shortzy.egg-info/SOURCES.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        1 2023-07-06 16:36:58.470000 shortzy-0.0.8/shortzy.egg-info/dependency_links.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        8 2023-07-06 16:36:58.470000 shortzy-0.0.8/shortzy.egg-info/requires.txt
+-rwx------   0 kevinnadar   (501) staff       (20)        8 2023-07-06 16:36:58.470000 shortzy-0.0.8/shortzy.egg-info/top_level.txt
```

### Comparing `shortzy-0.0.7/LICENSE` & `shortzy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.7/PKG-INFO` & `shortzy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortzy
-Version: 0.0.7
+Version: 0.0.8
 Summary: An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy
 Author: Kevin Nadar
 Author-email: jesikamaraj@gmail.com
 License: MIT
 Keywords: python,droplink,gplink,url-shortener,earn money,shareus,adlinkfly
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shortzy Version: 0.0.7 Summary: An Unofficial
+Metadata-Version: 2.1 Name: shortzy Version: 0.0.8 Summary: An Unofficial
 Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy Author: Kevin Nadar Author-
 email: jesikamaraj@gmail.com License: MIT Keywords: python,droplink,gplink,url-
 shortener,earn money,shareus,adlinkfly Platform: UNKNOWN Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
```

### Comparing `shortzy-0.0.7/README.md` & `shortzy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.7/setup.py` & `shortzy-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION ='0.0.8'
 DESCRIPTION = 'An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper'
 
 # Setting up
 setup(
     name="shortzy",
     version=VERSION,
     author="Kevin Nadar",
```

### Comparing `shortzy-0.0.7/shortzy/adlinkfly.py` & `shortzy-0.0.8/shortzy/adlinkfly.py`

 * *Files identical despite different names*

### Comparing `shortzy-0.0.7/shortzy/main.py` & `shortzy-0.0.8/shortzy/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .shareus import Shareus
 from .adlinkfly import Adlinkfly
+from .shareusio import ShareusIO
 
 
 class Shortzy:
     """
     A Unofficial Shortener API Wrapper for Adlinkfly Site and Alternative Sites
 
     :param api_key: Your API key
@@ -17,19 +18,26 @@
         self.base_site = base_site
 
         if not self.api_key:
             raise Exception("API key not provided")
 
         if self.base_site == "shareus.in":
             self.shortener = Shareus(api_key, base_site=base_site)
+        elif self.base_site == "shareus.io":
+            self.shortener = ShareusIO(api_key, base_site=base_site)
         else:
             self.shortener = Adlinkfly(api_key, base_site=base_site)
 
     async def convert(
-        self, link: str, silently_fail: bool = False, quick_link: bool = False, alias: str = "", ** kwargs
+        self,
+        link: str,
+        silently_fail: bool = False,
+        quick_link: bool = False,
+        alias: str = "",
+        **kwargs
     ) -> str:
         """
         It converts a link to a short link.
 
         :param link: The link you want to shorten
         :type link: str
 
@@ -89,15 +97,21 @@
 
         :return: The shortened link is being returned.
         """
         return await self.shortener.convert_from_text(
             text, silently_fail, quick_link, **kwargs
         )
 
-    async def bulk_convert(self, links: list, silently_fail: bool = False, quick_link: bool = False, **kwargs) -> list:
+    async def bulk_convert(
+        self,
+        links: list,
+        silently_fail: bool = False,
+        quick_link: bool = False,
+        **kwargs
+    ) -> list:
         """
         It converts a list of links to a list of short links.
 
         :param links: The list of links you want to shorten
         :type links: list
 
         :param silently_fail: If this is set to True, then instead of raising an exception, it will return
@@ -105,15 +119,17 @@
         :type silently_fail: bool (optional)
 
         :param quick_link: If you want to get a quick link, set this to True, defaults to False
         :type quick_link: bool (optional)
 
         :return: The list of shortened links is being returned.
         """
-        return await self.shortener.bulk_convert(links, silently_fail=silently_fail, quick_link=quick_link, **kwargs)
+        return await self.shortener.bulk_convert(
+            links, silently_fail=silently_fail, quick_link=quick_link, **kwargs
+        )
 
     async def is_short_link(self, link: str) -> bool:
         """
         It checks if the link is a short link.
 
         :param link: The link you want to check
         :type link: str
```

### Comparing `shortzy-0.0.7/shortzy/shareus.py` & `shortzy-0.0.8/shortzy/shareus.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
         if not self.api_key:
             raise Exception("API key not provided")
 
     async def __fetch(self, session: aiohttp.ClientSession, params: dict) -> dict:
         async with session.get(
             self.base_url, params=params, raise_for_status=True, ssl=False
         ) as response:
-            result = await response.json(content_type="text/html")
-            return result
+            return await response.json(content_type="text/html")
 
     async def convert(
         self, link: str, silently_fail: bool = False, quick_link: bool = False, **kwargs
     ) -> str:
         is_short_link = await self.is_short_link(link)
 
         if is_short_link:
@@ -47,15 +46,15 @@
 
                 if silently_fail:
                     return link
 
                 raise Exception(data["message"])
 
         except Exception as e:
-            raise Exception(e)
+            raise Exception(e) from e
 
     async def get_quick_link(self, url: str, **kwargs) -> str:
         quick_link = "https://api.{base_site}/directLink?token={api_key}&link={url}"
         return quick_link.format(
             base_site=self.base_site,
             api_key=self.api_key,
             url=url,
```

### Comparing `shortzy-0.0.7/shortzy.egg-info/PKG-INFO` & `shortzy-0.0.8/shortzy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortzy
-Version: 0.0.7
+Version: 0.0.8
 Summary: An Unofficial Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy
 Author: Kevin Nadar
 Author-email: jesikamaraj@gmail.com
 License: MIT
 Keywords: python,droplink,gplink,url-shortener,earn money,shareus,adlinkfly
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shortzy Version: 0.0.7 Summary: An Unofficial
+Metadata-Version: 2.1 Name: shortzy Version: 0.0.8 Summary: An Unofficial
 Asynchronous Python version of Adlinkfly and Alternative Website API wrapper
 Home-page: https://github.com/kevinnadar22/shortzy Author: Kevin Nadar Author-
 email: jesikamaraj@gmail.com License: MIT Keywords: python,droplink,gplink,url-
 shortener,earn money,shareus,adlinkfly Platform: UNKNOWN Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
```

