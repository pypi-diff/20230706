# Comparing `tmp/tvpy-0.0.7.tar.gz` & `tmp/tvpy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvpy-0.0.7.tar", max compression
+gzip compressed data, was "tvpy-0.0.8.tar", max compression
```

## Comparing `tvpy-0.0.7.tar` & `tvpy-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,22 @@
--rw-r--r--   0        0        0      360 2022-08-27 14:32:39.039418 tvpy-0.0.7/README.md
--rw-r--r--   0        0        0      762 2022-08-27 20:59:24.110975 tvpy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-27 14:32:39.040843 tvpy-0.0.7/tvpy/__init__.py
--rw-r--r--   0        0        0     1180 2022-08-27 20:54:28.502542 tvpy-0.0.7/tvpy/app.py
--rw-r--r--   0        0        0      373 2022-08-27 20:18:35.353603 tvpy-0.0.7/tvpy/index.css
--rw-r--r--   0        0        0      468 2022-08-27 20:56:44.158606 tvpy-0.0.7/tvpy/index.html
--rw-r--r--   0        0        0      794 2022-08-27 20:25:54.369130 tvpy-0.0.7/tvpy/index.js
--rw-r--r--   0        0        0      158 2022-08-27 14:32:39.041175 tvpy-0.0.7/tvpy/main.py
--rw-r--r--   0        0        0      141 2022-08-27 14:32:39.041314 tvpy-0.0.7/tvpy/scan.py
--rw-r--r--   0        0        0     1736 2022-08-27 16:10:11.450550 tvpy-0.0.7/tvpy/search.py
--rw-r--r--   0        0        0     1237 2022-08-27 20:59:29.211723 tvpy-0.0.7/setup.py
--rw-r--r--   0        0        0     1057 2022-08-27 20:59:29.211984 tvpy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      439 2022-10-27 22:41:22.168403 tvpy-0.0.8/README.md
+-rw-r--r--   0        0        0     1170 2022-10-27 22:42:33.431720 tvpy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-24 15:30:19.537240 tvpy-0.0.8/tvpy/__init__.py
+-rw-r--r--   0        0        0       75 2022-10-27 17:29:08.755964 tvpy-0.0.8/tvpy/config.py
+-rw-r--r--   0        0        0      359 2022-10-27 22:25:38.846201 tvpy-0.0.8/tvpy/console.py
+-rw-r--r--   0        0        0      373 2022-09-29 16:11:37.215342 tvpy-0.0.8/tvpy/index.css
+-rw-r--r--   0        0        0      510 2022-09-29 16:11:37.215342 tvpy-0.0.8/tvpy/index.html
+-rw-r--r--   0        0        0     1053 2022-09-29 16:11:37.215342 tvpy-0.0.8/tvpy/index.js
+-rw-r--r--   0        0        0      586 2022-10-27 20:40:17.015834 tvpy-0.0.8/tvpy/main.py
+-rw-r--r--   0        0        0     1196 2022-10-21 13:46:42.530428 tvpy-0.0.8/tvpy/tmdb.py
+-rw-r--r--   0        0        0     1289 2022-10-22 15:40:50.248053 tvpy-0.0.8/tvpy/torrent.py
+-rw-r--r--   0        0        0     2806 2022-10-27 22:01:30.888905 tvpy-0.0.8/tvpy/tv_down.py
+-rw-r--r--   0        0        0      413 2022-10-27 18:17:43.122558 tvpy-0.0.8/tvpy/tv_html.py
+-rw-r--r--   0        0        0     1367 2022-10-27 20:04:09.125420 tvpy-0.0.8/tvpy/tv_info.py
+-rw-r--r--   0        0        0     2585 2022-10-27 22:02:00.772627 tvpy-0.0.8/tvpy/tv_json.py
+-rw-r--r--   0        0        0     1023 2022-10-27 22:02:23.700415 tvpy-0.0.8/tvpy/tv_klyn.py
+-rw-r--r--   0        0        0      758 2022-10-27 22:01:45.132773 tvpy-0.0.8/tvpy/tv_renm.py
+-rw-r--r--   0        0        0     1930 2022-10-27 22:01:38.512834 tvpy-0.0.8/tvpy/tv_subs.py
+-rw-r--r--   0        0        0     1401 2022-10-27 22:26:08.469854 tvpy-0.0.8/tvpy/tvpy.py
+-rw-r--r--   0        0        0     1672 2022-10-27 22:02:06.892571 tvpy-0.0.8/tvpy/util.py
+-rw-r--r--   0        0        0     1877 2022-10-27 22:42:40.270753 tvpy-0.0.8/setup.py
+-rw-r--r--   0        0        0     1515 2022-10-27 22:42:40.271216 tvpy-0.0.8/PKG-INFO
```

### Comparing `tvpy-0.0.7/tvpy/index.js` & `tvpy-0.0.8/tvpy/index.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 function item(i) {
     return `
     <div class='item'>
       <div class='col'>
         <a target="_blank" href="https://www.imdb.com/title/${i.imdb_id}/">
-          <img style="max-width:160px;" src="data:image/jpg;base64,${i.poster_base64}"/>
+          <img style="max-width:160px" src="data:image/jpgbase64,${i.poster_base64}"/>
         </a>      
       </div>
       <div class='col'>
         <h2>${i.name}</h2>
         <p>${i.overview}</p>
         <span><b>${i.rating}</b> by ${i.ratingCount.toLocaleString('en-US')} users</span>
       </div>
@@ -24,8 +24,16 @@
         items.append(div)
     })
 }
 
 addEventListener('DOMContentLoaded', () => {
     data.sort((a, b) => b.rating - a.rating)
     render()
+
+    const socket = new WebSocket("ws://localhost:8765")
+    socket.onopen = function(e) {}
+    socket.onclose = function(event) {}
+    socket.onerror = function(error) {}
+    socket.onmessage = function(event) {
+        console.log(`[message]  ${event.data}`)
+    }
 })
```

### Comparing `tvpy-0.0.7/PKG-INFO` & `tvpy-0.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 Metadata-Version: 2.1
 Name: tvpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: 📺 TvPy
 Home-page: https://github.com/gkutiel/tvpy/tree/master
 Author: Gilad Kutiel
 Author-email: gilad.kutiel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: 1337x (>=1.2.3,<2.0.0)
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: fire (>=0.4.0,<0.5.0)
+Requires-Dist: fs.smbfs (>=1.0.5,<2.0.0)
+Requires-Dist: libtorrent (>=2.0.7,<3.0.0)
+Requires-Dist: parse-torrent-title (>=2.4,<3.0)
+Requires-Dist: pyright (>=1.1.273,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Requires-Dist: websockets (>=10.3,<11.0)
 Project-URL: Documentation, https://github.com/gkutiel/tvpy/tree/master
 Project-URL: Repository, https://github.com/gkutiel/tvpy/tree/master
 Description-Content-Type: text/markdown
 
 # 📺 TvPy 
-Generate html from folder names.
+Best command line to manage tv shows.
+
+[![asciicast](https://asciinema.org/a/c9vcmIziWPfZUXPDlVToBteyT.svg)](https://asciinema.org/a/c9vcmIziWPfZUXPDlVToBteyT)
 
 ## Installation
 ```shell
 > pip install tvpy
 ```
 
 ## Get an API Key
 You need to get an API key from [TMDB](https://www.themoviedb.org/settings/api) and save it as `key.txt` in your working directory.
 
 ## Usage
 ```shell
-> mkdir Carnival.Row Resident.Alien Liar Under.the.Banner.of.Heaven
-> tv-json . && tv-html
+> mkdir Carnival.Row 
+> tvpy Carnival.Row 
 ```
```

