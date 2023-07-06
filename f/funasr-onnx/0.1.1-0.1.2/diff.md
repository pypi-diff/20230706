# Comparing `tmp/funasr_onnx-0.1.1.tar.gz` & `tmp/funasr_onnx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr_onnx-0.1.1.tar", last modified: Mon Jun 19 11:16:15 2023, max compression
+gzip compressed data, was "funasr_onnx-0.1.2.tar", last modified: Thu Jul  6 08:03:22 2023, max compression
```

## Comparing `funasr_onnx-0.1.1.tar` & `funasr_onnx-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:16:15.533452 funasr_onnx-0.1.1/
--rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-06-19 11:16:15.533194 funasr_onnx-0.1.1/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     8039 2023-05-12 03:33:34.000000 funasr_onnx-0.1.1/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:16:15.511729 funasr_onnx-0.1.1/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr_onnx-0.1.1/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr_onnx-0.1.1/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr_onnx-0.1.1/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:16:15.532721 funasr_onnx-0.1.1/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr_onnx-0.1.1/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr_onnx-0.1.1/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr_onnx-0.1.1/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr_onnx-0.1.1/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr_onnx-0.1.1/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr_onnx-0.1.1/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr_onnx-0.1.1/funasr_onnx/vad_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:16:15.513578 funasr_onnx-0.1.1/funasr_onnx.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-06-19 11:16:15.000000 funasr_onnx-0.1.1/funasr_onnx.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)      485 2023-06-19 11:16:15.000000 funasr_onnx-0.1.1/funasr_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-19 11:16:15.000000 funasr_onnx-0.1.1/funasr_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      121 2023-06-19 11:16:15.000000 funasr_onnx-0.1.1/funasr_onnx.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       12 2023-06-19 11:16:15.000000 funasr_onnx-0.1.1/funasr_onnx.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-19 11:16:15.533505 funasr_onnx-0.1.1/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     1588 2023-06-19 11:16:01.000000 funasr_onnx-0.1.1/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.243365 funasr_onnx-0.1.2/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-07-06 08:03:22.243059 funasr_onnx-0.1.2/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     8039 2023-05-12 03:33:34.000000 funasr_onnx-0.1.2/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.238876 funasr_onnx-0.1.2/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr_onnx-0.1.2/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr_onnx-0.1.2/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr_onnx-0.1.2/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.242623 funasr_onnx-0.1.2/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr_onnx-0.1.2/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr_onnx-0.1.2/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr_onnx-0.1.2/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr_onnx-0.1.2/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr_onnx-0.1.2/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr_onnx-0.1.2/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr_onnx-0.1.2/funasr_onnx/vad_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 08:03:22.240099 funasr_onnx-0.1.2/funasr_onnx.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8657 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)      485 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      103 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       12 2023-07-06 08:03:22.000000 funasr_onnx-0.1.2/funasr_onnx.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-06 08:03:22.243437 funasr_onnx-0.1.2/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-06 08:02:59.000000 funasr_onnx-0.1.2/setup.py
```

### Comparing `funasr_onnx-0.1.1/PKG-INFO` & `funasr_onnx-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr_onnx
-Version: 0.1.1
+Version: 0.1.2
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
```

### Comparing `funasr_onnx-0.1.1/README.md` & `funasr_onnx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.1/funasr_onnx/paraformer_bin.py` & `funasr_onnx-0.1.2/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.1/funasr_onnx/punc_bin.py` & `funasr_onnx-0.1.2/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.1/funasr_onnx/utils/e2e_vad.py` & `funasr_onnx-0.1.2/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.1/funasr_onnx/utils/frontend.py` & `funasr_onnx-0.1.2/funasr_onnx/utils/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- encoding: utf-8 -*-
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 import copy
 
 import numpy as np
-from typeguard import check_argument_types
 import kaldi_native_fbank as knf
 
 root_dir = Path(__file__).resolve().parent
 
 logger_initialized = {}
 
 
@@ -25,15 +24,14 @@
             frame_length: int = 25,
             frame_shift: int = 10,
             lfr_m: int = 1,
             lfr_n: int = 1,
             dither: float = 1.0,
             **kwargs,
     ) -> None:
-        check_argument_types()
 
         opts = knf.FbankOptions()
         opts.frame_opts.samp_freq = fs
         opts.frame_opts.dither = dither
         opts.frame_opts.window_type = window
         opts.frame_opts.frame_shift_ms = float(frame_shift)
         opts.frame_opts.frame_length_ms = float(frame_length)
```

### Comparing `funasr_onnx-0.1.1/funasr_onnx/utils/postprocess_utils.py` & `funasr_onnx-0.1.2/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.1/funasr_onnx/utils/timestamp_utils.py` & `funasr_onnx-0.1.2/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.1/funasr_onnx/utils/utils.py` & `funasr_onnx-0.1.2/funasr_onnx/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 
 import numpy as np
 import yaml
 from onnxruntime import (GraphOptimizationLevel, InferenceSession,
                          SessionOptions, get_available_providers, get_device)
-from typeguard import check_argument_types
 
 import warnings
 
 root_dir = Path(__file__).resolve().parent
 
 logger_initialized = {}
 
 
 class TokenIDConverter():
     def __init__(self, token_list: Union[List, str],
                  ):
-        check_argument_types()
 
         self.token_list = token_list
         self.unk_symbol = token_list[-1]
         self.token2id = {v: i for i, v in enumerate(self.token_list)}
         self.unk_id = self.token2id[self.unk_symbol]
 
 
@@ -48,15 +46,14 @@
 class CharTokenizer():
     def __init__(
         self,
         symbol_value: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
         remove_non_linguistic_symbols: bool = False,
     ):
-        check_argument_types()
 
         self.space_symbol = space_symbol
         self.non_linguistic_symbols = self.load_symbols(symbol_value)
         self.remove_non_linguistic_symbols = remove_non_linguistic_symbols
 
     @staticmethod
     def load_symbols(value: Union[Path, str, Iterable[str]] = None) -> Set:
```

### Comparing `funasr_onnx-0.1.1/funasr_onnx/vad_bin.py` & `funasr_onnx-0.1.2/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.1.1/funasr_onnx.egg-info/PKG-INFO` & `funasr_onnx-0.1.2/funasr_onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr-onnx
-Version: 0.1.1
+Version: 0.1.2
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
```

### Comparing `funasr_onnx-0.1.1/setup.py` & `funasr_onnx-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.1.1'
+VERSION_NUM = '0.1.2'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab of DAMO Academy, Alibaba Group",
@@ -27,15 +27,14 @@
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=["librosa",
                       "onnxruntime>=1.7.0",
                       "scipy",
                       "numpy>=1.19.3",
-                      "typeguard==2.13.3",
                       "kaldi-native-fbank",
                       "PyYAML>=5.1.2",
                       "funasr",
                       "modelscope",
                       "onnx"
                       ],
     packages=[MODULE_NAME, f'{MODULE_NAME}.utils'],
```

