# Comparing `tmp/easy_db-0.9.8.tar.gz` & `tmp/easy_db-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easy_db-0.9.8.tar", last modified: Tue Sep 14 23:25:17 2021, max compression
+gzip compressed data, was "dist\easy_db-0.9.9.tar", last modified: Fri Dec 31 15:28:46 2021, max compression
```

## Comparing `easy_db-0.9.8.tar` & `easy_db-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-09-14 23:25:17.000000 easy_db-0.9.8/
--rw-rw-rw-   0        0        0     1090 2019-02-09 22:27:10.000000 easy_db-0.9.8/LICENSE.txt
--rw-rw-rw-   0        0        0       40 2019-02-11 04:19:31.000000 easy_db-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6191 2021-09-14 23:25:17.000000 easy_db-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     4269 2021-06-26 02:19:48.000000 easy_db-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2021-09-14 23:25:17.000000 easy_db-0.9.8/easy_db/
--rw-rw-rw-   0        0        0       32 2019-10-22 02:26:26.000000 easy_db-0.9.8/easy_db/__init__.py
--rw-rw-rw-   0        0        0    39389 2021-09-14 23:24:50.000000 easy_db-0.9.8/easy_db/database.py
--rw-rw-rw-   0        0        0     8819 2021-09-14 23:24:50.000000 easy_db-0.9.8/easy_db/util.py
-drwxrwxrwx   0        0        0        0 2021-09-14 23:25:17.000000 easy_db-0.9.8/easy_db.egg-info/
--rw-rw-rw-   0        0        0     6191 2021-09-14 23:25:15.000000 easy_db-0.9.8/easy_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2021-09-14 23:25:15.000000 easy_db-0.9.8/easy_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-14 23:25:15.000000 easy_db-0.9.8/easy_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2021-09-14 23:25:15.000000 easy_db-0.9.8/easy_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-09-14 23:25:15.000000 easy_db-0.9.8/easy_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-09-14 23:25:17.000000 easy_db-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1042 2021-09-14 23:24:50.000000 easy_db-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-31 15:28:46.000000 easy_db-0.9.9/
+-rw-rw-rw-   0        0        0     1090 2019-02-09 22:27:10.000000 easy_db-0.9.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       40 2019-02-11 04:19:31.000000 easy_db-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5009 2021-12-31 15:28:46.000000 easy_db-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4269 2021-06-26 02:19:48.000000 easy_db-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2021-12-31 15:28:46.000000 easy_db-0.9.9/easy_db/
+-rw-rw-rw-   0        0        0       32 2019-10-22 02:26:26.000000 easy_db-0.9.9/easy_db/__init__.py
+-rw-rw-rw-   0        0        0    40136 2021-12-31 15:21:00.000000 easy_db-0.9.9/easy_db/database.py
+-rw-rw-rw-   0        0        0     9008 2021-12-31 15:21:00.000000 easy_db-0.9.9/easy_db/util.py
+drwxrwxrwx   0        0        0        0 2021-12-31 15:28:46.000000 easy_db-0.9.9/easy_db.egg-info/
+-rw-rw-rw-   0        0        0     5009 2021-12-31 15:28:46.000000 easy_db-0.9.9/easy_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2021-12-31 15:28:46.000000 easy_db-0.9.9/easy_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-31 15:28:46.000000 easy_db-0.9.9/easy_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2021-12-31 15:28:46.000000 easy_db-0.9.9/easy_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-12-31 15:28:46.000000 easy_db-0.9.9/easy_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2021-12-31 15:28:46.000000 easy_db-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2021-12-31 15:21:00.000000 easy_db-0.9.9/setup.py
```

### Comparing `easy_db-0.9.8/LICENSE.txt` & `easy_db-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_db-0.9.8/README.md` & `easy_db-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `easy_db-0.9.8/easy_db/database.py` & `easy_db-0.9.9/easy_db/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,35 @@
             elif '.mdb' in self.db_location_str and os.path.isfile(self.db_location_str.replace('.mdb', '.accdb')):
                 error_str = '\n  ".mdb" file extension specified, but this file was not found.\n  An ".accdb" Access file was found instead.\n  Please change the specified file extension to use the existing database.\n'
             else:
                 error_str = '\n  Could not locate the specified Access database.\n'
             raise FileNotFoundError(error_str)
 
         absolute_path = os.path.abspath(self.db_location_str)  # NEED AN ABSOLUTE PATH FOR PYODBC!!!
-        conn = pyodbc.connect(
-            r"Driver={Microsoft Access Driver (*.mdb, *.accdb)};" +
-            r'Dbq=' + absolute_path + ';')
+
+        # try to connect a few times if first pass fails
+        # may occur if the Access locking/unlocking process is taking longer than usual
+        conn, tries = None, 0
+        while conn is None:
+            try:
+                tries += 1
+                conn = pyodbc.connect(
+                    r'Driver={Microsoft Access Driver (*.mdb, *.accdb)};' +
+                    r'Dbq=' + absolute_path + ';')
+            except pyodbc.Error:
+                time.sleep(0.7)  # time delay so Access can hopefully get unlocked
+            if tries > 5:
+                break
+
+        # now try again one more time to get the pyodbc error message/traceback
+        if conn is None:
+            conn = pyodbc.connect(
+                r'Driver={Microsoft Access Driver (*.mdb, *.accdb)};' +
+                r'Dbq=' + absolute_path + ';')
+
         if also_cursor:
             return conn, conn.cursor()
         else:
             return conn
 
 
     def _connection_sql_server(self, also_cursor: bool=False):
@@ -197,15 +215,18 @@
         Return list of dicts for rows with column names as keys.
         '''
         if fresh:
             self._clear_pull_cache(tablename)  # clear cache for this table
             return self.pull(tablename, columns, progress_handler=progress_handler)
 
         else:
-            requested_data_key = f'{tablename}_' + '_'.join(sorted(columns))  # key string for caching db pulls in dict
+            if columns == 'all':
+                requested_data_key = tablename
+            else:
+                requested_data_key = f'{tablename}_' + '_'.join(sorted(columns))  # key string for caching db pulls in dict
 
             try:
                 return self._pull_cache[requested_data_key]
 
             except KeyError:
                 # check for questionable table/column names
                 for name in [tablename] + list(columns):
@@ -465,15 +486,14 @@
             else:
                 progressbar = True
 
         if isinstance(data, dict):  # handle case of single row append by converting it to a list
             data = [data]
 
         if clean_column_names:
-            print('Cleaning column names in data to be appended.')
             for key in list(data[0].keys()):
                 for row in data:
                     row[util.clean_column_name(key)] = row.pop(key)
 
         if tablename not in self.table_names() and create_table_if_needed:
             self.create_table(tablename, {key: type(value).__name__ for key, value in data[0].items()})
         elif tablename not in self.table_names() and not create_table_if_needed:
@@ -490,27 +510,27 @@
                 data = [{col: d[col] for col in columns} for d in data]
             except KeyError:
                 print(f'Error!  Table {tablename} columns do not match the keys of the data to be appended.')
                 print('Try setting robust=True and/or /n  set clean_column_names=True to replace " " and "/" with underscores in data keys.')
                 return
 
         if self.db_type == 'SQLITE':
-            insert_sql = f"INSERT INTO '{tablename}' ({','.join(columns)}) VALUES "
+            insert_sql = f"INSERT INTO '{tablename}' ({','.join([f'[{col}]' for col in columns])}) VALUES "
         else:
             insert_sql = f"INSERT INTO [{tablename}] ({', '.join(columns)}) VALUES "
         insert_many_sql = insert_sql + f"({', '.join(['?' for _ in range(len(columns))])});"
 
         # Check for potential duplicate (key) entries if Access to avoid pyodbc error and crash of whole append.
         if self.db_type == 'ACCESS' and robust:
             dup_rows = self._check_potential_duplicates(tablename, data)
             key_cols = self.key_columns(tablename)
             if dup_rows:
                 non_dup_data = [d for d in data if tuple(d[key] for key in key_cols) not in dup_rows]
                 skip_count = len(data) - len(non_dup_data)
-                print(f"\n{skip_count} row{'s' if skip_count > 1 else ''} {'were' if skip_count > 1 else 'was'} skipped in .append due to being primary key duplicates\n  of rows that already exist in table: {tablename}")
+                print(f"\n{skip_count} row{'s were' if skip_count > 1 else ' was'} skipped in .append due to being primary key duplicates\n  of rows that already exist in table: {tablename}")
                 if not non_dup_data:
                     print('No remaining data to append.')
                     return
                 print(f'The remaining {len(non_dup_data)} rows are still being appended.\n')
                 data = non_dup_data
 
         is_sqlite = True if self.db_type == 'SQLITE' else False
```

### Comparing `easy_db-0.9.8/easy_db/util.py` & `easy_db-0.9.9/easy_db/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Return dict of Python types as keys and appropriate
     database types as values based on the provided db_type.
     '''
     if db_type == 'ACCESS':
         return {float: 'double',
                     'float': 'double',
                     'double': 'double',
+                    'real': 'double',
                     'float64': 'double',
                     'numpy.float64': 'double',
                     int: 'integer',
                     'int': 'integer',
                     'integer': 'integer',
                     str: 'varchar(255)',
                     'str': 'varchar(255)',
@@ -129,29 +130,33 @@
             return False
     if 'DROP' in name.upper():
         print(f'ERROR!!!  Prohibited characters detected in:\n  {name}')
         return False
     return True
 
 
+column_name_changes = set()
 def clean_column_name(col_name: str) -> str:
     '''
     Used to ensure column names do not have spaces or forward slashes
     Replace each bad character with an underscore.
     '''
     original_col_name = col_name
     changed = False
     if ' ' in col_name:
         col_name = col_name.replace(' ', '_')
         changed = True
     if '/' in col_name:
         col_name = col_name.replace('/', '_')
         changed = True
     if changed:
-        print(f'Column Name {original_col_name} changed to {col_name}')
+        change = f'Column Name {original_col_name} changed to {col_name}'
+        if change not in column_name_changes:
+            column_name_changes.add(change)
+            print(change)
     return col_name
 
 
 def clean_data(data, columns_and_types, db_type) -> List[dict]:
     '''
     Best effort to clean list of dicts representing database table rows to handle mismatched types,
     null values, and missing columns.
```

### Comparing `easy_db-0.9.8/setup.py` & `easy_db-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='easy_db',
-    version='0.9.8',
+    version='0.9.9',
     packages=['easy_db'],
     license='MIT',
     author='Zach Bateman',
     description='Easy Python database interaction',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zachbateman/easy_db.git',
-    download_url='https://github.com/zachbateman/easy_db/archive/v_0.9.8.tar.gz',
+    download_url='https://github.com/zachbateman/easy_db/archive/v_0.9.9.tar.gz',
     keywords=['DATABASE', 'SIMPLE', 'EASY'],
     install_requires=['pyodbc', 'tqdm'],
     classifiers=['Development Status :: 4 - Beta',
                    'License :: OSI Approved :: MIT License',
                    'Programming Language :: Python :: 3',
                    'Programming Language :: Python :: 3.7',
                    'Programming Language :: Python :: 3.8',
```

