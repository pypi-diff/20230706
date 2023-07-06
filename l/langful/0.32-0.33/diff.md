# Comparing `tmp/langful-0.32-py3-none-any.whl.zip` & `tmp/langful-0.33-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5419 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      224 b- defN 23-Jun-20 12:20 langful/__init__.py
--rw-rw-rw-  2.0 fat     9963 b- defN 23-Jul-04 11:45 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      527 b- defN 23-Jul-04 11:52 langful-0.32.dist-info/RECORD
-7 files, 15269 bytes uncompressed, 4489 bytes compressed:  70.6%
+Zip file size: 5446 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
+-rw-rw-rw-  2.0 fat    10230 b- defN 23-Jul-06 06:51 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jul-06 08:49 langful-0.33.dist-info/RECORD
+7 files, 15479 bytes uncompressed, 4516 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.32.dist-info/LICENSE
+Filename: langful-0.33.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.32.dist-info/METADATA
+Filename: langful-0.33.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.32.dist-info/WHEEL
+Filename: langful-0.33.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.32.dist-info/top_level.txt
+Filename: langful-0.33.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.32.dist-info/RECORD
+Filename: langful-0.33.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/__init__.py

```diff
@@ -1,15 +1,13 @@
 """
 # langful
 
 Help to localization
 
 # About
 
-github: https://github.com/cueavyqwp/langful
+github: https://github.com/cueavy/langful
 
 pypi: https://pypi.org/project/langful
-
-issues: https://github.com/cueavyqwp/langful/issues
 """
 
 from .lang import *
```

## langful/lang.py

```diff
@@ -237,29 +237,35 @@
     def lang_del( self , locale : str ) -> None :
         """
         del a lang
         """
         del self.languages[ locale ]
         del self.types[ locale ]
 
-    def get( self , key : str | int , locale : str = None ) -> str :
+    def lang_merge( self , to : str , locale : str = None , args : str | list = [] ) -> None :
+        """
+        merge to a locale
+        """
+        self.lang_set( to , self.merge( locale , args ) )
+
+    def get( self , key : str , locale : str = None ) -> str :
         """
         get the key by a locale dictionary
         """
         locale = self.locale_get( locale )
         return self.languages[ locale ][ key ]
 
-    def set( self , key : str | int , value : str , locale : str = None ) -> None :
+    def set( self , key : str , value : str , locale : str = None ) -> None :
         """
         set a value by a locale dictionary
         """
         locale = self.locale_get( locale )
         self.languages[ locale ][ key ] = value
 
-    def remove( self , key : str | int , locale : str = None ) -> None :
+    def remove( self , key : str , locale : str = None ) -> None :
         """
         remove a value by a locale dictionary
         """
         locale = self.locale_get( locale )
         del self.languages[ locale ][ key ]
 
     def save( self , separators : list = [ " ," , ": " ] ) -> None :
@@ -272,25 +278,27 @@
                 with open( os.path.join( self.lang_dir , key + suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         file.write( json.dumps( value , indent = 4 , separators = separators , ensure_ascii = False ) )
                     elif suffix == ".lang" :
                         file.write( to_lang( value ) )
         return self.languages
 
-    def merge( self , locale : str = None , args : list = [] ) -> dict :
+    def merge( self , locale : str = None , args : str | list = [] ) -> dict :
         """
         merge
         """
+        if isinstance( args , str ) :
+            args = [ args ]
         ret = self.lang_get( self.locale_get( locale ) )
         for i in args :
             for key , value in self.lang_get( i ).items() :
                 ret[ key ] = value
         return ret
 
-    def replace( self , key : str = None , args : list | str = None , locale : str = None , replace_letter : str = None ) -> str :
+    def replace( self , key : str = None , args : str | list  = None , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace
         """
         replace_letter = self.replace_letter_get( replace_letter )
         locale = self.locale_get( locale )
         text = self.get( key , locale ).split( replace_letter )
         if isinstance( args , str ) :
```

## Comparing `langful-0.32.dist-info/LICENSE` & `langful-0.33.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.32.dist-info/METADATA` & `langful-0.33.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.32
+Version: 0.33
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `langful-0.32.dist-info/RECORD` & `langful-0.33.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-langful/__init__.py,sha256=81IWJcsG-rF5MEPRQOPJcbnRgs3n1KvcLUeWUiHp8nI,224
-langful/lang.py,sha256=rV6Sym9m2fJj_nAF2q3nr1eweOqpBTsKakSYeFu7W3o,9963
-langful-0.32.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
-langful-0.32.dist-info/METADATA,sha256=aB6dvK-bIsIEEchBNJdXPR8WWbzxEpLdscS3Dqw0B5M,3389
-langful-0.32.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-langful-0.32.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.32.dist-info/RECORD,,
+langful/__init__.py,sha256=BSJ-BT1Yr3Xz-SFnmZu7QvgV5pgg2WEqUO42oM3Py2w,166
+langful/lang.py,sha256=gUPQ33vasv1NLBBXKwXpaxAlihseIvGeTA-2YWJDCwQ,10230
+langful-0.33.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
+langful-0.33.dist-info/METADATA,sha256=ZwGECitWv1iw4GfaygZaDMyR5qOjDG_9jcOWLF1qUFs,3389
+langful-0.33.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+langful-0.33.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.33.dist-info/RECORD,,
```

