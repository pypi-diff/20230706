# Comparing `tmp/directory_forms_api_client-7.2.1-py3-none-any.whl.zip` & `tmp/directory_forms_api_client-7.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8286 bytes, number of entries: 10
--rw-r--r--  2.0 unx       95 b- defN 23-Jul-05 15:09 directory_forms_api_client/__init__.py
--rw-r--r--  2.0 unx     3457 b- defN 23-Jul-05 15:09 directory_forms_api_client/actions.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Jul-05 15:09 directory_forms_api_client/client.py
--rw-r--r--  2.0 unx     1695 b- defN 23-Jul-05 15:09 directory_forms_api_client/forms.py
--rw-r--r--  2.0 unx     1828 b- defN 23-Jul-05 15:09 directory_forms_api_client/helpers.py
--rw-r--r--  2.0 unx     1091 b- defN 23-Jul-05 15:10 directory_forms_api_client-7.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     9887 b- defN 23-Jul-05 15:10 directory_forms_api_client-7.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 15:10 directory_forms_api_client-7.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-05 15:10 directory_forms_api_client-7.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      947 b- defN 23-Jul-05 15:10 directory_forms_api_client-7.2.1.dist-info/RECORD
-10 files, 20253 bytes uncompressed, 6630 bytes compressed:  67.3%
+Zip file size: 8287 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-06 08:57 directory_forms_api_client/__init__.py
+-rw-r--r--  2.0 unx     3457 b- defN 23-Jul-06 08:57 directory_forms_api_client/actions.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-Jul-06 08:57 directory_forms_api_client/client.py
+-rw-r--r--  2.0 unx     1695 b- defN 23-Jul-06 08:57 directory_forms_api_client/forms.py
+-rw-r--r--  2.0 unx     1828 b- defN 23-Jul-06 08:57 directory_forms_api_client/helpers.py
+-rw-r--r--  2.0 unx     1091 b- defN 23-Jul-06 08:57 directory_forms_api_client-7.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9887 b- defN 23-Jul-06 08:57 directory_forms_api_client-7.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 08:57 directory_forms_api_client-7.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 23-Jul-06 08:57 directory_forms_api_client-7.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      947 b- defN 23-Jul-06 08:57 directory_forms_api_client-7.2.2.dist-info/RECORD
+10 files, 20253 bytes uncompressed, 6631 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_forms_api_client/forms.py
 Comment: 
 
 Filename: directory_forms_api_client/helpers.py
 Comment: 
 
-Filename: directory_forms_api_client-7.2.1.dist-info/LICENSE
+Filename: directory_forms_api_client-7.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: directory_forms_api_client-7.2.1.dist-info/METADATA
+Filename: directory_forms_api_client-7.2.2.dist-info/METADATA
 Comment: 
 
-Filename: directory_forms_api_client-7.2.1.dist-info/WHEEL
+Filename: directory_forms_api_client-7.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: directory_forms_api_client-7.2.1.dist-info/top_level.txt
+Filename: directory_forms_api_client-7.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_forms_api_client-7.2.1.dist-info/RECORD
+Filename: directory_forms_api_client-7.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `directory_forms_api_client-7.2.1.dist-info/LICENSE` & `directory_forms_api_client-7.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_forms_api_client-7.2.1.dist-info/METADATA` & `directory_forms_api_client-7.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-forms-api-client
-Version: 7.2.1
+Version: 7.2.2
 Summary: Python API client for Directory forms .
 Home-page: https://github.com/uktrade/directory-forms-api-client
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -19,15 +19,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Requires-Dist: directory-client-core (<8.0.0,>=7.2.4)
+Requires-Dist: directory-client-core (<8.0.0,>=7.2.5)
 Provides-Extra: test
 Requires-Dist: django (<=4.2.3,>=2.2.10) ; extra == 'test'
 Requires-Dist: flake8 (==3.8.3) ; extra == 'test'
 Requires-Dist: pytest-codecov ; extra == 'test'
 Requires-Dist: pytest-cov ; extra == 'test'
 Requires-Dist: GitPython ; extra == 'test'
 Requires-Dist: pytest-django (==3.10.0) ; extra == 'test'
```

## Comparing `directory_forms_api_client-7.2.1.dist-info/RECORD` & `directory_forms_api_client-7.2.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 directory_forms_api_client/__init__.py,sha256=KqAK9V-nuLVYF7EzyQNFVSIC7E2O_jWWb2CtCYNPOU8,95
 directory_forms_api_client/actions.py,sha256=RZvarr9Jymd8zhesWGuSO8h3knccsmmWMNZ08OmbZ2Q,3457
 directory_forms_api_client/client.py,sha256=QWtgNsnsqDf1vXYh_QuYJHnMrlnEfEMK93b5NakiwQQ,1134
 directory_forms_api_client/forms.py,sha256=3VxOoX1KyE431TsNvjbE3EPlCf9e3F9HFXZIAqVMgb0,1695
 directory_forms_api_client/helpers.py,sha256=oz7N7YYW4FK5iwm5fWM7XwjOVndJbW3Ndr3FRMEdJNA,1828
-directory_forms_api_client-7.2.1.dist-info/LICENSE,sha256=q4QjlbTN37umB_xq3DRmS0qvT2tMO_5_-u0WWzYcDQE,1091
-directory_forms_api_client-7.2.1.dist-info/METADATA,sha256=HUm6FKLOVQvL8SUIEZmlnvv3WrUMfSIVwS8yvNW4R80,9887
-directory_forms_api_client-7.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-directory_forms_api_client-7.2.1.dist-info/top_level.txt,sha256=gv9OO61BimYYZjW7FO0hQ0kM1IUPSYZz7e83_7QBx7c,27
-directory_forms_api_client-7.2.1.dist-info/RECORD,,
+directory_forms_api_client-7.2.2.dist-info/LICENSE,sha256=q4QjlbTN37umB_xq3DRmS0qvT2tMO_5_-u0WWzYcDQE,1091
+directory_forms_api_client-7.2.2.dist-info/METADATA,sha256=TKs89YAu6Yi533BA1OUzeGiWeo235hiETBgacNMWZlQ,9887
+directory_forms_api_client-7.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+directory_forms_api_client-7.2.2.dist-info/top_level.txt,sha256=gv9OO61BimYYZjW7FO0hQ0kM1IUPSYZz7e83_7QBx7c,27
+directory_forms_api_client-7.2.2.dist-info/RECORD,,
```

