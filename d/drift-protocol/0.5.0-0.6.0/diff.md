# Comparing `tmp/drift_protocol-0.5.0-py3-none-any.whl.zip` & `tmp/drift_protocol-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 13069 bytes, number of entries: 14
--rw-r--r--  2.0 unx      285 b- defN 23-Jun-15 10:24 drift_protocol/__init__.py
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-15 10:24 drift_protocol/common/__init__.py
--rw-r--r--  2.0 unx     2580 b- defN 23-Jun-15 10:24 drift_protocol/common/data_payload_pb2.py
--rw-r--r--  2.0 unx     8282 b- defN 23-Jun-15 10:24 drift_protocol/common/drift_package_pb2.py
--rw-r--r--  2.0 unx     4542 b- defN 23-Jun-15 10:24 drift_protocol/common/status_code_pb2.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jun-15 10:24 drift_protocol/meta/__init__.py
--rw-r--r--  2.0 unx    35609 b- defN 23-Jun-15 10:24 drift_protocol/meta/meta_info_pb2.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-15 10:24 drift_protocol/trigger_service/__init__.py
--rw-r--r--  2.0 unx     3454 b- defN 23-Jun-15 10:24 drift_protocol/trigger_service/interval_trigger_message_pb2.py
--rw-r--r--  2.0 unx     2622 b- defN 23-Jun-15 10:24 drift_protocol/trigger_service/trigger_message_pb2.py
--rw-r--r--  2.0 unx     1807 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1296 b- defN 23-Jun-15 10:24 drift_protocol-0.5.0.dist-info/RECORD
-14 files, 60788 bytes uncompressed, 10859 bytes compressed:  82.1%
+Zip file size: 13403 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      285 b- defN 23-Aug-02 10:11 drift_protocol/__init__.py
+-rw-r--r--  2.0 unx       96 b- defN 23-Aug-02 10:11 drift_protocol/common/__init__.py
+-rw-r--r--  2.0 unx     2580 b- defN 23-Aug-02 10:11 drift_protocol/common/data_payload_pb2.py
+-rw-r--r--  2.0 unx     8282 b- defN 23-Aug-02 10:11 drift_protocol/common/drift_package_pb2.py
+-rw-r--r--  2.0 unx     4542 b- defN 23-Aug-02 10:11 drift_protocol/common/status_code_pb2.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Aug-02 10:11 drift_protocol/meta/__init__.py
+-rw-r--r--  2.0 unx    39953 b- defN 23-Aug-02 10:11 drift_protocol/meta/meta_info_pb2.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-02 10:11 drift_protocol/trigger_service/__init__.py
+-rw-r--r--  2.0 unx     3454 b- defN 23-Aug-02 10:11 drift_protocol/trigger_service/interval_trigger_message_pb2.py
+-rw-r--r--  2.0 unx     2622 b- defN 23-Aug-02 10:11 drift_protocol/trigger_service/trigger_message_pb2.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Aug-02 10:11 drift_protocol-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 10:11 drift_protocol-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Aug-02 10:11 drift_protocol-0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1296 b- defN 23-Aug-02 10:11 drift_protocol-0.6.0.dist-info/RECORD
+14 files, 65132 bytes uncompressed, 11193 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: drift_protocol/trigger_service/interval_trigger_message_pb2.py
 Comment: 
 
 Filename: drift_protocol/trigger_service/trigger_message_pb2.py
 Comment: 
 
-Filename: drift_protocol-0.5.0.dist-info/METADATA
+Filename: drift_protocol-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: drift_protocol-0.5.0.dist-info/WHEEL
+Filename: drift_protocol-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: drift_protocol-0.5.0.dist-info/top_level.txt
+Filename: drift_protocol-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drift_protocol-0.5.0.dist-info/RECORD
+Filename: drift_protocol-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drift_protocol/__init__.py

```diff
@@ -1,8 +1,8 @@
 """ Auto-generated file for package with generated protobuf bindings
 """
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 import google.protobuf as protobuf
 
 if protobuf.__version__ < '3.12.4':
     raise RuntimeError(f'Version of protobuf PIP package must be >=3.12.4. However you have {protobuf.__version__}')
```

## drift_protocol/common/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-from .status_code_pb2 import *
 from .drift_package_pb2 import *
+from .status_code_pb2 import *
 from .data_payload_pb2 import *
```

## drift_protocol/meta/meta_info_pb2.py

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='drift_protocol/meta/meta_info.proto',
   package='drift.proto.meta',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n#drift_protocol/meta/meta_info.proto\x12\x10\x64rift.proto.meta\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'drift_protocol/common/status_code.proto\"\xd6\x03\n\x11WaveletBufferInfo\x12\x13\n\x0b\x61\x62i_version\x18\x01 \x01(\r\x12\x14\n\x0cwavelet_type\x18\x02 \x01(\r\x12\x1b\n\x13\x64\x65\x63omposition_steps\x18\x03 \x01(\r\x12\x19\n\x11\x66loat_compression\x18\x04 \x01(\r\x12G\n\x0cno_denoising\x18\x0f \x01(\x0b\x32/.drift.proto.meta.WaveletBufferInfo.NoDenoisingH\x00\x12U\n\x13threshold_denoising\x18\x10 \x01(\x0b\x32\x36.drift.proto.meta.WaveletBufferInfo.ThresholdDenoisingH\x00\x12Q\n\x11partial_denoising\x18\x11 \x01(\x0b\x32\x34.drift.proto.meta.WaveletBufferInfo.PartialDenoisingH\x00\x1a\r\n\x0bNoDenoising\x1a*\n\x12ThresholdDenoising\x12\t\n\x01\x61\x18\x01 \x01(\x02\x12\t\n\x01\x62\x18\x02 \x01(\x02\x1a#\n\x10PartialDenoising\x12\x0f\n\x07partial\x18\x01 \x01(\x02\x42\x0b\n\tdenoising\"\xf9\x03\n\x08MetaInfo\x12\x31\n\x04type\x18\x01 \x01(\x0e\x32#.drift.proto.meta.MetaInfo.DataType\x12<\n\x10time_series_info\x18\x02 \x01(\x0b\x32 .drift.proto.meta.TimeSeriesInfoH\x00\x12\x31\n\nimage_info\x18\x03 \x01(\x0b\x32\x1b.drift.proto.meta.ImageInfoH\x00\x12\x39\n\x0bscalar_info\x18\x04 \x01(\x0b\x32\".drift.proto.meta.ScalarValuesInfoH\x00\x12/\n\ttext_info\x18\x05 \x01(\x0b\x32\x1a.drift.proto.meta.TextInfoH\x00\x12\x39\n\x0e\x61lignment_info\x18\x06 \x01(\x0b\x32\x1f.drift.proto.meta.AlignmentInfoH\x00\x12@\n\x13wavelet_buffer_info\x18\x07 \x01(\x0b\x32#.drift.proto.meta.WaveletBufferInfo\"X\n\x08\x44\x61taType\x12\x0f\n\x0bTIME_SERIES\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\x11\n\rSCALAR_VALUES\x10\x02\x12\x08\n\x04TEXT\x10\x03\x12\x13\n\x0f\x41LIGNED_PACKAGE\x10\x04\x42\x06\n\x04info\"\xcc\x01\n\x0eTimeSeriesInfo\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estop_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12\r\n\x05\x66irst\x18\x04 \x01(\x02\x12\x0c\n\x04last\x18\x05 \x01(\x02\x12\x0b\n\x03min\x18\x06 \x01(\x02\x12\x0b\n\x03max\x18\x07 \x01(\x02\x12\x0c\n\x04mean\x18\x08 \x01(\x02\"\x96\x01\n\tImageInfo\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.drift.proto.meta.ImageInfo.ImageType\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0e\n\x06height\x18\x03 \x01(\x04\x12\x16\n\x0e\x63hannel_layout\x18\x04 \x01(\t\"\x1d\n\tImageType\x12\x06\n\x02WB\x10\x00\x12\x08\n\x04JPEG\x10\x01\"\xa4\x01\n\x10ScalarValuesInfo\x12\x42\n\tvariables\x18\x01 \x03(\x0b\x32/.drift.proto.meta.ScalarValuesInfo.VariableInfo\x1aL\n\x0cVariableInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.drift.proto.common.StatusCode\"\x1d\n\x08TextInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\"\x96\x01\n\rAlignmentInfo\x12=\n\x08packages\x18\x01 \x03(\x0b\x32+.drift.proto.meta.AlignmentInfo.PackageInfo\x1a\x46\n\x0bPackageInfo\x12\r\n\x05topic\x18\x01 \x01(\t\x12(\n\x04meta\x18\x02 \x01(\x0b\x32\x1a.drift.proto.meta.MetaInfob\x06proto3'
+  serialized_pb=b'\n#drift_protocol/meta/meta_info.proto\x12\x10\x64rift.proto.meta\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'drift_protocol/common/status_code.proto\"\xd6\x03\n\x11WaveletBufferInfo\x12\x13\n\x0b\x61\x62i_version\x18\x01 \x01(\r\x12\x14\n\x0cwavelet_type\x18\x02 \x01(\r\x12\x1b\n\x13\x64\x65\x63omposition_steps\x18\x03 \x01(\r\x12\x19\n\x11\x66loat_compression\x18\x04 \x01(\r\x12G\n\x0cno_denoising\x18\x0f \x01(\x0b\x32/.drift.proto.meta.WaveletBufferInfo.NoDenoisingH\x00\x12U\n\x13threshold_denoising\x18\x10 \x01(\x0b\x32\x36.drift.proto.meta.WaveletBufferInfo.ThresholdDenoisingH\x00\x12Q\n\x11partial_denoising\x18\x11 \x01(\x0b\x32\x34.drift.proto.meta.WaveletBufferInfo.PartialDenoisingH\x00\x1a\r\n\x0bNoDenoising\x1a*\n\x12ThresholdDenoising\x12\t\n\x01\x61\x18\x01 \x01(\x02\x12\t\n\x01\x62\x18\x02 \x01(\x02\x1a#\n\x10PartialDenoising\x12\x0f\n\x07partial\x18\x01 \x01(\x02\x42\x0b\n\tdenoising\"\xc5\x04\n\x08MetaInfo\x12\x31\n\x04type\x18\x01 \x01(\x0e\x32#.drift.proto.meta.MetaInfo.DataType\x12<\n\x10time_series_info\x18\x02 \x01(\x0b\x32 .drift.proto.meta.TimeSeriesInfoH\x00\x12\x31\n\nimage_info\x18\x03 \x01(\x0b\x32\x1b.drift.proto.meta.ImageInfoH\x00\x12\x39\n\x0bscalar_info\x18\x04 \x01(\x0b\x32\".drift.proto.meta.ScalarValuesInfoH\x00\x12/\n\ttext_info\x18\x05 \x01(\x0b\x32\x1a.drift.proto.meta.TextInfoH\x00\x12\x39\n\x0e\x61lignment_info\x18\x06 \x01(\x0b\x32\x1f.drift.proto.meta.AlignmentInfoH\x00\x12:\n\x0ftyped_data_info\x18\x08 \x01(\x0b\x32\x1f.drift.proto.meta.TypedDataInfoH\x00\x12@\n\x13wavelet_buffer_info\x18\x07 \x01(\x0b\x32#.drift.proto.meta.WaveletBufferInfo\"h\n\x08\x44\x61taType\x12\x0f\n\x0bTIME_SERIES\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\x11\n\rSCALAR_VALUES\x10\x02\x12\x08\n\x04TEXT\x10\x03\x12\x13\n\x0f\x41LIGNED_PACKAGE\x10\x04\x12\x0e\n\nTYPED_DATA\x10\x05\x42\x06\n\x04info\"\xcc\x01\n\x0eTimeSeriesInfo\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estop_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04size\x18\x03 \x01(\x04\x12\r\n\x05\x66irst\x18\x04 \x01(\x02\x12\x0c\n\x04last\x18\x05 \x01(\x02\x12\x0b\n\x03min\x18\x06 \x01(\x02\x12\x0b\n\x03max\x18\x07 \x01(\x02\x12\x0c\n\x04mean\x18\x08 \x01(\x02\"\x96\x01\n\tImageInfo\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.drift.proto.meta.ImageInfo.ImageType\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0e\n\x06height\x18\x03 \x01(\x04\x12\x16\n\x0e\x63hannel_layout\x18\x04 \x01(\t\"\x1d\n\tImageType\x12\x06\n\x02WB\x10\x00\x12\x08\n\x04JPEG\x10\x01\"\xa4\x01\n\x10ScalarValuesInfo\x12\x42\n\tvariables\x18\x01 \x03(\x0b\x32/.drift.proto.meta.ScalarValuesInfo.VariableInfo\x1aL\n\x0cVariableInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.drift.proto.common.StatusCode\"\x1d\n\x08TextInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\"\x96\x01\n\rAlignmentInfo\x12=\n\x08packages\x18\x01 \x03(\x0b\x32+.drift.proto.meta.AlignmentInfo.PackageInfo\x1a\x46\n\x0bPackageInfo\x12\r\n\x05topic\x18\x01 \x01(\t\x12(\n\x04meta\x18\x02 \x01(\x0b\x32\x1a.drift.proto.meta.MetaInfo\"\x8a\x01\n\rTypedDataInfo\x12\x33\n\x05items\x18\x01 \x03(\x0b\x32$.drift.proto.meta.TypedDataInfo.Item\x1a\x44\n\x04Item\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.drift.proto.common.StatusCodeb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,drift__protocol_dot_common_dot_status__code__pb2.DESCRIPTOR,])
 
 
 
 _METAINFO_DATATYPE = _descriptor.EnumDescriptor(
   name='DataType',
@@ -55,19 +55,24 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='ALIGNED_PACKAGE', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='TYPED_DATA', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1014,
-  serialized_end=1102,
+  serialized_start=1074,
+  serialized_end=1178,
 )
 _sym_db.RegisterEnumDescriptor(_METAINFO_DATATYPE)
 
 _IMAGEINFO_IMAGETYPE = _descriptor.EnumDescriptor(
   name='ImageType',
   full_name='drift.proto.meta.ImageInfo.ImageType',
   filename=None,
@@ -83,16 +88,16 @@
       name='JPEG', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1441,
-  serialized_end=1470,
+  serialized_start=1517,
+  serialized_end=1546,
 )
 _sym_db.RegisterEnumDescriptor(_IMAGEINFO_IMAGETYPE)
 
 
 _WAVELETBUFFERINFO_NODENOISING = _descriptor.Descriptor(
   name='NoDenoising',
   full_name='drift.proto.meta.WaveletBufferInfo.NoDenoising',
@@ -312,15 +317,22 @@
       name='alignment_info', full_name='drift.proto.meta.MetaInfo.alignment_info', index=5,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='wavelet_buffer_info', full_name='drift.proto.meta.MetaInfo.wavelet_buffer_info', index=6,
+      name='typed_data_info', full_name='drift.proto.meta.MetaInfo.typed_data_info', index=6,
+      number=8, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='wavelet_buffer_info', full_name='drift.proto.meta.MetaInfo.wavelet_buffer_info', index=7,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -337,15 +349,15 @@
     _descriptor.OneofDescriptor(
       name='info', full_name='drift.proto.meta.MetaInfo.info',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
   serialized_start=605,
-  serialized_end=1110,
+  serialized_end=1186,
 )
 
 
 _TIMESERIESINFO = _descriptor.Descriptor(
   name='TimeSeriesInfo',
   full_name='drift.proto.meta.TimeSeriesInfo',
   filename=None,
@@ -417,16 +429,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1113,
-  serialized_end=1317,
+  serialized_start=1189,
+  serialized_end=1393,
 )
 
 
 _IMAGEINFO = _descriptor.Descriptor(
   name='ImageInfo',
   full_name='drift.proto.meta.ImageInfo',
   filename=None,
@@ -471,16 +483,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1320,
-  serialized_end=1470,
+  serialized_start=1396,
+  serialized_end=1546,
 )
 
 
 _SCALARVALUESINFO_VARIABLEINFO = _descriptor.Descriptor(
   name='VariableInfo',
   full_name='drift.proto.meta.ScalarValuesInfo.VariableInfo',
   filename=None,
@@ -510,16 +522,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1561,
-  serialized_end=1637,
+  serialized_start=1637,
+  serialized_end=1713,
 )
 
 _SCALARVALUESINFO = _descriptor.Descriptor(
   name='ScalarValuesInfo',
   full_name='drift.proto.meta.ScalarValuesInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -541,16 +553,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1473,
-  serialized_end=1637,
+  serialized_start=1549,
+  serialized_end=1713,
 )
 
 
 _TEXTINFO = _descriptor.Descriptor(
   name='TextInfo',
   full_name='drift.proto.meta.TextInfo',
   filename=None,
@@ -573,16 +585,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1639,
-  serialized_end=1668,
+  serialized_start=1715,
+  serialized_end=1744,
 )
 
 
 _ALIGNMENTINFO_PACKAGEINFO = _descriptor.Descriptor(
   name='PackageInfo',
   full_name='drift.proto.meta.AlignmentInfo.PackageInfo',
   filename=None,
@@ -612,16 +624,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1751,
-  serialized_end=1821,
+  serialized_start=1827,
+  serialized_end=1897,
 )
 
 _ALIGNMENTINFO = _descriptor.Descriptor(
   name='AlignmentInfo',
   full_name='drift.proto.meta.AlignmentInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -643,16 +655,86 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1671,
-  serialized_end=1821,
+  serialized_start=1747,
+  serialized_end=1897,
+)
+
+
+_TYPEDDATAINFO_ITEM = _descriptor.Descriptor(
+  name='Item',
+  full_name='drift.proto.meta.TypedDataInfo.Item',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='drift.proto.meta.TypedDataInfo.Item.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='status', full_name='drift.proto.meta.TypedDataInfo.Item.status', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1970,
+  serialized_end=2038,
+)
+
+_TYPEDDATAINFO = _descriptor.Descriptor(
+  name='TypedDataInfo',
+  full_name='drift.proto.meta.TypedDataInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='items', full_name='drift.proto.meta.TypedDataInfo.items', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_TYPEDDATAINFO_ITEM, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1900,
+  serialized_end=2038,
 )
 
 _WAVELETBUFFERINFO_NODENOISING.containing_type = _WAVELETBUFFERINFO
 _WAVELETBUFFERINFO_THRESHOLDDENOISING.containing_type = _WAVELETBUFFERINFO
 _WAVELETBUFFERINFO_PARTIALDENOISING.containing_type = _WAVELETBUFFERINFO
 _WAVELETBUFFERINFO.fields_by_name['no_denoising'].message_type = _WAVELETBUFFERINFO_NODENOISING
 _WAVELETBUFFERINFO.fields_by_name['threshold_denoising'].message_type = _WAVELETBUFFERINFO_THRESHOLDDENOISING
@@ -668,14 +750,15 @@
 _WAVELETBUFFERINFO.fields_by_name['partial_denoising'].containing_oneof = _WAVELETBUFFERINFO.oneofs_by_name['denoising']
 _METAINFO.fields_by_name['type'].enum_type = _METAINFO_DATATYPE
 _METAINFO.fields_by_name['time_series_info'].message_type = _TIMESERIESINFO
 _METAINFO.fields_by_name['image_info'].message_type = _IMAGEINFO
 _METAINFO.fields_by_name['scalar_info'].message_type = _SCALARVALUESINFO
 _METAINFO.fields_by_name['text_info'].message_type = _TEXTINFO
 _METAINFO.fields_by_name['alignment_info'].message_type = _ALIGNMENTINFO
+_METAINFO.fields_by_name['typed_data_info'].message_type = _TYPEDDATAINFO
 _METAINFO.fields_by_name['wavelet_buffer_info'].message_type = _WAVELETBUFFERINFO
 _METAINFO_DATATYPE.containing_type = _METAINFO
 _METAINFO.oneofs_by_name['info'].fields.append(
   _METAINFO.fields_by_name['time_series_info'])
 _METAINFO.fields_by_name['time_series_info'].containing_oneof = _METAINFO.oneofs_by_name['info']
 _METAINFO.oneofs_by_name['info'].fields.append(
   _METAINFO.fields_by_name['image_info'])
@@ -685,31 +768,38 @@
 _METAINFO.fields_by_name['scalar_info'].containing_oneof = _METAINFO.oneofs_by_name['info']
 _METAINFO.oneofs_by_name['info'].fields.append(
   _METAINFO.fields_by_name['text_info'])
 _METAINFO.fields_by_name['text_info'].containing_oneof = _METAINFO.oneofs_by_name['info']
 _METAINFO.oneofs_by_name['info'].fields.append(
   _METAINFO.fields_by_name['alignment_info'])
 _METAINFO.fields_by_name['alignment_info'].containing_oneof = _METAINFO.oneofs_by_name['info']
+_METAINFO.oneofs_by_name['info'].fields.append(
+  _METAINFO.fields_by_name['typed_data_info'])
+_METAINFO.fields_by_name['typed_data_info'].containing_oneof = _METAINFO.oneofs_by_name['info']
 _TIMESERIESINFO.fields_by_name['start_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TIMESERIESINFO.fields_by_name['stop_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _IMAGEINFO.fields_by_name['type'].enum_type = _IMAGEINFO_IMAGETYPE
 _IMAGEINFO_IMAGETYPE.containing_type = _IMAGEINFO
 _SCALARVALUESINFO_VARIABLEINFO.fields_by_name['status'].enum_type = drift__protocol_dot_common_dot_status__code__pb2._STATUSCODE
 _SCALARVALUESINFO_VARIABLEINFO.containing_type = _SCALARVALUESINFO
 _SCALARVALUESINFO.fields_by_name['variables'].message_type = _SCALARVALUESINFO_VARIABLEINFO
 _ALIGNMENTINFO_PACKAGEINFO.fields_by_name['meta'].message_type = _METAINFO
 _ALIGNMENTINFO_PACKAGEINFO.containing_type = _ALIGNMENTINFO
 _ALIGNMENTINFO.fields_by_name['packages'].message_type = _ALIGNMENTINFO_PACKAGEINFO
+_TYPEDDATAINFO_ITEM.fields_by_name['status'].enum_type = drift__protocol_dot_common_dot_status__code__pb2._STATUSCODE
+_TYPEDDATAINFO_ITEM.containing_type = _TYPEDDATAINFO
+_TYPEDDATAINFO.fields_by_name['items'].message_type = _TYPEDDATAINFO_ITEM
 DESCRIPTOR.message_types_by_name['WaveletBufferInfo'] = _WAVELETBUFFERINFO
 DESCRIPTOR.message_types_by_name['MetaInfo'] = _METAINFO
 DESCRIPTOR.message_types_by_name['TimeSeriesInfo'] = _TIMESERIESINFO
 DESCRIPTOR.message_types_by_name['ImageInfo'] = _IMAGEINFO
 DESCRIPTOR.message_types_by_name['ScalarValuesInfo'] = _SCALARVALUESINFO
 DESCRIPTOR.message_types_by_name['TextInfo'] = _TEXTINFO
 DESCRIPTOR.message_types_by_name['AlignmentInfo'] = _ALIGNMENTINFO
+DESCRIPTOR.message_types_by_name['TypedDataInfo'] = _TYPEDDATAINFO
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 WaveletBufferInfo = _reflection.GeneratedProtocolMessageType('WaveletBufferInfo', (_message.Message,), {
 
   'NoDenoising' : _reflection.GeneratedProtocolMessageType('NoDenoising', (_message.Message,), {
     'DESCRIPTOR' : _WAVELETBUFFERINFO_NODENOISING,
     '__module__' : 'drift_protocol.meta.meta_info_pb2'
@@ -793,9 +883,24 @@
   'DESCRIPTOR' : _ALIGNMENTINFO,
   '__module__' : 'drift_protocol.meta.meta_info_pb2'
   # @@protoc_insertion_point(class_scope:drift.proto.meta.AlignmentInfo)
   })
 _sym_db.RegisterMessage(AlignmentInfo)
 _sym_db.RegisterMessage(AlignmentInfo.PackageInfo)
 
+TypedDataInfo = _reflection.GeneratedProtocolMessageType('TypedDataInfo', (_message.Message,), {
+
+  'Item' : _reflection.GeneratedProtocolMessageType('Item', (_message.Message,), {
+    'DESCRIPTOR' : _TYPEDDATAINFO_ITEM,
+    '__module__' : 'drift_protocol.meta.meta_info_pb2'
+    # @@protoc_insertion_point(class_scope:drift.proto.meta.TypedDataInfo.Item)
+    })
+  ,
+  'DESCRIPTOR' : _TYPEDDATAINFO,
+  '__module__' : 'drift_protocol.meta.meta_info_pb2'
+  # @@protoc_insertion_point(class_scope:drift.proto.meta.TypedDataInfo)
+  })
+_sym_db.RegisterMessage(TypedDataInfo)
+_sym_db.RegisterMessage(TypedDataInfo.Item)
+
 
 # @@protoc_insertion_point(module_scope)
```

## Comparing `drift_protocol-0.5.0.dist-info/METADATA` & `drift_protocol-0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drift-protocol
-Version: 0.5.0
+Version: 0.6.0
 Summary: Protobuf Libraries to encode message in Drift infrastructure
 Home-page: https://github.com/panda-official/DriftProtocol/
 Author: PANDA, GmbH
 Author-email: info@panda.technology
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `drift_protocol-0.5.0.dist-info/RECORD` & `drift_protocol-0.6.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-drift_protocol/__init__.py,sha256=ccagWV-db3mD1SSONq-0Z7LAPlATdHqK09moSyKKzcY,285
-drift_protocol/common/__init__.py,sha256=KjFbGwPza4S-JtLUcce8ZuQaMwe0f-Wi17uAfBuhdF8,96
+drift_protocol/__init__.py,sha256=gaPZGK4f4FJ82wQZSgLa_gU6Dw02N8tWEDDJjyu4exQ,285
+drift_protocol/common/__init__.py,sha256=DX-W55c_-6n04NV1phPeBd1vN7t4QJZSRb2vXV5BEwA,96
 drift_protocol/common/data_payload_pb2.py,sha256=JRVWR043i9CKok3Lo_twtyKMgLiPLYpysVCqrYR17nU,2580
 drift_protocol/common/drift_package_pb2.py,sha256=Lgf7_HNKqGzA_3dtCALDlAlLJ1h7oCwhVyXtBilQb5M,8282
 drift_protocol/common/status_code_pb2.py,sha256=P2qnFsTCcx7hugviaA2yV5nM2PWKEMyjgVzVRoJawOo,4542
 drift_protocol/meta/__init__.py,sha256=qu7lcUVJvYebLqo4tSmTX66klkF9333pFiqjZaTaPQA,29
-drift_protocol/meta/meta_info_pb2.py,sha256=kIP2wZLwQtx3DZ2fGs6tnig5NIhOnRAcW2g7ba6_3Us,35609
+drift_protocol/meta/meta_info_pb2.py,sha256=Rbst3SykNls7M6v4ApbR05rfXBVYbUPcpUfi1UP5wRA,39953
 drift_protocol/trigger_service/__init__.py,sha256=BqR5M-dhiYxaAeEpZWnNxiq1OM9tTZ951mCt4XcM054,79
 drift_protocol/trigger_service/interval_trigger_message_pb2.py,sha256=93LNGo2Uf3s47bZ5mcBV6HlOcDbjEaxIHo1JhOl_GQk,3454
 drift_protocol/trigger_service/trigger_message_pb2.py,sha256=wbPLot0W6_msZifQGulaElWaqp05eb9hPPbw35CZW2U,2622
-drift_protocol-0.5.0.dist-info/METADATA,sha256=ItDKjlKfjthxwVvpCr_lQ_jVBbllZ3HwXhrPk0yjCmE,1807
-drift_protocol-0.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-drift_protocol-0.5.0.dist-info/top_level.txt,sha256=DbRiBVI9rCZ4d5UjXFR8gRrV-dJuSoWEsiNhNA8wcns,15
-drift_protocol-0.5.0.dist-info/RECORD,,
+drift_protocol-0.6.0.dist-info/METADATA,sha256=LmABpN9YdY0gRPTAhR0il0CJZNWguxa_pZEKn1FuuBI,1807
+drift_protocol-0.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+drift_protocol-0.6.0.dist-info/top_level.txt,sha256=DbRiBVI9rCZ4d5UjXFR8gRrV-dJuSoWEsiNhNA8wcns,15
+drift_protocol-0.6.0.dist-info/RECORD,,
```

