# Comparing `tmp/dopplrSDK-2.7.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-2.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4941 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    11035 b- defN 23-Jun-27 08:59 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      622 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 23-Jun-27 09:01 dopplrSDK-2.7.0.dist-info/RECORD
-6 files, 13314 bytes uncompressed, 4075 bytes compressed:  69.4%
+Zip file size: 5195 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    11876 b- defN 23-Jul-06 08:11 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-06 08:11 dopplrSDK-2.8.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      622 b- defN 23-Jul-06 08:11 dopplrSDK-2.8.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 08:11 dopplrSDK-2.8.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-06 08:11 dopplrSDK-2.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 23-Jul-06 08:11 dopplrSDK-2.8.0.dist-info/RECORD
+6 files, 14155 bytes uncompressed, 4329 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-2.7.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-2.8.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-2.7.0.dist-info/METADATA
+Filename: dopplrSDK-2.8.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-2.7.0.dist-info/WHEEL
+Filename: dopplrSDK-2.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-2.7.0.dist-info/top_level.txt
+Filename: dopplrSDK-2.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-2.7.0.dist-info/RECORD
+Filename: dopplrSDK-2.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -92,16 +92,15 @@
 
         UserKey=results[1]
         OrgName=results[0]
         
         cur=cnxn.cursor()
         file_name = os.path.basename(filePath)
         file_name1=file_name.split('.')
-        query="select count(\"TableName\") from doppler.\"DopplerLake\" where \"Source\"='MLStudio' and \"TableName\"="+"'"+file_name1[0]+"'"
- 
+        query="select count(\"TableName\") from doppler.\"DopplerLake\" DL join doppler.\"DopplerUser\" US on DL.\"UserKey\"=US.\"UserKey\" where \"Source\"='MLStudio' and \"TableName\"="+"'"+file_name1[0]+"'"+" and US.\"LoginName\"="+"'"+loginName+"'"
         cur.execute(query)
         results = cur.fetchone()
         if results[0]<1:
             insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name1[0]+"','"+file_type+"',null,'','Uploaded')"
             cur.execute(insert_query)
             cnxn.commit()
         else:
@@ -111,21 +110,39 @@
         insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM doppler.\"DopplerLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name1[0]+"'"
         
         cur1.execute(insert_query1)
         results = cur1.fetchone()
         SourceKey=results[0]
         SourceKey=str(SourceKey)
 
+        df = pd.read_csv(filePath)
+        cur_del=cnxn.cursor()
+        delete="DELETE FROM Doppler.\"DopplerSchema\" WHERE\"SourceKey\"="+SourceKey
+        cur_del.execute(delete)
+        cnxn.commit()
+        cur_sch=cnxn.cursor()
+        for name, dtype in df.dtypes.iteritems():
+            if(dtype == 'datetime64[ns]'):
+                dtype = 'Datetime'
+            maxlength = max(df[name].map(str).apply(len))
+            tpp=str(maxlength)
+            tp=str(dtype)
+            insert1="INSERT INTO doppler.\"DopplerSchema\"(\"SourceKey\",\"Column\" ,\"Type\",\"Length\") VALUES ({},'{}','{}','{}')".format(SourceKey,name,tp,tpp)
+            cur_sch.execute(insert1)
+            cnxn.commit()
+
 
-        ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/SOURCE/'+file_name)
-        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/SOURCE/'+file_name+"',\"Source\"= 'MLStudio' ,\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
+        ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/Source/'+file_name)
+        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/Source/'+file_name+"',\"Source\"= 'MLStudio' ,\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
         cur2=cnxn.cursor()
 
         cur2.execute(update_query)
         cnxn.commit()
+
+        
         if keys['Cloud'] == 'MinIO'or keys['Cloud'] =='AWS':
             
             client.upload_file(filePath, ContainerName, ConnectionString)
              # Generate a pre-signed URL        
             client.put_object_acl(ACL='public-read',
                               Bucket=ContainerName,
                               Key=ConnectionString)
```

## Comparing `dopplrSDK-2.7.0.dist-info/LICENSE.txt` & `dopplrSDK-2.8.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-2.7.0.dist-info/METADATA` & `dopplrSDK-2.8.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 2.7.0
+Version: 2.8.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

