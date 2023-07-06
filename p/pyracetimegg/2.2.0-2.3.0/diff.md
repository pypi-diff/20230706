# Comparing `tmp/pyracetimegg-2.2.0-py3-none-any.whl.zip` & `tmp/pyracetimegg-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20233 bytes, number of entries: 18
+Zip file size: 20294 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-05 06:04 pyracetimegg/__init__.py
--rw-rw-rw-  2.0 fat     6324 b- defN 23-Jul-05 06:04 pyracetimegg/api.py
+-rw-rw-rw-  2.0 fat     6997 b- defN 23-Jul-06 06:22 pyracetimegg/api.py
 -rw-rw-rw-  2.0 fat     5801 b- defN 23-Jun-20 19:30 pyracetimegg/category.py
 -rw-rw-rw-  2.0 fat     6507 b- defN 23-Jul-05 06:04 pyracetimegg/object_mapping.py
 -rw-rw-rw-  2.0 fat    14033 b- defN 23-Jun-20 19:30 pyracetimegg/race.py
 -rw-rw-rw-  2.0 fat     1036 b- defN 23-Jun-20 19:27 pyracetimegg/test_api.py
 -rw-rw-rw-  2.0 fat      628 b- defN 23-Jun-18 00:43 pyracetimegg/throttled_request.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 23-Jun-20 19:30 pyracetimegg/user.py
 -rw-rw-rw-  2.0 fat     1813 b- defN 23-Jun-23 14:00 pyracetimegg/utils.py
 -rw-rw-rw-  2.0 fat      292 b- defN 23-Jul-03 11:57 pyracetimegg/objects/__init__.py
--rw-rw-rw-  2.0 fat     5519 b- defN 23-Jul-05 06:04 pyracetimegg/objects/category.py
--rw-rw-rw-  2.0 fat    15084 b- defN 23-Jul-05 06:04 pyracetimegg/objects/race.py
--rw-rw-rw-  2.0 fat     4383 b- defN 23-Jul-05 06:04 pyracetimegg/objects/user.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Jul-05 06:05 pyracetimegg-2.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      390 b- defN 23-Jul-05 06:05 pyracetimegg-2.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 06:05 pyracetimegg-2.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-05 06:05 pyracetimegg-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1485 b- defN 23-Jul-05 06:05 pyracetimegg-2.2.0.dist-info/RECORD
-18 files, 69321 bytes uncompressed, 17805 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat     5513 b- defN 23-Jul-06 09:07 pyracetimegg/objects/category.py
+-rw-rw-rw-  2.0 fat    15135 b- defN 23-Jul-06 08:42 pyracetimegg/objects/race.py
+-rw-rw-rw-  2.0 fat     4389 b- defN 23-Jul-06 08:48 pyracetimegg/objects/user.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Jul-06 09:17 pyracetimegg-2.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      443 b- defN 23-Jul-06 09:17 pyracetimegg-2.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 09:17 pyracetimegg-2.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-06 09:17 pyracetimegg-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1485 b- defN 23-Jul-06 09:17 pyracetimegg-2.3.0.dist-info/RECORD
+18 files, 70098 bytes uncompressed, 17866 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: pyracetimegg/objects/race.py
 Comment: 
 
 Filename: pyracetimegg/objects/user.py
 Comment: 
 
-Filename: pyracetimegg-2.2.0.dist-info/LICENSE
+Filename: pyracetimegg-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyracetimegg-2.2.0.dist-info/METADATA
+Filename: pyracetimegg-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: pyracetimegg-2.2.0.dist-info/WHEEL
+Filename: pyracetimegg-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyracetimegg-2.2.0.dist-info/top_level.txt
+Filename: pyracetimegg-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyracetimegg-2.2.0.dist-info/RECORD
+Filename: pyracetimegg-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyracetimegg/api.py

```diff
@@ -44,23 +44,20 @@
                 ValueError("must be set name or discriminator")
 
         json_data = self.__api.fetch_json_from_site(f"user/search?{query}")
         return tuple(self.__api.get_instance(User, tmp) for tmp in json_data["results"])
 
     def search_user_by_term(self, term: str) -> tuple[User]:
         """
-        serch user by name or partial name or (name and discriminator)
+        search user by name or partial name or (name and discriminator)
 
         https://github.com/racetimeGG/racetime-app/wiki/Public-API-endpoints#user-search
 
         Args:
             term (str): term
-            site_url (user, optional):
-                if you want to connect a site other than racetime.gg
-                Defaults to https://racetime.gg/.
         Returns:
             User
         """
         json_data = self.__api.fetch_json_from_site(f"user/search?term={term}")
         return tuple(self.__api.get_instance(User, tmp) for tmp in json_data["results"])
 
     def fetch_all_races(self) -> tuple[Race]:
@@ -82,25 +79,41 @@
         Args:
             user_id (str): you can find at URL
         """
         user: User = self.__api.get_instance(User, user_id)
         user.load("name")
         return user
 
+    def fetch_user_by_url(self, url: str) -> User:
+        try:
+            if re.fullmatch(self.__api.get_url("user", "[0-9a-zA-Z]+"), url):
+                return self.fetch_user(url.split("/")[-1])
+        except Exception:
+            pass
+        raise ValueError(f"wrong url: url={url}")
+
     def fetch_category(self, category_slug: str) -> Category:
         """
         https://github.com/racetimeGG/racetime-app/wiki/Public-API-endpoints#category-detail
 
         Args:
             category_slug (str): you can find at URL
         """
         category: Category = self.__api.get_instance(Category, category_slug)
         category.load("name")
         return category
 
+    def fetch_category_by_url(self, url: str) -> Category:
+        try:
+            if re.fullmatch(self.__api.get_url("[0-9a-z-]+"), url):
+                return self.fetch_category(url.split("/")[-1])
+        except Exception:
+            pass
+        raise ValueError(f"wrong url: url={url}")
+
     @overload
     def fetch_race(self, race_name: str) -> Race:
         """
         https://github.com/racetimeGG/racetime-app/wiki/Public-API-endpoints#race-detail
 
         Args:
             race_name (str): you can find at URL.  it looks like xxx/xxx-xxx-xxx
@@ -142,17 +155,30 @@
             case _:
                 raise ValueError("args shuld be one or two")
 
         race: Race = self.__api.get_instance(Race, name)
         race.load("slug")
         return race
 
+    def fetch_race_by_url(self, url: str) -> Race:
+        try:
+            if re.fullmatch(self.__api.get_url("[0-9a-z-]+/[a-z]+-[a-z]+-[0-9]+"), url):
+                category_slug, race_slug = url.split("/")[-2:]
+                return self.fetch_race(category_slug, race_slug)
+        except Exception:
+            pass
+        raise ValueError(f"wrong url: url={url}")
+
     def fetch_by_url(self, url: str):
-        if re.fullmatch(self.__api.get_url("user", "[0-9a-zA-Z]+"), url):
-            return self.fetch_user(url.split("/")[-1])
-        elif re.fullmatch(self.__api.get_url("[0-9a-z-]+"), url):
-            return self.fetch_category(url.split("/")[-1])
-        elif re.fullmatch(self.__api.get_url("[0-9a-z-]+/[a-z]+-[a-z]+-[0-9]+"), url):
-            category_slug, race_slug = url.split("/")[-2:]
-            return self.fetch_race(category_slug, race_slug)
-        else:
-            raise ValueError(f"wrong url: url={url}")
+        try:
+            return self.fetch_user_by_url(url)
+        except ValueError:
+            pass
+        try:
+            return self.fetch_category_by_url(url)
+        except ValueError:
+            pass
+        try:
+            return self.fetch_race_by_url(url)
+        except ValueError:
+            pass
+        raise ValueError(f"wrong url: url={url}")
```

## pyracetimegg/objects/category.py

```diff
@@ -26,15 +26,15 @@
 
     @property
     def short_name(self) -> str:
         return self._get(currentframe().f_code.co_name)
 
     @property
     def url(self):
-        return f"/{self.slug}"
+        return self._api.get_url(self.slug)
 
     @property
     def data_url(self):
         return f"{self.url}/data"
 
     @property
     def image(self) -> str:
@@ -87,25 +87,25 @@
 
         match tag:
             case "past_race":
                 from pyracetimegg.objects.race import PastRaces
 
                 return {"past_race": PastRaces(self)}
             case "leaderboard":
-                json_data = self._api.fetch_json_from_site(self.slug, "leaderboards/data")
+                json_data = self._api.fetch_json(f"{self.url}/leaderboards/data")
                 leaderboards = dict()
                 for leaderboard in json_data["leaderboards"]:
                     goal_name = leaderboard["goal"]
                     leaderboards[goal_name] = tuple(
                         LeaderBoardParticipant.from_json(self._api, participant)
                         for participant in leaderboard["rankings"]
                     )
                 return {"leaderboard": leaderboards}
             case _:
-                json_data = self._api.fetch_json_from_site(self.data_url)
+                json_data = self._api.fetch_json(self.data_url)
                 _, data = self._format_api_data(json_data)
                 return data
 
     def _format_api_data(self, data_from_api: dict) -> tuple[ID, DATA]:
         from pyracetimegg.objects.race import Race, Goal
         from pyracetimegg.objects.user import User
```

## pyracetimegg/objects/race.py

```diff
@@ -115,31 +115,31 @@
 
     @property
     def category(self) -> Category:
         return self._get(currentframe().f_code.co_name)
 
     @property
     def url(self):
-        return f"/{self.name}"
+        return self._api.get_url(self.name)
 
     @property
     def data_url(self):
         return f"{self.url}/data"
 
     @property
     def websocket_url(self):
-        return f"/ws/race/{self.slug}"
+        return self._api.get_url("ws/race", self.slug)
 
     @property
     def websocket_bot_url(self):
-        return f"/ws/o/bot/{self.slug}"
+        return self._api.get_url("ws/o/bot", self.slug)
 
     @property
     def websocket_oauth_url(self):
-        return f"/ws/o/race/{self.slug}"
+        return self._api.get_url("ws/o/race", self.slug)
 
     @property
     def version(self) -> int:
         return self._get(currentframe().f_code.co_name)
 
     @property
     def info_bot(self) -> str:
@@ -259,15 +259,15 @@
     def entrants_count_inactive(self) -> int:
         return self._get(currentframe().f_code.co_name)
 
     def load_all(self):
         self._fetch_from_api("category")
 
     def _fetch_from_api(self, tag: TAG):
-        json_data = self._api.fetch_json_from_site(self.data_url)
+        json_data = self._api.fetch_json(self.data_url)
         _, data = self._format_api_data(json_data)
         return data
 
     def _format_api_data(self, data_from_api: dict) -> tuple[ID, DATA]:
         from pyracetimegg.objects.user import User
         from pyracetimegg.objects.category import Category
```

## pyracetimegg/objects/user.py

```diff
@@ -39,15 +39,15 @@
         first: int = 0
         second: int = 0
         third: int = 0
         forfeits: int = 0
 
     @property
     def url(self):
-        return f"/user/{self.id}"
+        return self._api.get_url("user", self.id)
 
     @property
     def data_url(self):
         return f"{self.url}/data"
 
     @property
     def name(self) -> str:
@@ -110,15 +110,15 @@
     def _fetch_from_api(self, tag: TAG):
         match tag:
             case "past_race":
                 from pyracetimegg.objects.race import PastRaces
 
                 return {"past_race": PastRaces(self)}
             case _:
-                json_data = self._api.fetch_json_from_site(self.data_url)
+                json_data = self._api.fetch_json(self.data_url)
                 json_data.setdefault("stats", None)
                 _, data = self._format_api_data(json_data)
                 return data
 
     def _format_api_data(self, data_from_api: dict) -> tuple[ID, DATA]:
         output = dict()
         id = data_from_api["id"]
```

## Comparing `pyracetimegg-2.2.0.dist-info/LICENSE` & `pyracetimegg-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyracetimegg-2.2.0.dist-info/RECORD` & `pyracetimegg-2.3.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 pyracetimegg/__init__.py,sha256=Bm5TTElMxFaNqWIyF-amLfuNH_6tH3nUq-H5CRGG8Mk,287
-pyracetimegg/api.py,sha256=ZZEiYMZF7iLr4J4eXX9VrEICfVpN3oXSbR_YDZj3TCk,6324
+pyracetimegg/api.py,sha256=ERlZNUT9nmO8XMgHdwbNgBUu6WOeJdj9QfK8TQMlXBg,6997
 pyracetimegg/category.py,sha256=Lvop4iXqTG2jYsOZEsF3ANs1xHNGjrc6UgTsaGIpyoY,5801
 pyracetimegg/object_mapping.py,sha256=pagsrOJob1t2rC9wbc19-SRYAcQra1yE1n6eugG8_aU,6507
 pyracetimegg/race.py,sha256=o2SK5fi6D12S_rSvz3W_PcscDOwsv_Sv3QX4tKgDpd8,14033
 pyracetimegg/test_api.py,sha256=LLwPFhYZ2H523K3aWSgoiJRZlNWy5GOoXYTzJH2Tam4,1036
 pyracetimegg/throttled_request.py,sha256=CByQaR8LOfDyynpW6c9JGsKLlUH89BixGUSfxWTxqoY,628
 pyracetimegg/user.py,sha256=HgtIYbT3Y2qcYFFQyan_Q_bHKk6N-Pv6DylhHEAGpkI,4548
 pyracetimegg/utils.py,sha256=Ku-g23_LGqpURx30cyyFMxDBNTytsNhX6pXuUxL_3-w,1813
 pyracetimegg/objects/__init__.py,sha256=RQqmuQ0oJqbTdSAFqKj6OVvpLDUOcJzC47LQhixrrSk,292
-pyracetimegg/objects/category.py,sha256=Ff5H0FJWYViYqFOjfftyK4qhiFkrPu8PO7Av3ra6E4I,5519
-pyracetimegg/objects/race.py,sha256=Wtlyuiu2NYFGoDRvuWLlntAyljHCrFiSlKI_pb2Oxh4,15084
-pyracetimegg/objects/user.py,sha256=vzuJeZ2YvO73e-w56u_SHsmwoehkMWlIZ_qUhrzsj5A,4383
-pyracetimegg-2.2.0.dist-info/LICENSE,sha256=mSzFA4DStG8ypPSSk-wJKg__IvKlL_Rw09wvcK7Wg2Y,1086
-pyracetimegg-2.2.0.dist-info/METADATA,sha256=cRdGUdiqR0baD5x2GT4NPyn1EpZApscsly-y_CmDSf8,390
-pyracetimegg-2.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyracetimegg-2.2.0.dist-info/top_level.txt,sha256=tj1v3W4XkbTuL2AJanPYmEUDaCB_XCtYiQmxG0uIMxA,13
-pyracetimegg-2.2.0.dist-info/RECORD,,
+pyracetimegg/objects/category.py,sha256=JFoUIKXJYIAoeazBr2414VDdLOGsg_c7vXZGVU1jT9M,5513
+pyracetimegg/objects/race.py,sha256=44XMqMV0gUy2yXKNhPx21MCmBPJZDrAJEW2MUhP7lKA,15135
+pyracetimegg/objects/user.py,sha256=siPEzsw3LzlDKVouogKG69qDzmqlalCdsYOA6rnZIsw,4389
+pyracetimegg-2.3.0.dist-info/LICENSE,sha256=mSzFA4DStG8ypPSSk-wJKg__IvKlL_Rw09wvcK7Wg2Y,1086
+pyracetimegg-2.3.0.dist-info/METADATA,sha256=eQPyOC8RQAvu90YwYyjQ-Rvj0FY1Fi6DCwZym05GggY,443
+pyracetimegg-2.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyracetimegg-2.3.0.dist-info/top_level.txt,sha256=tj1v3W4XkbTuL2AJanPYmEUDaCB_XCtYiQmxG0uIMxA,13
+pyracetimegg-2.3.0.dist-info/RECORD,,
```

