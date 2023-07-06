# Comparing `tmp/mcap-protobuf-support-0.3.0.tar.gz` & `tmp/mcap-protobuf-support-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-protobuf-support-0.3.0.tar", last modified: Fri Jun 16 00:58:48 2023, max compression
+gzip compressed data, was "mcap-protobuf-support-0.4.0.tar", last modified: Thu Jul  6 21:44:17 2023, max compression
```

## Comparing `mcap-protobuf-support-0.3.0.tar` & `mcap-protobuf-support-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/mcap_protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/mcap_protobuf/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 00:58:48.000000 mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:58:48.337872 mcap-protobuf-support-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-16 00:55:05.000000 mcap-protobuf-support-0.3.0/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:17.019137 mcap-protobuf-support-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 21:44:17.019137 mcap-protobuf-support-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:17.015137 mcap-protobuf-support-0.4.0/mcap_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/mcap_protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/mcap_protobuf/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/mcap_protobuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/mcap_protobuf/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/mcap_protobuf/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/mcap_protobuf/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:17.019137 mcap-protobuf-support-0.4.0/mcap_protobuf_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 21:44:17.000000 mcap-protobuf-support-0.4.0/mcap_protobuf_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 21:44:17.000000 mcap-protobuf-support-0.4.0/mcap_protobuf_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:44:17.000000 mcap-protobuf-support-0.4.0/mcap_protobuf_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 21:44:17.000000 mcap-protobuf-support-0.4.0/mcap_protobuf_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:44:17.000000 mcap-protobuf-support-0.4.0/mcap_protobuf_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-06 21:44:17.019137 mcap-protobuf-support-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:44:17.019137 mcap-protobuf-support-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-06 21:41:07.000000 mcap-protobuf-support-0.4.0/tests/test_writer.py
```

### Comparing `mcap-protobuf-support-0.3.0/PKG-INFO` & `mcap-protobuf-support-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.3.0
+Version: 0.4.0
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mcap-protobuf-support-0.3.0/README.md` & `mcap-protobuf-support-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.3.0/mcap_protobuf/decoder.py` & `mcap-protobuf-support-0.4.0/mcap_protobuf/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from collections import Counter
-from typing import Dict, Any, Type, Iterable, Optional, Callable
 import warnings
+from collections import Counter
+from typing import Any, Callable, Dict, Iterable, Optional, Type
 
-from google.protobuf.descriptor_pb2 import FileDescriptorSet, FileDescriptorProto
+from google.protobuf.descriptor_pb2 import FileDescriptorProto, FileDescriptorSet
 from google.protobuf.message_factory import MessageFactory
-from mcap.exceptions import McapError
-from mcap.records import Schema, Message
-from mcap.well_known import SchemaEncoding, MessageEncoding
+
 from mcap.decoder import DecoderFactory as McapDecoderFactory
+from mcap.exceptions import McapError
+from mcap.records import Message, Schema
+from mcap.well_known import MessageEncoding, SchemaEncoding
 
 
 class McapProtobufDecodeError(McapError):
     """Raised when a Message record cannot be decoded as a Protobuf message."""
 
     pass
```

### Comparing `mcap-protobuf-support-0.3.0/mcap_protobuf/reader.py` & `mcap-protobuf-support-0.4.0/mcap_protobuf/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 >>> from mcap_protobuf.decoder import DecoderFactory
 >>> reader = make_reader(open("proto.mcap", "rb"), decoder_factories=[DecoderFactory()])
 >>> for schema_, channel_, message_, proto_msg in reader.iter_decoded_messages():
 >>>     print(proto_msg)
 MyProtoClass(data="hello")
 MyProtoClass(data="goodbye")
 """
-from typing import IO, Union, Any, Dict, Iterator, Optional, Iterable
+import warnings
 from datetime import datetime
 from os import PathLike
-import warnings
-
-from .decoder import DecoderFactory
+from typing import IO, Any, Dict, Iterable, Iterator, Optional, Union
 
-from mcap.records import Message, Channel
 from mcap.reader import McapReader, make_reader
+from mcap.records import Channel, Message
+
+from .decoder import DecoderFactory
 
 warnings.warn(__doc__, DeprecationWarning)
 
 
 def read_protobuf_messages(
     source: Union[str, bytes, PathLike[str], McapReader, IO[bytes]],
     topics: Optional[Iterable[str]] = None,
```

### Comparing `mcap-protobuf-support-0.3.0/mcap_protobuf/schema.py` & `mcap-protobuf-support-0.4.0/mcap_protobuf/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Set
+
 from google.protobuf.descriptor import FileDescriptor
 from google.protobuf.descriptor_pb2 import FileDescriptorSet
+
 from mcap.writer import Writer as McapWriter
 
 
 def register_schema(writer: McapWriter, message_class: Any):
     file_descriptor_set = build_file_descriptor_set(message_class=message_class)
 
     return writer.register_schema(
```

### Comparing `mcap-protobuf-support-0.3.0/mcap_protobuf/writer.py` & `mcap-protobuf-support-0.4.0/mcap_protobuf/writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import time
 from io import BufferedWriter
-from typing import Optional, Dict, Any, Tuple, Union, IO
+from typing import IO, Any, Dict, Optional, Tuple, Union
 
-from mcap.writer import CompressionType, Writer as McapWriter
-from mcap.well_known import MessageEncoding
 import mcap
+from mcap.well_known import MessageEncoding
+from mcap.writer import CompressionType
+from mcap.writer import Writer as McapWriter
 
-from .schema import register_schema
 from . import __version__
+from .schema import register_schema
 
 
 def _library_identifier():
     """the default value written into MCAP headers by this library."""
     mcap_version = getattr(mcap, "__version__", "<=0.0.10")
     return f"python mcap-protobuf-support {__version__}; mcap {mcap_version}"
```

### Comparing `mcap-protobuf-support-0.3.0/mcap_protobuf_support.egg-info/PKG-INFO` & `mcap-protobuf-support-0.4.0/mcap_protobuf_support.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.3.0
+Version: 0.4.0
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mcap-protobuf-support-0.3.0/setup.cfg` & `mcap-protobuf-support-0.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 install_requires = 
 	mcap>=0.0.14
-	protobuf
+	protobuf>=3.8,<=4.21.11
 install_package_data = True
 packages = find:
 python_requires = >=3.7
 
 [options.package_data]
 mcap_protobuf = py.typed
```

### Comparing `mcap-protobuf-support-0.3.0/tests/generate.py` & `mcap-protobuf-support-0.4.0/tests/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import sys
 
 sys.path.append(os.path.dirname(__file__))  # for test_proto imports
 
 from typing import IO, Any  # noqa: #402
 
 from mcap_protobuf.writer import Writer  # noqa: #402
-
 from test_proto.complex_message_pb2 import ComplexMessage  # noqa: #402
 from test_proto.intermediate_message_1_pb2 import IntermediateMessage1  # noqa: #402
 from test_proto.intermediate_message_2_pb2 import IntermediateMessage2  # noqa: #402
 from test_proto.simple_message_pb2 import SimpleMessage  # noqa: #402
 
 
 def generate_sample_data(output: IO[Any]):
```

### Comparing `mcap-protobuf-support-0.3.0/tests/test_decoder.py` & `mcap-protobuf-support-0.4.0/tests/test_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from io import BytesIO
 
-from mcap.reader import make_reader
 from mcap_protobuf.decoder import DecoderFactory
 
+from mcap.reader import make_reader
+
 from .generate import generate_sample_data
 
 
 def test_protobuf_decoder():
     output = BytesIO()
     generate_sample_data(output)
```

### Comparing `mcap-protobuf-support-0.3.0/tests/test_writer.py` & `mcap-protobuf-support-0.4.0/tests/test_writer.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from io import BytesIO
 
-from mcap.reader import make_reader
-from mcap_protobuf.writer import Writer
-from mcap_protobuf.decoder import DecoderFactory
-
 import pytest
-from google.protobuf.timestamp_pb2 import Timestamp
 from google.protobuf.duration_pb2 import Duration
+from google.protobuf.timestamp_pb2 import Timestamp
+from mcap_protobuf.decoder import DecoderFactory
+from mcap_protobuf.writer import Writer
+
+from mcap.reader import make_reader
 
 
 def read_protobuf_messages(stream: BytesIO):
     return make_reader(
         stream, decoder_factories=[DecoderFactory()]
     ).iter_decoded_messages()
```

