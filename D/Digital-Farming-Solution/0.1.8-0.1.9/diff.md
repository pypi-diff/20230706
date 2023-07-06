# Comparing `tmp/Digital_Farming_Solution-0.1.8.tar.gz` & `tmp/Digital_Farming_Solution-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Farming_Solution-0.1.8.tar", last modified: Tue Jul  4 18:24:47 2023, max compression
+gzip compressed data, was "Digital_Farming_Solution-0.1.9.tar", last modified: Thu Jul  6 09:29:00 2023, max compression
```

## Comparing `Digital_Farming_Solution-0.1.8.tar` & `Digital_Farming_Solution-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 18:24:47.050458 Digital_Farming_Solution-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-07-04 18:24:46.943420 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution/
--rw-rw-rw-   0        0        0     9185 2023-07-04 18:24:15.000000 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution/Select_options.py
--rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:24:47.037544 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution.egg-info/
--rw-rw-rw-   0        0        0      609 2023-07-04 18:24:44.000000 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-04 18:24:46.000000 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 18:24:44.000000 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-04 18:24:45.000000 Digital_Farming_Solution-0.1.8/Digital_Farming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-07-04 18:24:47.046876 Digital_Farming_Solution-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-04 18:24:47.051455 Digital_Farming_Solution-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-07-04 18:24:23.000000 Digital_Farming_Solution-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:29:00.815617 Digital_Farming_Solution-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-07-06 09:29:00.729847 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution/
+-rw-rw-rw-   0        0        0     7983 2023-07-06 09:28:38.000000 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution/Select_options.py
+-rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 09:29:00.804646 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-07-06 09:28:59.000000 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-06 09:29:00.000000 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 09:28:59.000000 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-06 09:28:59.000000 Digital_Farming_Solution-0.1.9/Digital_Farming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-07-06 09:29:00.812626 Digital_Farming_Solution-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-06 09:29:00.816616 Digital_Farming_Solution-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-07-06 09:28:44.000000 Digital_Farming_Solution-0.1.9/setup.py
```

### Comparing `Digital_Farming_Solution-0.1.8/Digital_Farming_Solution/Select_options.py` & `Digital_Farming_Solution-0.1.9/Digital_Farming_Solution/Select_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     
     return df_final
 
 #############################################################################################################################################################################
 
 # Creating the function for Weather changes between the low and high yield
 
-def Weather_Change_With_Low_Vs_High_Yield(data,Yield_column,Weather_params):
+def Weather_Change_IN_Low_Vs_High_Yield(data,Yield_column,Weather_params):
 
     data = Yield_Binning(data,Yield_column)
     
     data = data[(data[Yield_column] > 0)]
     
     Weather_params.insert(0,Yield_column)
     
@@ -181,76 +181,48 @@
         
         fig = px.scatter(data, x= 'Month_Date', y="Avg_yield", size='Avg_yield',color = 'Month',title= 'Delta Change by ' + column_name +' .')
         
         fig.show()
 
 #################################################################################################################################################
 
-# Getting the Best planting and Harvest Dates
-def Best_Dates(data,Yield_cloumn,by,Season = False,return_dataframe = True):
+# Getting the Best dates to plant and harvest
+def Best_Dates(data, Yield_cloumn, by, return_dataframe = True):
     
     # Storing the name 
     column_name = by
-    
-    if Season == True:
-    
-        # Calculating the best planting dates
-        data = data.groupby([column_name,'season']).agg(Avg_yield=(Yield_cloumn, 'mean')).reset_index()
         
-        # strftime --> b for month (jan,feb) and d for day of the date
-        data['Month_Date'] = data[column_name].apply(lambda x: x.strftime('%b-%d'))
+    # Calculating the best planting dates
+    data = data.groupby([column_name]).agg(Avg_yield=(Yield_cloumn, 'mean')).reset_index()
 
-        # Convert the 'dates' column to datetime format with a fake year
-        data['Month_Date'] = pd.to_datetime('2020-' + data['Month_Date'], format='%Y-%b-%d')
+    # strftime --> b for month (jan,feb) and d for day of the date
+    data['Month_Date'] = data[column_name].apply(lambda x: x.strftime('%b-%d'))
 
-        # Sort the DataFrame by the 'dates' column
-        data = data.sort_values(by='Month_Date').reset_index(drop=True)
+    data['Month'] = data[column_name].apply(lambda x: x.strftime('%b'))
 
-        # Remove the fake year from the 'dates' column
-        data['Month_Date'] = data['Month_Date'].dt.strftime('%b-%d')
+    # Convert the 'dates' column to datetime format with a fake year
+    data['Month_Date'] = pd.to_datetime('2020-' + data['Month_Date'], format='%Y-%b-%d')
 
-        data.reset_index(drop = True,inplace = True)
-        
-        if return_dataframe == True:
-            
-            return data
-        
-        else:
-            
-            fig = px.bar(data, x= 'Month_Date', y='Avg_yield',color='season')
-            fig.update_layout(title = 'Best ' + column_name +' in the Season', yaxis_title = 'Average Yield') 
-            fig.show()
-    
-    else:
-        
-        # Calculating the best planting dates
-        data = data.groupby([column_name]).agg(Avg_yield=(Yield_cloumn, 'mean')).reset_index()
-        
-        # strftime --> b for month (jan,feb) and d for day of the date
-        data['Month_Date'] = data[column_name].apply(lambda x: x.strftime('%b-%d'))
+    # Sort the DataFrame by the 'dates' column
+    data = data.sort_values(by='Month_Date').reset_index(drop=True)
 
-        # Convert the 'dates' column to datetime format with a fake year
-        data['Month_Date'] = pd.to_datetime('2020-' + data['Month_Date'], format='%Y-%b-%d')
+    # Remove the fake year from the 'dates' column
+    data['Month_Date'] = data['Month_Date'].dt.strftime('%b-%d')
 
-        # Sort the DataFrame by the 'dates' column
-        data = data.sort_values(by='Month_Date').reset_index(drop=True)
+    data.reset_index(drop = True,inplace = True)
+    
+    data = data.dropna()
+    
+    if return_dataframe == True:
 
-        # Remove the fake year from the 'dates' column
-        data['Month_Date'] = data['Month_Date'].dt.strftime('%b-%d')
+        return data
 
-        data.reset_index(drop = True,inplace = True)
-        
-        if return_dataframe == True:
-            
-            return data
-        
-        else:
-            
-            fig = px.bar(data, x= 'Month_Date', y='Avg_yield')
-            fig.update_layout(title = 'Best ' + column_name +' in the Season', yaxis_title = 'Average Yield') 
-            fig.show()
-        
+    else:
 
+        fig = px.scatter(data, x='Month_Date', y='Avg_yield',size='Avg_yield',color = 'Month')
+        fig.update_layout(title = 'Best Dates', yaxis_title = 'Average Yield') 
+        fig.show()
+            
 ################################################################################################################
```

### Comparing `Digital_Farming_Solution-0.1.8/Digital_Farming_Solution.egg-info/PKG-INFO` & `Digital_Farming_Solution-0.1.9/Digital_Farming_Solution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital-Farming-Solution
-Version: 0.1.8
+Version: 0.1.9
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.8/PKG-INFO` & `Digital_Farming_Solution-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital_Farming_Solution
-Version: 0.1.8
+Version: 0.1.9
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.8/setup.py` & `Digital_Farming_Solution-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Farming_Solution",
-    version="0.1.8",
+    version="0.1.9",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description=" The packages are helps to the DFS Teams to perform some of the task easily.",
     long_description= 'By importing this packages we can work on easily and  get some meaningfull information.It is more siutable for the dataframe works and it will returnns the Dataframe.',
     long_description_content_type="text/markdown",
     packages=["Digital_Farming_Solution"],
     classifiers=[
```

