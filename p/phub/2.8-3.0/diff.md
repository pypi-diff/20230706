# Comparing `tmp/phub-2.8.tar.gz` & `tmp/phub-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.8.tar", last modified: Sat Jun 24 10:07:04 2023, max compression
+gzip compressed data, was "phub-3.0.tar", last modified: Thu Jul  6 18:54:54 2023, max compression
```

## Comparing `phub-2.8.tar` & `phub-3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.881997 phub-2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-24 10:06:51.000000 phub-2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-24 10:07:04.881997 phub-2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-24 10:06:51.000000 phub-2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-24 10:06:51.000000 phub-2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-24 10:07:04.881997 phub-2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-24 10:06:51.000000 phub-2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.877997 phub-2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.877997 phub-2.8/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-24 10:06:51.000000 phub-2.8/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-24 10:06:51.000000 phub-2.8/src/phub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-06-24 10:06:51.000000 phub-2.8/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-24 10:06:51.000000 phub-2.8/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-24 10:06:51.000000 phub-2.8/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-24 10:06:51.000000 phub-2.8/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-24 10:06:51.000000 phub-2.8/src/phub/phub_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-24 10:06:51.000000 phub-2.8/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.881997 phub-2.8/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:54:54.893506 phub-3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 18:54:42.000000 phub-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 18:54:54.893506 phub-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-06 18:54:42.000000 phub-3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-06 18:54:42.000000 phub-3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-06 18:54:54.893506 phub-3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 18:54:42.000000 phub-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:54:54.889506 phub-3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:54:54.893506 phub-3.0/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-06 18:54:42.000000 phub-3.0/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-06 18:54:42.000000 phub-3.0/src/phub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-07-06 18:54:42.000000 phub-3.0/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-06 18:54:42.000000 phub-3.0/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-06 18:54:42.000000 phub-3.0/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-06 18:54:42.000000 phub-3.0/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-06 18:54:42.000000 phub-3.0/src/phub/phub_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-07-06 18:54:42.000000 phub-3.0/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:54:54.893506 phub-3.0/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 18:54:54.000000 phub-3.0/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 18:54:54.000000 phub-3.0/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:54:54.000000 phub-3.0/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 18:54:54.000000 phub-3.0/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 18:54:54.000000 phub-3.0/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.8/LICENSE` & `phub-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.8/PKG-INFO` & `phub-3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.8
+Version: 3.0
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
@@ -19,38 +19,42 @@
 License-File: LICENSE
 
 ![PHUB](https://github.com/Egsagon/PHUB/blob/master/assets/banner.png)
 
 # PHUB - An API for PornHub.
 PHUB is an API wrapper for PornHub. It is able to fetch, search and download videos and supports account connections, achieved with efficient web scrapping using requests and regexes.
 
-> :warning: **Early development: bugs may occur** (also i'm a terrible programer)
+> :warning: **Early development + not maintained a lot** don't hesitate to submit issues and PRs
 
 ## Installation
 - Install using pip:
 ```sh
 pip install --upgrade phub
 ```
 
 - Or using this repository to get latest features:
 ```sh
 pip install --upgrade git+https://github.com/Egsagon/PHUB.git
 ```
 
 ## CLI usage
-You can use phub like so form the terminal to start a small downloading script:
-(Assuming `py` represents your python executable, on linux use `python3`)
+You can use phub like so from the terminal as as CLI script:
 ```sh
-py -m phub --help
+python3 -m phub
 ```
 
 Example for downloading a video knowing its url, in the best available quality:
 ```sh
-py -m phub --url https://... -q 'best'
-````
+py -m phub download --url https://www.pornhub.com/view_video.php?viewkey=xxx -q 'best'
+```
+
+You can also use the provided UI if you have `tkinter` installed:
+```sh
+py -m phub ui
+```
 
 ## Package usage
 Example video download usage:
 ```python
 import phub
 
 client = phub.Client()
@@ -61,15 +65,15 @@
 ```
 
 Example searching for videos:
 ```python
 record = client.search('enter query here')
 
 # Display all videos (careful if there is a lot of results)
-for video in record:
+for video in record.range(0, 10):
   print(video.title)
 ```
 
 ## Documentation
 See the [wiki](https://github.com/Egsagon/PHUB/wiki).
 
 ## Why?
```

### Comparing `phub-2.8/README.md` & `phub-3.0/src/phub.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,60 @@
+Metadata-Version: 2.1
+Name: phub
+Version: 3.0
+Summary: An API for PornHub
+Home-page: https://github.com/Egsagon/PHUB/
+Author: Egsagon
+Author-email: egsagon12@gmail.com
+License: GPLv3
+Platform: unix
+Platform: linux
+Platform: win32
+Platform: cygwin
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Education
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![PHUB](https://github.com/Egsagon/PHUB/blob/master/assets/banner.png)
 
 # PHUB - An API for PornHub.
 PHUB is an API wrapper for PornHub. It is able to fetch, search and download videos and supports account connections, achieved with efficient web scrapping using requests and regexes.
 
-> :warning: **Early development: bugs may occur** (also i'm a terrible programer)
+> :warning: **Early development + not maintained a lot** don't hesitate to submit issues and PRs
 
 ## Installation
 - Install using pip:
 ```sh
 pip install --upgrade phub
 ```
 
 - Or using this repository to get latest features:
 ```sh
 pip install --upgrade git+https://github.com/Egsagon/PHUB.git
 ```
 
 ## CLI usage
-You can use phub like so form the terminal to start a small downloading script:
-(Assuming `py` represents your python executable, on linux use `python3`)
+You can use phub like so from the terminal as as CLI script:
 ```sh
-py -m phub --help
+python3 -m phub
 ```
 
 Example for downloading a video knowing its url, in the best available quality:
 ```sh
-py -m phub --url https://... -q 'best'
-````
+py -m phub download --url https://www.pornhub.com/view_video.php?viewkey=xxx -q 'best'
+```
+
+You can also use the provided UI if you have `tkinter` installed:
+```sh
+py -m phub ui
+```
 
 ## Package usage
 Example video download usage:
 ```python
 import phub
 
 client = phub.Client()
@@ -41,15 +65,15 @@
 ```
 
 Example searching for videos:
 ```python
 record = client.search('enter query here')
 
 # Display all videos (careful if there is a lot of results)
-for video in record:
+for video in record.range(0, 10):
   print(video.title)
 ```
 
 ## Documentation
 See the [wiki](https://github.com/Egsagon/PHUB/wiki).
 
 ## Why?
```

### Comparing `phub-2.8/setup.cfg` & `phub-3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.8
+version = 3.0
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `phub-2.8/src/phub/__init__.py` & `phub-3.0/src/phub/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-## PHUB - A light API for interacting with PornHub. ##
+#### PHUB - A light API for interacting with PornHub. ####
 
 See https://github.com/Egsagon/PHUB for documentation.
 '''
 
 from phub import ( core, utils, consts, classes, parser )
 
 # Shortcuts
```

### Comparing `phub-2.8/src/phub/classes.py` & `phub-3.0/src/phub/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 '''
 ### Objects for the PHUB package. ###
 '''
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Self, Callable
+from typing import TYPE_CHECKING, Self, Callable, Generator
 if TYPE_CHECKING: from phub.core import Client
 
 import os
 import json
 from functools import cached_property
 from datetime import datetime, timedelta
 
+from bs4 import BeautifulSoup as Soup
+
 from phub import utils
 from phub import consts
 from phub import parser
 from phub.utils import log, download_presets as dlp
 
 # Errors
 class UserNotFoundError(Exception): pass
@@ -241,25 +243,27 @@
         segments = [url_base + segment for segment in utils.extract_urls(raw.text)]
         log('video', f'Parsed {len(segments)} video segments', level = 3)
         return segments
 
     def download(self,
                  path: str,
                  quality: utils.Quality,
-                 callback: Callable = dlp.bar(),
-                 max_retries: int = 5) -> str:
+                 callback: Callable = dlp.bar,
+                 max_retries: int = 5,
+                 **callback_arguments) -> str:
         '''
         #### Download the video locally. ####
         -------------------------------------
         
         Arguments:
-        - `path`               -- Directory or file to write to.
-        - `quality`            -- Desired video quality.
-        - `callback` (=`None`) -- Function to call to update download progress.
-        - `max_retries` (=`5`) -- Maximum retries per segment request.
+        - `path`                 -- Directory or file to write to.
+        - `quality`              -- Desired video quality.
+        - `callback`   (=`None`) -- Function to call to update download progress.
+        - `max_retries`   (=`5`) -- Maximum retries per segment request.
+        - `**callback_arguments` --Arguments to be passed to the callback on creation.
         
         NOTE 1 - If `path` is a directory, will create a new file in that directory
                  with the name of the video.
         NOTE 2 - Slow download. To use threaded downloads, call `get_M3U` instead.
         NOTE 3 - Glitchy logs.
         -------------------------------------
         Returns the path of the file.
@@ -268,37 +272,41 @@
         log('video', f'Downloading {self} at', path, level = 5)
         
         # Append name if path is directory
         if os.path.isdir(path):
             path += ('' if path.endswith('/') else '/') + utils.pathify(self.title) + '.mp4'
             log('video', f'Changing path to', path, level = 2)
         
-        log(' D L ', 'Starting video download for', self)
+        log('downl', 'Starting video download for', self)
         
         segments = self.get_M3U(quality, process = True)
         
+        # Initialise callback
+        callback_wrapper = callback(**callback_arguments)
+        
         # Start downloading
         with open(path, 'wb') as output:
             
             for index, url in enumerate(segments):
-                log(' D L ', f'Downloading {index + 1}/{len(segments)}', level = 3, r = 0) # TODO
-                if callback: callback(index + 1, len(segments))
+                log('downl', f'Downloading {index + 1}/{len(segments)}', level = 3, r = 0) # TODO
+                callback_wrapper(index + 1, len(segments))
                 
                 for i in range(max_retries):
                     res = self.client._call('GET', url, simple_url = False, throw = False)
                     
                     if not res.ok:                        
-                        log(' D L ', f'Segment download failed, retrying ({i}/{max_retries})', level = 1)
+                        log('downl', f'Segment download failed, retrying ({i}/{max_retries})', level = 1)
                         continue
                     
                     output.write(res.content)
                     break
         
         # Stop
-        log(' D L ', 'Successfully downloaded video at', path)
+        callback_wrapper(len(segments), len(segments)) # Make sure full progress is registered
+        log('downl', 'Successfully downloaded video at', path)
         return path
     
     # ======== Properties ======== #
     
     @cached_property
     def title(self) -> str:
         '''
@@ -546,9 +554,118 @@
         
         except IndexError:
             log('viter', 'Reached end of generation')
             raise StopIteration
         
         self.index += 1
         return result
+    
+    def range(self, start: int, stop: int, step: int = 1) -> Generator[Video , None, None]:
+        '''
+        #### Emit a generator containing a slice of videos. ####
+        --------------------------------------------------------
+        Arguments:
+        - `start`       -- Start index.
+        - `stop`        -- Stop index.
+        - `step` (=`1`) -- Step.
+        
+        --------------------------------------------------------
+        Yields `Video` objects.
+        '''
+        
+        for index in range(start, stop, step):
+            yield self[index]
+
+@dataclass
+class FeedItem:
+    type: consts.FeedType
+    content: str = field(repr = False)
+    author: str = field(repr = False)
+    url: str = field(repr = False)
+    date: str = field(repr = False)
+
+class Feed:
+    
+    def __init__(self, client: Client) -> None:
+        '''
+        #### Generate a new feed object. ####
+        -------------------------------------
+        
+        Arguments:
+        - `client` -- Client object to use.
+        '''
+
+        self.client = client
+        self.cache: dict[int, list[FeedItem]] = {}
+    
+    def _get_page(self, page: int) -> list[FeedItem]:
+        '''
+        #### Fetch a specific feed page. ####
+        -------------------------------------
         
-# EOF
+        Arguments:
+        - `page` -- Page index.
+        
+        -------------------------------------
+        Returns a list of 14 `FeedItem` elements.
+        '''
+        
+        # Fetch and parse page
+        url = 'feeds'
+        if page > 0: url += f'_ajax?ajax=1&page={page + 1}'
+        raw = self.client._call('GET', url).text
+        
+        soup = Soup(raw, 'html.parser')
+        sections: list[Soup] = soup.find_all('section', {'class': 'feedItemSection'})
+        
+        items = []
+        for section in sections:
+            
+            badge = section.find('span', {'class': 'usernameBadgesWrapper'})
+            stream = section.find('a', {'class': 'stream_link'})
+            
+            author = None
+            if badge:
+                author = User.get(client = self.client,
+                                  url = badge.find('a').get('href'))
+            
+            url = date = None
+            if stream:
+                url = stream.get('href')
+                date = stream.text
+            
+            content = section.find('div', {'class': 'feedInfo'}).text
+            if date: content = content.replace(date, '')
+            
+            items += [FeedItem(
+                type = section.get('data-table'),
+                content = utils.hard_strip(content),
+                author = author,
+                url = url,
+                date = utils.hard_strip(date)
+            )]
+        
+        # Save to cache
+        self.cache[page] = items
+        return items
+
+    def get(self, index: int) -> FeedItem:
+        '''
+        #### Get a specific feed item. ####
+        -----------------------------------
+        
+        Arguments:
+        - `index` -- The feed element index.
+        
+        -------------------------------------
+        Returns a `FeedItem` object.
+        '''
+        
+        page_index = index // 14
+        
+        page = self.cache.get(page_index)
+        if page is None:
+            page = self._get_page(page_index)
+        
+        return page[ index % 14 ]
+
+# EOF
```

### Comparing `phub-2.8/src/phub/consts.py` & `phub-3.0/src/phub/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,8 +49,21 @@
     
     # Match regexes
     is_valid_video_url   = re.compile( r'https://.{2,3}\.pornhub\.com/view_video\.php\?viewkey=[a-z\d]{13,15}'       ).fullmatch # Verify video URL validity
     
     # Old
     # video_model          = re.compile( r'<span class=\"usernameBadgesWrapper\"><a rel=\"\" href=\"(.*?)\"  class=\"bolded\">(.*?)</a>').findall # Get video author if model
 
+class FeedType:
+    '''
+    Types representation (most) feed elements.
+    '''
+    
+    SUBSCRIBED  = 'stream_subscriptions_pornstars'
+    ACHIEVEMENT = 'stream_achievements'
+    UPLOAD      = 'stream_videos_uploaded'
+    SITE_UPLOAD = 'stream_sites_subscriptions'
+    COMMENTED   = 'stream_grouped_comments_videos'
+    # TODO more stream types
+
+
 # EOF
```

### Comparing `phub-2.8/src/phub/core.py` & `phub-3.0/src/phub/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,24 @@
         Returns a `VideoIterator` object.
         '''
         
         url = consts.ROOT + f'users/{self.name}/videos/favorites'
         return classes.VideoIterator(self.client, url,
                                      corrector = utils.remove_video_ads)
 
+    @cached_property
+    def feed(self) -> classes.Feed:
+        '''
+        #### Get the account feed. ####
+        -------------------------------
+        Returns a `Feed` object.
+        '''
+        
+        return classes.Feed(self.client)
+
 class Client:
     '''
     Represents a Client capable of interacting with PornHub.
     '''
     
     def __init__(self,
                  username: str = None,
@@ -122,15 +132,15 @@
         # Connect Account object
         self.account: Account | None = Account(self)
         
         # Autologin
         self.logged = False
         if autologin: self.login()
         
-        log('client', 'Initialised new client', repr(self))
+        log('clien', 'Initialised new client', repr(self))
 
     def __repr__(self) -> str:
         '''
         Display Client object representation and informations about
         whether the account is connected.
         '''
         
@@ -163,15 +173,15 @@
             
             except json.JSONDecodeError or AssertionError:
                 raise ValueError('Invalid json file.')
         
         if isinstance(data, dict):
             if data.get('username') and data.get('password'):
                 
-                log('Initialising client from', type(data), level = 7)
+                log('clien', 'Initialising client from', type(data), level = 7)
                 return cls(**data)
             
             raise KeyError('Data must have username and password keys.')
         
         raise TypeError('Invalid type for data:', type(data))
     
     def _call(self,
@@ -196,24 +206,24 @@
         ----------------------------------------------------------------------------
         Returns a `requests.Response` object.
         '''
         
         url = consts.ROOT + utils.slash(func, '**') \
               if simple_url else func
         
-        log('client', f'Sending request at {utils.shortify(url, 25)}', level = 6)
+        log('clien', f'Sending request at {utils.shortify(url, 25)}', level = 6)
         
         response = self.session.request(
             method = method,
             url = url,
             headers = consts.HEADERS | headers | self.language,
             data = data
         )
         
-        log('client', 'Request passed with status', response.status_code, level = 6)
+        log('clien', 'Request passed with status', response.status_code, level = 6)
         
         if throw and not response.ok:
             raise ConnectionError(f'Request `{func}` failed:' + \
                 utils.shortify(response.text))
         
         return response
     
@@ -230,28 +240,28 @@
         '''
         
         log('client', 'Attempting loggin...', level = 6)
         
         # Extract token
         home = self._call('GET', '/').text
         token = consts.regexes.extract_token(home)
-        log('client', 'Extracted token', token, level = 5)
+        log('clien', 'Extracted token', token, level = 5)
         
         # Send credentials
-        log('client', 'Sending payload', level = 5)
+        log('clien', 'Sending payload', level = 5)
         payload = consts.LOGIN_PAYLOAD | self.creds | {'token': token}
         
         response = self._call('POST', 'front/authenticate', data = payload)
         success = int(response.json()['success'])
         
         if success:
-            log('client', 'Login successful!', level = 6)
+            log('clien', 'Login successful!', level = 6)
         
         else:
-            log('client', 'Login failed', level = 2)
+            log('clien', 'Login failed', level = 2)
             
             # Throw error
             if throw:
                 raise ConnectionRefusedError('Connection failed. Check credentials.')
         
         self.logged = success
         return success
@@ -288,15 +298,15 @@
         
         NOTE - `name` parameter is experimental.
         
         -----------------------------------------------------
         Returns a `User` object.
         '''
         
-        log('client', 'Fetching user', name, level = 6)
+        log('clien', 'Fetching user', name, level = 6)
         
         return classes.User.get(self, url, name)
     
     def search(self, query: str) -> classes.VideoIterator:
         '''
         #### Search for videos on PornHub servers. ####
         -----------------------------------------------
@@ -304,12 +314,12 @@
         Arguments:
         - `query` -- Sentence to send to the servers.
         
         -----------------------------------------------
         Returns a `VideoIterator` object.
         '''
         
-        log('client', 'Opening new search query:', query, level = 6)
+        log('clien', 'Opening new search query:', query, level = 6)
         url = consts.ROOT + 'video/search?search=' + query
         return classes.VideoIterator(self, url)
 
 # EOF
```

### Comparing `phub-2.8/src/phub/parser.py` & `phub-3.0/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.8/src/phub/phub_ui.py` & `phub-3.0/src/phub/phub_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,14 @@
         if not phub.consts.regexes.is_valid_video_url(url):
             return tkmb.showwarning('Error', 'Invalid video URL.')
         
         # Download
         threading.Thread(target = self.download, args = [url]).start()
 
 
-def main(client) -> None:
-    App(client).mainloop()
+def main() -> None:
+    App(phub.Client()).mainloop()
 
 if __name__ == '__main__':
-    main(phub.Client())
+    main()
 
 # EOF
```

### Comparing `phub-2.8/src/phub/utils.py` & `phub-3.0/src/phub/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,21 @@
     Returns a sanitized list of video URLs.
     '''
     
     return li[4:]
 
 def log(cls: str, *text, level: int = 1, r: bool = False) -> None:
     '''
-    Homemade logging.
+    #### Homemade logging. ####
+    ---------------------------
+    
+    Arguments:
+    - `*`            -- Log content.
+    - `level` (=`1`) -- Log level.
+    - `r` (=`False`) -- Wether log is inline.
     '''
     
     global DEBUG_RESET
     
     if not DEBUG: return
     
     text = ' '.join(map(str, text))
@@ -168,14 +174,30 @@
         print(raw, end = '', file = DEBUG_FILE)
         DEBUG_RESET = True
     
     elif r and DEBUG_RESET: print(f'\r{raw}', end = '', file = DEBUG_FILE)
     elif not r and DEBUG_RESET: print(f'\n{raw}', file = DEBUG_FILE)
     else: print(raw, file = DEBUG_FILE)
 
+def hard_strip(text: str, sep: str = ' ') -> str:
+    '''
+    #### Remove all useless spaces from a text. ####
+    ------------------------------------------------
+    
+    Arguments:
+    - `text`       -- The text to strip.
+    - `sep` (=` `) -- Separator between each words.
+    
+    ------------------------------------------------
+    Returns a stripped version of the text.
+    '''
+    
+    if not text: return
+    return sep.join(text.split())
+
 
 class download_presets:
     '''
     Callback presets for displaying download progress.
     '''
     
     @staticmethod
@@ -193,27 +215,27 @@
         
             print(tem.format(percent = percent, cur = cur, total = total),
                   end = '\n' if percent >= 100 else '')
         
         return wrapper
     
     @staticmethod
-    def bar(*args, **kwargs) -> Callable:
+    def bar(**kwargs) -> Callable:
         '''
-        Display current progress a a bar.
+        Display current progress as a tqdm bar.
         '''
         
-        bar = tqdm.tqdm(*args, **kwargs)
+        bar = tqdm.tqdm(**kwargs)
         
         def wrapper(current: int, total: int) -> None:
             
             bar.total = total
             bar.update(1)
             if current == total: bar.close()
-        
+            
         return wrapper
     
     @staticmethod
     def std(file = sys.stdout) -> Callable:
         '''
         Output progress as percentage to a file.
         '''
```

