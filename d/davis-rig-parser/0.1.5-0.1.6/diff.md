# Comparing `tmp/davis_rig_parser-0.1.5.tar.gz` & `tmp/davis_rig_parser-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/davis_rig_parser-0.1.5.tar", last modified: Mon Jul  3 16:07:48 2023, max compression
+gzip compressed data, was "davis_rig_parser-0.1.6.tar", last modified: Thu Jul  6 14:40:22 2023, max compression
```

## Comparing `davis_rig_parser-0.1.5.tar` & `davis_rig_parser-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5451 2023-07-03 16:07:20.000000 davis_rig_parser-0.1.5/README.md
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.5/davis_rig_parser/__init__.py
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18214 2023-06-28 21:45:24.000000 davis_rig_parser-0.1.5/davis_rig_parser/davis_rig_parser.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/requires.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/davis_rig_parser.egg-info/top_level.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/setup.cfg
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-03 16:07:05.000000 davis_rig_parser-0.1.5/setup.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-03 16:07:48.000000 davis_rig_parser-0.1.5/tests/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      302 2023-07-01 22:08:21.000000 davis_rig_parser-0.1.5/tests/test.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5451 2023-07-03 19:46:06.000000 davis_rig_parser-0.1.6/README.md
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/davis_rig_parser/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.1.6/davis_rig_parser/__init__.py
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    18475 2023-07-06 14:33:58.000000 davis_rig_parser-0.1.6/davis_rig_parser/davis_rig_parser.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/requires.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-06 14:40:22.000000 davis_rig_parser-0.1.6/davis_rig_parser.egg-info/top_level.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/setup.cfg
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-06 14:37:03.000000 davis_rig_parser-0.1.6/setup.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-06 14:40:22.948365 davis_rig_parser-0.1.6/tests/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.1.6/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `davis_rig_parser-0.1.5/README.md` & `davis_rig_parser-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `davis_rig_parser-0.1.5/davis_rig_parser/davis_rig_parser.py` & `davis_rig_parser-0.1.6/davis_rig_parser/davis_rig_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,24 @@
                     #entry is less than 100, the first row becomes the sum of the
                     #first entry and the second entry and all of the entries above
                     #the 1st shift to the left 1 place and the leftover rightmost
                     #entry becomes 0
                     cutslist = []
                     for row in lat_set:
                         cuts=0
-                        while row[0] < min_latency:
-                            row[0] = row[0] + row[1]
-                            row[1:-1] = row[2:]
-                            row[-1] = 0
-                            cuts +=1
-                            if cuts >5: #failsafe so the loop doesn't go infinite, arbitrarily set at 5
-                                break
+                        if len(row) ==1:
+                            row[0] = np.array([np.nan])[0]
+                        else:
+                            while row[0] < min_latency:
+                                row[0] = row[0] + row[1]
+                                row[1:-1] = row[2:]
+                                row[-1] = 0
+                                cuts +=1
+                                if cuts >5: #failsafe so the loop doesn't go infinite, arbitrarily set at 5
+                                    break
                         #then, set all ILIs under min_ILI to 0 to be deleted later
                         for j in range(len(row[1:])):
                             if row[j] < min_ILI and row[j] != 0:
                                 row[j] = 0
                                 cuts+=1
                             
                         cutslist.append(cuts)
@@ -183,16 +186,16 @@
                 
                 #Set concentrations to 0 if concentration column blank
                 df['CONCENTRATION']=df['CONCENTRATION'].str.strip()
                 df['CONCENTRATION'] = df['CONCENTRATION'].apply(lambda x: 0 if x == '' else x)
 
                 #Convert specific columns to numeric
                 df["SOLUTION"] = df["SOLUTION"].str.strip()
-                df[["PRESENTATION","TUBE","CONCENTRATION","LICKS","Latency"]] = \
-                    df[["PRESENTATION","TUBE","CONCENTRATION","LICKS","Latency"]].apply(pd.to_numeric)
+                df[["PRESENTATION","TUBE","LICKS","Latency"]] = \
+                    df[["PRESENTATION","TUBE","LICKS","Latency"]].apply(pd.to_numeric)
 
                 #Add in identifier columns
                 df.insert(loc=0, column='Animal', value=Detail_Dict['Animal'])
                 df.insert(loc=0, column='Date', value=Detail_Dict['StartDate'])
                 df.insert(loc=3, column='Trial_num', value='')
                 df['Trial_num'] = df.groupby('TUBE').cumcount()+1
 
@@ -245,34 +248,36 @@
 #     requires a bout_crit 
 #     
 #     Input: 1) Dataframe and Licking Matrix (obtained from MedMS8_reader_stone)
 #            2) Bout_crit; variable which is the time (ms) needed to pause between
 #               licks to count as a bout (details in: Davis 1996 & Spector et al. 1998).
 # 
 #     Output: Appended dataframe with the licks within a bout/trial, latency to 
-#             to first lick within trial    
+#             first lick within trial
 # =============================================================================
 
-    
-
     #Find where the last lick occured in each trial
-    last_lick = list(map(lambda x: [i for i, x_ in enumerate(x) if not \
-                                    np.isnan(x_)][-1], latency_array))
-    
+    if len(latency_array) > 0 and len(latency_array[0]) > 0:
+        last_lick = list(map(lambda x: [i for i, x_ in enumerate(x) if not np.isnan(x_)][-1], latency_array))
+    else:
+        last_lick = []
+
     #Create function to search rows of matrix avoiding 'runtime error' caused by Nans
     crit_nan_search = np.frompyfunc(lambda x: (~np.isnan(x)) & (x >=bout_crit), 1, 1)
     i = 0
     #Create empty list to store number of bouts by trial
     bouts = []; ILIs_win_bouts = []
     for i in range(latency_array.shape[0]):
         #Create condition if animal never licks within trial
-        if last_lick[i] == 0:
+        if latency_array.size == 0:
+            bouts.append([])
+            ILIs_win_bouts.append([])
+        elif last_lick[i] == 0:
             bouts.append(last_lick[i])
             ILIs_win_bouts.append(last_lick[i])
-            
         else:
             bout_pos = np.where(np.array(crit_nan_search(latency_array[i,:])).astype(int))
             
             #Insert the start number or row to get accurate count
             bout_pos = np.insert(bout_pos,0,0)  # inserting at the start
             
             #Caclulate bout duration
```

