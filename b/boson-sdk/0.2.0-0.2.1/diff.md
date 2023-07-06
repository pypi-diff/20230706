# Comparing `tmp/boson_sdk-0.2.0-py3-none-any.whl.zip` & `tmp/boson_sdk-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 20531 bytes, number of entries: 15
--rw-r--r--  2.0 unx      749 b- defN 23-Jun-02 17:56 boson/__init__.py
--rw-r--r--  2.0 unx     4209 b- defN 23-Jun-02 17:56 boson/base.py
--rw-r--r--  2.0 unx     5320 b- defN 23-Jun-02 17:56 boson/boson_v1_pb2.py
--rw-r--r--  2.0 unx     3684 b- defN 23-Jun-02 17:56 boson/conversion.py
--rw-r--r--  2.0 unx     7772 b- defN 23-Jun-02 17:56 boson/features_pb2.py
--rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 17:56 boson/grpc/__init__.py
--rw-r--r--  2.0 unx     5518 b- defN 23-Jun-02 17:56 boson/grpc/boson_v1_pb2_grpc.py
--rw-r--r--  2.0 unx     2159 b- defN 23-Jun-02 17:56 boson/grpc/server.py
--rw-r--r--  2.0 unx       57 b- defN 23-Jun-02 17:56 boson/http/__init__.py
--rw-r--r--  2.0 unx     2568 b- defN 23-Jun-02 17:56 boson/http/server.py
--rw-r--r--  2.0 unx    11356 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14911 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1168 b- defN 23-Jun-02 17:57 boson_sdk-0.2.0.dist-info/RECORD
-15 files, 59626 bytes uncompressed, 18619 bytes compressed:  68.8%
+Zip file size: 20524 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      749 b- defN 23-Jul-06 17:16 boson/__init__.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Jul-06 17:16 boson/base.py
+-rw-r--r--  2.0 unx     5320 b- defN 23-Jul-06 17:16 boson/boson_v1_pb2.py
+-rw-r--r--  2.0 unx     3684 b- defN 23-Jul-06 17:16 boson/conversion.py
+-rw-r--r--  2.0 unx     7772 b- defN 23-Jul-06 17:16 boson/features_pb2.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-06 17:16 boson/grpc/__init__.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-Jul-06 17:16 boson/grpc/boson_v1_pb2_grpc.py
+-rw-r--r--  2.0 unx     2159 b- defN 23-Jul-06 17:16 boson/grpc/server.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-06 17:16 boson/http/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Jul-06 17:16 boson/http/server.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jul-06 17:17 boson_sdk-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14911 b- defN 23-Jul-06 17:17 boson_sdk-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 17:17 boson_sdk-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-06 17:17 boson_sdk-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1168 b- defN 23-Jul-06 17:17 boson_sdk-0.2.1.dist-info/RECORD
+15 files, 59626 bytes uncompressed, 18612 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: boson/http/__init__.py
 Comment: 
 
 Filename: boson/http/server.py
 Comment: 
 
-Filename: boson_sdk-0.2.0.dist-info/LICENSE
+Filename: boson_sdk-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: boson_sdk-0.2.0.dist-info/METADATA
+Filename: boson_sdk-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: boson_sdk-0.2.0.dist-info/WHEEL
+Filename: boson_sdk-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: boson_sdk-0.2.0.dist-info/top_level.txt
+Filename: boson_sdk-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: boson_sdk-0.2.0.dist-info/RECORD
+Filename: boson_sdk-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## boson/boson_v1_pb2.py

```diff
@@ -12,22 +12,22 @@
 
 
 import boson.features_pb2 as features__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x62oson_v1.proto\x12\x0f\x62osonproviderv1\x1a\x0e\x66\x65\x61tures.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x14\n\x12\x44\x61tasetInfoRequest\"\xb1\x02\n\rSearchRequest\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\x12,\n\x08\x64\x61tetime\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x63ollections\x18\x05 \x03(\t\x12\x13\n\x0b\x66\x65\x61ture_ids\x18\x06 \x03(\t\x12\'\n\x06\x66ields\x18\x07 \x01(\x0b\x32\x17.bosonproviderv1.Fields\x12(\n\x07sort_by\x18\x08 \x03(\x0b\x32\x17.bosonproviderv1.SortBy\x12\r\n\x05limit\x18\t \x01(\x05\x12\x12\n\nintersects\x18\n \x01(\x0c\x12\x0c\n\x04page\x18\x0b \x01(\x05\x12\r\n\x05token\x18\x0c \x01(\t\"*\n\x06\x46ields\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"*\n\x06SortBy\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\tdirection\x18\x02 \x01(\t\"\xd8\x04\n\x0bWarpRequest\x12\x1f\n\x17input_spatial_reference\x18\x01 \x01(\t\x12 \n\x18output_spatial_reference\x18\x02 \x01(\t\x12\'\n\x1foutput_extent_spatial_reference\x18\x03 \x01(\t\x12\x19\n\x11output_pixel_size\x18\x04 \x03(\x01\x12\x15\n\routput_extent\x18\x05 \x03(\x01\x12\x1b\n\x13output_extent_wgs84\x18\x06 \x03(\x01\x12\x14\n\x0coutput_shape\x18\x07 \x03(\x04\x12\x12\n\npixel_type\x18\x08 \x01(\t\x12\x19\n\x11resampling_method\x18\t \x01(\t\x12-\n\rinput_no_data\x18\n \x03(\x0b\x32\x16.google.protobuf.Value\x12.\n\x0eoutput_no_data\x18\x0b \x03(\x0b\x32\x16.google.protobuf.Value\x12\x14\n\x0c\x63ontent_type\x18\x0c \x01(\t\x12\x30\n\x0ctime_instant\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ntime_range\x18\x0e \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0b\x61sset_bands\x18\x0f \x03(\x0b\x32\x1b.bosonproviderv1.AssetBands\x12\x17\n\x0finput_filepaths\x18\x10 \x03(\t\x12\'\n\x06\x66ilter\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\"C\n\nAssetBands\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12&\n\x05\x62\x61nds\x18\x02 \x03(\x0b\x32\x17.bosonproviderv1.BandID\"\"\n\x06\x42\x61ndID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x05\"\xf1\x01\n\x13\x44\x61tasetInfoResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\'\n\x0eoverall_extent\x18\x04 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x10\n\x08min_zoom\x18\x05 \x01(\x05\x12\x10\n\x08max_zoom\x18\x06 \x01(\x05\x12\x13\n\x0b\x63onforms_to\x18\x07 \x03(\t\x12\x1c\n\x05links\x18\x08 \x03(\x0b\x32\r.gogc.LinkMsg\x12(\n\x0b\x63ollections\x18\t \x03(\x0b\x32\x13.gogc.CollectionMsg\"W\n\x0eSearchResponse\x12\x36\n\x12\x66\x65\x61ture_collection\x18\x01 \x01(\x0b\x32\x1a.gogc.FeatureCollectionMsg\x12\r\n\x05token\x18\x02 \x01(\t\"n\n\x0eRasterResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\r\x12\x12\n\npixel_type\x18\x04 \x01(\t\x12\x15\n\rgeo_transform\x18\x05 \x03(\x01\x32\x83\x02\n\x0f\x42osonProviderV1\x12Z\n\x0b\x44\x61tasetInfo\x12#.bosonproviderv1.DatasetInfoRequest\x1a$.bosonproviderv1.DatasetInfoResponse\"\x00\x12K\n\x06Search\x12\x1e.bosonproviderv1.SearchRequest\x1a\x1f.bosonproviderv1.SearchResponse\"\x00\x12G\n\x04Warp\x12\x1c.bosonproviderv1.WarpRequest\x1a\x1f.bosonproviderv1.RasterResponse\"\x00\x42/Z-github.com/seerai/boson/server/v1/impl/remoteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x62oson_v1.proto\x12\x0f\x62osonproviderv1\x1a\x0e\x66\x65\x61tures.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x14\n\x12\x44\x61tasetInfoRequest\"\xb1\x02\n\rSearchRequest\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\x12,\n\x08\x64\x61tetime\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x63ollections\x18\x05 \x03(\t\x12\x13\n\x0b\x66\x65\x61ture_ids\x18\x06 \x03(\t\x12\'\n\x06\x66ields\x18\x07 \x01(\x0b\x32\x17.bosonproviderv1.Fields\x12(\n\x07sort_by\x18\x08 \x03(\x0b\x32\x17.bosonproviderv1.SortBy\x12\r\n\x05limit\x18\t \x01(\x05\x12\x12\n\nintersects\x18\n \x01(\x0c\x12\x0c\n\x04page\x18\x0b \x01(\x05\x12\r\n\x05token\x18\x0c \x01(\t\"*\n\x06\x46ields\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"*\n\x06SortBy\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\tdirection\x18\x02 \x01(\t\"\xd8\x04\n\x0bWarpRequest\x12\x1f\n\x17input_spatial_reference\x18\x01 \x01(\t\x12 \n\x18output_spatial_reference\x18\x02 \x01(\t\x12\'\n\x1foutput_extent_spatial_reference\x18\x03 \x01(\t\x12\x19\n\x11output_pixel_size\x18\x04 \x03(\x01\x12\x15\n\routput_extent\x18\x05 \x03(\x01\x12\x1b\n\x13output_extent_wgs84\x18\x06 \x03(\x01\x12\x14\n\x0coutput_shape\x18\x07 \x03(\x04\x12\x12\n\npixel_type\x18\x08 \x01(\t\x12\x19\n\x11resampling_method\x18\t \x01(\t\x12-\n\rinput_no_data\x18\n \x03(\x0b\x32\x16.google.protobuf.Value\x12.\n\x0eoutput_no_data\x18\x0b \x03(\x0b\x32\x16.google.protobuf.Value\x12\x14\n\x0c\x63ontent_type\x18\x0c \x01(\t\x12\x30\n\x0ctime_instant\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ntime_range\x18\x0e \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0b\x61sset_bands\x18\x0f \x03(\x0b\x32\x1b.bosonproviderv1.AssetBands\x12\x17\n\x0finput_filepaths\x18\x10 \x03(\t\x12\'\n\x06\x66ilter\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\"C\n\nAssetBands\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12&\n\x05\x62\x61nds\x18\x02 \x03(\x0b\x32\x17.bosonproviderv1.BandID\"\"\n\x06\x42\x61ndID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x05\"\xf1\x01\n\x13\x44\x61tasetInfoResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\'\n\x0eoverall_extent\x18\x04 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x10\n\x08min_zoom\x18\x05 \x01(\x05\x12\x10\n\x08max_zoom\x18\x06 \x01(\x05\x12\x13\n\x0b\x63onforms_to\x18\x07 \x03(\t\x12\x1c\n\x05links\x18\x08 \x03(\x0b\x32\r.gogc.LinkMsg\x12(\n\x0b\x63ollections\x18\t \x03(\x0b\x32\x13.gogc.CollectionMsg\"W\n\x0eSearchResponse\x12\x36\n\x12\x66\x65\x61ture_collection\x18\x01 \x01(\x0b\x32\x1a.gogc.FeatureCollectionMsg\x12\r\n\x05token\x18\x02 \x01(\t\"n\n\x0eRasterResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\r\x12\x12\n\npixel_type\x18\x04 \x01(\t\x12\x15\n\rgeo_transform\x18\x05 \x03(\x01\x32\x83\x02\n\x0f\x42osonProviderV1\x12Z\n\x0b\x44\x61tasetInfo\x12#.bosonproviderv1.DatasetInfoRequest\x1a$.bosonproviderv1.DatasetInfoResponse\"\x00\x12K\n\x06Search\x12\x1e.bosonproviderv1.SearchRequest\x1a\x1f.bosonproviderv1.SearchResponse\"\x00\x12G\n\x04Warp\x12\x1c.bosonproviderv1.WarpRequest\x1a\x1f.bosonproviderv1.RasterResponse\"\x00\x42/Z-github.com/seerai/boson-core/providers/remoteb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'boson_v1_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/seerai/boson/server/v1/impl/remote'
+  DESCRIPTOR._serialized_options = b'Z-github.com/seerai/boson-core/providers/remote'
   _DATASETINFOREQUEST._serialized_start=114
   _DATASETINFOREQUEST._serialized_end=134
   _SEARCHREQUEST._serialized_start=137
   _SEARCHREQUEST._serialized_end=442
   _FIELDS._serialized_start=444
   _FIELDS._serialized_end=486
   _SORTBY._serialized_start=488
```

## Comparing `boson_sdk-0.2.0.dist-info/LICENSE` & `boson_sdk-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `boson_sdk-0.2.0.dist-info/METADATA` & `boson_sdk-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boson-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for Boson Geospatial Service Mesh Providers
 Author-email: The SeerAI Team <contact@seer.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `boson_sdk-0.2.0.dist-info/RECORD` & `boson_sdk-0.2.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 boson/__init__.py,sha256=Xnoa1_beJWNJ7vMFMhJdJM3cMKOQzvK0cwnlh7GsprA,749
 boson/base.py,sha256=-HsRg75UFtc2V66HaT7-5ENJraDbfT8pPNh2JPskai0,4209
-boson/boson_v1_pb2.py,sha256=3SDZu0ktfhwRGkjrXDliI_uOQIYgZnqvGSTnF3Z7SEE,5320
+boson/boson_v1_pb2.py,sha256=acILI95zY6PPF7KyaJ2DQzYBKMOk3UeNUNlsWm-QV6E,5320
 boson/conversion.py,sha256=nOq_qjpjMRt9FV89OBLbiJQS8KG9KGVvv1_Zn4KS6Dw,3684
 boson/features_pb2.py,sha256=2pAy93Dujdq3k3p_rHNDMR_k-K8sUZG75RfABH8F_Wo,7772
 boson/grpc/__init__.py,sha256=Z1VcMBg4TgrsHfO7jI7pyAZ0jKzJ1ya4gn5gwJkYGp8,57
 boson/grpc/boson_v1_pb2_grpc.py,sha256=aL02_ezWzSWJIDy5n2mxCswmGA4bMyXbGkU6FURivGo,5518
 boson/grpc/server.py,sha256=XBMosGe56I827E00QGUsIngyZiWUyfAo0hbDNFamYLA,2159
 boson/http/__init__.py,sha256=1J3MipaATnk1VFxmMV0uXeW7DWrD9t6vfcDlHOEjyrA,57
 boson/http/server.py,sha256=Q2gKtPCyXenaxNRUNkZF28FvuzcqRmtDLICA-Wrbx6k,2568
-boson_sdk-0.2.0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-boson_sdk-0.2.0.dist-info/METADATA,sha256=hch7EbBGhlR3WQ25E--h2ioC18izNBABEoq7U8jjGlo,14911
-boson_sdk-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-boson_sdk-0.2.0.dist-info/top_level.txt,sha256=a05hL1bKBp1M9A2czOQcnAZrKe63bhOjgjTAf4ri-4c,6
-boson_sdk-0.2.0.dist-info/RECORD,,
+boson_sdk-0.2.1.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+boson_sdk-0.2.1.dist-info/METADATA,sha256=RZ1-gMeuitXhx8jKiKdRvTndFA24yzMk7UoX7rnq8Hk,14911
+boson_sdk-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+boson_sdk-0.2.1.dist-info/top_level.txt,sha256=a05hL1bKBp1M9A2czOQcnAZrKe63bhOjgjTAf4ri-4c,6
+boson_sdk-0.2.1.dist-info/RECORD,,
```

