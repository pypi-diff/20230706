# Comparing `tmp/sicdeploy-0.1.8-py3-none-any.whl.zip` & `tmp/sicdeploy-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4350 bytes, number of entries: 10
+Zip file size: 4361 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 08:36 sicdeploy/__init__.py
 -rw-r--r--  2.0 unx      133 b- defN 23-Jul-06 08:56 sicdeploy/run.py
 -rw-r--r--  2.0 unx     5488 b- defN 23-Jul-06 09:02 sicdeploy/commands/build.py
 -rw-r--r--  2.0 unx      388 b- defN 23-Jul-05 18:43 sicdeploy/templates/meta.yaml.dist
 -rw-r--r--  2.0 unx      286 b- defN 23-Jul-06 09:03 sicdeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx      162 b- defN 23-Jul-06 09:03 sicdeploy-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 09:03 sicdeploy-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jul-06 09:03 sicdeploy-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-06 09:03 sicdeploy-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      812 b- defN 23-Jul-06 09:03 sicdeploy-0.1.8.dist-info/RECORD
-10 files, 7419 bytes uncompressed, 2950 bytes compressed:  60.2%
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-06 09:14 sicdeploy-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 09:14 sicdeploy-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-06 09:14 sicdeploy-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-06 09:14 sicdeploy-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      812 b- defN 23-Jul-06 09:14 sicdeploy-0.1.9.dist-info/RECORD
+10 files, 7440 bytes uncompressed, 2961 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: sicdeploy/templates/meta.yaml.dist
 Comment: 
 
 Filename: sicdeploy/templates/setup.py.dist
 Comment: 
 
-Filename: sicdeploy-0.1.8.dist-info/METADATA
+Filename: sicdeploy-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: sicdeploy-0.1.8.dist-info/WHEEL
+Filename: sicdeploy-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: sicdeploy-0.1.8.dist-info/entry_points.txt
+Filename: sicdeploy-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: sicdeploy-0.1.8.dist-info/top_level.txt
+Filename: sicdeploy-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sicdeploy-0.1.8.dist-info/RECORD
+Filename: sicdeploy-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sicdeploy-0.1.8.dist-info/RECORD` & `sicdeploy-0.1.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 sicdeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sicdeploy/run.py,sha256=2T47_CwXa-aNRO0elSi72sktwHFuCl26lTgKJh1DjP0,133
 sicdeploy/commands/build.py,sha256=a_WDm3Wkp4oh0FRlsAfUEkI6w_KqKJVIP6wbZyGziho,5488
 sicdeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sicdeploy/templates/setup.py.dist,sha256=k4vdiwd7EBEvFTALTf08iDpSjTtqlVQXy1qTtn0BdGY,286
-sicdeploy-0.1.8.dist-info/METADATA,sha256=3E-YvcchVkwpwwnQgowFK8TtfAOPEk4mAufS_YJ415U,162
-sicdeploy-0.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sicdeploy-0.1.8.dist-info/entry_points.txt,sha256=aPu7GCyg3hhhyoHkZqMj61TPF7EsyaDvqAEhvv1sxhQ,48
-sicdeploy-0.1.8.dist-info/top_level.txt,sha256=z1VdGk0Z5y2MVfM9FrJVJBlziag04X0UKyu8PIyj7tM,10
-sicdeploy-0.1.8.dist-info/RECORD,,
+sicdeploy-0.1.9.dist-info/METADATA,sha256=pjvfc13hKg0jSFyr83FVFRFKO0B8yv5jscuwPloh5Lk,183
+sicdeploy-0.1.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sicdeploy-0.1.9.dist-info/entry_points.txt,sha256=aPu7GCyg3hhhyoHkZqMj61TPF7EsyaDvqAEhvv1sxhQ,48
+sicdeploy-0.1.9.dist-info/top_level.txt,sha256=z1VdGk0Z5y2MVfM9FrJVJBlziag04X0UKyu8PIyj7tM,10
+sicdeploy-0.1.9.dist-info/RECORD,,
```

