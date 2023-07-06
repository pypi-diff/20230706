# Comparing `tmp/tno.quantum.ml.classifiers.vc-1.0.1.tar.gz` & `tmp/tno.quantum.ml.classifiers.vc-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tno.quantum.ml.classifiers.vc-1.0.1.tar", last modified: Tue Feb 14 16:36:55 2023, max compression
+gzip compressed data, was "tno.quantum.ml.classifiers.vc-2.0.2.tar", last modified: Thu Jul  6 12:22:43 2023, max compression
```

## Comparing `tno.quantum.ml.classifiers.vc-1.0.1.tar` & `tno.quantum.ml.classifiers.vc-2.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.302605 tno.quantum.ml.classifiers.vc-1.0.1/
--rw-rw-rw-   0        0        0    11597 2023-02-13 07:38:37.000000 tno.quantum.ml.classifiers.vc-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3176 2023-02-14 16:36:55.303611 tno.quantum.ml.classifiers.vc-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1964 2023-02-14 15:16:44.000000 tno.quantum.ml.classifiers.vc-1.0.1/README.md
--rw-rw-rw-   0        0        0      958 2023-02-13 08:53:48.000000 tno.quantum.ml.classifiers.vc-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1975 2023-02-14 16:36:55.308608 tno.quantum.ml.classifiers.vc-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.203359 tno.quantum.ml.classifiers.vc-1.0.1/tno/
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.204368 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.204368 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.205358 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.283654 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/
--rw-rw-rw-   0        0        0      269 2023-02-13 08:53:48.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/__init__.py
--rw-rw-rw-   0        0        0    13154 2023-02-14 15:16:34.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/models.py
--rw-rw-rw-   0        0        0     1592 2023-02-13 07:38:37.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/optimizers.py
--rw-rw-rw-   0        0        0        0 2022-12-22 14:49:39.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/py.typed
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.300604 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/test/
--rw-rw-rw-   0        0        0       71 2022-07-20 08:52:35.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/test/__init__.py
--rw-rw-rw-   0        0        0    11291 2023-02-14 15:16:34.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/test/test_variational_classifier.py
--rw-rw-rw-   0        0        0    10291 2023-02-14 15:16:34.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/variational_classifier.py
-drwxrwxrwx   0        0        0        0 2023-02-14 16:36:55.260607 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/
--rw-rw-rw-   0        0        0     3176 2023-02-14 16:36:55.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      754 2023-02-14 16:36:55.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 16:36:55.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-02-14 16:36:55.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        2 2023-02-14 16:36:54.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      367 2023-02-14 16:36:55.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-02-14 16:36:55.000000 tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.761699 tno.quantum.ml.classifiers.vc-2.0.2/
+-rw-rw-rw-   0        0        0    11597 2023-02-27 16:28:47.000000 tno.quantum.ml.classifiers.vc-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3176 2023-07-06 12:22:43.762699 tno.quantum.ml.classifiers.vc-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1964 2023-07-06 11:43:55.000000 tno.quantum.ml.classifiers.vc-2.0.2/README.md
+-rw-rw-rw-   0        0        0      958 2023-07-06 11:45:06.000000 tno.quantum.ml.classifiers.vc-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1992 2023-07-06 12:22:43.764698 tno.quantum.ml.classifiers.vc-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.698702 tno.quantum.ml.classifiers.vc-2.0.2/tno/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.698702 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.699698 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.699698 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.757700 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/
+-rw-rw-rw-   0        0        0      269 2023-07-06 11:43:41.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/__init__.py
+-rw-rw-rw-   0        0        0    16358 2023-07-06 11:42:59.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/models.py
+-rw-rw-rw-   0        0        0     1592 2023-07-06 12:01:44.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/optimizers.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 16:28:48.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.760701 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/test/
+-rw-rw-rw-   0        0        0       71 2023-02-27 16:28:48.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/test/__init__.py
+-rw-rw-rw-   0        0        0    13213 2023-07-06 11:48:37.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/test/test_variational_classifier.py
+-rw-rw-rw-   0        0        0    10277 2023-07-06 11:43:32.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/variational_classifier.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:22:43.750701 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/
+-rw-rw-rw-   0        0        0     3176 2023-07-06 12:22:43.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2023-07-06 12:22:43.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:22:43.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-06 12:22:43.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 12:22:43.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      382 2023-07-06 12:22:43.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-06 12:22:43.000000 tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/top_level.txt
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/LICENSE` & `tno.quantum.ml.classifiers.vc-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/PKG-INFO` & `tno.quantum.ml.classifiers.vc-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tno.quantum.ml.classifiers.vc
-Version: 1.0.1
+Version: 2.0.2
 Summary: Quantum VC module
 Home-page: https://tno.nl
 Download-URL: https://pypi.org/project/tno.quantum.ml.classifiers.vc/#files
 Author: TNO Quantum
 Author-email: tnoquantum@tno.nl
 Maintainer: TNO Quantum
 Maintainer-email: tnoquantum@tno.nl
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/README.md` & `tno.quantum.ml.classifiers.vc-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/pyproject.toml` & `tno.quantum.ml.classifiers.vc-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.pylint.similarities]
 ignore-imports="yes"
 ignore-signatures="yes"
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "1.0.1"
+current = "2.0.2"
 regex = '''
 \d+\.\d+\.\d+(-(.*))?
 '''
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/setup.cfg` & `tno.quantum.ml.classifiers.vc-2.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -79,46 +79,47 @@
 000004e0: 6c2e 636c 6173 7369 6669 6572 732e 7663  l.classifiers.vc
 000004f0: 2e74 6573 740d 0a7a 6970 5f73 6166 6520  .test..zip_safe 
 00000500: 3d20 4661 6c73 650d 0a69 6e73 7461 6c6c  = False..install
 00000510: 5f72 6571 7569 7265 7320 3d20 0d0a 0973  _requires = ...s
 00000520: 6369 6b69 742d 6c65 6172 6e7e 3d31 2e30  cikit-learn~=1.0
 00000530: 2e32 0d0a 096e 756d 7079 3e3d 312e 3231  .2...numpy>=1.21
 00000540: 2e36 0d0a 0950 656e 6e79 4c61 6e65 7e3d  .6...PennyLane~=
-00000550: 302e 3234 2e30 0d0a 0970 656e 6e79 6c61  0.24.0...pennyla
-00000560: 6e65 5f71 6973 6b69 747e 3d30 2e32 342e  ne_qiskit~=0.24.
-00000570: 300d 0a09 746f 7263 687e 3d31 2e31 312e  0...torch~=1.11.
-00000580: 300d 0a09 746f 7263 6874 7970 696e 677e  0...torchtyping~
-00000590: 3d30 2e31 2e34 0d0a 0974 7164 6d7e 3d34  =0.1.4...tqdm~=4
-000005a0: 2e36 342e 310d 0a6e 616d 6573 7061 6365  .64.1..namespace
-000005b0: 5f70 6163 6b61 6765 7320 3d20 0d0a 0974  _packages = ...t
-000005c0: 6e6f 0d0a 0974 6e6f 2e71 7561 6e74 756d  no...tno.quantum
-000005d0: 0d0a 0974 6e6f 2e71 7561 6e74 756d 2e6d  ...tno.quantum.m
-000005e0: 6c0d 0a09 746e 6f2e 7175 616e 7475 6d2e  l...tno.quantum.
-000005f0: 6d6c 2e63 6c61 7373 6966 6965 7273 0d0a  ml.classifiers..
-00000600: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000610: 6461 7461 203d 2054 7275 650d 0a0d 0a5b  data = True....[
-00000620: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-00000630: 6461 7461 5d0d 0a74 6e6f 2e71 7561 6e74  data]..tno.quant
-00000640: 756d 2e6d 6c2e 636c 6173 7369 6669 6572  um.ml.classifier
-00000650: 732e 7663 203d 2070 792e 7479 7065 640d  s.vc = py.typed.
-00000660: 0a0d 0a5b 6f70 7469 6f6e 732e 6578 7472  ...[options.extr
-00000670: 6173 5f72 6571 7569 7265 5d0d 0a74 6573  as_require]..tes
-00000680: 7473 203d 200d 0a09 7079 7465 7374 7e3d  ts = ...pytest~=
-00000690: 372e 322e 300d 0a09 7079 7465 7374 2d63  7.2.0...pytest-c
-000006a0: 6f76 7e3d 342e 302e 300d 0a09 7061 6e64  ov~=4.0.0...pand
-000006b0: 6173 3e3d 312e 332e 350d 0a09 746e 6f2e  as>=1.3.5...tno.
-000006c0: 7175 616e 7475 6d2e 6d6c 2e64 6174 6173  quantum.ml.datas
-000006d0: 6574 737e 3d31 2e32 2e31 0d0a 6465 7620  ets~=1.2.1..dev 
+00000550: 302e 3239 2e31 0d0a 0974 6f72 6368 7e3d  0.29.1...torch~=
+00000560: 312e 3131 2e30 0d0a 0974 6f72 6368 7479  1.11.0...torchty
+00000570: 7069 6e67 7e3d 302e 312e 340d 0a09 7471  ping~=0.1.4...tq
+00000580: 646d 7e3d 342e 3634 2e31 0d0a 6e61 6d65  dm~=4.64.1..name
+00000590: 7370 6163 655f 7061 636b 6167 6573 203d  space_packages =
+000005a0: 200d 0a09 746e 6f0d 0a09 746e 6f2e 7175   ...tno...tno.qu
+000005b0: 616e 7475 6d0d 0a09 746e 6f2e 7175 616e  antum...tno.quan
+000005c0: 7475 6d2e 6d6c 0d0a 0974 6e6f 2e71 7561  tum.ml...tno.qua
+000005d0: 6e74 756d 2e6d 6c2e 636c 6173 7369 6669  ntum.ml.classifi
+000005e0: 6572 730d 0a69 6e63 6c75 6465 5f70 6163  ers..include_pac
+000005f0: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
+00000600: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000610: 6b61 6765 5f64 6174 615d 0d0a 746e 6f2e  kage_data]..tno.
+00000620: 7175 616e 7475 6d2e 6d6c 2e63 6c61 7373  quantum.ml.class
+00000630: 6966 6965 7273 2e76 6320 3d20 7079 2e74  ifiers.vc = py.t
+00000640: 7970 6564 0d0a 0d0a 5b6f 7074 696f 6e73  yped....[options
+00000650: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+00000660: 0d0a 7465 7374 7320 3d20 0d0a 0970 7974  ..tests = ...pyt
+00000670: 6573 747e 3d37 2e32 2e30 0d0a 0970 7974  est~=7.2.0...pyt
+00000680: 6573 742d 636f 767e 3d34 2e30 2e30 0d0a  est-cov~=4.0.0..
+00000690: 0970 616e 6461 733e 3d31 2e33 2e35 0d0a  .pandas>=1.3.5..
+000006a0: 0974 6e6f 2e71 7561 6e74 756d 2e6d 6c2e  .tno.quantum.ml.
+000006b0: 6461 7461 7365 7473 7e3d 312e 322e 310d  datasets~=1.2.1.
+000006c0: 0a09 7065 6e6e 796c 616e 655f 7169 736b  ..pennylane_qisk
+000006d0: 6974 7e3d 302e 3239 2e30 0d0a 6465 7620  it~=0.29.0..dev 
 000006e0: 3d20 0d0a 0962 6c61 636b 7e3d 3232 2e31  = ...black~=22.1
 000006f0: 302e 300d 0a09 6973 6f72 747e 3d35 2e31  0.0...isort~=5.1
 00000700: 302e 310d 0a09 6d79 7079 7e3d 302e 3938  0.1...mypy~=0.98
 00000710: 320d 0a09 7079 6c69 6e74 7e3d 322e 3135  2...pylint~=2.15
 00000720: 2e35 0d0a 0973 7068 696e 787e 3d35 2e33  .5...sphinx~=5.3
 00000730: 2e30 0d0a 0973 7068 696e 782d 6175 746f  .0...sphinx-auto
 00000740: 646f 632d 7479 7065 6869 6e74 737e 3d31  doc-typehints~=1
 00000750: 2e31 392e 350d 0a09 7370 6869 6e78 2d6d  .19.5...sphinx-m
 00000760: 6174 682d 646f 6c6c 6172 7e3d 312e 322e  ath-dollar~=1.2.
 00000770: 310d 0a09 7370 6869 6e78 2d72 7464 2d74  1...sphinx-rtd-t
-00000780: 6865 6d65 7e3d 312e 300d 0a0d 0a5b 6567  heme~=1.0....[eg
-00000790: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000007a0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000007b0: 3d20 300d 0a0d 0a                        = 0....
+00000780: 6865 6d65 7e3d 312e 300d 0a09 6a75 7079  heme~=1.0...jupy
+00000790: 7465 727e 3d31 2e30 2e30 0d0a 0d0a 5b65  ter~=1.0.0....[e
+000007a0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000007b0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000007c0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/models.py` & `tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """This module is used to define quantum models.
 
 To add a new model, you should implement the :py:class:`~vc.models.QModel`
 interface and update :py:func:`~vc.models.get_model`.
 """
 import copy
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, Tuple, Union
+from functools import partial
+from typing import Any, Callable, Dict, Tuple, Type, Union
 
 import numpy as np
 import pennylane
 import pennylane.measurements
 import torch
 from numpy.random import RandomState
 from numpy.typing import ArrayLike, NDArray
@@ -121,15 +122,15 @@
         r"""Maps input ``X`` in the range ``min_max`` to $(-\pi, \pi]$.
 
         Args:
             X: input data with shape (`n_samples`, `n_features`).
             min_max: minimum value and maximum value.
         """
         # Coerce into an ndarray
-        X = np.array(X)
+        X = np.asarray(X)
 
         # Convert to angles between -pi and pi
         angles = 2 * np.pi * (X - min_max[0]) / (min_max[1] - min_max[0]) - np.pi
 
         # Set number of qubits required by model and validate
         self.n_qubits = angles.shape[1]
         if self.n_classes > self.n_qubits:
@@ -196,16 +197,16 @@
             weights: TensorType, x: TensorType, qnode: pennylane.QNode = qnode
         ) -> TensorType:
             return qnode(weights, x)
 
         return _process_measurement
 
 
-class ProbabilitiesModel(QModel):
-    """Model that uses angle encoding and state probabilities."""
+class ProbabilitiesModel(QModel, ABC):
+    """Generic model that uses probabilities."""
 
     def __init__(
         self,
         backend: Dict[str, Any],
         n_classes: int,
         n_layers: int = 2,
         n_trainable_sublayers: int = 2,
@@ -227,15 +228,15 @@
 
         Args:
             backend: see docstring of :py:class:`~vc.models.QModel`.
             n_classes: see docstring of :py:class:`~vc.models.QModel`.
             n_layers: number of layers in $U(x)$ (equal to $L$).
             n_trainable_sublayers: number of layers for each $W$.
             scaling: scaling to apply to the preprocessed data, see
-                     :py:meth:`~vc.models.ExpectedValuesModel.preprocess`.
+                     :py:meth:`~vc.models.ProbabilitiesModel.preprocess`.
         """
         super().__init__(backend, n_classes)
         self.n_layers = n_layers
         self.n_trainable_sublayers = n_trainable_sublayers
         self.scaling = scaling
 
     def preprocess(
@@ -244,15 +245,15 @@
         r"""Maps input ``X`` in the range ``min_max`` to $(-\pi, \pi]$.
 
         Args:
             X: input data with shape (`n_samples`, `n_features`).
             min_max: minimum value and maximum value.
         """
         # Coerce into an ndarray
-        X = np.array(X)
+        X = np.asarray(X)
 
         # Convert to angles between -pi and pi
         angles = 2 * np.pi * (X - min_max[0]) / (min_max[1] - min_max[0]) - np.pi
 
         # Set number of qubits required by model and validate
         self.n_qubits = angles.shape[1]
         if self.n_classes > 2**self.n_qubits:
@@ -309,41 +310,137 @@
         if self.n_classes > 2:
             return pennylane.probs(wires=range(self.n_qubits))
 
         # Else measure the expected value for the first qubit
         return pennylane.expval(pennylane.PauliZ(0))
 
     def get_qfunc(self) -> Callable[[TensorType, TensorType], TensorType]:
-        """Define callable based on circuit.
-
-        This callable will aggregate (by averaging) the probabilities per output
-        state into an array with as many elements as classes we have. Note: in order
-        to make the sample size (for each aggregation) equal, some output states will
-        be ignored. As a result, the sum of the array elements may not sum to one.
-        """
+        """Get callable based on circuit."""
         dev = _get_device(self.backend, self.n_qubits)
         qnode = pennylane.QNode(self._circuit, dev, interface="torch")
+        return partial(self._process_measurement, qnode=qnode, n_classes=self.n_classes)
 
-        def _process_measurement(
-            weights: TensorType,
-            x: TensorType,
-            qnode: pennylane.QNode = qnode,
-            n_classes: int = self.n_classes,
-        ) -> TensorType:
-            probs: TensorType = qnode(weights, x)
-            if n_classes > 2:
-                aggregated_probs = []
-                for class_id in range(n_classes):
-                    aggregated_probs.append(
-                        probs[class_id::n_classes][: probs.numel() // n_classes].sum()
-                    )
-                return torch.stack(aggregated_probs).squeeze()
-            return probs
+    @staticmethod
+    @abstractmethod
+    def _process_measurement(
+        weights: TensorType,
+        x: TensorType,
+        qnode: pennylane.QNode,
+        n_classes: int,
+    ) -> TensorType:
+        """Define post-processing strategy."""
 
-        return _process_measurement
+
+class ModuloModel(ProbabilitiesModel):
+    r"""Model that uses post-processing with modulo.
+
+    See docstring of :py:class:`.vc.models.ProbabilitiesModel`.
+
+    The post-processing strategy assigns a class to an $n$-bit string
+    $b$ according to the following formula:
+
+    .. math::
+        f(b) = \left[b\right]_{10} \mod M
+
+    where:
+
+        - $M$ is the number of classes,
+        - $[\cdot]_{10}$ is the decimal representation of the argument.
+    """
+
+    @staticmethod
+    def _process_measurement(
+        weights: TensorType,
+        x: TensorType,
+        qnode: pennylane.QNode,
+        n_classes: int,
+    ) -> TensorType:
+        """Define post-processing strategy."""
+        measurement: TensorType = qnode(weights, x)
+        if n_classes > 2:
+            aggregated_measurement = []
+            for class_id in range(n_classes):
+                aggregated_measurement.append(
+                    measurement[class_id::n_classes][
+                        : measurement.numel() // n_classes
+                    ].sum()
+                )
+            return torch.stack(aggregated_measurement).squeeze()
+        return measurement
+
+
+class ParityModel(ProbabilitiesModel):
+    r"""Model that uses parity post-processing.
+
+    See docstring of :py:class:`.vc.models.ProbabilitiesModel`.
+
+    The post-processing strategy assigns a class to an $n$-bit string $b$
+    according to the following formula:
+
+    .. math::
+        f(b) = \left[b_0 ... b_{m-2}\left(\bigoplus_{i=m-1}^{n-1} b_i\right) \right]_{10}
+
+    where:
+
+        - $m=\lceil \log_2(M) \rceil$ with $M$ being the number of classes,
+        - $n$ is the number of bits,
+        - $[\cdot]_{10}$ is the decimal representation of the argument.
+
+    Reference: `"Quantum Policy Gradient Algorithm with Optimized Action Decoding"
+    by Meyer et al. <https://arxiv.org/abs/2212.06663v1>`_
+    """
+
+    @staticmethod
+    def _f(idx: int, n_bits_in: int, n_bits_out: int) -> int:
+        """Post-processing function.
+
+        Assigns a class index (an integer) to an arbitrary integer
+        (corresponding to a measured bit string).
+
+        Args:
+            idx: state index.
+            n_bits_in: number of bits used for the input index.
+            n_bits_out: number of bits to be used for the output class index.
+
+        Returns:
+            Class index assigned.
+        """
+        idx_bit_array = np.array(
+            list(map(int, [*np.binary_repr(idx, width=n_bits_in)]))
+        )
+        class_bit_array = idx_bit_array[-n_bits_out:]
+        if n_bits_out < n_bits_in:
+            class_bit_array[0] = idx_bit_array[: -(n_bits_out - 1)].sum() % 2
+
+        return int("".join([str(elem) for elem in np.flip(class_bit_array)]), 2)
+
+    @staticmethod
+    def _process_measurement(
+        weights: TensorType,
+        x: TensorType,
+        qnode: pennylane.QNode,
+        n_classes: int,
+    ) -> TensorType:
+        """Define post-processing strategy."""
+        measurement: TensorType = qnode(weights, x)
+        if n_classes > 2:
+            n_bits_in = int(np.log2(measurement.numel()))
+            n_bits_out = int(np.ceil(np.log2(n_classes)))
+            aggregated_measurement = [
+                torch.zeros(1, requires_grad=False) for _ in range(n_classes)
+            ]
+            for idx, prob in enumerate(measurement):
+                class_id = ParityModel._f(idx, n_bits_in, n_bits_out)
+                if class_id >= n_classes:
+                    continue
+                aggregated_measurement[class_id] = (
+                    aggregated_measurement[class_id] + prob
+                )
+            return torch.stack(aggregated_measurement).squeeze()
+        return measurement
 
 
 def get_model(
     model: Dict[str, Any],
     backend: Dict[str, Any],
     n_classes: int,
 ) -> QModel:
@@ -363,17 +460,19 @@
         An instance of a quantum model.
     """
     # Make sure there's no conflicting backend key
     model = copy.deepcopy(model)
     model.pop("backend", None)
 
     # Instantiate model
+    models: Dict[str, Type[QModel]]
     models = {
         "expected_values_model": ExpectedValuesModel,
-        "probabilities_model": ProbabilitiesModel,
+        "modulo_model": ModuloModel,
+        "parity_model": ParityModel,
     }
     if model["name"] not in models:
         raise ValueError("Invalid model name.")
 
     model_class = models[model["name"]]
     model_instance = model_class(
         backend,
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/optimizers.py` & `tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/optimizers.py`

 * *Files identical despite different names*

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/test/test_variational_classifier.py` & `tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/test/test_variational_classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import numpy as np
 import pytest
 from numpy.typing import NDArray
 from sklearn.preprocessing import StandardScaler
 from sklearn.utils.estimator_checks import check_estimator
 
 from tno.quantum.ml.classifiers.vc import VariationalClassifier
-from tno.quantum.ml.classifiers.vc.models import ModelError
+from tno.quantum.ml.classifiers.vc.models import ModelError, ParityModel
 from tno.quantum.ml.datasets import get_iris_dataset, get_wine_dataset
 
 # pylint: disable=invalid-name
 # pylint: disable=missing-function-docstring
 # pylint: disable=too-many-arguments
+# pylint: disable=protected-access
 
 
 def test_sklearn_compliance() -> None:
     classifier = VariationalClassifier(random_state=0)
     for estimator, check in check_estimator(classifier, generate_only=True):
         print(check)
         check(estimator)
@@ -50,15 +51,22 @@
             "expected_values_model",
             False,
             [160],
         ),
         (
             {"name": "default.qubit", "options": {}},
             {"name": "default.qubit", "options": {}},
-            "probabilities_model",
+            "modulo_model",
+            False,
+            [160],
+        ),
+        (
+            {"name": "default.qubit", "options": {}},
+            {"name": "default.qubit", "options": {}},
+            "parity_model",
             False,
             [160],
         ),
         (
             {"name": "default.qubit", "options": {}},
             {"name": "qiskit.aer", "options": {}},
             "expected_values_model",
@@ -127,15 +135,21 @@
             {"name": "default.qubit", "options": {}},
             "expected_values_model",
             [80],
             0.9,
         ),
         (
             {"name": "default.qubit", "options": {}},
-            "probabilities_model",
+            "modulo_model",
+            [80],
+            0.8,
+        ),
+        (
+            {"name": "default.qubit", "options": {}},
+            "parity_model",
             [80],
             0.8,
         ),
     ],
 )
 def test_variational_classifier_multiple_classes(
     backend: Dict[str, Any],
@@ -250,15 +264,17 @@
 
     # Fit
     expected_message = "one class found"
     with pytest.warns(UserWarning, match=expected_message):
         vc = vc.fit(X_training, y_training, n_iter=1)
 
 
-@pytest.mark.parametrize("model_name", ["probabilities_model", "expected_values_model"])
+@pytest.mark.parametrize(
+    "model_name", ["modulo_model", "expected_values_model", "parity_model"]
+)
 def test_maximum_number_of_classes(model_name: str) -> None:
     # Load training data
     X_training, y_training, _, _ = get_iris_dataset(
         n_features=1, n_classes=3, random_seed=0
     )
 
     # Define classifier
@@ -302,15 +318,17 @@
 
     # Fit
     expected_message = "fit method has not been called"
     with pytest.warns(UserWarning, match=expected_message):
         vc = vc.fit(X_training, y_training, n_iter=1)
 
 
-@pytest.mark.parametrize("model_name", ["probabilities_model", "expected_values_model"])
+@pytest.mark.parametrize(
+    "model_name", ["modulo_model", "expected_values_model", "parity_model"]
+)
 def test_non_random_init(model_name: str) -> None:
     # Load training data
     X_training, y_training, _, _ = get_iris_dataset(
         n_features=2, n_classes=2, random_seed=0
     )
 
     # Define classifier
@@ -324,14 +342,78 @@
 
     # Fit
     vc = vc.fit(X_training, y_training, n_iter=1)
 
     assert True
 
 
+def test_maximal_class_assignment_parity_model() -> None:
+    # Check that all class assignments correspond to a flip of the bitstring.
+    n_bits = 5
+    for idx in range(int(2**n_bits)):
+        assert (
+            int(
+                np.binary_repr(ParityModel._f(idx, n_bits, n_bits), width=n_bits)[::-1],
+                2,
+            )
+            == idx
+        )
+
+
+@pytest.mark.parametrize(
+    "n_bits_in,n_bits_out,assignments",
+    [
+        (4, 2, [0, 2, 1, 3, 1, 3, 0, 2, 1, 3, 0, 2, 0, 2, 1, 3]),
+        (
+            5,
+            3,
+            [
+                0,
+                4,
+                2,
+                6,
+                1,
+                5,
+                3,
+                7,
+                1,
+                5,
+                3,
+                7,
+                0,
+                4,
+                2,
+                6,
+                1,
+                5,
+                3,
+                7,
+                0,
+                4,
+                2,
+                6,
+                0,
+                4,
+                2,
+                6,
+                1,
+                5,
+                3,
+                7,
+            ],
+        ),
+    ],
+)
+def test_class_assignment_parity_model(
+    n_bits_in: int, n_bits_out: int, assignments: List[int]
+) -> None:
+    for idx, class_id in enumerate(assignments):
+        assert ParityModel._f(idx, n_bits_in, n_bits_out) == class_id
+
+
 def test_invalid_optimizer() -> None:
     # Load training data
     X_training, y_training, _, _ = get_iris_dataset(
         n_features=2, n_classes=2, random_seed=0
     )
 
     # Define classifier with invalid optimizer
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/tno/quantum/ml/classifiers/vc/variational_classifier.py` & `tno.quantum.ml.classifiers.vc-2.0.2/tno/quantum/ml/classifiers/vc/variational_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 ) -> Tuple[Dict[str, Any], Dict[str, Any], Dict[str, Any]]:
     """Set default value if the one provided is ``None``.
 
     Args:
         backend: see docstring of :py:func:`~vc.models.get_model`.
           default value ``{"name": "default.qubit", "options": {}}``.
         model: see docstring of :py:func:`~vc.models.get_model`
-          default value ``{"name": "probabilities_model",
+          default value ``{"name": "modulo_model",
           "options": {"n_layers": 2, "n_trainable_sublayers": 2, "scaling": 0.5}}``.
         optimizer: see docstring of :py:func:`~vc.optimizers.get_optimizer`
           default value ``{"name": "adam", "options": {}}``.
 
     Returns:
         Default backend, model, optimizer.
     """
     if backend is None:
         backend = {"name": "default.qubit", "options": {}}
     if model is None:
         model = {
-            "name": "probabilities_model",
+            "name": "modulo_model",
             "options": {"n_layers": 2, "n_trainable_sublayers": 2, "scaling": 0.5},
         }
     if optimizer is None:
         optimizer = {"name": "adam", "options": {}}
     return backend, model, optimizer
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/PKG-INFO` & `tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tno.quantum.ml.classifiers.vc
-Version: 1.0.1
+Version: 2.0.2
 Summary: Quantum VC module
 Home-page: https://tno.nl
 Download-URL: https://pypi.org/project/tno.quantum.ml.classifiers.vc/#files
 Author: TNO Quantum
 Author-email: tnoquantum@tno.nl
 Maintainer: TNO Quantum
 Maintainer-email: tnoquantum@tno.nl
```

### Comparing `tno.quantum.ml.classifiers.vc-1.0.1/tno.quantum.ml.classifiers.vc.egg-info/SOURCES.txt` & `tno.quantum.ml.classifiers.vc-2.0.2/tno.quantum.ml.classifiers.vc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

