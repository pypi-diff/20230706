# Comparing `tmp/resfeci-0.0.17.tar.gz` & `tmp/resfeci-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-7tvffme4\resfeci-0.0.17.tar", last modified: Wed Jul  5 02:49:44 2023, max compression
+gzip compressed data, was "C:\Users\jason\Desktop\Split_Excel\dist\.tmp-t9mt09u_\resfeci-0.0.18.tar", last modified: Thu Jul  6 02:30:34 2023, max compression
```

## Comparing `resfeci-0.0.17.tar` & `resfeci-0.0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.921710 resfeci-0.0.17/
--rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.17/LICENSE
--rw-rw-rw-   0        0        0     2651 2023-07-05 02:49:44.921204 resfeci-0.0.17/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2023-07-05 02:43:13.000000 resfeci-0.0.17/README.md
--rw-rw-rw-   0        0        0      809 2023-07-05 02:47:45.000000 resfeci-0.0.17/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 02:49:44.922217 resfeci-0.0.17/setup.cfg
--rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.17/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.892594 resfeci-0.0.17/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.910489 resfeci-0.0.17/src/resfeci/
--rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.17/src/resfeci/__init__.py
--rw-rw-rw-   0        0        0     5291 2023-07-05 02:48:56.000000 resfeci-0.0.17/src/resfeci/excel_split.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:49:44.919679 resfeci-0.0.17/src/resfeci.egg-info/
--rw-rw-rw-   0        0        0     2651 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 02:49:44.000000 resfeci-0.0.17/src/resfeci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 02:30:34.313111 resfeci-0.0.18/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 03:18:05.000000 resfeci-0.0.18/LICENSE
+-rw-rw-rw-   0        0        0     2701 2023-07-06 02:30:34.312095 resfeci-0.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2023-07-05 02:43:13.000000 resfeci-0.0.18/README.md
+-rw-rw-rw-   0        0        0      853 2023-07-06 02:28:43.000000 resfeci-0.0.18/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 02:30:34.313111 resfeci-0.0.18/setup.cfg
+-rw-rw-rw-   0        0        0       76 2023-07-04 06:55:59.000000 resfeci-0.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:30:34.274799 resfeci-0.0.18/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 02:30:34.291681 resfeci-0.0.18/src/resfeci/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:20:14.000000 resfeci-0.0.18/src/resfeci/__init__.py
+-rw-rw-rw-   0        0        0     6274 2023-07-06 02:28:43.000000 resfeci-0.0.18/src/resfeci/excel_split.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:30:34.310571 resfeci-0.0.18/src/resfeci.egg-info/
+-rw-rw-rw-   0        0        0     2701 2023-07-06 02:30:34.000000 resfeci-0.0.18/src/resfeci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-06 02:30:34.000000 resfeci-0.0.18/src/resfeci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 02:30:34.000000 resfeci-0.0.18/src/resfeci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 02:30:34.000000 resfeci-0.0.18/src/resfeci.egg-info/top_level.txt
```

### Comparing `resfeci-0.0.17/LICENSE` & `resfeci-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `resfeci-0.0.17/PKG-INFO` & `resfeci-0.0.18/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: resfeci
-Version: 0.0.17
+Version: 0.0.18
 Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ResFeci for Excel
 
 In it's current state, this package will allow you to quickly split a single Excel sheet into either separate tabs within the same report or into different Excel reports.  For example, if Column 'B' of your Excel report contains "Names" and "Jack" appears in 3 rows and "Jill" appears in 2, then, this will split the report into 2 separate reports (one for only Jack's rows and another for only Jill's rows); alternatively, this will create a new report with tabs entitled "Jack" and "Jill".
```

### Comparing `resfeci-0.0.17/README.md` & `resfeci-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `resfeci-0.0.17/pyproject.toml` & `resfeci-0.0.18/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires      = ["setuptools", "wheel", "openpyxl>=3.0.10", "pandas>=1.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resfeci"
-version = "0.0.17"
+version = "0.0.18"
 authors = [
   { name="Jason Yearry", email="jasonyearry@gmail.com" },
 ]
 
 
 description = "Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Excel", "Split", "opensource"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: Microsoft :: Windows",
+    "Development Status :: 4 - Beta"
 ]
 
 
 
 [project.urls]
 "Homepage" = "https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter"
```

### Comparing `resfeci-0.0.17/src/resfeci/excel_split.py` & `resfeci-0.0.18/src/resfeci/excel_split.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,14 +75,19 @@
 
     del final_destination_wb['Sheet'] # By default xlsx create sheet comes with a tab named sheet.  This gets rid of it.
     final_destination_wb.save('Split_Tab_Report.xlsx')
     final_destination_wb.close()
 
 def split_into_separate_reports(input_report_path, column_number_to_split_by, sheet=''):
 
+    # While pandas unique() is case-sensitive by default, Windows file-saving is not. For now, this script is case-sensitive. If you need two reports for "NAMES" and "NaMeS", Windows wouldn't recognize the
+    # case sensitivity in the filename and would just save a single "Names" report.  To get around this, I've created the unique_filename_index to be added to the filename.
+    unique_filename_index=2
+    previously_used_filenames=[]
+
     if sheet=='':
         df = pd.read_excel(input_report_path, sheet_name=0) # Sheet 0 = first sheet
     else:
         df = pd.read_excel(input_report_path, sheet_name=str(sheet))
 
     selected_col_values=df.iloc[:,int(column_number_to_split_by)-1].unique()
 
@@ -117,9 +122,18 @@
                     col_counter=col_counter+1
 
                 row_counter=row_counter+1
 
 
             unique_items=remove_illegal_characters(str(unique_items))
 
-            final_destination_wb.save(f'{str(unique_items)}.xlsx')
+            # Accounting for strings that differ only in case-sensitivity (i.e. "Name" vs. "NAMe")
+            # For now, the script is case sensitive
+
+            if unique_items.lower() not in previously_used_filenames:
+                previously_used_filenames.append(unique_items.lower())
+                final_destination_wb.save(f'{str(unique_items)}.xlsx')
+            elif unique_items.lower() in previously_used_filenames:
+                final_destination_wb.save(f'{str(unique_items)}_{str(unique_filename_index)}.xlsx')
+                unique_filename_index=unique_filename_index+1
             final_destination_wb.close()
+
```

### Comparing `resfeci-0.0.17/src/resfeci.egg-info/PKG-INFO` & `resfeci-0.0.18/src/resfeci.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: resfeci
-Version: 0.0.17
+Version: 0.0.18
 Summary: Currently allows you to quickly split an Excel report into multiple sheets or multiple reports based on unique column values.
 Author-email: Jason Yearry <jasonyearry@gmail.com>
 Project-URL: Homepage, https://github.com/Guitarman-Waiting-In-The-Sky/excel_splitter
 Keywords: Excel,Split,opensource
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ResFeci for Excel
 
 In it's current state, this package will allow you to quickly split a single Excel sheet into either separate tabs within the same report or into different Excel reports.  For example, if Column 'B' of your Excel report contains "Names" and "Jack" appears in 3 rows and "Jill" appears in 2, then, this will split the report into 2 separate reports (one for only Jack's rows and another for only Jill's rows); alternatively, this will create a new report with tabs entitled "Jack" and "Jill".
```

