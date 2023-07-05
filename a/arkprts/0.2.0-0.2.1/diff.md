# Comparing `tmp/arkprts-0.2.0.tar.gz` & `tmp/arkprts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.2.0.tar", last modified: Tue Jul  4 21:46:15 2023, max compression
+gzip compressed data, was "arkprts-0.2.1.tar", last modified: Wed Jul  5 00:01:55 2023, max compression
```

## Comparing `arkprts-0.2.0.tar` & `arkprts-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.843008 arkprts-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 21:46:04.000000 arkprts-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-04 21:46:15.843008 arkprts-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-04 21:46:04.000000 arkprts-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.839007 arkprts-0.2.0/arkprts/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/gamedata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.839007 arkprts-0.2.0/arkprts/models/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/models/social.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:04.000000 arkprts-0.2.0/arkprts/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.839007 arkprts-0.2.0/arkprts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 21:46:15.000000 arkprts-0.2.0/arkprts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-04 21:46:04.000000 arkprts-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:46:15.843008 arkprts-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-04 21:46:04.000000 arkprts-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:46:15.843008 arkprts-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-04 21:46:04.000000 arkprts-0.2.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 21:46:04.000000 arkprts-0.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 21:46:04.000000 arkprts-0.2.0/tests/test_gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:01:55.855189 arkprts-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 00:01:44.000000 arkprts-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-05 00:01:55.855189 arkprts-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-05 00:01:44.000000 arkprts-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:01:55.855189 arkprts-0.2.1/arkprts/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:01:55.855189 arkprts-0.2.1/arkprts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/models/social.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:01:44.000000 arkprts-0.2.1/arkprts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:01:55.855189 arkprts-0.2.1/arkprts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-05 00:01:55.000000 arkprts-0.2.1/arkprts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-05 00:01:55.000000 arkprts-0.2.1/arkprts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:01:55.000000 arkprts-0.2.1/arkprts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 00:01:55.000000 arkprts-0.2.1/arkprts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 00:01:55.000000 arkprts-0.2.1/arkprts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-05 00:01:44.000000 arkprts-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:01:55.855189 arkprts-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 00:01:44.000000 arkprts-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:01:55.855189 arkprts-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-05 00:01:44.000000 arkprts-0.2.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-05 00:01:44.000000 arkprts-0.2.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-05 00:01:44.000000 arkprts-0.2.1/tests/test_gamedata.py
```

### Comparing `arkprts-0.2.0/LICENSE` & `arkprts-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/PKG-INFO` & `arkprts-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.2.0
+Version: 0.2.1
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: rsa
```

### Comparing `arkprts-0.2.0/README.md` & `arkprts-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts/__main__.py` & `arkprts-0.2.1/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts/auth.py` & `arkprts-0.2.1/arkprts/auth.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts/automation.py` & `arkprts-0.2.1/arkprts/automation.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts/client.py` & `arkprts-0.2.1/arkprts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """Arknights client for accessing private data."""
 
     def _assert_private(self) -> None:
         """Assert that the client is not public."""
         if not isinstance(self.auth, authn.Auth):
             raise RuntimeError("This client can only access public data.")  # noqa: TRY004  # isn't a type check
 
-        if not self.network.default_server:
+        if not self.auth.server:
             raise RuntimeError("Missing a default server for a private client.")
 
     async def get_raw_data(self) -> typing.Any:
         """Get user data."""
         self._assert_private()
 
         return await self.request("account/syncData", json={"platform": 1})
```

### Comparing `arkprts-0.2.0/arkprts/errors.py` & `arkprts-0.2.1/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts/gamedata.py` & `arkprts-0.2.1/arkprts/gamedata.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts/models/base.py` & `arkprts-0.2.1/arkprts/models/base.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts/models/data.py` & `arkprts-0.2.1/arkprts/models/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     """Operator ID."""
     favor_point: int = pydantic.Field(alias="favorPoint")
     """Operator trust points."""
     potential_rank: int = pydantic.Field(alias="potentialRank")
     """Operator potential. Starts at 0."""
     main_skill_lvl: int = pydantic.Field(alias="mainSkillLvl")
     """Operator skill level."""
-    skin: str
+    skin: str = pydantic.Field(validation_alias=pydantic.AliasChoices("skinId", "skin"))
     """Operator skin ID."""
     level: int
     """Operator level."""
     exp: int
     """Operator experience."""
     evolve_phase: int = pydantic.Field(alias="evolvePhase")
     """Elite phase."""
@@ -297,15 +297,15 @@
 
     ts: typing.Optional[base.ArknightsTimestamp]
     """When the consumable expires."""
     count: int
     """Amount of consumables."""
 
 
-class User(base.BaseModel, extra="allow"):
+class User(base.BaseModel, extra="ignore"):
     """User sync data. Not fully modeled."""
 
     status: Status
     """General user data."""
     troop: Troops
     """Operator data."""
     skin: Skins
```

### Comparing `arkprts-0.2.0/arkprts/models/social.py` & `arkprts-0.2.1/arkprts/models/social.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/arkprts.egg-info/PKG-INFO` & `arkprts-0.2.1/arkprts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.2.0
+Version: 0.2.1
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: rsa
```

### Comparing `arkprts-0.2.0/pyproject.toml` & `arkprts-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "arkprts"
 requires-python = ">=3.9"
-version = "0.2.0"
+version = "0.2.1"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
```

### Comparing `arkprts-0.2.0/setup.py` & `arkprts-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.2.0",
+    version="0.2.1",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic==2.*"],
     extras_require={"all": ["rsa", "pycryptodome"], "rsa": ["rsa"], "aes": ["pycryptodome"]},
```

### Comparing `arkprts-0.2.0/tests/test_auth.py` & `arkprts-0.2.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.0/tests/test_client.py` & `arkprts-0.2.1/tests/test_client.py`

 * *Files identical despite different names*

