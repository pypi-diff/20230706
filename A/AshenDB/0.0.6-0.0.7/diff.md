# Comparing `tmp/AshenDB-0.0.6.tar.gz` & `tmp/AshenDB-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshenDB-0.0.6.tar", last modified: Sat Jun 10 01:26:46 2023, max compression
+gzip compressed data, was "AshenDB-0.0.7.tar", last modified: Thu Jul  6 20:59:06 2023, max compression
```

## Comparing `AshenDB-0.0.6.tar` & `AshenDB-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-06-10 01:26:46.893619 AshenDB-0.0.6/
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-06-10 01:26:46.892619 AshenDB-0.0.6/AshenDB.egg-info/
--rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/SOURCES.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/dependency_links.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/entry_points.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/requires.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-06-10 01:26:46.000000 AshenDB-0.0.6/AshenDB.egg-info/top_level.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.6/LICENSE
--rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-06-10 01:26:46.893619 AshenDB-0.0.6/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2080 2023-05-04 20:45:32.000000 AshenDB-0.0.6/README.rst
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-06-10 01:26:46.893619 AshenDB-0.0.6/ashendb/
--rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-05-04 20:43:34.000000 AshenDB-0.0.6/ashendb/__init__.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     6934 2023-05-06 10:06:48.000000 AshenDB-0.0.6/ashendb/client.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)    11191 2023-05-27 22:40:56.000000 AshenDB-0.0.6/ashendb/collection.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     7746 2023-05-04 20:46:23.000000 AshenDB-0.0.6/ashendb/database.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1257 2023-05-03 00:01:33.000000 AshenDB-0.0.6/ashendb/document.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.6/ashendb/exception.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)    10541 2023-06-10 01:06:02.000000 AshenDB-0.0.6/ashendb/helper.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-06-10 01:22:41.000000 AshenDB-0.0.6/pyproject.toml
--rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-06-10 01:26:46.893619 AshenDB-0.0.6/setup.cfg
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-07-06 20:59:06.431959 AshenDB-0.0.7/
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-07-06 20:59:06.430959 AshenDB-0.0.7/AshenDB.egg-info/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-07-06 20:59:06.000000 AshenDB-0.0.7/AshenDB.egg-info/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-07-06 20:59:06.000000 AshenDB-0.0.7/AshenDB.egg-info/SOURCES.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-07-06 20:59:06.000000 AshenDB-0.0.7/AshenDB.egg-info/dependency_links.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-07-06 20:59:06.000000 AshenDB-0.0.7/AshenDB.egg-info/entry_points.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-07-06 20:59:06.000000 AshenDB-0.0.7/AshenDB.egg-info/requires.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-07-06 20:59:06.000000 AshenDB-0.0.7/AshenDB.egg-info/top_level.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.7/LICENSE
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-07-06 20:59:06.431959 AshenDB-0.0.7/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     2080 2023-05-04 20:45:32.000000 AshenDB-0.0.7/README.rst
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-07-06 20:59:06.431959 AshenDB-0.0.7/ashendb/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-05-04 20:43:34.000000 AshenDB-0.0.7/ashendb/__init__.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7283 2023-06-11 06:30:08.000000 AshenDB-0.0.7/ashendb/client.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)    11371 2023-06-22 03:28:49.000000 AshenDB-0.0.7/ashendb/collection.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7746 2023-05-04 20:46:23.000000 AshenDB-0.0.7/ashendb/database.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1257 2023-05-03 00:01:33.000000 AshenDB-0.0.7/ashendb/document.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      176 2023-06-11 06:30:01.000000 AshenDB-0.0.7/ashendb/exception.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)    12245 2023-06-13 11:14:44.000000 AshenDB-0.0.7/ashendb/helper.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-07-06 20:59:01.000000 AshenDB-0.0.7/pyproject.toml
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-07-06 20:59:06.431959 AshenDB-0.0.7/setup.cfg
```

### Comparing `AshenDB-0.0.6/AshenDB.egg-info/PKG-INFO` & `AshenDB-0.0.7/AshenDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.6
+Version: 0.0.7
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.6/LICENSE` & `AshenDB-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.6/PKG-INFO` & `AshenDB-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.6
+Version: 0.0.7
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.6/README.rst` & `AshenDB-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.6/ashendb/__init__.py` & `AshenDB-0.0.7/ashendb/__init__.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.6/ashendb/client.py` & `AshenDB-0.0.7/ashendb/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,41 +6,47 @@
 
 
 # Client Class
 class AshenDB:
     """
     Entry point for AshenDB. This class is used to create, get, and delete databases.
 
+    Args:
+        cluster: The name of the cluster to use. Defaults to "ashendb".
     """
 
-    base: str = ".ashendb/"
+    def __init__(self, cluster: str) -> None:
+        if not cluster.isalnum():
+            raise InvalidClusterName(
+                "Cluster name must be alphanumeric and cannot contain spaces."
+            )
+        self.cluster = ".ashendb/" + cluster + "/"
 
-    @classmethod
-    async def get_db(cls, db_name: str) -> Database:
+    async def get_db(self, db_name: str) -> Database:
         """Get a single database from database name.
 
         Args:
             db_name: The name of the database.
 
         Raises:
             NotFound: If the database does not exist.
 
         Example:
             >>> db = await AshenDB.get_db("test")
             >>> db
             <Database: test>
         """
         db_name = str(db_name)
-        for name in await aios.listdir(cls.base):
+        for name in await aios.listdir(self.cluster):
             if name == db_name:
-                return Database(cls.base + name + "/")
+                return Database(self.cluster + name + "/")
         raise NotFound(f"Database '{db_name}' does not exist.")
 
     @classmethod
-    async def get_dbs(cls, db_names: list[str] = None) -> list[Database]:
+    async def get_dbs(self, db_names: list[str] = None) -> list[Database]:
         """Get multiple databases from list of database names.
 
         If no list is provided or the list is empty, all databases are returned.
 
         Args:
             db_names: The names of the databases.
 
@@ -55,26 +61,26 @@
 
             >>> dbs = await AshenDB.get_dbs()
             >>> dbs
             [<Database: test>, <Database: test2>, <Database: test3>]
         """
         final = []
         if db_names is None or len(db_names) == 0:
-            for name in await aios.listdir(cls.base):
-                final.append(Database(cls.base + name + "/"))
+            for name in await aios.listdir(self.cluster):
+                final.append(Database(self.cluster + name + "/"))
         elif isinstance(db_names, list) and len(db_names) > 0:
             for name in db_names:
-                final.append(await cls.get_db(name))
+                final.append(await self.get_db(name))
         else:
             raise InvalidArgumentType(f"Expected list, got {type(db_names)}.")
 
         return final
 
     @classmethod
-    async def iterate_dbs(cls, db_names: list[str]) -> Generator[Database, None, None]:
+    async def iterate_dbs(self, db_names: list[str]) -> Generator[Database, None, None]:
         """Iterate over multiple databases from list of database names.
 
         Args:
             db_names: The names of the databases.
 
         Raises:
             InvalidArgumentType: If the argument is not a list.
@@ -87,47 +93,47 @@
             <Database: test2>
 
             >>> dbs = [db async for db in AshenDB.iterate_dbs()]
             >>> dbs
             [<Database: test>, <Database: test2>, <Database: test3>]
         """
         if db_names is None or len(db_names) == 0:
-            for name in await aios.listdir(cls.base):
-                yield Database(cls.base + name + "/")
+            for name in await aios.listdir(self.cluster):
+                yield Database(self.cluster + name + "/")
         elif isinstance(db_names, list) and len(db_names) > 0:
             for name in db_names:
-                yield await cls.get_db(name)
+                yield await self.get_db(name)
         else:
             raise InvalidArgumentType(f"Expected list, got {type(db_names)}.")
 
     @classmethod
-    async def create_db(cls, db_name: str or int) -> Database:
+    async def create_db(self, db_name: str or int) -> Database:
         """Creates a single database.
 
         Args:
             db_name: The name of the database.
 
         Raises:
             AlreadyExists: If the database already exists.
 
         Example:
             >>> db = await AshenDB.create_db("test")
             >>> db
             <Database: test>
         """
         db_name = str(db_name)
-        path = cls.base + db_name
+        path = self.cluster + db_name
         if await aios.path.exists(path):
             raise AlreadyExists(f"Database '{db_name}' already exists.")
         else:
             await aios.mkdir(path)
             return Database(path + "/")
 
     @classmethod
-    async def create_dbs(cls, db_names: list[str]) -> list[Database]:
+    async def create_dbs(self, db_names: list[str]) -> list[Database]:
         """Create multiple databases.
 
         Args:
             db_names: The names of the databases.
 
         Raises:
             AlreadyExists: If one of the databases already exists.
@@ -139,21 +145,21 @@
             [<Database: test>, <Database: test2>]
         """
         final = []
         if db_names is None or len(db_names) == 0 or not isinstance(db_names, list):
             raise InvalidArgumentType(f"Expected list, got {type(db_names)}.")
 
         for name in db_names:
-            final.append(await cls.create_one(name))
+            final.append(await self.create_one(name))
 
         return final
 
     @classmethod
     async def iterate_create_dbs(
-        cls, db_names: list[str]
+        self, db_names: list[str]
     ) -> Generator[Database, None, None]:
         """Iterate over multiple databases from list of database names.
 
         Args:
             db_names: The names of the databases.
 
         Raises:
@@ -169,52 +175,52 @@
             >>> dbs = [db async for db in AshenDB.iterate_create_dbs()]
             >>> dbs
             [<Database: test>, <Database: test2>, <Database: test3>]
         """
         if db_names is None or len(db_names) == 0 or not isinstance(db_names, list):
             raise InvalidArgumentType(f"Expected list, got {type(db_names)}.")
         for name in db_names:
-            yield await cls.create_one(name)
+            yield await self.create_one(name)
 
     @classmethod
-    async def del_db(cls, db_name: str) -> None:
+    async def del_db(self, db_name: str) -> None:
         """Delete a single database.
 
         Args:
             db_name: The name of the database.
 
         Raises:
             NotFound: If the database does not exist.
 
         Example:
             >>> await AshenDB.delete_db("test")
 
         """
-        path = cls.base + db_name
+        path = self.cluster + db_name
         if await aios.path.exists(path):
             await aios.removedirs(path)
             return
         else:
             raise Exception(f"Database '{db_name}' does not exist.")
 
     @classmethod
-    async def del_dbs(cls, db_names: list[str]) -> None:
+    async def del_dbs(self, db_names: list[str]) -> None:
         """Delete multiple databases.
 
         If no list is provided or the list is empty, all databases are deleted.
 
         Args:
             db_names: The names of the databases.
 
         Raises:
             NotFound: If one of the databases does not exist.
 
         Example:
             >>> await AshenDB.delete_dbs(["test", "test2"])
         """
         if db_names is None:
-            for name in await aios.listdir(cls.base):
-                await cls.delete_db(name)
+            for name in await aios.listdir(self.cluster):
+                await self.delete_db(name)
             return
         for name in db_names:
-            await cls.delete_db(name)
+            await self.delete_db(name)
         return
```

### Comparing `AshenDB-0.0.6/ashendb/collection.py` & `AshenDB-0.0.7/ashendb/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,16 @@
                 raise NotFound("No document found")
             doc = Document(path)
             await doc.__ainit__()
             return doc
         except NotFound:
             for file in await aios.scandir(self.path):
                 async with aiofiles.open(file.path, "r") as f:
-                    data = json.loads(await f.read())
-                    if await match_data(data, query):
+                    document = json.loads(await f.read())
+                    if await match_data(document, query):
                         doc = Document(file.path)
                         await doc.__ainit__()
                         return doc
             raise NotFound("No document found")
         except Exception as e:
             print(e)
             raise ValueError("Either id or query must be provided")
@@ -108,15 +108,14 @@
         You can pass either a list of ids or a query. If both are passed then the ids will be used.
 
         Args:
             ids: The ids of the documents.
             query: A query to match the documents.
 
         Raises:
-            ValueError: If neither ids nor query is passed.
             NotFound: If no documents are found.
 
         Example:
             >>> docs = await coll.get_docs([1, 2, 3])
             >>> docs
             [<Document: 1>, <Document: 2>, <Document: 3>]
 
@@ -137,15 +136,21 @@
                         doc = Document(file.path)
                         await doc.__ainit__()
                         final.append(doc)
             if len(final) == 0 or len(final[0]) == 0:
                 raise NotFound("No documents found")
             return final
         else:
-            raise ValueError("Either ids or query must be provided")
+            for file in await aios.scandir(self.path):
+                doc = Document(file.path)
+                await doc.__ainit__()
+                final.append(doc)
+            if len(final) == 0 or len(final[0]) == 0:
+                raise NotFound("No documents found")
+            return final
 
     async def iterate_docs(
         self, *, ids: list[str or int] = None, query: dict = None
     ) -> Generator[Document, None, None]:
         """Iterate over multiple documents.
 
         You can pass either a list of ids or a query. If both are passed then the ids will be used.
```

### Comparing `AshenDB-0.0.6/ashendb/database.py` & `AshenDB-0.0.7/ashendb/database.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.6/ashendb/document.py` & `AshenDB-0.0.7/ashendb/document.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.6/pyproject.toml` & `AshenDB-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AshenDB"
-version = "0.0.6"
+version = "0.0.7"
 description = "Another stupid library for using json as Database"
 readme = "README.rst"
 authors = [{name = "Abdullah Al Muaz", email = "abdullahalmuaz15@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: MIT License",
```

