# Comparing `tmp/tesseract_sdk-0.7.0-py3-none-any.whl.zip` & `tmp/tesseract_sdk-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 28213 bytes, number of entries: 19
--rw-r--r--  2.0 unx      174 b- defN 23-Mar-27 22:31 tesseract/__init__.py
--rw-r--r--  2.0 unx     7866 b- defN 23-Mar-27 22:31 tesseract/_logging.py
--rw-r--r--  2.0 unx     1215 b- defN 23-Mar-27 22:31 tesseract/error_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-27 22:31 tesseract/error_pb2_grpc.py
--rw-r--r--  2.0 unx     2446 b- defN 23-Mar-27 22:31 tesseract/extract.py
--rw-r--r--  2.0 unx      455 b- defN 23-Mar-27 22:31 tesseract/features.py
--rw-r--r--  2.0 unx     8528 b- defN 23-Mar-27 22:31 tesseract/features_pb2.py
--rw-r--r--  2.0 unx     3240 b- defN 23-Mar-27 22:31 tesseract/inference_pb2.py
--rw-r--r--  2.0 unx     4125 b- defN 23-Mar-27 22:31 tesseract/inference_pb2_grpc.py
--rw-r--r--  2.0 unx     8065 b- defN 23-Mar-27 22:31 tesseract/server.py
--rw-r--r--  2.0 unx      535 b- defN 23-Mar-27 22:31 tesseract/tensor.py
--rw-r--r--  2.0 unx    15769 b- defN 23-Mar-27 22:31 tesseract/validate.py
--rw-r--r--  2.0 unx     1637 b- defN 23-Mar-27 22:31 tesseract/scripts/validate.py
--rw-r--r--  2.0 unx    11356 b- defN 23-Mar-27 22:31 tesseract_sdk-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14839 b- defN 23-Mar-27 22:31 tesseract_sdk-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 22:31 tesseract_sdk-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 23-Mar-27 22:31 tesseract_sdk-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Mar-27 22:31 tesseract_sdk-0.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1559 b- defN 23-Mar-27 22:31 tesseract_sdk-0.7.0.dist-info/RECORD
-19 files, 82136 bytes uncompressed, 25673 bytes compressed:  68.7%
+Zip file size: 28357 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-20 22:08 tesseract/__init__.py
+-rw-r--r--  2.0 unx     7866 b- defN 23-Jun-20 22:08 tesseract/_logging.py
+-rw-r--r--  2.0 unx     1215 b- defN 23-Jun-20 22:08 tesseract/error_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-20 22:08 tesseract/error_pb2_grpc.py
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-20 22:08 tesseract/extract.py
+-rw-r--r--  2.0 unx      455 b- defN 23-Jun-20 22:08 tesseract/features.py
+-rw-r--r--  2.0 unx     7772 b- defN 23-Jun-20 22:08 tesseract/features_pb2.py
+-rw-r--r--  2.0 unx     2866 b- defN 23-Jun-20 22:08 tesseract/inference_pb2.py
+-rw-r--r--  2.0 unx     4125 b- defN 23-Jun-20 22:08 tesseract/inference_pb2_grpc.py
+-rw-r--r--  2.0 unx     9022 b- defN 23-Jun-20 22:08 tesseract/server.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Jun-20 22:08 tesseract/tensor.py
+-rw-r--r--  2.0 unx    16221 b- defN 23-Jun-20 22:08 tesseract/validate.py
+-rw-r--r--  2.0 unx     1626 b- defN 23-Jun-20 22:08 tesseract/scripts/validate.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jun-20 22:09 tesseract_sdk-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14839 b- defN 23-Jun-20 22:09 tesseract_sdk-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 22:09 tesseract_sdk-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-20 22:09 tesseract_sdk-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-20 22:09 tesseract_sdk-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-20 22:09 tesseract_sdk-0.8.0.dist-info/RECORD
+19 files, 82404 bytes uncompressed, 25817 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: tesseract/validate.py
 Comment: 
 
 Filename: tesseract/scripts/validate.py
 Comment: 
 
-Filename: tesseract_sdk-0.7.0.dist-info/LICENSE
+Filename: tesseract_sdk-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: tesseract_sdk-0.7.0.dist-info/METADATA
+Filename: tesseract_sdk-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: tesseract_sdk-0.7.0.dist-info/WHEEL
+Filename: tesseract_sdk-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: tesseract_sdk-0.7.0.dist-info/entry_points.txt
+Filename: tesseract_sdk-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: tesseract_sdk-0.7.0.dist-info/top_level.txt
+Filename: tesseract_sdk-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tesseract_sdk-0.7.0.dist-info/RECORD
+Filename: tesseract_sdk-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tesseract/features_pb2.py

```diff
@@ -11,68 +11,60 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x66\x65\x61tures.proto\x12\x04gogc\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xea\x03\n\rCollectionMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x12\x0f\n\x07license\x18\x05 \x01(\t\x12\x1f\n\x06\x65xtent\x18\x06 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x1c\n\x05links\x18\x07 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x12\n\nextensions\x18\t \x03(\t\x12$\n\tproviders\x18\n \x03(\x0b\x32\x11.gogc.ProviderMsg\x12\x35\n\tsummaries\x18\x0b \x03(\x0b\x32\".gogc.CollectionMsg.SummariesEntry\x12\x38\n\x0bitem_assets\x18\x0c \x03(\x0b\x32#.gogc.CollectionMsg.ItemAssetsEntry\x1aH\n\x0eSummariesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a\x41\n\x0fItemAssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xb8\x01\n\x14\x46\x65\x61tureCollectionMsg\x12\"\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x10.gogc.FeatureMsg\x12\x1c\n\x05links\x18\x02 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x16\n\x0enumber_matched\x18\x03 \x01(\x03\x12\x17\n\x0fnumber_returned\x18\x04 \x01(\x03\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8b\x03\n\nFeatureMsg\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\x12\x10\n\x08geometry\x18\x03 \x01(\x0c\x12\x0c\n\x04\x62\x62ox\x18\x04 \x03(\x01\x12\x34\n\nproperties\x18\x05 \x03(\x0b\x32 .gogc.FeatureMsg.PropertiesEntry\x12\x1c\n\x05links\x18\x06 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x07 \x01(\t\x12\x12\n\nextensions\x18\x08 \x03(\t\x12,\n\x06\x61ssets\x18\t \x03(\x0b\x32\x1c.gogc.FeatureMsg.AssetsEntry\x12\x12\n\ncollection\x18\n \x01(\t\x1aI\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a=\n\x0b\x41ssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xbe\x02\n\x08\x41ssetMsg\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04href\x18\x04 \x01(\t\x12\r\n\x05roles\x18\x05 \x03(\t\x12!\n\x08\x65o_bands\x18\x06 \x03(\x0b\x32\x0f.gogc.EOBandMsg\x12)\n\x0craster_bands\x18\x07 \x03(\x0b\x32\x13.gogc.RasterBandMsg\x12!\n\x07storage\x18\t \x01(\x0b\x32\x10.gogc.StorageMsg\x12\x30\n\talternate\x18\n \x03(\x0b\x32\x1d.gogc.AssetMsg.AlternateEntry\x1a@\n\x0e\x41lternateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"T\n\nStorageMsg\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x16\n\x0erequester_pays\x18\x03 \x01(\x08\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\xa4\x01\n\tEOBandMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommon_name\x18\x02 \x01(\t\x12\x0b\n\x03gsd\x18\x03 \x01(\x01\x12\x19\n\x11\x63\x65nter_wavelength\x18\x04 \x01(\x01\x12\x1b\n\x13\x66ull_width_half_max\x18\x05 \x01(\x01\x12\x1a\n\x12solar_illumination\x18\x06 \x01(\x01\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x9b\x02\n\rRasterBandMsg\x12\'\n\x07no_data\x18\x01 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x10\n\x08sampling\x18\x02 \x01(\t\x12\x11\n\tdata_type\x18\x03 \x01(\t\x12\x17\n\x0f\x62its_per_sample\x18\x04 \x01(\x05\x12\x1a\n\x12spatial_resolution\x18\x05 \x01(\x01\x12-\n\nstatistics\x18\x06 \x01(\x0b\x32\x19.gogc.RasterStatisticsMsg\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\r\n\x05scale\x18\x08 \x01(\x01\x12\x0e\n\x06offset\x18\t \x01(\x01\x12+\n\thistogram\x18\n \x01(\x0b\x32\x18.gogc.RasterHistogramMsg\"l\n\x13RasterStatisticsMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x01\x12\x0f\n\x07minimum\x18\x02 \x01(\x01\x12\x0f\n\x07maximum\x18\x03 \x01(\x01\x12\x0e\n\x06stddev\x18\x04 \x01(\x01\x12\x15\n\rvalid_percent\x18\x05 \x01(\x01\"N\n\x12RasterHistogramMsg\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0f\n\x07\x62uckets\x18\x04 \x03(\x04\"_\n\tExtentMsg\x12\'\n\x07spatial\x18\x01 \x03(\x0b\x32\x16.gogc.SpatialExtentMsg\x12)\n\x08temporal\x18\x02 \x03(\x0b\x32\x17.gogc.TemporalExtentMsg\" \n\x10SpatialExtentMsg\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\"A\n\x11TemporalExtentMsg\x12,\n\x08interval\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x02\n\x07LinkMsg\x12\x0c\n\x04href\x18\x01 \x01(\t\x12\x0b\n\x03rel\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08hreflang\x18\x04 \x01(\t\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06length\x18\x06 \x01(\x03\x12\x0e\n\x06method\x18\x07 \x01(\t\x12+\n\x07headers\x18\x08 \x03(\x0b\x32\x1a.gogc.LinkMsg.HeadersEntry\x12%\n\x04\x62ody\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05merge\x18\n \x01(\x08\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"L\n\x0bProviderMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\x12\x0b\n\x03url\x18\x04 \x01(\tB!Z\x1fgithub.com/seerai/gogc/featuresb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x66\x65\x61tures.proto\x12\x04gogc\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x95\x03\n\rCollectionMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x12\x0f\n\x07license\x18\x05 \x01(\t\x12\x1f\n\x06\x65xtent\x18\x06 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x1c\n\x05links\x18\x07 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x12\n\nextensions\x18\t \x03(\t\x12$\n\tproviders\x18\n \x03(\x0b\x32\x11.gogc.ProviderMsg\x12*\n\tsummaries\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x38\n\x0bitem_assets\x18\x0c \x03(\x0b\x32#.gogc.CollectionMsg.ItemAssetsEntry\x1a\x41\n\x0fItemAssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xb8\x01\n\x14\x46\x65\x61tureCollectionMsg\x12\"\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x10.gogc.FeatureMsg\x12\x1c\n\x05links\x18\x02 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x16\n\x0enumber_matched\x18\x03 \x01(\x03\x12\x17\n\x0fnumber_returned\x18\x04 \x01(\x03\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x02\n\nFeatureMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08geometry\x18\x02 \x01(\x0c\x12\x0c\n\x04\x62\x62ox\x18\x03 \x03(\x01\x12+\n\nproperties\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1c\n\x05links\x18\x05 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x12\n\nextensions\x18\x07 \x03(\t\x12,\n\x06\x61ssets\x18\x08 \x03(\x0b\x32\x1c.gogc.FeatureMsg.AssetsEntry\x12\x12\n\ncollection\x18\t \x01(\t\x1a=\n\x0b\x41ssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xbe\x02\n\x08\x41ssetMsg\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04href\x18\x04 \x01(\t\x12\r\n\x05roles\x18\x05 \x03(\t\x12!\n\x08\x65o_bands\x18\x06 \x03(\x0b\x32\x0f.gogc.EOBandMsg\x12)\n\x0craster_bands\x18\x07 \x03(\x0b\x32\x13.gogc.RasterBandMsg\x12!\n\x07storage\x18\t \x01(\x0b\x32\x10.gogc.StorageMsg\x12\x30\n\talternate\x18\n \x03(\x0b\x32\x1d.gogc.AssetMsg.AlternateEntry\x1a@\n\x0e\x41lternateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"T\n\nStorageMsg\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x16\n\x0erequester_pays\x18\x03 \x01(\x08\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\xa4\x01\n\tEOBandMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommon_name\x18\x02 \x01(\t\x12\x0b\n\x03gsd\x18\x03 \x01(\x01\x12\x19\n\x11\x63\x65nter_wavelength\x18\x04 \x01(\x01\x12\x1b\n\x13\x66ull_width_half_max\x18\x05 \x01(\x01\x12\x1a\n\x12solar_illumination\x18\x06 \x01(\x01\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x9b\x02\n\rRasterBandMsg\x12\'\n\x07no_data\x18\x01 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x10\n\x08sampling\x18\x02 \x01(\t\x12\x11\n\tdata_type\x18\x03 \x01(\t\x12\x17\n\x0f\x62its_per_sample\x18\x04 \x01(\x05\x12\x1a\n\x12spatial_resolution\x18\x05 \x01(\x01\x12-\n\nstatistics\x18\x06 \x01(\x0b\x32\x19.gogc.RasterStatisticsMsg\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\r\n\x05scale\x18\x08 \x01(\x01\x12\x0e\n\x06offset\x18\t \x01(\x01\x12+\n\thistogram\x18\n \x01(\x0b\x32\x18.gogc.RasterHistogramMsg\"l\n\x13RasterStatisticsMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x01\x12\x0f\n\x07minimum\x18\x02 \x01(\x01\x12\x0f\n\x07maximum\x18\x03 \x01(\x01\x12\x0e\n\x06stddev\x18\x04 \x01(\x01\x12\x15\n\rvalid_percent\x18\x05 \x01(\x01\"N\n\x12RasterHistogramMsg\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0f\n\x07\x62uckets\x18\x04 \x03(\x04\"_\n\tExtentMsg\x12\'\n\x07spatial\x18\x01 \x03(\x0b\x32\x16.gogc.SpatialExtentMsg\x12)\n\x08temporal\x18\x02 \x03(\x0b\x32\x17.gogc.TemporalExtentMsg\" \n\x10SpatialExtentMsg\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\"A\n\x11TemporalExtentMsg\x12,\n\x08interval\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x02\n\x07LinkMsg\x12\x0c\n\x04href\x18\x01 \x01(\t\x12\x0b\n\x03rel\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08hreflang\x18\x04 \x01(\t\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06length\x18\x06 \x01(\x03\x12\x0e\n\x06method\x18\x07 \x01(\t\x12+\n\x07headers\x18\x08 \x03(\x0b\x32\x1a.gogc.LinkMsg.HeadersEntry\x12%\n\x04\x62ody\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05merge\x18\n \x01(\x08\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"L\n\x0bProviderMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\x12\x0b\n\x03url\x18\x04 \x01(\tB!Z\x1fgithub.com/seerai/gogc/featuresb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'features_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\037github.com/seerai/gogc/features'
-  _COLLECTIONMSG_SUMMARIESENTRY._options = None
-  _COLLECTIONMSG_SUMMARIESENTRY._serialized_options = b'8\001'
   _COLLECTIONMSG_ITEMASSETSENTRY._options = None
   _COLLECTIONMSG_ITEMASSETSENTRY._serialized_options = b'8\001'
-  _FEATUREMSG_PROPERTIESENTRY._options = None
-  _FEATUREMSG_PROPERTIESENTRY._serialized_options = b'8\001'
   _FEATUREMSG_ASSETSENTRY._options = None
   _FEATUREMSG_ASSETSENTRY._serialized_options = b'8\001'
   _ASSETMSG_ALTERNATEENTRY._options = None
   _ASSETMSG_ALTERNATEENTRY._serialized_options = b'8\001'
   _LINKMSG_HEADERSENTRY._options = None
   _LINKMSG_HEADERSENTRY._serialized_options = b'8\001'
   _COLLECTIONMSG._serialized_start=88
-  _COLLECTIONMSG._serialized_end=578
-  _COLLECTIONMSG_SUMMARIESENTRY._serialized_start=439
-  _COLLECTIONMSG_SUMMARIESENTRY._serialized_end=511
-  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_start=513
-  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_end=578
-  _FEATURECOLLECTIONMSG._serialized_start=581
-  _FEATURECOLLECTIONMSG._serialized_end=765
-  _FEATUREMSG._serialized_start=768
-  _FEATUREMSG._serialized_end=1163
-  _FEATUREMSG_PROPERTIESENTRY._serialized_start=1027
-  _FEATUREMSG_PROPERTIESENTRY._serialized_end=1100
-  _FEATUREMSG_ASSETSENTRY._serialized_start=1102
-  _FEATUREMSG_ASSETSENTRY._serialized_end=1163
-  _ASSETMSG._serialized_start=1166
-  _ASSETMSG._serialized_end=1484
-  _ASSETMSG_ALTERNATEENTRY._serialized_start=1420
-  _ASSETMSG_ALTERNATEENTRY._serialized_end=1484
-  _STORAGEMSG._serialized_start=1486
-  _STORAGEMSG._serialized_end=1570
-  _EOBANDMSG._serialized_start=1573
-  _EOBANDMSG._serialized_end=1737
-  _RASTERBANDMSG._serialized_start=1740
-  _RASTERBANDMSG._serialized_end=2023
-  _RASTERSTATISTICSMSG._serialized_start=2025
-  _RASTERSTATISTICSMSG._serialized_end=2133
-  _RASTERHISTOGRAMMSG._serialized_start=2135
-  _RASTERHISTOGRAMMSG._serialized_end=2213
-  _EXTENTMSG._serialized_start=2215
-  _EXTENTMSG._serialized_end=2310
-  _SPATIALEXTENTMSG._serialized_start=2312
-  _SPATIALEXTENTMSG._serialized_end=2344
-  _TEMPORALEXTENTMSG._serialized_start=2346
-  _TEMPORALEXTENTMSG._serialized_end=2411
-  _LINKMSG._serialized_start=2414
-  _LINKMSG._serialized_end=2676
-  _LINKMSG_HEADERSENTRY._serialized_start=2630
-  _LINKMSG_HEADERSENTRY._serialized_end=2676
-  _PROVIDERMSG._serialized_start=2678
-  _PROVIDERMSG._serialized_end=2754
+  _COLLECTIONMSG._serialized_end=493
+  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_start=428
+  _COLLECTIONMSG_ITEMASSETSENTRY._serialized_end=493
+  _FEATURECOLLECTIONMSG._serialized_start=496
+  _FEATURECOLLECTIONMSG._serialized_end=680
+  _FEATUREMSG._serialized_start=683
+  _FEATUREMSG._serialized_end=980
+  _FEATUREMSG_ASSETSENTRY._serialized_start=919
+  _FEATUREMSG_ASSETSENTRY._serialized_end=980
+  _ASSETMSG._serialized_start=983
+  _ASSETMSG._serialized_end=1301
+  _ASSETMSG_ALTERNATEENTRY._serialized_start=1237
+  _ASSETMSG_ALTERNATEENTRY._serialized_end=1301
+  _STORAGEMSG._serialized_start=1303
+  _STORAGEMSG._serialized_end=1387
+  _EOBANDMSG._serialized_start=1390
+  _EOBANDMSG._serialized_end=1554
+  _RASTERBANDMSG._serialized_start=1557
+  _RASTERBANDMSG._serialized_end=1840
+  _RASTERSTATISTICSMSG._serialized_start=1842
+  _RASTERSTATISTICSMSG._serialized_end=1950
+  _RASTERHISTOGRAMMSG._serialized_start=1952
+  _RASTERHISTOGRAMMSG._serialized_end=2030
+  _EXTENTMSG._serialized_start=2032
+  _EXTENTMSG._serialized_end=2127
+  _SPATIALEXTENTMSG._serialized_start=2129
+  _SPATIALEXTENTMSG._serialized_end=2161
+  _TEMPORALEXTENTMSG._serialized_start=2163
+  _TEMPORALEXTENTMSG._serialized_end=2228
+  _LINKMSG._serialized_start=2231
+  _LINKMSG._serialized_end=2493
+  _LINKMSG_HEADERSENTRY._serialized_start=2447
+  _LINKMSG_HEADERSENTRY._serialized_end=2493
+  _PROVIDERMSG._serialized_start=2495
+  _PROVIDERMSG._serialized_end=2571
 # @@protoc_insertion_point(module_scope)
```

## tesseract/inference_pb2.py

```diff
@@ -8,34 +8,31 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import tesseract.error_pb2 as error__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0finference.proto\x12\x08workerv1\x1a\x0b\x65rror.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\"v\n\x14SendAssetDataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12+\n\x06header\x18\x03 \x01(\x0b\x32\x19.workerv1.AssetDataHeaderH\x00\x12\r\n\x05index\x18\x04 \x01(\x05\x42\x06\n\x04part\"\xaa\x01\n\x15SendAssetDataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12+\n\x06header\x18\x03 \x01(\x0b\x32\x19.workerv1.AssetDataHeaderH\x00\x12 \n\x05\x65rror\x18\x05 \x01(\x0b\x32\x0f.geodesic.ErrorH\x00\x12\x1e\n\x04grid\x18\x06 \x01(\x0b\x32\x0e.workerv1.GridH\x00\x42\x06\n\x04part\"A\n\x0f\x41ssetDataHeader\x12\r\n\x05shape\x18\x01 \x03(\x04\x12\r\n\x05\x64type\x18\x02 \x01(\t\x12\x10\n\x08\x66ilepath\x18\x04 \x01(\t\"V\n\x04Grid\x12)\n\x05times\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x62\x61nds\x18\x02 \x03(\t\x12\t\n\x01x\x18\x03 \x03(\x01\x12\t\n\x01y\x18\x04 \x03(\x01\"I\n\rAssetDataInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05shape\x18\x02 \x03(\x04\x12\r\n\x05\x64type\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\"^\n\tModelInfo\x12\'\n\x06inputs\x18\x01 \x03(\x0b\x32\x17.workerv1.AssetDataInfo\x12(\n\x07outputs\x18\x02 \x03(\x0b\x32\x17.workerv1.AssetDataInfo2\xab\x01\n\x12InferenceServiceV1\x12V\n\rSendAssetData\x12\x1e.workerv1.SendAssetDataRequest\x1a\x1f.workerv1.SendAssetDataResponse\"\x00(\x01\x30\x01\x12=\n\x0cGetModelInfo\x12\x16.google.protobuf.Empty\x1a\x13.workerv1.ModelInfo\"\x00\x42\x31Z/github.com/seerai/tesseract/worker/v1/inferenceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0finference.proto\x12\x08workerv1\x1a\x0b\x65rror.proto\x1a\x1bgoogle/protobuf/empty.proto\"\x8e\x01\n\x14SendAssetDataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12+\n\x06header\x18\x03 \x01(\x0b\x32\x19.workerv1.AssetDataHeaderH\x00\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x16\n\x0egrid_for_index\x18\x05 \x01(\x05\x42\x06\n\x04part\"\x8a\x01\n\x15SendAssetDataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12+\n\x06header\x18\x03 \x01(\x0b\x32\x19.workerv1.AssetDataHeaderH\x00\x12 \n\x05\x65rror\x18\x05 \x01(\x0b\x32\x0f.geodesic.ErrorH\x00\x42\x06\n\x04part\"A\n\x0f\x41ssetDataHeader\x12\r\n\x05shape\x18\x01 \x03(\x04\x12\r\n\x05\x64type\x18\x02 \x01(\t\x12\x10\n\x08\x66ilepath\x18\x04 \x01(\t\"I\n\rAssetDataInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05shape\x18\x02 \x03(\x04\x12\r\n\x05\x64type\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\"^\n\tModelInfo\x12\'\n\x06inputs\x18\x01 \x03(\x0b\x32\x17.workerv1.AssetDataInfo\x12(\n\x07outputs\x18\x02 \x03(\x0b\x32\x17.workerv1.AssetDataInfo2\xab\x01\n\x12InferenceServiceV1\x12V\n\rSendAssetData\x12\x1e.workerv1.SendAssetDataRequest\x1a\x1f.workerv1.SendAssetDataResponse\"\x00(\x01\x30\x01\x12=\n\x0cGetModelInfo\x12\x16.google.protobuf.Empty\x1a\x13.workerv1.ModelInfo\"\x00\x42\x31Z/github.com/seerai/tesseract/worker/v1/inferenceb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'inference_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z/github.com/seerai/tesseract/worker/v1/inference'
-  _SENDASSETDATAREQUEST._serialized_start=104
-  _SENDASSETDATAREQUEST._serialized_end=222
-  _SENDASSETDATARESPONSE._serialized_start=225
-  _SENDASSETDATARESPONSE._serialized_end=395
-  _ASSETDATAHEADER._serialized_start=397
-  _ASSETDATAHEADER._serialized_end=462
-  _GRID._serialized_start=464
-  _GRID._serialized_end=550
-  _ASSETDATAINFO._serialized_start=552
-  _ASSETDATAINFO._serialized_end=625
-  _MODELINFO._serialized_start=627
-  _MODELINFO._serialized_end=721
-  _INFERENCESERVICEV1._serialized_start=724
-  _INFERENCESERVICEV1._serialized_end=895
+  _SENDASSETDATAREQUEST._serialized_start=72
+  _SENDASSETDATAREQUEST._serialized_end=214
+  _SENDASSETDATARESPONSE._serialized_start=217
+  _SENDASSETDATARESPONSE._serialized_end=355
+  _ASSETDATAHEADER._serialized_start=357
+  _ASSETDATAHEADER._serialized_end=422
+  _ASSETDATAINFO._serialized_start=424
+  _ASSETDATAINFO._serialized_end=497
+  _MODELINFO._serialized_start=499
+  _MODELINFO._serialized_end=593
+  _INFERENCESERVICEV1._serialized_start=596
+  _INFERENCESERVICEV1._serialized_end=767
 # @@protoc_insertion_point(module_scope)
```

## tesseract/server.py

```diff
@@ -1,16 +1,19 @@
 import os
 import json
+import re
 import uuid
 import inspect
 import traceback
 import logging
 from time import time
 from types import FunctionType
 from typing import Iterator
+from functools import partial
+from collections import defaultdict
 from concurrent import futures
 
 import grpc
 import numpy as np
 
 from tesseract.inference_pb2_grpc import (
     InferenceServiceV1Servicer,
@@ -37,14 +40,16 @@
             pass
     return model_args
 
 
 os.makedirs("/tmp/log/", exist_ok=True)
 logger = _get_logger(__name__)
 
+grid_re = re.compile(r"\[grid\-(x|y|t)\]")
+
 
 class TesseractModelServicer(InferenceServiceV1Servicer):
     def __init__(self, inference_func, model_info_func):
         self.inference_func = inference_func
         if not callable(inference_func):
             raise ValueError("inference_func must be a callable")
 
@@ -57,17 +62,21 @@
         for input in self.model_info["inputs"]:
             self.asset_types[input["name"]] = input.get("type")
 
         self.output_asset_names = [output["name"] for output in self.model_info["outputs"]]
 
         self.model_args = get_model_args()
         self.send_args = False
+        self.send_grids = False
         if self.model_args:
             signature = inspect.signature(inference_func)
-            for param in signature.parameters.values():
+            for key, param in signature.parameters.items():
+                if key == "grids":
+                    self.send_grids = True
+                    continue
                 if param.kind == param.VAR_KEYWORD:
                     self.send_args = True
 
     def GetModelInfo(self, request: None, context: grpc.ServicerContext) -> ModelInfo:
         model_info = self.model_info_func()
 
         # Get all of the inputs required by the model
@@ -92,28 +101,32 @@
     def SendAssetData(
         self, request: Iterator[SendAssetDataRequest], context: grpc.ServicerContext
     ) -> Iterator[SendAssetDataResponse]:
         user_logger = _child_logger(logger, "model", f"/tmp/log/{uuid.uuid4()}.log")
 
         logger.debug("receiving SendAssetDataRequest")
         try:
-            in_assets = self.read_asset_data(request, context)
+            in_assets, grids = self.read_asset_data(request, context)
         except Exception as e:
             yield error_response(
                 e, "invalid argument", grpc.StatusCode.INVALID_ARGUMENT, logger, context
             )
             return
 
         try:
             logger.info("running inference_func")
             t = time()
+
+            inference_func = self.inference_func
             if self.send_args:
-                out_assets = self.inference_func(in_assets, user_logger, **self.model_args)
-            else:
-                out_assets = self.inference_func(in_assets, user_logger)
+                inference_func = partial(inference_func, **self.model_args)
+            if self.send_grids:
+                inference_func = partial(inference_func, grids=grids)
+
+            out_assets = inference_func(assets=in_assets, logger=user_logger)
             logger.info(f"Done, inference_func finished in {time() - t} s")
         except Exception as e:
             yield error_response(e, "inference failed", grpc.StatusCode.INTERNAL, logger, context)
             return
 
         logger.debug("sending SendAssetDataResponse")
         for name, out_asset in out_assets.items():
@@ -144,21 +157,23 @@
         return f"${self.output_asset_names.index(asset_name)}"
 
     def read_asset_data(
         self, request: Iterator[SendAssetDataRequest], context: grpc.ServicerContext
     ) -> dict:
         # Parsed asset data
         in_assets = {}
+        grids = defaultdict(dict)
 
         # Get all the assets from the stream
         for req in request:
             name = req.name
             type_ = req.type
             header = req.header
             index = req.index
+            grid_for_index = req.grid_for_index
 
             if header is None:
                 raise ValueError("empty header received")
 
             logger.debug(f"received asset '{name}'")
 
             if type_ != "tensor" and type_ != "features":
@@ -172,19 +187,30 @@
             dtype = header.dtype
 
             logger.debug(f"reading asset '{name}' from {filepath}")
             if type_ == "tensor":
                 asset_data = read_array_file(filepath, shape, dtype)
             elif type_ == "features":
                 asset_data = read_geojson_file(filepath)
-            in_assets[name] = asset_data
-            in_assets[f"${index}"] = asset_data
-            logger.debug(f"read asset '{name}'")
 
-        return in_assets
+            # Is this a grid asset?
+            m = grid_re.search(name)
+            if m is not None:
+                asset_name_end, _ = m.span()
+                dimension = m.group(1)
+                asset_name = name[:asset_name_end]
+                grids[asset_name][dimension] = asset_data
+                grids[f"${grid_for_index}"][dimension] = asset_data
+                logger.debug(f"read {asset_name} grid dimension {dimension}'")
+            else:
+                in_assets[name] = asset_data
+                in_assets[f"${index}"] = asset_data
+                logger.debug(f"read asset '{name}'")
+
+        return in_assets, grids
 
     def get_feature_response(self, name: str, out_asset: dict) -> SendAssetDataResponse:
         filepath = write_geojson_file(out_asset)
 
         return SendAssetDataResponse(
             name=name, type="features", header=AssetDataHeader(filepath=filepath)
         )
```

## tesseract/validate.py

```diff
@@ -53,22 +53,30 @@
         except Exception:
             print("Cleaning Up")
             print("Killing model container")
             pass
 
         logs = None
         if self.print_container_logs:
-            logs = self.model_container.logs().decode()
+            try:
+                logs = self.model_container.logs().decode()
+            except docker.errors.NotFound:
+                pass
 
         try:
             self.model_container.kill()
-        except AttributeError:
+        except docker.errors.APIError:
             pass
 
         try:
+            self.model_container.remove()
+        except docker.error.APIError as e:
+            raise (e)
+
+        try:
             self.gutenberger.summary(stats=self.stats, logs=logs)
 
         except Exception:
             pass
 
     def model(self, status):
         status.update("[orange_red1]Starting Model Container")
@@ -81,15 +89,14 @@
             self.model_container = docker_client.containers.run(
                 image=self.image,
                 ports={50051: 50051},
                 environment=environment,
                 volumes={
                     self.tmp_path: {"bind": "/tmp", "mode": "rw"},
                 },
-                remove=True,
                 detach=True,
             )
         except Exception:
             raise Exception("could not start container", self.model_container.logs().decode())
 
         try:
             _ = docker_client.containers.get(self.model_container.name)
@@ -100,14 +107,19 @@
         self.gutenberger.task("Model Container Running")
 
     def grpc_client(self, status):
         status.update("[orange_red1]Waiting for connection to container")
         self.channel = grpc.insecure_channel("localhost:50051")
         try:
             grpc.channel_ready_future(self.channel).result(timeout=45)
+        except grpc.FutureTimeoutError:
+            self.gutenberger.task("[red]could not connect to the model container. GRPC Timeout. Docker logs:")
+            self.model_container.remove
+            print(self.model_container.logs().decode())
+            exit(1)
         except Exception as e:
             self.gutenberger.task("[red]could not connect to the model container. Docker logs:")
             print(self.model_container.logs().decode())
             raise (e)
         self.client = inference_pb2_grpc.InferenceServiceV1Stub(self.channel)
         self.gutenberger.task("Connection established")
```

## tesseract/scripts/validate.py

```diff
@@ -1,9 +1,8 @@
 import argparse
-import sys
 import json
 
 
 def validate_command(args):
     import tesseract.validate as validate
 
     # try to parse args as JSON
```

## Comparing `tesseract_sdk-0.7.0.dist-info/LICENSE` & `tesseract_sdk-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tesseract_sdk-0.7.0.dist-info/METADATA` & `tesseract_sdk-0.8.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-sdk
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python SDK for Tesseract Models
 Author-email: The SeerAI Team <contact@seer.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,15 +217,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geodesic-api (>=0.12.0)
 Requires-Dist: grpclib (>=0.4.2)
 Requires-Dist: protobuf (>=3.20.0)
-Requires-Dist: grpcio (~=1.50.0)
+Requires-Dist: grpcio (>=1.50.0)
 Requires-Dist: rich (~=12.5.1)
 Requires-Dist: docker (~=6.0.0)
 Provides-Extra: all
 Requires-Dist: tesseract-sdk[extract] ; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: tesseract-sdk[all] ; extra == 'dev'
 Requires-Dist: grpcio-tools ; extra == 'dev'
```

## Comparing `tesseract_sdk-0.7.0.dist-info/RECORD` & `tesseract_sdk-0.8.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 tesseract/__init__.py,sha256=BXgL6U622GrO0cvmm897-Dp7H46sidSnNwcy0sSfS88,174
 tesseract/_logging.py,sha256=wmRQLdOOfHXccTc2ThEmG7c4GI26XD1FoVndyCrOyZA,7866
 tesseract/error_pb2.py,sha256=VqDpB7NpGl5udAjVmXlleKYl3DUD-vsk1ZLi4te5PDI,1215
 tesseract/error_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 tesseract/extract.py,sha256=dU74cgUA92xOzNlLR4ooqGToM5BuygyB0cgRQkMheCY,2446
 tesseract/features.py,sha256=W3gqQ_9-sOpYpFsgClO5QRiaRTBBuOg0zVkGDwbUU94,455
-tesseract/features_pb2.py,sha256=z68eDG5TXnHkAmlw0MxVAnS-iMuNzQ_lbd9pyQ-SiyQ,8528
-tesseract/inference_pb2.py,sha256=wzWCvVmHwBgTi2FDD8bqbUbVilMe8Ok3MXuI_f4wJT8,3240
+tesseract/features_pb2.py,sha256=2pAy93Dujdq3k3p_rHNDMR_k-K8sUZG75RfABH8F_Wo,7772
+tesseract/inference_pb2.py,sha256=g4qGYsCFw2g4Z7v-5jSfQeRFxHg-c7TPfAhf3ltxLO0,2866
 tesseract/inference_pb2_grpc.py,sha256=Er6vnyf0Q4__iZEE3ex2o3TLCKZNpnCHfcHsv6tayVU,4125
-tesseract/server.py,sha256=pZkAZDvJ-o9HU2DeHy-fT6_Wqu8gGMpDNeRW8-VUhGs,8065
+tesseract/server.py,sha256=Bb7TCJvSdL2IGjSkoBs_zme2rK40kgpvc8oOj9xeBi8,9022
 tesseract/tensor.py,sha256=z7D4EJERohY84vuGkYEIcAJytwvWwK4Glzb8lch9eOk,535
-tesseract/validate.py,sha256=zsd1lkJisx4nk566AFfpCy5xFYGEfc8MX0WqU0MqmWw,15769
-tesseract/scripts/validate.py,sha256=unkb4BPoIwGR6IbJMOuCYddffDSU_yHoyKXv6Ix505A,1637
-tesseract_sdk-0.7.0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-tesseract_sdk-0.7.0.dist-info/METADATA,sha256=2qJEKrihF1E7MOLMmqMvXBjP1j8yyoqKLt561dTY2Go,14839
-tesseract_sdk-0.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tesseract_sdk-0.7.0.dist-info/entry_points.txt,sha256=mBWXQm3S2VxrpDpIm7tGofwEFNgim_e_qauU2KqLaIw,66
-tesseract_sdk-0.7.0.dist-info/top_level.txt,sha256=q1iuQze2tRHNnKxd8hyfkDbkrz6RHFbHJd8Pm9X4qOI,10
-tesseract_sdk-0.7.0.dist-info/RECORD,,
+tesseract/validate.py,sha256=atrWWqyjU5-PD4S7HiiMAJVx7maNw3GIhCj07XO0-H4,16221
+tesseract/scripts/validate.py,sha256=9GQAz1pkqDHUjv7GgKc5HdDk4UEVjxwRINQ82yDfMDg,1626
+tesseract_sdk-0.8.0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+tesseract_sdk-0.8.0.dist-info/METADATA,sha256=fYuYxl4-3PUsxCPeIbT37iENsErcKDFQw-06gCuVqIw,14839
+tesseract_sdk-0.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tesseract_sdk-0.8.0.dist-info/entry_points.txt,sha256=mBWXQm3S2VxrpDpIm7tGofwEFNgim_e_qauU2KqLaIw,66
+tesseract_sdk-0.8.0.dist-info/top_level.txt,sha256=q1iuQze2tRHNnKxd8hyfkDbkrz6RHFbHJd8Pm9X4qOI,10
+tesseract_sdk-0.8.0.dist-info/RECORD,,
```

