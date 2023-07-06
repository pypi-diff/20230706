# Comparing `tmp/gokyuzu-2.0.4.tar.gz` & `tmp/gokyuzu-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-2.0.4.tar", last modified: Mon Jul  3 19:03:43 2023, max compression
+gzip compressed data, was "gokyuzu-2.0.5.tar", last modified: Thu Jul  6 17:04:03 2023, max compression
```

## Comparing `gokyuzu-2.0.4.tar` & `gokyuzu-2.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.509438 gokyuzu-2.0.4/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     6427 2023-07-03 19:03:43.509312 gokyuzu-2.0.4/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     5652 2023-07-03 19:01:58.000000 gokyuzu-2.0.4/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.507897 gokyuzu-2.0.4/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     8595 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      688 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)      247 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskyRecords.py
--rw-r--r--   0 kilic      (501) staff       (20)     4014 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)    31236 2023-07-03 19:02:31.000000 gokyuzu-2.0.4/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.508786 gokyuzu-2.0.4/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     6427 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      357 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-07-03 19:03:43.000000 gokyuzu-2.0.4/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-07-03 19:03:04.000000 gokyuzu-2.0.4/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-07-03 19:03:43.509479 gokyuzu-2.0.4/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1028 2023-07-03 19:02:59.000000 gokyuzu-2.0.4/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-03 19:03:43.509007 gokyuzu-2.0.4/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     5440 2023-07-03 19:01:04.000000 gokyuzu-2.0.4/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 17:04:03.903820 gokyuzu-2.0.5/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-07-03 19:01:04.000000 gokyuzu-2.0.5/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     6440 2023-07-06 17:04:03.903692 gokyuzu-2.0.5/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     5652 2023-07-03 19:01:58.000000 gokyuzu-2.0.5/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 17:04:03.901743 gokyuzu-2.0.5/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     8595 2023-07-03 19:01:04.000000 gokyuzu-2.0.5/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      688 2023-07-03 19:01:04.000000 gokyuzu-2.0.5/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)      247 2023-07-03 19:01:04.000000 gokyuzu-2.0.5/gokyuzu/BlueskyRecords.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4014 2023-07-03 19:01:04.000000 gokyuzu-2.0.5/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)    33704 2023-07-06 16:57:14.000000 gokyuzu-2.0.5/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 17:04:03.902951 gokyuzu-2.0.5/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     6440 2023-07-06 17:04:03.000000 gokyuzu-2.0.5/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      357 2023-07-06 17:04:03.000000 gokyuzu-2.0.5/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-07-06 17:04:03.000000 gokyuzu-2.0.5/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-07-06 17:04:03.000000 gokyuzu-2.0.5/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-07-06 17:04:03.000000 gokyuzu-2.0.5/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-07-06 17:02:56.000000 gokyuzu-2.0.5/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-07-06 17:04:03.903859 gokyuzu-2.0.5/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1041 2023-07-06 17:03:08.000000 gokyuzu-2.0.5/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-07-06 17:04:03.903195 gokyuzu-2.0.5/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-07-03 19:01:04.000000 gokyuzu-2.0.5/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     5440 2023-07-03 19:01:04.000000 gokyuzu-2.0.5/tests/test_main.py
```

### Comparing `gokyuzu-2.0.4/PKG-INFO` & `gokyuzu-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.4
+Version: 2.0.5
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gokyuzu-2.0.4/README.md` & `gokyuzu-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.4/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-2.0.5/gokyuzu/BlueskyEndpoints.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.4/gokyuzu/BlueskyHelper.py` & `gokyuzu-2.0.5/gokyuzu/BlueskyHelper.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.4/gokyuzu/BlueskySession.py` & `gokyuzu-2.0.5/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.4/gokyuzu/__init__.py` & `gokyuzu-2.0.5/gokyuzu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,25 +216,24 @@
         
         if swapCommit is not None:
             request_data["swapCommit"] = swapCommit
 
         response = self.SESSION.postJson(request_url, json=request_data)
         return response
     
-    def deleteRecord(self, repo, record, collection, swapRecord=None, swapCommit=None):
+    def deleteRecord(self, repo, rkey, collection, swapRecord=None, swapCommit=None):
         request_url = self.ENDPOINTS.deleteRecord()
-        # TODO: rkey or record? 
         request_data = {
             "repo": repo,
-            "record": record,
+            "rkey": rkey,
             "collection": collection,
             "swapRecord": swapRecord,
             "swapCommit": swapCommit
         }
-        response = self.SESSION.postJson(request_url, json=request_data)
+        response = self.SESSION.post(request_url, json=request_data)
         return response
     
     def describeRepo(self, repo):
         request_url = self.ENDPOINTS.describeRepo()
         request_data = {
             "repo": repo
         }
@@ -246,23 +245,22 @@
         if commit is not None:
             request_url += "&commit={}".format(commit)
         response = self.SESSION.get(request_url)
         return response
 
     def listRecords(self, user_did, collection, limit=10, record_key_start=None, record_key_end=None, reverse=False):
         request_url = self.ENDPOINTS.listRecords()
-        request_data = {
-            "repo": user_did,
-            "collection": collection,
-            "limit": limit,
-            "rkeyStart": record_key_start,
-            "rkeyEnd": record_key_end,
-            "reverse": reverse
-        }
-        response = self.SESSION.postJson(request_url, json=request_data)
+        request_url += "?repo={}&collection={}&limit={}".format(user_did, collection, limit)
+        if record_key_start is not None:
+            request_url += "&rkeyStart={}".format(record_key_start)
+        if record_key_end is not None:
+            request_url += "&rkeyEnd={}".format(record_key_end)
+        if reverse:
+            request_url += "&reverse=true"
+        response = self.SESSION.get(request_url)
         return response
     
     def putRecord(self, repo, collection, record_key, record, validate=True, swapRecord=None, swapCommit=None):
         request_url = self.ENDPOINTS.putRecord()
         request_data = {
             "repo": repo,
             "collection": collection,
@@ -801,14 +799,81 @@
 
     #region unspecced
     def health(self):
         request_url = self.ENDPOINTS.health()
         response = self.SESSION.get(request_url)
         return response
     
+    def get_all_followers(self, handle, debug=False):
+        followers = []
+        next_cursor = None
+
+        while True:
+            if next_cursor is None:
+                response = self.getFollowers(handle, limit=100)
+            else:
+                response = self.getFollowers(handle, cursor=next_cursor, limit=100)
+            body = response.json()
+            followers.extend(body.get("followers", []))
+            old_cursor = next_cursor
+            next_cursor = body.get("cursor")
+
+            if old_cursor == next_cursor or not next_cursor:
+                break
+        if debug:
+            print("{} followers found for {}".format(len(followers), handle))
+        return followers
+
+    
+    def get_all_follows(self, handle, debug=False):
+        follows = []
+        next_cursor = None
+
+        while True:
+            if next_cursor is None:
+                response = self.getFollows(handle, limit=100)
+            else:
+                response = self.getFollows(handle, cursor=next_cursor, limit=100)
+            body = response.json()
+            follows.extend(body.get("follows", []))
+            old_cursor = next_cursor
+            next_cursor = body.get("cursor")
+
+            if old_cursor == next_cursor or not next_cursor:
+                break
+        if debug:
+            print("{} follows found for {}".format(len(follows), handle))
+        return follows
+    
+    def get_relavants_of(self, handle, debug=False):
+        followers = self.get_all_followers(handle, debug=debug)
+        follows = self.get_all_follows(handle, debug=debug)
+        follow_list = {}
+        for follower in followers:
+            follow_list[follower["handle"]] = follower
+        for follow in follows:
+            if follow["handle"] not in follow_list:
+                follow_list[follow["handle"]] = follow
+        return follow_list
+    
+    def merge_unique_lists(self, first_list, second_list):
+        merged_list = {}
+        for item in first_list:
+            merged_list[item["handle"]] = item
+        for item in second_list:
+            if item["handle"] not in merged_list:
+                merged_list[item["handle"]] = item
+        return merged_list
+    
+    def exclude_users(self, follow_list: dict, exluded_users):
+        for handle in exluded_users:
+            if handle in follow_list.keys():
+                follow_list.pop(handle)
+        return follow_list
+    
     def createLinkFromAtUri(self, at_uri):
         did, rkey = BlueskyHelper.analyze_at_uri(at_uri)
         handle = self.getProfile(did).json().get("handle")
         return BlueskyHelper.createPostLink(handle, rkey)
 
     def quote(self, text, repo, record_uri, record_cid, createdAt=None):
         if createdAt is None:
```

### Comparing `gokyuzu-2.0.4/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-2.0.5/gokyuzu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.4
+Version: 2.0.5
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gokyuzu-2.0.4/setup.py` & `gokyuzu-2.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='2.0.4',
+    version='2.0.5',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
     ],
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `gokyuzu-2.0.4/tests/test_main.py` & `gokyuzu-2.0.5/tests/test_main.py`

 * *Files identical despite different names*

