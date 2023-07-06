# Comparing `tmp/utilities_hki-0.1.6.tar.gz` & `tmp/utilities_hki-0.1.7.tar.gz`

## Comparing `utilities_hki-0.1.6.tar` & `utilities_hki-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/requirements.txt
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/__init__.py
--rwxr-xr-x   0        0        0    71816 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/analy_utils.py
--rwxr-xr-x   0        0        0     2729 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/db_utils.py
--rwxr-xr-x   0        0        0     2944 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/email_utils.py
--rwxr-xr-x   0        0        0     5268 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/fb_utils.py
--rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_2022-10-23.joblib
--rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_2023-04-02.joblib
--rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
--rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/.gitignore
--rwxr-xr-x   0        0        0    34522 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/LICENSE.txt
--rwxr-xr-x   0        0        0     4424 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/README.md
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 utilities_hki-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/requirements.txt
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/__init__.py
+-rwxr-xr-x   0        0        0    71817 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/analy_utils.py
+-rwxr-xr-x   0        0        0     2729 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/db_utils.py
+-rwxr-xr-x   0        0        0     2944 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/email_utils.py
+-rwxr-xr-x   0        0        0     5268 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/fb_utils.py
+-rwxr-xr-x   0        0        0   142582 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_2022-10-23.joblib
+-rwxr-xr-x   0        0        0    36982 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_2023-04-02.joblib
+-rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib
+-rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/.gitignore
+-rwxr-xr-x   0        0        0    34522 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/LICENSE.txt
+-rwxr-xr-x   0        0        0     4424 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/README.md
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 utilities_hki-0.1.7/PKG-INFO
```

### Comparing `utilities_hki-0.1.6/src/utilities_hki/analy_utils.py` & `utilities_hki-0.1.7/src/utilities_hki/analy_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -951,16 +951,17 @@
                  'campaign' : [col for col in vdf.columns if col.startswith('campaign')]}
     for out_col, in_cols in dict_cols.items():
         vdf[out_col] = vdf[in_cols].apply(lambda x: ','.join(x), axis=1)
         vdf[out_col] = vdf[out_col].apply(
             lambda x: {in_cols[i] : x.split(',')[i] for i in range(len(in_cols))})
     
     # add engagement types
-    visit_engagement = assign_cluster(vdf).reset_index()
-    vdf = vdf.merge(visit_engagement, how='left', on='visit_id')
+    if 'engagement_type' not in vdf.columns:
+        visit_engagement = assign_cluster(vdf).reset_index()
+        vdf = vdf.merge(visit_engagement, how='left', on='visit_id')
     vdf['engagement_type'] = vdf.engagement_type.str.replace(',', '').str.replace(' ', '_')
     
     # modify flow columns in input dataframe to include session starts/ends
     flows = ['action', 'action_site', 'page']
     for flow in flows:
         vdf[flow + '_flow'] = 'session-start,' + vdf[flow + '_flow'] + ',session-end'
     for flow in [flow for flow in flows if flow != 'action_site']:
@@ -1240,19 +1241,18 @@
 
     Returns
     -------
     pd.DataFrame
         Dataframe of numerical sequences of given action type flows.
     """
     
-    action_flow = pd.DataFrame()
+    action_flow = []
     actflow_cols = ['action_flow', 'action_category_flow', 'action_site_flow', 'action_ts']
-    for col in actflow_cols: action_flow = pd.concat(
-            [action_flow, df[col].str.split(',').explode()], axis=1)
-    action_flow = action_flow.reset_index(names='visitor_id')
+    for col in actflow_cols: action_flow.append(df[col].str.split(',').explode())
+    action_flow = pd.concat(action_flow, axis=1).reset_index()
     
     # filter action flow based on action types
     pat_ix = pd.Index([])  # select actions of given types 
     pat = r'.*_({})'.format('|'.join(action_types))
     pat_ix = action_flow.loc[action_flow.action_flow.apply(
         lambda x: bool(re.match(pat, x)))].index
     sess_ix = pd.Index([])  # select session-starts/ends
```

### Comparing `utilities_hki-0.1.6/src/utilities_hki/db_utils.py` & `utilities_hki-0.1.7/src/utilities_hki/db_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/src/utilities_hki/email_utils.py` & `utilities_hki-0.1.7/src/utilities_hki/email_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/src/utilities_hki/fb_utils.py` & `utilities_hki-0.1.7/src/utilities_hki/fb_utils.py`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/src/utilities_hki/data/gmm_2022-10-23.joblib` & `utilities_hki-0.1.7/src/utilities_hki/data/gmm_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/src/utilities_hki/data/gmm_2023-04-02.joblib` & `utilities_hki-0.1.7/src/utilities_hki/data/gmm_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib` & `utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2022-10-23.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib` & `utilities_hki-0.1.7/src/utilities_hki/data/gmm_scaler_2023-04-02.joblib`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/LICENSE.txt` & `utilities_hki-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/README.md` & `utilities_hki-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `utilities_hki-0.1.6/pyproject.toml` & `utilities_hki-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "utilities_hki"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Francisco Pena" },
   { name="Colleen Treado" },
 ]
 description = "Global utilities for Humankind data science"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `utilities_hki-0.1.6/PKG-INFO` & `utilities_hki-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilities_hki
-Version: 0.1.6
+Version: 0.1.7
 Summary: Global utilities for Humankind data science
 Project-URL: Homepage, https://github.com/humankind-datascience/utilities-hki
 Author: Francisco Pena, Colleen Treado
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

