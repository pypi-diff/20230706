# Comparing `tmp/lib310_lite-0.0.9.tar.gz` & `tmp/lib310_lite-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.9.tar", max compression
+gzip compressed data, was "lib310_lite-0.1.0.dev1.tar", max compression
```

## Comparing `lib310_lite-0.0.9.tar` & `lib310_lite-0.1.0.dev1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.9/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.9/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.0.9/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.9/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.9/lib310_lite/fucntion.py
--rw-r--r--   0        0        0    12102 2023-05-12 14:37:15.279167 lib310_lite-0.0.9/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0     1528 2023-05-12 10:35:08.523571 lib310_lite-0.0.9/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2818 2023-05-12 10:35:08.531397 lib310_lite-0.0.9/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      799 2023-05-12 12:40:20.982239 lib310_lite-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 lib310_lite-0.0.9/setup.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 lib310_lite-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      289 2023-07-05 13:20:23.360374 lib310_lite-0.1.0.dev1/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev1/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev1/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev1/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.1.0.dev1/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0    11378 2023-07-05 14:19:15.712417 lib310_lite-0.1.0.dev1/lib310_lite/laser/laser.py
+-rw-r--r--   0        0        0    12905 2023-05-31 18:31:27.737763 lib310_lite-0.1.0.dev1/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0     1528 2023-05-12 10:35:08.523571 lib310_lite-0.1.0.dev1/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2818 2023-05-12 10:35:08.531397 lib310_lite-0.1.0.dev1/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      828 2023-07-06 08:28:45.013372 lib310_lite-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev1/setup.py
+-rw-r--r--   0        0        0      934 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev1/PKG-INFO
```

### Comparing `lib310_lite-0.0.9/lib310_lite/bigquery/client.py` & `lib310_lite-0.1.0.dev1/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.9/lib310_lite/bigquery/constants.py` & `lib310_lite-0.1.0.dev1/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.9/lib310_lite/mldl/mldl.py` & `lib310_lite-0.1.0.dev1/lib310_lite/mldl/mldl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 import random
 import time
+import asyncio
 import pandas as pd
 from threading import Thread, Event
 from queue import Queue
 import concurrent.futures
 from bounded_pool_executor import BoundedThreadPoolExecutor
 import dask.dataframe as dd
 from ..bigquery.client import Client as BigQueryClient
 from ..bigquery.constants import FileFormat
 import hashlib
 
 # PGSQL
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
-from sqlalchemy.pool import NullPool
 from .models.SeqLangModel import SeqLangModel, SeqLang300Model, SeqLangT10Model, SeqLang300T10Model
 from .models.InteractionModel import InteractionModel, Interaction300Model, InteractionT10Model, Interaction300T10Model
 
 import time
 
 
 class MLDL:
@@ -26,166 +26,189 @@
     __TRAIN = 'TRAIN'
     __TEST = 'TEST'
     __VAL = 'VAL'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
     __PARTS = {__INTERACTION: 1}
 
-    def __init__(self, db_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
+    def __init__(self, db_url: str,
+                 cache_size: int = 50,
+                 num_threads: int = 10,
+                 random_seed: int = time.time()
+                 ):
         random.seed(random_seed)
-        self.engine = create_engine(db_url, pool_size=3 * num_threads, max_overflow=6 * num_threads, isolation_level='AUTOCOMMIT')
+        self.engine = create_engine(db_url, pool_size=3 * num_threads, max_overflow=6 * num_threads, pool_recycle=5*60, isolation_level="AUTOCOMMIT")
         self.Session = sessionmaker(bind=self.engine)
 
         self.bq_client = BigQueryClient()
 
         # this is the pool of samples row_id
-        self.sample_cache = []
+        self.pool = []
         # this is the maximum number of requests we fetch sooner from the database
         self.max_queue_size = cache_size
         # this is the number of threads we use to fetch data from the database
         self.num_threads = num_threads
         # this is the key that we know MLDL requests are same or not if it changes we need to fetch new data
         self.queue_key = None
         # this is the key shows that pool is still valid or not
         self.pool_key = None
-        # this is the queue that we use to cache requests and put it in the queue
-        self.queue = Queue(self.max_queue_size)
+        # this is the queue that cache the responses
+        self.responses_queue = Queue(self.max_queue_size)
+        # this is the queue that cache index of requests
+        self.requests_queue = Queue(self.max_queue_size * 2)
         # this is the thread that we use to fill the queue
         self.filler_thread = None
         # this is the event that we use to kill the filler thread
         self.kill_event = Event()
 
-    def get_batch(self, num: int, max_length: int = 300, min_num_feature: int = 0, stage: str = __TRAIN, interactions_count: int = 0 ,parts: dict = None, query: str = None):
-        """
-        Get a batch of data from the database with regard to the length of the sequence and the number of features
-        It also start the background thread to fill the caches and queue
-        :param num: number of samples
-        :param max_length: maximum length of the sequence
-        :param min_num_feature: minimum number of features
-        :param stage: TRAIN or TEST
-        :param parts: the parts of the data that we want to fetch
-        :param query: the query that we want to fetch If it is not None, it will ignore the other parameters except num and parts
-        :return: a pandas dataframe
-        """
-        stage = stage.upper()
-
-        if interactions_count < 0:
-            interactions_count = 0
-
-        qk = f'{num}_{max_length}_{min_num_feature}_{stage}'
-        hq = None
-        if query is not None:
-            hq = hashlib.sha1(query.encode('utf-8')).hexdigest()
-            qk = f'{num}_{hq}'
+        # Create an event loop
+        loop = asyncio.get_event_loop()
 
-        if parts is None:
-            parts = MLDL.__PARTS
-
-        hit = self.queue_key == qk
-        if hit:
-            # HIT
-            return pd.DataFrame(self.queue.get())
-        # MISS
+        # this is the thread that we use to fill request queue
+        self.fill_request_thread = None
+        # this kill fill requests thread
+        self.kill_fill_requests_event = Event()
+
+        # pool values
+        self.max_length = 10000000
+        self.token_size = -1
+        self.stage = self.__TRAIN
+        self.interactions_count = -1
+        self.query = None
+
+    def create_pool(self, max_length: int = 300, min_num_feature: int = 10, stage: str = __TRAIN, interactions_count: int = -1, query: str = None):
+        self.max_length = max_length
+        self.token_size = min_num_feature
+        self.stage = stage.upper()
+        self.interactions_count = interactions_count
+        self.query = query
 
         if query is not None and self.pool_key != query:
-            self.pool_key = hq
+            self.pool_key = hashlib.sha1(query.encode('utf-8')).hexdigest()
             res = self.bq_client.cache_query(
                 query=query,
-                name=hq,
+                name=self.pool_key,
                 destination_format=FileFormat.CSV
             )
             ddf = dd.read_csv(res['uri'])
             df = ddf.compute()
-            self.sample_cache = df['row_id'].tolist()
+            self.pool = df['row_id'].tolist()
 
-        elif len(self.sample_cache) == 0 or not self.pool_key or self.pool_key != f'{max_length}_{min_num_feature}_{stage}_{interactions_count}':
+        elif len(self.pool) == 0 or not self.pool_key or self.pool_key != f'{max_length}_{min_num_feature}_{stage}_{interactions_count}':
             table = '1_uniprot.pg_lang5'
             self.pool_key = f'{max_length}_{min_num_feature}_{stage}_{interactions_count}'
             tmp_query = f"SELECT row_id FROM `{table}` WHERE len <= {max_length} and token_size >= {min_num_feature} and stage = '{stage}'"
             if interactions_count > 0:
                 tmp_query += f" and interactions_count >= {interactions_count}"
             res = self.bq_client.cache_query(
                 query=tmp_query,
                 name=f'{max_length}_{min_num_feature}_{stage}',
                 destination_format=FileFormat.CSV
             )
             # print(res)
             ddf = dd.read_csv(res['uri'])
             df = ddf.compute()
-            self.sample_cache = df['row_id'].tolist()
-            # print('HERE')
+            self.pool = df['row_id'].tolist()
+        # shuffle the pool to make sure that we have a random pool
+        random.shuffle(self.pool)
+        return self.pool
+
+    def get_batch(self, num: int, parts: dict = None):
+        """
+        Get a batch of data from the database with regard to the length of the sequence and the number of features
+        It also start the background thread to fill the caches and queue
+        :param num: number of samples
+        :param parts: the parts of the data that we want to fetch
+        :return: a pandas dataframe
+        """
+
+        qk = f'{num}_{self.max_length}_{self.token_size}_{self.stage}'
+        if self.query is not None:
+            self.max_length = 10000000
+            self.token_size = -1
+            self.stage = self.__TRAIN
+            self.interactions_count = -1
+            hq = hashlib.sha1(self.query.encode('utf-8')).hexdigest()
+            qk = f'{num}_{hq}'
+
+        if parts is None:
+            parts = MLDL.__PARTS
 
+        # we check queue key to see if the query is the same or not
+        hit = self.queue_key == qk
+        if hit:
+            # HIT
+            return self.responses_queue.get()
+        # MISS
         # killing the previous thread
-        if self.filler_thread is not None:
-            self.kill_event.set()
-            self.queue.get()
-            self.filler_thread.join()
-            self.kill_event.clear()
-            self.queue = Queue(self.max_queue_size)
+        self.terminate()
+
+        # fill the index in request queue
+        self.fill_request_thread = Thread(target=self.fill_request_queue, args=[num])
+        self.fill_request_thread.start()
 
         # generate new key
         self.queue_key = qk
 
         # start new thread
-        self.filler_thread = Thread(target=self.filler, args=(num, stage, max_length, min_num_feature, parts))
+        self.filler_thread = Thread(target=self.filler, args=(num, parts))
         self.filler_thread.start()
 
         # if we do not put this it could effect on the performance of the program because of the racing between threads
         time.sleep(3)
 
-        return self.fetch_sample(num, stage, max_length, min_num_feature, parts)
+        return self.fetch_sample(num, parts)
 
-    def filler(self, num: int, stage: str, length: int, token_size: int, parts: dict = None):
+    def filler(self, num: int, parts: dict = None):
         """
         This function is used to fill the queue with data then get batch read data from the queue
         :param num: number of samples
-        :param stage: TRAIN or TEST
-        :param length: maximum length of the sequence
-        :param token_size: minimum number of features
         :param parts: the parts of the data that we want to fetch
         """
         if parts is None:
             parts = MLDL.__PARTS
+
         with BoundedThreadPoolExecutor(max_workers=self.num_threads) as executor:
             while not self.kill_event.is_set():
-                executor.submit(self.filler_worker, num, stage, length, token_size, parts)
-            while not self.queue.empty():
-                self.queue.get()
+                executor.submit(self.filler_worker, num, parts)
+            try:
+                while not self.responses_queue.empty():
+                    self.responses_queue.get()
+            except Exception as e:
+                print(e)
+                pass
             executor.shutdown(wait=True)
 
-    def filler_worker(self, num: int, stage: str, length: int, token_size: int, parts: dict = None):
+    def filler_worker(self, num: int, parts: dict = None):
         if parts is None:
             parts = MLDL.__PARTS
-        df = self.fetch_sample(num, stage, length, token_size, parts)
-        self.queue.put(df)
+        df = self.fetch_sample(num, parts)
+        self.responses_queue.put(df)
         return
 
-    def fetch_sample(self, num: int, stage: str, length: int, token_size: int, parts: dict = None, retry: int = 0):
+    def fetch_sample(self, num: int, parts: dict = None, retry: int = 0):
         """
         This function is used to fetch the data from the database
         Run two threads to fetch the data from the database
         :param num: number of samples
-        :param stage: TRAIN or TEST or VAL or any other stage
-        :param length: maximum length of the sequence
-        :param token_size: minimum number of features
         :param parts: the parts of the data that we want to fetch
         :param retry: number of retries max is constant 7
         :return: dataframe of the data
         """
 
         if parts is None:
             parts = MLDL.__PARTS
         try:
             # get random row_id from the pool
-            index_list = random.sample(self.sample_cache, min(num, len(self.sample_cache)))
+            index_list = self.requests_queue.get()
 
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                main_thread = executor.submit(self.fetch_sample_main, index_list, length, token_size, parts)
+                main_thread = executor.submit(self.fetch_sample_main, index_list, parts)
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
-                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list, length, token_size)
+                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list)
 
                 main_df = main_thread.result()
 
                 interaction_df = pd.DataFrame()
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
                     interaction_df = interaction_thread.result()
 
@@ -202,82 +225,104 @@
                 time.sleep(1)
             else:
                 time.sleep(retry * 10)
             retry += 1
             print(f'Cannot fetch data from database, retry number {retry} times')
             if retry > 7:
                 raise Exception('Cannot fetch data from database')
-            return self.fetch_sample(num, stage, length, token_size, parts, retry)
+            return self.fetch_sample(num, parts, retry)
 
-    def fetch_sample_main(self, index_list: list, length: int, token_size: int, parts: dict = None):
+    def fetch_sample_main(self, index_list: list, parts: dict = None):
         """
         This function is used to fetch the main data from the database
         :param index_list: list of row_ids
-        :param length: maximum length of the sequence
-        :param token_size: minimum number of features
         :param parts: parts of the data
         :return: dataframe of main data
         """
         # s = time.perf_counter()
         session = self.Session()
         if parts is None:
             parts = MLDL.__PARTS
         try:
-            if token_size >= 10 and length <= 300:
+            if self.token_size >= 10 and self.max_length <= 300:
                 results = session.query(SeqLang300T10Model).filter(SeqLang300T10Model.row_id.in_(index_list)).all()
-            elif token_size >= 10:
+            elif self.token_size >= 10:
                 results = session.query(SeqLangT10Model).filter(SeqLangT10Model.row_id.in_(index_list)).all()
-            elif length <= 300:
+            elif self.max_length <= 300:
                 results = session.query(SeqLang300Model).filter(SeqLang300Model.row_id.in_(index_list)).all()
             else:
                 results = session.query(SeqLangModel).filter(SeqLangModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
+            session.rollback()
             raise Exception('Cannot fetch data from database <SeqLang>')
         finally:
             session.close()
+            session.flush()
         # print('fetch_sample_main')
         # print(time.perf_counter() - s)
         return df
 
-    def fetch_sample_interaction(self, index_list: list, length: int, token_size: int):
+    def fetch_sample_interaction(self, index_list: list):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
-        :param length: maximum length of the sequence
-        :param token_size: size of the token
         :return: dataframe of interaction data
         """
         # s = time.perf_counter()
         session = self.Session()
         try:
-            if token_size >= 10 and length <= 300:
+            if self.token_size >= 10 and self.max_length <= 300:
                 results = session.query(Interaction300T10Model).filter(Interaction300T10Model.row_id.in_(index_list)).all()
-            elif token_size >= 10:
+            elif self.token_size >= 10:
                 results = session.query(InteractionT10Model).filter(InteractionT10Model.row_id.in_(index_list)).all()
-            elif length <= 300:
+            elif self.max_length <= 300:
                 results = session.query(Interaction300Model).filter(Interaction300Model.row_id.in_(index_list)).all()
             else:
                 results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
+            session.rollback()
             raise Exception('Cannot fetch data from database <Interaction>')
         finally:
             session.close()
+            session.flush()
         # print('fetch_sample_interaction')
         # print(time.perf_counter() - s)
         return df
 
+    def fill_request_queue(self, num: int):
+        """
+        This function is used to fill the queue with requests index from the pool
+        :param num:
+        :return:
+        """
+        i = 0
+        max_i = len(self.pool) // num
+        while not self.kill_fill_requests_event.is_set():
+            index_list = self.pool[i * num: (i + 1) * num]
+            self.requests_queue.put(index_list)
+            i = (i + 1) % max_i
+
     def terminate(self):
         """
         Terminate the filler threads and clear the queue
         """
         # Terminate the filler thread
         if self.filler_thread is not None:
             self.kill_event.set()
-            if not self.queue.empty():
-                self.queue.get()
+            self.kill_fill_requests_event.set()
+
+            if not self.responses_queue.empty():
+                self.responses_queue.get()
+            if not self.requests_queue.empty():
+                self.requests_queue.get()
+
             self.filler_thread.join()
+            self.fill_request_thread.join()
+
             self.kill_event.clear()
-            self.queue = Queue(self.max_queue_size)
+            self.kill_fill_requests_event.clear()
+
+            self.Session.close_all()
```

### Comparing `lib310_lite-0.0.9/lib310_lite/mldl/models/InteractionModel.py` & `lib310_lite-0.1.0.dev1/lib310_lite/mldl/models/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.9/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.1.0.dev1/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.9/pyproject.toml` & `lib310_lite-0.1.0.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.9"
+version = "0.1.0.dev1"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
@@ -19,17 +19,18 @@
 bounded_pool_executor = ">=0.0.0"
 dask = ">=2022.11.0"
 distributed = ">=2022.11.0"
 dask-sql = ">=2022.11.0"
 gcsfs = ">=2022.11.0"
 SQLAlchemy = ">=2.0.0"
 psycopg2-binary= ">=2.9.0"
-
+mysqlclient = ">=2.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">7.1.2"
 python-dotenv = ">=0.19.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `lib310_lite-0.0.9/setup.py` & `lib310_lite-0.1.0.dev1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['lib310_lite',
  'lib310_lite.bigquery',
+ 'lib310_lite.laser',
  'lib310_lite.mldl',
  'lib310_lite.mldl.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -16,20 +17,21 @@
  'dask-sql>=2022.11.0',
  'dask>=2022.11.0',
  'db-dtypes>=1.0.0',
  'distributed>=2022.11.0',
  'gcsfs>=2022.11.0',
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
+ 'mysqlclient>=2.0.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.9',
+    'version': '0.1.0.dev1',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.9/PKG-INFO` & `lib310_lite-0.1.0.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.9
+Version: 0.1.0.dev1
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
@@ -17,9 +17,10 @@
 Requires-Dist: dask (>=2022.11.0)
 Requires-Dist: dask-sql (>=2022.11.0)
 Requires-Dist: db-dtypes (>=1.0.0)
 Requires-Dist: distributed (>=2022.11.0)
 Requires-Dist: gcsfs (>=2022.11.0)
 Requires-Dist: google-cloud (>=0.34.0)
 Requires-Dist: google-cloud-bigquery (>=3.2.0)
+Requires-Dist: mysqlclient (>=2.0.0)
 Requires-Dist: numpy (<1.23.0)
 Requires-Dist: psycopg2-binary (>=2.9.0)
```

