# Comparing `tmp/veetility-0.1.97.tar.gz` & `tmp/veetility-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.97.tar", last modified: Tue Jul  4 10:25:05 2023, max compression
+gzip compressed data, was "veetility-0.1.98.tar", last modified: Thu Jul  6 17:27:36 2023, max compression
```

## Comparing `veetility-0.1.97.tar` & `veetility-0.1.98.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.119838 veetility-0.1.97/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-04 10:25:05.119674 veetility-0.1.97/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.97/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-04 10:25:05.119903 veetility-0.1.97/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-04 10:25:01.000000 veetility-0.1.97/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.114960 veetility-0.1.97/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.97/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.97/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.97/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.118344 veetility-0.1.97/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.97/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.97/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.97/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.97/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    31537 2023-07-04 10:24:35.000000 veetility-0.1.97/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.97/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53704 2023-07-04 10:08:58.000000 veetility-0.1.97/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.97/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.97/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.119458 veetility-0.1.97/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-04 10:25:04.000000 veetility-0.1.97/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-04 10:25:05.000000 veetility-0.1.97/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-04 10:25:04.000000 veetility-0.1.97/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-04 10:25:04.000000 veetility-0.1.97/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-04 10:25:05.000000 veetility-0.1.97/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.921010 veetility-0.1.98/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-06 17:27:36.920866 veetility-0.1.98/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.98/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-06 17:27:36.921062 veetility-0.1.98/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-06 17:26:22.000000 veetility-0.1.98/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.912028 veetility-0.1.98/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.98/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.98/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.98/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.919240 veetility-0.1.98/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.98/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    18470 2023-07-06 17:26:05.000000 veetility-0.1.98/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.98/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.98/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    31537 2023-07-04 10:24:35.000000 veetility-0.1.98/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.98/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    53704 2023-07-04 10:08:58.000000 veetility-0.1.98/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.98/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.98/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-06 17:27:36.920656 veetility-0.1.98/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-06 17:27:36.000000 veetility-0.1.98/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.97/PKG-INFO` & `veetility-0.1.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.97
+Version: 0.1.98
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.97/README.md` & `veetility-0.1.98/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/setup.py` & `veetility-0.1.98/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.97",
+    version="0.1.98",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.97/tests/test_best_fuzzy_match_dict.py` & `veetility-0.1.98/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/tests/test_identify_match_multi_cols.py` & `veetility-0.1.98/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/tests/test_prepare_string_matching.py` & `veetility-0.1.98/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility/cleaning_functions.py` & `veetility-0.1.98/veetility/cleaning_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,111 +38,113 @@
         errors (str, optional): How to handle errors during the conversion.
                                 Can be 'raise', 'ignore' or 'warn'
         cols_no_change (List[str], optional): A list of column names to be left unchanged.
 
     Returns:
         DataFrame: Output dataframe with the column names standardized."""
     
-    new_columns = []
+    new_columns = {}
     for column in df.columns:
         column = column.lower()
         hardcode_col_dict = {k.lower():v for k, v in hardcode_col_dict.items()} #make sure the keys are lowercase
         #hardcoded columns, for those unusual columns
         if column in hardcode_col_dict.keys():
-            column = hardcode_col_dict[column]
+            new_columns[column] = hardcode_col_dict[column]
         if 'day' == column:
-            column = 'date'
+            new_columns[column] = 'date'
         #Columns not to be changed and that don't get called similar things
         elif column in cols_no_change:
-            column = column
+            new_columns[column] = column
         elif ('created' in column) and (('date' in column) or ('time' in column) or ('video' in column)):
-            column = 'date'  # for organic
+            new_columns[column] = 'date'  # for organic
         elif ('video_create_time' in column):
-            column = 'post_timestamp'  # TikTok organic
+            new_columns[column] = 'post_timestamp'  # TikTok organic
         elif ('like' in column) or ('favorite' in column) or ('reaction' in column):
-            column = 'likes'
+            new_columns[column] = 'likes'
         elif ('video' not in column) and ('impression' in column) and ('unique' not in column):
-            column = 'impressions'
+            new_columns[column] = 'impressions'
         elif (column == 'reach') or (('impressions' in column) and ('unique' in column)):
-            column = 'reach'
-        elif ('campaign'in column) and ('name' in column):
-            column = 'campaign_name'
+            new_columns[column] = 'reach'
+        elif ('campaign' in column) and ('name' in column):
+            new_columns[column] = 'campaign_name'
         elif (('set' in column) or ('group' in column)) and ('name' in column):
-            column = 'group_name'
+            new_columns[column] = 'group_name'
         elif ('ad' in column) and ('name' in column):
-            column = 'ad_name' # for TikTok organic
+            new_columns[column] = 'ad_name' # for TikTok organic
         elif ('creative' in column) and ('name' in column):
-            column = 'creative_name'
+            new_columns[column] = 'creative_name'
         elif ('video' in column) and ('impression' in column):                       
-            column = 'video_impressions'
+            new_columns[column] = 'video_impressions'
         elif ('shares' in column) or ('retweet' in column):
-            column = 'shares'
+            new_columns[column] = 'shares'
         elif (('conversion' in column) or ('lifetime'in column)) and ('save' in column): #_1d_click_onsite_conversion_post_save in fb_ig_paid data
-            column = 'saved'
+            new_columns[column] = 'saved'
         
         elif ('video' in column) and ('view' in column) and not any(x in column for x in ['0', '5','2','3','6']): #don't include column with 25,50,75% completion
-            column = 'video_views'
+            new_columns[column] = 'video_views'
         elif ('video' in column) and ('25' in column):
-            column = 'ad_video_views_p_25'
+            new_columns[column] = 'ad_video_views_p_25'
         elif ('video' in column) and ('50' in column):
-            column = 'ad_video_views_p_50'
+            new_columns[column] = 'ad_video_views_p_50'
         elif ('video' in column) and ('75' in column):
-            column = 'ad_video_views_p_75'
+            new_columns[column] = 'ad_video_views_p_75'
         elif ('video' in column) and (('100' in column) or ('complet' in column) or('full' in column)):
-            column = 'video_completions'
+            new_columns[column] = 'video_completions'
         elif ('video' in column) and ('2' in column):
-            column = 'ad_video_watched_2_s'
+            new_columns[column] = 'ad_video_watched_2_s'
         elif ('video' in column) and ('3' in column):
-            column = 'ad_video_watched_3_s'
+            new_columns[column] = 'ad_video_watched_3_s'
         elif ('video' in column) and ('6' in column):
-            column = 'ad_video_watched_6_s'
-
+            new_columns[column] = 'ad_video_watched_6_s'
         
         elif ('organic' in column) and ('boosted' in column) or ( 'workstream' in column):
-            column = 'workstream'
+            new_columns[column] = 'workstream'
         elif 'currency' in column:
-            column = 'currency'
+            new_columns[column] = 'currency'
         elif 'country' in column:
-            column = 'country'
+            new_columns[column] = 'country'
         elif ('replies' in column) or ('comment' in column):
-            column = 'comments'
+            new_columns[column] = 'comments'
         elif (('page' in column) and('id' not in column)) or (column == 'profile') or ('business' in column) \
             or (('account' in column) and ('name' in column)) or (column == 'post_username'):
-            column = 'account_name'  # for twitter organic
+            new_columns[column] = 'account_name'  # for twitter organic
         elif ('caption' in column) or ('text' in column) or ('copy' in column) or ('message' in column) or(column == 'post') or (column == 'video_name'):
-            column = 'message'
+            new_columns[column] = 'message'
         elif (column == 'video_id') or ('post_id' in column) or ('ad_id' in column):
-            column = 'post_id'
+            new_columns[column] = 'post_id'
         elif ('url' in column) or (('link' in column) and ('clicks' not in column)):
-            column = 'url'
+            new_columns[column] = 'url'
         elif ('clicks' in column) and ('link' in column): #this is also equivalent to a swipe in Snapchat
-            column = 'link_clicks'  # for all_plats_paid
+            new_columns[column] = 'link_clicks'  # for all_plats_paid
         elif ('clicks' in column) and ('link' not in column):
-            column = 'clicks'  # for all_plats_paid
+            new_columns[column] = 'clicks'  # for all_plats_paid
         elif ('network' in column) or ('platform' in column):
-            column = 'platform'  # for li_tt_igStories_organic
+            new_columns[column] = 'platform'  # for li_tt_igStories_organic
         elif (('media' in column) and ('product' in column) and ('type' in column)) or ('placement' in column):
-            column = 'placement'
+            new_columns[column] = 'placement'
         elif (('type' in column) & ('post' in column)) or (('media' in column) and ('type' in column)) \
             or (('content' in column) and ('category' in column)): #creative media type for fb_ig_paid
-            column = 'media_type'
+            new_columns[column] = 'media_type'
         elif('cohort' in column):
-            column = 'cohort'
+            new_columns[column] = 'cohort'
         else:
             message = f'Column "{column}" in {name_of_df} not cleaned'
             if errors == 'raise':
                 raise Exception(message)
             cleaning_logger.logger.info(message)
 
-        new_columns.append(column)
-    if len(new_columns) != len(set(new_columns)):
-        error = f'Duplicate column names in {name_of_df} : {[item for item, count in Counter(new_columns).items() if count > 1]}'
+        new_columns[column] = column
+        duplicated_cols = [item for item,count in Counter(list(new_columns.values())).items() if count > 1]
+        print(f'{name_of_df} : {new_columns}')
+    if len(duplicated_cols) > 0:
+        error = f'Duplicate column names in {name_of_df} : {[f"{key} -> {value}" for key, value in dict.items() if value in duplicated_cols]}'
+        # error = f'Duplicate column names in {name_of_df} : {[item for item, count in Counter(new_columns).items() if count > 1]}'
         cleaning_logger.logger.exception(error)
         raise ValueError(error)
-    df.columns = new_columns
+    df.columns = list(new_columns.values())
 
     return df
 
 def extract_country_from_string(string, client_name, hardcode_dict):
     """Converts a string containing info identifying a certain 
     Args:
         string : str
```

### Comparing `veetility-0.1.97/veetility/generic_functions.py` & `veetility-0.1.98/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility/point_to_point_regressor.py` & `veetility-0.1.98/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility/quality_assessments.py` & `veetility-0.1.98/veetility/quality_assessments.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility/snowflake.py` & `veetility-0.1.98/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility/utility_functions.py` & `veetility-0.1.98/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility/v_lift.py` & `veetility-0.1.98/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility/view_through_rate.py` & `veetility-0.1.98/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.97/veetility.egg-info/PKG-INFO` & `veetility-0.1.98/veetility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.97
+Version: 0.1.98
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.97/veetility.egg-info/SOURCES.txt` & `veetility-0.1.98/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

