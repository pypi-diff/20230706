# Comparing `tmp/freem_bots-0.9.0-py3-none-any.whl.zip` & `tmp/freem_bots-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 12003 bytes, number of entries: 13
+Zip file size: 12002 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      713 b- defN 22-Jan-09 21:39 freem_bots/__init__.py
 -rw-r--r--  2.0 unx      439 b- defN 22-Jan-09 21:39 freem_bots/asyncio_queue_log_handler.py
 -rw-r--r--  2.0 unx     1410 b- defN 22-Jan-09 21:39 freem_bots/configuration.py
 -rw-r--r--  2.0 unx      185 b- defN 22-Jan-09 21:39 freem_bots/demoji_wrp.py
--rw-r--r--  2.0 unx    14081 b- defN 22-Feb-25 22:39 freem_bots/discord_bot.py
+-rw-r--r--  2.0 unx    14081 b- defN 22-Feb-26 01:12 freem_bots/discord_bot.py
 -rw-rw-rw-  2.0 unx        0 b- defN 22-Jan-09 21:39 freem_bots/py.typed
 -rw-r--r--  2.0 unx      433 b- defN 22-Jan-09 21:39 freem_bots/random_provider.py
 -rw-r--r--  2.0 unx    11828 b- defN 22-Jan-09 21:39 freem_bots/tts.py
--rw-rw-rw-  2.0 unx     1051 b- defN 22-Feb-25 23:01 freem_bots-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      855 b- defN 22-Feb-25 23:01 freem_bots-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-25 23:01 freem_bots-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Feb-25 23:01 freem_bots-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1053 b- defN 22-Feb-25 23:01 freem_bots-0.9.0.dist-info/RECORD
-13 files, 32151 bytes uncompressed, 10241 bytes compressed:  68.1%
+-rw-rw-rw-  2.0 unx     1051 b- defN 22-Feb-26 01:16 freem_bots-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      855 b- defN 22-Feb-26 01:16 freem_bots-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Feb-26 01:16 freem_bots-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 22-Feb-26 01:16 freem_bots-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1053 b- defN 22-Feb-26 01:16 freem_bots-0.9.2.dist-info/RECORD
+13 files, 32151 bytes uncompressed, 10240 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: freem_bots/random_provider.py
 Comment: 
 
 Filename: freem_bots/tts.py
 Comment: 
 
-Filename: freem_bots-0.9.0.dist-info/LICENSE
+Filename: freem_bots-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: freem_bots-0.9.0.dist-info/METADATA
+Filename: freem_bots-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: freem_bots-0.9.0.dist-info/WHEEL
+Filename: freem_bots-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: freem_bots-0.9.0.dist-info/top_level.txt
+Filename: freem_bots-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: freem_bots-0.9.0.dist-info/RECORD
+Filename: freem_bots-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `freem_bots-0.9.0.dist-info/LICENSE` & `freem_bots-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `freem_bots-0.9.0.dist-info/METADATA` & `freem_bots-0.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freem-bots
-Version: 0.9.0
+Version: 0.9.2
 Summary: Abstractions over Discord with simple TTS voice support
 Home-page: https://gitlab.com/torsten-projects/freem-bots
 Author: Jakub Rohla
 Author-email: freemanovec@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `freem_bots-0.9.0.dist-info/RECORD` & `freem_bots-0.9.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 freem_bots/asyncio_queue_log_handler.py,sha256=hYatnzFlpoBiecQXJh1id_yiVhbvnt9dg_DSP_5TmvE,439
 freem_bots/configuration.py,sha256=xL4ScIDt4sINMev8u-jAnLH_YjcTQI03fhuDdInd0SU,1410
 freem_bots/demoji_wrp.py,sha256=iiBY76iiCZGnBuN8gK95iunpW8_2O5s7hdq8BYHmaWE,185
 freem_bots/discord_bot.py,sha256=W8OtUGtuHIr2UiiIrID-2Db7FP8o8wXwYw1tWcek__s,14081
 freem_bots/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 freem_bots/random_provider.py,sha256=69vqf5QLu_RtBpQR8l0n8tvaHfZPqOx-w8MDR-HVci8,433
 freem_bots/tts.py,sha256=Sm2zOBervIXpil5y6u6vCf-mHXu3AmVpSFhdGmwvOUc,11828
-freem_bots-0.9.0.dist-info/LICENSE,sha256=HDdi-_VkM84Y05Jtn2CioIFdDThh5oCjvFmZLqSPfbc,1051
-freem_bots-0.9.0.dist-info/METADATA,sha256=f3k5jdlexr8Ok4SFwnOqCDfu9xCkUJkIC0FHX98xngQ,855
-freem_bots-0.9.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-freem_bots-0.9.0.dist-info/top_level.txt,sha256=t3J-AaAbwdyAIfgJ6uj-uFaCWQLFUmnFmnOhycqRnmM,11
-freem_bots-0.9.0.dist-info/RECORD,,
+freem_bots-0.9.2.dist-info/LICENSE,sha256=HDdi-_VkM84Y05Jtn2CioIFdDThh5oCjvFmZLqSPfbc,1051
+freem_bots-0.9.2.dist-info/METADATA,sha256=Q2yu0KrvanDduUzxzqO_rpAAjpF-Tr2d1z5FVwhuFMs,855
+freem_bots-0.9.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+freem_bots-0.9.2.dist-info/top_level.txt,sha256=t3J-AaAbwdyAIfgJ6uj-uFaCWQLFUmnFmnOhycqRnmM,11
+freem_bots-0.9.2.dist-info/RECORD,,
```

