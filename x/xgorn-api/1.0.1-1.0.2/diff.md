# Comparing `tmp/xgorn-api-1.0.1.tar.gz` & `tmp/xgorn-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgorn-api-1.0.1.tar", last modified: Tue Jul  4 03:12:10 2023, max compression
+gzip compressed data, was "xgorn-api-1.0.2.tar", last modified: Wed Jul  5 05:27:19 2023, max compression
```

## Comparing `xgorn-api-1.0.1.tar` & `xgorn-api-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/xgorn_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/xgorn_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-04 03:11:40.000000 xgorn-api-1.0.1/xgorn_api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:12:10.586305 xgorn-api-1.0.1/xgorn_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 03:12:10.000000 xgorn-api-1.0.1/xgorn_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:27:19.199775 xgorn-api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-05 05:27:07.000000 xgorn-api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-05 05:27:19.199775 xgorn-api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-05 05:27:07.000000 xgorn-api-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 05:27:19.199775 xgorn-api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-05 05:27:07.000000 xgorn-api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:27:19.199775 xgorn-api-1.0.2/xgorn_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-05 05:27:07.000000 xgorn-api-1.0.2/xgorn_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-05 05:27:07.000000 xgorn-api-1.0.2/xgorn_api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:27:19.199775 xgorn-api-1.0.2/xgorn_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-05 05:27:19.000000 xgorn-api-1.0.2/xgorn_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-05 05:27:19.000000 xgorn-api-1.0.2/xgorn_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 05:27:19.000000 xgorn-api-1.0.2/xgorn_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 05:27:19.000000 xgorn-api-1.0.2/xgorn_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 05:27:19.000000 xgorn-api-1.0.2/xgorn_api.egg-info/top_level.txt
```

### Comparing `xgorn-api-1.0.1/LICENSE` & `xgorn-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xgorn-api-1.0.1/setup.py` & `xgorn-api-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,27 +26,28 @@
 
 with open('xgorn_api/__init__.py', encoding='utf-8') as f:
     version = re.findall(r'__version__ = \'(.+)\'', f.read())[0]
 
 
 with open('xgorn_api/api.py', encoding='utf-8') as f:
     base_url = re.findall(r'self\.base_url = \'(.+)\'', f.read())[0]
+    base_url_ = base_url.replace("https://", "")
 
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name='xgorn-api',
     version=version,
-    description=f'API Interface for {base_url}',
+    description=f'API Interface for {base_url_}',
     long_description=readme,
     long_description_content_type='text/markdown',
-    url='https://github.com/api-xgorn-docs',
+    url='https://github.com/X-Gorn/xgorn-api',
     author='xgorn',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
@@ -56,20 +57,20 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Internet',
         'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     keywords='api scraper bypasser translator client library python',
     project_urls={
         'Web': base_url,
         'Documentation': base_url+'/docs'
     },
     python_requires='~=3.7',
     packages=find_packages(),
     install_requires=[
-        'requests',
+        'requests'
     ],
 )
```

### Comparing `xgorn-api-1.0.1/xgorn_api/__init__.py` & `xgorn-api-1.0.2/xgorn_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from .api import NoidAPI
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
```

### Comparing `xgorn-api-1.0.1/xgorn_api/api.py` & `xgorn-api-1.0.2/xgorn_api/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,77 +22,101 @@
 
 from requests import get, post
 
 
 class NoidAPI:
     
     def __init__(self) -> None:
+        self.bypass = Bypass(self)
+        self.scrape = Scrape(self)
+        self.translate = Translate(self)
+        self.music = Music(self)
         self.api_key = 'api-key'
         self.base_url = 'https://api.xgorn.pp.ua'
     
     def make_request(self, method: str, endpoint: str, **kwargs) -> dict:
         kwargs['api_key'] = self.api_key
         if self.api_key == 'api-key':
             return {'error': True, 'message': 'Invalid API key'}
         if method == 'get':
             return get(self.base_url+endpoint, params=kwargs).json()
         elif method == 'post':
             return post(self.base_url+endpoint, data=kwargs).json()
         else:
             return {'error': True, 'message': 'Invalid method'}
     
-    def ouo_bypass(self, url: str) -> dict:
-        return self.make_request('get', '/ouo_bypass', url=url)
+class Bypass:
     
-    def mirrored_bypass(self, url: str, host: str) -> dict:
-        return self.make_request('get', '/mirrored_bypass', url=url, host=host)
+    def __init__(self, api):
+        self.api = api
     
-    def tiktok_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/tiktok_scrape', url=url)
+    def ouo(self, url: str) -> dict:
+        return self.api.make_request('get', '/bypass/ouo', url=url)
     
-    def facebook_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/facebook_scrape', url=url)
+    def mirrored(self, url: str, host: str) -> dict:
+        return self.api.make_request('get', '/bypass/mirrored', url=url, host=host)
+
+class Scrape:
+    
+    def __init__(self, api):
+        self.api = api
+    
+    def tiktok(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/tiktok', url=url)
+    
+    def facebook(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/facebook', url=url)
     
-    def instagram_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/instagram_scrape', url=url)
+    def instagram(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/instagram', url=url)
     
-    def instagram_scrapev2(self, url: str) -> dict:
-        return self.make_request('get', '/instagram_scrapev2', url=url)
+    def instagramv2(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/instagramv2', url=url)
 
-    def twitter_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/twitter_scrape', url=url)
+    def twitter(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/twitter', url=url)
     
-    def twitter_scrapev2(self, url: str) -> dict:
-        return self.make_request('get', '/twitter_scrapev2', url=url)
+    def twitterv2(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/twitterv2', url=url)
     
-    def likee_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/likee_scrape', url=url)
+    def likee(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/likee', url=url)
     
-    def pinterest_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/pinterest_scrape', url=url)
+    def pinterest(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/pinterest', url=url)
     
-    def pinterest_scrapev2(self, url: str) -> dict:
-        return self.make_request('get', '/pinterest_scrapev2', url=url)
+    def pinterestv2(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/pinterestv2', url=url)
     
-    def terabox_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/terabox_scrape', url=url)
+    def terabox(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/terabox', url=url)
     
-    def gofile_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/gofile_scrape', url=url)
+    def gofile(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/gofile', url=url)
     
-    def krakenfiles_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/krakenfiles_scrape', url=url)
+    def krakenfiles(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/krakenfiles', url=url)
     
-    def yifysubtitles_scrape(self, imdb_id: str, lang: str) -> dict:
-        return self.make_request('get', '/yifysubtitles_scrape', imdb_id=imdb_id, lang=lang)
+    def yifysubtitles(self, imdb_id: str, lang: str) -> dict:
+        return self.api.make_request('get', '/scrape/yifysubtitles', imdb_id=imdb_id, lang=lang)
     
-    def filelions_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/filelions_scrape', url=url)
+    def filelions(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/filelions', url=url)
     
-    def streamwish_scrape(self, url: str) -> dict:
-        return self.make_request('get', '/streamwish_scrape', url=url)
+    def streamwish(self, url: str) -> dict:
+        return self.api.make_request('get', '/scrape/streamwish', url=url)
+
+class Translate:
+    
+    def __init__(self, api):
+        self.api = api
+    
+    def srt(self, url: str, source_lang: str, dest_lang: str) -> dict:
+        return self.api.make_request('get', '/translate/srt', url=url, source_lang=source_lang, dest_lang=dest_lang)
+
+class Music:
     
-    def srt_translate(self, url: str, source_lang: str, dest_lang: str) -> dict:
-        return self.make_request('get', '/srt_translate', url=url, source_lang=source_lang, dest_lang=dest_lang)
+    def __init__(self, api):
+        self.api = api
     
-    def shazam_music_find(self, url: str, type_: str) -> dict:
-        return self.make_request('get', '/shazam_music_find', url=url, type=type_)
+    def shazam(self, url: str, type_: str) -> dict:
+        return self.api.make_request('get', '/music/shazam', url=url, type=type_)
```

