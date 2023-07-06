# Comparing `tmp/EZSheets-2023.3.14.tar.gz` & `tmp/EZSheets-2023.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EZSheets-2023.3.14.tar", last modified: Tue Mar 14 21:09:12 2023, max compression
+gzip compressed data, was "dist\EZSheets-2023.8.6.tar", last modified: Thu Jul  6 21:45:15 2023, max compression
```

## Comparing `EZSheets-2023.3.14.tar` & `EZSheets-2023.8.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/
--rw-rw-rw-   0        0        0      164 2020-08-04 06:42:17.000000 EZSheets-2023.3.14/AUTHORS.txt
--rw-rw-rw-   0        0        0    35821 2019-02-08 06:36:15.000000 EZSheets-2023.3.14/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2019-02-08 06:36:15.000000 EZSheets-2023.3.14/MANIFEST.in
--rw-rw-rw-   0        0        0    12231 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/PKG-INFO
--rw-rw-rw-   0        0        0    11258 2023-03-14 21:05:38.000000 EZSheets-2023.3.14/README.md
--rw-rw-rw-   0        0        0        0 2019-02-08 06:36:15.000000 EZSheets-2023.3.14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/setup.cfg
--rw-rw-rw-   0        0        0     1632 2022-10-10 19:12:14.000000 EZSheets-2023.3.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/
-drwxrwxrwx   0        0        0        0 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/EZSheets.egg-info/
--rw-rw-rw-   0        0        0    12231 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/EZSheets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/EZSheets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/EZSheets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/EZSheets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/EZSheets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/src/ezsheets/
--rw-rw-rw-   0        0        0    77461 2023-03-14 21:05:55.000000 EZSheets-2023.3.14/src/ezsheets/__init__.py
--rw-rw-rw-   0        0        0     5731 2019-02-11 05:24:23.000000 EZSheets-2023.3.14/src/ezsheets/colorvalues.py
-drwxrwxrwx   0        0        0        0 2023-03-14 21:09:12.000000 EZSheets-2023.3.14/tests/
--rw-rw-rw-   0        0        0    31868 2019-03-04 08:28:11.000000 EZSheets-2023.3.14/tests/test_ezsheets.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/
+-rw-rw-rw-   0        0        0      164 2020-08-04 06:42:17.000000 EZSheets-2023.8.6/AUTHORS.txt
+-rw-rw-rw-   0        0        0    35821 2019-02-08 06:36:15.000000 EZSheets-2023.8.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2019-02-08 06:36:15.000000 EZSheets-2023.8.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12278 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11312 2023-07-06 21:41:59.000000 EZSheets-2023.8.6/README.md
+-rw-rw-rw-   0        0        0       34 2023-04-25 17:29:09.000000 EZSheets-2023.8.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2022-10-10 19:12:14.000000 EZSheets-2023.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/
+-rw-rw-rw-   0        0        0    12278 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/ezsheets/
+-rw-rw-rw-   0        0        0    79498 2023-07-06 21:41:31.000000 EZSheets-2023.8.6/src/ezsheets/__init__.py
+-rw-rw-rw-   0        0        0     6293 2023-04-25 17:21:45.000000 EZSheets-2023.8.6/src/ezsheets/colorvalues.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/tests/
+-rw-rw-rw-   0        0        0    31821 2023-07-06 20:09:52.000000 EZSheets-2023.8.6/tests/test_ezsheets.py
```

### Comparing `EZSheets-2023.3.14/LICENSE.txt` & `EZSheets-2023.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EZSheets-2023.3.14/PKG-INFO` & `EZSheets-2023.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EZSheets
-Version: 2023.3.14
-Summary: A Pythonic interface to the Google Sheets API that actually works as of March 2023.
+Version: 2023.8.6
+Summary: A Pythonic interface to the Google Sheets API that actually works as of July 2023.
 Home-page: https://github.com/asweigart/ezsheets
 Author: Al Sweigart
 Author-email: al@inventwithpython.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 # EZSheets
 
 
-A Pythonic interface to the Google Sheets API that actually works as of March 2023.
+A Pythonic interface to the Google Sheets API that actually works as of July 2023.
 
 ## Installation and Setup
 
 To install with pip, run:
 
     pip install ezsheets
 
@@ -60,15 +60,15 @@
 
 ### Configure the OAuth Consent Screen for Your Project
 
 Click on the Navigation button in the upper left and then navigate to "APIs & Services" and then "OAuth Consent Screen." The consent screen will appear the first time when you or users of your Python script use EZSheets. With a free Google account that is not set up as a Google Workspace user, you'll have to select the External User Type option instead of Internal User Type. These are further explained on Google's [Setting up your OAuth consent screen help page](https://support.google.com/cloud/answer/10311615).
 
 On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. You'll be taken to a page where you set up what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click "SAVE AND CONTINUE."
 
-Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `https://mail.google.com/` and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
+Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
 
 Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts will be limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail addresses and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
 
 Step 4 "Summary" provides a summary of the previous steps. If all the information looks right, click the "BACK TO DASHBOARD" button. The next step is to create credentials for your project.
 
 ### Create Credentials for Your Project
 
@@ -80,15 +80,15 @@
 
 The pop up that appears shows your , click "DOWNLOAD JSON" to download the credentials file. This file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Rename it to *credentials-sheets.json* and place it in the same folder that your Python script will be in.
 
 ### Log In with the Credentials File
 
 Run the Python interactive shell from the same folder that the *credentials-sheets.json* file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a *credentials-sheets.json* file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
 
-You will get a warning message that reads "Google hasnâ€™t verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
+You will get a warning message that reads "Google hasn't verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
 
 You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your *credentials-sheets.json* file, you'll now see a *token.json* file. Do not share these files: they can be used to log in and access your Google Sheets spreadsheets.
 
 ## Quickstart Guide
 
 After you've set up your credentials and token files, you can import EZSheets to access your Google Sheets. Create a `Spreadsheet` object by using the Spreadsheet's URL:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `EZSheets-2023.3.14/README.md` & `EZSheets-2023.8.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # EZSheets
 
 
-A Pythonic interface to the Google Sheets API that actually works as of March 2023.
+A Pythonic interface to the Google Sheets API that actually works as of July 2023.
 
 ## Installation and Setup
 
 To install with pip, run:
 
     pip install ezsheets
 
@@ -37,15 +37,15 @@
 
 ### Configure the OAuth Consent Screen for Your Project
 
 Click on the Navigation button in the upper left and then navigate to "APIs & Services" and then "OAuth Consent Screen." The consent screen will appear the first time when you or users of your Python script use EZSheets. With a free Google account that is not set up as a Google Workspace user, you'll have to select the External User Type option instead of Internal User Type. These are further explained on Google's [Setting up your OAuth consent screen help page](https://support.google.com/cloud/answer/10311615).
 
 On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. You'll be taken to a page where you set up what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click "SAVE AND CONTINUE."
 
-Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `https://mail.google.com/` and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
+Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
 
 Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts will be limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail addresses and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
 
 Step 4 "Summary" provides a summary of the previous steps. If all the information looks right, click the "BACK TO DASHBOARD" button. The next step is to create credentials for your project.
 
 ### Create Credentials for Your Project
 
@@ -57,15 +57,15 @@
 
 The pop up that appears shows your , click "DOWNLOAD JSON" to download the credentials file. This file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Rename it to *credentials-sheets.json* and place it in the same folder that your Python script will be in.
 
 ### Log In with the Credentials File
 
 Run the Python interactive shell from the same folder that the *credentials-sheets.json* file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a *credentials-sheets.json* file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
 
-You will get a warning message that reads "Google hasn’t verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
+You will get a warning message that reads "Google hasn't verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
 
 You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your *credentials-sheets.json* file, you'll now see a *token.json* file. Do not share these files: they can be used to log in and access your Google Sheets spreadsheets.
 
 ## Quickstart Guide
 
 After you've set up your credentials and token files, you can import EZSheets to access your Google Sheets. Create a `Spreadsheet` object by using the Spreadsheet's URL:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `EZSheets-2023.3.14/setup.py` & `EZSheets-2023.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `EZSheets-2023.3.14/src/EZSheets.egg-info/PKG-INFO` & `EZSheets-2023.8.6/src/EZSheets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EZSheets
-Version: 2023.3.14
-Summary: A Pythonic interface to the Google Sheets API that actually works as of March 2023.
+Version: 2023.8.6
+Summary: A Pythonic interface to the Google Sheets API that actually works as of July 2023.
 Home-page: https://github.com/asweigart/ezsheets
 Author: Al Sweigart
 Author-email: al@inventwithpython.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 # EZSheets
 
 
-A Pythonic interface to the Google Sheets API that actually works as of March 2023.
+A Pythonic interface to the Google Sheets API that actually works as of July 2023.
 
 ## Installation and Setup
 
 To install with pip, run:
 
     pip install ezsheets
 
@@ -60,15 +60,15 @@
 
 ### Configure the OAuth Consent Screen for Your Project
 
 Click on the Navigation button in the upper left and then navigate to "APIs & Services" and then "OAuth Consent Screen." The consent screen will appear the first time when you or users of your Python script use EZSheets. With a free Google account that is not set up as a Google Workspace user, you'll have to select the External User Type option instead of Internal User Type. These are further explained on Google's [Setting up your OAuth consent screen help page](https://support.google.com/cloud/answer/10311615).
 
 On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. You'll be taken to a page where you set up what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click "SAVE AND CONTINUE."
 
-Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `https://mail.google.com/` and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
+Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
 
 Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts will be limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail addresses and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
 
 Step 4 "Summary" provides a summary of the previous steps. If all the information looks right, click the "BACK TO DASHBOARD" button. The next step is to create credentials for your project.
 
 ### Create Credentials for Your Project
 
@@ -80,15 +80,15 @@
 
 The pop up that appears shows your , click "DOWNLOAD JSON" to download the credentials file. This file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Rename it to *credentials-sheets.json* and place it in the same folder that your Python script will be in.
 
 ### Log In with the Credentials File
 
 Run the Python interactive shell from the same folder that the *credentials-sheets.json* file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a *credentials-sheets.json* file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
 
-You will get a warning message that reads "Google hasnâ€™t verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
+You will get a warning message that reads "Google hasn't verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
 
 You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your *credentials-sheets.json* file, you'll now see a *token.json* file. Do not share these files: they can be used to log in and access your Google Sheets spreadsheets.
 
 ## Quickstart Guide
 
 After you've set up your credentials and token files, you can import EZSheets to access your Google Sheets. Create a `Spreadsheet` object by using the Spreadsheet's URL:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `EZSheets-2023.3.14/src/ezsheets/__init__.py` & `EZSheets-2023.8.6/src/ezsheets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 
 # IMPORTANT NOTE: This module has not been stress-tested for performance
 # and should not be considered "thread-safe" if multiple users are
 
 # TODO - figure out drive quotas
 # TODO - batch mode?
 
-import pickle, re, collections, time, webbrowser
+import collections
 import json
 import os.path
+import pickle
+import re
+import time
+import webbrowser
+
+from apiclient.http import MediaFileUpload, MediaIoBaseDownload
+from google.auth.transport.requests import Request
+from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
-from google_auth_oauthlib.flow import InstalledAppFlow
-from google.auth.transport.requests import Request
-from apiclient.http import MediaIoBaseDownload, MediaFileUpload
 
-
-__version__ = "2023.3.14"
+__version__ = "2023.8.6"
 
 # SCOPES_SHEETS = ['https://www.googleapis.com/auth/spreadsheets.readonly']
 SCOPES_SHEETS = ["https://www.googleapis.com/auth/spreadsheets"]
 SHEETS_SERVICE = None
 IS_INITIALIZED = False
 
 # SCOPES_DRIVE = ['https://www.googleapis.com/auth/drive.readonly']
@@ -589,17 +593,17 @@
                 len(self.spreadsheet.sheets) + value
             )  # convert this negative index into its corresponding positive index
         if value >= len(self.spreadsheet.sheets):
             raise IndexError("%r is out of range (0 to %d)" % (value, len(self.spreadsheet.sheets) - 1))
 
         # Update the index:
         if value > self._index:
-            value += (
-                1
-            )  # Google Sheets uses "before the move" indexes, which is confusing and I don't want to do it here.
+            # Google Sheets uses "before the move" indexes, which is confusing and I don't want to do it here.
+            value += 1
+
 
         # request = SHEETS_SERVICE.spreadsheets().batchUpdate(spreadsheetId=self._spreadsheet._spreadsheetId,
         # body={
         #    'requests': [{'updateSheetProperties': {'properties': {'sheetId': self._sheetId,
         #                                                           'index': value},
         #                                            'fields': 'index'}}]})
         # _logWriteRequest(); request.execute()
@@ -1362,15 +1366,14 @@
             }
         )
 
         # Update the local data in `_cells`:
         self._cells = {}
 
     def copyTo(self, destinationSpreadsheet):
-
         # NOTE: Don't update this method to allow ID or URL strings to be
         # passed, because we'll always need to call refresh() on the
         # spreadsheet object itself.
 
         if not isinstance(destinationSpreadsheet, Spreadsheet):
             raise TypeError(
                 "destinationSpreadsheet must be of type Spreadsheet, not %s" % (type(destinationSpreadsheet).__name__)
@@ -1621,15 +1624,15 @@
     while columnLetter:
         digits.append(ord(columnLetter[0]) - 64)
         columnLetter = columnLetter[1:]
 
     number = 0
     place = 0
     for digit in reversed(digits):
-        number += digit * (26 ** place)
+        number += digit * (26**place)
         place += 1
 
     return number
 
 
 def convertAddress(*address):
     if len(address) < 1 or len(address) > 2:
@@ -1649,32 +1652,58 @@
         # Convert (1, 2) to 'A2'
         return getColumnLetterOf(address[0]) + str(address[1])
 
     raise TypeError('The address argument must be a singe string like "A1" or a tuple of two 1-based integers.')
 
 
 def init(
-    credentialsFile="credentials-sheets.json",
+    credentialsFile='.',
     sheetsTokenFile="token-sheets.pickle",
     driveTokenFile="token-drive.pickle",
     _raiseException=True,
 ):
     global SHEETS_SERVICE, DRIVE_SERVICE, IS_INITIALIZED
 
-    IS_INITIALIZED = (
-        False
-    )  # Set this to False, in case module was initialized before but this current initialization fails.
+    # Set this to False, in case module was initialized before but this current initialization fails.
+    IS_INITIALIZED = False
+
+    # If the credentialsFile parameter is None, assume the credentials json file in the cwd.
+    # In version 2023.3.14 and before (and in Automate the Boring Stuff
+    # 2nd Edition), the credentials file had to be credentials-sheets.json.
+    # But this isn't the name it has when you download it from Google
+    # Cloud Console, so we'll just use the client_secret_*.json filename
+    # format it already has, and fall back on credentials-sheets.json.
+    # If credentialsFile is a folder name, use that folder to search for the credentials file.
+
+    # credentialsFile is a bit misleading of a name because it can be a file or a folder (that contains the credentials file)
+    if os.path.isdir(os.path.abspath(credentialsFile)):
+        possibleCredentialsFiles = []
+        for filename in os.listdir(os.path.abspath(credentialsFile)):
+            if (filename.startswith('client_secret_') and filename.endswith('.json')) or filename == 'credentials-sheets.json':
+                possibleCredentialsFiles.append(filename)
+        if len(possibleCredentialsFiles) == 0:
+            credentialsFile = 'credentials-sheets.json'  # Setting it to this nonexistant file will trigger the later EZSheetsException.
+        elif len(possibleCredentialsFiles) > 1:
+            raise EZSheetsException('You must specify a credentialsFile argument to init() because multiple possible credential files exist in ' + str(os.getcwd()) + ': ' + ', '.join(possibleCredentialsFiles))
+        elif len(possibleCredentialsFiles) == 1:
+            credentialsFile = os.path.join(os.path.abspath(credentialsFile), possibleCredentialsFiles[0])
 
     try:
         if not os.path.exists(credentialsFile):
             raise EZSheetsException(
                 'Can\'t find credentials file at %s. You can download this file from https://developers.google.com/sheets/api/quickstart/python  and clicking "Enable the Google Sheets API". Rename the downloaded file to credentials-sheets.json.'
                 % (os.path.abspath(credentialsFile))
             )
 
+        # Assume that the token files are in the same folder as the credentials file:
+        if not os.path.isabs(sheetsTokenFile):
+            sheetsTokenFile = os.path.join(os.path.dirname(os.path.abspath(credentialsFile)), sheetsTokenFile)
+        if not os.path.isabs(driveTokenFile):
+            driveTokenFile = os.path.join(os.path.dirname(os.path.abspath(credentialsFile)), driveTokenFile)
+
         # Log in to Google Sheets API to generate token-sheets.pickle.
         creds = None
         # The file token-sheets.pickle stores the user's access and refresh tokens, and is
         # created automatically when the authorization flow completes for the first
         # time.
         if os.path.exists(sheetsTokenFile):
             with open(sheetsTokenFile, "rb") as token:
@@ -1774,15 +1803,15 @@
     media = MediaFileUpload(filename, mimetype=mimeType)
     # file = DRIVE_SERVICE.files().create(body={'name': filename, 'mimeType': 'application/vnd.google-apps.spreadsheet'},
     #                                    media_body=media,
     #                                    fields='id').execute()
     file = _makeRequest(
         "drive.create",
         **{
-            "body": {"name": filename, "mimeType": "application/vnd.google-apps.spreadsheet"},
+            "body": {"name": os.path.basename(filename), "mimeType": "application/vnd.google-apps.spreadsheet"},
             "media_body": media,
             "fields": "id",
         }
     )
     return Spreadsheet(file.get("id"))
```

### Comparing `EZSheets-2023.3.14/tests/test_ezsheets.py` & `EZSheets-2023.8.6/tests/test_ezsheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -830,9 +830,7 @@
 
 
 
 def test_getitem(init, checkPreAndPostCondition):
     pass # TODO LEFT OFF
 
 
-if __name__ == '__main__':
-    pytest.main()
```

